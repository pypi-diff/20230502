# Comparing `tmp/quilt3-5.3.0.tar.gz` & `tmp/quilt3-5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/quilt/quilt/api/python/dist/.tmp-tptj4r8t/quilt3-5.3.0.tar", last modified: Tue Apr 11 14:19:20 2023, max compression
+gzip compressed data, was "/home/runner/work/quilt/quilt/api/python/dist/.tmp-bhlkdpzo/quilt3-5.3.1.tar", last modified: Tue May  2 11:19:41 2023, max compression
```

## Comparing `quilt3-5.3.0.tar` & `quilt3-5.3.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:19:20.000000 quilt3-5.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-11 14:18:57.000000 quilt3-5.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-11 14:18:57.000000 quilt3-5.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-11 14:19:20.000000 quilt3-5.3.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:19:20.000000 quilt3-5.3.0/quilt3/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:19:20.000000 quilt3-5.3.0/quilt3/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/backends/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/backends/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    47152 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    42579 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    62972 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/search_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)    19087 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:19:20.000000 quilt3-5.3.0/quilt3/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)    11102 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-11 14:18:57.000000 quilt3-5.3.0/quilt3/workflows/config-1.schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:19:20.000000 quilt3-5.3.0/quilt3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-11 14:19:20.000000 quilt3-5.3.0/quilt3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-11 14:19:20.000000 quilt3-5.3.0/quilt3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:19:20.000000 quilt3-5.3.0/quilt3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-11 14:19:20.000000 quilt3-5.3.0/quilt3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-11 14:19:20.000000 quilt3-5.3.0/quilt3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 14:19:20.000000 quilt3-5.3.0/quilt3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 14:19:20.000000 quilt3-5.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-11 14:18:57.000000 quilt3-5.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:19:20.000000 quilt3-5.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-04-11 14:18:57.000000 quilt3-5.3.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-04-11 14:18:57.000000 quilt3-5.3.0/tests/test_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-04-11 14:18:57.000000 quilt3-5.3.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    24967 2023-04-11 14:18:57.000000 quilt3-5.3.0/tests/test_data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-04-11 14:18:57.000000 quilt3-5.3.0/tests/test_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-11 14:18:57.000000 quilt3-5.3.0/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-11 14:18:57.000000 quilt3-5.3.0/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-11 14:18:57.000000 quilt3-5.3.0/tests/test_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-04-11 14:18:57.000000 quilt3-5.3.0/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-04-11 14:18:57.000000 quilt3-5.3.0/tests/test_workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:19:41.000000 quilt3-5.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-02 11:19:23.000000 quilt3-5.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-02 11:19:23.000000 quilt3-5.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-02 11:19:41.000000 quilt3-5.3.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:19:41.000000 quilt3-5.3.1/quilt3/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 11:19:23.000000 quilt3-5.3.1/quilt3/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-02 11:19:23.000000 quilt3-5.3.1/quilt3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-02 11:19:23.000000 quilt3-5.3.1/quilt3/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-05-02 11:19:23.000000 quilt3-5.3.1/quilt3/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:19:41.000000 quilt3-5.3.1/quilt3/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-02 11:19:23.000000 quilt3-5.3.1/quilt3/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-05-02 11:19:23.000000 quilt3-5.3.1/quilt3/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-02 11:19:23.000000 quilt3-5.3.1/quilt3/backends/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-05-02 11:19:23.000000 quilt3-5.3.1/quilt3/backends/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-05-02 11:19:23.000000 quilt3-5.3.1/quilt3/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47152 2023-05-02 11:19:23.000000 quilt3-5.3.1/quilt3/data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-02 11:19:23.000000 quilt3-5.3.1/quilt3/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42579 2023-05-02 11:19:23.000000 quilt3-5.3.1/quilt3/formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-02 11:19:23.000000 quilt3-5.3.1/quilt3/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16592 2023-05-02 11:19:23.000000 quilt3-5.3.1/quilt3/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63367 2023-05-02 11:19:23.000000 quilt3-5.3.1/quilt3/packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-02 11:19:23.000000 quilt3-5.3.1/quilt3/search_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-05-02 11:19:23.000000 quilt3-5.3.1/quilt3/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-05-02 11:19:23.000000 quilt3-5.3.1/quilt3/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19087 2023-05-02 11:19:23.000000 quilt3-5.3.1/quilt3/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:19:41.000000 quilt3-5.3.1/quilt3/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)    11102 2023-05-02 11:19:23.000000 quilt3-5.3.1/quilt3/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-05-02 11:19:23.000000 quilt3-5.3.1/quilt3/workflows/config-1.schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:19:41.000000 quilt3-5.3.1/quilt3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-02 11:19:41.000000 quilt3-5.3.1/quilt3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-02 11:19:41.000000 quilt3-5.3.1/quilt3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 11:19:41.000000 quilt3-5.3.1/quilt3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-02 11:19:41.000000 quilt3-5.3.1/quilt3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-02 11:19:41.000000 quilt3-5.3.1/quilt3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 11:19:41.000000 quilt3-5.3.1/quilt3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 11:19:41.000000 quilt3-5.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-02 11:19:23.000000 quilt3-5.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:19:41.000000 quilt3-5.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-05-02 11:19:23.000000 quilt3-5.3.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-05-02 11:19:23.000000 quilt3-5.3.1/tests/test_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-05-02 11:19:23.000000 quilt3-5.3.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24967 2023-05-02 11:19:23.000000 quilt3-5.3.1/tests/test_data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-05-02 11:19:23.000000 quilt3-5.3.1/tests/test_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-02 11:19:23.000000 quilt3-5.3.1/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-05-02 11:19:23.000000 quilt3-5.3.1/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-02 11:19:23.000000 quilt3-5.3.1/tests/test_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-05-02 11:19:23.000000 quilt3-5.3.1/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-05-02 11:19:23.000000 quilt3-5.3.1/tests/test_workflows.py
```

### Comparing `quilt3-5.3.0/LICENSE` & `quilt3-5.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quilt3-5.3.0/PKG-INFO` & `quilt3-5.3.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quilt3
-Version: 5.3.0
+Version: 5.3.1
 Summary: Quilt: where data comes together
 Home-page: https://github.com/quiltdata/quilt
 Author: quiltdata
 Author-email: contact@quiltdata.io
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `quilt3-5.3.0/quilt3/__init__.py` & `quilt3-5.3.1/quilt3/__init__.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.3.0/quilt3/admin.py` & `quilt3-5.3.1/quilt3/admin.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.3.0/quilt3/api.py` & `quilt3-5.3.1/quilt3/api.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.3.0/quilt3/backends/__init__.py` & `quilt3-5.3.1/quilt3/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.3.0/quilt3/backends/base.py` & `quilt3-5.3.1/quilt3/backends/base.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.3.0/quilt3/backends/local.py` & `quilt3-5.3.1/quilt3/backends/local.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.3.0/quilt3/backends/s3.py` & `quilt3-5.3.1/quilt3/backends/s3.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.3.0/quilt3/bucket.py` & `quilt3-5.3.1/quilt3/bucket.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.3.0/quilt3/data_transfer.py` & `quilt3-5.3.1/quilt3/data_transfer.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.3.0/quilt3/formats.py` & `quilt3-5.3.1/quilt3/formats.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.3.0/quilt3/imports.py` & `quilt3-5.3.1/quilt3/imports.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.3.0/quilt3/main.py` & `quilt3-5.3.1/quilt3/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,15 +288,15 @@
             help="Which page in the local catalog to open. Leave blank to go to the catalog landing page, pass in an "
                  "s3 url (e.g. 's3://bucket/myfile.txt') to go to file viewer, or pass in a package name in the form "
                  "'BUCKET:USER/PKG' to go to the package viewer.",
             type=str,
             nargs="?"
     )
     catalog_p.add_argument(
-            "--detailed_help",
+            "--detailed-help", "--detailed_help",
             help="Display detailed information about this command and then exit",
             action="store_true",
     )
     catalog_p.add_argument(
         "--host",
         type=str,
         default="127.0.0.1",
```

