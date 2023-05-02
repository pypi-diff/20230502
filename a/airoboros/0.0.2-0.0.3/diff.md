# Comparing `tmp/airoboros-0.0.2-py3-none-any.whl.zip` & `tmp/airoboros-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 13549 bytes, number of entries: 10
+Zip file size: 14012 bytes, number of entries: 10
 -rw-r--r--  2.0 unx        0 b- defN 23-May-01 08:36 airoboros/__init__.py
 -rw-r--r--  2.0 unx      466 b- defN 23-May-01 09:54 airoboros/entrypoint.py
 -rw-r--r--  2.0 unx      338 b- defN 23-May-01 19:03 airoboros/exceptions.py
--rw-r--r--  2.0 unx    25713 b- defN 23-May-01 19:24 airoboros/self_instruct.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-01 19:25 airoboros-0.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx      763 b- defN 23-May-01 19:25 airoboros-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-01 19:25 airoboros-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       55 b- defN 23-May-01 19:25 airoboros-0.0.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-May-01 19:25 airoboros-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      810 b- defN 23-May-01 19:25 airoboros-0.0.2.dist-info/RECORD
-10 files, 39604 bytes uncompressed, 12159 bytes compressed:  69.3%
+-rw-r--r--  2.0 unx    27679 b- defN 23-May-02 08:28 airoboros/self_instruct.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-02 08:56 airoboros-0.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      763 b- defN 23-May-02 08:56 airoboros-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-02 08:56 airoboros-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       55 b- defN 23-May-02 08:56 airoboros-0.0.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-May-02 08:56 airoboros-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      810 b- defN 23-May-02 08:56 airoboros-0.0.3.dist-info/RECORD
+10 files, 41570 bytes uncompressed, 12622 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: airoboros/exceptions.py
 Comment: 
 
 Filename: airoboros/self_instruct.py
 Comment: 
 
-Filename: airoboros-0.0.2.dist-info/LICENSE
+Filename: airoboros-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: airoboros-0.0.2.dist-info/METADATA
+Filename: airoboros-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: airoboros-0.0.2.dist-info/WHEEL
+Filename: airoboros-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: airoboros-0.0.2.dist-info/entry_points.txt
+Filename: airoboros-0.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: airoboros-0.0.2.dist-info/top_level.txt
+Filename: airoboros-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: airoboros-0.0.2.dist-info/RECORD
+Filename: airoboros-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## airoboros/self_instruct.py

