# Comparing `tmp/evergreen.py-3.5.8.tar.gz` & `tmp/evergreen.py-3.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evergreen.py-3.5.8.tar", max compression
+gzip compressed data, was "evergreen.py-3.5.9.tar", max compression
```

## Comparing `evergreen.py-3.5.8.tar` & `evergreen.py-3.5.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0    11336 2023-04-24 15:47:20.064053 evergreen.py-3.5.8/LICENSE
--rw-r--r--   0        0        0     6438 2023-04-24 15:47:20.064053 evergreen.py-3.5.8/README.md
--rw-r--r--   0        0        0     1375 2023-04-24 15:47:20.064053 evergreen.py-3.5.8/pyproject.toml
--rw-r--r--   0        0        0      717 2023-04-24 15:47:20.064053 evergreen.py-3.5.8/src/evergreen/__init__.py
--rw-r--r--   0        0        0     1453 2023-04-24 15:47:20.064053 evergreen.py-3.5.8/src/evergreen/alias.py
--rw-r--r--   0        0        0    51068 2023-04-24 15:47:20.068053 evergreen.py-3.5.8/src/evergreen/api.py
--rw-r--r--   0        0        0     2264 2023-04-24 15:47:20.068053 evergreen.py-3.5.8/src/evergreen/api_requests.py
--rw-r--r--   0        0        0     3039 2023-04-24 15:47:20.068053 evergreen.py-3.5.8/src/evergreen/base.py
--rw-r--r--   0        0        0     4558 2023-04-24 15:47:20.068053 evergreen.py-3.5.8/src/evergreen/build.py
--rw-r--r--   0        0        0        0 2023-04-24 15:47:20.068053 evergreen.py-3.5.8/src/evergreen/cli/__init__.py
--rw-r--r--   0        0        0    16690 2023-04-24 15:47:20.068053 evergreen.py-3.5.8/src/evergreen/cli/main.py
--rw-r--r--   0        0        0     1538 2023-04-24 15:47:20.068053 evergreen.py-3.5.8/src/evergreen/commitqueue.py
--rw-r--r--   0        0        0     1745 2023-04-24 15:47:20.068053 evergreen.py-3.5.8/src/evergreen/config.py
--rw-r--r--   0        0        0     7450 2023-04-24 15:47:20.068053 evergreen.py-3.5.8/src/evergreen/distro.py
--rw-r--r--   0        0        0        0 2023-04-24 15:47:20.068053 evergreen.py-3.5.8/src/evergreen/errors/__init__.py
--rw-r--r--   0        0        0     1444 2023-04-24 15:47:20.068053 evergreen.py-3.5.8/src/evergreen/errors/exceptions.py
--rw-r--r--   0        0        0     3381 2023-04-24 15:47:20.068053 evergreen.py-3.5.8/src/evergreen/host.py
--rw-r--r--   0        0        0     1788 2023-04-24 15:47:20.068053 evergreen.py-3.5.8/src/evergreen/manifest.py
--rw-r--r--   0        0        0        0 2023-04-24 15:47:20.068053 evergreen.py-3.5.8/src/evergreen/metrics/__init__.py
--rw-r--r--   0        0        0    15510 2023-04-24 15:47:20.068053 evergreen.py-3.5.8/src/evergreen/metrics/buildmetrics.py
--rw-r--r--   0        0        0     9141 2023-04-24 15:47:20.068053 evergreen.py-3.5.8/src/evergreen/metrics/versionmetrics.py
--rw-r--r--   0        0        0     6576 2023-04-24 15:47:20.068053 evergreen.py-3.5.8/src/evergreen/patch.py
--rw-r--r--   0        0        0    10706 2023-04-24 15:47:20.068053 evergreen.py-3.5.8/src/evergreen/performance_results.py
--rw-r--r--   0        0        0     1737 2023-04-24 15:47:20.068053 evergreen.py-3.5.8/src/evergreen/project.py
--rw-r--r--   0        0        0        0 2023-04-24 15:47:20.068053 evergreen.py-3.5.8/src/evergreen/py.typed
--rw-r--r--   0        0        0     1250 2023-04-24 15:47:20.068053 evergreen.py-3.5.8/src/evergreen/resource_type_permissions.py
--rw-r--r--   0        0        0     1633 2023-04-24 15:47:20.068053 evergreen.py-3.5.8/src/evergreen/stats.py
--rw-r--r--   0        0        0    14542 2023-04-24 15:47:20.068053 evergreen.py-3.5.8/src/evergreen/task.py
--rw-r--r--   0        0        0     2668 2023-04-24 15:47:20.068053 evergreen.py-3.5.8/src/evergreen/task_annotations.py
--rw-r--r--   0        0        0     1271 2023-04-24 15:47:20.068053 evergreen.py-3.5.8/src/evergreen/task_reliability.py
--rw-r--r--   0        0        0     1741 2023-04-24 15:47:20.068053 evergreen.py-3.5.8/src/evergreen/tst.py
--rw-r--r--   0        0        0      585 2023-04-24 15:47:20.068053 evergreen.py-3.5.8/src/evergreen/users_for_role.py
--rw-r--r--   0        0        0     3424 2023-04-24 15:47:20.068053 evergreen.py-3.5.8/src/evergreen/util.py
--rw-r--r--   0        0        0     8010 2023-04-24 15:47:20.068053 evergreen.py-3.5.8/src/evergreen/version.py
--rw-r--r--   0        0        0     7659 2023-04-24 15:48:06.429658 evergreen.py-3.5.8/setup.py
--rw-r--r--   0        0        0     7345 2023-04-24 15:48:06.430294 evergreen.py-3.5.8/PKG-INFO
+-rw-r--r--   0        0        0    11336 2023-05-02 20:54:24.594304 evergreen.py-3.5.9/LICENSE
+-rw-r--r--   0        0        0     6438 2023-05-02 20:54:24.594304 evergreen.py-3.5.9/README.md
+-rw-r--r--   0        0        0     1375 2023-05-02 20:54:24.594304 evergreen.py-3.5.9/pyproject.toml
+-rw-r--r--   0        0        0      717 2023-05-02 20:54:24.594304 evergreen.py-3.5.9/src/evergreen/__init__.py
+-rw-r--r--   0        0        0     1453 2023-05-02 20:54:24.594304 evergreen.py-3.5.9/src/evergreen/alias.py
+-rw-r--r--   0        0        0    51352 2023-05-02 20:54:24.594304 evergreen.py-3.5.9/src/evergreen/api.py
+-rw-r--r--   0        0        0     2386 2023-05-02 20:54:24.594304 evergreen.py-3.5.9/src/evergreen/api_requests.py
+-rw-r--r--   0        0        0     3039 2023-05-02 20:54:24.594304 evergreen.py-3.5.9/src/evergreen/base.py
+-rw-r--r--   0        0        0     4558 2023-05-02 20:54:24.594304 evergreen.py-3.5.9/src/evergreen/build.py
+-rw-r--r--   0        0        0        0 2023-05-02 20:54:24.594304 evergreen.py-3.5.9/src/evergreen/cli/__init__.py
+-rw-r--r--   0        0        0    16690 2023-05-02 20:54:24.594304 evergreen.py-3.5.9/src/evergreen/cli/main.py
+-rw-r--r--   0        0        0     1538 2023-05-02 20:54:24.594304 evergreen.py-3.5.9/src/evergreen/commitqueue.py
+-rw-r--r--   0        0        0     1745 2023-05-02 20:54:24.594304 evergreen.py-3.5.9/src/evergreen/config.py
+-rw-r--r--   0        0        0     7450 2023-05-02 20:54:24.594304 evergreen.py-3.5.9/src/evergreen/distro.py
+-rw-r--r--   0        0        0        0 2023-05-02 20:54:24.594304 evergreen.py-3.5.9/src/evergreen/errors/__init__.py
+-rw-r--r--   0        0        0     1444 2023-05-02 20:54:24.594304 evergreen.py-3.5.9/src/evergreen/errors/exceptions.py
+-rw-r--r--   0        0        0     3381 2023-05-02 20:54:24.594304 evergreen.py-3.5.9/src/evergreen/host.py
+-rw-r--r--   0        0        0     1788 2023-05-02 20:54:24.594304 evergreen.py-3.5.9/src/evergreen/manifest.py
+-rw-r--r--   0        0        0        0 2023-05-02 20:54:24.594304 evergreen.py-3.5.9/src/evergreen/metrics/__init__.py
+-rw-r--r--   0        0        0    15510 2023-05-02 20:54:24.594304 evergreen.py-3.5.9/src/evergreen/metrics/buildmetrics.py
+-rw-r--r--   0        0        0     9141 2023-05-02 20:54:24.594304 evergreen.py-3.5.9/src/evergreen/metrics/versionmetrics.py
+-rw-r--r--   0        0        0     6576 2023-05-02 20:54:24.594304 evergreen.py-3.5.9/src/evergreen/patch.py
+-rw-r--r--   0        0        0    10706 2023-05-02 20:54:24.594304 evergreen.py-3.5.9/src/evergreen/performance_results.py
+-rw-r--r--   0        0        0     1737 2023-05-02 20:54:24.594304 evergreen.py-3.5.9/src/evergreen/project.py
+-rw-r--r--   0        0        0        0 2023-05-02 20:54:24.594304 evergreen.py-3.5.9/src/evergreen/py.typed
+-rw-r--r--   0        0        0     1250 2023-05-02 20:54:24.594304 evergreen.py-3.5.9/src/evergreen/resource_type_permissions.py
+-rw-r--r--   0        0        0     1633 2023-05-02 20:54:24.594304 evergreen.py-3.5.9/src/evergreen/stats.py
+-rw-r--r--   0        0        0    14792 2023-05-02 20:54:24.594304 evergreen.py-3.5.9/src/evergreen/task.py
+-rw-r--r--   0        0        0     3400 2023-05-02 20:54:24.594304 evergreen.py-3.5.9/src/evergreen/task_annotations.py
+-rw-r--r--   0        0        0     1271 2023-05-02 20:54:24.598305 evergreen.py-3.5.9/src/evergreen/task_reliability.py
+-rw-r--r--   0        0        0     1741 2023-05-02 20:54:24.598305 evergreen.py-3.5.9/src/evergreen/tst.py
+-rw-r--r--   0        0        0      585 2023-05-02 20:54:24.598305 evergreen.py-3.5.9/src/evergreen/users_for_role.py
+-rw-r--r--   0        0        0     3424 2023-05-02 20:54:24.598305 evergreen.py-3.5.9/src/evergreen/util.py
+-rw-r--r--   0        0        0     8010 2023-05-02 20:54:24.598305 evergreen.py-3.5.9/src/evergreen/version.py
+-rw-r--r--   0        0        0     7659 2023-05-02 20:55:09.826945 evergreen.py-3.5.9/setup.py
+-rw-r--r--   0        0        0     7345 2023-05-02 20:55:09.827619 evergreen.py-3.5.9/PKG-INFO
```

### Comparing `evergreen.py-3.5.8/LICENSE` & `evergreen.py-3.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.8/README.md` & `evergreen.py-3.5.9/README.md`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.8/pyproject.toml` & `evergreen.py-3.5.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "evergreen.py"
-version = "3.5.8"
+version = "3.5.9"
 description = "Python client for the Evergreen API"
 authors = [
     "Dev Prod DAG <dev-prod-dag@mongodb.com>",
 ]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/evergreen-ci/evergreen.py"
```

