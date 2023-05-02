# Comparing `tmp/ghastoolkit-0.1.8.tar.gz` & `tmp/ghastoolkit-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghastoolkit-0.1.8.tar", last modified: Tue Apr 25 23:55:22 2023, max compression
+gzip compressed data, was "ghastoolkit-0.1.9.tar", last modified: Thu Apr 27 14:00:31 2023, max compression
```

## Comparing `ghastoolkit-0.1.8.tar` & `ghastoolkit-0.1.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:55:22.214814 ghastoolkit-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-25 23:55:22.214814 ghastoolkit-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 23:55:22.214814 ghastoolkit-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:55:22.210814 ghastoolkit-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:55:22.214814 ghastoolkit-0.1.8/src/ghastoolkit/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/src/ghastoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/src/ghastoolkit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:55:22.214814 ghastoolkit-0.1.8/src/ghastoolkit/codeql/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/src/ghastoolkit/codeql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/src/ghastoolkit/codeql/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/src/ghastoolkit/codeql/databases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:55:22.214814 ghastoolkit-0.1.8/src/ghastoolkit/octokit/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/src/ghastoolkit/octokit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/src/ghastoolkit/octokit/codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/src/ghastoolkit/octokit/dependencygraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/src/ghastoolkit/octokit/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     8490 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/src/ghastoolkit/octokit/octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/src/ghastoolkit/octokit/secretscanning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:55:22.214814 ghastoolkit-0.1.8/src/ghastoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-25 23:55:22.000000 ghastoolkit-0.1.8/src/ghastoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-25 23:55:22.000000 ghastoolkit-0.1.8/src/ghastoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 23:55:22.000000 ghastoolkit-0.1.8/src/ghastoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-25 23:55:22.000000 ghastoolkit-0.1.8/src/ghastoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 23:55:22.000000 ghastoolkit-0.1.8/src/ghastoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:55:22.214814 ghastoolkit-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/tests/test_codeqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/tests/test_codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/tests/test_depgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/tests/test_octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-25 23:54:51.000000 ghastoolkit-0.1.8/tests/test_secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:00:31.634497 ghastoolkit-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-27 14:00:31.634497 ghastoolkit-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 14:00:31.634497 ghastoolkit-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:00:31.630497 ghastoolkit-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:00:31.630497 ghastoolkit-0.1.9/src/ghastoolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/src/ghastoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/src/ghastoolkit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:00:31.634497 ghastoolkit-0.1.9/src/ghastoolkit/codeql/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/src/ghastoolkit/codeql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/src/ghastoolkit/codeql/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/src/ghastoolkit/codeql/databases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:00:31.634497 ghastoolkit-0.1.9/src/ghastoolkit/octokit/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/src/ghastoolkit/octokit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/src/ghastoolkit/octokit/codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/src/ghastoolkit/octokit/dependencygraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/src/ghastoolkit/octokit/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8490 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/src/ghastoolkit/octokit/octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/src/ghastoolkit/octokit/secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:00:31.630497 ghastoolkit-0.1.9/src/ghastoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-27 14:00:31.000000 ghastoolkit-0.1.9/src/ghastoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-27 14:00:31.000000 ghastoolkit-0.1.9/src/ghastoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 14:00:31.000000 ghastoolkit-0.1.9/src/ghastoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-27 14:00:31.000000 ghastoolkit-0.1.9/src/ghastoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 14:00:31.000000 ghastoolkit-0.1.9/src/ghastoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:00:31.634497 ghastoolkit-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/tests/test_codeqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/tests/test_codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/tests/test_depgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/tests/test_octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-27 13:59:46.000000 ghastoolkit-0.1.9/tests/test_secretscanning.py
```

### Comparing `ghastoolkit-0.1.8/LICENSE` & `ghastoolkit-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.8/PKG-INFO` & `ghastoolkit-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.1.8
+Version: 0.1.9
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.1.8/README.md` & `ghastoolkit-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.8/pyproject.toml` & `ghastoolkit-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ghastoolkit"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="GeekMasher" },
 ]
 description = "GitHub Advanced Security Python Toolkit"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `ghastoolkit-0.1.8/src/ghastoolkit/__init__.py` & `ghastoolkit-0.1.9/src/ghastoolkit/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __name__ = "ghastoolkit"
 __title__ = "GHAS Toolkit"
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 
 __description__ = "GitHub Advanced Security Python Toolkit"
 __summary__ = """\
 GitHub Advanced Security Python Toolkit
 """
 
 __url__ = "https://github.com/GeekMasher/ghastoolkit"
@@ -24,8 +24,8 @@
 from ghastoolkit.octokit.dependencygraph import (
     DependencyGraph,
     Dependencies,
     Dependency,
 )
 
 # CodeQL
-from ghastoolkit.codeql.databases import CodeQLDatabaseList, CodeQLDatabase
+from ghastoolkit.codeql.databases import CodeQLDatabases, CodeQLDatabase
```

