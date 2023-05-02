# Comparing `tmp/gpt4free-1.0.1.tar.gz` & `tmp/gpt4free-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "F:\Progamming Project\gpt4free python package\dist\.tmp-kn5ycqj3\gpt4free-1.0.1.tar", last modified: Tue May  2 13:37:56 2023, max compression
+gzip compressed data, was "F:\Progamming Project\gpt4free python package\dist\.tmp-r4xbsvi9\gpt4free-1.0.2.tar", last modified: Tue May  2 20:50:50 2023, max compression
```

## Comparing `gpt4free-1.0.1.tar` & `gpt4free-1.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 13:37:56.665055 gpt4free-1.0.1/
--rw-rw-rw-   0        0        0      171 2023-04-27 05:47:31.000000 gpt4free-1.0.1/AUTHORS.md
--rw-rw-rw-   0        0        0     3654 2023-04-27 05:47:31.000000 gpt4free-1.0.1/CONTRIBUTING.md
--rw-rw-rw-   0        0        0        0 2023-04-27 08:27:03.000000 gpt4free-1.0.1/HISTORY.md
--rw-rw-rw-   0        0        0     1739 2023-04-27 05:47:31.000000 gpt4free-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      209 2023-04-27 07:44:37.000000 gpt4free-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3533 2023-05-02 13:37:56.666055 gpt4free-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2116 2023-05-01 19:39:48.000000 gpt4free-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 13:37:56.649056 gpt4free-1.0.1/gpt4free/
--rw-rw-rw-   0        0        0     2068 2023-05-01 19:05:12.000000 gpt4free-1.0.1/gpt4free/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:37:56.659059 gpt4free-1.0.1/gpt4free/forefront/
--rw-rw-rw-   0        0        0     6503 2023-05-01 02:16:04.000000 gpt4free-1.0.1/gpt4free/forefront/__init__.py
--rw-rw-rw-   0        0        0      437 2023-05-01 02:16:04.000000 gpt4free-1.0.1/gpt4free/forefront/typing.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:37:56.659059 gpt4free-1.0.1/gpt4free/italygpt/
--rw-rw-rw-   0        0        0     1198 2023-05-02 13:23:51.000000 gpt4free-1.0.1/gpt4free/italygpt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:37:56.662061 gpt4free-1.0.1/gpt4free/theb/
--rw-rw-rw-   0        0        0     1887 2023-05-01 02:16:04.000000 gpt4free-1.0.1/gpt4free/theb/__init__.py
--rw-rw-rw-   0        0        0      106 2023-05-01 02:16:04.000000 gpt4free-1.0.1/gpt4free/theb/theb_test.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:37:56.663054 gpt4free-1.0.1/gpt4free/usesless/
--rw-rw-rw-   0        0        0     1744 2023-05-01 02:16:04.000000 gpt4free-1.0.1/gpt4free/usesless/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:37:56.664062 gpt4free-1.0.1/gpt4free/you/
--rw-rw-rw-   0        0        0     4037 2023-05-01 02:16:04.000000 gpt4free-1.0.1/gpt4free/you/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:37:56.656057 gpt4free-1.0.1/gpt4free.egg-info/
--rw-rw-rw-   0        0        0     3533 2023-05-02 13:37:56.000000 gpt4free-1.0.1/gpt4free.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      495 2023-05-02 13:37:56.000000 gpt4free-1.0.1/gpt4free.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 13:37:56.000000 gpt4free-1.0.1/gpt4free.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-02 13:37:56.000000 gpt4free-1.0.1/gpt4free.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      157 2023-05-02 13:37:56.000000 gpt4free-1.0.1/gpt4free.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-02 13:37:56.000000 gpt4free-1.0.1/gpt4free.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      451 2023-05-02 13:37:56.666055 gpt4free-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2237 2023-05-02 13:36:25.000000 gpt4free-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 20:50:50.328230 gpt4free-1.0.2/
+-rw-rw-rw-   0        0        0      171 2023-04-27 05:47:31.000000 gpt4free-1.0.2/AUTHORS.md
+-rw-rw-rw-   0        0        0     3654 2023-04-27 05:47:31.000000 gpt4free-1.0.2/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0        0 2023-04-27 08:27:03.000000 gpt4free-1.0.2/HISTORY.md
+-rw-rw-rw-   0        0        0     1739 2023-04-27 05:47:31.000000 gpt4free-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      209 2023-04-27 07:44:37.000000 gpt4free-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3964 2023-05-02 20:50:50.329234 gpt4free-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2528 2023-05-02 20:48:17.000000 gpt4free-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 20:50:50.305232 gpt4free-1.0.2/gpt4free/
+-rw-rw-rw-   0        0        0     2098 2023-05-02 20:50:04.000000 gpt4free-1.0.2/gpt4free/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 20:50:50.320229 gpt4free-1.0.2/gpt4free/forefront/
+-rw-rw-rw-   0        0        0     6503 2023-05-01 02:16:04.000000 gpt4free-1.0.2/gpt4free/forefront/__init__.py
+-rw-rw-rw-   0        0        0      437 2023-05-01 02:16:04.000000 gpt4free-1.0.2/gpt4free/forefront/typing.py
+drwxrwxrwx   0        0        0        0 2023-05-02 20:50:50.321234 gpt4free-1.0.2/gpt4free/italygpt/
+-rw-rw-rw-   0        0        0     1198 2023-05-02 13:23:51.000000 gpt4free-1.0.2/gpt4free/italygpt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 20:50:50.324231 gpt4free-1.0.2/gpt4free/theb/
+-rw-rw-rw-   0        0        0     1887 2023-05-01 02:16:04.000000 gpt4free-1.0.2/gpt4free/theb/__init__.py
+-rw-rw-rw-   0        0        0      106 2023-05-01 02:16:04.000000 gpt4free-1.0.2/gpt4free/theb/theb_test.py
+drwxrwxrwx   0        0        0        0 2023-05-02 20:50:50.326233 gpt4free-1.0.2/gpt4free/usesless/
+-rw-rw-rw-   0        0        0     1744 2023-05-01 02:16:04.000000 gpt4free-1.0.2/gpt4free/usesless/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 20:50:50.327232 gpt4free-1.0.2/gpt4free/you/
+-rw-rw-rw-   0        0        0     4037 2023-05-01 02:16:04.000000 gpt4free-1.0.2/gpt4free/you/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 20:50:50.317230 gpt4free-1.0.2/gpt4free.egg-info/
+-rw-rw-rw-   0        0        0     3964 2023-05-02 20:50:50.000000 gpt4free-1.0.2/gpt4free.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      495 2023-05-02 20:50:50.000000 gpt4free-1.0.2/gpt4free.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 20:50:50.000000 gpt4free-1.0.2/gpt4free.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-02 20:50:49.000000 gpt4free-1.0.2/gpt4free.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      157 2023-05-02 20:50:50.000000 gpt4free-1.0.2/gpt4free.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-02 20:50:50.000000 gpt4free-1.0.2/gpt4free.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      451 2023-05-02 20:50:50.330231 gpt4free-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2237 2023-05-02 20:50:04.000000 gpt4free-1.0.2/setup.py
```

### Comparing `gpt4free-1.0.1/CONTRIBUTING.md` & `gpt4free-1.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gpt4free-1.0.1/LICENSE` & `gpt4free-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt4free-1.0.1/PKG-INFO` & `gpt4free-1.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt4free
-Version: 1.0.1
+Version: 1.0.2
 Summary: decentralising the Ai Industry, just some language model api's...
 Home-page: https://github.com/rzashakeri/gpt4free-python-package
 Author: Reza Shakeri
 Author-email: rzashakeri@gmail.com
 License: GNU General Public License v3
 Project-URL: Homepage, https://github.com/rzashakeri/gpt4free-python-package
 Project-URL: Issue tracker, https://github.com/rzashakeri/gpt4free-python-package/issues
