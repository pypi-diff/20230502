# Comparing `tmp/nonebot-plugin-starrail-calendar-1.0.1.tar.gz` & `tmp/nonebot_plugin_starrail_calendar-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-starrail-calendar-1.0.1.tar", last modified: Tue May  2 04:03:24 2023, max compression
+gzip compressed data, was "nonebot_plugin_starrail_calendar-1.0.2.tar", last modified: Tue May  2 04:21:28 2023, max compression
```

## Comparing `nonebot-plugin-starrail-calendar-1.0.1.tar` & `nonebot_plugin_starrail_calendar-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 04:03:24.220087 nonebot-plugin-starrail-calendar-1.0.1/
--rw-rw-rw-   0        0        0    35823 2022-05-26 22:27:12.000000 nonebot-plugin-starrail-calendar-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       85 2023-05-01 14:36:59.000000 nonebot-plugin-starrail-calendar-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      414 2023-05-02 04:03:24.220087 nonebot-plugin-starrail-calendar-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      598 2023-05-02 01:45:54.000000 nonebot-plugin-starrail-calendar-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 04:03:24.219084 nonebot-plugin-starrail-calendar-1.0.1/nonebot_plugin_starrail_calendar.egg-info/
--rw-rw-rw-   0        0        0      414 2023-05-02 04:03:24.000000 nonebot-plugin-starrail-calendar-1.0.1/nonebot_plugin_starrail_calendar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-05-02 04:03:24.000000 nonebot-plugin-starrail-calendar-1.0.1/nonebot_plugin_starrail_calendar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 04:03:24.000000 nonebot-plugin-starrail-calendar-1.0.1/nonebot_plugin_starrail_calendar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2023-05-02 04:03:24.000000 nonebot-plugin-starrail-calendar-1.0.1/nonebot_plugin_starrail_calendar.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 04:03:24.000000 nonebot-plugin-starrail-calendar-1.0.1/nonebot_plugin_starrail_calendar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 04:03:24.221594 nonebot-plugin-starrail-calendar-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      881 2023-05-02 04:03:03.000000 nonebot-plugin-starrail-calendar-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 04:21:28.074546 nonebot_plugin_starrail_calendar-1.0.2/
+-rw-rw-rw-   0        0        0    35823 2022-05-26 22:27:12.000000 nonebot_plugin_starrail_calendar-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0       85 2023-05-01 14:36:59.000000 nonebot_plugin_starrail_calendar-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      414 2023-05-02 04:21:28.073541 nonebot_plugin_starrail_calendar-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      598 2023-05-02 01:45:54.000000 nonebot_plugin_starrail_calendar-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 04:21:28.060751 nonebot_plugin_starrail_calendar-1.0.2/nonebot_plugin_starrail_calendar/
+-rw-rw-rw-   0        0        0     6265 2023-05-02 02:36:57.000000 nonebot_plugin_starrail_calendar-1.0.2/nonebot_plugin_starrail_calendar/__init__.py
+-rw-rw-rw-   0        0        0     2387 2022-10-25 13:40:10.000000 nonebot_plugin_starrail_calendar-1.0.2/nonebot_plugin_starrail_calendar/browser.py
+-rw-rw-rw-   0        0        0     4739 2023-05-02 02:09:58.000000 nonebot_plugin_starrail_calendar-1.0.2/nonebot_plugin_starrail_calendar/data_source.py
+-rw-rw-rw-   0        0        0     1901 2023-05-02 03:04:38.000000 nonebot_plugin_starrail_calendar-1.0.2/nonebot_plugin_starrail_calendar/draw_calendar.py
+-rw-rw-rw-   0        0        0     2255 2023-04-29 01:27:19.000000 nonebot_plugin_starrail_calendar-1.0.2/nonebot_plugin_starrail_calendar/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 04:21:28.072539 nonebot_plugin_starrail_calendar-1.0.2/nonebot_plugin_starrail_calendar.egg-info/
+-rw-rw-rw-   0        0        0      414 2023-05-02 04:21:28.000000 nonebot_plugin_starrail_calendar-1.0.2/nonebot_plugin_starrail_calendar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      546 2023-05-02 04:21:28.000000 nonebot_plugin_starrail_calendar-1.0.2/nonebot_plugin_starrail_calendar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 04:21:28.000000 nonebot_plugin_starrail_calendar-1.0.2/nonebot_plugin_starrail_calendar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2023-05-02 04:21:28.000000 nonebot_plugin_starrail_calendar-1.0.2/nonebot_plugin_starrail_calendar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       33 2023-05-02 04:21:28.000000 nonebot_plugin_starrail_calendar-1.0.2/nonebot_plugin_starrail_calendar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 04:21:28.074546 nonebot_plugin_starrail_calendar-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      847 2023-05-02 04:20:47.000000 nonebot_plugin_starrail_calendar-1.0.2/setup.py
```

### Comparing `nonebot-plugin-starrail-calendar-1.0.1/LICENSE` & `nonebot_plugin_starrail_calendar-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-starrail-calendar-1.0.1/README.md` & `nonebot_plugin_starrail_calendar-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-starrail-calendar-1.0.1/setup.py` & `nonebot_plugin_starrail_calendar-1.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 
 from setuptools import setup, find_packages
 
 setup(
-    name="nonebot-plugin-starrail-calendar",
-    version="1.0.1",
-    keywords=["pip", "nonebot-plugin-starrail-calendar"],
+    name="nonebot_plugin_starrail_calendar",
+    version="1.0.2",
+    keywords=["pip", "nonebot_plugin_starrail_calendar"],
     description="查看《崩坏：星穹铁道》官方活动",
     long_description="查看《崩坏：星穹铁道》官方活动",
     license="GPL Licence",
     url="https://github.com/nicklly/nonebot_plugin_StarRail_calendar",
     author="TonyKun",
     author_email="1134741727@qq.com",
-    packages=find_packages(include=["template", "template.*"]),
+    packages=find_packages(),
     include_package_data=True,
     platforms="any",
     install_requires=[
         "nonebot2 == 2.0.0rc4",
         "nonebot-adapter-onebot == 2.2.2",
         "playwright == 1.32.1",
         "httpx == 0.23.3",
```

