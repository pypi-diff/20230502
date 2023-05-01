# Comparing `tmp/prompt_wrangler-0.3.4.tar.gz` & `tmp/prompt_wrangler-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompt_wrangler-0.3.4.tar", last modified: Mon May  1 23:20:05 2023, max compression
+gzip compressed data, was "prompt_wrangler-0.3.5.tar", last modified: Mon May  1 23:22:07 2023, max compression
```

## Comparing `prompt_wrangler-0.3.4.tar` & `prompt_wrangler-0.3.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-01 23:20:05.692951 prompt_wrangler-0.3.4/
--rw-r--r--   0 maxshaw    (501) staff       (20)     2032 2023-05-01 23:20:05.692814 prompt_wrangler-0.3.4/PKG-INFO
--rw-r--r--   0 maxshaw    (501) staff       (20)     1360 2023-05-01 23:19:56.000000 prompt_wrangler-0.3.4/README.md
-drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-01 23:20:05.690980 prompt_wrangler-0.3.4/__pycache__/
--rw-r--r--   0 maxshaw    (501) staff       (20)     1814 2023-05-01 21:04:39.000000 prompt_wrangler-0.3.4/__pycache__/test_mock.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0 maxshaw    (501) staff       (20)     1883 2023-05-01 20:47:14.000000 prompt_wrangler-0.3.4/__pycache__/test_prompt_wrangler.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0 maxshaw    (501) staff       (20)     1196 2023-05-01 21:40:23.000000 prompt_wrangler-0.3.4/__pycache__/test_real.cpython-310-pytest-7.2.2.pyc
-drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-01 23:20:05.691461 prompt_wrangler-0.3.4/prompt_wrangler/
--rw-r--r--   0 maxshaw    (501) staff       (20)       69 2023-05-01 23:03:32.000000 prompt_wrangler-0.3.4/prompt_wrangler/__init__.py
-drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-01 23:20:05.692578 prompt_wrangler-0.3.4/prompt_wrangler/__pycache__/
--rw-r--r--   0 maxshaw    (501) staff       (20)      286 2023-05-01 23:05:04.000000 prompt_wrangler-0.3.4/prompt_wrangler/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 maxshaw    (501) staff       (20)     4111 2023-05-01 21:03:40.000000 prompt_wrangler-0.3.4/prompt_wrangler/__pycache__/client.cpython-310.pyc
--rw-r--r--   0 maxshaw    (501) staff       (20)     3786 2023-05-01 21:03:28.000000 prompt_wrangler-0.3.4/prompt_wrangler/client.py
--rw-r--r--   0 maxshaw    (501) staff       (20)      552 2023-05-01 20:51:29.000000 prompt_wrangler-0.3.4/prompt_wrangler/client.pyi
-drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-01 23:20:05.692234 prompt_wrangler-0.3.4/prompt_wrangler.egg-info/
--rw-r--r--   0 maxshaw    (501) staff       (20)     2032 2023-05-01 23:20:05.000000 prompt_wrangler-0.3.4/prompt_wrangler.egg-info/PKG-INFO
--rw-r--r--   0 maxshaw    (501) staff       (20)      612 2023-05-01 23:20:05.000000 prompt_wrangler-0.3.4/prompt_wrangler.egg-info/SOURCES.txt
--rw-r--r--   0 maxshaw    (501) staff       (20)        1 2023-05-01 23:20:05.000000 prompt_wrangler-0.3.4/prompt_wrangler.egg-info/dependency_links.txt
--rw-r--r--   0 maxshaw    (501) staff       (20)        9 2023-05-01 23:20:05.000000 prompt_wrangler-0.3.4/prompt_wrangler.egg-info/requires.txt
--rw-r--r--   0 maxshaw    (501) staff       (20)       16 2023-05-01 23:20:05.000000 prompt_wrangler-0.3.4/prompt_wrangler.egg-info/top_level.txt
--rwxr-xr-x   0 maxshaw    (501) staff       (20)      866 2023-05-01 14:35:01.000000 prompt_wrangler-0.3.4/publish.sh
--rw-r--r--   0 maxshaw    (501) staff       (20)        0 2023-05-01 20:47:41.000000 prompt_wrangler-0.3.4/run_prompt.py
--rw-r--r--   0 maxshaw    (501) staff       (20)       38 2023-05-01 23:20:05.693001 prompt_wrangler-0.3.4/setup.cfg
--rw-r--r--   0 maxshaw    (501) staff       (20)     1062 2023-05-01 23:20:05.000000 prompt_wrangler-0.3.4/setup.py
--rw-r--r--   0 maxshaw    (501) staff       (20)      910 2023-05-01 21:04:37.000000 prompt_wrangler-0.3.4/test_mock.py
--rw-r--r--   0 maxshaw    (501) staff       (20)      408 2023-05-01 21:40:20.000000 prompt_wrangler-0.3.4/test_real.py
+drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-01 23:22:07.838355 prompt_wrangler-0.3.5/
+-rw-r--r--   0 maxshaw    (501) staff       (20)     2032 2023-05-01 23:22:07.838200 prompt_wrangler-0.3.5/PKG-INFO
+-rw-r--r--   0 maxshaw    (501) staff       (20)     1360 2023-05-01 23:21:59.000000 prompt_wrangler-0.3.5/README.md
+drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-01 23:22:07.834214 prompt_wrangler-0.3.5/__pycache__/
+-rw-r--r--   0 maxshaw    (501) staff       (20)     1814 2023-05-01 21:04:39.000000 prompt_wrangler-0.3.5/__pycache__/test_mock.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0 maxshaw    (501) staff       (20)     1883 2023-05-01 20:47:14.000000 prompt_wrangler-0.3.5/__pycache__/test_prompt_wrangler.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0 maxshaw    (501) staff       (20)     1196 2023-05-01 21:40:23.000000 prompt_wrangler-0.3.5/__pycache__/test_real.cpython-310-pytest-7.2.2.pyc
+drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-01 23:22:07.834724 prompt_wrangler-0.3.5/prompt_wrangler/
+-rw-r--r--   0 maxshaw    (501) staff       (20)       69 2023-05-01 23:03:32.000000 prompt_wrangler-0.3.5/prompt_wrangler/__init__.py
+drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-01 23:22:07.837964 prompt_wrangler-0.3.5/prompt_wrangler/__pycache__/
+-rw-r--r--   0 maxshaw    (501) staff       (20)      286 2023-05-01 23:05:04.000000 prompt_wrangler-0.3.5/prompt_wrangler/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 maxshaw    (501) staff       (20)     4111 2023-05-01 21:03:40.000000 prompt_wrangler-0.3.5/prompt_wrangler/__pycache__/client.cpython-310.pyc
+-rw-r--r--   0 maxshaw    (501) staff       (20)     3786 2023-05-01 21:03:28.000000 prompt_wrangler-0.3.5/prompt_wrangler/client.py
+-rw-r--r--   0 maxshaw    (501) staff       (20)      552 2023-05-01 20:51:29.000000 prompt_wrangler-0.3.5/prompt_wrangler/client.pyi
+drwxr-xr-x   0 maxshaw    (501) staff       (20)        0 2023-05-01 23:22:07.837441 prompt_wrangler-0.3.5/prompt_wrangler.egg-info/
+-rw-r--r--   0 maxshaw    (501) staff       (20)     2032 2023-05-01 23:22:07.000000 prompt_wrangler-0.3.5/prompt_wrangler.egg-info/PKG-INFO
+-rw-r--r--   0 maxshaw    (501) staff       (20)      612 2023-05-01 23:22:07.000000 prompt_wrangler-0.3.5/prompt_wrangler.egg-info/SOURCES.txt
+-rw-r--r--   0 maxshaw    (501) staff       (20)        1 2023-05-01 23:22:07.000000 prompt_wrangler-0.3.5/prompt_wrangler.egg-info/dependency_links.txt
+-rw-r--r--   0 maxshaw    (501) staff       (20)        9 2023-05-01 23:22:07.000000 prompt_wrangler-0.3.5/prompt_wrangler.egg-info/requires.txt
+-rw-r--r--   0 maxshaw    (501) staff       (20)       16 2023-05-01 23:22:07.000000 prompt_wrangler-0.3.5/prompt_wrangler.egg-info/top_level.txt
+-rwxr-xr-x   0 maxshaw    (501) staff       (20)      866 2023-05-01 14:35:01.000000 prompt_wrangler-0.3.5/publish.sh
+-rw-r--r--   0 maxshaw    (501) staff       (20)        0 2023-05-01 20:47:41.000000 prompt_wrangler-0.3.5/run_prompt.py
+-rw-r--r--   0 maxshaw    (501) staff       (20)       38 2023-05-01 23:22:07.838405 prompt_wrangler-0.3.5/setup.cfg
+-rw-r--r--   0 maxshaw    (501) staff       (20)     1062 2023-05-01 23:22:07.000000 prompt_wrangler-0.3.5/setup.py
+-rw-r--r--   0 maxshaw    (501) staff       (20)      910 2023-05-01 21:04:37.000000 prompt_wrangler-0.3.5/test_mock.py
+-rw-r--r--   0 maxshaw    (501) staff       (20)      408 2023-05-01 21:40:20.000000 prompt_wrangler-0.3.5/test_real.py
```

### Comparing `prompt_wrangler-0.3.4/PKG-INFO` & `prompt_wrangler-0.3.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompt_wrangler
-Version: 0.3.4
+Version: 0.3.5
 Summary: A Python wrapper for the Prompt Wrangler REST API.
 Home-page: UNKNOWN
 Author: Max Shaw
 Author-email: max@exit38.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -61,15 +61,15 @@
 # Get a prompt
 prompt_path = "my-workspace/my-prompt-slug"
 prompt = prompt_wrangler.prompt(prompt_path)
 
 # Run the prompt
 args = {'input_text': 'some input'}
 result = prompt.run(args=args)