@@ -34,14 +34,15 @@
 decentralising the Ai Industry, just some language model api's... based on [gpt4free repository](https://github.com/xtekky/gpt4free)
 
 ## Supported Stable Api's
 1. you
 2. theb
 3. forefront
 4. usesless
+5. italygpt
 
 ## How Use ?
 
 ### Example Usage For You
 
 ```python
 
@@ -122,9 +123,27 @@
 
     req = usesless.Completion.create(prompt=prompt, parentMessageId=message_id)
 
     print(f"Answer: {req['text']}")
     message_id = req["id"]
 ```
 
+### Example Usage For  italygpt
+
+```python
+# create an instance
+from gpt4free import italygpt
+italygpt = italygpt.Completion()
+
+# initialize api
+italygpt.init()
+
+# get an answer
+italygpt.create(prompt="What is the meaning of life?")
+print(italygpt.answer) # html formatted
+
+# keep the old conversation
+italygpt.create(prompt="Are you a human?", messages=italygpt.messages)
+print(italygpt.answer)
+```
```

### Comparing `gpt4free-1.0.1/README.md` & `gpt4free-1.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 decentralising the Ai Industry, just some language model api's... based on [gpt4free repository](https://github.com/xtekky/gpt4free)
 
 ## Supported Stable Api's
 1. you
 2. theb
 3. forefront
 4. usesless
