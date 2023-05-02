# Comparing `tmp/rele-1.8.0b0.tar.gz` & `tmp/rele-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rele-1.8.0b0.tar", last modified: Fri Apr 28 09:33:41 2023, max compression
+gzip compressed data, was "rele-1.9.0.tar", last modified: Tue May  2 15:01:08 2023, max compression
```

## Comparing `rele-1.8.0b0.tar` & `rele-1.9.0.tar`

### file list

```diff
@@ -1,50 +1,58 @@
-drwxr-xr-x   0 joseantonionavarrosaez   (503) staff       (20)        0 2023-04-28 09:33:41.293461 rele-1.8.0b0/
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)      566 2023-04-24 09:02:19.000000 rele-1.8.0b0/AUTHORS.md
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)    11352 2023-04-24 09:02:19.000000 rele-1.8.0b0/LICENSE
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)     3969 2023-04-28 09:33:41.293582 rele-1.8.0b0/PKG-INFO
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)     2830 2023-04-24 09:02:19.000000 rele-1.8.0b0/README.md
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)       76 2023-04-24 09:02:19.000000 rele-1.8.0b0/pyproject.toml
-drwxr-xr-x   0 joseantonionavarrosaez   (503) staff       (20)        0 2023-04-28 09:33:41.286390 rele-1.8.0b0/rele/
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)      395 2023-04-28 09:19:11.000000 rele-1.8.0b0/rele/__init__.py
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)     1453 2023-04-24 09:02:19.000000 rele-1.8.0b0/rele/__main__.py
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)      199 2023-04-24 09:02:19.000000 rele-1.8.0b0/rele/apps.py
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)     8719 2023-04-28 09:05:12.000000 rele-1.8.0b0/rele/client.py
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)     4352 2023-04-28 09:05:12.000000 rele-1.8.0b0/rele/config.py
-drwxr-xr-x   0 joseantonionavarrosaez   (503) staff       (20)        0 2023-04-28 09:33:41.290519 rele-1.8.0b0/rele/contrib/
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)      355 2023-04-24 09:02:19.000000 rele-1.8.0b0/rele/contrib/__init__.py
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)      400 2023-04-24 09:02:19.000000 rele-1.8.0b0/rele/contrib/django_db_middleware.py
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)      347 2023-04-24 09:02:19.000000 rele-1.8.0b0/rele/contrib/flask_middleware.py
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)     3860 2023-04-24 09:02:19.000000 rele-1.8.0b0/rele/contrib/logging_middleware.py
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)      306 2023-04-24 09:02:19.000000 rele-1.8.0b0/rele/contrib/unrecoverable_middleware.py
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)     1224 2023-04-24 09:02:19.000000 rele-1.8.0b0/rele/contrib/verbose_logging_middleware.py
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)     1840 2023-04-24 09:02:19.000000 rele-1.8.0b0/rele/discover.py
-drwxr-xr-x   0 joseantonionavarrosaez   (503) staff       (20)        0 2023-04-28 09:33:41.291019 rele-1.8.0b0/rele/management/
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)        0 2023-04-24 09:02:19.000000 rele-1.8.0b0/rele/management/__init__.py
-drwxr-xr-x   0 joseantonionavarrosaez   (503) staff       (20)        0 2023-04-28 09:33:41.291830 rele-1.8.0b0/rele/management/commands/
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)        0 2023-04-24 09:02:19.000000 rele-1.8.0b0/rele/management/commands/__init__.py
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)     1089 2023-04-24 09:02:19.000000 rele-1.8.0b0/rele/management/commands/runrele.py
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)      728 2023-04-24 09:02:19.000000 rele-1.8.0b0/rele/management/commands/showsubscriptions.py
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)      537 2023-04-24 09:02:19.000000 rele-1.8.0b0/rele/management/discover.py
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)     3486 2023-04-24 09:02:19.000000 rele-1.8.0b0/rele/middleware.py
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)     1581 2023-04-24 09:02:19.000000 rele-1.8.0b0/rele/publishing.py
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)     1118 2023-04-28 09:05:12.000000 rele-1.8.0b0/rele/retry_policy.py
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)     7182 2023-04-28 09:05:12.000000 rele-1.8.0b0/rele/subscription.py
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)     5562 2023-04-28 09:05:12.000000 rele-1.8.0b0/rele/worker.py
-drwxr-xr-x   0 joseantonionavarrosaez   (503) staff       (20)        0 2023-04-28 09:33:41.288534 rele-1.8.0b0/rele.egg-info/
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)     3969 2023-04-28 09:33:41.000000 rele-1.8.0b0/rele.egg-info/PKG-INFO
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)      988 2023-04-28 09:33:41.000000 rele-1.8.0b0/rele.egg-info/SOURCES.txt
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)        1 2023-04-28 09:33:41.000000 rele-1.8.0b0/rele.egg-info/dependency_links.txt
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)       49 2023-04-28 09:33:41.000000 rele-1.8.0b0/rele.egg-info/entry_points.txt
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)        1 2023-04-28 09:33:41.000000 rele-1.8.0b0/rele.egg-info/not-zip-safe
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)       80 2023-04-28 09:33:41.000000 rele-1.8.0b0/rele.egg-info/requires.txt
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)       11 2023-04-28 09:33:41.000000 rele-1.8.0b0/rele.egg-info/top_level.txt
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)      446 2023-04-28 09:33:41.294105 rele-1.8.0b0/setup.cfg
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)     2227 2023-04-24 09:02:19.000000 rele-1.8.0b0/setup.py
-drwxr-xr-x   0 joseantonionavarrosaez   (503) staff       (20)        0 2023-04-28 09:33:41.277934 rele-1.8.0b0/tests/
-drwxr-xr-x   0 joseantonionavarrosaez   (503) staff       (20)        0 2023-04-28 09:33:41.292636 rele-1.8.0b0/tests/commands/
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)        0 2023-04-24 09:02:19.000000 rele-1.8.0b0/tests/commands/__init__.py
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)     1326 2023-04-28 09:05:12.000000 rele-1.8.0b0/tests/commands/test_runrele.py
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)     1602 2023-04-24 09:02:19.000000 rele-1.8.0b0/tests/commands/test_showsubscriptions.py
-drwxr-xr-x   0 joseantonionavarrosaez   (503) staff       (20)        0 2023-04-28 09:33:41.293187 rele-1.8.0b0/tests/more_subs/
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)        0 2023-04-24 09:02:19.000000 rele-1.8.0b0/tests/more_subs/__init__.py
--rw-r--r--   0 joseantonionavarrosaez   (503) staff       (20)      131 2023-04-24 09:02:19.000000 rele-1.8.0b0/tests/more_subs/subs.py
+drwxr-xr-x   0 abarcel    (501) staff       (20)        0 2023-05-02 15:01:08.499046 rele-1.9.0/
+-rw-r--r--   0 abarcel    (501) staff       (20)      566 2023-05-02 14:41:25.000000 rele-1.9.0/AUTHORS.md
+-rw-r--r--   0 abarcel    (501) staff       (20)    11352 2023-05-02 14:41:25.000000 rele-1.9.0/LICENSE
+-rw-r--r--   0 abarcel    (501) staff       (20)     3947 2023-05-02 15:01:08.499324 rele-1.9.0/PKG-INFO
+-rw-r--r--   0 abarcel    (501) staff       (20)     2830 2023-05-02 14:41:25.000000 rele-1.9.0/README.md
+-rw-r--r--   0 abarcel    (501) staff       (20)       76 2023-05-02 14:41:25.000000 rele-1.9.0/pyproject.toml
+drwxr-xr-x   0 abarcel    (501) staff       (20)        0 2023-05-02 15:01:08.471138 rele-1.9.0/rele/
+-rw-r--r--   0 abarcel    (501) staff       (20)      390 2023-05-02 14:51:26.000000 rele-1.9.0/rele/__init__.py
+-rw-r--r--   0 abarcel    (501) staff       (20)     1453 2023-05-02 14:41:25.000000 rele-1.9.0/rele/__main__.py
+-rw-r--r--   0 abarcel    (501) staff       (20)      199 2023-05-02 14:41:25.000000 rele-1.9.0/rele/apps.py
+-rw-r--r--   0 abarcel    (501) staff       (20)     8719 2023-05-02 14:41:25.000000 rele-1.9.0/rele/client.py
+-rw-r--r--   0 abarcel    (501) staff       (20)     4352 2023-05-02 14:41:25.000000 rele-1.9.0/rele/config.py
+drwxr-xr-x   0 abarcel    (501) staff       (20)        0 2023-05-02 15:01:08.481718 rele-1.9.0/rele/contrib/
+-rw-r--r--   0 abarcel    (501) staff       (20)      355 2023-05-02 14:41:25.000000 rele-1.9.0/rele/contrib/__init__.py
+-rw-r--r--   0 abarcel    (501) staff       (20)      400 2023-05-02 14:41:25.000000 rele-1.9.0/rele/contrib/django_db_middleware.py
+-rw-r--r--   0 abarcel    (501) staff       (20)      347 2023-05-02 14:41:25.000000 rele-1.9.0/rele/contrib/flask_middleware.py
+-rw-r--r--   0 abarcel    (501) staff       (20)     3918 2023-05-02 14:41:25.000000 rele-1.9.0/rele/contrib/logging_middleware.py
+-rw-r--r--   0 abarcel    (501) staff       (20)      306 2023-05-02 14:41:25.000000 rele-1.9.0/rele/contrib/unrecoverable_middleware.py
+-rw-r--r--   0 abarcel    (501) staff       (20)     1224 2023-05-02 14:41:25.000000 rele-1.9.0/rele/contrib/verbose_logging_middleware.py
+-rw-r--r--   0 abarcel    (501) staff       (20)     1840 2023-05-02 14:41:25.000000 rele-1.9.0/rele/discover.py
+drwxr-xr-x   0 abarcel    (501) staff       (20)        0 2023-05-02 15:01:08.483250 rele-1.9.0/rele/management/
+-rw-r--r--   0 abarcel    (501) staff       (20)        0 2023-05-02 14:41:25.000000 rele-1.9.0/rele/management/__init__.py
+drwxr-xr-x   0 abarcel    (501) staff       (20)        0 2023-05-02 15:01:08.486739 rele-1.9.0/rele/management/commands/
+-rw-r--r--   0 abarcel    (501) staff       (20)        0 2023-05-02 14:41:25.000000 rele-1.9.0/rele/management/commands/__init__.py
+-rw-r--r--   0 abarcel    (501) staff       (20)     1089 2023-05-02 14:41:25.000000 rele-1.9.0/rele/management/commands/runrele.py
+-rw-r--r--   0 abarcel    (501) staff       (20)      728 2023-05-02 14:41:25.000000 rele-1.9.0/rele/management/commands/showsubscriptions.py
+-rw-r--r--   0 abarcel    (501) staff       (20)      537 2023-05-02 14:41:25.000000 rele-1.9.0/rele/management/discover.py
+-rw-r--r--   0 abarcel    (501) staff       (20)     3486 2023-05-02 14:41:25.000000 rele-1.9.0/rele/middleware.py
+-rw-r--r--   0 abarcel    (501) staff       (20)     1581 2023-05-02 14:41:25.000000 rele-1.9.0/rele/publishing.py
+-rw-r--r--   0 abarcel    (501) staff       (20)     1118 2023-05-02 14:41:25.000000 rele-1.9.0/rele/retry_policy.py
+-rw-r--r--   0 abarcel    (501) staff       (20)     7182 2023-05-02 14:41:25.000000 rele-1.9.0/rele/subscription.py
+-rw-r--r--   0 abarcel    (501) staff       (20)     5562 2023-05-02 14:41:25.000000 rele-1.9.0/rele/worker.py
+drwxr-xr-x   0 abarcel    (501) staff       (20)        0 2023-05-02 15:01:08.476846 rele-1.9.0/rele.egg-info/
+-rw-r--r--   0 abarcel    (501) staff       (20)     3947 2023-05-02 15:01:08.000000 rele-1.9.0/rele.egg-info/PKG-INFO
+-rw-r--r--   0 abarcel    (501) staff       (20)     1178 2023-05-02 15:01:08.000000 rele-1.9.0/rele.egg-info/SOURCES.txt
+-rw-r--r--   0 abarcel    (501) staff       (20)        1 2023-05-02 15:01:08.000000 rele-1.9.0/rele.egg-info/dependency_links.txt
+-rw-r--r--   0 abarcel    (501) staff       (20)       48 2023-05-02 15:01:08.000000 rele-1.9.0/rele.egg-info/entry_points.txt
+-rw-r--r--   0 abarcel    (501) staff       (20)        1 2023-05-02 15:01:08.000000 rele-1.9.0/rele.egg-info/not-zip-safe
+-rw-r--r--   0 abarcel    (501) staff       (20)       80 2023-05-02 15:01:08.000000 rele-1.9.0/rele.egg-info/requires.txt
+-rw-r--r--   0 abarcel    (501) staff       (20)       11 2023-05-02 15:01:08.000000 rele-1.9.0/rele.egg-info/top_level.txt
+-rw-r--r--   0 abarcel    (501) staff       (20)      446 2023-05-02 15:01:08.500802 rele-1.9.0/setup.cfg
+-rw-r--r--   0 abarcel    (501) staff       (20)     2227 2023-05-02 14:41:25.000000 rele-1.9.0/setup.py
+drwxr-xr-x   0 abarcel    (501) staff       (20)        0 2023-05-02 15:01:08.494723 rele-1.9.0/tests/
+drwxr-xr-x   0 abarcel    (501) staff       (20)        0 2023-05-02 15:01:08.496990 rele-1.9.0/tests/commands/
+-rw-r--r--   0 abarcel    (501) staff       (20)        0 2023-05-02 14:41:25.000000 rele-1.9.0/tests/commands/__init__.py
+-rw-r--r--   0 abarcel    (501) staff       (20)     1326 2023-05-02 14:41:25.000000 rele-1.9.0/tests/commands/test_runrele.py
+-rw-r--r--   0 abarcel    (501) staff       (20)     1602 2023-05-02 14:41:25.000000 rele-1.9.0/tests/commands/test_showsubscriptions.py
+drwxr-xr-x   0 abarcel    (501) staff       (20)        0 2023-05-02 15:01:08.498216 rele-1.9.0/tests/more_subs/
+-rw-r--r--   0 abarcel    (501) staff       (20)        0 2023-05-02 14:41:25.000000 rele-1.9.0/tests/more_subs/__init__.py
+-rw-r--r--   0 abarcel    (501) staff       (20)      131 2023-05-02 14:41:25.000000 rele-1.9.0/tests/more_subs/subs.py
+-rw-r--r--   0 abarcel    (501) staff       (20)    12466 2023-05-02 14:41:25.000000 rele-1.9.0/tests/test_client.py
+-rw-r--r--   0 abarcel    (501) staff       (20)     5086 2023-05-02 14:41:25.000000 rele-1.9.0/tests/test_config.py
+-rw-r--r--   0 abarcel    (501) staff       (20)      835 2023-05-02 14:41:25.000000 rele-1.9.0/tests/test_discover.py
+-rw-r--r--   0 abarcel    (501) staff       (20)     1010 2023-05-02 14:41:25.000000 rele-1.9.0/tests/test_middleware.py
+-rw-r--r--   0 abarcel    (501) staff       (20)     1905 2023-05-02 14:41:25.000000 rele-1.9.0/tests/test_publishing.py
+-rw-r--r--   0 abarcel    (501) staff       (20)      464 2023-05-02 14:41:25.000000 rele-1.9.0/tests/test_retry_policy.py
+-rw-r--r--   0 abarcel    (501) staff       (20)    12493 2023-05-02 14:41:25.000000 rele-1.9.0/tests/test_subscription.py
+-rw-r--r--   0 abarcel    (501) staff       (20)     5540 2023-05-02 14:41:25.000000 rele-1.9.0/tests/test_worker.py
```

### Comparing `rele-1.8.0b0/AUTHORS.md` & `rele-1.9.0/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `rele-1.8.0b0/LICENSE` & `rele-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rele-1.8.0b0/PKG-INFO` & `rele-1.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: rele
-Version: 1.8.0b0
+Version: 1.9.0
 Summary: Relé makes integration with Google PubSub easier.
 Home-page: https://github.com/mercadona/rele
 Author: Mercadona Tech
 Author-email: software.online@mercadona.es
 License: Apache Software License 2.0
 Keywords: rele
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
@@ -123,9 +122,7 @@
 ----
 
 ## Running Tests
 
 Does the code actually work?
 
       make test
-
-
```

