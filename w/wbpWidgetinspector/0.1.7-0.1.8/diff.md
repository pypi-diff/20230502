# Comparing `tmp/wbpWidgetinspector-0.1.7.tar.gz` & `tmp/wbpWidgetinspector-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbpWidgetinspector-0.1.7.tar", last modified: Wed Feb  8 16:17:36 2023, max compression
+gzip compressed data, was "wbpWidgetinspector-0.1.8.tar", last modified: Tue May  2 11:11:49 2023, max compression
```

## Comparing `wbpWidgetinspector-0.1.7.tar` & `wbpWidgetinspector-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 16:17:36.113218 wbpWidgetinspector-0.1.7/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-02-08 16:17:34.000000 wbpWidgetinspector-0.1.7/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 16:17:36.109218 wbpWidgetinspector-0.1.7/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 16:17:36.111218 wbpWidgetinspector-0.1.7/Lib/wbpWidgetinspector/
--rw-rw-rw-   0 root         (0) root         (0)     1721 2023-02-08 16:17:34.000000 wbpWidgetinspector-0.1.7/Lib/wbpWidgetinspector/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 16:17:36.113218 wbpWidgetinspector-0.1.7/Lib/wbpWidgetinspector.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1831 2023-02-08 16:17:36.000000 wbpWidgetinspector-0.1.7/Lib/wbpWidgetinspector.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      349 2023-02-08 16:17:36.000000 wbpWidgetinspector-0.1.7/Lib/wbpWidgetinspector.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-08 16:17:36.000000 wbpWidgetinspector-0.1.7/Lib/wbpWidgetinspector.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-02-08 16:17:36.000000 wbpWidgetinspector-0.1.7/Lib/wbpWidgetinspector.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-02-08 16:17:36.000000 wbpWidgetinspector-0.1.7/Lib/wbpWidgetinspector.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-02-08 16:17:36.000000 wbpWidgetinspector-0.1.7/Lib/wbpWidgetinspector.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1831 2023-02-08 16:17:36.113218 wbpWidgetinspector-0.1.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-02-08 16:17:34.000000 wbpWidgetinspector-0.1.7/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2155 2023-02-08 16:17:36.114219 wbpWidgetinspector-0.1.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-02-08 16:17:34.000000 wbpWidgetinspector-0.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:11:49.050387 wbpWidgetinspector-0.1.8/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-05-02 11:11:47.000000 wbpWidgetinspector-0.1.8/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:11:49.046387 wbpWidgetinspector-0.1.8/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:11:49.048387 wbpWidgetinspector-0.1.8/Lib/wbpWidgetinspector/
+-rw-rw-rw-   0 root         (0) root         (0)     1717 2023-05-02 11:11:47.000000 wbpWidgetinspector-0.1.8/Lib/wbpWidgetinspector/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 11:11:49.050387 wbpWidgetinspector-0.1.8/Lib/wbpWidgetinspector.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1853 2023-05-02 11:11:49.000000 wbpWidgetinspector-0.1.8/Lib/wbpWidgetinspector.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      349 2023-05-02 11:11:49.000000 wbpWidgetinspector-0.1.8/Lib/wbpWidgetinspector.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 11:11:49.000000 wbpWidgetinspector-0.1.8/Lib/wbpWidgetinspector.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-05-02 11:11:49.000000 wbpWidgetinspector-0.1.8/Lib/wbpWidgetinspector.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-02 11:11:49.000000 wbpWidgetinspector-0.1.8/Lib/wbpWidgetinspector.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-02 11:11:49.000000 wbpWidgetinspector-0.1.8/Lib/wbpWidgetinspector.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1853 2023-05-02 11:11:49.050387 wbpWidgetinspector-0.1.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      354 2023-05-02 11:11:47.000000 wbpWidgetinspector-0.1.8/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2171 2023-05-02 11:11:49.051387 wbpWidgetinspector-0.1.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-05-02 11:11:47.000000 wbpWidgetinspector-0.1.8/setup.py
```

### Comparing `wbpWidgetinspector-0.1.7/LICENSE` & `wbpWidgetinspector-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `wbpWidgetinspector-0.1.7/Lib/wbpWidgetinspector/__init__.py` & `wbpWidgetinspector-0.1.8/Lib/wbpWidgetinspector/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import wx
 from wx.lib.inspection import InspectionTool
 
 if TYPE_CHECKING:
     from wbBase.application import App
 
-__version__ = "0.1.7"
+__version__ = "0.1.8"
 
 
 class WidgetInspector:
     def __init__(self, alt=True, cmd=True, shift=False, keyCode=ord("I")):
         self._alt = alt
         self._cmd = cmd
         self._shift = shift
@@ -49,10 +49,10 @@
         setting it to display the widget under the cursor.
         """
         # get the current widget under the mouse
         wnd, __ = wx.FindWindowAtPointer()
         InspectionTool().Show(wnd)
 
 
-# widgetInspector = WidgetInspector()
-# wx.GetApp().AddPostInitAction(widgetInspector.initInspection)
+widgetInspector = WidgetInspector()
+wx.GetApp().AddPostInitAction(widgetInspector.initInspection)
```

