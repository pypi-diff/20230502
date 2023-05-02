# Comparing `tmp/phot2lc-1.7.5.tar.gz` & `tmp/phot2lc-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phot2lc-1.7.5.tar", last modified: Sat Apr 29 00:27:40 2023, max compression
+gzip compressed data, was "phot2lc-1.7.6.tar", last modified: Tue May  2 21:53:35 2023, max compression
```

## Comparing `phot2lc-1.7.5.tar` & `phot2lc-1.7.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2023-04-29 00:27:40.203914 phot2lc-1.7.5/
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     1058 2020-06-12 15:08:44.000000 phot2lc-1.7.5/LICENSE
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     1219 2023-04-29 00:27:40.203914 phot2lc-1.7.5/PKG-INFO
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)      640 2020-06-14 20:06:06.000000 phot2lc-1.7.5/README.md
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)       38 2023-04-29 00:27:40.203914 phot2lc-1.7.5/setup.cfg
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     1094 2023-04-29 00:27:25.000000 phot2lc-1.7.5/setup.py
-drwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2023-04-29 00:27:40.199914 phot2lc-1.7.5/src/
-drwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2023-04-29 00:27:40.203914 phot2lc-1.7.5/src/phot2lc/
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2020-06-12 15:54:42.000000 phot2lc-1.7.5/src/phot2lc/__init__.py
--rwxrwxrwx   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     2333 2023-04-29 00:14:55.000000 phot2lc-1.7.5/src/phot2lc/addstar
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)      281 2023-02-22 04:21:11.000000 phot2lc-1.7.5/src/phot2lc/config.dat
--rwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)    83856 2023-04-29 00:22:15.000000 phot2lc-1.7.5/src/phot2lc/phot2lc
--rwxrwxrwx   0 zachvanderbosch  (1000) zachvanderbosch  (1000)      314 2023-04-29 00:26:01.000000 phot2lc-1.7.5/src/phot2lc/photconfig
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)    17242 2023-02-22 04:27:41.000000 phot2lc-1.7.5/src/phot2lc/photfunc.py
--rwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     9083 2023-02-01 21:25:50.000000 phot2lc-1.7.5/src/phot2lc/quicklook
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     4266 2022-11-30 00:07:41.000000 phot2lc-1.7.5/src/phot2lc/teledat.py
--rw-r--r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     5861 2023-02-09 02:35:54.000000 phot2lc-1.7.5/src/phot2lc/ucm_utils.py
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)    21388 2023-04-29 00:27:11.000000 phot2lc-1.7.5/src/phot2lc/version_history.txt
--rwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     5981 2020-11-15 20:21:32.000000 phot2lc-1.7.5/src/phot2lc/weldlc
-drwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2023-04-29 00:27:40.203914 phot2lc-1.7.5/src/phot2lc.egg-info/
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     1219 2023-04-29 00:27:40.000000 phot2lc-1.7.5/src/phot2lc.egg-info/PKG-INFO
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)      421 2023-04-29 00:27:40.000000 phot2lc-1.7.5/src/phot2lc.egg-info/SOURCES.txt
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        1 2023-04-29 00:27:40.000000 phot2lc-1.7.5/src/phot2lc.egg-info/dependency_links.txt
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        8 2023-04-29 00:27:40.000000 phot2lc-1.7.5/src/phot2lc.egg-info/top_level.txt
+drwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2023-05-02 21:53:35.460662 phot2lc-1.7.6/
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     1058 2020-06-12 15:08:44.000000 phot2lc-1.7.6/LICENSE
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     1219 2023-05-02 21:53:35.460662 phot2lc-1.7.6/PKG-INFO
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)      640 2020-06-14 20:06:06.000000 phot2lc-1.7.6/README.md
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)       38 2023-05-02 21:53:35.460662 phot2lc-1.7.6/setup.cfg
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     1094 2023-05-02 21:52:36.000000 phot2lc-1.7.6/setup.py
+drwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2023-05-02 21:53:35.460662 phot2lc-1.7.6/src/
+drwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2023-05-02 21:53:35.460662 phot2lc-1.7.6/src/phot2lc/
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2020-06-12 15:54:42.000000 phot2lc-1.7.6/src/phot2lc/__init__.py
+-rwxrwxrwx   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     2333 2023-05-02 21:50:55.000000 phot2lc-1.7.6/src/phot2lc/addstar
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)      281 2023-02-22 04:21:11.000000 phot2lc-1.7.6/src/phot2lc/config.dat
+-rwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)    83856 2023-04-29 00:22:15.000000 phot2lc-1.7.6/src/phot2lc/phot2lc
+-rwxrwxrwx   0 zachvanderbosch  (1000) zachvanderbosch  (1000)      314 2023-04-29 00:26:01.000000 phot2lc-1.7.6/src/phot2lc/photconfig
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)    17242 2023-02-22 04:27:41.000000 phot2lc-1.7.6/src/phot2lc/photfunc.py
+-rwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     9083 2023-02-01 21:25:50.000000 phot2lc-1.7.6/src/phot2lc/quicklook
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     4266 2022-11-30 00:07:41.000000 phot2lc-1.7.6/src/phot2lc/teledat.py
+-rw-r--r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     5861 2023-02-09 02:35:54.000000 phot2lc-1.7.6/src/phot2lc/ucm_utils.py
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)    21475 2023-05-02 21:51:26.000000 phot2lc-1.7.6/src/phot2lc/version_history.txt
+-rwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     5981 2020-11-15 20:21:32.000000 phot2lc-1.7.6/src/phot2lc/weldlc
+drwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2023-05-02 21:53:35.460662 phot2lc-1.7.6/src/phot2lc.egg-info/
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     1219 2023-05-02 21:53:35.000000 phot2lc-1.7.6/src/phot2lc.egg-info/PKG-INFO
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)      421 2023-05-02 21:53:35.000000 phot2lc-1.7.6/src/phot2lc.egg-info/SOURCES.txt
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        1 2023-05-02 21:53:35.000000 phot2lc-1.7.6/src/phot2lc.egg-info/dependency_links.txt
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        8 2023-05-02 21:53:35.000000 phot2lc-1.7.6/src/phot2lc.egg-info/top_level.txt
```

### Comparing `phot2lc-1.7.5/LICENSE` & `phot2lc-1.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `phot2lc-1.7.5/PKG-INFO` & `phot2lc-1.7.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phot2lc
-Version: 1.7.5
+Version: 1.7.6
 Summary: Light curve extraction
 Home-page: https://github.com/zvanderbosch/phot2lc
 Author: Zach Vanderbosch
 Author-email: zvanderbosch@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
```

