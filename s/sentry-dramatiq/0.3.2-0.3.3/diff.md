# Comparing `tmp/sentry_dramatiq-0.3.2.tar.gz` & `tmp/sentry_dramatiq-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sentry_dramatiq-0.3.2.tar", last modified: Sun Apr 26 14:00:35 2020, max compression
+gzip compressed data, was "sentry_dramatiq-0.3.3.tar", last modified: Tue May  2 12:50:24 2023, max compression
```

## Comparing `sentry_dramatiq-0.3.2.tar` & `sentry_dramatiq-0.3.3.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 ramonsaraiva   (501) staff       (20)        0 2020-04-26 14:00:35.000000 sentry_dramatiq-0.3.2/
--rw-r--r--   0 ramonsaraiva   (501) staff       (20)     2745 2020-04-26 14:00:35.000000 sentry_dramatiq-0.3.2/PKG-INFO
--rw-r--r--   0 ramonsaraiva   (501) staff       (20)     1678 2020-04-25 13:39:55.000000 sentry_dramatiq-0.3.2/README.md
-drwxr-xr-x   0 ramonsaraiva   (501) staff       (20)        0 2020-04-26 14:00:35.000000 sentry_dramatiq-0.3.2/sentry_dramatiq/
--rw-r--r--   0 ramonsaraiva   (501) staff       (20)     5030 2020-04-26 13:58:55.000000 sentry_dramatiq-0.3.2/sentry_dramatiq/__init__.py
-drwxr-xr-x   0 ramonsaraiva   (501) staff       (20)        0 2020-04-26 14:00:35.000000 sentry_dramatiq-0.3.2/sentry_dramatiq.egg-info/
--rw-r--r--   0 ramonsaraiva   (501) staff       (20)     2745 2020-04-26 14:00:34.000000 sentry_dramatiq-0.3.2/sentry_dramatiq.egg-info/PKG-INFO
--rw-r--r--   0 ramonsaraiva   (501) staff       (20)      240 2020-04-26 14:00:34.000000 sentry_dramatiq-0.3.2/sentry_dramatiq.egg-info/SOURCES.txt
--rw-r--r--   0 ramonsaraiva   (501) staff       (20)        1 2020-04-26 14:00:34.000000 sentry_dramatiq-0.3.2/sentry_dramatiq.egg-info/dependency_links.txt
--rw-r--r--   0 ramonsaraiva   (501) staff       (20)       57 2020-04-26 14:00:34.000000 sentry_dramatiq-0.3.2/sentry_dramatiq.egg-info/requires.txt
--rw-r--r--   0 ramonsaraiva   (501) staff       (20)       16 2020-04-26 14:00:34.000000 sentry_dramatiq-0.3.2/sentry_dramatiq.egg-info/top_level.txt
--rw-r--r--   0 ramonsaraiva   (501) staff       (20)       38 2020-04-26 14:00:35.000000 sentry_dramatiq-0.3.2/setup.cfg
--rw-r--r--   0 ramonsaraiva   (501) staff       (20)     1240 2020-04-26 13:59:00.000000 sentry_dramatiq-0.3.2/setup.py
+drwxr-xr-x   0 ramonsaraiva   (501) staff       (20)        0 2023-05-02 12:50:24.384672 sentry_dramatiq-0.3.3/
+-rw-r--r--   0 ramonsaraiva   (501) staff       (20)     1072 2023-05-02 12:46:16.000000 sentry_dramatiq-0.3.3/LICENSE
+-rw-r--r--   0 ramonsaraiva   (501) staff       (20)     2450 2023-05-02 12:50:24.384526 sentry_dramatiq-0.3.3/PKG-INFO
+-rw-r--r--   0 ramonsaraiva   (501) staff       (20)     1678 2023-05-02 12:46:16.000000 sentry_dramatiq-0.3.3/README.md
+drwxr-xr-x   0 ramonsaraiva   (501) staff       (20)        0 2023-05-02 12:50:24.383074 sentry_dramatiq-0.3.3/sentry_dramatiq/
+-rw-r--r--   0 ramonsaraiva   (501) staff       (20)     5358 2023-05-02 12:47:38.000000 sentry_dramatiq-0.3.3/sentry_dramatiq/__init__.py
+drwxr-xr-x   0 ramonsaraiva   (501) staff       (20)        0 2023-05-02 12:50:24.384086 sentry_dramatiq-0.3.3/sentry_dramatiq.egg-info/
+-rw-r--r--   0 ramonsaraiva   (501) staff       (20)     2450 2023-05-02 12:50:24.000000 sentry_dramatiq-0.3.3/sentry_dramatiq.egg-info/PKG-INFO
+-rw-r--r--   0 ramonsaraiva   (501) staff       (20)      267 2023-05-02 12:50:24.000000 sentry_dramatiq-0.3.3/sentry_dramatiq.egg-info/SOURCES.txt
+-rw-r--r--   0 ramonsaraiva   (501) staff       (20)        1 2023-05-02 12:50:24.000000 sentry_dramatiq-0.3.3/sentry_dramatiq.egg-info/dependency_links.txt
+-rw-r--r--   0 ramonsaraiva   (501) staff       (20)       68 2023-05-02 12:50:24.000000 sentry_dramatiq-0.3.3/sentry_dramatiq.egg-info/requires.txt
+-rw-r--r--   0 ramonsaraiva   (501) staff       (20)       16 2023-05-02 12:50:24.000000 sentry_dramatiq-0.3.3/sentry_dramatiq.egg-info/top_level.txt
+-rw-r--r--   0 ramonsaraiva   (501) staff       (20)       38 2023-05-02 12:50:24.384724 sentry_dramatiq-0.3.3/setup.cfg
+-rw-r--r--   0 ramonsaraiva   (501) staff       (20)     1266 2023-05-02 12:47:38.000000 sentry_dramatiq-0.3.3/setup.py
+drwxr-xr-x   0 ramonsaraiva   (501) staff       (20)        0 2023-05-02 12:50:24.384290 sentry_dramatiq-0.3.3/tests/
+-rw-r--r--   0 ramonsaraiva   (501) staff       (20)     5183 2023-05-02 12:47:38.000000 sentry_dramatiq-0.3.3/tests/test_base.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sentry_dramatiq-0.3.2/PKG-INFO` & `sentry_dramatiq-0.3.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,60 @@
 Metadata-Version: 2.1
 Name: sentry_dramatiq
