# Comparing `tmp/durabletask-0.1.0a1.tar.gz` & `tmp/durabletask-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "durabletask-0.1.0a1.tar", last modified: Fri Apr 28 18:27:17 2023, max compression
+gzip compressed data, was "dist/durabletask-0.1.0a2.tar", last modified: Tue May  2 18:31:58 2023, max compression
```

## Comparing `durabletask-0.1.0a1.tar` & `durabletask-0.1.0a2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 deeagarwal  (1000) deeagarwal  (1000)        0 2023-04-28 18:27:17.129395 durabletask-0.1.0a1/
--rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)     1141 2023-04-19 19:02:05.000000 durabletask-0.1.0a1/LICENSE
--rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)    12935 2023-04-28 18:27:17.129395 durabletask-0.1.0a1/PKG-INFO
--rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)    10968 2023-04-25 08:33:49.000000 durabletask-0.1.0a1/README.md
-drwxr-xr-x   0 deeagarwal  (1000) deeagarwal  (1000)        0 2023-04-28 18:27:17.119395 durabletask-0.1.0a1/durabletask/
--rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)      139 2023-04-19 19:02:05.000000 durabletask-0.1.0a1/durabletask/__init__.py
--rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)     7943 2023-04-26 05:19:59.000000 durabletask-0.1.0a1/durabletask/client.py
-drwxr-xr-x   0 deeagarwal  (1000) deeagarwal  (1000)        0 2023-04-28 18:27:17.129395 durabletask-0.1.0a1/durabletask/internal/
--rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)        0 2023-04-19 19:02:05.000000 durabletask-0.1.0a1/durabletask/internal/__init__.py
--rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)     7253 2023-04-25 08:56:00.000000 durabletask-0.1.0a1/durabletask/internal/helpers.py
--rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)    21866 2023-04-19 19:02:05.000000 durabletask-0.1.0a1/durabletask/internal/orchestrator_service_pb2.py
--rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)    32567 2023-04-19 19:02:05.000000 durabletask-0.1.0a1/durabletask/internal/orchestrator_service_pb2_grpc.py
--rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)     3133 2023-04-25 08:43:01.000000 durabletask-0.1.0a1/durabletask/internal/shared.py
--rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)    12003 2023-04-26 05:12:44.000000 durabletask-0.1.0a1/durabletask/task.py
--rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)    35814 2023-04-26 05:04:21.000000 durabletask-0.1.0a1/durabletask/worker.py
-drwxr-xr-x   0 deeagarwal  (1000) deeagarwal  (1000)        0 2023-04-28 18:27:17.119395 durabletask-0.1.0a1/durabletask.egg-info/
--rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)    12935 2023-04-28 18:27:17.000000 durabletask-0.1.0a1/durabletask.egg-info/PKG-INFO
--rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)      603 2023-04-28 18:27:17.000000 durabletask-0.1.0a1/durabletask.egg-info/SOURCES.txt
--rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)        1 2023-04-28 18:27:17.000000 durabletask-0.1.0a1/durabletask.egg-info/dependency_links.txt
--rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)        7 2023-04-28 18:27:17.000000 durabletask-0.1.0a1/durabletask.egg-info/requires.txt
--rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)       12 2023-04-28 18:27:17.000000 durabletask-0.1.0a1/durabletask.egg-info/top_level.txt
--rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)     1060 2023-04-28 18:25:34.000000 durabletask-0.1.0a1/pyproject.toml
--rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)       38 2023-04-28 18:27:17.129395 durabletask-0.1.0a1/setup.cfg
--rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)      811 2023-04-28 18:25:23.000000 durabletask-0.1.0a1/setup.py
-drwxr-xr-x   0 deeagarwal  (1000) deeagarwal  (1000)        0 2023-04-28 18:27:17.129395 durabletask-0.1.0a1/tests/
--rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)     1730 2023-04-25 08:46:22.000000 durabletask-0.1.0a1/tests/test_activity_executor.py
--rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)     9257 2023-04-25 08:33:49.000000 durabletask-0.1.0a1/tests/test_orchestration_e2e.py
--rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)    34548 2023-04-25 08:33:49.000000 durabletask-0.1.0a1/tests/test_orchestration_executor.py
+drwxr-xr-x   0 deeagarwal  (1000) deeagarwal  (1000)        0 2023-05-02 18:31:58.000000 durabletask-0.1.0a2/
+-rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)     1141 2023-04-19 19:02:05.000000 durabletask-0.1.0a2/LICENSE
+-rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)    12935 2023-05-02 18:31:58.000000 durabletask-0.1.0a2/PKG-INFO
+-rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)    10968 2023-04-25 08:33:49.000000 durabletask-0.1.0a2/README.md
+drwxr-xr-x   0 deeagarwal  (1000) deeagarwal  (1000)        0 2023-05-02 18:31:58.000000 durabletask-0.1.0a2/durabletask/
+-rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)      139 2023-04-19 19:02:05.000000 durabletask-0.1.0a2/durabletask/__init__.py
+-rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)     8610 2023-05-02 18:24:37.000000 durabletask-0.1.0a2/durabletask/client.py
+drwxr-xr-x   0 deeagarwal  (1000) deeagarwal  (1000)        0 2023-05-02 18:31:58.000000 durabletask-0.1.0a2/durabletask/internal/
+-rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)        0 2023-04-19 19:02:05.000000 durabletask-0.1.0a2/durabletask/internal/__init__.py
+-rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)     7340 2023-05-02 18:24:37.000000 durabletask-0.1.0a2/durabletask/internal/helpers.py
+-rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)    21866 2023-04-19 19:02:05.000000 durabletask-0.1.0a2/durabletask/internal/orchestrator_service_pb2.py
+-rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)    32567 2023-04-19 19:02:05.000000 durabletask-0.1.0a2/durabletask/internal/orchestrator_service_pb2_grpc.py
+-rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)     3174 2023-05-02 18:24:37.000000 durabletask-0.1.0a2/durabletask/internal/shared.py
+-rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)    12471 2023-05-02 18:24:37.000000 durabletask-0.1.0a2/durabletask/task.py
+-rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)    37798 2023-05-02 18:24:43.000000 durabletask-0.1.0a2/durabletask/worker.py
+drwxr-xr-x   0 deeagarwal  (1000) deeagarwal  (1000)        0 2023-05-02 18:31:58.000000 durabletask-0.1.0a2/durabletask.egg-info/
+-rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)    12935 2023-05-02 18:31:58.000000 durabletask-0.1.0a2/durabletask.egg-info/PKG-INFO
+-rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)      603 2023-05-02 18:31:58.000000 durabletask-0.1.0a2/durabletask.egg-info/SOURCES.txt
+-rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)        1 2023-05-02 18:31:58.000000 durabletask-0.1.0a2/durabletask.egg-info/dependency_links.txt
+-rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)        7 2023-05-02 18:31:58.000000 durabletask-0.1.0a2/durabletask.egg-info/requires.txt
+-rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)       12 2023-05-02 18:31:58.000000 durabletask-0.1.0a2/durabletask.egg-info/top_level.txt
+-rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)     1060 2023-05-02 18:31:49.000000 durabletask-0.1.0a2/pyproject.toml
+-rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)       38 2023-05-02 18:31:58.000000 durabletask-0.1.0a2/setup.cfg
+-rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)      811 2023-05-02 18:31:37.000000 durabletask-0.1.0a2/setup.py
+drwxr-xr-x   0 deeagarwal  (1000) deeagarwal  (1000)        0 2023-05-02 18:31:58.000000 durabletask-0.1.0a2/tests/
+-rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)     1860 2023-05-02 18:24:37.000000 durabletask-0.1.0a2/tests/test_activity_executor.py
+-rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)    10831 2023-05-02 18:24:37.000000 durabletask-0.1.0a2/tests/test_orchestration_e2e.py
+-rw-r--r--   0 deeagarwal  (1000) deeagarwal  (1000)    36521 2023-05-02 18:24:37.000000 durabletask-0.1.0a2/tests/test_orchestration_executor.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `durabletask-0.1.0a1/LICENSE` & `durabletask-0.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `durabletask-0.1.0a1/PKG-INFO` & `durabletask-0.1.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: durabletask
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: A Durable Task Client SDK for Python
 Home-page: https://github.com/microsoft/durabletask-python
 Author: Chris Gillum
 Author-email: cgillum@microsoft.com
 License:     MIT License
         
             Copyright (c) Microsoft Corporation.
