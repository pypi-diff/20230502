# Comparing `tmp/airflow-provider-lakefs-0.45.0.tar.gz` & `tmp/airflow-provider-lakefs-0.46.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow-provider-lakefs-0.45.0.tar", last modified: Wed Mar 15 15:37:20 2023, max compression
+gzip compressed data, was "airflow-provider-lakefs-0.46.0.tar", last modified: Tue May  2 17:36:40 2023, max compression
```

## Comparing `airflow-provider-lakefs-0.45.0.tar` & `airflow-provider-lakefs-0.46.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 15:37:20.188819 airflow-provider-lakefs-0.45.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-15 15:37:11.000000 airflow-provider-lakefs-0.45.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-03-15 15:37:20.184819 airflow-provider-lakefs-0.45.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-03-15 15:37:11.000000 airflow-provider-lakefs-0.45.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 15:37:20.184819 airflow-provider-lakefs-0.45.0/airflow_provider_lakefs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-03-15 15:37:20.000000 airflow-provider-lakefs-0.45.0/airflow_provider_lakefs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-03-15 15:37:20.000000 airflow-provider-lakefs-0.45.0/airflow_provider_lakefs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 15:37:20.000000 airflow-provider-lakefs-0.45.0/airflow_provider_lakefs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-15 15:37:20.000000 airflow-provider-lakefs-0.45.0/airflow_provider_lakefs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-15 15:37:20.000000 airflow-provider-lakefs-0.45.0/airflow_provider_lakefs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-15 15:37:20.000000 airflow-provider-lakefs-0.45.0/airflow_provider_lakefs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 15:37:20.184819 airflow-provider-lakefs-0.45.0/lakefs_provider/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-03-15 15:37:11.000000 airflow-provider-lakefs-0.45.0/lakefs_provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 15:37:20.184819 airflow-provider-lakefs-0.45.0/lakefs_provider/example_dags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 15:37:11.000000 airflow-provider-lakefs-0.45.0/lakefs_provider/example_dags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-03-15 15:37:11.000000 airflow-provider-lakefs-0.45.0/lakefs_provider/example_dags/lakefs-dag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 15:37:20.184819 airflow-provider-lakefs-0.45.0/lakefs_provider/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 15:37:11.000000 airflow-provider-lakefs-0.45.0/lakefs_provider/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-03-15 15:37:11.000000 airflow-provider-lakefs-0.45.0/lakefs_provider/hooks/lakefs_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 15:37:20.184819 airflow-provider-lakefs-0.45.0/lakefs_provider/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 15:37:11.000000 airflow-provider-lakefs-0.45.0/lakefs_provider/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-03-15 15:37:11.000000 airflow-provider-lakefs-0.45.0/lakefs_provider/operators/commit_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-03-15 15:37:11.000000 airflow-provider-lakefs-0.45.0/lakefs_provider/operators/create_branch_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-03-15 15:37:11.000000 airflow-provider-lakefs-0.45.0/lakefs_provider/operators/create_symlink_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-03-15 15:37:11.000000 airflow-provider-lakefs-0.45.0/lakefs_provider/operators/get_commit_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-03-15 15:37:11.000000 airflow-provider-lakefs-0.45.0/lakefs_provider/operators/get_object_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-03-15 15:37:11.000000 airflow-provider-lakefs-0.45.0/lakefs_provider/operators/merge_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-03-15 15:37:11.000000 airflow-provider-lakefs-0.45.0/lakefs_provider/operators/upload_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 15:37:20.184819 airflow-provider-lakefs-0.45.0/lakefs_provider/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 15:37:11.000000 airflow-provider-lakefs-0.45.0/lakefs_provider/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-03-15 15:37:11.000000 airflow-provider-lakefs-0.45.0/lakefs_provider/sensors/commit_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-03-15 15:37:11.000000 airflow-provider-lakefs-0.45.0/lakefs_provider/sensors/file_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 15:37:20.188819 airflow-provider-lakefs-0.45.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-03-15 15:37:11.000000 airflow-provider-lakefs-0.45.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:40.780263 airflow-provider-lakefs-0.46.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-02 17:36:32.000000 airflow-provider-lakefs-0.46.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-05-02 17:36:40.780263 airflow-provider-lakefs-0.46.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-05-02 17:36:32.000000 airflow-provider-lakefs-0.46.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:40.776263 airflow-provider-lakefs-0.46.0/airflow_provider_lakefs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-05-02 17:36:40.000000 airflow-provider-lakefs-0.46.0/airflow_provider_lakefs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-02 17:36:40.000000 airflow-provider-lakefs-0.46.0/airflow_provider_lakefs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 17:36:40.000000 airflow-provider-lakefs-0.46.0/airflow_provider_lakefs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-02 17:36:40.000000 airflow-provider-lakefs-0.46.0/airflow_provider_lakefs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-02 17:36:40.000000 airflow-provider-lakefs-0.46.0/airflow_provider_lakefs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 17:36:40.000000 airflow-provider-lakefs-0.46.0/airflow_provider_lakefs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:40.776263 airflow-provider-lakefs-0.46.0/lakefs_provider/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-02 17:36:32.000000 airflow-provider-lakefs-0.46.0/lakefs_provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:40.776263 airflow-provider-lakefs-0.46.0/lakefs_provider/example_dags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:32.000000 airflow-provider-lakefs-0.46.0/lakefs_provider/example_dags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-05-02 17:36:32.000000 airflow-provider-lakefs-0.46.0/lakefs_provider/example_dags/lakefs-dag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:40.776263 airflow-provider-lakefs-0.46.0/lakefs_provider/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:32.000000 airflow-provider-lakefs-0.46.0/lakefs_provider/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-05-02 17:36:32.000000 airflow-provider-lakefs-0.46.0/lakefs_provider/hooks/lakefs_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:40.780263 airflow-provider-lakefs-0.46.0/lakefs_provider/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:32.000000 airflow-provider-lakefs-0.46.0/lakefs_provider/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-02 17:36:32.000000 airflow-provider-lakefs-0.46.0/lakefs_provider/operators/commit_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-02 17:36:32.000000 airflow-provider-lakefs-0.46.0/lakefs_provider/operators/create_branch_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-02 17:36:32.000000 airflow-provider-lakefs-0.46.0/lakefs_provider/operators/create_symlink_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-02 17:36:32.000000 airflow-provider-lakefs-0.46.0/lakefs_provider/operators/get_commit_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-02 17:36:32.000000 airflow-provider-lakefs-0.46.0/lakefs_provider/operators/get_object_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-02 17:36:32.000000 airflow-provider-lakefs-0.46.0/lakefs_provider/operators/merge_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-02 17:36:32.000000 airflow-provider-lakefs-0.46.0/lakefs_provider/operators/upload_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-02 17:36:32.000000 airflow-provider-lakefs-0.46.0/lakefs_provider/operators/with_metadata_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:40.780263 airflow-provider-lakefs-0.46.0/lakefs_provider/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:32.000000 airflow-provider-lakefs-0.46.0/lakefs_provider/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-02 17:36:32.000000 airflow-provider-lakefs-0.46.0/lakefs_provider/sensors/commit_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-02 17:36:32.000000 airflow-provider-lakefs-0.46.0/lakefs_provider/sensors/file_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 17:36:40.780263 airflow-provider-lakefs-0.46.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-02 17:36:32.000000 airflow-provider-lakefs-0.46.0/setup.py
```

### Comparing `airflow-provider-lakefs-0.45.0/LICENSE` & `airflow-provider-lakefs-0.46.0/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow-provider-lakefs-0.45.0/PKG-INFO` & `airflow-provider-lakefs-0.46.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-provider-lakefs
-Version: 0.45.0
+Version: 0.46.0
 Summary: A lakeFS provider package built by Treeverse.
 Home-page: https://lakefs.io
 Author: Treeverse
 Author-email: services@treeverse.io
 License: Apache License 2.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -58,15 +58,20 @@
     - Testing of production data before exposing it to users / consumers.
     - Testing of intermediate results in your DAG to avoid cascading quality issues.
 
 
 ## Publishing
 
 The repository include GitHub workflow that is trigger on publish event and will build and push the package to PyPI.
