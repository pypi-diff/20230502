# Comparing `tmp/EdgeGPT-0.3.4.tar.gz` & `tmp/EdgeGPT-0.3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EdgeGPT-0.3.4.tar", last modified: Tue May  2 04:36:57 2023, max compression
+gzip compressed data, was "EdgeGPT-0.3.4.1.tar", last modified: Tue May  2 04:48:53 2023, max compression
```

## Comparing `EdgeGPT-0.3.4.tar` & `EdgeGPT-0.3.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:36:57.734876 EdgeGPT-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-02 04:36:22.000000 EdgeGPT-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-05-02 04:36:57.734876 EdgeGPT-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-05-02 04:36:57.000000 EdgeGPT-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-02 04:36:57.734876 EdgeGPT-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-02 04:36:22.000000 EdgeGPT-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:36:57.730876 EdgeGPT-0.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:36:57.734876 EdgeGPT-0.3.4/src/EdgeGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-05-02 04:36:57.000000 EdgeGPT-0.3.4/src/EdgeGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-02 04:36:57.000000 EdgeGPT-0.3.4/src/EdgeGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 04:36:57.000000 EdgeGPT-0.3.4/src/EdgeGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-02 04:36:57.000000 EdgeGPT-0.3.4/src/EdgeGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-02 04:36:57.000000 EdgeGPT-0.3.4/src/EdgeGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 04:36:57.000000 EdgeGPT-0.3.4/src/EdgeGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    27654 2023-05-02 04:36:22.000000 EdgeGPT-0.3.4/src/EdgeGPT.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-02 04:36:22.000000 EdgeGPT-0.3.4/src/ImageGen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:48:53.188743 EdgeGPT-0.3.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-02 04:48:20.000000 EdgeGPT-0.3.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-05-02 04:48:53.188743 EdgeGPT-0.3.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-05-02 04:48:53.000000 EdgeGPT-0.3.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-02 04:48:53.188743 EdgeGPT-0.3.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-02 04:48:20.000000 EdgeGPT-0.3.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:48:53.188743 EdgeGPT-0.3.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:48:53.188743 EdgeGPT-0.3.4.1/src/EdgeGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-05-02 04:48:53.000000 EdgeGPT-0.3.4.1/src/EdgeGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-02 04:48:53.000000 EdgeGPT-0.3.4.1/src/EdgeGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 04:48:53.000000 EdgeGPT-0.3.4.1/src/EdgeGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-02 04:48:53.000000 EdgeGPT-0.3.4.1/src/EdgeGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-02 04:48:53.000000 EdgeGPT-0.3.4.1/src/EdgeGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 04:48:53.000000 EdgeGPT-0.3.4.1/src/EdgeGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    28330 2023-05-02 04:48:20.000000 EdgeGPT-0.3.4.1/src/EdgeGPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-02 04:48:20.000000 EdgeGPT-0.3.4.1/src/ImageGen.py
```

### Comparing `EdgeGPT-0.3.4/LICENSE` & `EdgeGPT-0.3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.3.4/PKG-INFO` & `EdgeGPT-0.3.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.3.4
+Version: 0.3.4.1
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,17 +1,18 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.4 Summary: Reverse engineered
-Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
-Cheong Author-email: acheong@student.dalat.org License: GNU General Public
-License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
-issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
-Classifier: Intended Audience :: Developers Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.4.1 Summary: Reverse
+engineered Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT
+Author: Antonio Cheong Author-email: acheong@student.dalat.org License: GNU
+General Public License v2.0 Project-URL: Bug Report, https://github.com/
+acheong08/EdgeGPT/issues/new Classifier: License :: OSI Approved :: The
+Unlicense (Unlicense) Classifier: Intended Audience :: Developers Classifier:
+Topic :: Software Development :: Libraries :: Python Modules Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Description-Content-Type: text/markdown
+License-File: LICENSE
    [EdgeGPT] # Edge GPT _The reverse engineering the chat feature of the new
     version of Bing_ English - ç®ä½ä¸­æ - ç¹é«ä¸­æ_(ä¸­åèºç£) -
                              EspaÃ±ol - æ¥æ¬èª
                [PyPI_version] [Python version] [Total downloads]
 --- ## Setup ### Install package ```bash python3 -m pip install EdgeGPT --
 upgrade ``` ### Requirements - python 3.8+ - A Microsoft Account with early
 access to
```

### Comparing `EdgeGPT-0.3.4/README.md` & `EdgeGPT-0.3.4.1/README.md`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.3.4/setup.py` & `EdgeGPT-0.3.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="EdgeGPT",
-    version="0.3.4",
+    version="0.3.4.1",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineered Edge Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/EdgeGPT",
```

### Comparing `EdgeGPT-0.3.4/src/EdgeGPT.egg-info/PKG-INFO` & `EdgeGPT-0.3.4.1/src/EdgeGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.3.4
+Version: 0.3.4.1
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,17 +1,18 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.4 Summary: Reverse engineered
-Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
-Cheong Author-email: acheong@student.dalat.org License: GNU General Public
-License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
-issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
-Classifier: Intended Audience :: Developers Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.4.1 Summary: Reverse
+engineered Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT
+Author: Antonio Cheong Author-email: acheong@student.dalat.org License: GNU
+General Public License v2.0 Project-URL: Bug Report, https://github.com/
+acheong08/EdgeGPT/issues/new Classifier: License :: OSI Approved :: The
+Unlicense (Unlicense) Classifier: Intended Audience :: Developers Classifier:
+Topic :: Software Development :: Libraries :: Python Modules Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Description-Content-Type: text/markdown
+License-File: LICENSE
    [EdgeGPT] # Edge GPT _The reverse engineering the chat feature of the new
     version of Bing_ English - ç®ä½ä¸­æ - ç¹é«ä¸­æ_(ä¸­åèºç£) -
                              EspaÃ±ol - æ¥æ¬èª
                [PyPI_version] [Python version] [Total downloads]
 --- ## Setup ### Install package ```bash python3 -m pip install EdgeGPT --
 upgrade ``` ### Requirements - python 3.8+ - A Microsoft Account with early
 access to
```

### Comparing `EdgeGPT-0.3.4/src/EdgeGPT.py` & `EdgeGPT-0.3.4.1/src/EdgeGPT.py`

 * *Files 3% similar despite different names*

```diff
@@ -558,14 +558,35 @@
 
 
 class Chatbot:
     """
     Combines everything to make it seamless
     """
 
+    def __init__(
+        self,
+        cookies: dict = None,
+        proxy: str | None = None,
+        cookie_path: str = None,
+    ) -> None:
+        if cookies is None:
+            cookies = {}
+        if cookie_path is not None:
+            try:
+                with open(cookie_path, encoding="utf-8") as f:
+                    self.cookies = json.load(f)
+            except FileNotFoundError as exc:
+                raise FileNotFoundError("Cookie file not found") from exc
+        else:
+            self.cookies = cookies
+        self.proxy: str | None = proxy
+        self.chat_hub: _ChatHub = _ChatHub(
+            _Conversation(self.cookies, self.proxy),
+        )
+
     @staticmethod
     async def create(
         cookies: dict = None,
         proxy: str | None = None,
         cookie_path: str = None,
     ):
         self = Chatbot()
```

