# Comparing `tmp/issue_db_api-0.6.5.tar.gz` & `tmp/issue_db_api-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "issue_db_api-0.6.5.tar", last modified: Tue May  2 11:20:19 2023, max compression
+gzip compressed data, was "issue_db_api-0.6.6.tar", last modified: Tue May  2 11:43:38 2023, max compression
```

## Comparing `issue_db_api-0.6.5.tar` & `issue_db_api-0.6.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-02 11:20:19.746783 issue_db_api-0.6.5/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       82 2023-04-20 09:20:00.000000 issue_db_api-0.6.5/.gitignore
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1069 2023-04-20 08:15:34.000000 issue_db_api-0.6.5/LICENSE
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      103 2023-04-20 08:15:34.000000 issue_db_api-0.6.5/MANIFEST.in
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-02 11:20:19.746783 issue_db_api-0.6.5/PKG-INFO
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      200 2023-04-20 08:15:34.000000 issue_db_api-0.6.5/README.md
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-02 11:20:19.742783 issue_db_api-0.6.5/issue_db_api/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      519 2023-05-02 11:19:38.000000 issue_db_api-0.6.5/issue_db_api/Cargo.toml
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       25 2023-04-20 10:30:30.000000 issue_db_api-0.6.5/issue_db_api/__init__.py
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     8096 2023-04-22 09:15:44.000000 issue_db_api-0.6.5/issue_db_api/issue_api.pyi
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-02 11:20:19.746783 issue_db_api-0.6.5/issue_db_api/src/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    44849 2023-05-02 11:19:21.000000 issue_db_api-0.6.5/issue_db_api/src/api_core.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1041 2023-04-20 08:15:34.000000 issue_db_api-0.6.5/issue_db_api/src/comments.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5280 2023-04-20 08:15:34.000000 issue_db_api-0.6.5/issue_db_api/src/config.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     3780 2023-04-22 08:55:43.000000 issue_db_api-0.6.5/issue_db_api/src/embedding.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1551 2023-04-20 08:15:34.000000 issue_db_api-0.6.5/issue_db_api/src/errors.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     8676 2023-04-20 08:15:34.000000 issue_db_api-0.6.5/issue_db_api/src/issues.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      571 2023-04-20 08:15:34.000000 issue_db_api-0.6.5/issue_db_api/src/labels.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    36983 2023-05-01 17:03:13.000000 issue_db_api-0.6.5/issue_db_api/src/lib.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    10977 2023-04-24 16:50:02.000000 issue_db_api-0.6.5/issue_db_api/src/models.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     3910 2023-05-01 16:59:08.000000 issue_db_api-0.6.5/issue_db_api/src/query.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     6385 2023-04-29 11:56:43.000000 issue_db_api-0.6.5/issue_db_api/src/repository.rs
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-02 11:20:19.746783 issue_db_api-0.6.5/issue_db_api/src/schemas/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5031 2023-04-20 08:15:34.000000 issue_db_api-0.6.5/issue_db_api/src/schemas/raw_issue_response.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       27 2023-04-20 08:15:34.000000 issue_db_api-0.6.5/issue_db_api/src/schemas.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1618 2023-04-20 08:15:34.000000 issue_db_api-0.6.5/issue_db_api/src/tags.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     2460 2023-04-22 09:10:31.000000 issue_db_api-0.6.5/issue_db_api/src/util.rs
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-02 11:20:19.742783 issue_db_api-0.6.5/issue_db_api.egg-info/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-02 11:20:19.000000 issue_db_api-0.6.5/issue_db_api.egg-info/PKG-INFO
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      748 2023-05-02 11:20:19.000000 issue_db_api-0.6.5/issue_db_api.egg-info/SOURCES.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-05-02 11:20:19.000000 issue_db_api-0.6.5/issue_db_api.egg-info/dependency_links.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.6.5/issue_db_api.egg-info/not-zip-safe
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       13 2023-05-02 11:20:19.000000 issue_db_api-0.6.5/issue_db_api.egg-info/top_level.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      529 2023-05-02 11:19:38.000000 issue_db_api-0.6.5/pyproject.toml
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       38 2023-05-02 11:20:19.746783 issue_db_api-0.6.5/setup.cfg
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      253 2023-04-20 08:15:34.000000 issue_db_api-0.6.5/setup.py
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-02 11:43:38.936177 issue_db_api-0.6.6/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       82 2023-04-20 09:20:00.000000 issue_db_api-0.6.6/.gitignore
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1069 2023-04-20 08:15:34.000000 issue_db_api-0.6.6/LICENSE
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      103 2023-04-20 08:15:34.000000 issue_db_api-0.6.6/MANIFEST.in
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-02 11:43:38.936177 issue_db_api-0.6.6/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      200 2023-04-20 08:15:34.000000 issue_db_api-0.6.6/README.md
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-02 11:43:38.932177 issue_db_api-0.6.6/issue_db_api/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      519 2023-05-02 11:43:06.000000 issue_db_api-0.6.6/issue_db_api/Cargo.toml
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       25 2023-04-20 10:30:30.000000 issue_db_api-0.6.6/issue_db_api/__init__.py
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     8096 2023-04-22 09:15:44.000000 issue_db_api-0.6.6/issue_db_api/issue_api.pyi
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-02 11:43:38.936177 issue_db_api-0.6.6/issue_db_api/src/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    44849 2023-05-02 11:19:21.000000 issue_db_api-0.6.6/issue_db_api/src/api_core.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1041 2023-04-20 08:15:34.000000 issue_db_api-0.6.6/issue_db_api/src/comments.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5280 2023-04-20 08:15:34.000000 issue_db_api-0.6.6/issue_db_api/src/config.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3780 2023-04-22 08:55:43.000000 issue_db_api-0.6.6/issue_db_api/src/embedding.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1551 2023-04-20 08:15:34.000000 issue_db_api-0.6.6/issue_db_api/src/errors.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     8676 2023-04-20 08:15:34.000000 issue_db_api-0.6.6/issue_db_api/src/issues.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      571 2023-04-20 08:15:34.000000 issue_db_api-0.6.6/issue_db_api/src/labels.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    37039 2023-05-02 11:42:57.000000 issue_db_api-0.6.6/issue_db_api/src/lib.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    10977 2023-04-24 16:50:02.000000 issue_db_api-0.6.6/issue_db_api/src/models.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3910 2023-05-01 16:59:08.000000 issue_db_api-0.6.6/issue_db_api/src/query.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     6385 2023-04-29 11:56:43.000000 issue_db_api-0.6.6/issue_db_api/src/repository.rs
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-02 11:43:38.936177 issue_db_api-0.6.6/issue_db_api/src/schemas/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5031 2023-04-20 08:15:34.000000 issue_db_api-0.6.6/issue_db_api/src/schemas/raw_issue_response.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       27 2023-04-20 08:15:34.000000 issue_db_api-0.6.6/issue_db_api/src/schemas.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1618 2023-04-20 08:15:34.000000 issue_db_api-0.6.6/issue_db_api/src/tags.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     2460 2023-04-22 09:10:31.000000 issue_db_api-0.6.6/issue_db_api/src/util.rs
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-02 11:43:38.932177 issue_db_api-0.6.6/issue_db_api.egg-info/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-02 11:43:38.000000 issue_db_api-0.6.6/issue_db_api.egg-info/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      748 2023-05-02 11:43:38.000000 issue_db_api-0.6.6/issue_db_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-05-02 11:43:38.000000 issue_db_api-0.6.6/issue_db_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.6.6/issue_db_api.egg-info/not-zip-safe
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       13 2023-05-02 11:43:38.000000 issue_db_api-0.6.6/issue_db_api.egg-info/top_level.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      529 2023-05-02 11:43:06.000000 issue_db_api-0.6.6/pyproject.toml
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       38 2023-05-02 11:43:38.936177 issue_db_api-0.6.6/setup.cfg
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      253 2023-04-20 08:15:34.000000 issue_db_api-0.6.6/setup.py
```

### Comparing `issue_db_api-0.6.5/LICENSE` & `issue_db_api-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.5/PKG-INFO` & `issue_db_api-0.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issue_db_api
-Version: 0.6.5
+Version: 0.6.6
 Author: Jesse Maarleveld
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `issue_db_api-0.6.5/issue_db_api/Cargo.toml` & `issue_db_api-0.6.6/issue_db_api/Cargo.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "issue-api-client"
-version = "0.6.5"
+version = "0.6.6"
 edition = "2021"
 
 [lib]
 name = "issue_api"
 crate-type = ["cdylib"]
 
 [features]
```

