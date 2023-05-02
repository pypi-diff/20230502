# Comparing `tmp/jsonrpcx-3.3.1-py3-none-any.whl.zip` & `tmp/jsonrpcx-4.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 14419 bytes, number of entries: 6
--rw-r--r--  2.0 unx    30429 b- defN 23-Apr-28 15:31 jsonrpcx/__init__.py
--rw-r--r--  2.0 unx     1023 b- defN 23-Apr-28 15:40 jsonrpcx-3.3.1.dist-info/LICENCE
--rw-r--r--  2.0 unx    14136 b- defN 23-Apr-28 15:40 jsonrpcx-3.3.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 15:40 jsonrpcx-3.3.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Apr-28 15:40 jsonrpcx-3.3.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      469 b- defN 23-Apr-28 15:40 jsonrpcx-3.3.1.dist-info/RECORD
-6 files, 46158 bytes uncompressed, 13573 bytes compressed:  70.6%
+Zip file size: 15161 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    32630 b- defN 23-May-02 18:21 jsonrpcx/__init__.py
+-rw-r--r--  2.0 unx     1023 b- defN 23-May-02 18:23 jsonrpcx-4.0.0.dist-info/LICENCE
+-rw-r--r--  2.0 unx    15210 b- defN 23-May-02 18:23 jsonrpcx-4.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-02 18:23 jsonrpcx-4.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-May-02 18:23 jsonrpcx-4.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      469 b- defN 23-May-02 18:23 jsonrpcx-4.0.0.dist-info/RECORD
+6 files, 49433 bytes uncompressed, 14315 bytes compressed:  71.0%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: jsonrpcx/__init__.py
 Comment: 
 
-Filename: jsonrpcx-3.3.1.dist-info/LICENCE
+Filename: jsonrpcx-4.0.0.dist-info/LICENCE
 Comment: 
 
-Filename: jsonrpcx-3.3.1.dist-info/METADATA
+Filename: jsonrpcx-4.0.0.dist-info/METADATA
 Comment: 
 
-Filename: jsonrpcx-3.3.1.dist-info/WHEEL
+Filename: jsonrpcx-4.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: jsonrpcx-3.3.1.dist-info/top_level.txt
+Filename: jsonrpcx-4.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: jsonrpcx-3.3.1.dist-info/RECORD
+Filename: jsonrpcx-4.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jsonrpcx/__init__.py

