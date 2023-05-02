# Comparing `tmp/word-search-generator-3.2.0.tar.gz` & `tmp/word-search-generator-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "word-search-generator-3.2.0.tar", last modified: Mon Mar  6 05:28:09 2023, max compression
+gzip compressed data, was "word-search-generator-3.3.0.tar", last modified: Tue May  2 16:12:33 2023, max compression
```

## Comparing `word-search-generator-3.2.0.tar` & `word-search-generator-3.3.0.tar`

### file list

```diff
@@ -1,60 +1,63 @@
-drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-03-06 05:28:09.223975 word-search-generator-3.2.0/
--rw-r--r--   0 jbd        (501) staff       (20)       51 2023-03-06 05:02:24.000000 word-search-generator-3.2.0/.flake8
-drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-03-06 05:28:09.192329 word-search-generator-3.2.0/.github/
-drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-03-06 05:28:09.202466 word-search-generator-3.2.0/.github/workflows/
--rw-r--r--   0 jbd        (501) staff       (20)      623 2022-10-24 19:07:34.000000 word-search-generator-3.2.0/.github/workflows/tests.yml
--rw-r--r--   0 jbd        (501) staff       (20)     1966 2022-12-02 05:03:47.000000 word-search-generator-3.2.0/.gitignore
--rw-r--r--   0 jbd        (501) staff       (20)      961 2023-03-06 05:02:24.000000 word-search-generator-3.2.0/.pre-commit-config.yaml
--rw-r--r--   0 jbd        (501) staff       (20)    13285 2023-03-06 05:06:59.000000 word-search-generator-3.2.0/CHANGLOG.md
--rw-r--r--   0 jbd        (501) staff       (20)     1077 2022-12-02 16:21:47.000000 word-search-generator-3.2.0/LICENSE
--rw-r--r--   0 jbd        (501) staff       (20)     6894 2023-03-06 05:28:09.223273 word-search-generator-3.2.0/PKG-INFO
--rw-r--r--   0 jbd        (501) staff       (20)     5806 2022-12-31 04:47:08.000000 word-search-generator-3.2.0/README.md
--rw-r--r--   0 jbd        (501) staff       (20)     2540 2023-03-06 05:16:29.000000 word-search-generator-3.2.0/pyproject.toml
--rw-r--r--   0 jbd        (501) staff       (20)      157 2023-03-06 05:02:24.000000 word-search-generator-3.2.0/requirements-dev.txt
--rw-r--r--   0 jbd        (501) staff       (20)       38 2023-01-20 23:10:24.000000 word-search-generator-3.2.0/requirements.txt
--rwxr-xr-x   0 jbd        (501) staff       (20)     1384 2023-03-06 05:27:14.000000 word-search-generator-3.2.0/run
--rw-r--r--   0 jbd        (501) staff       (20)       38 2023-03-06 05:28:09.224114 word-search-generator-3.2.0/setup.cfg
--rw-r--r--   0 jbd        (501) staff       (20)       38 2022-10-24 15:15:00.000000 word-search-generator-3.2.0/setup.py
-drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-03-06 05:28:09.192865 word-search-generator-3.2.0/src/
-drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-03-06 05:28:09.206712 word-search-generator-3.2.0/src/word_search_generator/
--rw-r--r--   0 jbd        (501) staff       (20)    21956 2023-03-06 05:06:51.000000 word-search-generator-3.2.0/src/word_search_generator/__init__.py
--rw-r--r--   0 jbd        (501) staff       (20)      119 2022-12-02 04:41:56.000000 word-search-generator-3.2.0/src/word_search_generator/__main__.py
--rw-r--r--   0 jbd        (501) staff       (20)     7804 2023-03-06 05:02:24.000000 word-search-generator-3.2.0/src/word_search_generator/cli.py
--rw-r--r--   0 jbd        (501) staff       (20)     1174 2023-01-09 17:44:57.000000 word-search-generator-3.2.0/src/word_search_generator/config.py
--rw-r--r--   0 jbd        (501) staff       (20)     6360 2023-03-06 05:02:24.000000 word-search-generator-3.2.0/src/word_search_generator/export.py
--rw-r--r--   0 jbd        (501) staff       (20)     7847 2023-01-10 03:52:45.000000 word-search-generator-3.2.0/src/word_search_generator/generate.py
-drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-03-06 05:28:09.212028 word-search-generator-3.2.0/src/word_search_generator/mask/
--rw-r--r--   0 jbd        (501) staff       (20)    11610 2023-03-05 05:39:02.000000 word-search-generator-3.2.0/src/word_search_generator/mask/__init__.py
--rw-r--r--   0 jbd        (501) staff       (20)     4202 2023-03-05 05:38:40.000000 word-search-generator-3.2.0/src/word_search_generator/mask/bitmap.py
--rw-r--r--   0 jbd        (501) staff       (20)     3713 2023-03-05 05:38:25.000000 word-search-generator-3.2.0/src/word_search_generator/mask/ellipse.py
--rw-r--r--   0 jbd        (501) staff       (20)    14321 2023-03-05 05:38:12.000000 word-search-generator-3.2.0/src/word_search_generator/mask/polygon.py
--rw-r--r--   0 jbd        (501) staff       (20)     6230 2023-03-05 05:37:52.000000 word-search-generator-3.2.0/src/word_search_generator/mask/shapes.py
--rw-r--r--   0 jbd        (501) staff       (20)        0 2021-09-14 03:56:24.000000 word-search-generator-3.2.0/src/word_search_generator/py.typed
--rw-r--r--   0 jbd        (501) staff       (20)    24021 2023-03-06 05:02:24.000000 word-search-generator-3.2.0/src/word_search_generator/utils.py
-drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-03-06 05:28:09.212452 word-search-generator-3.2.0/src/word_search_generator/word/
--rw-r--r--   0 jbd        (501) staff       (20)     6873 2023-01-10 03:52:45.000000 word-search-generator-3.2.0/src/word_search_generator/word/__init__.py
-drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-03-06 05:28:09.209824 word-search-generator-3.2.0/src/word_search_generator.egg-info/
--rw-r--r--   0 jbd        (501) staff       (20)     6894 2023-03-06 05:28:09.000000 word-search-generator-3.2.0/src/word_search_generator.egg-info/PKG-INFO
--rw-r--r--   0 jbd        (501) staff       (20)     1388 2023-03-06 05:28:09.000000 word-search-generator-3.2.0/src/word_search_generator.egg-info/SOURCES.txt
--rw-r--r--   0 jbd        (501) staff       (20)        1 2023-03-06 05:28:09.000000 word-search-generator-3.2.0/src/word_search_generator.egg-info/dependency_links.txt
--rw-r--r--   0 jbd        (501) staff       (20)       63 2023-03-06 05:28:09.000000 word-search-generator-3.2.0/src/word_search_generator.egg-info/entry_points.txt
--rw-r--r--   0 jbd        (501) staff       (20)      180 2023-03-06 05:28:09.000000 word-search-generator-3.2.0/src/word_search_generator.egg-info/requires.txt
--rw-r--r--   0 jbd        (501) staff       (20)       22 2023-03-06 05:28:09.000000 word-search-generator-3.2.0/src/word_search_generator.egg-info/top_level.txt
-drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-03-06 05:28:09.216024 word-search-generator-3.2.0/tests/
--rw-r--r--   0 jbd        (501) staff       (20)      460 2022-12-31 04:21:53.000000 word-search-generator-3.2.0/tests/__init__.py
--rw-r--r--   0 jbd        (501) staff       (20)    15078 2023-01-09 21:28:35.000000 word-search-generator-3.2.0/tests/test_Mask.py
--rw-r--r--   0 jbd        (501) staff       (20)     1188 2022-12-02 04:41:56.000000 word-search-generator-3.2.0/tests/test_Word.py
--rw-r--r--   0 jbd        (501) staff       (20)    12595 2023-01-10 03:52:45.000000 word-search-generator-3.2.0/tests/test_WordSearch.py
--rw-r--r--   0 jbd        (501) staff       (20)     5716 2023-03-06 05:02:24.000000 word-search-generator-3.2.0/tests/test_cli.py
--rw-r--r--   0 jbd        (501) staff       (20)     8797 2023-03-06 05:02:24.000000 word-search-generator-3.2.0/tests/test_export.py
--rw-r--r--   0 jbd        (501) staff       (20)     2556 2023-01-10 03:52:45.000000 word-search-generator-3.2.0/tests/test_generate.py
--rw-r--r--   0 jbd        (501) staff       (20)     2392 2022-12-31 04:21:53.000000 word-search-generator-3.2.0/tests/test_utils.py
-drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-03-06 05:28:09.216462 word-search-generator-3.2.0/tools/
--rw-r--r--   0 jbd        (501) staff       (20)     1125 2023-01-03 03:25:46.000000 word-search-generator-3.2.0/tools/pdf_layout_testing.py
-drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-03-06 05:28:09.222160 word-search-generator-3.2.0/tools/sample_word_lists/
--rw-r--r--   0 jbd        (501) staff       (20)       76 2021-08-19 05:15:03.000000 word-search-generator-3.2.0/tools/sample_word_lists/words-10.txt
--rw-r--r--   0 jbd        (501) staff       (20)      173 2021-08-19 05:15:05.000000 word-search-generator-3.2.0/tools/sample_word_lists/words-25.txt
--rw-r--r--   0 jbd        (501) staff       (20)       43 2021-08-19 05:15:01.000000 word-search-generator-3.2.0/tools/sample_word_lists/words-5.txt
--rw-r--r--   0 jbd        (501) staff       (20)      369 2021-08-19 05:15:06.000000 word-search-generator-3.2.0/tools/sample_word_lists/words-50.txt
--rw-r--r--   0 jbd        (501) staff       (20)       83 2021-08-19 05:15:08.000000 word-search-generator-3.2.0/tools/sample_word_lists/words-junk.txt
--rw-r--r--   0 jbd        (501) staff       (20)      523 2023-03-06 05:02:24.000000 word-search-generator-3.2.0/tox.ini
+drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-05-02 16:12:33.793887 word-search-generator-3.3.0/
+-rw-r--r--   0 jbd        (501) staff       (20)       51 2023-03-06 05:02:24.000000 word-search-generator-3.3.0/.flake8
+drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-05-02 16:12:33.695141 word-search-generator-3.3.0/.github/
+drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-05-02 16:12:33.732013 word-search-generator-3.3.0/.github/workflows/
+-rw-r--r--   0 jbd        (501) staff       (20)      623 2022-10-24 19:07:34.000000 word-search-generator-3.3.0/.github/workflows/tests.yml
+-rw-r--r--   0 jbd        (501) staff       (20)     1978 2023-03-15 21:31:53.000000 word-search-generator-3.3.0/.gitignore
+-rw-r--r--   0 jbd        (501) staff       (20)      961 2023-03-06 05:02:24.000000 word-search-generator-3.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 jbd        (501) staff       (20)    14802 2023-05-02 15:59:25.000000 word-search-generator-3.3.0/CHANGLOG.md
+-rw-r--r--   0 jbd        (501) staff       (20)     1077 2022-12-02 16:21:47.000000 word-search-generator-3.3.0/LICENSE
+-rw-r--r--   0 jbd        (501) staff       (20)     8042 2023-05-02 16:12:33.792548 word-search-generator-3.3.0/PKG-INFO
+-rw-r--r--   0 jbd        (501) staff       (20)     6954 2023-03-16 21:31:14.000000 word-search-generator-3.3.0/README.md
+-rw-r--r--   0 jbd        (501) staff       (20)      383 2023-03-16 21:34:27.000000 word-search-generator-3.3.0/TODO.md
+-rw-r--r--   0 jbd        (501) staff       (20)     2650 2023-03-15 21:31:53.000000 word-search-generator-3.3.0/pyproject.toml
+-rw-r--r--   0 jbd        (501) staff       (20)      157 2023-03-06 05:02:24.000000 word-search-generator-3.3.0/requirements-dev.txt
+-rw-r--r--   0 jbd        (501) staff       (20)       38 2023-01-20 23:10:24.000000 word-search-generator-3.3.0/requirements.txt
+-rwxr-xr-x   0 jbd        (501) staff       (20)     1384 2023-03-06 05:27:14.000000 word-search-generator-3.3.0/run
+-rw-r--r--   0 jbd        (501) staff       (20)       38 2023-05-02 16:12:33.794777 word-search-generator-3.3.0/setup.cfg
+-rw-r--r--   0 jbd        (501) staff       (20)       38 2022-10-24 15:15:00.000000 word-search-generator-3.3.0/setup.py
+drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-05-02 16:12:33.696725 word-search-generator-3.3.0/src/
+drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-05-02 16:12:33.741589 word-search-generator-3.3.0/src/word_search_generator/
+-rw-r--r--   0 jbd        (501) staff       (20)    22173 2023-05-02 15:59:25.000000 word-search-generator-3.3.0/src/word_search_generator/__init__.py
+-rw-r--r--   0 jbd        (501) staff       (20)      119 2022-12-02 04:41:56.000000 word-search-generator-3.3.0/src/word_search_generator/__main__.py
+-rw-r--r--   0 jbd        (501) staff       (20)     7856 2023-03-16 18:18:19.000000 word-search-generator-3.3.0/src/word_search_generator/cli.py
+-rw-r--r--   0 jbd        (501) staff       (20)     1174 2023-01-09 17:44:57.000000 word-search-generator-3.3.0/src/word_search_generator/config.py
+-rw-r--r--   0 jbd        (501) staff       (20)     6360 2023-03-06 05:02:24.000000 word-search-generator-3.3.0/src/word_search_generator/export.py
+-rw-r--r--   0 jbd        (501) staff       (20)     7847 2023-01-10 03:52:45.000000 word-search-generator-3.3.0/src/word_search_generator/generate.py
+drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-05-02 16:12:33.757199 word-search-generator-3.3.0/src/word_search_generator/mask/
+-rw-r--r--   0 jbd        (501) staff       (20)    11610 2023-03-15 21:31:53.000000 word-search-generator-3.3.0/src/word_search_generator/mask/__init__.py
+-rw-r--r--   0 jbd        (501) staff       (20)     4202 2023-03-15 21:31:53.000000 word-search-generator-3.3.0/src/word_search_generator/mask/bitmap.py
+-rw-r--r--   0 jbd        (501) staff       (20)     3694 2023-03-15 21:31:53.000000 word-search-generator-3.3.0/src/word_search_generator/mask/ellipse.py
+-rw-r--r--   0 jbd        (501) staff       (20)    14385 2023-03-15 21:31:53.000000 word-search-generator-3.3.0/src/word_search_generator/mask/polygon.py
+-rw-r--r--   0 jbd        (501) staff       (20)    13001 2023-05-02 15:59:25.000000 word-search-generator-3.3.0/src/word_search_generator/mask/shapes.py
+-rw-r--r--   0 jbd        (501) staff       (20)        0 2021-09-14 03:56:24.000000 word-search-generator-3.3.0/src/word_search_generator/py.typed
+-rw-r--r--   0 jbd        (501) staff       (20)    23777 2023-05-02 15:59:36.000000 word-search-generator-3.3.0/src/word_search_generator/utils.py
+drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-05-02 16:12:33.759165 word-search-generator-3.3.0/src/word_search_generator/word/
+-rw-r--r--   0 jbd        (501) staff       (20)     6873 2023-01-10 03:52:45.000000 word-search-generator-3.3.0/src/word_search_generator/word/__init__.py
+drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-05-02 16:12:33.752241 word-search-generator-3.3.0/src/word_search_generator.egg-info/
+-rw-r--r--   0 jbd        (501) staff       (20)     8042 2023-05-02 16:12:33.000000 word-search-generator-3.3.0/src/word_search_generator.egg-info/PKG-INFO
+-rw-r--r--   0 jbd        (501) staff       (20)     1450 2023-05-02 16:12:33.000000 word-search-generator-3.3.0/src/word_search_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 jbd        (501) staff       (20)        1 2023-05-02 16:12:33.000000 word-search-generator-3.3.0/src/word_search_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 jbd        (501) staff       (20)       63 2023-05-02 16:12:33.000000 word-search-generator-3.3.0/src/word_search_generator.egg-info/entry_points.txt
+-rw-r--r--   0 jbd        (501) staff       (20)      180 2023-05-02 16:12:33.000000 word-search-generator-3.3.0/src/word_search_generator.egg-info/requires.txt
+-rw-r--r--   0 jbd        (501) staff       (20)       22 2023-05-02 16:12:33.000000 word-search-generator-3.3.0/src/word_search_generator.egg-info/top_level.txt
+drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-05-02 16:12:33.767467 word-search-generator-3.3.0/tests/
+-rw-r--r--   0 jbd        (501) staff       (20)    14859 2023-03-16 18:31:53.000000 word-search-generator-3.3.0/tests/__init__.py
+-rw-r--r--   0 jbd        (501) staff       (20)    15204 2023-03-16 18:23:55.000000 word-search-generator-3.3.0/tests/test_Mask.py
+-rw-r--r--   0 jbd        (501) staff       (20)     1188 2022-12-02 04:41:56.000000 word-search-generator-3.3.0/tests/test_Word.py
+-rw-r--r--   0 jbd        (501) staff       (20)    12465 2023-03-16 21:43:26.000000 word-search-generator-3.3.0/tests/test_WordSearch.py
+-rw-r--r--   0 jbd        (501) staff       (20)     5761 2023-03-16 18:25:31.000000 word-search-generator-3.3.0/tests/test_cli.py
+-rw-r--r--   0 jbd        (501) staff       (20)     8797 2023-03-06 05:02:24.000000 word-search-generator-3.3.0/tests/test_export.py
+-rw-r--r--   0 jbd        (501) staff       (20)     2556 2023-01-10 03:52:45.000000 word-search-generator-3.3.0/tests/test_generate.py
+-rw-r--r--   0 jbd        (501) staff       (20)     1317 2023-03-16 18:22:16.000000 word-search-generator-3.3.0/tests/test_shapes.py
+-rw-r--r--   0 jbd        (501) staff       (20)     2392 2023-03-15 21:02:57.000000 word-search-generator-3.3.0/tests/test_utils.py
+drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-05-02 16:12:33.778143 word-search-generator-3.3.0/tools/
+-rw-r--r--   0 jbd        (501) staff       (20)      385 2023-03-16 18:09:20.000000 word-search-generator-3.3.0/tools/build_masks_output_dict.py
+-rw-r--r--   0 jbd        (501) staff       (20)     1125 2023-01-03 03:25:46.000000 word-search-generator-3.3.0/tools/pdf_layout_testing.py
+drwxr-xr-x   0 jbd        (501) staff       (20)        0 2023-05-02 16:12:33.789590 word-search-generator-3.3.0/tools/sample_word_lists/
+-rw-r--r--   0 jbd        (501) staff       (20)       76 2021-08-19 05:15:03.000000 word-search-generator-3.3.0/tools/sample_word_lists/words-10.txt
+-rw-r--r--   0 jbd        (501) staff       (20)      173 2021-08-19 05:15:05.000000 word-search-generator-3.3.0/tools/sample_word_lists/words-25.txt
+-rw-r--r--   0 jbd        (501) staff       (20)       43 2021-08-19 05:15:01.000000 word-search-generator-3.3.0/tools/sample_word_lists/words-5.txt
+-rw-r--r--   0 jbd        (501) staff       (20)      369 2021-08-19 05:15:06.000000 word-search-generator-3.3.0/tools/sample_word_lists/words-50.txt
+-rw-r--r--   0 jbd        (501) staff       (20)       83 2021-08-19 05:15:08.000000 word-search-generator-3.3.0/tools/sample_word_lists/words-junk.txt
+-rw-r--r--   0 jbd        (501) staff       (20)      523 2023-03-06 05:02:24.000000 word-search-generator-3.3.0/tox.ini
```

### Comparing `word-search-generator-3.2.0/.github/workflows/tests.yml` & `word-search-generator-3.3.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.2.0/.gitignore` & `word-search-generator-3.3.0/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 *.db
 /tmp
 .env
 /artwork
 .pypirc
 .python-version
 .idea
