# Comparing `tmp/dl_utils385-0.9.3.tar.gz` & `tmp/dl_utils385-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/louis/dl_utils_python_pkg/dist/tmpda1t7va8/dl_utils385-0.9.3.tar", last modified: Mon Mar  7 10:44:50 2022, max compression
+gzip compressed data, was "/home/louis/dl_utils_python_pkg/dist/tmplmcdnml5/dl_utils385-0.9.4.tar", last modified: Mon Mar  7 10:55:34 2022, max compression
```

## Comparing `dl_utils385-0.9.3.tar` & `dl_utils385-0.9.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2022-03-07 10:44:50.000000 dl_utils385-0.9.3/
--rw-r--r--   0 louis     (1000) louis     (1000)     1070 2021-05-03 16:19:56.000000 dl_utils385-0.9.3/LICENSE
--rw-r--r--   0 louis     (1000) louis     (1000)      507 2022-03-07 10:44:50.000000 dl_utils385-0.9.3/PKG-INFO
--rw-r--r--   0 louis     (1000) louis     (1000)       39 2021-05-03 16:19:40.000000 dl_utils385-0.9.3/README.md
--rw-r--r--   0 louis     (1000) louis     (1000)      104 2021-05-04 12:42:08.000000 dl_utils385-0.9.3/pyproject.toml
--rw-r--r--   0 louis     (1000) louis     (1000)      551 2022-03-07 10:44:50.000000 dl_utils385-0.9.3/setup.cfg
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2022-03-07 10:44:50.000000 dl_utils385-0.9.3/src/
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2022-03-07 10:44:50.000000 dl_utils385-0.9.3/src/dl_utils/
--rw-r--r--   0 louis     (1000) louis     (1000)        0 2021-05-04 12:50:53.000000 dl_utils385-0.9.3/src/dl_utils/__init__.py
--rw-r--r--   0 louis     (1000) louis     (1000)    13348 2022-03-05 16:04:25.000000 dl_utils385-0.9.3/src/dl_utils/label_funcs.py
--rw-r--r--   0 louis     (1000) louis     (1000)     7661 2022-01-03 11:53:11.000000 dl_utils385-0.9.3/src/dl_utils/misc.py
--rw-r--r--   0 louis     (1000) louis     (1000)     6138 2021-05-03 16:03:22.000000 dl_utils385-0.9.3/src/dl_utils/nns.py
--rw-r--r--   0 louis     (1000) louis     (1000)     2641 2021-05-03 16:31:19.000000 dl_utils385-0.9.3/src/dl_utils/probs.py
--rw-r--r--   0 louis     (1000) louis     (1000)     2239 2022-03-07 10:44:33.000000 dl_utils385-0.9.3/src/dl_utils/tensor_funcs.py
--rw-r--r--   0 louis     (1000) louis     (1000)     8676 2021-05-03 16:03:17.000000 dl_utils385-0.9.3/src/dl_utils/vision_dsets.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2022-03-07 10:44:50.000000 dl_utils385-0.9.3/src/dl_utils385.egg-info/
--rw-r--r--   0 louis     (1000) louis     (1000)      507 2022-03-07 10:44:50.000000 dl_utils385-0.9.3/src/dl_utils385.egg-info/PKG-INFO
--rw-r--r--   0 louis     (1000) louis     (1000)      372 2022-03-07 10:44:50.000000 dl_utils385-0.9.3/src/dl_utils385.egg-info/SOURCES.txt
--rw-r--r--   0 louis     (1000) louis     (1000)        1 2022-03-07 10:44:50.000000 dl_utils385-0.9.3/src/dl_utils385.egg-info/dependency_links.txt
--rw-r--r--   0 louis     (1000) louis     (1000)        9 2022-03-07 10:44:50.000000 dl_utils385-0.9.3/src/dl_utils385.egg-info/top_level.txt
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2022-03-07 10:55:34.000000 dl_utils385-0.9.4/
+-rw-r--r--   0 louis     (1000) louis     (1000)     1070 2021-05-03 16:19:56.000000 dl_utils385-0.9.4/LICENSE
+-rw-r--r--   0 louis     (1000) louis     (1000)      507 2022-03-07 10:55:34.000000 dl_utils385-0.9.4/PKG-INFO
+-rw-r--r--   0 louis     (1000) louis     (1000)       39 2021-05-03 16:19:40.000000 dl_utils385-0.9.4/README.md
+-rw-r--r--   0 louis     (1000) louis     (1000)      104 2021-05-04 12:42:08.000000 dl_utils385-0.9.4/pyproject.toml
+-rw-r--r--   0 louis     (1000) louis     (1000)      551 2022-03-07 10:55:34.000000 dl_utils385-0.9.4/setup.cfg
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2022-03-07 10:55:34.000000 dl_utils385-0.9.4/src/
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2022-03-07 10:55:34.000000 dl_utils385-0.9.4/src/dl_utils/
+-rw-r--r--   0 louis     (1000) louis     (1000)        0 2021-05-04 12:50:53.000000 dl_utils385-0.9.4/src/dl_utils/__init__.py
+-rw-r--r--   0 louis     (1000) louis     (1000)    13348 2022-03-05 16:04:25.000000 dl_utils385-0.9.4/src/dl_utils/label_funcs.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     7661 2022-01-03 11:53:11.000000 dl_utils385-0.9.4/src/dl_utils/misc.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     6138 2021-05-03 16:03:22.000000 dl_utils385-0.9.4/src/dl_utils/nns.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     2641 2021-05-03 16:31:19.000000 dl_utils385-0.9.4/src/dl_utils/probs.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     2320 2022-03-07 10:54:07.000000 dl_utils385-0.9.4/src/dl_utils/tensor_funcs.py
+-rw-r--r--   0 louis     (1000) louis     (1000)     8676 2021-05-03 16:03:17.000000 dl_utils385-0.9.4/src/dl_utils/vision_dsets.py
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2022-03-07 10:55:34.000000 dl_utils385-0.9.4/src/dl_utils385.egg-info/
+-rw-r--r--   0 louis     (1000) louis     (1000)      507 2022-03-07 10:55:33.000000 dl_utils385-0.9.4/src/dl_utils385.egg-info/PKG-INFO
+-rw-r--r--   0 louis     (1000) louis     (1000)      372 2022-03-07 10:55:34.000000 dl_utils385-0.9.4/src/dl_utils385.egg-info/SOURCES.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)        1 2022-03-07 10:55:33.000000 dl_utils385-0.9.4/src/dl_utils385.egg-info/dependency_links.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)        9 2022-03-07 10:55:34.000000 dl_utils385-0.9.4/src/dl_utils385.egg-info/top_level.txt
```

### Comparing `dl_utils385-0.9.3/LICENSE` & `dl_utils385-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dl_utils385-0.9.3/setup.cfg` & `dl_utils385-0.9.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dl_utils385
-version = 0.9.3
+version = 0.9.4
 author = Louis Mahon
 author_email = oneillml@tcd.ie
 description = Useful code for deep learning projects
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Lou1sM/dl_utils
 classifiers =
