# Comparing `tmp/pygpt4all-1.0.1.tar.gz` & `tmp/pygpt4all-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygpt4all-1.0.1.tar", last modified: Sun Apr 23 23:25:20 2023, max compression
+gzip compressed data, was "pygpt4all-1.1.0.tar", last modified: Tue May  2 20:08:02 2023, max compression
```

## Comparing `pygpt4all-1.0.1.tar` & `pygpt4all-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:25:20.528447 pygpt4all-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-23 23:25:12.000000 pygpt4all-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-23 23:25:20.528447 pygpt4all-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-04-23 23:25:12.000000 pygpt4all-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:25:20.528447 pygpt4all-1.0.1/pygpt4all/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 23:25:12.000000 pygpt4all-1.0.1/pygpt4all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-23 23:25:12.000000 pygpt4all-1.0.1/pygpt4all/_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-23 23:25:12.000000 pygpt4all-1.0.1/pygpt4all/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:25:20.528447 pygpt4all-1.0.1/pygpt4all/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 23:25:12.000000 pygpt4all-1.0.1/pygpt4all/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-23 23:25:12.000000 pygpt4all-1.0.1/pygpt4all/models/gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-23 23:25:12.000000 pygpt4all-1.0.1/pygpt4all/models/gpt4all_j.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 23:25:20.528447 pygpt4all-1.0.1/pygpt4all.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-23 23:25:20.000000 pygpt4all-1.0.1/pygpt4all.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-23 23:25:20.000000 pygpt4all-1.0.1/pygpt4all.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 23:25:20.000000 pygpt4all-1.0.1/pygpt4all.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 23:25:20.000000 pygpt4all-1.0.1/pygpt4all.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-23 23:25:20.000000 pygpt4all-1.0.1/pygpt4all.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 23:25:20.000000 pygpt4all-1.0.1/pygpt4all.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 23:25:20.528447 pygpt4all-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-23 23:25:12.000000 pygpt4all-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:08:02.453782 pygpt4all-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-02 20:07:52.000000 pygpt4all-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-02 20:08:02.453782 pygpt4all-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-02 20:07:52.000000 pygpt4all-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:08:02.449782 pygpt4all-1.1.0/pygpt4all/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-02 20:07:52.000000 pygpt4all-1.1.0/pygpt4all/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-02 20:07:52.000000 pygpt4all-1.1.0/pygpt4all/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-02 20:07:52.000000 pygpt4all-1.1.0/pygpt4all/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:08:02.449782 pygpt4all-1.1.0/pygpt4all/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:07:52.000000 pygpt4all-1.1.0/pygpt4all/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-02 20:07:52.000000 pygpt4all-1.1.0/pygpt4all/models/gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-02 20:07:52.000000 pygpt4all-1.1.0/pygpt4all/models/gpt4all_j.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:08:02.453782 pygpt4all-1.1.0/pygpt4all.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-02 20:08:02.000000 pygpt4all-1.1.0/pygpt4all.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-02 20:08:02.000000 pygpt4all-1.1.0/pygpt4all.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:08:02.000000 pygpt4all-1.1.0/pygpt4all.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:08:02.000000 pygpt4all-1.1.0/pygpt4all.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-02 20:08:02.000000 pygpt4all-1.1.0/pygpt4all.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-02 20:08:02.000000 pygpt4all-1.1.0/pygpt4all.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 20:08:02.453782 pygpt4all-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-02 20:07:52.000000 pygpt4all-1.1.0/setup.py
```

### Comparing `pygpt4all-1.0.1/LICENSE` & `pygpt4all-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygpt4all-1.0.1/pygpt4all/_logger.py` & `pygpt4all-1.1.0/pygpt4all/_logger.py`

 * *Files identical despite different names*

### Comparing `pygpt4all-1.0.1/setup.py` & `pygpt4all-1.1.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,26 +6,25 @@
 # read the contents of your README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
     name="pygpt4all",
-    version="1.0.1",
+    version="1.1.0",
     author="Abdeladim Sadiki",
     description="Official Python CPU inference for GPT4All language models based on llama.cpp and ggml",
     long_description=long_description,
     ext_modules=[],
     zip_safe=False,
     python_requires=">=3.8",
     packages=find_packages('.'),
     package_dir={'': '.'},
     long_description_content_type="text/markdown",
     license='MIT',
-    # project_urls={
-    #     'Documentation': '',
-    #     'Source': '',
-    #     'Tracker': '',
-    # },
-    install_requires=["pyllamacpp==1.0.6", "pygptj"],
-    # extras_require={"all": [""]},
+    project_urls={
+        'Documentation': 'https://nomic-ai.github.io/pygpt4all/',
+        'Source': 'https://github.com/nomic-ai/pygpt4all',
+        'Tracker': 'https://github.com/nomic-ai/pygpt4all/issues',
+    },
+    install_requires=["pyllamacpp", "pygptj"],
 )
```

