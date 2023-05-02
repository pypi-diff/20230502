# Comparing `tmp/regex-2023.3.23.tar.gz` & `tmp/regex-2023.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regex-2023.3.23.tar", last modified: Thu Mar 23 17:39:39 2023, max compression
+gzip compressed data, was "regex-2023.5.2.tar", last modified: Tue May  2 13:59:14 2023, max compression
```

## Comparing `regex-2023.3.23.tar` & `regex-2023.5.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 17:39:39.091309 regex-2023.3.23/
--rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-03-23 17:39:35.000000 regex-2023.3.23/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-23 17:39:35.000000 regex-2023.3.23/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    40644 2023-03-23 17:39:39.091309 regex-2023.3.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    39805 2023-03-23 17:39:35.000000 regex-2023.3.23/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 17:39:39.083308 regex-2023.3.23/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   143294 2023-03-23 17:39:35.000000 regex-2023.3.23/docs/Features.html
--rw-r--r--   0 runner    (1001) docker     (123)    29426 2023-03-23 17:39:35.000000 regex-2023.3.23/docs/UnicodeProperties.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 17:39:39.087309 regex-2023.3.23/regex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40644 2023-03-23 17:39:38.000000 regex-2023.3.23/regex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-03-23 17:39:39.000000 regex-2023.3.23/regex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 17:39:38.000000 regex-2023.3.23/regex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-23 17:39:38.000000 regex-2023.3.23/regex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 17:39:39.087309 regex-2023.3.23/regex_3/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-23 17:39:35.000000 regex-2023.3.23/regex_3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   824720 2023-03-23 17:39:35.000000 regex-2023.3.23/regex_3/_regex.c
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-03-23 17:39:35.000000 regex-2023.3.23/regex_3/_regex.h
--rw-r--r--   0 runner    (1001) docker     (123)   141150 2023-03-23 17:39:35.000000 regex-2023.3.23/regex_3/_regex_core.py
--rw-r--r--   0 runner    (1001) docker     (123)  1837887 2023-03-23 17:39:35.000000 regex-2023.3.23/regex_3/_regex_unicode.c
--rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-03-23 17:39:35.000000 regex-2023.3.23/regex_3/_regex_unicode.h
--rw-r--r--   0 runner    (1001) docker     (123)    32811 2023-03-23 17:39:35.000000 regex-2023.3.23/regex_3/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)   219546 2023-03-23 17:39:35.000000 regex-2023.3.23/regex_3/test_regex.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 17:39:39.091309 regex-2023.3.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-03-23 17:39:35.000000 regex-2023.3.23/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 17:39:39.091309 regex-2023.3.23/tools/
--rw-r--r--   0 runner    (1001) docker     (123)    55247 2023-03-23 17:39:35.000000 regex-2023.3.23/tools/build_regex_unicode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:59:14.603610 regex-2023.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-05-02 13:59:12.000000 regex-2023.5.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-02 13:59:12.000000 regex-2023.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    40894 2023-05-02 13:59:14.603610 regex-2023.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    39805 2023-05-02 13:59:12.000000 regex-2023.5.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:59:14.595609 regex-2023.5.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   143294 2023-05-02 13:59:12.000000 regex-2023.5.2/docs/Features.html
+-rw-r--r--   0 runner    (1001) docker     (123)    29426 2023-05-02 13:59:12.000000 regex-2023.5.2/docs/UnicodeProperties.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:59:14.599609 regex-2023.5.2/regex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    40894 2023-05-02 13:59:14.000000 regex-2023.5.2/regex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-02 13:59:14.000000 regex-2023.5.2/regex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 13:59:14.000000 regex-2023.5.2/regex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 13:59:14.000000 regex-2023.5.2/regex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:59:14.603610 regex-2023.5.2/regex_3/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-02 13:59:12.000000 regex-2023.5.2/regex_3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   824720 2023-05-02 13:59:12.000000 regex-2023.5.2/regex_3/_regex.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-05-02 13:59:12.000000 regex-2023.5.2/regex_3/_regex.h
+-rw-r--r--   0 runner    (1001) docker     (123)   141150 2023-05-02 13:59:12.000000 regex-2023.5.2/regex_3/_regex_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1837887 2023-05-02 13:59:12.000000 regex-2023.5.2/regex_3/_regex_unicode.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-05-02 13:59:12.000000 regex-2023.5.2/regex_3/_regex_unicode.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32811 2023-05-02 13:59:12.000000 regex-2023.5.2/regex_3/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)   219546 2023-05-02 13:59:12.000000 regex-2023.5.2/regex_3/test_regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 13:59:14.603610 regex-2023.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-02 13:59:12.000000 regex-2023.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:59:14.603610 regex-2023.5.2/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)    55247 2023-05-02 13:59:12.000000 regex-2023.5.2/tools/build_regex_unicode.py
```

### Comparing `regex-2023.3.23/LICENSE.txt` & `regex-2023.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `regex-2023.3.23/PKG-INFO` & `regex-2023.5.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: regex
-Version: 2023.3.23
-Summary: Alternative regular expression module, to replace re.
-Home-page: https://github.com/mrabarnett/mrab-regex
-Author: Matthew Barnett
-Author-email: regex@mrabarnett.plus.com
-License: Apache Software License
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Text Processing
-Classifier: Topic :: Text Processing :: General
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-License-File: LICENSE.txt
-
 Introduction
 ------------
 
 This regex implementation is backwards-compatible with the standard 're' module, but offers additional functionality.
 
 Note
 ----
```

