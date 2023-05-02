# Comparing `tmp/setuptools_dso-2.7a1.tar.gz` & `tmp/setuptools_dso-2.8a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/setuptools_dso-2.7a1.tar", last modified: Fri Feb  3 20:43:54 2023, max compression
+gzip compressed data, was "dist/setuptools_dso-2.8a1.tar", last modified: Tue May  2 20:00:31 2023, max compression
```

## Comparing `setuptools_dso-2.7a1.tar` & `setuptools_dso-2.8a1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 20:43:54.000000 setuptools_dso-2.7a1/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-03 20:43:39.000000 setuptools_dso-2.7a1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-02-03 20:43:39.000000 setuptools_dso-2.7a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-02-03 20:43:39.000000 setuptools_dso-2.7a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-02-03 20:43:54.000000 setuptools_dso-2.7a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-02-03 20:43:39.000000 setuptools_dso-2.7a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-03 20:43:39.000000 setuptools_dso-2.7a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-03 20:43:54.000000 setuptools_dso-2.7a1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1357 2023-02-03 20:43:39.000000 setuptools_dso-2.7a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 20:43:54.000000 setuptools_dso-2.7a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 20:43:54.000000 setuptools_dso-2.7a1/src/setuptools_dso/
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-02-03 20:43:39.000000 setuptools_dso-2.7a1/src/setuptools_dso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-02-03 20:43:39.000000 setuptools_dso-2.7a1/src/setuptools_dso/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    24211 2023-02-03 20:43:39.000000 setuptools_dso-2.7a1/src/setuptools_dso/dsocmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    16544 2023-02-03 20:43:39.000000 setuptools_dso-2.7a1/src/setuptools_dso/probe.py
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-02-03 20:43:39.000000 setuptools_dso-2.7a1/src/setuptools_dso/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 20:43:54.000000 setuptools_dso-2.7a1/src/setuptools_dso/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 20:43:39.000000 setuptools_dso-2.7a1/src/setuptools_dso/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-02-03 20:43:39.000000 setuptools_dso-2.7a1/src/setuptools_dso/test/test_probe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 20:43:54.000000 setuptools_dso-2.7a1/src/setuptools_dso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-02-03 20:43:54.000000 setuptools_dso-2.7a1/src/setuptools_dso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-02-03 20:43:54.000000 setuptools_dso-2.7a1/src/setuptools_dso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 20:43:54.000000 setuptools_dso-2.7a1/src/setuptools_dso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-03 20:43:54.000000 setuptools_dso-2.7a1/src/setuptools_dso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-03 20:43:54.000000 setuptools_dso-2.7a1/src/setuptools_dso.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:00:31.000000 setuptools_dso-2.8a1/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-02 20:00:17.000000 setuptools_dso-2.8a1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-02 20:00:17.000000 setuptools_dso-2.8a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-02 20:00:17.000000 setuptools_dso-2.8a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-02 20:00:31.000000 setuptools_dso-2.8a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 20:00:17.000000 setuptools_dso-2.8a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-02 20:00:17.000000 setuptools_dso-2.8a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-02 20:00:31.000000 setuptools_dso-2.8a1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1357 2023-05-02 20:00:17.000000 setuptools_dso-2.8a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:00:31.000000 setuptools_dso-2.8a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:00:31.000000 setuptools_dso-2.8a1/src/setuptools_dso/
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-05-02 20:00:17.000000 setuptools_dso-2.8a1/src/setuptools_dso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-05-02 20:00:17.000000 setuptools_dso-2.8a1/src/setuptools_dso/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26488 2023-05-02 20:00:17.000000 setuptools_dso-2.8a1/src/setuptools_dso/dsocmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16544 2023-05-02 20:00:17.000000 setuptools_dso-2.8a1/src/setuptools_dso/probe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-05-02 20:00:17.000000 setuptools_dso-2.8a1/src/setuptools_dso/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:00:31.000000 setuptools_dso-2.8a1/src/setuptools_dso/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:00:17.000000 setuptools_dso-2.8a1/src/setuptools_dso/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-02 20:00:17.000000 setuptools_dso-2.8a1/src/setuptools_dso/test/test_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-02 20:00:17.000000 setuptools_dso-2.8a1/src/setuptools_dso/test/test_probe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:00:31.000000 setuptools_dso-2.8a1/src/setuptools_dso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-02 20:00:31.000000 setuptools_dso-2.8a1/src/setuptools_dso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-02 20:00:31.000000 setuptools_dso-2.8a1/src/setuptools_dso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:00:31.000000 setuptools_dso-2.8a1/src/setuptools_dso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-02 20:00:31.000000 setuptools_dso-2.8a1/src/setuptools_dso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-02 20:00:31.000000 setuptools_dso-2.8a1/src/setuptools_dso.egg-info/top_level.txt
```

### Comparing `setuptools_dso-2.7a1/LICENSE` & `setuptools_dso-2.8a1/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools_dso-2.7a1/PKG-INFO` & `setuptools_dso-2.8a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools_dso
-Version: 2.7a1
+Version: 2.8a1
 Summary: setuptools extension to build non-python shared libraries
 Home-page: https://github.com/mdavidsaver/setuptools_dso
 Author: Michael Davidsaver
 Author-email: mdavidsaver@gmail.com
 License: BSD
 Project-URL: Documentation, https://mdavidsaver.github.io/setuptools_dso
 Project-URL: Release Notes, https://mdavidsaver.github.io/setuptools_dso/releasenotes.html
