# Comparing `tmp/issue_db_api-0.6.2.tar.gz` & `tmp/issue_db_api-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "issue_db_api-0.6.2.tar", last modified: Sat Apr 29 11:57:38 2023, max compression
+gzip compressed data, was "issue_db_api-0.6.3.tar", last modified: Mon May  1 17:30:56 2023, max compression
```

## Comparing `issue_db_api-0.6.2.tar` & `issue_db_api-0.6.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-29 11:57:38.939976 issue_db_api-0.6.2/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       82 2023-04-20 09:20:00.000000 issue_db_api-0.6.2/.gitignore
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1069 2023-04-20 08:15:34.000000 issue_db_api-0.6.2/LICENSE
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      103 2023-04-20 08:15:34.000000 issue_db_api-0.6.2/MANIFEST.in
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-04-29 11:57:38.935976 issue_db_api-0.6.2/PKG-INFO
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      200 2023-04-20 08:15:34.000000 issue_db_api-0.6.2/README.md
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-29 11:57:38.935976 issue_db_api-0.6.2/issue_db_api/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      469 2023-04-29 11:56:56.000000 issue_db_api-0.6.2/issue_db_api/Cargo.toml
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       25 2023-04-20 10:30:30.000000 issue_db_api-0.6.2/issue_db_api/__init__.py
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     8096 2023-04-22 09:15:44.000000 issue_db_api-0.6.2/issue_db_api/issue_api.pyi
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-29 11:57:38.935976 issue_db_api-0.6.2/issue_db_api/src/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    42186 2023-04-29 11:42:32.000000 issue_db_api-0.6.2/issue_db_api/src/api_core.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1041 2023-04-20 08:15:34.000000 issue_db_api-0.6.2/issue_db_api/src/comments.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5280 2023-04-20 08:15:34.000000 issue_db_api-0.6.2/issue_db_api/src/config.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     3780 2023-04-22 08:55:43.000000 issue_db_api-0.6.2/issue_db_api/src/embedding.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1551 2023-04-20 08:15:34.000000 issue_db_api-0.6.2/issue_db_api/src/errors.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     8676 2023-04-20 08:15:34.000000 issue_db_api-0.6.2/issue_db_api/src/issues.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      571 2023-04-20 08:15:34.000000 issue_db_api-0.6.2/issue_db_api/src/labels.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    36247 2023-04-22 10:20:48.000000 issue_db_api-0.6.2/issue_db_api/src/lib.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    10977 2023-04-24 16:50:02.000000 issue_db_api-0.6.2/issue_db_api/src/models.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     3425 2023-04-29 11:39:02.000000 issue_db_api-0.6.2/issue_db_api/src/query.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     6385 2023-04-29 11:56:43.000000 issue_db_api-0.6.2/issue_db_api/src/repository.rs
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-29 11:57:38.935976 issue_db_api-0.6.2/issue_db_api/src/schemas/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5031 2023-04-20 08:15:34.000000 issue_db_api-0.6.2/issue_db_api/src/schemas/raw_issue_response.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       27 2023-04-20 08:15:34.000000 issue_db_api-0.6.2/issue_db_api/src/schemas.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1618 2023-04-20 08:15:34.000000 issue_db_api-0.6.2/issue_db_api/src/tags.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     2460 2023-04-22 09:10:31.000000 issue_db_api-0.6.2/issue_db_api/src/util.rs
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-29 11:57:38.935976 issue_db_api-0.6.2/issue_db_api.egg-info/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-04-29 11:57:38.000000 issue_db_api-0.6.2/issue_db_api.egg-info/PKG-INFO
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      748 2023-04-29 11:57:38.000000 issue_db_api-0.6.2/issue_db_api.egg-info/SOURCES.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-29 11:57:38.000000 issue_db_api-0.6.2/issue_db_api.egg-info/dependency_links.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.6.2/issue_db_api.egg-info/not-zip-safe
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       13 2023-04-29 11:57:38.000000 issue_db_api-0.6.2/issue_db_api.egg-info/top_level.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      529 2023-04-29 11:56:56.000000 issue_db_api-0.6.2/pyproject.toml
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       38 2023-04-29 11:57:38.939976 issue_db_api-0.6.2/setup.cfg
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      253 2023-04-20 08:15:34.000000 issue_db_api-0.6.2/setup.py
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-01 17:30:56.597319 issue_db_api-0.6.3/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       82 2023-04-20 09:20:00.000000 issue_db_api-0.6.3/.gitignore
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1069 2023-04-20 08:15:34.000000 issue_db_api-0.6.3/LICENSE
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      103 2023-04-20 08:15:34.000000 issue_db_api-0.6.3/MANIFEST.in
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-01 17:30:56.597319 issue_db_api-0.6.3/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      200 2023-04-20 08:15:34.000000 issue_db_api-0.6.3/README.md
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-01 17:30:56.597319 issue_db_api-0.6.3/issue_db_api/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      519 2023-05-01 17:30:24.000000 issue_db_api-0.6.3/issue_db_api/Cargo.toml
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       25 2023-04-20 10:30:30.000000 issue_db_api-0.6.3/issue_db_api/__init__.py
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     8096 2023-04-22 09:15:44.000000 issue_db_api-0.6.3/issue_db_api/issue_api.pyi
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-01 17:30:56.597319 issue_db_api-0.6.3/issue_db_api/src/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    42451 2023-05-01 17:30:07.000000 issue_db_api-0.6.3/issue_db_api/src/api_core.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1041 2023-04-20 08:15:34.000000 issue_db_api-0.6.3/issue_db_api/src/comments.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5280 2023-04-20 08:15:34.000000 issue_db_api-0.6.3/issue_db_api/src/config.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3780 2023-04-22 08:55:43.000000 issue_db_api-0.6.3/issue_db_api/src/embedding.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1551 2023-04-20 08:15:34.000000 issue_db_api-0.6.3/issue_db_api/src/errors.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     8676 2023-04-20 08:15:34.000000 issue_db_api-0.6.3/issue_db_api/src/issues.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      571 2023-04-20 08:15:34.000000 issue_db_api-0.6.3/issue_db_api/src/labels.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    36983 2023-05-01 17:03:13.000000 issue_db_api-0.6.3/issue_db_api/src/lib.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    10977 2023-04-24 16:50:02.000000 issue_db_api-0.6.3/issue_db_api/src/models.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3910 2023-05-01 16:59:08.000000 issue_db_api-0.6.3/issue_db_api/src/query.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     6385 2023-04-29 11:56:43.000000 issue_db_api-0.6.3/issue_db_api/src/repository.rs
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-01 17:30:56.597319 issue_db_api-0.6.3/issue_db_api/src/schemas/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5031 2023-04-20 08:15:34.000000 issue_db_api-0.6.3/issue_db_api/src/schemas/raw_issue_response.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       27 2023-04-20 08:15:34.000000 issue_db_api-0.6.3/issue_db_api/src/schemas.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1618 2023-04-20 08:15:34.000000 issue_db_api-0.6.3/issue_db_api/src/tags.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     2460 2023-04-22 09:10:31.000000 issue_db_api-0.6.3/issue_db_api/src/util.rs
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-01 17:30:56.597319 issue_db_api-0.6.3/issue_db_api.egg-info/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-01 17:30:56.000000 issue_db_api-0.6.3/issue_db_api.egg-info/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      748 2023-05-01 17:30:56.000000 issue_db_api-0.6.3/issue_db_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-05-01 17:30:56.000000 issue_db_api-0.6.3/issue_db_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.6.3/issue_db_api.egg-info/not-zip-safe
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       13 2023-05-01 17:30:56.000000 issue_db_api-0.6.3/issue_db_api.egg-info/top_level.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      529 2023-05-01 17:30:24.000000 issue_db_api-0.6.3/pyproject.toml
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       38 2023-05-01 17:30:56.597319 issue_db_api-0.6.3/setup.cfg
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      253 2023-04-20 08:15:34.000000 issue_db_api-0.6.3/setup.py
```

### Comparing `issue_db_api-0.6.2/LICENSE` & `issue_db_api-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.2/PKG-INFO` & `issue_db_api-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issue_db_api
-Version: 0.6.2
+Version: 0.6.3
 Author: Jesse Maarleveld
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `issue_db_api-0.6.2/issue_db_api/issue_api.pyi` & `issue_db_api-0.6.3/issue_db_api/issue_api.pyi`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.2/issue_db_api/src/api_core.rs` & `issue_db_api-0.6.3/issue_db_api/src/api_core.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 use std::collections::HashMap;
+use std::io::Write;
 
 #[cfg(feature = "blocking")]
 use reqwest::blocking::Client;
 use reqwest::blocking::{ClientBuilder, multipart};
 
 use serde_json::{Map, Value};
 use lazy_init::Lazy;