```diff
@@ -1,23 +1,26 @@
-import asyncio
-import aiohttp
 import argparse
 import backoff
 import os
 import json
 import random
 import re
 import requests
 import secrets
+import signal
 import string
 import sys
+import threading
+import concurrent.futures
 from multiprocessing import Pool
 from functools import partial
 from loguru import logger
+from queue import Queue
 from typing import List, Dict, Any
+from uuid import uuid4
 from rouge_score import rouge_scorer
 from .exceptions import (
     RateLimitError,
     TooManyRequestsError,
     TokensExhaustedError,
     ServerOverloadedError,
     ServerError,
@@ -64,14 +67,15 @@
         "gpt-4-0314",
         "gpt-4-32k",
         "gpt-4-32k-0314",
         "gpt-3.5-turbo",
         "gpt-3.5-turbo-0301",
     ],
 }
+SCORER = rouge_scorer.RougeScorer(["rougeL"], use_stemmer=False)
 
 
 class SelfInstructor:
     """Class and methods used to generate instructions, based on self-instruct paper/code."""
 
     CLI_ARGS = {
         "--model": {
@@ -226,14 +230,15 @@
         self.samples_per_request = samples_per_request
         self.max_usage_tokens = max_usage_tokens
         self._validate_model()
         self.machine_tasks = []
         self._initialize_seed_tasks(seed_tasks, seed_tasks_path, use_dolly_seed)
         self.used_tokens = 0
         self.random_topics = set([])
+        self.stop_producing = False
 
     def _initialize_seed_tasks(
         self,
         seed_tasks: List[Dict[str, str]],
         seed_tasks_path: str,
         use_dolly_seed: bool,
     ):
@@ -312,54 +317,55 @@
         :return: The cleaned prompt text.
         :rtype: str
         """
         return re.sub(
             r"\s+", " ", " ".join(instruction.splitlines()).strip().rstrip(":")
         )
 
-    async def initialize_random_topics(self):
+    def initialize_random_topics(self):
         path = os.path.join(
             os.path.dirname(os.path.abspath(__file__)), ".seed", "topics.txt"
         )
         if os.path.exists(path):
             with open(path, "r") as infile:
                 self.random_topics = {
                     line.strip().lower() for line in infile.readlines() if line.strip()
                 }
                 logger.info(f"Using {len(self.random_topics)} cached random topics...")
             return
         logger.info("Generating random topics to use in prompts...")
-        futures = [
-            self._post_no_exc(
-                "/v1/completions",
-                {
-                    "model": "text-davinci-003",
-                    "prompt": ["Give me a list of 200 completely random topics."] * 20,
-                    "temperature": 1.0,
-                    "max_tokens": 800,
-                },
+        with concurrent.futures.ThreadPoolExecutor(20) as pool:
+            responses = pool.map(
+                partial(self._post_no_exc, "/v1/completions"),
+                [
+                    {
+                        "model": "text-davinci-003",
+                        "prompt": ["Give me a list of 200 completely random topics."]
+                        * 20,
+                        "temperature": 1.0,
+                        "max_tokens": 800,
+                    }
+                ]
+                * 20,
             )
-            for _ in range(20)
-        ]
-        responses = await asyncio.gather(*futures)
         with open(path, "w") as outfile:
             for response in responses:
                 if not response:
                     continue
                 for choice in response["choices"]:
                     for line in choice["text"].splitlines():
                         if match := re.search(r"\s*\d+\s*\.\s*(.+)", line):
                             topic = match.group(1).lower()
                             self.random_topics.add(topic)
                             outfile.write(topic + "\n")
         logger.success(
             f"Successfully generated {len(self.random_topics)} random topics..."
         )
 
-    async def generate_prompt_from_instructions(
+    def generate_prompt_from_instructions(
         self, instructions: List[Dict[str, any]]
     ) -> str:
         """Generate a single prompt string with multiple instructions.
 
         :param instructions: A list of instructions to encode.
         :type instructions: List[str]
 
@@ -481,85 +487,87 @@
                 f"Generated new task [has context: {context != ''}]: {instruction_text}"
             )
         return tasks
 
     @backoff.on_exception(
         backoff.expo,
         (
-            asyncio.TimeoutError,
+            requests.exceptions.ConnectionError,
+            requests.exceptions.Timeout,
             ServerError,
             RateLimitError,
             TooManyRequestsError,
             ServerOverloadedError,
         ),
     )
-    async def _post(self, path: str, payload: Dict[str, Any]) -> Dict[str, Any]:
+    def _post(self, path: str, payload: Dict[str, Any]) -> Dict[str, Any]:
         """Perform a post request to OpenAI API.
 
         :param path: URL path to send request to.
         :type path: str
 
         :param payload: Dict containing request body/payload.
         :type payload: Dict[str, Any]
 
         :return: Response object.
         :rtype: Dict[str, Any]
         """
         headers = {"Authorization": f"Bearer {self.openai_api_key}"}
         if self.organization_id:
             headers["OpenAI-Organization"] = self.organization_id
-        async with aiohttp.ClientSession() as session:
-            result = await session.post(
-                f"{OPENAI_API_BASE_URL}{path}",
-                headers=headers,
-                json=payload,
-                timeout=120.0,
-            )
-            if result.status != 200:
-                text = await result.text()
-                if "too many requests" in text.lower():
-                    raise TooManyRequestsError(text)
-                if "rate limit reached" in text.lower():
-                    raise RateLimitError(text)
-                elif "context_length_exceeded" in text.lower():
-                    raise ContextLengthExceededError(text)
-                elif "server_error" in text and "overloaded" in text.lower():
-                    raise ServerOverloadedError(text)
-                elif "bad gateway" in text.lower() or "server_error" in text.lower():
-                    raise ServerError(text)
-                else:
-                    raise BadResponseError(text)
-            result = await result.json()
-        logger.debug(f"POST {path} with {json.dumps(payload)}: {json.dumps(result)}")
+        request_id = str(uuid4())
+        logger.debug(f"POST [{request_id}] with payload {json.dumps(payload)}")
+        result = requests.post(
+            f"{OPENAI_API_BASE_URL}{path}",
+            headers=headers,
+            json=payload,
+            timeout=240.0,
+        )
+        if result.status_code != 200:
+            text = result.text
+            if "too many requests" in text.lower():
+                raise TooManyRequestsError(text)
+            if "rate limit reached" in text.lower():
+                raise RateLimitError(text)
+            elif "context_length_exceeded" in text.lower():
+                raise ContextLengthExceededError(text)
+            elif "server_error" in text and "overloaded" in text.lower():
+                raise ServerOverloadedError(text)
+            elif "bad gateway" in text.lower() or "server_error" in text.lower():
+                raise ServerError(text)
+            else:
+                raise BadResponseError(text)
+        result = result.json()
+        logger.debug(f"POST [{request_id}] response: {json.dumps(result)}")
         self.used_tokens += result["usage"]["total_tokens"]
         if self.max_usage_tokens and self.used_tokens > self.max_usage_tokens:
             raise TokensExhaustedError(f"Max token usage exceeded: {self.used_tokens}")
         logger.debug(f"token usage: {self.used_tokens}")
         return result
 
-    async def _post_no_exc(self, *a, **k):
+    def _post_no_exc(self, *a, **k) -> Dict[str, Any] | None:
         """Post, ignoring all exceptions."""
         try:
-            return await self._post(*a, **k)
+            return self._post(*a, **k)
         except Exception as ex:
             logger.error(f"Error performing post: {ex}")
         return None
 
-    async def generate_instruction_batch(self):
+    def generate_instruction_batch(self, queue: Queue) -> None:
         """Generate an set of instructions.
 
-        :return: List of machine-generated instructions, contexts, and responses.
-        :rtype: List[Dict[str, Any]]
+        :param queue: Queue to pass generated outputs to.
+        :type queue: Queue
         """
         instructions = random.sample(self.seed_tasks, self.samples_per_request)
-        prompt = await self.generate_prompt_from_instructions(instructions)
+        prompt = self.generate_prompt_from_instructions(instructions)
         estimated_tokens = int(len(prompt) / 4)
         if estimated_tokens > 2700:
             logger.warning("Skipping prompt, too long")
-            return []
+            return
         path = "/v1/completions" if self._completions else "/v1/chat/completions"
         payload = {
             "model": self.model,
             "temperature": self.temperature,
             "top_p": self.top_p,
             "frequency_penalty": self.frequency_penalty,
             "presence_penalty": self.presence_penalty,
@@ -567,66 +575,116 @@
             "max_tokens": 4000 - estimated_tokens if self._completions else None,
         }
         if self._completions:
             payload["prompt"] = prompt
         else:
             payload["messages"] = [{"role": "user", "content": prompt}]
         try:
-            return self.extract_instructions_from_response(
-                await self._post(path, payload)
-            )
+            for new_instruction in self.extract_instructions_from_response(
+                self._post(path, payload)
+            ):
+                queue.put(new_instruction)
         except ContextLengthExceededError:
             ...
-        return []
 
-    async def run(self):
-        """Run the self-instruct, instruction generation task to completion."""
-        scorer = rouge_scorer.RougeScorer(["rougeL"], use_stemmer=False)
-        await self.initialize_random_topics()
+    def generate_instruction_batches(self, queue: Queue) -> None:
+        """Generate batches of instructions, storing new instructions in queue.
+
+        :param queue: Queue to store new instructions in for post-processing.
+        :type queue: Queue
+        """
+        consecutive_errors = 0
+        while not self.stop_producing:
+            try:
+                self.generate_instruction_batch(queue)
+                consecutive_errors = 0
+            except TokensExhaustedError:
+                logger.error("Max tokens reached, stopping...")
+                break
+            except Exception as exc:
+                logger.error(f"Unhandled exception generating batch: {exc}")
+                consecutive_errors += 1
+                if consecutive_errors > 3:
+                    logger.error("Too many consecutive errors, shutting down!")
+                    os.kill(os.getpid(), signal.SIGKILL)
+
+    def validate_and_store_results(
+        self, queue: Queue, consume_remaining: bool = False
+    ) -> None:
+        """Dedupe based on rouge score for each new instruction and save results.
+
+        :param queue: Queue to consume messages from.
+        :type queue: Queue
+        """
         with open(self.output_path, "a+") as outfile:
-            while len(self.machine_tasks) <= self.instruction_count:
-                futures = [self.generate_instruction_batch() for _ in range(10)]
-                results = None
-                try:
-                    results = await asyncio.gather(*futures)
-                except TokensExhaustedError:
-                    logger.error("Max token usage reached.")
-                    break
-                new_instructions = [inst for insts in results for inst in insts]
-                for inst in new_instructions:
-                    with Pool(21) as pool:
-                        scores = pool.map(
-                            partial(scorer.score, inst["instruction"]),
-                            [
-                                item["instruction"]
-                                for item in self.seed_tasks + self.machine_tasks
-                            ],
-                        )
+            with Pool(60) as pool:
+                while (
+                    len(self.machine_tasks) < self.instruction_count
+                    or consume_remaining
+                ):
+                    instruction = queue.get()
+                    if not instruction:
+                        break
+                    scores = pool.map(
+                        partial(SCORER.score, instruction["instruction"]),
+                        [
+                            item["instruction"]
+                            for item in self.seed_tasks + self.machine_tasks
+                        ],
+                    )
                     scores = [score["rougeL"].fmeasure for score in scores]
                     max_score = max(scores)
                     if max_score > 0.7:
                         logger.warning(
-                            f"Skipping instruction, too similar: {max_score}: {inst['instruction']}"
+                            f"Skipping instruction, too similar: {max_score}: {instruction['instruction']}"
                         )
                         continue
-                    self.machine_tasks.append(inst)
-                    outfile.write(json.dumps(inst) + "\n")
-                outfile.flush()
-                logger.info(
-                    f"Generated {len(self.machine_tasks)} of {self.instruction_count}, tokens used: {self.used_tokens}"
-                )
+                    outfile.write(json.dumps(instruction) + "\n")
+                    outfile.flush()
+                    self.machine_tasks.append(instruction)
+                    logger.success(
+                        f"Generated unique instruction {len(self.machine_tasks)} of {self.instruction_count}"
+                    )
+            self.stop_producing = True
+
+    def run(self):
+        """Run the self-instruct, instruction generation task to completion."""
+        self.initialize_random_topics()
+        if len(self.machine_tasks) >= self.instruction_count:
+            logger.error(
+                f"Already have {len(self.machine_tasks)} machine-generated tasks!"
+            )
+            return
+        queue = Queue(maxsize=100)
+        producers = [
+            threading.Thread(target=self.generate_instruction_batches, args=(queue,))
+            for _ in range(50)
+        ]
+        for producer in producers:
+            producer.start()
+        consumer = threading.Thread(
+            target=self.validate_and_store_results, args=(queue,)
+        )
+        consumer.start()
+        consumer.join()
+        for producer in producers:
+            producer.join()
+
+        # Consume any tasks generated after the consumer stopped.
+        queue.put(None)
+        self.validate_and_store_results(queue, consume_remaining=True)
+
         logger.success(
             f"Finished generating {len(self.machine_tasks)} instructions and responses."
         )
 
 
 def main(args):
     random.seed(secrets.randbelow(1000000000))
     parser = argparse.ArgumentParser()
     for arg, kwargs in SelfInstructor.CLI_ARGS.items():
         parser.add_argument(arg, **kwargs)
-    instructor = SelfInstructor(**vars(parser.parse_args(args)))
-    asyncio.run(instructor.run())
+    SelfInstructor(**vars(parser.parse_args(args))).run()
 
 
 if __name__ == "__main__":
     main(sys.argv[1:])
```

