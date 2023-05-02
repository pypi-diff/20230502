# Comparing `tmp/pseudo_labeller-0.0.6.tar.gz` & `tmp/pseudo_labeller-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pseudo_labeller-0.0.6.tar", last modified: Thu Apr 27 13:52:36 2023, max compression
+gzip compressed data, was "pseudo_labeller-0.0.7.tar", last modified: Tue May  2 08:17:32 2023, max compression
```

## Comparing `pseudo_labeller-0.0.6.tar` & `pseudo_labeller-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:52:36.758310 pseudo_labeller-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-27 13:52:24.000000 pseudo_labeller-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-27 13:52:24.000000 pseudo_labeller-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-27 13:52:36.758310 pseudo_labeller-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-27 13:52:24.000000 pseudo_labeller-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:52:36.758310 pseudo_labeller-0.0.6/pseudo_labeller/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 13:52:24.000000 pseudo_labeller-0.0.6/pseudo_labeller/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:52:36.758310 pseudo_labeller-0.0.6/pseudo_labeller/model/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-27 13:52:24.000000 pseudo_labeller-0.0.6/pseudo_labeller/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-04-27 13:52:24.000000 pseudo_labeller-0.0.6/pseudo_labeller/model/idam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:52:36.758310 pseudo_labeller-0.0.6/pseudo_labeller/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 13:52:24.000000 pseudo_labeller-0.0.6/pseudo_labeller/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:52:36.758310 pseudo_labeller-0.0.6/pseudo_labeller.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-27 13:52:36.000000 pseudo_labeller-0.0.6/pseudo_labeller.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-27 13:52:36.000000 pseudo_labeller-0.0.6/pseudo_labeller.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 13:52:36.000000 pseudo_labeller-0.0.6/pseudo_labeller.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-27 13:52:36.000000 pseudo_labeller-0.0.6/pseudo_labeller.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-27 13:52:36.000000 pseudo_labeller-0.0.6/pseudo_labeller.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-27 13:52:24.000000 pseudo_labeller-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 13:52:36.758310 pseudo_labeller-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-27 13:52:24.000000 pseudo_labeller-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:17:32.523584 pseudo_labeller-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-02 08:17:21.000000 pseudo_labeller-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 08:17:21.000000 pseudo_labeller-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-02 08:17:32.523584 pseudo_labeller-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-02 08:17:21.000000 pseudo_labeller-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:17:32.523584 pseudo_labeller-0.0.7/pseudo_labeller/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 08:17:21.000000 pseudo_labeller-0.0.7/pseudo_labeller/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:17:32.523584 pseudo_labeller-0.0.7/pseudo_labeller/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-02 08:17:21.000000 pseudo_labeller-0.0.7/pseudo_labeller/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-05-02 08:17:21.000000 pseudo_labeller-0.0.7/pseudo_labeller/model/idam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:17:32.523584 pseudo_labeller-0.0.7/pseudo_labeller/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 08:17:21.000000 pseudo_labeller-0.0.7/pseudo_labeller/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:17:32.523584 pseudo_labeller-0.0.7/pseudo_labeller.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-02 08:17:32.000000 pseudo_labeller-0.0.7/pseudo_labeller.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-02 08:17:32.000000 pseudo_labeller-0.0.7/pseudo_labeller.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 08:17:32.000000 pseudo_labeller-0.0.7/pseudo_labeller.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-02 08:17:32.000000 pseudo_labeller-0.0.7/pseudo_labeller.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 08:17:32.000000 pseudo_labeller-0.0.7/pseudo_labeller.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-02 08:17:21.000000 pseudo_labeller-0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 08:17:32.523584 pseudo_labeller-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-02 08:17:21.000000 pseudo_labeller-0.0.7/setup.py
```

### Comparing `pseudo_labeller-0.0.6/LICENSE` & `pseudo_labeller-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pseudo_labeller-0.0.6/pseudo_labeller/model/idam.py` & `pseudo_labeller-0.0.7/pseudo_labeller/model/idam.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,9 +137,11 @@
             return x
         pv_meta = self.pv_meta_input(pv_meta)
         pv_meta = self.batch_norm_meta(pv_meta)
         pv_meta = F.relu(pv_meta)
         # Reshape to fit into 3DCNN
         x = torch.cat([x, pv_meta], dim=1)
         # Get pv_meta_output
-        x = F.relu(self.pv_meta_output(self.batch_norm_output_meta(x)))  # Generation can only be positive or 0, so ReLU
+        x = F.relu(
+            self.pv_meta_output(self.batch_norm_output_meta(x))
+        )  # Generation can only be positive or 0, so ReLU
         return x
```

### Comparing `pseudo_labeller-0.0.6/setup.py` & `pseudo_labeller-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 install_requires = (this_directory / "requirements.txt").read_text().splitlines()
 
 setup(
     name="pseudo_labeller",
-    version="0.0.6",
+    version="0.0.7",
     license="MIT",
     description="Psuedo PV/Irradience Labeller",
     author="Jacob Bieker",
     author_email="info@openclimatefix.org",
     company="Open Climate Fix Ltd",
     install_requires=install_requires,
     long_description=long_description,
```

