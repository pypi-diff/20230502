# Comparing `tmp/relative-addons-system-2.4.4.tar.gz` & `tmp/relative-addons-system-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relative-addons-system-2.4.4.tar", last modified: Tue Nov  8 14:35:57 2022, max compression
+gzip compressed data, was "relative-addons-system-2.5.0.tar", last modified: Tue May  2 09:09:09 2023, max compression
```

## Comparing `relative-addons-system-2.4.4.tar` & `relative-addons-system-2.5.0.tar`

### file list

```diff
@@ -1,30 +1,27 @@
-drwxrwxr-x   0 youngtitanium  (1000) youngtitanium  (1000)        0 2022-11-08 14:35:57.966009 relative-addons-system-2.4.4/
--rw-rw-r--   0 youngtitanium  (1000) youngtitanium  (1000)     1064 2022-10-11 13:46:51.000000 relative-addons-system-2.4.4/LICENSE
--rw-rw-r--   0 youngtitanium  (1000) youngtitanium  (1000)     4615 2022-11-08 14:35:57.965008 relative-addons-system-2.4.4/PKG-INFO
--rw-rw-r--   0 youngtitanium  (1000) youngtitanium  (1000)     2846 2022-10-12 08:11:17.000000 relative-addons-system-2.4.4/README.md
-drwxrwxr-x   0 youngtitanium  (1000) youngtitanium  (1000)        0 2022-11-08 14:35:57.578009 relative-addons-system-2.4.4/RelativeAddonsSystem/
--rwxrwxrwx   0 youngtitanium  (1000) youngtitanium  (1000)      307 2022-11-08 14:20:04.000000 relative-addons-system-2.4.4/RelativeAddonsSystem/__init__.py
-drwxrwxr-x   0 youngtitanium  (1000) youngtitanium  (1000)        0 2022-11-08 14:35:57.777009 relative-addons-system-2.4.4/RelativeAddonsSystem/addon/
--rw-rw-r--   0 youngtitanium  (1000) youngtitanium  (1000)     5068 2022-10-25 18:38:09.000000 relative-addons-system-2.4.4/RelativeAddonsSystem/addon/__init__.py
--rw-rw-r--   0 youngtitanium  (1000) youngtitanium  (1000)     1159 2022-10-11 12:53:02.000000 relative-addons-system-2.4.4/RelativeAddonsSystem/addon/configuration.py
--rw-rw-r--   0 youngtitanium  (1000) youngtitanium  (1000)     1549 2022-10-12 08:09:03.000000 relative-addons-system-2.4.4/RelativeAddonsSystem/addon/metadata.py
--rw-rw-r--   0 youngtitanium  (1000) youngtitanium  (1000)     1928 2022-11-08 14:18:56.000000 relative-addons-system-2.4.4/RelativeAddonsSystem/libraries.py
--rwxrwxrwx   0 youngtitanium  (1000) youngtitanium  (1000)    10587 2022-10-25 18:28:28.000000 relative-addons-system-2.4.4/RelativeAddonsSystem/system.py
-drwxrwxr-x   0 youngtitanium  (1000) youngtitanium  (1000)        0 2022-11-08 14:35:57.961008 relative-addons-system-2.4.4/RelativeAddonsSystem/utils/
--rwxrwxrwx   0 youngtitanium  (1000) youngtitanium  (1000)      138 2022-10-25 18:37:38.000000 relative-addons-system-2.4.4/RelativeAddonsSystem/utils/__init__.py
--rw-rw-r--   0 youngtitanium  (1000) youngtitanium  (1000)      382 2022-10-25 18:37:38.000000 relative-addons-system-2.4.4/RelativeAddonsSystem/utils/recursive_reload_module.py
--rwxrwxrwx   0 youngtitanium  (1000) youngtitanium  (1000)     1442 2022-05-31 14:24:29.000000 relative-addons-system-2.4.4/RelativeAddonsSystem/utils/version_checker.py
--rwxrwxrwx   0 youngtitanium  (1000) youngtitanium  (1000)      397 2022-05-29 14:01:09.000000 relative-addons-system-2.4.4/RelativeAddonsSystem/utils/version_tranform.py
--rw-rw-r--   0 youngtitanium  (1000) youngtitanium  (1000)      760 2022-11-08 14:20:31.000000 relative-addons-system-2.4.4/pyproject.toml
-drwxrwxr-x   0 youngtitanium  (1000) youngtitanium  (1000)        0 2022-11-08 14:35:57.963008 relative-addons-system-2.4.4/relative_addons_system.egg-info/
--rw-rw-r--   0 youngtitanium  (1000) youngtitanium  (1000)     4615 2022-11-08 14:35:57.000000 relative-addons-system-2.4.4/relative_addons_system.egg-info/PKG-INFO
--rw-rw-r--   0 youngtitanium  (1000) youngtitanium  (1000)      726 2022-11-08 14:35:57.000000 relative-addons-system-2.4.4/relative_addons_system.egg-info/SOURCES.txt
--rw-rw-r--   0 youngtitanium  (1000) youngtitanium  (1000)        1 2022-11-08 14:35:57.000000 relative-addons-system-2.4.4/relative_addons_system.egg-info/dependency_links.txt
--rw-rw-r--   0 youngtitanium  (1000) youngtitanium  (1000)       13 2022-11-08 14:35:57.000000 relative-addons-system-2.4.4/relative_addons_system.egg-info/requires.txt
--rw-rw-r--   0 youngtitanium  (1000) youngtitanium  (1000)       32 2022-11-08 14:35:57.000000 relative-addons-system-2.4.4/relative_addons_system.egg-info/top_level.txt
--rw-rw-r--   0 youngtitanium  (1000) youngtitanium  (1000)       38 2022-11-08 14:35:57.966009 relative-addons-system-2.4.4/setup.cfg
--rwxrwxrwx   0 youngtitanium  (1000) youngtitanium  (1000)      902 2022-11-08 14:20:04.000000 relative-addons-system-2.4.4/setup.py
-drwxrwxr-x   0 youngtitanium  (1000) youngtitanium  (1000)        0 2022-11-08 14:35:57.964008 relative-addons-system-2.4.4/virtualenv/
--rw-rw-r--   0 youngtitanium  (1000) youngtitanium  (1000)        0 2022-10-11 09:05:56.000000 relative-addons-system-2.4.4/virtualenv/__init__.py
-drwxrwxr-x   0 youngtitanium  (1000) youngtitanium  (1000)        0 2022-11-08 14:35:57.964008 relative-addons-system-2.4.4/virtualenv/lib/
--rw-rw-r--   0 youngtitanium  (1000) youngtitanium  (1000)        0 2022-10-11 09:05:56.000000 relative-addons-system-2.4.4/virtualenv/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:09:09.089102 relative-addons-system-2.5.0/
+-rw-rw-rw-   0        0        0     1064 2022-10-11 13:46:50.000000 relative-addons-system-2.5.0/LICENSE
+-rw-rw-rw-   0        0        0     5784 2023-05-02 09:09:09.086102 relative-addons-system-2.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3851 2023-05-02 08:59:29.000000 relative-addons-system-2.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 09:09:09.017121 relative-addons-system-2.5.0/RelativeAddonsSystem/
+-rw-rw-rw-   0        0        0      309 2023-05-02 09:00:55.000000 relative-addons-system-2.5.0/RelativeAddonsSystem/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:09:09.026101 relative-addons-system-2.5.0/RelativeAddonsSystem/addon/
+-rw-rw-rw-   0        0        0     5402 2023-05-02 08:41:08.000000 relative-addons-system-2.5.0/RelativeAddonsSystem/addon/__init__.py
+-rw-rw-rw-   0        0        0     1632 2023-05-02 08:26:45.000000 relative-addons-system-2.5.0/RelativeAddonsSystem/addon/metadata.py
+-rw-rw-rw-   0        0        0     1911 2023-05-02 08:06:08.000000 relative-addons-system-2.5.0/RelativeAddonsSystem/libraries.py
+-rw-rw-rw-   0        0        0    10612 2023-05-02 08:38:57.000000 relative-addons-system-2.5.0/RelativeAddonsSystem/system.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:09:09.052100 relative-addons-system-2.5.0/RelativeAddonsSystem/utils/
+-rw-rw-rw-   0        0        0      215 2023-04-16 16:56:05.000000 relative-addons-system-2.5.0/RelativeAddonsSystem/utils/__init__.py
+-rw-rw-rw-   0        0        0     2466 2023-05-02 08:33:45.000000 relative-addons-system-2.5.0/RelativeAddonsSystem/utils/cache.py
+-rw-rw-rw-   0        0        0      382 2022-10-25 18:37:38.000000 relative-addons-system-2.5.0/RelativeAddonsSystem/utils/recursive_reload_module.py
+-rw-rw-rw-   0        0        0     1629 2023-05-02 08:40:18.000000 relative-addons-system-2.5.0/RelativeAddonsSystem/utils/storage.py
+-rw-rw-rw-   0        0        0     1442 2022-05-31 14:24:28.000000 relative-addons-system-2.5.0/RelativeAddonsSystem/utils/version_checker.py
+-rw-rw-rw-   0        0        0      397 2023-05-02 08:06:08.000000 relative-addons-system-2.5.0/RelativeAddonsSystem/utils/version_transform.py
+-rw-rw-rw-   0        0        0      760 2023-05-02 09:02:47.000000 relative-addons-system-2.5.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-02 09:09:09.083100 relative-addons-system-2.5.0/relative_addons_system.egg-info/
+-rw-rw-rw-   0        0        0     5784 2023-05-02 09:09:08.000000 relative-addons-system-2.5.0/relative_addons_system.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      707 2023-05-02 09:09:08.000000 relative-addons-system-2.5.0/relative_addons_system.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 09:09:08.000000 relative-addons-system-2.5.0/relative_addons_system.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-02 09:09:08.000000 relative-addons-system-2.5.0/relative_addons_system.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-02 09:09:08.000000 relative-addons-system-2.5.0/relative_addons_system.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 09:09:09.089102 relative-addons-system-2.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      902 2022-11-08 14:20:04.000000 relative-addons-system-2.5.0/setup.py
```

### Comparing `relative-addons-system-2.4.4/LICENSE` & `relative-addons-system-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `relative-addons-system-2.4.4/README.md` & `relative-addons-system-2.5.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,26 @@
-## Relative Addons System
-**This is special system which allow you to manage your addons**
+# Relative Addons System
+**This is a special system that allows you to manage your addons in runtime.**
 
-**Addon** is a folder with ``addon.json`` and ``__init__.py`` files
+**The library has caching that allows it to work faster**
 
-**_Example:_**
+## Definitions
+**Addon** - directory that contains `addon.json` and `__init__.py`  
+**addon.json** is a `json` file that describes addon and must contain `name`, `author`, 
+`description` and `version`(strings)
+
+
+## Usage examples
 ```python
 from pathlib import Path
 
 from RelativeAddonsSystem import RelativeAddonsSystem, Addon, AddonMeta
 
 # Init addons system