### Comparing `phot2lc-1.7.5/README.md` & `phot2lc-1.7.6/README.md`

 * *Files identical despite different names*

### Comparing `phot2lc-1.7.5/setup.py` & `phot2lc-1.7.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="phot2lc",
-    version="1.7.5",
+    version="1.7.6",
     author="Zach Vanderbosch",
     author_email="zvanderbosch@gmail.com",
     description="Light curve extraction",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zvanderbosch/phot2lc",
     packages=setuptools.find_packages('src'),
```

### Comparing `phot2lc-1.7.5/src/phot2lc/addstar` & `phot2lc-1.7.6/src/phot2lc/addstar`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 # Oopen stars.dat file
 config_path = os.path.dirname(os.path.realpath(teledat.__file__))
 config_dat = []
 with open(config_path + "/config.dat") as f:
     for l in f.readlines():
         config_dat.append(l.strip("\n").split("=")[-1].strip())
 
-star_dat_file = config_dat[3]
+star_dat_file = config_dat[4]
 star_dat = pd.read_csv(
     star_dat_file,
     header=None,
     delim_whitespace=True,
     dtype=str
 )
```

### Comparing `phot2lc-1.7.5/src/phot2lc/phot2lc` & `phot2lc-1.7.6/src/phot2lc/phot2lc`

 * *Files identical despite different names*

### Comparing `phot2lc-1.7.5/src/phot2lc/photfunc.py` & `phot2lc-1.7.6/src/phot2lc/photfunc.py`

 * *Files identical despite different names*

### Comparing `phot2lc-1.7.5/src/phot2lc/quicklook` & `phot2lc-1.7.6/src/phot2lc/quicklook`

 * *Files identical despite different names*

### Comparing `phot2lc-1.7.5/src/phot2lc/teledat.py` & `phot2lc-1.7.6/src/phot2lc/teledat.py`

 * *Files identical despite different names*

### Comparing `phot2lc-1.7.5/src/phot2lc/ucm_utils.py` & `phot2lc-1.7.6/src/phot2lc/ucm_utils.py`

 * *Files identical despite different names*

### Comparing `phot2lc-1.7.5/src/phot2lc/version_history.txt` & `phot2lc-1.7.6/src/phot2lc/version_history.txt`

 * *Files 1% similar despite different names*

```diff
@@ -533,14 +533,19 @@
       addstar SDSSJ0000+1111 00:00:00.0 +11:11:11.1
 
  Version 1.7.5 (2023-04-28)
 ---------------------------
 > Minor bug fixes
 
 
+ Version 1.7.6 (2023-05-02)
+---------------------------
+> Minor bug fixes in addstar
+
+
```

### Comparing `phot2lc-1.7.5/src/phot2lc/weldlc` & `phot2lc-1.7.6/src/phot2lc/weldlc`

 * *Files identical despite different names*

### Comparing `phot2lc-1.7.5/src/phot2lc.egg-info/PKG-INFO` & `phot2lc-1.7.6/src/phot2lc.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phot2lc
-Version: 1.7.5
+Version: 1.7.6
 Summary: Light curve extraction
 Home-page: https://github.com/zvanderbosch/phot2lc
 Author: Zach Vanderbosch
 Author-email: zvanderbosch@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
```

