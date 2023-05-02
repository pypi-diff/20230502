# Comparing `tmp/tuotuo-0.0.2.tar.gz` & `tmp/tuotuo-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuotuo-0.0.2.tar", last modified: Mon May  1 21:21:50 2023, max compression
+gzip compressed data, was "tuotuo-0.0.3.tar", last modified: Tue May  2 07:30:18 2023, max compression
```

## Comparing `tuotuo-0.0.2.tar` & `tuotuo-0.0.3.tar`

### file list

```diff
@@ -1,45 +1,39 @@
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-01 21:21:50.434500 tuotuo-0.0.2/
--rw-r--r--   0 ericliu    (501) staff       (20)     6148 2023-03-15 07:18:48.000000 tuotuo-0.0.2/.DS_Store
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-01 21:21:50.416888 tuotuo-0.0.2/.github/
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-01 21:21:50.421039 tuotuo-0.0.2/.github/workflows/
--rw-r--r--   0 ericliu    (501) staff       (20)     1313 2023-04-29 20:29:10.000000 tuotuo-0.0.2/.github/workflows/python-package.yml
--rw-r--r--   0 ericliu    (501) staff       (20)     1337 2023-05-01 20:35:00.000000 tuotuo-0.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0 ericliu    (501) staff       (20)       60 2023-05-01 21:19:43.000000 tuotuo-0.0.2/.gitignore
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-01 21:21:50.421280 tuotuo-0.0.2/.vscode/
--rw-r--r--   0 ericliu    (501) staff       (20)      520 2023-04-19 20:08:42.000000 tuotuo-0.0.2/.vscode/c_cpp_properties.json
--rw-r--r--   0 ericliu    (501) staff       (20)     1069 2023-04-29 19:24:24.000000 tuotuo-0.0.2/LICENSE
--rw-r--r--   0 ericliu    (501) staff       (20)     1515 2023-05-01 21:21:50.434655 tuotuo-0.0.2/PKG-INFO
--rw-r--r--   0 ericliu    (501) staff       (20)      693 2023-04-22 09:04:54.000000 tuotuo-0.0.2/README.md
--rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-03-04 12:30:22.000000 tuotuo-0.0.2/__init__.py
--rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-30 20:29:58.000000 tuotuo-0.0.2/cutils.cpython-38-darwin.so
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-01 21:21:50.424353 tuotuo-0.0.2/notebook/
--rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:28.000000 tuotuo-0.0.2/notebook/__init__.py
--rw-r--r--   0 ericliu    (501) staff       (20)     4572 2023-04-23 10:52:23.000000 tuotuo-0.0.2/notebook/computational_test.ipynb
--rw-r--r--   0 ericliu    (501) staff       (20)    56721 2023-05-01 20:21:00.000000 tuotuo-0.0.2/notebook/main copy.ipynb
--rw-r--r--   0 ericliu    (501) staff       (20)    83540 2023-04-23 10:52:50.000000 tuotuo-0.0.2/notebook/main.ipynb
--rw-r--r--   0 ericliu    (501) staff       (20)    91088 2023-04-19 06:55:27.000000 tuotuo-0.0.2/notebook/reference.ipynb
--rw-r--r--   0 ericliu    (501) staff       (20)    19221 2023-03-04 12:35:47.000000 tuotuo-0.0.2/notebook/test.ipynb
--rw-r--r--   0 ericliu    (501) staff       (20)     1542 2023-05-01 12:02:13.000000 tuotuo-0.0.2/requirements.txt
--rw-r--r--   0 ericliu    (501) staff       (20)       79 2023-05-01 21:21:50.435072 tuotuo-0.0.2/setup.cfg
--rw-r--r--   0 ericliu    (501) staff       (20)     1555 2023-05-01 21:21:40.000000 tuotuo-0.0.2/setup.py
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-01 21:21:50.429659 tuotuo-0.0.2/src/
--rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:21.000000 tuotuo-0.0.2/src/__init__.py
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-01 21:21:50.417298 tuotuo-0.0.2/src/build/
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-01 21:21:50.429929 tuotuo-0.0.2/src/build/lib.macosx-10.14-arm64-cpython-38/
--rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 tuotuo-0.0.2/src/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-01 21:21:50.431256 tuotuo-0.0.2/src/build/temp.macosx-10.14-arm64-cpython-38/
--rw-r--r--   0 ericliu    (501) staff       (20)  1829576 2023-04-19 20:17:36.000000 tuotuo-0.0.2/src/build/temp.macosx-10.14-arm64-cpython-38/cutils.o
--rw-r--r--   0 ericliu    (501) staff       (20)  1030110 2023-04-19 20:14:47.000000 tuotuo-0.0.2/src/cutils.c
--rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 tuotuo-0.0.2/src/cutils.cpython-38-darwin.so
--rw-r--r--   0 ericliu    (501) staff       (20)   163779 2023-04-19 20:14:47.000000 tuotuo-0.0.2/src/cutils.html
--rw-r--r--   0 ericliu    (501) staff       (20)     2477 2023-04-19 20:11:37.000000 tuotuo-0.0.2/src/cutils.pyx
--rw-r--r--   0 ericliu    (501) staff       (20)     9448 2023-04-28 13:26:46.000000 tuotuo-0.0.2/src/generator.py
--rw-r--r--   0 ericliu    (501) staff       (20)    16219 2023-04-29 19:54:15.000000 tuotuo-0.0.2/src/lda_model.py
--rw-r--r--   0 ericliu    (501) staff       (20)     5422 2023-04-29 19:52:57.000000 tuotuo-0.0.2/src/text_pre_processor.py
--rw-r--r--   0 ericliu    (501) staff       (20)     9789 2023-05-01 20:58:36.000000 tuotuo-0.0.2/src/utils.py
-drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-01 21:21:50.434382 tuotuo-0.0.2/tuotuo.egg-info/
--rw-r--r--   0 ericliu    (501) staff       (20)     1515 2023-05-01 21:21:50.000000 tuotuo-0.0.2/tuotuo.egg-info/PKG-INFO
--rw-r--r--   0 ericliu    (501) staff       (20)      803 2023-05-01 21:21:50.000000 tuotuo-0.0.2/tuotuo.egg-info/SOURCES.txt
--rw-r--r--   0 ericliu    (501) staff       (20)        1 2023-05-01 21:21:50.000000 tuotuo-0.0.2/tuotuo.egg-info/dependency_links.txt
--rw-r--r--   0 ericliu    (501) staff       (20)       28 2023-05-01 21:21:50.000000 tuotuo-0.0.2/tuotuo.egg-info/requires.txt
--rw-r--r--   0 ericliu    (501) staff       (20)       15 2023-05-01 21:21:50.000000 tuotuo-0.0.2/tuotuo.egg-info/top_level.txt
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 07:30:18.477188 tuotuo-0.0.3/
+-rw-r--r--   0 ericliu    (501) staff       (20)     6148 2023-03-15 07:18:48.000000 tuotuo-0.0.3/.DS_Store
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 07:30:18.461090 tuotuo-0.0.3/.github/
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 07:30:18.465276 tuotuo-0.0.3/.github/workflows/
+-rw-r--r--   0 ericliu    (501) staff       (20)     1313 2023-04-29 20:29:10.000000 tuotuo-0.0.3/.github/workflows/python-package.yml
+-rw-r--r--   0 ericliu    (501) staff       (20)     1337 2023-05-01 20:35:00.000000 tuotuo-0.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 ericliu    (501) staff       (20)       89 2023-05-01 21:37:45.000000 tuotuo-0.0.3/.gitignore
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 07:30:18.465544 tuotuo-0.0.3/.vscode/
+-rw-r--r--   0 ericliu    (501) staff       (20)      520 2023-04-19 20:08:42.000000 tuotuo-0.0.3/.vscode/c_cpp_properties.json
+-rw-r--r--   0 ericliu    (501) staff       (20)     1069 2023-04-29 19:24:24.000000 tuotuo-0.0.3/LICENSE
+-rw-r--r--   0 ericliu    (501) staff       (20)     1513 2023-05-02 07:30:18.477317 tuotuo-0.0.3/PKG-INFO
+-rw-r--r--   0 ericliu    (501) staff       (20)      693 2023-04-22 09:04:54.000000 tuotuo-0.0.3/README.md
+-rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-30 20:29:58.000000 tuotuo-0.0.3/cutils.cpython-38-darwin.so
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 07:30:18.466811 tuotuo-0.0.3/notebook/
+-rw-r--r--   0 ericliu    (501) staff       (20)    56799 2023-05-02 07:22:32.000000 tuotuo-0.0.3/notebook/Our Model vs SKLearn.ipynb
+-rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:28.000000 tuotuo-0.0.3/notebook/__init__.py
+-rw-r--r--   0 ericliu    (501) staff       (20)     1542 2023-05-01 12:02:13.000000 tuotuo-0.0.3/requirements.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)       79 2023-05-02 07:30:18.477623 tuotuo-0.0.3/setup.cfg
+-rw-r--r--   0 ericliu    (501) staff       (20)     1568 2023-05-02 07:30:15.000000 tuotuo-0.0.3/setup.py
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 07:30:18.471415 tuotuo-0.0.3/src/
+-rw-r--r--   0 ericliu    (501) staff       (20)        0 2023-02-24 14:54:21.000000 tuotuo-0.0.3/src/__init__.py
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 07:30:18.461500 tuotuo-0.0.3/src/build/
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 07:30:18.471708 tuotuo-0.0.3/src/build/lib.macosx-10.14-arm64-cpython-38/
+-rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 tuotuo-0.0.3/src/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 07:30:18.473175 tuotuo-0.0.3/src/build/temp.macosx-10.14-arm64-cpython-38/
+-rw-r--r--   0 ericliu    (501) staff       (20)  1829576 2023-04-19 20:17:36.000000 tuotuo-0.0.3/src/build/temp.macosx-10.14-arm64-cpython-38/cutils.o
+-rw-r--r--   0 ericliu    (501) staff       (20)  1030110 2023-05-02 07:25:21.000000 tuotuo-0.0.3/src/cutils.c
+-rwxr-xr-x   0 ericliu    (501) staff       (20)   489176 2023-04-19 20:17:36.000000 tuotuo-0.0.3/src/cutils.cpython-38-darwin.so
+-rw-r--r--   0 ericliu    (501) staff       (20)     2477 2023-04-19 20:11:37.000000 tuotuo-0.0.3/src/cutils.pyx
+-rw-r--r--   0 ericliu    (501) staff       (20)     9448 2023-04-28 13:26:46.000000 tuotuo-0.0.3/src/generator.py
+-rw-r--r--   0 ericliu    (501) staff       (20)    16219 2023-04-29 19:54:15.000000 tuotuo-0.0.3/src/lda_model.py
+-rw-r--r--   0 ericliu    (501) staff       (20)     5422 2023-04-29 19:52:57.000000 tuotuo-0.0.3/src/text_pre_processor.py
+-rw-r--r--   0 ericliu    (501) staff       (20)     9789 2023-05-01 20:58:36.000000 tuotuo-0.0.3/src/utils.py
+drwxr-xr-x   0 ericliu    (501) staff       (20)        0 2023-05-02 07:30:18.477074 tuotuo-0.0.3/tuotuo.egg-info/
+-rw-r--r--   0 ericliu    (501) staff       (20)     1513 2023-05-02 07:30:18.000000 tuotuo-0.0.3/tuotuo.egg-info/PKG-INFO
+-rw-r--r--   0 ericliu    (501) staff       (20)      687 2023-05-02 07:30:18.000000 tuotuo-0.0.3/tuotuo.egg-info/SOURCES.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)        1 2023-05-02 07:30:18.000000 tuotuo-0.0.3/tuotuo.egg-info/dependency_links.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)       28 2023-05-02 07:30:18.000000 tuotuo-0.0.3/tuotuo.egg-info/requires.txt
+-rw-r--r--   0 ericliu    (501) staff       (20)        4 2023-05-02 07:30:18.000000 tuotuo-0.0.3/tuotuo.egg-info/top_level.txt
```

### Comparing `tuotuo-0.0.2/.DS_Store` & `tuotuo-0.0.3/.DS_Store`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.2/.github/workflows/python-package.yml` & `tuotuo-0.0.3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.2/.github/workflows/python-publish.yml` & `tuotuo-0.0.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.2/.vscode/c_cpp_properties.json` & `tuotuo-0.0.3/.vscode/c_cpp_properties.json`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.2/LICENSE` & `tuotuo-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.2/PKG-INFO` & `tuotuo-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tuotuo
-Version: 0.0.2
+Version: 0.0.3
 Summary: LDA & Neura based topic modelling library
 Home-page: https://github.com/RobbenRibery/TuoTuo
