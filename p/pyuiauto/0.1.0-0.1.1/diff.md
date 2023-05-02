# Comparing `tmp/pyUIauto-0.1.0.tar.gz` & `tmp/pyUIauto-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyUIauto-0.1.0.tar", max compression
+gzip compressed data, was "pyUIauto-0.1.1.tar", max compression
```

## Comparing `pyUIauto-0.1.0.tar` & `pyUIauto-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35823 2023-04-28 10:05:55.597442 pyUIauto-0.1.0/LICENSE
--rw-r--r--   0        0        0      905 2023-05-01 14:08:00.757332 pyUIauto-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-28 09:39:50.786949 pyUIauto-0.1.0/pyuiauto/__init__.py
--rw-r--r--   0        0        0      284 2023-04-30 16:07:58.633161 pyUIauto-0.1.0/pyuiauto/application.py
--rw-r--r--   0        0        0     4731 2023-05-01 11:25:04.657715 pyUIauto-0.1.0/pyuiauto/base/application.py
--rw-r--r--   0        0        0    16160 2023-04-28 09:47:59.849084 pyUIauto-0.1.0/pyuiauto/base/components.py
--rw-r--r--   0        0        0      480 2023-04-28 09:44:17.520045 pyUIauto-0.1.0/pyuiauto/components.py
--rw-r--r--   0        0        0      792 2023-04-28 09:39:50.791925 pyUIauto-0.1.0/pyuiauto/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-28 09:39:50.791925 pyUIauto-0.1.0/pyuiauto/mac/__init__.py
--rw-r--r--   0        0        0     4997 2023-05-01 11:00:46.295202 pyUIauto-0.1.0/pyuiauto/mac/application.py
--rw-r--r--   0        0        0    10173 2023-04-28 09:44:17.530103 pyUIauto-0.1.0/pyuiauto/mac/components.py
--rw-r--r--   0        0        0     2520 2023-04-28 09:39:50.795708 pyUIauto-0.1.0/pyuiauto/wait.py
--rw-r--r--   0        0        0        0 2023-04-28 09:39:50.795708 pyUIauto-0.1.0/pyuiauto/win/__init__.py
--rw-r--r--   0        0        0     5939 2023-05-01 11:03:16.196482 pyUIauto-0.1.0/pyuiauto/win/application.py
--rw-r--r--   0        0        0     9490 2023-04-30 10:25:31.695476 pyUIauto-0.1.0/pyuiauto/win/components.py
--rw-r--r--   0        0        0     3317 2023-04-28 12:19:18.231430 pyUIauto-0.1.0/README.md
--rw-r--r--   0        0        0     4321 2023-05-01 14:08:12.339877 pyUIauto-0.1.0/setup.py
--rw-r--r--   0        0        0     4207 2023-05-01 14:08:12.339877 pyUIauto-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-04-28 10:05:55.597442 pyUIauto-0.1.1/LICENSE
+-rw-r--r--   0        0        0      905 2023-05-02 16:12:27.990637 pyUIauto-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-28 09:39:50.786949 pyUIauto-0.1.1/pyuiauto/__init__.py
+-rw-r--r--   0        0        0      284 2023-05-02 16:12:27.991633 pyUIauto-0.1.1/pyuiauto/application.py
+-rw-r--r--   0        0        0     7030 2023-05-02 16:12:27.991633 pyUIauto-0.1.1/pyuiauto/base/application.py
+-rw-r--r--   0        0        0    16166 2023-05-02 16:12:27.992630 pyUIauto-0.1.1/pyuiauto/base/components.py
+-rw-r--r--   0        0        0      480 2023-04-28 09:44:17.520045 pyUIauto-0.1.1/pyuiauto/components.py
+-rw-r--r--   0        0        0      792 2023-04-28 09:39:50.791925 pyUIauto-0.1.1/pyuiauto/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-28 09:39:50.791925 pyUIauto-0.1.1/pyuiauto/mac/__init__.py
+-rw-r--r--   0        0        0     4999 2023-05-02 16:12:27.994623 pyUIauto-0.1.1/pyuiauto/mac/application.py
+-rw-r--r--   0        0        0    10176 2023-05-02 16:12:27.994623 pyUIauto-0.1.1/pyuiauto/mac/components.py
+-rw-r--r--   0        0        0     2522 2023-05-02 16:12:27.996620 pyUIauto-0.1.1/pyuiauto/wait.py
+-rw-r--r--   0        0        0        0 2023-04-28 09:39:50.795708 pyUIauto-0.1.1/pyuiauto/win/__init__.py
+-rw-r--r--   0        0        0     7407 2023-05-02 16:12:27.997615 pyUIauto-0.1.1/pyuiauto/win/application.py
+-rw-r--r--   0        0        0     9497 2023-05-02 16:12:27.999607 pyUIauto-0.1.1/pyuiauto/win/components.py
+-rw-r--r--   0        0        0     3843 2023-05-02 16:12:27.986304 pyUIauto-0.1.1/README.md
+-rw-r--r--   0        0        0     4847 2023-05-02 16:12:38.864334 pyUIauto-0.1.1/setup.py
+-rw-r--r--   0        0        0     4724 2023-05-02 16:12:38.864334 pyUIauto-0.1.1/PKG-INFO
```

### Comparing `pyUIauto-0.1.0/LICENSE` & `pyUIauto-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyUIauto-0.1.0/pyproject.toml` & `pyUIauto-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyUIauto"
-version = "0.1.0"
+version = "0.1.1"
 description = "Python UI Automation library, for cross-platform applications, interfacing through the accessibility API"
 authors = ["Harvey Fretwell <hgfretwell@gmail.com>"]
 maintainers = ["Harvey Fretwell <hgfretwell@gmail.com>"]
 
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/harveyf2801/pyUIauto"
```

### Comparing `pyUIauto-0.1.0/pyuiauto/base/components.py` & `pyUIauto-0.1.1/pyuiauto/base/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,15 +153,15 @@
         Gets all of the components descendants (recursive).\n
         Returns: 
                     descendants: all descendants in a list of type UIBaseComponentWrapper
                     (type should dynamicly wrap to it's cross compatible wrapper)'''
         raise NotImplementedError
 
     @abstractmethod
-    def findAll(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.5, **criteria) -> list[UIBaseComponentWrapper]:
+    def findAll(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria) -> list[UIBaseComponentWrapper]:
         '''Standard base class find all method\n
         Gets all of the components children with the specified criteria.
         Raises an exception if the criteria matches no components (pre order traversal, non recursive).\n
         Args:
                     control_type: the specified control type wrapper to search (of type UIBaseComponentWrapper)
                     
                     (optional criteria)
@@ -169,15 +169,15 @@
 
                     (extra OS specific accessibility API criteria)
         Returns: 
                     components: components dynamicly wrapped to it's cross compatible custom wrapper in a list of type UIBaseComponentWrapper'''
         raise NotImplementedError
     
     @abstractmethod
-    def findFirst(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.5, **criteria) -> UIBaseComponentWrapper:
+    def findFirst(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria) -> UIBaseComponentWrapper:
         '''Standard base class find first method\n
         Gets the first child component with the specified criteria.
         Raises an exception if the criteria matches no components (pre order traversal, non recursive).\n
         Args:
                     control_type: the specified control type wrapper to search (of type UIBaseComponentWrapper)
                     
                     (optional criteria)
@@ -185,15 +185,15 @@
 
                     (extra OS specific accessibility API criteria)
         Returns: 
                     component: component dynamicly wrapped to it's cross compatible custom wrapper of type UIBaseComponentWrapper'''
         raise NotImplementedError
     
     @abstractmethod
-    def findAllR(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.5, **criteria) -> list[UIBaseComponentWrapper]:
+    def findAllR(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria) -> list[UIBaseComponentWrapper]:
         '''Standard base class find all recursive method\n
         Gets all of the components children with the specified criteria.
         Raises an exception if the criteria matches no components (pre order traversal, recursive).\n
         Args:
                     control_type: the specified control type wrapper to search (of type UIBaseComponentWrapper)
                     
                     (optional criteria)
@@ -201,15 +201,15 @@
 
                     (extra OS specific accessibility API criteria)
         Returns: 
                     components: components dynamicly wrapped to it's cross compatible custom wrapper in a list of type UIBaseComponentWrapper'''
         raise NotImplementedError
     
     @abstractmethod
-    def findFirstR(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.5, **criteria) -> UIBaseComponentWrapper:
+    def findFirstR(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria) -> UIBaseComponentWrapper:
         '''Standard base class find first recursive method\n
         Gets the first child component with the specified criteria.
         Raises an exception if the criteria matches no components (pre order traversal, recursive).\n
         Args:
                     control_type: the specified control type wrapper to search (of type UIBaseComponentWrapper)
                     
                     (optional criteria)
@@ -217,15 +217,15 @@
 
                     (extra OS specific accessibility API criteria)
         Returns: 
                     component: component dynamicly wrapped to it's cross compatible custom wrapper of type UIBaseComponentWrapper'''
         raise NotImplementedError
     
     @abstractmethod
-    def find(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.5, **criteria) -> UIBaseComponentWrapper:
+    def find(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria) -> UIBaseComponentWrapper:
         '''Standard base class find method\n
         Finds a child component with the specified criteria.
         Raises an exception if the criteria matches > 1 or no components (non recursive).\n
         Args:
                     control_type: the specified control type wrapper to search (of type UIBaseComponentWrapper)
                     
                     (optional criteria)
@@ -233,15 +233,15 @@
 
                     (extra OS specific accessibility API criteria)
         Returns: 
                     component: component dynamicly wrapped to it's cross compatible custom wrapper of type UIBaseComponentWrapper'''
         raise NotImplementedError
 
     @abstractmethod
-    def findR(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.5, **criteria) -> UIBaseComponentWrapper:
+    def findR(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria) -> UIBaseComponentWrapper:
         '''Standard base class find recursive method\n
         Finds a child component with the specified criteria.
         Raises an exception if the criteria matches > 1 or no components (recursive).\n
         Args:
                     control_type: the specified control type wrapper to search (of type UIBaseComponentWrapper)
                     
                     (optional criteria)
```

### Comparing `pyUIauto-0.1.0/pyuiauto/exceptions.py` & `pyUIauto-0.1.1/pyuiauto/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyUIauto-0.1.0/pyuiauto/mac/application.py` & `pyUIauto-0.1.1/pyuiauto/mac/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,21 +67,21 @@
                                                     **options)
 
     def _findR(self, control_type: Type[UIBaseComponent], **options):
         return UIBaseComponent(self._app).findR(
                                                     control_type=control_type,
                                                     **options)
 
-    def window(self, timeout: int = 1, retry_interval: float = 0.1, **options) -> UIWindow:
+    def window(self, timeout: int = 1, retry_interval: float = 0.01, **options) -> UIWindow:
         try:
             return self.windows(timeout=timeout, retry_interval=retry_interval, **options)[-1]
         except ElementNotFound:
              raise WindowNotFound
     
-    def windows(self, timeout: int = 1, retry_interval: float = 0.1, **options) -> list[UIWindow]:
+    def windows(self, timeout: int = 1, retry_interval: float = 0.01, **options) -> list[UIWindow]:
         try:
             return self._findAllR(control_type=UIWindow, timeout=timeout, retry_interval=retry_interval, **options)
         except ElementNotFound:
              raise WindowNotFound
     
     def isAppAlreadyRunning(self):
         for i in atomacos.NativeUIElement.getRunningApps():
```

### Comparing `pyUIauto-0.1.0/pyuiauto/mac/components.py` & `pyUIauto-0.1.1/pyuiauto/mac/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         return self.component.AXSize
     
     def getChildren(self):
         return list(UIBaseComponent(component, component.AXRole) for component in self.component.AXChildren)
     
     getDescendants = getChildren
     
-    def _wait_find(self, function, check_function, control_type: Type, timeout: int = 1, retry_interval: float = 0.1, **criteria):
+    def _wait_find(self, function, check_function, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
         for i in (  {"conversion": "title", "apple": "AXTitle"},
                     {"conversion": "description", "apple": "AXDescription"},
                 ):
             try:
                 criteria[i["apple"]] = criteria.pop(i["conversion"])
             except KeyError:
                 pass
@@ -123,55 +123,55 @@
                 if type(item) == list:
                     return list(UIBaseComponent(i) for i in item)
                 else:
                     return UIBaseComponent(item)
             time.sleep(retry_interval)
         raise ElementNotFound(f"Element - ControlType: {control_type.native_control_type} - {criteria} - not found after {timeout} seconds")
 
-    def findFirst(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.5, **criteria):
+    def findFirst(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
         return self._wait_find(function=self.component.findFirst,
                                 check_function=self._check_element_exists,
                                 control_type=control_type,
                                 timeout=timeout,
                                 retry_interval = retry_interval,
                                 **criteria)
 
-    def findAll(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.5, **criteria):
+    def findAll(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
         return self._wait_find(function=self.component.findAll,
                                 check_function=self._check_elements_exist,
                                 control_type=control_type,
                                 timeout=timeout,
                                 retry_interval = retry_interval,
                                 **criteria)
 
-    def findFirstR(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.5, **criteria):
+    def findFirstR(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
         return self._wait_find(function=self.component.findFirstR,
                                 check_function=self._check_element_exists,
                                 control_type=control_type,
                                 timeout=timeout,
                                 retry_interval = retry_interval,
                                 **criteria)
 
-    def findAllR(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.5, **criteria):
+    def findAllR(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
         return self._wait_find(function=self.component.findAllR,
                                 check_function=self._check_elements_exist,
                                 control_type=control_type,
                                 timeout=timeout,
                                 retry_interval = retry_interval,
                                 **criteria)
     
-    def find(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.5, **criteria):
+    def find(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
         items = self.findAll(control_type, timeout, retry_interval, **criteria)
         
         if len(items) > 1:
             raise ElementNotFound(f"{len(items)} Elements found matching the criteria - ControlType: {control_type} - {criteria}")
 
         return items[0]
     
-    def findR(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.5, **criteria):
+    def findR(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
         items = self.findAllR(control_type, timeout, retry_interval, **criteria)
         
         if len(items) > 1:
             raise ElementNotFound(f"{len(items)} Elements found matching the criteria - ControlType: {control_type} - {criteria}")
 
         return items[0]
     
@@ -189,15 +189,15 @@
     def title(self) -> str:
         return self.component.AXTitle
 
 
 # ============================================
 
 
-class UIApplication(UIBaseComponent):
+class UIAppRoot(UIBaseComponent):
     native_control_type: str = "AXApplication"
 
 
 # ============================================
 
 
 class UIButton(UIBaseComponent, UIButtonWrapper):
```

### Comparing `pyUIauto-0.1.0/pyuiauto/wait.py` & `pyUIauto-0.1.1/pyuiauto/wait.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import time
 
-def wait_until_condition(conditional_func, timeout: float = 3, retry_interval: float = 0.1, *func_args, **func_kwargs) -> bool:
+def wait_until_condition(conditional_func, timeout: float = 3, retry_interval: float = 0.01, *func_args, **func_kwargs) -> bool:
     '''Wait until condition function\n
     Returns True if the conditional function returns a value that is True before the Timeout is reached.\n
     However, returns False if the conditional function doesn't return a value that is True before the Timeout is reached.\n
     Args:
                     conditional_func: the function to perform on each iteration check
                     
                     (optional)
@@ -18,15 +18,15 @@
     '''
     timeafter = time.time() + timeout
     while time.time() < timeafter:
         if conditional_func(*func_args, **func_kwargs): return True
         time.sleep(retry_interval)
     return False
 
-def wait_until_raise(conditional_func, error: Exception = TimeoutError(), timeout: float = 3, retry_interval: float = 0.1, *func_args, **func_kwargs):
+def wait_until_raise(conditional_func, error: Exception = TimeoutError(), timeout: float = 3, retry_interval: float = 0.01, *func_args, **func_kwargs):
     '''Wait until raise function\n
     Returns the value if the conditional function returns a value that is True before the Timeout is reached.\n
     However, raises an error if the conditional function doesn't return a value that is True before the Timeout is reached.\n
     Args:
                     conditional_func: the function to perform on each iteration check
                     
                     (optional)
```

### Comparing `pyUIauto-0.1.0/pyuiauto/win/components.py` & `pyUIauto-0.1.1/pyuiauto/win/components.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,58 +104,58 @@
     
     def getChildren(self):
         return list(UIBaseComponent(component) for component in self.component.children())
 
     def getDescendants(self):
         return list(UIBaseComponent(component) for component in self.component.descendants())
     
-    def _wait_find(self, function, check_function, control_type: Type, timeout: int = 1, retry_interval: float = 0.5, **criteria):
+    def _wait_find(self, function, check_function, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
         timeafter = time.time() + timeout
         while time.time() < timeafter:
             item = function(control_type=control_type.native_control_type, **criteria)
             item_check = check_function(item)
             if item_check:
                 if type(item) == list:
                     return list(UIBaseComponent(i) for i in item)
                 else:
                     return UIBaseComponent(item)
             time.sleep(retry_interval)
         raise ElementNotFound(f"CheckFunction returned: Element - ControlType: {control_type.native_control_type} - {criteria} - not found after {timeout} seconds")
         
-    def findAll(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.5, **criteria):
+    def findAll(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
         return self._wait_find(function=self.component.children,
                         check_function=self._check_elements_exist,
                         control_type=control_type,
                         timeout=timeout,
                         retry_interval=retry_interval,
                         **criteria)
     
-    def findFirst(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.5, **criteria):
+    def findFirst(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
         return self.findAll(control_type, timeout, retry_interval, **criteria)[0]
 
-    def find(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.5, **criteria):
+    def find(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
         items = self.findAll(control_type, timeout, retry_interval, **criteria)
         
         if len(items) > 1:
             raise ElementNotFound(f"{len(items)} Elements found matching the criteria - ControlType: {control_type} - {criteria}")
 
         return items[0]
     
-    def findAllR(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.5, **criteria):
+    def findAllR(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
         return self._wait_find(function=self.component.descendants,
                         check_function=self._check_elements_exist,
                         control_type=control_type,
                         timeout=timeout,
                         retry_interval=retry_interval,
                         **criteria)
     
-    def findFirstR(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.5, **criteria):
+    def findFirstR(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
         return self.findAllR(control_type, timeout, retry_interval, **criteria)[0]
 
-    def findR(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.5, **criteria):
+    def findR(self, control_type: Type, timeout: int = 1, retry_interval: float = 0.01, **criteria):
         items = self.findAllR(control_type, timeout, retry_interval, **criteria)
         
         if len(items) > 1:
             raise ElementNotFound(f"{len(items)} Elements found matching the criteria - ControlType: {control_type} - {criteria}")
 
         return items[0]
```

### Comparing `pyUIauto-0.1.0/README.md` & `pyUIauto-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 # pyUIauto
 
-| Branch      | Status                                                                                                                  |
+[![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)
+[![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)
+[![PyPi version](https://badgen.net/pypi/v/pyuiauto/)](https://pypi.org/project/pyuiauto/)
+[![PyPi license](https://badgen.net/pypi/license/pyuiauto/)](https://pypi.org/project/pyuiauto/)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/pyuiauto.svg)](https://pypi.python.org/pypi/pyuiauto/)
+
+
+| Tests       | Status                                                                                                                  |
 | :---------- | :---------------------------------------------------------------------------------------------------------------------: |
-| Main        | ![Main Branch](https://github.com/harveyf2801/pyUIauto/actions/workflows/run_dev_tests.yml/badge.svg?branch=main)       |
-| Develop     | ![Develop Branch](https://github.com/harveyf2801/pyUIauto/actions/workflows/run_dev_tests.yml/badge.svg?branch=develop) |
+| Development | ![Development Tests](https://github.com/harveyf2801/pyUIauto/actions/workflows/run_dev_tests.yml/badge.svg?branch=main)       |
+| Build       | ![Build Tests](https://github.com/harveyf2801/pyUIauto/actions/workflows/build_wheel.yml/badge.svg?branch=main) |
 
 Python UI Automation library, for cross-platform applications, interfacing through the accessibility API.
 
 ## Description
 
 This library / framework takes two popular UI automation libraries and combines their functionality by wrapping them into custom components and creating methods that function in similar ways for both OS. This project was originally designed as part of a QA automation project to perform end-to-end testing on desktop applications.
 
@@ -72,13 +79,15 @@
 ex. [atomacos](https://github.com/daveenguyen/atomacos)
 ex. [pyAutoGUI](https://github.com/asweigart/pyautogui)
 
 ## Version History
 
 - 0.1
   - Initial Release
+  - 0.1.1
+    - Added UISystemTrayIcon and UIPopupMenu manager
 
 ## Acknowledgments
 
 - [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)
 - [atomacos](https://github.com/daveenguyen/atomacos)
 - [pyAutoGUI](https://github.com/asweigart/pyautogui)
```

### Comparing `pyUIauto-0.1.0/setup.py` & `pyUIauto-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 extras_require = \
 {':sys_platform == "darwin"': ['atomacos>=3.3.0,<4.0.0'],
  ':sys_platform == "win32"': ['pywinauto>=0.6.8,<0.7.0']}
 
 setup_kwargs = {
     'name': 'pyuiauto',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Python UI Automation library, for cross-platform applications, interfacing through the accessibility API',
-    'long_description': '# pyUIauto\n\n| Branch      | Status                                                                                                                  |\n| :---------- | :---------------------------------------------------------------------------------------------------------------------: |\n| Main        | ![Main Branch](https://github.com/harveyf2801/pyUIauto/actions/workflows/run_dev_tests.yml/badge.svg?branch=main)       |\n| Develop     | ![Develop Branch](https://github.com/harveyf2801/pyUIauto/actions/workflows/run_dev_tests.yml/badge.svg?branch=develop) |\n\nPython UI Automation library, for cross-platform applications, interfacing through the accessibility API.\n\n## Description\n\nThis library / framework takes two popular UI automation libraries and combines their functionality by wrapping them into custom components and creating methods that function in similar ways for both OS. This project was originally designed as part of a QA automation project to perform end-to-end testing on desktop applications.\n\n## Getting Started\n\n### Dependencies\n\nPython Packages:\n\n- pywinauto (Windows / Linux)\n- atomacos (MacOS)\n- pyautogui\n\nOS Compatibility:\n\n- Windows\n- MacOS\n\n( Currently untested on Linux )\n\n## Example\n\n```python\n# Import the tools needed\nfrom platform import system\nimport os\nfrom pyuiauto.application import UIApplication\nfrom pyuiauto.components import UIButton\n\n# Finding the path location of the application\napp_paths = {\n  "Darwin": "/Applications/Visual Studio Code.app",\n  "Windows": os.path.expanduser(\'~\') + "\\\\AppData\\\\Local\\\\Programs\\\\Microsoft VS Code\\\\Code.exe"\n}\n\nif system() in app_paths:\n  appPath = app_paths[system()]\nelse:\n  raise NotImplementedError("The current OS is not currently supported: " + system())\n\n# Setting up an application template, launching the app, and connecting to it\napp = UIApplication(appName = "Visual Studio Code", appPath = appPath)\napp.launchApp()\napp.connectApp()\n\n# Finding the window component and searching for elements within this window component\nmain_window = app.window(title = "Visual Studio Code", timeout = 2)\nmain_window.findR(title = "Toggle Primary Side Bar (Ctrl+B)", control_type = UIButton).press() \'\'\'  press will invoke a button without manually moving the mouse and clicking it \n                                                                                          (a button could be invoked even if it isn\'t currently visible)  \'\'\'\nmain_window.findR(title = "Open Folder", control_type = UIButton).click() \'\'\' however, click will move the mouse to the button location and click it\n                                                                    (sometimes this can be more reliable) \'\'\'\n\n# Closing the window and terminating the application\nmain_window.close()\napp.terminateApp()\n```\n\n## Authors\n\nex. Harvey Fretwell\nex. [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)\nex. [atomacos](https://github.com/daveenguyen/atomacos)\nex. [pyAutoGUI](https://github.com/asweigart/pyautogui)\n\n## Version History\n\n- 0.1\n  - Initial Release\n\n## Acknowledgments\n\n- [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)\n- [atomacos](https://github.com/daveenguyen/atomacos)\n- [pyAutoGUI](https://github.com/asweigart/pyautogui)\n',
+    'long_description': '# pyUIauto\n\n[![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)\n[![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)\n[![PyPi version](https://badgen.net/pypi/v/pyuiauto/)](https://pypi.org/project/pyuiauto/)\n[![PyPi license](https://badgen.net/pypi/license/pyuiauto/)](https://pypi.org/project/pyuiauto/)\n[![PyPI pyversions](https://img.shields.io/pypi/pyversions/pyuiauto.svg)](https://pypi.python.org/pypi/pyuiauto/)\n\n\n| Tests       | Status                                                                                                                  |\n| :---------- | :---------------------------------------------------------------------------------------------------------------------: |\n| Development | ![Development Tests](https://github.com/harveyf2801/pyUIauto/actions/workflows/run_dev_tests.yml/badge.svg?branch=main)       |\n| Build       | ![Build Tests](https://github.com/harveyf2801/pyUIauto/actions/workflows/build_wheel.yml/badge.svg?branch=main) |\n\nPython UI Automation library, for cross-platform applications, interfacing through the accessibility API.\n\n## Description\n\nThis library / framework takes two popular UI automation libraries and combines their functionality by wrapping them into custom components and creating methods that function in similar ways for both OS. This project was originally designed as part of a QA automation project to perform end-to-end testing on desktop applications.\n\n## Getting Started\n\n### Dependencies\n\nPython Packages:\n\n- pywinauto (Windows / Linux)\n- atomacos (MacOS)\n- pyautogui\n\nOS Compatibility:\n\n- Windows\n- MacOS\n\n( Currently untested on Linux )\n\n## Example\n\n```python\n# Import the tools needed\nfrom platform import system\nimport os\nfrom pyuiauto.application import UIApplication\nfrom pyuiauto.components import UIButton\n\n# Finding the path location of the application\napp_paths = {\n  "Darwin": "/Applications/Visual Studio Code.app",\n  "Windows": os.path.expanduser(\'~\') + "\\\\AppData\\\\Local\\\\Programs\\\\Microsoft VS Code\\\\Code.exe"\n}\n\nif system() in app_paths:\n  appPath = app_paths[system()]\nelse:\n  raise NotImplementedError("The current OS is not currently supported: " + system())\n\n# Setting up an application template, launching the app, and connecting to it\napp = UIApplication(appName = "Visual Studio Code", appPath = appPath)\napp.launchApp()\napp.connectApp()\n\n# Finding the window component and searching for elements within this window component\nmain_window = app.window(title = "Visual Studio Code", timeout = 2)\nmain_window.findR(title = "Toggle Primary Side Bar (Ctrl+B)", control_type = UIButton).press() \'\'\'  press will invoke a button without manually moving the mouse and clicking it \n                                                                                          (a button could be invoked even if it isn\'t currently visible)  \'\'\'\nmain_window.findR(title = "Open Folder", control_type = UIButton).click() \'\'\' however, click will move the mouse to the button location and click it\n                                                                    (sometimes this can be more reliable) \'\'\'\n\n# Closing the window and terminating the application\nmain_window.close()\napp.terminateApp()\n```\n\n## Authors\n\nex. Harvey Fretwell\nex. [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)\nex. [atomacos](https://github.com/daveenguyen/atomacos)\nex. [pyAutoGUI](https://github.com/asweigart/pyautogui)\n\n## Version History\n\n- 0.1\n  - Initial Release\n  - 0.1.1\n    - Added UISystemTrayIcon and UIPopupMenu manager\n\n## Acknowledgments\n\n- [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)\n- [atomacos](https://github.com/daveenguyen/atomacos)\n- [pyAutoGUI](https://github.com/asweigart/pyautogui)\n',
     'author': 'Harvey Fretwell',
     'author_email': 'hgfretwell@gmail.com',
     'maintainer': 'Harvey Fretwell',
     'maintainer_email': 'hgfretwell@gmail.com',
     'url': 'https://github.com/harveyf2801/pyUIauto',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pyUIauto-0.1.0/PKG-INFO` & `pyUIauto-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyuiauto
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python UI Automation library, for cross-platform applications, interfacing through the accessibility API
 Home-page: https://github.com/harveyf2801/pyUIauto
 License: GPL-3.0-only
 Keywords: automation,accessibility,cross-platform,ui,desktop,pywinauto,atomac
 Author: Harvey Fretwell
 Author-email: hgfretwell@gmail.com
 Maintainer: Harvey Fretwell
@@ -18,18 +18,25 @@
 Requires-Dist: pyautogui (==0.9.41)
 Requires-Dist: pywinauto (>=0.6.8,<0.7.0); sys_platform == "win32"
 Project-URL: Repository, https://github.com/harveyf2801/pyUIauto
 Description-Content-Type: text/markdown
 
 # pyUIauto
 
-| Branch      | Status                                                                                                                  |
+[![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)
+[![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)
+[![PyPi version](https://badgen.net/pypi/v/pyuiauto/)](https://pypi.org/project/pyuiauto/)
+[![PyPi license](https://badgen.net/pypi/license/pyuiauto/)](https://pypi.org/project/pyuiauto/)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/pyuiauto.svg)](https://pypi.python.org/pypi/pyuiauto/)
+
+
+| Tests       | Status                                                                                                                  |
 | :---------- | :---------------------------------------------------------------------------------------------------------------------: |
-| Main        | ![Main Branch](https://github.com/harveyf2801/pyUIauto/actions/workflows/run_dev_tests.yml/badge.svg?branch=main)       |
-| Develop     | ![Develop Branch](https://github.com/harveyf2801/pyUIauto/actions/workflows/run_dev_tests.yml/badge.svg?branch=develop) |
+| Development | ![Development Tests](https://github.com/harveyf2801/pyUIauto/actions/workflows/run_dev_tests.yml/badge.svg?branch=main)       |
+| Build       | ![Build Tests](https://github.com/harveyf2801/pyUIauto/actions/workflows/build_wheel.yml/badge.svg?branch=main) |
 
 Python UI Automation library, for cross-platform applications, interfacing through the accessibility API.
 
 ## Description
 
 This library / framework takes two popular UI automation libraries and combines their functionality by wrapping them into custom components and creating methods that function in similar ways for both OS. This project was originally designed as part of a QA automation project to perform end-to-end testing on desktop applications.
 
@@ -94,14 +101,16 @@
 ex. [atomacos](https://github.com/daveenguyen/atomacos)
 ex. [pyAutoGUI](https://github.com/asweigart/pyautogui)
 
 ## Version History
 
 - 0.1
   - Initial Release
+  - 0.1.1
+    - Added UISystemTrayIcon and UIPopupMenu manager
 
 ## Acknowledgments
 
 - [pyWinAuto](https://github.com/pywinauto/pywinauto/tree/master)
 - [atomacos](https://github.com/daveenguyen/atomacos)
 - [pyAutoGUI](https://github.com/asweigart/pyautogui)
```

