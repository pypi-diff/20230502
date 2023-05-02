# Comparing `tmp/openai_forward-0.1.3.tar.gz` & `tmp/openai_forward-0.1.4.tar.gz`

## Comparing `openai_forward-0.1.3.tar` & `openai_forward-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 openai_forward-0.1.3/openai_forward/__init__.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 openai_forward-0.1.3/openai_forward/__main__.py
--rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 openai_forward-0.1.3/openai_forward/_base.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 openai_forward-0.1.3/openai_forward/app.py
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 openai_forward-0.1.3/openai_forward/config.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 openai_forward-0.1.3/openai_forward/openai.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.3/openai_forward/content/__init__.py
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 openai_forward-0.1.3/openai_forward/content/chat.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.3/openai_forward/content/image.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.3/openai_forward/routers/__init__.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 openai_forward-0.1.3/openai_forward/routers/openai_v1.py
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 openai_forward-0.1.3/openai_forward/routers/schemas.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 openai_forward-0.1.3/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.1.3/LICENSE
--rw-r--r--   0        0        0     6251 2020-02-02 00:00:00.000000 openai_forward-0.1.3/README.md
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 openai_forward-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     7521 2020-02-02 00:00:00.000000 openai_forward-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 openai_forward-0.1.4/openai_forward/__init__.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 openai_forward-0.1.4/openai_forward/__main__.py
+-rw-r--r--   0        0        0     3963 2020-02-02 00:00:00.000000 openai_forward-0.1.4/openai_forward/_base.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 openai_forward-0.1.4/openai_forward/app.py
+-rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 openai_forward-0.1.4/openai_forward/config.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 openai_forward-0.1.4/openai_forward/openai.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.4/openai_forward/content/__init__.py
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 openai_forward-0.1.4/openai_forward/content/chat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.4/openai_forward/content/image.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.4/openai_forward/routers/__init__.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 openai_forward-0.1.4/openai_forward/routers/openai_v1.py
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 openai_forward-0.1.4/openai_forward/routers/schemas.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 openai_forward-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.1.4/LICENSE
+-rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 openai_forward-0.1.4/README.md
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 openai_forward-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     7656 2020-02-02 00:00:00.000000 openai_forward-0.1.4/PKG-INFO
```

### Comparing `openai_forward-0.1.3/openai_forward/_base.py` & `openai_forward-0.1.4/openai_forward/_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,33 @@
 from fastapi import Request, HTTPException, status
 from fastapi.responses import StreamingResponse
 from loguru import logger
 import httpx
 from starlette.background import BackgroundTask
 import os
+from itertools import cycle
 from .content.chat import parse_chat_completions, ChatSaver
+from .config import env2list
 
 
 class OpenaiBase:
-    _default_api_key = os.environ.get("OPENAI_API_KEY", "").strip()
     _base_url = os.environ.get("OPENAI_BASE_URL", "https://api.openai.com").strip()
     _LOG_CHAT = os.environ.get("LOG_CHAT", "False").lower() == "true"
     _ROUTE_PREFIX = os.environ.get("ROUTE_PREFIX", "").strip()
-    IP_WHITELIST = os.environ.get("IP_WHITELIST", "").strip()
-    IP_BLACKLIST = os.environ.get("IP_BLACKLIST", "").strip()
-    if IP_BLACKLIST:
-        IP_BLACKLIST = [i.strip() for i in IP_BLACKLIST.split(' ')]
-    else:
-        IP_BLACKLIST = []
-    if IP_WHITELIST:
-        IP_WHITELIST = [i.strip() for i in IP_WHITELIST.split(' ')]
-    else:
-        IP_WHITELIST = []
+    _default_api_key_list = env2list("OPENAI_API_KEY", sep=" ")
+    _cycle_api_key = cycle(_default_api_key_list)
+    IP_WHITELIST = env2list("IP_WHITELIST", sep=" ")
+    IP_BLACKLIST = env2list("IP_BLACKLIST", sep=" ")
+
     if _ROUTE_PREFIX:
         if _ROUTE_PREFIX.endswith('/'):
             _ROUTE_PREFIX = _ROUTE_PREFIX[:-1]
         if not _ROUTE_PREFIX.startswith('/'):
             _ROUTE_PREFIX = '/' + _ROUTE_PREFIX
-    stream_timeout = 20
     timeout = 30