-Download-URL: https://github.com/RobbenRibery/TuoTuo/archive/refs/tags/Pypi-V0.0.2.tar.gz
+Download-URL: https://github.com/RobbenRibery/TuoTuo/archive/refs/tags/Pypi-0.03.tar.gz
 Author: tuotuo Superman
 Author-email: tuotuo@HanwellSquare.BigForce.com
 License: MIT
 Keywords: Generative Topic Modelling,Latent Dirichlet Allocation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `tuotuo-0.0.2/README.md` & `tuotuo-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.2/cutils.cpython-38-darwin.so` & `tuotuo-0.0.3/cutils.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.2/notebook/main copy.ipynb` & `tuotuo-0.0.3/notebook/Our Model vs SKLearn.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9916528035466461%*

 * *Differences: {"'cells'": "{0: {'execution_count': 1, 'outputs': {0: {'name': 'stderr', 'text': "*

 * *            "['/Users/ericliu/Desktop/Latent-Dirichilet-Allocation/.venv/lib/python3.8/site-packages/tqdm/auto.py:22: "*

 * *            'TqdmWarning: IProgress not found. Please update jupyter and ipywidgets. See '*

 * *            "https://ipywidgets.readthedocs.io/en/stable/user_install.html\\n', '  from "*

 * *            ".autonotebook import tqdm as notebook_tqdm\\n']}}}, 2: {'execution_count': 2}, 3: "*

 * *            "{'execution_count […]*

```diff
@@ -1,20 +1,20 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 332,
+            "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stdout",
+                    "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "The autoreload extension is already loaded. To reload it, use:\n",
-                        "  %reload_ext autoreload\n"
+                        "/Users/ericliu/Desktop/Latent-Dirichilet-Allocation/.venv/lib/python3.8/site-packages/tqdm/auto.py:22: TqdmWarning: IProgress not found. Please update jupyter and ipywidgets. See https://ipywidgets.readthedocs.io/en/stable/user_install.html\n",
+                        "  from .autonotebook import tqdm as notebook_tqdm\n"
                     ]
                 }
             ],
             "source": [
                 "%load_ext autoreload\n",
                 "%autoreload 2\n",
                 "import sys \n",
@@ -60,95 +60,95 @@
             "metadata": {},
             "source": [
                 "# Document Generation"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 333,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
                 "gen = doc_generator(\n",
                 "    M = 100,\n",
                 "    L = 20, \n",
                 "    topic_prior = tr.tensor([1,1,1,1,1], dtype=tr.double)\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 334,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "Dirichlet(concentration: torch.Size([5]))"
                         ]
                     },
-                    "execution_count": 334,
+                    "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "gen.alpha"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 335,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "torch.Size([100, 5])"
                         ]
                     },