### Comparing `evergreen.py-3.5.8/src/evergreen/__init__.py` & `evergreen.py-3.5.9/src/evergreen/__init__.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.8/src/evergreen/alias.py` & `evergreen.py-3.5.9/src/evergreen/alias.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.8/src/evergreen/api.py` & `evergreen.py-3.5.9/src/evergreen/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import requests
 import structlog
 from structlog.stdlib import LoggerFactory
 from tenacity import retry, retry_if_exception_type, stop_after_attempt, wait_exponential
 
 from evergreen.alias import VariantAlias
-from evergreen.api_requests import IssueLinkRequest, SlackAttachment
+from evergreen.api_requests import IssueLinkRequest, MetadataLinkRequest, SlackAttachment
 from evergreen.build import Build
 from evergreen.commitqueue import CommitQueue
 from evergreen.config import (
     DEFAULT_API_SERVER,
     DEFAULT_NETWORK_TIMEOUT_SEC,
     EvgAuth,
     get_auth_from_config,
@@ -981,24 +981,26 @@
         self,
         task_id: str,
         execution: Optional[int] = None,
         message: Optional[str] = None,
         issues: Optional[List[IssueLinkRequest]] = None,
         suspected_issues: Optional[List[IssueLinkRequest]] = None,
         metadata: Optional[Dict[str, Any]] = None,
+        metadata_links: Optional[List[MetadataLinkRequest]] = None,
     ) -> None:
         """
         Annotate the specified task.
 
         :param task_id: ID of task to annotate.
         :param execution: Execution number of task to annotate (default to latest).
         :param message: Message to add to the annotations.
         :param issues: Issues to attach to the annotation.
         :param suspected_issues: Suspected issues to add to the annotation.
         :param metadata: Extra metadata to add to the issue.
+        :param metadata_links: Metadata link to add to the annotation.
         """
         url = self._create_url(f"/tasks/{task_id}/annotation")
         request: Dict[str, Any] = {
             "task_id": task_id,
         }
 
         if execution is not None:
@@ -1012,14 +1014,17 @@
 
         if suspected_issues is not None:
             request["suspected_issues"] = [issue.as_dict() for issue in suspected_issues]
 
         if metadata is not None:
             request["metadata"] = metadata
 
+        if metadata_links is not None:
+            request["metadata_links"] = [link._asdict() for link in metadata_links]
+
         self._call_api(url, method="PUT", data=json.dumps(request))
 
     def performance_results_by_task(self, task_id: str) -> PerformanceData:
         """
         Get the 'perf.json' performance results for a given task_id.
 
         :param task_id: Id of task to query for.
```

### Comparing `evergreen.py-3.5.8/src/evergreen/api_requests.py` & `evergreen.py-3.5.9/src/evergreen/api_requests.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,21 @@
         """Get a dictionary representation of the issue link."""
         data: Dict[str, Any] = {"issue_key": self.issue_key, "url": self.url}
         if self.confidence_score is not None:
             data["confidence_score"] = self.confidence_score
         return data
 
 
+class MetadataLinkRequest(NamedTuple):
+    """Metadata Link to add to a task annotation."""
+
+    url: str
+    text: str
+
+
 class SlackAttachmentField(BaseModel):
     """
     Slack fields that get displayed in a table-like format.
 
     title: The field title.
     value: The field text. It can be formatted as plain text or with markdown by using mrkdwn_in.
     short: Indicates whether the field object is short enough to be displayed side-by-side with
