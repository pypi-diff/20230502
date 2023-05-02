# Comparing `tmp/sse-starlette-1.3.4.tar.gz` & `tmp/sse-starlette-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sse-starlette-1.3.4.tar", last modified: Wed Apr 19 04:06:33 2023, max compression
+gzip compressed data, was "sse-starlette-1.4.0.tar", last modified: Tue May  2 20:23:11 2023, max compression
```

## Comparing `sse-starlette-1.3.4.tar` & `sse-starlette-1.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-19 04:06:33.118712 sse-starlette-1.3.4/
--rw-r--r--   0 Q187392    (501) staff       (20)      395 2022-12-16 17:29:08.000000 sse-starlette-1.3.4/AUTHORS
--rw-r--r--   0 Q187392    (501) staff       (20)     1892 2023-03-11 18:12:47.000000 sse-starlette-1.3.4/CHANGELOG.md
--rw-r--r--   0 Q187392    (501) staff       (20)     1511 2022-12-16 17:29:08.000000 sse-starlette-1.3.4/LICENSE
--rw-r--r--   0 Q187392    (501) staff       (20)      103 2022-12-16 17:29:08.000000 sse-starlette-1.3.4/MANIFEST.in
--rw-r--r--   0 Q187392    (501) staff       (20)     5236 2023-04-19 04:06:33.118896 sse-starlette-1.3.4/PKG-INFO
--rw-r--r--   0 Q187392    (501) staff       (20)     3093 2023-03-11 18:06:25.000000 sse-starlette-1.3.4/README.md
--rw-r--r--   0 Q187392    (501) staff       (20)      106 2022-12-16 17:29:08.000000 sse-starlette-1.3.4/pyproject.toml
--rw-r--r--   0 Q187392    (501) staff       (20)     1800 2023-04-19 04:06:33.119660 sse-starlette-1.3.4/setup.cfg
--rw-r--r--   0 Q187392    (501) staff       (20)      152 2022-12-16 17:29:08.000000 sse-starlette-1.3.4/setup.py
-drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-19 04:06:33.114844 sse-starlette-1.3.4/sse_starlette/
--rw-r--r--   0 Q187392    (501) staff       (20)      143 2023-04-19 04:05:55.000000 sse-starlette-1.3.4/sse_starlette/__init__.py
--rw-r--r--   0 Q187392    (501) staff       (20)        0 2022-12-16 17:29:08.000000 sse-starlette-1.3.4/sse_starlette/py.typed
--rw-r--r--   0 Q187392    (501) staff       (20)    10462 2023-03-11 17:23:01.000000 sse-starlette-1.3.4/sse_starlette/sse.py
-drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-19 04:06:33.117523 sse-starlette-1.3.4/sse_starlette.egg-info/
--rw-r--r--   0 Q187392    (501) staff       (20)     5236 2023-04-19 04:06:32.000000 sse-starlette-1.3.4/sse_starlette.egg-info/PKG-INFO
--rw-r--r--   0 Q187392    (501) staff       (20)      392 2023-04-19 04:06:33.000000 sse-starlette-1.3.4/sse_starlette.egg-info/SOURCES.txt
--rw-r--r--   0 Q187392    (501) staff       (20)        1 2023-04-19 04:06:32.000000 sse-starlette-1.3.4/sse_starlette.egg-info/dependency_links.txt
--rw-r--r--   0 Q187392    (501) staff       (20)       10 2023-04-19 04:06:32.000000 sse-starlette-1.3.4/sse_starlette.egg-info/requires.txt
--rw-r--r--   0 Q187392    (501) staff       (20)       14 2023-04-19 04:06:32.000000 sse-starlette-1.3.4/sse_starlette.egg-info/top_level.txt
-drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-19 04:06:33.118417 sse-starlette-1.3.4/tests/
--rw-r--r--   0 Q187392    (501) staff       (20)     3675 2022-12-16 17:29:08.000000 sse-starlette-1.3.4/tests/test_event_source_response.py
--rw-r--r--   0 Q187392    (501) staff       (20)     2811 2022-12-16 17:29:08.000000 sse-starlette-1.3.4/tests/test_sse.py
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-05-02 20:23:11.623662 sse-starlette-1.4.0/
+-rw-r--r--   0 Q187392    (501) staff       (20)      395 2022-12-16 17:29:08.000000 sse-starlette-1.4.0/AUTHORS
+-rw-r--r--   0 Q187392    (501) staff       (20)     1892 2023-03-11 18:12:47.000000 sse-starlette-1.4.0/CHANGELOG.md
+-rw-r--r--   0 Q187392    (501) staff       (20)     1511 2022-12-16 17:29:08.000000 sse-starlette-1.4.0/LICENSE
+-rw-r--r--   0 Q187392    (501) staff       (20)      103 2022-12-16 17:29:08.000000 sse-starlette-1.4.0/MANIFEST.in
+-rw-r--r--   0 Q187392    (501) staff       (20)     5812 2023-05-02 20:23:11.623806 sse-starlette-1.4.0/PKG-INFO
+-rw-r--r--   0 Q187392    (501) staff       (20)     3669 2023-05-02 20:10:03.000000 sse-starlette-1.4.0/README.md
+-rw-r--r--   0 Q187392    (501) staff       (20)      106 2022-12-16 17:29:08.000000 sse-starlette-1.4.0/pyproject.toml
+-rw-r--r--   0 Q187392    (501) staff       (20)     1800 2023-05-02 20:23:11.675682 sse-starlette-1.4.0/setup.cfg
+-rw-r--r--   0 Q187392    (501) staff       (20)      152 2022-12-16 17:29:08.000000 sse-starlette-1.4.0/setup.py
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-05-02 20:23:11.616666 sse-starlette-1.4.0/sse_starlette/
+-rw-r--r--   0 Q187392    (501) staff       (20)      143 2023-05-02 20:19:39.000000 sse-starlette-1.4.0/sse_starlette/__init__.py
+-rw-r--r--   0 Q187392    (501) staff       (20)        0 2022-12-16 17:29:08.000000 sse-starlette-1.4.0/sse_starlette/py.typed
+-rw-r--r--   0 Q187392    (501) staff       (20)    10461 2023-05-02 20:19:23.000000 sse-starlette-1.4.0/sse_starlette/sse.py
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-05-02 20:23:11.619242 sse-starlette-1.4.0/sse_starlette.egg-info/
+-rw-r--r--   0 Q187392    (501) staff       (20)     5812 2023-05-02 20:23:10.000000 sse-starlette-1.4.0/sse_starlette.egg-info/PKG-INFO
+-rw-r--r--   0 Q187392    (501) staff       (20)      392 2023-05-02 20:23:11.000000 sse-starlette-1.4.0/sse_starlette.egg-info/SOURCES.txt
+-rw-r--r--   0 Q187392    (501) staff       (20)        1 2023-05-02 20:23:10.000000 sse-starlette-1.4.0/sse_starlette.egg-info/dependency_links.txt
+-rw-r--r--   0 Q187392    (501) staff       (20)       10 2023-05-02 20:23:10.000000 sse-starlette-1.4.0/sse_starlette.egg-info/requires.txt
+-rw-r--r--   0 Q187392    (501) staff       (20)       14 2023-05-02 20:23:10.000000 sse-starlette-1.4.0/sse_starlette.egg-info/top_level.txt
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-05-02 20:23:11.622740 sse-starlette-1.4.0/tests/
+-rw-r--r--   0 Q187392    (501) staff       (20)     3675 2023-05-02 20:07:36.000000 sse-starlette-1.4.0/tests/test_event_source_response.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     3028 2023-05-02 20:19:23.000000 sse-starlette-1.4.0/tests/test_sse.py
```

### Comparing `sse-starlette-1.3.4/CHANGELOG.md` & `sse-starlette-1.4.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `sse-starlette-1.3.4/LICENSE` & `sse-starlette-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sse-starlette-1.3.4/PKG-INFO` & `sse-starlette-1.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sse-starlette
-Version: 1.3.4
+Version: 1.4.0
 Summary: "SSE plugin for Starlette"
 Home-page: https://github.com/sysid/sse-starlette
 Author: sysid
 Author-email: sysid@gmx.de
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -82,22 +82,40 @@
           _log.info(f"Disconnected from client (via refresh/close) {req.client}")
           # Do any other cleanup, if any
           raise e
     return EventSourceResponse(event_publisher())
 ```
 
 ## Special use cases