```diff
@@ -393,22 +393,16 @@
                             data=requestMessage.stringify(),
                             headers={'content-type': 'application/json'},
                             timeout=30,
                             )
     return _processCallResponse(resp)
 
 
-class DiscoverMixin:
-    async def rpcDiscover(self) -> Dict:
-        """
-        Returns OpenRPC JSON (https://spec.open-rpc.org/) description of the API.
-        """
-        return self.rpcDiscover()
-
-    def rpcDiscover(self) -> Dict:
+class _DiscoverCore:
+    def _rpcDiscover(self) -> Dict:
         """
         Returns OpenRPC JSON (https://spec.open-rpc.org/) description of the API.
         """
         # TODO: Add better support for List[], Optional[] and Union[] all of those work to some extend but could have better support.
 
         def isParameterRequired(param: inspect.Parameter) -> bool:
             # Has a default value
@@ -462,25 +456,32 @@
                     "required": isParameterRequired(param),
                 }
                 schema = buildSchema(param.annotation)
                 if schema:
                     data.update(schema)
                 params.append(data)
             return params
-
+        
         def reduceMethodNamesWith(acc, method):
-            methodName = "rpc.discover" if method[0] == "rpcDiscover" else method[0]
+            methodNameMapping = {
+                "rpcDiscover": "rpc.discover",
+                "rpcCancel": "rpc.cancel",
+            }
+            methodName = methodNameMapping[method[0]] if method[0] in methodNameMapping.keys() else method[0]
             methodObject = method[1]
             if methodName[0] == "_" or methodName == "parseRequest":
                 # Don't add magic methods or private methods.
                 return acc
-            docstring = inspect.getdoc(methodObject)
+            returnsStream = inspect.isasyncgenfunction(methodObject)
+            docstring = inspect.getdoc(methodObject) or ""
+            methodReturnsStreamComment = "**This method returns an HTTP response stream which is an extension to JSON-RPC2.0 and not implemented in every library.**" if returnsStream else ""
+            methodComments = docstring + "\n\n" + methodReturnsStreamComment
             methodInfo = {
                 "name": methodName,
-                "description": docstring if docstring else "",
+                "description": methodComments,
                 "paramStructure": "by-name",
                 "params": buildParamList(inspect.signature(methodObject)),
             }
             schemaName = "Invokation Result"
             schema = buildSchema(inspect.signature(
                 methodObject).return_annotation, schemaName)
             # Currently the fallback is used if the return type is Optional or Union
@@ -496,41 +497,45 @@
             "info": self.delegate.experimentalOpenRPCInfo(),
             "servers": self.delegate.experimentalOpenRPCServers(),
             "methods": reduce(reduceMethodNamesWith, rpcMethods, [])
         }
         
 
 
+
+
+
 _COMMONSERVER_RUNNING_REQUESTS = {}
 
 
 class ExperimentalCancelRequestMixin():
     """This only works with async servers.
 
     An experimental mixin allowing you to cancel long running requests.
     Since this would allow every client to cancel requests from other clients this is currently considered experimental until there are solutions for this problem.
     Once this problem is solved this will be moved to the base class.
     """
 
     async def rpcCancel(self, id: str) -> None:
         """Cancel a long running request. This works similar to how it is described here https://microsoft.github.io/language-server-protocol/specifications/specification-3-15/
+        Note: Methods which stream responses can currently not be canceled.
 
         Args:
             cancelId (str): _description_
 
         Returns:
             None: SUBJECT TO CHANGE. This is actualy a notifications so it does not return anything acording to spec. This might change in the future.
         """
         messageId = id
         if messageId in _COMMONSERVER_RUNNING_REQUESTS:
             _COMMONSERVER_RUNNING_REQUESTS[messageId].cancel()
         return None
 
 
-class CommonServer(DiscoverMixin):
+class CommonServerCore(_DiscoverCore):
     def __init__(self, delegate=None):
         self.delegate = delegate
     
     def _error(self, messageId, jsonRpcErrorCode: int) -> Error:
         self.log.debug({
             PARSE_ERROR: "parse error",
             INVALID_REQUEST: "invalid request",
@@ -551,46 +556,14 @@
             return error
         method = callInfo["method"]
         params = callInfo["params"]
         assert type(params) in [list, dict], "params must be list or dict"
         result = method(**params) if type(params) == dict else method(*params)
         return Message.fromResponse(Response.fromResultPrimitive(result), messageId=callInfo["messageId"])
 
-    async def _async_processRequest(self, rawRequest: str) -> Message:
-            print("CALLING THIS FUNC")
-            error, callInfo = self._processRequestCore(rawRequest)
-            if error:
-                return error
-            method = callInfo["method"]
-            params = callInfo["params"]
-            messageId = callInfo["messageId"]
-            methodName = callInfo["methodName"]
-            assert type(params) in [list, dict], "params must be list or dict"
-            def mkResult(result):
-                return Message.fromResponse(Response.fromResultPrimitive(result), messageId=messageId)
-
-            methodCall = method(**params) if type(params) == dict else method(*params)
-            task = asyncio.create_task(methodCall)
-
-            isCancelRequest = methodName in ("rpcCancel", "rpc.cancel")
-
-            if not isCancelRequest:
-                await self.delegate.experimentalAddRunningRequest(messageId, task)
-
-            while task.done() == False:
-                await self.delegate.experimentalWaitOnCancelRequest()
-
-            if not isCancelRequest:
-                await self.delegate.experimentalRemoveRunningRequest(messageId)
-
-            try:
-                return mkResult(task.result())
-            except asyncio.exceptions.CancelledError:
-                return Message.fromResponse(Response.fromError(Error(theCode=REQUEST_CANCELLED, theMessage="Request was cancelled")), messageId=messageId)
-
     def _processRequestCore(self, rawRequest: str):
         # Instead of directly calling the rpc method we could just return information about
         # how it should be called. The advantage is that it can be used from a sync and async function call
         # allowing the new async feature of Python while maintaining backward compatibility
         if not rawRequest:
             return self._error(None, INVALID_REQUEST), None
 
@@ -641,14 +614,84 @@
             else:
                 raise Exception("JSON-RPC 2.0 CommonServer Parameters passed must bee DICT or LIST.")
         except Exception as ex:
             logging.exception(ex)
             return self._error(requestingRPCMessage.id, INTERNAL_ERROR), None
 
 
+class CommonSyncServer(CommonServerCore):
+    def rpcDiscover(self) -> Dict:
+        """
+        Returns OpenRPC JSON (https://spec.open-rpc.org/) description of the API.
+        """
+        return self._rpcDiscover()
+
+
+class CommonAsyncServer(CommonServerCore):
+    async def rpcDiscover(self) -> Dict:
+        """
+        Returns OpenRPC JSON (https://spec.open-rpc.org/) description of the API.
+        """
+        return self._rpcDiscover()
+
+    async def _async_processRequest(self, rawRequest: str, send=None) -> Optional[Message]:
+            print("CALLING THIS FUNC")
+            error, callInfo = self._processRequestCore(rawRequest)
+            if error:
+                return error
+            method = callInfo["method"]
+            params = callInfo["params"]
+            assert type(params) in [list, dict], "params must be list or dict"
+            # Check if the method is a generator function and if so it needs to be handled as a stream.
+            if inspect.isasyncgenfunction(method): 
+                await self._async_processRequestWithResponseStream(callInfo, send)
+                return None
+            return await self._async_processNormalRequest(callInfo)
+
+    async def _async_processNormalRequest(self, callInfo) -> Message:
+            method = callInfo["method"]
+            params = callInfo["params"]
+            methodName = callInfo["methodName"]
+            messageId = callInfo["messageId"]
+            methodCall = method(**params) if type(params) == dict else method(*params)
+            task = asyncio.create_task(methodCall)
+
+            isCancelRequest = methodName in ("rpcCancel", "rpc.cancel")
+
+            if not isCancelRequest:
+                await self.delegate.experimentalAddRunningRequest(messageId, task)
+
+            while task.done() == False:
+                await self.delegate.experimentalWaitOnCancelRequest()
+
+            if not isCancelRequest:
+                await self.delegate.experimentalRemoveRunningRequest(messageId)
+
+            try:
+                return Message.fromResponse(Response.fromResultPrimitive(task.result()), messageId=messageId)
+            except asyncio.exceptions.CancelledError:
+                return Message.fromResponse(Response.fromError(Error(theCode=REQUEST_CANCELLED, theMessage="Request was cancelled")), messageId=messageId)
+
+    async def _async_processRequestWithResponseStream(self, callInfo, send) -> None:
+            method = callInfo["method"]
+            params = callInfo["params"]
+            async for result in method(**params) if type(params) == dict else method(*params):
+                await send({
+                    'type': 'http.response.body',
+                    'body': json.dumps(result).encode("utf-8"),
+                    'more_body': True
+                })
+            # Close the response stream
+            await send({
+                'type': 'http.response.body',
+                'body': b'',
+            })
+
+
+
 class CommonDelegate:
     async def experimentalWaitOnCancelRequest(self) -> None:
         """This function is awaited in the time in between checking the status of a long running request.
         It provides a way to change how exactly the server waits and gives a way to improve the behaviour until a good soloutin is found which will be integrated into the library at which point this method might be removed.
         """
         await asyncio.sleep(1)
     
@@ -692,58 +735,62 @@
 
 
 class CGIServerDelegate(CommonDelegate):
     def HTTPHeader(self):
         return "Content-Type: application/json"
 
 
-class CommonCGIServer(CommonServer):
-    def _cgiserver_writeHeaders(self):
-        self.log.debug("writing header")
-        header = self.delegate.HTTPHeader()
-        print(header)
-        print()
-
-
-class CGIServer(CommonCGIServer):
+class CGIServer(CommonSyncServer):
     def __init__(self, delegate=None):
         super().__init__(delegate)
         self.log = logging.getLogger("CGIServer")
         self.log.debug("startet")
         if delegate == None:
             self.delegate = CGIServerDelegate()
         else:
             self.delegate = delegate
         self._cgiserver_writeHeaders()
         self._cgiserver_parseRequest()
 
+    def _cgiserver_writeHeaders(self):
+        self.log.debug("writing header")
+        header = self.delegate.HTTPHeader()
+        print(header)
+        print()
+
     def _cgiserver_parseRequest(self):
         self.log.debug("parsing request")
         try:
             raw = io.TextIOWrapper(sys.stdin.buffer, encoding='utf-8').read()
         except Exception as ex:
             self.log.exception(ex)
         try:
             print(self._processRequest(raw).stringify())
         except Exception as ex:
             self.log.exception(ex)
             raise ex
         exit(0)
 
 
-class AsyncCGIServer(CommonCGIServer):
+class AsyncCGIServer(CommonAsyncServer):
     def __init__(self, delegate=None):
         super().__init__(delegate)
         self.log = logging.getLogger("CGIServer")
         self.log.debug("startet")
         if delegate == None:
             self.delegate = CGIServerDelegate()
         else:
             self.delegate = delegate
         self._cgiserver_writeHeaders()
+
+    def _cgiserver_writeHeaders(self):
+        self.log.debug("writing header")
+        header = self.delegate.HTTPHeader()
+        print(header)
+        print()
     
     async def processRequests(self):
         self.log.debug("parsing request")
         try:
             raw = io.TextIOWrapper(sys.stdin.buffer, encoding='utf-8').read()
         except Exception as ex:
             self.log.exception(ex)
@@ -759,15 +806,15 @@
 
 
 class WSGIServerDelegate(CommonDelegate):
     def HTMLHeaders(self) -> List[str]:
         return [("Content-Type", "application/json")]
 
 
-class WSGIServer(CommonServer):
+class WSGIServer(CommonSyncServer):
     def __init__(self, *, delegate: WSGIServerDelegate=None):
         super().__init__(delegate)
         self.log = logging.getLogger("WSGIServer")
         self.log.debug("started")
         if delegate is None:
             self.delegate = WSGIServerDelegate()
         else:
@@ -790,15 +837,15 @@
         return iter([data])
 
 
 class ASGIServerDelegate(CommonDelegate):
     pass
 
 
-class ASGIServer(CommonServer):
+class ASGIServer(CommonAsyncServer):
     def __init__(self, *, delegate: ASGIServerDelegate=None):
         super().__init__(delegate)
         self.log = logging.getLogger("WSGIServer")
         self.log.debug("started")
         if delegate is None:
             self.delegate = ASGIServerDelegate()
         else:
@@ -827,13 +874,15 @@
                 [b'content-type', b'application/json'],
             ],
         })
         body = await read_body(receive)
         rpcRequest = body.decode("utf-8")
         print(rpcRequest)
         
-        rpcResult = await self._async_processRequest(rpcRequest)
-        await send({
-            'type': 'http.response.body',
-            'body': rpcResult.stringify().encode("utf-8")
-        })
+        rpcResult = await self._async_processRequest(rpcRequest, send)
+        # RPC Result is None if the response is a stream the response will already have been sent in that caase
+        if rpcResult is not None:
+            await send({
+                'type': 'http.response.body',
+                'body': rpcResult.stringify().encode("utf-8")
+            })
```

