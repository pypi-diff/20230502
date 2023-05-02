# Comparing `tmp/cwl-upgrader-1.2.4.tar.gz` & `tmp/cwl-upgrader-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cwl-upgrader-1.2.4.tar", last modified: Thu Sep  8 15:23:08 2022, max compression
+gzip compressed data, was "cwl-upgrader-1.2.5.tar", last modified: Tue May  2 07:47:22 2023, max compression
```

## Comparing `cwl-upgrader-1.2.4.tar` & `cwl-upgrader-1.2.5.tar`

### file list

```diff
@@ -1,44 +1,50 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-09-08 15:23:08.587624 cwl-upgrader-1.2.4/
--rw-r--r--   0 michael   (1000) michael   (1000)    11358 2022-09-08 15:22:56.000000 cwl-upgrader-1.2.4/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       91 2022-09-08 15:22:56.000000 cwl-upgrader-1.2.4/MANIFEST.in
--rw-r--r--   0 michael   (1000) michael   (1000)     6361 2022-09-08 15:22:56.000000 cwl-upgrader-1.2.4/Makefile
--rw-r--r--   0 michael   (1000) michael   (1000)     2484 2022-09-08 15:23:08.587624 cwl-upgrader-1.2.4/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      992 2022-09-08 15:22:56.000000 cwl-upgrader-1.2.4/README.rst
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-09-08 15:23:08.583624 cwl-upgrader-1.2.4/cwl_upgrader.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)     2484 2022-09-08 15:23:08.000000 cwl-upgrader-1.2.4/cwl_upgrader.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      912 2022-09-08 15:23:08.000000 cwl-upgrader-1.2.4/cwl_upgrader.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2022-09-08 15:23:08.000000 cwl-upgrader-1.2.4/cwl_upgrader.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       56 2022-09-08 15:23:08.000000 cwl-upgrader-1.2.4/cwl_upgrader.egg-info/entry_points.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      228 2022-09-08 15:23:08.000000 cwl-upgrader-1.2.4/cwl_upgrader.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       12 2022-09-08 15:23:08.000000 cwl-upgrader-1.2.4/cwl_upgrader.egg-info/top_level.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2022-09-08 15:23:02.000000 cwl-upgrader-1.2.4/cwl_upgrader.egg-info/zip-safe
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-09-08 15:23:08.583624 cwl-upgrader-1.2.4/cwlupgrader/
--rw-r--r--   0 michael   (1000) michael   (1000)       79 2022-09-08 15:22:56.000000 cwl-upgrader-1.2.4/cwlupgrader/__init__.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    30991 2022-09-08 15:22:56.000000 cwl-upgrader-1.2.4/cwlupgrader/main.py
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2022-09-08 15:22:56.000000 cwl-upgrader-1.2.4/cwlupgrader/py.typed
--rw-r--r--   0 michael   (1000) michael   (1000)      395 2022-09-08 15:23:08.587624 cwl-upgrader-1.2.4/setup.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)     2305 2022-09-08 15:22:56.000000 cwl-upgrader-1.2.4/setup.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-09-08 15:23:08.579624 cwl-upgrader-1.2.4/testdata/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-09-08 15:23:08.583624 cwl-upgrader-1.2.4/testdata/draft-3/
--rw-r--r--   0 michael   (1000) michael   (1000)    11102 2022-09-08 15:22:56.000000 cwl-upgrader-1.2.4/testdata/draft-3/attributor-prok-cheetah.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      625 2022-09-08 15:22:56.000000 cwl-upgrader-1.2.4/testdata/draft-3/wf.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-09-08 15:23:08.583624 cwl-upgrader-1.2.4/testdata/v1.0/
--rwxr-xr-x   0 michael   (1000) michael   (1000)     8843 2022-09-08 15:22:56.000000 cwl-upgrader-1.2.4/testdata/v1.0/attributor-prok-cheetah.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1157 2022-09-08 15:22:56.000000 cwl-upgrader-1.2.4/testdata/v1.0/conflict-wf.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      312 2022-09-08 15:22:56.000000 cwl-upgrader-1.2.4/testdata/v1.0/listing_deep1-arr.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      307 2022-09-08 15:22:56.000000 cwl-upgrader-1.2.4/testdata/v1.0/listing_deep1.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      219 2022-09-08 15:22:56.000000 cwl-upgrader-1.2.4/testdata/v1.0/networkaccess.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      489 2022-09-08 15:22:56.000000 cwl-upgrader-1.2.4/testdata/v1.0/wf.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-09-08 15:23:08.583624 cwl-upgrader-1.2.4/testdata/v1.1/
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1425 2022-09-08 15:22:56.000000 cwl-upgrader-1.2.4/testdata/v1.1/conflict-wf.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      425 2022-09-08 15:22:56.000000 cwl-upgrader-1.2.4/testdata/v1.1/listing_deep1-arr.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      404 2022-09-08 15:22:56.000000 cwl-upgrader-1.2.4/testdata/v1.1/listing_deep1.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      330 2022-09-08 15:22:56.000000 cwl-upgrader-1.2.4/testdata/v1.1/networkaccess.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-09-08 15:23:08.583624 cwl-upgrader-1.2.4/testdata/v1.2/
--rwxr-xr-x   0 michael   (1000) michael   (1000)      404 2022-09-08 15:22:56.000000 cwl-upgrader-1.2.4/testdata/v1.2/listing_deep1.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      330 2022-09-08 15:22:56.000000 cwl-upgrader-1.2.4/testdata/v1.2/networkaccess.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-09-08 15:23:08.587624 cwl-upgrader-1.2.4/tests/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2022-09-08 15:22:56.000000 cwl-upgrader-1.2.4/tests/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3710 2022-09-08 15:22:56.000000 cwl-upgrader-1.2.4/tests/test_complete.py
--rw-r--r--   0 michael   (1000) michael   (1000)      537 2022-09-08 15:22:56.000000 cwl-upgrader-1.2.4/tests/test_output_dir.py
--rw-r--r--   0 michael   (1000) michael   (1000)      787 2022-09-08 15:22:56.000000 cwl-upgrader-1.2.4/tests/util.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-02 07:47:22.500604 cwl-upgrader-1.2.5/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11358 2023-05-02 07:47:14.000000 cwl-upgrader-1.2.5/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       91 2023-05-02 07:47:14.000000 cwl-upgrader-1.2.5/MANIFEST.in
+-rw-r--r--   0 michael   (1000) michael   (1000)     6361 2023-05-02 07:47:14.000000 cwl-upgrader-1.2.5/Makefile
+-rw-r--r--   0 michael   (1000) michael   (1000)     2484 2023-05-02 07:47:22.500604 cwl-upgrader-1.2.5/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)      992 2023-05-02 07:47:14.000000 cwl-upgrader-1.2.5/README.rst
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-02 07:47:22.496604 cwl-upgrader-1.2.5/cwl_upgrader.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2484 2023-05-02 07:47:22.000000 cwl-upgrader-1.2.5/cwl_upgrader.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)     1086 2023-05-02 07:47:22.000000 cwl-upgrader-1.2.5/cwl_upgrader.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-05-02 07:47:22.000000 cwl-upgrader-1.2.5/cwl_upgrader.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       56 2023-05-02 07:47:22.000000 cwl-upgrader-1.2.5/cwl_upgrader.egg-info/entry_points.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      228 2023-05-02 07:47:22.000000 cwl-upgrader-1.2.5/cwl_upgrader.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       12 2023-05-02 07:47:22.000000 cwl-upgrader-1.2.5/cwl_upgrader.egg-info/top_level.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-05-02 07:47:19.000000 cwl-upgrader-1.2.5/cwl_upgrader.egg-info/zip-safe
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-02 07:47:22.496604 cwl-upgrader-1.2.5/cwlupgrader/
+-rw-r--r--   0 michael   (1000) michael   (1000)       79 2023-05-02 07:47:14.000000 cwl-upgrader-1.2.5/cwlupgrader/__init__.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    34460 2023-05-02 07:47:14.000000 cwl-upgrader-1.2.5/cwlupgrader/main.py
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-02 07:47:14.000000 cwl-upgrader-1.2.5/cwlupgrader/py.typed
+-rw-r--r--   0 michael   (1000) michael   (1000)      395 2023-05-02 07:47:22.500604 cwl-upgrader-1.2.5/setup.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)     2305 2023-05-02 07:47:14.000000 cwl-upgrader-1.2.5/setup.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-02 07:47:22.496604 cwl-upgrader-1.2.5/testdata/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-02 07:47:22.496604 cwl-upgrader-1.2.5/testdata/draft-3/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11102 2023-05-02 07:47:14.000000 cwl-upgrader-1.2.5/testdata/draft-3/attributor-prok-cheetah.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      625 2023-05-02 07:47:14.000000 cwl-upgrader-1.2.5/testdata/draft-3/wf.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-02 07:47:22.500604 cwl-upgrader-1.2.5/testdata/v1.0/
+-rw-r--r--   0 michael   (1000) michael   (1000)      433 2023-05-02 07:47:14.000000 cwl-upgrader-1.2.5/testdata/v1.0/1st-workflow.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      385 2023-05-02 07:47:14.000000 cwl-upgrader-1.2.5/testdata/v1.0/arguments.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     8843 2023-05-02 07:47:14.000000 cwl-upgrader-1.2.5/testdata/v1.0/attributor-prok-cheetah.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1157 2023-05-02 07:47:14.000000 cwl-upgrader-1.2.5/testdata/v1.0/conflict-wf.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      312 2023-05-02 07:47:14.000000 cwl-upgrader-1.2.5/testdata/v1.0/listing_deep1-arr.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      307 2023-05-02 07:47:14.000000 cwl-upgrader-1.2.5/testdata/v1.0/listing_deep1.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      219 2023-05-02 07:47:14.000000 cwl-upgrader-1.2.5/testdata/v1.0/networkaccess.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      333 2023-05-02 07:47:14.000000 cwl-upgrader-1.2.5/testdata/v1.0/tar-param.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      489 2023-05-02 07:47:14.000000 cwl-upgrader-1.2.5/testdata/v1.0/wf.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-02 07:47:22.500604 cwl-upgrader-1.2.5/testdata/v1.1/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1425 2023-05-02 07:47:14.000000 cwl-upgrader-1.2.5/testdata/v1.1/conflict-wf.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      425 2023-05-02 07:47:14.000000 cwl-upgrader-1.2.5/testdata/v1.1/listing_deep1-arr.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      404 2023-05-02 07:47:14.000000 cwl-upgrader-1.2.5/testdata/v1.1/listing_deep1.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      330 2023-05-02 07:47:14.000000 cwl-upgrader-1.2.5/testdata/v1.1/networkaccess.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-02 07:47:22.500604 cwl-upgrader-1.2.5/testdata/v1.2/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      432 2023-05-02 07:47:14.000000 cwl-upgrader-1.2.5/testdata/v1.2/1st-workflow.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      495 2023-05-02 07:47:14.000000 cwl-upgrader-1.2.5/testdata/v1.2/arguments.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      404 2023-05-02 07:47:14.000000 cwl-upgrader-1.2.5/testdata/v1.2/listing_deep1.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      330 2023-05-02 07:47:14.000000 cwl-upgrader-1.2.5/testdata/v1.2/networkaccess.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      443 2023-05-02 07:47:14.000000 cwl-upgrader-1.2.5/testdata/v1.2/tar-param.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-02 07:47:22.500604 cwl-upgrader-1.2.5/tests/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-02 07:47:14.000000 cwl-upgrader-1.2.5/tests/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4215 2023-05-02 07:47:14.000000 cwl-upgrader-1.2.5/tests/test_complete.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      537 2023-05-02 07:47:14.000000 cwl-upgrader-1.2.5/tests/test_output_dir.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      787 2023-05-02 07:47:14.000000 cwl-upgrader-1.2.5/tests/util.py
```

### Comparing `cwl-upgrader-1.2.4/LICENSE.txt` & `cwl-upgrader-1.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cwl-upgrader-1.2.4/Makefile` & `cwl-upgrader-1.2.5/Makefile`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 # `[[` conditional expressions.
 PYSOURCES=$(wildcard cwlupgrader/**.py tests/*.py) setup.py
 DEVPKGS=diff_cover black pylint pep257 pydocstyle flake8 tox tox-pyenv \
 	isort wheel autoflake flake8-bugbear pyupgrade bandit \
 	-rtest-requirements.txt -rmypy-requirements.txt
 DEBDEVPKGS=pylint python3-coverage sloccount \
 	   python3-flake8 shellcheck
-VERSION=1.2.4  # please also update setup.py
+VERSION=1.2.5  # please also update setup.py
 
 ## all                    : default task (install cwl-upgrader in dev mode)
 all: dev
 
 ## help                   : print this help message and exit
 help: Makefile
 	@sed -n 's/^##//p' $<
```

### Comparing `cwl-upgrader-1.2.4/PKG-INFO` & `cwl-upgrader-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: cwl-upgrader
-Version: 1.2.4
+Version: 1.2.5
 Summary: Common Workflow Language standalone document upgrader
 Home-page: https://github.com/common-workflow-language/cwl-upgrader
 Author: Common Workflow Language contributors
 Author-email: common-workflow-language@googlegroups.com
 License: Apache 2.0
 Download-URL: https://github.com/common-workflow-language/cwl-upgrader
 Description: =====================================================
```

### Comparing `cwl-upgrader-1.2.4/README.rst` & `cwl-upgrader-1.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `cwl-upgrader-1.2.4/cwl_upgrader.egg-info/PKG-INFO` & `cwl-upgrader-1.2.5/cwl_upgrader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: cwl-upgrader
-Version: 1.2.4
+Version: 1.2.5
 Summary: Common Workflow Language standalone document upgrader
 Home-page: https://github.com/common-workflow-language/cwl-upgrader
 Author: Common Workflow Language contributors
 Author-email: common-workflow-language@googlegroups.com
 License: Apache 2.0
 Download-URL: https://github.com/common-workflow-language/cwl-upgrader
 Description: =====================================================
```

### Comparing `cwl-upgrader-1.2.4/cwl_upgrader.egg-info/SOURCES.txt` & `cwl-upgrader-1.2.5/cwl_upgrader.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -12,23 +12,29 @@
 cwl_upgrader.egg-info/top_level.txt
 cwl_upgrader.egg-info/zip-safe
 cwlupgrader/__init__.py
 cwlupgrader/main.py
 cwlupgrader/py.typed
 testdata/draft-3/attributor-prok-cheetah.cwl
 testdata/draft-3/wf.cwl
+testdata/v1.0/1st-workflow.cwl
+testdata/v1.0/arguments.cwl
 testdata/v1.0/attributor-prok-cheetah.cwl
 testdata/v1.0/conflict-wf.cwl
 testdata/v1.0/listing_deep1-arr.cwl
 testdata/v1.0/listing_deep1.cwl
 testdata/v1.0/networkaccess.cwl
+testdata/v1.0/tar-param.cwl
 testdata/v1.0/wf.cwl
 testdata/v1.1/conflict-wf.cwl
 testdata/v1.1/listing_deep1-arr.cwl
 testdata/v1.1/listing_deep1.cwl
 testdata/v1.1/networkaccess.cwl
+testdata/v1.2/1st-workflow.cwl
+testdata/v1.2/arguments.cwl
 testdata/v1.2/listing_deep1.cwl
 testdata/v1.2/networkaccess.cwl
+testdata/v1.2/tar-param.cwl
 tests/__init__.py
 tests/test_complete.py
 tests/test_output_dir.py
 tests/util.py
```

### Comparing `cwl-upgrader-1.2.4/cwlupgrader/main.py` & `cwl-upgrader-1.2.5/cwlupgrader/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -195,15 +195,20 @@
     Will also prepend "#!/usr/bin/env cwl-runner\n" and
     set the executable bit if it is a CWL document.
     """
     ruamel.yaml.scalarstring.walk_tree(document)
     path = Path(dirname) / name
     with open(path, "w") as handle:
         if "cwlVersion" in document:
-            handle.write("#!/usr/bin/env cwl-runner\n")
+            if not (
+                document.ca
+                and document.ca.comment
+                and "cwl-runner" in document.ca.comment[1][0].value
+            ):
+                handle.write("#!/usr/bin/env cwl-runner\n")
         yaml.dump(document, stream=handle)
     if "cwlVersion" in document:
         path.chmod(path.stat().st_mode | stat.S_IXUSR | stat.S_IXGRP | stat.S_IXOTH)
 
 
 def process_imports(
     document: Any, imports: Set[str], updater: Callable[[Any, str], Any], outdir: str
@@ -245,20 +250,21 @@
     document["cwlVersion"] = "v1.1"
     return sort_v1_0(document)
 
 
 def v1_0_to_v1_2(document: CommentedMap, outdir: str) -> CommentedMap:
     """CWL v1.0.x to v1.2 transformation."""
     document = v1_0_to_v1_1(document, outdir)
-    document["cwlVersion"] = "v1.2"
+    document = v1_1_to_v1_2(document, outdir)
     return document
 
 
 def v1_1_to_v1_2(document: CommentedMap, outdir: str) -> CommentedMap:
     """CWL v1.1 to v1.2 transformation."""
+    document = _v1_1_to_v1_2(document, outdir)
     document["cwlVersion"] = "v1.2"
     return document
 
 
 def draft3_to_v1_0(document: CommentedMap, outdir: str) -> CommentedMap:
     """Transformation loop."""
     _draft3_to_v1_0(document, outdir)
@@ -346,14 +352,18 @@
                     with SourceLine(steps, index, Exception):
                         upgrade_v1_0_hints_and_reqs(entry)
                         if "run" in entry and isinstance(entry["run"], CommentedMap):
                             process = entry["run"]
                             _v1_0_to_v1_1(process, outdir)
                             if "cwlVersion" in process:
                                 del process["cwlVersion"]
+                        elif isinstance(entry["run"], str) and "#" not in entry["run"]:
+                            path = Path(document.lc.filename).parent / entry["run"]
+                            process = v1_0_to_v1_1(load_cwl_document(str(path)), outdir)
+                            write_cwl_document(process, path.name, outdir)
             elif isinstance(steps, MutableMapping):
                 for step_name in steps:
                     with SourceLine(steps, step_name, Exception):
                         entry = steps[step_name]
                         upgrade_v1_0_hints_and_reqs(entry)
                         if "run" in entry:
                             if isinstance(entry["run"], CommentedMap):
@@ -409,18 +419,70 @@
         elif document["class"] == "ExpressionTool":
             move_up_loadcontents(document)
             cleanup_v1_0_input_bindings(document)
     return document
 
 
 def _v1_0_to_v1_2(document: CommentedMap, outdir: str) -> CommentedMap:
-    return _v1_0_to_v1_1(document, outdir)  # nothing needs doing for v1.2
+    document = _v1_0_to_v1_1(document, outdir)
+    return _v1_1_to_v1_2(document, outdir)
 
 
 def _v1_1_to_v1_2(document: CommentedMap, outdir: str) -> CommentedMap:
+    if "class" in document:
+        if document["class"] == "Workflow":
+            steps = document["steps"]
+            if isinstance(steps, MutableSequence):
+                for index, entry in enumerate(steps):
+                    with SourceLine(steps, index, Exception):
+                        if "run" in entry and isinstance(entry["run"], CommentedMap):
+                            process = entry["run"]
+                            _v1_1_to_v1_2(process, outdir)
+                            if "cwlVersion" in process:
+                                del process["cwlVersion"]
+
+                        elif isinstance(entry["run"], str) and "#" not in entry["run"]:
+                            if hasattr(document.lc, "filename"):
+                                dirname = Path(document.lc.filename).parent
+                            else:
+                                dirname = Path(outdir)
+                            path = dirname / entry["run"]
+                            process = v1_1_to_v1_2(load_cwl_document(str(path)), outdir)
+                            write_cwl_document(process, path.name, outdir)
+            elif isinstance(steps, MutableMapping):
+                for step_name in steps:
+                    with SourceLine(steps, step_name, Exception):
+                        entry = steps[step_name]
+                        if "run" in entry:
+                            if isinstance(entry["run"], CommentedMap):
+                                process = entry["run"]
+                                _v1_1_to_v1_2(process, outdir)
+                                if "cwlVersion" in process:
+                                    del process["cwlVersion"]
+                            elif (
+                                isinstance(entry["run"], str)
+                                and "#" not in entry["run"]
+                            ):
+                                if hasattr(document.lc, "filename"):
+                                    dirname = Path(document.lc.filename).parent
+                                else:
+                                    dirname = Path(outdir)
+                                path = dirname / entry["run"]
+                                process = v1_1_to_v1_2(
+                                    load_cwl_document(str(path)), outdir
+                                )
+                                write_cwl_document(process, path.name, outdir)
+                            elif isinstance(entry["run"], str) and "#" in entry["run"]:
+                                pass  # reference to $graph entry
+                            else:
+                                raise Exception(
+                                    "'run' entry was neither a CWL Process nor "
+                                    "a path to one: %s.",
+                                    entry["run"],
+                                )
     return document
 
 
 def cleanup_v1_0_input_bindings(document: Dict[str, Any]) -> None:
     """In v1.1 Workflow or ExpressionTool level inputBindings are deprecated."""
 
     def cleanup(inp: Dict[str, Any]) -> None:
@@ -441,18 +503,18 @@
             cleanup(entry)
     elif isinstance(inputs, MutableMapping):
         for input_name in inputs:
             cleanup(inputs[input_name])
 
 
 def move_up_loadcontents(document: Dict[str, Any]) -> None:
-    """'loadContents' is promoted up a level in CWL v1.1."""
+    """Promote 'loadContents' up a level for CWL v1.1."""
 
     def cleanup(inp: Dict[str, Any]) -> None:
-        """Move loadContents to the preferred location"""
+        """Move loadContents to the preferred location."""
         if "inputBinding" in inp:
             bindings = inp["inputBinding"]
             for field in list(bindings.keys()):
                 if field == "loadContents":
                     inp[field] = bindings.pop(field)
 
     inputs = document["inputs"]
```

### Comparing `cwl-upgrader-1.2.4/setup.py` & `cwl-upgrader-1.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 README = os.path.join(SETUP_DIR, "README.rst")
 
 NEEDS_PYTEST = {"pytest", "test", "ptr"}.intersection(sys.argv)
 PYTEST_RUNNER = ["pytest-runner", "pytest-cov"] if NEEDS_PYTEST else []
 
 setup(
     name="cwl-upgrader",
-    version="1.2.4",
+    version="1.2.5",
     description="Common Workflow Language standalone document upgrader",
     long_description=open(README).read(),
     author="Common Workflow Language contributors",
     author_email="common-workflow-language@googlegroups.com",
     url="https://github.com/common-workflow-language/cwl-upgrader",
     download_url="https://github.com/common-workflow-language/cwl-upgrader",
     license="Apache 2.0",
@@ -26,15 +26,15 @@
     package_dir={"cwlupgrader.tests": "tests"},
     package_data={"cwlupgrader.tests": ["../testdata/**/*.cwl"]},
     install_requires=[
         "setuptools",
         "ruamel.yaml >= 0.16.0, < 0.17.22;python_version>='3.10'",
         "ruamel.yaml >= 0.15.98, < 0.17.22;python_version>='3.9'",
         "ruamel.yaml >= 0.15.78, < 0.17.22;python_version>='3.8'",
-        "ruamel.yaml >= 0.15.71, < 0.17.22",
+        "ruamel.yaml >= 0.15.71, < 0.17.23",
         "schema_salad",
     ],
     entry_points={"console_scripts": ["cwl-upgrader = cwlupgrader.main:main"]},
     python_requires=">=3.6, <4",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
@@ -51,10 +51,10 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
     ],
     zip_safe=True,
     setup_requires=PYTEST_RUNNER,
-    tests_require=["pytest < 7.2.0"],
+    tests_require=["pytest < 7.4.0"],
     test_suite="tests",
 )
```

### Comparing `cwl-upgrader-1.2.4/testdata/draft-3/attributor-prok-cheetah.cwl` & `cwl-upgrader-1.2.5/testdata/draft-3/attributor-prok-cheetah.cwl`

 * *Files identical despite different names*

### Comparing `cwl-upgrader-1.2.4/testdata/draft-3/wf.cwl` & `cwl-upgrader-1.2.5/testdata/draft-3/wf.cwl`

 * *Files identical despite different names*

### Comparing `cwl-upgrader-1.2.4/testdata/v1.0/attributor-prok-cheetah.cwl` & `cwl-upgrader-1.2.5/testdata/v1.0/attributor-prok-cheetah.cwl`

 * *Files identical despite different names*

### Comparing `cwl-upgrader-1.2.4/testdata/v1.0/conflict-wf.cwl` & `cwl-upgrader-1.2.5/testdata/v1.0/conflict-wf.cwl`

 * *Files identical despite different names*

### Comparing `cwl-upgrader-1.2.4/testdata/v1.1/conflict-wf.cwl` & `cwl-upgrader-1.2.5/testdata/v1.1/conflict-wf.cwl`

 * *Files identical despite different names*

### Comparing `cwl-upgrader-1.2.4/tests/test_complete.py` & `cwl-upgrader-1.2.5/tests/test_complete.py`

 * *Files 16% similar despite different names*

```diff
@@ -95,7 +95,23 @@
         [f"--dir={tmp_path}", "--v1.1-only", get_data("testdata/v1.0/conflict-wf.cwl")]
     )
     assert filecmp.cmp(
         get_data("testdata/v1.1/conflict-wf.cwl"),
         tmp_path / "conflict-wf.cwl",
         shallow=False,
     )
+
+def test_multi_version_upgrade_external_steps(tmp_path: Path) -> None:
+    """Test 1.0 to 1.2 upgrade of Workflow with external steps."""
+    main(
+        [f"--dir={tmp_path}", get_data("testdata/v1.0/1st-workflow.cwl")]
+    )
+    assert filecmp.cmp(
+        get_data("testdata/v1.2/arguments.cwl"),
+        tmp_path / "arguments.cwl",
+        shallow=False,
+    )
+    assert filecmp.cmp(
+        get_data("testdata/v1.2/tar-param.cwl"),
+        tmp_path / "tar-param.cwl",
+        shallow=False,
+    )
```

### Comparing `cwl-upgrader-1.2.4/tests/test_output_dir.py` & `cwl-upgrader-1.2.5/tests/test_output_dir.py`

 * *Files identical despite different names*

### Comparing `cwl-upgrader-1.2.4/tests/util.py` & `cwl-upgrader-1.2.5/tests/util.py`

 * *Files identical despite different names*