@@ -399,20 +400,29 @@
                                  suffix: &str,
                                  verb: Verb,
                                  payload: I,
                                  target_path: String) -> APIResult<()>
         where
             I: serde::Serialize,
     {
-        let response = self.build_request_base(suffix, verb)?.json(&payload).send()?;
-        let data = self.handle_error_status(response)?.bytes()?;
-        let mut cursor = std::io::Cursor::new(data);
+        let url = self.get_endpoint(suffix);
+        let client = reqwest::Client::new();
+        let rt = tokio::runtime::Builder::new_current_thread().enable_all().build()?;
         let mut file = std::fs::File::create(target_path)?;
-        std::io::copy(&mut cursor, &mut file)?;
-        Ok(())
+        let result: APIResult<()> = rt.block_on(async {
+            let mut stream = client
+                .get(url)
+                .send()
+                .await?;
+            while let Some(chunk) = stream.chunk().await? {
+                file.write_all(chunk.as_ref())?;
+            }
+            Ok(())
+        });
+        result
     }
 
     /***************************************************************************
      * Issue-related endpoints
      */
 
     pub(crate) fn search(&self, query: Query) -> APIResult<Vec<String>> {
```

### Comparing `issue_db_api-0.6.2/issue_db_api/src/comments.rs` & `issue_db_api-0.6.3/issue_db_api/src/comments.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.2/issue_db_api/src/config.rs` & `issue_db_api-0.6.3/issue_db_api/src/config.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.2/issue_db_api/src/embedding.rs` & `issue_db_api-0.6.3/issue_db_api/src/embedding.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.2/issue_db_api/src/errors.rs` & `issue_db_api-0.6.3/issue_db_api/src/errors.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.2/issue_db_api/src/issues.rs` & `issue_db_api-0.6.3/issue_db_api/src/issues.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.2/issue_db_api/src/labels.rs` & `issue_db_api-0.6.3/issue_db_api/src/labels.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.2/issue_db_api/src/lib.rs` & `issue_db_api-0.6.3/issue_db_api/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -361,14 +361,25 @@
                     IssueAPIError::new_err(
                         "issues_api.Query.tag cannot be called on a tag-query."
                     )
                 )
             }
             Ok(Query::Tag(cmp, name))
         }
