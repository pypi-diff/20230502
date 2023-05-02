# Comparing `tmp/lesscode_tool-0.0.4.tar.gz` & `tmp/lesscode_tool-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lesscode_tool-0.0.4.tar", last modified: Tue May  2 16:39:27 2023, max compression
+gzip compressed data, was "dist/lesscode_tool-0.0.5.tar", last modified: Tue May  2 17:02:02 2023, max compression
```

## Comparing `lesscode_tool-0.0.4.tar` & `lesscode_tool-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-05-02 16:39:27.000000 lesscode_tool-0.0.4/
--rw-r--r--   0 navy      (1000) navy      (1000)    11357 2023-05-02 15:26:13.000000 lesscode_tool-0.0.4/LICENSE
--rw-r--r--   0 navy      (1000) navy      (1000)      348 2023-05-02 16:39:27.000000 lesscode_tool-0.0.4/PKG-INFO
--rw-r--r--   0 navy      (1000) navy      (1000)     1317 2023-05-02 15:26:13.000000 lesscode_tool-0.0.4/README.md
-drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-05-02 16:39:27.000000 lesscode_tool-0.0.4/lesscode_tool.egg-info/
--rw-r--r--   0 navy      (1000) navy      (1000)      348 2023-05-02 16:39:27.000000 lesscode_tool-0.0.4/lesscode_tool.egg-info/PKG-INFO
--rw-r--r--   0 navy      (1000) navy      (1000)      383 2023-05-02 16:39:27.000000 lesscode_tool-0.0.4/lesscode_tool.egg-info/SOURCES.txt
--rw-r--r--   0 navy      (1000) navy      (1000)        1 2023-05-02 16:39:27.000000 lesscode_tool-0.0.4/lesscode_tool.egg-info/dependency_links.txt
--rw-r--r--   0 navy      (1000) navy      (1000)       56 2023-05-02 16:39:27.000000 lesscode_tool-0.0.4/lesscode_tool.egg-info/entry_points.txt
--rw-r--r--   0 navy      (1000) navy      (1000)       33 2023-05-02 16:39:27.000000 lesscode_tool-0.0.4/lesscode_tool.egg-info/requires.txt
--rw-r--r--   0 navy      (1000) navy      (1000)        4 2023-05-02 16:39:27.000000 lesscode_tool-0.0.4/lesscode_tool.egg-info/top_level.txt
-drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-05-02 16:39:27.000000 lesscode_tool-0.0.4/pkg/
--rw-r--r--   0 navy      (1000) navy      (1000)        1 2023-05-02 16:29:46.000000 lesscode_tool-0.0.4/pkg/__init__.py
--rwxr-xr-x   0 navy      (1000) navy      (1000)     1284 2023-05-02 16:39:02.000000 lesscode_tool-0.0.4/pkg/lesscode_tool.py
-drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-05-02 16:39:27.000000 lesscode_tool-0.0.4/pkg/tool/
--rw-r--r--   0 navy      (1000) navy      (1000)        0 2023-05-02 09:03:55.000000 lesscode_tool-0.0.4/pkg/tool/__init__.py
--rw-r--r--   0 navy      (1000) navy      (1000)      816 2023-05-02 14:41:37.000000 lesscode_tool-0.0.4/pkg/tool/convert.py
--rw-r--r--   0 navy      (1000) navy      (1000)     2080 2023-05-02 16:12:18.000000 lesscode_tool-0.0.4/pkg/tool/new.py
--rw-r--r--   0 navy      (1000) navy      (1000)     2126 2023-05-02 16:29:46.000000 lesscode_tool-0.0.4/pkg/tool/sqlacodegen.py
--rw-r--r--   0 navy      (1000) navy      (1000)       22 2023-05-02 16:39:02.000000 lesscode_tool-0.0.4/pkg/version.py
--rw-r--r--   0 navy      (1000) navy      (1000)       38 2023-05-02 16:39:27.000000 lesscode_tool-0.0.4/setup.cfg
--rwxr-xr-x   0 navy      (1000) navy      (1000)      702 2023-05-02 15:19:52.000000 lesscode_tool-0.0.4/setup.py
+drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-05-02 17:02:02.000000 lesscode_tool-0.0.5/
+-rw-r--r--   0 navy      (1000) navy      (1000)    11357 2023-05-02 15:26:13.000000 lesscode_tool-0.0.5/LICENSE
+-rw-r--r--   0 navy      (1000) navy      (1000)      348 2023-05-02 17:02:02.000000 lesscode_tool-0.0.5/PKG-INFO
+-rw-r--r--   0 navy      (1000) navy      (1000)     1317 2023-05-02 15:26:13.000000 lesscode_tool-0.0.5/README.md
+drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-05-02 17:02:02.000000 lesscode_tool-0.0.5/lesscode_tool.egg-info/
+-rw-r--r--   0 navy      (1000) navy      (1000)      348 2023-05-02 17:02:02.000000 lesscode_tool-0.0.5/lesscode_tool.egg-info/PKG-INFO
+-rw-r--r--   0 navy      (1000) navy      (1000)      383 2023-05-02 17:02:02.000000 lesscode_tool-0.0.5/lesscode_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 navy      (1000) navy      (1000)        1 2023-05-02 17:02:02.000000 lesscode_tool-0.0.5/lesscode_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 navy      (1000) navy      (1000)       56 2023-05-02 17:02:02.000000 lesscode_tool-0.0.5/lesscode_tool.egg-info/entry_points.txt
+-rw-r--r--   0 navy      (1000) navy      (1000)       33 2023-05-02 17:02:02.000000 lesscode_tool-0.0.5/lesscode_tool.egg-info/requires.txt
+-rw-r--r--   0 navy      (1000) navy      (1000)        4 2023-05-02 17:02:02.000000 lesscode_tool-0.0.5/lesscode_tool.egg-info/top_level.txt
+drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-05-02 17:02:02.000000 lesscode_tool-0.0.5/pkg/
+-rw-r--r--   0 navy      (1000) navy      (1000)        1 2023-05-02 16:29:46.000000 lesscode_tool-0.0.5/pkg/__init__.py
+-rwxr-xr-x   0 navy      (1000) navy      (1000)     1284 2023-05-02 16:39:02.000000 lesscode_tool-0.0.5/pkg/lesscode_tool.py
+drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-05-02 17:02:02.000000 lesscode_tool-0.0.5/pkg/tool/
+-rw-r--r--   0 navy      (1000) navy      (1000)        0 2023-05-02 09:03:55.000000 lesscode_tool-0.0.5/pkg/tool/__init__.py
+-rw-r--r--   0 navy      (1000) navy      (1000)      816 2023-05-02 14:41:37.000000 lesscode_tool-0.0.5/pkg/tool/convert.py
+-rw-r--r--   0 navy      (1000) navy      (1000)     6962 2023-05-02 17:01:35.000000 lesscode_tool-0.0.5/pkg/tool/new.py
+-rw-r--r--   0 navy      (1000) navy      (1000)     2126 2023-05-02 16:29:46.000000 lesscode_tool-0.0.5/pkg/tool/sqlacodegen.py
+-rw-r--r--   0 navy      (1000) navy      (1000)       22 2023-05-02 16:43:14.000000 lesscode_tool-0.0.5/pkg/version.py
+-rw-r--r--   0 navy      (1000) navy      (1000)       38 2023-05-02 17:02:02.000000 lesscode_tool-0.0.5/setup.cfg
+-rwxr-xr-x   0 navy      (1000) navy      (1000)      702 2023-05-02 16:52:06.000000 lesscode_tool-0.0.5/setup.py
```

### Comparing `lesscode_tool-0.0.4/LICENSE` & `lesscode_tool-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lesscode_tool-0.0.4/README.md` & `lesscode_tool-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `lesscode_tool-0.0.4/pkg/lesscode_tool.py` & `lesscode_tool-0.0.5/pkg/lesscode_tool.py`

 * *Files identical despite different names*

### Comparing `lesscode_tool-0.0.4/pkg/tool/convert.py` & `lesscode_tool-0.0.5/pkg/tool/convert.py`

 * *Files identical despite different names*

### Comparing `lesscode_tool-0.0.4/pkg/tool/sqlacodegen.py` & `lesscode_tool-0.0.5/pkg/tool/sqlacodegen.py`

 * *Files identical despite different names*

### Comparing `lesscode_tool-0.0.4/setup.py` & `lesscode_tool-0.0.5/setup.py`

 * *Files identical despite different names*