### Comparing `issue_db_api-0.6.5/issue_db_api/issue_api.pyi` & `issue_db_api-0.6.6/issue_db_api/issue_api.pyi`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.5/issue_db_api/src/api_core.rs` & `issue_db_api-0.6.6/issue_db_api/src/api_core.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.5/issue_db_api/src/comments.rs` & `issue_db_api-0.6.6/issue_db_api/src/comments.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.5/issue_db_api/src/config.rs` & `issue_db_api-0.6.6/issue_db_api/src/config.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.5/issue_db_api/src/embedding.rs` & `issue_db_api-0.6.6/issue_db_api/src/embedding.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.5/issue_db_api/src/errors.rs` & `issue_db_api-0.6.6/issue_db_api/src/errors.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.5/issue_db_api/src/issues.rs` & `issue_db_api-0.6.6/issue_db_api/src/issues.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.5/issue_db_api/src/labels.rs` & `issue_db_api-0.6.6/issue_db_api/src/labels.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.5/issue_db_api/src/lib.rs` & `issue_db_api-0.6.6/issue_db_api/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -101,22 +101,22 @@
             match num {
                 None => {
                     let msg = format!("Failed to convert float: {}", obj);
                     Err(PyValueError::new_err(msg))
                 }
                 Some(f) => Ok(Value::Number(f))
             }
