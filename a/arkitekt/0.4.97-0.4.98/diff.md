# Comparing `tmp/arkitekt-0.4.97.tar.gz` & `tmp/arkitekt-0.4.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkitekt-0.4.97.tar", max compression
+gzip compressed data, was "arkitekt-0.4.98.tar", max compression
```

## Comparing `arkitekt-0.4.97.tar` & `arkitekt-0.4.98.tar`

### file list

```diff
@@ -1,53 +1,54 @@
--rw-r--r--   0        0        0      402 2023-04-28 12:28:13.330574 arkitekt-0.4.97/arkitekt/__init__.py
--rw-r--r--   0        0        0       54 2022-09-28 15:15:28.986749 arkitekt-0.4.97/arkitekt/apps/__init__.py
--rw-r--r--   0        0        0      839 2023-04-19 15:51:04.434687 arkitekt-0.4.97/arkitekt/apps/connected.py
--rw-r--r--   0        0        0      979 2022-11-21 14:18:14.617734 arkitekt-0.4.97/arkitekt/apps/default.py
--rw-r--r--   0        0        0      299 2023-03-10 11:35:23.703615 arkitekt-0.4.97/arkitekt/apps/fakts.py
--rw-r--r--   0        0        0     1869 2023-03-10 11:35:23.703615 arkitekt-0.4.97/arkitekt/apps/fluss.py
--rw-r--r--   0        0        0      293 2023-03-10 11:35:23.703615 arkitekt-0.4.97/arkitekt/apps/herre.py
--rw-r--r--   0        0        0     2842 2023-02-14 16:53:09.149069 arkitekt-0.4.97/arkitekt/apps/mikro.py
--rw-r--r--   0        0        0     2274 2022-12-15 15:50:35.665918 arkitekt-0.4.97/arkitekt/apps/rekuest.py
--rw-r--r--   0        0        0      768 2023-04-19 08:13:05.317863 arkitekt-0.4.97/arkitekt/apps/unlok.py
--rw-r--r--   0        0        0    12110 2023-04-28 12:32:17.575384 arkitekt-0.4.97/arkitekt/builders.py
--rw-r--r--   0        0        0        0 2022-08-25 10:31:18.672462 arkitekt-0.4.97/arkitekt/cli/__init__.py
--rw-r--r--   0        0        0     5962 2023-03-30 09:24:17.794873 arkitekt-0.4.97/arkitekt/cli/build.py
--rw-r--r--   0        0        0    11011 2023-03-09 14:31:34.404795 arkitekt-0.4.97/arkitekt/cli/configs/introspect.yaml
--rw-r--r--   0        0        0    11706 2023-04-28 14:16:38.131941 arkitekt-0.4.97/arkitekt/cli/configs/latest.yaml
--rw-r--r--   0        0        0    11126 2023-03-09 14:46:09.667053 arkitekt-0.4.97/arkitekt/cli/configs/minimal.yaml
--rw-r--r--   0        0        0     3147 2023-03-30 10:04:52.303630 arkitekt-0.4.97/arkitekt/cli/deploy.py
--rw-r--r--   0        0        0     7187 2023-04-28 13:34:41.530924 arkitekt-0.4.97/arkitekt/cli/dev.py
--rw-r--r--   0        0        0     5546 2023-03-10 11:35:23.703615 arkitekt-0.4.97/arkitekt/cli/gen.py
--rw-r--r--   0        0        0     1355 2023-03-30 02:16:07.818458 arkitekt-0.4.97/arkitekt/cli/init.py
--rw-r--r--   0        0        0     1476 2023-03-30 08:40:09.488953 arkitekt-0.4.97/arkitekt/cli/inspect.py
--rw-r--r--   0        0        0    22518 2023-04-28 12:33:53.363792 arkitekt-0.4.97/arkitekt/cli/main.py
--rw-r--r--   0        0        0     2295 2023-04-28 12:32:03.303322 arkitekt-0.4.97/arkitekt/cli/run.py
--rw-r--r--   0        0        0      871 2023-03-10 11:35:23.703615 arkitekt-0.4.97/arkitekt/cli/scan.py
--rw-r--r--   0        0        0    24496 2023-04-28 14:09:38.190295 arkitekt-0.4.97/arkitekt/cli/schemas/latest/fluss.schema.graphql
--rw-r--r--   0        0        0   118448 2023-04-28 14:09:38.442296 arkitekt-0.4.97/arkitekt/cli/schemas/latest/gucker.schema.graphql
--rw-r--r--   0        0        0     4905 2023-04-28 14:09:38.226296 arkitekt-0.4.97/arkitekt/cli/schemas/latest/kuay.schema.graphql
--rw-r--r--   0        0        0   118448 2023-04-28 14:09:38.022295 arkitekt-0.4.97/arkitekt/cli/schemas/latest/mikro.schema.graphql
--rw-r--r--   0        0        0    51282 2023-04-28 14:09:38.118295 arkitekt-0.4.97/arkitekt/cli/schemas/latest/rekuest.schema.graphql
--rw-r--r--   0        0        0    10014 2023-04-28 14:09:38.270296 arkitekt-0.4.97/arkitekt/cli/schemas/latest/unlok.schema.graphql
--rw-r--r--   0        0        0      208 2023-03-10 15:06:16.963555 arkitekt-0.4.97/arkitekt/cli/templates/simple.py
--rw-r--r--   0        0        0     1302 2023-04-18 10:30:28.953168 arkitekt-0.4.97/arkitekt/cli/types.py
--rw-r--r--   0        0        0     1883 2023-03-10 12:35:52.050986 arkitekt-0.4.97/arkitekt/cli/ui.py
--rw-r--r--   0        0        0      429 2023-03-10 10:47:37.959663 arkitekt-0.4.97/arkitekt/cli/utils.py
--rw-r--r--   0        0        0      271 2023-03-10 11:35:23.703615 arkitekt-0.4.97/arkitekt/deployers/port.py
--rw-r--r--   0        0        0     1910 2022-10-22 17:12:22.527311 arkitekt-0.4.97/arkitekt/healthz.py
--rw-r--r--   0        0        0        0 2022-08-25 11:14:04.331138 arkitekt-0.4.97/arkitekt/qt/__init__.py
--rw-r--r--   0        0        0     6296 2022-08-25 10:31:18.764461 arkitekt-0.4.97/arkitekt/qt/assets/dark/gear.png
--rw-r--r--   0        0        0   105386 2022-08-25 10:31:18.764461 arkitekt-0.4.97/arkitekt/qt/assets/dark/green pulse.gif
--rw-r--r--   0        0        0    94769 2022-08-25 10:31:18.764461 arkitekt-0.4.97/arkitekt/qt/assets/dark/orange pulse.gif
--rw-r--r--   0        0        0   107513 2022-08-25 10:31:18.768461 arkitekt-0.4.97/arkitekt/qt/assets/dark/pink pulse.gif
--rw-r--r--   0        0        0   108749 2022-08-25 10:31:18.768461 arkitekt-0.4.97/arkitekt/qt/assets/dark/red pulse.gif
--rw-r--r--   0        0        0    10710 2022-08-25 10:31:18.768461 arkitekt-0.4.97/arkitekt/qt/assets/light/gear.png
--rw-r--r--   0        0        0   105386 2022-08-25 10:31:18.768461 arkitekt-0.4.97/arkitekt/qt/assets/light/green pulse.gif
--rw-r--r--   0        0        0    94769 2022-08-25 10:31:18.768461 arkitekt-0.4.97/arkitekt/qt/assets/light/orange pulse.gif
--rw-r--r--   0        0        0   107513 2022-08-25 10:31:18.772461 arkitekt-0.4.97/arkitekt/qt/assets/light/pink pulse.gif
--rw-r--r--   0        0        0   108749 2022-08-25 10:31:18.772461 arkitekt-0.4.97/arkitekt/qt/assets/light/red pulse.gif
--rw-r--r--   0        0        0     9166 2023-03-10 11:35:23.703615 arkitekt-0.4.97/arkitekt/qt/magic_bar.py
--rw-r--r--   0        0        0      324 2022-08-25 11:16:26.752819 arkitekt-0.4.97/arkitekt/qt/utils.py
--rw-r--r--   0        0        0      765 2023-03-17 17:13:40.500701 arkitekt-0.4.97/arkitekt/tqdm.py
--rw-r--r--   0        0        0     4801 2023-04-28 11:12:47.743764 arkitekt-0.4.97/arkitekt/utils.py
--rw-r--r--   0        0        0     2001 2023-04-28 14:23:12.101732 arkitekt-0.4.97/pyproject.toml
--rw-r--r--   0        0        0     1102 1970-01-01 00:00:00.000000 arkitekt-0.4.97/PKG-INFO
+-rw-r--r--   0        0        0      402 2023-04-28 12:28:13.330574 arkitekt-0.4.98/arkitekt/__init__.py
+-rw-r--r--   0        0        0       54 2022-09-28 15:15:28.986749 arkitekt-0.4.98/arkitekt/apps/__init__.py
+-rw-r--r--   0        0        0      839 2023-04-19 15:51:04.434687 arkitekt-0.4.98/arkitekt/apps/connected.py
+-rw-r--r--   0        0        0      979 2022-11-21 14:18:14.617734 arkitekt-0.4.98/arkitekt/apps/default.py
+-rw-r--r--   0        0        0      299 2023-03-10 11:35:23.703615 arkitekt-0.4.98/arkitekt/apps/fakts.py
+-rw-r--r--   0        0        0     1869 2023-03-10 11:35:23.703615 arkitekt-0.4.98/arkitekt/apps/fluss.py
+-rw-r--r--   0        0        0      293 2023-03-10 11:35:23.703615 arkitekt-0.4.98/arkitekt/apps/herre.py
+-rw-r--r--   0        0        0     2842 2023-02-14 16:53:09.149069 arkitekt-0.4.98/arkitekt/apps/mikro.py
+-rw-r--r--   0        0        0     2274 2022-12-15 15:50:35.665918 arkitekt-0.4.98/arkitekt/apps/rekuest.py
+-rw-r--r--   0        0        0      768 2023-04-19 08:13:05.317863 arkitekt-0.4.98/arkitekt/apps/unlok.py
+-rw-r--r--   0        0        0    12107 2023-05-02 10:57:58.871349 arkitekt-0.4.98/arkitekt/builders.py
+-rw-r--r--   0        0        0        0 2022-08-25 10:31:18.672462 arkitekt-0.4.98/arkitekt/cli/__init__.py
+-rw-r--r--   0        0        0     5962 2023-03-30 09:24:17.794873 arkitekt-0.4.98/arkitekt/cli/build.py
+-rw-r--r--   0        0        0    11011 2023-03-09 14:31:34.404795 arkitekt-0.4.98/arkitekt/cli/configs/introspect.yaml
+-rw-r--r--   0        0        0    11706 2023-04-28 14:16:38.131941 arkitekt-0.4.98/arkitekt/cli/configs/latest.yaml
+-rw-r--r--   0        0        0    11126 2023-03-09 14:46:09.667053 arkitekt-0.4.98/arkitekt/cli/configs/minimal.yaml
+-rw-r--r--   0        0        0     3147 2023-03-30 10:04:52.303630 arkitekt-0.4.98/arkitekt/cli/deploy.py
+-rw-r--r--   0        0        0     7327 2023-05-02 09:22:57.877413 arkitekt-0.4.98/arkitekt/cli/dev.py
+-rw-r--r--   0        0        0     5546 2023-03-10 11:35:23.703615 arkitekt-0.4.98/arkitekt/cli/gen.py
+-rw-r--r--   0        0        0     1355 2023-03-30 02:16:07.818458 arkitekt-0.4.98/arkitekt/cli/init.py
+-rw-r--r--   0        0        0     1476 2023-03-30 08:40:09.488953 arkitekt-0.4.98/arkitekt/cli/inspect.py
+-rw-r--r--   0        0        0    22346 2023-05-02 08:33:52.316141 arkitekt-0.4.98/arkitekt/cli/main.py
+-rw-r--r--   0        0        0     2420 2023-05-02 08:31:56.092091 arkitekt-0.4.98/arkitekt/cli/run.py
+-rw-r--r--   0        0        0      871 2023-03-10 11:35:23.703615 arkitekt-0.4.98/arkitekt/cli/scan.py
+-rw-r--r--   0        0        0    24496 2023-05-02 10:57:15.091215 arkitekt-0.4.98/arkitekt/cli/schemas/latest/fluss.schema.graphql
+-rw-r--r--   0        0        0   118448 2023-05-02 10:57:15.323216 arkitekt-0.4.98/arkitekt/cli/schemas/latest/gucker.schema.graphql
+-rw-r--r--   0        0        0     4820 2023-05-02 10:57:15.127215 arkitekt-0.4.98/arkitekt/cli/schemas/latest/kuay.schema.graphql
+-rw-r--r--   0        0        0   118448 2023-05-02 10:57:14.919215 arkitekt-0.4.98/arkitekt/cli/schemas/latest/mikro.schema.graphql
+-rw-r--r--   0        0        0    51282 2023-05-02 10:57:15.015215 arkitekt-0.4.98/arkitekt/cli/schemas/latest/rekuest.schema.graphql
+-rw-r--r--   0        0        0     9948 2023-05-02 10:57:15.167215 arkitekt-0.4.98/arkitekt/cli/schemas/latest/unlok.schema.graphql
+-rw-r--r--   0        0        0      208 2023-03-10 15:06:16.963555 arkitekt-0.4.98/arkitekt/cli/templates/simple.py
+-rw-r--r--   0        0        0     1326 2023-05-02 08:14:53.195649 arkitekt-0.4.98/arkitekt/cli/types.py
+-rw-r--r--   0        0        0     1883 2023-03-10 12:35:52.050986 arkitekt-0.4.98/arkitekt/cli/ui.py
+-rw-r--r--   0        0        0      429 2023-03-10 10:47:37.959663 arkitekt-0.4.98/arkitekt/cli/utils.py
+-rw-r--r--   0        0        0      271 2023-03-10 11:35:23.703615 arkitekt-0.4.98/arkitekt/deployers/port.py
+-rw-r--r--   0        0        0     1910 2022-10-22 17:12:22.527311 arkitekt-0.4.98/arkitekt/healthz.py
+-rw-r--r--   0        0        0        0 2022-08-25 11:14:04.331138 arkitekt-0.4.98/arkitekt/qt/__init__.py
+-rw-r--r--   0        0        0     6296 2022-08-25 10:31:18.764461 arkitekt-0.4.98/arkitekt/qt/assets/dark/gear.png
+-rw-r--r--   0        0        0   105386 2022-08-25 10:31:18.764461 arkitekt-0.4.98/arkitekt/qt/assets/dark/green pulse.gif
+-rw-r--r--   0        0        0    94769 2022-08-25 10:31:18.764461 arkitekt-0.4.98/arkitekt/qt/assets/dark/orange pulse.gif
+-rw-r--r--   0        0        0   107513 2022-08-25 10:31:18.768461 arkitekt-0.4.98/arkitekt/qt/assets/dark/pink pulse.gif
+-rw-r--r--   0        0        0   108749 2022-08-25 10:31:18.768461 arkitekt-0.4.98/arkitekt/qt/assets/dark/red pulse.gif
+-rw-r--r--   0        0        0    10710 2022-08-25 10:31:18.768461 arkitekt-0.4.98/arkitekt/qt/assets/light/gear.png
+-rw-r--r--   0        0        0   105386 2022-08-25 10:31:18.768461 arkitekt-0.4.98/arkitekt/qt/assets/light/green pulse.gif
+-rw-r--r--   0        0        0    94769 2022-08-25 10:31:18.768461 arkitekt-0.4.98/arkitekt/qt/assets/light/orange pulse.gif
+-rw-r--r--   0        0        0   107513 2022-08-25 10:31:18.772461 arkitekt-0.4.98/arkitekt/qt/assets/light/pink pulse.gif
+-rw-r--r--   0        0        0   108749 2022-08-25 10:31:18.772461 arkitekt-0.4.98/arkitekt/qt/assets/light/red pulse.gif
+-rw-r--r--   0        0        0     9166 2023-03-10 11:35:23.703615 arkitekt-0.4.98/arkitekt/qt/magic_bar.py
+-rw-r--r--   0        0        0      324 2022-08-25 11:16:26.752819 arkitekt-0.4.98/arkitekt/qt/utils.py
+-rw-r--r--   0        0        0        0 2023-05-02 08:15:03.535653 arkitekt-0.4.98/arkitekt/runners.py
+-rw-r--r--   0        0        0      765 2023-03-17 17:13:40.500701 arkitekt-0.4.98/arkitekt/tqdm.py
+-rw-r--r--   0        0        0     4801 2023-04-28 11:12:47.743764 arkitekt-0.4.98/arkitekt/utils.py
+-rw-r--r--   0        0        0     2001 2023-05-02 11:00:28.631822 arkitekt-0.4.98/pyproject.toml
+-rw-r--r--   0        0        0     1102 1970-01-01 00:00:00.000000 arkitekt-0.4.98/PKG-INFO
```

### Comparing `arkitekt-0.4.97/arkitekt/apps/connected.py` & `arkitekt-0.4.98/arkitekt/apps/connected.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.97/arkitekt/apps/default.py` & `arkitekt-0.4.98/arkitekt/apps/default.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.97/arkitekt/apps/fluss.py` & `arkitekt-0.4.98/arkitekt/apps/fluss.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.97/arkitekt/apps/mikro.py` & `arkitekt-0.4.98/arkitekt/apps/mikro.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.97/arkitekt/apps/rekuest.py` & `arkitekt-0.4.98/arkitekt/apps/rekuest.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.97/arkitekt/apps/unlok.py` & `arkitekt-0.4.98/arkitekt/apps/unlok.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.97/arkitekt/builders.py` & `arkitekt-0.4.98/arkitekt/builders.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,15 +283,15 @@
     )
 
 
 def publicqt(
     identifier: str,
     version: str = "latest",
     parent=None,
-    image: Optional[str] = None,
+    logo: Optional[str] = None,
     scopes: Optional[List[str]] = None,
     beacon_widget=None,
     login_widget=None,
     force_herre_grant=None,
     instance_id: str = "main",
     no_cache: bool = False,
 ) -> App:
@@ -318,15 +318,15 @@
         QtSelectableDiscovery,
     )
 
     manifest = Manifest(
         version=version,
         identifier=identifier,
         scopes=scopes or ["openid", "read", "write"],
-        image=image,
+        logo=logo,
     )
 
     create_arkitekt_folder(with_cache=True)
 
     beacon_widget = beacon_widget or SelectBeaconWidget(parent=parent)
 
     login_widget = login_widget or LoginWidget(identifier, version, parent=parent)
```

### Comparing `arkitekt-0.4.97/arkitekt/cli/build.py` & `arkitekt-0.4.98/arkitekt/cli/build.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.97/arkitekt/cli/configs/introspect.yaml` & `arkitekt-0.4.98/arkitekt/cli/configs/introspect.yaml`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.97/arkitekt/cli/configs/latest.yaml` & `arkitekt-0.4.98/arkitekt/cli/configs/latest.yaml`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.97/arkitekt/cli/configs/minimal.yaml` & `arkitekt-0.4.98/arkitekt/cli/configs/minimal.yaml`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.97/arkitekt/cli/deploy.py` & `arkitekt-0.4.98/arkitekt/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.97/arkitekt/cli/dev.py` & `arkitekt-0.4.98/arkitekt/cli/dev.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from rich import get_console
 import sys
 import inspect
 from rekuest.definition.registry import get_default_definition_registry
 from typing import MutableSet, Tuple, Any
 from arkitekt.cli.ui import construct_changes_group, construct_app_group
 from arkitekt.cli.utils import import_builder
+from .types import Manifest
 
 
 async def build_and_run(app):
     async with app:
         await app.rekuest.run()
 
 
@@ -75,25 +76,27 @@
     for change, path in changes:
         if os.path.normpath(path) == entrypoint_real_path:
             return True
     return False
 
 
 async def dev_module(
-    identifier=None,
+    manifest: Manifest,
     version=None,
-    entrypoint=None,
-    instance_id=None,
     url=None,
     builder: str = "arkitekt.builders.easy",
     deep: bool = False,
     headless: bool = False,
     nocache: bool = False,
+    instance_id: str = None,
 ):
-    entrypoint_file = f"{entrypoint}.py"
+    entrypoint = manifest.entrypoint
+    identifier = manifest.identifier
+    version = version or "dev"
+    entrypoint_file = f"{manifest.entrypoint}.py"
     entypoint_real_path = os.path.realpath(entrypoint_file)
 
     builder_func = import_builder(builder)
 
     console = get_console()
 
     generation_message = "[not bold white]This is a development tool for arkitekt apps. It will watch your app for changes and reload it when it detects a change. It will also print out the current state of your app.[/]"
@@ -108,15 +111,15 @@
         style="bold green",
         border_style="green",
         title="Arkitekt Dev Mode",
     )
     console.print(panel)
 
     try:
-        module = import_module(entrypoint)
+        module = import_module(manifest.entrypoint)
 
     except Exception:
         console.print_exception()
         panel = Panel(
             f"Error while importing your entrypoint please fix your file {entrypoint} and save",
             style="bold red",
             border_style="red",
```

