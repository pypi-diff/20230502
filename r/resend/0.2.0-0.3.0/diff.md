# Comparing `tmp/resend-0.2.0.tar.gz` & `tmp/resend-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/resend-0.2.0.tar", last modified: Wed Apr 26 01:56:23 2023, max compression
+gzip compressed data, was "dist/resend-0.3.0.tar", last modified: Tue May  2 21:42:06 2023, max compression
```

## Comparing `resend-0.2.0.tar` & `resend-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2023-04-26 01:56:23.000000 resend-0.2.0/
--rw-r--r--   0 derich     (501) staff       (20)     2392 2023-04-26 01:56:23.000000 resend-0.2.0/PKG-INFO
--rw-r--r--   0 derich     (501) staff       (20)     1263 2023-04-24 23:51:39.000000 resend-0.2.0/README.md
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2023-04-26 01:56:23.000000 resend-0.2.0/resend/
--rw-r--r--   0 derich     (501) staff       (20)       94 2023-04-24 23:51:39.000000 resend-0.2.0/resend/__init__.py
--rw-r--r--   0 derich     (501) staff       (20)     2327 2023-04-26 01:56:07.000000 resend-0.2.0/resend/api.py
--rw-r--r--   0 derich     (501) staff       (20)     3385 2023-04-24 23:51:39.000000 resend-0.2.0/resend/exceptions.py
--rw-r--r--   0 derich     (501) staff       (20)      163 2023-04-26 01:56:07.000000 resend-0.2.0/resend/version.py
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2023-04-26 01:56:23.000000 resend-0.2.0/resend.egg-info/
--rw-r--r--   0 derich     (501) staff       (20)     2392 2023-04-26 01:56:23.000000 resend-0.2.0/resend.egg-info/PKG-INFO
--rw-r--r--   0 derich     (501) staff       (20)      278 2023-04-26 01:56:23.000000 resend-0.2.0/resend.egg-info/SOURCES.txt
--rw-r--r--   0 derich     (501) staff       (20)        1 2023-04-26 01:56:23.000000 resend-0.2.0/resend.egg-info/dependency_links.txt
--rw-r--r--   0 derich     (501) staff       (20)        1 2023-04-26 01:56:23.000000 resend-0.2.0/resend.egg-info/not-zip-safe
--rw-r--r--   0 derich     (501) staff       (20)       17 2023-04-26 01:56:23.000000 resend-0.2.0/resend.egg-info/requires.txt
--rw-r--r--   0 derich     (501) staff       (20)        7 2023-04-26 01:56:23.000000 resend-0.2.0/resend.egg-info/top_level.txt
--rw-r--r--   0 derich     (501) staff       (20)       67 2023-04-26 01:56:23.000000 resend-0.2.0/setup.cfg
--rw-r--r--   0 derich     (501) staff       (20)     1112 2023-04-26 01:56:07.000000 resend-0.2.0/setup.py
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2023-05-02 21:42:06.000000 resend-0.3.0/
+-rw-r--r--   0 derich     (501) staff       (20)     2653 2023-05-02 21:42:06.000000 resend-0.3.0/PKG-INFO
+-rw-r--r--   0 derich     (501) staff       (20)     1444 2023-05-02 00:53:58.000000 resend-0.3.0/README.md
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2023-05-02 21:42:06.000000 resend-0.3.0/resend/
+-rw-r--r--   0 derich     (501) staff       (20)      334 2023-05-02 21:36:30.000000 resend-0.3.0/resend/__init__.py
+-rw-r--r--   0 derich     (501) staff       (20)     1019 2023-05-02 00:53:58.000000 resend-0.3.0/resend/api.py
+-rw-r--r--   0 derich     (501) staff       (20)      796 2023-05-02 00:53:58.000000 resend-0.3.0/resend/api_keys.py
+-rw-r--r--   0 derich     (501) staff       (20)     1033 2023-05-02 21:36:30.000000 resend-0.3.0/resend/domains.py
+-rw-r--r--   0 derich     (501) staff       (20)      588 2023-05-02 00:53:58.000000 resend-0.3.0/resend/emails.py
+-rw-r--r--   0 derich     (501) staff       (20)     4152 2023-05-02 21:36:30.000000 resend-0.3.0/resend/exceptions.py
+-rw-r--r--   0 derich     (501) staff       (20)     1694 2023-05-02 21:36:30.000000 resend-0.3.0/resend/request.py
+-rw-r--r--   0 derich     (501) staff       (20)      163 2023-05-02 21:36:45.000000 resend-0.3.0/resend/version.py
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2023-05-02 21:42:06.000000 resend-0.3.0/resend.egg-info/
+-rw-r--r--   0 derich     (501) staff       (20)     2653 2023-05-02 21:42:05.000000 resend-0.3.0/resend.egg-info/PKG-INFO
+-rw-r--r--   0 derich     (501) staff       (20)      350 2023-05-02 21:42:06.000000 resend-0.3.0/resend.egg-info/SOURCES.txt
+-rw-r--r--   0 derich     (501) staff       (20)        1 2023-05-02 21:42:05.000000 resend-0.3.0/resend.egg-info/dependency_links.txt
+-rw-r--r--   0 derich     (501) staff       (20)        1 2023-05-02 21:42:05.000000 resend-0.3.0/resend.egg-info/not-zip-safe
+-rw-r--r--   0 derich     (501) staff       (20)       17 2023-05-02 21:42:05.000000 resend-0.3.0/resend.egg-info/requires.txt
+-rw-r--r--   0 derich     (501) staff       (20)        7 2023-05-02 21:42:05.000000 resend-0.3.0/resend.egg-info/top_level.txt
+-rw-r--r--   0 derich     (501) staff       (20)       67 2023-05-02 21:42:06.000000 resend-0.3.0/setup.cfg
+-rw-r--r--   0 derich     (501) staff       (20)     1112 2023-05-02 21:37:28.000000 resend-0.3.0/setup.py
```

### Comparing `resend-0.2.0/PKG-INFO` & `resend-0.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resend
-Version: 0.2.0
+Version: 0.3.0
 Summary: Resend Python SDK
 Home-page: https://github.com/resendlabs/resend-python
 Author: Derich Pacheco
 Author-email: carlosderich@gmail.com
 License: UNKNOWN
 Description: # Resend Python SDK
         
