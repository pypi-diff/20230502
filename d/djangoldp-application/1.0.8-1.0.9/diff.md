# Comparing `tmp/djangoldp_application-1.0.8.tar.gz` & `tmp/djangoldp_application-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_application-1.0.8.tar", last modified: Mon Apr  3 14:24:55 2023, max compression
+gzip compressed data, was "dist/djangoldp_application-1.0.9.tar", last modified: Tue May  2 16:51:50 2023, max compression
```

## Comparing `djangoldp_application-1.0.8.tar` & `djangoldp_application-1.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 14:24:55.000000 djangoldp_application-1.0.8/
--rw-rw-rw-   0 root         (0) root         (0)     1076 2023-04-03 14:24:37.000000 djangoldp_application-1.0.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-04-03 14:24:37.000000 djangoldp_application-1.0.8/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-04-03 14:24:55.000000 djangoldp_application-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      300 2023-04-03 14:24:55.000000 djangoldp_application-1.0.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 14:24:55.000000 djangoldp_application-1.0.8/djangoldp_application.egg-info/
--rw-r--r--   0 root         (0) root         (0)      300 2023-04-03 14:24:55.000000 djangoldp_application-1.0.8/djangoldp_application.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-03 14:24:55.000000 djangoldp_application-1.0.8/djangoldp_application.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1108 2023-04-03 14:24:55.000000 djangoldp_application-1.0.8/djangoldp_application.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-03 14:24:55.000000 djangoldp_application-1.0.8/djangoldp_application.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-03 14:24:55.000000 djangoldp_application-1.0.8/djangoldp_application.egg-info/requires.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 14:24:55.000000 djangoldp_application-1.0.8/djangoldp_application/
--rw-rw-rw-   0 root         (0) root         (0)     9452 2023-04-03 14:24:37.000000 djangoldp_application-1.0.8/djangoldp_application/views.py
--rw-rw-rw-   0 root         (0) root         (0)    18785 2023-04-03 14:24:37.000000 djangoldp_application-1.0.8/djangoldp_application/models.py
--rw-rw-rw-   0 root         (0) root         (0)     4965 2023-04-03 14:24:37.000000 djangoldp_application-1.0.8/djangoldp_application/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2023-04-03 14:24:37.000000 djangoldp_application-1.0.8/djangoldp_application/djangoldp_urls.py
--rw-rw-rw-   0 root         (0) root         (0)       53 2023-04-03 14:24:52.000000 djangoldp_application-1.0.8/djangoldp_application/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-04-03 14:24:37.000000 djangoldp_application-1.0.8/djangoldp_application/apps.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-03 14:24:37.000000 djangoldp_application-1.0.8/djangoldp_application/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 14:24:55.000000 djangoldp_application-1.0.8/djangoldp_application/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     2264 2023-04-03 14:24:37.000000 djangoldp_application-1.0.8/djangoldp_application/migrations/0009_applicationgraphics.py
--rw-rw-rw-   0 root         (0) root         (0)    22281 2023-04-03 14:24:37.000000 djangoldp_application-1.0.8/djangoldp_application/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      899 2023-04-03 14:24:37.000000 djangoldp_application-1.0.8/djangoldp_application/migrations/0010_auto_20230331_0921.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-03 14:24:37.000000 djangoldp_application-1.0.8/djangoldp_application/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-04-03 14:24:37.000000 djangoldp_application-1.0.8/djangoldp_application/migrations/0003_application_api_url.py
--rw-rw-rw-   0 root         (0) root         (0)     1250 2023-04-03 14:24:37.000000 djangoldp_application-1.0.8/djangoldp_application/migrations/0005_auto_20230331_0850.py
--rw-rw-rw-   0 root         (0) root         (0)      438 2023-04-03 14:24:37.000000 djangoldp_application-1.0.8/djangoldp_application/migrations/0007_auto_20230331_0857.py
--rw-rw-rw-   0 root         (0) root         (0)     2157 2023-04-03 14:24:37.000000 djangoldp_application-1.0.8/djangoldp_application/migrations/0008_applicationnpm.py
--rw-rw-rw-   0 root         (0) root         (0)     1341 2023-04-03 14:24:37.000000 djangoldp_application-1.0.8/djangoldp_application/migrations/0004_auto_20230328_1657.py
--rw-rw-rw-   0 root         (0) root         (0)     2271 2023-04-03 14:24:37.000000 djangoldp_application-1.0.8/djangoldp_application/migrations/0002_deployment.py
--rw-rw-rw-   0 root         (0) root         (0)     2283 2023-04-03 14:24:37.000000 djangoldp_application-1.0.8/djangoldp_application/migrations/0006_applicationservice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 16:51:50.000000 djangoldp_application-1.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1076 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-02 16:51:50.000000 djangoldp_application-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      300 2023-05-02 16:51:50.000000 djangoldp_application-1.0.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 16:51:50.000000 djangoldp_application-1.0.9/djangoldp_application.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-05-02 16:51:49.000000 djangoldp_application-1.0.9/djangoldp_application.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 16:51:49.000000 djangoldp_application-1.0.9/djangoldp_application.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1108 2023-05-02 16:51:49.000000 djangoldp_application-1.0.9/djangoldp_application.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-02 16:51:49.000000 djangoldp_application-1.0.9/djangoldp_application.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-02 16:51:49.000000 djangoldp_application-1.0.9/djangoldp_application.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 16:51:50.000000 djangoldp_application-1.0.9/djangoldp_application/
+-rw-rw-rw-   0 root         (0) root         (0)    10807 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/djangoldp_application/views.py
+-rw-rw-rw-   0 root         (0) root         (0)    18785 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/djangoldp_application/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     5338 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/djangoldp_application/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      717 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/djangoldp_application/djangoldp_urls.py
+-rw-rw-rw-   0 root         (0) root         (0)       53 2023-05-02 16:51:47.000000 djangoldp_application-1.0.9/djangoldp_application/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/djangoldp_application/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/djangoldp_application/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 16:51:50.000000 djangoldp_application-1.0.9/djangoldp_application/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     2264 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/djangoldp_application/migrations/0009_applicationgraphics.py
+-rw-rw-rw-   0 root         (0) root         (0)    22281 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/djangoldp_application/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      899 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/djangoldp_application/migrations/0010_auto_20230331_0921.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/djangoldp_application/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/djangoldp_application/migrations/0003_application_api_url.py
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/djangoldp_application/migrations/0005_auto_20230331_0850.py
+-rw-rw-rw-   0 root         (0) root         (0)      438 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/djangoldp_application/migrations/0007_auto_20230331_0857.py
+-rw-rw-rw-   0 root         (0) root         (0)     2157 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/djangoldp_application/migrations/0008_applicationnpm.py
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/djangoldp_application/migrations/0004_auto_20230328_1657.py
+-rw-rw-rw-   0 root         (0) root         (0)     2271 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/djangoldp_application/migrations/0002_deployment.py
+-rw-rw-rw-   0 root         (0) root         (0)     2283 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/djangoldp_application/migrations/0006_applicationservice.py
```

### Comparing `djangoldp_application-1.0.8/README.md` & `djangoldp_application-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.0.8/setup.cfg` & `djangoldp_application-1.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.0.8/djangoldp_application.egg-info/SOURCES.txt` & `djangoldp_application-1.0.9/djangoldp_application.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.0.8/djangoldp_application/views.py` & `djangoldp_application-1.0.9/djangoldp_application/views.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,30 @@
+from django.http import JsonResponse
 from rest_framework import serializers, viewsets
 from rest_framework_yaml.parsers import YAMLParser
 from rest_framework_yaml.renderers import YAMLRenderer
 from .models import Application, Federation
 from djangoldp_component.models import Component, Package
