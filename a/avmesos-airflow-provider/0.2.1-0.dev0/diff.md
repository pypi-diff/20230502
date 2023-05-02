# Comparing `tmp/avmesos_airflow_provider-0.2.1.tar.gz` & `tmp/avmesos_airflow_provider-0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avmesos_airflow_provider-0.2.1.tar", last modified: Tue May  2 08:24:39 2023, max compression
+gzip compressed data, was "avmesos_airflow_provider-0.dev0.tar", last modified: Fri Jul 30 16:32:03 2021, max compression
```

## Comparing `avmesos_airflow_provider-0.2.1.tar` & `avmesos_airflow_provider-0.dev0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2023-05-02 08:24:39.043413 avmesos_airflow_provider-0.2.1/
--rw-r--r--   0 andreas   (1000) andreas   (1000)     3149 2023-05-02 08:24:39.043413 avmesos_airflow_provider-0.2.1/PKG-INFO
--rw-r--r--   0 andreas   (1000) andreas   (1000)     2865 2022-08-29 13:46:59.000000 avmesos_airflow_provider-0.2.1/README.md
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2023-05-02 08:24:39.043413 avmesos_airflow_provider-0.2.1/avmesos_airflow_provider/
--rw-r--r--   0 andreas   (1000) andreas   (1000)      314 2022-08-02 14:55:50.000000 avmesos_airflow_provider-0.2.1/avmesos_airflow_provider/__init__.py
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2023-05-02 08:24:39.043413 avmesos_airflow_provider-0.2.1/avmesos_airflow_provider/executors/
--rw-r--r--   0 andreas   (1000) andreas   (1000)        0 2021-07-20 14:54:15.000000 avmesos_airflow_provider-0.2.1/avmesos_airflow_provider/executors/__init__.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)    28433 2023-04-28 20:41:50.000000 avmesos_airflow_provider-0.2.1/avmesos_airflow_provider/executors/mesos_executor.py
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2023-05-02 08:24:39.043413 avmesos_airflow_provider-0.2.1/avmesos_airflow_provider/operators/
--rw-r--r--   0 andreas   (1000) andreas   (1000)        0 2021-04-26 16:29:56.000000 avmesos_airflow_provider-0.2.1/avmesos_airflow_provider/operators/__init__.py
--rw-r--r--   0 andreas   (1000) andreas   (1000)     9255 2022-04-27 13:28:19.000000 avmesos_airflow_provider-0.2.1/avmesos_airflow_provider/operators/mesos.py
-drwxr-xr-x   0 andreas   (1000) andreas   (1000)        0 2023-05-02 08:24:39.043413 avmesos_airflow_provider-0.2.1/avmesos_airflow_provider.egg-info/
--rw-r--r--   0 andreas   (1000) andreas   (1000)     3149 2023-05-02 08:24:38.000000 avmesos_airflow_provider-0.2.1/avmesos_airflow_provider.egg-info/PKG-INFO
--rw-r--r--   0 andreas   (1000) andreas   (1000)      485 2023-05-02 08:24:39.000000 avmesos_airflow_provider-0.2.1/avmesos_airflow_provider.egg-info/SOURCES.txt
--rw-r--r--   0 andreas   (1000) andreas   (1000)        1 2023-05-02 08:24:38.000000 avmesos_airflow_provider-0.2.1/avmesos_airflow_provider.egg-info/dependency_links.txt
--rw-r--r--   0 andreas   (1000) andreas   (1000)       77 2023-05-02 08:24:38.000000 avmesos_airflow_provider-0.2.1/avmesos_airflow_provider.egg-info/requires.txt
--rw-r--r--   0 andreas   (1000) andreas   (1000)       25 2023-05-02 08:24:38.000000 avmesos_airflow_provider-0.2.1/avmesos_airflow_provider.egg-info/top_level.txt
--rw-r--r--   0 andreas   (1000) andreas   (1000)       38 2023-05-02 08:24:39.043413 avmesos_airflow_provider-0.2.1/setup.cfg
--rw-r--r--   0 andreas   (1000) andreas   (1000)     1030 2023-05-01 18:47:24.000000 avmesos_airflow_provider-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-30 16:32:03.315919 avmesos_airflow_provider-0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (121)      533 2021-07-30 16:32:03.311919 avmesos_airflow_provider-0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2021-07-30 16:31:50.000000 avmesos_airflow_provider-0.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-30 16:32:03.311919 avmesos_airflow_provider-0.dev0/avmesos_airflow_provider/
+-rw-r--r--   0 runner    (1001) docker     (121)      309 2021-07-30 16:31:50.000000 avmesos_airflow_provider-0.dev0/avmesos_airflow_provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-30 16:32:03.311919 avmesos_airflow_provider-0.dev0/avmesos_airflow_provider/executors/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-30 16:31:50.000000 avmesos_airflow_provider-0.dev0/avmesos_airflow_provider/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21274 2021-07-30 16:31:50.000000 avmesos_airflow_provider-0.dev0/avmesos_airflow_provider/executors/mesos_executor.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-30 16:32:03.311919 avmesos_airflow_provider-0.dev0/avmesos_airflow_provider/operators/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-30 16:31:50.000000 avmesos_airflow_provider-0.dev0/avmesos_airflow_provider/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9145 2021-07-30 16:31:50.000000 avmesos_airflow_provider-0.dev0/avmesos_airflow_provider/operators/mesos.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-30 16:32:03.311919 avmesos_airflow_provider-0.dev0/avmesos_airflow_provider.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      533 2021-07-30 16:32:03.000000 avmesos_airflow_provider-0.dev0/avmesos_airflow_provider.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      485 2021-07-30 16:32:03.000000 avmesos_airflow_provider-0.dev0/avmesos_airflow_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-30 16:32:03.000000 avmesos_airflow_provider-0.dev0/avmesos_airflow_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2021-07-30 16:32:03.000000 avmesos_airflow_provider-0.dev0/avmesos_airflow_provider.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2021-07-30 16:32:03.000000 avmesos_airflow_provider-0.dev0/avmesos_airflow_provider.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-30 16:32:03.315919 avmesos_airflow_provider-0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      918 2021-07-30 16:31:50.000000 avmesos_airflow_provider-0.dev0/setup.py
```

### Comparing `avmesos_airflow_provider-0.2.1/avmesos_airflow_provider/operators/mesos.py` & `avmesos_airflow_provider-0.dev0/avmesos_airflow_provider/operators/mesos.py`

 * *Files 8% similar despite different names*

```diff
@@ -99,123 +99,112 @@
         self.mem_limit = memlimit
         self.network_mode = network_mode
         self.user = user
         self.volumes = volumes or []
         self.airflow_scheduler_url = airflow_scheduler_url
         self.container_type = container_type
 