+### Customize Ping
+By default, the server sends a ping every 15 seconds. You can customize this by: 
+1. setting the `ping` parameter
+2. by changing the `ping` event to a comment event so that it is not visible to the client
+```python
+@router.get("")
+async def handle():
+    generator = numbers(1, 100)
+    return EventSourceResponse(
+        generator,
+        headers={"Server": "nini"},
+        ping=5,
+        ping_message_factory=lambda: ServerSentEvent(**{"comment": "You can't see\r\nthis ping"}),
+    )
+```
+
 ### Fan out Proxies
 Fan out proxies usually rely on response being cacheable. To support that, you can set the value of `Cache-Control`.
 For example:
 ```python
 return EventSourceResponse(
         generator(), headers={"Cache-Control": "public, max-age=29"}
     )
 ```
+### Error Handling
+See example: `examples/error_handling.py`
 
 
 ## Development, Contributing
 Check `Makefile` for available commands and development support, e.g. run the unit tests:
 ```python
 make test
 ```
```

### Comparing `sse-starlette-1.3.4/README.md` & `sse-starlette-1.4.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -63,22 +63,40 @@
           _log.info(f"Disconnected from client (via refresh/close) {req.client}")
           # Do any other cleanup, if any
           raise e
     return EventSourceResponse(event_publisher())
 ```
 
 ## Special use cases
+### Customize Ping
+By default, the server sends a ping every 15 seconds. You can customize this by: 
+1. setting the `ping` parameter
+2. by changing the `ping` event to a comment event so that it is not visible to the client
+```python
+@router.get("")
+async def handle():
+    generator = numbers(1, 100)
+    return EventSourceResponse(
+        generator,
+        headers={"Server": "nini"},
+        ping=5,
+        ping_message_factory=lambda: ServerSentEvent(**{"comment": "You can't see\r\nthis ping"}),
+    )
+```
+
 ### Fan out Proxies
 Fan out proxies usually rely on response being cacheable. To support that, you can set the value of `Cache-Control`.
 For example:
 ```python
 return EventSourceResponse(
         generator(), headers={"Cache-Control": "public, max-age=29"}
     )
 ```
+### Error Handling
+See example: `examples/error_handling.py`
 
 
 ## Development, Contributing
 Check `Makefile` for available commands and development support, e.g. run the unit tests:
 ```python
 make test
 ```
```