-                    "execution_count": 335,
+                    "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "gen.theta.shape"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 336,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [],
             "source": [
                 "#gen.theta"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 337,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [],
             "source": [
                 "docs = gen.generate_doc()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 338,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [],
             "source": [
                 "#docs_raw_dict, raw_word_2_idx, raw_idx_2_word = data_loader('ap')"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 339,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "There are 100 documents in the dataset after processing\n",
@@ -159,15 +159,15 @@
             ],
             "source": [
                 "result = process_documents(docs, sample=True)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 340,
+            "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "dict_keys(['documents', 'vocab_doc_count_dict', 'vocab_doc_count_array', 'vocab_to_idx', 'idx_to_vocab'])\n"
@@ -176,15 +176,15 @@
             ],
             "source": [
                 "print(result.keys())"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 341,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "(100, 40)\n"
@@ -205,15 +205,15 @@
                 "        doc_vocab_count[doc_idx, vocab_idx] += 1 \n",
                 "\n",
                 "print(doc_vocab_count.shape)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 342,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -229,74 +229,74 @@
                             "        text-align: right;\n",
                             "    }\n",
                             "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
-                            "      <th>concert</th>\n",
-                            "      <th>genetics</th>\n",
-                            "      <th>Technique</th>\n",
-                            "      <th>decongestant</th>\n",
-                            "      <th>bruise</th>\n",
-                            "      <th>immunology</th>\n",
-                            "      <th>infection</th>\n",
                             "      <th>appetite</th>\n",
-                            "      <th>contagious</th>\n",
-                            "      <th>content</th>\n",
-                            "      <th>...</th>\n",
                             "      <th>divorce</th>\n",
-                            "      <th>contract</th>\n",
-                            "      <th>accuse</th>\n",
-                            "      <th>form</th>\n",
-                            "      <th>fever</th>\n",
-                            "      <th>attorney</th>\n",
+                            "      <th>genetics</th>\n",
                             "      <th>court</th>\n",
+                            "      <th>infection</th>\n",
                             "      <th>bankrupt</th>\n",
+                            "      <th>game</th>\n",
+                            "      <th>evidence</th>\n",
+                            "      <th>asymmetrical</th>\n",
+                            "      <th>energy</th>\n",
+                            "      <th>...</th>\n",
+                            "      <th>astrophysics</th>\n",
                             "      <th>copyright</th>\n",
-                            "      <th>scientst</th>\n",
+                            "      <th>picture</th>\n",
+                            "      <th>electricity</th>\n",
+                            "      <th>Olympic</th>\n",
+                            "      <th>exercise</th>\n",
+                            "      <th>research</th>\n",
+                            "      <th>physical</th>\n",
+                            "      <th>contract</th>\n",
+                            "      <th>fever</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>1.0</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>2.0</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>3.0</td>\n",
                             "      <td>1.0</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>1.0</td>\n",
                             "      <td>...</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>0.0</td>\n",
                             "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>2.0</td>\n",
+                            "      <td>0.0</td>\n",
                             "      <td>...</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
@@ -306,21 +306,21 @@
                             "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>2.0</td>\n",
+                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>1.0</td>\n",
                             "      <td>...</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
@@ -328,23 +328,23 @@
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>0.0</td>\n",
+                            "      <td>2.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>2.0</td>\n",
                             "      <td>...</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
@@ -352,22 +352,22 @@
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
+                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
+                            "      <td>2.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>...</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
@@ -402,178 +402,178 @@
                             "      <td>...</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>95</th>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>1.0</td>\n",
-                            "      <td>...</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
+                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
+                            "      <td>...</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
+                            "      <td>2.0</td>\n",
+                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
+                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>96</th>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
+                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>2.0</td>\n",
                             "      <td>0.0</td>\n",
+                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>...</td>\n",
                             "      <td>0.0</td>\n",
+                            "      <td>...</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
+                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>97</th>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>1.0</td>\n",
+                            "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>...</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
+                            "      <td>2.0</td>\n",
                             "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>98</th>\n",
+                            "      <td>2.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>...</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>2.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>0.0</td>\n",
+                            "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>99</th>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>1.0</td>\n",
+                            "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>2.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
+                            "      <td>...</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>1.0</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
+                            "      <td>2.0</td>\n",
                             "      <td>0.0</td>\n",
-                            "      <td>1.0</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "<p>100 rows \u00d7 40 columns</p>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "    concert  genetics  Technique  decongestant  bruise  immunology  infection  \\\n",
-                            "0       1.0       1.0        2.0           1.0     3.0         1.0        1.0   \n",
-                            "1       1.0       0.0        0.0           0.0     0.0         0.0        0.0   \n",
-                            "2       0.0       0.0        0.0           1.0     0.0         0.0        0.0   \n",
-                            "3       0.0       0.0        1.0           0.0     0.0         0.0        0.0   \n",
-                            "4       0.0       1.0        0.0           0.0     0.0         1.0        0.0   \n",
-                            "..      ...       ...        ...           ...     ...         ...        ...   \n",
-                            "95      0.0       0.0        0.0           1.0     0.0         0.0        0.0   \n",
-                            "96      1.0       0.0        0.0           0.0     0.0         0.0        0.0   \n",
-                            "97      1.0       1.0        1.0           0.0     0.0         0.0        1.0   \n",
-                            "98      0.0       0.0        0.0           1.0     0.0         0.0        1.0   \n",
-                            "99      0.0       1.0        0.0           1.0     0.0         0.0        2.0   \n",
+                            "    appetite  divorce  genetics  court  infection  bankrupt  game  evidence  \\\n",
+                            "0        1.0      1.0       1.0    1.0        1.0       1.0   1.0       1.0   \n",
+                            "1        0.0      0.0       1.0    0.0        0.0       0.0   0.0       0.0   \n",
+                            "2        0.0      0.0       0.0    0.0        0.0       1.0   0.0       0.0   \n",
+                            "3        0.0      2.0       0.0    0.0        0.0       1.0   1.0       1.0   \n",
+                            "4        0.0      0.0       0.0    0.0        0.0       0.0   1.0       0.0   \n",
+                            "..       ...      ...       ...    ...        ...       ...   ...       ...   \n",
+                            "95       0.0      0.0       0.0    0.0        0.0       1.0   0.0       0.0   \n",
+                            "96       0.0      1.0       0.0    0.0        0.0       2.0   0.0       1.0   \n",
+                            "97       0.0      0.0       0.0    0.0        1.0       0.0   0.0       0.0   \n",
+                            "98       2.0      0.0       0.0    0.0        0.0       0.0   0.0       0.0   \n",
+                            "99       0.0      0.0       0.0    1.0        0.0       0.0   0.0       0.0   \n",
                             "\n",
-                            "    appetite  contagious  content  ...  divorce  contract  accuse  form  \\\n",
-                            "0        0.0         0.0      0.0  ...      0.0       0.0     0.0   0.0   \n",
-                            "1        1.0         1.0      2.0  ...      0.0       0.0     0.0   0.0   \n",
-                            "2        2.0         0.0      0.0  ...      0.0       0.0     0.0   0.0   \n",
-                            "3        0.0         0.0      2.0  ...      0.0       0.0     0.0   0.0   \n",
-                            "4        0.0         0.0      0.0  ...      0.0       0.0     0.0   0.0   \n",
-                            "..       ...         ...      ...  ...      ...       ...     ...   ...   \n",
-                            "95       0.0         0.0      1.0  ...      0.0       0.0     0.0   0.0   \n",
-                            "96       2.0         0.0      0.0  ...      0.0       0.0     0.0   0.0   \n",
-                            "97       0.0         0.0      0.0  ...      0.0       0.0     0.0   0.0   \n",
-                            "98       1.0         0.0      0.0  ...      0.0       1.0     0.0   1.0   \n",
-                            "99       0.0         0.0      0.0  ...      1.0       0.0     0.0   1.0   \n",
+                            "    asymmetrical  energy  ...  astrophysics  copyright  picture  electricity  \\\n",
+                            "0            1.0     1.0  ...           0.0        0.0      0.0          0.0   \n",
+                            "1            0.0     0.0  ...           0.0        0.0      0.0          0.0   \n",
+                            "2            1.0     1.0  ...           0.0        0.0      0.0          0.0   \n",
+                            "3            0.0     0.0  ...           0.0        0.0      0.0          0.0   \n",
+                            "4            2.0     0.0  ...           0.0        0.0      0.0          0.0   \n",
+                            "..           ...     ...  ...           ...        ...      ...          ...   \n",
+                            "95           1.0     0.0  ...           0.0        0.0      2.0          1.0   \n",
+                            "96           0.0     0.0  ...           0.0        0.0      0.0          0.0   \n",
+                            "97           0.0     0.0  ...           1.0        0.0      0.0          0.0   \n",
+                            "98           0.0     0.0  ...           0.0        0.0      0.0          0.0   \n",
+                            "99           0.0     0.0  ...           0.0        0.0      0.0          1.0   \n",
                             "\n",
-                            "    fever  attorney  court  bankrupt  copyright  scientst  \n",
-                            "0     0.0       0.0    0.0       0.0        0.0       0.0  \n",
-                            "1     0.0       0.0    0.0       0.0        0.0       0.0  \n",
-                            "2     0.0       0.0    0.0       0.0        0.0       0.0  \n",
-                            "3     0.0       0.0    0.0       0.0        0.0       0.0  \n",
-                            "4     0.0       0.0    0.0       0.0        0.0       0.0  \n",
-                            "..    ...       ...    ...       ...        ...       ...  \n",
-                            "95    0.0       0.0    0.0       0.0        0.0       0.0  \n",
-                            "96    0.0       0.0    0.0       0.0        0.0       0.0  \n",
-                            "97    0.0       1.0    0.0       0.0        1.0       0.0  \n",
-                            "98    0.0       0.0    2.0       0.0        1.0       0.0  \n",
-                            "99    0.0       0.0    0.0       0.0        0.0       1.0  \n",
+                            "    Olympic  exercise  research  physical  contract  fever  \n",
+                            "0       0.0       0.0       0.0       0.0       0.0    0.0  \n",
+                            "1       0.0       0.0       0.0       0.0       0.0    0.0  \n",
+                            "2       0.0       0.0       0.0       0.0       0.0    0.0  \n",
+                            "3       0.0       0.0       0.0       0.0       0.0    0.0  \n",
+                            "4       0.0       0.0       0.0       0.0       0.0    0.0  \n",
+                            "..      ...       ...       ...       ...       ...    ...  \n",
+                            "95      0.0       0.0       0.0       0.0       1.0    0.0  \n",
+                            "96      0.0       0.0       0.0       0.0       1.0    0.0  \n",
+                            "97      0.0       2.0       1.0       0.0       0.0    0.0  \n",
+                            "98      0.0       0.0       0.0       0.0       1.0    0.0  \n",
+                            "99      1.0       1.0       0.0       0.0       2.0    0.0  \n",
                             "\n",
                             "[100 rows x 40 columns]"
                         ]
                     },
-                    "execution_count": 342,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "doc_vocab_count_df = pd.DataFrame(\n",
                 "    data = doc_vocab_count,\n",
@@ -588,15 +588,15 @@
             "metadata": {},
             "source": [
                 "# Our Model"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 343,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Topic Dirichlet Prior, Alpha\n",
@@ -608,31 +608,31 @@
                         "Var Inf - Word Dirichlet prior, Lambda\n",
                         "(5, 40)\n",
                         "\n",
                         "Var Inf - Topic Dirichlet prior, Gamma\n",
                         "(100, 5)\n",
                         "\n",
                         "Size of the vocab is 40\n",
-                        "Init perplexity = 98.20369822191614\n",
-                        "End perplexity = 51.75462762223653\n"
+                        "Init perplexity = 98.31667858811902\n",
+                        "End perplexity = 52.72568050990828\n"
                     ]
                 },
                 {
                     "data": {
                         "text/plain": [
-                            "[<matplotlib.lines.Line2D at 0x13aaa3b80>]"
+                            "[<matplotlib.lines.Line2D at 0x2af3b0910>]"
                         ]
                     },
-                    "execution_count": 343,
+                    "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 },
                 {
                     "data": {
-                        "image/png": "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XXedbrvtNuXn5ys3N1c33XSTSktLO/QET21trSRxmwcAgC6otrZWXq834TlJDyi7d+/WtGnTdODAAfXt21cTJkzQ2rVr1bdvX0nSL3/5SzmdTk2ZMkUNDQ2aOHGifv3rX3fodxQVFamqqkq9evWSw+FIav2h/paqqipuJXUixjk1GOfUYJxTg3FOnc4aa2OMamtrVVRUdMJzHeZk5llOI4FAQF6vV36/n/8H6ESMc2owzqnBOKcG45w66TDWfBcPAABIOwQUAACQdggoUTwej+655x55PB7bpXRrjHNqMM6pwTinBuOcOukw1vSgAACAtMMMCgAASDsEFAAAkHYIKAAAIO0QUAAAQNohoER4/PHHNXjwYGVlZWncuHFat26d7ZK6tAULFuiLX/yievXqpX79+mny5MnasmVLu3Pq6+s1a9Ys9enTRzk5OZoyZYpqamosVdw9PPjgg3I4HJo9e3Z4H+OcHHv27NG3vvUt9enTR9nZ2TrnnHP01ltvhY8bY3T33Xerf//+ys7OVllZmbZt22ax4q6ppaVF8+bNU0lJibKzszV06FDdd9997b6/hbHuuL/97W+66qqrVFRUJIfDoWXLlrU7fjJjevDgQU2fPl25ubnKy8vTddddp8OHD3dOwQbGGGOef/55k5mZaX7729+a9957z1x//fUmLy/P1NTU2C6ty5o4caJZsmSJ2bx5s3nnnXfM1772NVNcXGwOHz4cPuf73/++GThwoCkvLzdvvfWWufDCC81FF11ksequbd26dWbw4MHm3HPPNbfcckt4P+P82R08eNAMGjTIfOc73zGVlZVmx44d5vXXXzfbt28Pn/Pggw8ar9drli1bZjZt2mS+/vWvm5KSEnP06FGLlXc98+fPN3369DGvvvqq2blzp3nxxRdNTk6OefTRR8PnMNYd9+c//9ncdddd5qWXXjKSzMsvv9zu+MmM6eWXX27OO+88s3btWvPmm2+aYcOGmWnTpnVKvQSUYy644AIza9as8PuWlhZTVFRkFixYYLGq7mX//v1Gklm9erUxxhifz2cyMjLMiy++GD7ngw8+MJJMRUWFrTK7rNraWjN8+HCzcuVKc/HFF4cDCuOcHD/60Y/MhAkT4h4PBoOmsLDQ/PznPw/v8/l8xuPxmN///vepKLHbuPLKK821117bbt/VV19tpk+fboxhrJMhOqCczJi+//77RpJZv359+JzXXnvNOBwOs2fPnqTXyC0eSY2NjdqwYYPKysrC+5xOp8rKylRRUWGxsu7F7/dLkvLz8yVJGzZsUFNTU7txHzFihIqLixn3UzBr1ixdeeWV7cZTYpyT5ZVXXtHYsWP1zW9+U/369dOYMWP0xBNPhI/v3LlT1dXV7cbZ6/Vq3LhxjHMHXXTRRSovL9fWrVslSZs2bdKaNWt0xRVXSGKsO8PJjGlFRYXy8vI0duzY8DllZWVyOp2qrKxMek1J/zbjrujTTz9VS0uLCgoK2u0vKCjQhx9+aKmq7iUYDGr27NkaP368zj77bElSdXW1MjMzlZeX1+7cgoICVVdXW6iy63r++ef19ttva/369ccdY5yTY8eOHVq0aJFuu+02/ed//qfWr1+vm2++WZmZmZoxY0Z4LGP9d4Rx7pg5c+YoEAhoxIgRcrlcamlp0fz58zV9+nRJYqw7wcmMaXV1tfr169fuuNvtVn5+fqeMOwEFKTFr1ixt3rxZa9assV1Kt1NVVaVbbrlFK1euVFZWlu1yuq1gMKixY8fqgQcekCSNGTNGmzdv1uLFizVjxgzL1XUvL7zwgp599lk999xzGjVqlN555x3Nnj1bRUVFjPVphFs8ks444wy5XK7jnmqoqalRYWGhpaq6jxtvvFGvvvqq/vKXv+hzn/tceH9hYaEaGxvl8/nanc+4d8yGDRu0f/9+feELX5Db7Zbb7dbq1au1cOFCud1uFRQUMM5J0L9/f5111lnt9o0cOVK7du2SpPBY8t+Rz+6OO+7QnDlzNHXqVJ1zzjm65pprdOutt2rBggWSGOvOcDJjWlhYqP3797c73tzcrIMHD3bKuBNQJGVmZur8889XeXl5eF8wGFR5eblKS0stVta1GWN044036uWXX9aqVatUUlLS7vj555+vjIyMduO+ZcsW7dq1i3HvgEsvvVTvvvuu3nnnnfA2duxYTZ8+Pfwz4/zZjR8//rjH5Ldu3apBgwZJkkpKSlRYWNhunAOBgCorKxnnDqqrq5PT2f7Pk8vlUjAYlMRYd4aTGdPS0lL5fD5t2LAhfM6qVasUDAY1bty45BeV9LbbLur55583Ho/HLF261Lz//vtm5syZJi8vz1RXV9surcv6wQ9+YLxer/nrX/9q9u3bF97q6urC53z/+983xcXFZtWqVeatt94ypaWlprS01GLV3UPkUzzGMM7JsG7dOuN2u838+fPNtm3bzLPPPmt69OhhnnnmmfA5Dz74oMnLyzN/+tOfzD//+U8zadIkHn09BTNmzDADBgwIP2b80ksvmTPOOMPceeed4XMY646rra01GzduNBs3bjSSzMMPP2w2btxoPv74Y2PMyY3p5ZdfbsaMGWMqKyvNmjVrzPDhw3nMOBUee+wxU1xcbDIzM80FF1xg1q5da7ukLk1SzG3JkiXhc44ePWpuuOEG07t3b9OjRw/zjW98w+zbt89e0d1EdEBhnJNj+fLl5uyzzzYej8eMGDHC/OY3v2l3PBgMmnnz5pmCggLj8XjMpZdearZs2WKp2q4rEAiYW265xRQXF5usrCwzZMgQc9ddd5mGhobwOYx1x/3lL3+J+d/kGTNmGGNObkwPHDhgpk2bZnJyckxubq757ne/a2prazulXocxEUvzAQAApAF6UAAAQNohoAAAgLRDQAEAAGmHgAIAANIOAQUAAKQdAgoAAEg7BBQAAJB2CCgAACDtEFAAAEDaIaAAAIC0Q0ABAABph4ACAADSzv8HMZgsAqugq1QAAAAASUVORK5CYII=",
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAigAAAGeCAYAAAC+dvpwAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjcuMCwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy88F64QAAAACXBIWXMAAA9hAAAPYQGoP6dpAAAub0lEQVR4nO3de3jU1b3v8c9cksmFZAIBJgQTiECL91KpMcCup9s84qUWK489WNqiWG/FKtp6YbfY7q0UtX26W9xeqsciVdHWo7LVXfVYtFRqDIiXiiKXghCBBLkkExLIZWadP5KZzAwzA8HJrEl4v57n92Ty+/3ml5WlNZ+u+a61HMYYIwAAgAzitN0AAACAWAQUAACQcQgoAAAg4xBQAABAxiGgAACAjENAAQAAGYeAAgAAMg4BBQAAZBwCCgAAyDhu2w04GsFgUDt27FBBQYEcDoft5gAAgCNgjFFzc7NKS0vldB5mjMT00ooVK8zXv/51M2LECCPJPPfcc1HXg8GgmT9/vikpKTE5OTnm7LPPNhs2bIi6Z8+ePebb3/62KSgoMF6v18yePds0NzcfcRvq6uqMJA4ODg4ODo5+eNTV1R32b32vR1BaWlp02mmnafbs2br44osPuX7PPfdo0aJFWrJkiSoqKjR//nxNnTpVH330kXJyciRJM2fO1M6dO/Xqq6+qo6NDl19+ua666iotXbr0iNpQUFAgSaqrq1NhYWFvfwUAAGCB3+9XWVlZ+O94Mg5jjn6zQIfDoeeee04XXXSRJMkYo9LSUv3oRz/Sj3/8Y0lSU1OTfD6fHn30Uc2YMUPr1q3TiSeeqNWrV2vixImSpJdfflnnn3++Pv30U5WWlh7RL+j1etXU1ERAAQCgn+jN3++UFslu2bJF9fX1qq6uDp/zer2qrKxUTU2NJKmmpkZFRUXhcCJJ1dXVcjqdqq2tjfvctrY2+f3+qAMAAAxcKQ0o9fX1kiSfzxd13ufzha/V19dr+PDhUdfdbreGDBkSvifWwoUL5fV6w0dZWVkqmw0AADJMv5hmPG/ePDU1NYWPuro6200CAAB9KKUBpaSkRJLU0NAQdb6hoSF8raSkRLt27Yq63tnZqb1794bvieXxeFRYWBh1AACAgSulAaWiokIlJSVavnx5+Jzf71dtba2qqqokSVVVVWpsbNSaNWvC97z22msKBoOqrKxMZXMAAEA/1etpxvv379emTZvC32/ZskXvvfeehgwZovLycs2dO1d33nmnxo0bF55mXFpaGp7pc8IJJ+jcc8/VlVdeqQcffFAdHR267rrrNGPGjCOawQMAAAa+XgeUt99+W1/72tfC3990002SpFmzZunRRx/VLbfcopaWFl111VVqbGzUlClT9PLLL4fXQJGkJ554Qtddd53OPvtsOZ1OTZ8+XYsWLUrBrwMAAAaCz7UOii2sgwIAQP9jbR0UAACAVCCgAACAjENAAQAAGYeAAgAAMk6vZ/EMZGu27tUL7+/U+JICzTij3HZzAAA4ZjGCEmF9/X49+uYneu3jXYe/GQAA9BkCSgS30yFJCgT73cxrAAAGFAJKBFd3QOkkoAAAYBUBJYLbFQooQcstAQDg2EZAieB2dnVHZ4ARFAAAbCKgRHBRgwIAQEYgoERwU4MCAEBGIKBEcLkYQQEAIBMQUCKERlA6AhTJAgBgEwElAjUoAABkBgJKhCxXV3cQUAAAsIuAEoGF2gAAyAwElAgsdQ8AQGYgoERwUSQLAEBGIKBECK0kywgKAAB2EVAi9OzFQ0ABAMAmAkoEalAAAMgMBJQIPbN4qEEBAMAmAkoEalAAAMgMBJQIPbN4jIwhpAAAYAsBJUJWd5GsJDGIAgCAPQSUCKERFIk6FAAAbCKgRAjVoEjUoQAAYBMBJUL0CAoBBQAAWwgoEdyRASVAQAEAwBYCSgSn0yFHd0ahBgUAAHsIKDGyWAsFAADrCCgxwqvJ8hEPAADWEFBisB8PAAD2EVBiuFzsxwMAgG0ElBju8IaBjKAAAGALASVGaLE2alAAALCHgBLDRQ0KAADWEVBiuF18xAMAgG0ElBiMoAAAYB8BJUa4SDbALB4AAGwhoMQIF8kyggIAgDUElBihGhQ+4gEAwB4CSgwX66AAAGAdASVGz1L31KAAAGALASVGaASlg4XaAACwhoASI1QkSw0KAAD2EFBisFAbAAD2EVBiUIMCAIB9BJQYzOIBAMA+AkoMdjMGAMA+AkoMRlAAALCPgBKjZyVZalAAALCFgBLDzQgKAADWEVBiuELroFCDAgCANQSUGIygAABgHwElRk+RLDUoAADYQkCJwQgKAAD2EVBiuF3UoAAAYBsBJQYjKAAA2EdAieEK78VDQAEAwBYCSgw3RbIAAFhHQInh6l5Jlr14AACwp08CSnNzs+bOnatRo0YpNzdXkyZN0urVq8PXjTG6/fbbNWLECOXm5qq6ulobN27si6b0WlZooTY+4gEAwJo+CSjf//739eqrr+qxxx7TBx98oHPOOUfV1dXavn27JOmee+7RokWL9OCDD6q2tlb5+fmaOnWqDh482BfN6RU2CwQAwL6UB5QDBw7omWee0T333KOvfvWrGjt2rH7+859r7NixeuCBB2SM0W9+8xv99Kc/1bRp03TqqafqD3/4g3bs2KFly5alujm91rNZIAEFAABbUh5QOjs7FQgElJOTE3U+NzdXK1eu1JYtW1RfX6/q6urwNa/Xq8rKStXU1MR9Zltbm/x+f9TRV1hJFgAA+1IeUAoKClRVVaU77rhDO3bsUCAQ0OOPP66amhrt3LlT9fX1kiSfzxf1Pp/PF74Wa+HChfJ6veGjrKws1c0OC8/ioUgWAABr+qQG5bHHHpMxRiNHjpTH49GiRYt06aWXyuk8uh83b948NTU1hY+6uroUt7iHu7uN1KAAAGBPnwSUMWPGaMWKFdq/f7/q6uq0atUqdXR06Pjjj1dJSYkkqaGhIeo9DQ0N4WuxPB6PCgsLo46+Qg0KAAD29ek6KPn5+RoxYoT27dunV155RdOmTVNFRYVKSkq0fPny8H1+v1+1tbWqqqrqy+YcEWpQAACwz90XD33llVdkjNEXv/hFbdq0STfffLPGjx+vyy+/XA6HQ3PnztWdd96pcePGqaKiQvPnz1dpaakuuuiivmhOr7hZ6h4AAOv6JKA0NTVp3rx5+vTTTzVkyBBNnz5dCxYsUFZWliTplltuUUtLi6666io1NjZqypQpevnllw+Z+WODq7sGpYMiWQAArHEYY/rdX2K/3y+v16umpqaU16O8/vEuXf7oap0y0qsXfjglpc8GAOBY1pu/3+zFEyNUJMssHgAA7CGgxHCFa1AokgUAwBYCSgzWQQEAwD4CSgwXK8kCAGAdASUG04wBALCPgBKjp0iWGhQAAGwhoMQI1aAwggIAgD0ElBg9S90TUAAAsIWAEiNcg0KRLAAA1hBQYoRGUDqoQQEAwBoCSowsFzUoAADYRkCJQQ0KAAD2EVBihGpQjJGChBQAAKwgoMRwda+DIjGKAgCALQSUGKERFInF2gAAsIWAEsPlZAQFAADbCCgxspw9XcJaKAAA2EFAieF0OuToHkRhBAUAADsIKHGwozEAAHYRUOIIryYboEgWAAAbCChxsKMxAAB2EVDicLtYTRYAAJsIKHFQgwIAgF0ElDh69uOhBgUAABsIKHFQgwIAgF0ElDh6ZvEQUAAAsIGAEkeoSJYRFAAA7CCgxOGmBgUAAKsIKHG4qEEBAMAqAkocPSMoBBQAAGwgoMQRnmZMkSwAAFYQUOLoWaiNGhQAAGwgoMTBUvcAANhFQImDhdoAALCLgBIHNSgAANhFQImDdVAAALCLgBKHi2nGAABYRUCJI8tFDQoAADYRUOKgBgUAALsIKHH0rINCQAEAwAYCShzUoAAAYBcBJY7wQm0BZvEAAGADASUORlAAALCLgBIHK8kCAGAXASUONyMoAABYRUCJw+ViN2MAAGwioMQRGkHpYB0UAACsIKDE4aIGBQAAqwgocWRRgwIAgFUElDioQQEAwC4CShzM4gEAwC4CShyhGhQ2CwQAwA4CShxsFggAgF0ElDjCe/FQgwIAgBUElDgYQQEAwC4CShzhGhQCCgAAVhBQ4mAEBQAAuwgocbjCS91TgwIAgA0ElDgYQQEAwC4CShxuFzUoAADYRECJgxEUAADsIqDEEapBYSVZAADsSHlACQQCmj9/vioqKpSbm6sxY8bojjvukDE9f+yNMbr99ts1YsQI5ebmqrq6Whs3bkx1U45az148FMkCAGBDygPK3XffrQceeED/9V//pXXr1unuu+/WPffco3vvvTd8zz333KNFixbpwQcfVG1trfLz8zV16lQdPHgw1c05Ki42CwQAwCp3qh/45ptvatq0abrgggskSaNHj9aTTz6pVatWSeoaPfnNb36jn/70p5o2bZok6Q9/+IN8Pp+WLVumGTNmpLpJvRYqkqUGBQAAO1I+gjJp0iQtX75cGzZskCS9//77Wrlypc477zxJ0pYtW1RfX6/q6urwe7xeryorK1VTUxP3mW1tbfL7/VFHX3JTgwIAgFUpH0G57bbb5Pf7NX78eLlcLgUCAS1YsEAzZ86UJNXX10uSfD5f1Pt8Pl/4WqyFCxfq3//931Pd1IRczOIBAMCqlI+g/OlPf9ITTzyhpUuX6p133tGSJUv0q1/9SkuWLDnqZ86bN09NTU3ho66uLoUtPlTPbsYEFAAAbEj5CMrNN9+s2267LVxLcsopp2jr1q1auHChZs2apZKSEklSQ0ODRowYEX5fQ0ODvvSlL8V9psfjkcfjSXVTE2IWDwAAdqV8BKW1tVVOZ/RjXS6Xgt1/7CsqKlRSUqLly5eHr/v9ftXW1qqqqirVzTkq7u72B6hBAQDAipSPoFx44YVasGCBysvLddJJJ+ndd9/Vr3/9a82ePVuS5HA4NHfuXN15550aN26cKioqNH/+fJWWluqiiy5KdXOOCtOMAQCwK+UB5d5779X8+fP1gx/8QLt27VJpaamuvvpq3X777eF7brnlFrW0tOiqq65SY2OjpkyZopdfflk5OTmpbs5RCdWgUCQLAIAdDhO5xGs/4ff75fV61dTUpMLCwpQ/f1fzQZ2xYLmcDmnzwgtS/nwAAI5Fvfn7zV48cYRqUIJGCjKKAgBA2hFQ4gjVoEjUoQAAYAMBJY4sV09AoQ4FAID0I6DEET2CwlooAACkGwElDnfEOi6MoAAAkH4ElDgiBlDUwWJtAACkHQElDofDEV7unhEUAADSj4CSQM+GgdSgAACQbgSUBML78TCCAgBA2hFQEmA/HgAA7CGgJEANCgAA9hBQEgiNoHQEqEEBACDdCCgJZLmoQQEAwBYCSgLUoAAAYA8BJQFqUAAAsIeAkkB4BIWVZAEASDsCSgI9H/FQJAsAQLoRUBLoWUmWERQAANKNgJJAeCVZPuIBACDtCCgJuJnFAwCANQSUBFzM4gEAwBoCSgLsZgwAgD0ElARc3TUoTDMGACD9CCgJZPERDwAA1hBQEmCpewAA7CGgJBCqQQlQgwIAQNoRUBII16AwggIAQNoRUBJwsxcPAADWEFASoAYFAAB7CCgJZFGDAgCANQSUBBhBAQDAHgJKAuHNAgkoAACkHQElgdAISgdFsgAApB0BJQG3kxoUAABsIaAk0LNZICMoAACkGwElARc1KAAAWENAScDNLB4AAKwhoCQQnmYcoAYFAIB0I6AkwAgKAAD2EFAScLuoQQEAwBYCSgKMoAAAYA8BJYFQDUqAhdoAAEg7AkoCjKAAAGAPASWBns0CmcUDAEC6EVASCK0kS5EsAADpR0BJILSbcSc1KAAApB0BJYGezQIJKAAApBsBJQFqUAAAsIeAkgC7GQMAYA8BJQEXNSgAAFhDQEkgixoUAACsIaAkQA0KAAD2EFASYB0UAADsIaAkEK5BIaAAAJB2BJQEwnvxUCQLAEDaEVASYJoxAAD2EFAS6FlJliJZAADSjYCSADUoAADYQ0BJgL14AACwh4CSgIsiWQAArCGgJOBmoTYAAKwhoCTgdnV1TdBIQT7mAQAgrQgoCYQ+4pGkgCGgAACQTikPKKNHj5bD4TjkmDNnjiTp4MGDmjNnjoqLizVo0CBNnz5dDQ0NqW7G5+aODCiMoAAAkFYpDyirV6/Wzp07w8err74qSbrkkkskSTfeeKNeeOEFPf3001qxYoV27Nihiy++ONXN+NwiR1A6AtShAACQTu5UP3DYsGFR3991110aM2aMzjrrLDU1NemRRx7R0qVL9a//+q+SpMWLF+uEE07QW2+9pTPPPDPVzTlqjKAAAGBPn9agtLe36/HHH9fs2bPlcDi0Zs0adXR0qLq6OnzP+PHjVV5erpqamoTPaWtrk9/vjzr6WuQICou1AQCQXn0aUJYtW6bGxkZddtllkqT6+nplZ2erqKgo6j6fz6f6+vqEz1m4cKG8Xm/4KCsr68NWd3E4HCzWBgCAJX0aUB555BGdd955Ki0t/VzPmTdvnpqamsJHXV1dilqYXHixNgIKAABplfIalJCtW7fqL3/5i5599tnwuZKSErW3t6uxsTFqFKWhoUElJSUJn+XxeOTxePqqqQm5nQ61SQqwmiwAAGnVZyMoixcv1vDhw3XBBReEz51++unKysrS8uXLw+fWr1+vbdu2qaqqqq+actRCIygdrCYLAEBa9ckISjAY1OLFizVr1iy53T0/wuv16oorrtBNN92kIUOGqLCwUD/84Q9VVVWVUTN4QrK6V5OlBgUAgPTqk4Dyl7/8Rdu2bdPs2bMPufaf//mfcjqdmj59utra2jR16lTdf//9fdGMz40NAwEAsKNPAso555wjk2B5+JycHN1333267777+uJHpxSzeAAAsIO9eJJwudjRGAAAGwgoSbidXd3DNGMAANKLgJIENSgAANhBQEmCGhQAAOwgoCThpgYFAAArCChJuJysgwIAgA0ElCRCH/F0UIMCAEBaEVCScFGDAgCAFQSUJLKoQQEAwAoCShLUoAAAYAcBJYlQDQoLtQEAkF4ElCSoQQEAwA4CShLhEZQANSgAAKQTASUJt4u9eAAAsIGAkgRL3QMAYAcBJQkXRbIAAFhBQEmCERQAAOwgoCThCi91T5EsAADpREBJghEUAADsIKAkwSweAADsIKAkwQgKAAB2EFCSCM/iCRBQAABIJwJKEj178VAkCwBAOhFQkgjtZkwNCgAA6UVAScLt6q5B4SMeAADSioCShJuVZAEAsIKAkoQrPIuHGhQAANKJgJIEIygAANhBQEnCFVqojRoUAADSioCSBCMoAADYQUBJwk0NCgAAVhBQkghNM2YEBQCA9CKgJBFaqI29eAAASC8CShJu9uIBAMAKAkoSLvbiAQDACgJKElmhpe75iAcAgLQioCTBZoEAANhBQEmiZ5oxAQUAgHQioCThYqE2AACsIKAk0TOLhyJZAADSiYCShNtFDQoAADYQUJKgBgUAADsIKElQgwIAgB0ElCQYQQEAwA4CShKhEZQOimQBAEgrAkoSbjYLBADACgJKEm4XNSgAANhAQEmCGhQAAOwgoCThiggoxhBSAABIFwJKEqEaFImPeQAASCcCShKu7hoUiY95AABIJwJKEqEaFIkRFAAA0omAkkRkQAkECCgAAKQLASUJV9QICou1AQCQLgSUJBwOR9RMHgAAkB4ElMMIL3dPQAEAIG0IKIeRFRpBoQYFAIC0IaAcRmgEhRoUAADSh4ByGG4XGwYCAJBubtsNyHShEZRv/a5GQ/KzNTgvW0V52SrKy5I3N0tFuVny5mWpKC9bQ/OzVTzIo6GDuu6JnAUEAACOHAHlMCorhujFf+zUvtYO7WvtkNRyRO9zOqSSwhwdNzhPxw3O1XGDc1VenK/xJQUaO3yQcrJcfdtwAAD6MYfph7vg+f1+eb1eNTU1qbCwsE9/ljFGDf427Wtt177WdjV1B5XGA+1qOtChptYONR3o0J6Wdu1tadee/W3dQSYxl9OhMcPyNb6kUKePGqzJY4s1ZtggORyMuAAABq7e/P0moPSBjkBQe/a3a0fTAX2674A+3deqT/cd0ObP9uvj+mY1xgkwvkKPJo8Zqq9+YZjOOcmnvGwGtwAAA4v1gLJ9+3bdeuuteumll9Ta2qqxY8dq8eLFmjhxoqSuUYmf/exnevjhh9XY2KjJkyfrgQce0Lhx447o+ZkeUJIJjcis2+nX2u1NemvLHq3+ZJ/aO3tmCeVnu3TBqSN0ycQyTRw1mJEVAMCAYDWg7Nu3TxMmTNDXvvY1XXvttRo2bJg2btyoMWPGaMyYMZKku+++WwsXLtSSJUtUUVGh+fPn64MPPtBHH32knJycw/6M/hxQ4jnYEdCarfv0xsbdemntTm3d0xq+VjE0X5dPHq0ZXylXtptJVwCA/stqQLntttv097//XW+88Ubc68YYlZaW6kc/+pF+/OMfS5Kamprk8/n06KOPasaMGYf9GQMtoEQyxmjVlr16es2n+vMHO9XaHpAklQ/J04/O+YIuPLVUTmYHAQD6od78/U75/yV//vnnNXHiRF1yySUaPny4JkyYoIcffjh8fcuWLaqvr1d1dXX4nNfrVWVlpWpqauI+s62tTX6/P+oYqBwOhyqPL9avLjlNq39Srf+YdpKGDvJo295W3fDUe7rg3pX66/pdtpsJAECfSnlA2bx5c7ie5JVXXtG1116r66+/XkuWLJEk1dfXS5J8Pl/U+3w+X/harIULF8rr9YaPsrKyVDc7I+V73Ppe1Wj97Zb/pZunflEFHrfW7fTrssWrdcv/fV+t7Z22mwgAQJ9I+Uc82dnZmjhxot58883wueuvv16rV69WTU2N3nzzTU2ePFk7duzQiBEjwvd861vfksPh0B//+MdDntnW1qa2trbw936/X2VlZQPyI55k9rW0697XNmnxm1tkjHT80HwtunSCTh7ptd00AAAOy+pHPCNGjNCJJ54Yde6EE07Qtm3bJEklJSWSpIaGhqh7GhoawtdieTweFRYWRh3HosH52br9whP15JVnaoQ3R5t3t+ib9/9d/+eNzQqyFD8AYABJeUCZPHmy1q9fH3Vuw4YNGjVqlCSpoqJCJSUlWr58efi63+9XbW2tqqqqUt2cAenM44v10g3/oqkn+dQRMLrzf9bpmsfX6GBHwHbTAABIiZQHlBtvvFFvvfWWfvGLX2jTpk1aunSpHnroIc2ZM0dSVxHo3Llzdeedd+r555/XBx98oO9973sqLS3VRRddlOrmDFhFedl68Duna8E3T1a226n/91GDZv1+lfwHk69iCwBAf9AnC7W9+OKLmjdvnjZu3KiKigrddNNNuvLKK8PXQwu1PfTQQ2psbNSUKVN0//336wtf+MIRPX8gTzM+Gm9t3qMrl7yt5rZOnTiiUEtmn6FhBR7bzQIAIIr1lWT7GgHlUGu3N+myxau0e3+7Rhfn6bErKlU2JM92swAACLNaJAs7Th7p1dPXTNJxg3P1yZ5WTX/gTW3+bL/tZgEAcFQIKANIxdB8PXPtJH3RV6BdzW367iOrtKPxgO1mAQDQawSUAcZXmKMnrqzU8UPztb3xgL7zSK327G87/BsBAMggBJQBaOggjx77fqVKvTna/FmLZi1mdg8AoH8hoAxQI4ty9dj3K1Wcn6212/36/pK3WScFANBvEFAGsDHDBmnJ7DNU4HFr1Za9um7pO+oMBG03CwCAwyKgDHAnj/Tqkcu+Io/bqb+s26Xbn/9Q/XBmOQDgGENAOQacUTFEv50xQQ6HtLR2m+7/6z9tNwkAgKQIKMeIc08u0c8vPEmS9MtX1uuZNZ9abhEAAIkRUI4hsyaN1tVnHS9JuvWZf+iNjZ9ZbhEAAPERUI4xt04dr2+cVqrOoNG1j7+jtdubbDcJAIBDEFCOMU6nQ7+85FRNGlOs/W2dmvX7VfonS+IDADIMAeUY5HG79Lvvnq5TRnq1p6Vd3/0/tSyJDwDIKASUY1RBTpYevfwrOn5YvnY0HWRJfABARiGgHMOKB3n0+BXRS+I3syQ+ACADEFCOcaUxS+Jfvng1+/YAAKwjoKBnSfwct97euk8zH67V3pZ2280CABzDCCiQ1LUk/lNXnani/Gx9sL1J//t3NdrlP2i7WQCAYxQBBWEnlXr1x6ur5Cv0aOOu/brkdzX6dF+r7WYBAI5BBBREGTt8kJ6+epLKhuRq655WXfJgjdbt9NtuFgDgGENAwSHKi/P09NWTNGZYvnY2HdTF97+p//nHTtvNAgAcQwgoiKvEm6Nnrp2kfxk3VAc6Apqz9B3d/fLHCgSN7aYBAI4BBBQkVJSXrcWXfUVXf7Vrg8EH/vpPzX50tZpamYYMAOhbBBQk5XY5Ne/8E/TbGV9STpZTKzZ8pvMXvaGVG3fbbhoAYAAjoOCITPvSSD1z7SSVD8nT9sYD+s4jtfrpsg/U0tZpu2kAgAGIgIIjdlKpVy/d8C/6XtUoSdLjb23T1N/8TW/+k9EUAEBqEVDQK/ket/5j2sla+v1KjSzK1af7DujbD9fqh0++q7q9rJkCAEgNAgqOyqSxQ/XKjV/VzMpyORzSC+/v0Nm/XqGFL61T0wGKaAEAn4/DGNPv5o36/X55vV41NTWpsLDQdnOOeR/uaNKC/1mnN/+5R5I0OC9Lc742VjPOKNcgj9ty6wAAmaI3f78JKEgJY4xeX79Lv/jzx9q0a78kqTDHre9WjdKsSaM1vCDHcgsBALYRUGBNZyCoZ975VL/722Zt/qxFkpTtdmr6l0fq22eM0skjC+VwOCy3EgBgAwEF1gWDRq+ua9CDK/6pd7c1hs+PLynQtyaW6aIJIzUkP9teAwEAaUdAQcYwxmj1J/v0+Ftb9fKH9WrvDEqSslwOnfWF4Zp6kk/VJ/g0mLACAAMeAQUZqam1Q8+/v11/evtTfbC9KXze5XSosmKIzjnRp69+YZgqhubzMRAADEAEFGS89fXNemntTr28tl4f1zdHXSv15mjy2KGaMm6ozjy+WL5CCmwBYCAgoKBf2bqnRa98WK/l63bp3W2Nag8Eo66PLMrVl0cN1pfLi/Tl8sH6YkmBcrJclloLADhaBBT0W63tnVr9yT69uWm3Vm7arXU7/QrG/Bvqdjo0dvggnVTq1UmlhRo/okBf9BWoeJDHTqMBAEeEgIIBY39bp/5R16g1W/fpnW379F5do/a1xl+ptjg/W+N8gzRueIHGDMvX8cMG6fhh+Sr15srppKYFAGwjoGDAMsZoZ9NBfbjDr7Xbm/ThDr82NDRrW5J9gHKynBpdnK/RxfmqGJaviuJ8jR6ar9HFeRpW4KEgFwDShICCY05re6c27dqvDQ37tXFXszZ/1qLNn+3Xtr2t6ggk/lc8L9ulUcX5qhiap1HF+Ro1pOvr6KF58hXkMPICAClEQAG6dQaCqtt3QFt279eW3a36ZHeLPtnToi27W7Sj8cAh9S2RPG6nyobkqWxwrsqH5KlsSJ6OG5ynkUW5Ki3K0ZD8bEZfAKAXevP3m53cMKC5XU5VDM1XxdD8Q661dwZVt69VW/e0aMvuVm3b06JP9nR9/+m+A2rrDGrTrv3hvYViedxOjSzKla8wR75Cj3yFORpemKNhBR4V52ereFC2ivM9GpyXJbeLjcMBoDcIKDhmZbudGjNskMYMG3TItc5AUDsaD6puX6u27e0+9rRqe+MB7Wg8oF3NbWrrDGrz7hZt3t1y2J9VmOPW4PxsFeVmqSgvW4W5WSrIcasgx63CnK7XedluDfK4lJftVr7Hpdwst3KzXcrN6jpysp3KdjkZtQFwTCCgAHG4XU6VF+epvDhPk+Ncb+sMqKGpTdsbD2hX80E1+A+qwd+mev9B7dnfpj3727WnpV37WttljOQ/2Cn/wU5tTUHbPG5n15HlUrar63W226ksV+irQ1muru/dzq7XbpdDbmfX912vHXJ3X3c5Hd1fu+5zOhzh84ccjujvneHv1fPa4ZAz5rrToYjX0fc7Q/c7uu8L3eNwyBlxn8Oh7nsc1AYBxwACCnAUPG5XOMAk0xkIal9rh5oOtKuxtUONrR3a19ou/8FONR/sUHPE15b2gFrbur62tHXqQEdAB9sDau0IKBBRLNPWGVRbZ1A62NnXv2ZGczrUHVwiwk13eIl3zRETlpyRryPCkDPOs5wRwajn+57zoQDljAlZidoRGdIcMfdFhrnIUObovscZ5znxnpno93bEPN8Z5zmx9zoP86zoNvWcczij+6rrn1v0+xkRRCIEFKAPuV1ODSvwaFjB51tEriMQVGt7QO2dQbV1BtTWGdTBjoA6AkbtnUG1dwbVEegKLp3BrtcdnUbtgaACQaOOQFCdQRN+HQia8PedAaPOYNe50PnOQFAB07Urddc1KRDsORe6N2C6vgZNz7lg+JyiznWdV8R10/Us03Vv6PWRlu0HjRQMGEn9rs4fESKDnUM9oSfyq0M9oc+hniAUvqf7XML3hl/3hKKuZx56LvqZcc5HPEeKvu6I+V5yRJyP/Fldr7seoNCruM/qvkU9tzvC/dbzvpjz4cwX0c6IexM/JzosThw9WF8/tbQX/zRTi4AC9ANZLqe8ucdGoa0JBZbuIGOMukOMkQn2vA6GQlD4dc/7ghEBKRSOQt9HPr/r3ojX3SHKmOjnhdoRGa562tV1fyiUGRMdxkzE66CJ387Y38d0B7ag6QptivhZPfceGuwif6fo93W9x0hRv2MgdC7iZxmjrt8tou96nq2o58Q719t5oaF+DHR9l+J/m/B5dASCBBQACOn6eEJyySG2XOp/QgEwMgiacPCKDnShUCOjiHAWEZJC33c/10QEuMhA1v2IntemJ3hF/ozIe4Ixzw1GvK8rZB363GB3+uo639OO8HO6v/bcE3Nv9wUT7qvon9lzvieoxb4/dCn0lMhAGPpduq7rkGdEtiv2zebQUzr1OO/h/nH3KQIKACBlQgGz54MD4OgcG2PGAACgXyGgAACAjENAAQAAGYeAAgAAMg4BBQAAZBwCCgAAyDgEFAAAkHEIKAAAIOMQUAAAQMYhoAAAgIxDQAEAABmHgAIAADIOAQUAAGScfrmbcWgrar/fb7klAADgSIX+bof+jifTLwNKc3OzJKmsrMxySwAAQG81NzfL6/UmvcdhjiTGZJhgMKgdO3aooKBADocjpc/2+/0qKytTXV2dCgsLU/ps9KCf04N+Tg/6OT3o5/Tpq742xqi5uVmlpaVyOpNXmfTLERSn06njjjuuT39GYWEh/wNIA/o5Pejn9KCf04N+Tp++6OvDjZyEUCQLAAAyDgEFAABkHAJKDI/Ho5/97GfyeDy2mzKg0c/pQT+nB/2cHvRz+mRCX/fLIlkAADCwMYICAAAyDgEFAABkHAIKAADIOAQUAACQcQgoEe677z6NHj1aOTk5qqys1KpVq2w3qV9buHChvvKVr6igoEDDhw/XRRddpPXr10fdc/DgQc2ZM0fFxcUaNGiQpk+froaGBkstHhjuuusuORwOzZ07N3yOfk6N7du36zvf+Y6Ki4uVm5urU045RW+//Xb4ujFGt99+u0aMGKHc3FxVV1dr48aNFlvcPwUCAc2fP18VFRXKzc3VmDFjdMcdd0Tt30Jf997f/vY3XXjhhSotLZXD4dCyZcuirh9Jn+7du1czZ85UYWGhioqKdMUVV2j//v1902ADY4wxTz31lMnOzja///3vzYcffmiuvPJKU1RUZBoaGmw3rd+aOnWqWbx4sVm7dq157733zPnnn2/Ky8vN/v37w/dcc801pqyszCxfvty8/fbb5swzzzSTJk2y2Or+bdWqVWb06NHm1FNPNTfccEP4PP38+e3du9eMGjXKXHbZZaa2ttZs3rzZvPLKK2bTpk3he+666y7j9XrNsmXLzPvvv2++8Y1vmIqKCnPgwAGLLe9/FixYYIqLi82LL75otmzZYp5++mkzaNAg89vf/jZ8D33de3/+85/NT37yE/Pss88aSea5556Lun4kfXruueea0047zbz11lvmjTfeMGPHjjWXXnppn7SXgNLtjDPOMHPmzAl/HwgETGlpqVm4cKHFVg0su3btMpLMihUrjDHGNDY2mqysLPP000+H71m3bp2RZGpqamw1s99qbm4248aNM6+++qo566yzwgGFfk6NW2+91UyZMiXh9WAwaEpKSswvf/nL8LnGxkbj8XjMk08+mY4mDhgXXHCBmT17dtS5iy++2MycOdMYQ1+nQmxAOZI+/eijj4wks3r16vA9L730knE4HGb79u0pbyMf8Uhqb2/XmjVrVF1dHT7ndDpVXV2tmpoaiy0bWJqamiRJQ4YMkSStWbNGHR0dUf0+fvx4lZeX0+9HYc6cObrgggui+lOin1Pl+eef18SJE3XJJZdo+PDhmjBhgh5++OHw9S1btqi+vj6qn71eryorK+nnXpo0aZKWL1+uDRs2SJLef/99rVy5Uuedd54k+rovHEmf1tTUqKioSBMnTgzfU11dLafTqdra2pS3qV9uFphqu3fvViAQkM/nizrv8/n08ccfW2rVwBIMBjV37lxNnjxZJ598siSpvr5e2dnZKioqirrX5/Opvr7eQiv7r6eeekrvvPOOVq9efcg1+jk1Nm/erAceeEA33XST/u3f/k2rV6/W9ddfr+zsbM2aNSvcl/H+O0I/985tt90mv9+v8ePHy+VyKRAIaMGCBZo5c6Yk0dd94Ej6tL6+XsOHD4+67na7NWTIkD7pdwIK0mLOnDlau3atVq5cabspA05dXZ1uuOEGvfrqq8rJybHdnAErGAxq4sSJ+sUvfiFJmjBhgtauXasHH3xQs2bNsty6geVPf/qTnnjiCS1dulQnnXSS3nvvPc2dO1elpaX09TGEj3gkDR06VC6X65BZDQ0NDSopKbHUqoHjuuuu04svvqjXX39dxx13XPh8SUmJ2tvb1djYGHU//d47a9as0a5du/TlL39ZbrdbbrdbK1as0KJFi+R2u+Xz+ejnFBgxYoROPPHEqHMnnHCCtm3bJknhvuS/I5/fzTffrNtuu00zZszQKaecou9+97u68cYbtXDhQkn0dV84kj4tKSnRrl27oq53dnZq7969fdLvBBRJ2dnZOv3007V8+fLwuWAwqOXLl6uqqspiy/o3Y4yuu+46Pffcc3rttddUUVERdf30009XVlZWVL+vX79e27Zto9974eyzz9YHH3yg9957L3xMnDhRM2fODL+mnz+/yZMnHzJNfsOGDRo1apQkqaKiQiUlJVH97Pf7VVtbSz/3Umtrq5zO6D9PLpdLwWBQEn3dF46kT6uqqtTY2Kg1a9aE73nttdcUDAZVWVmZ+kalvOy2n3rqqaeMx+Mxjz76qPnoo4/MVVddZYqKikx9fb3tpvVb1157rfF6veavf/2r2blzZ/hobW0N33PNNdeY8vJy89prr5m3337bVFVVmaqqKoutHhgiZ/EYQz+nwqpVq4zb7TYLFiwwGzduNE888YTJy8szjz/+ePieu+66yxQVFZn//u//Nv/4xz/MtGnTmPp6FGbNmmVGjhwZnmb87LPPmqFDh5pbbrklfA993XvNzc3m3XffNe+++66RZH7961+bd99912zdutUYc2R9eu6555oJEyaY2tpas3LlSjNu3DimGafDvffea8rLy012drY544wzzFtvvWW7Sf2apLjH4sWLw/ccOHDA/OAHPzCDBw82eXl55pvf/KbZuXOnvUYPELEBhX5OjRdeeMGcfPLJxuPxmPHjx5uHHnoo6nowGDTz5883Pp/PeDwec/bZZ5v169dbam3/5ff7zQ033GDKy8tNTk6OOf74481PfvIT09bWFr6Hvu69119/Pe5/k2fNmmWMObI+3bNnj7n00kvNoEGDTGFhobn88stNc3Nzn7TXYUzE0nwAAAAZgBoUAACQcQgoAAAg4xBQAABAxiGgAACAjENAAQAAGYeAAgAAMg4BBQAAZBwCCgAAyDgEFAAAkHEIKAAAIOMQUAAAQMYhoAAAgIzz/wG+Hm2kq4mj2QAAAABJRU5ErkJggg==",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -656,63 +656,63 @@
                 ")\n",
                 "\n",
                 "plt.plot(perplexes)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 327,
+            "execution_count": 13,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "{0: 'FIFA',\n",
-                            " 1: 'evidence',\n",
-                            " 2: 'Technique',\n",
-                            " 3: 'game',\n",
-                            " 4: 'form',\n",
-                            " 5: 'divorce',\n",
-                            " 6: 'Symmetrical',\n",
-                            " 7: 'contract',\n",
-                            " 8: 'recreation',\n",
-                            " 9: 'accuse',\n",
+                            "{0: 'appetite',\n",
+                            " 1: 'divorce',\n",
+                            " 2: 'genetics',\n",
+                            " 3: 'court',\n",
+                            " 4: 'infection',\n",
+                            " 5: 'bankrupt',\n",
+                            " 6: 'game',\n",
+                            " 7: 'evidence',\n",
+                            " 8: 'asymmetrical',\n",
+                            " 9: 'energy',\n",
                             " 10: 'content',\n",
-                            " 11: 'injection',\n",
-                            " 12: 'court',\n",
-                            " 13: 'football',\n",
-                            " 14: 'picture',\n",
-                            " 15: 'concert',\n",
-                            " 16: 'attorney',\n",
-                            " 17: 'electricity',\n",
-                            " 18: 'research',\n",
-                            " 19: 'fever',\n",
-                            " 20: 'exercise',\n",
-                            " 21: 'appetite',\n",
-                            " 22: 'infection',\n",
-                            " 23: 'athletics',\n",
-                            " 24: 'copyright',\n",
-                            " 25: 'asymmetrical',\n",
-                            " 26: 'immunology',\n",
-                            " 27: 'contagious',\n",
-                            " 28: 'genetics',\n",
-                            " 29: 'bankrupt',\n",
-                            " 30: 'quantum',\n",
-                            " 31: 'physical',\n",
-                            " 32: 'energy',\n",
-                            " 33: 'decongestant',\n",
+                            " 11: 'concert',\n",
+                            " 12: 'attorney',\n",
+                            " 13: 'recreation',\n",
+                            " 14: 'Craftsmanship',\n",
+                            " 15: 'Symmetrical',\n",
+                            " 16: 'form',\n",
+                            " 17: 'immunology',\n",
+                            " 18: 'contagious',\n",
+                            " 19: 'bruise',\n",
+                            " 20: 'injection',\n",
+                            " 21: 'FIFA',\n",
+                            " 22: 'allergy',\n",
+                            " 23: 'scientst',\n",
+                            " 24: 'accuse',\n",
+                            " 25: 'decongestant',\n",
+                            " 26: 'Technique',\n",
+                            " 27: 'football',\n",
+                            " 28: 'athletics',\n",
+                            " 29: 'quantum',\n",
+                            " 30: 'astrophysics',\n",
+                            " 31: 'copyright',\n",
+                            " 32: 'picture',\n",
+                            " 33: 'electricity',\n",
                             " 34: 'Olympic',\n",
-                            " 35: 'allergy',\n",
-                            " 36: 'scientst',\n",
-                            " 37: 'bruise',\n",
-                            " 38: 'Craftsmanship',\n",
-                            " 39: 'astrophysics'}"
+                            " 35: 'exercise',\n",
+                            " 36: 'research',\n",
+                            " 37: 'physical',\n",
+                            " 38: 'contract',\n",
+                            " 39: 'fever'}"
                         ]
                     },
-                    "execution_count": 327,
+                    "execution_count": 13,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "lda.idx_2_word"
             ]
