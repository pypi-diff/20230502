# Comparing `tmp/EdgeGPT-0.3.3.tar.gz` & `tmp/EdgeGPT-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EdgeGPT-0.3.3.tar", last modified: Tue May  2 02:47:17 2023, max compression
+gzip compressed data, was "EdgeGPT-0.3.4.tar", last modified: Tue May  2 04:36:57 2023, max compression
```

## Comparing `EdgeGPT-0.3.3.tar` & `EdgeGPT-0.3.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 02:47:17.171166 EdgeGPT-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-02 02:46:47.000000 EdgeGPT-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-05-02 02:47:17.171166 EdgeGPT-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-05-02 02:47:16.000000 EdgeGPT-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-02 02:47:17.171166 EdgeGPT-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-02 02:46:47.000000 EdgeGPT-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 02:47:17.171166 EdgeGPT-0.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 02:47:17.171166 EdgeGPT-0.3.3/src/EdgeGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-05-02 02:47:17.000000 EdgeGPT-0.3.3/src/EdgeGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-02 02:47:17.000000 EdgeGPT-0.3.3/src/EdgeGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 02:47:17.000000 EdgeGPT-0.3.3/src/EdgeGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-02 02:47:17.000000 EdgeGPT-0.3.3/src/EdgeGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-02 02:47:17.000000 EdgeGPT-0.3.3/src/EdgeGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 02:47:17.000000 EdgeGPT-0.3.3/src/EdgeGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    25243 2023-05-02 02:46:47.000000 EdgeGPT-0.3.3/src/EdgeGPT.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-02 02:46:47.000000 EdgeGPT-0.3.3/src/ImageGen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:36:57.734876 EdgeGPT-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-02 04:36:22.000000 EdgeGPT-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-05-02 04:36:57.734876 EdgeGPT-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-05-02 04:36:57.000000 EdgeGPT-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-02 04:36:57.734876 EdgeGPT-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-02 04:36:22.000000 EdgeGPT-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:36:57.730876 EdgeGPT-0.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:36:57.734876 EdgeGPT-0.3.4/src/EdgeGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-05-02 04:36:57.000000 EdgeGPT-0.3.4/src/EdgeGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-02 04:36:57.000000 EdgeGPT-0.3.4/src/EdgeGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 04:36:57.000000 EdgeGPT-0.3.4/src/EdgeGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-02 04:36:57.000000 EdgeGPT-0.3.4/src/EdgeGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-02 04:36:57.000000 EdgeGPT-0.3.4/src/EdgeGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 04:36:57.000000 EdgeGPT-0.3.4/src/EdgeGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    27654 2023-05-02 04:36:22.000000 EdgeGPT-0.3.4/src/EdgeGPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-02 04:36:22.000000 EdgeGPT-0.3.4/src/ImageGen.py
```

### Comparing `EdgeGPT-0.3.3/LICENSE` & `EdgeGPT-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.3.3/PKG-INFO` & `EdgeGPT-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.3.3
+Version: 0.3.4
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.3 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.4 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `EdgeGPT-0.3.3/README.md` & `EdgeGPT-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.3.3/setup.py` & `EdgeGPT-0.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="EdgeGPT",
-    version="0.3.3",
+    version="0.3.4",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineered Edge Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/EdgeGPT",
```

### Comparing `EdgeGPT-0.3.3/src/EdgeGPT.egg-info/PKG-INFO` & `EdgeGPT-0.3.4/src/EdgeGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.3.3
+Version: 0.3.4
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.3 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.4 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `EdgeGPT-0.3.3/src/EdgeGPT.py` & `EdgeGPT-0.3.4/src/EdgeGPT.py`

 * *Files 4% similar despite different names*