+        
+        fn add_exists(&self, name: String, state: bool) -> PyResult<Query> {
+            if self.query.is_some() {
+                return Err(
+                    IssueAPIError::new_err(
+                        "issues_api.Query.tag cannot be called on a tag-query."
+                    )
+                )
+            }
+            Ok(Query::Exists(name, state))
+        }
 
         fn get_query(&self) -> PyResult<Query> {
             match self.query {
                 None => Err(
                     IssueAPIError::new_err("Cannot perform search with empty query")
                 ),
                 Some(ref q) => Ok(q.clone())
@@ -405,14 +416,26 @@
         fn tag(&self, name: String) -> PyResult<Self> {
             Ok(Self{query: Some(self.add_tag(name, QueryCMP::Eq)?)})
         }
 
         fn not_tag(&self, name: String) -> PyResult<Self> {
             Ok(Self{query: Some(self.add_tag(name, QueryCMP::Ne)?)})
         }
+        
+        fn exists(&self, field: String) -> PyResult<Self> {
+            Ok(
+                Self{query: Some(self.add_exists(field, true)?)}
+            )
+        }
+        
+        fn not_exists(&self, field: String) -> PyResult<Self> {
+            Ok(
+                Self{query: Some(self.add_exists(field, false)?)}
+            )
+        }
 
         fn to_json(&self, py: Python<'_>) -> PyResult<PyObject> {
             match self.query {
                 None => Ok(py.None()),
                 Some(ref q) => Ok(json_to_py(py, q.clone().into_json()))
             }
         }
```

### Comparing `issue_db_api-0.6.2/issue_db_api/src/models.rs` & `issue_db_api-0.6.3/issue_db_api/src/models.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.2/issue_db_api/src/query.rs` & `issue_db_api-0.6.3/issue_db_api/src/query.rs`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 #[derive(Debug, Clone)]
 pub enum Query {
     Tag(QueryCMP, String),
     Project(String),
     Identifier(String),
     Key(String),
     And(Vec<Query>),
-    Or(Vec<Query>)
+    Or(Vec<Query>),
+    Exists(String, bool)
 }
 
 
 #[allow(unused)]
 #[derive(Debug, Copy, Clone)]
 pub enum QueryCMP { Eq, Ne }
 
@@ -52,14 +53,21 @@
                 Value::Object(map)
             }
             Query::Or(branches) => {
                 let mut map = Map::new();
                 map.insert("$or".to_string(), serialize_logical_op_branches(branches));
                 Value::Object(map)
             }
+            Query::Exists(field, state) => {
+                let mut map = Map::new();
+                let mut inner_map = Map::new();
+                inner_map.insert("$exists".to_string(), Value::Bool(state));
+                map.insert(field, Value::Object(inner_map));
+                Value::Object(map)
+            }
         }
     }
 }
 
 fn serialize_logical_op_branches(arms: Vec<Query>) -> Value {
     let mut json_branches: Vec<Value> = Vec::with_capacity(arms.len());
     for branch in arms {
@@ -78,22 +86,25 @@
             },
             Query::Project(project) => write!(f, "{{\"tags\": {{\"$eq\": \"{}\"}}}}", project),
             Query::Identifier(ident) => write!(f, "{{\"_id\": {{\"$eq\": \"{}\"}}}}", ident),
             Query::Key(key) => write!(f, "{{\"key\": {{\"$eq\": \"{}\"}}}}", key),
             Query::And(arms)=> {
                 write!(f, "{{\"$and\": [")?;
                 write_logical_op_body(f, arms)?;
-                write!(f, "]")?;
+                write!(f, "]}}")?;
                 Ok(())
             },
             Query::Or(arms) => {
                 write!(f, "{{\"$or\": [")?;
                 write_logical_op_body(f, arms)?;
-                write!(f, "]")?;
+                write!(f, "]}}")?;
                 Ok(())
+            },
+            Query::Exists(value, state) => {
+                write!(f, "\"{}\": {{\"$exists\": {}}}}}", value, state)
             }
         }
     }
 }
 
 fn write_logical_op_body(f: &mut Formatter<'_>, arms: &Vec<Query>) -> std::fmt::Result {
     let mut first = true;
```

### Comparing `issue_db_api-0.6.2/issue_db_api/src/repository.rs` & `issue_db_api-0.6.3/issue_db_api/src/repository.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.2/issue_db_api/src/schemas/raw_issue_response.rs` & `issue_db_api-0.6.3/issue_db_api/src/schemas/raw_issue_response.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.2/issue_db_api/src/tags.rs` & `issue_db_api-0.6.3/issue_db_api/src/tags.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.2/issue_db_api/src/util.rs` & `issue_db_api-0.6.3/issue_db_api/src/util.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.2/issue_db_api.egg-info/PKG-INFO` & `issue_db_api-0.6.3/issue_db_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issue-db-api
-Version: 0.6.2
+Version: 0.6.3
 Author: Jesse Maarleveld
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `issue_db_api-0.6.2/issue_db_api.egg-info/SOURCES.txt` & `issue_db_api-0.6.3/issue_db_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.2/pyproject.toml` & `issue_db_api-0.6.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools.packages.find]
 where=["."]
 include = ["issue_db_api"]
 
 [project]
 name = "issue_db_api"
-version = "0.6.2"
+version = "0.6.3"
 authors = [
     {name = "Jesse Maarleveld"},
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Rust",
```