```

### Comparing `evergreen.py-3.5.8/src/evergreen/base.py` & `evergreen.py-3.5.9/src/evergreen/base.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.8/src/evergreen/build.py` & `evergreen.py-3.5.9/src/evergreen/build.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.8/src/evergreen/cli/main.py` & `evergreen.py-3.5.9/src/evergreen/cli/main.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.8/src/evergreen/commitqueue.py` & `evergreen.py-3.5.9/src/evergreen/commitqueue.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.8/src/evergreen/config.py` & `evergreen.py-3.5.9/src/evergreen/config.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.8/src/evergreen/distro.py` & `evergreen.py-3.5.9/src/evergreen/distro.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.8/src/evergreen/errors/exceptions.py` & `evergreen.py-3.5.9/src/evergreen/errors/exceptions.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.8/src/evergreen/host.py` & `evergreen.py-3.5.9/src/evergreen/host.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.8/src/evergreen/manifest.py` & `evergreen.py-3.5.9/src/evergreen/manifest.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.8/src/evergreen/metrics/buildmetrics.py` & `evergreen.py-3.5.9/src/evergreen/metrics/buildmetrics.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.8/src/evergreen/metrics/versionmetrics.py` & `evergreen.py-3.5.9/src/evergreen/metrics/versionmetrics.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.8/src/evergreen/patch.py` & `evergreen.py-3.5.9/src/evergreen/patch.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.8/src/evergreen/performance_results.py` & `evergreen.py-3.5.9/src/evergreen/performance_results.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.8/src/evergreen/project.py` & `evergreen.py-3.5.9/src/evergreen/project.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.8/src/evergreen/resource_type_permissions.py` & `evergreen.py-3.5.9/src/evergreen/resource_type_permissions.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.8/src/evergreen/stats.py` & `evergreen.py-3.5.9/src/evergreen/stats.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.8/src/evergreen/task.py` & `evergreen.py-3.5.9/src/evergreen/task.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """Task representation of evergreen."""
 from __future__ import absolute_import
 
 from datetime import timedelta
 from enum import IntEnum
 from typing import TYPE_CHECKING, Any, Callable, Dict, Iterable, List, Optional
 
