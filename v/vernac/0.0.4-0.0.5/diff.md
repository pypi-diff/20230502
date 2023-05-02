# Comparing `tmp/vernac-0.0.4.tar.gz` & `tmp/vernac-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vernac-0.0.4.tar", last modified: Sat Apr 15 17:43:18 2023, max compression
+gzip compressed data, was "vernac-0.0.5.tar", last modified: Tue May  2 00:40:49 2023, max compression
```

## Comparing `vernac-0.0.4.tar` & `vernac-0.0.5.tar`

### file list

```diff
@@ -1,33 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:43:18.337872 vernac-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:43:18.333872 vernac-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:43:18.337872 vernac-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-15 17:43:04.000000 vernac-0.0.4/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-15 17:43:04.000000 vernac-0.0.4/.github/workflows/test-some-examples.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-15 17:43:04.000000 vernac-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-15 17:43:04.000000 vernac-0.0.4/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-15 17:43:04.000000 vernac-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-15 17:43:18.337872 vernac-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-15 17:43:04.000000 vernac-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-15 17:43:04.000000 vernac-0.0.4/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:43:18.333872 vernac-0.0.4/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:43:18.337872 vernac-0.0.4/examples/reliable/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-15 17:43:04.000000 vernac-0.0.4/examples/reliable/benchmark.vn
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-15 17:43:04.000000 vernac-0.0.4/examples/reliable/fizzbuzz.vn
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-15 17:43:04.000000 vernac-0.0.4/examples/reliable/mergesort.vn
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:43:18.337872 vernac-0.0.4/examples/unreliable/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-15 17:43:04.000000 vernac-0.0.4/examples/unreliable/count_gpt_titles.vn
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-15 17:43:04.000000 vernac-0.0.4/examples/unreliable/hntoday.vn
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-15 17:43:04.000000 vernac-0.0.4/examples/unreliable/snake.vn
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-15 17:43:04.000000 vernac-0.0.4/local-dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-15 17:43:04.000000 vernac-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 17:43:18.337872 vernac-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:43:18.333872 vernac-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:43:18.337872 vernac-0.0.4/src/vernac/
--rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-04-15 17:43:04.000000 vernac-0.0.4/src/vernac/compile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:43:18.337872 vernac-0.0.4/src/vernac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-15 17:43:18.000000 vernac-0.0.4/src/vernac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-15 17:43:18.000000 vernac-0.0.4/src/vernac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 17:43:18.000000 vernac-0.0.4/src/vernac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-15 17:43:18.000000 vernac-0.0.4/src/vernac.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-15 17:43:18.000000 vernac-0.0.4/src/vernac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-15 17:43:18.000000 vernac-0.0.4/src/vernac.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:40:49.553106 vernac-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:40:49.533105 vernac-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:40:49.541105 vernac-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-02 00:40:37.000000 vernac-0.0.5/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-02 00:40:37.000000 vernac-0.0.5/.github/workflows/run-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-02 00:40:37.000000 vernac-0.0.5/.github/workflows/test-some-examples.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-02 00:40:37.000000 vernac-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-02 00:40:37.000000 vernac-0.0.5/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-02 00:40:37.000000 vernac-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-05-02 00:40:49.553106 vernac-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-02 00:40:37.000000 vernac-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-02 00:40:37.000000 vernac-0.0.5/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:40:49.533105 vernac-0.0.5/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:40:49.541105 vernac-0.0.5/examples/reliable/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-02 00:40:37.000000 vernac-0.0.5/examples/reliable/benchmark.vn
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-02 00:40:37.000000 vernac-0.0.5/examples/reliable/emoji.vn
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-02 00:40:37.000000 vernac-0.0.5/examples/reliable/fizzbuzz-with-test-buggy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-02 00:40:37.000000 vernac-0.0.5/examples/reliable/fizzbuzz-with-test.vn
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-02 00:40:37.000000 vernac-0.0.5/examples/reliable/fizzbuzz.vn
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-02 00:40:37.000000 vernac-0.0.5/examples/reliable/hngpt-with-test.vn
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-02 00:40:37.000000 vernac-0.0.5/examples/reliable/hngpt.vn
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-02 00:40:37.000000 vernac-0.0.5/examples/reliable/mergesort.vn
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-02 00:40:37.000000 vernac-0.0.5/examples/reliable/todo-cli.vn
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:40:49.545106 vernac-0.0.5/examples/reliable/todo-tui/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-02 00:40:37.000000 vernac-0.0.5/examples/reliable/todo-tui/todo-storage.vn
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-02 00:40:37.000000 vernac-0.0.5/examples/reliable/todo-tui/todo-tui.vn
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:40:49.545106 vernac-0.0.5/examples/unreliable/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-02 00:40:37.000000 vernac-0.0.5/examples/unreliable/count_gpt_titles.vn
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-02 00:40:37.000000 vernac-0.0.5/examples/unreliable/hntoday.vn
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-02 00:40:37.000000 vernac-0.0.5/examples/unreliable/snake.vn
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-02 00:40:37.000000 vernac-0.0.5/local-dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-02 00:40:37.000000 vernac-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 00:40:49.553106 vernac-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:40:49.537105 vernac-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:40:49.545106 vernac-0.0.5/src/vernac/
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-02 00:40:37.000000 vernac-0.0.5/src/vernac/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-02 00:40:37.000000 vernac-0.0.5/src/vernac/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-02 00:40:37.000000 vernac-0.0.5/src/vernac/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:40:49.553106 vernac-0.0.5/src/vernac/stages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 00:40:37.000000 vernac-0.0.5/src/vernac/stages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-02 00:40:37.000000 vernac-0.0.5/src/vernac/stages/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-02 00:40:37.000000 vernac-0.0.5/src/vernac/stages/check_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-05-02 00:40:37.000000 vernac-0.0.5/src/vernac/stages/check_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-02 00:40:37.000000 vernac-0.0.5/src/vernac/stages/document_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-05-02 00:40:37.000000 vernac-0.0.5/src/vernac/stages/generate_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-02 00:40:37.000000 vernac-0.0.5/src/vernac/stages/guess_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-02 00:40:37.000000 vernac-0.0.5/src/vernac/stages/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-02 00:40:37.000000 vernac-0.0.5/src/vernac/stages/map_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-05-02 00:40:37.000000 vernac-0.0.5/src/vernac/stages/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-02 00:40:37.000000 vernac-0.0.5/src/vernac/stages/read_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-05-02 00:40:37.000000 vernac-0.0.5/src/vernac/stages/run_pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:40:49.553106 vernac-0.0.5/src/vernac/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 00:40:37.000000 vernac-0.0.5/src/vernac/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-02 00:40:37.000000 vernac-0.0.5/src/vernac/test/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-02 00:40:37.000000 vernac-0.0.5/src/vernac/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:40:49.549106 vernac-0.0.5/src/vernac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-05-02 00:40:49.000000 vernac-0.0.5/src/vernac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-02 00:40:49.000000 vernac-0.0.5/src/vernac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 00:40:49.000000 vernac-0.0.5/src/vernac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-02 00:40:49.000000 vernac-0.0.5/src/vernac.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-02 00:40:49.000000 vernac-0.0.5/src/vernac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 00:40:49.000000 vernac-0.0.5/src/vernac.egg-info/top_level.txt
```

### Comparing `vernac-0.0.4/.github/workflows/publish-to-pypi.yml` & `vernac-0.0.5/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `vernac-0.0.4/.github/workflows/test-some-examples.yml` & `vernac-0.0.5/.github/workflows/test-some-examples.yml`

 * *Files identical despite different names*