-**Note** that the package version is specified in the `setup.py` - make sure to update before publishing.
+
+Use the following steps to release:
+
+- Update `setup.py` with the new package version
+- Update `CHANGELOG.md` with changes for the new release
+- Use GitHub release, use semver vX.X.X
 
 
 ## Community
 
 Stay up to date and get lakeFS support via:
 
 - [Slack](https://lakefs.io/slack) (to get help from our team and other users).
```

### Comparing `airflow-provider-lakefs-0.45.0/README.md` & `airflow-provider-lakefs-0.46.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,20 @@
     - Testing of production data before exposing it to users / consumers.
     - Testing of intermediate results in your DAG to avoid cascading quality issues.
 
 
 ## Publishing
 
 The repository include GitHub workflow that is trigger on publish event and will build and push the package to PyPI.
-**Note** that the package version is specified in the `setup.py` - make sure to update before publishing.
+
+Use the following steps to release:
+
+- Update `setup.py` with the new package version
+- Update `CHANGELOG.md` with changes for the new release
+- Use GitHub release, use semver vX.X.X
 
 
 ## Community
 
 Stay up to date and get lakeFS support via:
 
 - [Slack](https://lakefs.io/slack) (to get help from our team and other users).
```

### Comparing `airflow-provider-lakefs-0.45.0/airflow_provider_lakefs.egg-info/PKG-INFO` & `airflow-provider-lakefs-0.46.0/airflow_provider_lakefs.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-provider-lakefs
-Version: 0.45.0
+Version: 0.46.0
 Summary: A lakeFS provider package built by Treeverse.
 Home-page: https://lakefs.io
 Author: Treeverse
 Author-email: services@treeverse.io
 License: Apache License 2.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -58,15 +58,20 @@
     - Testing of production data before exposing it to users / consumers.
     - Testing of intermediate results in your DAG to avoid cascading quality issues.
 
 
 ## Publishing
 
 The repository include GitHub workflow that is trigger on publish event and will build and push the package to PyPI.
-**Note** that the package version is specified in the `setup.py` - make sure to update before publishing.
+
+Use the following steps to release:
+
+- Update `setup.py` with the new package version
+- Update `CHANGELOG.md` with changes for the new release
+- Use GitHub release, use semver vX.X.X
 
 
 ## Community
 
 Stay up to date and get lakeFS support via:
 
 - [Slack](https://lakefs.io/slack) (to get help from our team and other users).
```

### Comparing `airflow-provider-lakefs-0.45.0/airflow_provider_lakefs.egg-info/SOURCES.txt` & `airflow-provider-lakefs-0.46.0/airflow_provider_lakefs.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,10 +16,11 @@
 lakefs_provider/operators/commit_operator.py
 lakefs_provider/operators/create_branch_operator.py
 lakefs_provider/operators/create_symlink_operator.py
 lakefs_provider/operators/get_commit_operator.py
 lakefs_provider/operators/get_object_operator.py
 lakefs_provider/operators/merge_operator.py
 lakefs_provider/operators/upload_operator.py
+lakefs_provider/operators/with_metadata_operator.py
 lakefs_provider/sensors/__init__.py
 lakefs_provider/sensors/commit_sensor.py
 lakefs_provider/sensors/file_sensor.py
```

### Comparing `airflow-provider-lakefs-0.45.0/lakefs_provider/__init__.py` & `airflow-provider-lakefs-0.46.0/lakefs_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-lakefs-0.45.0/lakefs_provider/example_dags/lakefs-dag.py` & `airflow-provider-lakefs-0.46.0/lakefs_provider/example_dags/lakefs-dag.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Dict
-from collections.abc import Sequence
+from typing import Sequence
 
 from collections import namedtuple
 from itertools import zip_longest
+import time
 
 from io import StringIO
 
 from airflow.decorators import dag
 from airflow.utils.dates import days_ago
 from airflow.exceptions import AirflowFailException
 
@@ -31,25 +32,25 @@
     "repo": "example-repo",
     "path": "path/to/_SUCCESS",
     "default-branch": "main",
     "lakefs_conn_id": "conn_lakefs"
 }
 
 
-CONTENT = 'It is not enough to succeed.  Others must fail.'
+CONTENT_PREFIX = 'It is not enough to succeed.  Others must fail.'
 COMMIT_MESSAGE_1 = 'committing to lakeFS using airflow!'
 MERGE_MESSAGE_1 = 'merging to the default branch'
 
 
 IdAndMessage = namedtuple('IdAndMessage', ['id', 'message'])
 
 
-def check_equality(task_instance, actual: str, expected: str) -> None:
-    if actual != expected:
-        raise AirflowFailException(f'Got {actual} instead of {expected}')
+def check_expected_prefix(task_instance, actual: str, expected: str) -> None:
+    if not actual.startswith(expected):
+        raise AirflowFailException(f'Got:\n"{actual}"\nwhich does not start with\n{expected}')
 
 
 def check_logs(task_instance, repo: str, ref: str, commits: Sequence[str], messages: Sequence[str], amount: int=100) -> None:
     hook = LakeFSHook(default_args['lakefs_conn_id'])
     expected = [ IdAndMessage(commit, message) for commit, message in zip(commits, messages) ]
     actuals = (IdAndMessage(message=commit['message'], id=commit['id'])
                for commit in hook.log_commits(repo, ref, amount))
@@ -91,15 +92,15 @@
         task_id='create_branch',
         source_branch=default_args.get('default-branch')
     )
 
     # Create a path.
     task_create_file = LakeFSUploadOperator(
         task_id='upload_file',
-        content=NamedStringIO(content=CONTENT, name='content'))
+        content=NamedStringIO(content=f"{CONTENT_PREFIX} @{time.asctime()}", name='content'))
 
     task_get_branch_commit = LakeFSGetCommitOperator(
         do_xcom_push=True,
         task_id='get_branch_commit',
         ref=default_args['branch'])
 
     # Checks periodically for the path.
