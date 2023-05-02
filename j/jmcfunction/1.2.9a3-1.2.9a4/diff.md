# Comparing `tmp/jmcfunction-1.2.9a3.tar.gz` & `tmp/jmcfunction-1.2.9a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jmcfunction-1.2.9a3.tar", last modified: Tue Dec 20 05:29:52 2022, max compression
+gzip compressed data, was "jmcfunction-1.2.9a4.tar", last modified: Tue Dec 20 06:30:08 2022, max compression
```

## Comparing `jmcfunction-1.2.9a3.tar` & `jmcfunction-1.2.9a4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2022-12-20 05:29:52.512772 jmcfunction-1.2.9a3/
--rw-rw-rw-   0        0        0     2965 2022-12-20 05:29:52.506039 jmcfunction-1.2.9a3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-12-20 05:29:52.379971 jmcfunction-1.2.9a3/jmc/
--rw-rw-rw-   0        0        0     1172 2022-12-16 12:22:17.000000 jmcfunction-1.2.9a3/jmc/__init__.py
--rw-rw-rw-   0        0        0      834 2022-12-19 17:32:21.000000 jmcfunction-1.2.9a3/jmc/__main__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 05:29:52.425923 jmcfunction-1.2.9a3/jmc/compile/
--rw-rw-rw-   0        0        0      416 2022-11-30 12:06:26.000000 jmcfunction-1.2.9a3/jmc/compile/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-20 05:29:52.448935 jmcfunction-1.2.9a3/jmc/compile/command/
--rw-rw-rw-   0        0        0      242 2022-10-30 18:03:58.000000 jmcfunction-1.2.9a3/jmc/compile/command/__init__.py
--rw-rw-rw-   0        0        0    14930 2022-12-19 11:57:47.000000 jmcfunction-1.2.9a3/jmc/compile/command/_flow_control.py
-drwxrwxrwx   0        0        0        0 2022-12-20 05:29:52.475941 jmcfunction-1.2.9a3/jmc/compile/command/builtin_function/
--rw-rw-rw-   0        0        0      168 2022-10-30 18:03:58.000000 jmcfunction-1.2.9a3/jmc/compile/command/builtin_function/__init__.py
--rw-rw-rw-   0        0        0     5844 2022-11-24 03:20:23.000000 jmcfunction-1.2.9a3/jmc/compile/command/builtin_function/_var_operation.py
--rw-rw-rw-   0        0        0     1668 2022-12-16 05:00:12.000000 jmcfunction-1.2.9a3/jmc/compile/command/builtin_function/bool_function.py
--rw-rw-rw-   0        0        0    14590 2022-11-30 12:56:54.000000 jmcfunction-1.2.9a3/jmc/compile/command/builtin_function/execute_excluded.py
--rw-rw-rw-   0        0        0    16136 2022-12-17 11:03:52.000000 jmcfunction-1.2.9a3/jmc/compile/command/builtin_function/jmc_command.py
--rw-rw-rw-   0        0        0     3321 2022-11-09 16:09:58.000000 jmcfunction-1.2.9a3/jmc/compile/command/builtin_function/load_once.py
--rw-rw-rw-   0        0        0    24023 2022-12-17 14:19:36.000000 jmcfunction-1.2.9a3/jmc/compile/command/builtin_function/load_only.py
--rw-rw-rw-   0        0        0    17301 2022-12-19 15:32:36.000000 jmcfunction-1.2.9a3/jmc/compile/command/condition.py
--rw-rw-rw-   0        0        0      462 2022-10-30 18:03:58.000000 jmcfunction-1.2.9a3/jmc/compile/command/flow_control.py
--rw-rw-rw-   0        0        0    13701 2022-12-15 10:15:07.000000 jmcfunction-1.2.9a3/jmc/compile/command/jmc_function.py
--rw-rw-rw-   0        0        0    21241 2022-12-17 14:16:28.000000 jmcfunction-1.2.9a3/jmc/compile/command/utils.py
--rw-rw-rw-   0        0        0     6497 2022-12-19 15:32:41.000000 jmcfunction-1.2.9a3/jmc/compile/command/var_operation.py
--rw-rw-rw-   0        0        0    11885 2022-12-15 11:08:41.000000 jmcfunction-1.2.9a3/jmc/compile/compiling.py
--rw-rw-rw-   0        0        0    16726 2022-12-19 17:50:59.000000 jmcfunction-1.2.9a3/jmc/compile/datapack.py
--rw-rw-rw-   0        0        0     1343 2022-12-15 10:28:36.000000 jmcfunction-1.2.9a3/jmc/compile/datapack_data.py
--rw-rw-rw-   0        0        0     7603 2022-12-11 14:21:29.000000 jmcfunction-1.2.9a3/jmc/compile/exception.py
--rw-rw-rw-   0        0        0     2576 2022-12-19 16:41:39.000000 jmcfunction-1.2.9a3/jmc/compile/header.py
--rw-rw-rw-   0        0        0    11148 2022-12-19 17:28:39.000000 jmcfunction-1.2.9a3/jmc/compile/header_parse.py
--rw-rw-rw-   0        0        0    25607 2022-12-19 17:52:55.000000 jmcfunction-1.2.9a3/jmc/compile/lexer.py
--rw-rw-rw-   0        0        0    20680 2022-12-19 16:23:25.000000 jmcfunction-1.2.9a3/jmc/compile/lexer_func_content.py
--rw-rw-rw-   0        0        0     1026 2022-11-30 12:26:09.000000 jmcfunction-1.2.9a3/jmc/compile/log.py
--rw-rw-rw-   0        0        0     3425 2022-11-30 12:35:12.000000 jmcfunction-1.2.9a3/jmc/compile/test_compile.py
--rw-rw-rw-   0        0        0    39678 2022-12-19 17:50:58.000000 jmcfunction-1.2.9a3/jmc/compile/tokenizer.py
--rw-rw-rw-   0        0        0     7508 2022-12-19 16:22:35.000000 jmcfunction-1.2.9a3/jmc/compile/utils.py
--rw-rw-rw-   0        0        0     1375 2022-11-30 12:37:56.000000 jmcfunction-1.2.9a3/jmc/compile/vanilla_command.py
-drwxrwxrwx   0        0        0        0 2022-12-20 05:29:52.488945 jmcfunction-1.2.9a3/jmc/terminal/
--rw-rw-rw-   0        0        0      145 2022-11-04 14:49:47.000000 jmcfunction-1.2.9a3/jmc/terminal/__init__.py
--rw-rw-rw-   0        0        0    10129 2022-12-19 07:07:46.000000 jmcfunction-1.2.9a3/jmc/terminal/configuration.py
--rw-rw-rw-   0        0        0     1575 2022-12-15 08:48:10.000000 jmcfunction-1.2.9a3/jmc/terminal/main.py
--rw-rw-rw-   0        0        0     2382 2022-11-09 11:39:19.000000 jmcfunction-1.2.9a3/jmc/terminal/utils.py
--rw-rw-rw-   0        0        0     7172 2022-12-18 05:13:32.000000 jmcfunction-1.2.9a3/jmc/terminal_commands.py
-drwxrwxrwx   0        0        0        0 2022-12-20 05:29:52.505039 jmcfunction-1.2.9a3/jmcfunction.egg-info/
--rw-rw-rw-   0        0        0     2965 2022-12-20 05:29:52.000000 jmcfunction-1.2.9a3/jmcfunction.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1304 2022-12-20 05:29:52.000000 jmcfunction-1.2.9a3/jmcfunction.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-20 05:29:52.000000 jmcfunction-1.2.9a3/jmcfunction.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2022-12-20 05:29:52.000000 jmcfunction-1.2.9a3/jmcfunction.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        4 2022-12-20 05:29:52.000000 jmcfunction-1.2.9a3/jmcfunction.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-20 05:29:52.512772 jmcfunction-1.2.9a3/setup.cfg
--rw-rw-rw-   0        0        0     1712 2022-12-16 12:22:30.000000 jmcfunction-1.2.9a3/setup.py
+drwxrwxrwx   0        0        0        0 2022-12-20 06:30:08.477490 jmcfunction-1.2.9a4/
+-rw-rw-rw-   0        0        0     2965 2022-12-20 06:30:08.471489 jmcfunction-1.2.9a4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2022-12-20 06:30:08.313622 jmcfunction-1.2.9a4/jmc/
+-rw-rw-rw-   0        0        0     1172 2022-12-16 12:22:17.000000 jmcfunction-1.2.9a4/jmc/__init__.py
+-rw-rw-rw-   0        0        0      834 2022-12-20 06:29:47.000000 jmcfunction-1.2.9a4/jmc/__main__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 06:30:08.377938 jmcfunction-1.2.9a4/jmc/compile/
+-rw-rw-rw-   0        0        0      416 2022-11-30 12:06:26.000000 jmcfunction-1.2.9a4/jmc/compile/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-20 06:30:08.402944 jmcfunction-1.2.9a4/jmc/compile/command/
+-rw-rw-rw-   0        0        0      242 2022-10-30 18:03:58.000000 jmcfunction-1.2.9a4/jmc/compile/command/__init__.py
+-rw-rw-rw-   0        0        0    14930 2022-12-19 11:57:47.000000 jmcfunction-1.2.9a4/jmc/compile/command/_flow_control.py
+drwxrwxrwx   0        0        0        0 2022-12-20 06:30:08.435703 jmcfunction-1.2.9a4/jmc/compile/command/builtin_function/
+-rw-rw-rw-   0        0        0      168 2022-10-30 18:03:58.000000 jmcfunction-1.2.9a4/jmc/compile/command/builtin_function/__init__.py
+-rw-rw-rw-   0        0        0     5844 2022-11-24 03:20:23.000000 jmcfunction-1.2.9a4/jmc/compile/command/builtin_function/_var_operation.py
+-rw-rw-rw-   0        0        0     1668 2022-12-16 05:00:12.000000 jmcfunction-1.2.9a4/jmc/compile/command/builtin_function/bool_function.py
+-rw-rw-rw-   0        0        0    14590 2022-11-30 12:56:54.000000 jmcfunction-1.2.9a4/jmc/compile/command/builtin_function/execute_excluded.py
+-rw-rw-rw-   0        0        0    16136 2022-12-17 11:03:52.000000 jmcfunction-1.2.9a4/jmc/compile/command/builtin_function/jmc_command.py
+-rw-rw-rw-   0        0        0     3321 2022-11-09 16:09:58.000000 jmcfunction-1.2.9a4/jmc/compile/command/builtin_function/load_once.py
+-rw-rw-rw-   0        0        0    24023 2022-12-17 14:19:36.000000 jmcfunction-1.2.9a4/jmc/compile/command/builtin_function/load_only.py
+-rw-rw-rw-   0        0        0    17301 2022-12-19 15:32:36.000000 jmcfunction-1.2.9a4/jmc/compile/command/condition.py
+-rw-rw-rw-   0        0        0      462 2022-10-30 18:03:58.000000 jmcfunction-1.2.9a4/jmc/compile/command/flow_control.py
+-rw-rw-rw-   0        0        0    13701 2022-12-15 10:15:07.000000 jmcfunction-1.2.9a4/jmc/compile/command/jmc_function.py
+-rw-rw-rw-   0        0        0    21241 2022-12-17 14:16:28.000000 jmcfunction-1.2.9a4/jmc/compile/command/utils.py
+-rw-rw-rw-   0        0        0     6497 2022-12-19 15:32:41.000000 jmcfunction-1.2.9a4/jmc/compile/command/var_operation.py
+-rw-rw-rw-   0        0        0    11885 2022-12-15 11:08:41.000000 jmcfunction-1.2.9a4/jmc/compile/compiling.py
+-rw-rw-rw-   0        0        0    16726 2022-12-19 17:50:59.000000 jmcfunction-1.2.9a4/jmc/compile/datapack.py
+-rw-rw-rw-   0        0        0     1343 2022-12-15 10:28:36.000000 jmcfunction-1.2.9a4/jmc/compile/datapack_data.py
+-rw-rw-rw-   0        0        0     7603 2022-12-11 14:21:29.000000 jmcfunction-1.2.9a4/jmc/compile/exception.py
+-rw-rw-rw-   0        0        0     2576 2022-12-19 16:41:39.000000 jmcfunction-1.2.9a4/jmc/compile/header.py
+-rw-rw-rw-   0        0        0    11148 2022-12-19 17:28:39.000000 jmcfunction-1.2.9a4/jmc/compile/header_parse.py
+-rw-rw-rw-   0        0        0    25693 2022-12-20 06:28:22.000000 jmcfunction-1.2.9a4/jmc/compile/lexer.py
+-rw-rw-rw-   0        0        0    20680 2022-12-19 16:23:25.000000 jmcfunction-1.2.9a4/jmc/compile/lexer_func_content.py
+-rw-rw-rw-   0        0        0     1026 2022-11-30 12:26:09.000000 jmcfunction-1.2.9a4/jmc/compile/log.py
+-rw-rw-rw-   0        0        0     3425 2022-11-30 12:35:12.000000 jmcfunction-1.2.9a4/jmc/compile/test_compile.py
+-rw-rw-rw-   0        0        0    39678 2022-12-19 17:50:58.000000 jmcfunction-1.2.9a4/jmc/compile/tokenizer.py
+-rw-rw-rw-   0        0        0     7508 2022-12-19 16:22:35.000000 jmcfunction-1.2.9a4/jmc/compile/utils.py
+-rw-rw-rw-   0        0        0     1375 2022-11-30 12:37:56.000000 jmcfunction-1.2.9a4/jmc/compile/vanilla_command.py
+drwxrwxrwx   0        0        0        0 2022-12-20 06:30:08.452438 jmcfunction-1.2.9a4/jmc/terminal/
+-rw-rw-rw-   0        0        0      145 2022-11-04 14:49:47.000000 jmcfunction-1.2.9a4/jmc/terminal/__init__.py
+-rw-rw-rw-   0        0        0    10129 2022-12-19 07:07:46.000000 jmcfunction-1.2.9a4/jmc/terminal/configuration.py
+-rw-rw-rw-   0        0        0     1575 2022-12-15 08:48:10.000000 jmcfunction-1.2.9a4/jmc/terminal/main.py
+-rw-rw-rw-   0        0        0     2382 2022-11-09 11:39:19.000000 jmcfunction-1.2.9a4/jmc/terminal/utils.py
+-rw-rw-rw-   0        0        0     7172 2022-12-18 05:13:32.000000 jmcfunction-1.2.9a4/jmc/terminal_commands.py
+drwxrwxrwx   0        0        0        0 2022-12-20 06:30:08.469488 jmcfunction-1.2.9a4/jmcfunction.egg-info/
+-rw-rw-rw-   0        0        0     2965 2022-12-20 06:30:08.000000 jmcfunction-1.2.9a4/jmcfunction.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1304 2022-12-20 06:30:08.000000 jmcfunction-1.2.9a4/jmcfunction.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-12-20 06:30:08.000000 jmcfunction-1.2.9a4/jmcfunction.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2022-12-20 06:30:08.000000 jmcfunction-1.2.9a4/jmcfunction.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        4 2022-12-20 06:30:08.000000 jmcfunction-1.2.9a4/jmcfunction.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-12-20 06:30:08.478490 jmcfunction-1.2.9a4/setup.cfg
+-rw-rw-rw-   0        0        0     1712 2022-12-16 12:22:30.000000 jmcfunction-1.2.9a4/setup.py
```

### Comparing `jmcfunction-1.2.9a3/PKG-INFO` & `jmcfunction-1.2.9a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcfunction
-Version: 1.2.9a3
+Version: 1.2.9a4
 Summary: Compiler for JMC (JavaScript-like Minecraft Function), a mcfunction extension language for making Minecraft Datapack.
 Author: WingedSeal
 Author-email: firm09719@gmail.com
 License: MIT License
 Project-URL: Documentation, https://wingedseal.github.io/jmc/
 Project-URL: Repository, https://github.com/WingedSeal/jmc
 Keywords: python,minecraft,mcfunction,datapack,compiler