```

### Comparing `dl_utils385-0.9.3/src/dl_utils/label_funcs.py` & `dl_utils385-0.9.4/src/dl_utils/label_funcs.py`

 * *Files identical despite different names*

### Comparing `dl_utils385-0.9.3/src/dl_utils/misc.py` & `dl_utils385-0.9.4/src/dl_utils/misc.py`

 * *Files identical despite different names*

### Comparing `dl_utils385-0.9.3/src/dl_utils/nns.py` & `dl_utils385-0.9.4/src/dl_utils/nns.py`

 * *Files identical despite different names*

### Comparing `dl_utils385-0.9.3/src/dl_utils/probs.py` & `dl_utils385-0.9.4/src/dl_utils/probs.py`

 * *Files identical despite different names*

### Comparing `dl_utils385-0.9.3/src/dl_utils/tensor_funcs.py` & `dl_utils385-0.9.4/src/dl_utils/tensor_funcs.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,17 +21,19 @@
     if len(boolean_arrays) == 1: return boolean_arrays[0]
     return np.logical_or(boolean_arrays[0],recursive_np_or(boolean_arrays[1:]))
 
 def recursive_np_and(boolean_arrays):
     if len(boolean_arrays) == 1: return boolean_arrays[0]
     return np.logical_and(boolean_arrays[0],recursive_np_and(boolean_arrays[1:]))
 
-def np_load_all(dir_name,comb_method='stack'):
+def np_load_all(dir_name,comb_method='stack',restrict=-1):
     all_fnames = os.listdir(dir_name)
-    all_arrs = [np.load(os.path.join(dir_name,fn)) for fn in all_fnames]
+    if restrict == -1:
+        restrict = len(all_fnames)
+    all_arrs = [np.load(os.path.join(dir_name,fn)) for fn in all_fnames[:restrict]]
     if comb_method=='none':
         return all_arrs
     elif comb_method=='cat':
         return np.concatenate(all_arrs)
     elif comb_method=='stack':
         return np.stack(all_arrs)
```

### Comparing `dl_utils385-0.9.3/src/dl_utils/vision_dsets.py` & `dl_utils385-0.9.4/src/dl_utils/vision_dsets.py`

 * *Files identical despite different names*

