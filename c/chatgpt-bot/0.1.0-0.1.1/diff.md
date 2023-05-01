# Comparing `tmp/chatgpt_bot-0.1.0.tar.gz` & `tmp/chatgpt_bot-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt_bot-0.1.0.tar", max compression
+gzip compressed data, was "chatgpt_bot-0.1.1.tar", max compression
```

## Comparing `chatgpt_bot-0.1.0.tar` & `chatgpt_bot-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      515 2023-05-01 21:07:06.025192 chatgpt_bot-0.1.0/README.md
--rwxr-xr-x   0        0        0     3695 2023-05-01 21:06:26.925330 chatgpt_bot-0.1.0/chatgpt_bot/__init__.py
--rw-r--r--   0        0        0      452 2023-05-01 21:01:59.498330 chatgpt_bot-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 chatgpt_bot-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      515 2023-05-01 21:07:06.025192 chatgpt_bot-0.1.1/README.md
+-rwxr-xr-x   0        0        0     3695 2023-05-01 21:06:26.925330 chatgpt_bot-0.1.1/chatgpt_bot/__init__.py
+-rw-r--r--   0        0        0      569 2023-05-01 23:41:31.586081 chatgpt_bot-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1297 1970-01-01 00:00:00.000000 chatgpt_bot-0.1.1/PKG-INFO
```

### Comparing `chatgpt_bot-0.1.0/README.md` & `chatgpt_bot-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `chatgpt_bot-0.1.0/chatgpt_bot/__init__.py` & `chatgpt_bot-0.1.1/chatgpt_bot/__init__.py`

 * *Files identical despite different names*

### Comparing `chatgpt_bot-0.1.0/PKG-INFO` & `chatgpt_bot-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Metadata-Version: 2.1
 Name: chatgpt-bot
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library that takes the pain out of creating ChatGPT bots.
+Home-page: https://github.com/skorokithakis/ChatGPT-Bot
 License: MIT
 Author: Stavros Korokithakis
 Author-email: hi@stavros.io
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: openai (>=0.27.5,<0.28.0)
+Project-URL: Repository, https://github.com/skorokithakis/ChatGPT-Bot
 Description-Content-Type: text/markdown
 
 ChatGPT Bot
 ===========
 
 This is a small library that tries to make it easier to create a ChatGPT bot. It has
 a simple interface that keeps conversational context in a SQLite database:
```