### Comparing `quilt3-5.3.0/quilt3/packages.py` & `quilt3-5.3.1/quilt3/packages.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,18 @@
 # > The maximum length of a record in the input or result is 1 MB.
 # The actual limit is 1 MiB, but it's rounded because column names are included in this limit.
 DEFAULT_MANIFEST_MAX_RECORD_SIZE = 1_000_000
 MANIFEST_MAX_RECORD_SIZE = util.get_pos_int_from_env('QUILT_MANIFEST_MAX_RECORD_SIZE')
 if MANIFEST_MAX_RECORD_SIZE is None:
     MANIFEST_MAX_RECORD_SIZE = DEFAULT_MANIFEST_MAX_RECORD_SIZE
 
+SUPPORTED_HASH_TYPES = (
+    "SHA256",
+)
+
 
 def _fix_docstring(**kwargs):
     def f(wrapped):
         if sys.flags.optimize < 2:
             wrapped.__doc__ = textwrap.dedent(wrapped.__doc__) % kwargs
         return wrapped
     return f
@@ -88,14 +92,23 @@
 
 def _filesystem_safe_encode(key):
     """Returns the sha256 of the key. This ensures there are no slashes, uppercase/lowercase conflicts,
     avoids `OSError: [Errno 36] File name too long:`, etc."""
     return hashlib.sha256(key.encode()).hexdigest()
 
 
