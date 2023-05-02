# Comparing `tmp/chatgpt_bot-0.1.1.tar.gz` & `tmp/chatgpt_bot-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt_bot-0.1.1.tar", max compression
+gzip compressed data, was "chatgpt_bot-0.1.2.tar", max compression
```

## Comparing `chatgpt_bot-0.1.1.tar` & `chatgpt_bot-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      515 2023-05-01 21:07:06.025192 chatgpt_bot-0.1.1/README.md
--rwxr-xr-x   0        0        0     3695 2023-05-01 21:06:26.925330 chatgpt_bot-0.1.1/chatgpt_bot/__init__.py
--rw-r--r--   0        0        0      569 2023-05-01 23:41:31.586081 chatgpt_bot-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1297 1970-01-01 00:00:00.000000 chatgpt_bot-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      515 2023-05-01 21:07:06.025192 chatgpt_bot-0.1.2/README.md
+-rwxr-xr-x   0        0        0     4821 2023-05-02 00:09:31.445965 chatgpt_bot-0.1.2/chatgpt_bot/__init__.py
+-rw-r--r--   0        0        0      569 2023-05-02 00:10:01.945819 chatgpt_bot-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1297 1970-01-01 00:00:00.000000 chatgpt_bot-0.1.2/PKG-INFO
```

### Comparing `chatgpt_bot-0.1.1/README.md` & `chatgpt_bot-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `chatgpt_bot-0.1.1/chatgpt_bot/__init__.py` & `chatgpt_bot-0.1.2/chatgpt_bot/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """A small library that helps you to create ChatGPT bots."""
+import json
 import sqlite3
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 
 import openai
@@ -48,17 +49,32 @@
           "message" TEXT NOT NULL
         )
         """
         )
 
         self._cur.execute(
             """
+        CREATE TABLE IF NOT EXISTS "Metadata" (
+          "id" INTEGER PRIMARY KEY AUTOINCREMENT,
+          "conversation_id" TEXT NOT NULL,
+          "metadata" BLOB NOT NULL
+        )
+        """
+        )
+
+        self._cur.execute(
+            """
         CREATE INDEX IF NOT EXISTS "idx_message__conversation_id" ON "Message" ("conversation_id");
         """
         )
+        self._cur.execute(
+            """
+        CREATE INDEX IF NOT EXISTS "idx_metadata__conversation_id" ON "Metadata" ("conversation_id");
+        """
+        )
         self._con.commit()
 
     def _add_message(self, message: str, user: bool) -> None:
         """Add a message to the database."""
         self._cur.execute(
             """
         INSERT INTO "Message"
@@ -94,14 +110,33 @@
 
         messages = [
             {"id": x[0], "timestamp": x[1], "role": x[2], "message": x[3]}
             for x in reversed(self._cur.fetchall())
         ]
         return messages
 
+    def get_metadata(self) -> Any:
+        """Retrieve the metadata for the current conversation."""
+        self._cur.execute(
+            """SELECT id, metadata FROM "Metadata" WHERE conversation_id=?""",
+            (self._conversation_id,),
+        )
+        metadata = self._cur.fetchone()
+        if not metadata:
+            return None
+        return json.loads(metadata[1])
+
+    def set_metadata(self, metadata):
+        """Store some metadata for the current conversation."""
+        self._cur.execute(
+            """INSERT INTO "Metadata" (conversation_id, metadata) VALUES (?, ?);""",
+            (self._conversation_id, json.dumps(metadata)),
+        )
+        self._con.commit()
+
     def ask(self, message: str) -> str:
         """Ask ChatGPT a question."""
         chat = [{"role": "system", "content": self._system_prompt}]
         self._add_message(message, user=True)
         chat.extend(
             [{"role": m["role"], "content": m["message"]} for m in self._get_messages()]
         )
```

### Comparing `chatgpt_bot-0.1.1/pyproject.toml` & `chatgpt_bot-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chatgpt-bot"
-version = "0.1.1"
+version = "0.1.2"
 description = "A library that takes the pain out of creating ChatGPT bots."
 authors = ["Stavros Korokithakis <hi@stavros.io>"]
 repository = "https://github.com/skorokithakis/ChatGPT-Bot"
 homepage = "https://github.com/skorokithakis/ChatGPT-Bot"
 license = "MIT"
 readme = "README.md"
 packages = [{include = "chatgpt_bot"}]
```

### Comparing `chatgpt_bot-0.1.1/PKG-INFO` & `chatgpt_bot-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-bot
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library that takes the pain out of creating ChatGPT bots.
 Home-page: https://github.com/skorokithakis/ChatGPT-Bot
 License: MIT
 Author: Stavros Korokithakis
 Author-email: hi@stavros.io
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

