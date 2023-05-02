# Comparing `tmp/hx_requests-0.8.0.tar.gz` & `tmp/hx_requests-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hx_requests-0.8.0.tar", max compression
+gzip compressed data, was "hx_requests-0.9.0.tar", max compression
```

## Comparing `hx_requests-0.8.0.tar` & `hx_requests-0.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1073 2023-04-10 01:12:24.737968 hx_requests-0.8.0/LICENSE
--rw-r--r--   0        0        0     6283 2023-04-10 01:12:24.737968 hx_requests-0.8.0/README.md
--rw-r--r--   0        0        0     1799 2023-04-10 01:12:24.737968 hx_requests-0.8.0/hx_requests/.gitignore
--rw-r--r--   0        0        0       22 2023-04-10 01:12:59.026013 hx_requests-0.8.0/hx_requests/__init__.py
--rw-r--r--   0        0        0      153 2023-04-10 01:12:24.737968 hx_requests-0.8.0/hx_requests/apps.py
--rw-r--r--   0        0        0     1336 2023-04-10 01:12:24.737968 hx_requests-0.8.0/hx_requests/hx_messages.py
--rw-r--r--   0        0        0    10900 2023-04-10 01:12:24.737968 hx_requests-0.8.0/hx_requests/hx_requests.py
--rw-r--r--   0        0        0     1173 2023-04-10 01:12:24.737968 hx_requests-0.8.0/hx_requests/templates/hx_requests/modal.html
--rw-r--r--   0        0        0        0 2023-04-10 01:12:24.737968 hx_requests-0.8.0/hx_requests/templatetags/__init__.py
--rw-r--r--   0        0        0      620 2023-04-10 01:12:24.737968 hx_requests-0.8.0/hx_requests/templatetags/hx_tags.py
--rw-r--r--   0        0        0     1374 2023-04-10 01:12:24.737968 hx_requests-0.8.0/hx_requests/utils.py
--rw-r--r--   0        0        0     3199 2023-04-10 01:12:24.737968 hx_requests-0.8.0/hx_requests/views.py
--rw-r--r--   0        0        0     1435 2023-04-10 01:12:59.038013 hx_requests-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     7500 1970-01-01 00:00:00.000000 hx_requests-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-10 18:46:06.956240 hx_requests-0.9.0/LICENSE
+-rw-r--r--   0        0        0     6283 2023-04-10 18:46:06.956240 hx_requests-0.9.0/README.md
+-rw-r--r--   0        0        0     1799 2023-04-10 18:46:06.956240 hx_requests-0.9.0/hx_requests/.gitignore
+-rw-r--r--   0        0        0       22 2023-04-10 18:46:34.732752 hx_requests-0.9.0/hx_requests/__init__.py
+-rw-r--r--   0        0        0      153 2023-04-10 18:46:06.956240 hx_requests-0.9.0/hx_requests/apps.py
+-rw-r--r--   0        0        0     1336 2023-04-10 18:46:06.956240 hx_requests-0.9.0/hx_requests/hx_messages.py
+-rw-r--r--   0        0        0    10900 2023-04-10 18:46:06.956240 hx_requests-0.9.0/hx_requests/hx_requests.py
+-rw-r--r--   0        0        0     1173 2023-04-10 18:46:06.956240 hx_requests-0.9.0/hx_requests/templates/hx_requests/modal.html
+-rw-r--r--   0        0        0        0 2023-04-10 18:46:06.956240 hx_requests-0.9.0/hx_requests/templatetags/__init__.py
+-rw-r--r--   0        0        0      620 2023-04-10 18:46:06.956240 hx_requests-0.9.0/hx_requests/templatetags/hx_tags.py
+-rw-r--r--   0        0        0     1374 2023-04-10 18:46:06.956240 hx_requests-0.9.0/hx_requests/utils.py
+-rw-r--r--   0        0        0     3238 2023-04-10 18:46:06.956240 hx_requests-0.9.0/hx_requests/views.py
+-rw-r--r--   0        0        0     1435 2023-04-10 18:46:34.748752 hx_requests-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     7500 1970-01-01 00:00:00.000000 hx_requests-0.9.0/PKG-INFO
```

### Comparing `hx_requests-0.8.0/LICENSE` & `hx_requests-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hx_requests-0.8.0/README.md` & `hx_requests-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `hx_requests-0.8.0/hx_requests/.gitignore` & `hx_requests-0.9.0/hx_requests/.gitignore`

 * *Files identical despite different names*

