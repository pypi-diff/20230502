# Comparing `tmp/ablerConfig-0.1.1.tar.gz` & `tmp/ablerConfig-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ablerConfig-0.1.1.tar", last modified: Mon Apr 24 18:12:21 2023, max compression
+gzip compressed data, was "ablerConfig-0.1.2.tar", last modified: Mon May  1 22:01:34 2023, max compression
```

## Comparing `ablerConfig-0.1.1.tar` & `ablerConfig-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 18:12:21.935610 ablerConfig-0.1.1/
--rw-rw-rw-   0        0        0     2025 2023-04-24 18:12:21.934599 ablerConfig-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1257 2023-04-24 18:09:32.000000 ablerConfig-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 18:12:21.923426 ablerConfig-0.1.1/ablerConfig/
--rw-rw-rw-   0        0        0      131 2023-04-24 18:06:40.000000 ablerConfig-0.1.1/ablerConfig/__init__.py
--rw-rw-rw-   0        0        0    12847 2023-04-24 18:06:26.000000 ablerConfig-0.1.1/ablerConfig/config.py
-drwxrwxrwx   0        0        0        0 2023-04-24 18:12:21.932597 ablerConfig-0.1.1/ablerConfig.egg-info/
--rw-rw-rw-   0        0        0     2025 2023-04-24 18:12:21.000000 ablerConfig-0.1.1/ablerConfig.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-04-24 18:12:21.000000 ablerConfig-0.1.1/ablerConfig.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 18:12:21.000000 ablerConfig-0.1.1/ablerConfig.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-24 18:12:21.000000 ablerConfig-0.1.1/ablerConfig.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-24 18:12:21.000000 ablerConfig-0.1.1/ablerConfig.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 18:12:21.935610 ablerConfig-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1044 2023-04-24 18:06:50.000000 ablerConfig-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 22:01:34.201511 ablerConfig-0.1.2/
+-rw-rw-rw-   0        0        0     2025 2023-05-01 22:01:34.201511 ablerConfig-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1257 2023-04-24 18:09:32.000000 ablerConfig-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 22:01:34.201511 ablerConfig-0.1.2/ablerConfig/
+-rw-rw-rw-   0        0        0      103 2023-05-01 21:57:28.000000 ablerConfig-0.1.2/ablerConfig/__init__.py
+-rw-rw-rw-   0        0        0    13162 2023-05-01 21:56:39.000000 ablerConfig-0.1.2/ablerConfig/config.py
+drwxrwxrwx   0        0        0        0 2023-05-01 22:01:34.201511 ablerConfig-0.1.2/ablerConfig.egg-info/
+-rw-rw-rw-   0        0        0     2025 2023-05-01 22:01:34.000000 ablerConfig-0.1.2/ablerConfig.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-05-01 22:01:34.000000 ablerConfig-0.1.2/ablerConfig.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 22:01:34.000000 ablerConfig-0.1.2/ablerConfig.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-01 22:01:34.000000 ablerConfig-0.1.2/ablerConfig.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-01 22:01:34.000000 ablerConfig-0.1.2/ablerConfig.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 22:01:34.201511 ablerConfig-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1044 2023-05-01 21:57:44.000000 ablerConfig-0.1.2/setup.py
```

### Comparing `ablerConfig-0.1.1/PKG-INFO` & `ablerConfig-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ablerConfig
-Version: 0.1.1
+Version: 0.1.2
 Summary: 配置信息处理包
 Home-page: https://github.com/hanlaohan/abler-config
 Author: 憨老汉
 Author-email: hh28642257@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ablerConfig-0.1.1/README.md` & `ablerConfig-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ablerConfig-0.1.1/ablerConfig/config.py` & `ablerConfig-0.1.2/ablerConfig/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 (TOML不支持异质数组， 如 [1, '井眼井深', 0, 'm'])
 """
 from __future__ import annotations
 import os
 import pyjson5 as qjson  # 非常奇怪，不知道怎么格式化输出
 import json5 as json  # 要输出的时候改成这个，比较慢的
 
-DEF_CFG_NAME = ''       # 主程序首次调用 Config() 时设置
-LOCAL_CONF_DIR = ''     # 本地外部配置文件目录名
-CONF_EXT = '.json5'
+# DEF_CFG_NAME = ''       # 主程序首次调用 Config() 时设置
+# LOCAL_CONF_DIR = ''     # 本地外部配置文件目录名
+# CONF_EXT = '.json5'
 
 
 class ConfigError(Exception):
     def __init__(self, conf_name):
         filenames = [Config.conf_file_path(conf_name)]
-        if conf_name != DEF_CFG_NAME:
-            filenames.append(Config.conf_file_path(DEF_CFG_NAME))
+        if conf_name != Config.DEF_CFG_NAME:
+            filenames.append(Config.conf_file_path(Config.DEF_CFG_NAME))
         super().__init__('不存在任何配置文件', filenames)
 
 
 class ConfigNode(dict):
     # done：增加parent属性，自动从parent.default获取参数
     __old_setattr__ = object.__setattr__
 
@@ -130,48 +130,53 @@
             if _parent is None:
                 break
         if _parent is not None:
             setattr(_parent, names[i + 1], value)
 
 
 class Config:
+    CONF_DIR = 'config'
+    CONF_EXT = '.json5'
+    DEF_CFG_NAME = ''  # 主程序首次调用 Config() 时设置
+    LOCAL_CONF_DIR = ''  # 本地外部配置文件目录名
+
     main: Config = None
     root: ConfigNode = None
     """
     第一个创建的实例将作为系统的主配置对象
     """
 
     def __init__(self, conf_name=None, default='', local_dir='', show_message=print):
         if Config.main is None:
             Config.main = self
         self.root: ConfigNode = None
-        global DEF_CFG_NAME, LOCAL_CONF_DIR
-        self.conf_name = conf_name or default or DEF_CFG_NAME
-        if default != '' and DEF_CFG_NAME == '':
-            DEF_CFG_NAME = default
-        if DEF_CFG_NAME == '':
+        # global DEF_CFG_NAME, LOCAL_CONF_DIR
+        self.conf_name = conf_name or default or Config.DEF_CFG_NAME
+        if default != '' and Config.DEF_CFG_NAME == '':
+            Config.DEF_CFG_NAME = default
+        if Config.DEF_CFG_NAME == '':
             raise Exception('编码错误：首次调用Config()必须指定default=?')
-        if local_dir != '' and LOCAL_CONF_DIR == '':
-            LOCAL_CONF_DIR = local_dir
-        if LOCAL_CONF_DIR == '':
+        if local_dir != '' and Config.LOCAL_CONF_DIR == '':
+            Config.LOCAL_CONF_DIR = local_dir
+        if Config.LOCAL_CONF_DIR == '':
             raise Exception('编码错误：首次调用Config()必须指定local_dir=?')
 
         # self.default = self.open_conf_file(default, local=False)
         # self.root = self.open_conf_file(self.conf_name, local=True)
         # self._root = ConfigNode({'local': self.root, 'default': self.default})
         # self.root = self._root.local
         # self.default = self._root.default
 
         inner = self.open_conf_file(default, local=False)
-        if self.conf_name == DEF_CFG_NAME:
+        if self.conf_name == Config.DEF_CFG_NAME:
             self.root = inner
             if Config.root is None:
                 Config.root = self.root
         local = self.open_conf_file(self.conf_name, local=True, show_message=show_message)
-        if self.conf_name != DEF_CFG_NAME:
+        if self.conf_name != Config.DEF_CFG_NAME:
             self.default = inner
             self.root = local
             self.root.assign_default(self.default)
 
     def get_value(self, path):
         result = None
         if self.root is not None:
@@ -199,39 +204,39 @@
         result = self.get_value(path)
         # return ConfigNode(result)
         return result
 
     @staticmethod
     def conf_path(sub_name=None, local=False):
         if local:
-            path = os.path.abspath(os.path.join(os.getcwd(), '..', LOCAL_CONF_DIR))
+            path = os.path.abspath(os.path.join(os.getcwd(), '..', Config.LOCAL_CONF_DIR))
         else:
-            path = os.path.join(os.getcwd(), 'config')
+            path = os.path.join(os.getcwd(), Config.CONF_DIR)
         if sub_name is not None:
             path = os.path.join(path, sub_name)
         return path
 
     @staticmethod
     def conf_file_path(conf_name, local=False):
-        return Config.conf_path(sub_name=f"{conf_name}{CONF_EXT}", local=local)
+        return Config.conf_path(sub_name=f"{conf_name}{Config.CONF_EXT}", local=local)
 
     @classmethod
     def open_conf_file(cls, conf_name, local=False, show_message=print):
         conf_file = cls.conf_file_path(conf_name, local)
-        if local and (conf_name == DEF_CFG_NAME):
+        if local and (conf_name == Config.DEF_CFG_NAME):
             # 检查本地配置文件
             return cls.check_local_config(cls.root, show_message=show_message)
         return cls.load_from(conf_file)
 
     @classmethod
     def check_local_config(cls, root: ConfigNode, show_message=print):
         # default = cls.main.default
         # default_ver = default.get('cfg_version')
-        # default_file = cls.conf_file_path(DEF_CFG_NAME, local=False)
-        local_file = cls.conf_file_path(DEF_CFG_NAME, local=True)
+        # default_file = cls.conf_file_path(Config.DEF_CFG_NAME, local=False)
+        local_file = cls.conf_file_path(Config.DEF_CFG_NAME, local=True)
         _dir = os.path.dirname(local_file)
         if not os.path.exists(_dir):
             os.makedirs(_dir)
         # if not os.path.exists(local_file):
         #     _dir = os.path.dirname(local_file)
         #     if not os.path.exists(_dir):
         #         os.makedirs(_dir)
@@ -272,15 +277,15 @@
         if local_ver >= '1.4':
             root.assign_local(local)
         show_message('系统配置已更新，请进入系统后，尽快打开配置界面，检查各项设置')
 
     @classmethod
     def create_local_config(cls, root: ConfigNode, values: dict = None):
         local = root.take_local_settings(values)
-        cls.save_to_file(local, DEF_CFG_NAME, local=True)
+        cls.save_to_file(local, Config.DEF_CFG_NAME, local=True)
         return local
 
     @classmethod
     def object_of(cls, path):
         return cls.main.get_object(path)
 
     @classmethod
```

### Comparing `ablerConfig-0.1.1/ablerConfig.egg-info/PKG-INFO` & `ablerConfig-0.1.2/ablerConfig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ablerConfig
-Version: 0.1.1
+Version: 0.1.2
 Summary: 配置信息处理包
 Home-page: https://github.com/hanlaohan/abler-config
 Author: 憨老汉
 Author-email: hh28642257@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ablerConfig-0.1.1/setup.py` & `ablerConfig-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="ablerConfig",
-    version="0.1.1",
+    version="0.1.2",
     author="憨老汉",
     author_email="hh28642257@gmail.com",
     description="配置信息处理包",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hanlaohan/abler-config",
     packages=find_packages(),
```

