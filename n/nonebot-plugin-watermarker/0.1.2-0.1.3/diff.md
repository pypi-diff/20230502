# Comparing `tmp/nonebot-plugin-watermarker-0.1.2.tar.gz` & `tmp/nonebot_plugin_watermarker-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-watermarker-0.1.2.tar", last modified: Mon May  1 15:03:48 2023, max compression
+gzip compressed data, was "nonebot_plugin_watermarker-0.1.3.tar", last modified: Mon May  1 23:54:19 2023, max compression
```

## Comparing `nonebot-plugin-watermarker-0.1.2.tar` & `nonebot_plugin_watermarker-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 15:03:48.645784 nonebot-plugin-watermarker-0.1.2/
--rw-rw-rw-   0        0        0     1087 2023-05-01 12:04:12.000000 nonebot-plugin-watermarker-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     4000 2023-05-01 15:03:48.644787 nonebot-plugin-watermarker-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3644 2023-05-01 12:31:50.000000 nonebot-plugin-watermarker-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 15:03:48.633815 nonebot-plugin-watermarker-0.1.2/nonebot-plugin-watermarker/
--rw-rw-rw-   0        0        0     2081 2023-05-01 09:27:24.000000 nonebot-plugin-watermarker-0.1.2/nonebot-plugin-watermarker/__init__.py
--rw-rw-rw-   0        0        0      842 2023-05-01 09:25:17.000000 nonebot-plugin-watermarker-0.1.2/nonebot-plugin-watermarker/config.py
--rw-rw-rw-   0        0        0     2009 2023-05-01 08:46:06.000000 nonebot-plugin-watermarker-0.1.2/nonebot-plugin-watermarker/fuctions.py
-drwxrwxrwx   0        0        0        0 2023-05-01 15:03:48.642792 nonebot-plugin-watermarker-0.1.2/nonebot_plugin_watermarker.egg-info/
--rw-rw-rw-   0        0        0     4000 2023-05-01 15:03:48.000000 nonebot-plugin-watermarker-0.1.2/nonebot_plugin_watermarker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      390 2023-05-01 15:03:48.000000 nonebot-plugin-watermarker-0.1.2/nonebot_plugin_watermarker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 15:03:48.000000 nonebot-plugin-watermarker-0.1.2/nonebot_plugin_watermarker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-01 15:03:48.000000 nonebot-plugin-watermarker-0.1.2/nonebot_plugin_watermarker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-05-01 15:03:48.000000 nonebot-plugin-watermarker-0.1.2/nonebot_plugin_watermarker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 15:03:48.645784 nonebot-plugin-watermarker-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     4208 2023-05-01 15:03:22.000000 nonebot-plugin-watermarker-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 23:54:19.730735 nonebot_plugin_watermarker-0.1.3/
+-rw-rw-rw-   0        0        0     1087 2023-05-01 12:04:12.000000 nonebot_plugin_watermarker-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     4000 2023-05-01 23:54:19.729765 nonebot_plugin_watermarker-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3644 2023-05-01 12:31:50.000000 nonebot_plugin_watermarker-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 23:54:19.720766 nonebot_plugin_watermarker-0.1.3/nonebot_plugin_watermarker/
+-rw-rw-rw-   0        0        0     2081 2023-05-01 23:54:10.000000 nonebot_plugin_watermarker-0.1.3/nonebot_plugin_watermarker/__init__.py
+-rw-rw-rw-   0        0        0      842 2023-05-01 09:25:17.000000 nonebot_plugin_watermarker-0.1.3/nonebot_plugin_watermarker/config.py
+-rw-rw-rw-   0        0        0     2009 2023-05-01 08:46:06.000000 nonebot_plugin_watermarker-0.1.3/nonebot_plugin_watermarker/fuctions.py
+drwxrwxrwx   0        0        0        0 2023-05-01 23:54:19.728739 nonebot_plugin_watermarker-0.1.3/nonebot_plugin_watermarker.egg-info/
+-rw-rw-rw-   0        0        0     4000 2023-05-01 23:54:19.000000 nonebot_plugin_watermarker-0.1.3/nonebot_plugin_watermarker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2023-05-01 23:54:19.000000 nonebot_plugin_watermarker-0.1.3/nonebot_plugin_watermarker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 23:54:19.000000 nonebot_plugin_watermarker-0.1.3/nonebot_plugin_watermarker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-01 23:54:19.000000 nonebot_plugin_watermarker-0.1.3/nonebot_plugin_watermarker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-05-01 23:54:19.000000 nonebot_plugin_watermarker-0.1.3/nonebot_plugin_watermarker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 23:54:19.730735 nonebot_plugin_watermarker-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     4208 2023-05-01 23:53:54.000000 nonebot_plugin_watermarker-0.1.3/setup.py
```

### Comparing `nonebot-plugin-watermarker-0.1.2/LICENSE` & `nonebot_plugin_watermarker-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-watermarker-0.1.2/PKG-INFO` & `nonebot_plugin_watermarker-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nonebot-plugin-watermarker
-Version: 0.1.2
+Name: nonebot_plugin_watermarker
+Version: 0.1.3
 Summary: 为nonebot机器人发送的图片加上水印
 Home-page: https://github.com/X-Skirt-X/nonebot-plugin-watermarker
 Author: XU
 Author-email: Woyerpa@outlook.com
 License: MIT License
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-watermarker Version: 0.1.2 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_watermarker Version: 0.1.3 Summary:
 ä¸ºnonebotæºå¨äººåéçå¾çå ä¸æ°´å° Home-page: https://github.com/X-
 Skirt-X/nonebot-plugin-watermarker Author: XU Author-email: Woyerpa@outlook.com
 License: MIT License Platform: UNKNOWN Description-Content-Type: text/markdown
 License-File: LICENSE
                             [PoweredByNonebotLogo]
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
```

### Comparing `nonebot-plugin-watermarker-0.1.2/README.md` & `nonebot_plugin_watermarker-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-watermarker-0.1.2/nonebot-plugin-watermarker/__init__.py` & `nonebot_plugin_watermarker-0.1.3/nonebot_plugin_watermarker/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-watermarker-0.1.2/nonebot-plugin-watermarker/config.py` & `nonebot_plugin_watermarker-0.1.3/nonebot_plugin_watermarker/config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-watermarker-0.1.2/nonebot-plugin-watermarker/fuctions.py` & `nonebot_plugin_watermarker-0.1.3/nonebot_plugin_watermarker/fuctions.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-watermarker-0.1.2/nonebot_plugin_watermarker.egg-info/PKG-INFO` & `nonebot_plugin_watermarker-0.1.3/nonebot_plugin_watermarker.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-watermarker
-Version: 0.1.2
+Version: 0.1.3
 Summary: 为nonebot机器人发送的图片加上水印
 Home-page: https://github.com/X-Skirt-X/nonebot-plugin-watermarker
 Author: XU
 Author-email: Woyerpa@outlook.com
 License: MIT License
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-watermarker Version: 0.1.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-watermarker Version: 0.1.3 Summary:
 ä¸ºnonebotæºå¨äººåéçå¾çå ä¸æ°´å° Home-page: https://github.com/X-
 Skirt-X/nonebot-plugin-watermarker Author: XU Author-email: Woyerpa@outlook.com
 License: MIT License Platform: UNKNOWN Description-Content-Type: text/markdown
 License-File: LICENSE
                             [PoweredByNonebotLogo]
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
```

### Comparing `nonebot-plugin-watermarker-0.1.2/setup.py` & `nonebot_plugin_watermarker-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
     
 setup(
-    name='nonebot-plugin-watermarker',
+    name='nonebot_plugin_watermarker',
 
-    version="0.1.2",
+    version="0.1.3",
     description=(
         '为nonebot机器人发送的图片加上水印'
 
     ),
     long_description="""<div align="center">
   <p><img src="https://user-images.githubusercontent.com/91937041/235443858-85949be1-08d6-4d7a-b132-b1aed71ab943.png" width="560" alt="PoweredByNonebotLogo"></p>
   <a href="https://v2.nonebot.dev/store"><img src="https://ghproxy.com/https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-from setuptools import setup, find_packages setup( name='nonebot-plugin-
-watermarker', version="0.1.2", description=
+from setuptools import setup, find_packages setup
+( name='nonebot_plugin_watermarker', version="0.1.3", description=
 ( 'ä¸ºnonebotæºå¨äººåéçå¾çå ä¸æ°´å°' ), long_description="""
                             [PoweredByNonebotLogo]
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
 # nonebot-plugin-watermarker _â¨ ä¸ºä½ çbotååºçå¾çæ·»å æ°´å°! â¨_
                            [license] [pypi] [python]
  * [ðç®ä»](#ç®ä») * [ð¿ å®è£æ¹æ³](#å®è£æ¹æ³) *
```