+from django.conf import settings
+
+
+ANSIBLE_SERVERS = set({"127.0.0.1"})
+
+
+if hasattr(settings, "ANSIBLE_SERVERS"):
+    ANSIBLE_SERVERS = ANSIBLE_SERVERS.union(getattr(settings, "ANSIBLE_SERVERS"))
+
+
+def get_client_ip(request):
+    x_forwarded_for = request.META.get("HTTP_X_FORWARDED_FOR")
+    if x_forwarded_for:
+        ip = x_forwarded_for.split(",")[0]
+    else:
+        ip = request.META.get("REMOTE_ADDR")
+    return ip
 
 
 def format(value):
     v = value.lower()
     if v == "false":
         return False
     elif v == "true":
@@ -222,7 +240,29 @@
 
 class ApplicationDetailViewSet(viewsets.ModelViewSet):
     queryset = Application.objects.all()
     serializer_class = ApplicationDetailSerializer
     lookup_field = "slug"
     parser_classes = (YAMLParser,)
     renderer_classes = (YAMLRenderer,)
+
+
+def mark_as_done(request, slug):
+    if request.method == "GET" and get_client_ip(request) in ANSIBLE_SERVERS:
+        application = Application.objects.get(slug=slug)
+        for deploy in application.deployments.filter(status="Todo"):
+            deploy.status = "Done"
+            deploy.save()
+        return JsonResponse({"status": "success"}, status=200)
+    else:
+        return JsonResponse({"status": "invalid request"}, status=400)
+
+
+def mark_as_failed(request, slug):
+    if request.method == "GET" and get_client_ip(request) in ANSIBLE_SERVERS:
+        application = Application.objects.get(slug=slug)
+        for deploy in application.deployments.filter(status="Todo"):
+            deploy.status = "Failed"
+            deploy.save()
+        return JsonResponse({"status": "success"}, status=200)
+    else:
+        return JsonResponse({"status": "invalid request"}, status=400)
```

### Comparing `djangoldp_application-1.0.8/djangoldp_application/models.py` & `djangoldp_application-1.0.9/djangoldp_application/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.0.8/djangoldp_application/admin.py` & `djangoldp_application-1.0.9/djangoldp_application/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+from django import forms
 from django.contrib import admin
