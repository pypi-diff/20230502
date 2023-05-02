# Comparing `tmp/wbpFonttools-0.1.8.tar.gz` & `tmp/wbpFonttools-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbpFonttools-0.1.8.tar", last modified: Fri Apr 21 13:01:40 2023, max compression
+gzip compressed data, was "wbpFonttools-0.1.9.tar", last modified: Tue May  2 09:59:55 2023, max compression
```

## Comparing `wbpFonttools-0.1.8.tar` & `wbpFonttools-0.1.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 13:01:40.662122 wbpFonttools-0.1.8/
--rw-rw-rw-   0 root         (0) root         (0)     1080 2023-04-21 13:01:38.000000 wbpFonttools-0.1.8/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 13:01:40.655121 wbpFonttools-0.1.8/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 13:01:40.660122 wbpFonttools-0.1.8/Lib/wbpFonttools/
--rw-rw-rw-   0 root         (0) root         (0)     1684 2023-04-21 13:01:38.000000 wbpFonttools-0.1.8/Lib/wbpFonttools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4895 2023-04-21 13:01:38.000000 wbpFonttools-0.1.8/Lib/wbpFonttools/config.py
--rw-rw-rw-   0 root         (0) root         (0)     6779 2023-04-21 13:01:38.000000 wbpFonttools-0.1.8/Lib/wbpFonttools/control.py
--rw-rw-rw-   0 root         (0) root         (0)     1544 2023-04-21 13:01:38.000000 wbpFonttools-0.1.8/Lib/wbpFonttools/dialog.py
--rw-rw-rw-   0 root         (0) root         (0)     3581 2023-04-21 13:01:38.000000 wbpFonttools-0.1.8/Lib/wbpFonttools/document.py
--rw-rw-rw-   0 root         (0) root         (0)     1991 2023-04-21 13:01:38.000000 wbpFonttools-0.1.8/Lib/wbpFonttools/selectFontsDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     3277 2023-04-21 13:01:38.000000 wbpFonttools-0.1.8/Lib/wbpFonttools/template.py
--rw-rw-rw-   0 root         (0) root         (0)     2071 2023-04-21 13:01:38.000000 wbpFonttools-0.1.8/Lib/wbpFonttools/tools.py
--rw-rw-rw-   0 root         (0) root         (0)     2332 2023-04-21 13:01:38.000000 wbpFonttools-0.1.8/Lib/wbpFonttools/view.py
--rw-rw-rw-   0 root         (0) root         (0)    12103 2023-04-21 13:01:38.000000 wbpFonttools-0.1.8/Lib/wbpFonttools/window.py
--rw-rw-rw-   0 root         (0) root         (0)     4362 2023-04-21 13:01:38.000000 wbpFonttools-0.1.8/Lib/wbpFonttools/windowUI.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 13:01:40.662122 wbpFonttools-0.1.8/Lib/wbpFonttools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2323 2023-04-21 13:01:40.000000 wbpFonttools-0.1.8/Lib/wbpFonttools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      594 2023-04-21 13:01:40.000000 wbpFonttools-0.1.8/Lib/wbpFonttools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 13:01:40.000000 wbpFonttools-0.1.8/Lib/wbpFonttools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       41 2023-04-21 13:01:40.000000 wbpFonttools-0.1.8/Lib/wbpFonttools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       84 2023-04-21 13:01:40.000000 wbpFonttools-0.1.8/Lib/wbpFonttools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 13:01:40.000000 wbpFonttools-0.1.8/Lib/wbpFonttools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2323 2023-04-21 13:01:40.662122 wbpFonttools-0.1.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      761 2023-04-21 13:01:38.000000 wbpFonttools-0.1.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2251 2023-04-21 13:01:40.663122 wbpFonttools-0.1.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-04-21 13:01:38.000000 wbpFonttools-0.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:59:55.894666 wbpFonttools-0.1.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2023-05-02 09:59:53.000000 wbpFonttools-0.1.9/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:59:55.887666 wbpFonttools-0.1.9/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:59:55.892666 wbpFonttools-0.1.9/Lib/wbpFonttools/
+-rw-rw-rw-   0 root         (0) root         (0)     1658 2023-05-02 09:59:53.000000 wbpFonttools-0.1.9/Lib/wbpFonttools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4895 2023-05-02 09:59:53.000000 wbpFonttools-0.1.9/Lib/wbpFonttools/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     6779 2023-05-02 09:59:53.000000 wbpFonttools-0.1.9/Lib/wbpFonttools/control.py
+-rw-rw-rw-   0 root         (0) root         (0)     1544 2023-05-02 09:59:53.000000 wbpFonttools-0.1.9/Lib/wbpFonttools/dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     3581 2023-05-02 09:59:53.000000 wbpFonttools-0.1.9/Lib/wbpFonttools/document.py
+-rw-rw-rw-   0 root         (0) root         (0)     1991 2023-05-02 09:59:53.000000 wbpFonttools-0.1.9/Lib/wbpFonttools/selectFontsDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     3277 2023-05-02 09:59:53.000000 wbpFonttools-0.1.9/Lib/wbpFonttools/template.py
+-rw-rw-rw-   0 root         (0) root         (0)     2071 2023-05-02 09:59:53.000000 wbpFonttools-0.1.9/Lib/wbpFonttools/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     2332 2023-05-02 09:59:53.000000 wbpFonttools-0.1.9/Lib/wbpFonttools/view.py
+-rw-rw-rw-   0 root         (0) root         (0)    12103 2023-05-02 09:59:53.000000 wbpFonttools-0.1.9/Lib/wbpFonttools/window.py
+-rw-rw-rw-   0 root         (0) root         (0)     4362 2023-05-02 09:59:53.000000 wbpFonttools-0.1.9/Lib/wbpFonttools/windowUI.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:59:55.894666 wbpFonttools-0.1.9/Lib/wbpFonttools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2323 2023-05-02 09:59:55.000000 wbpFonttools-0.1.9/Lib/wbpFonttools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      594 2023-05-02 09:59:55.000000 wbpFonttools-0.1.9/Lib/wbpFonttools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 09:59:55.000000 wbpFonttools-0.1.9/Lib/wbpFonttools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-05-02 09:59:55.000000 wbpFonttools-0.1.9/Lib/wbpFonttools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2023-05-02 09:59:55.000000 wbpFonttools-0.1.9/Lib/wbpFonttools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-02 09:59:55.000000 wbpFonttools-0.1.9/Lib/wbpFonttools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2323 2023-05-02 09:59:55.894666 wbpFonttools-0.1.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      761 2023-05-02 09:59:53.000000 wbpFonttools-0.1.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2251 2023-05-02 09:59:55.895666 wbpFonttools-0.1.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-05-02 09:59:53.000000 wbpFonttools-0.1.9/setup.py
```

### Comparing `wbpFonttools-0.1.8/LICENSE` & `wbpFonttools-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.1.8/Lib/wbpFonttools/__init__.py` & `wbpFonttools-0.1.9/Lib/wbpFonttools/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,29 +2,27 @@
 
 from typing import TYPE_CHECKING, Iterable, List, Optional
 
 import wx
 
 from .config import FonttoolsPreferences, ObjectViewPreferences, XmlViewPreferences
 from .dialog import SelectFontsDialog