## Comparing `jsonrpcx-3.3.1.dist-info/LICENCE` & `jsonrpcx-4.0.0.dist-info/LICENCE`

 * *Files identical despite different names*

## Comparing `jsonrpcx-3.3.1.dist-info/METADATA` & `jsonrpcx-4.0.0.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonrpcx
-Version: 3.3.1
+Version: 4.0.0
 Summary: A battle tested Python JSON-RPC2.0 library supporting client and server code in sync and async fashion.
 Home-page: https://codeberg.org/_laphilipa/jsonrpcx
 License: ISC
 Keywords: JSON,jsonrpc,rpc
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
@@ -29,14 +29,15 @@
 
 # Overview
 
 A JSON-RPC 2.0 implementation.
 
 Features:
 - **Experimental support for request canceling with `rpc.cancel(id)` in async servers**
+- **Experimental support for response streaming in async servers**
 - Supports calling JSON-RCP 2.0 servers
 - Build a JSON-RPC server using ASGI, WSGI and CGI
 - Optionally supports async client and server code
 - Use the JSON-RPC 2.0 with any transport layer by using building blocks
 - Battle tested code because it was alreay used ~10 years in varioius closed source projects
 - Unittests are written for new code and whenever a bug is fixed for older parts
 - Abstracts handling of datetime.datetime() over the RPC
