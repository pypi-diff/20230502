# Comparing `tmp/ahk-1.0.0.tar.gz` & `tmp/ahk-1.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ahk-1.0.0.tar", last modified: Tue May  2 04:43:32 2023, max compression
+gzip compressed data, was "ahk-1.0.0b0.tar", last modified: Tue May  2 04:34:59 2023, max compression
```

## Comparing `ahk-1.0.0.tar` & `ahk-1.0.0b0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:43:32.465834 ahk-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-02 04:43:18.000000 ahk-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17855 2023-05-02 04:43:32.465834 ahk-1.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:43:32.461834 ahk-1.0.0/ahk/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-02 04:43:18.000000 ahk-1.0.0/ahk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:43:32.461834 ahk-1.0.0/ahk/_async/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-02 04:43:18.000000 ahk-1.0.0/ahk/_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   169734 2023-05-02 04:43:18.000000 ahk-1.0.0/ahk/_async/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    42426 2023-05-02 04:43:18.000000 ahk-1.0.0/ahk/_async/transport.py
--rw-r--r--   0 runner    (1001) docker     (123)    28809 2023-05-02 04:43:18.000000 ahk-1.0.0/ahk/_async/window.py
--rw-r--r--   0 runner    (1001) docker     (123)    82888 2023-05-02 04:43:18.000000 ahk-1.0.0/ahk/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-05-02 04:43:18.000000 ahk-1.0.0/ahk/_hotkey.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:43:32.465834 ahk-1.0.0/ahk/_sync/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-02 04:43:18.000000 ahk-1.0.0/ahk/_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   164017 2023-05-02 04:43:18.000000 ahk-1.0.0/ahk/_sync/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    38263 2023-05-02 04:43:18.000000 ahk-1.0.0/ahk/_sync/transport.py
--rw-r--r--   0 runner    (1001) docker     (123)    26252 2023-05-02 04:43:18.000000 ahk-1.0.0/ahk/_sync/window.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-02 04:43:18.000000 ahk-1.0.0/ahk/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-02 04:43:18.000000 ahk-1.0.0/ahk/directives.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-02 04:43:18.000000 ahk-1.0.0/ahk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-05-02 04:43:18.000000 ahk-1.0.0/ahk/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-05-02 04:43:18.000000 ahk-1.0.0/ahk/message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:43:18.000000 ahk-1.0.0/ahk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:43:32.465834 ahk-1.0.0/ahk/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    78237 2023-05-02 04:43:18.000000 ahk-1.0.0/ahk/templates/daemon.ahk
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-05-02 04:43:18.000000 ahk-1.0.0/ahk/templates/hotkeys.ahk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:43:32.461834 ahk-1.0.0/ahk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17855 2023-05-02 04:43:32.000000 ahk-1.0.0/ahk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-02 04:43:32.000000 ahk-1.0.0/ahk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 04:43:32.000000 ahk-1.0.0/ahk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-02 04:43:32.000000 ahk-1.0.0/ahk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 04:43:32.000000 ahk-1.0.0/ahk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-02 04:43:18.000000 ahk-1.0.0/buildunasync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:43:32.465834 ahk-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    16995 2023-05-02 04:43:18.000000 ahk-1.0.0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-02 04:43:18.000000 ahk-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-02 04:43:32.465834 ahk-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 04:43:18.000000 ahk-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:34:59.929923 ahk-1.0.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-02 04:34:49.000000 ahk-1.0.0b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17857 2023-05-02 04:34:59.929923 ahk-1.0.0b0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:34:59.925923 ahk-1.0.0b0/ahk/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:34:59.925923 ahk-1.0.0b0/ahk/_async/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   169734 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/_async/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42426 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/_async/transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28809 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/_async/window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82888 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/_hotkey.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:34:59.929923 ahk-1.0.0b0/ahk/_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   164017 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/_sync/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38263 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/_sync/transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26252 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/_sync/window.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/directives.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:34:59.929923 ahk-1.0.0b0/ahk/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    78237 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/templates/daemon.ahk
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-05-02 04:34:49.000000 ahk-1.0.0b0/ahk/templates/hotkeys.ahk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:34:59.925923 ahk-1.0.0b0/ahk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17857 2023-05-02 04:34:59.000000 ahk-1.0.0b0/ahk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-02 04:34:59.000000 ahk-1.0.0b0/ahk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 04:34:59.000000 ahk-1.0.0b0/ahk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-02 04:34:59.000000 ahk-1.0.0b0/ahk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 04:34:59.000000 ahk-1.0.0b0/ahk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-02 04:34:49.000000 ahk-1.0.0b0/buildunasync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:34:59.929923 ahk-1.0.0b0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    16995 2023-05-02 04:34:49.000000 ahk-1.0.0b0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-02 04:34:49.000000 ahk-1.0.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-02 04:34:59.929923 ahk-1.0.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 04:34:49.000000 ahk-1.0.0b0/setup.py
```

### Comparing `ahk-1.0.0/PKG-INFO` & `ahk-1.0.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahk
-Version: 1.0.0
+Version: 1.0.0b0
 Summary: A Python wrapper for AHK
 Home-page: https://github.com/spyoungtech/ahk
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Keywords: ahk,autohotkey,windows,mouse,keyboard,automation,pyautogui
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Desktop Environment
```

### Comparing `ahk-1.0.0/ahk/__init__.py` & `ahk-1.0.0b0/ahk/__init__.py`

 * *Files identical despite different names*

### Comparing `ahk-1.0.0/ahk/_async/engine.py` & `ahk-1.0.0b0/ahk/_async/engine.py`

 * *Files identical despite different names*

### Comparing `ahk-1.0.0/ahk/_async/transport.py` & `ahk-1.0.0b0/ahk/_async/transport.py`

 * *Files identical despite different names*

### Comparing `ahk-1.0.0/ahk/_async/window.py` & `ahk-1.0.0b0/ahk/_async/window.py`

 * *Files identical despite different names*

### Comparing `ahk-1.0.0/ahk/_constants.py` & `ahk-1.0.0b0/ahk/_constants.py`

 * *Files identical despite different names*

### Comparing `ahk-1.0.0/ahk/_hotkey.py` & `ahk-1.0.0b0/ahk/_hotkey.py`

 * *Files identical despite different names*

### Comparing `ahk-1.0.0/ahk/_sync/engine.py` & `ahk-1.0.0b0/ahk/_sync/engine.py`

 * *Files identical despite different names*

### Comparing `ahk-1.0.0/ahk/_sync/transport.py` & `ahk-1.0.0b0/ahk/_sync/transport.py`

 * *Files identical despite different names*

### Comparing `ahk-1.0.0/ahk/_sync/window.py` & `ahk-1.0.0b0/ahk/_sync/window.py`

 * *Files identical despite different names*

### Comparing `ahk-1.0.0/ahk/_utils.py` & `ahk-1.0.0b0/ahk/_utils.py`

 * *Files identical despite different names*

### Comparing `ahk-1.0.0/ahk/directives.py` & `ahk-1.0.0b0/ahk/directives.py`

 * *Files identical despite different names*

### Comparing `ahk-1.0.0/ahk/keys.py` & `ahk-1.0.0b0/ahk/keys.py`

 * *Files identical despite different names*

### Comparing `ahk-1.0.0/ahk/message.py` & `ahk-1.0.0b0/ahk/message.py`

 * *Files identical despite different names*

### Comparing `ahk-1.0.0/ahk/templates/daemon.ahk` & `ahk-1.0.0b0/ahk/templates/daemon.ahk`

 * *Files identical despite different names*

### Comparing `ahk-1.0.0/ahk/templates/hotkeys.ahk` & `ahk-1.0.0b0/ahk/templates/hotkeys.ahk`

 * *Files identical despite different names*

### Comparing `ahk-1.0.0/ahk.egg-info/PKG-INFO` & `ahk-1.0.0b0/ahk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahk
-Version: 1.0.0
+Version: 1.0.0b0
 Summary: A Python wrapper for AHK
 Home-page: https://github.com/spyoungtech/ahk
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Keywords: ahk,autohotkey,windows,mouse,keyboard,automation,pyautogui
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Desktop Environment
```

### Comparing `ahk-1.0.0/ahk.egg-info/SOURCES.txt` & `ahk-1.0.0b0/ahk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ahk-1.0.0/buildunasync.py` & `ahk-1.0.0b0/buildunasync.py`

 * *Files identical despite different names*

### Comparing `ahk-1.0.0/docs/README.md` & `ahk-1.0.0b0/docs/README.md`

 * *Files identical despite different names*

### Comparing `ahk-1.0.0/setup.cfg` & `ahk-1.0.0b0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ahk
-version = 1.0.0
+version = 1.0.0b
 author_email = spencer.young@spyoung.com
 author = Spencer Young
 description = A Python wrapper for AHK
 long_description = file: docs/README.md
 long_description_content_type = text/markdown
 url = https://github.com/spyoungtech/ahk
 keywords =
```

