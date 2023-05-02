# Comparing `tmp/spacs-0.0.4.tar.gz` & `tmp/spacs-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacs-0.0.4.tar", max compression
+gzip compressed data, was "spacs-0.0.5.tar", max compression
```

## Comparing `spacs-0.0.4.tar` & `spacs-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1093 2023-04-26 20:46:06.053000 spacs-0.0.4/LICENSE
--rw-r--r--   0        0        0      418 2023-04-27 14:19:10.951829 spacs-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1503 2023-04-26 20:00:05.390203 spacs-0.0.4/README.md
--rw-r--r--   0        0        0      149 2023-04-27 14:17:02.802475 spacs-0.0.4/spacs/__init__.py
--rw-r--r--   0        0        0     8876 2023-04-27 14:18:56.817227 spacs-0.0.4/spacs/client.py
--rw-r--r--   0        0        0     2164 1970-01-01 00:00:00.000000 spacs-0.0.4/setup.py
--rw-r--r--   0        0        0     1928 1970-01-01 00:00:00.000000 spacs-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-04-26 20:46:06.053000 spacs-0.0.5/LICENSE
+-rw-r--r--   0        0        0      418 2023-05-01 18:16:18.894444 spacs-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1763 2023-05-01 18:22:46.781118 spacs-0.0.5/README.md
+-rw-r--r--   0        0        0      184 2023-05-01 15:11:43.780995 spacs-0.0.5/spacs/__init__.py
+-rw-r--r--   0        0        0     7951 2023-05-01 18:26:26.527288 spacs-0.0.5/spacs/client.py
+-rw-r--r--   0        0        0     2424 1970-01-01 00:00:00.000000 spacs-0.0.5/setup.py
+-rw-r--r--   0        0        0     2172 1970-01-01 00:00:00.000000 spacs-0.0.5/PKG-INFO
```

### Comparing `spacs-0.0.4/LICENSE` & `spacs-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spacs-0.0.4/spacs/client.py` & `spacs-0.0.5/spacs/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,28 +4,38 @@
 from enum import StrEnum
 from typing import Any, ClassVar, Self, Awaitable, Type
 
 import aiohttp
 from aiohttp import ClientConnectorError, ClientResponse
 from pydantic import BaseModel
 
-RequestContent = BaseModel | dict[str, Any] | None
+ResponseModel = Type[BaseModel] | None
+RequestContent = dict[str, Any] | BaseModel | None
 JsonResponseContent = dict[str, Any] | list[dict[str, Any]]
 ModelResponse = BaseModel | list[BaseModel]
-SpacsClientResponse = str | JsonResponseContent | ModelResponse
+SpacsResponse = str | JsonResponseContent | ModelResponse
 
 _logger = logging.getLogger(__name__)
 
 
 class ContentType(StrEnum):
     JSON = "application/json"
     FORM = "application/x-www-form-urlencoded"
     HTML = "text/html"
 
 
+class SpacsRequest(BaseModel):
+    path: str
+    params: RequestContent = None
+    body: RequestContent = None
+    headers: dict[str, str] = None
+    content_type: ContentType = ContentType.JSON
+    response_model: ResponseModel = None
+
+
 class SpacsClient:
     base_url: str | None
     path_prefix: str
 
     _sessions: ClassVar[list[Self]] = []
     _logger: logging.Logger
     _session: aiohttp.ClientSession | None = None
@@ -67,117 +77,61 @@
 
     async def close(self) -> None:
         if not self.is_open:
             return _logger.warning("No session to close")
         await self._session.close()
         self._session = None
 
-    async def get(
-        self,
-        path: str,
-        *,
-        params: RequestContent = None,
-        body: RequestContent = None,
-        headers: dict[str, str] | None = None,
-        content_type: ContentType = ContentType.JSON,
-        response_model: Type[BaseModel] | None = None,
-    ) -> SpacsClientResponse:
-        return await self._request(
-            self.session.get, path, params, body, headers, content_type, response_model
-        )
+    async def get(self, request: SpacsRequest) -> SpacsResponse:
+        return await self._request(self.session.get, request)
 