+.ruff_cache
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 *.pyc
```

### Comparing `word-search-generator-3.2.0/.pre-commit-config.yaml` & `word-search-generator-3.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.2.0/CHANGLOG.md` & `word-search-generator-3.3.0/CHANGLOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,42 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [3.3.0] - 2023-05-02
+
+### Added
+
+- New pre-built mask shapes: [Club](https://github.com/joshbduncan/word-search-generator/wiki/Pre-Built-Mask-Shapes#Club), [Fish](https://github.com/joshbduncan/word-search-generator/wiki/Pre-Built-Mask-Shapes#Fish), [Flower](https://github.com/joshbduncan/word-search-generator/wiki/Pre-Built-Mask-Shapes#Flower), and [Spade](https://github.com/joshbduncan/word-search-generator/wiki/Pre-Built-Mask-Shapes#Spade)
+- Testing for built-in masks shapes based on known output
+- 'tools/build_masks_output_dict.py' tool for generating known built-in shapes output dict for us in testing
+
+### Fixed
+
+- During mask generation, each class and subclass now refers to their own `build_mask()` method instead of the base class.
+- Incorrect horizontal center calculation for `Spade` and `Club` masks on even sized masks.
+
+### Changed
+
+- The `.random_words()` method default to **NOT** resetting the puzzle size.
+- Radius calculation for the `RegularPolygon` mask.
+- If the `random_words()` method is called on an empty `WordSearch()` object, an appropriate puzzle size is calculated.
+- Cleaned up variable naming a bit to make things clear
+    - cli.py `BUILTIN_SHAPES` -> `BUILTIN_MASK_SHAPES_OBJECTS`
+    - shapes.py `MASK_SHAPES` -> `BUILTIN_MASK_SHAPES`
+- Cleaned up calculation of built-in shape objects
+- Cleaned up imports for 'test/__init__.py'
+- README and wiki mention puzzle masking.
+
+### Removed
+
+- `make_header()` function no longer needed as header is created with f-strings now
+
 ## [3.2.0] - 2023-03-06
 
 ### Changed
 
 - Moved build system from setup.cfg to pyproject.toml
 - Added [ruff](https://github.com/charliermarsh/ruff) to the dev tool set (plus tox, pre-commit)
     - Fixed all ruff suggestions
```

### Comparing `word-search-generator-3.2.0/LICENSE` & `word-search-generator-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.2.0/PKG-INFO` & `word-search-generator-3.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: word-search-generator
-Version: 3.2.0
+Version: 3.3.0
 Summary: Make awesome Word Search puzzles
 Author-email: Josh Duncan <joshbduncan@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/joshbduncan/word-search-generator
 Project-URL: documentation, https://github.com/joshbduncan/word-search-generator/wiki
 Project-URL: repository, https://github.com/joshbduncan/word-search-generator.git
 Project-URL: changelog, https://github.com/joshbduncan/word-search-generator/blob/main/CHANGLOG.md
@@ -150,24 +150,53 @@
 >>> from word_search_generator import WordSearch
 >>> puzzle = WordSearch(level=3)
 >>> puzzle.random_words(10, secret=True, reset_size=True)
 ```
 
 😓 Too hard? Go the easy route with `puzzle.level = 1` or `puzzle.directions = "E"`.
 
+🎭 How about adding a mask ([docs](https://github.com/joshbduncan/word-search-generator/wiki/Puzzle-Masking))? ...Fancy!
+
+```pycon
+>>> from word_search_generator.mask.shapes import Heart
+>>> puzzle.apply_mask(Heart())
+>>> puzzle.show()
+-------------------------
+       WORD SEARCH
+-------------------------
+    C L C       C Y E
+  Q S T N S   T E L D K
+Z L O Z T P A K T H N M W
+C C L Q C O N R S P Z V U
+M I X V G O U R H S Z C H
+  M H K D T T L E C U Q
+  H C T H O R S E B M
+    Z I S W R B P E G
+      Y P I G B X Q
+        C A T N G
+        A R W O
+          K D Q
+            A
+
+Find these words: CAT, DOG, DONKEY, GOAT, HORSE, PIG, SHEEP, TURTLE
+* Words can go S, NE, E, and, SE.
+
+Answer Key: CAT E @ (5, 10), DOG NE @ (7, 12), DONKEY NE @ (5, 6), GOAT NE @ (5, 5), HORSE E @ (5, 7), PIG E @ (5, 9), SHEEP S @ (9, 4), TURTLE NE @ (6, 6)
+```
+
 💾 Save your AWESOME puzzle as a PDF.
 
 ```pycon
 >>> puzzle.save(path="~/Desktop/puzzle.pdf")
 >>> "~/Desktop/puzzle.pdf"
 ```
 
 ## 🖥 CLI Integration
 
-You can play WordSearch in your CLI too! WordSearch Generator installs the console entry-point `word-search` so you can interact with the package right in your console.
+You can play WordSearch in your CLI too ([docs](https://github.com/joshbduncan/word-search-generator/wiki/Command-Line-Interface-(CLI)))! WordSearch Generator installs the console entry-point `word-search` so you can interact with the package right in your console.
 
 ```bash
 $ word-search -r 10 -s 15 -l 3
 -----------------------------
          WORD SEARCH
 -----------------------------
 J W X O X N A Q C A Q Z D R G
@@ -188,8 +217,12 @@
 
 Find these words: AFTER, BABY, BRING, DEAL, KIND, MODERN, MYSELF, PURPOSE, RATE, THESE
 * Words can go N, S, SW, W, E, NW, NE, and, SE.
 
 Answer Key: AFTER S @ (13, 8), BABY E @ (6, 13), BRING S @ (8, 5), DEAL N @ (1, 12), KIND SW @ (14, 2), MODERN NE @ (3, 15), MYSELF E @ (4, 2), PURPOSE S @ (14, 7), RATE SW @ (14, 1), THESE E @ (8, 12)
 ```
 
+## 📔 Documentation
+
+If you need more info, most of the fun parts of Word-Search-Generator are documented on Github in the [Project Wiki](https://github.com/joshbduncan/word-search-generator/wiki).
+
 Happy WordSearching ✌️
```

### Comparing `word-search-generator-3.2.0/README.md` & `word-search-generator-3.3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -125,24 +125,53 @@
 >>> from word_search_generator import WordSearch
 >>> puzzle = WordSearch(level=3)
 >>> puzzle.random_words(10, secret=True, reset_size=True)
 ```
 
 😓 Too hard? Go the easy route with `puzzle.level = 1` or `puzzle.directions = "E"`.
 
+🎭 How about adding a mask ([docs](https://github.com/joshbduncan/word-search-generator/wiki/Puzzle-Masking))? ...Fancy!
+
+```pycon
+>>> from word_search_generator.mask.shapes import Heart
+>>> puzzle.apply_mask(Heart())
+>>> puzzle.show()
+-------------------------
+       WORD SEARCH
+-------------------------
+    C L C       C Y E
+  Q S T N S   T E L D K
+Z L O Z T P A K T H N M W
+C C L Q C O N R S P Z V U
+M I X V G O U R H S Z C H
+  M H K D T T L E C U Q
+  H C T H O R S E B M
+    Z I S W R B P E G
+      Y P I G B X Q
+        C A T N G
+        A R W O
+          K D Q
+            A
+
+Find these words: CAT, DOG, DONKEY, GOAT, HORSE, PIG, SHEEP, TURTLE
+* Words can go S, NE, E, and, SE.
+
+Answer Key: CAT E @ (5, 10), DOG NE @ (7, 12), DONKEY NE @ (5, 6), GOAT NE @ (5, 5), HORSE E @ (5, 7), PIG E @ (5, 9), SHEEP S @ (9, 4), TURTLE NE @ (6, 6)
+```
+
 💾 Save your AWESOME puzzle as a PDF.
 
 ```pycon
 >>> puzzle.save(path="~/Desktop/puzzle.pdf")
 >>> "~/Desktop/puzzle.pdf"
 ```
 
 ## 🖥 CLI Integration
 
-You can play WordSearch in your CLI too! WordSearch Generator installs the console entry-point `word-search` so you can interact with the package right in your console.
+You can play WordSearch in your CLI too ([docs](https://github.com/joshbduncan/word-search-generator/wiki/Command-Line-Interface-(CLI)))! WordSearch Generator installs the console entry-point `word-search` so you can interact with the package right in your console.
 
 ```bash
 $ word-search -r 10 -s 15 -l 3
 -----------------------------
          WORD SEARCH
 -----------------------------
 J W X O X N A Q C A Q Z D R G
@@ -163,8 +192,12 @@
 
 Find these words: AFTER, BABY, BRING, DEAL, KIND, MODERN, MYSELF, PURPOSE, RATE, THESE
 * Words can go N, S, SW, W, E, NW, NE, and, SE.
 
 Answer Key: AFTER S @ (13, 8), BABY E @ (6, 13), BRING S @ (8, 5), DEAL N @ (1, 12), KIND SW @ (14, 2), MODERN NE @ (3, 15), MYSELF E @ (4, 2), PURPOSE S @ (14, 7), RATE SW @ (14, 1), THESE E @ (8, 12)
 ```
 
+## 📔 Documentation
+
+If you need more info, most of the fun parts of Word-Search-Generator are documented on Github in the [Project Wiki](https://github.com/joshbduncan/word-search-generator/wiki).
+
 Happy WordSearching ✌️
```

### Comparing `word-search-generator-3.2.0/pyproject.toml` & `word-search-generator-3.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -91,10 +91,12 @@
 fixable = ["B", "I"]
 format = "grouped"
 line-length = 88
 show-fixes = true
 src = ["src", "test"]
 target-version = "py37"
 
-# Ignore `E402` (import violations) in all `__init__.py` files, and in `path/to/file.py`.
 [tool.ruff.per-file-ignores]
+# Ignore `E402` (import violations) in all `__init__.py`.
 "__init__.py" = ["E402"]
+# Ignore `TCH004` in `bitmap.py` (https://github.com/charliermarsh/ruff/issues/2852).
+"src/word_search_generator/mask/bitmap.py" = ["TCH004"]
```

### Comparing `word-search-generator-3.2.0/run` & `word-search-generator-3.3.0/run`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.2.0/src/word_search_generator/__init__.py` & `word-search-generator-3.3.0/src/word_search_generator/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     Generate Word Search puzzles with Python.
     -----------
     :copyright: (c) 2021 Josh Duncan.
     :license: MIT, see LICENSE for more details.
 """
 
 __app_name__ = "word-search"
-__version__ = "3.2.0"
+__version__ = "3.3.0"
 
 
 import json
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Set
 
 from . import export, generate, utils
@@ -308,27 +308,27 @@
     # ************************************************* #
 
     def random_words(
         self,
         count: int,
         action: str = "REPLACE",
         secret: bool = False,
-        reset_size: bool = True,
+        reset_size: bool = False,
     ) -> None:
         """Add `count` randomly generated words to the puzzle.
 
         Args:
             count (int): Count of random words to add.
             action (str): Should the random words be added ("ADD") to the current
                 wordlist or should they replace ("REPLACE") the current wordlist.
                 Defaults to "REPLACE".
             secret (bool, optional): Should the new words
                 be secret. Defaults to False.
             reset_size (bool, optional): Reset the puzzle
-                size based on the updated words. Defaults to True.
+                size based on the updated words. Defaults to False.
 
         Raises:
             TypeError: Must be an integer.
             ValueError: Must be greater than `config.min_puzzle_words` and
             less than `config.max_puzzle_words`.
         """
         if not isinstance(count, int):
@@ -411,16 +411,20 @@
 
     def _generate(self, fill_puzzle: bool = True) -> None:
         """Generate the puzzle grid."""
         self._puzzle = utils.build_puzzle(self.size, "")
         min_word_length = (
             min([len(word.text) for word in self.words]) if self.words else self.size
         )
-        if self.size < min_word_length:
+        if self.size and self.size < min_word_length:
             raise PuzzleSizeError
+        # if an empty puzzle object is created then the `random_words()` method
+        # is called set the calculate an appropriate puzzle size
+        if not self.size:
+            self.reset_size()
         for word in self.words:
             word.remove_from_puzzle()
         if not self.mask or len(self.mask) != self.size:
             self._mask = utils.build_puzzle(self.size, ACTIVE)
         if fill_puzzle:
             self._fill_puzzle()
         if self.force_all_words and self.unplaced_hidden_words:
```

### Comparing `word-search-generator-3.2.0/src/word_search_generator/cli.py` & `word-search-generator-3.3.0/src/word_search_generator/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .mask.bitmap import Image
 from .word import Direction
 
 if TYPE_CHECKING:  # pragma: no cover
     from typing import Sequence
 
 
-BUILTIN_SHAPES = shapes.get_shape_objects()
+BUILTIN_MASK_SHAPES_OBJECTS = shapes.get_shape_objects()
 
 
 class RandomAction(argparse.Action):
     """Restrict argparse `-r`, `--random` inputs."""
 
     def __call__(self, parser, namespace, values, option_string=None):
         min_val = config.min_puzzle_words
@@ -119,18 +119,18 @@
         type=pathlib.Path,
         help="Mask the puzzle to a provided image \
 (accepts: BMP, JPEG, PNG).",
     )
     mask_group.add_argument(
         "-m",
         "--mask",
-        choices=BUILTIN_SHAPES,
+        choices=BUILTIN_MASK_SHAPES_OBJECTS,
         metavar="MASK_SHAPE",
         help=f"Mask the puzzle to a shape \
-(choices: {', '.join(BUILTIN_SHAPES)}).",
+(choices: {', '.join(BUILTIN_MASK_SHAPES_OBJECTS)}).",
     )
     parser.add_argument(
         "-o",
         "--output",
         type=pathlib.Path,
         help="Output path for the saved puzzle.",
     )
@@ -179,15 +179,15 @@
         "--version", action="version", version=f"%(prog)s {__version__}"
     )
     args = parser.parse_args(argv)
 
     # check for mask preview first
     if args.preview_masks:
         preview_size = 21
