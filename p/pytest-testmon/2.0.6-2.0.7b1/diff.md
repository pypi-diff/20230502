# Comparing `tmp/pytest-testmon-2.0.6.tar.gz` & `tmp/pytest-testmon-2.0.7b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-testmon-2.0.6.tar", last modified: Thu Apr  6 15:30:20 2023, max compression
+gzip compressed data, was "pytest-testmon-2.0.7b1.tar", last modified: Tue May  2 07:59:57 2023, max compression
```

## Comparing `pytest-testmon-2.0.6.tar` & `pytest-testmon-2.0.7b1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 poko      (1000) poko      (1000)        0 2023-04-06 15:30:20.021736 pytest-testmon-2.0.6/
--rw-r--r--   0 poko      (1000) poko      (1000)    34633 2023-01-12 14:59:27.000000 pytest-testmon-2.0.6/LICENSE
--rw-r--r--   0 poko      (1000) poko      (1000)       74 2023-03-09 09:22:22.000000 pytest-testmon-2.0.6/MANIFEST.in
--rw-r--r--   0 poko      (1000) poko      (1000)     2429 2023-04-06 15:30:20.021736 pytest-testmon-2.0.6/PKG-INFO
--rw-r--r--   0 poko      (1000) poko      (1000)     1208 2023-03-27 16:31:43.000000 pytest-testmon-2.0.6/README.md
--rw-r--r--   0 poko      (1000) poko      (1000)     1619 2023-04-06 15:26:55.000000 pytest-testmon-2.0.6/pyproject.toml
-drwxr-xr-x   0 poko      (1000) poko      (1000)        0 2023-04-06 15:30:20.021736 pytest-testmon-2.0.6/pytest_testmon.egg-info/
--rw-r--r--   0 poko      (1000) poko      (1000)     2429 2023-04-06 15:30:20.000000 pytest-testmon-2.0.6/pytest_testmon.egg-info/PKG-INFO
--rw-r--r--   0 poko      (1000) poko      (1000)      463 2023-04-06 15:30:20.000000 pytest-testmon-2.0.6/pytest_testmon.egg-info/SOURCES.txt
--rw-r--r--   0 poko      (1000) poko      (1000)        1 2023-04-06 15:30:20.000000 pytest-testmon-2.0.6/pytest_testmon.egg-info/dependency_links.txt
--rw-r--r--   0 poko      (1000) poko      (1000)       51 2023-04-06 15:30:20.000000 pytest-testmon-2.0.6/pytest_testmon.egg-info/entry_points.txt
--rw-r--r--   0 poko      (1000) poko      (1000)       28 2023-04-06 15:30:20.000000 pytest-testmon-2.0.6/pytest_testmon.egg-info/requires.txt
--rw-r--r--   0 poko      (1000) poko      (1000)        8 2023-04-06 15:30:20.000000 pytest-testmon-2.0.6/pytest_testmon.egg-info/top_level.txt
--rw-r--r--   0 poko      (1000) poko      (1000)     1219 2023-04-06 15:30:20.021736 pytest-testmon-2.0.6/setup.cfg
--rw-r--r--   0 poko      (1000) poko      (1000)       69 2023-04-06 15:26:55.000000 pytest-testmon-2.0.6/setup.py
-drwxr-xr-x   0 poko      (1000) poko      (1000)        0 2023-04-06 15:30:20.021736 pytest-testmon-2.0.6/testmon/
--rw-r--r--   0 poko      (1000) poko      (1000)       44 2023-04-06 15:26:56.000000 pytest-testmon-2.0.6/testmon/__init__.py
--rw-r--r--   0 poko      (1000) poko      (1000)      183 2023-04-06 15:26:56.000000 pytest-testmon-2.0.6/testmon/common.py
--rw-r--r--   0 poko      (1000) poko      (1000)     3786 2023-04-06 15:26:56.000000 pytest-testmon-2.0.6/testmon/configure.py
--rw-r--r--   0 poko      (1000) poko      (1000)    22226 2023-04-06 15:26:56.000000 pytest-testmon-2.0.6/testmon/db.py
--rw-r--r--   0 poko      (1000) poko      (1000)     7867 2023-04-06 15:26:56.000000 pytest-testmon-2.0.6/testmon/process_code.py
--rw-r--r--   0 poko      (1000) poko      (1000)    17025 2023-04-06 15:26:55.000000 pytest-testmon-2.0.6/testmon/pytest_testmon.py
--rw-r--r--   0 poko      (1000) poko      (1000)    18896 2023-04-06 15:26:56.000000 pytest-testmon-2.0.6/testmon/testmon_core.py
--rw-r--r--   0 poko      (1000) poko      (1000)     1232 2023-01-12 14:59:27.000000 pytest-testmon-2.0.6/testmon/tox_testmon.py
+drwxr-xr-x   0 poko      (1000) poko      (1000)        0 2023-05-02 07:59:57.175580 pytest-testmon-2.0.7b1/
+-rw-r--r--   0 poko      (1000) poko      (1000)    34633 2023-01-12 14:59:27.000000 pytest-testmon-2.0.7b1/LICENSE
+-rw-r--r--   0 poko      (1000) poko      (1000)       74 2023-03-09 09:22:22.000000 pytest-testmon-2.0.7b1/MANIFEST.in
+-rw-r--r--   0 poko      (1000) poko      (1000)     2431 2023-05-02 07:59:57.175580 pytest-testmon-2.0.7b1/PKG-INFO
+-rw-r--r--   0 poko      (1000) poko      (1000)     1208 2023-04-27 09:24:29.000000 pytest-testmon-2.0.7b1/README.md
+-rw-r--r--   0 poko      (1000) poko      (1000)     1619 2023-05-02 07:51:34.000000 pytest-testmon-2.0.7b1/pyproject.toml
+drwxr-xr-x   0 poko      (1000) poko      (1000)        0 2023-05-02 07:59:57.171580 pytest-testmon-2.0.7b1/pytest_testmon.egg-info/
+-rw-r--r--   0 poko      (1000) poko      (1000)     2431 2023-05-02 07:59:57.000000 pytest-testmon-2.0.7b1/pytest_testmon.egg-info/PKG-INFO
+-rw-r--r--   0 poko      (1000) poko      (1000)      463 2023-05-02 07:59:57.000000 pytest-testmon-2.0.7b1/pytest_testmon.egg-info/SOURCES.txt
+-rw-r--r--   0 poko      (1000) poko      (1000)        1 2023-05-02 07:59:57.000000 pytest-testmon-2.0.7b1/pytest_testmon.egg-info/dependency_links.txt
+-rw-r--r--   0 poko      (1000) poko      (1000)       51 2023-05-02 07:59:57.000000 pytest-testmon-2.0.7b1/pytest_testmon.egg-info/entry_points.txt
+-rw-r--r--   0 poko      (1000) poko      (1000)       28 2023-05-02 07:59:57.000000 pytest-testmon-2.0.7b1/pytest_testmon.egg-info/requires.txt
+-rw-r--r--   0 poko      (1000) poko      (1000)        8 2023-05-02 07:59:57.000000 pytest-testmon-2.0.7b1/pytest_testmon.egg-info/top_level.txt
+-rw-r--r--   0 poko      (1000) poko      (1000)     1219 2023-05-02 07:59:57.175580 pytest-testmon-2.0.7b1/setup.cfg
+-rw-r--r--   0 poko      (1000) poko      (1000)       69 2023-05-02 07:51:34.000000 pytest-testmon-2.0.7b1/setup.py
+drwxr-xr-x   0 poko      (1000) poko      (1000)        0 2023-05-02 07:59:57.175580 pytest-testmon-2.0.7b1/testmon/
+-rw-r--r--   0 poko      (1000) poko      (1000)       46 2023-05-02 07:51:35.000000 pytest-testmon-2.0.7b1/testmon/__init__.py
+-rw-r--r--   0 poko      (1000) poko      (1000)     1495 2023-05-02 07:51:35.000000 pytest-testmon-2.0.7b1/testmon/common.py
+-rw-r--r--   0 poko      (1000) poko      (1000)     3786 2023-05-02 07:51:35.000000 pytest-testmon-2.0.7b1/testmon/configure.py
+-rw-r--r--   0 poko      (1000) poko      (1000)    22138 2023-05-02 07:51:35.000000 pytest-testmon-2.0.7b1/testmon/db.py
+-rw-r--r--   0 poko      (1000) poko      (1000)     7969 2023-05-02 07:51:34.000000 pytest-testmon-2.0.7b1/testmon/process_code.py
+-rw-r--r--   0 poko      (1000) poko      (1000)    17066 2023-05-02 07:51:34.000000 pytest-testmon-2.0.7b1/testmon/pytest_testmon.py
+-rw-r--r--   0 poko      (1000) poko      (1000)    19048 2023-05-02 07:51:34.000000 pytest-testmon-2.0.7b1/testmon/testmon_core.py
+-rw-r--r--   0 poko      (1000) poko      (1000)     1232 2023-01-12 14:59:27.000000 pytest-testmon-2.0.7b1/testmon/tox_testmon.py
```

### Comparing `pytest-testmon-2.0.6/LICENSE` & `pytest-testmon-2.0.7b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-testmon-2.0.6/PKG-INFO` & `pytest-testmon-2.0.7b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-testmon
-Version: 2.0.6
+Version: 2.0.7b1
 Summary: selects tests affected by changed files and methods
 Home-page: https://testmon.org
 Author: Tibor Arpas, Tomas Matlovic
 Author-email: Tibor Arpas <tibor@testmon.org>
 License: AGPL
 Project-URL: Source, https://github.com/tarpas/pytest-testmon
 Keywords: testing,pytest,plugin
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytest-testmon Version: 2.0.6 Summary: selects
+Metadata-Version: 2.1 Name: pytest-testmon Version: 2.0.7b1 Summary: selects
 tests affected by changed files and methods Home-page: https://testmon.org
 Author: Tibor Arpas, Tomas Matlovic Author-email: Tibor Arpas
 testmon.org> License: AGPL Project-URL: Source, https://github.com/tarpas/
 pytest-testmon Keywords: testing,pytest,plugin Platform: linux Platform: osx
 Platform: win32 Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: Developers Classifier: Operating System :: POSIX Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: MacOS
