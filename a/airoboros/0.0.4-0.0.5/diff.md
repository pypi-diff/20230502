# Comparing `tmp/airoboros-0.0.4-py3-none-any.whl.zip` & `tmp/airoboros-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 15395 bytes, number of entries: 10
+Zip file size: 16201 bytes, number of entries: 10
 -rw-r--r--  2.0 unx        0 b- defN 23-May-01 08:36 airoboros/__init__.py
 -rw-r--r--  2.0 unx      466 b- defN 23-May-01 09:54 airoboros/entrypoint.py
 -rw-r--r--  2.0 unx      338 b- defN 23-May-01 19:03 airoboros/exceptions.py
--rw-r--r--  2.0 unx    27679 b- defN 23-May-02 08:28 airoboros/self_instruct.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-02 09:02 airoboros-0.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     5437 b- defN 23-May-02 09:02 airoboros-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-02 09:02 airoboros-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       55 b- defN 23-May-02 09:02 airoboros-0.0.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-May-02 09:02 airoboros-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      811 b- defN 23-May-02 09:02 airoboros-0.0.4.dist-info/RECORD
-10 files, 46245 bytes uncompressed, 14005 bytes compressed:  69.7%
+-rw-r--r--  2.0 unx    28601 b- defN 23-May-02 15:33 airoboros/self_instruct.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-02 17:48 airoboros-0.0.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5992 b- defN 23-May-02 17:48 airoboros-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-02 17:48 airoboros-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       55 b- defN 23-May-02 17:48 airoboros-0.0.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-May-02 17:48 airoboros-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      811 b- defN 23-May-02 17:48 airoboros-0.0.5.dist-info/RECORD
+10 files, 47722 bytes uncompressed, 14811 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: airoboros/exceptions.py
 Comment: 
 
 Filename: airoboros/self_instruct.py
 Comment: 
 
-Filename: airoboros-0.0.4.dist-info/LICENSE
+Filename: airoboros-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: airoboros-0.0.4.dist-info/METADATA
+Filename: airoboros-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: airoboros-0.0.4.dist-info/WHEEL
+Filename: airoboros-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: airoboros-0.0.4.dist-info/entry_points.txt
+Filename: airoboros-0.0.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: airoboros-0.0.4.dist-info/top_level.txt
+Filename: airoboros-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: airoboros-0.0.4.dist-info/RECORD
+Filename: airoboros-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## airoboros/self_instruct.py