-from evergreen.api_requests import IssueLinkRequest
+from evergreen.api_requests import IssueLinkRequest, MetadataLinkRequest
 from evergreen.base import _BaseEvergreenObject, evg_attrib, evg_datetime_attrib
 from evergreen.manifest import Manifest
 from evergreen.task_annotations import TaskAnnotation
 
 if TYPE_CHECKING:
     from evergreen.api import EvergreenApi
     from evergreen.tst import Tst  # noqa: F401
@@ -414,25 +414,33 @@
 
     def annotate(
         self,
         message: Optional[str] = None,
         issues: Optional[List[IssueLinkRequest]] = None,
         suspected_issues: Optional[List[IssueLinkRequest]] = None,
         metadata: Optional[Dict[str, Any]] = None,
+        metadata_links: Optional[List[MetadataLinkRequest]] = None,
     ) -> None:
         """
         Annotate the specified task.
 
         :param message: Message to add to the annotations.
         :param issues: Issues to attach to the annotation.
         :param suspected_issues: Suspected issues to add to the annotation.
         :param metadata: Extra metadata to add to the issue.
+        :param metadata_links: Metadata links to add to the annotation.
         """
         self._api.annotate_task(
-            self.task_id, self.execution, message, issues, suspected_issues, metadata
+            self.task_id,
+            self.execution,
+            message,
+            issues,
+            suspected_issues,
+            metadata,
+            metadata_links,
         )
 
     def __repr__(self) -> str:
         """
         Get a string representation of Task for debugging purposes.
 
         :return: String representation of Task.
```

### Comparing `evergreen.py-3.5.8/src/evergreen/task_annotations.py` & `evergreen.py-3.5.9/src/evergreen/task_annotations.py`

 * *Files 11% similar despite different names*

```diff
@@ -46,14 +46,30 @@
 
     @property
     def source(self) -> Source:
         """Get the source of this note."""
         return Source(self.json["source"], self._api)
 
 
+class MetadataLink(_BaseEvergreenObject):
+    """Representation of a metadata link associated with a task annotation."""
+
+    url = evg_attrib("url")
+    text = evg_attrib("text")
+
+    def __init__(self, json: Dict[str, Any], api: "EvergreenApi") -> None:
+        """Create an instance of a task annotation metadata link."""
+        super().__init__(json, api)
+
+    @property
+    def source(self) -> Source:
+        """Get the source of this metadata link."""
+        return Source(self.json["source"], self._api)
+
+
 class TaskAnnotation(_BaseEvergreenObject):
     """Representation of a task annotation."""
 
     task_id = evg_attrib("task_id")
     task_execution = evg_attrib("task_execution")
 
     def __init__(self, json: Dict[str, Any], api: "EvergreenApi") -> None:
@@ -75,7 +91,12 @@
         """Get metadata associated with this annotation."""
         return self.json.get("metadata", {})
 
     @property
     def note(self) -> Note:
         """Get a note about this annotation."""
         return Note(self.json.get("note", {}), self._api)
+
+    @property
+    def metadata_links(self) -> List[MetadataLink]:
+        """Get metadata links for this annotation."""
+        return [MetadataLink(link, self._api) for link in self.json.get("metadata_links", [])]
```

### Comparing `evergreen.py-3.5.8/src/evergreen/task_reliability.py` & `evergreen.py-3.5.9/src/evergreen/task_reliability.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.8/src/evergreen/tst.py` & `evergreen.py-3.5.9/src/evergreen/tst.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.8/src/evergreen/users_for_role.py` & `evergreen.py-3.5.9/src/evergreen/users_for_role.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.8/src/evergreen/util.py` & `evergreen.py-3.5.9/src/evergreen/util.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.8/src/evergreen/version.py` & `evergreen.py-3.5.9/src/evergreen/version.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.8/setup.py` & `evergreen.py-3.5.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'tenacity>=5']
 
 entry_points = \
 {'console_scripts': ['evg-api = evergreen.cli.main:main']}
 
 setup_kwargs = {
     'name': 'evergreen.py',
-    'version': '3.5.8',
+    'version': '3.5.9',
     'description': 'Python client for the Evergreen API',
     'long_description': '# Evergreen.py\n\nA client library for the Evergreen API written in python. Currently supports the V2 version of\nthe API. For more details, see https://github.com/evergreen-ci/evergreen/wiki/REST-V2-Usage.\n\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/evergreen.py) [![PyPI](https://img.shields.io/pypi/v/evergreen.py.svg)](https://pypi.org/project/evergreen.py/) [![Coverage Status](https://coveralls.io/repos/github/evergreen-ci/evergreen.py/badge.svg?branch=master)](https://coveralls.io/github/evergreen-ci/evergreen.py?branch=master)\n\n## Table of contents\n\n1. [Description](#description)\n2. [Getting Help](#getting-help)\n3. [Dependencies](#dependencies)\n4. [Installation](#installation)\n5. [Usage](#usage)\n6. [Documentation](#documentation)\n7. [Contributor\'s Guide](#contributors-guide)\n   - [Setting up a local development environment](#setting-up-a-local-development-environment)\n   - [Linting/formatting](#lintingformatting)\n   - [Running tests](#running-tests)\n   - [Automatically running checks on commit](#automatically-running-checks-on-commit)\n   - [Versioning](#versioning)\n   - [Code Review](#code-review)\n   - [Deployment](#deployment)\n\n## Description\n\nThis is a Python client library for interacting with Evergreen and Evergreen objects. It currently only\nsupports the V2 version of Evergreen\'s api. It can be used either by Python code in a separate application\nor on the command line to get data about Evergreen objects quickly and easily.\n\n## Getting Help\n\n### What\'s the right channel to ask my question?\n\nIf you have a question about evergreen.py, please mention @dag-on-call in\nslack channel [#evergreen-users](https://mongodb.slack.com/messages/#evergreen-users/),\nor email us at\ndev-prod-dag@mongodb.com.\n\n### How can I request a change/report a bug in evergreen.py?\n\nCreate a [DAG ticket](https://jira.mongodb.org/projects/DAG).\n\n### What should I include in my ticket or #evergreen-users question?\n\nSince #evergreen-users questions are interrupts,\nplease include as much information as possible.\nThis can help avoid long information-gathering threads.\n\nPlease include the following:\n\n- **Motivation for Request**\n  - provide us the motivation for this change.\n- **Context**\n  - provide some background contexts for this issue.\n- **Description**\n  - provide some descriptions on how this issue happened.\n\n## Dependencies\n\n- Python 3.7 or later\n\n## Installation\n\n```bash\n$ pip install evergreen.py\n```\n\n## Usage\n\nThis client can be used either in code or directly via the command line.\n\nIn code:\n\n```python\n>> from evergreen.api import EvgAuth, EvergreenApi\n>> api = EvergreenApi.get_api(EvgAuth(\'david.bradford\', \'***\'))\n>> project = api.project_by_id(\'mongodb-mongo-master\')\n>> project.display_name\n\'MongoDB (master)\'\n```\n\nCli:\n\n```bash\n$ evg-api --json list-hosts\n{\n    "host_id": "host num 0",\n    "host_url": "host.num.com",\n    "distro": {\n        "distro_id": "ubuntu1804-build",\n        "provider": "static",\n        "image_id": ""\n    },\n    "provisioned": true,\n    "started_by": "mci",\n    "host_type": "",\n    "user": "mci-exec",\n    "status": "running",\n    "running_task": {\n        "task_id": null,\n        "name": null,\n        "dispatch_time": null,\n        "version_id": null,\n        "build_id": null\n    },\n    "user_host": false\n}\n```\n\nThe `patch_from_diff` API requires the Evergreen CLI to be installed.\n\nAdd the following to the host\'s DOCKERFILE:\n\n```bash\nRUN wget https://evergreen.mongodb.com/clients/linux_amd64/evergreen\nRUN chmod +x evergreen\nENV PATH="/project:$PATH"\n```\n\nYou will need to provide an .evergreen.yml file with credentials to use the CLI. Assuming you are using the [web-app](https://github.com/10gen/helm-charts/tree/master/charts/web-app) chart this can be done by [mounting](https://kanopy.corp.mongodb.com/docs/getting_started/application_configuration/#configuration-filesvolumes) [kubernetes secrets](https://kanopy.corp.mongodb.com/docs/cheatsheet/#interacting-with-kubernetes-secrets) in your pod.\n\nStore the secret in the cluster:\n\n```bash\nkubectl create secret generic <secret_name> --from-file .evergreen.yml --namespace <namespace>\n```\n\nIn environments/deployment.yml configure the file to be mounted and linked to the correct location:\n\n```yaml\nvolumeSecrets:\n  - name: <secret_name>\n    path: /etc/secrets\nlifecycle:\n  postStart:\n    type: exec\n    command:\n      - /bin/sh\n      - -c\n      - ln -sf /etc/secrets/.evergreen.yml\n```\n\n## Documentation\n\nYou can find the documentation [here](https://evergreen-ci.github.io/evergreen.py/).\n\n## Contributor\'s Guide\n\n### Setting up a local development environment\n\n#### Requirements\n\n- Poetry 1.1 or later\n\nYou will need Evergreen credentials on your local machine to use this library or the attached CLI. You\ncan set up your credentials by following the link [here](https://github.com/evergreen-ci/evergreen/wiki/Using-the-Command-Line-Tool#downloading-the-command-line-tool).\n\n### Linting/formatting\n\nThis project uses [black](https://github.com/psf/black) for formatting.\n\n```bash\npoetry run black src tests\n```\n\n### Running tests\n\n```bash\npoetry run pytest\n```\n\nThere are a few tests that are slow running. These tests are not run by default, but can be included\nby setting the env variable RUN_SLOW_TESTS to any value.\n\n```\n$ RUN_SLOW_TEST=1 poetry run pytest\n```\n\nTo get code coverage information:\n\n```\n$ poetry run pytest --cov=src --cov-report=html\n```\n\n### Automatically running checks on commit\n\nThis project has [pre-commit](https://pre-commit.com/) configured. Pre-commit will run\nconfigured checks at git commit time. To enable pre-commit on your local repository run:\n\n```bash\n$ poetry run pre-commit install\n```\n\n### Versioning\n\nBefore deploying a new version, please update the `CHANGELOG.md` file with a description of what\nis being changed.\n\nDeploys to [PyPi](https://pypi.org/project/evergreen.py/) are done automatically on merges to master.\nIn order to avoid overwriting a previous deploy, the version should be updated on all changes. The\n[semver](https://semver.org/) versioning scheme should be used for determining the version number.\n\nThe version is found in the `pyproject.toml` file.\n\n### Code Review\n\nThis project uses the [Evergreen Commit Queue](https://github.com/evergreen-ci/evergreen/wiki/Commit-Queue#pr).\nAdd a PR comment with `evergreen merge` to trigger a merge.\n\n### Deployment\n\nDeployment to production is automatically triggered on merges to master.\n',
     'author': 'Dev Prod DAG',
     'author_email': 'dev-prod-dag@mongodb.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/evergreen-ci/evergreen.py',
```

### Comparing `evergreen.py-3.5.8/PKG-INFO` & `evergreen.py-3.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evergreen.py
-Version: 3.5.8
+Version: 3.5.9
 Summary: Python client for the Evergreen API
 Home-page: https://github.com/evergreen-ci/evergreen.py
 License: Apache-2.0
 Author: Dev Prod DAG
 Author-email: dev-prod-dag@mongodb.com
 Requires-Python: >=3.6.1,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
```