### Comparing `sse-starlette-1.3.4/setup.cfg` & `sse-starlette-1.4.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sse-starlette
-version = 1.3.4
+version = 1.4.0
 description = "SSE plugin for Starlette"
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 author = sysid
 author_email = sysid@gmx.de
 url = https://github.com/sysid/sse-starlette
 classifiers =
```

### Comparing `sse-starlette-1.3.4/sse_starlette/sse.py` & `sse-starlette-1.4.0/sse_starlette/sse.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,27 +93,27 @@
 
     def encode(self) -> bytes:
         buffer = io.StringIO()
         if self.comment is not None:
             for chunk in self.LINE_SEP_EXPR.split(str(self.comment)):
                 buffer.write(f": {chunk}")
                 buffer.write(self._sep)
-            return buffer.getvalue().encode("utf-8")
 
         if self.id is not None:
             buffer.write(self.LINE_SEP_EXPR.sub("", f"id: {self.id}"))
             buffer.write(self._sep)
 
         if self.event is not None:
             buffer.write(self.LINE_SEP_EXPR.sub("", f"event: {self.event}"))
             buffer.write(self._sep)
 
-        for chunk in self.LINE_SEP_EXPR.split(str(self.data)):
-            buffer.write(f"data: {chunk}")
-            buffer.write(self._sep)
+        if self.data is not None:
+            for chunk in self.LINE_SEP_EXPR.split(str(self.data)):
+                buffer.write(f"data: {chunk}")
+                buffer.write(self._sep)
 
         if self.retry is not None:
             if not isinstance(self.retry, int):
                 raise TypeError("retry argument must be int")
             buffer.write(f"retry: {self.retry}")
             buffer.write(self._sep)
 