-system = RelativeAddonsSystem(Path(__file__).parent / "addons")
+system = RelativeAddonsSystem(Path(__file__).parent / "addons", auto_install_requirements=True)
 
 # return list of Addon objects
 addons: list[Addon] = system.get_all_addons()
 
 if len(addons) < 1:
     print("No addons found")
 else:
@@ -34,45 +40,45 @@
             print("Addon dependencies already satisfied")
         
         # Get addon module
         module = addon.module # ADDON_DIR / __init__.py module
         ...
 ```
 
-**In this example, we have listed all addons and install their dependencies if they are not installed**
+**In this example, we have listed all addons and installed their dependencies if they were not already installed.**
 
-**You can also disable or enable addons:**
+**We can also disable or enable addons:**
 
 ```python
 from pathlib import Path
 
 from RelativeAddonsSystem import RelativeAddonsSystem, Addon
 
 # Init addons system
-system = RelativeAddonsSystem(Path(__file__).parent / "addons")
+system = RelativeAddonsSystem(Path(__file__).parent / "addons", auto_install_requirements=True)
 
 addons: list[Addon] = system.get_enabled_addons() # get all enabled addons
 
 if len(addons) > 0:
     addon: Addon = addons[0] # first addon from list
     addon.disable() # disable addon
     
     ...
     
     addon.enable() # enable addon
 ```
 
-**_Or import, reimport(Useful when you updated your addon) module:_**
+**_Or import and re-import the module (useful when we have updated your addon):_**
 ```python
 from pathlib import Path
 
 from RelativeAddonsSystem import RelativeAddonsSystem, Addon
 
 # Init addons system