### Comparing `vernac-0.0.4/.gitignore` & `vernac-0.0.5/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -132,7 +132,10 @@
 .tool-versions
 
 # direnv config (often contains secrets)
 .envrc
 
 # VS Code (not sure about this; can always add later)
 .vscode/
+
+# vernac logs dir
+logs/
```

### Comparing `vernac-0.0.4/LICENSE` & `vernac-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vernac-0.0.4/dev-requirements.txt` & `vernac-0.0.5/dev-requirements.txt`

 * *Files 11% similar despite different names*

```diff
@@ -12,152 +12,113 @@
     # via stack-data
 async-timeout==4.0.2
     # via aiohttp
 attrs==22.2.0
     # via aiohttp
 backcall==0.2.0
     # via ipython
-bleach==6.0.0
-    # via readme-renderer
 build==0.10.0
-    # via
-    #   pip-tools
-    #   vernac (pyproject.toml)
+    # via pip-tools
 certifi==2022.12.7
     # via requests
-cffi==1.15.1
-    # via cryptography
 charset-normalizer==3.1.0
     # via
     #   aiohttp
     #   requests
 click==8.1.3
     # via
     #   pip-tools
     #   shiv
-cryptography==40.0.1
-    # via secretstorage
 decorator==5.1.1
     # via ipython
