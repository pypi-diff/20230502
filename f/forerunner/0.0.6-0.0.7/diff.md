# Comparing `tmp/forerunner-0.0.6.tar.gz` & `tmp/forerunner-0.0.7.tar.gz`

## Comparing `forerunner-0.0.6.tar` & `forerunner-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 forerunner-0.0.6/Makefile
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 forerunner-0.0.6/README.md
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 forerunner-0.0.6/src/forerunner/__init__.py
--rw-r--r--   0        0        0     5108 2020-02-02 00:00:00.000000 forerunner-0.0.6/src/forerunner/app.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 forerunner-0.0.6/src/forerunner/cli.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 forerunner-0.0.6/src/forerunner/console.py
--rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 forerunner-0.0.6/src/forerunner/module.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 forerunner-0.0.6/src/forerunner/utils.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 forerunner-0.0.6/src/forerunner/dependency/depends.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 forerunner-0.0.6/src/forerunner/dependency/utils.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 forerunner-0.0.6/src/forerunner/job/__init__.py
--rw-r--r--   0        0        0     7533 2020-02-02 00:00:00.000000 forerunner-0.0.6/src/forerunner/job/base.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 forerunner-0.0.6/src/forerunner/job/cron.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 forerunner-0.0.6/src/forerunner/job/sub.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 forerunner-0.0.6/src/forerunner/queue/__init__.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 forerunner-0.0.6/src/forerunner/queue/queue.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 forerunner-0.0.6/.gitignore
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 forerunner-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 forerunner-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 forerunner-0.0.7/Makefile
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 forerunner-0.0.7/README.md
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 forerunner-0.0.7/src/forerunner/__init__.py
+-rw-r--r--   0        0        0     6422 2020-02-02 00:00:00.000000 forerunner-0.0.7/src/forerunner/app.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 forerunner-0.0.7/src/forerunner/cli.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 forerunner-0.0.7/src/forerunner/console.py
+-rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 forerunner-0.0.7/src/forerunner/module.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 forerunner-0.0.7/src/forerunner/server.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 forerunner-0.0.7/src/forerunner/utils.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 forerunner-0.0.7/src/forerunner/dependency/depends.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 forerunner-0.0.7/src/forerunner/dependency/utils.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 forerunner-0.0.7/src/forerunner/job/__init__.py
+-rw-r--r--   0        0        0     8178 2020-02-02 00:00:00.000000 forerunner-0.0.7/src/forerunner/job/base.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 forerunner-0.0.7/src/forerunner/job/cron.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 forerunner-0.0.7/src/forerunner/job/sub.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 forerunner-0.0.7/src/forerunner/queue/__init__.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 forerunner-0.0.7/src/forerunner/queue/queue.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 forerunner-0.0.7/.gitignore
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 forerunner-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 forerunner-0.0.7/PKG-INFO
```

### Comparing `forerunner-0.0.6/src/forerunner/app.py` & `forerunner-0.0.7/src/forerunner/app.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 import asyncio
 import signal
 from inspect import iscoroutinefunction
 from typing import Callable, List, Literal
 
+import uvicorn
+from prometheus_client import make_asgi_app
 from structlog import get_logger
 
 from forerunner.job.sub import Sub
 from forerunner.queue.queue import BaseQueue
+from forerunner.server import MetricsServer
 
 from .job import Cron
 from .module import Module
 from .utils import init_module_jobs
 
 
 class App:
     def __init__(
         self,
         name: str = "app",
         *,
         modules: List[Module] = [],
         exception_callbacks: List[Callable] = [],
+        prometheus_enabled: bool = False,
     ):
         self.name = name
         self.modules = modules
         self.exception_callbacks = exception_callbacks
+        self.prometheus_enabled = prometheus_enabled
+
+        self._prometheus_asgi_server: MetricsServer | None = None
+        self._prometheus_asgi_task: asyncio.Task | None = None
 
         self.logger = get_logger(app=self.name)
         self.jobs = []
 
         for module in self.modules:
             module_jobs = init_module_jobs(
                 app_name=self.name,
@@ -106,27 +114,38 @@
             )
             self.jobs.append(job)
             return func
 
         return _sub_wrapper
 
     async def startup(self):
+        if self.prometheus_enabled:
+            self.logger.debug("Starting prometheus web server...")
+            asgi_app = make_asgi_app()
+            config = uvicorn.Config(asgi_app, port=8003)
+            self._prometheus_asgi_server = MetricsServer(config)
+            self._prometheus_asgi_app_task = asyncio.create_task(
+                self._prometheus_asgi_server.serve()
+            )
+            self.logger.debug("Started prometheus web server")
+
         self.logger.info("Starting...")
         if len(self.startup_funcs) > 0:
             self.logger.debug("Running startup funcs...")
             for func in self.startup_funcs:
                 await func() if iscoroutinefunction(func) else func()
 
     async def shutdown(self):
         self.logger.info("Shutting down...")
+
+        # Stop jobs
         for job in self.jobs:
             if job.is_stopped:
                 continue
             job.stop()