### Comparing `ghastoolkit-0.1.8/src/ghastoolkit/__main__.py` & `ghastoolkit-0.1.9/src/ghastoolkit/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.8/src/ghastoolkit/codeql/databases.py` & `ghastoolkit-0.1.9/src/ghastoolkit/codeql/databases.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,31 +10,39 @@
 from ghastoolkit.codeql.consts import CODEQL_LANGUAGES
 from ghastoolkit.octokit.codescanning import CodeScanning, logging
 from ghastoolkit.octokit.github import Repository
 from ghastoolkit.octokit.octokit import GitHub
 from requests import request
 
 
+__CODEQL_DATABASE_PATHS__ = [os.path.expanduser("~/.codeql/databases")]
+
 logger = logging.getLogger("ghastoolkit.codeql")
 
 
 @dataclass
 class CodeQLDatabase:
     name: str
     language: str
     repository: Optional[Repository] = None
+
+    # path to when the DB should be
     path: Optional[str] = None
+    path_download: Optional[str] = None
 
     def __post_init__(self):
         if self.path:
             if not os.path.exists(self.path):
                 raise Exception("Database folder incorrect")
             # TODO: check and load DB data
-        elif not self.path:
-            self.path = self.findOrCreatePath()
+        else:
+            self.path = self.createPath()
+
+        if not self.path_download:
+            self.path_download = self.createDownloadPath()
 
         if self.language not in CODEQL_LANGUAGES:
             raise Exception("Language is not supported by CodeQL Summary Generator")
 
     def __str__(self) -> str:
         name = str(self.repository) if self.repository else self.name
         return f"CodeQLDatabase('{name}', '{self.language}')"
@@ -61,15 +69,23 @@
             if own and own == owner:
                 return self.repository.repo.title().replace(" ", "")
 
             return f"{own.title()}{repo.title()}".replace(" ", "")
         new_name = self.name.replace("-", " ")
         return new_name.title().replace(" ", "")
 
-    def findOrCreatePath(self, root: Optional[str] = None) -> str:
+    def createPath(self) -> Optional[str]:
+        for root in __CODEQL_DATABASE_PATHS__:
+            if not os.path.exists(root):
+                continue
+
+            return os.path.join(root, self.database_folder)
+        return
+
+    def createDownloadPath(self, root: Optional[str] = None) -> str:
         """Find a path where"""
         if not root:
             root = os.path.join(tempfile.gettempdir(), "codeql-db")
         if self.repository:
             return os.path.join(
                 root, self.language, self.repository.owner, self.repository.repo
             )
@@ -97,16 +113,20 @@
 
         with open(path, "r") as handle:
             data = safe_load(handle)
 
         db = CodeQLDatabase(name, data.get("primaryLanguage"), path=path)
         return db
 
-    def downloadDatabase(self, output: str, use_cache: bool = True) -> str:
+    def downloadDatabase(self, output: Optional[str], use_cache: bool = True) -> str:
         """Download CodeQL database"""
+        output = output or self.path or self.path_download
+        if not output:
+            raise Exception(f"CodeQL Database path not set")
+
         if not self.language or not self.repository:
             raise Exception(
                 f"Database download requires a repository and language to be set"
             )
         codescanning = CodeScanning()
         codeqldb_info = codescanning.getCodeQLDatabase(self.language)
 
@@ -151,31 +171,68 @@
 
         # SECURITY: Do we trust this DB?
         with zipfile.ZipFile(output_zip) as zf:
             zf.extractall(output_db)
 
         logger.info(f" >>> {output_db}")
         codeql_lang_path = os.path.join(output_db, self.language)
+
         if os.path.exists(codeql_lang_path):
             return codeql_lang_path
 
         for codeql_dir in os.listdir(output_db):
             codeql_dir = os.path.join(output_db, codeql_dir)
             if os.path.isdir(codeql_dir):
                 return codeql_dir
 