```diff
@@ -188,15 +188,15 @@
         self.invocation_id: int = invocation_id
 
     def update(
         self,
         prompt: str,
         conversation_style: CONVERSATION_STYLE_TYPE,
         options: list | None = None,
-        webpage_context: str | None = None
+        webpage_context: str | None = None,
     ) -> None:
         """
         Updates request object
         """
         if options is None:
             options = [
                 "deepleo",
@@ -257,35 +257,93 @@
                 },
             ],
             "invocationId": str(self.invocation_id),
             "target": "chat",
             "type": 4,
         }
         if webpage_context:
-            self.struct["arguments"][0]["previousMessages"] = [{
-                "author": 'user',
-                "description": webpage_context,
-                "contextType": 'WebPage',
-                "messageType": 'Context',
-                "messageId": 'discover-web--page-ping-mriduna-----',
-            }]
+            self.struct["arguments"][0]["previousMessages"] = [
+                {
+                    "author": "user",
+                    "description": webpage_context,
+                    "contextType": "WebPage",
+                    "messageType": "Context",
+                    "messageId": "discover-web--page-ping-mriduna-----",
+                }
+            ]
         self.invocation_id += 1
 
 
 class _Conversation:
     """
     Conversation API
     """
 
+    def __init__(
+        self,
+        cookies: dict | None = None,
+        proxy: str | None = None,
+        async_mode: bool = False,
+    ) -> None:
+        if async_mode:
+            return
+        self.struct: dict = {
+            "conversationId": None,
+            "clientId": None,
+            "conversationSignature": None,
+            "result": {"value": "Success", "message": None},
+        }
+        self.proxy = proxy
+        proxy = (
+            proxy
+            or os.environ.get("all_proxy")
+            or os.environ.get("ALL_PROXY")
+            or os.environ.get("https_proxy")
+            or os.environ.get("HTTPS_PROXY")
+            or None
+        )
+        if proxy is not None and proxy.startswith("socks5h://"):
+            proxy = "socks5://" + proxy[len("socks5h://") :]
+        self.session = httpx.Client(
+            proxies=proxy,
+            timeout=30,
+            headers=HEADERS_INIT_CONVER,
+        )
+        for cookie in cookies:
+            self.session.cookies.set(cookie["name"], cookie["value"])
+
+        # Send GET request
+        response = self.session.get(
+            url=os.environ.get("BING_PROXY_URL")
+            or "https://edgeservices.bing.com/edgesvc/turing/conversation/create",
+        )
+        if response.status_code != 200:
+            response = self.session.get(
+                "https://edge.churchless.tech/edgesvc/turing/conversation/create",
+            )
+        if response.status_code != 200:
+            print(f"Status code: {response.status_code}")
+            print(response.text)
+            print(response.url)
+            raise Exception("Authentication failed")
+        try:
+            self.struct = response.json()
+        except (json.decoder.JSONDecodeError, NotAllowedToAccess) as exc:
+            raise Exception(
+                "Authentication failed. You have not been accepted into the beta.",
+            ) from exc
+        if self.struct["result"]["value"] == "UnauthorizedRequest":
+            raise NotAllowedToAccess(self.struct["result"]["message"])
+
     @staticmethod
     async def create(
         cookies: dict,
         proxy: str | None = None,
     ) -> None:
-        self = _Conversation()
+        self = _Conversation(async_mode=True)
         self.struct = {
             "conversationId": None,
             "clientId": None,
             "conversationSignature": None,
             "result": {"value": "Success", "message": None},
         }
         self.proxy = proxy
@@ -305,15 +363,15 @@
             headers=HEADERS_INIT_CONVER,
         ) as client:
             for cookie in cookies:
                 client.cookies.set(cookie["name"], cookie["value"])
 
             # Send GET request
             response = await client.get(
-                url = os.environ.get("BING_PROXY_URL")
+                url=os.environ.get("BING_PROXY_URL")
                 or "https://edgeservices.bing.com/edgesvc/turing/conversation/create",
             )
             if response.status_code != 200:
                 response = await client.get(
                     "https://edge.churchless.tech/edgesvc/turing/conversation/create",
                 )
         if response.status_code != 200:
@@ -352,15 +410,15 @@
         self,
         prompt: str,
         wss_link: str,
         cookies: str,
         conversation_style: CONVERSATION_STYLE_TYPE = None,
         raw: bool = False,
         options: dict = None,
-        webpage_context: str | None = None
+        webpage_context: str | None = None,
     ) -> Generator[str, None, None]:
         """
         Ask a question to the bot
         """
         if self.wss and not self.wss.closed:
             await self.wss.close()
         # Check if websocket is closed
@@ -378,32 +436,30 @@
                 conversation_style=conversation_style,
                 options=options,
                 webpage_context=webpage_context,
             )
         else:
             async with httpx.AsyncClient() as client:
                 response = await client.post(
-                    'https://sydney.bing.com/sydney/UpdateConversation/',
+                    "https://sydney.bing.com/sydney/UpdateConversation/",
                     json={
                         "messages": [
                             {
                                 "author": "user",
                                 "description": webpage_context,
                                 "contextType": "WebPage",
-                                "messageType": "Context"
+                                "messageType": "Context",
                             }
                         ],
                         "conversationId": self.request.conversation_id,
                         "source": "cib",
                         "traceId": _get_ran_hex(32),
-                        "participant": {
-                            "id": self.request.client_id
-                        },
-                        "conversationSignature": self.request.conversation_signature
-                    }
+                        "participant": {"id": self.request.client_id},
+                        "conversationSignature": self.request.conversation_signature,
+                    },
                 )
             if response.status_code != 200:
                 print(f"Status code: {response.status_code}")
                 print(response.text)
                 print(response.url)
                 raise Exception("Update web page context failed")
             # Construct a ChatHub request
@@ -412,34 +468,39 @@
                 conversation_style=conversation_style,
                 options=options,
             )
         # Send request
         await self.wss.send(_append_identifier(self.request.struct))
         final = False
         draw = False
-        resp_txt = ''
-        resp_txt_no_link = ''
+        resp_txt = ""
+        resp_txt_no_link = ""
         while not final:
             objects = str(await self.wss.recv()).split(DELIMITER)
             for obj in objects:
                 if obj is None or not obj:
                     continue
                 response = json.loads(obj)
                 if response.get("type") != 2 and raw:
                     yield False, response
                 elif response.get("type") == 1 and response["arguments"][0].get(
                     "messages",
                 ):
                     try:
                         if not draw:
-                            if response["arguments"][0]["messages"][0]["contentOrigin"] != "Apology":
+                            if (
+                                response["arguments"][0]["messages"][0]["contentOrigin"]
+                                != "Apology"
+                            ):
                                 resp_txt = response["arguments"][0]["messages"][0][
                                     "adaptiveCards"
-                                ][0]["body"][0].get("text", '')
-                                resp_txt_no_link = response["arguments"][0]["messages"][0].get("text", '')
+                                ][0]["body"][0].get("text", "")
+                                resp_txt_no_link = response["arguments"][0]["messages"][
+                                    0
+                                ].get("text", "")
                         yield False, resp_txt
                     except Exception as exc:
                         print(exc)
                         if not draw:
                             continue
                         for item in cookies:
                             if item["name"] == "_U":
@@ -466,18 +527,25 @@
                     if draw:
                         cache = response["item"]["messages"][1]["adaptiveCards"][0][
                             "body"
                         ][0]["text"]
                         response["item"]["messages"][1]["adaptiveCards"][0]["body"][0][
                             "text"
                         ] = (cache + resp_txt)
-                    if response["item"]["messages"][-1]["contentOrigin"] == "Apology" and resp_txt:
+                    if (
+                        response["item"]["messages"][-1]["contentOrigin"] == "Apology"
+                        and resp_txt
+                    ):
                         response["item"]["messages"][-1]["text"] = resp_txt_no_link
-                        response["item"]["messages"][-1]["adaptiveCards"][0]["body"][0]["text"] = resp_txt
-                        print(f"Preserved the message from being deleted", file=sys.stderr)
+                        response["item"]["messages"][-1]["adaptiveCards"][0]["body"][0][
+                            "text"
+                        ] = resp_txt
+                        print(
+                            f"Preserved the message from being deleted", file=sys.stderr
+                        )
                     final = True
                     yield True, response
 
     async def _initial_handshake(self) -> None:
         await self.wss.send(_append_identifier({"protocol": "json", "version": 1}))
         await self.wss.recv()
 
@@ -530,15 +598,15 @@
         """
         async for final, response in self.chat_hub.ask_stream(
             prompt=prompt,
             conversation_style=conversation_style,
             wss_link=wss_link,
             options=options,
             cookies=self.cookies,
-            webpage_context=webpage_context
+            webpage_context=webpage_context,
         ):
             if final:
                 return response
         await self.chat_hub.wss.close()
         return None
 
     async def ask_stream(
@@ -556,15 +624,15 @@
         async for response in self.chat_hub.ask_stream(
             prompt=prompt,
             conversation_style=conversation_style,
             wss_link=wss_link,
             raw=raw,
             options=options,
             cookies=self.cookies,
-            webpage_context=webpage_context
+            webpage_context=webpage_context,
         ):
             yield response
 
     async def close(self) -> None:
         """
         Close the connection
         """
```

