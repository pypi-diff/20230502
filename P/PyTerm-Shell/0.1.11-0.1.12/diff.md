# Comparing `tmp/PyTerm-Shell-0.1.11.tar.gz` & `tmp/PyTerm-Shell-0.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyTerm-Shell-0.1.11.tar", last modified: Tue May  2 01:16:02 2023, max compression
+gzip compressed data, was "PyTerm-Shell-0.1.12.tar", last modified: Tue May  2 01:20:45 2023, max compression
```

## Comparing `PyTerm-Shell-0.1.11.tar` & `PyTerm-Shell-0.1.12.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-02 01:16:02.037128 PyTerm-Shell-0.1.11/
--rw-rw-r--   0 nick      (1000) nick      (1000)       53 2023-05-02 01:05:57.000000 PyTerm-Shell-0.1.11/MANIFEST.in
--rw-rw-r--   0 nick      (1000) nick      (1000)     2756 2023-05-02 01:16:02.037128 PyTerm-Shell-0.1.11/PKG-INFO
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-02 01:16:02.025122 PyTerm-Shell-0.1.11/PyTerm/
--rw-rw-r--   0 nick      (1000) nick      (1000)    12547 2023-05-02 00:25:56.000000 PyTerm-Shell-0.1.11/PyTerm/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)       48 2023-05-02 00:50:12.000000 PyTerm-Shell-0.1.11/PyTerm/cli_assist.py
--rw-rw-r--   0 nick      (1000) nick      (1000)       96 2023-05-01 21:20:12.000000 PyTerm-Shell-0.1.11/PyTerm/config.json
--rw-rw-r--   0 nick      (1000) nick      (1000)      295 2023-05-01 21:20:12.000000 PyTerm-Shell-0.1.11/PyTerm/styles.css
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-02 01:16:02.037128 PyTerm-Shell-0.1.11/PyTerm_Shell.egg-info/
--rw-rw-r--   0 nick      (1000) nick      (1000)     2756 2023-05-02 01:16:02.000000 PyTerm-Shell-0.1.11/PyTerm_Shell.egg-info/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)      290 2023-05-02 01:16:02.000000 PyTerm-Shell-0.1.11/PyTerm_Shell.egg-info/SOURCES.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-05-02 01:16:02.000000 PyTerm-Shell-0.1.11/PyTerm_Shell.egg-info/dependency_links.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       50 2023-05-02 01:16:02.000000 PyTerm-Shell-0.1.11/PyTerm_Shell.egg-info/entry_points.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        7 2023-05-02 01:16:02.000000 PyTerm-Shell-0.1.11/PyTerm_Shell.egg-info/top_level.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)     2421 2023-05-02 01:13:29.000000 PyTerm-Shell-0.1.11/README.md
--rw-rw-r--   0 nick      (1000) nick      (1000)       38 2023-05-02 01:16:02.037128 PyTerm-Shell-0.1.11/setup.cfg
--rw-rw-r--   0 nick      (1000) nick      (1000)      803 2023-05-02 01:15:50.000000 PyTerm-Shell-0.1.11/setup.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-02 01:20:45.402740 PyTerm-Shell-0.1.12/
+-rw-rw-r--   0 nick      (1000) nick      (1000)       53 2023-05-02 01:05:57.000000 PyTerm-Shell-0.1.12/MANIFEST.in
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2756 2023-05-02 01:20:45.402740 PyTerm-Shell-0.1.12/PKG-INFO
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-02 01:20:45.394736 PyTerm-Shell-0.1.12/PyTerm/
+-rw-rw-r--   0 nick      (1000) nick      (1000)    12547 2023-05-02 00:25:56.000000 PyTerm-Shell-0.1.12/PyTerm/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)       48 2023-05-02 00:50:12.000000 PyTerm-Shell-0.1.12/PyTerm/cli_assist.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)       96 2023-05-01 21:20:12.000000 PyTerm-Shell-0.1.12/PyTerm/config.json
+-rw-rw-r--   0 nick      (1000) nick      (1000)      295 2023-05-01 21:20:12.000000 PyTerm-Shell-0.1.12/PyTerm/styles.css
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2023-05-02 01:20:45.402740 PyTerm-Shell-0.1.12/PyTerm_Shell.egg-info/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2756 2023-05-02 01:20:45.000000 PyTerm-Shell-0.1.12/PyTerm_Shell.egg-info/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)      325 2023-05-02 01:20:45.000000 PyTerm-Shell-0.1.12/PyTerm_Shell.egg-info/SOURCES.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        1 2023-05-02 01:20:45.000000 PyTerm-Shell-0.1.12/PyTerm_Shell.egg-info/dependency_links.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       50 2023-05-02 01:20:45.000000 PyTerm-Shell-0.1.12/PyTerm_Shell.egg-info/entry_points.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        8 2023-05-02 01:20:45.000000 PyTerm-Shell-0.1.12/PyTerm_Shell.egg-info/requires.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        7 2023-05-02 01:20:45.000000 PyTerm-Shell-0.1.12/PyTerm_Shell.egg-info/top_level.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2421 2023-05-02 01:13:29.000000 PyTerm-Shell-0.1.12/README.md
+-rw-rw-r--   0 nick      (1000) nick      (1000)       38 2023-05-02 01:20:45.402740 PyTerm-Shell-0.1.12/setup.cfg
+-rw-rw-r--   0 nick      (1000) nick      (1000)      853 2023-05-02 01:20:34.000000 PyTerm-Shell-0.1.12/setup.py
```

### Comparing `PyTerm-Shell-0.1.11/PKG-INFO` & `PyTerm-Shell-0.1.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTerm-Shell
-Version: 0.1.11
+Version: 0.1.12
 Summary: Making an aesthetic minimalist Linux shell in Python
 Home-page: https://github.com/MetalKamina/PyTerm
 Author: Nick Tsiones
 Author-email: ntsiones@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PyTerm-Shell-0.1.11/PyTerm/__init__.py` & `PyTerm-Shell-0.1.12/PyTerm/__init__.py`

 * *Files identical despite different names*

### Comparing `PyTerm-Shell-0.1.11/PyTerm_Shell.egg-info/PKG-INFO` & `PyTerm-Shell-0.1.12/PyTerm_Shell.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTerm-Shell
-Version: 0.1.11
+Version: 0.1.12
 Summary: Making an aesthetic minimalist Linux shell in Python
 Home-page: https://github.com/MetalKamina/PyTerm
 Author: Nick Tsiones
 Author-email: ntsiones@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PyTerm-Shell-0.1.11/README.md` & `PyTerm-Shell-0.1.12/README.md`

 * *Files identical despite different names*

### Comparing `PyTerm-Shell-0.1.11/setup.py` & `PyTerm-Shell-0.1.12/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,20 +7,23 @@
 long_description = (this_directory / "README.md").read_text()
 
 setup (
  name = 'PyTerm-Shell',
  description = 'Making an aesthetic minimalist Linux shell in Python',
  long_description = long_description,
  long_description_content_type='text/markdown',
- version = '0.1.11',
+ version = '0.1.12',
  python_requires='>=3.7',
  entry_points = {
         'console_scripts': ['PyTerm=PyTerm.cli_assist:main'],
  },
  include_package_data=True,
+ install_requires=[
+          'textual',
+      ],
  author="Nick Tsiones",
  license='MIT',
  url='https://github.com/MetalKamina/PyTerm',
   author_email='ntsiones@gmail.com',
   classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
```