@@ -137,19 +138,19 @@
     task_get_file = LakeFSGetObjectOperator(
         task_id='get_object',
         do_xcom_push=True,
         ref=default_args['branch'])
 
     # Check its contents
     task_check_contents = PythonOperator(
-        task_id='check_equality',
-        python_callable=check_equality,
+        task_id='check_expected_prefix',
+        python_callable=check_expected_prefix,
         op_kwargs={
             'actual': '''{{ task_instance.xcom_pull(task_ids='get_object', key='return_value') }}''',
-            'expected': CONTENT,
+            'expected': CONTENT_PREFIX,
         })
 
     # Merge the changes back to the main branch.
     task_merge = LakeFSMergeOperator(
         task_id='merge_branches',
         do_xcom_push=True,
         source_ref=default_args.get('branch'),
```

### Comparing `airflow-provider-lakefs-0.45.0/lakefs_provider/hooks/lakefs_hook.py` & `airflow-provider-lakefs-0.46.0/lakefs_provider/hooks/lakefs_hook.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-lakefs-0.45.0/lakefs_provider/operators/commit_operator.py` & `airflow-provider-lakefs-0.46.0/lakefs_provider/operators/commit_operator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import Any, Dict
 
-from airflow.models import BaseOperator
 from airflow.utils.decorators import apply_defaults
+from airflow.utils.helpers import build_airflow_url_with_query
 
 from lakefs_provider.hooks.lakefs_hook import LakeFSHook
+from lakefs_provider.operators.with_metadata_operator import WithLakeFSMetadataOperator
 
 
-class LakeFSCommitOperator(BaseOperator):
+class LakeFSCommitOperator(WithLakeFSMetadataOperator):
     """
     Commit changes to a lakeFS branch.
 
     :param lakefs_conn_id: connection to run the operator with
     :type lakefs_conn_id: str
     :param repo: The lakeFS repo for the commit.
     :type repo: str
@@ -44,11 +45,14 @@
 
     def execute(self, context: Dict[str, Any]) -> Any:
         hook = LakeFSHook(lakefs_conn_id=self.lakefs_conn_id)
 
         self.log.info("Committing to lakeFS branch '%s' in repo '%s'",
                       self.branch, self.repo)
 
-        self.metadata.__setitem__("airflow_task_id", self.task_id)
+        self.metadata["airflow_task_id"] = self.task_id
+
+        self.enrich_metadata(context)
+
         ref = hook.commit(self.repo, self.branch, self.msg, self.metadata)
 
         return ref
```

### Comparing `airflow-provider-lakefs-0.45.0/lakefs_provider/operators/create_branch_operator.py` & `airflow-provider-lakefs-0.46.0/lakefs_provider/operators/create_branch_operator.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-lakefs-0.45.0/lakefs_provider/operators/create_symlink_operator.py` & `airflow-provider-lakefs-0.46.0/lakefs_provider/operators/create_symlink_operator.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-lakefs-0.45.0/lakefs_provider/operators/get_commit_operator.py` & `airflow-provider-lakefs-0.46.0/lakefs_provider/operators/get_commit_operator.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-lakefs-0.45.0/lakefs_provider/operators/get_object_operator.py` & `airflow-provider-lakefs-0.46.0/lakefs_provider/operators/get_object_operator.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-lakefs-0.45.0/lakefs_provider/operators/merge_operator.py` & `airflow-provider-lakefs-0.46.0/lakefs_provider/operators/merge_operator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import Any, Dict
 
 from airflow.models import BaseOperator
 from airflow.utils.decorators import apply_defaults
 
 from lakefs_provider.hooks.lakefs_hook import LakeFSHook
+from lakefs_provider.operators.with_metadata_operator import WithLakeFSMetadataOperator
 
 
-class LakeFSMergeOperator(BaseOperator):
+class LakeFSMergeOperator(WithLakeFSMetadataOperator):
     """
     Merge source branch to destination branch
 
     :param lakefs_conn_id: connection to run the operator with
     :type lakefs_conn_id: str
     :param repo: The lakeFS repo.
     :type repo: str
@@ -48,11 +49,14 @@
 
     def execute(self, context: Dict[str, Any]) -> Any:
         hook = LakeFSHook(lakefs_conn_id=self.lakefs_conn_id)
 
         self.log.info("Merging to lakeFS branch '%s' in repo '%s' from source ref '%s'",
                       self.destination_branch, self.repo, self.source_ref)
 
-        self.metadata.__setitem__("airflow_task_id", self.task_id)
+        self.metadata["airflow_task_id"] = self.task_id
+
+        self.enrich_metadata(context)
+
         ref = hook.merge(self.repo, self.source_ref, self.destination_branch, self.msg, self.metadata)
 
         return ref
```

### Comparing `airflow-provider-lakefs-0.45.0/lakefs_provider/operators/upload_operator.py` & `airflow-provider-lakefs-0.46.0/lakefs_provider/operators/upload_operator.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-lakefs-0.45.0/lakefs_provider/sensors/commit_sensor.py` & `airflow-provider-lakefs-0.46.0/lakefs_provider/sensors/commit_sensor.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-lakefs-0.45.0/lakefs_provider/sensors/file_sensor.py` & `airflow-provider-lakefs-0.46.0/lakefs_provider/sensors/file_sensor.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-lakefs-0.45.0/setup.py` & `airflow-provider-lakefs-0.46.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 """Perform the package airflow-provider-lakeFS setup."""
 setup(
     name='airflow-provider-lakefs',
-    version='0.45.0',
+    version='0.46.0',
     description='A lakeFS provider package built by Treeverse.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     entry_points={
         "apache_airflow_provider": [
             "provider_info=lakefs_provider.__init__:get_provider_info"
         ]
```

