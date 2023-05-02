# Comparing `tmp/wbpTextedit-0.1.5.tar.gz` & `tmp/wbpTextedit-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbpTextedit-0.1.5.tar", last modified: Sat Apr  8 09:36:45 2023, max compression
+gzip compressed data, was "wbpTextedit-0.1.6.tar", last modified: Tue May  2 10:27:52 2023, max compression
```

## Comparing `wbpTextedit-0.1.5.tar` & `wbpTextedit-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 09:36:45.587120 wbpTextedit-0.1.5/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-04-08 09:36:43.000000 wbpTextedit-0.1.5/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 09:36:45.581120 wbpTextedit-0.1.5/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 09:36:45.584120 wbpTextedit-0.1.5/Lib/wbpTextedit/
--rw-rw-rw-   0 root         (0) root         (0)      560 2023-04-08 09:36:43.000000 wbpTextedit-0.1.5/Lib/wbpTextedit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3641 2023-04-08 09:36:43.000000 wbpTextedit-0.1.5/Lib/wbpTextedit/config.py
--rw-rw-rw-   0 root         (0) root         (0)     7646 2023-04-08 09:36:43.000000 wbpTextedit-0.1.5/Lib/wbpTextedit/control.py
--rw-rw-rw-   0 root         (0) root         (0)      484 2023-04-08 09:36:43.000000 wbpTextedit-0.1.5/Lib/wbpTextedit/document.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 09:36:45.587120 wbpTextedit-0.1.5/Lib/wbpTextedit/template/
--rw-rw-rw-   0 root         (0) root         (0)     4999 2023-04-08 09:36:43.000000 wbpTextedit-0.1.5/Lib/wbpTextedit/template/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1590 2023-04-08 09:36:43.000000 wbpTextedit-0.1.5/Lib/wbpTextedit/template/ini.py
--rw-rw-rw-   0 root         (0) root         (0)     4858 2023-04-08 09:36:43.000000 wbpTextedit-0.1.5/Lib/wbpTextedit/template/python.py
--rw-rw-rw-   0 root         (0) root         (0)     1107 2023-04-08 09:36:43.000000 wbpTextedit-0.1.5/Lib/wbpTextedit/template/xml.py
--rw-rw-rw-   0 root         (0) root         (0)      783 2023-04-08 09:36:43.000000 wbpTextedit-0.1.5/Lib/wbpTextedit/view.py
--rw-rw-rw-   0 root         (0) root         (0)     1395 2023-04-08 09:36:43.000000 wbpTextedit-0.1.5/Lib/wbpTextedit/window.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 09:36:45.586120 wbpTextedit-0.1.5/Lib/wbpTextedit.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1838 2023-04-08 09:36:45.000000 wbpTextedit-0.1.5/Lib/wbpTextedit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      567 2023-04-08 09:36:45.000000 wbpTextedit-0.1.5/Lib/wbpTextedit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-08 09:36:45.000000 wbpTextedit-0.1.5/Lib/wbpTextedit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-04-08 09:36:45.000000 wbpTextedit-0.1.5/Lib/wbpTextedit.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-08 09:36:45.000000 wbpTextedit-0.1.5/Lib/wbpTextedit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-08 09:36:45.000000 wbpTextedit-0.1.5/Lib/wbpTextedit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1838 2023-04-08 09:36:45.587120 wbpTextedit-0.1.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      458 2023-04-08 09:36:43.000000 wbpTextedit-0.1.5/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2027 2023-04-08 09:36:45.588121 wbpTextedit-0.1.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-04-08 09:36:43.000000 wbpTextedit-0.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:27:52.316700 wbpTextedit-0.1.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-05-02 10:27:50.000000 wbpTextedit-0.1.6/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:27:52.309700 wbpTextedit-0.1.6/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:27:52.313700 wbpTextedit-0.1.6/Lib/wbpTextedit/
+-rw-rw-rw-   0 root         (0) root         (0)      560 2023-05-02 10:27:50.000000 wbpTextedit-0.1.6/Lib/wbpTextedit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3641 2023-05-02 10:27:50.000000 wbpTextedit-0.1.6/Lib/wbpTextedit/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     7646 2023-05-02 10:27:50.000000 wbpTextedit-0.1.6/Lib/wbpTextedit/control.py
+-rw-rw-rw-   0 root         (0) root         (0)      484 2023-05-02 10:27:50.000000 wbpTextedit-0.1.6/Lib/wbpTextedit/document.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:27:52.316700 wbpTextedit-0.1.6/Lib/wbpTextedit/template/
+-rw-rw-rw-   0 root         (0) root         (0)     4999 2023-05-02 10:27:50.000000 wbpTextedit-0.1.6/Lib/wbpTextedit/template/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1590 2023-05-02 10:27:50.000000 wbpTextedit-0.1.6/Lib/wbpTextedit/template/ini.py
+-rw-rw-rw-   0 root         (0) root         (0)     4858 2023-05-02 10:27:50.000000 wbpTextedit-0.1.6/Lib/wbpTextedit/template/python.py
+-rw-rw-rw-   0 root         (0) root         (0)     1107 2023-05-02 10:27:50.000000 wbpTextedit-0.1.6/Lib/wbpTextedit/template/xml.py
+-rw-rw-rw-   0 root         (0) root         (0)      783 2023-05-02 10:27:50.000000 wbpTextedit-0.1.6/Lib/wbpTextedit/view.py
+-rw-rw-rw-   0 root         (0) root         (0)     1395 2023-05-02 10:27:50.000000 wbpTextedit-0.1.6/Lib/wbpTextedit/window.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:27:52.315700 wbpTextedit-0.1.6/Lib/wbpTextedit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2082 2023-05-02 10:27:52.000000 wbpTextedit-0.1.6/Lib/wbpTextedit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      567 2023-05-02 10:27:52.000000 wbpTextedit-0.1.6/Lib/wbpTextedit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 10:27:52.000000 wbpTextedit-0.1.6/Lib/wbpTextedit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-05-02 10:27:52.000000 wbpTextedit-0.1.6/Lib/wbpTextedit.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-02 10:27:52.000000 wbpTextedit-0.1.6/Lib/wbpTextedit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-02 10:27:52.000000 wbpTextedit-0.1.6/Lib/wbpTextedit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2082 2023-05-02 10:27:52.316700 wbpTextedit-0.1.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      703 2023-05-02 10:27:50.000000 wbpTextedit-0.1.6/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2026 2023-05-02 10:27:52.317700 wbpTextedit-0.1.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-02 10:27:50.000000 wbpTextedit-0.1.6/setup.py
```

### Comparing `wbpTextedit-0.1.5/LICENSE` & `wbpTextedit-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wbpTextedit-0.1.5/Lib/wbpTextedit/__init__.py` & `wbpTextedit-0.1.6/Lib/wbpTextedit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from .template import PlainTextTemplate
 from .config import TextEditPreferences, PlainTextPreferences
 from .template.python import PythonTextTemplate, PythonTextPreferences
 from .template.xml import XMLTextTemplate, XMLTextPreferences
 from .template.ini import IniTextTemplate, IniTextPreferences
 
 