+        raise Exception(f"Database downloaded but not DB files...")
+
+
+class CodeQLDatabases(list[CodeQLDatabase]):
+    def loadDefault(self):
+        """Load Databases from standard locations"""
+        for location in __CODEQL_DATABASE_PATHS__:
+            if not os.path.exists(location):
+                continue
+            self.findDatabases(location)
 
-class CodeQLDatabaseList(list[CodeQLDatabase]):
     @staticmethod
-    def findDatabases(path: str) -> "CodeQLDatabaseList":
-        if not os.path.exists(path):
-            raise Exception("Root database folder does not exist")
+    def loadLocalDatabase() -> "CodeQLDatabases":
+        """Load all Local Databases"""
+        db = CodeQLDatabases()
+        db.loadDefault()
+        return db
+
+    def getRemoteDatabases(self, repository: Repository):
+        """Find all remote databases and return a list of them"""
+        cs = CodeScanning(repository)
+        databases = cs.getCodeQLDatabases()
+        for db in databases:
+            lang = db.get("language")
+            if not lang:
+                raise Exception(f"CodeQL remote language is not set")
+            self.append(
+                CodeQLDatabase(
+                    f"{repository.repo}-{lang}", language=lang, repository=repository
+                )
+            )
+
+    @staticmethod
+    def loadRemoteDatabases(repository: Repository) -> "CodeQLDatabases":
+        """Use API to find all the databases and return a list of them"""
+        dbs = CodeQLDatabases()
+        dbs.getRemoteDatabases(repository)
+        return dbs
 
-        paths = CodeQLDatabaseList()
+    def findDatabases(self, path: str):
+        if not os.path.exists(path):
+            raise Exception(f"Path does not exist: {path}")
 
         for root, _, files in os.walk(path):
             for file in files:
                 if file == "codeql-database.yml":
                     path = os.path.join(root, file)
-                    paths.append(CodeQLDatabase.loadDatabaseYml(path))
+                    self.append(CodeQLDatabase.loadDatabaseYml(path))
 
-        return paths
+    def downloadDatabases(self):
+        for db in self:
+            db.downloadDatabase(None)
```

### Comparing `ghastoolkit-0.1.8/src/ghastoolkit/octokit/codescanning.py` & `ghastoolkit-0.1.9/src/ghastoolkit/octokit/codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.8/src/ghastoolkit/octokit/dependencygraph.py` & `ghastoolkit-0.1.9/src/ghastoolkit/octokit/dependencygraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.8/src/ghastoolkit/octokit/github.py` & `ghastoolkit-0.1.9/src/ghastoolkit/octokit/github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.8/src/ghastoolkit/octokit/octokit.py` & `ghastoolkit-0.1.9/src/ghastoolkit/octokit/octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.8/src/ghastoolkit/octokit/secretscanning.py` & `ghastoolkit-0.1.9/src/ghastoolkit/octokit/secretscanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.8/src/ghastoolkit.egg-info/PKG-INFO` & `ghastoolkit-0.1.9/src/ghastoolkit.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.1.8
+Version: 0.1.9
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.1.8/src/ghastoolkit.egg-info/SOURCES.txt` & `ghastoolkit-0.1.9/src/ghastoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.8/tests/test_codeqldb.py` & `ghastoolkit-0.1.9/tests/test_codeqldb.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 class TestCodeQLDb(unittest.TestCase):
     def setUp(self):
         self.repo = Repository("GeekMasher", "ghastoolkit")
 
     def test_path(self):
         codeql = CodeQLDatabase("db", "java", self.repo)
         self.assertEqual(
-            codeql.findOrCreatePath("/tmp"),
+            codeql.createDownloadPath("/tmp"),
             os.path.join("/tmp", "java", "GeekMasher", "ghastoolkit")
         )
 
         codeql = CodeQLDatabase("db", "java")
         self.assertEqual(
-            codeql.findOrCreatePath("/tmp"),
+            codeql.createDownloadPath("/tmp"),
             os.path.join("/tmp", "java", "db")
         )
```

### Comparing `ghastoolkit-0.1.8/tests/test_codescanning.py` & `ghastoolkit-0.1.9/tests/test_codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.8/tests/test_depgraph.py` & `ghastoolkit-0.1.9/tests/test_depgraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.8/tests/test_github.py` & `ghastoolkit-0.1.9/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.8/tests/test_octokit.py` & `ghastoolkit-0.1.9/tests/test_octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.1.8/tests/test_secretscanning.py` & `ghastoolkit-0.1.9/tests/test_secretscanning.py`

 * *Files identical despite different names*