-Version: 0.3.2
+Version: 0.3.3
 Summary: Dramatiq task processor integration for the Sentry SDK
 Home-page: https://github.com/jmagnusson/sentry-dramatiq
 Author: Jacob Magnusson
 Author-email: m@jacobian.se
 License: BSD
-Description: # sentry-dramatiq
-        
-        [![Travis CI build status (Linux)](https://travis-ci.org/jmagnusson/sentry-dramatiq.svg?branch=master)](https://travis-ci.org/jmagnusson/sentry-dramatiq)
-        [![PyPI version](https://img.shields.io/pypi/v/sentry-dramatiq.svg)](https://pypi.python.org/pypi/sentry-dramatiq/)
-        [![License](https://img.shields.io/pypi/l/sentry-dramatiq.svg)](https://pypi.python.org/pypi/sentry-dramatiq/)
-        [![Available as wheel](https://img.shields.io/pypi/wheel/sentry-dramatiq.svg)](https://pypi.python.org/pypi/sentry-dramatiq/)
-        [![Supported Python versions](https://img.shields.io/pypi/pyversions/sentry-dramatiq.svg)](https://pypi.python.org/pypi/sentry-dramatiq/)
-        [![PyPI status (alpha/beta/stable)](https://img.shields.io/pypi/status/sentry-dramatiq.svg)](https://pypi.python.org/pypi/sentry-dramatiq/)
-        [![Coverage Status](https://coveralls.io/repos/github/jmagnusson/sentry-dramatiq/badge.svg?branch=master)](https://coveralls.io/github/jmagnusson/sentry-dramatiq?branch=master)
-        
-        [Dramatiq task processor](https://dramatiq.io/) integration for the [Sentry SDK](https://docs.sentry.io/error-reporting/quickstart/?platform=python).
-        
-        ## Installation
-        
-        ```
-        pip install sentry-dramatiq
-        ```
-        
-        ## Setup
-        
-        ```python
-        import sentry_sdk
-        import sentry_dramatiq
-        
-        sentry_sdk.init(
-            '__DSN__',
-            integrations=[sentry_dramatiq.DramatiqIntegration()],
-        )
-        ```
-        
-        ## Features
-        
-        - Tags Sentry events with the message ID as `dramatiq_message_id`
-        - Adds all info about a Dramatiq message to a separate context (shows up as its own section in the Sentry UI)
-        
-        ## Known limitations
-        
-        - `sentry_sdk.init()` has to be called before broker is initialized as the integration monkey patches `Broker.__init__`
-        
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
+License-File: LICENSE
+
+# sentry-dramatiq
+
+[![Travis CI build status (Linux)](https://travis-ci.org/jmagnusson/sentry-dramatiq.svg?branch=master)](https://travis-ci.org/jmagnusson/sentry-dramatiq)
+[![PyPI version](https://img.shields.io/pypi/v/sentry-dramatiq.svg)](https://pypi.python.org/pypi/sentry-dramatiq/)
+[![License](https://img.shields.io/pypi/l/sentry-dramatiq.svg)](https://pypi.python.org/pypi/sentry-dramatiq/)
+[![Available as wheel](https://img.shields.io/pypi/wheel/sentry-dramatiq.svg)](https://pypi.python.org/pypi/sentry-dramatiq/)
+[![Supported Python versions](https://img.shields.io/pypi/pyversions/sentry-dramatiq.svg)](https://pypi.python.org/pypi/sentry-dramatiq/)
+[![PyPI status (alpha/beta/stable)](https://img.shields.io/pypi/status/sentry-dramatiq.svg)](https://pypi.python.org/pypi/sentry-dramatiq/)
+[![Coverage Status](https://coveralls.io/repos/github/jmagnusson/sentry-dramatiq/badge.svg?branch=master)](https://coveralls.io/github/jmagnusson/sentry-dramatiq?branch=master)
+
+[Dramatiq task processor](https://dramatiq.io/) integration for the [Sentry SDK](https://docs.sentry.io/error-reporting/quickstart/?platform=python).
+
+## Installation
+
+```
+pip install sentry-dramatiq
+```
+
+## Setup
+
+```python
+import sentry_sdk
+import sentry_dramatiq
+
+sentry_sdk.init(
+    '__DSN__',
+    integrations=[sentry_dramatiq.DramatiqIntegration()],
+)
+```
+
+## Features
+
+- Tags Sentry events with the message ID as `dramatiq_message_id`
+- Adds all info about a Dramatiq message to a separate context (shows up as its own section in the Sentry UI)
+
+## Known limitations
+
+- `sentry_sdk.init()` has to be called before broker is initialized as the integration monkey patches `Broker.__init__`
```

### Comparing `sentry_dramatiq-0.3.2/README.md` & `sentry_dramatiq-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `sentry_dramatiq-0.3.2/sentry_dramatiq/__init__.py` & `sentry_dramatiq-0.3.3/sentry_dramatiq/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import json
 from typing import Any, Callable, Dict, Optional, Union
 
 from dramatiq.broker import Broker
 from dramatiq.message import Message
 from dramatiq.middleware import Middleware, default_middleware
+from dramatiq.errors import Retry
 from sentry_sdk import Hub
 from sentry_sdk.integrations import Integration
 from sentry_sdk.utils import (
     AnnotatedValue,
     capture_internal_exceptions,
-    event_from_exception
+    event_from_exception,
 )
 
 
 class DramatiqIntegration(Integration):
     """Dramatiq integration for Sentry
 
     Please make sure that you call `sentry_sdk.init` *before* initializing
@@ -32,15 +33,15 @@
     original_broker__init__ = Broker.__init__
 
     def sentry_patched_broker__init__(self, *args, **kw):
         hub = Hub.current
         integration = hub.get_integration(DramatiqIntegration)
 
         try:
-            middleware = kw.pop('middleware')
+            middleware = kw.pop("middleware")
         except KeyError:
             # Unfortunately Broker and StubBroker allows middleware to be
             # passed in as positional arguments, whilst RabbitmqBroker and
             # RedisBroker does not.
             if len(args) > 0:
                 assert len(args) < 2
                 middleware = None if args[0] is None else args[0]
@@ -50,19 +51,20 @@
 
         if middleware is None:
             middleware = list(m() for m in default_middleware)
         else:
             middleware = list(middleware)
 
         if integration is not None:
-            assert SentryMiddleware not in (m.__class__ for m in middleware),\
-                "Sentry middleware must not be passed in manually to broker"
+            assert SentryMiddleware not in (
+                m.__class__ for m in middleware
+            ), "Sentry middleware must not be passed in manually to broker"
             middleware.insert(0, SentryMiddleware())
 
-        kw['middleware'] = middleware
+        kw["middleware"] = middleware
         # raise Exception([args, kw])
         original_broker__init__(self, *args, **kw)
 
     Broker.__init__ = sentry_patched_broker__init__
 
 
 class SentryMiddleware(Middleware):
@@ -80,28 +82,35 @@
             return
 
         message._scope_manager = hub.push_scope()
         message._scope_manager.__enter__()
 
         with hub.configure_scope() as scope:
             scope.transaction = message.actor_name
-            scope.set_tag('dramatiq_message_id', message.message_id)
+            scope.set_tag("dramatiq_message_id", message.message_id)
             scope.add_event_processor(
                 _make_message_event_processor(message, integration)
             )
 
     def after_process_message(self, broker, message, *, result=None, exception=None):
         hub = Hub.current
         integration = hub.get_integration(DramatiqIntegration)
 
         if integration is None:
             return
 
+        actor = broker.get_actor(message.actor_name)
+        throws = message.options.get("throws") or actor.options.get("throws")
+
         try:
-            if exception is not None:
+            if (
+                exception is not None
+                and not (throws and isinstance(exception, throws))
+                and not isinstance(exception, Retry)
+            ):
                 event, hint = event_from_exception(
                     exception,
                     client_options=hub.client.options,
                     mechanism={"type": "dramatiq", "handled": False},
                 )
                 hub.capture_event(event, hint=hint)
         finally:
@@ -137,21 +146,21 @@
             return
 
         data = None  # type: Optional[Union[AnnotatedValue, Dict[str, Any]]]
 
         content_length = self.content_length()
         contexts = event.setdefault("contexts", {})
         request_info = contexts.setdefault("dramatiq", {})
-        request_info['type'] = "dramatiq"
+        request_info["type"] = "dramatiq"
 
         bodies = client.options["request_bodies"]
         if (
             bodies == "never"
-            or (bodies == "small" and content_length > 10 ** 3)
-            or (bodies == "medium" and content_length > 10 ** 4)
+            or (bodies == "small" and content_length > 10**3)
+            or (bodies == "medium" and content_length > 10**4)
         ):
             data = AnnotatedValue(
                 "",
                 {"rem": [["!config", "x", 0, content_length]], "len": content_length},
             )
         else:
             data = self.message_data
```

### Comparing `sentry_dramatiq-0.3.2/sentry_dramatiq.egg-info/PKG-INFO` & `sentry_dramatiq-0.3.3/sentry_dramatiq.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,60 @@
 Metadata-Version: 2.1
 Name: sentry-dramatiq
-Version: 0.3.2
+Version: 0.3.3
 Summary: Dramatiq task processor integration for the Sentry SDK
 Home-page: https://github.com/jmagnusson/sentry-dramatiq
 Author: Jacob Magnusson
 Author-email: m@jacobian.se
 License: BSD
-Description: # sentry-dramatiq
-        
-        [![Travis CI build status (Linux)](https://travis-ci.org/jmagnusson/sentry-dramatiq.svg?branch=master)](https://travis-ci.org/jmagnusson/sentry-dramatiq)
-        [![PyPI version](https://img.shields.io/pypi/v/sentry-dramatiq.svg)](https://pypi.python.org/pypi/sentry-dramatiq/)
-        [![License](https://img.shields.io/pypi/l/sentry-dramatiq.svg)](https://pypi.python.org/pypi/sentry-dramatiq/)
-        [![Available as wheel](https://img.shields.io/pypi/wheel/sentry-dramatiq.svg)](https://pypi.python.org/pypi/sentry-dramatiq/)
-        [![Supported Python versions](https://img.shields.io/pypi/pyversions/sentry-dramatiq.svg)](https://pypi.python.org/pypi/sentry-dramatiq/)
-        [![PyPI status (alpha/beta/stable)](https://img.shields.io/pypi/status/sentry-dramatiq.svg)](https://pypi.python.org/pypi/sentry-dramatiq/)
-        [![Coverage Status](https://coveralls.io/repos/github/jmagnusson/sentry-dramatiq/badge.svg?branch=master)](https://coveralls.io/github/jmagnusson/sentry-dramatiq?branch=master)
-        
-        [Dramatiq task processor](https://dramatiq.io/) integration for the [Sentry SDK](https://docs.sentry.io/error-reporting/quickstart/?platform=python).
-        
-        ## Installation
-        
-        ```
-        pip install sentry-dramatiq
-        ```
-        
-        ## Setup
-        
-        ```python
-        import sentry_sdk
-        import sentry_dramatiq
-        
-        sentry_sdk.init(
-            '__DSN__',
-            integrations=[sentry_dramatiq.DramatiqIntegration()],
-        )
-        ```
-        
-        ## Features
-        
-        - Tags Sentry events with the message ID as `dramatiq_message_id`
-        - Adds all info about a Dramatiq message to a separate context (shows up as its own section in the Sentry UI)
-        
-        ## Known limitations
-        
-        - `sentry_sdk.init()` has to be called before broker is initialized as the integration monkey patches `Broker.__init__`
-        
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
+License-File: LICENSE
+
+# sentry-dramatiq
+
+[![Travis CI build status (Linux)](https://travis-ci.org/jmagnusson/sentry-dramatiq.svg?branch=master)](https://travis-ci.org/jmagnusson/sentry-dramatiq)
+[![PyPI version](https://img.shields.io/pypi/v/sentry-dramatiq.svg)](https://pypi.python.org/pypi/sentry-dramatiq/)
+[![License](https://img.shields.io/pypi/l/sentry-dramatiq.svg)](https://pypi.python.org/pypi/sentry-dramatiq/)
+[![Available as wheel](https://img.shields.io/pypi/wheel/sentry-dramatiq.svg)](https://pypi.python.org/pypi/sentry-dramatiq/)
+[![Supported Python versions](https://img.shields.io/pypi/pyversions/sentry-dramatiq.svg)](https://pypi.python.org/pypi/sentry-dramatiq/)
+[![PyPI status (alpha/beta/stable)](https://img.shields.io/pypi/status/sentry-dramatiq.svg)](https://pypi.python.org/pypi/sentry-dramatiq/)
+[![Coverage Status](https://coveralls.io/repos/github/jmagnusson/sentry-dramatiq/badge.svg?branch=master)](https://coveralls.io/github/jmagnusson/sentry-dramatiq?branch=master)
+
+[Dramatiq task processor](https://dramatiq.io/) integration for the [Sentry SDK](https://docs.sentry.io/error-reporting/quickstart/?platform=python).
+
+## Installation
+
+```
+pip install sentry-dramatiq
+```
+
+## Setup
+
+```python
+import sentry_sdk
+import sentry_dramatiq
+
+sentry_sdk.init(
+    '__DSN__',
+    integrations=[sentry_dramatiq.DramatiqIntegration()],
+)
+```
+
+## Features
+
+- Tags Sentry events with the message ID as `dramatiq_message_id`
+- Adds all info about a Dramatiq message to a separate context (shows up as its own section in the Sentry UI)
+
+## Known limitations
+
+- `sentry_sdk.init()` has to be called before broker is initialized as the integration monkey patches `Broker.__init__`
```