### Comparing `wbpWidgetinspector-0.1.7/Lib/wbpWidgetinspector.egg-info/PKG-INFO` & `wbpWidgetinspector-0.1.8/Lib/wbpWidgetinspector.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbpWidgetinspector
-Version: 0.1.7
+Version: 0.1.8
 Summary: Itegrate Widgetinspector in Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbpwidgetinspector
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbpwidgetinspector
 Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbpwidgetinspector/
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbpwidgetinspector/-/issues
@@ -18,22 +18,22 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Environment :: MacOS X :: Cocoa
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications :: GTK
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: User Interfaces
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # wbpWidgetinspector
 
 Widgetinspector plugin for Workbench applications. This plugin allows you to 
 launch the wx Widgetinspector from within your running application.
```

### Comparing `wbpWidgetinspector-0.1.7/PKG-INFO` & `wbpWidgetinspector-0.1.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbpWidgetinspector
-Version: 0.1.7
+Version: 0.1.8
 Summary: Itegrate Widgetinspector in Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbpwidgetinspector
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbpwidgetinspector
 Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbpwidgetinspector/
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbpwidgetinspector/-/issues
@@ -18,22 +18,22 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Environment :: MacOS X :: Cocoa
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications :: GTK
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: User Interfaces
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # wbpWidgetinspector
 
 Widgetinspector plugin for Workbench applications. This plugin allows you to 
 launch the wx Widgetinspector from within your running application.
```

### Comparing `wbpWidgetinspector-0.1.7/setup.cfg` & `wbpWidgetinspector-0.1.8/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.7
+current_version = 0.1.8
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
 
@@ -36,44 +36,43 @@
 	Operating System :: MacOS
 	Operating System :: Microsoft :: Windows
 	Operating System :: POSIX
 	Environment :: MacOS X :: Cocoa
 	Environment :: Win32 (MS Windows)
 	Environment :: X11 Applications :: GTK
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: Implementation :: CPython
 	Intended Audience :: Developers
 	Topic :: Software Development :: Libraries
 	Topic :: Software Development :: User Interfaces
 
 [options]
 package_dir = 
 	=Lib
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
-	wbBase>=0.1.46
+	wbBase>=0.1.56
 
 [options.packages.find]
 where = Lib
 
 [options.entry_points]
 wbbase.plugin = widgetinspector = wbpWidgetinspector
 
 [bumpversion:file:Lib/wbpWidgetinspector/__init__.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
 
 [tox:tox]
-min_version = 4.3
+min_version = 4.5
 env_list = 
-	py37
 	py38
 	py39
 	py310
 
 [testenv]
 deps = 
 	pytest
```