-    async def post(
-        self,
-        path: str,
-        *,
-        params: RequestContent = None,
-        body: RequestContent = None,
-        headers: dict[str, str] | None = None,
-        content_type: ContentType = ContentType.JSON,
-        response_model: Type[BaseModel] | None = None,
-    ) -> SpacsClientResponse:
-        return await self._request(
-            self.session.post, path, params, body, headers, content_type, response_model
-        )
+    async def post(self, request: SpacsRequest) -> SpacsResponse:
+        return await self._request(self.session.post, request)
 
-    async def put(
-        self,
-        path: str,
-        *,
-        params: RequestContent = None,
-        body: RequestContent = None,
-        headers: dict[str, str] | None = None,
-        content_type: ContentType = ContentType.JSON,
-        response_model: Type[BaseModel] | None = None,
-    ) -> SpacsClientResponse:
-        return await self._request(
-            self.session.put, path, params, body, headers, content_type, response_model
-        )
+    async def put(self, request: SpacsRequest) -> SpacsResponse:
+        return await self._request(self.session.put, request)
 
-    async def delete(
-        self,
-        path: str,
-        *,
-        params: RequestContent = None,
-        body: RequestContent = None,
-        headers: dict[str, str] | None = None,
-        content_type: ContentType = ContentType.JSON,
-        response_model: Type[BaseModel] | None = None,
-    ) -> SpacsClientResponse:
-        return await self._request(
-            self.session.delete,
-            path,
-            params,
-            body,
-            headers,
-            content_type,
-            response_model,
-        )
+    async def delete(self, request: SpacsRequest) -> SpacsResponse:
+        return await self._request(self.session.delete, request)
 
     async def _request(
         self,
         action: Callable[..., Awaitable[ClientResponse]],
-        path: str,
-        params: RequestContent = None,
-        body: RequestContent = None,
-        headers: dict[str, str] | None = None,
-        content_type: ContentType = ContentType.JSON,
-        response_model: Type[BaseModel] | None = None,
-    ) -> SpacsClientResponse:
+        request: SpacsRequest,
+    ) -> SpacsResponse:
         """Generic function for issuing requests"""
-        if headers is None:
-            headers = {}
-        headers["Content-Type"] = content_type.value
-
-        params_transformed = self._transform_content(params)
-        body_transformed = self._transform_content(body)
-        path = self._build_path(path)
+        request = self._prepare_request(request)
 
         start_time = datetime.datetime.now(tz=datetime.timezone.utc)
         base_log_info = {
             "method": action.__name__,
             "base_url": self.base_url,
-            "path": path,
+            "path": request.path,
         }
 
         try:
             async with action(
-                path, params=params_transformed, json=body_transformed, headers=headers
+                request.path,
+                params=request.params,
+                json=request.body,
+                headers=request.headers,
             ) as response:
                 end_time = datetime.datetime.now(tz=datetime.timezone.utc)
                 self._logger.debug(
                     {
                         "msg": "Request completed",
                         **base_log_info,
                         "status": response.status,
                         "duration": str(end_time - start_time),
                     }
                 )
                 if response.ok:
-                    return await self._handle_ok_response(response, response_model)
+                    return await self._handle_ok_response(
+                        response, request.response_model
+                    )
                 else:
                     raise SpacsRequestError(
                         status_code=response.status,
                         reason=response.reason,
                     )
         except ClientConnectorError as error:
             self._logger.error("Failed to connect to server.")
@@ -190,57 +144,72 @@
                     "msg": "Request error",
                     **base_log_info,
                     "error": str(error),
                 }
             )
             raise error
 
+    def _prepare_request(self, request: SpacsRequest) -> SpacsRequest:
+        # Copy content to not modify inputs to `SpacsClient` actions
+        result = request.copy(deep=True)
+
+        if result.headers is None:
+            result.headers = {}
+
+        result.headers["Content-Type"] = result.content_type.value
+        result.path = self._build_path(result.path)
+        result.params = self._prepare_content(result.params)
+        result.body = self._prepare_content(result.body)
+        return result
+
     def _build_path(self, path: str) -> str:
         result = f"/{path.strip('/')}"
         if self.path_prefix:
             result = f"/{self.path_prefix}{result}"
         return result
 
     @classmethod
     async def close_all(cls) -> None:
         for session in cls._sessions:
             if not session.is_open:
                 continue
             await session.close()
 
     @classmethod