@@ -16,15 +16,15 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 
-# JMC &middot; [![license-mit](https://badgen.net/badge/license/MIT/blue/)](https://github.com/WingedSeal/jmc/blob/main/LICENSE) [![release](https://badgen.net/badge/release/v1.2.9-alpha.3/blue/)](https://github.com/WingedSeal/jmc/releases/latest) [![build-passing](https://badgen.net/badge/build/passing/green/)](https://wingedseal.github.io/jmc/#/) [![discord-invite](https://badgen.net/badge/discord/Official-Server/blue/?icon=discord)](https://discord.gg/PNWKpwdzD3)
+# JMC &middot; [![license-mit](https://badgen.net/badge/license/MIT/blue/)](https://github.com/WingedSeal/jmc/blob/main/LICENSE) [![release](https://badgen.net/badge/release/v1.2.9-alpha.4/blue/)](https://github.com/WingedSeal/jmc/releases/latest) [![build-passing](https://badgen.net/badge/build/passing/green/)](https://wingedseal.github.io/jmc/#/) [![discord-invite](https://badgen.net/badge/discord/Official-Server/blue/?icon=discord)](https://discord.gg/PNWKpwdzD3)
 
 ## (JavaScript-like Minecraft Function)
 
 JMC (JavaScript-like Minecraft Function) is a mcfunction extension language for making Minecraft Datapack.
 
 ![JMC-icon](https://github.com/WingedSeal/jmc/blob/webpage/src/assets/image/jmc_icon192.png?raw=true)
```

### Comparing `jmcfunction-1.2.9a3/jmc/__init__.py` & `jmcfunction-1.2.9a4/jmc/__init__.py`

 * *Files identical despite different names*

### Comparing `jmcfunction-1.2.9a3/jmc/__main__.py` & `jmcfunction-1.2.9a4/jmc/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Main module"""
 import atexit
 from .compile import Logger
 from .terminal.utils import RestartException, handle_exception
 from .terminal import GlobalData, Colors, start
 
-VERSION = 'v1.2.9-alpha.3'
+VERSION = 'v1.2.9-alpha.4'
 CONFIG_FILE_NAME = 'jmc_config.json'
 GlobalData().init(VERSION, CONFIG_FILE_NAME)
 
 from . import terminal_commands  # noqa
 
 logger = Logger(__name__)
```

### Comparing `jmcfunction-1.2.9a3/jmc/compile/command/_flow_control.py` & `jmcfunction-1.2.9a4/jmc/compile/command/_flow_control.py`

 * *Files identical despite different names*

### Comparing `jmcfunction-1.2.9a3/jmc/compile/command/builtin_function/_var_operation.py` & `jmcfunction-1.2.9a4/jmc/compile/command/builtin_function/_var_operation.py`

 * *Files identical despite different names*

### Comparing `jmcfunction-1.2.9a3/jmc/compile/command/builtin_function/bool_function.py` & `jmcfunction-1.2.9a4/jmc/compile/command/builtin_function/bool_function.py`

 * *Files identical despite different names*

### Comparing `jmcfunction-1.2.9a3/jmc/compile/command/builtin_function/execute_excluded.py` & `jmcfunction-1.2.9a4/jmc/compile/command/builtin_function/execute_excluded.py`

 * *Files identical despite different names*

### Comparing `jmcfunction-1.2.9a3/jmc/compile/command/builtin_function/jmc_command.py` & `jmcfunction-1.2.9a4/jmc/compile/command/builtin_function/jmc_command.py`

 * *Files identical despite different names*

### Comparing `jmcfunction-1.2.9a3/jmc/compile/command/builtin_function/load_once.py` & `jmcfunction-1.2.9a4/jmc/compile/command/builtin_function/load_once.py`

 * *Files identical despite different names*

### Comparing `jmcfunction-1.2.9a3/jmc/compile/command/builtin_function/load_only.py` & `jmcfunction-1.2.9a4/jmc/compile/command/builtin_function/load_only.py`

 * *Files identical despite different names*

### Comparing `jmcfunction-1.2.9a3/jmc/compile/command/condition.py` & `jmcfunction-1.2.9a4/jmc/compile/command/condition.py`

 * *Files identical despite different names*

### Comparing `jmcfunction-1.2.9a3/jmc/compile/command/jmc_function.py` & `jmcfunction-1.2.9a4/jmc/compile/command/jmc_function.py`

 * *Files identical despite different names*

### Comparing `jmcfunction-1.2.9a3/jmc/compile/command/utils.py` & `jmcfunction-1.2.9a4/jmc/compile/command/utils.py`

 * *Files identical despite different names*

### Comparing `jmcfunction-1.2.9a3/jmc/compile/command/var_operation.py` & `jmcfunction-1.2.9a4/jmc/compile/command/var_operation.py`

 * *Files identical despite different names*

### Comparing `jmcfunction-1.2.9a3/jmc/compile/compiling.py` & `jmcfunction-1.2.9a4/jmc/compile/compiling.py`

 * *Files identical despite different names*

### Comparing `jmcfunction-1.2.9a3/jmc/compile/datapack.py` & `jmcfunction-1.2.9a4/jmc/compile/datapack.py`

 * *Files identical despite different names*

### Comparing `jmcfunction-1.2.9a3/jmc/compile/datapack_data.py` & `jmcfunction-1.2.9a4/jmc/compile/datapack_data.py`

 * *Files identical despite different names*

### Comparing `jmcfunction-1.2.9a3/jmc/compile/exception.py` & `jmcfunction-1.2.9a4/jmc/compile/exception.py`

 * *Files identical despite different names*

### Comparing `jmcfunction-1.2.9a3/jmc/compile/header.py` & `jmcfunction-1.2.9a4/jmc/compile/header.py`

 * *Files identical despite different names*

### Comparing `jmcfunction-1.2.9a3/jmc/compile/header_parse.py` & `jmcfunction-1.2.9a4/jmc/compile/header_parse.py`

 * *Files identical despite different names*

### Comparing `jmcfunction-1.2.9a3/jmc/compile/lexer.py` & `jmcfunction-1.2.9a4/jmc/compile/lexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,26 +99,28 @@
             raw_string = _test_file
         tokenizer = Tokenizer(raw_string, file_path_str)
         if is_load:
             self.load_tokenizer = tokenizer
 
         for command in tokenizer.programs:
             if command[0].string == 'function' and len(command) == 4:
-                self.parse_func(tokenizer, command, file_path_str)
                 self.parse_current_load()
+                self.parse_func(tokenizer, command, file_path_str)
             elif command[0].string == 'function' and len(command) != 2:
                 raise JMCSyntaxException(
                     f"'function' expect 1(Minecraft syntax) or 3(JMC syntax) arguments (got {len(command)-1})",
                     command[0],
                     tokenizer, suggestion="Probably caused by missing function body ('{')")
             elif command[0].string == 'new':
                 self.parse_new(tokenizer, command)
             elif command[0].string == 'class':
+                self.parse_current_load()
                 self.parse_class(tokenizer, command, file_path_str)
             elif command[0].string == '@import':
+                self.parse_current_load()
                 if len(command) < 2:
                     raise JMCSyntaxException(
                         "Expected string after '@import'", command[0], tokenizer, col_length=True)
                 if command[1].token_type != TokenType.STRING:
                     raise JMCSyntaxException(
                         "Expected string after '@import'", command[1], tokenizer)
                 if len(command) > 2:
```

### Comparing `jmcfunction-1.2.9a3/jmc/compile/lexer_func_content.py` & `jmcfunction-1.2.9a4/jmc/compile/lexer_func_content.py`

 * *Files identical despite different names*

### Comparing `jmcfunction-1.2.9a3/jmc/compile/log.py` & `jmcfunction-1.2.9a4/jmc/compile/log.py`

 * *Files identical despite different names*

### Comparing `jmcfunction-1.2.9a3/jmc/compile/test_compile.py` & `jmcfunction-1.2.9a4/jmc/compile/test_compile.py`

 * *Files identical despite different names*

### Comparing `jmcfunction-1.2.9a3/jmc/compile/tokenizer.py` & `jmcfunction-1.2.9a4/jmc/compile/tokenizer.py`

 * *Files identical despite different names*

### Comparing `jmcfunction-1.2.9a3/jmc/compile/utils.py` & `jmcfunction-1.2.9a4/jmc/compile/utils.py`

 * *Files identical despite different names*

### Comparing `jmcfunction-1.2.9a3/jmc/compile/vanilla_command.py` & `jmcfunction-1.2.9a4/jmc/compile/vanilla_command.py`

 * *Files identical despite different names*

### Comparing `jmcfunction-1.2.9a3/jmc/terminal/configuration.py` & `jmcfunction-1.2.9a4/jmc/terminal/configuration.py`

 * *Files identical despite different names*

### Comparing `jmcfunction-1.2.9a3/jmc/terminal/main.py` & `jmcfunction-1.2.9a4/jmc/terminal/main.py`

 * *Files identical despite different names*

### Comparing `jmcfunction-1.2.9a3/jmc/terminal/utils.py` & `jmcfunction-1.2.9a4/jmc/terminal/utils.py`

 * *Files identical despite different names*

### Comparing `jmcfunction-1.2.9a3/jmc/terminal_commands.py` & `jmcfunction-1.2.9a4/jmc/terminal_commands.py`

 * *Files identical despite different names*

### Comparing `jmcfunction-1.2.9a3/jmcfunction.egg-info/PKG-INFO` & `jmcfunction-1.2.9a4/jmcfunction.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcfunction
-Version: 1.2.9a3
+Version: 1.2.9a4
 Summary: Compiler for JMC (JavaScript-like Minecraft Function), a mcfunction extension language for making Minecraft Datapack.
 Author: WingedSeal
 Author-email: firm09719@gmail.com
 License: MIT License
 Project-URL: Documentation, https://wingedseal.github.io/jmc/
 Project-URL: Repository, https://github.com/WingedSeal/jmc
 Keywords: python,minecraft,mcfunction,datapack,compiler
@@ -16,15 +16,15 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 
-# JMC &middot; [![license-mit](https://badgen.net/badge/license/MIT/blue/)](https://github.com/WingedSeal/jmc/blob/main/LICENSE) [![release](https://badgen.net/badge/release/v1.2.9-alpha.3/blue/)](https://github.com/WingedSeal/jmc/releases/latest) [![build-passing](https://badgen.net/badge/build/passing/green/)](https://wingedseal.github.io/jmc/#/) [![discord-invite](https://badgen.net/badge/discord/Official-Server/blue/?icon=discord)](https://discord.gg/PNWKpwdzD3)
+# JMC &middot; [![license-mit](https://badgen.net/badge/license/MIT/blue/)](https://github.com/WingedSeal/jmc/blob/main/LICENSE) [![release](https://badgen.net/badge/release/v1.2.9-alpha.4/blue/)](https://github.com/WingedSeal/jmc/releases/latest) [![build-passing](https://badgen.net/badge/build/passing/green/)](https://wingedseal.github.io/jmc/#/) [![discord-invite](https://badgen.net/badge/discord/Official-Server/blue/?icon=discord)](https://discord.gg/PNWKpwdzD3)
 
 ## (JavaScript-like Minecraft Function)
 
 JMC (JavaScript-like Minecraft Function) is a mcfunction extension language for making Minecraft Datapack.
 
 ![JMC-icon](https://github.com/WingedSeal/jmc/blob/webpage/src/assets/image/jmc_icon192.png?raw=true)
```

### Comparing `jmcfunction-1.2.9a3/jmcfunction.egg-info/SOURCES.txt` & `jmcfunction-1.2.9a4/jmcfunction.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jmcfunction-1.2.9a3/setup.py` & `jmcfunction-1.2.9a4/setup.py`

 * *Files identical despite different names*