-system = RelativeAddonsSystem(Path(__file__).parent / "addons")
+system = RelativeAddonsSystem(Path(__file__).parent / "addons", auto_install_requirements=True)
 
 addons: list[Addon] = system.get_enabled_addons() # get all enabled addons
 
 if len(addons) > 0:
     addon: Addon = addons[0] # first addon from list
     
     module = addon.module
@@ -81,27 +87,50 @@
 
     # Reimport module
     module = addon.reload_module()
     
     ... # Work with module
 ```
 
-**_You can also change the meta in your code:_**
+**_We can also change the metadata in your code:_**
 ```python
 from pathlib import Path
 
 from RelativeAddonsSystem import RelativeAddonsSystem, Addon, AddonMeta
 
 # Init addons system
-system = RelativeAddonsSystem(Path(__file__).parent / "addons")
+system = RelativeAddonsSystem(Path(__file__).parent / "addons", auto_install_requirements=True)
 
 addons: list[Addon] = system.get_enabled_addons() # get all enabled addons
 
 if len(addons) > 0:
     addon: Addon = addons[0] # first addon from list
     
     meta: AddonMeta = addon.meta
 
     meta.set("version", "1.2")
 
     meta.save()
 ```
+
+**_Or set specific data into the addon's storage:_**
+```python
+from pathlib import Path
+
+from RelativeAddonsSystem import RelativeAddonsSystem, Addon
+from RelativeAddonsSystem.utils import Storage
+
+# Init addons system
+system = RelativeAddonsSystem(Path(__file__).parent / "addons", auto_install_requirements=True)
+
+addons: list[Addon] = system.get_enabled_addons() # get all enabled addons
+
+if len(addons) > 0:
+    addon: Addon = addons[0] # first addon from list
+    
+    # Loaded the ADDON_DIR/ADDON_NAME-storage.json file
+    storage: Storage = addon.get_storage()
+
+    storage.set("api_version", "1.2")
+
+    storage.save()
+```
```