-    def _transform_content(cls, content: RequestContent) -> dict[str, str] | None:
+    async def _handle_ok_response(
+        cls, response: ClientResponse, model: Type[BaseModel] | None
+    ) -> str | JsonResponseContent | ModelResponse:
+        content = await cls._parse_response(response)
+        if model is not None and not isinstance(response, str):
+            content = cls._response_content_to_model(content, model)
+        return content
+
+    @staticmethod
+    def _prepare_content(content: RequestContent) -> RequestContent:
         """Ensures input objects are in acceptable formats for requests"""
 
         if content is None:
             return
 
         if isinstance(content, BaseModel):
             content = content.dict()
+
+        # At this point, `content` is a regular dictionary
         for key in content:
             value = content[key]
             if isinstance(value, datetime.datetime):
                 # Convert `datetime` items to ISO 8601 strings
                 content[key] = value.isoformat()
             elif isinstance(value, datetime.timedelta):
                 # `timedelta` items represented as seconds (float)
                 content[key] = value.total_seconds()
             elif isinstance(value, bool):
                 content[key] = str(value)
         return content
 
-    @classmethod
-    async def _handle_ok_response(
-        cls, response: ClientResponse, model: Type[BaseModel] | None
-    ) -> str | JsonResponseContent | ModelResponse:
-        content = await cls._parse_response(response)
-        if model is not None and not isinstance(response, str):
-            content = cls._response_content_to_model(content, model)
-        return content
-
     @staticmethod
     async def _parse_response(response: ClientResponse) -> str | JsonResponseContent:
         match response.content_type:
             case ContentType.HTML:
                 return await response.text()
             case _:
                 return await response.json()
