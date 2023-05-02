# Comparing `tmp/pyepic-1.0.8.tar.gz` & `tmp/pyepic-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyepic-1.0.8.tar", last modified: Fri Apr 30 08:54:07 2021, max compression
+gzip compressed data, was "pyepic-1.0.9.tar", last modified: Wed May  5 10:22:32 2021, max compression
```

## Comparing `pyepic-1.0.8.tar` & `pyepic-1.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-30 08:54:07.811839 pyepic-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1516 2021-04-30 08:53:58.000000 pyepic-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1343 2021-04-30 08:54:07.811839 pyepic-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      704 2021-04-30 08:53:58.000000 pyepic-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-30 08:54:07.811839 pyepic-1.0.8/pyepic/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-04-30 08:53:58.000000 pyepic-1.0.8/pyepic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-30 08:54:07.811839 pyepic-1.0.8/pyepic/applications/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-30 08:53:58.000000 pyepic-1.0.8/pyepic/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6070 2021-04-30 08:53:58.000000 pyepic-1.0.8/pyepic/applications/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2634 2021-04-30 08:53:58.000000 pyepic-1.0.8/pyepic/applications/msc_nastran.py
--rw-r--r--   0 runner    (1001) docker     (121)     5675 2021-04-30 08:53:58.000000 pyepic-1.0.8/pyepic/applications/openfoam.py
--rw-r--r--   0 runner    (1001) docker     (121)     2576 2021-04-30 08:53:58.000000 pyepic-1.0.8/pyepic/applications/zcfd.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-30 08:54:07.811839 pyepic-1.0.8/pyepic/client/
--rw-r--r--   0 runner    (1001) docker     (121)     1604 2021-04-30 08:53:58.000000 pyepic-1.0.8/pyepic/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3916 2021-04-30 08:53:58.000000 pyepic-1.0.8/pyepic/client/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     6429 2021-04-30 08:53:58.000000 pyepic-1.0.8/pyepic/client/catalog.py
--rw-r--r--   0 runner    (1001) docker     (121)    22727 2021-04-30 08:53:58.000000 pyepic-1.0.8/pyepic/client/data.py
--rw-r--r--   0 runner    (1001) docker     (121)     4607 2021-04-30 08:53:58.000000 pyepic-1.0.8/pyepic/client/desktop.py
--rw-r--r--   0 runner    (1001) docker     (121)     8884 2021-04-30 08:53:58.000000 pyepic-1.0.8/pyepic/client/job.py
--rw-r--r--   0 runner    (1001) docker     (121)     3067 2021-04-30 08:53:58.000000 pyepic-1.0.8/pyepic/client/projects.py
--rw-r--r--   0 runner    (1001) docker     (121)     3037 2021-04-30 08:53:58.000000 pyepic-1.0.8/pyepic/client/teams.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-30 08:54:07.811839 pyepic-1.0.8/pyepic/desktops/
--rw-r--r--   0 runner    (1001) docker     (121)     1604 2021-04-30 08:53:58.000000 pyepic-1.0.8/pyepic/desktops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5097 2021-04-30 08:53:58.000000 pyepic-1.0.8/pyepic/desktops/desktop.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-30 08:54:07.811839 pyepic-1.0.8/pyepic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1343 2021-04-30 08:54:07.000000 pyepic-1.0.8/pyepic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      619 2021-04-30 08:54:07.000000 pyepic-1.0.8/pyepic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-30 08:54:07.000000 pyepic-1.0.8/pyepic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2021-04-30 08:54:07.000000 pyepic-1.0.8/pyepic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-04-30 08:54:07.000000 pyepic-1.0.8/pyepic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       97 2021-04-30 08:53:58.000000 pyepic-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      637 2021-04-30 08:54:07.815839 pyepic-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      170 2021-04-30 08:53:58.000000 pyepic-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 10:22:32.105601 pyepic-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1516 2021-05-05 10:22:21.000000 pyepic-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1343 2021-05-05 10:22:32.105601 pyepic-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      704 2021-05-05 10:22:21.000000 pyepic-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 10:22:32.101600 pyepic-1.0.9/pyepic/
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2021-05-05 10:22:21.000000 pyepic-1.0.9/pyepic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 10:22:32.105601 pyepic-1.0.9/pyepic/applications/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-05 10:22:21.000000 pyepic-1.0.9/pyepic/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8449 2021-05-05 10:22:21.000000 pyepic-1.0.9/pyepic/applications/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2634 2021-05-05 10:22:21.000000 pyepic-1.0.9/pyepic/applications/msc_nastran.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5675 2021-05-05 10:22:21.000000 pyepic-1.0.9/pyepic/applications/openfoam.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2576 2021-05-05 10:22:21.000000 pyepic-1.0.9/pyepic/applications/zcfd.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 10:22:32.105601 pyepic-1.0.9/pyepic/client/
+-rw-r--r--   0 runner    (1001) docker     (121)     1604 2021-05-05 10:22:21.000000 pyepic-1.0.9/pyepic/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3912 2021-05-05 10:22:21.000000 pyepic-1.0.9/pyepic/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6429 2021-05-05 10:22:21.000000 pyepic-1.0.9/pyepic/client/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22928 2021-05-05 10:22:21.000000 pyepic-1.0.9/pyepic/client/data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4607 2021-05-05 10:22:21.000000 pyepic-1.0.9/pyepic/client/desktop.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8884 2021-05-05 10:22:21.000000 pyepic-1.0.9/pyepic/client/job.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3067 2021-05-05 10:22:21.000000 pyepic-1.0.9/pyepic/client/projects.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3037 2021-05-05 10:22:21.000000 pyepic-1.0.9/pyepic/client/teams.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 10:22:32.105601 pyepic-1.0.9/pyepic/desktops/
+-rw-r--r--   0 runner    (1001) docker     (121)     1604 2021-05-05 10:22:21.000000 pyepic-1.0.9/pyepic/desktops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5097 2021-05-05 10:22:21.000000 pyepic-1.0.9/pyepic/desktops/desktop.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 10:22:32.105601 pyepic-1.0.9/pyepic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1343 2021-05-05 10:22:31.000000 pyepic-1.0.9/pyepic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      619 2021-05-05 10:22:31.000000 pyepic-1.0.9/pyepic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-05 10:22:31.000000 pyepic-1.0.9/pyepic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2021-05-05 10:22:31.000000 pyepic-1.0.9/pyepic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-05-05 10:22:31.000000 pyepic-1.0.9/pyepic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       97 2021-05-05 10:22:21.000000 pyepic-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      637 2021-05-05 10:22:32.105601 pyepic-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      170 2021-05-05 10:22:21.000000 pyepic-1.0.9/setup.py
```

### Comparing `pyepic-1.0.8/LICENSE` & `pyepic-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyepic-1.0.8/PKG-INFO` & `pyepic-1.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyepic
-Version: 1.0.8
+Version: 1.0.9
 Summary: "Python SDK for EPIC"
 Home-page: https://github.com/zenotech/pyepic/
 Author: "Zenotech"
 Author-email: "support@zenotech.com"
 License: BSD 3-Clause License
 Description: # pyepic
         [![Documentation Status](https://readthedocs.org/projects/pyepic/badge/?version=latest)](http://pyepic.readthedocs.io/?badge=latest) [![PyPI version fury.io](https://badge.fury.io/py/pyepic.svg)](https://pypi.python.org/pypi/pyepic/)
```

### Comparing `pyepic-1.0.8/README.md` & `pyepic-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyepic-1.0.8/pyepic/applications/base.py` & `pyepic-1.0.9/pyepic/applications/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -182,7 +182,78 @@
                     input_data=DataSpec(
                         path=self.path,
                     ),
                 ),
             ],
         )
         return spec
