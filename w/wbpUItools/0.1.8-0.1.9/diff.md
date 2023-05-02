# Comparing `tmp/wbpUItools-0.1.8.tar.gz` & `tmp/wbpUItools-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbpUItools-0.1.8.tar", last modified: Sun Apr  9 14:50:10 2023, max compression
+gzip compressed data, was "wbpUItools-0.1.9.tar", last modified: Tue May  2 10:33:21 2023, max compression
```

## Comparing `wbpUItools-0.1.8.tar` & `wbpUItools-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 14:50:10.237079 wbpUItools-0.1.8/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-04-09 14:50:08.000000 wbpUItools-0.1.8/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 14:50:10.229079 wbpUItools-0.1.8/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 14:50:10.231079 wbpUItools-0.1.8/Lib/wbpUItools/
--rw-rw-rw-   0 root         (0) root         (0)     4947 2023-04-09 14:50:08.000000 wbpUItools-0.1.8/Lib/wbpUItools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 14:50:10.234079 wbpUItools-0.1.8/Lib/wbpUItools/control/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-09 14:50:08.000000 wbpUItools-0.1.8/Lib/wbpUItools/control/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4166 2023-04-09 14:50:08.000000 wbpUItools-0.1.8/Lib/wbpUItools/control/panelItemPicker.py
--rw-rw-rw-   0 root         (0) root         (0)     5762 2023-04-09 14:50:08.000000 wbpUItools-0.1.8/Lib/wbpUItools/control/panelItemPickerUI.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 14:50:10.236079 wbpUItools-0.1.8/Lib/wbpUItools/dialog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-09 14:50:08.000000 wbpUItools-0.1.8/Lib/wbpUItools/dialog/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1832 2023-04-09 14:50:08.000000 wbpUItools-0.1.8/Lib/wbpUItools/dialog/checkListDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     2479 2023-04-09 14:50:08.000000 wbpUItools-0.1.8/Lib/wbpUItools/dialog/dialogItemPicker.py
--rw-rw-rw-   0 root         (0) root         (0)     1727 2023-04-09 14:50:08.000000 wbpUItools-0.1.8/Lib/wbpUItools/dialog/dialogItemPickerUI.py
--rw-rw-rw-   0 root         (0) root         (0)     1568 2023-04-09 14:50:08.000000 wbpUItools-0.1.8/Lib/wbpUItools/dialog/dialogTwoStrings.py
--rw-rw-rw-   0 root         (0) root         (0)     2725 2023-04-09 14:50:08.000000 wbpUItools-0.1.8/Lib/wbpUItools/dialog/dialogTwoStringsUI.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 14:50:10.233079 wbpUItools-0.1.8/Lib/wbpUItools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1931 2023-04-09 14:50:10.000000 wbpUItools-0.1.8/Lib/wbpUItools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      663 2023-04-09 14:50:10.000000 wbpUItools-0.1.8/Lib/wbpUItools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 14:50:10.000000 wbpUItools-0.1.8/Lib/wbpUItools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-04-09 14:50:10.000000 wbpUItools-0.1.8/Lib/wbpUItools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-09 14:50:10.000000 wbpUItools-0.1.8/Lib/wbpUItools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-09 14:50:10.000000 wbpUItools-0.1.8/Lib/wbpUItools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1931 2023-04-09 14:50:10.237079 wbpUItools-0.1.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-04-09 14:50:08.000000 wbpUItools-0.1.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2019 2023-04-09 14:50:10.238079 wbpUItools-0.1.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-04-09 14:50:08.000000 wbpUItools-0.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:33:21.698206 wbpUItools-0.1.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-05-02 10:33:19.000000 wbpUItools-0.1.9/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:33:21.689955 wbpUItools-0.1.9/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:33:21.693622 wbpUItools-0.1.9/Lib/wbpUItools/
+-rw-rw-rw-   0 root         (0) root         (0)     4917 2023-05-02 10:33:19.000000 wbpUItools-0.1.9/Lib/wbpUItools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:33:21.696372 wbpUItools-0.1.9/Lib/wbpUItools/control/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 10:33:19.000000 wbpUItools-0.1.9/Lib/wbpUItools/control/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3383 2023-05-02 10:33:19.000000 wbpUItools-0.1.9/Lib/wbpUItools/control/checkAllListBox.py
+-rw-rw-rw-   0 root         (0) root         (0)     4166 2023-05-02 10:33:19.000000 wbpUItools-0.1.9/Lib/wbpUItools/control/panelItemPicker.py
+-rw-rw-rw-   0 root         (0) root         (0)     5762 2023-05-02 10:33:19.000000 wbpUItools-0.1.9/Lib/wbpUItools/control/panelItemPickerUI.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:33:21.698206 wbpUItools-0.1.9/Lib/wbpUItools/dialog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 10:33:19.000000 wbpUItools-0.1.9/Lib/wbpUItools/dialog/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1815 2023-05-02 10:33:19.000000 wbpUItools-0.1.9/Lib/wbpUItools/dialog/checkListDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     2479 2023-05-02 10:33:19.000000 wbpUItools-0.1.9/Lib/wbpUItools/dialog/dialogItemPicker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1727 2023-05-02 10:33:19.000000 wbpUItools-0.1.9/Lib/wbpUItools/dialog/dialogItemPickerUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     1568 2023-05-02 10:33:19.000000 wbpUItools-0.1.9/Lib/wbpUItools/dialog/dialogTwoStrings.py
+-rw-rw-rw-   0 root         (0) root         (0)     2725 2023-05-02 10:33:19.000000 wbpUItools-0.1.9/Lib/wbpUItools/dialog/dialogTwoStringsUI.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:33:21.695455 wbpUItools-0.1.9/Lib/wbpUItools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2039 2023-05-02 10:33:21.000000 wbpUItools-0.1.9/Lib/wbpUItools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      705 2023-05-02 10:33:21.000000 wbpUItools-0.1.9/Lib/wbpUItools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 10:33:21.000000 wbpUItools-0.1.9/Lib/wbpUItools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-05-02 10:33:21.000000 wbpUItools-0.1.9/Lib/wbpUItools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-02 10:33:21.000000 wbpUItools-0.1.9/Lib/wbpUItools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-02 10:33:21.000000 wbpUItools-0.1.9/Lib/wbpUItools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2039 2023-05-02 10:33:21.698206 wbpUItools-0.1.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      590 2023-05-02 10:33:19.000000 wbpUItools-0.1.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2080 2023-05-02 10:33:21.699123 wbpUItools-0.1.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-05-02 10:33:19.000000 wbpUItools-0.1.9/setup.py
```

### Comparing `wbpUItools-0.1.8/LICENSE` & `wbpUItools-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wbpUItools-0.1.8/Lib/wbpUItools/__init__.py` & `wbpUItools-0.1.9/Lib/wbpUItools/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
 import os
 from typing import Optional, TYPE_CHECKING, Iterable, List, Union
 
 import wx
 
