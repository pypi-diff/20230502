# Comparing `tmp/ratsnlp-1.0.52.tar.gz` & `tmp/ratsnlp-1.0.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ratsnlp-1.0.52.tar", last modified: Tue Jun 28 06:11:24 2022, max compression
+gzip compressed data, was "ratsnlp-1.0.53.tar", last modified: Tue May  2 09:25:29 2023, max compression
```

## Comparing `ratsnlp-1.0.52.tar` & `ratsnlp-1.0.53.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 ratsgo     (501) staff       (20)        0 2022-06-28 06:11:24.786585 ratsnlp-1.0.52/
--rw-r--r--   0 ratsgo     (501) staff       (20)     1068 2022-06-28 06:06:01.000000 ratsnlp-1.0.52/LICENSE
--rw-r--r--   0 ratsgo     (501) staff       (20)      539 2022-06-28 06:11:24.786452 ratsnlp-1.0.52/PKG-INFO
--rw-r--r--   0 ratsgo     (501) staff       (20)      145 2022-06-28 06:06:01.000000 ratsnlp-1.0.52/README.md
-drwxr-xr-x   0 ratsgo     (501) staff       (20)        0 2022-06-28 06:11:24.780897 ratsnlp-1.0.52/ratsnlp/
--rw-r--r--   0 ratsgo     (501) staff       (20)        0 2022-06-28 06:06:01.000000 ratsnlp-1.0.52/ratsnlp/__init__.py
-drwxr-xr-x   0 ratsgo     (501) staff       (20)        0 2022-06-28 06:11:24.782525 ratsnlp-1.0.52/ratsnlp/nlpbook/
--rw-r--r--   0 ratsgo     (501) staff       (20)       70 2022-06-28 06:06:01.000000 ratsnlp-1.0.52/ratsnlp/nlpbook/__init__.py
-drwxr-xr-x   0 ratsgo     (501) staff       (20)        0 2022-06-28 06:11:24.783398 ratsnlp-1.0.52/ratsnlp/nlpbook/classification/
--rw-r--r--   0 ratsgo     (501) staff       (20)      181 2022-06-28 06:06:01.000000 ratsnlp-1.0.52/ratsnlp/nlpbook/classification/__init__.py
--rw-r--r--   0 ratsgo     (501) staff       (20)     4335 2022-06-28 06:06:01.000000 ratsnlp-1.0.52/ratsnlp/nlpbook/classification/arguments.py
--rw-r--r--   0 ratsgo     (501) staff       (20)     5695 2022-06-28 06:06:01.000000 ratsnlp-1.0.52/ratsnlp/nlpbook/classification/corpus.py
--rw-r--r--   0 ratsgo     (501) staff       (20)      627 2022-06-28 06:06:01.000000 ratsnlp-1.0.52/ratsnlp/nlpbook/classification/deploy.py
--rw-r--r--   0 ratsgo     (501) staff       (20)     2797 2022-06-28 06:06:01.000000 ratsnlp-1.0.52/ratsnlp/nlpbook/classification/index.html
--rw-r--r--   0 ratsgo     (501) staff       (20)     1758 2022-06-28 06:06:01.000000 ratsnlp-1.0.52/ratsnlp/nlpbook/classification/task.py
--rw-r--r--   0 ratsgo     (501) staff       (20)     2246 2022-06-28 06:06:01.000000 ratsnlp-1.0.52/ratsnlp/nlpbook/data_utils.py
-drwxr-xr-x   0 ratsgo     (501) staff       (20)        0 2022-06-28 06:11:24.784166 ratsnlp-1.0.52/ratsnlp/nlpbook/generation/
--rw-r--r--   0 ratsgo     (501) staff       (20)      170 2022-06-28 06:06:01.000000 ratsnlp-1.0.52/ratsnlp/nlpbook/generation/__init__.py
--rw-r--r--   0 ratsgo     (501) staff       (20)     4280 2022-06-28 06:06:01.000000 ratsnlp-1.0.52/ratsnlp/nlpbook/generation/arguments.py
--rw-r--r--   0 ratsgo     (501) staff       (20)     5379 2022-06-28 06:06:01.000000 ratsnlp-1.0.52/ratsnlp/nlpbook/generation/corpus.py
--rw-r--r--   0 ratsgo     (501) staff       (20)      882 2022-06-28 06:06:01.000000 ratsnlp-1.0.52/ratsnlp/nlpbook/generation/deploy.py
--rw-r--r--   0 ratsgo     (501) staff       (20)     5354 2022-06-28 06:06:01.000000 ratsnlp-1.0.52/ratsnlp/nlpbook/generation/index.html
--rw-r--r--   0 ratsgo     (501) staff       (20)     1301 2022-06-28 06:06:01.000000 ratsnlp-1.0.52/ratsnlp/nlpbook/generation/task.py
--rw-r--r--   0 ratsgo     (501) staff       (20)      653 2022-06-28 06:06:01.000000 ratsnlp-1.0.52/ratsnlp/nlpbook/metrics.py
-drwxr-xr-x   0 ratsgo     (501) staff       (20)        0 2022-06-28 06:11:24.784958 ratsnlp-1.0.52/ratsnlp/nlpbook/ner/
--rw-r--r--   0 ratsgo     (501) staff       (20)      149 2022-06-28 06:06:01.000000 ratsnlp-1.0.52/ratsnlp/nlpbook/ner/__init__.py
--rw-r--r--   0 ratsgo     (501) staff       (20)     4726 2022-06-28 06:06:01.000000 ratsnlp-1.0.52/ratsnlp/nlpbook/ner/arguments.py
--rw-r--r--   0 ratsgo     (501) staff       (20)    12164 2022-06-28 06:06:01.000000 ratsnlp-1.0.52/ratsnlp/nlpbook/ner/corpus.py
--rw-r--r--   0 ratsgo     (501) staff       (20)      627 2022-06-28 06:06:01.000000 ratsnlp-1.0.52/ratsnlp/nlpbook/ner/deploy.py
--rw-r--r--   0 ratsgo     (501) staff       (20)     2887 2022-06-28 06:06:01.000000 ratsnlp-1.0.52/ratsnlp/nlpbook/ner/index.html
--rw-r--r--   0 ratsgo     (501) staff       (20)     1768 2022-06-28 06:06:01.000000 ratsnlp-1.0.52/ratsnlp/nlpbook/ner/task.py
-drwxr-xr-x   0 ratsgo     (501) staff       (20)        0 2022-06-28 06:11:24.785449 ratsnlp-1.0.52/ratsnlp/nlpbook/paircls/
--rw-r--r--   0 ratsgo     (501) staff       (20)       62 2022-06-28 06:06:01.000000 ratsnlp-1.0.52/ratsnlp/nlpbook/paircls/__init__.py
--rw-r--r--   0 ratsgo     (501) staff       (20)     2675 2022-06-28 06:06:01.000000 ratsnlp-1.0.52/ratsnlp/nlpbook/paircls/corpus.py
--rw-r--r--   0 ratsgo     (501) staff       (20)      641 2022-06-28 06:06:01.000000 ratsnlp-1.0.52/ratsnlp/nlpbook/paircls/deploy.py
--rw-r--r--   0 ratsgo     (501) staff       (20)     3921 2022-06-28 06:06:01.000000 ratsnlp-1.0.52/ratsnlp/nlpbook/paircls/index.html
-drwxr-xr-x   0 ratsgo     (501) staff       (20)        0 2022-06-28 06:11:24.786241 ratsnlp-1.0.52/ratsnlp/nlpbook/qa/
--rw-r--r--   0 ratsgo     (501) staff       (20)      146 2022-06-28 06:06:01.000000 ratsnlp-1.0.52/ratsnlp/nlpbook/qa/__init__.py
--rw-r--r--   0 ratsgo     (501) staff       (20)     4984 2022-06-28 06:06:01.000000 ratsnlp-1.0.52/ratsnlp/nlpbook/qa/arguments.py
--rw-r--r--   0 ratsgo     (501) staff       (20)    17108 2022-06-28 06:06:01.000000 ratsnlp-1.0.52/ratsnlp/nlpbook/qa/corpus.py
--rw-r--r--   0 ratsgo     (501) staff       (20)      639 2022-06-28 06:06:01.000000 ratsnlp-1.0.52/ratsnlp/nlpbook/qa/deploy.py
--rw-r--r--   0 ratsgo     (501) staff       (20)     3258 2022-06-28 06:06:01.000000 ratsnlp-1.0.52/ratsnlp/nlpbook/qa/index.html
--rw-r--r--   0 ratsgo     (501) staff       (20)     2088 2022-06-28 06:06:01.000000 ratsnlp-1.0.52/ratsnlp/nlpbook/qa/task.py
--rw-r--r--   0 ratsgo     (501) staff       (20)     1150 2022-06-28 06:06:01.000000 ratsnlp-1.0.52/ratsnlp/nlpbook/trainer.py
--rw-r--r--   0 ratsgo     (501) staff       (20)     8762 2022-06-28 06:06:01.000000 ratsnlp-1.0.52/ratsnlp/nlpbook/utils.py
-drwxr-xr-x   0 ratsgo     (501) staff       (20)        0 2022-06-28 06:11:24.781423 ratsnlp-1.0.52/ratsnlp.egg-info/
--rw-r--r--   0 ratsgo     (501) staff       (20)      539 2022-06-28 06:11:24.000000 ratsnlp-1.0.52/ratsnlp.egg-info/PKG-INFO
--rw-r--r--   0 ratsgo     (501) staff       (20)     1314 2022-06-28 06:11:24.000000 ratsnlp-1.0.52/ratsnlp.egg-info/SOURCES.txt
--rw-r--r--   0 ratsgo     (501) staff       (20)        1 2022-06-28 06:11:24.000000 ratsnlp-1.0.52/ratsnlp.egg-info/dependency_links.txt
--rw-r--r--   0 ratsgo     (501) staff       (20)      113 2022-06-28 06:11:24.000000 ratsnlp-1.0.52/ratsnlp.egg-info/requires.txt
--rw-r--r--   0 ratsgo     (501) staff       (20)        8 2022-06-28 06:11:24.000000 ratsnlp-1.0.52/ratsnlp.egg-info/top_level.txt
--rw-r--r--   0 ratsgo     (501) staff       (20)       38 2022-06-28 06:11:24.786626 ratsnlp-1.0.52/setup.cfg
--rw-r--r--   0 ratsgo     (501) staff       (20)     1015 2022-06-28 06:11:22.000000 ratsnlp-1.0.52/setup.py
+drwxr-xr-x   0 ratsgo     (502) staff       (20)        0 2023-05-02 09:25:29.202000 ratsnlp-1.0.53/
+-rw-r--r--   0 ratsgo     (502) staff       (20)     1068 2023-05-02 09:20:17.000000 ratsnlp-1.0.53/LICENSE
+-rw-r--r--   0 ratsgo     (502) staff       (20)      520 2023-05-02 09:25:29.201805 ratsnlp-1.0.53/PKG-INFO
+-rw-r--r--   0 ratsgo     (502) staff       (20)      145 2023-05-02 09:20:17.000000 ratsnlp-1.0.53/README.md
+drwxr-xr-x   0 ratsgo     (502) staff       (20)        0 2023-05-02 09:25:29.196614 ratsnlp-1.0.53/ratsnlp/
+-rw-r--r--   0 ratsgo     (502) staff       (20)        0 2023-05-02 09:20:17.000000 ratsnlp-1.0.53/ratsnlp/__init__.py
+drwxr-xr-x   0 ratsgo     (502) staff       (20)        0 2023-05-02 09:25:29.197879 ratsnlp-1.0.53/ratsnlp/nlpbook/
+-rw-r--r--   0 ratsgo     (502) staff       (20)       70 2023-05-02 09:20:17.000000 ratsnlp-1.0.53/ratsnlp/nlpbook/__init__.py
+drwxr-xr-x   0 ratsgo     (502) staff       (20)        0 2023-05-02 09:25:29.198712 ratsnlp-1.0.53/ratsnlp/nlpbook/classification/
+-rw-r--r--   0 ratsgo     (502) staff       (20)      181 2023-05-02 09:20:17.000000 ratsnlp-1.0.53/ratsnlp/nlpbook/classification/__init__.py
+-rw-r--r--   0 ratsgo     (502) staff       (20)     4335 2023-05-02 09:20:17.000000 ratsnlp-1.0.53/ratsnlp/nlpbook/classification/arguments.py
+-rw-r--r--   0 ratsgo     (502) staff       (20)     5695 2023-05-02 09:20:17.000000 ratsnlp-1.0.53/ratsnlp/nlpbook/classification/corpus.py
+-rw-r--r--   0 ratsgo     (502) staff       (20)      627 2023-05-02 09:20:17.000000 ratsnlp-1.0.53/ratsnlp/nlpbook/classification/deploy.py
+-rw-r--r--   0 ratsgo     (502) staff       (20)     2797 2023-05-02 09:20:17.000000 ratsnlp-1.0.53/ratsnlp/nlpbook/classification/index.html
+-rw-r--r--   0 ratsgo     (502) staff       (20)     1758 2023-05-02 09:20:17.000000 ratsnlp-1.0.53/ratsnlp/nlpbook/classification/task.py
+-rw-r--r--   0 ratsgo     (502) staff       (20)     2246 2023-05-02 09:20:17.000000 ratsnlp-1.0.53/ratsnlp/nlpbook/data_utils.py
+drwxr-xr-x   0 ratsgo     (502) staff       (20)        0 2023-05-02 09:25:29.199569 ratsnlp-1.0.53/ratsnlp/nlpbook/generation/
+-rw-r--r--   0 ratsgo     (502) staff       (20)      170 2023-05-02 09:20:17.000000 ratsnlp-1.0.53/ratsnlp/nlpbook/generation/__init__.py
+-rw-r--r--   0 ratsgo     (502) staff       (20)     4280 2023-05-02 09:20:17.000000 ratsnlp-1.0.53/ratsnlp/nlpbook/generation/arguments.py
+-rw-r--r--   0 ratsgo     (502) staff       (20)     5379 2023-05-02 09:20:17.000000 ratsnlp-1.0.53/ratsnlp/nlpbook/generation/corpus.py
+-rw-r--r--   0 ratsgo     (502) staff       (20)      882 2023-05-02 09:20:17.000000 ratsnlp-1.0.53/ratsnlp/nlpbook/generation/deploy.py
+-rw-r--r--   0 ratsgo     (502) staff       (20)     5354 2023-05-02 09:20:17.000000 ratsnlp-1.0.53/ratsnlp/nlpbook/generation/index.html
+-rw-r--r--   0 ratsgo     (502) staff       (20)     1301 2023-05-02 09:20:17.000000 ratsnlp-1.0.53/ratsnlp/nlpbook/generation/task.py
+-rw-r--r--   0 ratsgo     (502) staff       (20)      653 2023-05-02 09:20:17.000000 ratsnlp-1.0.53/ratsnlp/nlpbook/metrics.py
+drwxr-xr-x   0 ratsgo     (502) staff       (20)        0 2023-05-02 09:25:29.200328 ratsnlp-1.0.53/ratsnlp/nlpbook/ner/
+-rw-r--r--   0 ratsgo     (502) staff       (20)      149 2023-05-02 09:20:17.000000 ratsnlp-1.0.53/ratsnlp/nlpbook/ner/__init__.py
+-rw-r--r--   0 ratsgo     (502) staff       (20)     4726 2023-05-02 09:20:17.000000 ratsnlp-1.0.53/ratsnlp/nlpbook/ner/arguments.py
+-rw-r--r--   0 ratsgo     (502) staff       (20)    12164 2023-05-02 09:20:17.000000 ratsnlp-1.0.53/ratsnlp/nlpbook/ner/corpus.py
+-rw-r--r--   0 ratsgo     (502) staff       (20)      627 2023-05-02 09:20:17.000000 ratsnlp-1.0.53/ratsnlp/nlpbook/ner/deploy.py
+-rw-r--r--   0 ratsgo     (502) staff       (20)     2887 2023-05-02 09:20:17.000000 ratsnlp-1.0.53/ratsnlp/nlpbook/ner/index.html
+-rw-r--r--   0 ratsgo     (502) staff       (20)     1768 2023-05-02 09:20:17.000000 ratsnlp-1.0.53/ratsnlp/nlpbook/ner/task.py
+drwxr-xr-x   0 ratsgo     (502) staff       (20)        0 2023-05-02 09:25:29.200815 ratsnlp-1.0.53/ratsnlp/nlpbook/paircls/
+-rw-r--r--   0 ratsgo     (502) staff       (20)       62 2023-05-02 09:20:17.000000 ratsnlp-1.0.53/ratsnlp/nlpbook/paircls/__init__.py
+-rw-r--r--   0 ratsgo     (502) staff       (20)     2675 2023-05-02 09:20:17.000000 ratsnlp-1.0.53/ratsnlp/nlpbook/paircls/corpus.py
+-rw-r--r--   0 ratsgo     (502) staff       (20)      641 2023-05-02 09:20:17.000000 ratsnlp-1.0.53/ratsnlp/nlpbook/paircls/deploy.py
+-rw-r--r--   0 ratsgo     (502) staff       (20)     3921 2023-05-02 09:20:17.000000 ratsnlp-1.0.53/ratsnlp/nlpbook/paircls/index.html
+drwxr-xr-x   0 ratsgo     (502) staff       (20)        0 2023-05-02 09:25:29.201584 ratsnlp-1.0.53/ratsnlp/nlpbook/qa/
+-rw-r--r--   0 ratsgo     (502) staff       (20)      146 2023-05-02 09:20:17.000000 ratsnlp-1.0.53/ratsnlp/nlpbook/qa/__init__.py
+-rw-r--r--   0 ratsgo     (502) staff       (20)     4984 2023-05-02 09:20:17.000000 ratsnlp-1.0.53/ratsnlp/nlpbook/qa/arguments.py
+-rw-r--r--   0 ratsgo     (502) staff       (20)    17108 2023-05-02 09:20:17.000000 ratsnlp-1.0.53/ratsnlp/nlpbook/qa/corpus.py
+-rw-r--r--   0 ratsgo     (502) staff       (20)      639 2023-05-02 09:20:17.000000 ratsnlp-1.0.53/ratsnlp/nlpbook/qa/deploy.py
+-rw-r--r--   0 ratsgo     (502) staff       (20)     3258 2023-05-02 09:20:17.000000 ratsnlp-1.0.53/ratsnlp/nlpbook/qa/index.html
+-rw-r--r--   0 ratsgo     (502) staff       (20)     2088 2023-05-02 09:20:17.000000 ratsnlp-1.0.53/ratsnlp/nlpbook/qa/task.py
+-rw-r--r--   0 ratsgo     (502) staff       (20)     1150 2023-05-02 09:20:17.000000 ratsnlp-1.0.53/ratsnlp/nlpbook/trainer.py
+-rw-r--r--   0 ratsgo     (502) staff       (20)     8762 2023-05-02 09:20:17.000000 ratsnlp-1.0.53/ratsnlp/nlpbook/utils.py
+drwxr-xr-x   0 ratsgo     (502) staff       (20)        0 2023-05-02 09:25:29.197260 ratsnlp-1.0.53/ratsnlp.egg-info/
+-rw-r--r--   0 ratsgo     (502) staff       (20)      520 2023-05-02 09:25:29.000000 ratsnlp-1.0.53/ratsnlp.egg-info/PKG-INFO
+-rw-r--r--   0 ratsgo     (502) staff       (20)     1314 2023-05-02 09:25:29.000000 ratsnlp-1.0.53/ratsnlp.egg-info/SOURCES.txt
+-rw-r--r--   0 ratsgo     (502) staff       (20)        1 2023-05-02 09:25:29.000000 ratsnlp-1.0.53/ratsnlp.egg-info/dependency_links.txt
+-rw-r--r--   0 ratsgo     (502) staff       (20)      113 2023-05-02 09:25:29.000000 ratsnlp-1.0.53/ratsnlp.egg-info/requires.txt
+-rw-r--r--   0 ratsgo     (502) staff       (20)        8 2023-05-02 09:25:29.000000 ratsnlp-1.0.53/ratsnlp.egg-info/top_level.txt
+-rw-r--r--   0 ratsgo     (502) staff       (20)       38 2023-05-02 09:25:29.202056 ratsnlp-1.0.53/setup.cfg
+-rw-r--r--   0 ratsgo     (502) staff       (20)     1015 2023-05-02 09:21:46.000000 ratsnlp-1.0.53/setup.py
```

### Comparing `ratsnlp-1.0.52/LICENSE` & `ratsnlp-1.0.53/LICENSE`

 * *Files identical despite different names*

### Comparing `ratsnlp-1.0.52/PKG-INFO` & `ratsnlp-1.0.53/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: ratsnlp
-Version: 1.0.52
+Version: 1.0.53
 Summary: tools for Natural Language Processing
 Home-page: https://github.com/ratsgo/ratsnlp
 Author: ratsgo
 Author-email: ratsgo@naver.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
 
 # ratsnlp
 
 자연어 처리 실습을 위한 패키지입니다. 구글 코랩(colab) 환경에서 동작할 수 있도록 작성하였습니다.
