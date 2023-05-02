# Comparing `tmp/gpyt-0.1.2.tar.gz` & `tmp/gpyt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpyt-0.1.2.tar", max compression
+gzip compressed data, was "gpyt-0.1.3.tar", max compression
```

## Comparing `gpyt-0.1.2.tar` & `gpyt-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0      458 2023-05-01 20:13:45.517304 gpyt-0.1.2/README.md
--rw-r--r--   0        0        0      974 2023-05-01 19:43:03.287304 gpyt-0.1.2/gpyt/__init__.py
--rw-r--r--   0        0        0       30 2023-05-01 19:44:00.177304 gpyt-0.1.2/gpyt/__main__.py
--rw-r--r--   0        0        0      636 2023-05-01 19:40:49.577304 gpyt-0.1.2/gpyt/app.py
--rw-r--r--   0        0        0      877 2023-05-01 19:53:17.717304 gpyt-0.1.2/gpyt/assistant.py
--rw-r--r--   0        0        0      332 2023-05-01 20:17:32.707304 gpyt-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      852 1970-01-01 00:00:00.000000 gpyt-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      657 2023-05-01 23:17:49.417304 gpyt-0.1.3/README.md
+-rw-r--r--   0        0        0     1351 2023-05-02 00:03:47.517304 gpyt-0.1.3/gpyt/__init__.py
+-rw-r--r--   0        0        0      139 2023-05-01 23:19:19.957304 gpyt-0.1.3/gpyt/__main__.py
+-rw-r--r--   0        0        0     1863 2023-05-01 23:46:09.787304 gpyt-0.1.3/gpyt/app.py
+-rw-r--r--   0        0        0     1558 2023-05-02 00:00:28.177304 gpyt-0.1.3/gpyt/assistant.py
+-rw-r--r--   0        0        0      225 2023-05-01 23:48:52.967304 gpyt-0.1.3/gpyt/debug.py
+-rw-r--r--   0        0        0       44 2023-05-01 23:33:50.517304 gpyt-0.1.3/gpyt/exception.py
+-rw-r--r--   0        0        0      353 2023-05-02 00:04:48.157304 gpyt-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1093 1970-01-01 00:00:00.000000 gpyt-0.1.3/PKG-INFO
```

### Comparing `gpyt-0.1.2/PKG-INFO` & `gpyt-0.1.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,43 @@
 Metadata-Version: 2.1
 Name: gpyt
-Version: 0.1.2
+Version: 0.1.3
 Summary: GPT on the command line.
 Author: Justin Stitt
 Author-email: jstitt007@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: openai (>=0.27.5,<0.28.0)
+Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # gpyt
 
 Interact with GPT on the command line.
 
 
+> WIP
+
+### How to run:
+```sh
+$ pip install gpyt
+
+add `OPENAI_API_KEY="<your_openai_api_key>"` in a `.env` at $HOME
+
+$ python -m gpyt
+```
 
 ### Desired Features
 * `copy` to copy GPT's response to clipboard
 * color coded responses
 * add gpt jailbreaks (DAN-esque)
 * `new` to start a new chat (clear all history and console window)
 * store chat logs somewhere.
-* add special flags like -t (terse) or -v (verbose) or -d (detailed) or -i (informal) or -f (for file input)
+* add special flags like -t (terse) or -v (verbose) or -d (detailed) or -i
+  (informal) or -f (for file input) or --dan (for jailbreak)
 * scrolling text (adjustable speed, or disable all together)
 * use streams api?
+* model select CLI
+* loading wheel
```