## Comparing `airoboros-0.0.2.dist-info/LICENSE` & `airoboros-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `airoboros-0.0.2.dist-info/METADATA` & `airoboros-0.0.3.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airoboros
-Version: 0.0.2
+Version: 0.0.3
 Summary: Re-implementation of the self-instruct paper, with updated prompts, models, etc.
 Home-page: https://github.com/jondurbin/airoboros
 Author: Jon Durbin
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `airoboros-0.0.2.dist-info/RECORD` & `airoboros-0.0.3.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 airoboros/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 airoboros/entrypoint.py,sha256=w_S4_2Zoc2CmmcphEfyrONj4B0PnIklKyntp8WtNJPQ,466
 airoboros/exceptions.py,sha256=06gczZXTyuUFq11YTEQgGaZ6_MW5P0hvGTac2sRC0Wg,338
-airoboros/self_instruct.py,sha256=eTujLsRrZcEUQLeFnYJEPUi7Mw_hiOrkzMSQQoX784g,25713
-airoboros-0.0.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-airoboros-0.0.2.dist-info/METADATA,sha256=t3xVbweQ8bxaN4jXyB2Yhk1qVGO0u3VinWTt5mCtP74,763
-airoboros-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-airoboros-0.0.2.dist-info/entry_points.txt,sha256=Vhqdse5ngtMRa1qClYmg8Wy-tErchBpzLZBOWOnyXew,55
-airoboros-0.0.2.dist-info/top_level.txt,sha256=MSIee4BzO3BXxJ2dBXvQwpCKxiT9yE-lQ6_HRSW7COo,10
-airoboros-0.0.2.dist-info/RECORD,,
+airoboros/self_instruct.py,sha256=FgQuht7ENa8XTlYL2HEJujzRE7JlxEbcjA1AymroZVc,27679
+airoboros-0.0.3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+airoboros-0.0.3.dist-info/METADATA,sha256=qk37kh6ge4vB1foj2xFFEkQO6_YVwErmyX6aL1fzwb0,763
+airoboros-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+airoboros-0.0.3.dist-info/entry_points.txt,sha256=Vhqdse5ngtMRa1qClYmg8Wy-tErchBpzLZBOWOnyXew,55
+airoboros-0.0.3.dist-info/top_level.txt,sha256=MSIee4BzO3BXxJ2dBXvQwpCKxiT9yE-lQ6_HRSW7COo,10
+airoboros-0.0.3.dist-info/RECORD,,
```