+from django.core.exceptions import ValidationError
 from djangoldp.admin import DjangoLDPAdmin
 from .models import (
     Application,
     Federation,
     ApplicationService,
     ApplicationNPM,
     ApplicationGraphics,
@@ -138,19 +140,26 @@
         "base_component__component__short_description",
         "base_component__application__friendly_name",
         "base_component__application__short_description",
     ]
     ordering = ["base_component__application__slug", "component__slug"]
 
 
+class DeploymentAdmin(DjangoLDPAdmin):
+    list_display = ("application", "date", "status")
+    exclude = ("urlid", "slug", "is_backlink", "allow_create_backlink")
+    search_fields = ["urlid", "application__slug", "application__friendly_name"]
+    ordering = ["application__slug", "date"]
+
+
 admin.site.register(Application, ApplicationAdmin)
 admin.site.register(Federation, EmptyAdmin)
 admin.site.register(ApplicationGraphics, EmptyAdmin)
 admin.site.register(ApplicationService, EmptyAdmin)
 admin.site.register(ApplicationNPM, EmptyAdmin)
 admin.site.register(ApplicationComponent, ApplicationComponentAdmin)
 admin.site.register(ApplicationPackage, ApplicationPackageAdmin)
 admin.site.register(ApplicationComponentParameter, EmptyAdmin)
 admin.site.register(ApplicationPackageParameter, EmptyAdmin)
 admin.site.register(ComponentExtension, ComponentExtensionAdmin)
 admin.site.register(ComponentExtensionParameter, EmptyAdmin)
-admin.site.register(Deployment, EmptyAdmin)
+admin.site.register(Deployment, DeploymentAdmin)
```

### Comparing `djangoldp_application-1.0.8/djangoldp_application/migrations/0009_applicationgraphics.py` & `djangoldp_application-1.0.9/djangoldp_application/migrations/0009_applicationgraphics.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.0.8/djangoldp_application/migrations/0001_initial.py` & `djangoldp_application-1.0.9/djangoldp_application/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.0.8/djangoldp_application/migrations/0010_auto_20230331_0921.py` & `djangoldp_application-1.0.9/djangoldp_application/migrations/0010_auto_20230331_0921.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.0.8/djangoldp_application/migrations/0005_auto_20230331_0850.py` & `djangoldp_application-1.0.9/djangoldp_application/migrations/0005_auto_20230331_0850.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.0.8/djangoldp_application/migrations/0008_applicationnpm.py` & `djangoldp_application-1.0.9/djangoldp_application/migrations/0008_applicationnpm.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.0.8/djangoldp_application/migrations/0004_auto_20230328_1657.py` & `djangoldp_application-1.0.9/djangoldp_application/migrations/0004_auto_20230328_1657.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.0.8/djangoldp_application/migrations/0002_deployment.py` & `djangoldp_application-1.0.9/djangoldp_application/migrations/0002_deployment.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.0.8/djangoldp_application/migrations/0006_applicationservice.py` & `djangoldp_application-1.0.9/djangoldp_application/migrations/0006_applicationservice.py`

 * *Files identical despite different names*

