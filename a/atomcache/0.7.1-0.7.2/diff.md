# Comparing `tmp/atomcache-0.7.1.tar.gz` & `tmp/atomcache-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atomcache-0.7.1.tar", max compression
+gzip compressed data, was "atomcache-0.7.2.tar", max compression
```

## Comparing `atomcache-0.7.1.tar` & `atomcache-0.7.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2021-10-31 14:30:27.194665 atomcache-0.7.1/LICENSE
--rw-r--r--   0        0        0     4164 2022-12-02 13:52:44.271882 atomcache-0.7.1/README.md
--rw-r--r--   0        0        0      160 2022-12-02 14:10:51.606908 atomcache-0.7.1/atomcache/__init__.py
--rw-r--r--   0        0        0     1421 2022-11-21 07:51:46.391406 atomcache-0.7.1/atomcache/backend.py
--rw-r--r--   0        0        0    10102 2022-12-02 13:46:21.563348 atomcache-0.7.1/atomcache/base.py
--rw-r--r--   0        0        0        0 2022-03-11 07:33:27.689230 atomcache-0.7.1/atomcache/py.typed
--rw-r--r--   0        0        0     4962 2022-12-02 13:47:43.971863 atomcache-0.7.1/atomcache/redis.py
--rw-r--r--   0        0        0      932 2022-12-02 14:09:56.663041 atomcache-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     5039 2022-12-02 14:13:34.387745 atomcache-0.7.1/setup.py
--rw-r--r--   0        0        0     4935 2022-12-02 14:13:34.388090 atomcache-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2021-10-31 14:30:27.194665 atomcache-0.7.2/LICENSE
+-rw-r--r--   0        0        0     4164 2022-12-02 13:52:44.271882 atomcache-0.7.2/README.md
+-rw-r--r--   0        0        0      160 2023-05-02 08:09:07.408140 atomcache-0.7.2/atomcache/__init__.py
+-rw-r--r--   0        0        0     1421 2023-05-02 08:34:44.766221 atomcache-0.7.2/atomcache/backend.py
+-rw-r--r--   0        0        0     9930 2023-05-02 08:34:44.775221 atomcache-0.7.2/atomcache/base.py
+-rw-r--r--   0        0        0        0 2022-03-11 07:33:27.689230 atomcache-0.7.2/atomcache/py.typed
+-rw-r--r--   0        0        0     4962 2023-05-02 08:34:44.768221 atomcache-0.7.2/atomcache/redis.py
+-rw-r--r--   0        0        0      951 2023-05-02 08:36:16.764119 atomcache-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     5034 1970-01-01 00:00:00.000000 atomcache-0.7.2/setup.py
+-rw-r--r--   0        0        0     4927 1970-01-01 00:00:00.000000 atomcache-0.7.2/PKG-INFO
```

### Comparing `atomcache-0.7.1/LICENSE` & `atomcache-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `atomcache-0.7.1/README.md` & `atomcache-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `atomcache-0.7.1/atomcache/backend.py` & `atomcache-0.7.2/atomcache/backend.py`

 * *Files identical despite different names*

### Comparing `atomcache-0.7.1/atomcache/base.py` & `atomcache-0.7.2/atomcache/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import asyncio
 import inspect
 import json
 from functools import partial
 from hashlib import sha256
 from typing import Any, Awaitable, Callable, Coroutine, Dict, Optional, TypeVar, Union
 
-from redis.asyncio import Redis
 from fastapi import FastAPI, Request, Response, params
 from fastapi.encoders import jsonable_encoder
 from fastapi.routing import APIRoute
 from starlette.datastructures import CommaSeparatedStrings
 
+from redis.asyncio import Redis
+
 from .backend import DEFAULT_LOCK_TIMEOUT, EX, BaseCacheBackend
 from .redis import RedisCacheBackend
 
 MIN_AUTOREFRESH_RATE = 60
 _ResponseT = TypeVar("_ResponseT")
 
 
@@ -65,23 +66,19 @@
         self.auto_refresh = auto_refresh
         self._expire = exp
         self.namespace = namespace
         self._lock_timeout = lock_timeout
         self._allow_cache_control = cache_control
         self._autorefresh_callback: Union[Callable, Awaitable, None] = None
         self._autorefresh_task: Optional[asyncio.Future] = None
-        self._request: Optional[Request] = None
-        self._cache_control: bool = False
+        self._no_cache: bool = False
 
     async def __call__(self, request: Request):
-        self._request = request
         if self._allow_cache_control:
-            self._cache_control = "no-cache" in CommaSeparatedStrings(request.headers.get("Cache-Control", ""))
-        if self.auto_refresh:
-            await self.raise_try()
+            self._no_cache = "no-cache" in CommaSeparatedStrings(request.headers.get("Cache-Control", ""))
         return self
 
     def set_namespace(self, namespace: str):  # noqa: WPS615 FIXME: unpythonic setter
         self.namespace = namespace
 
     def set_autorefresh_callback(self, endpoint: Union[Callable, Coroutine]):  # noqa: WPS231 WPS615
         kwargs = {}
@@ -103,15 +100,15 @@
         return f"{self.namespace}{cache_id}"
 
     def set(self, response: _ResponseT, cache_id: str = "") -> _ResponseT:  # noqa: WPS125
         if isinstance(response, Response):
             cache = response.body
         else:
             cache = json.dumps(jsonable_encoder(response))
-        if not self._cache_control:
+        if not self._no_cache:
             asyncio.ensure_future(self.backend.set(key=self.get_key(cache_id), value=cache, expire=self._expire))
         return response
 
     def mset(self, cache: dict[str, Any]) -> dict[str, Any]:
         encoded_cache = {self.get_key(k): json.dumps(jsonable_encoder(v)) for k, v in cache.items()}
         asyncio.ensure_future(self.backend.mset(encoded_cache, self._expire))
         return cache
@@ -119,15 +116,15 @@
     async def get(
         self,
         cache_id: str = "",
         with_lock=True,
         decode=True,
         lockspace: Optional[str] = None,
     ) -> Any:
-        if self._cache_control:
+        if self._no_cache:
             return None
         cached, _ = await self.backend.get(
             key=self.get_key(cache_id), timeout=self._lock_timeout, with_lock=with_lock, lockspace=lockspace
         )
         return json.loads(cached) if cached is not None and decode else cached
 
     async def mget(self, *cache_ids: str, decode=True) -> dict[str, Any]:
@@ -145,15 +142,15 @@
             cache_id (str, optional): Cache identifier. Defaults to "".
             with_lock (bool, optional): Lock the cache if there is no response. Defaults to True.
             lockspace (str, optional): Key to use for lock
 
         Raises:
             CachedResponse: generate response from cache.
         """
-        if self._cache_control:
+        if self._no_cache:
             return
         cached_content, ttl = await self.backend.get(
             self.get_key(cache_id),
             timeout=self._lock_timeout,
             with_lock=with_lock,
             lockspace=lockspace,
         )
```

### Comparing `atomcache-0.7.1/atomcache/redis.py` & `atomcache-0.7.2/atomcache/redis.py`

 * *Files identical despite different names*

### Comparing `atomcache-0.7.1/pyproject.toml` & `atomcache-0.7.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 [tool.poetry]
 name = "atomcache"
-version = "0.7.1"
+version = "0.7.2"
 description = "Asynchronous cache manager designed for horizontally scaled web applications."
 authors = ["Serghei Ungurean <srg@intelbit.io>", "Nichita Morcotilo <nmorkotilo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pysergio/atomcache"
 repository = "https://github.com/pysergio/atomcache"
 
 [tool.poetry.dependencies]
-python = "^3.7"
-fastapi = ">=0.61.2 <=0.88.0"
-redis = "^4.3.5"
+python = "^3.8"
+fastapi = ">=0.61.2"
+redis = "^4.5.4"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
+autoflake = "1.7.8"
 pytest = "^6.2.5"
 pytest-asyncio = "^0.16.0"
 pytest-cov = "^3.0.0"
-isort = "^5.10.0"
-autoflake = "^1.4"
-black = "^22.8"
+isort = "^5.12"
+black = "^23.3"
 wemake-python-styleguide = "^0.17"
-mypy = "^0.981"
+mypy = "^1.2.0"
 flake8-fixme = "^1.1"
 coverage = "^6.5.0"
+types-redis = "^4.5.4"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
```

### Comparing `atomcache-0.7.1/setup.py` & `atomcache-0.7.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 packages = \
 ['atomcache']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['fastapi>=0.61.2,<=0.88.0', 'redis>=4.3.5,<5.0.0']
+['fastapi>=0.61.2', 'redis>=4.5.4,<5.0.0']
 
 setup_kwargs = {
     'name': 'atomcache',
-    'version': '0.7.1',
+    'version': '0.7.2',
     'description': 'Asynchronous cache manager designed for horizontally scaled web applications.',
     'long_description': '<p align="center">\n<a href="https://codecov.io/gh/pysergio/atomcache"> \n <img src="https://codecov.io/gh/pysergio/atomcache/branch/master/graph/badge.svg?token=OVZABBE1UJ"/> \n</a>\n<a href="https://pypi.org/project/atomcache" target="_blank">\n    <img src="https://img.shields.io/pypi/v/atomcache?color=%2334D058&label=pypi%20package" alt="Package version">\n</a>\n<a href="https://pypi.org/project/atomcache" target="_blank">\n    <img src="https://img.shields.io/pypi/pyversions/atomcache.svg?color=%2334D058" alt="Supported Python versions">\n</a>\n</p>\n\n## Introduction\nAsynchronous cache manager designed for horizontally scaled web applications.\n**NOTE:** _Currently has implementation only for FastAPI using Redis._\n\n## Requirements\n\nPython 3.7+\n\n* <a href="https://redis.readthedocs.io/en/latest/_modules/redis/asyncio/client.html?" class="external-link" target="_blank">redis</a> for cache implementation.\n* <a href="https://fastapi.tiangolo.com" class="external-link" target="_blank">FastAPI</a> for the web parts.\n  \n## Installation\n\n<div class="termy">\n\n```console\n$ pip install atomcache\n\n---> 100%\n```\n\n## Explanation schema\n\n![Class Diagram](http://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/pysergio/atomcache/master/README.md)\n\n<details markdown="1">\n<summary>As UML</summary>\n\n```plantuml\n@startuml\n    !theme materia\n    participant Redis\n    participant Instance_A as A\n    participant Instance_B as B\n    participant Instance_N as C\n\n\n    B <-> Redis: GET: Cache=null & GET: Lock=null\n\n    B <-> Redis: SET: Lock = true\n\n    activate B #Red\n    A <--> Redis: GET: Cache=null & GET: Lock=true\n    activate A #Transparent\n    C <--> Redis: GET: Cache=null & GET: Lock=true\n    activate C #Transparent\n    B <--> B: Do the computation\n    B -> Redis: SET: Cache={...}\n    deactivate B\n\n    group Notify Cache SET\n        Redis -> C\n        Redis -> A\n    end\n    group GET Cache\n        Redis <-> C\n    deactivate C\n        Redis <-> A\n    deactivate A\n    end\n@enduml\n```\n</details>\n\n## Examples:\n\n### Usage as FastAPI Dependency\n\n* Create a file `events.py` with:\n\n```Python\nfrom typing import Optional, Callable\n\nfrom redis.asyncio import Redis\nfrom fastapi import FastAPI, Depends\nfrom atomcache import Cache\n\n\ndef create_start_app_handler(app: FastAPI) -> Callable:\n    async def start_app() -> None:\n        redis: Redis = await Redis.from_url(url="redis://localhost", encoding="utf-8")\n        await Cache.init(app, redis)\n\n    return start_app\n\n\ndef create_stop_app_handler(app: FastAPI) -> Callable:\n    async def stop_app() -> None:\n        await Cache.backend.close()\n\n    return stop_app\n```\n\n* Create a file `main.py` with:\n\n```Python\nfrom typing import Optional\n\nfrom fastapi import FastAPI, Depends\nfrom atomcache import Cache\n\nfrom .events import create_start_app_handler, create_stop_app_handler\n\napp = FastAPI()\n\napp.add_event_handler("startup", create_start_app_handler(app))\napp.add_event_handler("shutdown", create_stop_app_handler(app))\n\n\n@router.get("/resources", response_model=List[TheResponseModel], name="main:test-example")\nasync def resources(offset: int = 0, items: int = 10, cache: Cache = Depends(Cache(exp=600)):\n    cache_id = f"{offset}-{items}"  # Build cache identifier\n    await cache.raise_try(cache_id)  # Try to respond from cache\n    response = await db.find(TheResponseModel, skip=offset, limit=items)\n    await asyncio.sleep(10)  # Do some heavy work for 10 sec, see `lock_timeout`\n    return cache.set(response, cache_id=cache_id)\n```\n\n### Direct cache usage for avoiding repetitive calling on external resources:\n\n```Python\nfrom aiohttp import ClientSession\nfrom atomcache import Cache\n\ncache = Cache(exp=1200, namespace="my-namespace:")\n\n\nasync def requesting_helper(ref: str) -> List[dict]:\n    cached_value = await cache.get(cache_id=ref)\n    if cached_value is not None:\n        return cached_value\n\n    async with ClientSession() as session:\n        async with session.get(f"https://external-api.io/{ref}") as response:\n            if response.ok:\n                cached_value = response.json()\n                return cache.set(cached_value, cache_id=ref)\n    return []\n```\n',
     'author': 'Serghei Ungurean',
     'author_email': 'srg@intelbit.io',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/pysergio/atomcache',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['atomcache']
-package_data = \ {'': ['*']} install_requires = \ ['fastapi>=0.61.2,<=0.88.0',
-'redis>=4.3.5,<5.0.0'] setup_kwargs = { 'name': 'atomcache', 'version':
-'0.7.1', 'description': 'Asynchronous cache manager designed for horizontally
+package_data = \ {'': ['*']} install_requires = \ ['fastapi>=0.61.2',
+'redis>=4.5.4,<5.0.0'] setup_kwargs = { 'name': 'atomcache', 'version':
+'0.7.2', 'description': 'Asynchronous cache manager designed for horizontally
 scaled web applications.', 'long_description': '
       \n\n_[https://codecov.io/gh/pysergio/atomcache/branch/master/graph/
  badge.svg?token=OVZABBE1UJ]_\n\n\n_[Package_version]\n\n\n_[Supported_Python
                                  versions]\n\n
 \n\n## Introduction\nAsynchronous cache manager designed for horizontally
 scaled web applications.\n**NOTE:** _Currently has implementation only for
 FastAPI using Redis._\n\n## Requirements\n\nPython 3.7+\n\n* redis for cache
@@ -46,11 +46,11 @@
 aiohttp import ClientSession\nfrom atomcache import Cache\n\ncache = Cache
 (exp=1200, namespace="my-namespace:")\n\n\nasync def requesting_helper(ref:
 str) -> List[dict]:\n cached_value = await cache.get(cache_id=ref)\n if
 cached_value is not None:\n return cached_value\n\n async with ClientSession()
 as session:\n async with session.get(f"https://external-api.io/{ref}") as
 response:\n if response.ok:\n cached_value = response.json()\n return cache.set
 (cached_value, cache_id=ref)\n return []\n```\n', 'author': 'Serghei Ungurean',
-'author_email': 'srg@intelbit.io', 'maintainer': None, 'maintainer_email':
-None, 'url': 'https://github.com/pysergio/atomcache', 'packages': packages,
+'author_email': 'srg@intelbit.io', 'maintainer': 'None', 'maintainer_email':
+'None', 'url': 'https://github.com/pysergio/atomcache', 'packages': packages,
 'package_data': package_data, 'install_requires': install_requires,
-'python_requires': '>=3.7,<4.0', } setup(**setup_kwargs)
+'python_requires': '>=3.8,<4.0', } setup(**setup_kwargs)
```

### Comparing `atomcache-0.7.1/PKG-INFO` & `atomcache-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: atomcache
-Version: 0.7.1
+Version: 0.7.2
 Summary: Asynchronous cache manager designed for horizontally scaled web applications.
 Home-page: https://github.com/pysergio/atomcache
 License: MIT
 Author: Serghei Ungurean
 Author-email: srg@intelbit.io
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: fastapi (>=0.61.2,<=0.88.0)
-Requires-Dist: redis (>=4.3.5,<5.0.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: fastapi (>=0.61.2)
+Requires-Dist: redis (>=4.5.4,<5.0.0)
 Project-URL: Repository, https://github.com/pysergio/atomcache
 Description-Content-Type: text/markdown
 
 <p align="center">
 <a href="https://codecov.io/gh/pysergio/atomcache"> 
  <img src="https://codecov.io/gh/pysergio/atomcache/branch/master/graph/badge.svg?token=OVZABBE1UJ"/> 
 </a>
```

#### html2text {}

```diff
@@ -1,18 +1,17 @@
-Metadata-Version: 2.1 Name: atomcache Version: 0.7.1 Summary: Asynchronous
+Metadata-Version: 2.1 Name: atomcache Version: 0.7.2 Summary: Asynchronous
 cache manager designed for horizontally scaled web applications. Home-page:
 https://github.com/pysergio/atomcache License: MIT Author: Serghei Ungurean
-Author-email: srg@intelbit.io Requires-Python: >=3.7,<4.0 Classifier: License
+Author-email: srg@intelbit.io Requires-Python: >=3.8,<4.0 Classifier: License
 :: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Requires-Dist: fastapi
-(>=0.61.2,<=0.88.0) Requires-Dist: redis (>=4.3.5,<5.0.0) Project-URL:
-Repository, https://github.com/pysergio/atomcache Description-Content-Type:
-text/markdown
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: fastapi
+(>=0.61.2) Requires-Dist: redis (>=4.5.4,<5.0.0) Project-URL: Repository,
+https://github.com/pysergio/atomcache Description-Content-Type: text/markdown
         [https://codecov.io/gh/pysergio/atomcache/branch/master/graph/
    badge.svg?token=OVZABBE1UJ] [Package_version] [Supported_Python_versions]
 ## Introduction Asynchronous cache manager designed for horizontally scaled web
 applications. **NOTE:** _Currently has implementation only for FastAPI using
 Redis._ ## Requirements Python 3.7+ * redis for cache implementation. * FastAPI
 for the web parts. ## Installation
 ```console $ pip install atomcache ---> 100% ``` ## Explanation schema ![Class
```

