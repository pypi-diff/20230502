# Comparing `tmp/webui2-2.2.0.1.tar.gz` & `tmp/webui2-2.2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webui2-2.2.0.1.tar", last modified: Sun Apr 30 23:49:08 2023, max compression
+gzip compressed data, was "webui2-2.2.0.2.tar", last modified: Tue May  2 12:43:32 2023, max compression
```

## Comparing `webui2-2.2.0.1.tar` & `webui2-2.2.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 23:49:08.914609 webui2-2.2.0.1/
--rw-rw-rw-   0        0        0    35149 2023-04-29 20:30:45.000000 webui2-2.2.0.1/LICENSE
--rw-rw-rw-   0        0        0     1125 2023-04-30 23:49:08.913184 webui2-2.2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      583 2023-04-29 20:30:45.000000 webui2-2.2.0.1/README.md
--rw-rw-rw-   0        0        0      746 2023-04-30 23:45:45.000000 webui2-2.2.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-30 23:49:08.914609 webui2-2.2.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-30 23:49:08.902814 webui2-2.2.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-30 23:49:08.909882 webui2-2.2.0.1/src/webui/
--rw-rw-rw-   0        0        0        0 2023-04-29 20:30:45.000000 webui2-2.2.0.1/src/webui/__init__.py
--rw-rw-rw-   0        0        0   388608 2023-04-30 20:52:33.000000 webui2-2.2.0.1/src/webui/webui-2-x64.dll
--rw-rw-rw-   0        0        0   199040 2023-04-30 23:37:39.000000 webui2-2.2.0.1/src/webui/webui-2-x64.dyn
--rw-rw-rw-   0        0        0   198704 2023-04-30 23:32:35.000000 webui2-2.2.0.1/src/webui/webui-2-x64.so
--rw-rw-rw-   0        0        0    10857 2023-04-29 20:30:45.000000 webui2-2.2.0.1/src/webui/webui.py
-drwxrwxrwx   0        0        0        0 2023-04-30 23:49:08.913184 webui2-2.2.0.1/src/webui2.egg-info/
--rw-rw-rw-   0        0        0     1125 2023-04-30 23:49:08.000000 webui2-2.2.0.1/src/webui2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2023-04-30 23:49:08.000000 webui2-2.2.0.1/src/webui2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 23:49:08.000000 webui2-2.2.0.1/src/webui2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-30 23:49:08.000000 webui2-2.2.0.1/src/webui2.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 12:43:32.746071 webui2-2.2.0.2/
+-rw-rw-rw-   0        0        0    35149 2023-04-29 20:30:45.000000 webui2-2.2.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1125 2023-05-02 12:43:32.746071 webui2-2.2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      583 2023-04-29 20:30:45.000000 webui2-2.2.0.2/README.md
+-rw-rw-rw-   0        0        0      746 2023-05-02 12:42:20.000000 webui2-2.2.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-02 12:43:32.750083 webui2-2.2.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-02 12:43:32.736533 webui2-2.2.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 12:43:32.746071 webui2-2.2.0.2/src/webui/
+-rw-rw-rw-   0        0        0        0 2023-04-29 20:30:45.000000 webui2-2.2.0.2/src/webui/__init__.py
+-rw-rw-rw-   0        0        0   388608 2023-04-30 20:52:33.000000 webui2-2.2.0.2/src/webui/webui-2-x64.dll
+-rw-rw-rw-   0        0        0   199040 2023-04-30 23:37:39.000000 webui2-2.2.0.2/src/webui/webui-2-x64.dyn
+-rw-rw-rw-   0        0        0   198704 2023-04-30 23:32:35.000000 webui2-2.2.0.2/src/webui/webui-2-x64.so
+-rw-rw-rw-   0        0        0    10855 2023-05-02 12:42:05.000000 webui2-2.2.0.2/src/webui/webui.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:43:32.746071 webui2-2.2.0.2/src/webui2.egg-info/
+-rw-rw-rw-   0        0        0     1125 2023-05-02 12:43:32.000000 webui2-2.2.0.2/src/webui2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2023-05-02 12:43:32.000000 webui2-2.2.0.2/src/webui2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 12:43:32.000000 webui2-2.2.0.2/src/webui2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-02 12:43:32.000000 webui2-2.2.0.2/src/webui2.egg-info/top_level.txt
```

### Comparing `webui2-2.2.0.1/LICENSE` & `webui2-2.2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `webui2-2.2.0.1/PKG-INFO` & `webui2-2.2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webui2
-Version: 2.2.0.1
+Version: 2.2.0.2
 Summary: Use any web browser as GUI
 Author: Hassan Draga
 Project-URL: Homepage, https://github.com/alifcommunity/webui
 Project-URL: Bug Tracker, https://github.com/alifcommunity/webui/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `webui2-2.2.0.1/README.md` & `webui2-2.2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `webui2-2.2.0.1/pyproject.toml` & `webui2-2.2.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "webui2"
-version = "2.2.0.1"
+version = "2.2.0.2"
 authors = [
   { name="Hassan Draga" },
 ]
 description = "Use any web browser as GUI"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `webui2-2.2.0.1/src/webui/webui-2-x64.dll` & `webui2-2.2.0.2/src/webui/webui-2-x64.dll`

 * *Files identical despite different names*

### Comparing `webui2-2.2.0.1/src/webui/webui-2-x64.dyn` & `webui2-2.2.0.2/src/webui/webui-2-x64.dyn`

 * *Files identical despite different names*

### Comparing `webui2-2.2.0.1/src/webui/webui-2-x64.so` & `webui2-2.2.0.2/src/webui/webui-2-x64.so`

 * *Files identical despite different names*

### Comparing `webui2-2.2.0.1/src/webui/webui.py` & `webui2-2.2.0.2/src/webui/webui.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,15 +248,15 @@
         webui_lib.webui_run(self.window, 
             ctypes.c_char_p(script.encode('utf-8')))
 
 
 def _get_library_path() -> str:
     global webui_path
     if platform.system() == 'Darwin':
-        file = '/webui-2-x64.dylib'
+        file = '/webui-2-x64.dyn'
         path = os.getcwd() + file
         if os.path.exists(path):
             return path
         path = webui_path + file
         if os.path.exists(path):
             return path
         return path
```

### Comparing `webui2-2.2.0.1/src/webui2.egg-info/PKG-INFO` & `webui2-2.2.0.2/src/webui2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webui2
-Version: 2.2.0.1
+Version: 2.2.0.2
 Summary: Use any web browser as GUI
 Author: Hassan Draga
 Project-URL: Homepage, https://github.com/alifcommunity/webui
 Project-URL: Bug Tracker, https://github.com/alifcommunity/webui/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

