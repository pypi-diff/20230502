# Comparing `tmp/pybravia-0.3.2.tar.gz` & `tmp/pybravia-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybravia-0.3.2.tar", max compression
+gzip compressed data, was "pybravia-0.3.3.tar", max compression
```

## Comparing `pybravia-0.3.2.tar` & `pybravia-0.3.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     3070 2023-03-03 09:36:54.775432 pybravia-0.3.2/README.md
--rw-r--r--   0        0        0      317 2023-03-03 09:36:54.775432 pybravia-0.3.2/pybravia/__init__.py
--rw-r--r--   0        0        0    21109 2023-03-03 09:36:54.775432 pybravia-0.3.2/pybravia/client.py
--rw-r--r--   0        0        0      544 2023-03-03 09:36:54.775432 pybravia-0.3.2/pybravia/const.py
--rw-r--r--   0        0        0      638 2023-03-03 09:36:54.775432 pybravia-0.3.2/pybravia/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-03 09:36:54.775432 pybravia-0.3.2/pybravia/py.typed
--rw-r--r--   0        0        0      444 2023-03-03 09:36:54.775432 pybravia-0.3.2/pybravia/util.py
--rw-r--r--   0        0        0      644 2023-03-03 09:36:54.775432 pybravia-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     3775 1970-01-01 00:00:00.000000 pybravia-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     3070 2023-05-02 21:50:22.711235 pybravia-0.3.3/README.md
+-rw-r--r--   0        0        0      317 2023-05-02 21:50:22.711235 pybravia-0.3.3/pybravia/__init__.py
+-rw-r--r--   0        0        0    21399 2023-05-02 21:50:22.711235 pybravia-0.3.3/pybravia/client.py
+-rw-r--r--   0        0        0      544 2023-05-02 21:50:22.711235 pybravia-0.3.3/pybravia/const.py
+-rw-r--r--   0        0        0      638 2023-05-02 21:50:22.711235 pybravia-0.3.3/pybravia/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-02 21:50:22.711235 pybravia-0.3.3/pybravia/py.typed
+-rw-r--r--   0        0        0      444 2023-05-02 21:50:22.711235 pybravia-0.3.3/pybravia/util.py
+-rw-r--r--   0        0        0      644 2023-05-02 21:50:22.715235 pybravia-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     3775 1970-01-01 00:00:00.000000 pybravia-0.3.3/PKG-INFO
```

### Comparing `pybravia-0.3.2/README.md` & `pybravia-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pybravia-0.3.2/pybravia/client.py` & `pybravia-0.3.3/pybravia/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -384,30 +384,38 @@
             {"scheme": scheme},
         )
         result = resp.get("result", [[]])[0]
         return [d["source"] for d in result if "source" in d]
 
     async def get_content_count(self, source: str) -> int:
         """Get count of contents in the source."""
+
+        # Extended timeout due to
+        # https://github.com/home-assistant/core/issues/91781#issuecomment-1532151925
         resp = await self.send_rest_req(
             SERVICE_AV_CONTENT,
             "getContentCount",
             {"source": source},
+            timeout=20,
         )
         result = resp.get("result", [{}])[0]
         return result.get("count", 0)
 
     async def get_content_list(
         self, source: str, index: int = 0, count: int = 50
     ) -> list[dict[str, Any]]:
         """Get list of contents in the source."""
+
+        # Extended timeout due to
+        # https://github.com/home-assistant/core/issues/91781#issuecomment-1532168838
         resp = await self.send_rest_req(
             SERVICE_AV_CONTENT,
             "getContentList",
             {"source": source, "stIdx": index, "cnt": count},
+            timeout=20,
         )
         result = resp.get("result", [[]])[0]
         return result
 
     async def get_content_list_full(self, source: str) -> list[dict[str, Any]]:
         """Get full list of contents in the source."""
         result = []
```

### Comparing `pybravia-0.3.2/pybravia/const.py` & `pybravia-0.3.3/pybravia/const.py`

 * *Files identical despite different names*

### Comparing `pybravia-0.3.2/pybravia/exceptions.py` & `pybravia-0.3.3/pybravia/exceptions.py`

 * *Files identical despite different names*

### Comparing `pybravia-0.3.2/pyproject.toml` & `pybravia-0.3.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybravia"
-version = "0.3.2"
+version = "0.3.3"
 description = "Python async library for remote control of Sony Bravia TVs 2013 and newer."
 authors = ["Arem Draft <artemon_93@mail.ru>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Drafteed/pybravia"
 packages = [
   { include = "pybravia" }
```

### Comparing `pybravia-0.3.2/PKG-INFO` & `pybravia-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybravia
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python async library for remote control of Sony Bravia TVs 2013 and newer.
 Home-page: https://github.com/Drafteed/pybravia
 License: MIT
 Author: Arem Draft
 Author-email: artemon_93@mail.ru
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