@@ -29,15 +29,15 @@
         
 Project-URL: repository, https://github.com/microsoft/durabletask-python
 Project-URL: changelog, https://github.com/microsoft/durabletask-python/blob/main/CHANGELOG.md
 Keywords: durable,task,workflow
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Durable Task Client SDK for Python
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![Build Validation](https://github.com/microsoft/durabletask-python/actions/workflows/pr-validation.yml/badge.svg)](https://github.com/microsoft/durabletask-python/actions/workflows/pr-validation.yml)
```

### Comparing `durabletask-0.1.0a1/README.md` & `durabletask-0.1.0a2/README.md`

 * *Files identical despite different names*

### Comparing `durabletask-0.1.0a1/durabletask/client.py` & `durabletask-0.1.0a2/durabletask/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,27 +93,27 @@
 
     def __init__(self, *,
                  host_address: Union[str, None] = None,
                  log_handler=None,
                  log_formatter: Union[logging.Formatter, None] = None):
         channel = shared.get_grpc_channel(host_address)
         self._stub = stubs.TaskHubSidecarServiceStub(channel)
-        self._logger = shared.get_logger(log_handler, log_formatter)
+        self._logger = shared.get_logger("client", log_handler, log_formatter)
 
     def schedule_new_orchestration(self, orchestrator: Union[task.Orchestrator[TInput, TOutput], str], *,
                                    input: Union[TInput, None] = None,
                                    instance_id: Union[str, None] = None,
                                    start_at: Union[datetime, None] = None) -> str:
 
         name = orchestrator if isinstance(orchestrator, str) else task.get_name(orchestrator)
 
         req = pb.CreateInstanceRequest(
             name=name,
             instanceId=instance_id if instance_id else uuid.uuid4().hex,
-            input=wrappers_pb2.StringValue(value=shared.to_json(input)) if input else None,
+            input=wrappers_pb2.StringValue(value=shared.to_json(input)) if input is not None else None,
             scheduledStartTimestamp=helpers.new_timestamp(start_at) if start_at else None,
             version=wrappers_pb2.StringValue(value=""))
 
         self._logger.info(f"Starting new '{name}' instance with ID = '{req.instanceId}'.")
         res: pb.CreateInstanceResponse = self._stub.StartInstance(req)
         return res.instanceId
 
@@ -140,15 +140,27 @@
     def wait_for_orchestration_completion(self, instance_id: str, *,
                                           fetch_payloads: bool = True,
                                           timeout: int = 60) -> Union[OrchestrationState, None]:
         req = pb.GetInstanceRequest(instanceId=instance_id, getInputsAndOutputs=fetch_payloads)
         try:
             self._logger.info(f"Waiting {timeout}s for instance '{instance_id}' to complete.")
             res: pb.GetInstanceResponse = self._stub.WaitForInstanceCompletion(req, timeout=timeout)
-            return new_orchestration_state(req.instanceId, res)
+            state = new_orchestration_state(req.instanceId, res)
+            if not state:
+                return None
+
+            if state.runtime_status == OrchestrationStatus.FAILED and state.failure_details is not None:
+                details = state.failure_details
+                self._logger.info(f"Instance '{instance_id}' failed: [{details.error_type}] {details.message}")
+            elif state.runtime_status == OrchestrationStatus.TERMINATED:
+                self._logger.info(f"Instance '{instance_id}' was terminated.")
+            elif state.runtime_status == OrchestrationStatus.COMPLETED:
+                self._logger.info(f"Instance '{instance_id}' completed.")
+
+            return state
         except grpc.RpcError as rpc_error:
             if rpc_error.code() == grpc.StatusCode.DEADLINE_EXCEEDED:  # type: ignore
                 # Replace gRPC error with the built-in TimeoutError
                 raise TimeoutError("Timed-out waiting for the orchestration to complete")
             else:
                 raise
```

### Comparing `durabletask-0.1.0a1/durabletask/internal/helpers.py` & `durabletask-0.1.0a2/durabletask/internal/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 
 import traceback
 from datetime import datetime
-from typing import Union
+from typing import List, Union
 
 from google.protobuf import timestamp_pb2, wrappers_pb2
 
 import durabletask.internal.orchestrator_service_pb2 as pb
 
 # TODO: The new_xxx_event methods are only used by test code and should be moved elsewhere
 
@@ -157,22 +157,21 @@
         return wrappers_pb2.StringValue(value=val)
 
 
 def new_complete_orchestration_action(
         id: int,
         status: pb.OrchestrationStatus,
         result: Union[str, None] = None,
-        failure_details: Union[pb.TaskFailureDetails, None] = None) -> pb.OrchestratorAction:
-
+        failure_details: Union[pb.TaskFailureDetails, None] = None,
+        carryover_events: Union[List[pb.HistoryEvent], None] = None) -> pb.OrchestratorAction:
     completeOrchestrationAction = pb.CompleteOrchestrationAction(
         orchestrationStatus=status,
         result=get_string_value(result),
-        failureDetails=failure_details)
-
-    # TODO: CarryoverEvents
+        failureDetails=failure_details,
+        carryoverEvents=carryover_events)
 
     return pb.OrchestratorAction(id=id, completeOrchestration=completeOrchestrationAction)
 
 
 def new_create_timer_action(id: int, fire_at: datetime) -> pb.OrchestratorAction:
     timestamp = timestamp_pb2.Timestamp()
     timestamp.FromDatetime(fire_at)
