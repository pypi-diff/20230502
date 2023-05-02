# Comparing `tmp/jupyter_ai_magics-0.6.0.tar.gz` & `tmp/jupyter_ai_magics-0.6.1.tar.gz`

## Comparing `jupyter_ai_magics-0.6.0.tar` & `jupyter_ai_magics-0.6.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.0/setup.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.0/jupyter_ai_magics/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.0/jupyter_ai_magics/_version.py
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.0/jupyter_ai_magics/exception.py
--rw-r--r--   0        0        0     8841 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.0/jupyter_ai_magics/magics.py
--rw-r--r--   0        0        0     5633 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.0/jupyter_ai_magics/providers.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.0/jupyter_ai_magics/tests/__init__.py
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.0/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.0/LICENSE
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.0/README.md
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.1/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.1/setup.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.1/jupyter_ai_magics/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.1/jupyter_ai_magics/_version.py
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.1/jupyter_ai_magics/exception.py
+-rw-r--r--   0        0        0     8841 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.1/jupyter_ai_magics/magics.py
+-rw-r--r--   0        0        0     5633 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.1/jupyter_ai_magics/providers.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.1/jupyter_ai_magics/tests/__init__.py
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.1/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.1/LICENSE
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.1/README.md
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 jupyter_ai_magics-0.6.1/PKG-INFO
```

### Comparing `jupyter_ai_magics-0.6.0/package.json` & `jupyter_ai_magics-0.6.1/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.6.1'"}*

```diff
@@ -16,9 +16,9 @@
         "type": "git",
         "url": "https://github.com/jupyterlab/jupyter-ai.git"
     },
     "scripts": {
         "dev-install": "pip install -e \".[all]\"",
         "dev-uninstall": "pip uninstall jupyter_ai_magics -y"
     },
-    "version": "0.6.0"
+    "version": "0.6.1"
 }
```

### Comparing `jupyter_ai_magics-0.6.0/jupyter_ai_magics/__init__.py` & `jupyter_ai_magics-0.6.1/jupyter_ai_magics/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.6.0/jupyter_ai_magics/exception.py` & `jupyter_ai_magics-0.6.1/jupyter_ai_magics/exception.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.6.0/jupyter_ai_magics/magics.py` & `jupyter_ai_magics-0.6.1/jupyter_ai_magics/magics.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.6.0/jupyter_ai_magics/providers.py` & `jupyter_ai_magics-0.6.1/jupyter_ai_magics/providers.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.6.0/.gitignore` & `jupyter_ai_magics-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.6.0/LICENSE` & `jupyter_ai_magics-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.6.0/pyproject.toml` & `jupyter_ai_magics-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-0.6.0/PKG-INFO` & `jupyter_ai_magics-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_ai_magics
-Version: 0.6.0
+Version: 0.6.1
 Summary: Jupyter AI magics Python package. Not published on NPM.
 Project-URL: Homepage, https://github.com/jupyterlab/jupyter-ai
 Project-URL: Bug Tracker, https://github.com/jupyterlab/jupyter-ai/issues
 Project-URL: Repository, https://github.com/jupyterlab/jupyter-ai.git
 Author-email: Project Jupyter <jupyter@googlegroups.com>
 License: BSD 3-Clause License
```