+
+
+class JobArray(object):
+    """A helper class for submitting an array of  jobs to EPIC.
+
+    :param array_name: The name to give the array in EPIC
+    :type array_name: str
+    :param array_root_folder: The epic data path to the root of the array data folder, formed as an epic url (e.g. "epic://path_to/data"). Any data in a folder called "common" within this folder will be shared between all jobs in the array.
+    :type array_root_folder: str
+
+    :var config: The Job configuration options object, common to all jobs in the array
+    :vartype config: :class:`Config`
+    :var jobs: The jobs that make up this array
+    :vartype jobs: list
+    """
+
+    def __init__(
+        self,
+        array_name,
+        array_root_folder,
+    ):
+        self.array_name = array_name
+        self.array_root_folder = array_root_folder
+        self.jobs = []
+        self.config = Config()
+
+    def add_job(self, job):
+        """Add a job to this array
+
+        :param job: The code of the EPIC batch queue to submit to
+        :type job: class:`Job`
+        """
+        if isinstance(job, Job):
+            self.jobs.append(job)
+        else:
+            raise Exception("Can only append Job instances to a JobArray")
+
+    def get_job_create_spec(self, queue_code):
+        """Get a JobArraySpec for this array. The JobArraySpec can be used to submit the array to EPIC via the client.
+
+        :param queue_code: The code of the EPIC batch queue to submit to
+        :type queue_code: str
+
+        :return: Job ArraySpecification
+        :rtype: class:`epiccore.models.JobArraySpec`
+        """
+        job_bindings = []
+        for job in self.jobs:
+            job_bindings.append(
+                JobDataBinding(
+                    name=job.job_name,
+                    spec=job.get_job_spec(),
+                    app_options=job.get_applications_options(),
+                    cluster=JobClusterSpec(
+                        queue_code=queue_code,
+                    ),
+                    input_data=DataSpec(
+                        path=job.path,
+                    ),
+                )
+            )
+
+        spec = JobArraySpec(
+            name=self.array_name,
+            config=self.config.get_configuration(),
+            jobs=job_bindings,
+            common_data=DataSpec(
+                path=self.array_root_folder,
+            ),
+        )
+        return spec
```

### Comparing `pyepic-1.0.8/pyepic/applications/msc_nastran.py` & `pyepic-1.0.9/pyepic/applications/msc_nastran.py`

 * *Files identical despite different names*

### Comparing `pyepic-1.0.8/pyepic/applications/openfoam.py` & `pyepic-1.0.9/pyepic/applications/openfoam.py`

 * *Files identical despite different names*

### Comparing `pyepic-1.0.8/pyepic/applications/zcfd.py` & `pyepic-1.0.9/pyepic/applications/zcfd.py`

 * *Files identical despite different names*

### Comparing `pyepic-1.0.8/pyepic/client/__init__.py` & `pyepic-1.0.9/pyepic/client/__init__.py`

 * *Files identical despite different names*

### Comparing `pyepic-1.0.8/pyepic/client/base.py` & `pyepic-1.0.9/pyepic/client/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     ):
         """Constructor method"""
         self.LIMIT = 10
         self.configuration = epiccore.Configuration(
             host=connection_url,
             api_key={"Bearer": "Bearer {}".format(connection_token)},
         )
