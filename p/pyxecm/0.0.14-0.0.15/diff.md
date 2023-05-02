# Comparing `tmp/pyxecm-0.0.14.tar.gz` & `tmp/pyxecm-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxecm-0.0.14.tar", last modified: Tue May  2 14:51:12 2023, max compression
+gzip compressed data, was "pyxecm-0.0.15.tar", last modified: Tue May  2 21:23:18 2023, max compression
```

## Comparing `pyxecm-0.0.14.tar` & `pyxecm-0.0.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:51:12.800557 pyxecm-0.0.14/
--rw-rw-rw-   0 root         (0) root         (0)    11360 2023-05-02 14:50:53.000000 pyxecm-0.0.14/LICENSE
--rw-r--r--   0 root         (0) root         (0)      870 2023-05-02 14:51:12.800557 pyxecm-0.0.14/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-05-02 14:50:53.000000 pyxecm-0.0.14/README.md
--rw-rw-rw-   0 root         (0) root         (0)      922 2023-05-02 14:51:02.000000 pyxecm-0.0.14/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:51:12.798557 pyxecm-0.0.14/pyxecm/
--rw-rw-rw-   0 root         (0) root         (0)      508 2023-05-02 14:50:53.000000 pyxecm-0.0.14/pyxecm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    28270 2023-05-02 14:50:53.000000 pyxecm-0.0.14/pyxecm/k8s.py
--rw-rw-rw-   0 root         (0) root         (0)    69124 2023-05-02 14:50:53.000000 pyxecm-0.0.14/pyxecm/m365.py
--rw-rw-rw-   0 root         (0) root         (0)    49931 2023-05-02 14:50:53.000000 pyxecm-0.0.14/pyxecm/main.py
--rw-rw-rw-   0 root         (0) root         (0)     3784 2023-05-02 14:50:53.000000 pyxecm-0.0.14/pyxecm/otac.py
--rw-rw-rw-   0 root         (0) root         (0)   219914 2023-05-02 14:50:53.000000 pyxecm-0.0.14/pyxecm/otcs.py
--rw-rw-rw-   0 root         (0) root         (0)   115012 2023-05-02 14:50:53.000000 pyxecm-0.0.14/pyxecm/otds.py
--rw-rw-rw-   0 root         (0) root         (0)     1586 2023-05-02 14:50:53.000000 pyxecm-0.0.14/pyxecm/otiv.py
--rw-rw-rw-   0 root         (0) root         (0)    10224 2023-05-02 14:50:53.000000 pyxecm-0.0.14/pyxecm/otpd.py
--rw-rw-rw-   0 root         (0) root         (0)   226140 2023-05-02 14:50:53.000000 pyxecm-0.0.14/pyxecm/payload.py
--rw-rw-rw-   0 root         (0) root         (0)     5987 2023-05-02 14:50:53.000000 pyxecm-0.0.14/pyxecm/sap.py
--rw-rw-rw-   0 root         (0) root         (0)     2394 2023-05-02 14:50:53.000000 pyxecm-0.0.14/pyxecm/translate.py
--rw-rw-rw-   0 root         (0) root         (0)     2695 2023-05-02 14:50:53.000000 pyxecm-0.0.14/pyxecm/web.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:51:12.799557 pyxecm-0.0.14/pyxecm.egg-info/
--rw-r--r--   0 root         (0) root         (0)      870 2023-05-02 14:51:12.000000 pyxecm-0.0.14/pyxecm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      394 2023-05-02 14:51:12.000000 pyxecm-0.0.14/pyxecm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 14:51:12.000000 pyxecm-0.0.14/pyxecm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-02 14:51:12.000000 pyxecm-0.0.14/pyxecm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-02 14:51:12.000000 pyxecm-0.0.14/pyxecm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-02 14:51:12.800557 pyxecm-0.0.14/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      418 2023-05-02 14:50:53.000000 pyxecm-0.0.14/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 21:23:18.970272 pyxecm-0.0.15/
+-rw-rw-rw-   0 root         (0) root         (0)    11360 2023-05-02 21:23:02.000000 pyxecm-0.0.15/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-05-02 21:23:18.969272 pyxecm-0.0.15/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      729 2023-05-02 21:23:02.000000 pyxecm-0.0.15/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      930 2023-05-02 21:23:08.000000 pyxecm-0.0.15/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 21:23:18.968272 pyxecm-0.0.15/pyxecm/
+-rw-rw-rw-   0 root         (0) root         (0)      508 2023-05-02 21:23:02.000000 pyxecm-0.0.15/pyxecm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    30519 2023-05-02 21:23:02.000000 pyxecm-0.0.15/pyxecm/k8s.py
+-rw-rw-rw-   0 root         (0) root         (0)    69124 2023-05-02 21:23:02.000000 pyxecm-0.0.15/pyxecm/m365.py
+-rw-rw-rw-   0 root         (0) root         (0)    49946 2023-05-02 21:23:02.000000 pyxecm-0.0.15/pyxecm/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     7463 2023-05-02 21:23:02.000000 pyxecm-0.0.15/pyxecm/otac.py
+-rw-rw-rw-   0 root         (0) root         (0)   216194 2023-05-02 21:23:02.000000 pyxecm-0.0.15/pyxecm/otcs.py
+-rw-rw-rw-   0 root         (0) root         (0)   113213 2023-05-02 21:23:02.000000 pyxecm-0.0.15/pyxecm/otds.py
+-rw-rw-rw-   0 root         (0) root         (0)     1586 2023-05-02 21:23:02.000000 pyxecm-0.0.15/pyxecm/otiv.py
+-rw-rw-rw-   0 root         (0) root         (0)    10224 2023-05-02 21:23:02.000000 pyxecm-0.0.15/pyxecm/otpd.py
+-rw-rw-rw-   0 root         (0) root         (0)   226245 2023-05-02 21:23:02.000000 pyxecm-0.0.15/pyxecm/payload.py
+-rw-rw-rw-   0 root         (0) root         (0)     5987 2023-05-02 21:23:02.000000 pyxecm-0.0.15/pyxecm/sap.py
+-rw-rw-rw-   0 root         (0) root         (0)     2394 2023-05-02 21:23:02.000000 pyxecm-0.0.15/pyxecm/translate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2695 2023-05-02 21:23:02.000000 pyxecm-0.0.15/pyxecm/web.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 21:23:18.969272 pyxecm-0.0.15/pyxecm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-05-02 21:23:18.000000 pyxecm-0.0.15/pyxecm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      394 2023-05-02 21:23:18.000000 pyxecm-0.0.15/pyxecm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 21:23:18.000000 pyxecm-0.0.15/pyxecm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       78 2023-05-02 21:23:18.000000 pyxecm-0.0.15/pyxecm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-02 21:23:18.000000 pyxecm-0.0.15/pyxecm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-02 21:23:18.970272 pyxecm-0.0.15/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      418 2023-05-02 21:23:02.000000 pyxecm-0.0.15/setup.py
```

### Comparing `pyxecm-0.0.14/LICENSE` & `pyxecm-0.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.14/pyproject.toml` & `pyxecm-0.0.15/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 
 [build-system]
   build-backend = "setuptools.build_meta"
   requires = ["setuptools >= 61.0"]
 
 [project]
   classifiers = ["Development Status :: 4 - Beta", "Programming Language :: Python :: 3", "License :: OSI Approved :: Apache Software License", "Operating System :: OS Independent", "Intended Audience :: Developers", "Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Content Management System"]
-  dependencies = ["requests < 3", "requests_toolbelt", "setuptools", "kubernetes", "python-hcl2", "zipfile36"]
+  dependencies = ["requests < 3", "requests_toolbelt", "setuptools", "kubernetes", "python-hcl2", "zipfile36", "suds"]
   description = "A library to connect to Opentext Extended ECM"
   name = "pyxecm"
   readme = "README.md"
   requires-python = ">=3.10"
-  version = "0.0.14"
+  version = "0.0.15"
 
   [[project.authors]]
     email = "kgatzweiler@opentext.com"
     name = "Kai Gatzweiler"
 
   [[project.authors]]
     email = "mdiefenb@opentext.com"
```

### Comparing `pyxecm-0.0.14/pyxecm/k8s.py` & `pyxecm-0.0.15/pyxecm/k8s.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Kubernetes Module to implement functions to read / write Kubernetes objects
 such as Pods, Stateful Sets, Config Maps, ...
 
+https://github.com/kubernetes-client/python 
 https://github.com/kubernetes-client/python/blob/master/kubernetes/README.md
 https://github.com/kubernetes-client/python/tree/master/examples
 
 Class: K8s
 Methods:
 
 __init__ : class initializer
@@ -97,259 +98,264 @@
 
     def getNetworkingV1Api(self):
         return self._networking_v1_api
 
     def getNamespace(self):
         return self._namespace
 
-    def getPod(self, podName: str):
+    def getPod(self, pod_name: str):
         """getPod: get a pod in the configured namespace (the namespace is defined in the class constructor).
         Args:
-            podName (string): name of the Kubernetes pod in the current namespace
+            pod_name (string): name of the Kubernetes pod in the current namespace
         Return: V1Pod (object):
                 api_version='v1',
                 kind='Pod',
                 metadata=V1ObjectMeta(...),
                 spec=V1PodSpec(...),
                 status=V1PodStatus(...)
         """
 
         try:
             response = self.getCoreV1Api().read_namespaced_pod(
-                name=podName, namespace=self.getNamespace()
+                name=pod_name, namespace=self.getNamespace()
             )
         except ApiException as e:
-            logger.error("Failed to get Pod -> {}; error -> {}".format(podName, str(e)))
+            logger.error("Failed to get Pod -> {}; error -> {}".format(pod_name, str(e)))
             return None
 
         return response
 
-    def listPods(self, fieldSelector: str = "", labelSelector: str = ""):
+    # end method definition
+
+    def listPods(self, field_selector: str = "", label_selector: str = ""):
         """listPods: list all Kubernetes pods in a given namespace. The list can be further restricted
                      by specifying a field or label selector.
         Args:
-            podName (string): name of the Kubernetes pod in the current namespace
-            conditionName (string): name of the condition, e.g. "Ready"
-        Return: V1PodList (object):
-                api_version: The Kubernetes API version.
-                items: A list of V1Pod objects, each representing a pod. You can access the fields of a
-                       V1Pod object using dot notation, for example, pod.metadata.name to access the name of the pod
-                kind: The Kubernetes object kind, which is always "PodList".
-                metadata: Additional metadata about the pod list, such as the resource version.
+            field_selector (string): filter result based on fields
+            label_selector (string): filter result based on labels
+        Return: V1PodList (object) or None if the call fails
+                Properties can be accessed with the "." notation (this is an object not a dict!):
+                - api_version: The Kubernetes API version.
+                - items: A list of V1Pod objects, each representing a pod. You can access the fields of a
+                        V1Pod object using dot notation, for example, pod.metadata.name to access the name of the pod
+                - kind: The Kubernetes object kind, which is always "PodList".
+                - metadata: Additional metadata about the pod list, such as the resource version.
         """
 
         try:
             response = self.getCoreV1Api().list_namespaced_pod(
-                field_selector=fieldSelector,
-                label_selector=labelSelector,
+                field_selector=field_selector,
+                label_selector=label_selector,
                 namespace=self.getNamespace(),
             )
         except ApiException as e:
             logger.error(
                 "Failed to list Pods with field_selector -> {} and label_selector -> {}; error -> {}".format(
-                    fieldSelector, labelSelector, str(e)
+                    field_selector, label_selector, str(e)
                 )
             )
             return None
 
         return response
 
-    def waitPodCondition(self, podName: str, conditionName: str):
+    # end method definition
+
+    def waitPodCondition(self, pod_name: str, condition_name: str):
         """waitPodCondition: wait for the pod to reach a defined condition (e.g. "Ready").
         Args:
-            podName (string): name of the Kubernetes pod in the current namespace
-            conditionName (string): name of the condition, e.g. "Ready"
+            pod_name (string): name of the Kubernetes pod in the current namespace
+            condition_name (string): name of the condition, e.g. "Ready"
         Return: True once the pod reaches the condition - otherwise wait forever
         """
 
         ready = False
         while not ready:
             try:
                 pod_status = self.getCoreV1Api().read_namespaced_pod_status(
-                    podName, self.getNamespace()
+                    pod_name, self.getNamespace()
                 )
 
                 # Check if the pod has reached the defined condition:
                 for cond in pod_status.status.conditions:
-                    if cond.type == conditionName and cond.status == "True":
+                    if cond.type == condition_name and cond.status == "True":
                         logger.info(
                             "Pod -> {} is in state -> {}!".format(
-                                podName, conditionName
+                                pod_name, condition_name
                             )
                         )
                         ready = True
                         break
                 else:
                     logger.info(
                         "Pod -> {} is not yet in state -> {}. Waiting...".format(
-                            podName, conditionName
+                            pod_name, condition_name
                         )
                     )
                     time.sleep(30)
                     continue
 
             except ApiException as e:
                 logger.error(
-                    "Failed to wait for pod -> {}; error -> {}".format(podName, str(e))
+                    "Failed to wait for pod -> {}; error -> {}".format(pod_name, str(e))
                 )
 
     # end method definition
 
-    def execPodCommand(self, podName: str, command: list):
+    def execPodCommand(self, pod_name: str, command: list):
         """execPodCommand: execute a command inside a Kubernetes pod (similar to kubectl exec on command line).
         Args:
-            podName (string): name of the Kubernetes pod in the current namespace
+            pod_name (string): name of the Kubernetes pod in the current namespace
             command (list): list of command and its parameters, e.g. ["/bin/bash", "-c", "pwd"]
                             The "-c" is required to make the shell executing the command.
         Return: response of the command or None if the call fails
         """
 
-        pod = self.getPod(podName)
+        pod = self.getPod(pod_name)
         if not pod:
-            logger.error("Pod -> {} does not exist".format(podName))
+            logger.error("Pod -> {} does not exist".format(pod_name))
 
         logger.info(
-            "Execute command -> {} in pod -> {}".format(command, podName))
+            "Execute command -> {} in pod -> {}".format(command, pod_name))
 
         try:
             response = stream(
                 self.getCoreV1Api().connect_get_namespaced_pod_exec,
-                podName,
+                pod_name,
                 self.getNamespace(),
                 command=command,
                 stderr=True,
                 stdin=False,
                 stdout=True,
                 tty=False,
             )
         except ApiException as e:
             logger.error(
                 "Failed to execute command -> {} in pod -> {}; error -> {}".format(
-                    command, podName, str(e)
+                    command, pod_name, str(e)
                 )
             )
             return None
 
         return response
 
     # end method definition
 
     # Some commands like the OTAC spawner need to run interactive - otherwise the command "hangs"
-    def execPodCommandInteractive(self, podName: str, commands: list, timeout: int = 30, writeStderrToErrorLog: bool = True):
+    def execPodCommandInteractive(self, pod_name: str, commands: list, timeout: int = 30, write_stderr_to_error_log: bool = True):
         """execPodCommandInteractive: execute a command inside a Kubernetes pod (similar to kubectl exec on command line).
                                       Other than execPodCommand() method above this is an interactive execution using
                                       stdin and reading the output from stdout and stderr. This is required for longer
                                       running commands. It is currently used for restarting the spawner of Archive Center.
                                       The output of the command is pushed into the logging.
         Args:
-            podName (string): name of the Kubernetes pod in the current namespace
+            pod_name (string): name of the Kubernetes pod in the current namespace
             commands (list): list of command and its parameters, e.g. ["/bin/bash", "/etc/init.d/spawner restart"]
                              Here we should NOT have a "-c" parameter!
             timeout (integer): timeout duration that is waited for any response. 
                                Each time a resonse is found in stdout or stderr we wait another timeout duration
                                to make sure we get the full output of the command.
-            writeStderrToErrorLog (boolean): flag to control if output in stderr should be written to info or error log stream.
-                                             Default is write to error log (True)
+            write_stderr_to_error_log (boolean): flag to control if output in stderr should be written to info or error log stream.
+                                                 Default is write to error log (True)
         Return: response of the connect_get_namespaced_pod_exec() or None if the call fails
         """
 
-        pod = self.getPod(podName)
+        pod = self.getPod(pod_name)
         if not pod:
-            logger.error("Pod -> {} does not exist".format(podName))
+            logger.error("Pod -> {} does not exist".format(pod_name))
 
         if not commands:
             return None
 
         # Get first command - this should be the shell:
         command = commands.pop(0)
 
         try:
             response = stream(
                 self.getCoreV1Api().connect_get_namespaced_pod_exec,
-                podName,
+                pod_name,
                 self.getNamespace(),
                 command=command,
                 stderr=True,
                 stdin=True,  # This is important!
                 stdout=True,
                 tty=False,
                 _preload_content=False  # This is important!
             )
         except ApiException as e:
             logger.error(
                 "Failed to execute command -> {} in pod -> {}; error -> {}".format(
-                    command, podName, str(e)
+                    command, pod_name, str(e)
                 )
             )
             return None
 
         while response.is_open():
             got_response = False
             response.update(timeout=timeout)
             if response.peek_stdout():
                 logger.info(response.read_stdout().replace("\n", " "))
                 got_response = True
             if response.peek_stderr():
-                if writeStderrToErrorLog:
+                if write_stderr_to_error_log:
                     logger.error(response.read_stderr().replace("\n", " "))
                 else:
                     logger.info(response.read_stderr().replace("\n", " "))
                 got_response = True
             if commands:
                 command = commands.pop(0)
                 logger.info(
-                    "Execute command -> {} in pod -> {}".format(command, podName))
+                    "Execute command -> {} in pod -> {}".format(command, pod_name))
                 response.write_stdin(command + "\n")
             else:
                 # We continue as long as we get some response during timeout period
                 if not got_response:
                     break
 
         response.close()
 
         return response
 
     # end method definition
 
-    def deletePod(self, podName: str):
+    def deletePod(self, pod_name: str):
         """deletePod: delete a pod in the configured namespace (the namespace is defined in the class constructor).
         Args:
-            podName (string): name of the Kubernetes pod in the current namespace
+            pod_name (string): name of the Kubernetes pod in the current namespace
         Return: V1Status (object):
                 api_version: The Kubernetes API version.
                 kind: The Kubernetes object kind, which is always "Status".
                 metadata: Additional metadata about the status object, such as the resource version.
                 status: The status of the operation, which is either "Success" or an error status.
                 message: A human-readable message explaining the status.
                 reason: A short string that describes the reason for the status.
                 code: An HTTP status code that corresponds to the status.
         """
 
-        pod = self.getPod(podName)
+        pod = self.getPod(pod_name)
         if not pod:
-            logger.error("Pod -> {} does not exist".format(podName))
+            logger.error("Pod -> {} does not exist".format(pod_name))
 
         try:
             response = self.getCoreV1Api().delete_namespaced_pod(
-                podName, namespace=self.getNamespace()
+                pod_name, namespace=self.getNamespace()
             )
         except ApiException as e:
             logger.error(
-                "Failed to delete Pod -> {}; error -> {}".format(podName, str(e))
+                "Failed to delete Pod -> {}; error -> {}".format(pod_name, str(e))
             )
             return None
 
         return response
 
     # end method definition
 
-    def getConfigMap(self, configMapName: str):
+    def getConfigMap(self, config_map_name: str):
         """getConfigMap: get a config map in the configured namespace (the namespace is defined in the class constructor).
         Args:
-            configMapName (string): name of the Kubernetes config map in the current namespace
+            config_map_name (string): name of the Kubernetes config map in the current namespace
         Return: V1ConfigMap (object) that includes these fields:
                 api_version: The Kubernetes API version.
                 metadata: A V1ObjectMeta object representing metadata about the V1ConfigMap object,
                           such as its name, labels, and annotations.
                 data: A dictionary containing the non-binary data stored in the ConfigMap,
                       where the keys represent the keys of the data items and the values represent
                       the values of the data items.
@@ -357,289 +363,328 @@
                              where the keys represent the keys of the binary data items and the values
                              represent the values of the binary data items. Binary data is encoded as base64
                              strings in the dictionary values.
         """
 
         try:
             response = self.getCoreV1Api().read_namespaced_config_map(
-                name=configMapName, namespace=self.getNamespace()
+                name=config_map_name, namespace=self.getNamespace()
             )
         except ApiException as e:
             logger.error("Failed to get Config Map -> {}; error -> {}".format(str(e)))
             return None
 
         return response
 
     # end method definition
 
-    def listConfigMaps(self, fieldSelector: str = "", labelSelector: str = ""):
+    def listConfigMaps(self, field_selector: str = "", label_selector: str = ""):
+        """listConfigMaps: lists all Kubernetes Config Maps in the current namespace.
+                           The list can be filtered by providing field selectors and
+                           label selectors.
+        Args:
+            field_selector (string): filter result based on fields
+            label_selector (string): filter result based on labels
+        Return: V1ConfigMapList (object) or None if the call fails
+                Properties can be accessed with the "." notation (this is an object not a dict!):
+                - api_version: The Kubernetes API version.
+                - items: A list of V1ConfigMap objects, each representing a config map. You can access the fields of a
+                        V1Pod object using dot notation, for example, cm.metadata.name to access the name of the config map
+                - kind: The Kubernetes object kind, which is always "ConfigMapList".
+                - metadata: Additional metadata about the config map list, such as the resource version.
+        """
+
         try:
             response = self.getCoreV1Api().list_namespaced_config_map(
-                field_selector=fieldSelector,
-                label_selector=labelSelector,
+                field_selector=field_selector,
+                label_selector=label_selector,
                 namespace=self.getNamespace(),
             )
         except ApiException as e:
             logger.error(
                 "Failed to list Config Maps with field_selector -> {} and label_selector -> {}; error -> {}".format(
-                    fieldSelector, labelSelector, str(e)
+                    field_selector, label_selector, str(e)
                 )
             )
             return None
 
         return response
 
     # end method definition
 
-    def findConfigMap(self, configMapName: str):
+    def findConfigMap(self, config_map_name: str):
         try:
             response = self.listConfigMaps(
-                fieldSelector="metadata.name={}".format(configMapName)
+                fieldSelector="metadata.name={}".format(config_map_name)
             )
         except ApiException as e:
             logger.error(
                 "Failed to find Config Map -> {}; error -> {}".format(
-                    configMapName, str(e)
+                    config_map_name, str(e)
                 )
             )
             return None
 
         return response
 
     # end method definition
 
-    def replaceConfigMap(self, configMapName: str, configMapData: dict):
+    def replaceConfigMap(self, config_map_name: str, config_map_data: dict):
         try:
             response = self.getCoreV1Api().replace_namespaced_config_map(
-                name=configMapName,
+                name=config_map_name,
                 namespace=self.getNamespace(),
                 body=client.V1ConfigMap(
                     metadata=client.V1ObjectMeta(
-                        name=configMapName,
+                        name=config_map_name,
                     ),
-                    data=configMapData,
+                    data=config_map_data,
                 ),
             )
         except ApiException as e:
             logger.error(
                 "Failed to replace Config Map -> {}; error -> {}".format(
-                    configMapName, str(e)
+                    config_map_name, str(e)
                 )
             )
             return None
 
         return response
 
     # end method definition
 