-        if conf.getboolean("mesos", "AUTHENTICATE"):
-            if not conf.get("mesos", "DEFAULT_PRINCIPAL"):
+        if conf.getboolean('mesos', 'AUTHENTICATE'):
+            if not conf.get('mesos', 'DEFAULT_PRINCIPAL'):
                 self.log.error("Expecting authentication principal in the environment")
-                raise AirflowException(
-                    "mesos.default_principal not provided in authenticated mode"
-                )
-            if not conf.get("mesos", "DEFAULT_SECRET"):
+                raise AirflowException("mesos.default_principal not provided in authenticated mode")
+            if not conf.get('mesos', 'DEFAULT_SECRET'):
                 self.log.error("Expecting authentication secret in the environment")
-                raise AirflowException(
-                    "mesos.default_secret not provided in authenticated mode"
-                )
-            self.principal = conf.get("mesos", "DEFAULT_PRINCIPAL")
-            self.secret = conf.get("mesos", "DEFAULT_SECRET")
+                raise AirflowException("mesos.default_secret not provided in authenticated mode")
+            self.principal = conf.get('mesos', 'DEFAULT_PRINCIPAL')
+            self.secret = conf.get('mesos', 'DEFAULT_SECRET')             
 
     def execute(self, context) -> Optional[str]:
-        print("Add MesosTask %s with command %s", self.task_id, self.command)
-        self.log.info("Add MesosTask %s with command %s", self.task_id, self.command)
+        print('Add MesosTask %s with command %s', self.task_id, self.command)
+        self.log.info('Add MesosTask %s with command %s', self.task_id, self.command)
         headers = {
             "Content-Type": "application/json",
             "cache-control": "no-cache",
         }
 
         data = {}
         data["container_type"] = self.container_type
-        data["airflow_task_id"] = "airflow." + self.dag_id + "." + self.task_id
+        data["airflow_task_id"] = "airflow." + self.dag_id + "." + self.task_id 
 
         if self.command != None:
             data["command"] = self.command
 
         if self.image != None:
             data["image"] = self.image
 
         data["container_type"] = "MESOS"
 
