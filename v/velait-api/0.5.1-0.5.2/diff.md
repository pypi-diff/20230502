# Comparing `tmp/velait_api-0.5.1.tar.gz` & `tmp/velait_api-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velait_api-0.5.1.tar", last modified: Fri Apr  7 09:25:55 2023, max compression
+gzip compressed data, was "velait_api-0.5.2.tar", last modified: Tue May  2 05:28:22 2023, max compression
```

## Comparing `velait_api-0.5.1.tar` & `velait_api-0.5.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 09:25:55.712113 velait_api-0.5.1/
--rw-rw-rw-   0        0        0      189 2023-04-07 09:25:55.712113 velait_api-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-02-14 06:59:16.000000 velait_api-0.5.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-07 09:25:55.712113 velait_api-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0      495 2023-04-07 08:57:56.000000 velait_api-0.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:25:55.376928 velait_api-0.5.1/velait/
--rw-rw-rw-   0        0        0        0 2023-03-15 06:47:28.000000 velait_api-0.5.1/velait/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:25:55.681029 velait_api-0.5.1/velait/main/
--rw-rw-rw-   0        0        0        0 2023-02-21 05:58:35.000000 velait_api-0.5.1/velait/main/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:25:55.686316 velait_api-0.5.1/velait/main/api/
--rw-rw-rw-   0        0        0        0 2023-02-21 05:58:35.000000 velait_api-0.5.1/velait/main/api/__init__.py
--rw-rw-rw-   0        0        0     1572 2023-03-16 05:55:42.000000 velait_api-0.5.1/velait/main/api/exception_handlers.py
--rw-rw-rw-   0        0        0     5012 2023-03-15 06:50:44.000000 velait_api-0.5.1/velait/main/api/pagination.py
--rw-rw-rw-   0        0        0     1341 2023-02-24 08:04:34.000000 velait_api-0.5.1/velait/main/api/responses.py
--rw-rw-rw-   0        0        0     1326 2023-03-16 06:14:42.000000 velait_api-0.5.1/velait/main/api/serializers.py
--rw-rw-rw-   0        0        0     5346 2023-03-16 05:57:04.000000 velait_api-0.5.1/velait/main/api/views.py
--rw-rw-rw-   0        0        0      210 2023-04-07 09:18:38.000000 velait_api-0.5.1/velait/main/apps.py
--rw-rw-rw-   0        0        0      507 2023-03-15 06:51:08.000000 velait_api-0.5.1/velait/main/exceptions.py
--rw-rw-rw-   0        0        0     3475 2023-04-04 10:05:12.000000 velait_api-0.5.1/velait/main/logging.py
--rw-rw-rw-   0        0        0      590 2023-04-04 09:22:28.000000 velait_api-0.5.1/velait/main/middleware.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:25:55.687318 velait_api-0.5.1/velait/main/migrations/
--rw-rw-rw-   0        0        0        0 2023-02-21 05:58:35.000000 velait_api-0.5.1/velait/main/migrations/__init__.py
--rw-rw-rw-   0        0        0     1335 2023-04-07 09:01:13.000000 velait_api-0.5.1/velait/main/models.py
--rw-rw-rw-   0        0        0      506 2023-02-21 05:58:35.000000 velait_api-0.5.1/velait/main/parser.py
--rw-rw-rw-   0        0        0      479 2023-03-15 06:45:44.000000 velait_api-0.5.1/velait/main/render.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:25:55.688315 velait_api-0.5.1/velait/main/services/
--rw-rw-rw-   0        0        0        0 2023-02-21 05:58:35.000000 velait_api-0.5.1/velait/main/services/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:25:55.691316 velait_api-0.5.1/velait/main/services/search/
--rw-rw-rw-   0        0        0        0 2023-03-15 06:49:26.000000 velait_api-0.5.1/velait/main/services/search/__init__.py
--rw-rw-rw-   0        0        0     3895 2023-03-15 06:53:04.000000 velait_api-0.5.1/velait/main/services/search/base_search.py
--rw-rw-rw-   0        0        0     2135 2023-03-15 06:52:14.000000 velait_api-0.5.1/velait/main/services/search/search.py
--rw-rw-rw-   0        0        0      380 2023-02-21 05:58:35.000000 velait_api-0.5.1/velait/main/services/utils.py
--rw-rw-rw-   0        0        0      818 2023-04-04 09:59:51.000000 velait_api-0.5.1/velait/main/settings.py
--rw-rw-rw-   0        0        0     2633 2023-04-07 09:23:26.000000 velait_api-0.5.1/velait/main/signals.py
--rw-rw-rw-   0        0        0      193 2023-04-04 09:22:21.000000 velait_api-0.5.1/velait/main/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:25:55.699347 velait_api-0.5.1/velait/velait_users/
--rw-rw-rw-   0        0        0        0 2023-02-21 05:58:35.000000 velait_api-0.5.1/velait/velait_users/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:25:55.702070 velait_api-0.5.1/velait/velait_users/api/
--rw-rw-rw-   0        0        0        0 2023-04-07 08:52:46.000000 velait_api-0.5.1/velait/velait_users/api/__init__.py
--rw-rw-rw-   0        0        0      322 2023-04-07 08:53:32.000000 velait_api-0.5.1/velait/velait_users/api/serializers.py
--rw-rw-rw-   0        0        0      421 2023-04-07 08:55:32.000000 velait_api-0.5.1/velait/velait_users/api/views.py
--rw-rw-rw-   0        0        0      168 2023-03-15 06:45:44.000000 velait_api-0.5.1/velait/velait_users/apps.py
--rw-rw-rw-   0        0        0      263 2023-03-15 06:48:57.000000 velait_api-0.5.1/velait/velait_users/exceptions.py
--rw-rw-rw-   0        0        0     2799 2023-04-04 09:56:27.000000 velait_api-0.5.1/velait/velait_users/middleware.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:25:55.703054 velait_api-0.5.1/velait/velait_users/migrations/
--rw-rw-rw-   0        0        0        0 2023-02-21 05:58:35.000000 velait_api-0.5.1/velait/velait_users/migrations/__init__.py
--rw-rw-rw-   0        0        0     1206 2023-03-15 06:45:44.000000 velait_api-0.5.1/velait/velait_users/services.py
--rw-rw-rw-   0        0        0      388 2023-03-15 06:45:44.000000 velait_api-0.5.1/velait/velait_users/urls.py
--rw-rw-rw-   0        0        0     1873 2023-04-07 08:53:00.000000 velait_api-0.5.1/velait/velait_users/views.py
-drwxrwxrwx   0        0        0        0 2023-04-07 09:25:55.711058 velait_api-0.5.1/velait_api.egg-info/
--rw-rw-rw-   0        0        0      189 2023-04-07 09:25:55.000000 velait_api-0.5.1/velait_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1227 2023-04-07 09:25:55.000000 velait_api-0.5.1/velait_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 09:25:55.000000 velait_api-0.5.1/velait_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      117 2023-04-07 09:25:55.000000 velait_api-0.5.1/velait_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-07 09:25:55.000000 velait_api-0.5.1/velait_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 05:28:22.874672 velait_api-0.5.2/
+-rw-rw-rw-   0        0        0      189 2023-05-02 05:28:22.873692 velait_api-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-02-14 06:59:16.000000 velait_api-0.5.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-02 05:28:22.874672 velait_api-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      495 2023-05-02 05:27:41.000000 velait_api-0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 05:28:22.551819 velait_api-0.5.2/velait/
+-rw-rw-rw-   0        0        0        0 2023-03-15 06:47:28.000000 velait_api-0.5.2/velait/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 05:28:22.621259 velait_api-0.5.2/velait/main/
+-rw-rw-rw-   0        0        0        0 2023-02-21 05:58:35.000000 velait_api-0.5.2/velait/main/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 05:28:22.714297 velait_api-0.5.2/velait/main/api/
+-rw-rw-rw-   0        0        0        0 2023-02-21 05:58:35.000000 velait_api-0.5.2/velait/main/api/__init__.py
+-rw-rw-rw-   0        0        0     1572 2023-03-16 05:55:42.000000 velait_api-0.5.2/velait/main/api/exception_handlers.py
+-rw-rw-rw-   0        0        0     5012 2023-03-15 06:50:44.000000 velait_api-0.5.2/velait/main/api/pagination.py
+-rw-rw-rw-   0        0        0     1341 2023-02-24 08:04:34.000000 velait_api-0.5.2/velait/main/api/responses.py
+-rw-rw-rw-   0        0        0     1444 2023-05-02 05:28:13.000000 velait_api-0.5.2/velait/main/api/serializers.py
+-rw-rw-rw-   0        0        0     5346 2023-03-16 05:57:04.000000 velait_api-0.5.2/velait/main/api/views.py
+-rw-rw-rw-   0        0        0      210 2023-04-07 09:18:38.000000 velait_api-0.5.2/velait/main/apps.py
+-rw-rw-rw-   0        0        0      507 2023-03-15 06:51:08.000000 velait_api-0.5.2/velait/main/exceptions.py
+-rw-rw-rw-   0        0        0     3475 2023-04-04 10:05:12.000000 velait_api-0.5.2/velait/main/logging.py
+-rw-rw-rw-   0        0        0      590 2023-04-04 09:22:28.000000 velait_api-0.5.2/velait/main/middleware.py
+drwxrwxrwx   0        0        0        0 2023-05-02 05:28:22.716299 velait_api-0.5.2/velait/main/migrations/
+-rw-rw-rw-   0        0        0        0 2023-02-21 05:58:35.000000 velait_api-0.5.2/velait/main/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1335 2023-04-07 09:01:13.000000 velait_api-0.5.2/velait/main/models.py
+-rw-rw-rw-   0        0        0      506 2023-02-21 05:58:35.000000 velait_api-0.5.2/velait/main/parser.py
+-rw-rw-rw-   0        0        0      479 2023-03-15 06:45:44.000000 velait_api-0.5.2/velait/main/render.py
+drwxrwxrwx   0        0        0        0 2023-05-02 05:28:22.723039 velait_api-0.5.2/velait/main/services/
+-rw-rw-rw-   0        0        0        0 2023-02-21 05:58:35.000000 velait_api-0.5.2/velait/main/services/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 05:28:22.775104 velait_api-0.5.2/velait/main/services/search/
+-rw-rw-rw-   0        0        0        0 2023-03-15 06:49:26.000000 velait_api-0.5.2/velait/main/services/search/__init__.py
+-rw-rw-rw-   0        0        0     3895 2023-03-15 06:53:04.000000 velait_api-0.5.2/velait/main/services/search/base_search.py
+-rw-rw-rw-   0        0        0     2135 2023-03-15 06:52:14.000000 velait_api-0.5.2/velait/main/services/search/search.py
+-rw-rw-rw-   0        0        0      380 2023-02-21 05:58:35.000000 velait_api-0.5.2/velait/main/services/utils.py
+-rw-rw-rw-   0        0        0      818 2023-04-04 09:59:51.000000 velait_api-0.5.2/velait/main/settings.py
+-rw-rw-rw-   0        0        0     2633 2023-04-07 09:23:26.000000 velait_api-0.5.2/velait/main/signals.py
+-rw-rw-rw-   0        0        0      193 2023-04-04 09:22:21.000000 velait_api-0.5.2/velait/main/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 05:28:22.839965 velait_api-0.5.2/velait/velait_users/
+-rw-rw-rw-   0        0        0        0 2023-02-21 05:58:35.000000 velait_api-0.5.2/velait/velait_users/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 05:28:22.854984 velait_api-0.5.2/velait/velait_users/api/
+-rw-rw-rw-   0        0        0        0 2023-04-07 08:52:46.000000 velait_api-0.5.2/velait/velait_users/api/__init__.py
+-rw-rw-rw-   0        0        0      322 2023-04-07 08:53:32.000000 velait_api-0.5.2/velait/velait_users/api/serializers.py
+-rw-rw-rw-   0        0        0      421 2023-04-07 08:55:32.000000 velait_api-0.5.2/velait/velait_users/api/views.py
+-rw-rw-rw-   0        0        0      168 2023-03-15 06:45:44.000000 velait_api-0.5.2/velait/velait_users/apps.py
+-rw-rw-rw-   0        0        0      263 2023-03-15 06:48:57.000000 velait_api-0.5.2/velait/velait_users/exceptions.py
+-rw-rw-rw-   0        0        0     2799 2023-04-04 09:56:27.000000 velait_api-0.5.2/velait/velait_users/middleware.py
+drwxrwxrwx   0        0        0        0 2023-05-02 05:28:22.855975 velait_api-0.5.2/velait/velait_users/migrations/
+-rw-rw-rw-   0        0        0        0 2023-02-21 05:58:35.000000 velait_api-0.5.2/velait/velait_users/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1206 2023-03-15 06:45:44.000000 velait_api-0.5.2/velait/velait_users/services.py
+-rw-rw-rw-   0        0        0      388 2023-03-15 06:45:44.000000 velait_api-0.5.2/velait/velait_users/urls.py
+-rw-rw-rw-   0        0        0     1873 2023-04-07 08:53:00.000000 velait_api-0.5.2/velait/velait_users/views.py
+drwxrwxrwx   0        0        0        0 2023-05-02 05:28:22.873692 velait_api-0.5.2/velait_api.egg-info/
+-rw-rw-rw-   0        0        0      189 2023-05-02 05:28:22.000000 velait_api-0.5.2/velait_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1227 2023-05-02 05:28:22.000000 velait_api-0.5.2/velait_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 05:28:22.000000 velait_api-0.5.2/velait_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      117 2023-05-02 05:28:22.000000 velait_api-0.5.2/velait_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-02 05:28:22.000000 velait_api-0.5.2/velait_api.egg-info/top_level.txt
```

### Comparing `velait_api-0.5.1/velait/main/api/exception_handlers.py` & `velait_api-0.5.2/velait/main/api/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `velait_api-0.5.1/velait/main/api/pagination.py` & `velait_api-0.5.2/velait/main/api/pagination.py`

 * *Files identical despite different names*