### Comparing `relative-addons-system-2.4.4/RelativeAddonsSystem/addon/configuration.py` & `relative-addons-system-2.5.0/RelativeAddonsSystem/utils/storage.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,56 @@
 import json
 from pathlib import Path
+from typing import Any
 
 
-class AddonConfig:
+class Storage:
 
     def __init__(self, path: Path):
         self._path = path
 
         self._map = {}
 
         self.read()
 
+    def initialize(self, default_data: dict):
+        if not isinstance(default_data, dict):
+            raise ValueError("Default data should be dictionary type")
+
+        flush = False
+
+        for key, value in default_data.items():
+            if key not in self._map:
+                self._map[key] = value
+                if not flush:
+                    flush = True
+
+        if flush:
+            self.save()
+
     def read(self):
         if not self._path.exists():
-            with open(self._path, "w", encoding="utf8") as file:
-                json.dump({}, file, ensure_ascii=False, indent=4)
+            self.save()
 
             self._map = {}
             return
 
-        with open(self._path, "r", encoding="utf8") as file:
+        with self._path.open("r", encoding="utf8") as file:
             self._map = json.load(file)
 
     def save(self):
-        with open(self._path, "w", encoding="utf8") as file:
-            json.dump(self._map, file, ensure_ascii=False, indent=4)
+        with self._path.open("w", encoding="utf8") as file:
+            json.dump(self._map, file, ensure_ascii=False, indent=2)
 
