# Comparing `tmp/wbBase-0.1.55.tar.gz` & `tmp/wbBase-0.1.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbBase-0.1.55.tar", last modified: Sun Apr 30 08:43:35 2023, max compression
+gzip compressed data, was "wbBase-0.1.56.tar", last modified: Tue May  2 09:43:09 2023, max compression
```

## Comparing `wbBase-0.1.55.tar` & `wbBase-0.1.56.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 08:43:35.465984 wbBase-0.1.55/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-04-30 08:43:33.000000 wbBase-0.1.55/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 08:43:35.452983 wbBase-0.1.55/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 08:43:35.458984 wbBase-0.1.55/Lib/wbBase/
--rw-rw-rw-   0 root         (0) root         (0)      153 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23475 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/application.py
--rw-rw-rw-   0 root         (0) root         (0)     2165 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/applicationInfo.py
--rw-rw-rw-   0 root         (0) root         (0)    20585 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/applicationWindow.py
--rw-rw-rw-   0 root         (0) root         (0)   309800 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/artprovider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 08:43:35.462984 wbBase-0.1.55/Lib/wbBase/control/
--rw-rw-rw-   0 root         (0) root         (0)     1118 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/control/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4414 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/control/externalToolConfig.py
--rw-rw-rw-   0 root         (0) root         (0)     5891 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/control/externalToolConfigUI.py
--rw-rw-rw-   0 root         (0) root         (0)     2666 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/control/filling.py
--rw-rw-rw-   0 root         (0) root         (0)     1670 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/control/iePanel.py
--rw-rw-rw-   0 root         (0) root         (0)     8569 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/control/propgrid.py
--rw-rw-rw-   0 root         (0) root         (0)    47198 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/control/textEditControl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 08:43:35.463984 wbBase-0.1.55/Lib/wbBase/dialog/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/dialog/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2342 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/dialog/multiSaveModifiedDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     3293 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/dialog/multiSaveModifiedDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)    20381 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/dialog/preferences.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 08:43:35.465984 wbBase-0.1.55/Lib/wbBase/document/
--rw-rw-rw-   0 root         (0) root         (0)    23492 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/document/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    36999 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/document/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     4743 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/document/notebook.py
--rw-rw-rw-   0 root         (0) root         (0)     8016 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/document/template.py
--rw-rw-rw-   0 root         (0) root         (0)     9208 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/document/view.py
--rw-rw-rw-   0 root         (0) root         (0)    21455 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/panelManager.py
--rw-rw-rw-   0 root         (0) root         (0)     3366 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/pluginManager.py
--rw-rw-rw-   0 root         (0) root         (0)     2942 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/pluginManager_old.py
--rw-rw-rw-   0 root         (0) root         (0)     8814 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/scripting.py
--rw-rw-rw-   0 root         (0) root         (0)      922 2023-04-30 08:43:33.000000 wbBase-0.1.55/Lib/wbBase/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 08:43:35.460984 wbBase-0.1.55/Lib/wbBase.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2708 2023-04-30 08:43:35.000000 wbBase-0.1.55/Lib/wbBase.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1027 2023-04-30 08:43:35.000000 wbBase-0.1.55/Lib/wbBase.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-30 08:43:35.000000 wbBase-0.1.55/Lib/wbBase.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-04-30 08:43:35.000000 wbBase-0.1.55/Lib/wbBase.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-30 08:43:35.000000 wbBase-0.1.55/Lib/wbBase.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2708 2023-04-30 08:43:35.465984 wbBase-0.1.55/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1347 2023-04-30 08:43:33.000000 wbBase-0.1.55/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2008 2023-04-30 08:43:35.466984 wbBase-0.1.55/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-04-30 08:43:33.000000 wbBase-0.1.55/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:43:09.338598 wbBase-0.1.56/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-05-02 09:43:07.000000 wbBase-0.1.56/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:43:09.326597 wbBase-0.1.56/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:43:09.331597 wbBase-0.1.56/Lib/wbBase/
+-rw-rw-rw-   0 root         (0) root         (0)      153 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23487 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/application.py
+-rw-rw-rw-   0 root         (0) root         (0)     2165 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/applicationInfo.py
+-rw-rw-rw-   0 root         (0) root         (0)    20585 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/applicationWindow.py
+-rw-rw-rw-   0 root         (0) root         (0)   309800 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/artprovider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:43:09.335597 wbBase-0.1.56/Lib/wbBase/control/
+-rw-rw-rw-   0 root         (0) root         (0)     1118 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/control/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4414 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/control/externalToolConfig.py
+-rw-rw-rw-   0 root         (0) root         (0)     5891 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/control/externalToolConfigUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     2666 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/control/filling.py
+-rw-rw-rw-   0 root         (0) root         (0)     1670 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/control/iePanel.py
+-rw-rw-rw-   0 root         (0) root         (0)     8569 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/control/propgrid.py
+-rw-rw-rw-   0 root         (0) root         (0)    47198 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/control/textEditControl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:43:09.336598 wbBase-0.1.56/Lib/wbBase/dialog/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/dialog/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2342 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/dialog/multiSaveModifiedDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     3293 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/dialog/multiSaveModifiedDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)    20381 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/dialog/preferences.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:43:09.338598 wbBase-0.1.56/Lib/wbBase/document/
+-rw-rw-rw-   0 root         (0) root         (0)    23492 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/document/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    36999 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/document/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     4743 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/document/notebook.py
+-rw-rw-rw-   0 root         (0) root         (0)     8016 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/document/template.py
+-rw-rw-rw-   0 root         (0) root         (0)     9208 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/document/view.py
+-rw-rw-rw-   0 root         (0) root         (0)    21455 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/panelManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     3366 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/pluginManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2942 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/pluginManager_old.py
+-rw-rw-rw-   0 root         (0) root         (0)     8814 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/scripting.py
+-rw-rw-rw-   0 root         (0) root         (0)      922 2023-05-02 09:43:07.000000 wbBase-0.1.56/Lib/wbBase/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:43:09.333597 wbBase-0.1.56/Lib/wbBase.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2708 2023-05-02 09:43:09.000000 wbBase-0.1.56/Lib/wbBase.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-05-02 09:43:09.000000 wbBase-0.1.56/Lib/wbBase.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 09:43:09.000000 wbBase-0.1.56/Lib/wbBase.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-05-02 09:43:09.000000 wbBase-0.1.56/Lib/wbBase.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-02 09:43:09.000000 wbBase-0.1.56/Lib/wbBase.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2708 2023-05-02 09:43:09.338598 wbBase-0.1.56/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1347 2023-05-02 09:43:07.000000 wbBase-0.1.56/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2008 2023-05-02 09:43:09.339598 wbBase-0.1.56/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-05-02 09:43:07.000000 wbBase-0.1.56/setup.py
```

### Comparing `wbBase-0.1.55/LICENSE` & `wbBase-0.1.56/LICENSE`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.55/Lib/wbBase/application.py` & `wbBase-0.1.56/Lib/wbBase/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,17 +159,18 @@
         """
         Constructor
         """
         self._debug: int = debug
         self.iconName: str = iconName
         self._test = test
         self._splashScreen: Optional[AppSplashScreen] = None
+        self._extChangeMode: int = self.EXT_CHANGE_TEST_ON_REQUEST
+        self.allowMultipleInstances: bool = False
         self.info: ApplicationInfo = self._getAppInfo(info)
         self.cmdLineArguments: Namespace = self._getCmdLineArguments()
-        self._extChangeMode: int = self.EXT_CHANGE_TEST_ON_REQUEST
         self.extChangeTimerInterval: int = 60
         self.sharedDataDir: str = ""
         self.privateDataDir: str = ""
         self.globalObjects: List[str] = []
         self.dirs = AppDirs(self.info.AppName, self.info.VendorName)
         wx.App.__init__(self, redirect=False, useBestVisual=True)
 
@@ -179,18 +180,17 @@
     # =========================================================================
     # Private methods
     # =========================================================================
 
     def _getAppInfo(self, info: Optional[ApplicationInfo] = None) -> ApplicationInfo:
         if isinstance(info, ApplicationInfo):
             return info
-        if not self.test:
-            appInfoString = self.getResource("application.yml")
-            if isinstance(appInfoString, str):
-                return ApplicationInfo.fromString(appInfoString)
+        appInfoString = self.getResource("application.yml")
+        if isinstance(appInfoString, str):
+            return ApplicationInfo.fromString(appInfoString)
         return ApplicationInfo()
 
     def _getCmdLineArguments(self) -> Namespace:
         """
         :return: parsed command line arguments
         """
         if self.test:
```