-        for shape in BUILTIN_SHAPES:
+        for shape in BUILTIN_MASK_SHAPES_OBJECTS:
             mask = eval(f"shapes.{shape}")()
             mask.generate(preview_size)
             print(f"{shape}")
             mask.show(True)
             print()
         return 0
```

### Comparing `word-search-generator-3.2.0/src/word_search_generator/config.py` & `word-search-generator-3.3.0/src/word_search_generator/config.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.2.0/src/word_search_generator/export.py` & `word-search-generator-3.3.0/src/word_search_generator/export.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.2.0/src/word_search_generator/generate.py` & `word-search-generator-3.3.0/src/word_search_generator/generate.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.2.0/src/word_search_generator/mask/__init__.py` & `word-search-generator-3.3.0/src/word_search_generator/mask/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         """
         return [[char] * size for _ in range(size)]
 
     def generate(self, puzzle_size: int) -> None:
         """Generate a new mask at `puzzle_size` and either fill points (`Bitmap`),
         or connect points (`Polygon`) and then fill the resulting polygon shape."""
         self.puzzle_size = puzzle_size
-        self._mask = Mask.build_mask(self.puzzle_size)
+        self._mask = self.build_mask(self.puzzle_size)
         self._draw()
 
     def _draw(self) -> None:
         """Placeholder for custom subclass `_draw()` methods.
 
         Raises:
             MaskNotGenerated: Mask has not yet been generated.