+        } else if obj.is_instance_of::<PyBool>()? {     // Must be before int because issubclass(bool, int)
+            Ok(Value::Bool(obj.extract::<bool>()?))
         } else if obj.is_instance_of::<PyInt>()? {
             Ok(Value::Number(Number::from(obj.extract::<i64>()?)))
         } else if obj.is_instance_of::<PyLong>()? {
             Ok(Value::Number(Number::from(obj.extract::<i64>()?)))
         } else if obj.is_instance_of::<PyString>()? {
             Ok(Value::String(obj.extract::<String>()?))
-        } else if obj.is_instance_of::<PyBool>()? {
-            Ok(Value::Bool(obj.extract::<bool>()?))
         } else if obj.is_none() {
            Ok(Value::Null)
         } else {
             let msg = format!("Cannot convert \"{}\" object to JSON", obj.get_type().name()?);
             Err(PyTypeError::new_err(msg))
         }
     }
```

### Comparing `issue_db_api-0.6.5/issue_db_api/src/models.rs` & `issue_db_api-0.6.6/issue_db_api/src/models.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.5/issue_db_api/src/query.rs` & `issue_db_api-0.6.6/issue_db_api/src/query.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.5/issue_db_api/src/repository.rs` & `issue_db_api-0.6.6/issue_db_api/src/repository.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.5/issue_db_api/src/schemas/raw_issue_response.rs` & `issue_db_api-0.6.6/issue_db_api/src/schemas/raw_issue_response.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.5/issue_db_api/src/tags.rs` & `issue_db_api-0.6.6/issue_db_api/src/tags.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.5/issue_db_api/src/util.rs` & `issue_db_api-0.6.6/issue_db_api/src/util.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.5/issue_db_api.egg-info/PKG-INFO` & `issue_db_api-0.6.6/issue_db_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issue-db-api
-Version: 0.6.5
+Version: 0.6.6
 Author: Jesse Maarleveld
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `issue_db_api-0.6.5/issue_db_api.egg-info/SOURCES.txt` & `issue_db_api-0.6.6/issue_db_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.5/pyproject.toml` & `issue_db_api-0.6.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools.packages.find]
 where=["."]
 include = ["issue_db_api"]
 
 [project]
 name = "issue_db_api"
-version = "0.6.5"
+version = "0.6.6"
 authors = [
     {name = "Jesse Maarleveld"},
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Rust",
```