### Comparing `wbBase-0.1.55/Lib/wbBase/applicationInfo.py` & `wbBase-0.1.56/Lib/wbBase/applicationInfo.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.55/Lib/wbBase/applicationWindow.py` & `wbBase-0.1.56/Lib/wbBase/applicationWindow.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.55/Lib/wbBase/artprovider.py` & `wbBase-0.1.56/Lib/wbBase/artprovider.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.55/Lib/wbBase/control/__init__.py` & `wbBase-0.1.56/Lib/wbBase/control/__init__.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.55/Lib/wbBase/control/externalToolConfig.py` & `wbBase-0.1.56/Lib/wbBase/control/externalToolConfig.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.55/Lib/wbBase/control/externalToolConfigUI.py` & `wbBase-0.1.56/Lib/wbBase/control/externalToolConfigUI.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.55/Lib/wbBase/control/filling.py` & `wbBase-0.1.56/Lib/wbBase/control/filling.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.55/Lib/wbBase/control/iePanel.py` & `wbBase-0.1.56/Lib/wbBase/control/iePanel.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.55/Lib/wbBase/control/propgrid.py` & `wbBase-0.1.56/Lib/wbBase/control/propgrid.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.55/Lib/wbBase/control/textEditControl.py` & `wbBase-0.1.56/Lib/wbBase/control/textEditControl.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.55/Lib/wbBase/dialog/multiSaveModifiedDialog.py` & `wbBase-0.1.56/Lib/wbBase/dialog/multiSaveModifiedDialog.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.55/Lib/wbBase/dialog/multiSaveModifiedDialogUI.py` & `wbBase-0.1.56/Lib/wbBase/dialog/multiSaveModifiedDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.55/Lib/wbBase/dialog/preferences.py` & `wbBase-0.1.56/Lib/wbBase/dialog/preferences.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.55/Lib/wbBase/document/__init__.py` & `wbBase-0.1.56/Lib/wbBase/document/__init__.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.55/Lib/wbBase/document/manager.py` & `wbBase-0.1.56/Lib/wbBase/document/manager.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.55/Lib/wbBase/document/notebook.py` & `wbBase-0.1.56/Lib/wbBase/document/notebook.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.55/Lib/wbBase/document/template.py` & `wbBase-0.1.56/Lib/wbBase/document/template.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.55/Lib/wbBase/document/view.py` & `wbBase-0.1.56/Lib/wbBase/document/view.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.55/Lib/wbBase/panelManager.py` & `wbBase-0.1.56/Lib/wbBase/panelManager.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.55/Lib/wbBase/pluginManager.py` & `wbBase-0.1.56/Lib/wbBase/pluginManager.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.55/Lib/wbBase/pluginManager_old.py` & `wbBase-0.1.56/Lib/wbBase/pluginManager_old.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.55/Lib/wbBase/scripting.py` & `wbBase-0.1.56/Lib/wbBase/scripting.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.55/Lib/wbBase/tools.py` & `wbBase-0.1.56/Lib/wbBase/tools.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.55/Lib/wbBase.egg-info/PKG-INFO` & `wbBase-0.1.56/Lib/wbBase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbBase
-Version: 0.1.55
+Version: 0.1.56
 Summary: Base package for WorkBench applications.
 Home-page: https://gitlab.com/workbench2/wbbase
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/wbbase
 Project-URL: Documentation, https://workbench2.gitlab.io/wbbase
 Project-URL: Tracker, https://gitlab.com/workbench2/wbbase/-/issues
```

### Comparing `wbBase-0.1.55/Lib/wbBase.egg-info/SOURCES.txt` & `wbBase-0.1.56/Lib/wbBase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.55/PKG-INFO` & `wbBase-0.1.56/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbBase
-Version: 0.1.55
+Version: 0.1.56
 Summary: Base package for WorkBench applications.
 Home-page: https://gitlab.com/workbench2/wbbase
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/wbbase
 Project-URL: Documentation, https://workbench2.gitlab.io/wbbase
 Project-URL: Tracker, https://gitlab.com/workbench2/wbbase/-/issues
```

### Comparing `wbBase-0.1.55/README.md` & `wbBase-0.1.56/README.md`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.55/setup.cfg` & `wbBase-0.1.56/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.55
+current_version = 0.1.56
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
```