@@ -266,15 +266,15 @@
     def generate(self, puzzle_size: int) -> None:
         """Generate a new mask at `puzzle_size` and the apply all Mask objects
         from `CompoundMask.masks` in order.
 
         Note: Unlike the parent `Mask` object a `CompoundMask` is initially filled
         with `config.ACTIVE`. This allows for the proper inaction between masks."""
         self.puzzle_size = puzzle_size
-        self._mask = Mask.build_mask(self.puzzle_size, ACTIVE)
+        self._mask = self.build_mask(self.puzzle_size, ACTIVE)
         for mask in self.masks:
             mask.generate(self.puzzle_size)
             self._apply_mask(mask)
 
     def _apply_mask(self, mask: Mask) -> None:
         """Apply `Mask` to the compound mask.
```

### Comparing `word-search-generator-3.2.0/src/word_search_generator/mask/bitmap.py` & `word-search-generator-3.3.0/src/word_search_generator/mask/bitmap.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         """
         super().__init__(method=method, static=static)
         self.fp = fp
 
     def generate(self, puzzle_size: int) -> None:
         """Generate a new mask at `puzzle_size` from a raster image."""
         self.puzzle_size = puzzle_size
-        self._mask = Mask.build_mask(self.puzzle_size)
+        self._mask = self.build_mask(self.puzzle_size)
         self.points = Image.process_image(
             PILImage.open(self.fp, formats=("BMP", "JPEG", "PNG")),
             self.puzzle_size,
             Image.threshold,
         )
         if not self.points:
             raise ContrastError("The provided image lacked enough contrast.")
