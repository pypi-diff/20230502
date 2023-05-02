# Comparing `tmp/conversations-0.8.0.tar.gz` & `tmp/conversations-0.9.0.tar.gz`

## Comparing `conversations-0.8.0.tar` & `conversations-0.9.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 conversations-0.8.0/CHANGELOG.md
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 conversations-0.8.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 conversations-0.8.0/.github/workflows/commitlint.yml
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 conversations-0.8.0/.github/workflows/lint-pr.yml
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 conversations-0.8.0/.github/workflows/md-lint.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 conversations-0.8.0/.github/workflows/release.yml
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 conversations-0.8.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 conversations-0.8.0/conversations/__about__.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 conversations-0.8.0/conversations/__init__.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 conversations-0.8.0/tests/__init__.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 conversations-0.8.0/tests/test_package.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 conversations-0.8.0/.gitignore
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 conversations-0.8.0/LICENSE.txt
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 conversations-0.8.0/README.md
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 conversations-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 conversations-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 conversations-0.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 conversations-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 conversations-0.9.0/.github/workflows/commitlint.yml
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 conversations-0.9.0/.github/workflows/lint-pr.yml
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 conversations-0.9.0/.github/workflows/md-lint.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 conversations-0.9.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 conversations-0.9.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 conversations-0.9.0/conversations/__about__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 conversations-0.9.0/conversations/__init__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 conversations-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 conversations-0.9.0/tests/test_package.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 conversations-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 conversations-0.9.0/LICENSE.txt
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 conversations-0.9.0/README.md
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 conversations-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 conversations-0.9.0/PKG-INFO
```

### Comparing `conversations-0.8.0/CONTRIBUTING.md` & `conversations-0.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `conversations-0.8.0/.github/workflows/release.yml` & `conversations-0.9.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `conversations-0.8.0/.github/workflows/test.yml` & `conversations-0.9.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `conversations-0.8.0/.gitignore` & `conversations-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `conversations-0.8.0/LICENSE.txt` & `conversations-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `conversations-0.8.0/pyproject.toml` & `conversations-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -60,7 +60,9 @@
 version_variable = "conversations/__about__.py:__version__"
 version_source = "tag"
 tag_commit = true
 branch = "main"
 commit_parser = "semantic_release.history.angular_parser"
 build_command="hatch build"
 commit_version_number=true
+commit_subject="chore: release {version}"
+
```

### Comparing `conversations-0.8.0/PKG-INFO` & `conversations-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conversations
-Version: 0.8.0
+Version: 0.9.0
 Project-URL: Documentation, https://github.com/rob-luke/conversations#readme
 Project-URL: Issues, https://github.com/rob-luke/conversations/issues
 Project-URL: Source, https://github.com/rob-luke/conversations
 Author-email: Robert Luke <code@robertluke.net>
 License-File: LICENSE.txt
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
```