-    def get(self, name: str, default: object=None):
+    def get(self, name: str, default: Any = None) -> int | str | dict | list | float | bool:
         if name not in self._map:
             return default
         return self._map[name]
 
-    def set(self, name: str, value: object):
+    def set(self, name: str, value: int | str | dict | list | float | bool):
         json.dumps(value)
 
         self._map[name] = value
 
     def keys(self):
         return self._map.keys()
 
@@ -43,7 +58,10 @@
         self.set(key, value)
 
     def __getitem__(self, item):
         if item not in self._map:
             raise KeyError(item)
 
         return self._map[item]
+
+    def __contains__(self, item):
+        return item in self._map
```

### Comparing `relative-addons-system-2.4.4/RelativeAddonsSystem/addon/metadata.py` & `relative-addons-system-2.5.0/RelativeAddonsSystem/addon/metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import json
 from pathlib import Path
+from typing import Any
 
 
 class AddonMeta:
-
     name: str
     version: str
     description: str
     author: str
-    status: str
-    requirements: list[dict[str, str]]
+    status: str | None
+    requirements: list[dict[str, str]] | None
 
     def __init__(self, path: Path):
         self._path = path
 
         self._keys = []
 
         self.load()
 
-    def get(self, name: str, default: object):
+    def get(self, name: str, default: Any = None) -> int | str | dict | list | float | bool:
         if name not in self:
             return default
 
         return self[name]
 
     def set(self, name: str, value: object):
         json.dumps(value)
@@ -64,8 +64,8 @@
                 {
                     name: self[name]
                     for name in self._keys
                 },
                 meta_file,
                 ensure_ascii=False,
                 indent=4
-            )
+            )
```

### Comparing `relative-addons-system-2.4.4/RelativeAddonsSystem/libraries.py` & `relative-addons-system-2.5.0/RelativeAddonsSystem/libraries.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 from pathlib import Path
 import subprocess
 from contextvars import ContextVar
 
-from RelativeAddonsSystem import utils
+from . import utils
 
 
 pip_executable = Path(sys.executable).parent / "pip"
 
 installed_libraries = ContextVar("installed_libraries", default={})
 
 
@@ -35,21 +35,21 @@
 
 def install_libraries(libraries: list[dict[str, str]]) -> list[str]:
     names = []
     for requirement in libraries:
         if requirement["name"].lower() not in installed_libraries.get():
             name = requirement["name"].lower()
             if "version" in requirement and not requirement["version"] == "*":
-                name += "==" + utils.version_tranform.to_library_version(requirement["version"])
+                name += "==" + utils.version_transform.to_library_version(requirement["version"])
             names.append(name)
 
         elif not utils.check_version(requirement["version"], installed_libraries.get()[requirement["name"].lower()]):
             name = requirement["name"].lower()
             if "version" in requirement and not requirement["version"] == "*":
-                name += "==" + utils.version_tranform.to_library_version(requirement["version"])
+                name += "==" + utils.version_transform.to_library_version(requirement["version"])
 
             names.append(name)
 
     if len(names):
         out = subprocess.getoutput(
             str(pip_executable.absolute()) + " install " + " ".join(names)
         )
```

### Comparing `relative-addons-system-2.4.4/RelativeAddonsSystem/system.py` & `relative-addons-system-2.5.0/RelativeAddonsSystem/system.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 import shutil
 from pathlib import Path
 import os
 import json
 import warnings
 
-from . import libraries
+from . import libraries, utils
 from .addon import Addon
 
 
 class RelativeAddonsSystem:
-
-    def __init__(self, addons_directory: str | Path, auto_install_requirements: bool = False):
+    def __init__(
+        self,
+        addons_directory: str | Path,
+        auto_install_requirements: bool = False,
+        cache_path: str | Path = Path(".ras-cache.json")
+    ):
         self.addon_with_requirements_problem = []