-    def getStatefulSet(self, stsName: str):
+    def getStatefulSet(self, sts_name: str):
+        """Get a Kubernetes Stateful Set based on its name
+
+        Args:
+            sts_name (string): name of the Kubernetes stateful set
+
+        Returns:
+            K8s response
+        """
+
         try:
             response = self.getAppsV1Api().read_namespaced_stateful_set(
-                name=stsName, namespace=self.getNamespace()
+                name=sts_name, namespace=self.getNamespace()
             )
         except ApiException as e:
             logger.error(
-                "Failed to get Stateful Set -> {}; error -> {}".format(stsName, str(e))
+                "Failed to get Stateful Set -> {}; error -> {}".format(sts_name, str(e))
             )
             return None
 
         return response
 
     # end method definition
 
-    def getStatefulSetScale(self, stsName: str):
+    def getStatefulSetScale(self, sts_name: str):
+        """Get the number of replicas for a Kubernetes Stateful Set
+
+        Args:
+            sts_name (string): name of the Kubernetes stateful set
+
+        Returns:
+            K8S response: response of the Kubernetes API
+        """
+
         try:
             response = self.getAppsV1Api().read_namespaced_stateful_set_scale(
-                name=stsName, namespace=self.getNamespace()
+                name=sts_name, namespace=self.getNamespace()
             )
         except ApiException as e:
             logger.error(
                 "Failed to get scaling (replicas) of Stateful Set -> {}; error -> {}".format(
-                    stsName, str(e)
+                    sts_name, str(e)
                 )
             )
             return None
 
         return response
 
     # end method definition
 
-    def patchStatefulSet(self, stsName: str, stsBody: dict):
+    def patchStatefulSet(self, sts_name: str, sts_body: dict):
         """patchStatefulSet: patch a Stateful set with new values
         Args:
-            stsName (string): name of the Kubernetes stateful set in the current namespace
-            stsBody (string): patch string
+            sts_name (string): name of the Kubernetes stateful set in the current namespace
+            sts_body (string): patch string
         Return: response of the Kubernetes patch command or None if the call fails
         """
 
         try:
             response = self.getAppsV1Api().patch_namespaced_stateful_set(
-                name=stsName, namespace=self.getNamespace(), body=stsBody
+                name=sts_name, namespace=self.getNamespace(), body=sts_body
             )
         except ApiException as e:
             logger.error(
                 "Failed to patch Stateful Set -> {} with -> {}; error -> {}".format(
-                    stsName, stsBody, str(e)
+                    sts_name, sts_body, str(e)
                 )
             )
             return None
 
         return response
 
     # end method definition
 
-    def scaleStatefulSet(self, stsName: str, scale: int):
+    def scaleStatefulSet(self, sts_name: str, scale: int):
         """scaleStatefulSet: scale a stateful set to a specific number of replicas. It uses the class method patchStatefulSet() above.
         Args:
-            stsName (string): name of the Kubernetes stateful set in the current namespace
+            sts_name (string): name of the Kubernetes stateful set in the current namespace
         Return: response of the Kubernetes patch command or None if the call fails
         """
 
         try:
             response = self.patchStatefulSet(
-                stsName, stsBody={"spec": {"replicas": scale}}
+                sts_name, stsBody={"spec": {"replicas": scale}}
             )
         except ApiException as e:
             logger.error(
                 "Failed to scale Stateful Set -> {} to -> {} replicas; error -> {}".format(
-                    stsName, scale, str(e)
+                    sts_name, scale, str(e)
                 )
             )
             return None
 
         return response
 
     # end method definition
 
-    def getService(self, serviceName: str):
+    def getService(self, service_name: str):
         """getService: gets a Kubernetes service with a defined name in the
         current namespace
         Args:
-            serviceName (string): name of the Kubernetes service in the current namespace
+            service_name (string): name of the Kubernetes service in the current namespace
         Return: <class 'kubernetes.client.models.v1_service.V1Service'> or None if the call fails
                 This is NOT a dict but an object - the you have to use the "." syntax to access to returned elements
         """
 
         try:
             response = self.getCoreV1Api().read_namespaced_service(
-                name=serviceName, namespace=self.getNamespace()
+                name=service_name, namespace=self.getNamespace()
             )
         except ApiException as e:
             logger.error(
-                "Failed to get Service -> {}; error -> {}".format(serviceName, str(e))
+                "Failed to get Service -> {}; error -> {}".format(service_name, str(e))
             )
             return None
 
         return response
 
-    def listServices(self, fieldSelector: str = "", labelSelector: str = ""):
+    def listServices(self, field_selector: str = "", label_selector: str = ""):
         """listServices: lists all Kubernetes Service in the current namespace.
                          The list can be filtered by providing field selectors and
                         label selectors.
         Args:
-            fieldSelector (string): filter result based on fields
-            labelSelector (string): filter result based on labels
-        Return: Object of <class 'kubernetes.client.models.v1_service_list.V1ServiceList'> or None if the call fails
-                This is NOT a dict but an object - you have to use the "." syntax to access to returned elements
+            field_selector (string): filter result based on fields
+            label_selector (string): filter result based on labels
+        Return: V1ServiceList (object) or None if the call fails
+                Properties can be accessed with the "." notation (this is an object not a dict!):
+                - api_version: The Kubernetes API version.
+                - items: A list of V1Service objects, each representing a service. You can access the fields of a
+                        V1Service object using dot notation, for example, service.metadata.name to access the name of the service
+                - kind: The Kubernetes object kind, which is always "ServiceList".
+                - metadata: Additional metadata about the pod list, such as the resource version.
         """
+
         try:
             response = self.getCoreV1Api().list_namespaced_service(
-                field_selector=fieldSelector,
-                label_selector=labelSelector,
+                field_selector=field_selector,
+                label_selector=label_selector,
                 namespace=self.getNamespace(),
             )
         except ApiException as e:
             logger.error(
                 "Failed to list Services with field_selector -> {} and label_selector -> {}; error -> {}".format(
-                    fieldSelector, labelSelector, str(e)
+                    field_selector, label_selector, str(e)
                 )
             )
             return None
 
         return response
 
     # end method definition
 
-    def patchService(self, serviceName: str, serviceBody: dict):
+    def patchService(self, service_name: str, service_body: dict):
         """patchService: patches a Kubernetes Service with an updated spec
         Args:
-            serviceName (string): name of the Kubernetes Ingress in the current namespace
-            serviceBody (dict): new / updated Service body spec (will be merged with existing values)
+            service_name (string): name of the Kubernetes Ingress in the current namespace
+            service_body (dict): new / updated Service body spec (will be merged with existing values)
         Return: Object of <class 'kubernetes.client.models.v1_service.V1Service'> or None if the call fails
                 This is NOT a dict but an object - you have to use the "." syntax to access to returned elements
         """
 
         try:
             response = self.getCoreV1Api().patch_namespaced_service(
-                name=serviceName, namespace=self.getNamespace(), body=serviceBody
+                name=service_name, namespace=self.getNamespace(), body=service_body
             )
         except ApiException as e:
             logger.error(
                 "Failed to patch Service -> {} with -> {}; error -> {}".format(
-                    serviceName, serviceBody, str(e)
+                    service_name, service_body, str(e)
                 )
             )
             return None
 
         return response
 
     # end method definition
 
-    def getIngress(self, ingressName: str):
+    def getIngress(self, ingress_name: str):
         """getIngress: gets a Kubernetes Ingress with a defined name in the
         current namespace
         Args:
-            ingressName (string): name of the Kubernetes Ingress in the current namespace
+            ingress_name (string): name of the Kubernetes Ingress in the current namespace
         Return: Object of <class 'kubernetes.client.models.v1_ingress.V1Ingress'> or None if the call fails
                 This is NOT a dict but an object - the you have to use the "." syntax to access to returned elements
         """
 
         try:
             response = self.getNetworkingV1Api().read_namespaced_ingress(
-                name=ingressName, namespace=self.getNamespace()
+                name=ingress_name, namespace=self.getNamespace()
             )
         except ApiException as e:
             logger.error(
-                "Failed to get Ingress -> {}; error -> {}".format(ingressName, str(e))
+                "Failed to get Ingress -> {}; error -> {}".format(ingress_name, str(e))
             )
             return None
 
         return response
 
     # end method definition
 
-    def patchIngress(self, ingressName: str, ingressBody: dict):
+    def patchIngress(self, ingress_name: str, ingress_body: dict):
         """patchIngress: patches a Kubernetes Ingress with a updated spec
         Args:
-            ingressName (string): name of the Kubernetes Ingress in the current namespace
-            ingressBody (dict): new / updated ingress body spec (will be merged with existing values)
+            ingress_name (string): name of the Kubernetes Ingress in the current namespace
+            ingress_body (dict): new / updated ingress body spec (will be merged with existing values)
         Return: Object of <class 'kubernetes.client.models.v1_ingress.V1Ingress'> or None if the call fails
                 This is NOT a dict but an object - you have to use the "." syntax to access to returned elements
         """
 
         try:
             response = self.getNetworkingV1Api().patch_namespaced_ingress(
-                name=ingressName,
+                name=ingress_name,
                 namespace=self.getNamespace(),
-                body=ingressBody,
+                body=ingress_body,
             )
         except ApiException as e:
             logger.error(
                 "Failed to patch Ingress -> {} with -> {}; error -> {}".format(
-                    ingressName, ingressBody, str(e)
+                    ingress_name, ingress_body, str(e)
                 )
             )
             return None
 
         return response
 
     # end method definition
 
     def updateIngressBackendServices(
-        self, ingressName: str, hostname: str, serviceName: str, servicePort: int
+        self, ingress_name: str, hostname: str, service_name: str, service_port: int
     ):
         """updateIngressBackendService: updates a backend service and port of an Kubernetes Ingress
 
         "spec": {
             "rules": [
                 {
                     "host": host,
@@ -669,15 +714,15 @@
             hostname (string): hostname that should get an updated backend service / port
             serviceName (string): new backend service name
             servicePort (int): new backend service port
         Return: Object of <class 'kubernetes.client.models.v1_ingress.V1Ingress'> or None if the call fails
                 This is NOT a dict but an object - you have to use the "." syntax to access to returned elements
         """
 
-        ingress = self.getIngress(ingressName)
+        ingress = self.getIngress(ingress_name)
         if not ingress:
             return None
 
         host = ""
         rules = ingress.spec.rules
         rule_index = 0
         for rule in rules:
@@ -685,41 +730,41 @@
                 host = rule.host
                 path = rule.http.paths[0]
                 backend = path.backend
                 service = backend.service
 
                 logger.info(
                     "Replace backend service -> {} ({}) with new backend service -> {} ({})".format(
-                        service.name, service.port.number, serviceName, servicePort
+                        service.name, service.port.number, service_name, service_port
                     )
                 )
 
-                service.name = serviceName
-                service.port.number = servicePort
+                service.name = service_name
+                service.port.number = service_port
                 break
             else:
                 rule_index += 1
 
         if not host:
             logger.error("Cannot find host -> {}.")
             return None
 
         body = [
             {
                 "op": "replace",
                 "path": "/spec/rules/{}/http/paths/0/backend/service/name".format(
                     rule_index
                 ),
-                "value": serviceName,
+                "value": service_name,
             },
             {
                 "op": "replace",
                 "path": "/spec/rules/{}/http/paths/0/backend/service/port/number".format(
                     rule_index
                 ),
-                "value": servicePort,
+                "value": service_port,
             },
         ]
 
-        return self.patchIngress(ingressName, body)
+        return self.patchIngress(ingress_name, body)
 
     # end method definition
```

### Comparing `pyxecm-0.0.14/pyxecm/m365.py` & `pyxecm-0.0.15/pyxecm/m365.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.14/pyxecm/main.py` & `pyxecm-0.0.15/pyxecm/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
         logging.StreamHandler(sys.stdout),
     ],
 )
 logger = logging.getLogger(os.path.basename(__file__))
 
 
 def initM365() -> object:
-    """Initialize the M365 class we use to talk to the Microsoft Graph API.
+    """Initialize the M365 object we use to talk to the Microsoft Graph API.
 
     Args: None
     Return:
         M365 object
     """
 
     logger.info("Microsoft 365 Tenant ID     = " + O365_TENANT_ID)
@@ -213,15 +213,15 @@
         return m365_object
     else:
         logger.error("Failed toconnect to Microsoft Graph API.")
         return None
 
 
 def initK8s(inCluster: bool = True) -> object:
-    """Initialize the Kubernetes class we use to talk to the Kubernetes objects.
+    """Initialize the Kubernetes object we use to talk to the Kubernetes API.
 
     Args:
         inCluster (boolean): controls wether the code runs inside a pod (inCluster = True)
                              or locally (access via .kube / kubectl, inCluster = False)
     Return:
         K8s object
         The global variables otcs_replicas_frontend and otcs_replicas_backend are initialized
@@ -270,20 +270,19 @@
         )
     )
 
     return k8s_object
 
 
 def initOTDS():
-    """Initialize the OTDS class and parameters and authenticate at OTDS once it is ready.
+    """Initialize the OTDS object and parameters and authenticate at OTDS once it is ready.
 
     Args: None
     Return:
         OTDS object
-        OTDS admin password
     """
 
     logger.info("Connection parameters OTDS:")
     logger.info("OTDS Protocol          = " + OTDS_PROTOCOL)
     logger.info("OTDS Public Protocol   = " + OTDS_PUBLIC_PROTOCOL)
     logger.info("OTDS Hostname          = " + OTDS_HOSTNAME)
     logger.info("OTDS Public URL        = " + OTDS_PUBLIC_URL)
@@ -308,15 +307,15 @@
     otds_object.enableAudit()
 
     return otds_object
     # end function definition
 
 
 def initOTAC(k8s_object: object) -> object:
-    """Initialize the OTAC class and parameters.
+    """Initialize the OTAC object and parameters.
        Configure the Archive Server as a known server
        if environment variable OTAC_KNOWN_SERVER is set.
 
     Args: None
     Return:
         OTAC object
     """
@@ -330,15 +329,15 @@
     logger.debug("OTAC Admin Password   = " + OTAC_PASSWORD)
     logger.info(
         "OTAC Known Server      = "
         + (OTAC_KNOWN_SERVER if OTAC_KNOWN_SERVER != "" else "<not configured>")
     )
 
     otac_object = otac.OTAC(
-        OTAC_PROTOCOL, OTAC_HOSTNAME, OTAC_PORT, OTAC_ADMIN, OTAC_PASSWORD
+        OTAC_PROTOCOL, OTAC_HOSTNAME, OTAC_PORT, OTAC_ADMIN, OTAC_PASSWORD, OTDS_ADMIN, OTDS_PASSWORD
     )
 
     # is there a known server configured for Archive Center (to sync content with)
     if otac_object and OTAC_KNOWN_SERVER != "":
         # wait until the OTAC pod is in ready state
         logger.info("Waiting for Archive Center to become ready...")
         k8s_object.waitPodCondition(OTAC_K8S_POD_NAME, "Ready")
@@ -450,15 +449,15 @@
 
         otds_object.updateResource(name="cs", resource=otcs_resource)
 
     return otcs_object
     # end function definition
 
 def initOTIV(otds_object: object) -> object:
-    """Initialize the OTIV (Intelligent Viewing) OTDS settings.
+    """Initialize the OTIV (Intelligent Viewing) object and its OTDS settings.
 
     Args:
         otds_object (object): OTDS object
     Return:
         otiv_object (object): OTIV object
     """
 
@@ -490,15 +489,15 @@
     
     return otiv_object
 
     # end function definition
 
 
 def initOTPD(k8s_object: object) -> object:
-    """Initialize the OTPD (PowerDocs) class and parameters.
+    """Initialize the OTPD (PowerDocs) object and parameters.
 
     Args: None
     Return:
         OTPD (PowerDocs) object
     """
 
     logger.info("Connection parameters OTPD (PowerDocs):")
```

### Comparing `pyxecm-0.0.14/pyxecm/otcs.py` & `pyxecm-0.0.15/pyxecm/otcs.py`

 * *Files 5% similar despite different names*

```diff
@@ -314,19 +314,19 @@
             None.
         Return:
             Dict of request header values.
         """
 
         # create union of two dicts: cookie and headers
         # (with Python 3.9 this would be easier with the "|" operator)
-        requestHeader = {}
-        requestHeader.update(self.cookie())
-        requestHeader.update(requestFormHeaders)
+        request_header = {}
+        request_header.update(self.cookie())
+        request_header.update(requestFormHeaders)
 
-        return requestHeader
+        return request_header
 
     # end method definition
 
     def requestJsonHeader(self):
         """Deliver the request header used for the CRUD REST API calls.
            Consists of Cookie + Json Headers (see global vasriable)
 
@@ -334,19 +334,19 @@
             None.
         Return:
             Dict of request header values.
         """
 
         # create union of two dicts: cookie and headers
         # (with Python 3.9 this would be easier with the "|" operator)
-        requestHeader = {}
-        requestHeader.update(self.cookie())
-        requestHeader.update(requestJsonHeaders)
+        request_header = {}
+        request_header.update(self.cookie())
+        request_header.update(requestJsonHeaders)
 
-        return requestHeader
+        return request_header
 
     # end method definition
 
     def requestDownloadHeader(self):
         """Deliver the request header used for the CRUD REST API calls.
            Consists of Cookie + Form Headers (see global vasriable)
 
@@ -354,19 +354,19 @@
             None.
         Return:
             Dict of request header values.
         """
 
         # create union of two dicts: cookie and headers
         # (with Python 3.9 this would be easier with the "|" operator)
-        requestHeader = {}
-        requestHeader.update(self.cookie())
-        requestHeader.update(requestDownloadHeaders)
+        request_header = {}
+        request_header.update(self.cookie())
+        request_header.update(requestDownloadHeaders)
 
-        return requestHeader
+        return request_header
 
     # end method definition
 
     def parseRequestResponse(
         self,
         response_object: object,
         additional_error_message: str = "",
@@ -656,25 +656,25 @@
         """Checks if the Content Server pod is ready to receive requests.
 
         Args:
             None.
         Return: True if pod is ready. False if pod is not yet ready.
         """
 
-        requestUrl = self.config()["configuredUrl"]
+        request_url = self.config()["configuredUrl"]
 
-        logger.info("Trying to retrieve OTCS url -> {}".format(requestUrl))
+        logger.info("Trying to retrieve OTCS url -> {}".format(request_url))
 
         try:
             checkcsConfiguredResponse = requests.get(
-                requestUrl, headers=requestJsonHeaders
+                request_url, headers=requestJsonHeaders
             )
         except Exception as e:
             logger.warning(
-                "Unable to connect to -> {} : {}".format(requestUrl, e))
+                "Unable to connect to -> {} : {}".format(request_url, e))
             logger.warning("OTCS service may not be ready yet.")
             return False
 
         if checkcsConfiguredResponse.ok:
             return True
         else:
             return False
@@ -698,43 +698,43 @@
 
         logger.info(
             "Requesting OTCS ticket from -> {}".format(
                 self.config()["authenticationUrl"]
             )
         )
 
-        authenticateResponse = None
+        response = None
         try:
-            authenticateResponse = requests.post(
+            response = requests.post(
                 self.config()["authenticationUrl"],
                 data=self.credentials(),
                 headers=requestFormHeaders,
             )
         except Exception as e:
             logger.warning(
                 "Unable to connect to -> {} : {}".format(
                     self.config()["authenticationUrl"], e
                 )
             )
             logger.warning("OTCS service may not be ready yet.")
             return None
 
-        if authenticateResponse.ok:
+        if response.ok:
             authenticate_dict = self.parseRequestResponse(
-                authenticateResponse, "This can be normal during restart", False
+                response, "This can be normal during restart", False
             )
             if not authenticate_dict:
                 return None
             else:
                 otcs_ticket = authenticate_dict["ticket"]
                 logger.info("Ticket -> {}".format(otcs_ticket))
         else:
             logger.error(
                 "Failed to request an OTCS ticket; error -> {}".format(
-                    authenticateResponse.text
+                    response.text
                 )
             )
             return None
 
         # Store authentication ticket:
         self._cookie = {
           "otcsticket": otcs_ticket,
@@ -766,39 +766,39 @@
                     filename, os.path.dirname(xmlfilepath)
                 )
             )
             return None
 
         llconfig_file = {"file": (filename, open(xmlfilepath), "text/xml")}
 
-        requestUrl = self.config()["importSettingsUrl"]
-        requestHeader = self._cookie
+        request_url = self.config()["importSettingsUrl"]
+        request_header = self._cookie
 
         retries = 0
         while True:
-            importResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 files=llconfig_file,
-                headers=requestHeader,
+                headers=request_header,
                 cookies=self.cookie(),
             )
-            if importResponse.ok:
+            if response.ok:
                 logger.debug(
                     "Admin settings in file -> {} have been applied".format(xmlfilepath))
-                return self.parseRequestResponse(importResponse)
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif importResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to import settings file -> {}; status -> {}; error -> {}".format(
-                        xmlfilepath, importResponse.status_code, importResponse.text
+                        xmlfilepath, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def getGroup(self, name: str, show_error: bool = False):
@@ -818,39 +818,39 @@
                 }
             ]
             To access the id of the first group found use ["data"][0]["id"]
         """
 
         # Add query parameters (these are NOT passed via JSon body!)
         # type = 1 ==> Group
-        requestUrl = self.config()["groupsUrl"] + \
+        request_url = self.config()["groupsUrl"] + \
             "?where_type=1&query={}".format(name)
-        requestHeader = self.requestFormHeader()
+        request_header = self.requestFormHeader()
 
         logger.info(
-            "Get group with name -> {}; calling -> {}".format(name, requestUrl))
+            "Get group with name -> {}; calling -> {}".format(name, request_url))
 
         retries = 0
         while True:
-            getGroupResponse = requests.get(
-                requestUrl, headers=requestHeader, cookies=self.cookie()
+            response = requests.get(
+                request_url, headers=request_header, cookies=self.cookie()
             )
-            if getGroupResponse.ok:
-                return self.parseRequestResponse(getGroupResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif getGroupResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 if show_error:
                     logger.error(
                         "Failed to get group -> {}; status -> {}; error -> {}".format(
-                            name, getGroupResponse.status_code, getGroupResponse.text
+                            name, response.status_code, response.text
                         )
                     )
                 else:
                     logger.info("Group -> {} not found.".format(name))
                 return None
 
     # end method definition
@@ -876,39 +876,39 @@
                 }
             ]
             To access the (login) name of the first user found use ["data"][0]["name"]
         """
 
         # Add query parameters (these are NOT passed via JSon body!)
         # type = 0 ==> User
-        requestUrl = self.config()["usersUrl"] + \
+        request_url = self.config()["usersUrl"] + \
             "?where_type=0&query={}".format(name)
-        requestHeader = self.requestFormHeader()
+        request_header = self.requestFormHeader()
 
         logger.info(
-            "Get user with name -> {}; calling -> {}".format(name, requestUrl))
+            "Get user with name -> {}; calling -> {}".format(name, request_url))
 
         retries = 0
         while True:
-            getUserResponse = requests.get(
-                requestUrl, headers=requestHeader, cookies=self.cookie()
+            response = requests.get(
+                request_url, headers=request_header, cookies=self.cookie()
             )
-            if getUserResponse.ok:
-                return self.parseRequestResponse(getUserResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif getUserResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 if show_error:
                     logger.error(
                         "Failed to get user -> {}; status -> {}; error -> {}".format(
-                            name, getUserResponse.status_code, getUserResponse.text
+                            name, response.status_code, response.text
                         )
                     )
                 else:
                     logger.info("User -> {} not found.".format(name))
                 return None
 
     # end method definition
@@ -920,41 +920,41 @@
             name (string): name of the group
         Return:
             Group information (json) or None if the group couldn't be created (e.g. because it exisits already).
         """
 
         groupPostBody = {"type": 1, "name": name}
 
-        requestUrl = self.config()["groupsUrl"]
-        requestHeader = self.requestFormHeader()
+        request_url = self.config()["groupsUrl"]
+        request_header = self.requestFormHeader()
 
         logger.info(
-            "Adding group -> {}; calling -> {}".format(name, requestUrl))
+            "Adding group -> {}; calling -> {}".format(name, request_url))
         logger.debug("Group Attributes -> {}".format(groupPostBody))
 
         retries = 0
         while True:
-            groupResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 data=groupPostBody,
-                headers=requestHeader,
+                headers=request_header,
                 cookies=self.cookie(),
             )
-            if groupResponse.ok:
-                return self.parseRequestResponse(groupResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif groupResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to add group -> {}; status -> {}; error -> {}".format(
-                        name, groupResponse.status_code, groupResponse.text
+                        name, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def addUser(
@@ -996,39 +996,39 @@
             "privilege_modify_users": ("Modify Users" in privileges),
             "privilege_modify_groups": ("Modify Groups" in privileges),
             "privilege_user_admin_rights": ("User Admin Rights" in privileges),
             "privilege_grant_discovery": ("Grant Discovery" in privileges),
             "privilege_system_admin_rights": ("System Admin Rights" in privileges)
         }
 
-        requestUrl = self.config()["usersUrl"]
-        requestHeader = self.requestFormHeader()
+        request_url = self.config()["usersUrl"]
+        request_header = self.requestFormHeader()
 
-        logger.info("Adding user -> {}; calling -> {}".format(name, requestUrl))
+        logger.info("Adding user -> {}; calling -> {}".format(name, request_url))
 
         retries = 0
         while True:
-            userResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 data=userPostBody,
-                headers=requestHeader,
+                headers=request_header,
                 cookies=self.cookie(),
             )
-            if userResponse.ok:
-                return self.parseRequestResponse(userResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif userResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to add user -> {}; status -> {}; error -> {}".format(
-                        name, userResponse.status_code, userResponse.text
+                        name, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def searchUser(self, value: str, field: str = "where_name"):
@@ -1037,40 +1037,40 @@
         Args:
             value (string): field value
             field (string): user field to search with (where_name, where_first_name, where_last_name)
         Return:
             User information (json) or None if the user couldn't be found (e.g. because it doesn't exist).
         """
 
-        requestUrl = self.config()["membersUrl"] + "?" + field + "=" + value
-        requestHeader = self.requestFormHeader()
+        request_url = self.config()["membersUrl"] + "?" + field + "=" + value
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Searching user by field -> {}, value -> {}; calling -> {}".format(
-                field, value, requestUrl
+                field, value, request_url
             )
         )
 
         retries = 0
         while True:
-            userResponse = requests.get(
-                requestUrl, headers=requestHeader, cookies=self.cookie()
+            response = requests.get(
+                request_url, headers=request_header, cookies=self.cookie()
             )
-            if userResponse.ok:
-                return self.parseRequestResponse(userResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif userResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Cannot find user with -> {} = {}; status -> {}; error -> {}".format(
-                        field, value, userResponse.status_code, userResponse.text
+                        field, value, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def updateUser(self, user_id: int, field: str, value: str):
@@ -1082,44 +1082,44 @@
             field (string): user field
         Return:
             User information (json) or None if the user couldn't be updated (e.g. because it doesn't exist).
         """
 
         userPutBody = {field: value}
 
-        requestUrl = self.config()["membersUrl"] + "/" + str(user_id)
-        requestHeader = self.requestFormHeader()
+        request_url = self.config()["membersUrl"] + "/" + str(user_id)
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Updating user with ID -> {}, field -> {}, value -> {}; calling -> {}".format(
-                user_id, field, value, requestUrl
+                user_id, field, value, request_url
             )
         )
         logger.debug("User Attributes -> {}".format(userPutBody))
 
         retries = 0
         while True:
-            userResponse = requests.put(
-                requestUrl,
+            response = requests.put(
+                request_url,
                 data=userPutBody,
-                headers=requestHeader,
+                headers=request_header,
                 cookies=self.cookie(),
             )
-            if userResponse.ok:
-                return self.parseRequestResponse(userResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif userResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to update user -> {}; status -> {}; error -> {}".format(
-                        user_id, userResponse.status_code, userResponse.text
+                        user_id, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def updateUserProfile(self, field: str, value):
@@ -1131,45 +1131,45 @@
             field (string): user field
         Return:
             User information (json) or None if the user couldn't be updated (e.g. because it doesn't exist).
         """
 
         userProfilePutBody = {"SmartUI": {field: value}}
 
-        requestUrl = self.config()["membersUrl"] + "/preferences"
-        requestHeader = self.requestFormHeader()
+        request_url = self.config()["membersUrl"] + "/preferences"
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Updating profile for current user, field -> {}, value -> {}; calling -> {}".format(
-                field, value, requestUrl
+                field, value, request_url
             )
         )
         logger.debug("User Attributes -> {}".format(userProfilePutBody))
 
         retries = 0
         while True:
             # This REST API needs a special treatment: we encapsulate the payload as JSON into a "body" tag.
-            userProfileResponse = requests.put(
-                requestUrl,
+            response = requests.put(
+                request_url,
                 data={"body": json.dumps(userProfilePutBody)},
-                headers=requestHeader,
+                headers=request_header,
                 cookies=self.cookie(),
             )
-            if userProfileResponse.ok:
-                return self.parseRequestResponse(userProfileResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif userProfileResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to update profile of current user; status -> {}; error -> {}".format(
-                        userProfileResponse.status_code, userProfileResponse.text
+                        response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def updateUserPhoto(self, user_id: int, photo_id: int):
@@ -1180,43 +1180,43 @@
             photo_id (integer): Node ID of the photo
         Return:
             Node information (json) or None if no node with this nickname is found.
         """
 
         updateUserPutBody = {"photo_id": photo_id}
 
-        requestUrl = self.config()["usersUrl"] + "/" + str(user_id)
-        requestHeader = self.requestFormHeader()
+        request_url = self.config()["usersUrl"] + "/" + str(user_id)
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Update user ID -> {} with photo ID -> {}; calling -> {}".format(
-                user_id, photo_id, requestUrl
+                user_id, photo_id, request_url
             )
         )
 
         retries = 0
         while True:
-            updateUserResponse = requests.put(
-                requestUrl,
+            response = requests.put(
+                request_url,
                 data=updateUserPutBody,
-                headers=requestHeader,
+                headers=request_header,
                 cookies=self.cookie(),
             )
-            if updateUserResponse.ok:
-                return self.parseRequestResponse(updateUserResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif updateUserResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to update user with ID -> {}; status -> {}; error -> {}".format(
-                        user_id, updateUserResponse.status_code, updateUserResponse.text
+                        user_id, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def isProxy(self, user_name: str) -> bool:
@@ -1245,43 +1245,43 @@
         """Get list of user proxies.
            This method needs to be called as the user the proxy is acting for.
         Args: None
         Return:
             Node information (json) or None if REST call fails.
         """
 
-        requestUrl = self.config()["usersUrl"] + "/proxies"
-        requestHeader = self.requestFormHeader()
+        request_url = self.config()["usersUrl"] + "/proxies"
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Get proxy users for current user; calling -> {}".format(
-                requestUrl)
+                request_url)
         )
 
         retries = 0
         while True:
 
             # This REST API needs a special treatment: we encapsulate the payload as JSON into a "add_assignment" tag.
-            proxyResponse = requests.get(
-                requestUrl,
-                headers=requestHeader,
+            response = requests.get(
+                request_url,
+                headers=request_header,
                 cookies=self.cookie(),
             )
-            if proxyResponse.ok:
-                return self.parseRequestResponse(proxyResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif proxyResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to get proxy users for current user; status -> {}; error -> {}".format(
-                        proxyResponse.status_code, proxyResponse.text
+                        response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def updateUserProxy(
@@ -1308,45 +1308,45 @@
         post_dict = {}
         if from_date and to_date:
             post_dict["from_date"] = from_date
             post_dict["to_date"] = to_date
 
         proxyPostBody = {str(proxy_user_id): post_dict}
 
-        requestUrl = self.config()["usersUrl"] + "/proxies"
-        requestHeader = self.requestFormHeader()
+        request_url = self.config()["usersUrl"] + "/proxies"
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Assign proxy user with ID -> {} to current user; calling -> {}".format(
-                proxy_user_id, requestUrl
+                proxy_user_id, request_url
             )
         )
 
         retries = 0
         while True:
 
             # This REST API needs a special treatment: we encapsulate the payload as JSON into a "add_assignment" tag.
-            proxyResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 data={"add_proxy": json.dumps(proxyPostBody)},
-                headers=requestHeader,
+                headers=request_header,
                 cookies=self.cookie(),
             )
-            if proxyResponse.ok:
-                return self.parseRequestResponse(proxyResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif proxyResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to assign proxy user with ID -> {} to current user; status -> {}; error -> {}".format(
-                        proxy_user_id, proxyResponse.status_code, proxyResponse.text
+                        proxy_user_id, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def addFavorite(self, node_id: int):
@@ -1354,42 +1354,42 @@
 
         Args:
             nodeid (integer): ID of the node.
         Return:
             Response (json) or None if the favorite creation has failed.
         """
 
-        requestUrl = self.config()["favoritesUrl"] + "/" + str(node_id)
-        requestHeader = self.requestFormHeader()
+        request_url = self.config()["favoritesUrl"] + "/" + str(node_id)
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Adding favorite for node ID -> {}; calling -> {}".format(
-                node_id, requestUrl
+                node_id, request_url
             )
         )
 
         retries = 0
         while True:
-            addFavoriteResponse = requests.post(
-                requestUrl, headers=requestHeader, cookies=self.cookie()
+            response = requests.post(
+                request_url, headers=request_header, cookies=self.cookie()
             )
-            if addFavoriteResponse.ok:
-                return self.parseRequestResponse(addFavoriteResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif addFavoriteResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to add favorite for node ID -> {}; status -> {}; error -> {}".format(
                         node_id,
-                        addFavoriteResponse.status_code,
-                        addFavoriteResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def getGroupMembers(self, group: int, member_type: int, limit: int = 100):
@@ -1401,49 +1401,49 @@
             limit (integer): max number of results (internal default is 25)
         Return:
             Group members (json) or None if the group members couldn't be found.
         """
 
         # default limit is 25 which may not be enough for groups with many members
         # where_type = 1 makes sure we just get groups and not users
-        requestUrl = (
+        request_url = (
             self.config()["membersUrl"]
             + "/"
             + str(group)
             + "/members?where_type="
             + str(member_type)
             + "&limit="
             + str(limit)
         )
-        requestHeader = self.requestFormHeader()
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Getting members of group -> {}; calling -> {}".format(
-                group, requestUrl)
+                group, request_url)
         )
 
         retries = 0
         while True:
-            groupMembersResponse = requests.get(
-                requestUrl, headers=requestHeader, cookies=self.cookie()
+            response = requests.get(
+                request_url, headers=request_header, cookies=self.cookie()
             )
-            if groupMembersResponse.ok:
-                return self.parseRequestResponse(groupMembersResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif groupMembersResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to get members of group -> {}; status -> {}; error -> {}".format(
                         group,
-                        groupMembersResponse.status_code,
-                        groupMembersResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def addGroupMember(self, member: int, group: int):
@@ -1454,47 +1454,47 @@
             group (integer): ID of the target group.
         Return:
             Response (json) or None if the adding fails.
         """
 
         groupMemberPostBody = {"member_id": member}
 
-        requestUrl = self.config()["membersUrl"] + \
+        request_url = self.config()["membersUrl"] + \
             "/" + str(group) + "/members"
-        requestHeader = self.requestFormHeader()
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Adding member -> {} to group -> {}; calling -> {}".format(
-                member, group, requestUrl
+                member, group, request_url
             )
         )
 
         retries = 0
         while True:
-            groupMemberResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 data=groupMemberPostBody,
-                headers=requestHeader,
+                headers=request_header,
                 cookies=self.cookie(),
             )
-            if groupMemberResponse.ok:
-                return self.parseRequestResponse(groupMemberResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif groupMemberResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to add member -> {} to group -> {}; status -> {}; error -> {}".format(
                         member,
                         group,
-                        groupMemberResponse.status_code,
-                        groupMemberResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def getNode(self, node_id: int):
@@ -1563,37 +1563,37 @@
                             ]
                         }
                     ]
                 }
             ]
         """
 
-        requestUrl = self.config()["nodesUrlv2"] + "/" + str(node_id)
-        requestHeader = self.requestFormHeader()
+        request_url = self.config()["nodesUrlv2"] + "/" + str(node_id)
+        request_header = self.requestFormHeader()
 
         logger.info(
-            "Get node with ID -> {}; calling -> {}".format(node_id, requestUrl))
+            "Get node with ID -> {}; calling -> {}".format(node_id, request_url))
 
         retries = 0
         while True:
-            getNodeResponse = requests.get(
-                requestUrl, headers=requestHeader, cookies=self.cookie()
+            response = requests.get(
+                request_url, headers=request_header, cookies=self.cookie()
             )
-            if getNodeResponse.ok:
-                return self.parseRequestResponse(getNodeResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif getNodeResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to get node with ID -> {}; status -> {}; error -> {}".format(
-                        node_id, getNodeResponse.status_code, getNodeResponse.text
+                        node_id, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def getNodeByParentAndName(self, parent_id: int, name: str, show_error: bool = False):
@@ -1609,49 +1609,49 @@
             Access to node ID with: response["results"][0]["data"]["properties"]["id"]
         """
 
         # Add query parameters (these are NOT passed via JSon body!)
         query = {"where_name": name}
         encoded_query = urllib.parse.urlencode(query, doseq=True)
 
-        requestUrl = (
+        request_url = (
             self.config()["nodesUrlv2"]
             + "/"
             + str(parent_id)
             + "/nodes?{}".format(encoded_query)
         )
-        requestHeader = self.requestFormHeader()
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Get node with name -> {} and parent ID -> {}; calling -> {}".format(
-                name, parent_id, requestUrl
+                name, parent_id, request_url
             )
         )
 
         retries = 0
         while True:
-            getNodeResponse = requests.get(
-                requestUrl, headers=requestHeader, cookies=self.cookie()
+            response = requests.get(
+                request_url, headers=request_header, cookies=self.cookie()
             )
-            if getNodeResponse.ok:
-                return self.parseRequestResponse(getNodeResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif getNodeResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 if show_error:
                     logger.error(
                         "Failed to get node with name -> {} and parent ID -> {}; status -> {}; error -> {}".format(
                             name,
                             parent_id,
-                            getNodeResponse.status_code,
-                            getNodeResponse.text,
+                            response.status_code,
+                            response.text,
                         )
                     )
                 else:
                     logger.info(
                         "Node with name -> {} and parent ID -> {} not found.".format(
                             name, parent_id
                         )
@@ -1726,40 +1726,40 @@
         Args:
             nickname (string): Nickname of the node.
             show_error (boolean): treat as error if node is not found
         Return:
             Node information (json) or None if no node with this nickname is found.
         """
 
-        requestUrl = self.config()["nicknameUrl"] + "/" + nickname + "/nodes"
-        requestHeader = self.requestFormHeader()
+        request_url = self.config()["nicknameUrl"] + "/" + nickname + "/nodes"
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Get node with nickname -> {}; calling -> {}".format(
-                nickname, requestUrl)
+                nickname, request_url)
         )
 
         retries = 0
         while True:
-            getNodeResponse = requests.get(
-                requestUrl, headers=requestHeader, cookies=self.cookie()
+            response = requests.get(
+                request_url, headers=request_header, cookies=self.cookie()
             )
-            if getNodeResponse.ok:
-                return self.parseRequestResponse(getNodeResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif getNodeResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 if show_error:
                     logger.error(
                         "Failed to get node with nickname -> {}; status -> {}; error -> {}".format(
-                            nickname, getNodeResponse.status_code, getNodeResponse.text
+                            nickname, response.status_code, response.text
                         )
                     )
                 else:
                     logger.info(
                         "Node with nickname -> {} not found.".format(
                             nickname)
                     )
@@ -1801,48 +1801,48 @@
         if show_hidden:
             query["show_hidden"] = show_hidden
         if page > 1:
             query["page"] = page
 
         encodedQuery = urllib.parse.urlencode(query, doseq=True)
 
-        requestUrl = (
+        request_url = (
             self.config()["nodesUrlv2"]
             + "/"
             + str(parent_node_id)
             + "/nodes"
             + "?{}".format(encodedQuery)
         )
-        requestHeader = self.requestFormHeader()
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Get subnodes of parent node with ID -> {}; calling -> {}".format(
-                parent_node_id, requestUrl
+                parent_node_id, request_url
             )
         )
 
         retries = 0
         while True:
-            getNodesResponse = requests.get(
-                requestUrl, headers=requestHeader, cookies=self.cookie()
+            response = requests.get(
+                request_url, headers=request_header, cookies=self.cookie()
             )
-            if getNodesResponse.ok:
-                return self.parseRequestResponse(getNodesResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif getNodesResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to get subnodes for parent node with ID -> {}; status -> {}; error -> {}".format(
                         parent_node_id,
-                        getNodesResponse.status_code,
-                        getNodesResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def renameNode(self, node_id: int, name: str, description: str, name_multilingual: dict = {}, description_multilingual: dict = {}):
@@ -1860,46 +1860,46 @@
         renameNodePutBody = {"name": name, "description": description}
 
         if name_multilingual:
             renameNodePutBody["name_multilingual"] = name_multilingual
         if description_multilingual:
             renameNodePutBody["description_multilingual"] = description_multilingual
 
-        requestUrl = self.config()["nodesUrlv2"] + "/" + str(node_id)
-        requestHeader = self.requestFormHeader()
+        request_url = self.config()["nodesUrlv2"] + "/" + str(node_id)
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Renaming node -> {} to -> {}; calling -> {}".format(
-                node_id, name, requestUrl
+                node_id, name, request_url
             )
         )
 
         retries = 0
         while True:
-            nodeRenameResponse = requests.put(
-                requestUrl,
+            response = requests.put(
+                request_url,
                 data={"body": json.dumps(renameNodePutBody)},
-                headers=requestHeader,
+                headers=request_header,
                 cookies=self.cookie(),
             )
-            if nodeRenameResponse.ok:
-                return self.parseRequestResponse(nodeRenameResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif nodeRenameResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to rename node -> {} to -> {}; status -> {}; error -> {}".format(
                         node_id,
                         name,
-                        nodeRenameResponse.status_code,
-                        nodeRenameResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def getVolumes(self):
@@ -1908,36 +1908,36 @@
         Args:
             None
         Return:
             Volume Details (json) or None if an error occured.
             ["results"]["data"]["properties"]["id"] is the node ID of the volume.
         """
 
-        requestUrl = self.config()["volumeUrl"]
-        requestHeader = self.requestFormHeader()
+        request_url = self.config()["volumeUrl"]
+        request_header = self.requestFormHeader()
 
-        logger.info("Get volumes; calling -> {}".format(requestUrl))
+        logger.info("Get volumes; calling -> {}".format(request_url))
 
         retries = 0
         while True:
-            getVolumeResponse = requests.get(
-                requestUrl, headers=requestHeader, cookies=self.cookie()
+            response = requests.get(
+                request_url, headers=request_header, cookies=self.cookie()
             )
-            if getVolumeResponse.ok:
-                return self.parseRequestResponse(getVolumeResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif getVolumeResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to get volumes; status -> {}; error -> {}".format(
-                        getVolumeResponse.status_code, getVolumeResponse.text
+                        response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def getVolume(self, volume_type: int):
@@ -1946,41 +1946,41 @@
         Args:
             volume_type (integer): ID of the volume type
         Return:
             Volume Details (json) or None if volume is not found.
             ["results"]["data"]["properties"]["id"] is the node ID of the volume.
         """
 
-        requestUrl = self.config()["volumeUrl"] + "/" + str(volume_type)
-        requestHeader = self.requestFormHeader()
+        request_url = self.config()["volumeUrl"] + "/" + str(volume_type)
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Get volume type -> {}; calling -> {}".format(
-                volume_type, requestUrl)
+                volume_type, request_url)
         )
 
         retries = 0
         while True:
-            getVolumeResponse = requests.get(
-                requestUrl, headers=requestHeader, cookies=self.cookie()
+            response = requests.get(
+                request_url, headers=request_header, cookies=self.cookie()
             )
-            if getVolumeResponse.ok:
-                return self.parseRequestResponse(getVolumeResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif getVolumeResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to get volume type -> {}; status -> {}; error -> {}".format(
                         volume_type,
-                        getVolumeResponse.status_code,
-                        getVolumeResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def search(
@@ -2025,44 +2025,44 @@
         if slice_id > 0:
             searchPostBody["slice_id"] = slice_id
         if query_id > 0:
             searchPostBody["query_id"] = query_id
         if template_id > 0:
             searchPostBody["template_id"] = template_id
 
-        requestUrl = self.config()["searchUrl"]
-        requestHeader = self.requestFormHeader()
+        request_url = self.config()["searchUrl"]
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Serarch for term -> {}; calling -> {}".format(
-                search_term, requestUrl)
+                search_term, request_url)
         )
 
         retries = 0
         while True:
-            getNodesResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 data=searchPostBody,
-                headers=requestHeader,
+                headers=request_header,
                 cookies=self.cookie(),
             )
-            if getNodesResponse.ok:
-                return self.parseRequestResponse(getNodesResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif getNodesResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to search for term -> {}; status -> {}; error -> {}".format(
                         search_term,
-                        getNodesResponse.status_code,
-                        getNodesResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def getExternalSystemConnection(self, connection_name: str, show_error: bool = False):
@@ -2071,44 +2071,44 @@
         Args:
             connection_name (string): Name of the connection
             show_error (boolean): treat as error if node is not found
         Return:
             External system Details (json) or None if the REST call fails.
         """
 
-        requestUrl = self.config()["externalSystem"] + \
+        request_url = self.config()["externalSystem"] + \
             "/" + connection_name + "/config"
-        requestHeader = self.cookie()
+        request_header = self.cookie()
 
         logger.info(
             "Get external system connection -> {}; calling -> {}".format(
-                connection_name, requestUrl
+                connection_name, request_url
             )
         )
 
         retries = 0
         while True:
-            externalSystemResponse = requests.get(
-                requestUrl, headers=requestHeader, cookies=self.cookie()
+            response = requests.get(
+                request_url, headers=request_header, cookies=self.cookie()
             )
-            if externalSystemResponse.ok:
-                return self.parseRequestResponse(externalSystemResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif externalSystemResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 if show_error:
                     logger.error(
                         "Failed to get external system connection -> {}; status -> {}; error -> {}".format(
                             connection_name,
-                            externalSystemResponse.status_code,
-                            externalSystemResponse.text,
+                            response.status_code,
+                            response.text,
                         )
                     )
                 else:
                     logger.info(
                         "External system -> {} not found.".format(
                             connection_name)
                     )
@@ -2155,45 +2155,45 @@
 
         if authentication_method == "OAUTH" and client_id and client_secret:
             externalSystemPostBody["authentication_method"] = str(
                 authentication_method)
             externalSystemPostBody["client_id"] = str(client_id)
             externalSystemPostBody["client_secret"] = str(client_secret)
 
-        requestUrl = self.config()["externalSystem"]
-        requestHeader = self.cookie()
+        request_url = self.config()["externalSystem"]
+        request_header = self.cookie()
 
         logger.info(
             "Creating external system connection -> {} of type -> {} and URL -> {}; calling -> {}".format(
-                connection_name, connection_type, as_url, requestUrl
+                connection_name, connection_type, as_url, request_url
             )
         )
 
         retries = 0
         while True:
-            externalSystemResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 data=externalSystemPostBody,
-                headers=requestHeader,
+                headers=request_header,
                 cookies=self.cookie(),
             )
-            if externalSystemResponse.ok:
-                return self.parseRequestResponse(externalSystemResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif externalSystemResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to create external system connection -> {}; status -> {}; error -> {}".format(
                         connection_name,
-                        externalSystemResponse.status_code,
-                        externalSystemResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def downloadConfigFile(self, otcs_url_suffix: str, file_path: str) -> bool:
@@ -2208,23 +2208,23 @@
             file_path (str): local path to save the file (direcotry + filename)
 
         Returns:
             boolean: True if the download succeeds, False otherwise
         """
 
 
-        requestUrl = self.config()["baseUrl"] + otcs_url_suffix
-        # requestHeader = self.cookie()
-        requestHeader = self.requestDownloadHeader()
+        request_url = self.config()["baseUrl"] + otcs_url_suffix
+        # request_header = self.cookie()
+        request_header = self.requestDownloadHeader()
 
         logger.info(
-            "Download config file from URL -> {}".format(requestUrl))
+            "Download config file from URL -> {}".format(request_url))
 
         try:
-            response = requests.get(requestUrl, headers=requestHeader, cookies=self.cookie())
+            response = requests.get(request_url, headers=request_header, cookies=self.cookie())
             response.raise_for_status()
         except requests.exceptions.HTTPError as errh:
             logger.error("Http Error -> {}".format(errh))
             return False
         except requests.exceptions.ConnectionError as errc:
             logger.error("Error Connecting -> {}".format(errc))
             return False
@@ -2240,15 +2240,15 @@
         # Open file in write binary mode
         with open(file_path, 'wb') as file:
             # Write the content to the file
             file.write(content)
 
         logger.info(
             "Successfully downloaded config file -> {} to -> {}; status code -> {}".format(
-                requestUrl, file_path, response.status_code
+                request_url, file_path, response.status_code
             )
         )
 
         return True
 
     # end method definition
 
@@ -2302,49 +2302,49 @@
         else:
             logger.warning("Cannot access -> {}".format(package_url))
             return None
 
         uploadPostData = {"type": str(volume_type), "name": file_name}
         uploadPostFiles = [("file", (f"{file_name}", file, mime_type))]
 
-        requestUrl = self.config()["nodesUrlv2"]
-        requestHeader = (
+        request_url = self.config()["nodesUrlv2"]
+        request_header = (
             self.cookie()
         )  # for some reason we have to omit the other header parts here - otherwise we get a 500 response
 
         logger.info(
             "Uploading package -> {} with mime type -> {}; calling -> {}".format(
-                file_name, mime_type, requestUrl
+                file_name, mime_type, request_url
             )
         )
 
         retries = 0
         while True:
-            uploadResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 data=uploadPostData,
                 files=uploadPostFiles,
-                headers=requestHeader,
+                headers=request_header,
                 cookies=self.cookie(),
             )
-            if uploadResponse.ok:
-                return self.parseRequestResponse(uploadResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif uploadResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to upload file -> {} to volume -> {}; status -> {}; error -> {}".format(
                         package_url,
                         volume_type,
-                        uploadResponse.status_code,
-                        uploadResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def uploadFileToParent(
@@ -2400,49 +2400,49 @@
         uploadPostData = {
             "type": str(144),
             "name": file_name,
             "parent_id": str(parent_id),
         }
         uploadPostFiles = [("file", (f"{file_name}", file_content, mime_type))]
 
-        requestUrl = self.config()["nodesUrlv2"]
-        requestHeader = (
+        request_url = self.config()["nodesUrlv2"]
+        request_header = (
             self.cookie()
         )  # for some reason we have to omit the other header parts here - otherwise we get a 500 response
 
         logger.info(
             "Uploading file -> {} with mime type -> {} to parent -> {}; calling -> {}".format(
-                file_name, mime_type, parent_id, requestUrl
+                file_name, mime_type, parent_id, request_url
             )
         )
 
         retries = 0
         while True:
-            uploadResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 data=uploadPostData,
                 files=uploadPostFiles,
-                headers=requestHeader,
+                headers=request_header,
                 cookies=self.cookie(),
             )
-            if uploadResponse.ok:
-                return self.parseRequestResponse(uploadResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif uploadResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to upload file -> {} to parent -> {}; status -> {}; error -> {}".format(
                         file_url,
                         parent_id,
-                        uploadResponse.status_code,
-                        uploadResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def addDocumentVersion(
@@ -2497,50 +2497,50 @@
             return None
 
         uploadPostData = {
             "description": description
         }
         uploadPostFiles = [("file", (f"{file_name}", file_content, mime_type))]
 
-        requestUrl = self.config()["nodesUrlv2"] + \
+        request_url = self.config()["nodesUrlv2"] + \
             "/" + str(node_id) + "/versions"
-        requestHeader = (
+        request_header = (
             self.cookie()
         )  # for some reason we have to omit the other header parts here - otherwise we get a 500 response
 
         logger.info(
             "Uploading document version -> {} with mime type -> {} to document node -> {}; calling -> {}".format(
-                file_name, mime_type, node_id, requestUrl
+                file_name, mime_type, node_id, request_url
             )
         )
 
         retries = 0
         while True:
-            uploadResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 data=uploadPostData,
                 files=uploadPostFiles,
-                headers=requestHeader,
+                headers=request_header,
                 cookies=self.cookie(),
             )
-            if uploadResponse.ok:
-                return self.parseRequestResponse(uploadResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif uploadResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to add version -> {} to document -> {}; status -> {}; error -> {}".format(
                         file_url,
                         node_id,
-                        uploadResponse.status_code,
-                        uploadResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def getLatestDocumentVersion(self, node_id: int):
@@ -2548,38 +2548,38 @@
 
         Args:
             node_id (integer) is the node Id of the node
         Return:
             Node information (json) or None if no node with this ID is found.
         """
 
-        requestUrl = self.config()["nodesUrl"] + \
+        request_url = self.config()["nodesUrl"] + \
             "/" + str(node_id) + "/versions/latest"
-        requestHeader = self.requestFormHeader()
+        request_header = self.requestFormHeader()
 
         logger.info(
-            "Get latest version of document with node ID -> {}; calling -> {}".format(node_id, requestUrl))
+            "Get latest version of document with node ID -> {}; calling -> {}".format(node_id, request_url))
 
         retries = 0
         while True:
-            getNodeResponse = requests.get(
-                requestUrl, headers=requestHeader, cookies=self.cookie()
+            response = requests.get(
+                request_url, headers=request_header, cookies=self.cookie()
             )
-            if getNodeResponse.ok:
-                return self.parseRequestResponse(getNodeResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif getNodeResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to get latest version of document with node ID -> {}; status -> {}; error -> {}".format(
-                        node_id, getNodeResponse.status_code, getNodeResponse.text
+                        node_id, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def downloadDocument(self, node_id: int, file_path: str, version_number: str = ""):
@@ -2602,41 +2602,41 @@
             logger.error("Directory -> {} does not exist".format(directory))
             return False
 
         if not version_number:
             response = self.getLatestDocumentVersion(node_id)
             version_number = response["data"]["version_number"]
 
-        requestUrl = self.config()["nodesUrlv2"] + \
+        request_url = self.config()["nodesUrlv2"] + \
             "/" + str(node_id) + "/versions/" + \
             str(version_number) + "/content/" + str(node_id)
-        requestHeader = self.requestDownloadHeader()
+        request_header = self.requestDownloadHeader()
 
         logger.info(
-            "Download document with node ID -> {}; calling -> {}".format(node_id, requestUrl))
+            "Download document with node ID -> {}; calling -> {}".format(node_id, request_url))
 
         retries = 0
         while True:
-            getNodeResponse = requests.get(
-                requestUrl, headers=requestHeader, cookies=self.cookie()
+            response = requests.get(
+                request_url, headers=request_header, cookies=self.cookie()
             )
-            if getNodeResponse.ok:
+            if response.ok:
                 #                content = self.parseRequestResponse(getNodeResponse)["data"]
-                content = getNodeResponse.content
+                content = response.content
                 break
             # Check if Session has expired - then re-authenticate and try once more
-            elif getNodeResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to download document with node ID -> {}; status -> {}; error -> {}".format(
-                        node_id, getNodeResponse.status_code, getNodeResponse.text
+                        node_id, response.status_code, response.text
                     )
                 )
                 return False
 
         logger.info(
             "Writing document content to file -> {}".format(file_path))
 
@@ -2656,42 +2656,42 @@
             workbench_name (string): name of the workbench to be created
         Return:
             Create response (json) or None if the creation fails.
         """
 
         createWorbenchPostData = {"type": "528", "name": workbench_name}
 
-        requestUrl = self.config()["nodesUrlv2"]
-        requestHeader = self.requestFormHeader()
+        request_url = self.config()["nodesUrlv2"]
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Create transport workbench -> {}; calling -> {}".format(
-                workbench_name, requestUrl
+                workbench_name, request_url
             )
         )
         retries = 0
         while True:
-            createResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 data=createWorbenchPostData,
-                headers=requestHeader,
+                headers=request_header,
                 cookies=self.cookie(),
             )
-            if createResponse.ok:
-                return self.parseRequestResponse(createResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif createResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to create transport workbench -> {}; status -> {}; error -> {}".format(
-                        workbench_name, createResponse.status_code, createResponse.text
+                        workbench_name, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def unpackTransportPackage(self, package_id: int, workbench_id: int):
@@ -2702,47 +2702,47 @@
             workbench_iD (integer): ID of target workbench
         Return:
             Unpack response (json) or None if the unpacking fails.
         """
 
         unpackPackagePostData = {"workbench_id": workbench_id}
 
-        requestUrl = self.config()["nodesUrlv2"] + \
+        request_url = self.config()["nodesUrlv2"] + \
             "/" + str(package_id) + "/unpack"
-        requestHeader = self.requestFormHeader()
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Unpack transport package with ID -> {} into workbench with ID -> {}; calling -> {}".format(
-                package_id, workbench_id, requestUrl
+                package_id, workbench_id, request_url
             )
         )
 
         retries = 0
         while True:
-            unpackResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 data=unpackPackagePostData,
-                headers=requestHeader,
+                headers=request_header,
                 cookies=self.cookie(),
             )
-            if unpackResponse.ok:
-                return self.parseRequestResponse(unpackResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif unpackResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to unpack package -> {}; to workbench -> {}; status -> {}; error -> {}".format(
                         package_id,
                         workbench_id,
-                        unpackResponse.status_code,
-                        unpackResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def deployWorkbench(self, workbench_id: int):
@@ -2750,55 +2750,55 @@
 
         Args:
             workbench_iD (integer): ID of the workbench to be deployed
         Return:
             Deploy response (json) or None if the deployment fails.
         """
 
-        requestUrl = self.config()["nodesUrlv2"] + \
+        request_url = self.config()["nodesUrlv2"] + \
             "/" + str(workbench_id) + "/deploy"
-        requestHeader = self.requestFormHeader()
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Deploy workbench with ID -> {}; calling -> {}".format(
-                workbench_id, requestUrl
+                workbench_id, request_url
             )
         )
 
         retries = 0
         while True:
             # As this is a potentially long-running request we put it in try / except:
             try:
-                deployResponse = requests.post(
-                    requestUrl, headers=requestHeader, cookies=self.cookie()
+                response = requests.post(
+                    request_url, headers=request_header, cookies=self.cookie()
                 )
             except Exception as e:
                 logger.error(
                     "Error deploying workbench -> {} : error -> {}".format(
                         workbench_id, e
                     )
                 )
                 return None
-            if deployResponse.ok:
-                response_dict = self.parseRequestResponse(deployResponse)
+            if response.ok:
+                response_dict = self.parseRequestResponse(response)
                 if not response_dict:
                     logger.error(
                         "Error deploying workbench -> {}".format(workbench_id))
                     return None
                 return response_dict
             # Check if Session has expired - then re-authenticate and try once more
-            elif deployResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.warning(
                     "Failed to depoloy workbench -> {}; status -> {}; error -> {}".format(
-                        workbench_id, deployResponse.status_code, deployResponse.text
+                        workbench_id, response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def deployTransport(
@@ -3083,39 +3083,39 @@
 
         Args:
             None
         Return:
             Workspace Types (json) or None if the request fails.
         """
 
-        requestUrl = (
+        request_url = (
             self.config()["businessworkspacetypes"]
             + "?expand_templates=true&expand_wksp_info=true"
         )
-        requestHeader = self.requestFormHeader()
+        request_header = self.requestFormHeader()
 
-        logger.info("Get workspace types; calling -> {}".format(requestUrl))
+        logger.info("Get workspace types; calling -> {}".format(request_url))
 
         retries = 0
         while True:
-            workspaceTypeResponse = requests.get(
-                requestUrl, headers=requestHeader, cookies=self.cookie()
+            response = requests.get(
+                request_url, headers=request_header, cookies=self.cookie()
             )
-            if workspaceTypeResponse.ok:
-                return self.parseRequestResponse(workspaceTypeResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif workspaceTypeResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to get workspace types; status -> {}; error -> {}".format(
-                        workspaceTypeResponse.status_code, workspaceTypeResponse.text
+                        response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def getBusinessObjectType(self, external_system_id: str, type_name: str):
@@ -3124,48 +3124,48 @@
         Args:
             external_system_id (string): external system Id (such as "TM6")
             type_name (string): type name (such as "SAP Customer")
         Return:
             Workspace Type information (json) or None if the request fails.
         """
 
-        requestUrl = (
+        request_url = (
             self.config()["externalSystem"]
             + "/"
             + str(external_system_id)
             + "/botypes/"
             + str(type_name)
         )
-        requestHeader = self.requestFormHeader()
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Get business object type -> {} for external system -> {}; calling -> {}".format(
-                type_name, external_system_id, requestUrl
+                type_name, external_system_id, request_url
             )
         )
 
         retries = 0
         while True:
-            businessObjectTypeResponse = requests.get(
-                requestUrl, headers=requestHeader, cookies=self.cookie()
+            response = requests.get(
+                request_url, headers=request_header, cookies=self.cookie()
             )
-            if businessObjectTypeResponse.ok:
-                return self.parseRequestResponse(businessObjectTypeResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif businessObjectTypeResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to get business object type -> {}; status -> {}; error -> {}".format(
                         type_name,
-                        businessObjectTypeResponse.status_code,
-                        businessObjectTypeResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def getWorkspaceCreateForm(
@@ -3186,57 +3186,57 @@
             parent_id (string): parent ID of the workspaces. Needs only be specified in special
                                 cases where workspace location cannot be derived from workspace
                                 type definition, e.g. sub-workspace
         Return:
             Workspace Create Form data (json) or None if the request fails.
         """
 
-        requestUrl = self.config()[
+        request_url = self.config()[
             "businessworkspacecreateform"
         ] + "?template_id={}".format(template_id)
         # Is a parent ID specifified? Then we need to add it to the request URL
         if parent_id is not None:
-            requestUrl += "&parent_id={}".format(parent_id)
+            request_url += "&parent_id={}".format(parent_id)
         # Is this workspace connected to a business application / external system?
         if external_system_id and bo_type and bo_id:
-            requestUrl += "&ext_system_id={}".format(external_system_id)
-            requestUrl += "&bo_type={}".format(bo_type)
-            requestUrl += "&bo_id={}".format(bo_id)
+            request_url += "&ext_system_id={}".format(external_system_id)
+            request_url += "&bo_type={}".format(bo_type)
+            request_url += "&bo_id={}".format(bo_id)
             logger.info(
                 "Use business object connection -> ({}, {}, {}) for workspace template -> {}".format(
                     external_system_id, bo_type, bo_id, template_id
                 )
             )
-        requestHeader = self.requestFormHeader()
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Get workspace create form for template -> {}; calling -> {}".format(
-                template_id, requestUrl
+                template_id, request_url
             )
         )
 
         retries = 0
         while True:
-            workspaceCreateFormResponse = requests.get(
-                requestUrl, headers=requestHeader, cookies=self.cookie()
+            response = requests.get(
+                request_url, headers=request_header, cookies=self.cookie()
             )
-            if workspaceCreateFormResponse.ok:
-                return self.parseRequestResponse(workspaceCreateFormResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif workspaceCreateFormResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to get workspace create form for template -> {}; status -> {}; error -> {}".format(
                         template_id,
-                        workspaceCreateFormResponse.status_code,
-                        workspaceCreateFormResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def getWorkspace(self, node_id: int):
@@ -3244,41 +3244,41 @@
 
         Args:
             node_id (integer) is the node Id of the workspace
         Return:
             Node information (json) or None if no node with this ID is found.
         """
 
-        requestUrl = self.config()["businessworkspaces"] + "/" + str(node_id)
-        requestHeader = self.requestFormHeader()
+        request_url = self.config()["businessworkspaces"] + "/" + str(node_id)
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Get workspace with ID -> {}; calling -> {}".format(
-                node_id, requestUrl)
+                node_id, request_url)
         )
 
         retries = 0
         while True:
-            getWorkspaceResponse = requests.get(
-                requestUrl, headers=requestHeader, cookies=self.cookie()
+            response = requests.get(
+                request_url, headers=request_header, cookies=self.cookie()
             )
-            if getWorkspaceResponse.ok:
-                return self.parseRequestResponse(getWorkspaceResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif getWorkspaceResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to get workspace with ID -> {}; status -> {}; error -> {}".format(
                         node_id,
-                        getWorkspaceResponse.status_code,
-                        getWorkspaceResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def getWorkspaceByNameAndType(
@@ -3301,44 +3301,44 @@
         query = {
             "where_name": name,
             "where_workspace_type_name": type_name,
             "expanded_view": expanded_view,
         }
         encodedQuery = urllib.parse.urlencode(query, doseq=True)
 
-        requestUrl = self.config()["businessworkspaces"] + \
+        request_url = self.config()["businessworkspaces"] + \
             "?{}".format(encodedQuery)
-        requestHeader = self.requestFormHeader()
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Get workspace with name -> {} and type -> {}; calling -> {}".format(
-                name, type_name, requestUrl
+                name, type_name, request_url
             )
         )
 
         retries = 0
         while True:
-            getWorkpaceResponse = requests.get(
-                requestUrl, headers=requestHeader, cookies=self.cookie()
+            response = requests.get(
+                request_url, headers=request_header, cookies=self.cookie()
             )
-            if getWorkpaceResponse.ok:
-                return self.parseRequestResponse(getWorkpaceResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif getWorkpaceResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.warning(
                     "Failed to get workspace -> {} of type -> {}; status -> {}; error -> {}".format(
                         name,
                         type_name,
-                        getWorkpaceResponse.status_code,
-                        getWorkpaceResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def createWorkspace(
@@ -3404,48 +3404,48 @@
         else:
             logger.info(
                 "Determine location of workspace -> {} via workspace type -> {}".format(
                     workspace_name, workspace_type
                 )
             )
 
-        requestUrl = self.config()["businessworkspaces"]
-        requestHeader = self.requestFormHeader()
+        request_url = self.config()["businessworkspaces"]
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Create workspace -> {} with type -> {} from template -> {}; calling -> {}".format(
-                workspace_name, workspace_type, workspace_template_id, requestUrl
+                workspace_name, workspace_type, workspace_template_id, request_url
             )
         )
 
         retries = 0
         while True:
             # This REST API needs a special treatment: we encapsulate the payload as JSON into a "body" tag.
             # See https://developer.opentext.com/apis/14ba85a7-4693-48d3-8c93-9214c663edd2/4403207c-40f1-476a-b794-fdb563e37e1f/07229613-7ef4-4519-8b8a-47eaff639d42#operation/createBusinessWorkspace
-            workspaceResponse = requests.post(
-                requestUrl,
-                headers=requestHeader,
+            response = requests.post(
+                request_url,
+                headers=request_header,
                 data={"body": json.dumps(createWorkspacePostData)},
                 cookies=self.cookie(),
             )
-            if workspaceResponse.ok:
-                return self.parseRequestResponse(workspaceResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif workspaceResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to create workspace -> {} from template -> {}; status -> {}; error -> {}".format(
                         workspace_name,
                         workspace_template_id,
-                        workspaceResponse.status_code,
-                        workspaceResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def createWorkspaceRelationship(
@@ -3462,48 +3462,48 @@
         """
 
         createWorkspaceRelationshipPostData = {
             "rel_bw_id": str(related_workspace_id),
             "rel_type": relationship_type,
         }
 
-        requestUrl = self.config()["businessworkspaces"] + "/{}/relateditems".format(
+        request_url = self.config()["businessworkspaces"] + "/{}/relateditems".format(
             workspace_id
         )
-        requestHeader = self.requestFormHeader()
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Create workspace relationship between -> {} and -> {}; calling -> {}".format(
-                workspace_id, related_workspace_id, requestUrl
+                workspace_id, related_workspace_id, request_url
             )
         )
 
         retries = 0
         while True:
-            workspaceRelationshipResponse = requests.post(
-                requestUrl,
-                headers=requestHeader,
+            response = requests.post(
+                request_url,
+                headers=request_header,
                 data=createWorkspaceRelationshipPostData,
                 cookies=self.cookie(),
             )
-            if workspaceRelationshipResponse.ok:
-                return self.parseRequestResponse(workspaceRelationshipResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif workspaceRelationshipResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to create workspace relationship between -> {} and -> {}; status -> {}; error -> {}".format(
                         workspace_id,
                         related_workspace_id,
-                        workspaceRelationshipResponse.status_code,
-                        workspaceRelationshipResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def getWorkspaceRelationships(self, workspace_id: int):
@@ -3511,45 +3511,45 @@
 
         Args:
             workspace_id: ID of the workspace template
         Return:
             Workspace relationships (json) or None if the request fails.
         """
 
-        requestUrl = (
+        request_url = (
             self.config()["businessworkspaces"] + "/" +
             str(workspace_id) + "/relateditems"
         )
-        requestHeader = self.requestFormHeader()
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Get related workspaces for workspace -> {}; calling -> {}".format(
-                workspace_id, requestUrl
+                workspace_id, request_url
             )
         )
 
         retries = 0
         while True:
-            workspaceRolesResponse = requests.get(
-                requestUrl, headers=requestHeader, cookies=self.cookie()
+            response = requests.get(
+                request_url, headers=request_header, cookies=self.cookie()
             )
-            if workspaceRolesResponse.ok:
-                return self.parseRequestResponse(workspaceRolesResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif workspaceRolesResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to get related workspaces of workspace -> {}; status -> {}; error -> {}".format(
                         workspace_id,
-                        workspaceRolesResponse.status_code,
-                        workspaceRolesResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def getWorkspaceRoles(self, workspace_id: int):
@@ -3557,45 +3557,45 @@
 
         Args:
             workspace_id: ID of the workspace template
         Return:
             Workspace Roles data (json) or None if the request fails.
         """
 
-        requestUrl = (
+        request_url = (
             self.config()["businessworkspaces"] + "/" +
             str(workspace_id) + "/roles"
         )
-        requestHeader = self.requestFormHeader()
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Get workspace roles of workspace -> {}; calling -> {}".format(
-                workspace_id, requestUrl
+                workspace_id, request_url
             )
         )
 
         retries = 0
         while True:
-            workspaceRolesResponse = requests.get(
-                requestUrl, headers=requestHeader, cookies=self.cookie()
+            response = requests.get(
+                request_url, headers=request_header, cookies=self.cookie()
             )
-            if workspaceRolesResponse.ok:
-                return self.parseRequestResponse(workspaceRolesResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif workspaceRolesResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to get roles of workspace -> {}; status -> {}; error -> {}".format(
                         workspace_id,
-                        workspaceRolesResponse.status_code,
-                        workspaceRolesResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def addMemberToWorkspace(self, workspace_id: int, role_id: int, member_id: int, show_warning: bool = True):
@@ -3608,72 +3608,72 @@
             show_warning: if True shows a warning if member is already in role
         Return:
             Workspace Role Membership (json) or None if the request fails.
         """
 
         addMemberToWorkspacePostData = {"id": str(member_id)}
 
-        requestUrl = self.config()[
+        request_url = self.config()[
             "businessworkspaces"
         ] + "/{}/roles/{}/members".format(workspace_id, role_id)
-        requestHeader = self.requestFormHeader()
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Check if user/group -> {} is already in role -> {} of workspace -> {}; calling -> {}".format(
-                member_id, role_id, workspace_id, requestUrl
+                member_id, role_id, workspace_id, request_url
             )
         )
 
-        workspaceMembershipResponse = requests.get(
-            requestUrl, headers=requestHeader, cookies=self.cookie()
+        response = requests.get(
+            request_url, headers=request_header, cookies=self.cookie()
         )
-        if not workspaceMembershipResponse.ok:
+        if not response.ok:
             logger.error(
                 "Failed to get workspace members; status -> {}; error -> {}".format(
-                    workspaceMembershipResponse.status_code,
-                    workspaceMembershipResponse.text,
+                    response.status_code,
+                    response.text,
                 )
             )
             return None
 
         workspace_members = self.parseRequestResponse(
-            workspaceMembershipResponse)
+            response)
 
         if self.existResultItem(workspace_members, "id", member_id):
             if show_warning:
                 logger.warning(
                     "User -> {} is already a member of role -> {} of workspace -> {}".format(
                         member_id, role_id, workspace_id
                     )
                 )
             return workspace_members
 
         logger.info(
             "Add user/group -> {} to role -> {} of workspace -> {}; calling -> {}".format(
-                member_id, role_id, workspace_id, requestUrl
+                member_id, role_id, workspace_id, request_url
             )
         )
 
-        workspaceMembershipResponse = requests.post(
-            requestUrl,
-            headers=requestHeader,
+        response = requests.post(
+            request_url,
+            headers=request_header,
             data=addMemberToWorkspacePostData,
             cookies=self.cookie(),
         )
 
-        if workspaceMembershipResponse.ok:
-            return self.parseRequestResponse(workspaceMembershipResponse)
+        if response.ok:
+            return self.parseRequestResponse(response)
         else:
             logger.error(
                 "Failed to add user/group -> {} to role -> {} of workspace -> {}; status -> {}; error -> {}".format(
                     member_id,
                     role_id,
                     workspace_id,
-                    workspaceMembershipResponse.status_code,
-                    workspaceMembershipResponse.text,
+                    response.status_code,
+                    response.text,
                 )
             )
             return None
 
     # end method definition
 
     def removeMemberFromWorkspace(self, workspace_id: int, role_id: int, member_id: int, show_warning: bool = True):
@@ -3684,27 +3684,27 @@
             role_id (integer): ID of the role
             member_id (integer): User or Group Id
             show_warning: if True shows a warning if member is not in role
         Return:
             Workspace Role Membership (json) or None if the request fails.
         """
 
-        requestUrl = self.config()[
+        request_url = self.config()[
             "businessworkspaces"
         ] + "/{}/roles/{}/members".format(workspace_id, role_id)
-        requestHeader = self.requestFormHeader()
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Check if user/group -> {} is in role -> {} of workspace -> {}; calling -> {}".format(
-                member_id, role_id, workspace_id, requestUrl
+                member_id, role_id, workspace_id, request_url
             )
         )
 
         workspaceMembershipResponse = requests.get(
-            requestUrl, headers=requestHeader, cookies=self.cookie()
+            request_url, headers=request_header, cookies=self.cookie()
         )
         if not workspaceMembershipResponse.ok:
             logger.error(
                 "Failed to get workspace members; status -> {}; error -> {}".format(
                     workspaceMembershipResponse.status_code,
                     workspaceMembershipResponse.text,
                 )
@@ -3719,27 +3719,27 @@
                 logger.warning(
                     "User -> {} is not a member of role -> {} of workspace -> {}".format(
                         member_id, role_id, workspace_id
                     )
                 )
             return None
 
-        requestUrl = self.config()[
+        request_url = self.config()[
             "businessworkspaces"
         ] + "/{}/roles/{}/members/{}".format(workspace_id, role_id, member_id)
 
         logger.info(
             "Removing user/group -> {} from role -> {} of workspace -> {}; calling -> {}".format(
-                member_id, role_id, workspace_id, requestUrl
+                member_id, role_id, workspace_id, request_url
             )
         )
 
         workspaceMembershipResponse = requests.delete(
-            requestUrl,
-            headers=requestHeader,
+            request_url,
+            headers=request_header,
             cookies=self.cookie(),
         )
 
         if workspaceMembershipResponse.ok:
             return self.parseRequestResponse(workspaceMembershipResponse)
         else:
             logger.error(
@@ -3777,54 +3777,54 @@
                                  1 = sub-items
                                  2 = This item and sub-items
                                  3 = This item and immediate sub-items
         Return:
             Workspace Role Membership (json) or None if the request fails.
         """
 
-        requestUrl = self.config()["businessworkspaces"] + "/{}/roles/{}".format(
+        request_url = self.config()["businessworkspaces"] + "/{}/roles/{}".format(
             workspace_id, role_id
         )
 
-        requestHeader = self.requestFormHeader()
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Updating Permissions of role -> {} of workspace -> {} with permissions -> {}; calling -> {}".format(
-                role_id, workspace_id, permissions, requestUrl
+                role_id, workspace_id, permissions, request_url
             )
         )
 
         permissionPostData = {
             "permissions": permissions,
             "apply_to": apply_to,
         }
 
         retries = 0
         while True:
-            workspacePermissionResponse = requests.put(
-                requestUrl,
-                headers=requestHeader,
+            response = requests.put(
+                request_url,
+                headers=request_header,
                 data={"body": json.dumps(permissionPostData)},
                 cookies=self.cookie(),
             )
-            if workspacePermissionResponse.ok:
-                return self.parseRequestResponse(workspacePermissionResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif workspacePermissionResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to update permissions for role -> {} of workspace -> {}; status -> {}; error -> {}".format(
                         role_id,
                         workspace_id,
-                        workspacePermissionResponse.status_code,
-                        workspacePermissionResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def createItem(
@@ -3858,46 +3858,46 @@
         }
 
         if url:
             createItemPostData["url"] = url
         if original_id > 0:
             createItemPostData["original_id"] = original_id
 
-        requestUrl = self.config()["nodesUrlv2"]
-        requestHeader = self.requestFormHeader()
+        request_url = self.config()["nodesUrlv2"]
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Create item -> {} (type -> {}) under parent -> {}; calling -> {}".format(
-                item_name, item_type, parent_id, requestUrl
+                item_name, item_type, parent_id, request_url
             )
         )
 
         retries = 0
         while True:
             # This REST API needs a special treatment: we encapsulate the payload as JSON into a "body" tag.
-            createItemResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 data={"body": json.dumps(createItemPostData)},
-                headers=requestHeader,
+                headers=request_header,
                 cookies=self.cookie(),
             )
-            if createItemResponse.ok:
-                return self.parseRequestResponse(createItemResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif createItemResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to create item -> {}; status -> {}; error -> {}".format(
                         item_name,
-                        createItemResponse.status_code,
-                        createItemResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def updateItem(
@@ -3924,46 +3924,46 @@
             "description": item_description,
         }
 
         if parent_id:
             # this is a move operation
             updateItemPutData["parent_id"] = parent_id
 
-        requestUrl = self.config()["nodesUrlv2"] + "/" + str(node_id)
-        requestHeader = self.requestFormHeader()
+        request_url = self.config()["nodesUrlv2"] + "/" + str(node_id)
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Update item -> {} with data -> {}; calling -> {}".format(
-                item_name, updateItemPutData, requestUrl
+                item_name, updateItemPutData, request_url
             )
         )
 
         retries = 0
         while True:
             # This REST API needs a special treatment: we encapsulate the payload as JSON into a "body" tag.
-            updateItemResponse = requests.put(
-                requestUrl,
+            response = requests.put(
+                request_url,
                 data={"body": json.dumps(updateItemPutData)},
-                headers=requestHeader,
+                headers=request_header,
                 cookies=self.cookie(),
             )
-            if updateItemResponse.ok:
-                return self.parseRequestResponse(updateItemResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif updateItemResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to update item -> {}; status -> {}; error -> {}".format(
                         item_name,
-                        updateItemResponse.status_code,
-                        updateItemResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def getWebReportParameters(self, nickname: str):
@@ -3984,48 +3984,48 @@
                 "default_value": null,
                 "description": "string",
                 "mandatory": true
             }
             None if the REST call has failed.
         """
 
-        requestUrl = self.config()["webReportsUrl"] + \
+        request_url = self.config()["webReportsUrl"] + \
             "/" + nickname + "/parameters"
-        requestHeader = self.requestFormHeader()
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Retrieving parameters of Web Report with nickname -> {}; calling -> {}".format(
-                nickname, requestUrl
+                nickname, request_url
             )
         )
         retries = 0
         while True:
-            runWebReportResponse = requests.get(
-                requestUrl, headers=requestHeader, cookies=self.cookie()
+            response = requests.get(
+                request_url, headers=request_header, cookies=self.cookie()
             )
-            if runWebReportResponse.ok:
+            if response.ok:
                 # Return the "data" element which is a list of dict items:
-                result_dict = self.parseRequestResponse(runWebReportResponse)
+                result_dict = self.parseRequestResponse(response)
                 logger.debug(
                     "Web Report parameters result -> {}".format(result_dict))
                 if not result_dict.get("data"):
                     return None
                 return result_dict["data"]
             # Check if Session has expired - then re-authenticate and try once more
-            elif runWebReportResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to retrieve parameters of Web Report with nickname -> {}; status -> {}; error -> {}".format(
                         nickname,
-                        runWebReportResponse.status_code,
-                        runWebReportResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def runWebReport(self, nickname: str, web_report_parameters: dict = {}):
@@ -4034,45 +4034,45 @@
         Args:
             nickname (str): nickname of the Web Reports node.
             web_report_parameters (dict): Parameters of the Web Report (names + value pairs)
         Return:
             Response (json) or None if the Web Report execution has failed.
         """
 
-        requestUrl = self.config()["webReportsUrl"] + "/" + nickname
-        requestHeader = self.requestFormHeader()
+        request_url = self.config()["webReportsUrl"] + "/" + nickname
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Running Web Report with nickname -> {}; calling -> {}".format(
-                nickname, requestUrl
+                nickname, request_url
             )
         )
 
         retries = 0
         while True:
-            runWebReportResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 data=web_report_parameters,
-                headers=requestHeader,
+                headers=request_header,
                 cookies=self.cookie(),
             )
-            if runWebReportResponse.ok:
-                return self.parseRequestResponse(runWebReportResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif runWebReportResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to run web report with nickname -> {}; status -> {}; error -> {}".format(
                         nickname,
-                        runWebReportResponse.status_code,
-                        runWebReportResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def installCSApplication(self, application_name: str):
@@ -4082,45 +4082,45 @@
             application_name (string): name of the application (e.g. OTPOReports, OTRMReports, OTRMSecReports)
         Return:
             Response (json) or None if the installation of the CS Application has failed.
         """
 
         installCSApplicationPostData = {"appName": application_name}
 
-        requestUrl = self.config()["csApplicationsUrl"] + "/install"
-        requestHeader = self.requestFormHeader()
+        request_url = self.config()["csApplicationsUrl"] + "/install"
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Install CS Application -> {}; calling -> {}".format(
-                application_name, requestUrl
+                application_name, request_url
             )
         )
 
         retries = 0
         while True:
-            installCSApplicationResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 data=installCSApplicationPostData,
-                headers=requestHeader,
+                headers=request_header,
                 cookies=self.cookie(),
             )
-            if installCSApplicationResponse.ok:
-                return self.parseRequestResponse(installCSApplicationResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif installCSApplicationResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to install CS Application -> {}; status -> {}; error -> {}".format(
                         application_name,
-                        installCSApplicationResponse.status_code,
-                        installCSApplicationResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def assignItemToUserGroup(
@@ -4140,52 +4140,52 @@
 
         assignmentPostData = {
             "subject": subject,
             "instruction": instruction,
             "assignees": assignees,
         }
 
-        requestUrl = (
+        request_url = (
             self.config()["nodesUrlv2"] + "/" +
             str(node_id) + "/xgovassignments"
         )
 
-        requestHeader = self.requestFormHeader()
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Assign item with ID -> {} to assignees -> {} (subject -> {}); calling -> {}".format(
-                node_id, assignees, subject, requestUrl
+                node_id, assignees, subject, request_url
             )
         )
 
         retries = 0
         while True:
             # This REST API needs a special treatment: we encapsulate the payload as JSON into a "add_assignment" tag.
-            assignmentResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 data={"add_assignment": json.dumps(assignmentPostData)},
-                headers=requestHeader,
+                headers=request_header,
                 cookies=self.cookie(),
             )
-            if assignmentResponse.ok:
-                return self.parseRequestResponse(assignmentResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif assignmentResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to assign item with ID -> {} to assignees -> {} (subject -> {}); status -> {}; error -> {}".format(
                         node_id,
                         assignees,
                         subject,
-                        assignmentResponse.status_code,
-                        assignmentResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def convertPermissionStringToPermissionValue(self, permissions: list) -> int:
@@ -4311,65 +4311,65 @@
         }
 
         # Assignees can be specified for owner and group and must be specified for custom:
         #
         if assignee:
             permissionPostData["right_id"] = assignee
 
-        requestUrl = (
+        request_url = (
             self.config()["nodesUrlv2"]
             + "/"
             + str(node_id)
             + "/permissions/"
             + assignee_type
         )
 
-        requestHeader = self.requestFormHeader()
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Assign permissions -> {} to item with ID -> {}; assignee type -> {}; calling -> {}".format(
-                permissions, node_id, assignee_type, requestUrl
+                permissions, node_id, assignee_type, request_url
             )
         )
 
         retries = 0
         while True:
             # This REST API needs a special treatment: we encapsulate the payload as JSON into a "body" tag.
             if assignee_type == "custom":
                 # Custom also has a REST POST - we prefer this one as to
                 # also allows to add a new assigned permission (user or group):
-                permissionResponse = requests.post(
-                    requestUrl,
+                response = requests.post(
+                    request_url,
                     data={"body": json.dumps(permissionPostData)},
-                    headers=requestHeader,
+                    headers=request_header,
                     cookies=self.cookie(),
                 )
             else:
                 # Owner, Owner Group and Public require REST PUT:
-                permissionResponse = requests.put(
-                    requestUrl,
+                response = requests.put(
+                    request_url,
                     data={"body": json.dumps(permissionPostData)},
-                    headers=requestHeader,
+                    headers=request_header,
                     cookies=self.cookie(),
                 )
-            if permissionResponse.ok:
-                return self.parseRequestResponse(permissionResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif permissionResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to assign permissions -> {} to item with ID -> {}; status -> {}; error -> {}".format(
                         permissions,
                         node_id,
-                        permissionResponse.status_code,
-                        permissionResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def assignClassification(
@@ -4391,48 +4391,48 @@
             classification_list.append({"id": classification})
 
         classificationPostData = {
             "class_id": classification_list,
             "apply_to_sub_items": apply_to_sub_items,
         }
 
-        requestUrl = self.config()["nodesUrl"] + \
+        request_url = self.config()["nodesUrl"] + \
             "/" + str(node_id) + "/classifications"
 
-        requestHeader = self.requestFormHeader()
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Assign classifications with IDs -> {} to item with ID -> {}; calling -> {}".format(
-                classifications, node_id, requestUrl
+                classifications, node_id, request_url
             )
         )
 
         retries = 0
         while True:
-            classificationResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 data=classificationPostData,
-                headers=requestHeader,
+                headers=request_header,
                 cookies=self.cookie(),
             )
-            if classificationResponse.ok:
-                return self.parseRequestResponse(classificationResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif classificationResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to assign classifications with IDs -> {} to item with ID -> {}; status -> {}; error -> {}".format(
                         classifications,
                         node_id,
-                        classificationResponse.status_code,
-                        classificationResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def assignRMClassification(
@@ -4449,50 +4449,50 @@
         """
 
         rmClassificationPostData = {
             "class_id": rm_classification,
             "apply_to_sub_items": apply_to_sub_items,
         }
 
-        requestUrl = (
+        request_url = (
             self.config()["nodesUrl"] + "/" +
             str(node_id) + "/rmclassifications"
         )
 
-        requestHeader = self.requestFormHeader()
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Assign RM classifications with ID -> {} to item with ID -> {}; calling -> {}".format(
-                rm_classification, node_id, requestUrl
+                rm_classification, node_id, request_url
             )
         )
 
         retries = 0
         while True:
-            classificationResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 data=rmClassificationPostData,
-                headers=requestHeader,
+                headers=request_header,
                 cookies=self.cookie(),
             )
-            if classificationResponse.ok:
-                return self.parseRequestResponse(classificationResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif classificationResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to assign RM classifications with ID -> {} to item with ID -> {}; status -> {}; error -> {}".format(
                         rm_classification,
                         node_id,
-                        classificationResponse.status_code,
-                        classificationResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def registerWorkspaceTemplate(self, node_id: int):
@@ -4501,46 +4501,46 @@
             node_id (integer): node ID of the Extended ECM workspace template
         Return:
             Response (json) or None if the registration of the workspace template has failed.
         """
 
         registrationPostData = {"ids": "{{ {} }}".format(node_id)}
 
-        requestUrl = self.config()["xEngProjectTemplateUrl"]
+        request_url = self.config()["xEngProjectTemplateUrl"]
 
-        requestHeader = self.requestFormHeader()
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Register workspace template with ID -> {}; calling -> {}".format(
-                node_id, requestUrl
+                node_id, request_url
             )
         )
 
         retries = 0
         while True:
-            registrationResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 data=registrationPostData,
-                headers=requestHeader,
+                headers=request_header,
                 cookies=self.cookie(),
             )
-            if registrationResponse.ok:
-                return self.parseRequestResponse(registrationResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif registrationResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to register Workspace Template with ID -> {}; status -> {}; error -> {}".format(
                         node_id,
-                        registrationResponse.status_code,
-                        registrationResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def getRecordsManagementRSIs(self, limit: int = 100):
@@ -4587,40 +4587,40 @@
                 "Disposition": "string",
                 "ApprovalFlag": 0,
                 "MaximumRet": 0,
                 "ObjectType": "LIV"
             }
         """
 
-        requestUrl = self.config()["rsisUrl"] + "?limit=" + str(limit)
-        requestHeader = self.requestFormHeader()
+        request_url = self.config()["rsisUrl"] + "?limit=" + str(limit)
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Get list of Records Management RSIs; calling -> {}".format(
-                requestUrl)
+                request_url)
         )
 
         retries = 0
         while True:
-            rsisResponse = requests.get(
-                requestUrl, headers=requestHeader, cookies=self.cookie()
+            response = requests.get(
+                request_url, headers=request_header, cookies=self.cookie()
             )
-            if rsisResponse.ok:
-                rsi_dict = self.parseRequestResponse(rsisResponse)
+            if response.ok:
+                rsi_dict = self.parseRequestResponse(response)
                 return rsi_dict["results"]["data"]["rsis"]
             # Check if Session has expired - then re-authenticate and try once more
-            elif rsisResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to get list of Records Management RSIs; status -> {}; error -> {}".format(
-                        rsisResponse.status_code, rsisResponse.text
+                        response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def getRecordsManagementCodes(self):
@@ -4629,40 +4629,40 @@
            other higher-level Records Management configurations
 
         Args: None
         Return:
             RSI data (json) or None if the request fails.
         """
 
-        requestUrl = self.config()["recordsManagementUrlv2"] + "/rmcodes"
-        requestHeader = self.requestFormHeader()
+        request_url = self.config()["recordsManagementUrlv2"] + "/rmcodes"
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Get list of Records Management codes; calling -> {}".format(
-                requestUrl)
+                request_url)
         )
 
         retries = 0
         while True:
-            rmCodesResponse = requests.get(
-                requestUrl, headers=requestHeader, cookies=self.cookie()
+            response = requests.get(
+                request_url, headers=request_header, cookies=self.cookie()
             )
-            if rmCodesResponse.ok:
-                rm_codes_dict = self.parseRequestResponse(rmCodesResponse)
+            if response.ok:
+                rm_codes_dict = self.parseRequestResponse(response)
                 return rm_codes_dict["results"]["data"]
             # Check if Session has expired - then re-authenticate and try once more
-            elif rmCodesResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to get list of Records Management codes; status -> {}; error -> {}".format(
-                        rmCodesResponse.status_code, rmCodesResponse.text
+                        response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     # This is not yet working. REST API endpoint seems not to be in 22.4. Retest with 23.1
@@ -4675,41 +4675,41 @@
             rm_codes: dict with the updated codes
         Return:
             RSI data (json) or None if the request fails.
         """
 
         updateRMCodesPostData = {}
 
-        requestUrl = self.config()["recordsManagementUrl"] + "/rmcodes"
-        requestHeader = self.requestFormHeader()
+        request_url = self.config()["recordsManagementUrl"] + "/rmcodes"
+        request_header = self.requestFormHeader()
 
         logger.info(
-            "Update Records Management codes; calling -> {}".format(requestUrl))
+            "Update Records Management codes; calling -> {}".format(request_url))
 
         retries = 0
         while True:
-            rmCodesResponse = requests.post(
-                requestUrl,
-                headers=requestHeader,
+            response = requests.post(
+                request_url,
+                headers=request_header,
                 data=updateRMCodesPostData,
                 cookies=self.cookie(),
             )
-            if rmCodesResponse.ok:
-                rm_codes_dict = self.parseRequestResponse(rmCodesResponse)
+            if response.ok:
+                rm_codes_dict = self.parseRequestResponse(response)
                 return rm_codes_dict["results"]["data"]
             # Check if Session has expired - then re-authenticate and try once more
-            elif rmCodesResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to update Records Management codes; status -> {}; error -> {}".format(
-                        rmCodesResponse.status_code, rmCodesResponse.text
+                        response.status_code, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def createRecordsManagementRSI(
@@ -4746,46 +4746,46 @@
             "statusDate": status_date,
             "description": description,
             "subject": subject,
             "title": title,
             "dispcontrol": dispcontrol,
         }
 
-        requestUrl = self.config()["rsiSchedulesUrl"]
+        request_url = self.config()["rsiSchedulesUrl"]
 
-        requestHeader = self.requestFormHeader()
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Create Records Management RSI -> {}; calling -> {}".format(
-                name, requestUrl
+                name, request_url
             )
         )
 
         retries = 0
         while True:
-            rsiResponse = requests.post(
-                requestUrl,
-                headers=requestHeader,
+            response = requests.post(
+                request_url,
+                headers=request_header,
                 data=createRSIPostData,
                 cookies=self.cookie(),
             )
-            if rsiResponse.ok:
-                return self.parseRequestResponse(rsiResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif rsiResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to create Records Management RSI -> {}; status -> {}; error -> {}".format(
                         name,
-                        rsiResponse.status_code,
-                        rsiResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def createRecordsManagementRSISchedule(
@@ -4881,47 +4881,47 @@
             "newStatus": new_status,
             "minNumVersionsToKeep": min_num_versions_to_keep,
             "purgeSuperseded": purge_superseded,
             "purgeMajors": purge_majors,
             "markOfficialRendition": mark_official_rendition,
         }
 
-        requestUrl = self.config()["rsiSchedulesUrl"] + \
+        request_url = self.config()["rsiSchedulesUrl"] + \
             "/" + str(rsi_id) + "/stages"
 
-        requestHeader = self.requestFormHeader()
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Create Records Management RSI Schedule -> {} for RSI -> {}; calling -> {}".format(
-                stage, rsi_id, requestUrl
+                stage, rsi_id, request_url
             )
         )
 
         retries = 0
         while True:
-            rsiScheduleResponse = requests.post(
-                requestUrl,
-                headers=requestHeader,
+            response = requests.post(
+                request_url,
+                headers=request_header,
                 data=createRSISchedulePostData,
                 cookies=self.cookie(),
             )
-            if rsiScheduleResponse.ok:
-                return self.parseRequestResponse(rsiScheduleResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif rsiScheduleResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to create Records Management RSI Schedule -> {}; status -> {}; error -> {}".format(
                         stage,
-                        rsiScheduleResponse.status_code,
-                        rsiScheduleResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def createRecordsManagementHold(
@@ -4960,46 +4960,46 @@
             "date_to_remove": date_to_remove,
             "alternate_id": alternate_id,
         }
 
         if parent_id > 0:
             createHoldPostData["parent_id"] = parent_id
 
-        requestUrl = self.config()["holdsUrl"]
+        request_url = self.config()["holdsUrl"]
 
-        requestHeader = self.requestFormHeader()
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Create Records Management Hold -> {}; calling -> {}".format(
-                name, requestUrl
+                name, request_url
             )
         )
 
         retries = 0
         while True:
-            holdsResponse = requests.post(
-                requestUrl,
-                headers=requestHeader,
+            response = requests.post(
+                request_url,
+                headers=request_header,
                 data=createHoldPostData,
                 cookies=self.cookie(),
             )
-            if holdsResponse.ok:
-                return self.parseRequestResponse(holdsResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif holdsResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to create Records Management Hold -> {}; status -> {}; error -> {}".format(
                         name,
-                        holdsResponse.status_code,
-                        holdsResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def getRecordsManagementHolds(self):
@@ -5031,67 +5031,67 @@
                             "ParentID": 0
                         }
                     ]
                 }
             }
         """
 
-        requestUrl = self.config()["holdsUrlv2"]
+        request_url = self.config()["holdsUrlv2"]
 
-        requestHeader = self.requestFormHeader()
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Get list of Records Management Holds; calling -> {}".format(
-                requestUrl
+                request_url
             )
         )
 
         retries = 0
         while True:
-            holdsResponse = requests.get(
-                requestUrl,
-                headers=requestHeader,
+            response = requests.get(
+                request_url,
+                headers=request_header,
                 cookies=self.cookie(),
             )
-            if holdsResponse.ok:
-                return self.parseRequestResponse(holdsResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif holdsResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to get list of Records Management Holds; status -> {}; error -> {}".format(
-                        holdsResponse.status_code,
-                        holdsResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def importRecordsManagementSettings(self, file_path: str):
         """Import Records Management settings from a file that is uploaded from the python pod
         Args:
             file_path (string): path + filename of config file in Python container filesystem
         Return:
             True if if the REST call succeeds or False otherwise.
         """
 
-        requestUrl = self.config()["recordsManagementUrl"] + "/importSettings"
+        request_url = self.config()["recordsManagementUrl"] + "/importSettings"
 
-        requestHeader = (
+        request_header = (
             self.cookie()
         )  # for some reason we have to omit the other header parts here - otherwise we get a 400 response
 
         logger.info(
             "Importing Records Management Settings from file -> {}; calling -> {}".format(
-                file_path, requestUrl
+                file_path, request_url
             )
         )
 
         filename = os.path.basename(file_path)
         if not os.path.exists(file_path):
             logger.error(
                 "The file -> {} does not exist in path -> {}!".format(
@@ -5099,34 +5099,34 @@
                 )
             )
             return False
         settingsPostFile = {"file": (filename, open(file_path), "text/xml")}
 
         retries = 0
         while True:
-            settingsResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 files=settingsPostFile,
-                headers=requestHeader,
+                headers=request_header,
                 cookies=self.cookie(),
             )
-            if settingsResponse.ok:
+            if response.ok:
                 return True
             # Check if Session has expired - then re-authenticate and try once more
-            elif settingsResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to import Records Management Settings from file -> {}; status -> {}; error -> {}".format(
                         file_path,
-                        settingsResponse.status_code,
-                        settingsResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return False
 
     # end method definition
 
     def importRecordsManagementCodes(
@@ -5137,23 +5137,23 @@
             file_path (string): path + filename of settings file in Python container filesystem
             update_existing_codes (boolean): Flag that controls whether existing table maintenance codes
                                              should be updated.
         Return:
             True if if the REST call succeeds or False otherwise.
         """
 
-        requestUrl = self.config()["recordsManagementUrl"] + "/importCodes"
+        request_url = self.config()["recordsManagementUrl"] + "/importCodes"
 
-        requestHeader = (
+        request_header = (
             self.cookie()
         )  # for some reason we have to omit the other header parts here - otherwise we get a 400 response
 
         logger.info(
             "Importing Records Management Codes from file -> {}; calling -> {}".format(
-                file_path, requestUrl
+                file_path, request_url
             )
         )
 
         settingsPostData = {"updateExistingCodes": update_existing_codes}
 
         filename = os.path.basename(file_path)
         if not os.path.exists(file_path):
@@ -5163,35 +5163,35 @@
                 )
             )
             return False
         settingsPostFile = {"file": (filename, open(file_path), "text/xml")}
 
         retries = 0
         while True:
-            settingsResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 data=settingsPostData,
                 files=settingsPostFile,
-                headers=requestHeader,
+                headers=request_header,
                 cookies=self.cookie(),
             )
-            if settingsResponse.ok:
+            if response.ok:
                 return True
             # Check if Session has expired - then re-authenticate and try once more
-            elif settingsResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to import Records Management Codes from file -> {}; status -> {}; error -> {}".format(
                         file_path,
-                        settingsResponse.status_code,
-                        settingsResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return False
 
     # end method definition
 
     def importRecordsManagementRSIs(
@@ -5205,23 +5205,23 @@
             file_path (string): path + filename of config file in Python container filesystem
             update_existing_rsis (boolean): whether or not existing RSIs should be updated (or ignored)
             delete_schedules (boolean): whether RSI Schedules should be deleted
         Return:
             True if if the REST call succeeds or False otherwise.
         """
 
-        requestUrl = self.config()["recordsManagementUrl"] + "/importRSIs"
+        request_url = self.config()["recordsManagementUrl"] + "/importRSIs"
 
-        requestHeader = (
+        request_header = (
             self.cookie()
         )  # for some reason we have to omit the other header parts here - otherwise we get a 400 response
 
         logger.info(
             "Importing Records Management RSIs from file -> {}; calling -> {}".format(
-                file_path, requestUrl
+                file_path, request_url
             )
         )
 
         settingsPostData = {
             "updateExistingRSIs": update_existing_rsis,
             "deleteSchedules": delete_schedules,
         }
@@ -5234,58 +5234,58 @@
                 )
             )
             return False
         settingsPostFile = {"file": (filename, open(file_path), "text/xml")}
 
         retries = 0
         while True:
-            settingsResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 data=settingsPostData,
                 files=settingsPostFile,
-                headers=requestHeader,
+                headers=request_header,
                 cookies=self.cookie(),
             )
-            if settingsResponse.ok:
+            if response.ok:
                 return True
             # Check if Session has expired - then re-authenticate and try once more
-            elif settingsResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to import Records Management RSIs from file -> {}; status -> {}; error -> {}".format(
                         file_path,
-                        settingsResponse.status_code,
-                        settingsResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return False
 
     # end method definition
 
     def importPhysicalObjectsSettings(self, file_path: str):
         """Import Physical Objects settings from a config file that is uploaded from the python pod
         Args:
             file_path (string): path + filename of config file in Python container filesystem
         Return:
             True if if the REST call succeeds or False otherwise.
         """
 
-        requestUrl = self.config()["physicalObjectsUrl"] + "/importSettings"
+        request_url = self.config()["physicalObjectsUrl"] + "/importSettings"
 
-        requestHeader = (
+        request_header = (
             self.cookie()
         )  # for some reason we have to omit the other header parts here - otherwise we get a 400 response
 
         logger.info(
             "Importing Physical Objects Settings from server file -> {}; calling -> {}".format(
-                file_path, requestUrl
+                file_path, request_url
             )
         )
 
         filename = os.path.basename(file_path)
         if not os.path.exists(file_path):
             logger.error(
                 "The file -> {} does not exist in path -> {}!".format(
@@ -5293,34 +5293,34 @@
                 )
             )
             return False
         settingsPostFile = {"file": (filename, open(file_path), "text/xml")}
 
         retries = 0
         while True:
-            settingsResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 files=settingsPostFile,
-                headers=requestHeader,
+                headers=request_header,
                 cookies=self.cookie(),
             )
-            if settingsResponse.ok:
+            if response.ok:
                 return True
             # Check if Session has expired - then re-authenticate and try once more
-            elif settingsResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to import Physical Objects settings from file -> {}; status -> {}; error -> {}".format(
                         file_path,
-                        settingsResponse.status_code,
-                        settingsResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return False
 
     # end method definition
 
     def importPhysicalObjectsCodes(
@@ -5330,23 +5330,23 @@
         Args:
             file_path (string): path + filename of config file in Python container filesystem
             update_existing_codes (boolean): whether or not existing codes should be updated (default = True)
         Return:
             True if if the REST call succeeds or False otherwise.
         """
 
-        requestUrl = self.config()["physicalObjectsUrl"] + "/importCodes"
+        request_url = self.config()["physicalObjectsUrl"] + "/importCodes"
 
-        requestHeader = (
+        request_header = (
             self.cookie()
         )  # for some reason we have to omit the other header parts here - otherwise we get a 400 response
 
         logger.info(
             "Importing Physical Objects Codes from file -> {}; calling -> {}".format(
-                file_path, requestUrl
+                file_path, request_url
             )
         )
 
         settingsPostData = {"updateExistingCodes": update_existing_codes}
 
         filename = os.path.basename(file_path)
         if not os.path.exists(file_path):
@@ -5356,58 +5356,58 @@
                 )
             )
             return False
         settingsPostFile = {"file": (filename, open(file_path), "text/xml")}
 
         retries = 0
         while True:
-            settingsResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 data=settingsPostData,
                 files=settingsPostFile,
-                headers=requestHeader,
+                headers=request_header,
                 cookies=self.cookie(),
             )
-            if settingsResponse.ok:
+            if response.ok:
                 return True
             # Check if Session has expired - then re-authenticate and try once more
-            elif settingsResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to import Physical Objects Codes from file -> {}; status -> {}; error -> {}".format(
                         file_path,
-                        settingsResponse.status_code,
-                        settingsResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return False
 
     # end method definition
 
     def importPhysicalObjectsLocators(self, file_path: str):
         """Import Physical Objects locators from a config file that is uploaded from the python pod
         Args:
             file_path (string): path + filename of config file in Python container filesystem
         Return:
             True if if the REST call succeeds or False otherwise.
         """
 
-        requestUrl = self.config()["physicalObjectsUrl"] + "/importLocators"
+        request_url = self.config()["physicalObjectsUrl"] + "/importLocators"
 
-        requestHeader = (
+        request_header = (
             self.cookie()
         )  # for some reason we have to omit the other header parts here - otherwise we get a 400 response
 
         logger.info(
             "Importing Physical Objects Locators from file -> {}; calling -> {}".format(
-                file_path, requestUrl
+                file_path, request_url
             )
         )
 
         filename = os.path.basename(file_path)
         if not os.path.exists(file_path):
             logger.error(
                 "The file -> {} does not exist in path -> {}!".format(
@@ -5415,34 +5415,34 @@
                 )
             )
             return False
         settingsPostFile = {"file": (filename, open(file_path), "text/xml")}
 
         retries = 0
         while True:
-            settingsResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 files=settingsPostFile,
-                headers=requestHeader,
+                headers=request_header,
                 cookies=self.cookie(),
             )
-            if settingsResponse.ok:
+            if response.ok:
                 return True
             # Check if Session has expired - then re-authenticate and try once more
-            elif settingsResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to import Physical Objects Locators from file -> {}; status -> {}; error -> {}".format(
                         file_path,
-                        settingsResponse.status_code,
-                        settingsResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return False
 
     # end method definition
 
     def importSecurityClearanceCodes(self, file_path: str, include_users: bool = False):
@@ -5450,23 +5450,23 @@
         Args:
             file_path (string): path + filename of config file in Python container filesystem
             include_users (boolean): defines if users should be included or not
         Return:
             True if if the REST call succeeds or False otherwise.
         """
 
-        requestUrl = self.config()["securityClearancesUrl"] + "/importCodes"
+        request_url = self.config()["securityClearancesUrl"] + "/importCodes"
 
-        requestHeader = (
+        request_header = (
             self.cookie()
         )  # for some reason we have to omit the other header parts here - otherwise we get a 400 response
 
         logger.info(
             "Importing Security Clearance Codes from file -> {}; calling -> {}".format(
-                file_path, requestUrl
+                file_path, request_url
             )
         )
 
         settingsPostData = {"includeusers": include_users}
 
         filename = os.path.basename(file_path)
         if not os.path.exists(file_path):
@@ -5476,35 +5476,35 @@
                 )
             )
             return False
         settingsPostFile = {"file": (filename, open(file_path), "text/xml")}
 
         retries = 0
         while True:
-            settingsResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 data=settingsPostData,
                 files=settingsPostFile,
-                headers=requestHeader,
+                headers=request_header,
                 cookies=self.cookie(),
             )
-            if settingsResponse.ok:
+            if response.ok:
                 return True
             # Check if Session has expired - then re-authenticate and try once more
-            elif settingsResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to import Security Clearance Codes from file -> {}; status -> {}; error -> {}".format(
                         file_path,
-                        settingsResponse.status_code,
-                        settingsResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return False
 
     # end method definition
 
     def assignUserSecurityClearance(self, user_id: int, security_clearance: int):
@@ -5517,48 +5517,48 @@
             REST response or None if the REST call fails.
         """
 
         assignUserSecurityClearancePostData = {
             "securityLevel": security_clearance,
         }
 
-        requestUrl = self.config()[
+        request_url = self.config()[
             "userSecurityUrl"
         ] + "/{}/securityclearancelevel".format(user_id)
-        requestHeader = self.requestFormHeader()
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Assign security clearance -> {} to user ID -> {}; calling -> {}".format(
-                security_clearance, user_id, requestUrl
+                security_clearance, user_id, request_url
             )
         )
 
         retries = 0
         while True:
-            securityClearanceResponse = requests.post(
-                requestUrl,
-                headers=requestHeader,
+            response = requests.post(
+                request_url,
+                headers=request_header,
                 data=assignUserSecurityClearancePostData,
                 cookies=self.cookie(),
             )
-            if securityClearanceResponse.ok:
-                return self.parseRequestResponse(securityClearanceResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif securityClearanceResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to assign security clearance -> {} to user -> {}; status -> {}; error -> {}".format(
                         user_id,
                         security_clearance,
-                        securityClearanceResponse.status_code,
-                        securityClearanceResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def assignUserSupplementalMarkings(self, user_id: int, supplemental_markings: list):
@@ -5572,48 +5572,48 @@
             REST response or None if the REST call fails.
         """
 
         assignUserSupplementalMarkingsPostData = {
             "suppMarks": supplemental_markings,
         }
 
-        requestUrl = self.config()[
+        request_url = self.config()[
             "userSecurityUrl"
         ] + "/{}/supplementalmarkings".format(user_id)
-        requestHeader = self.requestFormHeader()
+        request_header = self.requestFormHeader()
 
         logger.info(
             "Assign supplemental markings -> {} to user ID -> {}; calling -> {}".format(
-                supplemental_markings, user_id, requestUrl
+                supplemental_markings, user_id, request_url
             )
         )
 
         retries = 0
         while True:
-            supplementalMarkingsResponse = requests.post(
-                requestUrl,
-                headers=requestHeader,
+            response = requests.post(
+                request_url,
+                headers=request_header,
                 data=assignUserSupplementalMarkingsPostData,
                 cookies=self.cookie(),
             )
-            if supplementalMarkingsResponse.ok:
-                return self.parseRequestResponse(supplementalMarkingsResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif supplementalMarkingsResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning(
                     "Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to assign supplemental markings -> {} to user -> {}; status -> {}; error -> {}".format(
                         user_id,
                         supplemental_markings,
-                        supplementalMarkingsResponse.status_code,
-                        supplementalMarkingsResponse.text,
+                        response.status_code,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def volumeTranslator(self, current_node_id: int, translator: object, languages: list):
@@ -5641,7 +5641,9 @@
         response = self.renameNode(current_node_id, name, description, names_multilingual, descriptions_multilingual)
 
         # Get children nodes of the current node:
         results = self.getSubnodes(current_node_id, limit=200)["results"]
 
         for result in results:
             self.volumeTranslator(result["data"]["properties"]["id"], translator, languages)
+
+    # end method definition
```

### Comparing `pyxecm-0.0.14/pyxecm/otds.py` & `pyxecm-0.0.15/pyxecm/otds.py`

 * *Files 4% similar despite different names*

```diff
@@ -279,37 +279,37 @@
         if self._cookie and not revalidate:
             return self._cookie
 
         otds_ticket = "NotSet"
 
         logger.info("Requesting OTDS ticket from {}".format(self.credentialUrl()))
 
-        authenticateResponse = None
+        response = None
         try:
-            authenticateResponse = requests.post(
+            response = requests.post(
                 self.credentialUrl(), json=self.credentials(), headers=requestHeaders
             )
         except Exception as e:
             logger.warning(
                 "Unable to connect to -> {} : {}".format(self.credentialUrl(), e)
             )
             logger.warning("OTDS service may not be ready yet.")
             return None
 
-        if authenticateResponse.ok:
-            authenticate_dict = self.parseRequestResponse(authenticateResponse)
+        if response.ok:
+            authenticate_dict = self.parseRequestResponse(response)
             if not authenticate_dict:
                 return None
             else:
                 otds_ticket = authenticate_dict["ticket"]
                 logger.info("Ticket -> {}".format(otds_ticket))
         else:
             logger.error(
                 "Failed to request an OTDS ticket; error -> {}".format(
-                    authenticateResponse.text
+                    response.text
                 )
             )
             return None
 
         self._cookie = {"OTDSTicket": otds_ticket}
         return self._cookie
 
@@ -332,16 +332,16 @@
             resource_id (string): OTDS resource ID (this is ID not the resource name!)
             update (boolean): whether or not an existing license should be updated
         Return: Request response (json) or None if the REST call fails
         """
 
         logger.info("Reading license file -> {}...".format(path_to_license_file))
         try:
-            with open(path_to_license_file) as licenseFile:
-                license_content = licenseFile.read()
+            with open(path_to_license_file) as license_file:
+                license_content = license_file.read()
         except IOError as e:
             logger.error(
                 "Error opening license file -> {}; error -> {}".format(
                     path_to_license_file, e.strerror
                 )
             )
             return None
@@ -352,112 +352,112 @@
             "values": [
                 {"name": "oTLicenseFile", "values": license_content},
                 {"name": "oTLicenseResource", "values": resource_id},
                 {"name": "oTLicenseFingerprintGenerator", "values": [None]},
             ],
         }
 
-        requestUrl = self.licenseUrl()
+        request_url = self.licenseUrl()
         # Check if we want to update an existing license:
         if update:
             existing_license = self.getLicensesForResource(resource_id)
             if existing_license:
-                requestUrl += "/" + existing_license[0]["id"]
+                request_url += "/" + existing_license[0]["id"]
             else:
                 logger.info(
                     "No existing license for resource -> {} found - adding a new license...".format(
                         resource_id
                     )
                 )
                 # change strategy to create a new license:
                 update = False
 
         logger.info(
             "Adding product license -> {} for product -> {} to resource -> {}; calling -> {}".format(
-                path_to_license_file, product_description, resource_id, requestUrl
+                path_to_license_file, product_description, resource_id, request_url
             )
         )
 
         retries = 0
         while True:
             if update:
                 # Do a REST PUT call for update an existing license:
-                uploadLicenseResponse = requests.put(
-                    requestUrl,
+                response = requests.put(
+                    request_url,
                     json=licensePostBodyJson,
                     headers=requestHeaders,
                     cookies=self.cookie(),
                 )
             else:
                 # Do a REST POST call for creation of a new license:
-                uploadLicenseResponse = requests.post(
-                    requestUrl,
+                response = requests.post(
+                    request_url,
                     json=licensePostBodyJson,
                     headers=requestHeaders,
                     cookies=self.cookie(),
                 )
-            if uploadLicenseResponse.ok:
-                return self.parseRequestResponse(uploadLicenseResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif uploadLicenseResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to add product license -> {} for product -> {}; error -> {}".format(
                         path_to_license_file,
                         product_description,
-                        uploadLicenseResponse.text,
+                        response.text,
                     )
                 )
                 return None
 
     # end method definition
 
     def getLicensesForResource(self, resource_id: str):
         """Get a product license for a resource in OTDS.
 
         Args:
             resource_id (string): OTDS resource ID (this is ID not the resource name!)
         Return: Licenses for a resource or None if the REST call fails
         """
 
-        requestUrl = (
+        request_url = (
             self.licenseUrl()
             + "/assignedlicenses?resourceID="
             + resource_id
             + "&validOnly=false"
         )
 
         logger.info(
             "Get license for resource -> {}; calling -> {}".format(
-                resource_id, requestUrl
+                resource_id, request_url
             )
         )
 
         retries = 0
         while True:
-            licenseResponse = requests.get(
-                requestUrl, headers=requestHeaders, cookies=self.cookie()
+            response = requests.get(
+                request_url, headers=requestHeaders, cookies=self.cookie()
             )
-            if licenseResponse.ok:
-                response_dict = self.parseRequestResponse(licenseResponse)
+            if response.ok:
+                response_dict = self.parseRequestResponse(response)
                 if not response_dict:
                     return None
                 return response_dict["licenseObjects"]["_licenses"]
             # Check if Session has expired - then re-authenticate and try once more
-            elif licenseResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to get license for resource -> {}; error -> {}".format(
-                        resource_id, licenseResponse.text
+                        resource_id, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def deleteLicenseFromResource(self, resource_id: str, license_id: str):
@@ -465,38 +465,38 @@
 
         Args:
             resource_id (string): OTDS resource ID (this is ID not the resource name!)
             licenseId (string): OTDS license ID (this is the ID not the license name!)
         Return: True if successful or False if the REST call fails
         """
 
-        requestUrl = "{}/{}".format(self.licenseUrl(), license_id)
+        request_url = "{}/{}".format(self.licenseUrl(), license_id)
 
         logger.info(
             "Deleting product license -> {} from resource -> {}; calling -> {}".format(
-                license_id, resource_id, requestUrl
+                license_id, resource_id, request_url
             )
         )
 
         retries = 0
         while True:
-            deleteResponse = requests.delete(
-                requestUrl, headers=requestHeaders, cookies=self.cookie()
+            response = requests.delete(
+                request_url, headers=requestHeaders, cookies=self.cookie()
             )
-            if deleteResponse.ok:
+            if response.ok:
                 return True
             # Check if Session has expired - then re-authenticate and try once more
-            elif deleteResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to delete license -> {} for resource -> {}; error -> {}".format(
-                        license_id, resource_id, deleteResponse.text
+                        license_id, resource_id, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def assignUserToLicense(
@@ -546,49 +546,49 @@
         licensePostBodyJson = {
             "_oTLicenseType": license_type,
             "_oTLicenseProduct": "users",
             "name": userLocation,
             "values": [{"name": "counter", "values": [license_feature]}],
         }
 
-        requestUrl = self.licenseUrl() + "/object/" + licenseLocation
+        request_url = self.licenseUrl() + "/object/" + licenseLocation
 
         logger.info(
             "Assign license feature -> {} of license -> {} associated with resource -> {} to user -> {}; calling -> {}".format(
-                license_feature, licenseLocation, resource_id, user_id, requestUrl
+                license_feature, licenseLocation, resource_id, user_id, request_url
             )
         )
 
         retries = 0
         while True:
-            addLicenseResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 json=licensePostBodyJson,
                 headers=requestHeaders,
                 cookies=self.cookie(),
             )
-            if addLicenseResponse.ok:
+            if response.ok:
                 logger.info(
                     "Added license feature -> {} for user -> {}".format(
                         license_feature, user_id
                     )
                 )
                 return True
             # Check if Session has expired - then re-authenticate and try once more
-            elif addLicenseResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to add license feature -> {} associated with resource -> {} for user -> {}; status code -> {}".format(
                         license_feature,
                         resource_id,
                         user_id,
-                        addLicenseResponse.status_code,
+                        response.status_code,
                     )
                 )
                 return False
 
     # end method definition
 
     def addPartition(self, name: str, description: str):
@@ -598,41 +598,41 @@
             name (string): name of the new partition
         Return:
             Request response (json) or None if the creation fails.
         """
 
         partitionPostBodyJson = {"name": name, "description": description}
 
-        requestUrl = self.partitionUrl()
+        request_url = self.partitionUrl()
 
         logger.info(
             "Adding user partition -> {} ({}); calling -> {}".format(
-                name, description, requestUrl
+                name, description, request_url
             )
         )
 
         retries = 0
         while True:
-            partitionResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 json=partitionPostBodyJson,
                 headers=requestHeaders,
                 cookies=self.cookie(),
             )
-            if partitionResponse.ok:
-                return self.parseRequestResponse(partitionResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif partitionResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to add user partition -> {}; error -> {}".format(
-                        name, partitionResponse.text
+                        name, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def getPartition(self, name: str, show_error: bool = True):
@@ -641,37 +641,37 @@
         Args:
             name (string): name of the partition to retrieve
             show_error (boolean): whether or not we want to log an error if partion is not found
         Return:
             Request response (json) or None if the creation fails.
         """
 
-        requestUrl = "{}/{}".format(self.config()["partitionUrl"], name)
+        request_url = "{}/{}".format(self.config()["partitionUrl"], name)
 
         logger.info(
-            "Getting user partition -> {}; calling -> {}".format(name, requestUrl)
+            "Getting user partition -> {}; calling -> {}".format(name, request_url)
         )
 
         retries = 0
         while True:
-            partitionResponse = requests.get(
-                requestUrl, headers=requestHeaders, cookies=self.cookie()
+            response = requests.get(
+                request_url, headers=requestHeaders, cookies=self.cookie()
             )
-            if partitionResponse.ok:
-                return self.parseRequestResponse(partitionResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif partitionResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 if show_error:
                     logger.error(
                         "Failed to get partition -> {}; warning -> {}".format(
-                            name, partitionResponse.text
+                            name, response.text
                         )
                     )
                 return None
 
     # end method definition
 
     def addUser(
@@ -703,42 +703,42 @@
                 {"name": "givenName", "values": [first_name]},
                 {"name": "mail", "values": [email]},
             ],
             "name": name,
             "description": description,
         }
 
-        requestUrl = self.usersUrl()
+        request_url = self.usersUrl()
 
         logger.info(
             "Adding user -> {} to partition -> {}; calling -> {}".format(
-                name, partition, requestUrl
+                name, partition, request_url
             )
         )
         logger.debug("User Attributes -> {}".format(userPostBodyJson))
 
         retries = 0
         while True:
-            userResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 json=userPostBodyJson,
                 headers=requestHeaders,
                 cookies=self.cookie(),
             )
-            if userResponse.ok:
-                return self.parseRequestResponse(userResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif userResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to add user -> {}; error -> {}".format(
-                        name, userResponse.text
+                        name, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def getUser(self, partition: str, user_id: str):
@@ -747,38 +747,38 @@
         Args:
             partition (string): name of the partition
             user_id (string): ID of the user (= login name)
         Return:
             Request response (json) or None if the creation fails.
         """
 
-        requestUrl = self.usersUrl() + "/" + user_id + "@" + partition
+        request_url = self.usersUrl() + "/" + user_id + "@" + partition
 
         logger.info(
             "Get user -> {} in partition -> {}; calling -> {}".format(
-                user_id, partition, requestUrl
+                user_id, partition, request_url
             )
         )
 
         retries = 0
         while True:
-            userResponse = requests.get(
-                requestUrl, headers=requestHeaders, cookies=self.cookie()
+            response = requests.get(
+                request_url, headers=requestHeaders, cookies=self.cookie()
             )
-            if userResponse.ok:
-                return self.parseRequestResponse(userResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif userResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to get user -> {}; error -> {}".format(
-                        user_id, userResponse.text
+                        user_id, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def updateUser(
@@ -796,41 +796,41 @@
         """
 
         userPatchBodyJson = {
             "userPartitionID": partition,
             "values": [{"name": attribute_name, "values": [attribute_value]}],
         }
 
-        requestUrl = self.usersUrl() + "/" + user_id
+        request_url = self.usersUrl() + "/" + user_id
 
         logger.info(
             "Update user -> {} attribute -> {} to value -> {}; calling -> {}".format(
-                user_id, attribute_name, attribute_value, requestUrl
+                user_id, attribute_name, attribute_value, request_url
             )
         )
 
         retries = 0
         while True:
-            userResponse = requests.patch(
-                requestUrl,
+            response = requests.patch(
+                request_url,
                 json=userPatchBodyJson,
                 headers=requestHeaders,
                 cookies=self.cookie(),
             )
-            if userResponse.ok:
-                return self.parseRequestResponse(userResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif userResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to update user -> {}; error -> {}".format(
-                        user_id, userResponse.text
+                        user_id, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def deleteUser(self, partition: str, user_id: str):
@@ -839,38 +839,38 @@
         Args:
             partition (string): name of the partition
             user_id (string): Id (= login name) of the user
         Return:
             Request response (json) or None if the reset fails.
         """
 
-        requestUrl = self.usersUrl() + "/" + user_id + "@" + partition
+        request_url = self.usersUrl() + "/" + user_id + "@" + partition
 
         logger.info(
             "Delete user -> {} in partition -> {}; calling -> {}".format(
-                user_id, partition, requestUrl
+                user_id, partition, request_url
             )
         )
 
         retries = 0
         while True:
-            userResponse = requests.delete(
-                requestUrl, headers=requestHeaders, cookies=self.cookie()
+            response = requests.delete(
+                request_url, headers=requestHeaders, cookies=self.cookie()
             )
-            if userResponse.ok:
+            if response.ok:
                 return True
             # Check if Session has expired - then re-authenticate and try once more
-            elif userResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to delete user -> {}; error -> {}".format(
-                        user_id, userResponse.text
+                        user_id, response.text
                     )
                 )
                 return False
 
     # end method definition
 
     def resetUserPassword(self, user_id: str, password: str):
@@ -881,44 +881,44 @@
             password (string): new password of the user
         Return:
             Request response (json) or None if the reset fails.
         """
 
         userPostBodyJson = {"newPassword": password}
 
-        requestUrl = "{}/{}/password".format(self.usersUrl(), user_id)
+        request_url = "{}/{}/password".format(self.usersUrl(), user_id)
 
         logger.info(
             "Resetting password for user -> {}; calling -> {}".format(
-                user_id, requestUrl
+                user_id, request_url
             )
         )
 
         retries = 0
         while True:
-            userResponse = requests.put(
-                requestUrl,
+            response = requests.put(
+                request_url,
                 json=userPostBodyJson,
                 headers=requestHeaders,
                 cookies=self.cookie(),
             )
-            if userResponse.ok:
-                return userResponse.ok
+            if response.ok:
+                return response.ok
             # Check if Session has expired - then re-authenticate and try once more
-            elif userResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to reset password for user -> {}; error -> {}".format(
-                        user_id, userResponse.text
+                        user_id, response.text
                     )
                 )
-                return userResponse.ok
+                return response.ok
 
     # end method definition
 
     def addGroup(self, partition: str, name: str, description: str):
         """Add a new user group to a user partition in OTDS
 
         Args:
@@ -931,42 +931,42 @@
 
         groupPostBodyJson = {
             "userPartitionID": partition,
             "name": name,
             "description": description,
         }
 
-        requestUrl = self.groupsUrl()
+        request_url = self.groupsUrl()
 
         logger.info(
             "Adding group -> {} to partition -> {}; calling -> {}".format(
-                name, partition, requestUrl
+                name, partition, request_url
             )
         )
         logger.info("Group Attributes -> {}".format(groupPostBodyJson))
 
         retries = 0
         while True:
-            groupResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 json=groupPostBodyJson,
                 headers=requestHeaders,
                 cookies=self.cookie(),
             )
-            if groupResponse.ok:
-                return self.parseRequestResponse(groupResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif groupResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to add group -> {}; error -> {}".format(
-                        name, groupResponse.text
+                        name, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def getGroup(self, group: str):
@@ -990,34 +990,34 @@
                 'customAttributes': None,
                 'originUUID': None,
                 'urlId': 'Sales@Content Server Members',
                 'urlLocation': 'oTGroup=3f921294-b92a-4c9e-bf7c-b50df16bb937,orgunit=groups,partition=Content Server Members,dc=identity,dc=opentext,dc=net'
             }
         """
 
-        requestUrl = self.groupsUrl() + "/" + group
+        request_url = self.groupsUrl() + "/" + group
 
-        logger.info("Get group -> {}; calling -> {}".format(group, requestUrl))
+        logger.info("Get group -> {}; calling -> {}".format(group, request_url))
 
         retries = 0
         while True:
-            groupResponse = requests.get(
-                requestUrl, headers=requestHeaders, cookies=self.cookie()
+            response = requests.get(
+                request_url, headers=requestHeaders, cookies=self.cookie()
             )
-            if groupResponse.ok:
-                return self.parseRequestResponse(groupResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif groupResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to get group -> {}; error -> {}".format(
-                        group, groupResponse.text
+                        group, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def addUserToGroup(self, user: str, group: str):
@@ -1028,41 +1028,41 @@
             group (string): name of the OTDS group (needs to exist)
         Return:
             Request return code.
         """
 
         userToGroupPostBodyJson = {"stringList": [group]}
 
-        requestUrl = self.usersUrl() + "/" + user + "/memberof"
+        request_url = self.usersUrl() + "/" + user + "/memberof"
 
         logger.info(
             "Adding user -> {} to group -> {}; calling -> {}".format(
-                user, group, requestUrl
+                user, group, request_url
             )
         )
 
         retries = 0
         while True:
-            userToGroupResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 json=userToGroupPostBodyJson,
                 headers=requestHeaders,
                 cookies=self.cookie(),
             )
-            if userToGroupResponse.ok:
+            if response.ok:
                 return True
             # Check if Session has expired - then re-authenticate and try once more
-            elif userToGroupResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to add user -> {} to group -> {}; error -> {}".format(
-                        user, group, userToGroupResponse.text
+                        user, group, response.text
                     )
                 )
                 return False
 
     # end method definition
 
     def addGroupToParentGroup(self, group: str, parent_group: str):
@@ -1073,42 +1073,42 @@
             parent_group (string): name of the OTDS parent group (needs to exist)
         Return:
             Request return code.
         """
 
         groupToParentGroupPostBodyJson = {"stringList": [parent_group]}
 
-        requestUrl = self.groupsUrl() + "/" + group + "/memberof"
+        request_url = self.groupsUrl() + "/" + group + "/memberof"
 
         logger.info(
             "Adding group -> {} to parent group -> {}; calling -> {}".format(
-                group, parent_group, requestUrl
+                group, parent_group, request_url
             )
         )
 
         retries = 0
         while True:
-            groupToParentGroupResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 json=groupToParentGroupPostBodyJson,
                 headers=requestHeaders,
                 cookies=self.cookie(),
             )
 
-            if groupToParentGroupResponse.ok:
+            if response.ok:
                 return True
             # Check if Session has expired - then re-authenticate and try once more
-            elif groupToParentGroupResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to add group -> {} to parent group -> {}; error -> {}".format(
-                        group, parent_group, groupToParentGroupResponse.text
+                        group, parent_group, response.text
                     )
                 )
                 return False
 
     # end method definition
 
     def addResource(
@@ -1136,41 +1136,41 @@
         }
 
         # Check if there's additional payload for the body provided to handle special cases:
         if additional_payload:
             # Merge additional payload:
             resourcePostBodyJson.update(additional_payload)
 
-        requestUrl = self.config()["resourceUrl"]
+        request_url = self.config()["resourceUrl"]
 
         logger.info(
             "Adding resource -> {} ({}); calling -> {}".format(
-                name, description, requestUrl
+                name, description, request_url
             )
         )
 
         retries = 0
         while True:
-            resourceResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 json=resourcePostBodyJson,
                 headers=requestHeaders,
                 cookies=self.cookie(),
             )
-            if resourceResponse.ok:
-                return self.parseRequestResponse(resourceResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif resourceResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to add resource -> {}; error -> {}".format(
-                        name, resourceResponse.text
+                        name, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def getResource(self, name: str, show_error: bool = False):
@@ -1179,37 +1179,37 @@
         Args:
             name (string): name of the new OTDS resource
             show_error (boolean): treat as error if resource is not found
         Return:
             Request response (json) or None if the REST call fails.
         """
 
-        requestUrl = "{}/{}".format(self.config()["resourceUrl"], name)
+        request_url = "{}/{}".format(self.config()["resourceUrl"], name)
 
-        logger.info("Retrieving resource -> {}; calling -> {}".format(name, requestUrl))
+        logger.info("Retrieving resource -> {}; calling -> {}".format(name, request_url))
 
         retries = 0
         while True:
-            resourceResponse = requests.get(
-                requestUrl, headers=requestHeaders, cookies=self.cookie()
+            response = requests.get(
+                request_url, headers=requestHeaders, cookies=self.cookie()
             )
-            if resourceResponse.ok:
-                return self.parseRequestResponse(resourceResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif resourceResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 # We don't necessarily want to log an error as this function
                 # is also used in wait loops:
                 if show_error:
                     logger.warning(
                         "Failed to retrieve resource -> {}; warning -> {}".format(
-                            name, resourceResponse.text
+                            name, response.text
                         )
                     )
                 else:
                     logger.info("Resource -> {} not found.".format(name))
                 return None
 
     # end method definition
@@ -1221,37 +1221,37 @@
             name (string): name of the new OTDS resource
             resource (object): updated resource object of getResource called before
             show_error (boolean): treat as error if resource is not found
         Return:
             Request response (json) or None if the REST call fails.
         """
 
-        requestUrl = "{}/{}".format(self.config()["resourceUrl"], name)
+        request_url = "{}/{}".format(self.config()["resourceUrl"], name)
 
-        logger.info("Updating resource -> {}; calling -> {}".format(name, requestUrl))
+        logger.info("Updating resource -> {}; calling -> {}".format(name, request_url))
 
         retries = 0
         while True:
-            resourceResponse = requests.put(
-                requestUrl, json=resource, headers=requestHeaders, cookies=self.cookie()
+            response = requests.put(
+                request_url, json=resource, headers=requestHeaders, cookies=self.cookie()
             )
-            if resourceResponse.ok:
-                return self.parseRequestResponse(resourceResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif resourceResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 # We don't necessarily want to log an error as this function
                 # is also used in wait loops:
                 if show_error:
                     logger.warning(
                         "Failed to retrieve resource -> {}; warning -> {}".format(
-                            name, resourceResponse.text
+                            name, response.text
                         )
                     )
                 else:
                     logger.info("Resource -> {} not found.".format(name))
                 return None
 
     # end method definition
@@ -1263,73 +1263,73 @@
             resource_id (string): ID of the OTDS resource
         Return:
             Request response (json) or None if the REST call fails.
         """
 
         resourcePostBodyJson = {}
 
-        requestUrl = "{}/{}/activate".format(self.config()["resourceUrl"], resource_id)
+        request_url = "{}/{}/activate".format(self.config()["resourceUrl"], resource_id)
 
         logger.info(
-            "Activating resource -> {}; calling -> {}".format(resource_id, requestUrl)
+            "Activating resource -> {}; calling -> {}".format(resource_id, request_url)
         )
 
         retries = 0
         while True:
-            resourceResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 json=resourcePostBodyJson,
                 headers=requestHeaders,
                 cookies=self.cookie(),
             )
-            if resourceResponse.ok:
-                return self.parseRequestResponse(resourceResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif resourceResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to activate resource -> {}; error -> {}".format(
-                        resource_id, resourceResponse.text
+                        resource_id, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def getAccessRoles(self):
         """Get a list of all OTDS access roles
 
         Args: None
         Return:
             Request response (json) or None if the REST call fails.
         """
 
-        requestUrl = self.config()["accessRoleUrl"]
+        request_url = self.config()["accessRoleUrl"]
 
-        logger.info("Retrieving access roles; calling -> {}".format(requestUrl))
+        logger.info("Retrieving access roles; calling -> {}".format(request_url))
 
         retries = 0
         while True:
-            accessRolesResponse = requests.get(
-                requestUrl, headers=requestHeaders, cookies=self.cookie()
+            response = requests.get(
+                request_url, headers=requestHeaders, cookies=self.cookie()
             )
-            if accessRolesResponse.ok:
-                return self.parseRequestResponse(accessRolesResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif accessRolesResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to retrieve access roles; error -> {}".format(
-                        accessRolesResponse.text
+                        response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def getAccessRole(self, name: str):
@@ -1337,36 +1337,36 @@
 
         Args:
             name (string): name of the access role
         Return:
             Request response (json) or None if the REST call fails.
         """
 
-        requestUrl = self.config()["accessRoleUrl"] + "/" + name
+        request_url = self.config()["accessRoleUrl"] + "/" + name
 
         logger.info(
-            "Retrieving access role -> {}; calling -> {}".format(name, requestUrl)
+            "Retrieving access role -> {}; calling -> {}".format(name, request_url)
         )
 
         retries = 0
         while True:
-            accessRolesResponse = requests.get(
-                requestUrl, headers=requestHeaders, cookies=self.cookie()
+            response = requests.get(
+                request_url, headers=requestHeaders, cookies=self.cookie()
             )
-            if accessRolesResponse.ok:
-                return self.parseRequestResponse(accessRolesResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif accessRolesResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to retrieve access role -> {}; error -> {}".format(
-                        name, accessRolesResponse.text
+                        name, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def addPartitionToAccessRole(
@@ -1383,40 +1383,40 @@
             Request response (json) or None if the REST call fails.
         """
 
         accessRolePostBodyJson = {
             "userPartitions": [{"name": partition, "location": location}]
         }
 
-        requestUrl = "{}/{}/members".format(self.config()["accessRoleUrl"], access_role)
+        request_url = "{}/{}/members".format(self.config()["accessRoleUrl"], access_role)
 
         logger.info(
             "Add user partition -> {} to access role -> {}; calling -> {}".format(
-                partition, access_role, requestUrl
+                partition, access_role, request_url
             )
         )
 
         retries = 0
         while True:
-            accessRoleResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 json=accessRolePostBodyJson,
                 headers=requestHeaders,
                 cookies=self.cookie(),
             )
-            if accessRoleResponse.ok:
+            if response.ok:
                 return True
-            elif accessRoleResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to add partition -> {} to access role -> {}; error -> {}".format(
-                        partition, access_role, accessRoleResponse.text
+                        partition, access_role, response.text
                     )
                 )
                 return False
 
     # end method definition
 
     def addUserToAccessRole(self, access_role: str, user_id: str, location: str = ""):
@@ -1453,40 +1453,40 @@
                 user_id, access_role
             )
         )
 
         # create payload for REST call:
         accessRolePostBodyJson = {"users": [{"name": user_id, "location": location}]}
 
-        requestUrl = "{}/{}/members".format(self.config()["accessRoleUrl"], access_role)
+        request_url = "{}/{}/members".format(self.config()["accessRoleUrl"], access_role)
 
         logger.info(
             "Add user -> {} to access role -> {}; calling -> {}".format(
-                user_id, access_role, requestUrl
+                user_id, access_role, request_url
             )
         )
 
         retries = 0
         while True:
-            accessRoleResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 json=accessRolePostBodyJson,
                 headers=requestHeaders,
                 cookies=self.cookie(),
             )
-            if accessRoleResponse.ok:
+            if response.ok:
                 return True
-            elif accessRoleResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to add user -> {} to access role -> {}; error -> {}".format(
-                        user_id, access_role, accessRoleResponse.text
+                        user_id, access_role, response.text
                     )
                 )
                 return False
 
     # end method definition
 
     def addGroupToAccessRole(self, access_role: str, group: str, location: str = ""):
@@ -1523,40 +1523,40 @@
                 group, access_role
             )
         )
 
         # create payload for REST call:
         accessRolePostBodyJson = {"groups": [{"name": group, "location": location}]}
 
-        requestUrl = "{}/{}/members".format(self.config()["accessRoleUrl"], access_role)
+        request_url = "{}/{}/members".format(self.config()["accessRoleUrl"], access_role)
 
         logger.info(
             "Add group -> {} to access role -> {}; calling -> {}".format(
-                group, access_role, requestUrl
+                group, access_role, request_url
             )
         )
 
         retries = 0
         while True:
-            accessRoleResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 json=accessRolePostBodyJson,
                 headers=requestHeaders,
                 cookies=self.cookie(),
             )
-            if accessRoleResponse.ok:
+            if response.ok:
                 return True
-            elif accessRoleResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to add group -> {} to access role -> {}; error -> {}".format(
-                        group, access_role, accessRoleResponse.text
+                        group, access_role, response.text
                     )
                 )
                 return False
 
     # end method definition
 
     def updateAccessRoleAttributes(self, name: str, attributeList: list):
@@ -1579,41 +1579,41 @@
         access_role = self.getAccessRole(name)
         if not access_role:
             logger.error("Failed to get access role -> {}".format(name))
             return None
 
         accessRolePutBodyJson = {"attributes": attributeList}
 
-        requestUrl = "{}/{}/attributes".format(self.config()["accessRoleUrl"], name)
+        request_url = "{}/{}/attributes".format(self.config()["accessRoleUrl"], name)
 
         logger.info(
             "Update access role -> {} with attributes -> {}; calling -> {}".format(
-                name, accessRolePutBodyJson, requestUrl
+                name, accessRolePutBodyJson, request_url
             )
         )
 
         retries = 0
         while True:
-            accessRoleResponse = requests.put(
-                requestUrl,
+            response = requests.put(
+                request_url,
                 json=accessRolePutBodyJson,
                 headers=requestHeaders,
                 cookies=self.cookie(),
             )
-            if accessRoleResponse.ok:
-                return self.parseRequestResponse(accessRoleResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif accessRoleResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to update access role -> {}; error -> {}".format(
-                        name, accessRoleResponse.text
+                        name, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def addSystemAttribute(self, name: str, value: str, description: str = ""):
@@ -1629,82 +1629,82 @@
 
         systemAttributePostBodyJson = {
             "name": name,
             "value": value,
             "friendlyName": description,
         }
 
-        requestUrl = "{}/system_attributes".format(self.config()["systemConfigUrl"])
+        request_url = "{}/system_attributes".format(self.config()["systemConfigUrl"])
 
         if description:
             logger.info(
                 "Add system attribute -> {} ({}) with value -> {}; calling -> {}".format(
-                    name, description, value, requestUrl
+                    name, description, value, request_url
                 )
             )
         else:
             logger.info(
                 "Add system attribute -> {} with value -> {}; calling -> {}".format(
-                    name, value, requestUrl
+                    name, value, request_url
                 )
             )
 
         retries = 0
         while True:
-            systemAttributeResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 json=systemAttributePostBodyJson,
                 headers=requestHeaders,
                 cookies=self.cookie(),
             )
-            if systemAttributeResponse.ok:
-                return self.parseRequestResponse(systemAttributeResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif systemAttributeResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to add system attribute -> {} with value -> {}; error -> {}".format(
-                        name, value, systemAttributeResponse.text
+                        name, value, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def getTrustedSites(self):
         """get all configured OTDS trusted sites
 
         Args: None
         Return:
             Request response (json) or None if the REST call fails.
         """
 
-        requestUrl = "{}/whitelist".format(self.config()["systemConfigUrl"])
+        request_url = "{}/whitelist".format(self.config()["systemConfigUrl"])
 
-        logger.info("Retrieving trusted sites; calling -> {}".format(requestUrl))
+        logger.info("Retrieving trusted sites; calling -> {}".format(request_url))
 
         retries = 0
         while True:
-            trustedSitesResponse = requests.get(
-                requestUrl, headers=requestHeaders, cookies=self.cookie()
+            response = requests.get(
+                request_url, headers=requestHeaders, cookies=self.cookie()
             )
-            if trustedSitesResponse.ok:
-                return self.parseRequestResponse(trustedSitesResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif trustedSitesResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to retrieve trusted sites; error -> {}".format(
-                        trustedSitesResponse.text
+                        response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def addTrustedSite(self, trusted_site: str):
@@ -1723,33 +1723,33 @@
         existingTrustedSites = self.getTrustedSites()
 
         if existingTrustedSites:
             trustedSitePostBodyJson["stringList"].extend(
                 existingTrustedSites["stringList"]
             )
 
-        requestUrl = "{}/whitelist".format(self.config()["systemConfigUrl"])
+        request_url = "{}/whitelist".format(self.config()["systemConfigUrl"])
 
         logger.info(
-            "Add trusted site -> {}; calling -> {}".format(trusted_site, requestUrl)
+            "Add trusted site -> {}; calling -> {}".format(trusted_site, request_url)
         )
 
-        trustedSiteResponse = requests.put(
-            requestUrl,
+        response = requests.put(
+            request_url,
             json=trustedSitePostBodyJson,
             headers=requestHeaders,
             cookies=self.cookie(),
         )
-        if not trustedSiteResponse.ok:
+        if not response.ok:
             logger.error(
                 "Failed to add trusted site -> {}; error -> {}".format(
-                    trusted_site, trustedSiteResponse.text
+                    trusted_site, response.text
                 )
             )
-        return trustedSiteResponse
+        return response
 
     # end method definition
 
     def enableAudit(self):
         """enable Audit
 
         Args:
@@ -1809,29 +1809,29 @@
                 "Tenant Create",
                 "Tenant Delete",
                 "Tenant Modify",
                 "Migration",
             ],
         }
 
-        requestUrl = "{}/audit".format(self.config()["systemConfigUrl"])
+        request_url = "{}/audit".format(self.config()["systemConfigUrl"])
 
-        logger.info("Enable audit; calling -> {}".format(requestUrl))
+        logger.info("Enable audit; calling -> {}".format(request_url))
 
-        auditResponse = requests.put(
-            requestUrl,
+        response = requests.put(
+            request_url,
             json=auditPutBodyJson,
             headers=requestHeaders,
             cookies=self.cookie(),
         )
-        if not auditResponse.ok:
+        if not response.ok:
             logger.error(
-                "Failed to enable audit; error -> {}".format(auditResponse.text)
+                "Failed to enable audit; error -> {}".format(response.text)
             )
-        return auditResponse
+        return response
 
     # end method definition
 
     def addOauthClient(
         self,
         client_id: str,
         description: str,
@@ -1869,41 +1869,41 @@
             "useSessionRefreshTokenLifeTime": True,
             "confidential": confidential,
             "authScopes": auth_scopes,
             "allowedScopes": allowed_scopes,
             "defaultScopes": default_scopes,
         }
 
-        requestUrl = self.oauthClientUrl()
+        request_url = self.oauthClientUrl()
 
         logger.info(
             "Adding oauth client -> {} ({}); calling -> {}".format(
-                description, client_id, requestUrl
+                description, client_id, request_url
             )
         )
 
         retries = 0
         while True:
-            oauthClientResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 json=oauthClientPostBodyJson,
                 headers=requestHeaders,
                 cookies=self.cookie(),
             )
-            if oauthClientResponse.ok:
-                return self.parseRequestResponse(oauthClientResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif oauthClientResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to add OAuth client -> {}; error -> {}".format(
-                        client_id, oauthClientResponse.text
+                        client_id, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def getOauthClient(self, client_id, show_error: bool = True):
@@ -1912,73 +1912,73 @@
         Args:
             client_id (string): name (= ID) of the OAuth client to retrieve
             show_error (boolean): whether or not we want to log an error if partion is not found
         Return:
             Request response (json) or None if the client is not found.
         """
 
-        requestUrl = "{}/{}".format(self.oauthClientUrl(), client_id)
+        request_url = "{}/{}".format(self.oauthClientUrl(), client_id)
 
         logger.info(
-            "Get oauth client -> {}; calling -> {}".format(client_id, requestUrl)
+            "Get oauth client -> {}; calling -> {}".format(client_id, request_url)
         )
 
         retries = 0
         while True:
-            oauthClientResponse = requests.get(
-                requestUrl, headers=requestHeaders, cookies=self.cookie()
+            response = requests.get(
+                request_url, headers=requestHeaders, cookies=self.cookie()
             )
-            if oauthClientResponse.ok:
-                return self.parseRequestResponse(oauthClientResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif oauthClientResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 if show_error:
                     logger.error(
                         "Failed to get oauth client -> {}; error -> {}".format(
-                            client_id, oauthClientResponse.text
+                            client_id, response.text
                         )
                     )
                 return None
 
     # end method definition
 
     def updateOauthClient(self, client_id, updates: dict):
         oauthClientPatchBodyJson = updates
 
-        requestUrl = "{}/{}".format(self.oauthClientUrl(), client_id)
+        request_url = "{}/{}".format(self.oauthClientUrl(), client_id)
 
         logger.info(
             "Update OAuth client -> {} with -> {}; calling -> {}".format(
-                client_id, updates, requestUrl
+                client_id, updates, request_url
             )
         )
 
         retries = 0
         while True:
-            oauthClientResponse = requests.patch(
-                requestUrl,
+            response = requests.patch(
+                request_url,
                 json=oauthClientPatchBodyJson,
                 headers=requestHeaders,
                 cookies=self.cookie(),
             )
-            if oauthClientResponse.ok:
-                return self.parseRequestResponse(oauthClientResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif oauthClientResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to update OAuth client -> {}; error -> {}".format(
-                        client_id, oauthClientResponse.text
+                        client_id, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def addOauthClientsToAccessRole(self, access_role_name: str):
@@ -1996,29 +1996,29 @@
             "Get access role -> {}; calling -> {}".format(
                 access_role_name, accessRolesUrl
             )
         )
 
         retries = 0
         while True:
-            accessRolesGetResponse = requests.get(
+            response = requests.get(
                 accessRolesUrl, headers=requestHeaders, cookies=self.cookie()
             )
-            if accessRolesGetResponse.ok:
-                accessRolesJson = self.parseRequestResponse(accessRolesGetResponse)
+            if response.ok:
+                accessRolesJson = self.parseRequestResponse(response)
                 break
             # Check if Session has expired - then re-authenticate and try once more
-            elif accessRolesGetResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to retrieve role -> {}; url -> {} : error -> {}".format(
-                        access_role_name, accessRolesUrl, accessRolesGetResponse.text
+                        access_role_name, accessRolesUrl, response.text
                     )
                 )
                 return None
 
         # Checking if OAuthClients partition already added to access role
         userPartitions = accessRolesJson["accessRoleMembers"]["userPartitions"]
         for userPartition in userPartitions:
@@ -2055,58 +2055,58 @@
             "name": oauthClientLocation,
             "userPartition": None,
         }
         accessRolesJson["accessRoleMembers"]["organizationalUnits"].append(
             oauthClientsOuBlock
         )
 
-        updateAccessRoleResponse = requests.put(
+        response = requests.put(
             accessRolesUrl,
             json=accessRolesJson,
             headers=requestHeaders,
             cookies=self.cookie(),
         )
 
-        if updateAccessRoleResponse.ok:
+        if response.ok:
             logger.info(
                 "OauthClients partition successfully added to access role -> {}".format(
                     access_role_name
                 )
             )
         else:
             logger.warning(
                 "Status code of {} returned attempting to add OAuthClients to access role {}: error -> {}".format(
-                    updateAccessRoleResponse.status_code,
+                    response.status_code,
                     access_role_name,
-                    updateAccessRoleResponse.text,
+                    response.text,
                 )
             )
-        return updateAccessRoleResponse
+        return response
 
     # end method definition
 
     def getAccessToken(self, client_id, client_secret):
         encodedClientSecret = "{}:{}".format(client_id, client_secret).encode("utf-8")
         accessTokenRequestHeaders = {
             "Authorization": "Basic "
             + base64.b64encode(encodedClientSecret).decode("utf-8"),
             "Content-Type": "application/x-www-form-urlencoded",
         }
 
-        requestUrl = self.tokenUrl()
+        request_url = self.tokenUrl()
 
-        accessTokenResponse = requests.post(
-            requestUrl,
+        response = requests.post(
+            request_url,
             data={"grant_type": "client_credentials"},
             headers=accessTokenRequestHeaders,
         )
 
         accessToken = None
-        if accessTokenResponse.ok:
-            accessTokenJson = self.parseRequestResponse(accessTokenResponse)
+        if response.ok:
+            accessTokenJson = self.parseRequestResponse(response)
 
             if "access_token" in accessTokenJson:
                 accessToken = accessTokenJson["access_token"]
 
         return accessToken
 
     # end method definition
@@ -2204,41 +2204,41 @@
                     "_name": "Auth Response Binding",
                     "_description": "Specifies the SAML binding to use for the response to an AuthnRequest",
                     "_value": "urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST",
                 },
             ],
         }
 
-        requestUrl = self.authHandlerUrl()
+        request_url = self.authHandlerUrl()
 
         logger.info(
             "Adding SAML auth handler -> {} ({}); calling -> {}".format(
-                name, description, requestUrl
+                name, description, request_url
             )
         )
 
         retries = 0
         while True:
-            authHandlerResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 json=authHandlerPostBodyJson,
                 headers=requestHeaders,
                 cookies=self.cookie(),
             )
-            if authHandlerResponse.ok:
-                return self.parseRequestResponse(authHandlerResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif authHandlerResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to add SAML auth handler -> {}; error -> {}".format(
-                        name, authHandlerResponse.text
+                        name, response.text
                     )
                 )
                 return None
 
     # end method definition
 
     def addAuthHandlerSAP(
@@ -2310,32 +2310,32 @@
                     "_confidential": True,
                     "_keepOriginal": False,
                 },
             ],
         }
 
         # 2. Create the auth handler in OTDS
-        requestUrl = self.authHandlerUrl()
+        request_url = self.authHandlerUrl()
 
         logger.info(
             "Adding SAP auth handler -> {} ({}); calling -> {}".format(
-                name, description, requestUrl
+                name, description, request_url
             )
         )
 
-        authHandlerResponse = requests.post(
-            requestUrl,
+        response = requests.post(
+            request_url,
             json=authHandlerPostBodyJson,
             headers=requestHeaders,
             cookies=self.cookie(),
         )
-        if not authHandlerResponse.ok:
+        if not response.ok:
             logger.error(
                 "Failed to add SAP auth handler -> {}; error -> {}".format(
-                    name, authHandlerResponse.text
+                    name, response.text
                 )
             )
             return None
 
         # 3. Upload the certificate file:
 
         # Check that the certificate (PSE) file is readable:
@@ -2404,40 +2404,40 @@
             "file1": (
                 os.path.basename(certificate_file),
                 open(certificate_file, "rb"),
                 "application/octet-stream",
             )
         }
 
-        requestUrl = self.authHandlerUrl() + "/" + name + "/files"
+        request_url = self.authHandlerUrl() + "/" + name + "/files"
 
         logger.info(
             "Uploading certificate file -> {} for SAP auth handler -> {} ({}); calling -> {}".format(
-                certificate_file, name, description, requestUrl
+                certificate_file, name, description, request_url
             )
         )
 
         # it is important to NOT pass the headers parameter here!
         # Basically, if you specify a files parameter (a dictionary),
         # then requests will send a multipart/form-data POST automatically:
-        authHandlerResponse = requests.post(
-            requestUrl,
+        response = requests.post(
+            request_url,
             data=authHandlerPostData,
             files=authHandlerPostFiles,
             cookies=self.cookie(),
         )
-        if not authHandlerResponse.ok:
+        if not response.ok:
             logger.error(
                 "Failed to upload certificate file -> {} for SAP auth handler -> {}; error -> {}".format(
-                    certificate_file, name, authHandlerResponse.text
+                    certificate_file, name, response.text
                 )
             )
             return None
 
-        return authHandlerResponse
+        return response
 
     # end method definition
 
     def addAuthHandlerOAuth(
         self,
         name: str,
         description: str,
@@ -2803,41 +2803,41 @@
                     "_allowedValues": None,
                     "_confidential": False,
                     "_keepOriginal": False,
                 },
             ],
         }
 
-        requestUrl = self.authHandlerUrl()
+        request_url = self.authHandlerUrl()
 
         logger.info(
             "Adding OAuth auth handler -> {} ({}); calling -> {}".format(
-                name, description, requestUrl
+                name, description, request_url
             )
         )
 
         retries = 0
         while True:
-            authHandlerResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 json=authHandlerPostBodyJson,
                 headers=requestHeaders,
                 cookies=self.cookie(),
             )
-            if authHandlerResponse.ok:
-                return self.parseRequestResponse(authHandlerResponse)
+            if response.ok:
+                return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
-            elif authHandlerResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to add OAuth auth handler -> {}; error -> {}".format(
-                        name, authHandlerResponse.text
+                        name, response.text
                     )
                 )
                 return None
 
         # end method definition
 
     def consolidate(self, resource_name: str):
@@ -2866,41 +2866,41 @@
         consolidationPostBodyJson = {
             "cleanupUsersInResource": False,
             "cleanupGroupsInResource": False,
             "resourceList": [resourceDN],
             "objectToConsolidate": resourceDN,
         }
 
-        requestUrl = "{}".format(self.consolidationUrl())
+        request_url = "{}".format(self.consolidationUrl())
 
         logger.info(
             "Consolidation of resource -> {}; calling -> {}".format(
-                resourceDN, requestUrl
+                resourceDN, request_url
             )
         )
 
         retries = 0
         while True:
-            consolidationResponse = requests.post(
-                requestUrl,
+            response = requests.post(
+                request_url,
                 json=consolidationPostBodyJson,
                 headers=requestHeaders,
                 cookies=self.cookie(),
             )
-            if consolidationResponse.ok:
+            if response.ok:
                 return True
             # Check if Session has expired - then re-authenticate and try once more
-            elif consolidationResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to consolidate; error -> {}".format(
-                        consolidationResponse.text
+                        response.text
                     )
                 )
                 return False
 
     # end method definition
 
     def impersonateResource(
@@ -2920,41 +2920,41 @@
         """
 
         impersonationPutBodyJson = {
             "allowImpersonation": allow_impersonation,
             "impersonateList": impersonation_list,
         }
 
-        requestUrl = "{}/{}/impersonation".format(self.resourceUrl(), resource_name)
+        request_url = "{}/{}/impersonation".format(self.resourceUrl(), resource_name)
 
         logger.info(
             "Impersonation settings for resource -> {}; calling -> {}".format(
-                resource_name, requestUrl
+                resource_name, request_url
             )
         )
 
         retries = 0
         while True:
-            impersonationResponse = requests.put(
-                requestUrl,
+            response = requests.put(
+                request_url,
                 json=impersonationPutBodyJson,
                 headers=requestHeaders,
                 cookies=self.cookie(),
             )
-            if impersonationResponse.ok:
+            if response.ok:
                 return True
             # Check if Session has expired - then re-authenticate and try once more
-            elif impersonationResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to set impersonation for resource -> {}; error -> {}".format(
-                        resource_name, impersonationResponse.text
+                        resource_name, response.text
                     )
                 )
                 return False
 
     # end method definition
 
     def impersonateOauthClient(
@@ -2974,39 +2974,39 @@
         """
 
         impersonationPutBodyJson = {
             "allowImpersonation": allow_impersonation,
             "impersonateList": impersonation_list,
         }
 
-        requestUrl = "{}/{}/impersonation".format(self.oauthClientUrl(), client_id)
+        request_url = "{}/{}/impersonation".format(self.oauthClientUrl(), client_id)
 
         logger.info(
             "Impersonation settings for OAuth Client -> {}; calling -> {}".format(
-                client_id, requestUrl
+                client_id, request_url
             )
         )
 
         retries = 0
         while True:
-            impersonationResponse = requests.put(
-                requestUrl,
+            response = requests.put(
+                request_url,
                 json=impersonationPutBodyJson,
                 headers=requestHeaders,
                 cookies=self.cookie(),
             )
-            if impersonationResponse.ok:
+            if response.ok:
                 return True
             # Check if Session has expired - then re-authenticate and try once more
-            elif impersonationResponse.status_code == 401 and retries == 0:
+            elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
                     "Failed to set impersonation for OAuth Client -> {}; error -> {}".format(
-                        client_id, impersonationResponse.text
+                        client_id, response.text
                     )
                 )
                 return False
 
     # end method definition
```

### Comparing `pyxecm-0.0.14/pyxecm/otiv.py` & `pyxecm-0.0.15/pyxecm/otiv.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.14/pyxecm/otpd.py` & `pyxecm-0.0.15/pyxecm/otpd.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.14/pyxecm/payload.py` & `pyxecm-0.0.15/pyxecm/payload.py`

 * *Files 1% similar despite different names*

```diff
@@ -4390,16 +4390,16 @@
 
         # end method definition
 
     def processPermissions(self, permissions: list):
         """Process items specified in payload and upadate permissions.
 
         Args:
-            permissions: list of items to apply permissions to. Each list item is a dict
-                         with this structure:
+            permissions: list of items to apply permissions to.
+                         Each list item in the payload is a dict with this structure:
                             {
                                 nodeid = "..."
                                 volume = "..."
                                 nickname = "..."
                                 public_access_permissions = ["see", "see_content", ...]
                                 owner_permissions = []
                                 owner_group_permissions = []
@@ -4490,16 +4490,17 @@
                     continue
 
             # Now we should have a value for node_id:
             if not node_id:
                 logger.error("No node ID found! Skipping permission...")
                 continue
             else:
+                node_name = self._otcs.getResultValue(node, "name")
                 logger.info(
-                    "Found node ID -> {} to apply permission to.".format(node_id))
+                    "Found node -> {} with ID -> {} to apply permission to.".format(node_name, node_id))
 
             if "apply_to" in permission:
                 apply_to = permission["apply_to"]
             else:
                 apply_to = 2  # make item + sub-items the default
 
             # 1. Process Owner Permissions (list canbe empty!)
```

### Comparing `pyxecm-0.0.14/pyxecm/sap.py` & `pyxecm-0.0.15/pyxecm/sap.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.14/pyxecm/translate.py` & `pyxecm-0.0.15/pyxecm/translate.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.14/pyxecm/web.py` & `pyxecm-0.0.15/pyxecm/web.py`

 * *Files identical despite different names*