@@ -370,28 +371,68 @@
         super.experimentalAddRunningRequest(messageId, task)
 
     async def experimentalRemoveRunningRequest(self, messageId: Any) -> None:
         super.experimentalRemoveRunningRequest(messageID)
 
 ```
 
+# Experimental support for response streaming
+
+There is currently no definition for how request canceling should be implemented in JSON-RPC 2.0.
+
+On the Server:
+```python
+from jsonrpcx import *
+
+class Service(ASGIServer, ExperimentalCancelRequestMixin):
+    async def streamedResponse(self):
+        # Any dict or list (json serializable) that is returned with the `yield` keyword will be streamed to the client
+        for i in range(10):
+            yield {"res": f"test {i=}"}
+            await asyncio.sleep(5)
+
+```
+
+On the client:
+```python
+import httpx
+import asyncio
+
+async def main():
+    client = httpx.AsyncClient()
+    async with client.stream('POST', 'http://127.0.0.1:8000', timeout=5000, json={
+        "jsonrpc": "2.0",
+        "method": "streamedResponse",
+        "params": [],
+        "id": 1
+    }) as response:
+        async for chunk in response.aiter_bytes():
+            print(chunk)
+            
+            
+if __name__ == '__main__':
+    asyncio.run(main())
+```
+
+
+
 # Setup development
 
 Run `pipenv install`
 
 # Testing
 Run `pipenv run pytest`
 
 # Running the Example server
 ```uvicorn exampleserver:app --reload```
 
 # Publish
 
 - `python3 setup.py bdist_wheel`
-- `twine upload dist/*`
+- `twine upload dist/* --skip-existing`
 # Improvement ideas
 
 - Instead of throwing CircularReference detected when what is returned from a function can not be serialized by json send a JSON serialization exception.
 - Add middle wear support
 - Add authentication middlewear
 - Add stream support for websockets
 - Improve secutiry problem with rpc.cancel (currently anyone can cancel any request as long as they know the messageId)
```