-# from .dialog.checkListDialogUI import CheckListDialogUI
+from .dialog.checkListDialogUI import CheckListDialogUI
 from .dialog.dialogItemPicker import DialogItemPicker
 
 if TYPE_CHECKING:
     from wbBase.application import App
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 
 
 def AskString(message: str, value: str = "", title: str = "") -> Optional[str]:
     app: App = wx.GetApp()
     return wx.GetTextFromUser(
         message,
         caption=title or app.AppDisplayName,
@@ -94,29 +94,29 @@
         default_extension="",
         wildcard="Any files (*.*)|*.*",
         flags=wx.FD_SAVE | wx.FD_OVERWRITE_PROMPT,
         parent=wx.GetApp().TopWindow,
     )
 
 
-# class CheckListDialog(CheckListDialogUI):
-#     def __init__(self, message, title="Workbench", choices=None, checked=None):
-#         super().__init__(wx.GetApp().TopWindow)
-#         self.Title = title
-#         self.message.Label = message
-#         if isinstance(choices, Iterable):
-#             self.checkList.SetItems([c for c in choices])
-#             if isinstance(checked, Iterable):
-#                 self.checkList.SetCheckedStrings([i for i in checked if i in choices])
+class CheckListDialog(CheckListDialogUI):
+    def __init__(self, message, title="Workbench", choices=None, checked=None):
+        super().__init__(wx.GetApp().TopWindow)
+        self.Title = title
+        self.message.Label = message
+        if isinstance(choices, Iterable):
+            self.checkList.SetItems([c for c in choices])
+            if isinstance(checked, Iterable):
+                self.checkList.SetCheckedStrings([i for i in checked if i in choices])
 
 
-# def getCheckList(message, title="Workbench", choices=None, checked=None):
-#     with CheckListDialog(message, title, choices, checked) as dialog:
-#         if dialog.ShowModal() == wx.ID_OK:
-#             return dialog.checkList.GetCheckedStrings()
+def getCheckList(message, title="Workbench", choices=None, checked=None):
+    with CheckListDialog(message, title, choices, checked) as dialog:
+        if dialog.ShowModal() == wx.ID_OK:
+            return dialog.checkList.GetCheckedStrings()
 
 
 def pickItems(
     message: str = "Select options",
     title: str = "",
     options: Optional[Iterable[str]] = None,
     selection: Optional[Iterable[str]] = None,
@@ -157,9 +157,9 @@
 
 globalObjects = [
     "AskString",
     "AskYesNoCancel",
     "Message",
     "GetFile",
     "PutFile",
-    # "getCheckList",
+    "getCheckList",
 ]
```

### Comparing `wbpUItools-0.1.8/Lib/wbpUItools/control/panelItemPicker.py` & `wbpUItools-0.1.9/Lib/wbpUItools/control/panelItemPicker.py`

 * *Files identical despite different names*

### Comparing `wbpUItools-0.1.8/Lib/wbpUItools/control/panelItemPickerUI.py` & `wbpUItools-0.1.9/Lib/wbpUItools/control/panelItemPickerUI.py`

 * *Files identical despite different names*

### Comparing `wbpUItools-0.1.8/Lib/wbpUItools/dialog/checkListDialogUI.py` & `wbpUItools-0.1.9/Lib/wbpUItools/dialog/checkListDialogUI.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ###########################################################################
 ## Python code generated with wxFormBuilder (version 3.10.1-0-g8feb16b3)
 ## http://www.wxformbuilder.org/
 ##
 ## PLEASE DO *NOT* EDIT THIS FILE!
 ###########################################################################
 
-from alphaWXtools.control.alphaCheckListBox import AlphaCheckListBox
+from ..control.checkAllListBox import CheckAllListBox
 import wx
 import wx.xrc
 
 ###########################################################################
 ## Class CheckListDialogUI
 ###########################################################################
 
@@ -26,15 +26,15 @@
 
         self.message = wx.StaticText( self, wx.ID_ANY, u"Message", wx.DefaultPosition, wx.DefaultSize, 0 )
         self.message.Wrap( -1 )
 
         sizer.Add( self.message, 0, wx.ALL|wx.EXPAND, 5 )
 
         checkListChoices = []
-        self.checkList = AlphaCheckListBox( self, wx.ID_ANY, wx.DefaultPosition, wx.DefaultSize, checkListChoices, wx.LB_NEEDED_SB )
+        self.checkList = CheckAllListBox( self, wx.ID_ANY, wx.DefaultPosition, wx.DefaultSize, checkListChoices, wx.LB_NEEDED_SB )
         sizer.Add( self.checkList, 1, wx.ALL|wx.EXPAND, 5 )
 
         buttons = wx.StdDialogButtonSizer()
         self.buttonsOK = wx.Button( self, wx.ID_OK )
         buttons.AddButton( self.buttonsOK )
         self.buttonsCancel = wx.Button( self, wx.ID_CANCEL )
         buttons.AddButton( self.buttonsCancel )
```

### Comparing `wbpUItools-0.1.8/Lib/wbpUItools/dialog/dialogItemPicker.py` & `wbpUItools-0.1.9/Lib/wbpUItools/dialog/dialogItemPicker.py`

 * *Files identical despite different names*

### Comparing `wbpUItools-0.1.8/Lib/wbpUItools/dialog/dialogItemPickerUI.py` & `wbpUItools-0.1.9/Lib/wbpUItools/dialog/dialogItemPickerUI.py`

 * *Files identical despite different names*

### Comparing `wbpUItools-0.1.8/Lib/wbpUItools/dialog/dialogTwoStrings.py` & `wbpUItools-0.1.9/Lib/wbpUItools/dialog/dialogTwoStrings.py`

 * *Files identical despite different names*

### Comparing `wbpUItools-0.1.8/Lib/wbpUItools/dialog/dialogTwoStringsUI.py` & `wbpUItools-0.1.9/Lib/wbpUItools/dialog/dialogTwoStringsUI.py`

 * *Files identical despite different names*

### Comparing `wbpUItools-0.1.8/Lib/wbpUItools.egg-info/PKG-INFO` & `wbpUItools-0.1.9/Lib/wbpUItools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbpUItools
-Version: 0.1.8
+Version: 0.1.9
 Summary: UI tools for Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbpUItools
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbpUItools
 Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbpUItools
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbpUItools/-/issues
@@ -21,40 +21,42 @@
 Classifier: Environment :: MacOS X :: Cocoa
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications :: GTK
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # wbpUItools
 
-UI tools plugin for Workbench applications.
+UI tools plugin for [Workbench](https://pypi.org/project/wbBase/) applications.
 
 This plugin provides some useful functions for user interaction
 in Python scripts.
 
 ## Installation
 
 ```shell
 pip install wbpUItools
 ```
 
 Installing this plugin registers an entry point 
 in the group "*wbbase.plugin*" named "*uitools*".
 
 To use the plugin in your application, 
-add it to your *application.yaml* file as follows:
+add it to your *application.yml* file as follows:
 ```yaml
 AppName: myApp
 Plugins:
 - Name: uitools
 ```
+
 ## Documentation
 
 For details read the [Documentation](https://workbench2.gitlab.io/workbench-plugins/wbpUItools).
```

### Comparing `wbpUItools-0.1.8/Lib/wbpUItools.egg-info/SOURCES.txt` & `wbpUItools-0.1.9/Lib/wbpUItools.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 Lib/wbpUItools.egg-info/PKG-INFO
 Lib/wbpUItools.egg-info/SOURCES.txt
 Lib/wbpUItools.egg-info/dependency_links.txt
 Lib/wbpUItools.egg-info/entry_points.txt
 Lib/wbpUItools.egg-info/requires.txt
 Lib/wbpUItools.egg-info/top_level.txt
 Lib/wbpUItools/control/__init__.py
+Lib/wbpUItools/control/checkAllListBox.py
 Lib/wbpUItools/control/panelItemPicker.py
 Lib/wbpUItools/control/panelItemPickerUI.py
 Lib/wbpUItools/dialog/__init__.py
 Lib/wbpUItools/dialog/checkListDialogUI.py
 Lib/wbpUItools/dialog/dialogItemPicker.py
 Lib/wbpUItools/dialog/dialogItemPickerUI.py
 Lib/wbpUItools/dialog/dialogTwoStrings.py
```

### Comparing `wbpUItools-0.1.8/PKG-INFO` & `wbpUItools-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbpUItools
-Version: 0.1.8
+Version: 0.1.9
 Summary: UI tools for Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbpUItools
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbpUItools
 Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbpUItools
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbpUItools/-/issues
@@ -21,40 +21,42 @@
 Classifier: Environment :: MacOS X :: Cocoa
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications :: GTK
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # wbpUItools
 
-UI tools plugin for Workbench applications.
+UI tools plugin for [Workbench](https://pypi.org/project/wbBase/) applications.
 
 This plugin provides some useful functions for user interaction
 in Python scripts.
 
 ## Installation
 
 ```shell
 pip install wbpUItools
 ```
 
 Installing this plugin registers an entry point 
 in the group "*wbbase.plugin*" named "*uitools*".
 
 To use the plugin in your application, 
-add it to your *application.yaml* file as follows:
+add it to your *application.yml* file as follows:
 ```yaml
 AppName: myApp
 Plugins:
 - Name: uitools
 ```
+
 ## Documentation
 
 For details read the [Documentation](https://workbench2.gitlab.io/workbench-plugins/wbpUItools).
```

### Comparing `wbpUItools-0.1.8/setup.cfg` & `wbpUItools-0.1.9/setup.cfg`

 * *Files 4% similar despite different names*

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
 
@@ -43,34 +43,35 @@
 	Environment :: MacOS X :: Cocoa
 	Environment :: Win32 (MS Windows)
 	Environment :: X11 Applications :: GTK
 	Programming Language :: Python :: 3
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
 python_requires = >=3.8,<3.11
 install_requires = 
-	wbBase>=0.1.52
+	wbBase>=0.1.56
 
 [options.packages.find]
 where = Lib
 
 [options.entry_points]
 wbbase.plugin = uitools = wbpUItools
 
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