@@ -25,38 +25,48 @@
         ```
         
         ## Setup
         
         First, you need to get an API key, which is available in the [Resend Dashboard](https://resend.com).
         
         ```py
-        from resend import Resend
+        import resend
+        import os
         
-        client = Resend(api_key="kl_123")
+        resend.api_key = os.environ["RESEND_API_KEY"]
         ```
         
         ## Example
         
         ```py
         import os
-        from resend import Resend
+        import resend
+        
+        resend.api_key = os.environ["RESEND_API_KEY"]
         
-        client = Resend(api_key=os.environ["RESEND_API_KEY"])
+        params = {
+            "from": "r@email.io",
+            "to": ["to@gmail.com"],
+            "subject": "hi",
+            "html": "<strong>hello, world!</strong>",
+            "reply_to": "to@gmail.com",
+            "bcc": "to@gmail.com",
+            "cc": ["to@gmail.com"],
+            "tags": [
+                {"name": "tag1", "value": "tagvalue1"},
+                {"name": "tag2", "value": "tagvalue2"},
+            ],
+        }
+        
+        r = resend.Emails.send(
         
-        client.send_email(
-            to="to@email.com",
-            sender="from@email.com",
-            subject="hi",
-            html="<strong>hello, world!</strong>"
         )
+        print(r)
         ```
         
-        ## Example sending email using React
-        
-        Coming soon.
 Keywords: email,email platform
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `resend-0.2.0/README.md` & `resend-0.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -17,31 +17,40 @@
 ```
 
 ## Setup
 
 First, you need to get an API key, which is available in the [Resend Dashboard](https://resend.com).
 
 ```py
-from resend import Resend
+import resend
+import os
 
-client = Resend(api_key="kl_123")
+resend.api_key = os.environ["RESEND_API_KEY"]
 ```
 
 ## Example
 
 ```py
 import os
-from resend import Resend
+import resend
 
-client = Resend(api_key=os.environ["RESEND_API_KEY"])
+resend.api_key = os.environ["RESEND_API_KEY"]
 
-client.send_email(
-    to="to@email.com",
-    sender="from@email.com",
-    subject="hi",
-    html="<strong>hello, world!</strong>"
-)
-```
+params = {
+    "from": "r@email.io",
+    "to": ["to@gmail.com"],
+    "subject": "hi",
+    "html": "<strong>hello, world!</strong>",
+    "reply_to": "to@gmail.com",
+    "bcc": "to@gmail.com",
+    "cc": ["to@gmail.com"],
+    "tags": [
+        {"name": "tag1", "value": "tagvalue1"},
+        {"name": "tag2", "value": "tagvalue2"},
+    ],
+}
 
-## Example sending email using React
+r = resend.Emails.send(
 
-Coming soon.
+)
+print(r)
+```
```

### Comparing `resend-0.2.0/resend/api.py` & `resend-0.3.0/resend/request.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,88 +1,59 @@
-from typing import Dict, List
+from typing import Dict
 
 import requests
 
+import resend
 from resend.exceptions import raise_for_code_and_type
+from resend.version import get_version
 
-from .version import get_version
-
-
-class Resend:
-    """Resend SDK main client class
-
-    Raises:
-        ValueError: raises ValueError when api key is
-    """
 
+# This class wraps the HTTP request creation logic
+class Request:
     base_url: str = "https://api.resend.com"
-    timeout_ms: int = 60_000
 
-    def __init__(self, api_key: str):
-        if not api_key:
-            raise ValueError("Resend API Key is required.")
-        self.__api_key = api_key
+    def __init__(self, path: str, params: Dict, verb: str):
+        self.path = path
+        self.params = params
+        self.verb = verb
+
+    def perform(self):
+        resp = self.make_request(url=f"{self.base_url}{self.path}")
+
+        # delete calls do not return a body
+        if resp.text == "" and resp.status_code == 200:
+            return None
+
+        # handle error in case there is a statusCode attr present
+        # and status != 200
+        if resp.status_code != 200 and resp.json().get("statusCode"):
+            error = resp.json()
+            raise_for_code_and_type(
+                code=error.get("statusCode"),
+                message=error.get("message"),
+                error_type=error.get("name"),
+            )
+
+        return resp.json()
 
     def __get_headers(self) -> Dict:
         """get_headers returns the HTTP headers that will be
         used for every req.
 
         Returns:
-            Dict: _description_
+            Dict: configured HTTP Headers
         """
         return {
             "Accept": "application/json",
-            "Authorization": f"Bearer {self.__api_key}",
+            "Authorization": f"Bearer {resend.api_key}",
             "User-Agent": f"python:{get_version()}",
         }
 
-    def _make_request(self, url, params, headers):
+    def make_request(self, url: str):
+        headers = self.__get_headers()
+        params = self.params
+        verb = self.verb
+
         try:
-            return requests.post(url, json=params, headers=headers)
+            return requests.request(verb, url, json=params, headers=headers)
         except requests.HTTPError as e:
             raise e
-
-    def send_email(
-        self,
-        sender: str,
-        to: str,
-        subject: str,
-        text: str = None,
-        bcc: str = None,
-        cc: str = None,
-        html: str = None,
-        attachments: List[Dict] = None,
-    ):
-        if not sender:
-            raise ValueError("sender is required.")
-        if not to:
-            raise ValueError("to is required.")
-        if not subject:
-            raise ValueError("subject is required.")
-
-        url = f"{self.base_url}/email"
-        headers = self.__get_headers()
-
-        params: Dict = {"to": to, "from": sender, "subject": subject}
-        if text:
-            params["text"] = text
-        elif html:
-            params["html"] = html
-
-        if cc:
-            params["cc"] = cc
-        if bcc:
-            params["bcc"] = bcc
-        if attachments:
-            params["attachments"] = attachments
-
-        resp = self._make_request(url, params, headers)
-
-        if resp.status_code != 200 or resp.json().get("error") is not None:
-            error = resp.json().get("error")
-            raise_for_code_and_type(
-                code=error.get("code"),
-                message=error.get("message"),
-                error_type=error.get("type"),
-            )
-
-        return resp.json()
```

### Comparing `resend-0.2.0/resend/exceptions.py` & `resend-0.3.0/resend/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -74,14 +74,41 @@
             message=message,
             suggested_action=suggested_action,
             code=code,
             error_type=error_type,
         )
 
 