+def _check_hash_type_support(hash_type: str) -> None:
+    if hash_type not in SUPPORTED_HASH_TYPES:
+        raise QuiltException(
+            f"Unsupported hash type: {hash_type!r}. "
+            f"Supported types: {', '.join(SUPPORTED_HASH_TYPES)}. "
+            "Try to update quilt3."
+        )
+
+
 class ObjectPathCache:
     @classmethod
     def _cache_path(cls, url):
         url_hash = _filesystem_safe_encode(url)
         return CACHE_PATH / url_hash[0:2] / url_hash[2:]
 
     @classmethod
@@ -192,16 +205,15 @@
 
     def _verify_hash(self, read_bytes):
         """
         Verifies hash of bytes
         """
         if self.hash is None:
             raise QuiltException("Hash missing - need to build the package")
-        if self.hash.get('type') != 'SHA256':
-            raise NotImplementedError
+        _check_hash_type_support(self.hash.get('type'))
         digest = hashlib.sha256(read_bytes).hexdigest()
         if digest != self.hash.get('value'):
             raise QuiltException("Hash validation failed")
 
     def set(self, path=None, meta=None):
         """
         Returns self with the physical key set to path.
@@ -1319,17 +1331,17 @@
         `new_pkg["entry_1"] = ["s3://bucket/prefix/entry_1.json"]`
 
         By default, push will not overwrite an existing package if its top hash does not match
         the parent hash of the package being pushed. Use `force=True` to skip the check.
 
         Args:
             name: name for package in registry
-            dest: where to copy the objects in the package
-                Must be either an S3 URI prefix in the registry bucket, or a callable that takes
-                logical_key, package_entry, and top_hash and returns S3 URI. S3 URIs format is s3://$bucket/$key.
+            dest: where to copy the objects in the package. Must be either an S3 URI prefix (e.g., s3://$bucket/$key)
+                in the registry bucket, or a callable that takes logical_key, package_entry, and top_hash
+                and returns an S3 URI.
             registry: registry where to create the new package
             message: the commit message for the new package
             selector_fn: An optional function that determines which package entries should be copied to S3.
                 The function takes in two arguments, logical_key and package_entry, and should return False if that
                 PackageEntry should not be copied to the destination registry during push.
                 If for example you have a package where the files are spread over multiple buckets
                 and you add a single local file, you can use selector_fn to only
@@ -1647,14 +1659,17 @@
         Args:
             src(str): URL of the directory
             extra_files_ok(bool): Whether extra files in the directory should cause a failure.
 
         Returns:
             True if the package matches the directory; False otherwise.
         """
+        for lk, e in self.walk():
+            _check_hash_type_support(e.hash["type"])
+
         src = PhysicalKey.from_url(fix_url(src))
         src_dict = dict(list_url(src))
         url_list = []
         size_list = []
         for logical_key, entry in self.walk():
             src_size = src_dict.pop(logical_key, None)
             if src_size is None:
```

### Comparing `quilt3-5.3.0/quilt3/search_util.py` & `quilt3-5.3.1/quilt3/search_util.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.3.0/quilt3/session.py` & `quilt3-5.3.1/quilt3/session.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.3.0/quilt3/telemetry.py` & `quilt3-5.3.1/quilt3/telemetry.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.3.0/quilt3/util.py` & `quilt3-5.3.1/quilt3/util.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.3.0/quilt3/workflows/__init__.py` & `quilt3-5.3.1/quilt3/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.3.0/quilt3/workflows/config-1.schema.json` & `quilt3-5.3.1/quilt3/workflows/config-1.schema.json`

 * *Files identical despite different names*

### Comparing `quilt3-5.3.0/quilt3.egg-info/PKG-INFO` & `quilt3-5.3.1/quilt3.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quilt3
-Version: 5.3.0
+Version: 5.3.1
 Summary: Quilt: where data comes together
 Home-page: https://github.com/quiltdata/quilt
 Author: quiltdata
 Author-email: contact@quiltdata.io
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `quilt3-5.3.0/quilt3.egg-info/SOURCES.txt` & `quilt3-5.3.1/quilt3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quilt3-5.3.0/quilt3.egg-info/requires.txt` & `quilt3-5.3.1/quilt3.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `quilt3-5.3.0/setup.py` & `quilt3-5.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.3.0/tests/test_api.py` & `quilt3-5.3.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.3.0/tests/test_bucket.py` & `quilt3-5.3.1/tests/test_bucket.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.3.0/tests/test_cli.py` & `quilt3-5.3.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.3.0/tests/test_data_transfer.py` & `quilt3-5.3.1/tests/test_data_transfer.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.3.0/tests/test_formats.py` & `quilt3-5.3.1/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.3.0/tests/test_search.py` & `quilt3-5.3.1/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.3.0/tests/test_session.py` & `quilt3-5.3.1/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.3.0/tests/test_telemetry.py` & `quilt3-5.3.1/tests/test_telemetry.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.3.0/tests/test_util.py` & `quilt3-5.3.1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `quilt3-5.3.0/tests/test_workflows.py` & `quilt3-5.3.1/tests/test_workflows.py`

 * *Files identical despite different names*