### Comparing `arkitekt-0.4.97/arkitekt/cli/gen.py` & `arkitekt-0.4.98/arkitekt/cli/gen.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.97/arkitekt/cli/init.py` & `arkitekt-0.4.98/arkitekt/cli/init.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.97/arkitekt/cli/inspect.py` & `arkitekt-0.4.98/arkitekt/cli/inspect.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.97/arkitekt/cli/main.py` & `arkitekt-0.4.98/arkitekt/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,17 +181,15 @@
     if not manifest:
         raise click.ClickException(
             "No manifest found. Please run `arkitekt init` first before deploying an arkitekt app."
         )
 
     asyncio.run(
         run_easy(
-            entrypoint=manifest.entrypoint,
-            identifier=manifest.identifier,
-            version=version or manifest.version,
+            manifest=manifest,
             url=url,
             instance_id=instance,
             headless=headless,
             nocache=nocache,
         )
     )
 
@@ -297,17 +295,16 @@
     if not manifest:
         raise click.ClickException(
             "No manifest found. Please run `arkitekt init` first before deploying an arkitekt app."
         )
 
     asyncio.run(
         dev_module(
-            identifier=manifest.identifier,
-            version=version or "dev",
-            entrypoint=manifest.entrypoint,
+            manifest=manifest,
+            version=version,
             builder=builder,
             deep=deep,
             url=url,
             instance_id=instance,
             headless=headless,
             nocache=nocache,
         )
```

### Comparing `arkitekt-0.4.97/arkitekt/cli/scan.py` & `arkitekt-0.4.98/arkitekt/cli/scan.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.97/arkitekt/cli/schemas/latest/fluss.schema.graphql` & `arkitekt-0.4.98/arkitekt/cli/schemas/latest/fluss.schema.graphql`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.97/arkitekt/cli/schemas/latest/gucker.schema.graphql` & `arkitekt-0.4.98/arkitekt/cli/schemas/latest/gucker.schema.graphql`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.97/arkitekt/cli/schemas/latest/kuay.schema.graphql` & `arkitekt-0.4.98/arkitekt/cli/schemas/latest/kuay.schema.graphql`

 * *Files 2% similar despite different names*

```diff
@@ -109,21 +109,17 @@
   latestPull: DateTime
   containers: [Container]
 }
 
 type Deployment {
   """"""
   id: ID!
-
-  """"""
   version: String!
-
-  """"""
   identifier: String!
-  scopes: GenericScalar
+  scopes: [String]!
   requirements: GenericScalar
 
   """"""
   repo: GithubRepo
 
   """"""
   createdAt: DateTime!
@@ -158,17 +154,14 @@
   branch: String!
 
   """"""
   createdAt: DateTime!
 
   """"""
   deployments: [Deployment!]!
-  version: String!
-  identifier: String!
-  scopes: [String]!
   readme: String
 }
 
 """
 The `DateTime` scalar type represents a DateTime
 value as specified by
 [iso8601](https://en.wikipedia.org/wiki/ISO_8601).
```

### Comparing `arkitekt-0.4.97/arkitekt/cli/schemas/latest/mikro.schema.graphql` & `arkitekt-0.4.98/arkitekt/cli/schemas/latest/mikro.schema.graphql`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.97/arkitekt/cli/schemas/latest/rekuest.schema.graphql` & `arkitekt-0.4.98/arkitekt/cli/schemas/latest/rekuest.schema.graphql`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.97/arkitekt/cli/schemas/latest/unlok.schema.graphql` & `arkitekt-0.4.98/arkitekt/cli/schemas/latest/unlok.schema.graphql`

 * *Files 12% similar despite different names*

```diff
@@ -11,20 +11,15 @@
   ): Application
   applications: [Application]
   myapplications: [Application]
   application(
     """The ID to search by"""
     clientId: ID!
   ): Application
-  clients: [Application]
   myclients: [Application]
-  client(
-    """The ID to search by"""
-    id: ID!
-  ): Application
   scopes(
     """Unique app name for user"""
     search: String
 
     """Unique app name for user"""
     values: [ID]
   ): [Scope]
@@ -92,53 +87,61 @@
 
     """Search for substring of username"""
     search: String
 
     """Filter by user"""
     user: ID
   ): [Channel]
-  privatefaktapp(
+  client(
     """The FaktApp ID"""
     id: ID
 
-    """Unique app name for user"""
-    identifier: String
+    """The client id of one associated oauth2 application"""
+    clientId: ID
 
-    """Unique app name for user"""
-    version: String
-  ): FaktApplication
-  privatefaktapps: [FaktApplication]
-  publicfaktapp(
+    """The FaktApp ID"""
+    token: ID
+  ): Client
+  myPrivateClients: [Client]
+  clients: [Client]
+  myPublicClients: [Client]
+  app(
     """The FaktApp ID"""
     id: ID
 
     """Unique app name for user"""
     identifier: String
 
     """Unique app name for user"""
     version: String
-  ): FaktApplication
-  publicfaktapps: [FaktApplication]
-  app(
+
+    """The client id of one associated oauth2 application"""
+    clientId: ID
+  ): App
+  apps(
+    """Search for substring of identifier"""
+    search: String
+  ): [App]
+  release(
     """The FaktApp ID"""
     id: ID
 
     """Unique app name for user"""
     identifier: String
 
     """Unique app name for user"""
     version: String
 
     """The client id of one associated oauth2 application"""
-    clientId: String
-  ): App
-  apps(
-    """Search for substring of identifier"""
-    search: String
-  ): [App]
+    clientId: ID
+  ): Release
+  releases(
+    """Filter by app"""
+    app: ID
+  ): [Release]
 
   """Get information on your Docker Template"""
   member(
     """The Whale ID"""
     id: ID!
   ): Member
   graphs: [Graph]
@@ -173,15 +176,15 @@
   created: DateTime!
 
   """"""
   updated: DateTime!
 
   """"""
   algorithm: ApplicationAlgorithm
-  faktapplication: FaktApplication
+  client: Client
 
   """The Url of the Image"""
   image: String
 }
 
 type HerreUser {
   """"""
@@ -294,67 +297,79 @@
   """RSA with SHA-2 256"""
   RS256
 
   """HMAC with SHA-2 256"""
   HS256
 }
 
-type FaktApplication {
+type Client {
   """"""
   id: ID!
 
   """"""
-  app: App
+  release: Release
 
   """"""
-  application: Application!
+  oauth2Client: Application!
 
   """"""
-  kind: FaktApplicationKind
+  kind: ClientKind
 
   """"""
   token: String!
 
   """"""
   clientId: String!
 
   """"""
   clientSecret: String!
   scopes: [String]!
 
   """"""
-  logo: String
-
-  """"""
   creator: HerreUser!
 
   """"""
   user: HerreUser
 }
 
-type App {
+type Release {
   """"""
   id: ID!
 
   """"""
-  identifier: String!
+  app: App!
 
   """"""
   version: String!
 
   """"""
   name: String!
   logo: String
 
   """"""
-  faktApplications: [FaktApplication!]!
+  clients: [Client!]!
+}
+
+type App {
+  """"""
+  id: ID!
+
+  """"""
+  name: String!
+
+  """"""
+  identifier: String!
+  logo: String
+
+  """"""
+  releases: [Release!]!
 }
 
 """An enumeration."""
-enum FaktApplicationKind {
+enum ClientKind {
   """Website"""
   WEBSITE
 
   """Dekstop"""
   DESKTOP
 
   """User"""
@@ -449,14 +464,17 @@
 
   """"""
   identifier: String
   scopes: GenericScalar
 
   """"""
   graph: Graph
+
+  """"""
+  logo: String
 }
 
 """The root Mutation"""
 type Mutation {
   deleteApplication(
     """The ID of the application"""
     clientId: ID!
@@ -506,51 +524,47 @@
     name: String
 
     """The expo token"""
     token: String!
   ): Channel
   publishToChannel(channel: ID!, message: String!, title: String!): PublishResult
   notifyUser(channels: [String], message: String!, title: String!, user: ID!): [PublishResult]
-  createPrivateFakt(
+  createPrivateClient(
     """The Name of this Elemet"""
     identifier: String!
 
     """The ID of the User to imitate (only managers can do this)"""
     imitate: ID
 
     """A list of potential scopes for this app"""
     scopes: [String]!
 
     """The Repo of the Docker (Repo on Dockerhub)"""
     version: String!
-  ): FaktApplication
-  createPublicFakt(
+  ): Client
+  createPublicClient(
     """The Name of this Elemet"""
     identifier: String!
 
     """The kind of this app"""
     kind: PublicFaktType!
 
     """A list of potential redirects for this app"""
     redirectUris: [String]!
 
     """A list of potential scopes for this app"""
     scopes: [String]!
 
     """The Repo of the Docker (Repo on Dockerhub)"""
     version: String!
-  ): FaktApplication
-  deletePrivateFakt(
-    """The ID of the application"""
-    id: ID!
-  ): DeletePrivateFaktResult
-  deletePublicFakt(
+  ): Client
+  deleteClient(
     """The ID of the application"""
     id: ID!
-  ): DeletePublicFaktResult
+  ): DeleteClientResult
   updateApp(
     """The id of the app"""
     id: ID!
 
     """The Logo of this Apps"""
     logo: Upload
   ): App
@@ -604,17 +618,13 @@
 }
 
 enum PublicFaktType {
   DEKSTOP
   WEBSITE
 }
 
-type DeletePrivateFaktResult {
-  id: ID
-}
-
-type DeletePublicFaktResult {
+type DeleteClientResult {
   id: ID
 }
 
 """The configuration"""
 scalar Config
```

### Comparing `arkitekt-0.4.97/arkitekt/cli/types.py` & `arkitekt-0.4.98/arkitekt/cli/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     PIP = "pip"
 
 
 class Manifest(BaseModel):
     identifier: str
     version: str
     author: str
+    logo: Optional[str]
     entrypoint: str
     scopes: List[str]
     requirements: List[Requirement] = Field(default_factory=list)
     created_at: datetime.datetime = Field(default_factory=datetime.datetime.now)
 
 
 class PortBuild(BaseModel):
```

### Comparing `arkitekt-0.4.97/arkitekt/cli/ui.py` & `arkitekt-0.4.98/arkitekt/cli/ui.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.97/arkitekt/healthz.py` & `arkitekt-0.4.98/arkitekt/healthz.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.97/arkitekt/qt/assets/dark/gear.png` & `arkitekt-0.4.98/arkitekt/qt/assets/dark/gear.png`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.97/arkitekt/qt/assets/dark/green pulse.gif` & `arkitekt-0.4.98/arkitekt/qt/assets/dark/green pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.97/arkitekt/qt/assets/dark/orange pulse.gif` & `arkitekt-0.4.98/arkitekt/qt/assets/dark/orange pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.97/arkitekt/qt/assets/dark/pink pulse.gif` & `arkitekt-0.4.98/arkitekt/qt/assets/dark/pink pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.97/arkitekt/qt/assets/dark/red pulse.gif` & `arkitekt-0.4.98/arkitekt/qt/assets/dark/red pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.97/arkitekt/qt/assets/light/gear.png` & `arkitekt-0.4.98/arkitekt/qt/assets/light/gear.png`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.97/arkitekt/qt/assets/light/green pulse.gif` & `arkitekt-0.4.98/arkitekt/qt/assets/light/green pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.97/arkitekt/qt/assets/light/orange pulse.gif` & `arkitekt-0.4.98/arkitekt/qt/assets/light/orange pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.97/arkitekt/qt/assets/light/pink pulse.gif` & `arkitekt-0.4.98/arkitekt/qt/assets/light/pink pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.97/arkitekt/qt/assets/light/red pulse.gif` & `arkitekt-0.4.98/arkitekt/qt/assets/light/red pulse.gif`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.97/arkitekt/qt/magic_bar.py` & `arkitekt-0.4.98/arkitekt/qt/magic_bar.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.97/arkitekt/tqdm.py` & `arkitekt-0.4.98/arkitekt/tqdm.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.97/arkitekt/utils.py` & `arkitekt-0.4.98/arkitekt/utils.py`

 * *Files identical despite different names*

### Comparing `arkitekt-0.4.97/pyproject.toml` & `arkitekt-0.4.98/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "arkitekt"
-version = "0.4.97"
+version = "0.4.98"
 description = "client for the arkitekt platform"
 authors = ["jhnnsrs <jhnnsrs@gmail.com>"]
 license = "CC BY-NC 3.0"
 packages = [{ include = "arkitekt" }]
 
 [tool.poetry.dependencies]
 python = "^3.8, <=3.12"
-herre = ">=0.3.18"
-fakts = ">=0.3.20"
+herre = ">=0.3.19"
+fakts = ">=0.3.21"
 rekuest = ">=0.1.30"
-mikro = ">=0.3.60"
+mikro = ">=0.3.61"
 unlok = ">=0.1.12"
-fluss = ">=0.1.46"
+fluss = ">=0.1.47"
 rich-click = { version = "^1.6.1", optional = true }
 watchfiles = { version = "^0.18.1", optional = true }
 turms = { version = ">=0.3.1a0", python = "^3.9", optional = true }
 reaktion = { version = ">=0.1.21", python = "^3.9", optional = true }
 
 
 [tool.poetry.extras]
```

### Comparing `arkitekt-0.4.97/PKG-INFO` & `arkitekt-0.4.98/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: arkitekt
-Version: 0.4.97
+Version: 0.4.98
 Summary: client for the arkitekt platform
 License: CC BY-NC 3.0
 Author: jhnnsrs
 Author-email: jhnnsrs@gmail.com
 Requires-Python: >=3.8,<=3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: cli
 Provides-Extra: scheduler
-Requires-Dist: fakts (>=0.3.20)
-Requires-Dist: fluss (>=0.1.46)
-Requires-Dist: herre (>=0.3.18)
-Requires-Dist: mikro (>=0.3.60)
+Requires-Dist: fakts (>=0.3.21)
+Requires-Dist: fluss (>=0.1.47)
+Requires-Dist: herre (>=0.3.19)
+Requires-Dist: mikro (>=0.3.61)
 Requires-Dist: reaktion (>=0.1.21) ; (python_version >= "3.9" and python_version < "4.0") and (extra == "scheduler")
 Requires-Dist: rekuest (>=0.1.30)
 Requires-Dist: rich-click (>=1.6.1,<2.0.0) ; extra == "cli"
 Requires-Dist: turms (>=0.3.1a0) ; (python_version >= "3.9" and python_version < "4.0") and (extra == "cli")
 Requires-Dist: unlok (>=0.1.12)
 Requires-Dist: watchfiles (>=0.18.1,<0.19.0) ; extra == "cli"
```