-        self.already_checked_addons = []
         self.pip_libraries = []
 
         if not isinstance(addons_directory, Path):
             addons_directory = Path(addons_directory)
 
         if not addons_directory.exists():
             addons_directory.mkdir(parents=True)
 
         if addons_directory.is_file():
             raise ValueError("Addons directory cannot be a file")
 
         self._directory = addons_directory
 
+        utils.RelativeAddonsSystemCache(cache_path)
+
         self.auto_install_requirements = auto_install_requirements
 
+        libraries.get_installed_libraries()
+
     @property
     def directory(self):
         """
         **Path to addons directory**
 
         :return: pathlib.Path
         """
@@ -48,60 +55,57 @@
             return name
         elif not isinstance(name, str):
             raise ValueError("Expected str, but got {}".format(name.__class__.__name__))
 
         addons_list = list(
             filter(
                 lambda filename: (self.directory / filename).is_dir(),
-                os.listdir(self.directory)
+                os.listdir(str(self.directory)),
             )
         )
 
         for addon_dir_name in addons_list:
-            addon_dir_name: str
             addon_path = self.directory / addon_dir_name
             addon_dir_list = os.listdir(addon_path)
 
-            if "__init__.py" not in addon_dir_list and "addon.json" not in addon_dir_list:
+            if (
+                "__init__.py" not in addon_dir_list
+                and "addon.json" not in addon_dir_list
+            ):
                 continue
 
             with open(addon_path / "addon.json", encoding="utf8") as f:
                 addon_info = json.load(f)
 
             if addon_info["name"] == name:
                 return Addon(path=addon_path, meta_path=addon_path / "addon.json")
 
-    def check_addon_requirements(
-            self,
-            name: str | Addon,
-            alert: bool = False
-    ) -> bool:
+    def check_addon_requirements(self, name: str | Addon, alert: bool = False) -> bool:
         """
         **Automatically checks the requirements of addon**
 
-        :param name: name of addon. You can pass here the addon name or its "object"(dictionary {path: ..., info: ...})
+        :param name: name of addon. You can pass here the addon name or RelativeAddonsSystem.Addon
         :param alert: bool. Alert if problem
         :return: bool. True if addon requirements is satisfied
         """
 
         addon = self.get_addon_by_name(name)
 
         if not addon:
             return False
 
-        if addon.meta["name"] in self.already_checked_addons:
-            return True
+        result = addon.check_requirements(alert=alert)
 
-        return addon.check_requirements(alert=alert)
+        return result
 
     def install_addon_requirements(self, name: str | Addon) -> list[str]:
         """
         **Automatic installation of addon requirements if required**
 
-        :param name: name of addon. You can pass here addon name or its "object"(dictionary {path: ..., info: ...})
+        :param name: name of addon. You can pass here addon name or RelativeAddonsSystem.Addon
         :return: list of installed libraries
         """
 
         addon = self.get_addon_by_name(name)
 
         if addon is None:
             raise ValueError("Cannot find this addon.")
@@ -115,15 +119,15 @@
         :param status: str, optional. Filter addons by its status.
         :return: list of addons RelativeAddonsSystem.Addon
         """
 
         addons_list = list(
             filter(
                 lambda filename: (self.directory / filename).is_dir(),
-                os.listdir(self.directory)
+                os.listdir(self.directory),
             )
         )
 
         addons = []
 
         for addon_name in addons_list:
             addon_name: str
@@ -134,22 +138,23 @@
             if "__init__.py" not in addon_files or "addon.json" not in addon_files:
                 continue
 
             with open(addon_path / "addon.json", encoding="utf8") as f:
                 addon_meta = json.load(f)
 
             if (
-                    "name" not in addon_meta
-                    or "description" not in addon_meta
-                    or "version" not in addon_meta
-                    or "author" not in addon_meta
+                "name" not in addon_meta
+                or "description" not in addon_meta
+                or "version" not in addon_meta
+                or "author" not in addon_meta
             ):
                 warnings.warn(
                     "addon [{}] does not have required fields: name/description/version/author".format(
-                        addon_path.absolute())
+                        addon_path.absolute()
+                    )
                 )
                 continue
             addon = Addon(path=addon_path, meta_path=addon_path / "addon.json")
 
             if "status" not in addon.meta:
                 addon.meta["status"] = "disabled"
                 addon.meta.save()
@@ -159,24 +164,20 @@
                     continue
 
             if "requirements" not in addon.meta:
                 addon.meta["requirements"] = []
                 addon.meta.save()
 
             if self.auto_install_requirements and not self.check_addon_requirements(
-                    addon_meta["name"],
-                    alert=True
+                addon_meta["name"], alert=True
             ):
                 self.install_addon_requirements(addon)
 
             addons.append(addon)
 
-        if self.auto_install_requirements:
-            libraries.get_installed_libraries(force=True)
-
         return addons
 
     def get_enabled_addons(self) -> list[Addon]:
         """
         **Get the enabled addons**
 
         :return: list of the addons objects