-    non_stream_timeout = 30
     chatsaver = ChatSaver(save_interval=10)
 
     def validate_request_host(self, ip):
         if self.IP_WHITELIST and ip not in self.IP_WHITELIST:
             raise HTTPException(status_code=status.HTTP_403_FORBIDDEN,
                                 detail=f"Forbidden, ip={ip} not in whitelist!")
         if self.IP_BLACKLIST and ip in self.IP_BLACKLIST:
@@ -62,16 +56,16 @@
         url_path = request.url.path
         url_path = url_path[len(cls._ROUTE_PREFIX):]
         url = httpx.URL(path=url_path, query=request.url.query.encode('utf-8'))
         headers = dict(request.headers)
         auth = headers.pop("authorization", None)
         if auth and str(auth).startswith("Bearer sk-"):
             tmp_headers = {'Authorization': auth}
-        elif cls._default_api_key:
-            auth = "Bearer " + cls._default_api_key
+        elif cls._default_api_key_list:
+            auth = "Bearer " + next(cls._cycle_api_key)
             tmp_headers = {'Authorization': auth}
         else:
             tmp_headers = {}
 
         headers.pop("host", None)
         headers.update(tmp_headers)
         if cls._LOG_CHAT:
```

### Comparing `openai_forward-0.1.3/openai_forward/app.py` & `openai_forward-0.1.4/openai_forward/app.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.3/openai_forward/config.py` & `openai_forward-0.1.4/openai_forward/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from loguru import logger
 import orjson
 from sparrow import relp
 from typing import Union, List, Dict
 import sys
 import logging
+import os
 
 
 class InterceptHandler(logging.Handler):
     def emit(self, record):
         # Get corresponding Loguru level if it exists
         try:
             level = logger.level(record.levelname).name
@@ -71,7 +72,17 @@
 def json_dump(data: Union[List, Dict], filepath: str, rel=False, indent_2=False, mode='wb'):
     orjson_option = 0
     if indent_2:
         orjson_option = orjson.OPT_INDENT_2
     abs_path = relp(filepath, parents=1) if rel else filepath
     with open(abs_path, mode=mode) as f:
         f.write(orjson.dumps(data, option=orjson_option))