### Comparing `velait_api-0.5.1/velait/main/api/responses.py` & `velait_api-0.5.2/velait/main/api/responses.py`

 * *Files identical despite different names*

### Comparing `velait_api-0.5.1/velait/main/api/serializers.py` & `velait_api-0.5.2/velait/main/api/serializers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from django.utils import timezone
 from rest_framework import serializers
 
 from velait.main.models import BaseModel
 
 
 class BaseSerializer(serializers.ModelSerializer):
     id = serializers.UUIDField(source='uuid', read_only=True)
@@ -26,22 +27,23 @@
 
     def get_user_id(self, instance):
         raise NotImplementedError("You need to add get_user() function to your serializers")
 
     def update(self, instance, validated_data):
         try:
             validated_data['updated_by_id'] = self.get_user_id(instance)
+            validated_data['updated_at'] = timezone.now()
         except NotImplementedError:
             pass
 
         return super(BaseSerializer, self).update(instance=instance, validated_data=validated_data)
 
     def create(self, validated_data):
         try:
-            validated_data['created_by_id'] = self.get_user_id(None)
+            validated_data['created_by_id'] = self.get_user_id(self.context['request'].user)
         except NotImplementedError:
             pass
 
         return super(BaseSerializer, self).create(validated_data)
 
 
 __all__ = ['BaseSerializer']