-__version__ = "0.1.5"
+__version__ = "0.1.6"
 
 doctemplates = (PlainTextTemplate, PythonTextTemplate, XMLTextTemplate, IniTextTemplate)
 
 preferencepages = (
     TextEditPreferences,
     PlainTextPreferences,
     PythonTextPreferences,
```

### Comparing `wbpTextedit-0.1.5/Lib/wbpTextedit/config.py` & `wbpTextedit-0.1.6/Lib/wbpTextedit/config.py`

 * *Files identical despite different names*

### Comparing `wbpTextedit-0.1.5/Lib/wbpTextedit/control.py` & `wbpTextedit-0.1.6/Lib/wbpTextedit/control.py`

 * *Files identical despite different names*

### Comparing `wbpTextedit-0.1.5/Lib/wbpTextedit/template/__init__.py` & `wbpTextedit-0.1.6/Lib/wbpTextedit/template/__init__.py`

 * *Files identical despite different names*

### Comparing `wbpTextedit-0.1.5/Lib/wbpTextedit/template/ini.py` & `wbpTextedit-0.1.6/Lib/wbpTextedit/template/ini.py`

 * *Files identical despite different names*

### Comparing `wbpTextedit-0.1.5/Lib/wbpTextedit/template/python.py` & `wbpTextedit-0.1.6/Lib/wbpTextedit/template/python.py`

 * *Files identical despite different names*

### Comparing `wbpTextedit-0.1.5/Lib/wbpTextedit/template/xml.py` & `wbpTextedit-0.1.6/Lib/wbpTextedit/template/xml.py`

 * *Files identical despite different names*

### Comparing `wbpTextedit-0.1.5/Lib/wbpTextedit/view.py` & `wbpTextedit-0.1.6/Lib/wbpTextedit/view.py`

 * *Files identical despite different names*

### Comparing `wbpTextedit-0.1.5/Lib/wbpTextedit/window.py` & `wbpTextedit-0.1.6/Lib/wbpTextedit/window.py`

 * *Files identical despite different names*

### Comparing `wbpTextedit-0.1.5/Lib/wbpTextedit.egg-info/PKG-INFO` & `wbpTextedit-0.1.6/Lib/wbpTextedit.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: wbpTextedit
-Version: 0.1.5
+Version: 0.1.6
 Summary: Text editor for Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbptextedit
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbptextedit
-Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbptextedit/
+Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbptextedit
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbptextedit/-/issues
 Keywords: workbench,wxPython,GUI
 Platform: WIN32
 Platform: WIN64
 Platform: OSX
 Platform: POSIX
 Classifier: Development Status :: 3 - Alpha
@@ -32,23 +32,34 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # wbpTextedit
 
 Text editor plugin for Workbench applications.
 
+This plugin provides document templates to create, view and edit 
+the following file types:
+
+- Plain text (*.txt)
+- Python scripts (*.py, *.pyw)
+- ini-style configuration files (*.ini, *.cfg)
+- XML text files (*.xml, *.xsd)
+
 ## Installation
 
 ```shell
 pip install wbpTextedit
 ```
 
-This plugin provides document templates to create, view and edit the following file types:
-
-- Plain text (*.txt)
-- Python scripts (*.py, *.pyw)
-- ini-style configuration files (*.ini, *.cfg)
-- XML text files (*.xml, *.xsd)
+Installing this plugin registers an entry point 
+in the group "*wbbase.plugin*" named "*textedit*".
 
+To use the plugin in your application, 
+add it to your *application.yaml* file as follows:
+```yaml
+AppName: myApp
+Plugins:
+- Name: textedit
+```
 ## Documentation
 
-For details read the [Documentation](https://workbench2.gitlab.io/workbench-plugins/wbpTextedit/).
+For details read the [Documentation](https://workbench2.gitlab.io/workbench-plugins/wbptextedit).
```

### Comparing `wbpTextedit-0.1.5/Lib/wbpTextedit.egg-info/SOURCES.txt` & `wbpTextedit-0.1.6/Lib/wbpTextedit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wbpTextedit-0.1.5/PKG-INFO` & `wbpTextedit-0.1.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: wbpTextedit
-Version: 0.1.5
+Version: 0.1.6
 Summary: Text editor for Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbptextedit
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbptextedit
-Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbptextedit/
+Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbptextedit
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbptextedit/-/issues
 Keywords: workbench,wxPython,GUI
 Platform: WIN32
 Platform: WIN64
 Platform: OSX
 Platform: POSIX
 Classifier: Development Status :: 3 - Alpha
@@ -32,23 +32,34 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # wbpTextedit
 
 Text editor plugin for Workbench applications.
 
+This plugin provides document templates to create, view and edit 
+the following file types:
+
+- Plain text (*.txt)
+- Python scripts (*.py, *.pyw)
+- ini-style configuration files (*.ini, *.cfg)
+- XML text files (*.xml, *.xsd)
+
 ## Installation
 
 ```shell
 pip install wbpTextedit
 ```
 
-This plugin provides document templates to create, view and edit the following file types:
-
-- Plain text (*.txt)
-- Python scripts (*.py, *.pyw)
-- ini-style configuration files (*.ini, *.cfg)
-- XML text files (*.xml, *.xsd)
+Installing this plugin registers an entry point 
+in the group "*wbbase.plugin*" named "*textedit*".
 
+To use the plugin in your application, 
+add it to your *application.yaml* file as follows:
+```yaml
+AppName: myApp
+Plugins:
+- Name: textedit
+```
 ## Documentation
 
-For details read the [Documentation](https://workbench2.gitlab.io/workbench-plugins/wbpTextedit/).
+For details read the [Documentation](https://workbench2.gitlab.io/workbench-plugins/wbptextedit).
```

### Comparing `wbpTextedit-0.1.5/setup.cfg` & `wbpTextedit-0.1.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.5
+current_version = 0.1.6
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
 
@@ -19,15 +19,15 @@
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 license_files = LICENSE
 url = https://gitlab.com/workbench2/workbench-plugins/wbptextedit
 project_urls = 
 	Source = https://gitlab.com/workbench2/workbench-plugins/wbptextedit
-	Documentation = https://workbench2.gitlab.io/workbench-plugins/wbptextedit/
+	Documentation = https://workbench2.gitlab.io/workbench-plugins/wbptextedit
 	Tracker = https://gitlab.com/workbench2/workbench-plugins/wbptextedit/-/issues
 platforms = 
 	WIN32
 	WIN64
 	OSX
 	POSIX
 keywords =
```