### Comparing `regex-2023.3.23/README.rst` & `regex-2023.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+Metadata-Version: 2.1
+Name: regex
+Version: 2023.5.2
+Summary: Alternative regular expression module, to replace re.
+Home-page: https://github.com/mrabarnett/mrab-regex
+Author: Matthew Barnett
+Author-email: regex@mrabarnett.plus.com
+License: Apache Software License
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Text Processing
+Classifier: Topic :: Text Processing :: General
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+
 Introduction
 ------------
 
 This regex implementation is backwards-compatible with the standard 're' module, but offers additional functionality.
 
 Note
 ----
```

### Comparing `regex-2023.3.23/docs/Features.html` & `regex-2023.5.2/docs/Features.html`

 * *Files identical despite different names*

### Comparing `regex-2023.3.23/docs/UnicodeProperties.rst` & `regex-2023.5.2/docs/UnicodeProperties.rst`

 * *Files identical despite different names*

### Comparing `regex-2023.3.23/regex.egg-info/PKG-INFO` & `regex-2023.5.2/regex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Metadata-Version: 2.1
 Name: regex
-Version: 2023.3.23
+Version: 2023.5.2
 Summary: Alternative regular expression module, to replace re.
 Home-page: https://github.com/mrabarnett/mrab-regex
 Author: Matthew Barnett
 Author-email: regex@mrabarnett.plus.com
 License: Apache Software License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: General
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

### Comparing `regex-2023.3.23/regex_3/_regex.c` & `regex-2023.5.2/regex_3/_regex.c`

 * *Files identical despite different names*

### Comparing `regex-2023.3.23/regex_3/_regex.h` & `regex-2023.5.2/regex_3/_regex.h`

 * *Files identical despite different names*

### Comparing `regex-2023.3.23/regex_3/_regex_core.py` & `regex-2023.5.2/regex_3/_regex_core.py`

 * *Files identical despite different names*

### Comparing `regex-2023.3.23/regex_3/_regex_unicode.c` & `regex-2023.5.2/regex_3/_regex_unicode.c`

 * *Files identical despite different names*

### Comparing `regex-2023.3.23/regex_3/_regex_unicode.h` & `regex-2023.5.2/regex_3/_regex_unicode.h`

 * *Files identical despite different names*

### Comparing `regex-2023.3.23/regex_3/regex.py` & `regex-2023.5.2/regex_3/regex.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,15 @@
   "sub", "subf", "subfn", "subn", "template", "Scanner", "A", "ASCII", "B",
   "BESTMATCH", "D", "DEBUG", "E", "ENHANCEMATCH", "S", "DOTALL", "F",
   "FULLCASE", "I", "IGNORECASE", "L", "LOCALE", "M", "MULTILINE", "P", "POSIX",
   "R", "REVERSE", "T", "TEMPLATE", "U", "UNICODE", "V0", "VERSION0", "V1",
   "VERSION1", "X", "VERBOSE", "W", "WORD", "error", "Regex", "__version__",
   "__doc__", "RegexFlag"]
 
-__version__ = "2.5.125"
+__version__ = "2.5.126"
 
 # --------------------------------------------------------------------
 # Public interface.
 
 def match(pattern, string, flags=0, pos=None, endpos=None, partial=False,
   concurrent=None, timeout=None, ignore_unused=False, **kwargs):
     """Try to apply the pattern at the start of the string, returning a match
```

### Comparing `regex-2023.3.23/regex_3/test_regex.py` & `regex-2023.5.2/regex_3/test_regex.py`

 * *Files identical despite different names*

### Comparing `regex-2023.3.23/setup.py` & `regex-2023.5.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,29 +3,34 @@
 from os.path import join
 
 with open('README.rst') as file:
     long_description = file.read()
 
 setup(
     name='regex',
-    version='2023.3.23',
+    version='2023.5.2',
     description='Alternative regular expression module, to replace re.',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Matthew Barnett',
     author_email='regex@mrabarnett.plus.com',
     url='https://github.com/mrabarnett/mrab-regex',
     license='Apache Software License',
 
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Scientific/Engineering :: Information Analysis',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: Text Processing',
         'Topic :: Text Processing :: General',
     ],
     python_requires='>=3.8',
```

### Comparing `regex-2023.3.23/tools/build_regex_unicode.py` & `regex-2023.5.2/tools/build_regex_unicode.py`

 * *Files identical despite different names*