```

### Comparing `pytest-testmon-2.0.6/README.md` & `pytest-testmon-2.0.7b1/README.md`

 * *Files identical despite different names*

### Comparing `pytest-testmon-2.0.6/pyproject.toml` & `pytest-testmon-2.0.7b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest-testmon-2.0.6/pytest_testmon.egg-info/PKG-INFO` & `pytest-testmon-2.0.7b1/pytest_testmon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-testmon
-Version: 2.0.6
+Version: 2.0.7b1
 Summary: selects tests affected by changed files and methods
 Home-page: https://testmon.org
 Author: Tibor Arpas, Tomas Matlovic
 Author-email: Tibor Arpas <tibor@testmon.org>
 License: AGPL
 Project-URL: Source, https://github.com/tarpas/pytest-testmon
 Keywords: testing,pytest,plugin
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytest-testmon Version: 2.0.6 Summary: selects
+Metadata-Version: 2.1 Name: pytest-testmon Version: 2.0.7b1 Summary: selects
 tests affected by changed files and methods Home-page: https://testmon.org
 Author: Tibor Arpas, Tomas Matlovic Author-email: Tibor Arpas
 testmon.org> License: AGPL Project-URL: Source, https://github.com/tarpas/
 pytest-testmon Keywords: testing,pytest,plugin Platform: linux Platform: osx
 Platform: win32 Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: Developers Classifier: Operating System :: POSIX Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: MacOS