-    
+
     def set_limt(self, limit):
         self.LIMIT = limit
 
 
 class EPICClient(object):
     """A wrapper class around the epiccore API.
```

### Comparing `pyepic-1.0.8/pyepic/client/catalog.py` & `pyepic-1.0.9/pyepic/client/catalog.py`

 * *Files identical despite different names*

### Comparing `pyepic-1.0.8/pyepic/client/data.py` & `pyepic-1.0.9/pyepic/client/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         local_path,
         file_queue,
         cancel_event=None,
         dryrun=False,
         callback=None,
         download_thread=True,
         overwrite_existing=False,
-        meta_data={}
+        meta_data={},
     ):
         threading.Thread.__init__(self)
         self.__s3_client = s3_client
         self.__bucket_name = bucket_name
         self.__s3_prefix = s3_prefix
         self.__file_q = file_queue
         self.__cancelled = cancel_event
@@ -164,16 +164,16 @@
             return (key_name, full_file_path, False)
         else:
             self.__s3_client.download_file(self.__bucket_name, key_name, full_file_path)
             return (key_name, full_file_path, True)
 
     def upload_file(self, file_full_path):
         last_modified = os.path.getmtime(file_full_path)
-        key_name = file_full_path.split(self.__local_path)[1]
-        if key_name.startswith('/'):
+        key_name = os.path.relpath(file_full_path, self.__local_path)
+        if key_name.startswith("/"):
             key_name = key_name[1:]
         s3_key_name = self.__s3_prefix + key_name
         upload = False
         try:
             s3_head = self.__s3_client.head_object(
                 Bucket=self.__bucket_name, Key=s3_key_name
             )
@@ -184,15 +184,18 @@
         except ClientError as e:
             if e.response["Error"]["Code"] == "404":
                 upload = True
             else:
                 raise e
         if upload and not self.__dryrun:
             self.__s3_client.upload_file(
-                file_full_path, self.__bucket_name, s3_key_name,  ExtraArgs={'Metadata': self.__meta_data}
+                file_full_path,
+                self.__bucket_name,
+                s3_key_name,
+                ExtraArgs={"Metadata": self.__meta_data},
             )
             return (file_full_path, s3_key_name, True)
         return (file_full_path, s3_key_name, False)
 
 
 class DataObject(object):
     """Class representing a file or folder
