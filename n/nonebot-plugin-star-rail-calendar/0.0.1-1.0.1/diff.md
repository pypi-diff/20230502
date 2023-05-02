# Comparing `tmp/nonebot_plugin_star_rail_calendar-0.0.1.tar.gz` & `tmp/nonebot_plugin_star_rail_calendar-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_star_rail_calendar-0.0.1.tar", last modified: Mon May  1 14:37:12 2023, max compression
+gzip compressed data, was "nonebot_plugin_star_rail_calendar-1.0.1.tar", last modified: Tue May  2 01:42:08 2023, max compression
```

## Comparing `nonebot_plugin_star_rail_calendar-0.0.1.tar` & `nonebot_plugin_star_rail_calendar-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 14:37:12.814690 nonebot_plugin_star_rail_calendar-0.0.1/
--rw-rw-rw-   0        0        0    35823 2022-05-26 22:27:12.000000 nonebot_plugin_star_rail_calendar-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       85 2023-05-01 14:36:59.000000 nonebot_plugin_star_rail_calendar-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      417 2023-05-01 14:37:12.814690 nonebot_plugin_star_rail_calendar-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      580 2023-05-01 13:40:49.000000 nonebot_plugin_star_rail_calendar-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 14:37:12.799431 nonebot_plugin_star_rail_calendar-0.0.1/nonebot_plugin_star_rail_calendar/
--rw-rw-rw-   0        0        0     6249 2023-05-01 13:45:34.000000 nonebot_plugin_star_rail_calendar-0.0.1/nonebot_plugin_star_rail_calendar/__init__.py
--rw-rw-rw-   0        0        0     2387 2022-10-25 13:40:10.000000 nonebot_plugin_star_rail_calendar-0.0.1/nonebot_plugin_star_rail_calendar/browser.py
--rw-rw-rw-   0        0        0     4861 2023-04-29 07:06:31.000000 nonebot_plugin_star_rail_calendar-0.0.1/nonebot_plugin_star_rail_calendar/data_source.py
--rw-rw-rw-   0        0        0     1931 2023-04-29 01:21:32.000000 nonebot_plugin_star_rail_calendar-0.0.1/nonebot_plugin_star_rail_calendar/draw_calendar.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:37:12.813251 nonebot_plugin_star_rail_calendar-0.0.1/nonebot_plugin_star_rail_calendar/template/
--rw-rw-rw-   0        0        0     2371 2023-05-01 13:36:07.000000 nonebot_plugin_star_rail_calendar-0.0.1/nonebot_plugin_star_rail_calendar/template/calendar.html
--rw-rw-rw-   0        0        0     6882 2022-06-26 03:57:47.000000 nonebot_plugin_star_rail_calendar-0.0.1/nonebot_plugin_star_rail_calendar/template/index.css
--rw-rw-rw-   0        0        0   315626 2022-06-26 03:57:47.000000 nonebot_plugin_star_rail_calendar-0.0.1/nonebot_plugin_star_rail_calendar/template/iview.css
--rw-rw-rw-   0        0        0     6346 2022-06-26 03:57:47.000000 nonebot_plugin_star_rail_calendar-0.0.1/nonebot_plugin_star_rail_calendar/template/normalize.css
--rw-rw-rw-   0        0        0     2255 2023-04-29 01:27:19.000000 nonebot_plugin_star_rail_calendar-0.0.1/nonebot_plugin_star_rail_calendar/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:37:12.807253 nonebot_plugin_star_rail_calendar-0.0.1/nonebot_plugin_star_rail_calendar.egg-info/
--rw-rw-rw-   0        0        0      417 2023-05-01 14:37:12.000000 nonebot_plugin_star_rail_calendar-0.0.1/nonebot_plugin_star_rail_calendar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      776 2023-05-01 14:37:12.000000 nonebot_plugin_star_rail_calendar-0.0.1/nonebot_plugin_star_rail_calendar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 14:37:12.000000 nonebot_plugin_star_rail_calendar-0.0.1/nonebot_plugin_star_rail_calendar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-01 14:37:12.000000 nonebot_plugin_star_rail_calendar-0.0.1/nonebot_plugin_star_rail_calendar.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 14:37:12.000000 nonebot_plugin_star_rail_calendar-0.0.1/nonebot_plugin_star_rail_calendar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 14:37:12.816082 nonebot_plugin_star_rail_calendar-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      762 2023-05-01 14:35:43.000000 nonebot_plugin_star_rail_calendar-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 01:42:08.443920 nonebot_plugin_star_rail_calendar-1.0.1/
+-rw-rw-rw-   0        0        0    35823 2022-05-26 22:27:12.000000 nonebot_plugin_star_rail_calendar-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       85 2023-05-01 14:36:59.000000 nonebot_plugin_star_rail_calendar-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      417 2023-05-02 01:42:08.443920 nonebot_plugin_star_rail_calendar-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      580 2023-05-01 13:40:49.000000 nonebot_plugin_star_rail_calendar-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 01:42:08.421555 nonebot_plugin_star_rail_calendar-1.0.1/nonebot_plugin_star_rail_calendar/
+-rw-rw-rw-   0        0        0     6249 2023-05-01 13:45:34.000000 nonebot_plugin_star_rail_calendar-1.0.1/nonebot_plugin_star_rail_calendar/__init__.py
+-rw-rw-rw-   0        0        0     2387 2022-10-25 13:40:10.000000 nonebot_plugin_star_rail_calendar-1.0.1/nonebot_plugin_star_rail_calendar/browser.py
+-rw-rw-rw-   0        0        0     4861 2023-04-29 07:06:31.000000 nonebot_plugin_star_rail_calendar-1.0.1/nonebot_plugin_star_rail_calendar/data_source.py
+-rw-rw-rw-   0        0        0     1931 2023-04-29 01:21:32.000000 nonebot_plugin_star_rail_calendar-1.0.1/nonebot_plugin_star_rail_calendar/draw_calendar.py
+drwxrwxrwx   0        0        0        0 2023-05-02 01:42:08.442625 nonebot_plugin_star_rail_calendar-1.0.1/nonebot_plugin_star_rail_calendar/template/
+-rw-rw-rw-   0        0        0     2371 2023-05-01 13:36:07.000000 nonebot_plugin_star_rail_calendar-1.0.1/nonebot_plugin_star_rail_calendar/template/calendar.html
+-rw-rw-rw-   0        0        0     6882 2022-06-26 03:57:47.000000 nonebot_plugin_star_rail_calendar-1.0.1/nonebot_plugin_star_rail_calendar/template/index.css
+-rw-rw-rw-   0        0        0   315626 2022-06-26 03:57:47.000000 nonebot_plugin_star_rail_calendar-1.0.1/nonebot_plugin_star_rail_calendar/template/iview.css
+-rw-rw-rw-   0        0        0     6346 2022-06-26 03:57:47.000000 nonebot_plugin_star_rail_calendar-1.0.1/nonebot_plugin_star_rail_calendar/template/normalize.css
+-rw-rw-rw-   0        0        0     2255 2023-04-29 01:27:19.000000 nonebot_plugin_star_rail_calendar-1.0.1/nonebot_plugin_star_rail_calendar/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 01:42:08.435608 nonebot_plugin_star_rail_calendar-1.0.1/nonebot_plugin_star_rail_calendar.egg-info/
+-rw-rw-rw-   0        0        0      417 2023-05-02 01:42:08.000000 nonebot_plugin_star_rail_calendar-1.0.1/nonebot_plugin_star_rail_calendar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      776 2023-05-02 01:42:08.000000 nonebot_plugin_star_rail_calendar-1.0.1/nonebot_plugin_star_rail_calendar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 01:42:08.000000 nonebot_plugin_star_rail_calendar-1.0.1/nonebot_plugin_star_rail_calendar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      117 2023-05-02 01:42:08.000000 nonebot_plugin_star_rail_calendar-1.0.1/nonebot_plugin_star_rail_calendar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 01:42:08.000000 nonebot_plugin_star_rail_calendar-1.0.1/nonebot_plugin_star_rail_calendar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 01:42:08.443920 nonebot_plugin_star_rail_calendar-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      885 2023-05-02 01:41:49.000000 nonebot_plugin_star_rail_calendar-1.0.1/setup.py
```

### Comparing `nonebot_plugin_star_rail_calendar-0.0.1/LICENSE` & `nonebot_plugin_star_rail_calendar-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_star_rail_calendar-0.0.1/README.md` & `nonebot_plugin_star_rail_calendar-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_star_rail_calendar-0.0.1/nonebot_plugin_star_rail_calendar/__init__.py` & `nonebot_plugin_star_rail_calendar-1.0.1/nonebot_plugin_star_rail_calendar/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_star_rail_calendar-0.0.1/nonebot_plugin_star_rail_calendar/browser.py` & `nonebot_plugin_star_rail_calendar-1.0.1/nonebot_plugin_star_rail_calendar/browser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_star_rail_calendar-0.0.1/nonebot_plugin_star_rail_calendar/data_source.py` & `nonebot_plugin_star_rail_calendar-1.0.1/nonebot_plugin_star_rail_calendar/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_star_rail_calendar-0.0.1/nonebot_plugin_star_rail_calendar/draw_calendar.py` & `nonebot_plugin_star_rail_calendar-1.0.1/nonebot_plugin_star_rail_calendar/draw_calendar.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_star_rail_calendar-0.0.1/nonebot_plugin_star_rail_calendar/template/calendar.html` & `nonebot_plugin_star_rail_calendar-1.0.1/nonebot_plugin_star_rail_calendar/template/calendar.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_star_rail_calendar-0.0.1/nonebot_plugin_star_rail_calendar/template/index.css` & `nonebot_plugin_star_rail_calendar-1.0.1/nonebot_plugin_star_rail_calendar/template/index.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_star_rail_calendar-0.0.1/nonebot_plugin_star_rail_calendar/template/iview.css` & `nonebot_plugin_star_rail_calendar-1.0.1/nonebot_plugin_star_rail_calendar/template/iview.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_star_rail_calendar-0.0.1/nonebot_plugin_star_rail_calendar/template/normalize.css` & `nonebot_plugin_star_rail_calendar-1.0.1/nonebot_plugin_star_rail_calendar/template/normalize.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_star_rail_calendar-0.0.1/nonebot_plugin_star_rail_calendar/utils.py` & `nonebot_plugin_star_rail_calendar-1.0.1/nonebot_plugin_star_rail_calendar/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_star_rail_calendar-0.0.1/nonebot_plugin_star_rail_calendar.egg-info/SOURCES.txt` & `nonebot_plugin_star_rail_calendar-1.0.1/nonebot_plugin_star_rail_calendar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_star_rail_calendar-0.0.1/setup.py` & `nonebot_plugin_star_rail_calendar-1.0.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 
 from setuptools import setup, find_packages
 
 setup(
     name="nonebot_plugin_star_rail_calendar",
-    version="0.0.1",
+    version="1.0.1",
     keywords=["pip", "nonebot_plugin_star_rail_calendar"],
     description="查看《崩坏：星穹铁道》官方活动",
     long_description="查看《崩坏：星穹铁道》官方活动",
     license="GPL Licence",
     url="https://github.com/nicklly/nonebot_plugin_star_rail_calendar",
     author="TonyKun",
     author_email="1134741727@qq.com",
-    packages=find_packages(include=["template","template.*"]),
+    packages=find_packages(include=["template", "template.*"]),
     include_package_data=True,
     platforms="any",
     install_requires=[
         "nonebot2 >= 2.0.0b1",
         "nonebot-adapter-onebot >= 2.0.0b1",
+        "playwright == 1.32.1",
+        "httpx == 0.23.3",
+        "apscheduler == 3.10.1",
+        'jinja2 == 3.1.2'
     ],
 )
```

