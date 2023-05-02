# Comparing `tmp/hiyobot-0.1.4.tar.gz` & `tmp/hiyobot-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hiyobot-0.1.4.tar", last modified: Thu Apr  6 13:24:27 2023, max compression
+gzip compressed data, was "hiyobot-0.1.5.tar", last modified: Tue May  2 06:04:36 2023, max compression
```

## Comparing `hiyobot-0.1.4.tar` & `hiyobot-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:24:27.964928 hiyobot-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-06 13:24:16.000000 hiyobot-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-04-06 13:24:27.964928 hiyobot-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-04-06 13:24:16.000000 hiyobot-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:24:27.964928 hiyobot-0.1.4/hiyobot/
--rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-04-06 13:24:16.000000 hiyobot-0.1.4/hiyobot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:24:27.964928 hiyobot-0.1.4/hiyobot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-04-06 13:24:27.000000 hiyobot-0.1.4/hiyobot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-06 13:24:27.000000 hiyobot-0.1.4/hiyobot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 13:24:27.000000 hiyobot-0.1.4/hiyobot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-06 13:24:27.000000 hiyobot-0.1.4/hiyobot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-06 13:24:27.000000 hiyobot-0.1.4/hiyobot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 13:24:27.964928 hiyobot-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-06 13:24:16.000000 hiyobot-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:04:36.098813 hiyobot-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-02 06:04:23.000000 hiyobot-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-05-02 06:04:36.098813 hiyobot-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-02 06:04:23.000000 hiyobot-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:04:36.098813 hiyobot-0.1.5/hiyobot/
+-rw-r--r--   0 runner    (1001) docker     (123)     7795 2023-05-02 06:04:23.000000 hiyobot-0.1.5/hiyobot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:04:36.098813 hiyobot-0.1.5/hiyobot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-05-02 06:04:36.000000 hiyobot-0.1.5/hiyobot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-02 06:04:36.000000 hiyobot-0.1.5/hiyobot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 06:04:36.000000 hiyobot-0.1.5/hiyobot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-02 06:04:36.000000 hiyobot-0.1.5/hiyobot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 06:04:36.000000 hiyobot-0.1.5/hiyobot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 06:04:36.098813 hiyobot-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-02 06:04:23.000000 hiyobot-0.1.5/setup.py
```

### Comparing `hiyobot-0.1.4/LICENSE` & `hiyobot-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hiyobot-0.1.4/PKG-INFO` & `hiyobot-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiyobot
-Version: 0.1.4
+Version: 0.1.5
 Summary: A simple bot framework for Hack.chat.
 Home-page: https://github.com/Hiyoteam/hiyobot
 Author: MaggieLOL
 Author-email: tanhanzesnd@gmail.com
 License: GPL-2.0
 Keywords: bot hack.chat hack.chat-bot
 Classifier: Development Status :: 3 - Alpha
