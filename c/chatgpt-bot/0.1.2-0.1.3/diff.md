# Comparing `tmp/chatgpt_bot-0.1.2.tar.gz` & `tmp/chatgpt_bot-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt_bot-0.1.2.tar", max compression
+gzip compressed data, was "chatgpt_bot-0.1.3.tar", max compression
```

## Comparing `chatgpt_bot-0.1.2.tar` & `chatgpt_bot-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      515 2023-05-01 21:07:06.025192 chatgpt_bot-0.1.2/README.md
--rwxr-xr-x   0        0        0     4821 2023-05-02 00:09:31.445965 chatgpt_bot-0.1.2/chatgpt_bot/__init__.py
--rw-r--r--   0        0        0      569 2023-05-02 00:10:01.945819 chatgpt_bot-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1297 1970-01-01 00:00:00.000000 chatgpt_bot-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      621 2023-05-02 00:55:38.104075 chatgpt_bot-0.1.3/README.md
+-rwxr-xr-x   0        0        0     4964 2023-05-02 00:53:52.160595 chatgpt_bot-0.1.3/chatgpt_bot/__init__.py
+-rw-r--r--   0        0        0      569 2023-05-02 00:56:05.047942 chatgpt_bot-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1403 1970-01-01 00:00:00.000000 chatgpt_bot-0.1.3/PKG-INFO
```

### Comparing `chatgpt_bot-0.1.2/README.md` & `chatgpt_bot-0.1.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -7,8 +7,12 @@
 ```python
 from chatgpt_bot import Conversation
 
 >>> conversation = Conversation("some random ID", api_key="YOUR_OPENAI_API_KEY")
 >>> conversation.ask("Hi, how are you today?")
 "As an AI language model, I don't have feelings, but I'm always ready to assist you
 with any questions or tasks you have. How can I help you today?"
+
+>>> conversation.set_metadata({"anything": "here"})
+>>> conversation.get_metadata()
+{"anything": "here"}
 ```
```

### Comparing `chatgpt_bot-0.1.2/chatgpt_bot/__init__.py` & `chatgpt_bot-0.1.3/chatgpt_bot/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         """
         )
 
         self._cur.execute(
             """
         CREATE TABLE IF NOT EXISTS "Metadata" (
           "id" INTEGER PRIMARY KEY AUTOINCREMENT,
-          "conversation_id" TEXT NOT NULL,
+          "conversation_id" TEXT NOT NULL UNIQUE,
           "metadata" BLOB NOT NULL
         )
         """
         )
 
         self._cur.execute(
             """
@@ -124,15 +124,20 @@
         if not metadata:
             return None
         return json.loads(metadata[1])
 
     def set_metadata(self, metadata):
         """Store some metadata for the current conversation."""
         self._cur.execute(
-            """INSERT INTO "Metadata" (conversation_id, metadata) VALUES (?, ?);""",
+            """
+            INSERT INTO Metadata (conversation_id, metadata)
+            VALUES (?, ?)
+            ON CONFLICT(conversation_id) DO UPDATE SET
+                metadata = excluded.metadata;
+            """,
             (self._conversation_id, json.dumps(metadata)),
         )
         self._con.commit()
 
     def ask(self, message: str) -> str:
         """Ask ChatGPT a question."""
         chat = [{"role": "system", "content": self._system_prompt}]
```

### Comparing `chatgpt_bot-0.1.2/pyproject.toml` & `chatgpt_bot-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chatgpt-bot"
-version = "0.1.2"
+version = "0.1.3"
 description = "A library that takes the pain out of creating ChatGPT bots."
 authors = ["Stavros Korokithakis <hi@stavros.io>"]
 repository = "https://github.com/skorokithakis/ChatGPT-Bot"
 homepage = "https://github.com/skorokithakis/ChatGPT-Bot"
 license = "MIT"
 readme = "README.md"
 packages = [{include = "chatgpt_bot"}]
```

### Comparing `chatgpt_bot-0.1.2/PKG-INFO` & `chatgpt_bot-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-bot
-Version: 0.1.2
+Version: 0.1.3
 Summary: A library that takes the pain out of creating ChatGPT bots.
 Home-page: https://github.com/skorokithakis/ChatGPT-Bot
 License: MIT
 Author: Stavros Korokithakis
 Author-email: hi@stavros.io
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -27,9 +27,13 @@
 ```python
 from chatgpt_bot import Conversation
 
 >>> conversation = Conversation("some random ID", api_key="YOUR_OPENAI_API_KEY")
 >>> conversation.ask("Hi, how are you today?")
 "As an AI language model, I don't have feelings, but I'm always ready to assist you
 with any questions or tasks you have. How can I help you today?"
+
+>>> conversation.set_metadata({"anything": "here"})
+>>> conversation.get_metadata()
+{"anything": "here"}
 ```
```