-
         self.logger.info("Waiting for Jobs to finish. (CTRL+C to force quit)")
         while not self._force_exit:
             if all([job.is_stopped for job in self.jobs]):
                 break
             await asyncio.sleep(0.1)
 
         if self._force_exit:
@@ -135,19 +154,28 @@
                 job.cancel()
 
         if len(self.shutdown_funcs) > 0:
             self.logger.debug("Running shutdown funcs...")
             for func in self.shutdown_funcs:
                 await func() if iscoroutinefunction(func) else func()
 
+        # Shutdown metrics webserver
+        if self.prometheus_enabled and self._prometheus_asgi_server is not None:
+            self.logger.debug("Stopping prometheus web server...")
+            self._prometheus_asgi_server.should_exit = True
+            try:
+                await asyncio.wait_for(self._prometheus_asgi_app_task, timeout=30)
+            except asyncio.TimeoutError:
+                self._prometheus_asgi_app_task.cancel()
+            self.logger.debug("Stopped prometheus webserver")
+
         self.logger.info("App has stopped")
 
     async def _main_loop(self):
         self.logger.info("Running...")
-        self._init_signal_handlers()
 
         for job in self.jobs:
             job.start()
 
         counter = 0
         while not self._should_exit:
             counter += 1
@@ -168,13 +196,14 @@
 
     def _init_signal_handlers(self):
         loop = asyncio.get_event_loop()
         for sig in [signal.SIGINT, signal.SIGTERM]:
             loop.add_signal_handler(sig, self._handle_exit, sig)
 
     async def _run(self):
+        self._init_signal_handlers()
         await self.startup()
         await self._main_loop()
         await self.shutdown()
 
     def run(self):
         asyncio.run(self._run())
```

### Comparing `forerunner-0.0.6/src/forerunner/module.py` & `forerunner-0.0.7/src/forerunner/module.py`

 * *Files identical despite different names*

### Comparing `forerunner-0.0.6/src/forerunner/utils.py` & `forerunner-0.0.7/src/forerunner/utils.py`

 * *Files identical despite different names*

### Comparing `forerunner-0.0.6/src/forerunner/dependency/depends.py` & `forerunner-0.0.7/src/forerunner/dependency/depends.py`

 * *Files identical despite different names*

### Comparing `forerunner-0.0.6/src/forerunner/dependency/utils.py` & `forerunner-0.0.7/src/forerunner/dependency/utils.py`

 * *Files identical despite different names*

### Comparing `forerunner-0.0.6/src/forerunner/job/base.py` & `forerunner-0.0.7/src/forerunner/job/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import asyncio
 import inspect
 from contextlib import AsyncExitStack
 from functools import cache
 from typing import Callable, Dict, List, Literal, cast
 
 import structlog
+from prometheus_client import Counter
 
 from forerunner.console import console
 from forerunner.dependency.depends import Depends
 from forerunner.dependency.utils import resolve_dependencies
 from forerunner.queue.queue import BasePayload, BaseQueue
 
 logger = structlog.get_logger()
@@ -41,14 +42,25 @@
         self._task: asyncio.Task | None = None
         self._worker_tasks: List[asyncio.Task] = []
         self._exception_callback_tasks: List[asyncio.Task] = []
         self._stop_task: asyncio.Task | None = None
 
         self._worker_sem = asyncio.BoundedSemaphore(self.n_workers)
 
+        self._prom_run_func_success_total = Counter(
+            name=f"{self.job_name}_func_success_total",
+            documentation="Number of successful wrapped function calls",
+            namespace=f"forerunner_{self.app_name}",
+        )
+        self._prom_run_func_failure_total = Counter(
+            name=f"{self.job_name}_func_failure_total",
+            documentation="Number of failed wrapped function calls",
+            namespace=f"forerunner_{self.app_name}",
+        )
+
     @property
     def is_stopped(self):
         return (
             self._task is None
             and self._stop_task is None
             and len(self._worker_tasks) == 0
             and len(self._exception_callback_tasks) == 0
@@ -88,15 +100,17 @@
             self._worker_tasks.remove(task)
 
         async def retry_func_wrapper(*args, **kwargs):
             n_attempt = 0
             while n_attempt <= self.n_retries:
                 try:
                     res = await self.func(*args, **kwargs)
+                    self._prom_run_func_success_total.inc()
                 except Exception:
+                    self._prom_run_func_failure_total.inc()
                     self.logger.error(
                         "Exception raised by wrapped func. Retrying...",
                         n_attempt=n_attempt,
                     )
                     console.print_exception()
 
                     n_attempt += 1
```

### Comparing `forerunner-0.0.6/src/forerunner/job/cron.py` & `forerunner-0.0.7/src/forerunner/job/cron.py`

 * *Files identical despite different names*

### Comparing `forerunner-0.0.6/src/forerunner/job/sub.py` & `forerunner-0.0.7/src/forerunner/job/sub.py`

 * *Files identical despite different names*

### Comparing `forerunner-0.0.6/src/forerunner/queue/queue.py` & `forerunner-0.0.7/src/forerunner/queue/queue.py`

 * *Files identical despite different names*

