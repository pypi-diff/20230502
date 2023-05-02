# Comparing `tmp/log10_io-0.0.4.tar.gz` & `tmp/log10_io-0.0.5.tar.gz`

## Comparing `log10_io-0.0.4.tar` & `log10_io-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 log10_io-0.0.4/requirements.txt
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 log10_io-0.0.4/setup.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 log10_io-0.0.4/.github/workflows/release.yml
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 log10_io-0.0.4/examples/chatcompletion.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 log10_io-0.0.4/examples/chatcompletion_async_vs_sync.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 log10_io-0.0.4/examples/completion.py
--rw-r--r--   0        0        0    10777 2020-02-02 00:00:00.000000 log10_io-0.0.4/examples/langchain_babyagi.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 log10_io-0.0.4/examples/langchain_multiple_tools.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 log10_io-0.0.4/examples/langchain_simple_sequential.py
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 log10_io-0.0.4/examples/langchain_sqlagent.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 log10_io-0.0.4/examples/multiple_sessions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 log10_io-0.0.4/log10/        __init__.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 log10_io-0.0.4/log10/bigquery.py
--rw-r--r--   0        0        0     9672 2020-02-02 00:00:00.000000 log10_io-0.0.4/log10/load.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 log10_io-0.0.4/log10/schemas/bigquery.json
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 log10_io-0.0.4/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 log10_io-0.0.4/LICENSE
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 log10_io-0.0.4/README.md
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 log10_io-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 log10_io-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 log10_io-0.0.5/requirements.txt
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 log10_io-0.0.5/setup.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 log10_io-0.0.5/.github/workflows/release.yml
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 log10_io-0.0.5/examples/chatcompletion.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 log10_io-0.0.5/examples/chatcompletion_async_vs_sync.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 log10_io-0.0.5/examples/completion.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 log10_io-0.0.5/examples/completion_ada.py
+-rw-r--r--   0        0        0    10777 2020-02-02 00:00:00.000000 log10_io-0.0.5/examples/langchain_babyagi.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 log10_io-0.0.5/examples/langchain_multiple_tools.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 log10_io-0.0.5/examples/langchain_simple_sequential.py
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 log10_io-0.0.5/examples/langchain_sqlagent.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 log10_io-0.0.5/examples/multiple_sessions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 log10_io-0.0.5/log10/        __init__.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 log10_io-0.0.5/log10/bigquery.py
+-rw-r--r--   0        0        0    10194 2020-02-02 00:00:00.000000 log10_io-0.0.5/log10/load.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 log10_io-0.0.5/log10/schemas/bigquery.json
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 log10_io-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 log10_io-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 log10_io-0.0.5/README.md
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 log10_io-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 log10_io-0.0.5/PKG-INFO
```

### Comparing `log10_io-0.0.4/.github/workflows/release.yml` & `log10_io-0.0.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.4/examples/chatcompletion_async_vs_sync.py` & `log10_io-0.0.5/examples/chatcompletion_async_vs_sync.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.4/examples/langchain_babyagi.py` & `log10_io-0.0.5/examples/langchain_babyagi.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.4/examples/langchain_multiple_tools.py` & `log10_io-0.0.5/examples/langchain_multiple_tools.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.4/examples/langchain_simple_sequential.py` & `log10_io-0.0.5/examples/langchain_simple_sequential.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.4/examples/langchain_sqlagent.py` & `log10_io-0.0.5/examples/langchain_sqlagent.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.4/examples/multiple_sessions.py` & `log10_io-0.0.5/examples/multiple_sessions.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.4/log10/bigquery.py` & `log10_io-0.0.5/log10/bigquery.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.4/log10/load.py` & `log10_io-0.0.5/log10/load.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 target_service = os.environ.get("LOG10_DATA_STORE")
 
 if target_service == "bigquery":
     from log10.bigquery import initialize_bigquery
     bigquery_client, bigquery_table = initialize_bigquery()
     import uuid
     from datetime import datetime, timezone
+elif target_service is None:
+    target_service = "log10"  # default to log10
 
 
 def get_session_id():
     if target_service == "bigquery":
         return str(uuid.uuid4())
 
     try:
@@ -69,22 +71,31 @@
             elapsed_time = time.perf_counter() - start_time
             logging.debug(
                 f"TIMED BLOCK - {block_name} took {elapsed_time:.6f} seconds to execute.")
     else:
         yield
 
 