-
```

### Comparing `ratsnlp-1.0.52/ratsnlp/nlpbook/classification/arguments.py` & `ratsnlp-1.0.53/ratsnlp/nlpbook/classification/arguments.py`

 * *Files identical despite different names*

### Comparing `ratsnlp-1.0.52/ratsnlp/nlpbook/classification/corpus.py` & `ratsnlp-1.0.53/ratsnlp/nlpbook/classification/corpus.py`

 * *Files identical despite different names*

### Comparing `ratsnlp-1.0.52/ratsnlp/nlpbook/classification/deploy.py` & `ratsnlp-1.0.53/ratsnlp/nlpbook/classification/deploy.py`

 * *Files identical despite different names*

### Comparing `ratsnlp-1.0.52/ratsnlp/nlpbook/classification/index.html` & `ratsnlp-1.0.53/ratsnlp/nlpbook/classification/index.html`

 * *Files identical despite different names*

### Comparing `ratsnlp-1.0.52/ratsnlp/nlpbook/classification/task.py` & `ratsnlp-1.0.53/ratsnlp/nlpbook/classification/task.py`

 * *Files identical despite different names*

### Comparing `ratsnlp-1.0.52/ratsnlp/nlpbook/data_utils.py` & `ratsnlp-1.0.53/ratsnlp/nlpbook/data_utils.py`

 * *Files identical despite different names*

### Comparing `ratsnlp-1.0.52/ratsnlp/nlpbook/generation/arguments.py` & `ratsnlp-1.0.53/ratsnlp/nlpbook/generation/arguments.py`

 * *Files identical despite different names*

### Comparing `ratsnlp-1.0.52/ratsnlp/nlpbook/generation/corpus.py` & `ratsnlp-1.0.53/ratsnlp/nlpbook/generation/corpus.py`

 * *Files identical despite different names*

### Comparing `ratsnlp-1.0.52/ratsnlp/nlpbook/generation/deploy.py` & `ratsnlp-1.0.53/ratsnlp/nlpbook/generation/deploy.py`

 * *Files identical despite different names*

### Comparing `ratsnlp-1.0.52/ratsnlp/nlpbook/generation/index.html` & `ratsnlp-1.0.53/ratsnlp/nlpbook/generation/index.html`

 * *Files identical despite different names*

### Comparing `ratsnlp-1.0.52/ratsnlp/nlpbook/generation/task.py` & `ratsnlp-1.0.53/ratsnlp/nlpbook/generation/task.py`

 * *Files identical despite different names*

### Comparing `ratsnlp-1.0.52/ratsnlp/nlpbook/metrics.py` & `ratsnlp-1.0.53/ratsnlp/nlpbook/metrics.py`

 * *Files identical despite different names*

### Comparing `ratsnlp-1.0.52/ratsnlp/nlpbook/ner/arguments.py` & `ratsnlp-1.0.53/ratsnlp/nlpbook/ner/arguments.py`

 * *Files identical despite different names*

### Comparing `ratsnlp-1.0.52/ratsnlp/nlpbook/ner/corpus.py` & `ratsnlp-1.0.53/ratsnlp/nlpbook/ner/corpus.py`

 * *Files identical despite different names*

### Comparing `ratsnlp-1.0.52/ratsnlp/nlpbook/ner/deploy.py` & `ratsnlp-1.0.53/ratsnlp/nlpbook/ner/deploy.py`

 * *Files identical despite different names*

### Comparing `ratsnlp-1.0.52/ratsnlp/nlpbook/ner/index.html` & `ratsnlp-1.0.53/ratsnlp/nlpbook/ner/index.html`

 * *Files identical despite different names*

### Comparing `ratsnlp-1.0.52/ratsnlp/nlpbook/ner/task.py` & `ratsnlp-1.0.53/ratsnlp/nlpbook/ner/task.py`

 * *Files identical despite different names*

### Comparing `ratsnlp-1.0.52/ratsnlp/nlpbook/paircls/corpus.py` & `ratsnlp-1.0.53/ratsnlp/nlpbook/paircls/corpus.py`

 * *Files identical despite different names*

### Comparing `ratsnlp-1.0.52/ratsnlp/nlpbook/paircls/deploy.py` & `ratsnlp-1.0.53/ratsnlp/nlpbook/paircls/deploy.py`

 * *Files identical despite different names*

### Comparing `ratsnlp-1.0.52/ratsnlp/nlpbook/paircls/index.html` & `ratsnlp-1.0.53/ratsnlp/nlpbook/paircls/index.html`

 * *Files identical despite different names*

### Comparing `ratsnlp-1.0.52/ratsnlp/nlpbook/qa/arguments.py` & `ratsnlp-1.0.53/ratsnlp/nlpbook/qa/arguments.py`

 * *Files identical despite different names*

### Comparing `ratsnlp-1.0.52/ratsnlp/nlpbook/qa/corpus.py` & `ratsnlp-1.0.53/ratsnlp/nlpbook/qa/corpus.py`

 * *Files identical despite different names*

### Comparing `ratsnlp-1.0.52/ratsnlp/nlpbook/qa/deploy.py` & `ratsnlp-1.0.53/ratsnlp/nlpbook/qa/deploy.py`

 * *Files identical despite different names*

### Comparing `ratsnlp-1.0.52/ratsnlp/nlpbook/qa/index.html` & `ratsnlp-1.0.53/ratsnlp/nlpbook/qa/index.html`

 * *Files identical despite different names*

### Comparing `ratsnlp-1.0.52/ratsnlp/nlpbook/qa/task.py` & `ratsnlp-1.0.53/ratsnlp/nlpbook/qa/task.py`

 * *Files identical despite different names*

### Comparing `ratsnlp-1.0.52/ratsnlp/nlpbook/trainer.py` & `ratsnlp-1.0.53/ratsnlp/nlpbook/trainer.py`

 * *Files identical despite different names*

### Comparing `ratsnlp-1.0.52/ratsnlp/nlpbook/utils.py` & `ratsnlp-1.0.53/ratsnlp/nlpbook/utils.py`

 * *Files identical despite different names*

### Comparing `ratsnlp-1.0.52/ratsnlp.egg-info/PKG-INFO` & `ratsnlp-1.0.53/ratsnlp.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: ratsnlp
-Version: 1.0.52
+Version: 1.0.53
 Summary: tools for Natural Language Processing
 Home-page: https://github.com/ratsgo/ratsnlp
 Author: ratsgo
 Author-email: ratsgo@naver.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
 
 # ratsnlp
 
 자연어 처리 실습을 위한 패키지입니다. 구글 코랩(colab) 환경에서 동작할 수 있도록 작성하였습니다.
-
```

### Comparing `ratsnlp-1.0.52/ratsnlp.egg-info/SOURCES.txt` & `ratsnlp-1.0.53/ratsnlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ratsnlp-1.0.52/setup.py` & `ratsnlp-1.0.53/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 def requirements():
     with open(os.path.join(os.path.dirname(__file__), 'requirements.txt'), encoding='utf-8') as f:
         return f.read().splitlines()
 
 
 setuptools.setup(
     name="ratsnlp",
-    version="1.0.52",
+    version="1.0.53",
     license='MIT',
     author="ratsgo",
     author_email="ratsgo@naver.com",
     description="tools for Natural Language Processing",
     long_description=open('README.md').read(),
     url="https://github.com/ratsgo/ratsnlp",
     packages=setuptools.find_packages(),
```

