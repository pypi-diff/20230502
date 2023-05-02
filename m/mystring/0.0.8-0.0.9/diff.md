# Comparing `tmp/mystring-0.0.8.tar.gz` & `tmp/mystring-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mystring-0.0.8.tar", last modified: Mon Feb 27 04:25:29 2023, max compression
+gzip compressed data, was "mystring-0.0.9.tar", last modified: Sun Mar  5 22:54:59 2023, max compression
```

## Comparing `mystring-0.0.8.tar` & `mystring-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 04:25:29.583308 mystring-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-02-27 04:25:23.000000 mystring-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-27 04:25:29.583308 mystring-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-27 04:25:23.000000 mystring-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 04:25:29.583308 mystring-0.0.8/mystring/
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-02-27 04:25:23.000000 mystring-0.0.8/mystring/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 04:25:29.583308 mystring-0.0.8/mystring.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-27 04:25:29.000000 mystring-0.0.8/mystring.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-02-27 04:25:29.000000 mystring-0.0.8/mystring.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 04:25:29.000000 mystring-0.0.8/mystring.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-27 04:25:29.000000 mystring-0.0.8/mystring.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 04:25:29.583308 mystring-0.0.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3409 2023-02-27 04:25:23.000000 mystring-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:54:59.363714 mystring-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-05 22:54:55.000000 mystring-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-05 22:54:59.363714 mystring-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-05 22:54:55.000000 mystring-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:54:59.363714 mystring-0.0.9/mystring/
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-03-05 22:54:55.000000 mystring-0.0.9/mystring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:54:59.363714 mystring-0.0.9/mystring.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-05 22:54:59.000000 mystring-0.0.9/mystring.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-05 22:54:59.000000 mystring-0.0.9/mystring.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 22:54:59.000000 mystring-0.0.9/mystring.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-05 22:54:59.000000 mystring-0.0.9/mystring.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-05 22:54:59.363714 mystring-0.0.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3409 2023-03-05 22:54:55.000000 mystring-0.0.9/setup.py
```

### Comparing `mystring-0.0.8/LICENSE` & `mystring-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mystring-0.0.8/mystring/__init__.py` & `mystring-0.0.9/mystring/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,17 +20,19 @@
         return self
 
     def pres(self, *args):
         for arg in args:
             self = self.pre(arg)
         return self
 
+    @empty
     def empty(self):
         return self is None or self.strip() == '' or self.strip().lower() == 'nan'
 
+    @empty
     def notempty(self):
         return not self.empty()
 
     def format(self, numstyle='06'):
         return format(int(self),numstyle)
 
     def splitsies(self,*args,joiner=":"):
```

### Comparing `mystring-0.0.8/setup.py` & `mystring-0.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