+class ValidationError(ResendError):
+    """see https://resend.com/docs/errors"""
+
+    def __init__(
+        self,
+        message,
+        error_type,
+        code,
+    ):
+        default_message = """
+        The request body is missing one or more required fields."""
+
+        suggested_action = """Check the error message
+        to see the list of missing fields."""
+
+        if message == "":
+            message = default_message
+
+        ResendError.__init__(
+            self,
+            code=code or 400,
+            message=message,
+            suggested_action=suggested_action,
+            error_type=error_type,
+        )
+
+
 class MissingRequiredFieldsError(ResendError):
     """see https://resend.com/docs/errors"""
 
     def __init__(
         self,
         message,
         error_type,
@@ -102,21 +129,24 @@
             message=message,
             suggested_action=suggested_action,
             error_type=error_type,
         )
 
 
 ERRORS: Dict[str, Dict[str, ResendError]] = {
+    "400": {"validation_error": ValidationError},
     "422": {"missing_required_fields": MissingRequiredFieldsError},
     "401": {"missing_api_key": MissingApiKeyError},
     "403": {"invalid_api_key": InvalidApiKeyError},
 }
 
 
 def raise_for_code_and_type(code, error_type, message: str) -> ResendError:
+    error = ERRORS.get(str(code))
+
     # Handle the case where the error might be unknown