-from .document import FontToolsDocument
+from .document import FontToolsDocument, TTFont
 from .template import (
     OpenType_OTF_Template,
     OpenType_TTC_Template,
     OpenType_TTF_Template,
     WebFont_WOFF_2_Template,
     WebFont_WOFF_Template,
 )
 
 if TYPE_CHECKING:
     from wbBase.application import App
 
-    from .document import TTFont
-
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 
 
 def CurrentFont() -> Optional[TTFont]:
     """
     Get the currently active font
     """
     app: App = wx.GetApp()
```

### Comparing `wbpFonttools-0.1.8/Lib/wbpFonttools/config.py` & `wbpFonttools-0.1.9/Lib/wbpFonttools/config.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.1.8/Lib/wbpFonttools/control.py` & `wbpFonttools-0.1.9/Lib/wbpFonttools/control.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.1.8/Lib/wbpFonttools/dialog.py` & `wbpFonttools-0.1.9/Lib/wbpFonttools/dialog.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.1.8/Lib/wbpFonttools/document.py` & `wbpFonttools-0.1.9/Lib/wbpFonttools/document.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.1.8/Lib/wbpFonttools/selectFontsDialogUI.py` & `wbpFonttools-0.1.9/Lib/wbpFonttools/selectFontsDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.1.8/Lib/wbpFonttools/template.py` & `wbpFonttools-0.1.9/Lib/wbpFonttools/template.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.1.8/Lib/wbpFonttools/tools.py` & `wbpFonttools-0.1.9/Lib/wbpFonttools/tools.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.1.8/Lib/wbpFonttools/view.py` & `wbpFonttools-0.1.9/Lib/wbpFonttools/view.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.1.8/Lib/wbpFonttools/window.py` & `wbpFonttools-0.1.9/Lib/wbpFonttools/window.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.1.8/Lib/wbpFonttools/windowUI.py` & `wbpFonttools-0.1.9/Lib/wbpFonttools/windowUI.py`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.1.8/Lib/wbpFonttools.egg-info/PKG-INFO` & `wbpFonttools-0.1.9/Lib/wbpFonttools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbpFonttools
-Version: 0.1.8
+Version: 0.1.9
 Summary: FontTools font editor for Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbpfonttools
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbpfonttools
 Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbpfonttools
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbpfonttools/-/issues
```

### Comparing `wbpFonttools-0.1.8/Lib/wbpFonttools.egg-info/SOURCES.txt` & `wbpFonttools-0.1.9/Lib/wbpFonttools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.1.8/PKG-INFO` & `wbpFonttools-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbpFonttools
-Version: 0.1.8
+Version: 0.1.9
 Summary: FontTools font editor for Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbpfonttools
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbpfonttools
 Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbpfonttools
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbpfonttools/-/issues
```

### Comparing `wbpFonttools-0.1.8/README.md` & `wbpFonttools-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `wbpFonttools-0.1.8/setup.cfg` & `wbpFonttools-0.1.9/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.8
+current_version = 0.1.9
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
 
@@ -52,29 +52,29 @@
 
 [options]
 package_dir = 
 	=Lib
 packages = find:
 python_requires = >=3.8,<3.11
 install_requires = 
-	wbBase>=0.1.52
+	wbBase>=0.1.56
 	fonttools[ufo,lxml,woff,unicode,interpolatable,plot,symfont]>=4.39.3
 
 [options.packages.find]
 where = Lib
 
 [options.entry_points]
 wbbase.plugin = fonttools = wbpFonttools
 
 [bumpversion:file:Lib/wbpFonttools/__init__.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
 
 [tox:tox]
-min_version = 4.4
+min_version = 4.5
 env_list = 
 	py38
 	py39
 	py10
 
 [testenv]
 deps =
```