-docutils==0.19
-    # via readme-renderer
 executing==1.2.0
     # via stack-data
 frozenlist==1.3.3
     # via
     #   aiohttp
     #   aiosignal
 idna==3.4
     # via
     #   requests
     #   yarl
-importlib-metadata==6.3.0
-    # via
-    #   keyring
-    #   twine
+iniconfig==2.0.0
+    # via pytest
 ipython==8.12.0
     # via vernac (pyproject.toml)
-jaraco-classes==3.2.3
-    # via keyring
 jedi==0.18.2
     # via ipython
-jeepney==0.8.0
-    # via
-    #   keyring
-    #   secretstorage
-keyring==23.13.1
-    # via twine
 markdown-it-py==2.2.0
     # via rich
 matplotlib-inline==0.1.6
     # via ipython
 mdurl==0.1.2
     # via markdown-it-py
-more-itertools==9.1.0
-    # via jaraco-classes
 multidict==6.0.4
     # via
     #   aiohttp
     #   yarl
 openai==0.27.4
     # via vernac (pyproject.toml)
 packaging==23.1
-    # via build
+    # via
+    #   build
+    #   pytest
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
 pip-tools==6.13.0
     # via vernac (pyproject.toml)
-pkginfo==1.9.6
-    # via twine
+pluggy==1.0.0
+    # via pytest
 prompt-toolkit==3.0.38
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-pycparser==2.21
-    # via cffi
 pygments==2.15.0
     # via
     #   ipython
-    #   readme-renderer
     #   rich
 pyproject-hooks==1.0.0
     # via build
-readme-renderer==37.3
-    # via twine
+pytest==7.3.1
+    # via
+    #   pytest-asyncio
+    #   vernac (pyproject.toml)
+pytest-asyncio==0.21.0
+    # via vernac (pyproject.toml)
 requests==2.28.2
     # via
     #   openai
-    #   requests-toolbelt
-    #   twine
     #   vernac (pyproject.toml)
-requests-toolbelt==0.10.1
-    # via twine
-rfc3986==2.0.0
-    # via twine
 rich==13.3.3
-    # via
-    #   twine
-    #   vernac (pyproject.toml)
-secretstorage==3.3.3
-    # via keyring
+    # via vernac (pyproject.toml)
 shiv==1.0.3
     # via vernac (pyproject.toml)
 six==1.16.0
-    # via
-    #   asttokens
-    #   bleach
+    # via asttokens
 stack-data==0.6.2
     # via ipython
 tomli-w==1.0.0
     # via vernac (pyproject.toml)
 tqdm==4.65.0
     # via openai
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-twine==4.0.2
-    # via vernac (pyproject.toml)
 urllib3==1.26.15
-    # via
-    #   requests
-    #   twine
+    # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
-webencodings==0.5.1
-    # via bleach
 wheel==0.40.0
     # via pip-tools
 yarl==1.8.2
     # via aiohttp
-zipp==3.15.0
-    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `vernac-0.0.4/examples/unreliable/hntoday.vn` & `vernac-0.0.5/examples/unreliable/hntoday.vn`

 * *Files identical despite different names*