```

### Comparing `pytest-testmon-2.0.6/setup.cfg` & `pytest-testmon-2.0.7b1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytest-testmon-2.0.6/testmon/configure.py` & `pytest-testmon-2.0.7b1/testmon/configure.py`

 * *Files identical despite different names*

### Comparing `pytest-testmon-2.0.6/testmon/db.py` & `pytest-testmon-2.0.7b1/testmon/db.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,26 +11,14 @@
 DATA_VERSION = 9
 
 ChangedFileData = namedtuple(
     "ChangedFileData", "filename name method_checksums id failed"
 )
 
 
-class CachedProperty:
-    def __init__(self, func):
-        self.__doc__ = getattr(func, "__doc__")
-        self.func = func
-
-    def __get__(self, obj, cls):
-        if obj is None:
-            return self
-        value = obj.__dict__[self.func.__name__] = self.func(obj)
-        return value
-
-
 class TestmonDbException(Exception):
     pass
 
 
 def connect(datafile, readonly=False):
     connection = sqlite3.connect(
         f"file:{datafile}{'?mode=ro' if readonly else ''}", uri=True
@@ -441,41 +429,45 @@
                 ]
             )
 
         return result
 
     def fetch_unknown_files(self, files_checksums, exec_id):
         with self.con as con:
-            self.con.execute("DELETE FROM temp_files_checksums")
+            con.execute(
+                "DELETE FROM temp_files_checksums WHERE exec_id = ?", (exec_id,)
+            )
             con.executemany(
                 "INSERT INTO temp_files_checksums VALUES (?, ?, ?)",
                 [
                     (exec_id, file, checksum)
                     for file, checksum in files_checksums.items()
                 ],
             )
-            result = []
-            for row in self.con.execute(
-                f"""
+            return self._fetch_unknown_files_from_one_v(con, exec_id, exec_id)
+
+    def _fetch_unknown_files_from_one_v(self, con, exec_id, files_shas_id):
+        result = []
+        for row in con.execute(
+            f"""
                 SELECT DISTINCT
                     f.filename
                 FROM test_execution te, test_execution_file_fp te_ffp, file_fp f
                 LEFT OUTER JOIN temp_files_checksums tfc
-                ON f.filename = tfc.filename and f.checksum = tfc.checksum AND tfc.exec_id = ?
+                ON f.filename = tfc.filename and f.checksum = tfc.checksum AND tfc.exec_id = :files_shas_id
                 WHERE
-                    te.{self._test_execution_fk_column()} = ? AND
+                    te.{self._test_execution_fk_column()} = :exec_id AND
                     te.id = te_ffp.test_execution_id AND
                     te_ffp.fingerprint_id = f.id AND
                     (f.checksum IS NULL OR tfc.checksum IS NULL)
                 """,
-                [exec_id, exec_id],
-            ):
-                result.append(row["filename"])
-
-            return result
+            {"files_shas_id": files_shas_id, "exec_id": exec_id},
+        ):
+            result.append(row["filename"])
+        return result
 
     def delete_filenames(self, con):
         con.execute("DELETE FROM temp_filenames")
 
     def determine_tests(self, exec_id, files_mhashes):
         with self.con as con:
             con.execute(
@@ -586,15 +578,14 @@
             FROM
                 file_fp f
                 """,
         )
 
         return [row[0] for row in cursor]
 