+
         response = requests.request(
-            method="POST",
+            method="POST", 
             url=self.airflow_scheduler_url + "/v0/queue_command",
-            data=json.dumps(data),
-            headers=headers,
+            data=json.dumps(data), 
+            headers=headers
         )
 
         if response.status_code == 200:
             task = None
             i = 0
             while task == None and i <= 10:
                 task_info = requests.request(
-                    method="GET",
-                    url=self.airflow_scheduler_url
-                    + "/v0/task/"
-                    + data["airflow_task_id"],
+                    method="GET", 
+                    url=self.airflow_scheduler_url + "/v0/task/" + data["airflow_task_id"],
                     data=json.dumps(data),
-                    headers=headers,
+                    headers=headers
                 )
                 task = task_info.json()
                 time.sleep(5)
                 i += 1
 
-            self.container_id = task["status"]["container_status"]["container_id"][
-                "value"
-            ]
+            self.container_id = task["status"]["container_status"]["container_id"]["value"]
             self.agent_id = task["status"]["agent_id"]["value"]
             self._attach_container_output()
 
     def _get_agent_address(self):
         """
         Get Agent address of the given agent_id
         """
         agent_info = requests.request(
-            method="GET",
+            method="GET", 
             url=self.airflow_scheduler_url + "/v0/agent/" + self.agent_id,
             headers=self._authentication_header(),
         )
         return agent_info.json()
 
     def _attach_container_output(self):
         """
         Streams all output data (e.g. STDOUT/STDERR) to the
         client from the agent.
         """
-        message = {
-            "type": "ATTACH_CONTAINER_OUTPUT",
-            "attach_container_output": {"container_id": {"value": self.container_id}},
+        message = {            
+            'type': 'ATTACH_CONTAINER_OUTPUT',
+            'attach_container_output': {
+                'container_id': {'value': self.container_id }
+            }
         }
-
+ 
         auth = self._authentication_header()
 
         headers = {
-            "Content-Type": "application/json",
-            "Accept": "application/recordio",
-            "Message-Accept": "application/json",
-            "Authorization": auth["authorization"],
+            'Content-Type': 'application/json',
+            'Accept': 'application/recordio',
+            'Message-Accept': 'application/json',
+            'Authorization': auth["authorization"]
         }
 
         agent_info = self._get_agent_address()
 
         http = urllib3.PoolManager()
-        print(
-            "https://" + agent_info["hostname"] + ":" + agent_info["port"] + "/api/v1"
-        )
+        print("https://" + agent_info["hostname"] + ":" + agent_info["port"] + "/api/v1")
         task_info = http.request(
-            method="POST",
-            url="https://"
-            + agent_info["hostname"]
-            + ":"
-            + agent_info["port"]
-            + "/api/v1/",
+            method="POST", 
+            url="https://" + agent_info["hostname"] + ":" + agent_info["port"] + "/api/v1/",
             body=json.dumps(message),
             preload_content=False,
-            headers=headers,
+            headers=headers
         )
 
         self._process_output_stream(task_info)
 
     def _process_output_stream(self, response):
         """
         Gets data streamed over the given response and places the
@@ -223,31 +212,37 @@
         receive data messages.
 
         :param response: Response from an http post
         :type response: requests.models.Response
         """
         try:
             for chunk in response.stream():
-                clean = re.sub(r".*\n", "", chunk.decode("utf-8"))
+                clean = re.sub(r'.*\n', "", chunk.decode('utf-8'))
                 data = json.loads(clean)
                 if "type" in data:
                     if data["type"] == "DATA":
                         message = data["data"]["data"]
                         decode = base64.b64decode(message)
                         self.log.info("%s", decode)
 
         except Exception as e:
             raise AirflowException(
-                "Error parsing output stream: {error}".format(error=e)
-            )
+                "Error parsing output stream: {error}".format(error=e))
+
+    
 
     def _authentication_header(self):
         """
         Return the BasicAuth authentication header
         """
-        if self.principal is not None and self.secret is not None:
-            return urllib3.make_headers(basic_auth=self.principal + ":" + self.secret)
+        if (self.principal is not None
+                and self.secret is not None):
+            return urllib3.make_headers(
+                basic_auth=self.principal + ":" + self.secret
+            )
 
         return None
 
     def on_kill(self) -> None:
         self.log.info("TODO: mesos operator on_kill")
+    
+
```

