# Comparing `tmp/wtt02-0.3.2.tar.gz` & `tmp/wtt02-0.3.3.tar.gz`

## Comparing `wtt02-0.3.2.tar` & `wtt02-0.3.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 wtt02-0.3.2/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtt02-0.3.2/tests/__init__.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 wtt02-0.3.2/tests/test_load.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 wtt02-0.3.2/wtt02/__about__.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 wtt02-0.3.2/wtt02/__init__.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 wtt02-0.3.2/wtt02/_env.py
--rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 wtt02-0.3.2/wtt02/main.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 wtt02-0.3.2/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 wtt02-0.3.2/LICENSE.txt
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 wtt02-0.3.2/README.md
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 wtt02-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 wtt02-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 wtt02-0.3.3/Makefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtt02-0.3.3/tests/__init__.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 wtt02-0.3.3/tests/test_load.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 wtt02-0.3.3/wtt02/__about__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 wtt02-0.3.3/wtt02/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 wtt02-0.3.3/wtt02/_env.py
+-rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 wtt02-0.3.3/wtt02/main.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 wtt02-0.3.3/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 wtt02-0.3.3/LICENSE.txt
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 wtt02-0.3.3/README.md
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 wtt02-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 wtt02-0.3.3/PKG-INFO
```

### Comparing `wtt02-0.3.2/tests/test_load.py` & `wtt02-0.3.3/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `wtt02-0.3.2/wtt02/main.py` & `wtt02-0.3.3/wtt02/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Package for wtt02."""
 
+import gzip
 from pathlib import Path
+import shutil
 from typing import Optional, Union
 import os
 import logging
 
 import platform
 import zipfile
 import tempfile
@@ -39,15 +41,14 @@
     return con.execute(file_path.read_text())
 
 
 def get_connection(
     database: str = ":memory:",
     read_only: bool = False,
     config: Optional[dict] = None,
-    s3_uri: Optional[str] = None,
     file_path: Optional[Path] = None,
 ) -> duckdb.DuckDBPyConnection:
     """Return a connection with wtt02 loaded."""
     if "WTT_02_LICENSE" not in os.environ:
         raise WTT02ConfigurationException(
             "WTT_02_LICENSE environment variable not set. "
             "Check the docs or email at help@wheretrue.com"
@@ -63,67 +64,72 @@
         read_only=read_only,
         config=config,
     )
 
     try:
         con.load_extension(EXTENSION_NAME)
         return con
-    except duckdb.IOException:
-        logger.info("Extension not found, installing. This only happens once per version/matchine.")
+    except duckdb.IOException as exp:
+        logger.info("Extension not found, installing. This only happens once per version/machine.")
         extension_path = os.getenv("WTT02_EXTENSION_PATH")
 
         if extension_path:
             extension_path = Path(extension_path).absolute()
             con.install_extension(str(extension_path), force_install=True)
             con.load_extension(EXTENSION_NAME)
 
         elif file_path is not None and file_path.exists():
             con.install_extension(str(file_path.absolute()), force_install=True)
             con.load_extension(EXTENSION_NAME)
 
-        elif s3_uri is not None:
-            # download
-            pass
-
         else:
+            version = __version__
+            name = "wtt02"
+
             platform_uname = platform.uname()
             operating_system = platform_uname.system
             architecture = platform_uname.machine
-            version = __version__
 
-            from wtt02._env import ENVIRONMENT
-
-            name = "wtt02"
-            bucket = f"wtt-02-dist-{ENVIRONMENT}"
-            filename = f"{name}-{version}-{operating_system}-{architecture}.zip"
-
-            full_s3_path = (
-                f"http://{bucket}.s3.amazonaws.com/extension/{name}/{filename}"
-            )
-            logger.info("Downloading extension from %s", full_s3_path)
+            if operating_system.lower() == "windows":
+                duckdb_arch = "windows_amd64"
+            elif operating_system.lower() == "darwin" and architecture.lower() == "x86_64":
+                duckdb_arch = "osx_amd64"
+            elif operating_system.lower() == "darwin" and architecture.lower() == "arm64":
+                duckdb_arch = "osx_arm64"
+            elif operating_system.lower() == "linux" and architecture.lower() == "x86_64":
+                duckdb_arch = "linux_amd64_gcc4"
+            else:
+                raise WTTException(
+                    f"Unable to find extension for {operating_system} {architecture}"
+                )
+
+            filename = f"{name}.duckdb_extension.gz"
+            url = f"https://dbe.wheretrue.com/{name}/{version}/v0.7.1/{duckdb_arch}/{filename}"
+            logger.info("Downloading extension from %s", url)
 
             with tempfile.TemporaryDirectory() as temp_dir:
                 temp_dir_path = Path(temp_dir)
                 temp_file_name = temp_dir_path / filename
 
                 try:
-                    urllib.request.urlretrieve(full_s3_path, temp_file_name)
+                    urllib.request.urlretrieve(url, temp_file_name)
                 except Exception as exp:
                     raise WTTException(
-                        f"Unable to download extension from {full_s3_path}"
+                        f"Unable to download extension from {url}"
                     ) from exp
 
-                with zipfile.ZipFile(temp_file_name, "r") as zip_ref:
-                    zip_ref.extract(f"{name}.duckdb_extension", temp_dir)
+                output_file = temp_dir_path / filename.rstrip(".gz")
+                with gzip.open(temp_file_name, "rb") as f_in:
+                    with open(output_file, "wb") as f_out:
+                        shutil.copyfileobj(f_in, f_out)
 
-                output_file = temp_dir_path / f"{name}.duckdb_extension"
                 if not output_file.exists():
                     raise WTTException(
                         f"Unable to find extension file at {output_file}"
-                    )
+                    ) from exp
 
                 logging.info("Installing extension from %s", output_file)
                 con.install_extension(output_file.as_posix(), force_install=True)
 
                 con.load_extension(EXTENSION_NAME)
 
     return con
```

### Comparing `wtt02-0.3.2/LICENSE.txt` & `wtt02-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wtt02-0.3.2/pyproject.toml` & `wtt02-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wtt02-0.3.2/PKG-INFO` & `wtt02-0.3.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wtt02
-Version: 0.3.2
+Version: 0.3.3
 Author-email: Trent Hauck <thauck@wheretrue.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