@@ -184,127 +185,128 @@
 
         return self.get_all_addons(status="enabled")
 
     def get_disabled_addons(self) -> list[Addon]:
         """
         **Get disabled addons**
 
-        :return: list of addons "objects"(dictionary {path: ..., info: ...})
+        :return: list of addons RelativeAddonsSystem.Addon
         """
 
         return self.get_all_addons(status="disabled")
 
     def get_enabled_addons_as_python_modules(self) -> list[Addon]:
         """
         **Get enabled addons as python modules**
 
-        :return: list of addons "objects"(dictionary {path: ..., info: ..., module: ...})
+        :return: list of addons RelativeAddonsSystem.Addon
         """
         enabled_addons = self.get_enabled_addons()
 
         addons = []
 
         for addon in enabled_addons:
             if addon.meta["name"] in self.addon_with_requirements_problem:
                 continue
 
             addon.get_module()
 
-            addons.append(
-                addon
-            )
+            addons.append(addon)
 
         return addons
 
     def get_disabled_addons_as_python_modules(self) -> list[Addon]:
         """
         **Get disabled addons as python modules**
 
-        :return: list of addons objects
+        :return: list of addons with imported modules
         """
 
         enabled_addons = self.get_disabled_addons()
 
         addons = []
 
         for addon in enabled_addons:
             if addon.meta["name"] in self.addon_with_requirements_problem:
                 continue
 
             addon.get_module()
 
-            addons.append(
-                addon
-            )
+            addons.append(addon)
 
         return addons
 
     def get_addon_as_python_module(self, name: str | Addon) -> Addon:
         """
         **Get addon as python module**
 
-        :param name: pass here the addon name or its object
-        :return: addon object
+        :param name: pass here the addon name or RelativeAddonsSystem.Addon
+        :return: RelativeAddonsSystem.Addon
         """
         addon = self.get_addon_by_name(name)
 
         if not addon:
             raise ValueError("Cannot find this addon")
 
-        if name not in self.already_checked_addons:
-            if name in self.addon_with_requirements_problem or not self.check_addon_requirements(name):
+        if self._cache.addon_updated(addon):
+            if (
+                name in self.addon_with_requirements_problem
+                or not self.check_addon_requirements(name)
+            ):
                 raise ValueError("Requirements of addon not satisfied")
 
         addon.get_module()
 
         return addon
 
     def reload_addon(self, name: str | dict) -> Addon:
         """
         **Re-imports addon**
 
-        :param name: name of addon or its object
-        :return: addon object
+        :param name: name of addon or RelativeAddonsSystem.Addon
+        :return: RelativeAddonsSystem.Addon
         """
         addon = self.get_addon_as_python_module(name)
         addon.reload_module()
 
         if addon.meta["name"] in self.already_checked_addons:
             self.already_checked_addons.remove(addon.meta["name"])
 
         return addon
 
     def enable_addon(self, name: str | Addon) -> Addon:
         """
         **enable addon**
 
-        :param name: name of addon. You can also pass here the object of addon
-        :return: same addon
+        :param name: name of addon. You can also pass here the RelativeAddonsSystem.Addon
+        :return: RelativeAddonsSystem.Addon
         """
         addon = self.get_addon_by_name(name)
 
         if not addon:
-            raise ValueError("Cannot find addon \"{name}\"".format(name=name))
+            raise ValueError('Cannot find addon "{name}"'.format(name=name))
 
         if not self.check_addon_requirements(addon):
-            raise ValueError("Requirements of {name} not satisfied!".format(name=addon.meta["name"]))
+            raise ValueError(
+                "Requirements of {name} not satisfied!".format(name=addon.meta["name"])
+            )
 
         addon.enable()
 
         if addon.meta["name"] in self.already_checked_addons:
             self.already_checked_addons.remove(addon.meta["name"])
 
         return addon
 
     def disable_addon(self, name: str) -> Addon:
         """
         **disable addon**
 
-        :param name: name of addon. You can also pass here the object of addon
-        :return: same addon
+        :param name: name of addon. You can also pass here the RelativeAddonsSystem.Addon
+        :return: RelativeAddonsSystem.Addon
         """
         addon = self.get_addon_by_name(name)
 
         if not addon:
             raise ValueError("Cannot find this addon")
 
         addon.disable()
@@ -314,15 +316,15 @@
 
         return addon
 
     def remove_addon(self, name: str) -> bool:
         """
         **remove addon**
 
-        :param name: name of addon. You can also pass here the addon object
+        :param name: name of addon. You can also pass here the RelativeAddonsSystem.Addon
         :return: bool. True if successfully removed addon
         """
 
         addon = self.get_addon_by_name(name)
 
         if not addon:
             raise ValueError("Cannot find this addon")
@@ -334,15 +336,15 @@
 
         return True
 
     def pack_addon(self, name: str) -> str | None:
         """
         **Make tar-archive from addon(for sharing)**
 
-        :param name: the name of the addon. You can also pass here the addon object
+        :param name: the name of the addon. You can also pass here the RelativeAddonsSystem.Addon
         :return: Path to addon or if it is not found - None
         """
         addon = self.get_addon_by_name(name)
 
         if not addon:
             return
```

### Comparing `relative-addons-system-2.4.4/RelativeAddonsSystem/utils/version_checker.py` & `relative-addons-system-2.5.0/RelativeAddonsSystem/utils/version_checker.py`

 * *Files identical despite different names*

### Comparing `relative-addons-system-2.4.4/pyproject.toml` & `relative-addons-system-2.5.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "relative-addons-system"
-version = "2.4.4"
+version = "2.5.0"
 description = "Easier way to manage your project addons"
 authors = [{ name = "kuyugama(youngtitanium)", email = "kuyugamas@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `relative-addons-system-2.4.4/relative_addons_system.egg-info/SOURCES.txt` & `relative-addons-system-2.5.0/relative_addons_system.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 README.md
 pyproject.toml
 setup.py
 RelativeAddonsSystem/__init__.py
 RelativeAddonsSystem/libraries.py
 RelativeAddonsSystem/system.py
 RelativeAddonsSystem/addon/__init__.py
-RelativeAddonsSystem/addon/configuration.py
 RelativeAddonsSystem/addon/metadata.py
 RelativeAddonsSystem/utils/__init__.py
+RelativeAddonsSystem/utils/cache.py
 RelativeAddonsSystem/utils/recursive_reload_module.py
+RelativeAddonsSystem/utils/storage.py
 RelativeAddonsSystem/utils/version_checker.py
-RelativeAddonsSystem/utils/version_tranform.py
+RelativeAddonsSystem/utils/version_transform.py
 relative_addons_system.egg-info/PKG-INFO
 relative_addons_system.egg-info/SOURCES.txt
 relative_addons_system.egg-info/dependency_links.txt
 relative_addons_system.egg-info/requires.txt
-relative_addons_system.egg-info/top_level.txt
-virtualenv/__init__.py
-virtualenv/lib/__init__.py
+relative_addons_system.egg-info/top_level.txt
```

### Comparing `relative-addons-system-2.4.4/setup.py` & `relative-addons-system-2.5.0/setup.py`

 * *Files identical despite different names*