```

### Comparing `word-search-generator-3.2.0/src/word_search_generator/mask/ellipse.py` & `word-search-generator-3.3.0/src/word_search_generator/mask/ellipse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import math
 from typing import List, Optional, Tuple
 
 from ..utils import distance, float_range
-from . import Mask
 from .bitmap import Bitmap
 
 
 class Ellipse(Bitmap):
     """This class represents a subclass of the Bitmap object
     and generates an Ellipse masks."""
 
@@ -36,15 +35,15 @@
         self.width = width
         self.height = height
         self.center = center
 
     def generate(self, puzzle_size: int) -> None:
         """Generate a new mask at `puzzle_size`."""
         self.puzzle_size = puzzle_size
-        self._mask = Mask.build_mask(self.puzzle_size)
+        self._mask = self.build_mask(self.puzzle_size)
         self.points = Ellipse.calculate_ellipse_points(
             self.width if self.width else self.puzzle_size,
             self.height if self.height else self.puzzle_size,
             self.center
             if self.center
             else (self.puzzle_size // 2, self.puzzle_size // 2),
             puzzle_size,
```

### Comparing `word-search-generator-3.2.0/src/word_search_generator/mask/polygon.py` & `word-search-generator-3.3.0/src/word_search_generator/mask/polygon.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         right_offset = len(self.points) // 2
         right_side = [self.points[0]] + list(reversed(self.points))[:right_offset]
         return left_side, right_side
 
     def generate(self, puzzle_size: int) -> None:
         """Generate a new mask at `puzzle_size`."""
         self.puzzle_size = puzzle_size
-        self._mask = Mask.build_mask(self.puzzle_size)
+        self._mask = self.build_mask(self.puzzle_size)
         self._draw()
 
     def _draw(self) -> None:  # doesn't draw evenly on second half pf point (going up)
         """Connect each coordinate point within `.points` in the
         order they are listed and then fill in the resulting shape."""
         for i in range(len(self.points)):
             p1 = self.points[i]
@@ -229,23 +229,28 @@
         self.vertices = vertices
         self.radius = radius
         self.center = center
         self.angle = angle
 
     def generate(self, puzzle_size: int) -> None:
         self.puzzle_size = puzzle_size
-        self._mask = Mask.build_mask(self.puzzle_size)
+        self._mask = self.build_mask(self.puzzle_size)
         radius = (
-            self.puzzle_size // 2 - 1 if puzzle_size % 2 == 0 else self.puzzle_size // 2
+            self.radius
+            if self.radius
+            else (
+                self.puzzle_size // 2 - 1
+                if puzzle_size % 2 == 0
+                else self.puzzle_size // 2
+            )
         )
-        center = (radius, radius)
         self.points = RegularPolygon.calculate_vertices(
             self.vertices,
-            self.radius if self.radius else radius,
-            self.center if self.center else center,
+            radius,
+            self.center if self.center else (radius, radius),
             self.angle,
         )
         self._draw()
 
     @staticmethod
     def calculate_vertices(
         vertices: int,
@@ -323,15 +328,15 @@
         self.outer_radius = outer_radius
         self.inner_radius = inner_radius
         self.center = center
         self.angle = angle
 
     def generate(self, puzzle_size: int) -> None:
         self.puzzle_size = puzzle_size
-        self._mask = Mask.build_mask(self.puzzle_size)
+        self._mask = self.build_mask(self.puzzle_size)
         puzzle_radius = (
             self.puzzle_size // 2 - 1 if puzzle_size % 2 == 0 else self.puzzle_size // 2
         )
         puzzle_center = (puzzle_radius, puzzle_radius)
         self.points = Star.calculate_vertices(
             self.outer_vertices,
             self.outer_radius if self.outer_radius else puzzle_radius,
```

### Comparing `word-search-generator-3.2.0/src/word_search_generator/utils.py` & `word-search-generator-3.3.0/src/word_search_generator/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,15 @@
     shortest_word_length = len(min(all_words, key=len))
     if not size:
         longest = max(10, longest_word_length)
         # calculate multiplier for larger word lists so that most have room to fit
         multiplier = len(all_words) / 15 if len(all_words) > 15 else 1
         # level lengths in config.py are nice multiples of 2
         l_size = log2(len(level)) if level else 1  # protect against log(0) in tests
-        size = round(longest + l_size * 2 * multiplier)
-        if size > config.max_puzzle_size:
-            size = config.max_puzzle_size
+        size = min(round(longest + l_size * 2 * multiplier), config.max_puzzle_size)
     else:
         if size < shortest_word_length:
             print(
                 "Puzzle sized adjust to fit word with the shortest length.",
                 file=sys.stderr,
             )
             size = shortest_word_length + 1
@@ -137,15 +135,15 @@
     if not word_set:
         raise ValueError("Use words longer than one-character and without punctuation.")
     return word_set
 
 
 def contains_punctuation(word):
     """Check to see if punctuation is present in the provided string."""
-    return any([bool(c in string.punctuation) for c in word])
+    return any(bool(c in string.punctuation) for c in word)
 
 
 def is_palindrome(word: str) -> bool:
     """Check is a word in a palindrome."""
     return word == word[::-1]
 
 
@@ -221,23 +219,14 @@
         for char in word.text:
             output[y][x] = f"\u001b[1m\u001b[31m{char}\u001b[0m"
             x += word.direction.c_move
             y += word.direction.r_move
     return output
 
 
-def make_header(size: int, text: str) -> str:
-    """Generate a header that fits the current puzzle size."""
-    hr = "-" * max(11, (size * 2 - 1))
-    padding = " " * ((len(hr) - len(text)) // 2)
-    return f"""{hr}
-{padding}{text}{padding}
-{hr}"""
-
-
 def stringify(puzzle: Puzzle, bbox: tuple[tuple[int, int], tuple[int, int]]) -> str:
     """Convert puzzle array of nested lists into a string."""
     min_x, min_y = bbox[0]
     max_x, max_y = bbox[1]
     output = []
     offset = " " if max_x - min_x < 5 else ""
     for line in puzzle[min_y : max_y + 1]:
@@ -248,16 +237,17 @@
 
 
 def format_puzzle_for_show(ws: WordSearch, show_solution: bool = False) -> str:
     word_list = get_word_list_str(ws.key)
     # highlight solution if provided
     puzzle_list = highlight_solution(ws) if show_solution else ws.puzzle
     # calculate header length based on cropped puzzle size to account for masks
-    header_width = ws.bounding_box[1][0] - ws.bounding_box[0][0] + 1
-    header = make_header(header_width, "WORD SEARCH")
+    header_width = max(11, (ws.bounding_box[1][0] - ws.bounding_box[0][0] + 1) * 2 - 1)
+    hr = "-" * header_width
+    header = hr + "\n" + f"{'WORD SEARCH':^{header_width}}" + "\n" + hr
     answer_key_intro = (
         "Answer Key (*Secret Words)" if ws.placed_secret_words else "Answer Key"
     )
     return f"""{header}
 {stringify(puzzle_list, ws.bounding_box)}
 
 Find these words: {word_list if word_list else '<ALL SECRET WORDS>'}
```

### Comparing `word-search-generator-3.2.0/src/word_search_generator/word/__init__.py` & `word-search-generator-3.3.0/src/word_search_generator/word/__init__.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.2.0/src/word_search_generator.egg-info/PKG-INFO` & `word-search-generator-3.3.0/src/word_search_generator.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: word-search-generator
-Version: 3.2.0
+Version: 3.3.0
 Summary: Make awesome Word Search puzzles
 Author-email: Josh Duncan <joshbduncan@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/joshbduncan/word-search-generator
 Project-URL: documentation, https://github.com/joshbduncan/word-search-generator/wiki
 Project-URL: repository, https://github.com/joshbduncan/word-search-generator.git
 Project-URL: changelog, https://github.com/joshbduncan/word-search-generator/blob/main/CHANGLOG.md
@@ -150,24 +150,53 @@
 >>> from word_search_generator import WordSearch
 >>> puzzle = WordSearch(level=3)
 >>> puzzle.random_words(10, secret=True, reset_size=True)
 ```
 
 😓 Too hard? Go the easy route with `puzzle.level = 1` or `puzzle.directions = "E"`.
 
+🎭 How about adding a mask ([docs](https://github.com/joshbduncan/word-search-generator/wiki/Puzzle-Masking))? ...Fancy!
+
+```pycon
+>>> from word_search_generator.mask.shapes import Heart
+>>> puzzle.apply_mask(Heart())
+>>> puzzle.show()
+-------------------------
+       WORD SEARCH
+-------------------------
+    C L C       C Y E
+  Q S T N S   T E L D K
+Z L O Z T P A K T H N M W
+C C L Q C O N R S P Z V U
+M I X V G O U R H S Z C H
+  M H K D T T L E C U Q
+  H C T H O R S E B M
+    Z I S W R B P E G
+      Y P I G B X Q
+        C A T N G
+        A R W O
+          K D Q
+            A
+
+Find these words: CAT, DOG, DONKEY, GOAT, HORSE, PIG, SHEEP, TURTLE
+* Words can go S, NE, E, and, SE.
+
+Answer Key: CAT E @ (5, 10), DOG NE @ (7, 12), DONKEY NE @ (5, 6), GOAT NE @ (5, 5), HORSE E @ (5, 7), PIG E @ (5, 9), SHEEP S @ (9, 4), TURTLE NE @ (6, 6)
+```
+
 💾 Save your AWESOME puzzle as a PDF.
 
 ```pycon
 >>> puzzle.save(path="~/Desktop/puzzle.pdf")
 >>> "~/Desktop/puzzle.pdf"
 ```
 
 ## 🖥 CLI Integration
 
-You can play WordSearch in your CLI too! WordSearch Generator installs the console entry-point `word-search` so you can interact with the package right in your console.
+You can play WordSearch in your CLI too ([docs](https://github.com/joshbduncan/word-search-generator/wiki/Command-Line-Interface-(CLI)))! WordSearch Generator installs the console entry-point `word-search` so you can interact with the package right in your console.
 
 ```bash
 $ word-search -r 10 -s 15 -l 3
 -----------------------------
          WORD SEARCH
 -----------------------------
 J W X O X N A Q C A Q Z D R G
@@ -188,8 +217,12 @@
 
 Find these words: AFTER, BABY, BRING, DEAL, KIND, MODERN, MYSELF, PURPOSE, RATE, THESE
 * Words can go N, S, SW, W, E, NW, NE, and, SE.
 
 Answer Key: AFTER S @ (13, 8), BABY E @ (6, 13), BRING S @ (8, 5), DEAL N @ (1, 12), KIND SW @ (14, 2), MODERN NE @ (3, 15), MYSELF E @ (4, 2), PURPOSE S @ (14, 7), RATE SW @ (14, 1), THESE E @ (8, 12)
 ```
 
+## 📔 Documentation
+
+If you need more info, most of the fun parts of Word-Search-Generator are documented on Github in the [Project Wiki](https://github.com/joshbduncan/word-search-generator/wiki).
+
 Happy WordSearching ✌️
```

### Comparing `word-search-generator-3.2.0/src/word_search_generator.egg-info/SOURCES.txt` & `word-search-generator-3.3.0/src/word_search_generator.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 .flake8
 .gitignore
 .pre-commit-config.yaml
 CHANGLOG.md
 LICENSE
 README.md
+TODO.md
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 run
 setup.py
 tox.ini
 .github/workflows/tests.yml
@@ -34,14 +35,16 @@
 tests/__init__.py
 tests/test_Mask.py
 tests/test_Word.py
 tests/test_WordSearch.py
 tests/test_cli.py
 tests/test_export.py
 tests/test_generate.py
+tests/test_shapes.py
 tests/test_utils.py
+tools/build_masks_output_dict.py
 tools/pdf_layout_testing.py
 tools/sample_word_lists/words-10.txt
 tools/sample_word_lists/words-25.txt
 tools/sample_word_lists/words-5.txt
 tools/sample_word_lists/words-50.txt
 tools/sample_word_lists/words-junk.txt
```

### Comparing `word-search-generator-3.2.0/tests/test_Mask.py` & `word-search-generator-3.3.0/tests/test_Mask.py`

 * *Files 2% similar despite different names*

```diff
@@ -405,20 +405,26 @@
 
 def test_connect_points_no_generated():
     pm = Polygon()
     with pytest.raises(MaskNotGenerated):
         pm._connect_points((0, 0), (1, 1))
 
 
-def test_fill_shape_no_generated():
+def test_fill_shape_not_generated():
     pm = Polygon()
     with pytest.raises(MaskNotGenerated):
         pm._fill_shape("J")
 
 
+def test_generate_method_no_size():
+    m = Mask()
+    with pytest.raises(TypeError):
+        m.generate()  # type: ignore
+
+
 def test_regular_polygon_too_few_vertices():
     with pytest.raises(ValueError):
         pm = RegularPolygon(2)  # noqa: F841
 
 
 def test_star_polygon_too_few_vertices():
     with pytest.raises(ValueError):
```

### Comparing `word-search-generator-3.2.0/tests/test_Word.py` & `word-search-generator-3.3.0/tests/test_Word.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.2.0/tests/test_WordSearch.py` & `word-search-generator-3.3.0/tests/test_WordSearch.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,25 @@
 
 import pytest
 
 from word_search_generator import (
     Key,
     MissingWordError,
     Puzzle,
-    PuzzleNotGeneratedError,
     PuzzleSizeError,
     WordSearch,
     config,
     utils,
 )
 from word_search_generator.config import level_dirs
-from word_search_generator.mask.polygon import Rectangle, Star
+from word_search_generator.mask.polygon import Rectangle
 from word_search_generator.utils import get_random_words
 from word_search_generator.word import Direction, Word
 
-from . import ITERATIONS, MASKS, WORDS
+from . import BUILTIN_MASK_SHAPES_OBJECTS, ITERATIONS, WORDS
 
 
 def check_chars(puzzle, word):
     row, col = word.position
     for c in word.text:
         if c != puzzle[row][col]:
             return False
@@ -486,26 +485,20 @@
     assert ws.puzzle[1][1] == ws.cropped_puzzle[0][0]
     assert ws.puzzle[size - 10][size - 10] == ws.cropped_puzzle[size - 11][size - 11]
 
 
 def test_word_placement():
     results = []
     for _ in range(ITERATIONS):
-        p = WordSearch(size=random.randint(8, 21))
+        p = WordSearch(size=random.randint(21, 35))
         p.random_words(random.randint(5, 21))
-        mask = random.choice(MASKS)
+        mask = random.choice(BUILTIN_MASK_SHAPES_OBJECTS)
         if mask:
             p.apply_mask(mask)
         results.append(all(check_chars(p.puzzle, word) for word in p.placed_words))
     assert all(results)
 
 
 def test_puzzle_size_error():
     p = WordSearch("abracadabra")
     with pytest.raises(PuzzleSizeError):
         p.size = 5
-
-
-def test_not_generated_error():
-    p = WordSearch(size=21)
-    with pytest.raises(PuzzleNotGeneratedError):
-        p.apply_mask(Star())
```

### Comparing `word-search-generator-3.2.0/tests/test_cli.py` & `word-search-generator-3.3.0/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import subprocess
 from pathlib import Path
 
 from PIL import Image
 
 from word_search_generator.word import Direction, Word
 
-from . import ITERATIONS, MASKS
+from . import BUILTIN_MASK_SHAPES_OBJECTS, ITERATIONS
 
 
 def check_chars(puzzle, word):
     row, col = word.position
     for c in word.text:
         if c != puzzle[row][col]:
             return False
@@ -174,17 +174,17 @@
             word.start_row = int(data[4]) - 1
             word.start_column = int(data[3]) - 1
             words.add(word)
         return words
 
     results = []
     for _ in range(ITERATIONS):
-        size = random.randint(8, 21)
+        size = random.randint(18, 36)
         words = random.randint(5, 21)
-        mask = random.choice(MASKS)
+        mask = random.choice(BUILTIN_MASK_SHAPES_OBJECTS)
         command = f"word-search -r {words} -s {size}"
         if mask:
             command += f" -m {mask.__class__.__name__}"
         output = subprocess.check_output(command, shell=True, text=True)
         puzzle = parse_puzzle(output)
         words = parse_words(output)
         results.append(all(check_chars(puzzle, word) for word in words))  # type: ignore
```

### Comparing `word-search-generator-3.2.0/tests/test_export.py` & `word-search-generator-3.3.0/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.2.0/tests/test_generate.py` & `word-search-generator-3.3.0/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.2.0/tests/test_utils.py` & `word-search-generator-3.3.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.2.0/tools/pdf_layout_testing.py` & `word-search-generator-3.3.0/tools/pdf_layout_testing.py`

 * *Files identical despite different names*

### Comparing `word-search-generator-3.2.0/tox.ini` & `word-search-generator-3.3.0/tox.ini`

 * *Files identical despite different names*