-prediciton = result.prediction
+prediction = result.prediction
 ```
 
 ## License
 
 This project is licensed under the MIT License.
 
 ## Local Development
```

### Comparing `prompt_wrangler-0.3.4/README.md` & `prompt_wrangler-0.3.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 # Get a prompt
 prompt_path = "my-workspace/my-prompt-slug"
 prompt = prompt_wrangler.prompt(prompt_path)
 
 # Run the prompt
 args = {'input_text': 'some input'}
 result = prompt.run(args=args)
-prediciton = result.prediction
+prediction = result.prediction
 ```
 
 ## License
 
 This project is licensed under the MIT License.
 
 ## Local Development
```

### Comparing `prompt_wrangler-0.3.4/__pycache__/test_mock.cpython-310-pytest-7.2.2.pyc` & `prompt_wrangler-0.3.5/__pycache__/test_mock.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `prompt_wrangler-0.3.4/__pycache__/test_prompt_wrangler.cpython-310-pytest-7.2.2.pyc` & `prompt_wrangler-0.3.5/__pycache__/test_prompt_wrangler.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `prompt_wrangler-0.3.4/__pycache__/test_real.cpython-310-pytest-7.2.2.pyc` & `prompt_wrangler-0.3.5/__pycache__/test_real.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `prompt_wrangler-0.3.4/prompt_wrangler/__pycache__/client.cpython-310.pyc` & `prompt_wrangler-0.3.5/prompt_wrangler/__pycache__/client.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `prompt_wrangler-0.3.4/prompt_wrangler/client.py` & `prompt_wrangler-0.3.5/prompt_wrangler/client.py`

 * *Files identical despite different names*