```

### Comparing `spacs-0.0.4/setup.py` & `spacs-0.0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.8.4,<4.0.0', 'pydantic>=1.10.7,<2.0.0']
 
 setup_kwargs = {
     'name': 'spacs',
-    'version': '0.0.4',
+    'version': '0.0.5',
     'description': 'Simple Pydantic AIOHTTP Client Sessions',
-    'long_description': '# SPACS: Simple Pydantic AIOHTTP Client Sessions\n\nA package to assist in managing and using long-lived AIOHTTP client sessions with simplicity. Built to handle Pydantic objects.\n\n## Features\n\n* Handles request params and bodies as either Pydantic objects or native Python dictionaries, converting items to JSON-safe format.\n* Abstracts away internals of managing the request/response objects, instead either returning parsed response content on success, or raising a specialized error object.\n* Automatically manages persistent connections to be shared over extended lifespan across application, cleaning up all open connections on teardown.\n* Utilizes modern Python type hinting.\n\n## Usage\n\n```python\nimport spacs\nfrom pydantic import BaseModel\n\n...\n\nexample_client = spacs.SpacsClient(base_url="http://example.com")\n\n# Basic request with error handling\ntry:\n    apple_response = await example_client.get("fruit/apple", params={"cultivar": "honeycrisp"})\nexcept spacs.SpacsRequestError as error:\n    print({"code": error.status_code, "reason": error.reason})\n\n# Sending Pydantic objects via HTTP POST\nclass MyModel(BaseModel):\n    name: str\n    age: int\n\nexample_object = MyModel(name="James", age=25)\nperson_response = await example_client.post("person", body=example_object)\n\n# Manually closing a session\nawait example_client.close()\n# Alternatively, to close all open sessions:\nawait spacs.SpacsClient.close_all()\n```\n\n## Building\n\n```\npoetry build\n```\n',
+    'long_description': '# SPACS: Simple Pydantic AIOHTTP Client Sessions\n\nA package to assist in managing and using long-lived AIOHTTP client sessions with simplicity. Built to handle Pydantic objects.\n\n## Features\n\n- Handles request params and bodies as either Pydantic objects or native Python dictionaries, converting items to JSON-safe format.\n- Abstracts away internals of managing the request/response objects, instead either returning parsed response content on success, or raising a specialized error object.\n- Automatically manages persistent connections to be shared over extended lifespan across application, cleaning up all open connections on teardown.\n- Utilizes modern Python type hinting.\n\n## Installation\n\nUsing poetry (preferred):\n\n```bash\npoetry add spacs\n```\n\nUsing pip:\n\n```bash\npip install spacs\n```\n\n## Usage\n\n```python\nfrom spacs import SpacsClient, SpacsRequest, SpacsRequestError\nfrom pydantic import BaseModel\n\n...\n\nexample_client = SpacsClient(base_url="http://example.com")\n\n# Basic request with error handling\ntry:\n    request = SpacsRequest(path="/fruit/apple", params={"cultivar": "honeycrisp"})\n    apples = await example_client.get(request)\nexcept SpacsRequestError as error:\n    print({"code": error.status_code, "reason": error.reason})\n\n# Sending Pydantic objects via HTTP POST\nclass MyModel(BaseModel):\n    name: str\n    age: int\n\nexample_object = MyModel(name="James", age=25)\nrequest = SpacsRequest(path="/person", body=example_object, response_model=MyModel)\ncreated_person = await example_client.post(request)\n\n# Manually closing a session\nawait example_client.close()\n# Alternatively, to close all open sessions:\nawait SpacsClient.close_all()\n```\n\n## Building\n\n```\npoetry build\n```\n',
     'author': 'rlebel12',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/rlebel12/spacs',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `spacs-0.0.4/PKG-INFO` & `spacs-0.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacs
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple Pydantic AIOHTTP Client Sessions
 Home-page: https://github.com/rlebel12/spacs
 Author: rlebel12
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
@@ -14,47 +14,63 @@
 
 # SPACS: Simple Pydantic AIOHTTP Client Sessions
 
 A package to assist in managing and using long-lived AIOHTTP client sessions with simplicity. Built to handle Pydantic objects.
 
 ## Features
 
-* Handles request params and bodies as either Pydantic objects or native Python dictionaries, converting items to JSON-safe format.
-* Abstracts away internals of managing the request/response objects, instead either returning parsed response content on success, or raising a specialized error object.
-* Automatically manages persistent connections to be shared over extended lifespan across application, cleaning up all open connections on teardown.
-* Utilizes modern Python type hinting.
+- Handles request params and bodies as either Pydantic objects or native Python dictionaries, converting items to JSON-safe format.
+- Abstracts away internals of managing the request/response objects, instead either returning parsed response content on success, or raising a specialized error object.
+- Automatically manages persistent connections to be shared over extended lifespan across application, cleaning up all open connections on teardown.
+- Utilizes modern Python type hinting.
+
+## Installation
+
+Using poetry (preferred):
+
+```bash
+poetry add spacs
+```
+
+Using pip:
+
+```bash
+pip install spacs
+```
 
 ## Usage
 
 ```python
-import spacs
+from spacs import SpacsClient, SpacsRequest, SpacsRequestError
 from pydantic import BaseModel
 
 ...
 
-example_client = spacs.SpacsClient(base_url="http://example.com")
+example_client = SpacsClient(base_url="http://example.com")
 
 # Basic request with error handling
 try:
-    apple_response = await example_client.get("fruit/apple", params={"cultivar": "honeycrisp"})
-except spacs.SpacsRequestError as error:
+    request = SpacsRequest(path="/fruit/apple", params={"cultivar": "honeycrisp"})
+    apples = await example_client.get(request)
+except SpacsRequestError as error:
     print({"code": error.status_code, "reason": error.reason})
 
 # Sending Pydantic objects via HTTP POST
 class MyModel(BaseModel):
     name: str
     age: int
 
 example_object = MyModel(name="James", age=25)
-person_response = await example_client.post("person", body=example_object)
+request = SpacsRequest(path="/person", body=example_object, response_model=MyModel)
+created_person = await example_client.post(request)
 
 # Manually closing a session
 await example_client.close()
 # Alternatively, to close all open sessions:
-await spacs.SpacsClient.close_all()
+await SpacsClient.close_all()
 ```
 
 ## Building
 
 ```
 poetry build
 ```
```