```

### Comparing `tuotuo-0.0.2/requirements.txt` & `tuotuo-0.0.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.2/setup.py` & `tuotuo-0.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,45 +4,45 @@
 from setuptools import Extension, setup
 from Cython.Build import cythonize
 import numpy 
 from distutils.core import setup
 from pathlib import Path
 this_directory = Path(__file__).parent
 
-extensions = [
-    Extension(
-        "src/cutils", 
-        ["src/cutils.pyx"],
-        include_dirs=[numpy.get_include()], 
-    ),
-]
+# extensions = [
+#     Extension(
+#         "src/cutils", 
+#         ["src/cutils.pyx"],
+#         include_dirs=[numpy.get_include()], 
+#     ),
+# ]
 
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name = 'tuotuo',
     packages = ['src'],
-    version = '0.0.2',  
+    version = '0.0.3',  
     license='MIT',
     description = 'LDA & Neura based topic modelling library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'tuotuo Superman',
     author_email = 'tuotuo@HanwellSquare.BigForce.com',
     url = 'https://github.com/RobbenRibery/TuoTuo',
-    download_url = 'https://github.com/RobbenRibery/TuoTuo/archive/refs/tags/Pypi-V0.0.2.tar.gz',
+    download_url = 'https://github.com/RobbenRibery/TuoTuo/archive/refs/tags/Pypi-0.03.tar.gz',
     keywords = ['Generative Topic Modelling','Latent Dirichlet Allocation'],
     install_requires=[            
         'numpy',
         'torch',
         'scipy',
         'pyro',
         'nltk',
     ],