@@ -12,17 +12,21 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Hiyobot
-一个简单hack.chat机器人框架。
-English document? use [this](https://deepl.com/)
-<img src="https://img.shields.io/badge/Powered%20By-Python-blue.svg"></img> <img src="https://img.shields.io/badge/Powered%20By-websocket_client-blue.svg"></img> <img src="https://img.shields.io/badge/Document%20version-0.0.2-green.svg"></img><img src="https://img.shields.io/pypi/v/hiyobot"></img><img src="https://github.com/Hiyoteam/hiyobot/actions/workflows/python-publish.yml/badge.svg"></img>
+一个简单hack.chat机器人框架。    
+If your native language is not Chinese, please jump [here](https://deepl.com/) .     
+<img src="https://img.shields.io/badge/Powered%20By-Python-blue.svg"></img>     
+<img src="https://img.shields.io/badge/Powered%20By-websocket_client-blue.svg"></img>    
+<img src="https://img.shields.io/badge/Document%20version-0.0.2-green.svg"></img>
+<img src="https://img.shields.io/pypi/v/hiyobot"></img>     
+<img src="https://github.com/Hiyoteam/hiyobot/actions/workflows/python-publish.yml/badge.svg"></img>          
 
 # 如何安装？
 在你的控制台里面输入`pip3 install hiyobot --upgrade`，如果你使用镜像源，可能无法获取到最新的构建，需要加上`-i https://pypi.org/simple`的参数。输出应该是这样的：
 ```
 Collecting hiyobot
   Downloading hiyobot-<version>-py3-none-any.whl (8.3 kB)
 Requirement already satisfied: websocket-client in c:\users\administrator\appdata\local\programs\python\python310\lib\site-packages (from hiyobot) (1.3.2)
```

### Comparing `hiyobot-0.1.4/README.md` & `hiyobot-0.1.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Hiyobot
-一个简单hack.chat机器人框架。
-English document? use [this](https://deepl.com/)
-<img src="https://img.shields.io/badge/Powered%20By-Python-blue.svg"></img> <img src="https://img.shields.io/badge/Powered%20By-websocket_client-blue.svg"></img> <img src="https://img.shields.io/badge/Document%20version-0.0.2-green.svg"></img><img src="https://img.shields.io/pypi/v/hiyobot"></img><img src="https://github.com/Hiyoteam/hiyobot/actions/workflows/python-publish.yml/badge.svg"></img>
+一个简单hack.chat机器人框架。    
+If your native language is not Chinese, please jump [here](https://deepl.com/) .     
+<img src="https://img.shields.io/badge/Powered%20By-Python-blue.svg"></img>     
+<img src="https://img.shields.io/badge/Powered%20By-websocket_client-blue.svg"></img>    
+<img src="https://img.shields.io/badge/Document%20version-0.0.2-green.svg"></img>
+<img src="https://img.shields.io/pypi/v/hiyobot"></img>     
+<img src="https://github.com/Hiyoteam/hiyobot/actions/workflows/python-publish.yml/badge.svg"></img>          
 
 # 如何安装？
 在你的控制台里面输入`pip3 install hiyobot --upgrade`，如果你使用镜像源，可能无法获取到最新的构建，需要加上`-i https://pypi.org/simple`的参数。输出应该是这样的：
 ```
 Collecting hiyobot
   Downloading hiyobot-<version>-py3-none-any.whl (8.3 kB)
 Requirement already satisfied: websocket-client in c:\users\administrator\appdata\local\programs\python\python310\lib\site-packages (from hiyobot) (1.3.2)
```

### Comparing `hiyobot-0.1.4/hiyobot/__init__.py` & `hiyobot-0.1.5/hiyobot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         logging.debug("Ready for include module")
         plugin_name=plugin_name.replace("-","_")
         #import
         plugin=__import__(plugin_name)
         for command in plugin.exports:
             self._bindRaw(command)
         logging.debug(f"Included plugin {plugin_name}")
-    def send(self,data:dict|str):
+    def send(self,data):
         if type(data) == str:
             #auto-detect&convert type
             data=Message.Text(data)
         self.ws.send(json.dumps(data))
         dumped=json.dumps(data)
         if MAX_RECV_LOG_LIMIT != 0:
             if len(dumped) >= MAX_RECV_LOG_LIMIT:
```

### Comparing `hiyobot-0.1.4/hiyobot.egg-info/PKG-INFO` & `hiyobot-0.1.5/hiyobot.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiyobot
-Version: 0.1.4
+Version: 0.1.5
 Summary: A simple bot framework for Hack.chat.
 Home-page: https://github.com/Hiyoteam/hiyobot
 Author: MaggieLOL
 Author-email: tanhanzesnd@gmail.com
 License: GPL-2.0
 Keywords: bot hack.chat hack.chat-bot
 Classifier: Development Status :: 3 - Alpha
@@ -12,17 +12,21 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Hiyobot
-一个简单hack.chat机器人框架。
-English document? use [this](https://deepl.com/)
-<img src="https://img.shields.io/badge/Powered%20By-Python-blue.svg"></img> <img src="https://img.shields.io/badge/Powered%20By-websocket_client-blue.svg"></img> <img src="https://img.shields.io/badge/Document%20version-0.0.2-green.svg"></img><img src="https://img.shields.io/pypi/v/hiyobot"></img><img src="https://github.com/Hiyoteam/hiyobot/actions/workflows/python-publish.yml/badge.svg"></img>
+一个简单hack.chat机器人框架。    
+If your native language is not Chinese, please jump [here](https://deepl.com/) .     
+<img src="https://img.shields.io/badge/Powered%20By-Python-blue.svg"></img>     
+<img src="https://img.shields.io/badge/Powered%20By-websocket_client-blue.svg"></img>    
+<img src="https://img.shields.io/badge/Document%20version-0.0.2-green.svg"></img>
+<img src="https://img.shields.io/pypi/v/hiyobot"></img>     
+<img src="https://github.com/Hiyoteam/hiyobot/actions/workflows/python-publish.yml/badge.svg"></img>          
 
 # 如何安装？
 在你的控制台里面输入`pip3 install hiyobot --upgrade`，如果你使用镜像源，可能无法获取到最新的构建，需要加上`-i https://pypi.org/simple`的参数。输出应该是这样的：
 ```
 Collecting hiyobot
   Downloading hiyobot-<version>-py3-none-any.whl (8.3 kB)
 Requirement already satisfied: websocket-client in c:\users\administrator\appdata\local\programs\python\python310\lib\site-packages (from hiyobot) (1.3.2)
```

### Comparing `hiyobot-0.1.4/setup.py` & `hiyobot-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hiyobot', # 你的项目名称
-    version='0.1.4', # 你的项目版本
+    version='0.1.5', # 你的项目版本
     description='A simple bot framework for Hack.chat.', # 你的项目简介
     long_description=open('README.md').read(), # 你的项目详细介绍，一般从README.md文件中读取
     long_description_content_type='text/markdown', # 你的项目详细介绍的格式，一般为markdown格式
     url='https://github.com/Hiyoteam/hiyobot', # 你的项目主页，一般为github仓库地址
     author='MaggieLOL', # 你的姓名或者团队名称
     author_email='tanhanzesnd@gmail.com', # 你的邮箱或者团队邮箱
     license='GPL-2.0', # 你的项目使用的许可证，一般为MIT或者其他开源许可证
@@ -22,8 +22,8 @@
     install_requires="""cffi==1.15.1
 gevent==22.10.2
 greenlet==2.0.2
 pycparser==2.21
 websocket==0.2.1
 zope.event==4.6
 zope.interface==6.0""".splitlines(),
-)
+)
```