### Comparing `hx_requests-0.8.0/hx_requests/hx_messages.py` & `hx_requests-0.9.0/hx_requests/hx_messages.py`

 * *Files identical despite different names*

### Comparing `hx_requests-0.8.0/hx_requests/hx_requests.py` & `hx_requests-0.9.0/hx_requests/hx_requests.py`

 * *Files identical despite different names*

### Comparing `hx_requests-0.8.0/hx_requests/templates/hx_requests/modal.html` & `hx_requests-0.9.0/hx_requests/templates/hx_requests/modal.html`

 * *Files identical despite different names*

### Comparing `hx_requests-0.8.0/hx_requests/templatetags/hx_tags.py` & `hx_requests-0.9.0/hx_requests/templatetags/hx_tags.py`

 * *Files identical despite different names*

### Comparing `hx_requests-0.8.0/hx_requests/utils.py` & `hx_requests-0.9.0/hx_requests/utils.py`

 * *Files identical despite different names*

### Comparing `hx_requests-0.8.0/hx_requests/views.py` & `hx_requests-0.9.0/hx_requests/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,30 +19,23 @@
     HXReqeust.
     """
 
     hx_requests: Dict = []
 
     def get(self, request: HttpRequest, *args: Any, **kwargs: Any) -> HttpResponse:
         if is_htmx_request(request):
-            super().get(request, *args, **kwargs)
-            hx_request = self.get_hx_request(request)
-            hx_request.view = self
+            hx_request = self._setup_hx_request(request, *args, **kwargs)
             kwargs = self.get_extra_kwargs(request)
-            hx_request.setup_hx_request(request)
             return hx_request.get(request, *args, **kwargs)
         return super().get(request, *args, **kwargs)
 
     def post(self, request: HttpRequest, *args: Any, **kwargs: Any) -> HttpResponse:
         if is_htmx_request(request):
-            # Call get to setup neccessary parts for the context
-            super().get(request, *args, **kwargs)
-            hx_request = self.get_hx_request(request)
-            hx_request.view = self
+            hx_request = self._setup_hx_request(request, *args, **kwargs)
             kwargs = self.get_extra_kwargs(request)
-            hx_request.setup_hx_request(request)
             return hx_request.post(request, *args, **kwargs)
         return super().post(request, *args, **kwargs)
 
     def get_hx_request(self, request):
         hx_request_name = request.GET.get("hx_request_name")
         self._get_hx_reqeust_classes()
         try:
@@ -80,7 +73,15 @@
 
     def get_extra_kwargs(self, request):
         kwargs = {}
         for key in request.GET:
             kwargs[key] = request.GET.get(key)
 
         return deserialize_kwargs(**kwargs)
+
+    def _setup_hx_request(self, request, *args, **kwargs):
+        # Call get even on post to setup neccessary parts for the context
+        super().get(request, *args, **kwargs)
+        hx_request = self.get_hx_request(request)
+        hx_request.view = self
+        hx_request.setup_hx_request(request)
+        return hx_request
```

### Comparing `hx_requests-0.8.0/pyproject.toml` & `hx_requests-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hx-requests"
-version = "0.8.0"
+version = "0.9.0"
 description = "Facilitates the usage of HTMX with Django"
 authors = ["yaakovLowenstein <lowensteinyaakov@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/yaakovLowenstein/hx-requests"
 keywords = ["django", "htmx"]
     classifiers=[
```

### Comparing `hx_requests-0.8.0/PKG-INFO` & `hx_requests-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hx-requests
-Version: 0.8.0
+Version: 0.9.0
 Summary: Facilitates the usage of HTMX with Django
 Home-page: https://github.com/yaakovLowenstein/hx-requests
 License: MIT
 Keywords: django,htmx
 Author: yaakovLowenstein
 Author-email: lowensteinyaakov@gmail.com
 Requires-Python: >=3.8,<4.0
```