-    ext_modules=cythonize(extensions, annotate=True),
+    #ext_modules=cythonize(extensions, annotate=True),
     classifiers=[
         'Development Status :: 3 - Alpha', 
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'License :: OSI Approved :: MIT License',  
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
```

### Comparing `tuotuo-0.0.2/src/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so` & `tuotuo-0.0.3/src/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.2/src/build/temp.macosx-10.14-arm64-cpython-38/cutils.o` & `tuotuo-0.0.3/src/build/temp.macosx-10.14-arm64-cpython-38/cutils.o`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.2/src/cutils.c` & `tuotuo-0.0.3/src/cutils.c`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.2/src/cutils.cpython-38-darwin.so` & `tuotuo-0.0.3/src/cutils.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.2/src/cutils.pyx` & `tuotuo-0.0.3/src/cutils.pyx`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.2/src/generator.py` & `tuotuo-0.0.3/src/generator.py`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.2/src/lda_model.py` & `tuotuo-0.0.3/src/lda_model.py`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.2/src/text_pre_processor.py` & `tuotuo-0.0.3/src/text_pre_processor.py`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.2/src/utils.py` & `tuotuo-0.0.3/src/utils.py`

 * *Files identical despite different names*

### Comparing `tuotuo-0.0.2/tuotuo.egg-info/PKG-INFO` & `tuotuo-0.0.3/tuotuo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tuotuo
-Version: 0.0.2
+Version: 0.0.3
 Summary: LDA & Neura based topic modelling library
 Home-page: https://github.com/RobbenRibery/TuoTuo
-Download-URL: https://github.com/RobbenRibery/TuoTuo/archive/refs/tags/Pypi-V0.0.2.tar.gz
+Download-URL: https://github.com/RobbenRibery/TuoTuo/archive/refs/tags/Pypi-0.03.tar.gz
 Author: tuotuo Superman
 Author-email: tuotuo@HanwellSquare.BigForce.com
 License: MIT
 Keywords: Generative Topic Modelling,Latent Dirichlet Allocation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `tuotuo-0.0.2/tuotuo.egg-info/SOURCES.txt` & `tuotuo-0.0.3/tuotuo.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 .DS_Store
 .gitignore
 LICENSE
 README.md
-__init__.py
 cutils.cpython-38-darwin.so
 requirements.txt
 setup.cfg
 setup.py
 .github/workflows/python-package.yml
 .github/workflows/python-publish.yml
 .vscode/c_cpp_properties.json
+notebook/Our Model vs SKLearn.ipynb
 notebook/__init__.py
-notebook/computational_test.ipynb
-notebook/main copy.ipynb
-notebook/main.ipynb
-notebook/reference.ipynb
-notebook/test.ipynb
 src/__init__.py
 src/cutils.c
 src/cutils.cpython-38-darwin.so
-src/cutils.html
 src/cutils.pyx
 src/generator.py
 src/lda_model.py
 src/text_pre_processor.py
 src/utils.py
 src/build/lib.macosx-10.14-arm64-cpython-38/cutils.cpython-38-darwin.so
 src/build/temp.macosx-10.14-arm64-cpython-38/cutils.o
```