```diff
@@ -7,30 +7,31 @@
 import requests
 import secrets
 import signal
 import string
 import sys
 import threading
 import concurrent.futures
-from multiprocessing import Pool
 from functools import partial
 from loguru import logger
 from queue import Queue
+from rouge_score import rouge_scorer
 from typing import List, Dict, Any
 from uuid import uuid4
-from rouge_score import rouge_scorer
 from .exceptions import (
     RateLimitError,
     TooManyRequestsError,
     TokensExhaustedError,
     ServerOverloadedError,
     ServerError,
     ContextLengthExceededError,
     BadResponseError,
 )
+from langchain.vectorstores import Chroma
+from langchain.embeddings import HuggingFaceEmbeddings
 
 # Defaults and constants.
 BATCH_SIZE = 13
 DEFAULT_PROMPT = f"""You are asked to generate a set of {BATCH_SIZE} diverse prompts.  These prompts will be given to a GPT model and we will evaluate the GPT model for completing the prompts.
 
 Here are the requirements:
  * Try not to repeat the verb for each __instruction__ to maximize diversity.
@@ -67,15 +68,14 @@
         "gpt-4-0314",
         "gpt-4-32k",
         "gpt-4-32k-0314",
         "gpt-3.5-turbo",
         "gpt-3.5-turbo-0301",
     ],
 }
-SCORER = rouge_scorer.RougeScorer(["rougeL"], use_stemmer=False)
 
 
 class SelfInstructor:
     """Class and methods used to generate instructions, based on self-instruct paper/code."""
 
     CLI_ARGS = {
         "--model": {
@@ -162,14 +162,24 @@
             "default": 2,
             "help": "presence penalty to use in OpenAI requests",
         },
         "--max-usage-tokens": {
             "type": int,
             "help": "Maximum token usage, calculated as sum of total_tokens from responses",
         },
+        "--prompt-generation-concurrency": {
+            "type": int,
+            "help": "Number of concurrent prompt generation threads/requests to use",
+            "default": 50,
+        },
+        "--min-docsearch-score": {
+            "type": float,
+            "help": "Minimum similarity score when querying vector DB to consider a prompt unique",
+            "default": "0.35",
+        },
     }
 
     def __init__(
         self,
         *,
         model: str = "gpt-3.5-turbo",
         organization_id: str = None,
@@ -188,14 +198,16 @@
         max_instruction_length: int = 150,
         samples_per_request: int = 3,
         temperature: float = 0.7,
         top_p: float = 0.5,
         frequency_penalty: int = 0,
         presence_penalty: int = 2,
         max_usage_tokens: int | None = None,
+        prompt_generation_concurrency: int = 50,
+        min_docsearch_score: float = 0.35,
     ):
         """Constructor."""
         self.model = model
         self.organization_id = organization_id
         self.openai_api_key = openai_api_key or os.environ.get("OPENAI_API_KEY")
         if not self.openai_api_key:
             raise ValueError(
@@ -231,14 +243,27 @@
         self.max_usage_tokens = max_usage_tokens
         self._validate_model()
         self.machine_tasks = []
         self._initialize_seed_tasks(seed_tasks, seed_tasks_path, use_dolly_seed)
         self.used_tokens = 0
         self.random_topics = set([])
         self.stop_producing = False
+        self.prompt_generation_concurrency = prompt_generation_concurrency
+        self.min_docsearch_score = min_docsearch_score
+        self._initialize_docstore()
+
+    def _initialize_docstore(self):
+        """Initialize the in-memory vector database used to check prompt uniqueness."""
+        logger.info(
+            "Initializing in-memory document store for similarity comparison..."
+        )
+        texts = [
+            prompt["instruction"] for prompt in self.seed_tasks + self.machine_tasks
+        ]
+        self.docstore = Chroma.from_texts(texts, HuggingFaceEmbeddings())
 
     def _initialize_seed_tasks(
         self,
         seed_tasks: List[Dict[str, str]],
         seed_tasks_path: str,
         use_dolly_seed: bool,
     ):
@@ -480,15 +505,15 @@
                 {
                     "instruction": instruction_text,
                     "context": context,
                     "response": response,
                 }
             )
             logger.info(
-                f"Generated new task [has context: {context != ''}]: {instruction_text}"
+                f"Generated candidate task [has context: {context != ''}]: {instruction_text}"
             )
         return tasks
 
     @backoff.on_exception(
         backoff.expo,
         (
             requests.exceptions.ConnectionError,
@@ -612,56 +637,50 @@
     ) -> None:
         """Dedupe based on rouge score for each new instruction and save results.
 
         :param queue: Queue to consume messages from.
         :type queue: Queue
         """
         with open(self.output_path, "a+") as outfile:
-            with Pool(60) as pool:
-                while (
-                    len(self.machine_tasks) < self.instruction_count
-                    or consume_remaining
-                ):
-                    instruction = queue.get()
-                    if not instruction:
-                        break
-                    scores = pool.map(
-                        partial(SCORER.score, instruction["instruction"]),
-                        [
-                            item["instruction"]
-                            for item in self.seed_tasks + self.machine_tasks
-                        ],
-                    )
-                    scores = [score["rougeL"].fmeasure for score in scores]
-                    max_score = max(scores)
-                    if max_score > 0.7:
-                        logger.warning(
-                            f"Skipping instruction, too similar: {max_score}: {instruction['instruction']}"
-                        )
-                        continue
-                    outfile.write(json.dumps(instruction) + "\n")
-                    outfile.flush()
-                    self.machine_tasks.append(instruction)
-                    logger.success(
-                        f"Generated unique instruction {len(self.machine_tasks)} of {self.instruction_count}"
+            while len(self.machine_tasks) < self.instruction_count or consume_remaining:
+                instruction = queue.get()
+                if not instruction:
+                    break
+                similar = self.docstore.similarity_search_with_score(
+                    instruction["instruction"], k=1
+                )
+                similarity_score = 1.0
+                for _, score in similar:
+                    similarity_score = score
+                if similarity_score <= self.min_docsearch_score:
+                    logger.warning(
+                        f"Skipping instruction, too similar [{score}]: {instruction['instruction']}"
                     )
-            self.stop_producing = True
+                    continue
+                outfile.write(json.dumps(instruction) + "\n")
+                outfile.flush()
+                self.machine_tasks.append(instruction)
+                self.docstore.add_texts([instruction["instruction"]])
+                logger.success(
+                    f"Generated unique [score={similarity_score}] instruction [total={len(self.machine_tasks)}]: {instruction['instruction']}"
+                )
+        self.stop_producing = True
 
     def run(self):
         """Run the self-instruct, instruction generation task to completion."""
         self.initialize_random_topics()
         if len(self.machine_tasks) >= self.instruction_count:
             logger.error(
                 f"Already have {len(self.machine_tasks)} machine-generated tasks!"
             )
             return
         queue = Queue(maxsize=100)
         producers = [
             threading.Thread(target=self.generate_instruction_batches, args=(queue,))
-            for _ in range(50)
+            for _ in range(self.prompt_generation_concurrency)
         ]
         for producer in producers:
             producer.start()
         consumer = threading.Thread(
             target=self.validate_and_store_results, args=(queue,)
         )
         consumer.start()
```