+
+
+def str2list(s: str, sep=' '):
+    if s:
+        return [i.strip() for i in s.split(sep) if i.strip()]
+    else:
+        return []
+
+def env2list(env_name: str, sep=" "):
+    return str2list(os.environ.get(env_name, "").strip(), sep=sep)
```

### Comparing `openai_forward-0.1.3/openai_forward/openai.py` & `openai_forward-0.1.4/openai_forward/openai.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.3/openai_forward/content/chat.py` & `openai_forward-0.1.4/openai_forward/content/chat.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.3/openai_forward/routers/schemas.py` & `openai_forward-0.1.4/openai_forward/routers/schemas.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.3/.gitignore` & `openai_forward-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.3/LICENSE` & `openai_forward-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.3/README.md` & `openai_forward-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -43,46 +43,48 @@
 - [Service Deployment](#Service-Deployment)
 - [Service Usage](#Service-Usage)
 - [Configuration](#Configuration)
 
 # Features
 
 - [x] Supports forwarding of all OpenAI interfaces
-- [x] Supports request IP verification
-- [x] Supports streaming forwarding
-- [x] Supports default API key
+- [x] Request IP verification
+- [x] Streaming Response
+- [x] Supports default API key (cyclic call with multiple API keys)
 - [x] pip installation and deployment
 - [x] Docker deployment
 - [x] Support for multiple worker processes
-- [x] Support for specifying the forwarding routing prefix.
+- [x] Support for specifying the forwarding routing prefix
 
 # Usage
 
 > Here, the proxy address set up by the individual, https://caloi.top, is used as an example
 
 ### Using in a module
 
+
+**Python**
+
+```diff
+  import openai
++ openai.api_base = "https://caloi.top/v1"
+  openai.api_key = "sk-******"
+```
+
 **JS/TS**
 
 ```diff
   import { Configuration } from "openai";
   
   const configuration = new Configuration({
-+ basePath: "https://caloi.top",
++ basePath: "https://caloi.top/v1",
   apiKey: "sk-******",
   });
 ```
 
-**Python**
-
-```diff
-  import openai
-+ openai.api_base = "https://caloi.top/v1"
-  openai.api_key = "sk-******"
-```
 
 ### Image Generation (DALL-E):
 
 ```bash 
 curl --location 'https://caloi.top/v1/images/generations' \ 
 --header 'Authorization: Bearer sk-******' \ 
 --header 'Content-Type: application/json' \ 
@@ -151,16 +153,15 @@
 ``` 
 
 The 9999 port of the host is mapped, and the service can be accessed through `http://{ip}:9999`.
 Note: You can also pass in the environment variable OPENAI_API_KEY=sk-xxx as the default API key in the startup command.
 
 # Service Usage
 
-Simply replace the OpenAI API address with the address of the service we set up, such as:
-
+Simply replace the OpenAI API address with the address of the service we set up, such as `Chat Completion`
 ```bash 
 https://api.openai.com/v1/chat/completions 
 ``` 
 
 Replace with
 
 ```bash 
@@ -177,13 +178,13 @@
 | --workers | Number of worker processes | 1 |
 
 **Environment Variable Configuration Options**  
 refer to the `.env` file in the project root directory
 
 | Environment Variable  | Description | Default Value |
 |-----------------|------------|:------------------------:|
-| OPENAI_API_KEY  | Default API key | None |
+| OPENAI_API_KEY  | Default API key, supports multiple default API keys separated by space. | None |
 | OPENAI_BASE_URL | Forwarding base URL | `https://api.openai.com` |
 |LOG_CHAT| Whether to log chat content | `true` |
 |ROUTE_PREFIX| Route prefix | None |
-| IP_WHITELIST    | IP whitelist | None |
-| IP_BLACKLIST    | IP blacklist | None |
+| IP_WHITELIST    | IP whitelist, separated by space. | None |
+| IP_BLACKLIST    | IP blacklist, separated by space. | None |
```

#### html2text {}

```diff
@@ -10,57 +10,59 @@
 directly access OpenAI. The service is deployed on a server that can access the
 OpenAI API, and OpenAI requests are forwarded through the service, i.e. a
 reverse proxy service is set up. Test access: https://caloi.top/v1/chat/
 completions is equivalent to https://api.openai.com/v1/chat/completions # Table
 of Contents - [Features](#Features) - [Usage](#Usage) - [Service Deployment]
 (#Service-Deployment) - [Service Usage](#Service-Usage) - [Configuration]
 (#Configuration) # Features - [x] Supports forwarding of all OpenAI interfaces
-- [x] Supports request IP verification - [x] Supports streaming forwarding -
-[x] Supports default API key - [x] pip installation and deployment - [x] Docker
-deployment - [x] Support for multiple worker processes - [x] Support for
-specifying the forwarding routing prefix. # Usage > Here, the proxy address set
-up by the individual, https://caloi.top, is used as an example ### Using in a
-module **JS/TS** ```diff import { Configuration } from "openai"; const
-configuration = new Configuration({ + basePath: "https://caloi.top", apiKey:
-"sk-******", }); ``` **Python** ```diff import openai + openai.api_base =
-"https://caloi.top/v1" openai.api_key = "sk-******" ``` ### Image Generation
-(DALL-E): ```bash curl --location 'https://caloi.top/v1/images/generations' \ -
--header 'Authorization: Bearer sk-******' \ --header 'Content-Type:
-application/json' \ --data '{ "prompt": "A photo of a cat", "n": 1, "size":
-"512x512" }' ``` ### [chatgpt-web](https://github.com/Chanzhaoyu/chatgpt-web)
-Modify the `OPENAI_API_BASE_URL` in [Docker Compose](https://github.com/
-Chanzhaoyu/chatgpt-web#docker-compose) to the address of the proxy service we
-set up: ```bash OPENAI_API_BASE_URL: https://caloi.top ``` ### [ChatGPT-Next-
-Web](https://github.com/Yidadaa/ChatGPT-Next-Web) Replace `BASE_URL` in the
-docker startup command with the address of the proxy service we set up: ```bash
-docker run -d -p 3000:3000 -e OPENAI_API_KEY="sk-******" -e CODE="" -
-e BASE_URL="caloi.top" yidadaa/chatgpt-next-web ``` # Service Deployment Two
-service deployment methods are provided, choose one ## Use `pip` (recommended)
-**Installation** ```bash pip install openai-forward ``` **Run forwarding
-service** The port number can be specified through `--port`, which defaults to
-`8000`, and the number of worker processes can be specified through `--
-workers`, which defaults to `1`. ```bash openai_forward run --port=9999 --
+- [x] Request IP verification - [x] Streaming Response - [x] Supports default
+API key (cyclic call with multiple API keys) - [x] pip installation and
+deployment - [x] Docker deployment - [x] Support for multiple worker processes
+- [x] Support for specifying the forwarding routing prefix # Usage > Here, the
+proxy address set up by the individual, https://caloi.top, is used as an
+example ### Using in a module **Python** ```diff import openai +
+openai.api_base = "https://caloi.top/v1" openai.api_key = "sk-******" ``` **JS/
+TS** ```diff import { Configuration } from "openai"; const configuration = new
+Configuration({ + basePath: "https://caloi.top/v1", apiKey: "sk-******", });
+``` ### Image Generation (DALL-E): ```bash curl --location 'https://caloi.top/
+v1/images/generations' \ --header 'Authorization: Bearer sk-******' \ --header
+'Content-Type: application/json' \ --data '{ "prompt": "A photo of a cat", "n":
+1, "size": "512x512" }' ``` ### [chatgpt-web](https://github.com/Chanzhaoyu/
+chatgpt-web) Modify the `OPENAI_API_BASE_URL` in [Docker Compose](https://
+github.com/Chanzhaoyu/chatgpt-web#docker-compose) to the address of the proxy
+service we set up: ```bash OPENAI_API_BASE_URL: https://caloi.top ``` ###
+[ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-Web) Replace
+`BASE_URL` in the docker startup command with the address of the proxy service
+we set up: ```bash docker run -d -p 3000:3000 -e OPENAI_API_KEY="sk-******" -
+e CODE="" -e BASE_URL="caloi.top" yidadaa/chatgpt-next-web ``` # Service
+Deployment Two service deployment methods are provided, choose one ## Use `pip`
+(recommended) **Installation** ```bash pip install openai-forward ``` **Run
+forwarding service** The port number can be specified through `--port`, which
+defaults to `8000`, and the number of worker processes can be specified through
+`--workers`, which defaults to `1`. ```bash openai_forward run --port=9999 --
 workers=1 ``` The service is now set up, and the usage is to replace `https://
 api.openai.com` with the port number of the service `http://{ip}:{port}`. Of
 course, OPENAI_API_KEY can also be passed in as an environment variable as the
 default API key, so that the client does not need to pass in the Authorization
 in the header when requesting the relevant route. Startup command with default
 API key: ```bash OPENAI_API_KEY="sk-xxx" openai_forward run --port=9999 --
 workers=1 ``` Note: If both the default API key and the API key passed in the
 request header exist, the API key in the request header will override the
 default API key. ## Use Docker ```bash docker run --name="openai-forward" -d -
 p 9999:8000 beidongjiedeguang/openai-forward:latest ``` The 9999 port of the
 host is mapped, and the service can be accessed through `http://{ip}:9999`.
 Note: You can also pass in the environment variable OPENAI_API_KEY=sk-xxx as
 the default API key in the startup command. # Service Usage Simply replace the
-OpenAI API address with the address of the service we set up, such as: ```bash
-https://api.openai.com/v1/chat/completions ``` Replace with ```bash http://
-{ip}:{port}/v1/chat/completions ``` # Configuration **`openai-forward run`
-Parameter Configuration Options** | Configuration Option | Description |
-Default Value | |-----------| --- | :---: | | --port | Service port number |
-8000 | | --workers | Number of worker processes | 1 | **Environment Variable
-Configuration Options** refer to the `.env` file in the project root directory
-| Environment Variable | Description | Default Value | |-----------------|-----
--------|:------------------------:| | OPENAI_API_KEY | Default API key | None |
-| OPENAI_BASE_URL | Forwarding base URL | `https://api.openai.com` | |LOG_CHAT|
-Whether to log chat content | `true` | |ROUTE_PREFIX| Route prefix | None | |
-IP_WHITELIST | IP whitelist | None | | IP_BLACKLIST | IP blacklist | None |
+OpenAI API address with the address of the service we set up, such as `Chat
+Completion` ```bash https://api.openai.com/v1/chat/completions ``` Replace with
+```bash http://{ip}:{port}/v1/chat/completions ``` # Configuration **`openai-
+forward run` Parameter Configuration Options** | Configuration Option |
+Description | Default Value | |-----------| --- | :---: | | --port | Service
+port number | 8000 | | --workers | Number of worker processes | 1 |
+**Environment Variable Configuration Options** refer to the `.env` file in the
+project root directory | Environment Variable | Description | Default Value |
+|-----------------|------------|:------------------------:| | OPENAI_API_KEY |
+Default API key, supports multiple default API keys separated by space. | None
+| | OPENAI_BASE_URL | Forwarding base URL | `https://api.openai.com` |
+|LOG_CHAT| Whether to log chat content | `true` | |ROUTE_PREFIX| Route prefix |
+None | | IP_WHITELIST | IP whitelist, separated by space. | None | |
+IP_BLACKLIST | IP blacklist, separated by space. | None |
```

### Comparing `openai_forward-0.1.3/pyproject.toml` & `openai_forward-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.3/PKG-INFO` & `openai_forward-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_forward
-Version: 0.1.3
+Version: 0.1.4
 Summary: 🚀 Openai api forward · OpenAI 接口转发服务 · streaming forward
 Project-URL: Homepage, https://github.com/beidongjiedeguang/openai-forward
 Project-URL: Documentation, https://github.com/beidongjiedeguang/openai-forward#openai-forward
 Project-URL: Issues, https://github.com/beidongjiedeguang/openai-forward/issues
 Project-URL: Source, https://github.com/beidongjiedeguang/openai-forward
 Author-email: kunyuan <beidongjiedeguang@gmail.com>
 License-File: LICENSE
@@ -75,46 +75,48 @@
 - [Service Deployment](#Service-Deployment)
 - [Service Usage](#Service-Usage)
 - [Configuration](#Configuration)
 
 # Features
 
 - [x] Supports forwarding of all OpenAI interfaces
-- [x] Supports request IP verification
-- [x] Supports streaming forwarding
-- [x] Supports default API key
+- [x] Request IP verification
+- [x] Streaming Response
+- [x] Supports default API key (cyclic call with multiple API keys)
 - [x] pip installation and deployment
 - [x] Docker deployment
 - [x] Support for multiple worker processes
-- [x] Support for specifying the forwarding routing prefix.
+- [x] Support for specifying the forwarding routing prefix
 
 # Usage
 
 > Here, the proxy address set up by the individual, https://caloi.top, is used as an example
 
 ### Using in a module
 
+
+**Python**
+
+```diff
+  import openai
++ openai.api_base = "https://caloi.top/v1"
+  openai.api_key = "sk-******"
+```
+
 **JS/TS**
 
 ```diff
   import { Configuration } from "openai";
   
   const configuration = new Configuration({
-+ basePath: "https://caloi.top",
++ basePath: "https://caloi.top/v1",
   apiKey: "sk-******",
   });
 ```
 
-**Python**
-
-```diff
-  import openai
-+ openai.api_base = "https://caloi.top/v1"
-  openai.api_key = "sk-******"
-```
 
 ### Image Generation (DALL-E):
 
 ```bash 
 curl --location 'https://caloi.top/v1/images/generations' \ 
 --header 'Authorization: Bearer sk-******' \ 
 --header 'Content-Type: application/json' \ 
@@ -183,16 +185,15 @@
 ``` 
 
 The 9999 port of the host is mapped, and the service can be accessed through `http://{ip}:9999`.
 Note: You can also pass in the environment variable OPENAI_API_KEY=sk-xxx as the default API key in the startup command.
 
 # Service Usage
 
-Simply replace the OpenAI API address with the address of the service we set up, such as:
-
+Simply replace the OpenAI API address with the address of the service we set up, such as `Chat Completion`
 ```bash 
 https://api.openai.com/v1/chat/completions 
 ``` 
 
 Replace with
 
 ```bash 
@@ -209,13 +210,13 @@
 | --workers | Number of worker processes | 1 |
 
 **Environment Variable Configuration Options**  
 refer to the `.env` file in the project root directory
 
 | Environment Variable  | Description | Default Value |
 |-----------------|------------|:------------------------:|
-| OPENAI_API_KEY  | Default API key | None |
+| OPENAI_API_KEY  | Default API key, supports multiple default API keys separated by space. | None |
 | OPENAI_BASE_URL | Forwarding base URL | `https://api.openai.com` |
 |LOG_CHAT| Whether to log chat content | `true` |
 |ROUTE_PREFIX| Route prefix | None |
-| IP_WHITELIST    | IP whitelist | None |
-| IP_BLACKLIST    | IP blacklist | None |
+| IP_WHITELIST    | IP whitelist, separated by space. | None |
+| IP_BLACKLIST    | IP blacklist, separated by space. | None |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openai_forward Version: 0.1.3 Summary: ð Openai
+Metadata-Version: 2.1 Name: openai_forward Version: 0.1.4 Summary: ð Openai
 api forward Â· OpenAI æ¥å£è½¬åæå¡ Â· streaming forward Project-URL:
 Homepage, https://github.com/beidongjiedeguang/openai-forward Project-URL:
 Documentation, https://github.com/beidongjiedeguang/openai-forward#openai-
 forward Project-URL: Issues, https://github.com/beidongjiedeguang/openai-
 forward/issues Project-URL: Source, https://github.com/beidongjiedeguang/
 openai-forward Author-email: kunyuan
 gmail.com> License-File: LICENSE Keywords:
@@ -28,57 +28,59 @@
 directly access OpenAI. The service is deployed on a server that can access the
 OpenAI API, and OpenAI requests are forwarded through the service, i.e. a
 reverse proxy service is set up. Test access: https://caloi.top/v1/chat/
 completions is equivalent to https://api.openai.com/v1/chat/completions # Table
 of Contents - [Features](#Features) - [Usage](#Usage) - [Service Deployment]
 (#Service-Deployment) - [Service Usage](#Service-Usage) - [Configuration]
 (#Configuration) # Features - [x] Supports forwarding of all OpenAI interfaces
-- [x] Supports request IP verification - [x] Supports streaming forwarding -
-[x] Supports default API key - [x] pip installation and deployment - [x] Docker
-deployment - [x] Support for multiple worker processes - [x] Support for
-specifying the forwarding routing prefix. # Usage > Here, the proxy address set
-up by the individual, https://caloi.top, is used as an example ### Using in a
-module **JS/TS** ```diff import { Configuration } from "openai"; const
-configuration = new Configuration({ + basePath: "https://caloi.top", apiKey:
-"sk-******", }); ``` **Python** ```diff import openai + openai.api_base =
-"https://caloi.top/v1" openai.api_key = "sk-******" ``` ### Image Generation
-(DALL-E): ```bash curl --location 'https://caloi.top/v1/images/generations' \ -
--header 'Authorization: Bearer sk-******' \ --header 'Content-Type:
-application/json' \ --data '{ "prompt": "A photo of a cat", "n": 1, "size":
-"512x512" }' ``` ### [chatgpt-web](https://github.com/Chanzhaoyu/chatgpt-web)
-Modify the `OPENAI_API_BASE_URL` in [Docker Compose](https://github.com/
-Chanzhaoyu/chatgpt-web#docker-compose) to the address of the proxy service we
-set up: ```bash OPENAI_API_BASE_URL: https://caloi.top ``` ### [ChatGPT-Next-
-Web](https://github.com/Yidadaa/ChatGPT-Next-Web) Replace `BASE_URL` in the
-docker startup command with the address of the proxy service we set up: ```bash
-docker run -d -p 3000:3000 -e OPENAI_API_KEY="sk-******" -e CODE="" -
-e BASE_URL="caloi.top" yidadaa/chatgpt-next-web ``` # Service Deployment Two
-service deployment methods are provided, choose one ## Use `pip` (recommended)
-**Installation** ```bash pip install openai-forward ``` **Run forwarding
-service** The port number can be specified through `--port`, which defaults to
-`8000`, and the number of worker processes can be specified through `--
-workers`, which defaults to `1`. ```bash openai_forward run --port=9999 --
+- [x] Request IP verification - [x] Streaming Response - [x] Supports default
+API key (cyclic call with multiple API keys) - [x] pip installation and
+deployment - [x] Docker deployment - [x] Support for multiple worker processes
+- [x] Support for specifying the forwarding routing prefix # Usage > Here, the
+proxy address set up by the individual, https://caloi.top, is used as an
+example ### Using in a module **Python** ```diff import openai +
+openai.api_base = "https://caloi.top/v1" openai.api_key = "sk-******" ``` **JS/
+TS** ```diff import { Configuration } from "openai"; const configuration = new
+Configuration({ + basePath: "https://caloi.top/v1", apiKey: "sk-******", });
+``` ### Image Generation (DALL-E): ```bash curl --location 'https://caloi.top/
+v1/images/generations' \ --header 'Authorization: Bearer sk-******' \ --header
+'Content-Type: application/json' \ --data '{ "prompt": "A photo of a cat", "n":
+1, "size": "512x512" }' ``` ### [chatgpt-web](https://github.com/Chanzhaoyu/
+chatgpt-web) Modify the `OPENAI_API_BASE_URL` in [Docker Compose](https://
+github.com/Chanzhaoyu/chatgpt-web#docker-compose) to the address of the proxy
+service we set up: ```bash OPENAI_API_BASE_URL: https://caloi.top ``` ###
+[ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-Web) Replace
+`BASE_URL` in the docker startup command with the address of the proxy service
+we set up: ```bash docker run -d -p 3000:3000 -e OPENAI_API_KEY="sk-******" -
+e CODE="" -e BASE_URL="caloi.top" yidadaa/chatgpt-next-web ``` # Service
+Deployment Two service deployment methods are provided, choose one ## Use `pip`
+(recommended) **Installation** ```bash pip install openai-forward ``` **Run
+forwarding service** The port number can be specified through `--port`, which
+defaults to `8000`, and the number of worker processes can be specified through
+`--workers`, which defaults to `1`. ```bash openai_forward run --port=9999 --
 workers=1 ``` The service is now set up, and the usage is to replace `https://
 api.openai.com` with the port number of the service `http://{ip}:{port}`. Of
 course, OPENAI_API_KEY can also be passed in as an environment variable as the
 default API key, so that the client does not need to pass in the Authorization
 in the header when requesting the relevant route. Startup command with default
 API key: ```bash OPENAI_API_KEY="sk-xxx" openai_forward run --port=9999 --
 workers=1 ``` Note: If both the default API key and the API key passed in the
 request header exist, the API key in the request header will override the
 default API key. ## Use Docker ```bash docker run --name="openai-forward" -d -
 p 9999:8000 beidongjiedeguang/openai-forward:latest ``` The 9999 port of the
 host is mapped, and the service can be accessed through `http://{ip}:9999`.
 Note: You can also pass in the environment variable OPENAI_API_KEY=sk-xxx as
 the default API key in the startup command. # Service Usage Simply replace the
-OpenAI API address with the address of the service we set up, such as: ```bash
-https://api.openai.com/v1/chat/completions ``` Replace with ```bash http://
-{ip}:{port}/v1/chat/completions ``` # Configuration **`openai-forward run`
-Parameter Configuration Options** | Configuration Option | Description |
-Default Value | |-----------| --- | :---: | | --port | Service port number |
-8000 | | --workers | Number of worker processes | 1 | **Environment Variable
-Configuration Options** refer to the `.env` file in the project root directory
-| Environment Variable | Description | Default Value | |-----------------|-----
--------|:------------------------:| | OPENAI_API_KEY | Default API key | None |
-| OPENAI_BASE_URL | Forwarding base URL | `https://api.openai.com` | |LOG_CHAT|
-Whether to log chat content | `true` | |ROUTE_PREFIX| Route prefix | None | |
-IP_WHITELIST | IP whitelist | None | | IP_BLACKLIST | IP blacklist | None |
+OpenAI API address with the address of the service we set up, such as `Chat
+Completion` ```bash https://api.openai.com/v1/chat/completions ``` Replace with
+```bash http://{ip}:{port}/v1/chat/completions ``` # Configuration **`openai-
+forward run` Parameter Configuration Options** | Configuration Option |
+Description | Default Value | |-----------| --- | :---: | | --port | Service
+port number | 8000 | | --workers | Number of worker processes | 1 |
+**Environment Variable Configuration Options** refer to the `.env` file in the
+project root directory | Environment Variable | Description | Default Value |
+|-----------------|------------|:------------------------:| | OPENAI_API_KEY |
+Default API key, supports multiple default API keys separated by space. | None
+| | OPENAI_BASE_URL | Forwarding base URL | `https://api.openai.com` |
+|LOG_CHAT| Whether to log chat content | `true` | |ROUTE_PREFIX| Route prefix |
+None | | IP_WHITELIST | IP whitelist, separated by space. | None | |
+IP_BLACKLIST | IP blacklist, separated by space. | None |
```