+5. italygpt
 
 ## How Use ?
 
 ### Example Usage For You
 
 ```python
 
@@ -95,7 +96,25 @@
 
     req = usesless.Completion.create(prompt=prompt, parentMessageId=message_id)
 
     print(f"Answer: {req['text']}")
     message_id = req["id"]
 ```
 
+### Example Usage For  italygpt
+
+```python
+# create an instance
+from gpt4free import italygpt
+italygpt = italygpt.Completion()
+
+# initialize api
+italygpt.init()
+
+# get an answer
+italygpt.create(prompt="What is the meaning of life?")
+print(italygpt.answer) # html formatted
+
+# keep the old conversation
+italygpt.create(prompt="Are you a human?", messages=italygpt.messages)
+print(italygpt.answer)
+```
```

### Comparing `gpt4free-1.0.1/gpt4free/__init__.py` & `gpt4free-1.0.2/gpt4free/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from enum import Enum
 
 from gpt4free import forefront
 from gpt4free import theb
 from gpt4free import you
 from gpt4free import usesless
+from gpt4free import italygpt
 
 __author__ = """Reza Shakeri"""
 __email__ = "rzashakeri@outlook.com"
-__version__ = "0.1.5"
+__version__ = "1.0.2"
 
 
 class Provider(Enum):
     """An enum representing  different providers."""
 
     You = 'you'
     Poe = 'poe'
```

### Comparing `gpt4free-1.0.1/gpt4free/forefront/__init__.py` & `gpt4free-1.0.2/gpt4free/forefront/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt4free-1.0.1/gpt4free/italygpt/__init__.py` & `gpt4free-1.0.2/gpt4free/italygpt/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt4free-1.0.1/gpt4free/theb/__init__.py` & `gpt4free-1.0.2/gpt4free/theb/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt4free-1.0.1/gpt4free/usesless/__init__.py` & `gpt4free-1.0.2/gpt4free/usesless/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt4free-1.0.1/gpt4free/you/__init__.py` & `gpt4free-1.0.2/gpt4free/you/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt4free-1.0.1/gpt4free.egg-info/PKG-INFO` & `gpt4free-1.0.2/gpt4free.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt4free
-Version: 1.0.1
+Version: 1.0.2
 Summary: decentralising the Ai Industry, just some language model api's...
 Home-page: https://github.com/rzashakeri/gpt4free-python-package
 Author: Reza Shakeri
 Author-email: rzashakeri@gmail.com
 License: GNU General Public License v3
 Project-URL: Homepage, https://github.com/rzashakeri/gpt4free-python-package
 Project-URL: Issue tracker, https://github.com/rzashakeri/gpt4free-python-package/issues
@@ -34,14 +34,15 @@
 decentralising the Ai Industry, just some language model api's... based on [gpt4free repository](https://github.com/xtekky/gpt4free)
 
 ## Supported Stable Api's
 1. you
 2. theb
 3. forefront
 4. usesless
+5. italygpt
 
 ## How Use ?
 
 ### Example Usage For You
 
 ```python
 
@@ -122,9 +123,27 @@
 
     req = usesless.Completion.create(prompt=prompt, parentMessageId=message_id)
 
     print(f"Answer: {req['text']}")
     message_id = req["id"]
 ```
 
+### Example Usage For  italygpt
+
+```python
+# create an instance
+from gpt4free import italygpt
+italygpt = italygpt.Completion()
+
+# initialize api
+italygpt.init()
+
+# get an answer
+italygpt.create(prompt="What is the meaning of life?")
+print(italygpt.answer) # html formatted
+
+# keep the old conversation
+italygpt.create(prompt="Are you a human?", messages=italygpt.messages)
+print(italygpt.answer)
+```
```

### Comparing `gpt4free-1.0.1/setup.py` & `gpt4free-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         "Ai"
     ],
     name='gpt4free',
     packages=find_packages(include=['gpt4free', 'gpt4free.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/rzashakeri/gpt4free-python-package',
-    version='1.0.1',
+    version='1.0.2',
     zip_safe=False,
     project_urls={
         "Homepage": "https://github.com/rzashakeri/gpt4free-python-package",
         "Issue tracker": "https://github.com/rzashakeri/gpt4free-python-package/issues",
         "Release notes": "https://github.com/rzashakeri/gpt4free-python-package/releases",
         "Source": "https://github.com/rzashakeri/gpt4free-python-package",
         "Discussions": "https://github.com/rzashakeri/gpt4free-python-package/discussions",
```