### Comparing `rele-1.8.0b0/README.md` & `rele-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `rele-1.8.0b0/rele/__main__.py` & `rele-1.9.0/rele/__main__.py`

 * *Files identical despite different names*

### Comparing `rele-1.8.0b0/rele/client.py` & `rele-1.9.0/rele/client.py`

 * *Files identical despite different names*

### Comparing `rele-1.8.0b0/rele/config.py` & `rele-1.9.0/rele/config.py`

 * *Files identical despite different names*

### Comparing `rele-1.8.0b0/rele/contrib/logging_middleware.py` & `rele-1.9.0/rele/contrib/logging_middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
     def __init__(self):
         self._logger = None
 
     def setup(self, config, **kwargs):
         self._logger = logging.getLogger(__name__)
         self._app_name = config.app_name
+        self._encoder = config.encoder
 
     def _build_data_metrics(
         self, subscription, message, status, start_processing_time=None
     ):
         result = {
             "agent": self._app_name,
             "topic": subscription.topic,
@@ -67,15 +68,15 @@
             f"for {topic}: {str(exception.__class__.__name__)}",
             exc_info=True,
             extra={
                 "metrics": {
                     "name": "publications",
                     "data": {"agent": self._app_name, "topic": topic},
                 },
-                "subscription_message": json.dumps(message),
+                "subscription_message": json.dumps(message, cls=self._encoder),
             },
         )
 
     def pre_process_message(self, subscription, message):
         self._logger.debug(
             f"Start processing message for {subscription}",
             extra={
```

### Comparing `rele-1.8.0b0/rele/contrib/verbose_logging_middleware.py` & `rele-1.9.0/rele/contrib/verbose_logging_middleware.py`

 * *Files identical despite different names*

### Comparing `rele-1.8.0b0/rele/discover.py` & `rele-1.9.0/rele/discover.py`

 * *Files identical despite different names*

### Comparing `rele-1.8.0b0/rele/management/commands/runrele.py` & `rele-1.9.0/rele/management/commands/runrele.py`

 * *Files identical despite different names*

### Comparing `rele-1.8.0b0/rele/management/commands/showsubscriptions.py` & `rele-1.9.0/rele/management/commands/showsubscriptions.py`

 * *Files identical despite different names*

### Comparing `rele-1.8.0b0/rele/management/discover.py` & `rele-1.9.0/rele/management/discover.py`

 * *Files identical despite different names*

### Comparing `rele-1.8.0b0/rele/middleware.py` & `rele-1.9.0/rele/middleware.py`

 * *Files identical despite different names*

### Comparing `rele-1.8.0b0/rele/publishing.py` & `rele-1.9.0/rele/publishing.py`

 * *Files identical despite different names*

### Comparing `rele-1.8.0b0/rele/retry_policy.py` & `rele-1.9.0/rele/retry_policy.py`

 * *Files identical despite different names*

### Comparing `rele-1.8.0b0/rele/subscription.py` & `rele-1.9.0/rele/subscription.py`

 * *Files identical despite different names*

### Comparing `rele-1.8.0b0/rele/worker.py` & `rele-1.9.0/rele/worker.py`

 * *Files identical despite different names*

### Comparing `rele-1.8.0b0/rele.egg-info/PKG-INFO` & `rele-1.9.0/rele.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: rele
-Version: 1.8.0b0
+Version: 1.9.0
 Summary: Relé makes integration with Google PubSub easier.
 Home-page: https://github.com/mercadona/rele
 Author: Mercadona Tech
 Author-email: software.online@mercadona.es
 License: Apache Software License 2.0
 Keywords: rele
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
@@ -123,9 +122,7 @@
 ----
 
 ## Running Tests
 
 Does the code actually work?
 
       make test
-
-
```

### Comparing `rele-1.8.0b0/rele.egg-info/SOURCES.txt` & `rele-1.9.0/rele.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -29,12 +29,20 @@
 rele/contrib/unrecoverable_middleware.py
 rele/contrib/verbose_logging_middleware.py
 rele/management/__init__.py
 rele/management/discover.py
 rele/management/commands/__init__.py
 rele/management/commands/runrele.py
 rele/management/commands/showsubscriptions.py
+tests/test_client.py
+tests/test_config.py
+tests/test_discover.py
+tests/test_middleware.py
+tests/test_publishing.py
+tests/test_retry_policy.py
+tests/test_subscription.py
+tests/test_worker.py
 tests/commands/__init__.py
 tests/commands/test_runrele.py
 tests/commands/test_showsubscriptions.py
 tests/more_subs/__init__.py
 tests/more_subs/subs.py
```

### Comparing `rele-1.8.0b0/setup.py` & `rele-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `rele-1.8.0b0/tests/commands/test_runrele.py` & `rele-1.9.0/tests/commands/test_runrele.py`

 * *Files identical despite different names*

### Comparing `rele-1.8.0b0/tests/commands/test_showsubscriptions.py` & `rele-1.9.0/tests/commands/test_showsubscriptions.py`

 * *Files identical despite different names*

