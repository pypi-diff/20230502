# Comparing `tmp/crackerjack-0.1.8.tar.gz` & `tmp/crackerjack-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crackerjack-0.1.8.tar", last modified: Mon May  1 23:09:00 2023, max compression
+gzip compressed data, was "crackerjack-0.1.9.tar", last modified: Tue May  2 08:30:38 2023, max compression
```

## Comparing `crackerjack-0.1.8.tar` & `crackerjack-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.1.8/LICENSE
--rw-r--r--   0        0        0     2856 2023-04-26 12:28:28.914334 crackerjack-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-05-01 23:08:28.495079 crackerjack-0.1.8/crackerjack/.crackerjack-config.yaml
--rw-r--r--   0        0        0      197 2023-05-01 23:08:32.884162 crackerjack-0.1.8/crackerjack/.gitignore
--rw-r--r--   0        0        0      768 2023-05-01 23:08:28.479220 crackerjack-0.1.8/crackerjack/.libcst.codemod.yaml
--rw-r--r--   0        0        0     2055 2023-05-01 23:08:32.884329 crackerjack-0.1.8/crackerjack/.pre-commit-config.yaml
--rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.1.8/crackerjack/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.1.8/crackerjack/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.1.8/crackerjack/__init__.py
--rw-r--r--   0        0        0     1099 2023-05-01 23:08:32.884408 crackerjack-0.1.8/crackerjack/__main__.py
--rw-r--r--   0        0        0     4966 2023-05-01 23:08:32.884487 crackerjack-0.1.8/crackerjack/crackerjack.py
--rw-r--r--   0        0        0     1708 2023-05-01 23:08:32.884579 crackerjack-0.1.8/crackerjack/pyproject.toml
--rw-r--r--   0        0        0     5606 2023-04-25 20:30:39.178113 crackerjack-0.1.8/crackerjack/test1.py
--rw-r--r--   0        0        0     1705 2023-05-01 23:09:00.904627 crackerjack-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3860 1970-01-01 00:00:00.000000 crackerjack-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2856 2023-04-26 12:28:28.914334 crackerjack-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-05-02 08:30:21.144672 crackerjack-0.1.9/crackerjack/.crackerjack-config.yaml
+-rw-r--r--   0        0        0      197 2023-05-02 08:30:21.083979 crackerjack-0.1.9/crackerjack/.gitignore
+-rw-r--r--   0        0        0      768 2023-05-02 08:30:21.125590 crackerjack-0.1.9/crackerjack/.libcst.codemod.yaml
+-rw-r--r--   0        0        0     2055 2023-05-02 08:30:36.204284 crackerjack-0.1.9/crackerjack/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.1.9/crackerjack/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.1.9/crackerjack/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.1.9/crackerjack/__init__.py
+-rw-r--r--   0        0        0     1099 2023-05-01 23:08:32.884408 crackerjack-0.1.9/crackerjack/__main__.py
+-rw-r--r--   0        0        0     4968 2023-05-02 08:30:36.204493 crackerjack-0.1.9/crackerjack/crackerjack.py
+-rw-r--r--   0        0        0     1690 2023-05-02 08:30:36.204656 crackerjack-0.1.9/crackerjack/pyproject.toml
+-rw-r--r--   0        0        0     5606 2023-04-25 20:30:39.178113 crackerjack-0.1.9/crackerjack/test1.py
+-rw-r--r--   0        0        0     1687 2023-05-02 08:30:38.171002 crackerjack-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3860 1970-01-01 00:00:00.000000 crackerjack-0.1.9/PKG-INFO
```

### Comparing `crackerjack-0.1.8/LICENSE` & `crackerjack-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `crackerjack-0.1.8/README.md` & `crackerjack-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `crackerjack-0.1.8/crackerjack/.libcst.codemod.yaml` & `crackerjack-0.1.9/crackerjack/.libcst.codemod.yaml`

 * *Files identical despite different names*

### Comparing `crackerjack-0.1.8/crackerjack/.pre-commit-config.yaml` & `crackerjack-0.1.9/crackerjack/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         name: check-added-large-files
   - repo: https://github.com/psf/black
     rev: '23.3.0'
     hooks:
       - id: black
         language_version: python3.11
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.263
+    rev: v0.0.264
     hooks:
       - id: ruff
   - repo: https://github.com/fredrikaverpil/creosote
     rev: v2.6.1
     hooks:
       - id: creosote
         args:
@@ -60,15 +60,15 @@
   #        name: pdoc
   #        entry: pdoc --html -f -o docs module1 module2 module3
   #        language_version: python3.11
   #        require_serial: true
   #        types: [ python ]
   #        always_run: true
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.263
+    rev: v0.0.264
     hooks:
       - id: ruff
   - repo: https://github.com/psf/black
     rev: '23.3.0'
     hooks:
       - id: black
         language_version: python3.11
```

### Comparing `crackerjack-0.1.8/crackerjack/__main__.py` & `crackerjack-0.1.9/crackerjack/__main__.py`

 * *Files identical despite different names*

### Comparing `crackerjack-0.1.8/crackerjack/crackerjack.py` & `crackerjack-0.1.9/crackerjack/crackerjack.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         await self.pkg_dir.mkdir(exist_ok=True)
         print("\nCrackerjacking...\n")
         if self.pkg_path.stem == "crackerjack":
             run(["pre-commit", "autoupdate"])
         if not options.do_not_update_configs:
             await self.update_pkg_configs()
         if options.interactive:
-            for hook in ("ruff", "mypy"):
+            for hook in ("refurb", "mypy"):
                 await self.run_interactive(hook)
         check_all = call(["pre-commit", "run"])
         if check_all > 0:
             call(["pre-commit", "run", "--all-files"])
         if options.publish:
             check_output(["pdm", "bump", options.publish])
             run(["pdm", "publish"])
```

### Comparing `crackerjack-0.1.8/crackerjack/pyproject.toml` & `crackerjack-0.1.9/crackerjack/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     "py311",
 ]
 
 [tool.mypy]
 strict = false
 pretty = true
 ignore_missing_imports = false
-exclude = "tests"
 
 
 [tool.refurb]
 enable_all = true
```

### Comparing `crackerjack-0.1.8/crackerjack/test1.py` & `crackerjack-0.1.9/crackerjack/test1.py`

 * *Files identical despite different names*

### Comparing `crackerjack-0.1.8/pyproject.toml` & `crackerjack-0.1.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -26,27 +26,26 @@
     "py311",
 ]
 
 [tool.mypy]
 strict = false
 pretty = true
 ignore_missing_imports = false
-exclude = "tests"
 
 [tool.refurb]
 enable_all = true
 
 [tool.pytype]
 inputs = [
     "package_name",
 ]
 
 [project]
 name = "Crackerjack"
-version = "0.1.8"
+version = "0.1.9"
 description = "Crackerjack code formatting style."
 requires-python = ">=3.11"
 readme = "README.md"
 keywords = [
     "black",
     "ruff",
     "mypy",
```

### Comparing `crackerjack-0.1.8/PKG-INFO` & `crackerjack-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crackerjack
-Version: 0.1.8
+Version: 0.1.9
 Summary: Crackerjack code formatting style.
 Keywords: black ruff mypy creosote refurb
 Home-page: https://github.com/lesleslie/crackerjack
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 Maintainer-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Environment :: Console
```