+def log_url(res, completionID):
+    output = res.json()
+    organizationSlug = output['organizationSlug']
+    full_url = url + '/app/' + organizationSlug + '/completions/' + completionID
+    logging.debug(f"LOG10: Completion URL: {full_url}")
+
+
 async def log_async(completion_url, func, **kwargs):
     async with ClientSession() as session:
         res = requests.request("POST",
                                completion_url, headers={"x-log10-token": token, "Content-Type": "application/json"}, json={
                                    "organization_id": org_id
                                })
         # todo: handle session id for bigquery scenario
         completionID = res.json()['completionID']
+        if DEBUG:
+            log_url(res, completionID)
         log_row = {
             # do we want to also store args?
             "status": "started",
             "orig_module": func.__module__,
             "orig_qualname": func.__qualname__,
             "request": json.dumps(kwargs),
             "session_id": sessionID,
@@ -111,15 +122,16 @@
 
 def log_sync(completion_url, func, **kwargs):
     res = requests.request("POST",
                            completion_url, headers={"x-log10-token": token, "Content-Type": "application/json"}, json={
                                "organization_id": org_id
                            })
     completionID = res.json()['completionID']
-
+    if DEBUG:
+        log_url(res, completionID)
     res = requests.request("POST",
                            completion_url + "/" + completionID,
                            headers={"x-log10-token": token,
                                     "Content-Type": "application/json"},
                            json={
                                # do we want to also store args?
                                "status": "started",
@@ -153,15 +165,16 @@
                           "line": frame.line,
                            "lineno": frame.lineno,
                             "name": frame.name} for frame in current_stack_frame])
 
             start_time = time.perf_counter()
             output = func(*args, **kwargs)
             duration = time.perf_counter() - start_time
-            logging.debug(f"TIMED BLOCK - OpenAI call duration: {duration}")
+            logging.debug(
+                f"LOG10: TIMED BLOCK - OpenAI call duration: {duration}")
 
             if USE_ASYNC:
                 with timed_block("extra time spent waiting for log10 call"):
                     while result_queue.empty():
                         pass
                     completionID = result_queue.get()
 
@@ -175,37 +188,38 @@
 
                 if target_service == "log10":
                     res = requests.request("POST",
                                            completion_url + "/" + completionID,
                                            headers={
                                                "x-log10-token": token, "Content-Type": "application/json"},
                                            json=log_row)
-
                 elif target_service == "bigquery":
                     try:
                         log_row["id"] = str(uuid.uuid4())
-                        log_row["created_at"] = datetime.now(timezone.utc).isoformat()
+                        log_row["created_at"] = datetime.now(
+                            timezone.utc).isoformat()
                         log_row["request"] = json.dumps(kwargs)
- 
+
                         if func.__qualname__ == "Completion.create":
                             log_row["kind"] = "completion"
                         elif func.__qualname__ == "ChatCompletion.create":
                             log_row["kind"] = "chat"
 
                         log_row["orig_module"] = func.__module__
                         log_row["orig_qualname"] = func.__qualname__
                         log_row["session_id"] = sessionID
 
-                        bigquery_client.insert_rows_json(bigquery_table, [log_row])
+                        bigquery_client.insert_rows_json(
+                            bigquery_table, [log_row])
 
                     except Exception as e:
                         logging.error(
-                            f"failed to insert in Bigquery: {log_row} with error {e}")
+                            f"LOG10: failed to insert in Bigquery: {log_row} with error {e}")
         except Exception as e:
-            logging.error("failed", e)
+            logging.error("LOG10: failed", e)
 
         return output
 
     return wrapper
 
 
 def set_sync_log_text(USE_ASYNC=True):
```

### Comparing `log10_io-0.0.4/log10/schemas/bigquery.json` & `log10_io-0.0.5/log10/schemas/bigquery.json`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.4/LICENSE` & `log10_io-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.4/README.md` & `log10_io-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.4/pyproject.toml` & `log10_io-0.0.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "log10-io"
-version = "0.0.4"
+version = "0.0.5"
 authors = []
 license = "MIT"
 description = "Unified LLM data management"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `log10_io-0.0.4/PKG-INFO` & `log10_io-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log10-io
-Version: 0.0.4
+Version: 0.0.5
 Summary: Unified LLM data management
 Project-URL: Homepage, https://github.com/log10-io/log10
 Project-URL: Bug Tracker, https://github.com/log10-io/log10/issues
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