## Comparing `airoboros-0.0.4.dist-info/LICENSE` & `airoboros-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `airoboros-0.0.4.dist-info/METADATA` & `airoboros-0.0.5.dist-info/METADATA`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: airoboros
-Version: 0.0.4
-Summary: Re-implementation of the self-instruct paper, with updated prompts, models, etc.
+Version: 0.0.5
+Summary: Updated and improved implementation of the self-instruct system.
 Home-page: https://github.com/jondurbin/airoboros
 Author: Jon Durbin
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
@@ -13,100 +13,89 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: rouge-score (>=0.1.2)
 Requires-Dist: aiohttp (>=3.8)
 Requires-Dist: backoff (>=2.2)
 Requires-Dist: requests (>=2.28)
 Requires-Dist: loguru (>=0.7)
+Requires-Dist: chromadb (>=0.3.21)
+Requires-Dist: langchain (>=0.0.155)
+Requires-Dist: sentence-transformers (>=2.2.2)
 Provides-Extra: dev
 Requires-Dist: black ; extra == 'dev'
 Requires-Dist: flake8 ; extra == 'dev'
 
-# AIroboros: Using large language models to fine-tune large language models.
+# airoboros: using large language models to fine-tune large language models
 
 This is my take on implementing the [Self-Instruct paper](https://arxiv.org/abs/2212.10560).  The approach is quite heavily modified, and uses the human generated seeds provided by [Databricks Dolly Project](https://huggingface.co/datasets/databricks/databricks-dolly-15k)
 
 This updated implementation supports either the /v1/completions endpoint or /v1/chat/completions, which is particularly useful in that it supports gpt-4 and gpt-3.5-turbo (which is 1/10 the cost of text-davinci-003).
 
+
+## Key differences
+
+* Sample instructions in prompts by default use the human-generated seeds from Dolly.
+* Machine-generated instructions are not sampled for prompt examples, to avoid degredation.
+* Support for either /v1/completions or /v1/chat/completions APIs (which allows gpt-3.5-turbo instead of text-davinci-003, as well as gpt-4 if you have access).
+* In memory vector db (Chroma) for similarity comparison, which is much faster than calculating rouge score for each generated instruction.
+* (Seemingly) better prompt, which includes injection of random topics to relate the instructions to, which creates much more diverse prompts.
+* Multi-threaded producers/consumer implementation for significantly faster runtimes (generally 150+ unique prompts per minute, more initially since there are fewer duplicates, decreasing over time).
+* Tries to ensure the context, if provided, is relevant to the topic and contains all the information that would be necessary to respond to the instruction, and nost just a link to article/etc.
+* Generally speaking, this implementation tries to reduce some of the [noise](https://github.com/tloen/alpaca-lora/issues/65)
+
+
 ## Generating instructions
 
 See available options via:
 ```
 airoboros generate-instructions --help
 ```
 
 Example output:
 ```
-usage: self_instruct.py [-h] [--model MODEL]
-                        [--organization-id ORGANIZATION_ID]
-                        [--openai-api-key OPENAI_API_KEY]
-                        [--instruction-count INSTRUCTION_COUNT]
-                        [--seed-tasks-path SEED_TASKS_PATH]
-                        [--output-path OUTPUT_PATH] [--overwrite]
-                        [--default-prompt-prefix DEFAULT_PROMPT_PREFIX]
-                        [--classification-prompt-prefix CLASSIFICATION_PROMPT_PREFIX]
-                        [--contextual-prompt-prefix CONTEXTUAL_PROMPT_PREFIX]
-                        [--skip-instruction-re SKIP_INSTRUCTION_RE]
-                        [--code-gen-re CODE_GEN_RE]
-                        [--min-instruction-length MIN_INSTRUCTION_LENGTH]
-                        [--max-instruction-length MAX_INSTRUCTION_LENGTH]
-                        [--max-tokens MAX_TOKENS] [--temperature TEMPERATURE]
-                        [--top-p TOP_P]
-                        [--frequency-penalty FREQUENCY_PENALTY]
-                        [--presence-penalty PRESENCE_PENALTY]
-                        [--max-usage-tokens MAX_USAGE_TOKENS]
+usage: self_instruct.py [-h] [--model MODEL] [--organization-id ORGANIZATION_ID] [--openai-api-key OPENAI_API_KEY] [--instruction-count INSTRUCTION_COUNT] [--seed-tasks-path SEED_TASKS_PATH] [--output-path OUTPUT_PATH] [--overwrite] [--append] [--prompt PROMPT] [--skip-instruction-re SKIP_INSTRUCTION_RE] [--code-gen-re CODE_GEN_RE]
+                        [--samples-per-request SAMPLES_PER_REQUEST] [--min-instruction-length MIN_INSTRUCTION_LENGTH] [--max-instruction-length MAX_INSTRUCTION_LENGTH] [--temperature TEMPERATURE] [--top-p TOP_P] [--frequency-penalty FREQUENCY_PENALTY] [--presence-penalty PRESENCE_PENALTY] [--max-usage-tokens MAX_USAGE_TOKENS]
+                        [--prompt-generation-concurrency PROMPT_GENERATION_CONCURRENCY] [--min-docsearch-score MIN_DOCSEARCH_SCORE]
 
 options:
   -h, --help            show this help message and exit
-  --model MODEL         OpenAI model/engine to use for prompt generation,
-                        which can be either part of the /v1/completions or
-                        /v1/chat/completions endpoints
+  --model MODEL         OpenAI model/engine to use for prompt generation, which can be either part of the /v1/completions or /v1/chat/completions endpoints
   --organization-id ORGANIZATION_ID
-                        organization ID to include in the request to OpenAI,
-                        defaults to organization ID tied to the API key
+                        organization ID to include in the request to OpenAI, defaults to organization ID tied to the API key
   --openai-api-key OPENAI_API_KEY
-                        OpenAI API key to use, defaults to the OPENAI_API_KEY
-                        environment variable
+                        OpenAI API key to use, defaults to the OPENAI_API_KEY environment variable
   --instruction-count INSTRUCTION_COUNT
-                        number of instructions to generate, not including the
-                        seed instructions
+                        number of instructions to generate, not including the seed instructions
   --seed-tasks-path SEED_TASKS_PATH
                         path to an input seed instructions JSONL file
   --output-path OUTPUT_PATH
                         path to store all generated instructions in
   --overwrite           overwrite output path if it exists
-  --default-prompt-prefix DEFAULT_PROMPT_PREFIX
-                        prompt prefix to use for generating open, non-
-                        classification tasks
-  --classification-prompt-prefix CLASSIFICATION_PROMPT_PREFIX
-                        prompt prefix to use for generating classification
-                        tasks
-  --contextual-prompt-prefix CONTEXTUAL_PROMPT_PREFIX
-                        prompt prefix to use for generating tasks with
-                        context, e.g. closed Q&A
+  --append              append to output path if it exists
+  --prompt PROMPT       prompt prefix to use for generating tasks
   --skip-instruction-re SKIP_INSTRUCTION_RE
-                        regular expression used to filter low-quality/unusable
-                        instructions
+                        regular expression used to filter low-quality/unusable instructions
   --code-gen-re CODE_GEN_RE
-                        regular expression used to filter coding/programming
-                        tasks
+                        regular expression used to filter coding/programming tasks
+  --samples-per-request SAMPLES_PER_REQUEST
+                        number of random sample instructions to include in prompts
   --min-instruction-length MIN_INSTRUCTION_LENGTH
                         minimum instruction length
   --max-instruction-length MAX_INSTRUCTION_LENGTH
                         maximum instruction length
-  --max-tokens MAX_TOKENS
-                        maximum number of tokens in an instruction
   --temperature TEMPERATURE
                         temperature parameter to use in OpenAI requests
   --top-p TOP_P         top-p parameter to use in OpenAI requests
   --frequency-penalty FREQUENCY_PENALTY
                         frequency penalty to use in OpenAI requests
   --presence-penalty PRESENCE_PENALTY
                         presence penalty to use in OpenAI requests
   --max-usage-tokens MAX_USAGE_TOKENS
-                        Maximum token usage, calculated as sum of total_tokens
-                        from responses
+                        Maximum token usage, calculated as sum of total_tokens from responses
+  --prompt-generation-concurrency PROMPT_GENERATION_CONCURRENCY
+                        Number of concurrent prompt generation threads/requests to use
+  --min-docsearch-score MIN_DOCSEARCH_SCORE
 ```
 
 ## Coming soon
 
 Scripts for fine-tuning various models using the self-instruct (and human-generated) prompts.
```