@@ -241,15 +244,15 @@
 
     def _fetch_session_details_from_epic(self):
         with epiccore.ApiClient(self.configuration) as api_client:
             instance = epiccore.DataApi(api_client)
             return instance.data_session_list()
 
     def _refresh_credentials(self):
-        " Refresh AWS access credentials "
+        "Refresh AWS access credentials"
         session_details = self._fetch_session_details_from_epic()
         credentials = {
             "access_key": session_details.session_token.aws_key_id,
             "secret_key": session_details.session_token.aws_secret_key,
             "token": session_details.session_token.aws_session_token,
             "expiry_time": session_details.session_token.expiration.isoformat(),
             "region": session_details.aws_region,
@@ -270,15 +273,18 @@
             session._credentials = session_credentials
             session.set_config_variable("region", session_details["region"])
             autorefresh_session = boto3.Session(botocore_session=session)
             self._s3_client = autorefresh_session.client("s3")
             self._s3_prefix = session_details["s3_obj_key"]
             self._s3_bucket = session_details["s3_location"]
             profile_details = self._fetch_profile_details_from_epic()
-            self._meta_data = {"Source": self.meta_source, "User-Profile": str( profile_details.id)}
+            self._meta_data = {
+                "Source": self.meta_source,
+                "User-Profile": str(profile_details.id),
+            }
 
     def _epic_path_to_s3(self, epic_path):
         self._connect()
         if epic_path[:7] != "epic://":
             raise ValueError("Path specification must start with epic://")
         raw_path = epic_path[7:]
         s3_path = "{}{}".format(self._s3_prefix, raw_path)
@@ -334,15 +340,15 @@
         if "Contents" in response:
             for item in response["Contents"]:
                 file = DataObject(
                     item["Key"].split("/")[-1],
                     self._s3_to_epic_path(item["Key"]),
                     folder=False,
                     size=item["Size"],
-                    last_modified=item['LastModified'].isoformat()
+                    last_modified=item["LastModified"].isoformat(),
                 )
                 yield file
 
     def download_file(self, epic_path, destination):
         """
         Download the contents of epic_path
             :param epic_path: Path of a file in the form epic://[<folder>]/<file>
@@ -369,20 +375,24 @@
         """
         self._connect()
         if type(file) == str:
             if epic_path.endswith("/"):
                 file_name = os.path.basename(file)
                 epic_path += file_name
             s3_path = self._epic_path_to_s3(epic_path)
-            self._s3_client.upload_file(file, self._s3_bucket, s3_path, ExtraArgs={'Metadata': self._meta_data})
+            self._s3_client.upload_file(
+                file, self._s3_bucket, s3_path, ExtraArgs={"Metadata": self._meta_data}
+            )
         else:
             if epic_path.endswith("/"):
                 raise ValueError("Invalid file epic path")
             s3_path = self._epic_path_to_s3(epic_path)
-            self._s3_client.upload_fileobj(file, self._s3_bucket, s3_path, ExtraArgs={'Metadata': self._meta_data})
+            self._s3_client.upload_fileobj(
+                file, self._s3_bucket, s3_path, ExtraArgs={"Metadata": self._meta_data}
+            )
 
     def delete(self, epic_path, dryrun=False):
         """
         Delete the file of folder at epic_path
             :param epic_path: Path of a file or folder to delete in the form epic://[<folder>]/<file>
             :type epic_path: str
             :param dryrun: If dryrun is True then return a list of files that would be deleted without actually deleting them
@@ -393,15 +403,17 @@
         """
         self._connect()
         deleted = []
         if not epic_path.endswith("/"):
             key = self._epic_path_to_s3(epic_path)
             deleted.append(epic_path)
             if not dryrun:
-                response = self._s3_client.delete_object(Bucket=self._s3_bucket, Key=key)
+                response = self._s3_client.delete_object(
+                    Bucket=self._s3_bucket, Key=key
+                )
             return deleted
         else:
             objects = []
             prefix = self._epic_path_to_s3(epic_path)
             key_list = self._list_contents(prefix)
             for item in key_list:
                 deleted.append(self._s3_to_epic_path(item))
@@ -540,15 +552,15 @@
                 local_source,
                 file_queue,
                 cancel_event=cancel_event,
                 dryrun=dryrun,
                 callback=callback,
                 download_thread=False,
                 overwrite_existing=overwrite_existing,
-                meta_data=self._meta_data
+                meta_data=self._meta_data,
             )
             t.daemon = True
             t.start()
             thread_pool.append(t)
         file_count = 0
         for dirname, _, filenames in os.walk(local_source):
             for filename in filenames:
```

### Comparing `pyepic-1.0.8/pyepic/client/desktop.py` & `pyepic-1.0.9/pyepic/client/desktop.py`

 * *Files identical despite different names*

### Comparing `pyepic-1.0.8/pyepic/client/job.py` & `pyepic-1.0.9/pyepic/client/job.py`

 * *Files identical despite different names*

### Comparing `pyepic-1.0.8/pyepic/client/projects.py` & `pyepic-1.0.9/pyepic/client/projects.py`

 * *Files identical despite different names*

### Comparing `pyepic-1.0.8/pyepic/client/teams.py` & `pyepic-1.0.9/pyepic/client/teams.py`

 * *Files identical despite different names*

### Comparing `pyepic-1.0.8/pyepic/desktops/__init__.py` & `pyepic-1.0.9/pyepic/desktops/__init__.py`

 * *Files identical despite different names*

### Comparing `pyepic-1.0.8/pyepic/desktops/desktop.py` & `pyepic-1.0.9/pyepic/desktops/desktop.py`

 * *Files identical despite different names*

### Comparing `pyepic-1.0.8/pyepic.egg-info/PKG-INFO` & `pyepic-1.0.9/pyepic.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyepic
-Version: 1.0.8
+Version: 1.0.9
 Summary: "Python SDK for EPIC"
 Home-page: https://github.com/zenotech/pyepic/
 Author: "Zenotech"
 Author-email: "support@zenotech.com"
 License: BSD 3-Clause License
 Description: # pyepic
         [![Documentation Status](https://readthedocs.org/projects/pyepic/badge/?version=latest)](http://pyepic.readthedocs.io/?badge=latest) [![PyPI version fury.io](https://badge.fury.io/py/pyepic.svg)](https://pypi.python.org/pypi/pyepic/)
```

### Comparing `pyepic-1.0.8/pyepic.egg-info/SOURCES.txt` & `pyepic-1.0.9/pyepic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyepic-1.0.8/setup.cfg` & `pyepic-1.0.9/setup.cfg`

 * *Files identical despite different names*