```

### Comparing `durabletask-0.1.0a1/durabletask/internal/orchestrator_service_pb2.py` & `durabletask-0.1.0a2/durabletask/internal/orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `durabletask-0.1.0a1/durabletask/internal/orchestrator_service_pb2_grpc.py` & `durabletask-0.1.0a2/durabletask/internal/orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `durabletask-0.1.0a1/durabletask/internal/shared.py` & `durabletask-0.1.0a2/durabletask/internal/shared.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,17 +22,18 @@
     if host_address is None:
         host_address = get_default_host_address()
     channel = grpc.insecure_channel(host_address)
     return channel
 
 
 def get_logger(
+        name_suffix: str,
         log_handler: Union[logging.Handler, None] = None,
         log_formatter: Union[logging.Formatter, None] = None) -> logging.Logger:
-    logger = logging.Logger("durabletask")
+    logger = logging.Logger(f"durabletask-{name_suffix}")
 
     # Add a default log handler if none is provided
     if log_handler is None:
         log_handler = logging.StreamHandler()
         log_handler.setLevel(logging.INFO)
     logger.handlers.append(log_handler)
```

### Comparing `durabletask-0.1.0a1/durabletask/task.py` & `durabletask-0.1.0a2/durabletask/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,14 +143,27 @@
         Returns
         -------
         Task[TOutput]
             A Durable Task that completes when the event is received.
         """
         pass
 
+    @abstractmethod
+    def continue_as_new(self, new_input: Any, *, save_events: bool = False) -> None:
+        """Continue the orchestration execution as a new instance.
+
+        Parameters
+        ----------
+        new_input : Any
+            The new input to use for the new orchestration instance.
+        save_events : bool
+            A flag indicating whether to add any unprocessed external events in the new orchestration history.
+        """
+        pass
+
 
 class FailureDetails:
     def __init__(self, message: str, error_type: str, stack_trace: Union[str, None]):
         self._message = message
         self._error_type = error_type
         self._stack_trace = stack_trace
```

### Comparing `durabletask-0.1.0a1/durabletask/worker.py` & `durabletask-0.1.0a2/durabletask/worker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 
 import concurrent.futures
 import logging
-from dataclasses import dataclass
 from datetime import datetime, timedelta
 from threading import Event, Thread
 from types import GeneratorType
 from typing import Any, Dict, Generator, List, Sequence, TypeVar, Union
 
 import grpc
 from google.protobuf import empty_pb2
@@ -25,16 +24,16 @@
 
 class _Registry:
 
     orchestrators: Dict[str, task.Orchestrator]
     activities: Dict[str, task.Activity]
 
     def __init__(self):
-        self.orchestrators = dict[str, task.Orchestrator]()
-        self.activities = dict[str, task.Activity]()
+        self.orchestrators = {}
+        self.activities = {}
 
     def add_orchestrator(self, fn: task.Orchestrator) -> str:
         if fn is None:
             raise ValueError('An orchestrator function argument is required.')
 
         name = task.get_name(fn)
         self.add_named_orchestrator(name, fn)
@@ -86,15 +85,15 @@
 
     def __init__(self, *,
                  host_address: Union[str, None] = None,
                  log_handler=None,
                  log_formatter: Union[logging.Formatter, None] = None):
         self._registry = _Registry()
         self._host_address = host_address if host_address else shared.get_default_host_address()
-        self._logger = shared.get_logger(log_handler, log_formatter)
+        self._logger = shared.get_logger("worker", log_handler, log_formatter)
         self._shutdown = Event()
         self._response_stream = None
         self._is_running = False
 
     def __enter__(self):
         return self
 
@@ -145,29 +144,29 @@
                             elif work_item.HasField('activityRequest'):
                                 executor.submit(self._execute_activity, work_item.activityRequest, stub)
                             else:
                                 self._logger.warning(f'Unexpected work item type: {request_type}')
 
                     except grpc.RpcError as rpc_error:
                         if rpc_error.code() == grpc.StatusCode.CANCELLED:  # type: ignore
-                            self._logger.warning(f'Disconnected from {self._host_address}')
+                            self._logger.info(f'Disconnected from {self._host_address}')
                         elif rpc_error.code() == grpc.StatusCode.UNAVAILABLE:  # type: ignore
                             self._logger.warning(
                                 f'The sidecar at address {self._host_address} is unavailable - will continue retrying')
                         else:
                             self._logger.warning(f'Unexpected error: {rpc_error}')
                     except Exception as ex:
                         self._logger.warning(f'Unexpected error: {ex}')
 
                     # CONSIDER: exponential backoff
                     self._shutdown.wait(5)
                 self._logger.info("No longer listening for work items")
                 return
 
-        self._logger.info(f"starting gRPC worker that connects to {self._host_address}")
+        self._logger.info(f"Starting gRPC worker that connects to {self._host_address}")
         self._runLoop = Thread(target=run_loop)
         self._runLoop.start()
         self._is_running = True
 
     def stop(self):
         """Stops the worker and waits for any pending work items to complete."""
         if not self._is_running:
@@ -216,37 +215,33 @@
         try:
             stub.CompleteActivityTask(res)
         except Exception as ex:
             self._logger.exception(
                 f"Failed to deliver activity response for '{req.name}#{req.taskId}' of orchestration ID '{instance_id}' to sidecar: {ex}")
 
 
-@dataclass
-class _ExternalEvent:
-    name: str
-    data: Any
-
-
 class _RuntimeOrchestrationContext(task.OrchestrationContext):
     _generator: Union[Generator[task.Task, Any, Any], None]
     _previous_task: Union[task.Task, None]
 
     def __init__(self, instance_id: str):
         self._generator = None
         self._is_replaying = True
         self._is_complete = False
         self._result = None
-        self._pending_actions = dict[int, pb.OrchestratorAction]()
-        self._pending_tasks = dict[int, task.CompletableTask]()
+        self._pending_actions = {}
+        self._pending_tasks = {}
         self._sequence_number = 0
         self._current_utc_datetime = datetime(1000, 1, 1)
         self._instance_id = instance_id
         self._completion_status: Union[pb.OrchestrationStatus, None] = None
-        self._received_events: Dict[str, List[_ExternalEvent]] = {}
+        self._received_events: Dict[str, List[Any]] = {}
         self._pending_events: Dict[str, List[task.CompletableTask]] = {}
+        self._new_input: Union[Any, None] = None
+        self._save_events = False
 
     def run(self, generator: Generator[task.Task, Any, Any]):
         self._generator = generator
         # TODO: Do something with this task
         task = next(generator)  # this starts the generator
         # TODO: Check if the task is null?
         self._previous_task = task
@@ -278,35 +273,69 @@
                         break
 
     def set_complete(self, result: Any, status: pb.OrchestrationStatus, is_result_encoded: bool = False):
         if self._is_complete:
             return
 
         self._is_complete = True
+        self._completion_status = status
+        self._pending_actions.clear()  # Cancel any pending actions
+
         self._result = result
         result_json: Union[str, None] = None
         if result is not None:
             result_json = result if is_result_encoded else shared.to_json(result)
         action = ph.new_complete_orchestration_action(
             self.next_sequence_number(), status, result_json)
         self._pending_actions[action.id] = action
 
     def set_failed(self, ex: Exception):
         if self._is_complete:
             return
 
         self._is_complete = True
         self._pending_actions.clear()  # Cancel any pending actions
+        self._completion_status = pb.ORCHESTRATION_STATUS_FAILED
+
         action = ph.new_complete_orchestration_action(
             self.next_sequence_number(), pb.ORCHESTRATION_STATUS_FAILED, None, ph.new_failure_details(ex)
         )
         self._pending_actions[action.id] = action
 
+    def set_continued_as_new(self, new_input: Any, save_events: bool):
+        if self._is_complete:
+            return
+
+        self._is_complete = True
+        self._pending_actions.clear()  # Cancel any pending actions
+        self._completion_status = pb.ORCHESTRATION_STATUS_CONTINUED_AS_NEW
+        self._new_input = new_input
+        self._save_events = save_events
+
     def get_actions(self) -> List[pb.OrchestratorAction]:
-        return list(self._pending_actions.values())
+        if self._completion_status == pb.ORCHESTRATION_STATUS_CONTINUED_AS_NEW:
+            # When continuing-as-new, we only return a single completion action.
+            carryover_events: Union[List[pb.HistoryEvent], None] = None
+            if self._save_events:
+                carryover_events = []
+                # We need to save the current set of pending events so that they can be
+                # replayed when the new instance starts.
+                for event_name, values in self._received_events.items():
+                    for event_value in values:
+                        encoded_value = shared.to_json(event_value) if event_value else None
+                        carryover_events.append(ph.new_event_raised_event(event_name, encoded_value))
+            action = ph.new_complete_orchestration_action(
+                self.next_sequence_number(),
+                pb.ORCHESTRATION_STATUS_CONTINUED_AS_NEW,
+                result=shared.to_json(self._new_input) if self._new_input is not None else None,
+                failure_details=None,
+                carryover_events=carryover_events)
+            return [action]
+        else:
+            return list(self._pending_actions.values())
 
     def next_sequence_number(self) -> int:
         self._sequence_number += 1
         return self._sequence_number
 
     @property
     def instance_id(self) -> str:
@@ -366,29 +395,35 @@
     def wait_for_external_event(self, name: str) -> task.Task:
         # Check to see if this event has already been received, in which case we
         # can return it immediately. Otherwise, record out intent to receive an
         # event with the given name so that we can resume the generator when it
         # arrives. If there are multiple events with the same name, we return
         # them in the order they were received.
         external_event_task = task.CompletableTask()
-        event_name = name.upper()
+        event_name = name.casefold()
         event_list = self._received_events.get(event_name, None)
         if event_list:
-            event = event_list.pop(0)
+            event_data = event_list.pop(0)
             if not event_list:
                 del self._received_events[event_name]
-            external_event_task.complete(event.data)
+            external_event_task.complete(event_data)
         else:
             task_list = self._pending_events.get(event_name, None)
             if not task_list:
                 task_list = []
                 self._pending_events[event_name] = task_list
             task_list.append(external_event_task)
         return external_event_task
 
+    def continue_as_new(self, new_input, *, save_events: bool = False) -> None:
+        if self._is_complete:
+            return
+
+        self.set_continued_as_new(new_input, save_events)
+
 
 class _OrchestrationExecutor:
     _generator: Union[task.Orchestrator, None]
 
     def __init__(self, registry: _Registry, logger: logging.Logger):
         self._registry = registry
         self._logger = logger
@@ -411,21 +446,24 @@
             # Get new actions by executing newly received events into the orchestrator function
             if self._logger.level <= logging.DEBUG:
                 summary = _get_new_event_summary(new_events)
                 self._logger.debug(f"{instance_id}: Processing {len(new_events)} new event(s): {summary}")
             ctx._is_replaying = False
             for new_event in new_events:
                 self.process_event(ctx, new_event)
-                if ctx._is_complete:
-                    break
+
         except Exception as ex:
             # Unhandled exceptions fail the orchestration
             ctx.set_failed(ex)
 
-        if ctx._completion_status:
+        if not ctx._is_complete:
+            task_count = len(ctx._pending_tasks)
+            event_count = len(ctx._pending_events)
+            self._logger.info(f"{instance_id}: Waiting for {task_count} task(s) and {event_count} event(s).")
+        elif ctx._completion_status and ctx._completion_status is not pb.ORCHESTRATION_STATUS_CONTINUED_AS_NEW:
             completion_status_str = pbh.get_orchestration_status_str(ctx._completion_status)
             self._logger.info(f"{instance_id}: Orchestration completed with status: {completion_status_str}")
 
         actions = ctx.get_actions()
         if self._logger.level <= logging.DEBUG:
             self._logger.debug(f"{instance_id}: Returning {len(actions)} action(s): {_get_action_summary(actions)}")
         return actions
@@ -566,17 +604,17 @@
                     return
                 sub_orch_task.fail(
                     f"Sub-orchestration task #{task_id} failed: {failedEvent.failureDetails.errorMessage}",
                     failedEvent.failureDetails)
                 ctx.resume()
             elif event.HasField("eventRaised"):
                 # event names are case-insensitive
-                event_name = event.eventRaised.name.upper()
+                event_name = event.eventRaised.name.casefold()
                 if not ctx.is_replaying:
-                    self._logger.info(f"Event raised: {event_name}")
+                    self._logger.info(f"{ctx.instance_id} Event raised: {event_name}")
                 task_list = ctx._pending_events.get(event_name, None)
                 decoded_result: Union[Any, None] = None
                 if task_list:
                     event_task = task_list.pop(0)
                     if not ph.is_empty(event.eventRaised.input):
                         decoded_result = shared.from_json(event.eventRaised.input.value)
                     event_task.complete(decoded_result)
@@ -587,15 +625,15 @@
                     # buffer the event
                     event_list = ctx._received_events.get(event_name, None)
                     if not event_list:
                         event_list = []
                         ctx._received_events[event_name] = event_list
                     if not ph.is_empty(event.eventRaised.input):
                         decoded_result = shared.from_json(event.eventRaised.input.value)
-                    event_list.append(_ExternalEvent(event.eventRaised.name, decoded_result))
+                    event_list.append(decoded_result)
                     if not ctx.is_replaying:
                         self._logger.info(f"{ctx.instance_id}: Event '{event_name}' has been buffered as there are no tasks waiting for it.")
             elif event.HasField("executionSuspended"):
                 if not self._is_suspended and not ctx.is_replaying:
                     self._logger.info(f"{ctx.instance_id}: Execution suspended.")
                 self._is_suspended = True
             elif event.HasField("executionResumed") and self._is_suspended:
@@ -694,29 +732,29 @@
 def _get_new_event_summary(new_events: Sequence[pb.HistoryEvent]) -> str:
     """Returns a summary of the new events that can be used for logging."""
     if not new_events:
         return "[]"
     elif len(new_events) == 1:
         return f"[{new_events[0].WhichOneof('eventType')}]"
     else:
-        counts = dict[str, int]()
+        counts = {}
         for event in new_events:
             event_type = event.WhichOneof('eventType')
             counts[event_type] = counts.get(event_type, 0) + 1
         return f"[{', '.join(f'{name}={count}' for name, count in counts.items())}]"
 
 
 def _get_action_summary(new_actions: Sequence[pb.OrchestratorAction]) -> str:
     """Returns a summary of the new actions that can be used for logging."""
     if not new_actions:
         return "[]"
     elif len(new_actions) == 1:
         return f"[{new_actions[0].WhichOneof('orchestratorActionType')}]"
     else:
-        counts = dict[str, int]()
+        counts = {}
         for action in new_actions:
             action_type = action.WhichOneof('orchestratorActionType')
             counts[action_type] = counts.get(action_type, 0) + 1
         return f"[{', '.join(f'{name}={count}' for name, count in counts.items())}]"
 
 
 def _is_suspendable(event: pb.HistoryEvent) -> bool:
```

### Comparing `durabletask-0.1.0a1/durabletask.egg-info/PKG-INFO` & `durabletask-0.1.0a2/durabletask.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: durabletask
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: A Durable Task Client SDK for Python
 Home-page: https://github.com/microsoft/durabletask-python
 Author: Chris Gillum
 Author-email: cgillum@microsoft.com
 License:     MIT License
         
             Copyright (c) Microsoft Corporation.
@@ -29,15 +29,15 @@
         
 Project-URL: repository, https://github.com/microsoft/durabletask-python
 Project-URL: changelog, https://github.com/microsoft/durabletask-python/blob/main/CHANGELOG.md
 Keywords: durable,task,workflow
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Durable Task Client SDK for Python
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![Build Validation](https://github.com/microsoft/durabletask-python/actions/workflows/pr-validation.yml/badge.svg)](https://github.com/microsoft/durabletask-python/actions/workflows/pr-validation.yml)
```

### Comparing `durabletask-0.1.0a1/durabletask.egg-info/SOURCES.txt` & `durabletask-0.1.0a2/durabletask.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `durabletask-0.1.0a1/pyproject.toml` & `durabletask-0.1.0a2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "durabletask"
-version = "0.1.0-alpha.1"
+version = "0.1.0-alpha.2"
 description = "A Durable Task Client SDK for Python"
 keywords = [
     "durable",
     "task",
     "workflow"
 ]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
 ]
-requires-python = ">=3.9"
+requires-python = ">=3.7"
 license = {file = "LICENSE"}
 readme = "README.md"
 dependencies = [
     "grpcio",
 ]
 
 [project.urls]
```

### Comparing `durabletask-0.1.0a1/setup.py` & `durabletask-0.1.0a2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="durabletask",
-    version="0.1.0-alpha.1",
+    version="0.1.0-alpha.2",
     author="Chris Gillum",
     author_email="cgillum@microsoft.com",
     description="Durable Task Framework for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/microsoft/durabletask-python",
     packages=setuptools.find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.9',
+    python_requires='>=3.7',
 )
```

### Comparing `durabletask-0.1.0a1/tests/test_activity_executor.py` & `durabletask-0.1.0a2/tests/test_activity_executor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 
 import json
+import logging
 from typing import Any, Tuple, Union
 
-import durabletask.internal.shared as shared
 from durabletask import task, worker
 
-TEST_LOGGER = shared.get_logger()
+logging.basicConfig(
+    format='%(asctime)s.%(msecs)03d %(name)s %(levelname)s: %(message)s',
+    datefmt='%Y-%m-%d %H:%M:%S',
+    level=logging.DEBUG)
+TEST_LOGGER = logging.getLogger("tests")
 TEST_INSTANCE_ID = 'abc123'
 TEST_TASK_ID = 42
 
 
 def test_activity_inputs():
     """Validates activity function input population"""
     def test_activity(ctx: task.ActivityContext, test_input: Any):
```

### Comparing `durabletask-0.1.0a1/tests/test_orchestration_e2e.py` & `durabletask-0.1.0a2/tests/test_orchestration_e2e.py`

 * *Files 4% similar despite different names*

```diff
@@ -228,7 +228,43 @@
         assert state.runtime_status == client.OrchestrationStatus.RUNNING
 
         task_hub_client.terminate_orchestration(id, output="some reason for termination")
         state = task_hub_client.wait_for_orchestration_completion(id, timeout=30)
         assert state is not None
         assert state.runtime_status == client.OrchestrationStatus.TERMINATED
         assert state.serialized_output == json.dumps("some reason for termination")
+
+
+def test_continue_as_new():
+    all_results = []
+
+    def orchestrator(ctx: task.OrchestrationContext, input: int):
+        result = yield ctx.wait_for_external_event("my_event")
+        if not ctx.is_replaying:
+            # NOTE: Real orchestrations should never interact with nonlocal variables like this.
+            nonlocal all_results
+            all_results.append(result)
+
+        if len(all_results) <= 4:
+            ctx.continue_as_new(max(all_results), save_events=True)
+        else:
+            return all_results
+
+    # Start a worker, which will connect to the sidecar in a background thread
+    with worker.TaskHubGrpcWorker() as w:
+        w.add_orchestrator(orchestrator)
+        w.start()
+
+        task_hub_client = client.TaskHubGrpcClient()
+        id = task_hub_client.schedule_new_orchestration(orchestrator, input=0)
+        task_hub_client.raise_orchestration_event(id, "my_event", data=1)
+        task_hub_client.raise_orchestration_event(id, "my_event", data=2)
+        task_hub_client.raise_orchestration_event(id, "my_event", data=3)
+        task_hub_client.raise_orchestration_event(id, "my_event", data=4)
+        task_hub_client.raise_orchestration_event(id, "my_event", data=5)
+
+        state = task_hub_client.wait_for_orchestration_completion(id, timeout=30)
+        assert state is not None
+        assert state.runtime_status == client.OrchestrationStatus.COMPLETED
+        assert state.serialized_output == json.dumps(all_results)
+        assert state.serialized_input == json.dumps(4)
+        assert all_results == [1, 2, 3, 4, 5]
```

### Comparing `durabletask-0.1.0a1/tests/test_orchestration_executor.py` & `durabletask-0.1.0a2/tests/test_orchestration_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 # Licensed under the MIT License.
 
 import json
 import logging
 from datetime import datetime, timedelta
 from typing import List
 
+import pytest
+
 import durabletask.internal.helpers as helpers
 import durabletask.internal.orchestrator_service_pb2 as pb
 from durabletask import task, worker
 
 logging.basicConfig(
     format='%(asctime)s.%(msecs)03d %(name)s %(levelname)s: %(message)s',
     datefmt='%Y-%m-%d %H:%M:%S',
@@ -581,14 +583,49 @@
     executor = worker._OrchestrationExecutor(registry, TEST_LOGGER)
     actions = executor.execute(TEST_INSTANCE_ID, old_events, new_events)
     complete_action = get_and_validate_single_complete_orchestration_action(actions)
     assert complete_action.orchestrationStatus == pb.ORCHESTRATION_STATUS_TERMINATED
     assert complete_action.result.value == json.dumps("terminated!")
 
 
+@pytest.mark.parametrize("save_events", [True, False])
+def test_continue_as_new(save_events: bool):
+    """Tests the behavior of the continue-as-new API"""
+    def orchestrator(ctx: task.OrchestrationContext, input: int):
+        yield ctx.create_timer(ctx.current_utc_datetime + timedelta(days=1))
+        ctx.continue_as_new(input + 1, save_events=save_events)
+
+    registry = worker._Registry()
+    orchestrator_name = registry.add_orchestrator(orchestrator)
+
+    old_events = [
+        helpers.new_orchestrator_started_event(),
+        helpers.new_execution_started_event(orchestrator_name, TEST_INSTANCE_ID, encoded_input="1"),
+        helpers.new_event_raised_event("my_event", encoded_input="42"),
+        helpers.new_event_raised_event("my_event", encoded_input="43"),
+        helpers.new_event_raised_event("my_event", encoded_input="44"),
+        helpers.new_timer_created_event(1, datetime.utcnow() + timedelta(days=1))]
+    new_events = [
+        helpers.new_timer_fired_event(1, datetime.utcnow() + timedelta(days=1))]
+
+    # Execute the orchestration. It should be in a running state waiting for the timer to fire
+    executor = worker._OrchestrationExecutor(registry, TEST_LOGGER)
+    actions = executor.execute(TEST_INSTANCE_ID, old_events, new_events)
+    complete_action = get_and_validate_single_complete_orchestration_action(actions)
+    assert complete_action.orchestrationStatus == pb.ORCHESTRATION_STATUS_CONTINUED_AS_NEW
+    assert complete_action.result.value == json.dumps(2)
+    assert len(complete_action.carryoverEvents) == (3 if save_events else 0)
+    for i in range(len(complete_action.carryoverEvents)):
+        event = complete_action.carryoverEvents[i]
+        assert type(event) is pb.HistoryEvent
+        assert event.HasField("eventRaised")
+        assert event.eventRaised.name.casefold() == "my_event".casefold()  # event names are case-insensitive
+        assert event.eventRaised.input.value == json.dumps(42 + i)
+
+
 def test_fan_out():
     """Tests that a fan-out pattern correctly schedules N tasks"""
     def hello(_, name: str):
         return f"Hello {name}!"
 
     def orchestrator(ctx: task.OrchestrationContext, count: int):
         tasks = []
```

