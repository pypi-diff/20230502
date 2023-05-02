# Comparing `tmp/lesscode_tool-0.0.2.tar.gz` & `tmp/lesscode_tool-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lesscode_tool-0.0.2.tar", last modified: Tue May  2 16:29:53 2023, max compression
+gzip compressed data, was "dist/lesscode_tool-0.0.3.tar", last modified: Tue May  2 16:35:28 2023, max compression
```

## Comparing `lesscode_tool-0.0.2.tar` & `lesscode_tool-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-05-02 16:29:53.000000 lesscode_tool-0.0.2/
--rw-r--r--   0 navy      (1000) navy      (1000)    11357 2023-05-02 15:26:13.000000 lesscode_tool-0.0.2/LICENSE
--rw-r--r--   0 navy      (1000) navy      (1000)      348 2023-05-02 16:29:53.000000 lesscode_tool-0.0.2/PKG-INFO
--rw-r--r--   0 navy      (1000) navy      (1000)     1317 2023-05-02 15:26:13.000000 lesscode_tool-0.0.2/README.md
-drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-05-02 16:29:53.000000 lesscode_tool-0.0.2/lesscode_tool.egg-info/
--rw-r--r--   0 navy      (1000) navy      (1000)      348 2023-05-02 16:29:53.000000 lesscode_tool-0.0.2/lesscode_tool.egg-info/PKG-INFO
--rw-r--r--   0 navy      (1000) navy      (1000)      383 2023-05-02 16:29:53.000000 lesscode_tool-0.0.2/lesscode_tool.egg-info/SOURCES.txt
--rw-r--r--   0 navy      (1000) navy      (1000)        1 2023-05-02 16:29:53.000000 lesscode_tool-0.0.2/lesscode_tool.egg-info/dependency_links.txt
--rw-r--r--   0 navy      (1000) navy      (1000)       56 2023-05-02 16:29:53.000000 lesscode_tool-0.0.2/lesscode_tool.egg-info/entry_points.txt
--rw-r--r--   0 navy      (1000) navy      (1000)       33 2023-05-02 16:29:53.000000 lesscode_tool-0.0.2/lesscode_tool.egg-info/requires.txt
--rw-r--r--   0 navy      (1000) navy      (1000)        4 2023-05-02 16:29:53.000000 lesscode_tool-0.0.2/lesscode_tool.egg-info/top_level.txt
-drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-05-02 16:29:53.000000 lesscode_tool-0.0.2/pkg/
--rw-r--r--   0 navy      (1000) navy      (1000)        1 2023-05-02 16:29:46.000000 lesscode_tool-0.0.2/pkg/__init__.py
--rwxr-xr-x   0 navy      (1000) navy      (1000)     1308 2023-05-02 16:29:46.000000 lesscode_tool-0.0.2/pkg/lesscode_tool.py
-drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-05-02 16:29:53.000000 lesscode_tool-0.0.2/pkg/tool/
--rw-r--r--   0 navy      (1000) navy      (1000)        0 2023-05-02 09:03:55.000000 lesscode_tool-0.0.2/pkg/tool/__init__.py
--rw-r--r--   0 navy      (1000) navy      (1000)      816 2023-05-02 14:41:37.000000 lesscode_tool-0.0.2/pkg/tool/convert.py
--rw-r--r--   0 navy      (1000) navy      (1000)     2080 2023-05-02 16:12:18.000000 lesscode_tool-0.0.2/pkg/tool/new.py
--rw-r--r--   0 navy      (1000) navy      (1000)     2126 2023-05-02 16:29:46.000000 lesscode_tool-0.0.2/pkg/tool/sqlacodegen.py
--rw-r--r--   0 navy      (1000) navy      (1000)       22 2023-05-02 16:29:46.000000 lesscode_tool-0.0.2/pkg/version.py
--rw-r--r--   0 navy      (1000) navy      (1000)       38 2023-05-02 16:29:53.000000 lesscode_tool-0.0.2/setup.cfg
--rwxr-xr-x   0 navy      (1000) navy      (1000)      702 2023-05-02 15:19:52.000000 lesscode_tool-0.0.2/setup.py
+drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-05-02 16:35:28.000000 lesscode_tool-0.0.3/
+-rw-r--r--   0 navy      (1000) navy      (1000)    11357 2023-05-02 15:26:13.000000 lesscode_tool-0.0.3/LICENSE
+-rw-r--r--   0 navy      (1000) navy      (1000)      348 2023-05-02 16:35:28.000000 lesscode_tool-0.0.3/PKG-INFO
+-rw-r--r--   0 navy      (1000) navy      (1000)     1317 2023-05-02 15:26:13.000000 lesscode_tool-0.0.3/README.md
+drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-05-02 16:35:28.000000 lesscode_tool-0.0.3/lesscode_tool.egg-info/
+-rw-r--r--   0 navy      (1000) navy      (1000)      348 2023-05-02 16:35:28.000000 lesscode_tool-0.0.3/lesscode_tool.egg-info/PKG-INFO
+-rw-r--r--   0 navy      (1000) navy      (1000)      383 2023-05-02 16:35:28.000000 lesscode_tool-0.0.3/lesscode_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 navy      (1000) navy      (1000)        1 2023-05-02 16:35:28.000000 lesscode_tool-0.0.3/lesscode_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 navy      (1000) navy      (1000)       56 2023-05-02 16:35:28.000000 lesscode_tool-0.0.3/lesscode_tool.egg-info/entry_points.txt
+-rw-r--r--   0 navy      (1000) navy      (1000)       33 2023-05-02 16:35:28.000000 lesscode_tool-0.0.3/lesscode_tool.egg-info/requires.txt
+-rw-r--r--   0 navy      (1000) navy      (1000)        4 2023-05-02 16:35:28.000000 lesscode_tool-0.0.3/lesscode_tool.egg-info/top_level.txt
+drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-05-02 16:35:28.000000 lesscode_tool-0.0.3/pkg/
+-rw-r--r--   0 navy      (1000) navy      (1000)        1 2023-05-02 16:29:46.000000 lesscode_tool-0.0.3/pkg/__init__.py
+-rwxr-xr-x   0 navy      (1000) navy      (1000)     1306 2023-05-02 16:35:03.000000 lesscode_tool-0.0.3/pkg/lesscode_tool.py
+drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-05-02 16:35:28.000000 lesscode_tool-0.0.3/pkg/tool/
+-rw-r--r--   0 navy      (1000) navy      (1000)        0 2023-05-02 09:03:55.000000 lesscode_tool-0.0.3/pkg/tool/__init__.py
+-rw-r--r--   0 navy      (1000) navy      (1000)      816 2023-05-02 14:41:37.000000 lesscode_tool-0.0.3/pkg/tool/convert.py
+-rw-r--r--   0 navy      (1000) navy      (1000)     2080 2023-05-02 16:12:18.000000 lesscode_tool-0.0.3/pkg/tool/new.py
+-rw-r--r--   0 navy      (1000) navy      (1000)     2126 2023-05-02 16:29:46.000000 lesscode_tool-0.0.3/pkg/tool/sqlacodegen.py
+-rw-r--r--   0 navy      (1000) navy      (1000)       22 2023-05-02 16:35:04.000000 lesscode_tool-0.0.3/pkg/version.py
+-rw-r--r--   0 navy      (1000) navy      (1000)       38 2023-05-02 16:35:28.000000 lesscode_tool-0.0.3/setup.cfg
+-rwxr-xr-x   0 navy      (1000) navy      (1000)      702 2023-05-02 15:19:52.000000 lesscode_tool-0.0.3/setup.py
```

### Comparing `lesscode_tool-0.0.2/LICENSE` & `lesscode_tool-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lesscode_tool-0.0.2/README.md` & `lesscode_tool-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `lesscode_tool-0.0.2/pkg/lesscode_tool.py` & `lesscode_tool-0.0.3/pkg/lesscode_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!/usr/bin/env python3
 """
 Example of program which uses [options] shortcut in pattern.
 
 Usage:
-  lesscode_tool (new -d dir [-p project]|sqlacodegen -u url [-t table][-f file])
-
+  lesscodeTool (new -d dir [-p project]|sqlacodegen -u url [-t table][-f file])
 Options:
   -h, --help                查看帮助
   -v, --version            展示版本号
   -d, --dir dir            项目目录
   -u, --url url            数据库连接
   -f, --file file          表结构类输出文件
   -p, --project project    项目模板名
```

### Comparing `lesscode_tool-0.0.2/pkg/tool/convert.py` & `lesscode_tool-0.0.3/pkg/tool/convert.py`

 * *Files identical despite different names*

### Comparing `lesscode_tool-0.0.2/pkg/tool/new.py` & `lesscode_tool-0.0.3/pkg/tool/new.py`

 * *Files identical despite different names*

### Comparing `lesscode_tool-0.0.2/pkg/tool/sqlacodegen.py` & `lesscode_tool-0.0.3/pkg/tool/sqlacodegen.py`

 * *Files identical despite different names*

### Comparing `lesscode_tool-0.0.2/setup.py` & `lesscode_tool-0.0.3/setup.py`

 * *Files identical despite different names*

