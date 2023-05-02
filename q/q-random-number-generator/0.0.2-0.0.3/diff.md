# Comparing `tmp/q_random_number_generator-0.0.2.tar.gz` & `tmp/q_random_number_generator-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "q_random_number_generator-0.0.2.tar", last modified: Tue May  2 12:08:16 2023, max compression
+gzip compressed data, was "q_random_number_generator-0.0.3.tar", last modified: Tue May  2 12:17:47 2023, max compression
```

## Comparing `q_random_number_generator-0.0.2.tar` & `q_random_number_generator-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 12:08:16.428180 q_random_number_generator-0.0.2/
--rw-rw-rw-   0        0        0     1065 2023-05-02 11:39:46.000000 q_random_number_generator-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      508 2023-05-02 12:08:16.427178 q_random_number_generator-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       64 2023-05-02 11:39:46.000000 q_random_number_generator-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 12:08:16.423178 q_random_number_generator-0.0.2/q_random_number_generator.egg-info/
--rw-rw-rw-   0        0        0      508 2023-05-02 12:08:16.000000 q_random_number_generator-0.0.2/q_random_number_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-05-02 12:08:16.000000 q_random_number_generator-0.0.2/q_random_number_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 12:08:16.000000 q_random_number_generator-0.0.2/q_random_number_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 12:08:16.000000 q_random_number_generator-0.0.2/q_random_number_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 12:08:16.429180 q_random_number_generator-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      667 2023-05-02 12:08:08.000000 q_random_number_generator-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:17:47.853293 q_random_number_generator-0.0.3/
+-rw-rw-rw-   0        0        0     1065 2023-05-02 11:39:46.000000 q_random_number_generator-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      522 2023-05-02 12:17:47.851061 q_random_number_generator-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       78 2023-05-02 12:16:38.000000 q_random_number_generator-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 12:17:47.836249 q_random_number_generator-0.0.3/q_random_number_generator/
+-rw-rw-rw-   0        0        0       32 2023-05-02 12:16:24.000000 q_random_number_generator-0.0.3/q_random_number_generator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:17:47.848544 q_random_number_generator-0.0.3/q_random_number_generator.egg-info/
+-rw-rw-rw-   0        0        0      522 2023-05-02 12:17:47.000000 q_random_number_generator-0.0.3/q_random_number_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-05-02 12:17:47.000000 q_random_number_generator-0.0.3/q_random_number_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 12:17:47.000000 q_random_number_generator-0.0.3/q_random_number_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-05-02 12:17:47.000000 q_random_number_generator-0.0.3/q_random_number_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 12:17:47.854305 q_random_number_generator-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      667 2023-05-02 12:16:29.000000 q_random_number_generator-0.0.3/setup.py
```

### Comparing `q_random_number_generator-0.0.2/LICENSE` & `q_random_number_generator-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `q_random_number_generator-0.0.2/setup.py` & `q_random_number_generator-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="q_random_number_generator",
-    version="0.0.2",
+    version="0.0.3",
     author="Allen Wu",
     author_email="allen91.wu@gmail.com",
     description="Using qiskit to realize random number generator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/allen91wu/q_random_number_generator",
     packages=setuptools.find_packages(),
```

