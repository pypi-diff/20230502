# Comparing `tmp/vue2img-0.0.4.tar.gz` & `tmp/vue2img-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vue2img-0.0.4.tar", last modified: Mon Apr 24 03:38:24 2023, max compression
+gzip compressed data, was "vue2img-0.0.5.tar", last modified: Tue May  2 04:28:23 2023, max compression
```

## Comparing `vue2img-0.0.4.tar` & `vue2img-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 03:38:24.139109 vue2img-0.0.4/
--rw-rw-rw-   0        0        0     1086 2023-03-31 15:06:16.000000 vue2img-0.0.4/LICENSE
--rw-rw-rw-   0        0        0       55 2023-04-24 03:29:08.000000 vue2img-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      746 2023-04-24 03:38:24.138111 vue2img-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      108 2023-03-31 15:08:31.000000 vue2img-0.0.4/README.md
--rw-rw-rw-   0        0        0       55 2023-04-24 03:14:17.000000 vue2img-0.0.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 03:38:24.139109 vue2img-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      997 2023-04-24 03:38:21.000000 vue2img-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 03:38:24.121170 vue2img-0.0.4/vue2img/
--rw-rw-rw-   0        0        0      178 2023-04-24 02:43:47.000000 vue2img-0.0.4/vue2img/__init__.py
--rw-rw-rw-   0        0        0     1383 2023-04-22 10:16:30.000000 vue2img-0.0.4/vue2img/app.py
--rw-rw-rw-   0        0        0     9659 2023-04-24 03:04:14.000000 vue2img-0.0.4/vue2img/dom.py
--rw-rw-rw-   0        0        0      483 2023-04-24 03:04:58.000000 vue2img-0.0.4/vue2img/manager.py
--rw-rw-rw-   0        0        0     2098 2023-04-24 03:35:55.000000 vue2img-0.0.4/vue2img/operation.py
--rw-rw-rw-   0        0        0    24514 2023-04-24 03:38:11.000000 vue2img-0.0.4/vue2img/stopwords.py
--rw-rw-rw-   0        0        0     4157 2023-04-24 03:14:14.000000 vue2img-0.0.4/vue2img/template.py
-drwxrwxrwx   0        0        0        0 2023-04-24 03:38:24.137124 vue2img-0.0.4/vue2img.egg-info/
--rw-rw-rw-   0        0        0      746 2023-04-24 03:38:24.000000 vue2img-0.0.4/vue2img.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-04-24 03:38:24.000000 vue2img-0.0.4/vue2img.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 03:38:24.000000 vue2img-0.0.4/vue2img.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-04-24 03:38:24.000000 vue2img-0.0.4/vue2img.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-24 03:38:24.000000 vue2img-0.0.4/vue2img.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 04:28:23.249497 vue2img-0.0.5/
+-rw-rw-rw-   0        0        0     1086 2023-03-31 15:06:16.000000 vue2img-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-04-24 03:40:26.000000 vue2img-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      746 2023-05-02 04:28:23.248507 vue2img-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      108 2023-03-31 15:08:31.000000 vue2img-0.0.5/README.md
+-rw-rw-rw-   0        0        0       55 2023-04-24 03:14:17.000000 vue2img-0.0.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 04:28:23.249497 vue2img-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      997 2023-05-02 04:02:03.000000 vue2img-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 04:28:23.230561 vue2img-0.0.5/vue2img/
+-rw-rw-rw-   0        0        0      178 2023-04-24 02:43:47.000000 vue2img-0.0.5/vue2img/__init__.py
+-rw-rw-rw-   0        0        0     1383 2023-04-22 10:16:30.000000 vue2img-0.0.5/vue2img/app.py
+-rw-rw-rw-   0        0        0     9659 2023-04-24 03:04:14.000000 vue2img-0.0.5/vue2img/dom.py
+-rw-rw-rw-   0        0        0      483 2023-04-24 03:04:58.000000 vue2img-0.0.5/vue2img/manager.py
+-rw-rw-rw-   0        0        0     2098 2023-04-24 03:35:55.000000 vue2img-0.0.5/vue2img/operation.py
+-rw-rw-rw-   0        0        0    24514 2023-04-24 03:38:11.000000 vue2img-0.0.5/vue2img/stopwords.py
+-rw-rw-rw-   0        0        0     5167 2023-05-02 04:21:17.000000 vue2img-0.0.5/vue2img/template.py
+drwxrwxrwx   0        0        0        0 2023-05-02 04:28:23.246507 vue2img-0.0.5/vue2img.egg-info/
+-rw-rw-rw-   0        0        0      746 2023-05-02 04:28:23.000000 vue2img-0.0.5/vue2img.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-05-02 04:28:23.000000 vue2img-0.0.5/vue2img.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 04:28:23.000000 vue2img-0.0.5/vue2img.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-02 04:28:23.000000 vue2img-0.0.5/vue2img.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-02 04:28:23.000000 vue2img-0.0.5/vue2img.egg-info/top_level.txt
```

### Comparing `vue2img-0.0.4/LICENSE` & `vue2img-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vue2img-0.0.4/PKG-INFO` & `vue2img-0.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vue2img
-Version: 0.0.4
+Version: 0.0.5
 Summary: 通过 .vue 模板生成图片
 Home-page: https://github.com/Drelf2018/vue2img
 Author: Drelf2018
 Author-email: drelf2018@outlook.com
 License: MIT
 Keywords: python,vue
 Platform: UNKNOWN
```

### Comparing `vue2img-0.0.4/setup.py` & `vue2img-0.0.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt", "r", encoding="utf8") as f:
     requires = f.read()
 
 setup(
     name="vue2img",
-    version="0.0.4",
+    version="0.0.5",
     license="MIT",
     author="Drelf2018",
     author_email="drelf2018@outlook.com",
     description="通过 .vue 模板生成图片",
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
```

### Comparing `vue2img-0.0.4/vue2img/app.py` & `vue2img-0.0.5/vue2img/app.py`

 * *Files identical despite different names*

### Comparing `vue2img-0.0.4/vue2img/dom.py` & `vue2img-0.0.5/vue2img/dom.py`

 * *Files identical despite different names*

### Comparing `vue2img-0.0.4/vue2img/operation.py` & `vue2img-0.0.5/vue2img/operation.py`

 * *Files identical despite different names*

### Comparing `vue2img-0.0.4/vue2img/stopwords.py` & `vue2img-0.0.5/vue2img/stopwords.py`

 * *Files identical despite different names*

### Comparing `vue2img-0.0.4/vue2img.egg-info/PKG-INFO` & `vue2img-0.0.5/vue2img.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vue2img
-Version: 0.0.4
+Version: 0.0.5
 Summary: 通过 .vue 模板生成图片
 Home-page: https://github.com/Drelf2018/vue2img
 Author: Drelf2018
 Author-email: drelf2018@outlook.com
 License: MIT
 Keywords: python,vue
 Platform: UNKNOWN
```