@@ -268,13 +268,13 @@
         # Alternatively one can send periodically a comment line
         # (one starting with a ':' character)
         while self.active:
             await anyio.sleep(self._ping_interval)
             if self.ping_message_factory:
                 assert isinstance(self.ping_message_factory, Callable)  # type: ignore  # https://github.com/python/mypy/issues/6864
             ping = (
-                ServerSentEvent(datetime.utcnow(), event="ping").encode()
+                ServerSentEvent(comment=f"ping - {datetime.utcnow()}").encode()
                 if self.ping_message_factory is None
                 else ensure_bytes(self.ping_message_factory())
             )
             _log.debug(f"ping: {ping.decode()}")
             await send({"type": "http.response.body", "body": ping, "more_body": True})
```

### Comparing `sse-starlette-1.3.4/sse_starlette.egg-info/PKG-INFO` & `sse-starlette-1.4.0/sse_starlette.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sse-starlette
-Version: 1.3.4
+Version: 1.4.0
 Summary: "SSE plugin for Starlette"
 Home-page: https://github.com/sysid/sse-starlette
 Author: sysid
 Author-email: sysid@gmx.de
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -82,22 +82,40 @@
           _log.info(f"Disconnected from client (via refresh/close) {req.client}")
           # Do any other cleanup, if any
           raise e
     return EventSourceResponse(event_publisher())
 ```
 
 ## Special use cases
+### Customize Ping
+By default, the server sends a ping every 15 seconds. You can customize this by: 
+1. setting the `ping` parameter
+2. by changing the `ping` event to a comment event so that it is not visible to the client
+```python
+@router.get("")
+async def handle():
+    generator = numbers(1, 100)
+    return EventSourceResponse(
+        generator,
+        headers={"Server": "nini"},
+        ping=5,
+        ping_message_factory=lambda: ServerSentEvent(**{"comment": "You can't see\r\nthis ping"}),
+    )
+```
+
 ### Fan out Proxies
 Fan out proxies usually rely on response being cacheable. To support that, you can set the value of `Cache-Control`.
 For example:
 ```python
 return EventSourceResponse(
         generator(), headers={"Cache-Control": "public, max-age=29"}
     )
 ```
+### Error Handling
+See example: `examples/error_handling.py`
 
 
 ## Development, Contributing
 Check `Makefile` for available commands and development support, e.g. run the unit tests:
 ```python
 make test
 ```
```

### Comparing `sse-starlette-1.3.4/tests/test_event_source_response.py` & `sse-starlette-1.4.0/tests/test_event_source_response.py`

 * *Files identical despite different names*

### Comparing `sse-starlette-1.3.4/tests/test_sse.py` & `sse-starlette-1.4.0/tests/test_sse.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,22 @@
             dict(data="foo", event="bar", id="xyz"),
             b"id: xyz\r\nevent: bar\r\ndata: foo\r\n\r\n",
         ),
         (
             dict(data="foo", event="bar", id="xyz", retry=1),
             b"id: xyz\r\nevent: bar\r\ndata: foo\r\nretry: 1\r\n\r\n",
         ),
+        (
+            dict(comment="a comment"),
+            b": a comment\r\n\r\n",
+        ),
+        (
+            dict(data="foo", comment="a comment"),
+            b": a comment\r\ndata: foo\r\n\r\n",
+        ),
     ],
 )
 def test_server_sent_event(input, expected):
     print(input, expected)
     if isinstance(input, str):
         assert ServerSentEvent(input).encode() == expected
     else:
```