-    @lru_cache(128)
     def filenames_fingerprints(self, exec_id):
         cursor = self.con.execute(
             f"""
             SELECT DISTINCT
                 f.filename,
                 f.mtime,
                 f.checksum,
@@ -661,10 +652,10 @@
         execution_metadata,
     ):
         exec_id, packages_changed = self.fetch_or_create_environment(
             environment_name, system_packages, python_version
         )
         return {
             "exec_id": exec_id,
-            "filenames": self.filenames(exec_id),
+            "filenames": self.all_filenames(),
             "packages_changed": packages_changed,
         }
```

### Comparing `pytest-testmon-2.0.6/testmon/process_code.py` & `pytest-testmon-2.0.7b1/testmon/process_code.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,15 +119,14 @@
         )
         self.fs_checksum = (
             fs_checksum or bytes_to_string_and_checksum(bytes(source_code, "utf-8"))[1]
         )
         self.ext = ext
 
     def dump_and_block(self, node, end, name="unknown", into_block=False):
-
         if isinstance(node, ast.AST):
             class_name = node.__class__.__name__
             fields = []
             for field_name, field_value in ast.iter_fields(node):
                 transform_into_block = (
                     class_name in ("AsyncFunctionDef", "FunctionDef", "Module")
                 ) and field_name == "body"
@@ -202,15 +201,15 @@
     except FileNotFoundError:
         return None, None
 
     source, checksum = bytes_to_string_and_checksum(source_bytes)
     return source, checksum
 
 
-def get_files_shas(directory):
+def noncached_get_files_shas(directory):
     all_shas = {}
     try:
         result = run(
             ["git", "ls-files", "--stage", "-m", directory],
             capture_output=True,
             universal_newlines=True,
             check=True,
@@ -227,14 +226,19 @@
         else:
             all_shas[filename] = hsh
     for modified_file in modified_files:
         del all_shas[modified_file]
     return all_shas
 
 
+@lru_cache()
+def get_files_shas(directory):
+    return noncached_get_files_shas(directory)
+
+
 def get_source_sha(directory, filename):
     try:
         sha = get_files_shas(directory)[filename]
         return (None, sha)
     except KeyError:
         pass
     return read_source_sha(Path(directory) / filename)
```

### Comparing `pytest-testmon-2.0.6/testmon/pytest_testmon.py` & `pytest-testmon-2.0.7b1/testmon/pytest_testmon.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,42 +124,46 @@
         "environment_expression",
     ]:
         if config.getoption(label):
             result.append(label.replace("testmon_", ""))
     return result
 
 
+def get_system_packages():
+    return ", ".join(sorted(str(p) for p in pkg_resources.working_set))
+
+
 def init_testmon_data(config):
     environment = config.getoption("environment_expression") or eval_environment(
         config.getini("environment_expression")
     )
-    packages = ", ".join(sorted(str(p) for p in pkg_resources.working_set))
+    packages = get_system_packages()
 
     url = config.getini("testmon_url")
     rpc_proxy = None
 
     if config.testmon_config.tmnet or getattr(config, "tmnet", None):
         rpc_proxy = getattr(config, "tmnet", None)
 
         if not url:
             url = "https://api1.testmon.net/"
         if not rpc_proxy:
             tmnet_api_key = config.getini("tmnet_api_key")
-            if "TMNET_DEV_API_KEY" in os.environ:
+            if "TMNET_API_KEY" in os.environ:
                 if tmnet_api_key:
                     logger.warning(
-                        "Duplicate TMNET_DEV_API_KEY (environment and ini file). \
-                         Using TMNET_DEV_API_KEY from %s",
+                        "Duplicate TMNET_API_KEY (environment and ini file). \
+                         Using TMNET_API_KEY from %s",
                         config.inipath,
                     )
                 else:
-                    tmnet_api_key = os.getenv("TMNET_DEV_API_KEY")
+                    tmnet_api_key = os.getenv("TMNET_API_KEY")
             elif tmnet_api_key is None:
                 logger.warning(
-                    "TMNET_DEV_API_KEY not set.",
+                    "TMNET_API_KEY not set.",
                 )
             rpc_proxy = xmlrpc.client.ServerProxy(
                 url,
                 allow_none=True,
                 headers=[("x-api-key", tmnet_api_key)],
             )
 
@@ -219,15 +223,14 @@
     cov_plugin = config.pluginmanager.get_plugin("_cov")
 
     tm_conf = configure.header_collect_select(
         config, coverage_stack, cov_plugin=cov_plugin
     )
     config.testmon_config = tm_conf
     if tm_conf.select or tm_conf.collect:
-
         try:
             init_testmon_data(config)
             register_plugins(config, tm_conf.select, tm_conf.collect, cov_plugin)
         except TestmonException as error:
             pytest.exit(str(error))
```

### Comparing `pytest-testmon-2.0.6/testmon/testmon_core.py` & `pytest-testmon-2.0.7b1/testmon/testmon_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,24 @@
 import random
 import sys
 import sysconfig
 import textwrap
 from functools import lru_cache
 from collections import defaultdict
 from xmlrpc.client import Fault, ProtocolError
-from subprocess import check_output, CalledProcessError
 from socket import gaierror
 
 import pkg_resources
 import pytest
 from coverage import Coverage, CoverageData
 
 from testmon import db
 from testmon import VERSION as TM_CLIENT_VERSION
 
-from testmon.common import get_logger
+from testmon.common import get_logger, git_current_head
 
 from testmon.process_code import (
     match_fingerprint,
     create_fingerprint,
     methods_to_checksums,
     get_source_sha,
     Module,
@@ -56,17 +55,15 @@
     def __init__(self, rootdir, packages=None):
         self.rootdir = rootdir
         self.packages = packages
         self.cache = {}
 
     def get_file(self, filename):
         if filename not in self.cache:
-            code, checksum = get_source_sha(
-                directory=".", filename=os.path.join(self.rootdir, filename)
-            )
+            code, checksum = get_source_sha(directory=self.rootdir, filename=filename)
             if checksum:
                 fs_mtime = os.path.getmtime(os.path.join(self.rootdir, filename))
                 self.cache[filename] = Module(
                     source_code=code,
                     mtime=fs_mtime,
                     ext=filename.rsplit(".", 1)[1],
                     fs_checksum=checksum,
@@ -150,44 +147,39 @@
 
         if database:
             self.db = database
         else:
             self.db = db.DB(os.path.join(self.rootdir, get_data_file_path()))
 
         try:
-            git_head_sha = None
-            try:
-                git_head_sha = (
-                    check_output(["git", "rev-parse", "HEAD"]).decode("ascii").strip()
-                )
-            except (CalledProcessError, FileNotFoundError):
-                pass
             result = self.db.initiate_execution(
                 self.environment,
                 system_packages,
                 python_version,
                 {
                     "tm_client_version": TM_CLIENT_VERSION,
-                    "git_head_sha": git_head_sha,
+                    "git_head_sha": git_current_head(),
                     "ci": os.environ.get("CI"),
                 },
             )
         except (ConnectionRefusedError, Fault, ProtocolError, gaierror) as exc:
             logger.error(
                 "%s error when communication with testmon.net. (falling back to .testmondata locally)",
                 exc,
             )
             self.db = db.DB(os.path.join(self.rootdir, get_data_file_path()))
             result = self.db.initiate_execution(
                 self.environment, system_packages, python_version, {}
             )
         self.exec_id = result["exec_id"]
-        self.all_files = set(result["filenames"])
 
         self.system_packages_change = result["packages_changed"]
+        self.files_of_interest = result["filenames"]
+
+        self.all_files = {}
         self.unstable_test_names = None
         self.unstable_files = None
         self.stable_test_names = None
         self.stable_files = None
 
     def close_connection(self):
         pass
@@ -242,15 +234,15 @@
 
         to_delete = list(set(self.all_tests) - collected)
         with self.db as database:
             database.delete_test_executions(to_delete, self.exec_id)
 
     def determine_stable(self, assert_old=True):
         files_checksums = {}
-        for filename in self.all_files:
+        for filename in self.files_of_interest:
             module = self.source_tree.get_file(filename)
             if module:
                 files_checksums[filename] = module.fs_checksum
 
         new_changed_file_data = self.db.fetch_unknown_files(
             files_checksums, self.exec_id
         )
@@ -260,14 +252,15 @@
         affected_tests = self.db.determine_tests(self.exec_id, files_mhashes)[
             "affected"
         ]
 
         if assert_old:
             self.assert_old_determin_stable(affected_tests)
 
+        self.all_files = set(self.db.filenames(self.exec_id))
         self.unstable_test_names = set()
         self.unstable_files = set()
 
         for fingerprint_miss in affected_tests:
             self.unstable_test_names.add(fingerprint_miss)
             self.unstable_files.add(fingerprint_miss.split("::", 1)[0])
 
@@ -286,17 +279,27 @@
             self.exec_id,
         )
 
         _, fingerprint_misses = split_filter(
             self.source_tree, check_fingerprint, changed_file_data
         )
 
-        assert {fingerprint_miss[1] for fingerprint_miss in fingerprint_misses} == set(
+        if {fingerprint_miss[1] for fingerprint_miss in fingerprint_misses} != set(
             new_fingerprint_misses
-        )
+        ):
+            print("ERROR: old and new fingerprint misses differ.. printing old algo")
+            print(
+                "\n".join(
+                    sorted(
+                        {fingerprint_miss[1] for fingerprint_miss in fingerprint_misses}
+                    )
+                )
+            )
+            print("printing new algo")
+            print("\n".join(sorted(new_fingerprint_misses)))
 
     @property
     def avg_durations(self):
         stats = defaultdict(lambda: {"test_execution": 0, "sum_duration": 0})
 
         for (
             test_execution_id,
@@ -328,15 +331,14 @@
         self.db.insert_test_file_fps(test_executions_fingerprints, self.exec_id)
 
     def fetch_saving_stats(self, select):
         return self.db.fetch_saving_stats(self.exec_id, select)
 
 
 def get_new_mtimes(filesystem, hits):
-
     try:
         for hit in hits:
             module = filesystem.get_file(hit[0])
             if module:
                 yield module.mtime, module.fs_checksum, hit[3]
     except KeyError:
         for hit in hits:
```

### Comparing `pytest-testmon-2.0.6/testmon/tox_testmon.py` & `pytest-testmon-2.0.7b1/testmon/tox_testmon.py`

 * *Files identical despite different names*