-    if ERRORS.get(code).get(error_type) is None:
-        raise ResendError()
+    if error is None or error.get(error_type) is None:
+        raise ResendError(code=code, message=message, error_type=error_type)
 
     # Raise error from errors list
-    error: ResendError = ERRORS.get(code).get(error_type)
+    error: ResendError = error.get(error_type)
     raise error(code=code, message=message, error_type=error_type)
```

### Comparing `resend-0.2.0/resend.egg-info/PKG-INFO` & `resend-0.3.0/resend.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resend
-Version: 0.2.0
+Version: 0.3.0
 Summary: Resend Python SDK
 Home-page: https://github.com/resendlabs/resend-python
 Author: Derich Pacheco
 Author-email: carlosderich@gmail.com
 License: UNKNOWN
 Description: # Resend Python SDK
         
@@ -25,38 +25,48 @@
         ```
         
         ## Setup
         
         First, you need to get an API key, which is available in the [Resend Dashboard](https://resend.com).
         
         ```py
-        from resend import Resend
+        import resend
+        import os
         
-        client = Resend(api_key="kl_123")
+        resend.api_key = os.environ["RESEND_API_KEY"]
         ```
         
         ## Example
         
         ```py
         import os
-        from resend import Resend
+        import resend
+        
+        resend.api_key = os.environ["RESEND_API_KEY"]
         
-        client = Resend(api_key=os.environ["RESEND_API_KEY"])
+        params = {
+            "from": "r@email.io",
+            "to": ["to@gmail.com"],
+            "subject": "hi",
+            "html": "<strong>hello, world!</strong>",
+            "reply_to": "to@gmail.com",
+            "bcc": "to@gmail.com",
+            "cc": ["to@gmail.com"],
+            "tags": [
+                {"name": "tag1", "value": "tagvalue1"},
+                {"name": "tag2", "value": "tagvalue2"},
+            ],
+        }
+        
+        r = resend.Emails.send(
         
-        client.send_email(
-            to="to@email.com",
-            sender="from@email.com",
-            subject="hi",
-            html="<strong>hello, world!</strong>"
         )
+        print(r)
         ```
         
-        ## Example sending email using React
-        
-        Coming soon.
 Keywords: email,email platform
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `resend-0.2.0/setup.py` & `resend-0.3.0/setup.py`

 * *Files identical despite different names*