### Comparing `prompt_wrangler-0.3.4/prompt_wrangler/client.pyi` & `prompt_wrangler-0.3.5/prompt_wrangler/client.pyi`

 * *Files identical despite different names*

### Comparing `prompt_wrangler-0.3.4/prompt_wrangler.egg-info/PKG-INFO` & `prompt_wrangler-0.3.5/prompt_wrangler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompt-wrangler
-Version: 0.3.4
+Version: 0.3.5
 Summary: A Python wrapper for the Prompt Wrangler REST API.
 Home-page: UNKNOWN
 Author: Max Shaw
 Author-email: max@exit38.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -61,15 +61,15 @@
 # Get a prompt
 prompt_path = "my-workspace/my-prompt-slug"
 prompt = prompt_wrangler.prompt(prompt_path)
 
 # Run the prompt
 args = {'input_text': 'some input'}
 result = prompt.run(args=args)
-prediciton = result.prediction
+prediction = result.prediction
 ```
 
 ## License
 
 This project is licensed under the MIT License.
 
 ## Local Development
```

### Comparing `prompt_wrangler-0.3.4/prompt_wrangler.egg-info/SOURCES.txt` & `prompt_wrangler-0.3.5/prompt_wrangler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prompt_wrangler-0.3.4/publish.sh` & `prompt_wrangler-0.3.5/publish.sh`

 * *Files identical despite different names*

### Comparing `prompt_wrangler-0.3.4/setup.py` & `prompt_wrangler-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="prompt_wrangler",
-    version="0.3.4",
+    version="0.3.5",
     author="Max Shaw",
     author_email="max@exit38.org",
     description="A Python wrapper for the Prompt Wrangler REST API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # url="https://github.com/exit38/prompt_wrangler",
     packages=find_packages(),
```

### Comparing `prompt_wrangler-0.3.4/test_mock.py` & `prompt_wrangler-0.3.5/test_mock.py`

 * *Files identical despite different names*