```

### Comparing `setuptools_dso-2.7a1/README.md` & `setuptools_dso-2.8a1/README.md`

 * *Files identical despite different names*

### Comparing `setuptools_dso-2.7a1/setup.py` & `setuptools_dso-2.8a1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as F:
     long_description = F.read()
 
 setup(
     name='setuptools_dso',
-    version="2.7a1",
+    version="2.8a1",
     description="setuptools extension to build non-python shared libraries",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/mdavidsaver/setuptools_dso',
     project_urls={
         'Documentation':'https://mdavidsaver.github.io/setuptools_dso',
         'Release Notes':'https://mdavidsaver.github.io/setuptools_dso/releasenotes.html',
```

### Comparing `setuptools_dso-2.7a1/src/setuptools_dso/__init__.py` & `setuptools_dso-2.8a1/src/setuptools_dso/__init__.py`

 * *Files identical despite different names*

### Comparing `setuptools_dso-2.7a1/src/setuptools_dso/compiler.py` & `setuptools_dso-2.8a1/src/setuptools_dso/compiler.py`

 * *Files identical despite different names*

### Comparing `setuptools_dso-2.7a1/src/setuptools_dso/dsocmd.py` & `setuptools_dso-2.8a1/src/setuptools_dso/dsocmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright 2022  Michael Davidsaver
 # SPDX-License-Identifier: BSD
 # See LICENSE
 import sys
 import os
+import re
 
 from collections import defaultdict
 from importlib import import_module # say that three times fast...
 from multiprocessing import Pool
 import multiprocessing as MP
 
 try:
@@ -60,14 +61,73 @@
                 self._F = fn, args, kws
             def get(self):
                 fn, args, kws = self._F
                 return fn(*args, **kws)
         def apply_async(self, fn, args, kws):
             return self.DummyJob(fn, args, kws)
 
+def _system_concurrency():
+    if 'NUM_JOBS' in os.environ: # because it is so very cumbersome to pass extra build args through pip and setuptools ...
+        # we trust that our user knows what is being requested...
+        return int(os.environ['NUM_JOBS'])
+
+    # from this point, fail softly
+
+    # find available CPU concurrency
+    if hasattr(os, 'cpu_count'): # py3
+        njobs = os.cpu_count()
+    else:
+        njobs = 2 # why not?
+
+    # estimate available memory concurrency.  (lots of swapping erases any benefit of parallel compile)
+    nmem = njobs
+    if os.path.isfile('/proc/meminfo'): # Linux
+        meminfo={}
+        units = {
+            'kB': 1024,
+            None: 1,
+        }
+        # lines like:
+        #   MemTotal:       15951564 kB
+        #   HugePages_Total:       0
+        pat = re.compile(r'([^:]+):\s*([0-9]+)\s*(\S+)?')
+        with open('/proc/meminfo', 'r') as F:
+            for L in F:
+                M = pat.match(L)
+                if M is not None:
+                    name, val, unit = M.groups()
+                    meminfo[name] = float(val)*units[unit]
+                # else: # ignore unknown lines
+
+        avail_phy = meminfo.get('MemAvailable') # physical unused and disk cache
+        if avail_phy:
+            # Estimated peak physical RAM usage for a single GCC run.
+            # Measured max RSS for a single GCC run when compiling epics-base circa 7.0.7 is ~130 MB.
+            job_max_mem = 128 * 2**20
+            # Arbitrarily multiply because I don't have confidence in the generality of this measurement.
+            job_max_mem *= 4
+
+            nmem = int(avail_phy / job_max_mem)
+
+    njobs = max(1, min(njobs, nmem))
+
+    return njobs
+
+
+def system_concurrency():
+    """Estimate the number of concurrent compile jobs this system can perform.
+    
+    Tries to use both available CPU and memory resource information.
+    """
+    try:
+        return _system_concurrency()
+    except Exception as e: # fail softly with a pessimistic estimate
+        log.warn('Warning: Unable to estimate system concurrency, default to sequential build: %r'%e)
+        return 1
+
 def massage_dir_list(bdirs, indirs):
     """Process a list of directories for use with -I or -L
     For relative paths, also include paths relative to a build directory
     """
     indirs = indirs or []
     dirs = indirs[:]
 
@@ -344,21 +404,16 @@
         # sort by language
         for src in sources:
             SRC[self.compiler.language_map[os.path.splitext(src)[-1]]].append(src)
 
         # do the actual compiling
         objects = []
 
-        if 'NUM_JOBS' in os.environ: # because it is so very cumbersome to pass extra build args through pip and setuptools ...
-            nworkers = int(os.environ['NUM_JOBS'])
-        elif hasattr(os, 'cpu_count'): # py3
-            nworkers = os.cpu_count()
-        else:
-            nworkers = 2 # why not?
-
+        nworkers = system_concurrency()
+        log.info('effective NUM_JOBS=%d'%nworkers)
         with Pool(nworkers) as P:
             jobs = []
             for lang, srcs in SRC.items():
 
                 # submit jobs
                 # allocate every n-th object to the n-th worker.
                 # Load not well balanced, but easy to do.
@@ -390,15 +445,17 @@
             # this install_name will be replaced below (cf. 'install_name_tool')
             extra_args.extend(['-install_name', '@rpath/%s'%solibbase])
 
         elif sys.platform == "win32":
             # The .lib is considered "temporary" for extensions, but not for us
             # so we pass export_symbols=None and put it along side the .dll
             # eg. "pkg\mod\mylib.dll" and "pkg\mod\mylib.lib"
-            extra_args.append('/IMPLIB:%s.lib'%(os.path.splitext(outlib)[0]))
+            outlib_lib = '%s.lib' % os.path.splitext(outlib)[0]
+            outlib_exp = '%s.exp' % os.path.splitext(outlib)[0]
+            extra_args.append('/IMPLIB:%s'%outlib_lib)
 
         elif baselib!=solib: # ELF
             extra_args.extend(['-Wl,-h,%s'%solibbase])
 
         language = dso.language or self.compiler.detect_language(sources)
 
         self.compiler.link_shared_object(
@@ -424,21 +481,25 @@
             #self.copy_file(outlib, outbaselib) # link="sym" seem to get the target path wrong
 
         if self.inplace:
             build_py = self.get_finalized_command('build_py')
             pkg = '.'.join(dso.name.split('.')[:-1])    # path.to.dso -> path.to
             pkgdir = build_py.get_package_dir(pkg)      # path.to -> src/path/to
 
-            solib_dst   = os.path.join(pkgdir, os.path.basename(solib))     # path/to/dso.so -> src/path/to/dso.so
-            baselib_dst = os.path.join(pkgdir, os.path.basename(baselib))
+            def inplace_dst(path): # build/.../path/to/dso.so -> src/path/to/dso.so
+                return os.path.join(pkgdir, os.path.basename(path))
 
-            self.mkpath(os.path.dirname(solib_dst))
-            self.copy_file(outlib, solib_dst)
+            self.mkpath(os.path.dirname(inplace_dst(outlib)))
+            self.copy_file(outlib, inplace_dst(outlib))
             if baselib!=solib:
-                self.copy_file(outbaselib, baselib_dst)
+                self.copy_file(outbaselib, inplace_dst(outbaselib))
+            if sys.platform == "win32":
+                # on windows linking to x.dll goes through x.lib and x.exp first
+                self.copy_file(outlib_lib, inplace_dst(outlib_lib))
+                self.copy_file(outlib_exp, inplace_dst(outlib_exp))
 
     def gen_info_module(self, dso):
         if not dso.gen_info:
             log.debug("skiping creation of info module")
             return
 
         parts = dso.name.split(".")
```

### Comparing `setuptools_dso-2.7a1/src/setuptools_dso/probe.py` & `setuptools_dso-2.8a1/src/setuptools_dso/probe.py`

 * *Files identical despite different names*

### Comparing `setuptools_dso-2.7a1/src/setuptools_dso/runtime.py` & `setuptools_dso-2.8a1/src/setuptools_dso/runtime.py`

 * *Files identical despite different names*

### Comparing `setuptools_dso-2.7a1/src/setuptools_dso/test/test_probe.py` & `setuptools_dso-2.8a1/src/setuptools_dso/test/test_probe.py`

 * *Files identical despite different names*

### Comparing `setuptools_dso-2.7a1/src/setuptools_dso.egg-info/PKG-INFO` & `setuptools_dso-2.8a1/src/setuptools_dso.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-dso
-Version: 2.7a1
+Version: 2.8a1
 Summary: setuptools extension to build non-python shared libraries
 Home-page: https://github.com/mdavidsaver/setuptools_dso
 Author: Michael Davidsaver
 Author-email: mdavidsaver@gmail.com
 License: BSD
 Project-URL: Documentation, https://mdavidsaver.github.io/setuptools_dso
 Project-URL: Release Notes, https://mdavidsaver.github.io/setuptools_dso/releasenotes.html
```