```

### Comparing `velait_api-0.5.1/velait/main/api/views.py` & `velait_api-0.5.2/velait/main/api/views.py`

 * *Files identical despite different names*

### Comparing `velait_api-0.5.1/velait/main/logging.py` & `velait_api-0.5.2/velait/main/logging.py`

 * *Files identical despite different names*

### Comparing `velait_api-0.5.1/velait/main/middleware.py` & `velait_api-0.5.2/velait/main/middleware.py`

 * *Files identical despite different names*

### Comparing `velait_api-0.5.1/velait/main/models.py` & `velait_api-0.5.2/velait/main/models.py`

 * *Files identical despite different names*

### Comparing `velait_api-0.5.1/velait/main/services/search/base_search.py` & `velait_api-0.5.2/velait/main/services/search/base_search.py`

 * *Files identical despite different names*

### Comparing `velait_api-0.5.1/velait/main/services/search/search.py` & `velait_api-0.5.2/velait/main/services/search/search.py`

 * *Files identical despite different names*

### Comparing `velait_api-0.5.1/velait/main/settings.py` & `velait_api-0.5.2/velait/main/settings.py`

 * *Files identical despite different names*

### Comparing `velait_api-0.5.1/velait/main/signals.py` & `velait_api-0.5.2/velait/main/signals.py`

 * *Files identical despite different names*

### Comparing `velait_api-0.5.1/velait/velait_users/middleware.py` & `velait_api-0.5.2/velait/velait_users/middleware.py`

 * *Files identical despite different names*

### Comparing `velait_api-0.5.1/velait/velait_users/services.py` & `velait_api-0.5.2/velait/velait_users/services.py`

 * *Files identical despite different names*

### Comparing `velait_api-0.5.1/velait/velait_users/views.py` & `velait_api-0.5.2/velait/velait_users/views.py`

 * *Files identical despite different names*

### Comparing `velait_api-0.5.1/velait_api.egg-info/SOURCES.txt` & `velait_api-0.5.2/velait_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

