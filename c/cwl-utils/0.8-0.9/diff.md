# Comparing `tmp/cwl-utils-0.8.tar.gz` & `tmp/cwl-utils-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cwl-utils-0.8.tar", last modified: Fri Dec 11 10:15:35 2020, max compression
+gzip compressed data, was "dist/cwl-utils-0.9.tar", last modified: Fri Dec 11 10:15:08 2020, max compression
```

## Comparing `cwl-utils-0.8.tar` & `cwl-utils-0.9.tar`

### file list

```diff
@@ -1,48 +1,57 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2020-12-11 10:15:35.030481 cwl-utils-0.8/
--rw-r--r--   0 michael   (1000) michael   (1000)       32 2019-05-22 09:05:15.000000 cwl-utils-0.8/.dockerignore
--rw-r--r--   0 michael   (1000) michael   (1000)     1212 2020-11-09 14:29:16.000000 cwl-utils-0.8/.gitignore
--rw-r--r--   0 michael   (1000) michael   (1000)     1661 2020-10-27 14:02:13.000000 cwl-utils-0.8/.travis.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    35147 2019-05-22 09:05:15.000000 cwl-utils-0.8/LICENSE
--rw-r--r--   0 michael   (1000) michael   (1000)      213 2020-11-09 14:29:16.000000 cwl-utils-0.8/MANIFEST.in
--rw-r--r--   0 michael   (1000) michael   (1000)     5867 2020-12-11 10:15:28.000000 cwl-utils-0.8/Makefile
--rw-r--r--   0 michael   (1000) michael   (1000)     2025 2020-12-11 10:15:35.030481 cwl-utils-0.8/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)     1298 2020-12-11 10:15:28.000000 cwl-utils-0.8/README.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2020-12-11 10:15:35.030481 cwl-utils-0.8/cwl_utils/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2019-05-22 09:05:15.000000 cwl-utils-0.8/cwl_utils/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)       20 2020-12-11 10:15:28.000000 cwl-utils-0.8/cwl_utils/__meta__.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2399 2020-12-02 09:17:38.000000 cwl-utils-0.8/cwl_utils/cite_extract.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    87408 2020-12-11 10:15:28.000000 cwl-utils-0.8/cwl_utils/cwl_expression_refactor.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3255 2020-12-02 09:17:38.000000 cwl-utils-0.8/cwl_utils/docker_extract.py
--rw-r--r--   0 michael   (1000) michael   (1000)    46565 2020-10-23 11:39:32.000000 cwl-utils-0.8/cwl_utils/first_tool.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     9112 2020-12-11 10:15:28.000000 cwl-utils-0.8/cwl_utils/graph_split.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4087 2020-12-11 10:15:28.000000 cwl-utils-0.8/cwl_utils/image_puller.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2020-12-11 10:15:35.030481 cwl-utils-0.8/cwl_utils/parser/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2019-05-22 09:05:15.000000 cwl-utils-0.8/cwl_utils/parser/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)   421527 2020-12-11 10:15:28.000000 cwl-utils-0.8/cwl_utils/parser_v1_0.py
--rw-r--r--   0 michael   (1000) michael   (1000)   485250 2020-12-11 10:15:28.000000 cwl-utils-0.8/cwl_utils/parser_v1_1.py
--rw-r--r--   0 michael   (1000) michael   (1000)   531754 2020-12-11 10:15:28.000000 cwl-utils-0.8/cwl_utils/parser_v1_2.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2020-12-11 10:15:35.030481 cwl-utils-0.8/cwl_utils.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)     2025 2020-12-11 10:15:35.000000 cwl-utils-0.8/cwl_utils.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      977 2020-12-11 10:15:35.000000 cwl-utils-0.8/cwl_utils.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2020-12-11 10:15:35.000000 cwl-utils-0.8/cwl_utils.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       93 2020-12-11 10:15:35.000000 cwl-utils-0.8/cwl_utils.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       10 2020-12-11 10:15:35.000000 cwl-utils-0.8/cwl_utils.egg-info/top_level.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       12 2020-10-27 14:02:13.000000 cwl-utils-0.8/mypy_requirements.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       87 2020-12-02 09:17:38.000000 cwl-utils-0.8/requirements.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      389 2020-12-11 10:15:35.030481 cwl-utils-0.8/setup.cfg
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1296 2020-12-11 10:15:28.000000 cwl-utils-0.8/setup.py
--rw-r--r--   0 michael   (1000) michael   (1000)       22 2020-10-27 14:02:13.000000 cwl-utils-0.8/test-requirements.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2020-12-11 10:15:35.030481 cwl-utils-0.8/testdata/
--rw-r--r--   0 michael   (1000) michael   (1000)     1506 2019-05-22 09:05:15.000000 cwl-utils-0.8/testdata/dockstore-tool-md5sum.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      252 2019-05-22 09:05:15.000000 cwl-utils-0.8/testdata/md5sum.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)        6 2019-05-22 09:05:15.000000 cwl-utils-0.8/testdata/md5sum.input
--rw-r--r--   0 michael   (1000) michael   (1000)      120 2019-05-22 09:05:15.000000 cwl-utils-0.8/testdata/md5sum.json
--rw-r--r--   0 michael   (1000) michael   (1000)      677 2020-10-27 14:02:13.000000 cwl-utils-0.8/testdata/workflow_input_format_expr.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      729 2020-10-27 14:02:13.000000 cwl-utils-0.8/testdata/workflow_input_sf_expr.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      729 2020-10-27 14:02:13.000000 cwl-utils-0.8/testdata/workflow_input_sf_expr_array.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2020-12-11 10:15:35.030481 cwl-utils-0.8/tests/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2019-05-22 09:05:15.000000 cwl-utils-0.8/tests/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      378 2020-12-02 09:17:38.000000 cwl-utils-0.8/tests/test_cite_extract.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1366 2020-12-11 10:15:28.000000 cwl-utils-0.8/tests/test_docker_extract.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1481 2020-12-11 10:15:28.000000 cwl-utils-0.8/tests/test_etools_to_clt.py
--rw-r--r--   0 michael   (1000) michael   (1000)      617 2020-12-11 10:15:28.000000 cwl-utils-0.8/tests/test_graph_split.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2020-12-11 10:15:08.734009 cwl-utils-0.9/
+-rw-r--r--   0 michael   (1000) michael   (1000)       32 2019-05-22 09:05:15.000000 cwl-utils-0.9/.dockerignore
+-rw-r--r--   0 michael   (1000) michael   (1000)     1212 2020-11-09 14:29:16.000000 cwl-utils-0.9/.gitignore
+-rw-r--r--   0 michael   (1000) michael   (1000)     1661 2020-10-27 14:02:13.000000 cwl-utils-0.9/.travis.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    35147 2019-05-22 09:05:15.000000 cwl-utils-0.9/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)      213 2020-11-09 14:29:16.000000 cwl-utils-0.9/MANIFEST.in
+-rw-r--r--   0 michael   (1000) michael   (1000)     5967 2020-12-02 09:17:38.000000 cwl-utils-0.9/Makefile
+-rw-r--r--   0 michael   (1000) michael   (1000)     3292 2020-12-11 10:15:08.734009 cwl-utils-0.9/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)     2381 2020-12-02 09:17:41.000000 cwl-utils-0.9/README.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2020-12-11 10:15:08.734009 cwl-utils-0.9/cwl_utils/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2019-05-22 09:05:15.000000 cwl-utils-0.9/cwl_utils/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)       20 2020-12-11 10:06:02.000000 cwl-utils-0.9/cwl_utils/__meta__.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2399 2020-12-02 09:17:38.000000 cwl-utils-0.9/cwl_utils/cite_extract.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     5259 2020-12-02 09:17:38.000000 cwl-utils-0.9/cwl_utils/cwl_expression_refactor.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    89100 2020-12-02 09:17:38.000000 cwl-utils-0.9/cwl_utils/cwl_v1_0_expression_refactor.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    89607 2020-12-02 09:17:38.000000 cwl-utils-0.9/cwl_utils/cwl_v1_1_expression_refactor.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    95543 2020-12-02 09:17:38.000000 cwl-utils-0.9/cwl_utils/cwl_v1_2_expression_refactor.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3255 2020-12-02 09:17:38.000000 cwl-utils-0.9/cwl_utils/docker_extract.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    46565 2020-10-23 11:39:32.000000 cwl-utils-0.9/cwl_utils/first_tool.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     9064 2020-12-02 09:17:38.000000 cwl-utils-0.9/cwl_utils/graph_split.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4061 2020-11-19 18:49:38.000000 cwl-utils-0.9/cwl_utils/image_puller.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2020-12-11 10:15:08.734009 cwl-utils-0.9/cwl_utils/parser/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2019-05-22 09:05:15.000000 cwl-utils-0.9/cwl_utils/parser/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)   424780 2020-12-11 10:05:44.000000 cwl-utils-0.9/cwl_utils/parser_v1_0.py
+-rw-r--r--   0 michael   (1000) michael   (1000)   488814 2020-12-11 10:05:44.000000 cwl-utils-0.9/cwl_utils/parser_v1_1.py
+-rw-r--r--   0 michael   (1000) michael   (1000)   535366 2020-12-11 10:05:44.000000 cwl-utils-0.9/cwl_utils/parser_v1_2.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2020-12-11 10:15:08.734009 cwl-utils-0.9/cwl_utils.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3292 2020-12-11 10:15:08.000000 cwl-utils-0.9/cwl_utils.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)     1369 2020-12-11 10:15:08.000000 cwl-utils-0.9/cwl_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2020-12-11 10:15:08.000000 cwl-utils-0.9/cwl_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      113 2020-12-11 10:15:08.000000 cwl-utils-0.9/cwl_utils.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       10 2020-12-11 10:15:08.000000 cwl-utils-0.9/cwl_utils.egg-info/top_level.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       12 2020-10-27 14:02:13.000000 cwl-utils-0.9/mypy_requirements.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       87 2020-12-02 09:17:38.000000 cwl-utils-0.9/requirements.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      389 2020-12-11 10:15:08.734009 cwl-utils-0.9/setup.cfg
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1318 2020-12-02 09:17:38.000000 cwl-utils-0.9/setup.py
+-rw-r--r--   0 michael   (1000) michael   (1000)       22 2020-10-27 14:02:13.000000 cwl-utils-0.9/test-requirements.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2020-12-11 10:15:08.734009 cwl-utils-0.9/testdata/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1506 2019-05-22 09:05:15.000000 cwl-utils-0.9/testdata/dockstore-tool-md5sum.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      252 2019-05-22 09:05:15.000000 cwl-utils-0.9/testdata/md5sum.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)        6 2019-05-22 09:05:15.000000 cwl-utils-0.9/testdata/md5sum.input
+-rw-r--r--   0 michael   (1000) michael   (1000)      120 2019-05-22 09:05:15.000000 cwl-utils-0.9/testdata/md5sum.json
+-rw-r--r--   0 michael   (1000) michael   (1000)      677 2020-10-27 14:02:13.000000 cwl-utils-0.9/testdata/workflow_input_format_expr.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      677 2020-11-13 10:18:13.000000 cwl-utils-0.9/testdata/workflow_input_format_expr_v1_1.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      677 2020-11-13 10:18:13.000000 cwl-utils-0.9/testdata/workflow_input_format_expr_v1_2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      729 2020-10-27 14:02:13.000000 cwl-utils-0.9/testdata/workflow_input_sf_expr.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      729 2020-10-27 14:02:13.000000 cwl-utils-0.9/testdata/workflow_input_sf_expr_array.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      729 2020-11-13 10:18:13.000000 cwl-utils-0.9/testdata/workflow_input_sf_expr_array_v1_1.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      739 2020-11-13 10:18:13.000000 cwl-utils-0.9/testdata/workflow_input_sf_expr_array_v1_2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      729 2020-11-13 10:18:13.000000 cwl-utils-0.9/testdata/workflow_input_sf_expr_v1_1.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      729 2020-11-13 10:18:13.000000 cwl-utils-0.9/testdata/workflow_input_sf_expr_v1_2.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2020-12-11 10:15:08.734009 cwl-utils-0.9/tests/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2019-05-22 09:05:15.000000 cwl-utils-0.9/tests/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      378 2020-12-02 09:17:38.000000 cwl-utils-0.9/tests/test_cite_extract.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1340 2020-12-02 09:17:38.000000 cwl-utils-0.9/tests/test_docker_extract.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5633 2020-12-02 09:17:38.000000 cwl-utils-0.9/tests/test_etools_to_clt.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      587 2020-11-19 18:49:38.000000 cwl-utils-0.9/tests/test_graph_split.py
```

### Comparing `cwl-utils-0.8/.gitignore` & `cwl-utils-0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `cwl-utils-0.8/.travis.yml` & `cwl-utils-0.9/.travis.yml`

 * *Files identical despite different names*

### Comparing `cwl-utils-0.8/LICENSE` & `cwl-utils-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cwl-utils-0.8/Makefile` & `cwl-utils-0.9/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 MODULE=cwl_utils
 
 # `SHELL=bash` doesn't work for some, so don't use BASH-isms like
 # `[[` conditional expressions.
 PYSOURCES=$(filter-out cwl_utils/parser_v%,$(wildcard ${MODULE}/**.py tests/*.py)) setup.py
 DEVPKGS=diff_cover black pylint coverage pep257 pydocstyle flake8 mypy\
-	isort wheel
+	isort wheel autoflake
 DEBDEVPKGS=pep8 python-autopep8 pylint python-coverage pydocstyle sloccount \
 	   python-flake8 python-mock shellcheck
 VERSION=$(shell awk '{print $3}' < cwl_utils/__meta__.py )
 # VERSION=3.0.$(shell TZ=UTC git log --first-parent --max-count=1 \
 # 	--format=format:%cd --date=format-local:%Y%m%d%H%M%S)
 mkfile_dir := $(dir $(abspath $(lastword $(MAKEFILE_LIST))))
 UNAME_S=$(shell uname -s)
@@ -77,14 +77,17 @@
 	rm -f diff-cover.html
 
 # Linting and code style related targets
 ## sorting imports using isort: https://github.com/timothycrosley/isort
 sort_imports: $(PYSOURCES)
 	isort $^
 
+remove_unused_imports: $(PYSOURCES)
+	autoflake --in-place --remove-all-unused-imports $^
+
 pep257: pydocstyle
 ## pydocstyle      : check Python code style
 pydocstyle: $(PYSOURCES)
 	pydocstyle --add-ignore=D100,D101,D102,D103 $^ || true
 
 pydocstyle_report.txt: $(PYSOURCES)
 	pydocstyle setup.py $^ > $@ 2>&1 || true
```

### Comparing `cwl-utils-0.8/README.md` & `cwl-utils-0.9/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,70 @@
 # cwl-utils
 
-A collection of scripts to demonstrate the use of the [new Python classes for loading and parsing CWL v1.0 documents](https://github.com/common-workflow-language/cwl-utils/blob/master/cwl_utils/parser_v1_0.py).
-
-
-`cwl_utils/parser_v1_0.py` was created via
-`schema-salad-tool --codegen python https://github.com/common-workflow-language/common-workflow-language/raw/master/v1.0/CommonWorkflowLanguage.yml`
+A collection of scripts to demonstrate the use of the new Python classes for
+loading and parsing [CWL v1.0 ](https://github.com/common-workflow-language/cwl-utils/blob/main/cwl_utils/parser/v1_0.py),
+ [CWL v1.1](https://github.com/common-workflow-language/cwl-utils/blob/main/cwl_utils/parser/v1_1.py),
+and [CWL v1.2](https://github.com/common-workflow-language/cwl-utils/blob/main/cwl_utils/parser/v1_2.py)
+documents.
 
 ## Install
 
-Requires Python 3.6.x or Python 3.7
+Requires Python 3.6+
 
 ``` bash
-git clone https://github.com/common-workflow-language/cwl-utils.git
-virtualenv -p python3.6 venv3.6
+virtualenv -p python3.6 venv3.6  # Python 3.7, 3.8, or 3.9 would also work
 source venv3.6/bin/activate
 pip install cwl-utils
 ```
+or install the latest development version of `cwl-utils`
+
+``` bash
+git clone https://github.com/common-workflow-language/cwl-utils.git
+cd cwl-utils
+virtualenv -p python3.6 venv3.6  # Python 3.7, 3.8, or 3.9 would also work
+source venv3.6/bin/activate
+pip install .
+```
 
 ## Usage
 
-### Pull the image with Docker
+### Pull the all referenced software container images
 
-This is the default behaviour:
+`docker_extract.py` is useful to cache or pre-pull all software container images
+referenced in a CWL CommandLineTool or CWL Workflow (including all referenced
+CommandLineTools and sub-Workflows and so on).
+
+The default behaviour is to use the Docker engine to download and save the software
+container images in Docker format.
 
 ```bash
 python docker_extract.py DIRECTORY path_to_my_workflow.cwl
 ```
 
-### Pull the image with Singularity
+Or you can use the Singularity software container engine to download and save the
+software container images and convert them to the Singularity format at the same
+time.
 
 ```bash
 python docker_extract.py --singularity DIRECTORY path_to_my_workflow.cwl
 ```
 
-## Regenerate
+## Development
 
-To regenerate install `schema_salad` package and run:
+### Regenerate parsers
+
+To regenerate install the `schema_salad` package and run:
+
+`cwl_utils/parser_v1_0.py` was created via
+`schema-salad-tool --codegen python https://github.com/common-workflow-language/common-workflow-language/raw/main/v1.0/CommonWorkflowLanguage.yml`
+
+`cwl_utils/parser_v1_1.py` was created via
+`schema-salad-tool --codegen python https://github.com/common-workflow-language/cwl-v1.1/raw/main/CommonWorkflowLanguage.yml`
+
+`cwl_utils/parser_v1_2.py` was created via
+`schema-salad-tool --codegen python https://github.com/common-workflow-language/cwl-v1.2/raw/main/CommonWorkflowLanguage.yml`
 
-```
-schema-salad-tool --codegen python \
-    https://raw.githubusercontent.com/common-workflow-language/common-workflow-language/master/v1.0/CommonWorkflowLanguage.yml
-```
 
-## Release
+### Release
 
-To release CWLUtils, bump the version in `cwl_utils/__meta__.py`, and tag that commit with the new version. TravisCI should release that tag.
+To release CWLUtils, bump the version in `cwl_utils/__meta__.py`, and tag that
+commit with the new version. TravisCI should release that tag.
```

### Comparing `cwl-utils-0.8/cwl_utils/cite_extract.py` & `cwl-utils-0.9/cwl_utils/cite_extract.py`

 * *Files identical despite different names*

### Comparing `cwl-utils-0.8/cwl_utils/cwl_expression_refactor.py` & `cwl-utils-0.9/cwl_utils/cwl_v1_0_expression_refactor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 #!/usr/bin/env python3
-import argparse
+"""CWL Expression refactoring tool for CWL v1.0 ."""
 import copy
 import hashlib
-import shutil
-import sys
 from collections.abc import Mapping
 from typing import (
     Any,
     Dict,
     List,
     MutableSequence,
     Optional,
@@ -16,105 +14,22 @@
     Tuple,
     Type,
     Union,
     cast,
 )
 
 from cwltool.errors import WorkflowException
-from cwltool.expression import do_eval
+from cwltool.expression import do_eval, interpolate
 from cwltool.sandboxjs import JavascriptException
 from cwltool.utils import CWLObjectType, CWLOutputType
-from cwltool.loghandler import _logger as _cwltoollogger
 from ruamel import yaml
 from schema_salad.sourceline import SourceLine
 from schema_salad.utils import json_dumps
-from pathlib import Path
-import cwl_utils.parser_v1_0 as cwl
-
-import logging
 
-_logger = logging.getLogger("cwl-expression-refactor")  # pylint: disable=invalid-name
-defaultStreamHandler = logging.StreamHandler()  # pylint: disable=invalid-name
-_logger.addHandler(defaultStreamHandler)
-_logger.setLevel(logging.INFO)
-_cwltoollogger.setLevel(100)
-
-
-def parse_args(args: List[str]) -> argparse.Namespace:
-    """Argument parser."""
-    parser = argparse.ArgumentParser(
-        description="Tool to upgrade refactor CWL documents so that any CWL expression "
-        "are separate steps as either ExpressionTools or CommandLineTools."
-    )
-    parser.add_argument(
-        "--etools",
-        help="Output ExpressionTools, don't go all the way to CommandLineTools.",
-        action="store_true",
-    )
-    parser.add_argument(
-        "--skip-some1",
-        help="Don't process CommandLineTool.inputs.inputBinding and CommandLineTool.arguments sections.",
-        action="store_true",
-    )
-    parser.add_argument(
-        "--skip-some2",
-        help="Don't process CommandLineTool.outputEval or CommandLineTool.requirements.InitialWorkDirRequirement.",
-        action="store_true",
-    )
-    parser.add_argument("dir", help="Directory in which to save converted files")
-    parser.add_argument(
-        "inputs",
-        nargs="+",
-        help="One or more CWL documents.",
-    )
-    return parser.parse_args(args)
-
-
-def main(args: Optional[List[str]] = None) -> int:
-    """Collect the arguments and run."""
-    if not args:
-        args = sys.argv[1:]
-    return run(parse_args(args))
-
-
-def run(args: argparse.Namespace) -> int:
-    """Load the first command line argument, print the results to stdout."""
-    for document in args.inputs:
-        _logger.info("Processing %s.", document)
-        top = cwl.load_document(document)
-        output = Path(args.dir) / Path(document).name
-        result, modified = traverse(
-            top, not args.etools, args.skip_some1, args.skip_some2
-        )
-        if not modified:
-            shutil.copyfile(document, output)
-            continue
-        if not isinstance(result, MutableSequence):
-            result_json = cwl.save(
-                result,
-                base_url=result.loadingOptions.fileuri
-                if result.loadingOptions.fileuri
-                else "",
-            )
-        #   ^^ Setting the base_url and keeping the default value
-        #      for relative_uris=True means that the IDs in the generated
-        #      JSON/YAML are kept clean of the path to the input document
-        else:
-            result_json = [
-                cwl.save(result_item, base_url=result_item.loadingOptions.fileuri)
-                for result_item in result
-            ]
-        yaml.scalarstring.walk_tree(result_json)
-        # ^ converts multine line strings to nice multiline YAML
-        with open(output, "w", encoding="utf-8") as output_filehandle:
-            output_filehandle.write(
-                "#!/usr/bin/env cwl-runner\n"
-            )  # TODO: teach the codegen to do this?
-            yaml.round_trip_dump(result_json, output_filehandle)
-    return 0
+import cwl_utils.parser_v1_0 as cwl
 
 
 def expand_stream_shortcuts(process: cwl.CommandLineTool) -> cwl.CommandLineTool:
     """Rewrite the "type: stdout" shortcut to use an explicit random filename."""
     if not process.outputs:
         return process
     result = None
@@ -138,29 +53,31 @@
 
 
 def escape_expression_field(contents: str) -> str:
     """Escape sequences similar to CWL expressions or param references."""
     return contents.replace("${", "$/{").replace("$(", "$/(")
 
 
-def clean_type_ids(cwltype: Any) -> Any:
+def clean_type_ids(
+    cwltype: Union[cwl.ArraySchema, cwl.InputRecordSchema]
+) -> Union[cwl.ArraySchema, cwl.InputRecordSchema]:
     """Simplify type identifiers."""
     result = copy.deepcopy(cwltype)
-    if isinstance(cwltype, cwl.ArraySchema):
+    if isinstance(result, cwl.ArraySchema):
         if isinstance(result.items, MutableSequence):
             for item in result.items:
                 if hasattr(item, "id"):
                     item.id = item.id.split("#")[-1]
         elif isinstance(result.items, cwl.InputRecordSchema):
             if result.items.name:
                 result.items.name = result.items.name.split("/")[-1]
             if result.items.fields:
                 for field in result.items.fields:
                     field.name = field.name.split("/")[-1]
-    elif isinstance(cwltype, cwl.InputRecordSchema):
+    elif isinstance(result, cwl.InputRecordSchema):
         result.name = result.name.split("/")[-1]
         if result.fields:
             for field in result.fields:
                 field.name = field.name.split("/")[-1]
     return result
 
 
@@ -173,28 +90,56 @@
     CWL expressions in the $() form are converted to the ${} form.
     """
     if not isinstance(string, Text):
         return None
     if string.strip().startswith("${"):
         return string
     if "$(" in string:
+        runtime: CWLObjectType = {
+            "cores": 0,
+            "ram": 0,
+            "outdir": "/root",
+            "tmpdir": "/tmp",
+            "outdirSize": 0,
+            "tmpdirSize": 0,
+        }
         try:
             do_eval(
                 string,
                 inputs,
                 context=self,
                 requirements=[],
                 outdir="",
                 tmpdir="",
                 resources={},
             )
         except (WorkflowException, JavascriptException):
-            # TODO: what if the $() expr is in the middle of the string?
-            # TODO: what if there are multple $() expressions?
-            return "${return " + string.strip()[2:-1] + ";}"
+            if (
+                string[0:2] != "$("
+                or not string.endswith(")")
+                or len(string.split("$(")) > 2
+            ):
+                # then it is a string interpolation
+                return cast(
+                    str,
+                    interpolate(
+                        scan=string,
+                        rootvars={
+                            "inputs": inputs,
+                            "context": self,
+                            "runtime": runtime,
+                        },
+                        fullJS=True,
+                        escaping_behavior=2,
+                        convert_to_expression=True,
+                    ),
+                )
+            else:
+                # it is a CWL Expression in $() with no string interpolation
+                return "${return " + string.strip()[2:-1] + ";}"
     return None
 
 
 def etool_to_cltool(
     etool: cwl.ExpressionTool, expressionLib: Optional[List[str]] = None
 ) -> cwl.CommandLineTool:
     """Convert a ExpressionTool to a CommandLineTool."""
@@ -233,44 +178,46 @@
 var inputs=$(inputs);
 var runtime=$(runtime);"""
     if expressionLib:
         contents += "\n" + "\n".join(expressionLib)
     contents += (
         """
 var ret = function(){"""
-        + etool.expression.strip()[2:-1]
+        + escape_expression_field(etool.expression.strip()[2:-1])
         + """}();
 process.stdout.write(JSON.stringify(ret));"""
     )
-    contents = escape_expression_field(contents)
-    listing = [cwl.Dirent("expression.js", contents, writable=None)]
+    listing = [cwl.Dirent(entryname="expression.js", entry=contents, writable=None)]
     iwdr = cwl.InitialWorkDirRequirement(listing)
     containerReq = cwl.DockerRequirement(dockerPull="node:slim")
+    softwareHint = cwl.SoftwareRequirement(
+        packages=[cwl.SoftwarePackage(package="nodejs")]
+    )
     return cwl.CommandLineTool(
         inputs=inputs,
         outputs=outputs,
         id=etool.id,
         requirements=[iwdr],
-        hints=[containerReq],
+        hints=[containerReq, softwareHint],
         label=etool.label,
         doc=etool.doc,
         cwlVersion=etool.cwlVersion,
         baseCommand=["nodejs", "expression.js"],
         stdout="cwl.output.json",
         extension_fields=etool.extension_fields,
         loadingOptions=etool.loadingOptions,
     )
 
 
 def traverse(
     process: Union[cwl.CommandLineTool, cwl.ExpressionTool, cwl.Workflow],
-    replace_etool: bool = False,
-    inside: bool = False,
-    skip_command_line1: bool = False,
-    skip_command_line2: bool = False,
+    replace_etool: bool,
+    inside: bool,
+    skip_command_line1: bool,
+    skip_command_line2: bool,
 ) -> Tuple[Union[cwl.CommandLineTool, cwl.ExpressionTool, cwl.Workflow], bool]:
     """Convert the given process and any subprocesess."""
     if not inside and isinstance(process, cwl.CommandLineTool):
         process = expand_stream_shortcuts(process)
         wf_inputs = []
         wf_outputs = []
         step_inputs = []
@@ -334,69 +281,95 @@
             workflow, replace_etool, skip_command_line1, skip_command_line2
         )
         if modified:
             return result, True
         else:
             return process, False
     if isinstance(process, cwl.ExpressionTool) and replace_etool:
-        return etool_to_cltool(process), True
+        expression = get_expression(process.expression, empty_inputs(process), None)
+        # Why call get_expression on an ExpressionTool?
+        # It normalizes the form of $() CWL expressions into the ${} style
+        if expression:
+            process2 = copy.deepcopy(process)
+            process2.expression = expression
+        else:
+            process2 = process
+        return etool_to_cltool(process2), True
     if isinstance(process, cwl.Workflow):
         return traverse_workflow(
             process, replace_etool, skip_command_line1, skip_command_line2
         )
     return process, False
 
 
 def load_step(
     step: cwl.WorkflowStep,
-    replace_etool: bool = False,
-    skip_command_line1: bool = False,
-    skip_command_line2: bool = False,
+    replace_etool: bool,
+    skip_command_line1: bool,
+    skip_command_line2: bool,
 ) -> bool:
     """If the step's Process is not inline, load and process it."""
     modified = False
     if isinstance(step.run, str):
         step.run, modified = traverse(
-            cwl.load_document(step.run),
+            cwl.load_document(step.run, baseuri=step.loadingOptions.fileuri),
             replace_etool,
             True,
             skip_command_line1,
             skip_command_line2,
         )
     return modified
 
 
 def generate_etool_from_expr(
     expr: str,
     target: Union[cwl.CommandInputParameter, cwl.InputParameter],
     no_inputs: bool = False,
     self_type: Optional[
-        Union[cwl.InputParameter, cwl.CommandInputParameter]
+        Union[
+            cwl.InputParameter,
+            cwl.CommandInputParameter,
+            List[Union[cwl.InputParameter, cwl.CommandInputParameter]],
+        ]
     ] = None,  # if the "self" input should be a different type than the "result" output
     extra_processes: Optional[
         Sequence[Union[cwl.Workflow, cwl.WorkflowStep, cwl.CommandLineTool]]
     ] = None,
 ) -> cwl.ExpressionTool:
     """Convert a CWL Expression into an ExpressionTool."""
     inputs = yaml.comments.CommentedSeq()
     if not no_inputs:
         if not self_type:
             self_type = target
-        new_type = clean_type_ids(self_type.type)
+        if isinstance(self_type, list):
+            new_type: Union[
+                List[Union[cwl.ArraySchema, cwl.InputRecordSchema]],
+                Union[cwl.ArraySchema, cwl.InputRecordSchema],
+            ] = [clean_type_ids(t.type) for t in self_type]
+        else:
+            new_type = clean_type_ids(self_type.type)
         inputs.append(
             cwl.InputParameter(
                 id="self",
-                label=self_type.label,
-                secondaryFiles=self_type.secondaryFiles,
-                streamable=self_type.streamable,
-                doc=self_type.doc,
-                format=self_type.format,
+                label=self_type.label if not isinstance(self_type, list) else None,
+                secondaryFiles=self_type.secondaryFiles
+                if not isinstance(self_type, list)
+                else None,
+                streamable=self_type.streamable
+                if not isinstance(self_type, list)
+                else None,
+                doc=self_type.doc if not isinstance(self_type, list) else None,
+                format=self_type.format if not isinstance(self_type, list) else None,
                 type=new_type,
-                extension_fields=self_type.extension_fields,
-                loadingOptions=self_type.loadingOptions,
+                extension_fields=self_type.extension_fields
+                if not isinstance(self_type, list)
+                else None,
+                loadingOptions=self_type.loadingOptions
+                if not isinstance(self_type, list)
+                else None,
             )
         )
     outputs = yaml.comments.CommentedSeq()
     outputs.append(
         cwl.ExpressionToolOutputParameter(
             id="result",
             label=target.label,
@@ -537,32 +510,38 @@
                 if isinstance(outp.outputSource, MutableSequence):
                     for index, outputSource in enumerate(outp.outputSource):
                         if outputSource == name:
                             outp.outputSource[index] = target
 
 
 def empty_inputs(
-    process_or_step: Union[cwl.CommandLineTool, cwl.WorkflowStep, cwl.Workflow],
+    process_or_step: Union[
+        cwl.CommandLineTool, cwl.WorkflowStep, cwl.ExpressionTool, cwl.Workflow
+    ],
     parent: Optional[cwl.Workflow] = None,
 ) -> Dict[str, Any]:
     """Produce a mock input object for the given inputs."""
     result = {}
     if isinstance(process_or_step, cwl.Process):
         for param in process_or_step.inputs:
             result[param.id.split("#")[-1]] = example_input(param.type)
     else:
         for param in process_or_step.in_:
-            try:
-                result[param.id.split("#")[-1]] = example_input(
-                    type_for_source(
-                        process_or_step.run, param.id.split("/")[-1], parent
+            param_id = param.id.split("/")[-1]
+            if param.source is None and param.valueFrom:
+                result[param_id] = example_input("string")
+            elif param.source is None and param.default:
+                result[param_id] = param.default
+            else:
+                try:
+                    result[param_id] = example_input(
+                        type_for_source(process_or_step.run, param.source, parent)
                     )
-                )
-            except WorkflowException:
-                pass
+                except WorkflowException:
+                    pass
     return result
 
 
 def example_input(some_type: Any) -> Any:
     """Produce a fake input for the given type."""
     # TODO: accept some sort of context object with local custom type definitions
     if some_type == "Directory":
@@ -587,60 +566,79 @@
             "location": "https://www.example.com/example.txt",
             "basename": "example.txt",
             "size": 23,
             "contents": "hoopla",
             "nameroot": "example",
             "nameext": "txt",
         }
+    if some_type == "int":
+        return 23
+    if some_type == "string":
+        return "hoopla!"
+    if some_type == "boolean":
+        return True
     return None
 
 
 def type_for_source(
     process: Union[cwl.CommandLineTool, cwl.Workflow, cwl.ExpressionTool],
     sourcenames: Union[str, List[str]],
     parent: Optional[cwl.Workflow] = None,
-) -> Any:
-    # TODO: if there are multiple source names, why don't we return a mixed type?
+) -> Union[List[Any], Any]:
     """Determine the type for the given sourcenames."""
-    return param_for_source_id(process, sourcenames, parent).type
+    params = param_for_source_id(process, sourcenames, parent)
+    if not isinstance(params, list):
+        return params.type
+    new_type: List[Any] = []
+    for p in params:
+        if isinstance(p, str) and p not in new_type:
+            new_type.append(p)
+        elif hasattr(p, "type") and p.type not in new_type:
+            new_type.append(p.type)
+    return new_type
 
 
 def param_for_source_id(
     process: Union[cwl.CommandLineTool, cwl.Workflow, cwl.ExpressionTool],
     sourcenames: Union[str, List[str]],
     parent: Optional[cwl.Workflow] = None,
-) -> Any:
+) -> Union[List[cwl.InputParameter], cwl.InputParameter]:
     """Find the process input parameter that matches one of the given sourcenames."""
-    # TODO: if there are multiple source names, why don't we return multipe parameters?
     if isinstance(sourcenames, str):
         sourcenames = [sourcenames]
+    params: List[cwl.InputParameter] = []
     for sourcename in sourcenames:
-        for param in process.inputs:
-            if param.id.split("#")[-1] == sourcename.split("#")[-1]:
-                return param
+        if not isinstance(process, cwl.Workflow):
+            for param in process.inputs:
+                if param.id.split("#")[-1] == sourcename.split("#")[-1]:
+                    params.append(param)
         targets = [process]
         if parent:
             targets.append(parent)
         for target in targets:
             if isinstance(target, cwl.Workflow):
                 for inp in target.inputs:
                     if inp.id.split("#")[-1] == sourcename.split("#")[-1]:
-                        return inp
+                        params.append(inp)
                 for step in target.steps:
                     if sourcename.split("/")[0] == step.id.split("#")[-1] and step.out:
                         for outp in step.out:
                             outp_id = outp if isinstance(outp, str) else outp.id
                             if outp_id.split("/")[-1] == sourcename.split("/", 1)[1]:
                                 if step.run and step.run.outputs:
                                     for output in step.run.outputs:
                                         if (
                                             output.id.split("#")[-1]
                                             == sourcename.split("/", 1)[1]
                                         ):
-                                            return output
+                                            params.append(output)
+    if len(params) == 1:
+        return params[0]
+    elif len(params) > 1:
+        return params
     raise WorkflowException(
         "param {} not found in {}\n or\n {}.".format(
             sourcename,
             yaml.round_trip_dump(cwl.save(process)),
             yaml.round_trip_dump(cwl.save(parent)),
         )
     )
@@ -651,29 +649,31 @@
     "basename": "em.pty",
     "nameroot": "em",
     "nameext": "pty",
 }
 
 TOPLEVEL_SF_EXPR_ERROR = (
     "Input '{}'. Sorry, CWL Expressions as part of a secondaryFiles "
-    "specification in a Workflow level input are not able to be refactored "
-    "into separate ExpressionTool/CommandLineTool steps."
+    "specification in a Workflow level input or standalone CommandLine Tool "
+    "are not able to be refactored into separate ExpressionTool or "
+    "CommandLineTool steps."
 )
 
 TOPLEVEL_FORMAT_EXPR_ERROR = (
     "Input '{}'. Sorry, CWL Expressions as part of a format "
     "specification in a Workflow level input are not able to be refactored "
     "into separate ExpressionTool/CommandLineTool steps."
 )
 
 
 def process_workflow_inputs_and_outputs(
     workflow: cwl.Workflow, replace_etool: bool
-) -> None:
+) -> bool:
     """Do any needed conversions on the given Workflow's inputs and outputs."""
+    modified = False
     inputs = empty_inputs(workflow)
     for index, param in enumerate(workflow.inputs):
         with SourceLine(workflow.inputs, index, WorkflowException):
             if param.format and get_expression(param.format, inputs, None):
                 raise SourceLine(
                     param.loadingOptions.original_doc,
                     "format",
@@ -693,18 +693,19 @@
                                 param.loadingOptions.original_doc,
                                 index2,
                                 raise_type=WorkflowException,
                             ).makeError(
                                 "Entry {},".format(index)
                                 + TOPLEVEL_SF_EXPR_ERROR.format(param.id.split("#")[-1])
                             )
+    return modified
 
 
 def process_workflow_reqs_and_hints(
-    workflow: cwl.Workflow, replace_etool: bool = False
+    workflow: cwl.Workflow, replace_etool: bool
 ) -> bool:
     """
     Convert any expressions in a workflow's reqs and hints.
 
     Each expression will be converted to an additional step.
     The converted requirement will be copied to all workflow steps that don't have that
     requirement type. Those affected steps will gain an additional input from the relevant
@@ -1025,36 +1026,36 @@
     return modified
 
 
 def process_level_reqs(
     process: cwl.CommandLineTool,
     step: cwl.WorkflowStep,
     parent: cwl.Workflow,
-    replace_etool: bool = False,
-    skip_command_line1: bool = False,
-    skip_command_line2: bool = False,
+    replace_etool: bool,
+    skip_command_line1: bool,
+    skip_command_line2: bool,
 ) -> bool:
     """Convert expressions inside a process into new adjacent steps."""
     # This is for reqs inside a Process (CommandLineTool, ExpressionTool)
     # differences from process_workflow_reqs_and_hints() are:
-    # - the name of the generated ETools/CTools contain the name of the step, not "workflow"
+    # - the name of the generated ETools/CTools contains the name of the step, not "workflow"
     # - Generated ETools/CTools are adjacent steps
     # - Replace the CWL Expression inplace with a CWL parameter reference
     # - Don't create a new Requirement, nor delete the existing Requirement
     # - the Process is passed to replace_expr_with_etool for later searching for JS expressionLibs
     # - in addition to adding the input to the step for the ETool/CTool result, add it to the Process.inputs as well
     if not process.requirements:
         return False
     modified = False
     target_process = step.run
     inputs = empty_inputs(process)
     generated_res_reqs: List[Tuple[str, str]] = []
     generated_iwdr_reqs: List[Tuple[str, Union[int, str], Any]] = []
     generated_envVar_reqs: List[Tuple[str, Union[int, str]]] = []
-    step_name = step.id.split("#", 1)[1]
+    step_name = step.id.split("#", 1)[-1]
     for req_index, req in enumerate(process.requirements):
         if req and isinstance(req, cwl.EnvVarRequirement):
             if req.envDef:
                 for env_index, envDef in enumerate(req.envDef):
                     if envDef.envValue:
                         expression = get_expression(envDef.envValue, inputs, None)
                         if expression:
@@ -1171,55 +1172,50 @@
                                 (etool_id, listing_index, target_type)
                             )
                         elif isinstance(entry, cwl.Dirent):
                             if entry.entry:
                                 expression = get_expression(entry.entry, inputs, None)
                                 if expression:
                                     modified = True
-                                    if entry.entryname is None:
-                                        raise SourceLine(
-                                            req.listing,
-                                            listing_index,
-                                            raise_type=WorkflowException,
-                                        ).makeError(
-                                            "`entryname` is required: {}".format(entry)
+                                    if entry.entryname is not None:
+                                        entryname_expr = get_expression(
+                                            entry.entryname, inputs, None
                                         )
-                                    entryname_expr = get_expression(
-                                        entry.entryname, inputs, None
-                                    )
-                                    entryname = (
-                                        entry.entryname
-                                        if entryname_expr
-                                        else '"{}"'.format(entry.entryname)
-                                    )
-                                    d_target_type = ["File", "Directory"]
-                                    target = cwl.InputParameter(
-                                        id=None,
-                                        type=d_target_type,
-                                    )
-                                    etool_id = "_expression_{}_InitialWorkDirRequirement_{}".format(
-                                        step_name, listing_index
-                                    )
-
-                                    new_expression = (
-                                        "${var result; var entryname = "
-                                        + entryname
-                                        + "; var entry = "
-                                        + entry.entry[2:-1]
-                                        + """;
+                                        entryname = (
+                                            entry.entryname
+                                            if entryname_expr
+                                            else '"{}"'.format(entry.entryname)
+                                        )
+                                        new_expression = (
+                                            "${var result; var entryname = "
+                                            + entryname
+                                            + "; var entry = "
+                                            + entry.entry[2:-1]
+                                            + """;
 if (typeof entry === 'string' || entry instanceof String) {
 result = {"class": "File", "basename": entryname, "contents": entry} ;
 if (typeof entryname === 'string' || entryname instanceof String) {
 result.basename = entryname ;
 }
 } else {
 result = entry ;
 }
 return result; }"""
+                                        )
+                                    else:
+                                        new_expression = expression
+                                    d_target_type = ["File", "Directory"]
+                                    target = cwl.InputParameter(
+                                        id=None,
+                                        type=d_target_type,
                                     )
+                                    etool_id = "_expression_{}_InitialWorkDirRequirement_{}".format(
+                                        step_name, listing_index
+                                    )
+
                                     replace_clt_hintreq_expr_with_etool(
                                         new_expression,
                                         etool_id,
                                         parent,
                                         target,
                                         step,
                                         replace_etool,
@@ -1297,17 +1293,17 @@
         )
 
 
 def traverse_CommandLineTool(
     clt: cwl.CommandLineTool,
     parent: cwl.Workflow,
     step: cwl.WorkflowStep,
-    replace_etool: bool = False,
-    skip_command_line1: bool = False,
-    skip_command_line2: bool = False,
+    replace_etool: bool,
+    skip_command_line1: bool,
+    skip_command_line2: bool,
 ) -> bool:
     """Extract any CWL Expressions within the given CommandLineTool into sibling steps."""
     modified = False
     # don't modifiy clt, modify step.run
     target_clt = step.run
     inputs = empty_inputs(clt)
     step_id = step.id.split("#")[-1]
@@ -1320,16 +1316,16 @@
                     inp_id = "_arguments_{}".format(index)
                     etool_id = "_expression_{}{}".format(step_id, inp_id)
                     target_type = "Any"
                     target = cwl.InputParameter(id=None, type=target_type)
                     replace_step_clt_expr_with_etool(
                         expression, etool_id, parent, target, step, replace_etool
                     )
-                    target_clt.arguments[index].valueFrom = "$(inputs.{})".format(
-                        inp_id
+                    target_clt.arguments[index] = cwl.CommandLineBinding(
+                        valueFrom="$(inputs.{})".format(inp_id)
                     )
                     target_clt.inputs.append(
                         cwl.CommandInputParameter(
                             id=inp_id,
                             type=target_type,
                         )
                     )
@@ -1504,21 +1500,37 @@
                     )  # a deepcopy would be convienant, but params2.cwl gives it problems
                     new_clt_step.id = new_clt_step.id.split("#")[-1]
                     new_clt_step.run = copy.copy(step.run)
                     new_clt_step.run.id = None
                     remove_JSReq(new_clt_step.run, skip_command_line1)
                     for new_outp in new_clt_step.run.outputs:
                         if new_outp.id.split("#")[-1] == outp_id:
-                            if new_outp.outputBinding:
-                                new_outp.outputBinding.outputEval = None
-                                new_outp.outputBinding.loadContents = None
-                            new_outp.type = cwl.CommandOutputArraySchema(
-                                items="File",
-                                type="array",
-                            )
+                            if isinstance(
+                                new_outp,
+                                (
+                                    cwl.WorkflowOutputParameter,
+                                    cwl.ExpressionToolOutputParameter,
+                                ),
+                            ):
+                                new_outp.type = cwl.OutputArraySchema(
+                                    items="File", type="array"
+                                )
+                            elif isinstance(new_outp, cwl.CommandOutputParameter):
+                                if new_outp.outputBinding:
+                                    new_outp.outputBinding.outputEval = None
+                                    new_outp.outputBinding.loadContents = None
+                                new_outp.type = cwl.CommandOutputArraySchema(
+                                    items="File",
+                                    type="array",
+                                )
+                            else:
+                                raise Exception(
+                                    "Unimplemented OutputParamter type: %s",
+                                    type(new_outp),
+                                )
                     new_clt_step.in_ = copy.deepcopy(step.in_)
                     for inp in new_clt_step.in_:
                         inp.id = inp.id.split("/")[-1]
                         inp.source = inp.id
                         inp.linkMerge = None
                     for index, out in enumerate(new_clt_step.out):
                         new_clt_step.out[index] = out.split("/")[-1]
@@ -1588,15 +1600,15 @@
                         for index, source in enumerate(inp.source):
                             if simplify_step_id(source) == old:
                                 inp.source[index] = new
 
 
 def remove_JSReq(
     process: Union[cwl.CommandLineTool, cwl.WorkflowStep, cwl.Workflow],
-    skip_command_line1: bool = False,
+    skip_command_line1: bool,
 ) -> None:
     """Since the InlineJavascriptRequiment is longer needed, remove it."""
     if skip_command_line1 and isinstance(process, cwl.CommandLineTool):
         return
     if process.hints:
         process.hints[:] = [
             hint
@@ -1617,15 +1629,15 @@
 
 def replace_step_clt_expr_with_etool(
     expr: str,
     name: str,
     workflow: cwl.Workflow,
     target: cwl.InputParameter,
     step: cwl.WorkflowStep,
-    replace_etool: bool = False,
+    replace_etool: bool,
     self_name: Optional[str] = None,
 ) -> None:
     """Convert a step level CWL Expression to a sibling expression step."""
     etool_inputs = cltool_inputs_to_etool_inputs(step.run)
     temp_etool = generate_etool_from_expr2(
         expr, target, etool_inputs, self_name, step.run, [workflow]
     )
@@ -1652,15 +1664,15 @@
 
 def replace_clt_hintreq_expr_with_etool(
     expr: str,
     name: str,
     workflow: cwl.Workflow,
     target: cwl.InputParameter,
     step: cwl.WorkflowStep,
-    replace_etool: bool = False,
+    replace_etool: bool,
     self_name: Optional[str] = None,
 ) -> Union[cwl.CommandLineTool, cwl.ExpressionTool]:
     """Factor out an expression inside a CommandLineTool req or hint into a sibling step."""
     # Same as replace_step_clt_expr_with_etool or different?
     etool_inputs = cltool_inputs_to_etool_inputs(step.run)
     temp_etool = generate_etool_from_expr2(
         expr, target, etool_inputs, self_name, step.run, [workflow]
@@ -1811,17 +1823,17 @@
         cwlVersion="v1.0",
     )
 
 
 def traverse_step(
     step: cwl.WorkflowStep,
     parent: cwl.Workflow,
-    replace_etool: bool = False,
-    skip_command_line1: bool = False,
-    skip_command_line2: bool = False,
+    replace_etool: bool,
+    skip_command_line1: bool,
+    skip_command_line2: bool,
 ) -> bool:
     """Process the given WorkflowStep."""
     modified = False
     inputs = empty_inputs(step, parent)
     step_id = step.id.split("#")[-1]
     original_process = copy.deepcopy(step.run)
     original_step_ins = copy.deepcopy(step.in_)
@@ -1836,45 +1848,57 @@
                         if not step.scatter:
                             self.append(
                                 example_input(
                                     type_for_source(parent, source.split("#")[-1])
                                 )
                             )
                         else:
-                            self.append(
-                                example_input(type_for_source(parent, source).type)
-                            )
+                            scattered_source_type = type_for_source(parent, source)
+                            if isinstance(scattered_source_type, list):
+                                for stype in scattered_source_type:
+                                    self.append(example_input(stype.type))
+                            else:
+                                self.append(example_input(scattered_source_type.type))
                 else:
                     if not step.scatter:
                         self = example_input(
                             type_for_source(parent, inp.source.split("#")[-1])
                         )
                     else:
-                        self = example_input(type_for_source(parent, inp.source).type)
+                        scattered_source_type2 = type_for_source(parent, inp.source)
+                        if isinstance(scattered_source_type2, list):
+                            self = example_input(scattered_source_type2[0].type)
+                        else:
+                            self = example_input(scattered_source_type2.type)
             expression = get_expression(inp.valueFrom, inputs, self)
             if expression:
                 modified = True
                 etool_id = "_expression_{}_{}".format(step_id, inp.id.split("/")[-1])
                 target = get_input_for_id(inp.id, original_process)
                 if not target:
                     raise WorkflowException("target not found")
                 input_source_id = None
-                source_type = None
+                source_type: Optional[
+                    Union[List[cwl.InputParameter], cwl.InputParameter]
+                ] = None
                 if inp.source:
                     if isinstance(inp.source, MutableSequence):
                         input_source_id = []
                         source_types: List[cwl.InputParameter] = []
                         for source in inp.source:
                             source_id = source.split("#")[-1]
                             input_source_id.append(source_id)
-                            temp_type = param_for_source_id(
-                                step.run, source_id, parent
-                            ).type
-                            if temp_type not in source_types:
-                                source_types.append(temp_type)
+                            temp_type = type_for_source(step.run, source_id, parent)
+                            if isinstance(temp_type, list):
+                                for ttype in temp_type:
+                                    if ttype not in source_types:
+                                        source_types.append(ttype)
+                            else:
+                                if temp_type not in source_types:
+                                    source_types.append(temp_type)
                         source_type = cwl.InputParameter(
                             id=None,
                             type=cwl.ArraySchema(source_types, "array"),
                         )
                     else:
                         input_source_id = inp.source.split("#")[-1]
                         source_type = param_for_source_id(
@@ -1911,15 +1935,20 @@
                     replace_etool,
                     source_type,
                 )
                 inp.valueFrom = None
                 inp.source = "{}/result".format(etool_id)
     # TODO: skip or special process for sub workflows?
     process_modified = process_level_reqs(
-        original_process, step, parent, replace_etool, skip_command_line1
+        original_process,
+        step,
+        parent,
+        replace_etool,
+        skip_command_line1,
+        skip_command_line2,
     )
     if process_modified:
         modified = True
     if isinstance(original_process, cwl.CommandLineTool):
         clt_modified = traverse_CommandLineTool(
             original_process,
             parent,
@@ -1938,32 +1967,38 @@
 ) -> List[cwl.InputParameter]:
     """Create InputParametes to match the given WorkflowStep inputs."""
     params = []
     for inp in step_ins:
         inp_id = inp.id.split("#")[-1].split("/")[-1]
         if inp.source and inp_id != except_in_id:
             param = copy.deepcopy(param_for_source_id(parent, sourcenames=inp.source))
-            param.id = inp_id
-            param.type = clean_type_ids(param.type)
-            params.append(param)
+            if isinstance(param, list):
+                for p in param:
+                    p.id = inp_id
+                    p.type = clean_type_ids(p.type)
+                    params.append(p)
+            else:
+                param.id = inp_id
+                param.type = clean_type_ids(param.type)
+                params.append(param)
     return params
 
 
 def replace_step_valueFrom_expr_with_etool(
     expr: str,
     name: str,
     workflow: cwl.Workflow,
     target: Union[cwl.CommandInputParameter, cwl.InputParameter],
     step: cwl.WorkflowStep,
     step_inp: cwl.WorkflowStepInput,
     original_process: Union[cwl.CommandLineTool, cwl.ExpressionTool],
     original_step_ins: List[cwl.WorkflowStepInput],
-    source: Union[str, List[Any]],
-    replace_etool: bool = False,
-    source_type: Optional[Union[cwl.InputParameter, cwl.CommandInputParameter]] = None,
+    source: Union[str, List[str]],
+    replace_etool: bool,
+    source_type: Optional[Union[cwl.InputParameter, List[cwl.InputParameter]]] = None,
 ) -> None:
     """Replace a WorkflowStep level 'valueFrom' expression with a sibling ExpressionTool step."""
     step_inp_id = step_inp.id.split("/")[-1]
     etool_inputs = workflow_step_to_InputParameters(
         original_step_ins, workflow, step_inp_id
     )
     if source:
@@ -2026,17 +2061,17 @@
             scatterMethod=step.scatterMethod,
         )
     )
 
 
 def traverse_workflow(
     workflow: cwl.Workflow,
-    replace_etool: bool = False,
-    skip_command_line1: bool = False,
-    skip_command_line2: bool = False,
+    replace_etool: bool,
+    skip_command_line1: bool,
+    skip_command_line2: bool,
 ) -> Tuple[cwl.Workflow, bool]:
     """Traverse a workflow, processing each step."""
     modified = False
     for index, step in enumerate(workflow.steps):
         if isinstance(step.run, cwl.ExpressionTool) and replace_etool:
             workflow.steps[index].run = etool_to_cltool(step.run)
             modified = True
@@ -2045,29 +2080,26 @@
                 step, replace_etool, skip_command_line1, skip_command_line2
             )
             if step_modified:
                 modified = True
     for step in workflow.steps:
         if not step.id.startswith("_expression"):
             step_modified = traverse_step(
-                step, workflow, skip_command_line1, skip_command_line2
+                step, workflow, replace_etool, skip_command_line1, skip_command_line2
             )
             if step_modified:
                 modified = True
-    process_workflow_inputs_and_outputs(workflow, replace_etool)
-    process_workflow_reqs_and_hints(workflow, replace_etool)
+    if process_workflow_inputs_and_outputs(workflow, replace_etool):
+        modified = True
+    if process_workflow_reqs_and_hints(workflow, replace_etool):
+        modified = True
     if workflow.requirements:
         workflow.requirements[:] = [
             x
             for x in workflow.requirements
             if not isinstance(
                 x, (cwl.InlineJavascriptRequirement, cwl.StepInputExpressionRequirement)
             )
         ]
     else:
         workflow.requirements = None
     return workflow, modified
-
-
-if __name__ == "__main__":
-    main()
-    sys.exit(0)
```

### Comparing `cwl-utils-0.8/cwl_utils/docker_extract.py` & `cwl-utils-0.9/cwl_utils/docker_extract.py`

 * *Files identical despite different names*

### Comparing `cwl-utils-0.8/cwl_utils/first_tool.py` & `cwl-utils-0.9/cwl_utils/first_tool.py`

 * *Files identical despite different names*

### Comparing `cwl-utils-0.8/cwl_utils/graph_split.py` & `cwl-utils-0.9/cwl_utils/graph_split.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 #!/usr/bin/env python
 """
 Unpacks the result of `cwltool --unpack`.
 
 Only tested with a single v1.0 workflow.
 """
 
-import os
-import sys
-import json
 import argparse
-from pathlib import Path
-from typing import IO, Any, Dict, List, MutableMapping, Set, Text, Union, cast
+import json
+import os
+from typing import Any, IO, MutableMapping, Set, Text, Union, cast
 
+from cwlformat.formatter import stringify_dict
 from ruamel import yaml
 from schema_salad.sourceline import SourceLine, add_lc_filename
-from cwlformat.formatter import stringify_dict
 
 
 def main() -> None:
     """Split the packed CWL at the path of the first argument."""
     parser = argparse.ArgumentParser(description="Split the packed CWL.")
     parser.add_argument("cwlfile")
     parser.add_argument(
```

### Comparing `cwl-utils-0.8/cwl_utils/image_puller.py` & `cwl-utils-0.9/cwl_utils/image_puller.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,20 +13,18 @@
         """Create an ImagePuller."""
         self.req = req
         self.save_directory = save_directory
 
     @abstractmethod
     def get_image_name(self) -> str:
         """Get the engine-specific image name."""
-        pass
 
     @abstractmethod
     def save_docker_image(self) -> None:
         """Download and save the image to disk."""
-        pass
 
     @staticmethod
     def _run_command_pull(cmd_pull: List[str]) -> None:
         try:
             subprocess.run(
                 cmd_pull, check=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT
             )
```

### Comparing `cwl-utils-0.8/cwl_utils/parser_v1_0.py` & `cwl-utils-0.9/cwl_utils/parser_v1_0.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,34 +21,35 @@
     Union,
 )
 from urllib.parse import quote, urlsplit, urlunsplit
 from urllib.request import pathname2url
 
 from ruamel import yaml
 from ruamel.yaml.comments import CommentedMap
+
 from schema_salad.exceptions import SchemaSaladException, ValidationException
 from schema_salad.fetcher import DefaultFetcher, Fetcher
 from schema_salad.sourceline import SourceLine, add_lc_filename
 
 _vocab = {}  # type: Dict[str, str]
 _rvocab = {}  # type: Dict[str, str]
 
 
-class Savable(object):
+class Savable:
     @classmethod
     def fromDoc(cls, _doc, baseuri, loadingOptions, docRoot=None):
         # type: (Any, str, LoadingOptions, Optional[str]) -> Savable
         pass
 
     def save(self, top=False, base_url="", relative_uris=True):
         # type: (bool, str, bool) -> Dict[str, str]
         pass
 
 
-class LoadingOptions(object):
+class LoadingOptions:
     def __init__(
         self,
         fetcher=None,  # type: Optional[Fetcher]
         namespaces=None,  # type: Optional[Dict[str, str]]
         schemas=None,  # type: Optional[Dict[str, str]]
         fileuri=None,  # type: Optional[str]
         copyfrom=None,  # type: Optional[LoadingOptions]
@@ -68,16 +69,16 @@
             if namespaces is None:
                 self.namespaces = copyfrom.namespaces
             if schemas is None:
                 self.schemas = copyfrom.schemas
 
         if fetcher is None:
             import requests
-            from cachecontrol.wrapper import CacheControl
             from cachecontrol.caches import FileCache
+            from cachecontrol.wrapper import CacheControl
 
             if "HOME" in os.environ:
                 session = CacheControl(
                     requests.Session(),
                     cache=FileCache(
                         os.path.join(os.environ["HOME"], ".cache", "salad")
                     ),
@@ -214,20 +215,20 @@
 
     if vocab_term:
         split = urlsplit(url)
         if bool(split.scheme):
             if url in loadingOptions.rvocab:
                 return loadingOptions.rvocab[url]
         else:
-            raise ValidationException("Term '{}' not in vocabulary".format(url))
+            raise ValidationException(f"Term '{url}' not in vocabulary")
 
     return url
 
 
-class _Loader(object):
+class _Loader:
     def load(self, doc, baseuri, loadingOptions, docRoot=None):
         # type: (Any, str, LoadingOptions, Optional[str]) -> Any
         pass
 
 
 class _AnyLoader(_Loader):
     def load(self, doc, baseuri, loadingOptions, docRoot=None):
@@ -279,28 +280,78 @@
             except ValidationException as e:
                 errors.append(e.with_sourceline(SourceLine(doc, i, str)))
         if errors:
             raise ValidationException("", None, errors)
         return r
 
     def __repr__(self):  # type: () -> str
-        return "array<{}>".format(self.items)
+        return f"array<{self.items}>"
 
 
 class _EnumLoader(_Loader):
     def __init__(self, symbols):
         # type: (Sequence[str]) -> None
         self.symbols = symbols
 
     def load(self, doc, baseuri, loadingOptions, docRoot=None):
         # type: (Any, str, LoadingOptions, Optional[str]) -> Any
         if doc in self.symbols:
             return doc
         else:
-            raise ValidationException("Expected one of {}".format(self.symbols))
+            raise ValidationException(f"Expected one of {self.symbols}")
+
+
+class _SecondaryDSLLoader(_Loader):
+    def __init__(self, inner):
+        # type: (_Loader) -> None
+        self.inner = inner
+
+    def load(self, doc, baseuri, loadingOptions, docRoot=None):
+        # type: (Any, str, LoadingOptions, Optional[str]) -> Any
+        r: List[Dict[str, Any]] = []
+        if isinstance(doc, MutableSequence):
+            for d in doc:
+                if isinstance(d, str):
+                    if d.endswith("?"):
+                        r.append({"pattern": d[:-1], "required": False})
+                    else:
+                        r.append({"pattern": d})
+                elif isinstance(d, dict):
+                    new_dict: Dict[str, Any] = {}
+                    if "pattern" in d:
+                        new_dict["pattern"] = d.pop("pattern")
+                    else:
+                        raise ValidationException(
+                            "Missing pattern in secondaryFiles specification entry: {}".format(
+                                d
+                            )
+                        )
+                    new_dict["required"] = (
+                        d.pop("required") if "required" in d else None
+                    )
+
+                    if len(d):
+                        raise ValidationException(
+                            "Unallowed values in secondaryFiles specification entry: {}".format(
+                                d
+                            )
+                        )
+
+                else:
+                    raise ValidationException(
+                        "Expected a string or sequence of (strings or mappings)."
+                    )
+        elif isinstance(doc, str):
+            if doc.endswith("?"):
+                r.append({"pattern": doc[:-1], "required": False})
+            else:
+                r.append({"pattern": doc})
+        else:
+            raise ValidationException("Expected str or sequence of str")
+        return self.inner.load(r, baseuri, loadingOptions, docRoot)
 
 
 class _RecordLoader(_Loader):
     def __init__(self, classtype):
         # type: (Type[Savable]) -> None
         self.classtype = classtype
 
@@ -310,30 +361,39 @@
             raise ValidationException("Expected a dict")
         return self.classtype.fromDoc(doc, baseuri, loadingOptions, docRoot=docRoot)
 
     def __repr__(self):  # type: () -> str
         return str(self.classtype)
 
 
+class _ExpressionLoader(_Loader):
+    def __init__(self, items: Type[str]) -> None:
+        self.items = items
+
+    def load(self, doc, baseuri, loadingOptions, docRoot=None):
+        # type: (Any, str, LoadingOptions, Optional[str]) -> Any
+        if not isinstance(doc, str):
+            raise ValidationException("Expected a str")
+        return doc
+
+
 class _UnionLoader(_Loader):
     def __init__(self, alternates):
         # type: (Sequence[_Loader]) -> None
         self.alternates = alternates
 
     def load(self, doc, baseuri, loadingOptions, docRoot=None):
         # type: (Any, str, LoadingOptions, Optional[str]) -> Any
         errors = []
         for t in self.alternates:
             try:
                 return t.load(doc, baseuri, loadingOptions, docRoot=docRoot)
             except ValidationException as e:
                 errors.append(
-                    ValidationException(
-                        "tried {} but".format(t.__class__.__name__), None, [e]
-                    )
+                    ValidationException(f"tried {t.__class__.__name__} but", None, [e])
                 )
         raise ValidationException("", None, errors, "-")
 
     def __repr__(self):  # type: () -> str
         return " | ".join(str(a) for a in self.alternates)
 
 
@@ -344,26 +404,31 @@
         self.scoped_id = scoped_id
         self.vocab_term = vocab_term
         self.scoped_ref = scoped_ref
 
     def load(self, doc, baseuri, loadingOptions, docRoot=None):
         # type: (Any, str, LoadingOptions, Optional[str]) -> Any
         if isinstance(doc, MutableSequence):
-            doc = [
-                expand_url(
-                    i,
-                    baseuri,
-                    loadingOptions,
-                    self.scoped_id,
-                    self.vocab_term,
-                    self.scoped_ref,
-                )
-                for i in doc
-            ]
-        if isinstance(doc, str):
+            newdoc = []
+            for i in doc:
+                if isinstance(i, str):
+                    newdoc.append(
+                        expand_url(
+                            i,
+                            baseuri,
+                            loadingOptions,
+                            self.scoped_id,
+                            self.vocab_term,
+                            self.scoped_ref,
+                        )
+                    )
+                else:
+                    newdoc.append(i)
+            doc = newdoc
+        elif isinstance(doc, str):
             doc = expand_url(
                 doc,
                 baseuri,
                 loadingOptions,
                 self.scoped_id,
                 self.vocab_term,
                 self.scoped_ref,
@@ -525,17 +590,17 @@
         pathsp = path.split("#", 2)
         frag = "#" + quote(str(pathsp[1])) if len(pathsp) == 2 else ""
         urlpath = pathname2url(str(pathsp[0]))
     else:
         urlpath = pathname2url(path)
         frag = ""
     if urlpath.startswith("//"):
-        return "file:{}{}".format(urlpath, frag)
+        return f"file:{urlpath}{frag}"
     else:
-        return "file://{}{}".format(urlpath, frag)
+        return f"file://{urlpath}{frag}"
 
 
 def prefix_url(url, namespaces):  # type: (str, Dict[str, str]) -> str
     for k, v in namespaces.items():
         if url.startswith(v):
             return k + ":" + url[len(v) :]
     return url
@@ -668,15 +733,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `name`, `doc`, `type`" % (k),
+                            "invalid field `{}`, expected one of: `name`, `doc`, `type`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'RecordField'", None, _errors__)
@@ -787,15 +852,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `fields`, `type`" % (k),
+                            "invalid field `{}`, expected one of: `fields`, `type`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'RecordSchema'", None, _errors__)
@@ -897,15 +962,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `symbols`, `type`" % (k),
+                            "invalid field `{}`, expected one of: `symbols`, `type`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'EnumSchema'", None, _errors__)
@@ -1006,15 +1071,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `items`, `type`" % (k),
+                            "invalid field `{}`, expected one of: `items`, `type`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'ArraySchema'", None, _errors__)
@@ -1339,15 +1404,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `location`, `path`, `basename`, `dirname`, `nameroot`, `nameext`, `checksum`, `size`, `secondaryFiles`, `format`, `contents`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `location`, `path`, `basename`, `dirname`, `nameroot`, `nameext`, `checksum`, `size`, `secondaryFiles`, `format`, `contents`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'File'", None, _errors__)
@@ -1608,15 +1673,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `location`, `path`, `basename`, `listing`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `location`, `path`, `basename`, `listing`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'Directory'", None, _errors__)
@@ -1822,15 +1887,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `name`, `doc`, `type`, `inputBinding`, `label`" % (k),
+                            "invalid field `{}`, expected one of: `name`, `doc`, `type`, `inputBinding`, `label`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'InputRecordField'", None, _errors__)
@@ -1994,15 +2059,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `fields`, `type`, `label`, `name`" % (k),
+                            "invalid field `{}`, expected one of: `fields`, `type`, `label`, `name`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'InputRecordSchema'", None, _errors__)
@@ -2172,15 +2237,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `symbols`, `type`, `label`, `name`, `inputBinding`" % (k),
+                            "invalid field `{}`, expected one of: `symbols`, `type`, `label`, `name`, `inputBinding`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'InputEnumSchema'", None, _errors__)
@@ -2337,15 +2402,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `items`, `type`, `label`, `inputBinding`" % (k),
+                            "invalid field `{}`, expected one of: `items`, `type`, `label`, `inputBinding`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'InputArraySchema'", None, _errors__)
@@ -2502,15 +2567,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `name`, `doc`, `type`, `outputBinding`" % (k),
+                            "invalid field `{}`, expected one of: `name`, `doc`, `type`, `outputBinding`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'OutputRecordField'", None, _errors__)
@@ -2644,15 +2709,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `fields`, `type`, `label`" % (k),
+                            "invalid field `{}`, expected one of: `fields`, `type`, `label`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'OutputRecordSchema'", None, _errors__)
@@ -2789,15 +2854,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `symbols`, `type`, `label`, `outputBinding`" % (k),
+                            "invalid field `{}`, expected one of: `symbols`, `type`, `label`, `outputBinding`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'OutputEnumSchema'", None, _errors__)
@@ -2944,15 +3009,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `items`, `type`, `label`, `outputBinding`" % (k),
+                            "invalid field `{}`, expected one of: `items`, `type`, `label`, `outputBinding`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'OutputArraySchema'", None, _errors__)
@@ -3192,15 +3257,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `label`, `secondaryFiles`, `streamable`, `doc`, `id`, `format`, `inputBinding`, `default`, `type`" % (k),
+                            "invalid field `{}`, expected one of: `label`, `secondaryFiles`, `streamable`, `doc`, `id`, `format`, `inputBinding`, `default`, `type`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'InputParameter'", None, _errors__)
@@ -3446,15 +3511,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `label`, `secondaryFiles`, `streamable`, `doc`, `id`, `outputBinding`, `format`" % (k),
+                            "invalid field `{}`, expected one of: `label`, `secondaryFiles`, `streamable`, `doc`, `id`, `outputBinding`, `format`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'OutputParameter'", None, _errors__)
@@ -3618,15 +3683,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `expressionLib`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `expressionLib`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'InlineJavascriptRequirement'", None, _errors__)
@@ -3721,15 +3786,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `types`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `types`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'SchemaDefRequirement'", None, _errors__)
@@ -3828,15 +3893,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `envName`, `envValue`" % (k),
+                            "invalid field `{}`, expected one of: `envName`, `envValue`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'EnvironmentDef'", None, _errors__)
@@ -4058,15 +4123,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `loadContents`, `position`, `prefix`, `separate`, `itemSeparator`, `valueFrom`, `shellQuote`" % (k),
+                            "invalid field `{}`, expected one of: `loadContents`, `position`, `prefix`, `separate`, `itemSeparator`, `valueFrom`, `shellQuote`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandLineBinding'", None, _errors__)
@@ -4234,15 +4299,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `glob`, `loadContents`, `outputEval`" % (k),
+                            "invalid field `{}`, expected one of: `glob`, `loadContents`, `outputEval`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandOutputBinding'", None, _errors__)
@@ -4405,15 +4470,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `name`, `doc`, `type`, `inputBinding`, `label`" % (k),
+                            "invalid field `{}`, expected one of: `name`, `doc`, `type`, `inputBinding`, `label`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandInputRecordField'", None, _errors__)
@@ -4577,15 +4642,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `fields`, `type`, `label`, `name`" % (k),
+                            "invalid field `{}`, expected one of: `fields`, `type`, `label`, `name`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandInputRecordSchema'", None, _errors__)
@@ -4755,15 +4820,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `symbols`, `type`, `label`, `name`, `inputBinding`" % (k),
+                            "invalid field `{}`, expected one of: `symbols`, `type`, `label`, `name`, `inputBinding`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandInputEnumSchema'", None, _errors__)
@@ -4920,15 +4985,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `items`, `type`, `label`, `inputBinding`" % (k),
+                            "invalid field `{}`, expected one of: `items`, `type`, `label`, `inputBinding`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandInputArraySchema'", None, _errors__)
@@ -5085,15 +5150,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `name`, `doc`, `type`, `outputBinding`" % (k),
+                            "invalid field `{}`, expected one of: `name`, `doc`, `type`, `outputBinding`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandOutputRecordField'", None, _errors__)
@@ -5250,15 +5315,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `fields`, `type`, `label`, `name`" % (k),
+                            "invalid field `{}`, expected one of: `fields`, `type`, `label`, `name`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandOutputRecordSchema'", None, _errors__)
@@ -5405,15 +5470,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `symbols`, `type`, `label`, `outputBinding`" % (k),
+                            "invalid field `{}`, expected one of: `symbols`, `type`, `label`, `outputBinding`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandOutputEnumSchema'", None, _errors__)
@@ -5560,15 +5625,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `items`, `type`, `label`, `outputBinding`" % (k),
+                            "invalid field `{}`, expected one of: `items`, `type`, `label`, `outputBinding`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandOutputArraySchema'", None, _errors__)
@@ -5811,15 +5876,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `label`, `secondaryFiles`, `streamable`, `doc`, `id`, `format`, `inputBinding`, `default`, `type`" % (k),
+                            "invalid field `{}`, expected one of: `label`, `secondaryFiles`, `streamable`, `doc`, `id`, `format`, `inputBinding`, `default`, `type`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandInputParameter'", None, _errors__)
@@ -6084,15 +6149,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `label`, `secondaryFiles`, `streamable`, `doc`, `id`, `outputBinding`, `format`, `type`" % (k),
+                            "invalid field `{}`, expected one of: `label`, `secondaryFiles`, `streamable`, `doc`, `id`, `outputBinding`, `format`, `type`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandOutputParameter'", None, _errors__)
@@ -6478,15 +6543,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `id`, `inputs`, `outputs`, `requirements`, `hints`, `label`, `doc`, `cwlVersion`, `class`, `baseCommand`, `arguments`, `stdin`, `stderr`, `stdout`, `successCodes`, `temporaryFailCodes`, `permanentFailCodes`" % (k),
+                            "invalid field `{}`, expected one of: `id`, `inputs`, `outputs`, `requirements`, `hints`, `label`, `doc`, `cwlVersion`, `class`, `baseCommand`, `arguments`, `stdin`, `stderr`, `stdout`, `successCodes`, `temporaryFailCodes`, `permanentFailCodes`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandLineTool'", None, _errors__)
@@ -6801,15 +6866,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `dockerPull`, `dockerLoad`, `dockerFile`, `dockerImport`, `dockerImageId`, `dockerOutputDirectory`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `dockerPull`, `dockerLoad`, `dockerFile`, `dockerImport`, `dockerImageId`, `dockerOutputDirectory`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'DockerRequirement'", None, _errors__)
@@ -6934,15 +6999,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `packages`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `packages`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'SoftwareRequirement'", None, _errors__)
@@ -7054,15 +7119,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `package`, `version`, `specs`" % (k),
+                            "invalid field `{}`, expected one of: `package`, `version`, `specs`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'SoftwarePackage'", None, _errors__)
@@ -7193,15 +7258,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `entryname`, `entry`, `writable`" % (k),
+                            "invalid field `{}`, expected one of: `entryname`, `entry`, `writable`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'Dirent'", None, _errors__)
@@ -7301,15 +7366,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `listing`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `listing`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'InitialWorkDirRequirement'", None, _errors__)
@@ -7399,15 +7464,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `envDef`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `envDef`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'EnvVarRequirement'", None, _errors__)
@@ -7489,15 +7554,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`" % (k),
+                            "invalid field `{}`, expected one of: `class`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'ShellCommandRequirement'", None, _errors__)
@@ -7713,15 +7778,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `coresMin`, `coresMax`, `ramMin`, `ramMax`, `tmpdirMin`, `tmpdirMax`, `outdirMin`, `outdirMax`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `coresMin`, `coresMax`, `ramMin`, `ramMax`, `tmpdirMin`, `tmpdirMax`, `outdirMin`, `outdirMax`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'ResourceRequirement'", None, _errors__)
@@ -7972,15 +8037,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `label`, `secondaryFiles`, `streamable`, `doc`, `id`, `outputBinding`, `format`, `type`" % (k),
+                            "invalid field `{}`, expected one of: `label`, `secondaryFiles`, `streamable`, `doc`, `id`, `outputBinding`, `format`, `type`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'ExpressionToolOutputParameter'", None, _errors__)
@@ -8251,15 +8316,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `id`, `inputs`, `outputs`, `requirements`, `hints`, `label`, `doc`, `cwlVersion`, `class`, `expression`" % (k),
+                            "invalid field `{}`, expected one of: `id`, `inputs`, `outputs`, `requirements`, `hints`, `label`, `doc`, `cwlVersion`, `class`, `expression`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'ExpressionTool'", None, _errors__)
@@ -8561,15 +8626,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `label`, `secondaryFiles`, `streamable`, `doc`, `id`, `outputBinding`, `format`, `outputSource`, `linkMerge`, `type`" % (k),
+                            "invalid field `{}`, expected one of: `label`, `secondaryFiles`, `streamable`, `doc`, `id`, `outputBinding`, `format`, `outputSource`, `linkMerge`, `type`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'WorkflowOutputParameter'", None, _errors__)
@@ -8839,15 +8904,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `source`, `linkMerge`, `id`, `default`, `valueFrom`" % (k),
+                            "invalid field `{}`, expected one of: `source`, `linkMerge`, `id`, `default`, `valueFrom`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'WorkflowStepInput'", None, _errors__)
@@ -8976,15 +9041,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `id`" % (k),
+                            "invalid field `{}`, expected one of: `id`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'WorkflowStepOutput'", None, _errors__)
@@ -9268,15 +9333,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `id`, `in`, `out`, `requirements`, `hints`, `label`, `doc`, `run`, `scatter`, `scatterMethod`" % (k),
+                            "invalid field `{}`, expected one of: `id`, `in`, `out`, `requirements`, `hints`, `label`, `doc`, `run`, `scatter`, `scatterMethod`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'WorkflowStep'", None, _errors__)
@@ -9386,15 +9451,15 @@
 
 class Workflow(Process):
     """
 A workflow describes a set of **steps** and the **dependencies** between
 those steps.  When a step produces output that will be consumed by a
 second step, the first step is a dependency of the second step.
 
-When there is a dependency, the workflow engine must execute the preceeding
+When there is a dependency, the workflow engine must execute the preceding
 step and wait for it to successfully produce output before executing the
 dependent step.  If two steps are defined in the workflow graph that
 are not directly or indirectly dependent, these steps are **independent**,
 and may execute in any order or execute concurrently.  A workflow is
 complete when all steps have been executed.
 
 Dependencies between parameters are expressed using the `source` field on
@@ -9614,15 +9679,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `id`, `inputs`, `outputs`, `requirements`, `hints`, `label`, `doc`, `cwlVersion`, `class`, `steps`" % (k),
+                            "invalid field `{}`, expected one of: `id`, `inputs`, `outputs`, `requirements`, `hints`, `label`, `doc`, `cwlVersion`, `class`, `steps`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'Workflow'", None, _errors__)
@@ -9761,15 +9826,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`" % (k),
+                            "invalid field `{}`, expected one of: `class`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'SubworkflowFeatureRequirement'", None, _errors__)
@@ -9839,15 +9904,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`" % (k),
+                            "invalid field `{}`, expected one of: `class`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'ScatterFeatureRequirement'", None, _errors__)
@@ -9917,15 +9982,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`" % (k),
+                            "invalid field `{}`, expected one of: `class`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'MultipleInputFeatureRequirement'", None, _errors__)
@@ -9995,15 +10060,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`" % (k),
+                            "invalid field `{}`, expected one of: `class`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'StepInputExpressionRequirement'", None, _errors__)
@@ -10241,15 +10306,15 @@
 ArraySchemaLoader = _RecordLoader(ArraySchema)
 CWLVersionLoader = _EnumLoader(("draft-2", "draft-3.dev1", "draft-3.dev2", "draft-3.dev3", "draft-3.dev4", "draft-3.dev5", "draft-3", "draft-4.dev1", "draft-4.dev2", "draft-4.dev3", "v1.0.dev4", "v1.0",))
 CWLTypeLoader = _EnumLoader(("File", "Directory",))
 FileLoader = _RecordLoader(File)
 DirectoryLoader = _RecordLoader(Directory)
 SchemaBaseLoader = _RecordLoader(SchemaBase)
 ParameterLoader = _RecordLoader(Parameter)
-ExpressionLoader = _EnumLoader(("ExpressionPlaceholder",))
+ExpressionLoader = _ExpressionLoader(str)
 InputBindingLoader = _RecordLoader(InputBinding)
 OutputBindingLoader = _RecordLoader(OutputBinding)
 InputSchemaLoader = _RecordLoader(InputSchema)
 OutputSchemaLoader = _RecordLoader(OutputSchema)
 InputRecordFieldLoader = _RecordLoader(InputRecordField)
 InputRecordSchemaLoader = _RecordLoader(InputRecordSchema)
 InputEnumSchemaLoader = _RecordLoader(InputEnumSchema)
@@ -10457,7 +10522,21 @@
     add_lc_filename(result, uri)
 
     if loadingOptions is None:
         loadingOptions = LoadingOptions(fileuri=uri)
     loadingOptions.idx[uri] = result
 
     return _document_load(union_of_CommandLineToolLoader_or_ExpressionToolLoader_or_WorkflowLoader_or_array_of_union_of_CommandLineToolLoader_or_ExpressionToolLoader_or_WorkflowLoader, result, uri, loadingOptions)
+
+
+def load_document_by_yaml(yaml, uri, loadingOptions=None):
+    # type: (Any, str, Optional[LoadingOptions]) -> Any
+    '''Shortcut to load via a YAML object.
+    yaml: must be from ruamel.yaml.main.round_trip_load with preserve_quotes=True
+    '''
+    add_lc_filename(yaml, uri)
+
+    if loadingOptions is None:
+        loadingOptions = LoadingOptions(fileuri=uri)
+    loadingOptions.idx[uri] = yaml
+
+    return _document_load(union_of_CommandLineToolLoader_or_ExpressionToolLoader_or_WorkflowLoader_or_array_of_union_of_CommandLineToolLoader_or_ExpressionToolLoader_or_WorkflowLoader, yaml, uri, loadingOptions)
```

### Comparing `cwl-utils-0.8/cwl_utils/parser_v1_1.py` & `cwl-utils-0.9/cwl_utils/parser_v1_1.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,34 +21,35 @@
     Union,
 )
 from urllib.parse import quote, urlsplit, urlunsplit
 from urllib.request import pathname2url
 
 from ruamel import yaml
 from ruamel.yaml.comments import CommentedMap
+
 from schema_salad.exceptions import SchemaSaladException, ValidationException
 from schema_salad.fetcher import DefaultFetcher, Fetcher
 from schema_salad.sourceline import SourceLine, add_lc_filename
 
 _vocab = {}  # type: Dict[str, str]
 _rvocab = {}  # type: Dict[str, str]
 
 
-class Savable(object):
+class Savable:
     @classmethod
     def fromDoc(cls, _doc, baseuri, loadingOptions, docRoot=None):
         # type: (Any, str, LoadingOptions, Optional[str]) -> Savable
         pass
 
     def save(self, top=False, base_url="", relative_uris=True):
         # type: (bool, str, bool) -> Dict[str, str]
         pass
 
 
-class LoadingOptions(object):
+class LoadingOptions:
     def __init__(
         self,
         fetcher=None,  # type: Optional[Fetcher]
         namespaces=None,  # type: Optional[Dict[str, str]]
         schemas=None,  # type: Optional[Dict[str, str]]
         fileuri=None,  # type: Optional[str]
         copyfrom=None,  # type: Optional[LoadingOptions]
@@ -68,16 +69,16 @@
             if namespaces is None:
                 self.namespaces = copyfrom.namespaces
             if schemas is None:
                 self.schemas = copyfrom.schemas
 
         if fetcher is None:
             import requests
-            from cachecontrol.wrapper import CacheControl
             from cachecontrol.caches import FileCache
+            from cachecontrol.wrapper import CacheControl
 
             if "HOME" in os.environ:
                 session = CacheControl(
                     requests.Session(),
                     cache=FileCache(
                         os.path.join(os.environ["HOME"], ".cache", "salad")
                     ),
@@ -214,20 +215,20 @@
 
     if vocab_term:
         split = urlsplit(url)
         if bool(split.scheme):
             if url in loadingOptions.rvocab:
                 return loadingOptions.rvocab[url]
         else:
-            raise ValidationException("Term '{}' not in vocabulary".format(url))
+            raise ValidationException(f"Term '{url}' not in vocabulary")
 
     return url
 
 
-class _Loader(object):
+class _Loader:
     def load(self, doc, baseuri, loadingOptions, docRoot=None):
         # type: (Any, str, LoadingOptions, Optional[str]) -> Any
         pass
 
 
 class _AnyLoader(_Loader):
     def load(self, doc, baseuri, loadingOptions, docRoot=None):
@@ -279,28 +280,78 @@
             except ValidationException as e:
                 errors.append(e.with_sourceline(SourceLine(doc, i, str)))
         if errors:
             raise ValidationException("", None, errors)
         return r
 
     def __repr__(self):  # type: () -> str
-        return "array<{}>".format(self.items)
+        return f"array<{self.items}>"
 
 
 class _EnumLoader(_Loader):
     def __init__(self, symbols):
         # type: (Sequence[str]) -> None
         self.symbols = symbols
 
     def load(self, doc, baseuri, loadingOptions, docRoot=None):
         # type: (Any, str, LoadingOptions, Optional[str]) -> Any
         if doc in self.symbols:
             return doc
         else:
-            raise ValidationException("Expected one of {}".format(self.symbols))
+            raise ValidationException(f"Expected one of {self.symbols}")
+
+
+class _SecondaryDSLLoader(_Loader):
+    def __init__(self, inner):
+        # type: (_Loader) -> None
+        self.inner = inner
+
+    def load(self, doc, baseuri, loadingOptions, docRoot=None):
+        # type: (Any, str, LoadingOptions, Optional[str]) -> Any
+        r: List[Dict[str, Any]] = []
+        if isinstance(doc, MutableSequence):
+            for d in doc:
+                if isinstance(d, str):
+                    if d.endswith("?"):
+                        r.append({"pattern": d[:-1], "required": False})
+                    else:
+                        r.append({"pattern": d})
+                elif isinstance(d, dict):
+                    new_dict: Dict[str, Any] = {}
+                    if "pattern" in d:
+                        new_dict["pattern"] = d.pop("pattern")
+                    else:
+                        raise ValidationException(
+                            "Missing pattern in secondaryFiles specification entry: {}".format(
+                                d
+                            )
+                        )
+                    new_dict["required"] = (
+                        d.pop("required") if "required" in d else None
+                    )
+
+                    if len(d):
+                        raise ValidationException(
+                            "Unallowed values in secondaryFiles specification entry: {}".format(
+                                d
+                            )
+                        )
+
+                else:
+                    raise ValidationException(
+                        "Expected a string or sequence of (strings or mappings)."
+                    )
+        elif isinstance(doc, str):
+            if doc.endswith("?"):
+                r.append({"pattern": doc[:-1], "required": False})
+            else:
+                r.append({"pattern": doc})
+        else:
+            raise ValidationException("Expected str or sequence of str")
+        return self.inner.load(r, baseuri, loadingOptions, docRoot)
 
 
 class _RecordLoader(_Loader):
     def __init__(self, classtype):
         # type: (Type[Savable]) -> None
         self.classtype = classtype
 
@@ -310,30 +361,39 @@
             raise ValidationException("Expected a dict")
         return self.classtype.fromDoc(doc, baseuri, loadingOptions, docRoot=docRoot)
 
     def __repr__(self):  # type: () -> str
         return str(self.classtype)
 
 
+class _ExpressionLoader(_Loader):
+    def __init__(self, items: Type[str]) -> None:
+        self.items = items
+
+    def load(self, doc, baseuri, loadingOptions, docRoot=None):
+        # type: (Any, str, LoadingOptions, Optional[str]) -> Any
+        if not isinstance(doc, str):
+            raise ValidationException("Expected a str")
+        return doc
+
+
 class _UnionLoader(_Loader):
     def __init__(self, alternates):
         # type: (Sequence[_Loader]) -> None
         self.alternates = alternates
 
     def load(self, doc, baseuri, loadingOptions, docRoot=None):
         # type: (Any, str, LoadingOptions, Optional[str]) -> Any
         errors = []
         for t in self.alternates:
             try:
                 return t.load(doc, baseuri, loadingOptions, docRoot=docRoot)
             except ValidationException as e:
                 errors.append(
-                    ValidationException(
-                        "tried {} but".format(t.__class__.__name__), None, [e]
-                    )
+                    ValidationException(f"tried {t.__class__.__name__} but", None, [e])
                 )
         raise ValidationException("", None, errors, "-")
 
     def __repr__(self):  # type: () -> str
         return " | ".join(str(a) for a in self.alternates)
 
 
@@ -344,26 +404,31 @@
         self.scoped_id = scoped_id
         self.vocab_term = vocab_term
         self.scoped_ref = scoped_ref
 
     def load(self, doc, baseuri, loadingOptions, docRoot=None):
         # type: (Any, str, LoadingOptions, Optional[str]) -> Any
         if isinstance(doc, MutableSequence):
-            doc = [
-                expand_url(
-                    i,
-                    baseuri,
-                    loadingOptions,
-                    self.scoped_id,
-                    self.vocab_term,
-                    self.scoped_ref,
-                )
-                for i in doc
-            ]
-        if isinstance(doc, str):
+            newdoc = []
+            for i in doc:
+                if isinstance(i, str):
+                    newdoc.append(
+                        expand_url(
+                            i,
+                            baseuri,
+                            loadingOptions,
+                            self.scoped_id,
+                            self.vocab_term,
+                            self.scoped_ref,
+                        )
+                    )
+                else:
+                    newdoc.append(i)
+            doc = newdoc
+        elif isinstance(doc, str):
             doc = expand_url(
                 doc,
                 baseuri,
                 loadingOptions,
                 self.scoped_id,
                 self.vocab_term,
                 self.scoped_ref,
@@ -525,17 +590,17 @@
         pathsp = path.split("#", 2)
         frag = "#" + quote(str(pathsp[1])) if len(pathsp) == 2 else ""
         urlpath = pathname2url(str(pathsp[0]))
     else:
         urlpath = pathname2url(path)
         frag = ""
     if urlpath.startswith("//"):
-        return "file:{}{}".format(urlpath, frag)
+        return f"file:{urlpath}{frag}"
     else:
-        return "file://{}{}".format(urlpath, frag)
+        return f"file://{urlpath}{frag}"
 
 
 def prefix_url(url, namespaces):  # type: (str, Dict[str, str]) -> str
     for k, v in namespaces.items():
         if url.startswith(v):
             return k + ":" + url[len(v) :]
     return url
@@ -672,15 +737,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `doc`, `name`, `type`" % (k),
+                            "invalid field `{}`, expected one of: `doc`, `name`, `type`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'RecordField'", None, _errors__)
@@ -791,15 +856,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `fields`, `type`" % (k),
+                            "invalid field `{}`, expected one of: `fields`, `type`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'RecordSchema'", None, _errors__)
@@ -901,15 +966,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `symbols`, `type`" % (k),
+                            "invalid field `{}`, expected one of: `symbols`, `type`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'EnumSchema'", None, _errors__)
@@ -1010,15 +1075,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `items`, `type`" % (k),
+                            "invalid field `{}`, expected one of: `items`, `type`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'ArraySchema'", None, _errors__)
@@ -1290,15 +1355,15 @@
                     )
                 )
         else:
             size = None
         if 'secondaryFiles' in _doc:
             try:
                 secondaryFiles = load_field(_doc.get(
-                    'secondaryFiles'), union_of_None_type_or_array_of_union_of_FileLoader_or_DirectoryLoader, baseuri, loadingOptions)
+                    'secondaryFiles'), secondaryfilesdsl_union_of_None_type_or_array_of_union_of_FileLoader_or_DirectoryLoader, baseuri, loadingOptions)
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
                         "the `secondaryFiles` field is not valid because:",
                         SourceLine(_doc, 'secondaryFiles', str),
                         [e]
                     )
@@ -1343,15 +1408,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `location`, `path`, `basename`, `dirname`, `nameroot`, `nameext`, `checksum`, `size`, `secondaryFiles`, `format`, `contents`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `location`, `path`, `basename`, `dirname`, `nameroot`, `nameext`, `checksum`, `size`, `secondaryFiles`, `format`, `contents`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'File'", None, _errors__)
@@ -1612,15 +1677,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `location`, `path`, `basename`, `listing`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `location`, `path`, `basename`, `listing`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'Directory'", None, _errors__)
@@ -1762,15 +1827,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `loadContents`" % (k),
+                            "invalid field `{}`, expected one of: `loadContents`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'InputBinding'", None, _errors__)
@@ -1914,15 +1979,15 @@
                     )
                 )
         else:
             label = None
         if 'secondaryFiles' in _doc:
             try:
                 secondaryFiles = load_field(_doc.get(
-                    'secondaryFiles'), union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
+                    'secondaryFiles'), secondaryfilesdsl_union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
                         "the `secondaryFiles` field is not valid because:",
                         SourceLine(_doc, 'secondaryFiles', str),
                         [e]
                     )
@@ -1995,15 +2060,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `doc`, `name`, `type`, `label`, `secondaryFiles`, `streamable`, `format`, `loadContents`, `loadListing`" % (k),
+                            "invalid field `{}`, expected one of: `doc`, `name`, `type`, `label`, `secondaryFiles`, `streamable`, `format`, `loadContents`, `loadListing`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'InputRecordField'", None, _errors__)
@@ -2214,15 +2279,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `fields`, `type`, `label`, `doc`, `name`" % (k),
+                            "invalid field `{}`, expected one of: `fields`, `type`, `label`, `doc`, `name`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'InputRecordSchema'", None, _errors__)
@@ -2399,15 +2464,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `symbols`, `type`, `label`, `doc`, `name`" % (k),
+                            "invalid field `{}`, expected one of: `symbols`, `type`, `label`, `doc`, `name`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'InputEnumSchema'", None, _errors__)
@@ -2587,15 +2652,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `items`, `type`, `label`, `doc`, `name`" % (k),
+                            "invalid field `{}`, expected one of: `items`, `type`, `label`, `doc`, `name`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'InputArraySchema'", None, _errors__)
@@ -2757,15 +2822,15 @@
                     )
                 )
         else:
             label = None
         if 'secondaryFiles' in _doc:
             try:
                 secondaryFiles = load_field(_doc.get(
-                    'secondaryFiles'), union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
+                    'secondaryFiles'), secondaryfilesdsl_union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
                         "the `secondaryFiles` field is not valid because:",
                         SourceLine(_doc, 'secondaryFiles', str),
                         [e]
                     )
@@ -2810,15 +2875,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `doc`, `name`, `type`, `label`, `secondaryFiles`, `streamable`, `format`" % (k),
+                            "invalid field `{}`, expected one of: `doc`, `name`, `type`, `label`, `secondaryFiles`, `streamable`, `format`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'OutputRecordField'", None, _errors__)
@@ -3015,15 +3080,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `fields`, `type`, `label`, `doc`, `name`" % (k),
+                            "invalid field `{}`, expected one of: `fields`, `type`, `label`, `doc`, `name`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'OutputRecordSchema'", None, _errors__)
@@ -3200,15 +3265,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `symbols`, `type`, `label`, `doc`, `name`" % (k),
+                            "invalid field `{}`, expected one of: `symbols`, `type`, `label`, `doc`, `name`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'OutputEnumSchema'", None, _errors__)
@@ -3388,15 +3453,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `items`, `type`, `label`, `doc`, `name`" % (k),
+                            "invalid field `{}`, expected one of: `items`, `type`, `label`, `doc`, `name`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'OutputArraySchema'", None, _errors__)
@@ -3554,15 +3619,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `expressionLib`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `expressionLib`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'InlineJavascriptRequirement'", None, _errors__)
@@ -3661,15 +3726,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `types`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `types`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'SchemaDefRequirement'", None, _errors__)
@@ -3765,15 +3830,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `pattern`, `required`" % (k),
+                            "invalid field `{}`, expected one of: `pattern`, `required`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'SecondaryFileSchema'", None, _errors__)
@@ -3871,15 +3936,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `loadListing`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `loadListing`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'LoadListingRequirement'", None, _errors__)
@@ -3978,15 +4043,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `envName`, `envValue`" % (k),
+                            "invalid field `{}`, expected one of: `envName`, `envValue`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'EnvironmentDef'", None, _errors__)
@@ -4208,15 +4273,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `loadContents`, `position`, `prefix`, `separate`, `itemSeparator`, `valueFrom`, `shellQuote`" % (k),
+                            "invalid field `{}`, expected one of: `loadContents`, `position`, `prefix`, `separate`, `itemSeparator`, `valueFrom`, `shellQuote`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandLineBinding'", None, _errors__)
@@ -4400,15 +4465,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `loadContents`, `loadListing`, `glob`, `outputEval`" % (k),
+                            "invalid field `{}`, expected one of: `loadContents`, `loadListing`, `glob`, `outputEval`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandOutputBinding'", None, _errors__)
@@ -4510,15 +4575,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `inputBinding`" % (k),
+                            "invalid field `{}`, expected one of: `inputBinding`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandLineBindable'", None, _errors__)
@@ -4652,15 +4717,15 @@
                     )
                 )
         else:
             label = None
         if 'secondaryFiles' in _doc:
             try:
                 secondaryFiles = load_field(_doc.get(
-                    'secondaryFiles'), union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
+                    'secondaryFiles'), secondaryfilesdsl_union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
                         "the `secondaryFiles` field is not valid because:",
                         SourceLine(_doc, 'secondaryFiles', str),
                         [e]
                     )
@@ -4747,15 +4812,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `doc`, `name`, `type`, `label`, `secondaryFiles`, `streamable`, `format`, `loadContents`, `loadListing`, `inputBinding`" % (k),
+                            "invalid field `{}`, expected one of: `doc`, `name`, `type`, `label`, `secondaryFiles`, `streamable`, `format`, `loadContents`, `loadListing`, `inputBinding`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandInputRecordField'", None, _errors__)
@@ -4989,15 +5054,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `fields`, `type`, `label`, `doc`, `name`, `inputBinding`" % (k),
+                            "invalid field `{}`, expected one of: `fields`, `type`, `label`, `doc`, `name`, `inputBinding`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandInputRecordSchema'", None, _errors__)
@@ -5197,15 +5262,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `symbols`, `type`, `label`, `doc`, `name`, `inputBinding`" % (k),
+                            "invalid field `{}`, expected one of: `symbols`, `type`, `label`, `doc`, `name`, `inputBinding`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandInputEnumSchema'", None, _errors__)
@@ -5408,15 +5473,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `items`, `type`, `label`, `doc`, `name`, `inputBinding`" % (k),
+                            "invalid field `{}`, expected one of: `items`, `type`, `label`, `doc`, `name`, `inputBinding`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandInputArraySchema'", None, _errors__)
@@ -5587,15 +5652,15 @@
                     )
                 )
         else:
             label = None
         if 'secondaryFiles' in _doc:
             try:
                 secondaryFiles = load_field(_doc.get(
-                    'secondaryFiles'), union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
+                    'secondaryFiles'), secondaryfilesdsl_union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
                         "the `secondaryFiles` field is not valid because:",
                         SourceLine(_doc, 'secondaryFiles', str),
                         [e]
                     )
@@ -5654,15 +5719,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `doc`, `name`, `type`, `label`, `secondaryFiles`, `streamable`, `format`, `outputBinding`" % (k),
+                            "invalid field `{}`, expected one of: `doc`, `name`, `type`, `label`, `secondaryFiles`, `streamable`, `format`, `outputBinding`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandOutputRecordField'", None, _errors__)
@@ -5866,15 +5931,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `fields`, `type`, `label`, `doc`, `name`" % (k),
+                            "invalid field `{}`, expected one of: `fields`, `type`, `label`, `doc`, `name`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandOutputRecordSchema'", None, _errors__)
@@ -6051,15 +6116,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `symbols`, `type`, `label`, `doc`, `name`" % (k),
+                            "invalid field `{}`, expected one of: `symbols`, `type`, `label`, `doc`, `name`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandOutputEnumSchema'", None, _errors__)
@@ -6239,15 +6304,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `items`, `type`, `label`, `doc`, `name`" % (k),
+                            "invalid field `{}`, expected one of: `items`, `type`, `label`, `doc`, `name`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandOutputArraySchema'", None, _errors__)
@@ -6395,15 +6460,15 @@
                     )
                 )
         else:
             label = None
         if 'secondaryFiles' in _doc:
             try:
                 secondaryFiles = load_field(_doc.get(
-                    'secondaryFiles'), union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
+                    'secondaryFiles'), secondaryfilesdsl_union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
                         "the `secondaryFiles` field is not valid because:",
                         SourceLine(_doc, 'secondaryFiles', str),
                         [e]
                     )
@@ -6529,15 +6594,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `label`, `secondaryFiles`, `streamable`, `doc`, `id`, `format`, `loadContents`, `loadListing`, `default`, `type`, `inputBinding`" % (k),
+                            "invalid field `{}`, expected one of: `label`, `secondaryFiles`, `streamable`, `doc`, `id`, `format`, `loadContents`, `loadListing`, `default`, `type`, `inputBinding`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandInputParameter'", None, _errors__)
@@ -6721,15 +6786,15 @@
                     )
                 )
         else:
             label = None
         if 'secondaryFiles' in _doc:
             try:
                 secondaryFiles = load_field(_doc.get(
-                    'secondaryFiles'), union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
+                    'secondaryFiles'), secondaryfilesdsl_union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
                         "the `secondaryFiles` field is not valid because:",
                         SourceLine(_doc, 'secondaryFiles', str),
                         [e]
                     )
@@ -6813,15 +6878,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `label`, `secondaryFiles`, `streamable`, `doc`, `id`, `format`, `type`, `outputBinding`" % (k),
+                            "invalid field `{}`, expected one of: `label`, `secondaryFiles`, `streamable`, `doc`, `id`, `format`, `type`, `outputBinding`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandOutputParameter'", None, _errors__)
@@ -7207,15 +7272,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `id`, `label`, `doc`, `inputs`, `outputs`, `requirements`, `hints`, `cwlVersion`, `class`, `baseCommand`, `arguments`, `stdin`, `stderr`, `stdout`, `successCodes`, `temporaryFailCodes`, `permanentFailCodes`" % (k),
+                            "invalid field `{}`, expected one of: `id`, `label`, `doc`, `inputs`, `outputs`, `requirements`, `hints`, `cwlVersion`, `class`, `baseCommand`, `arguments`, `stdin`, `stderr`, `stdout`, `successCodes`, `temporaryFailCodes`, `permanentFailCodes`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandLineTool'", None, _errors__)
@@ -7548,15 +7613,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `dockerPull`, `dockerLoad`, `dockerFile`, `dockerImport`, `dockerImageId`, `dockerOutputDirectory`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `dockerPull`, `dockerLoad`, `dockerFile`, `dockerImport`, `dockerImageId`, `dockerOutputDirectory`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'DockerRequirement'", None, _errors__)
@@ -7681,15 +7746,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `packages`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `packages`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'SoftwareRequirement'", None, _errors__)
@@ -7801,15 +7866,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `package`, `version`, `specs`" % (k),
+                            "invalid field `{}`, expected one of: `package`, `version`, `specs`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'SoftwarePackage'", None, _errors__)
@@ -7943,15 +8008,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `entryname`, `entry`, `writable`" % (k),
+                            "invalid field `{}`, expected one of: `entryname`, `entry`, `writable`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'Dirent'", None, _errors__)
@@ -8051,15 +8116,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `listing`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `listing`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'InitialWorkDirRequirement'", None, _errors__)
@@ -8149,15 +8214,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `envDef`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `envDef`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'EnvVarRequirement'", None, _errors__)
@@ -8239,15 +8304,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`" % (k),
+                            "invalid field `{}`, expected one of: `class`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'ShellCommandRequirement'", None, _errors__)
@@ -8463,15 +8528,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `coresMin`, `coresMax`, `ramMin`, `ramMax`, `tmpdirMin`, `tmpdirMax`, `outdirMin`, `outdirMax`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `coresMin`, `coresMax`, `ramMin`, `ramMax`, `tmpdirMin`, `tmpdirMax`, `outdirMin`, `outdirMax`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'ResourceRequirement'", None, _errors__)
@@ -8617,15 +8682,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `enableReuse`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `enableReuse`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'WorkReuse'", None, _errors__)
@@ -8728,15 +8793,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `networkAccess`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `networkAccess`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'NetworkAccess'", None, _errors__)
@@ -8854,15 +8919,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `inplaceUpdate`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `inplaceUpdate`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'InplaceUpdateRequirement'", None, _errors__)
@@ -8957,15 +9022,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `timelimit`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `timelimit`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'ToolTimeLimit'", None, _errors__)
@@ -9070,15 +9135,15 @@
                     )
                 )
         else:
             label = None
         if 'secondaryFiles' in _doc:
             try:
                 secondaryFiles = load_field(_doc.get(
-                    'secondaryFiles'), union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
+                    'secondaryFiles'), secondaryfilesdsl_union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
                         "the `secondaryFiles` field is not valid because:",
                         SourceLine(_doc, 'secondaryFiles', str),
                         [e]
                     )
@@ -9148,15 +9213,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `label`, `secondaryFiles`, `streamable`, `doc`, `id`, `format`, `type`" % (k),
+                            "invalid field `{}`, expected one of: `label`, `secondaryFiles`, `streamable`, `doc`, `id`, `format`, `type`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'ExpressionToolOutputParameter'", None, _errors__)
@@ -9315,15 +9380,15 @@
                     )
                 )
         else:
             label = None
         if 'secondaryFiles' in _doc:
             try:
                 secondaryFiles = load_field(_doc.get(
-                    'secondaryFiles'), union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
+                    'secondaryFiles'), secondaryfilesdsl_union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
                         "the `secondaryFiles` field is not valid because:",
                         SourceLine(_doc, 'secondaryFiles', str),
                         [e]
                     )
@@ -9449,15 +9514,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `label`, `secondaryFiles`, `streamable`, `doc`, `id`, `format`, `loadContents`, `loadListing`, `default`, `type`, `inputBinding`" % (k),
+                            "invalid field `{}`, expected one of: `label`, `secondaryFiles`, `streamable`, `doc`, `id`, `format`, `loadContents`, `loadListing`, `default`, `type`, `inputBinding`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'WorkflowInputParameter'", None, _errors__)
@@ -9755,15 +9820,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `id`, `label`, `doc`, `inputs`, `outputs`, `requirements`, `hints`, `cwlVersion`, `class`, `expression`" % (k),
+                            "invalid field `{}`, expected one of: `id`, `label`, `doc`, `inputs`, `outputs`, `requirements`, `hints`, `cwlVersion`, `class`, `expression`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'ExpressionTool'", None, _errors__)
@@ -9941,15 +10006,15 @@
                     )
                 )
         else:
             label = None
         if 'secondaryFiles' in _doc:
             try:
                 secondaryFiles = load_field(_doc.get(
-                    'secondaryFiles'), union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
+                    'secondaryFiles'), secondaryfilesdsl_union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
                         "the `secondaryFiles` field is not valid because:",
                         SourceLine(_doc, 'secondaryFiles', str),
                         [e]
                     )
@@ -10047,15 +10112,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `label`, `secondaryFiles`, `streamable`, `doc`, `id`, `format`, `outputSource`, `linkMerge`, `type`" % (k),
+                            "invalid field `{}`, expected one of: `label`, `secondaryFiles`, `streamable`, `doc`, `id`, `format`, `outputSource`, `linkMerge`, `type`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'WorkflowOutputParameter'", None, _errors__)
@@ -10370,15 +10435,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `id`, `source`, `linkMerge`, `loadContents`, `loadListing`, `label`, `default`, `valueFrom`" % (k),
+                            "invalid field `{}`, expected one of: `id`, `source`, `linkMerge`, `loadContents`, `loadListing`, `label`, `default`, `valueFrom`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'WorkflowStepInput'", None, _errors__)
@@ -10532,15 +10597,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `id`" % (k),
+                            "invalid field `{}`, expected one of: `id`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'WorkflowStepOutput'", None, _errors__)
@@ -10773,15 +10838,15 @@
                         [e]
                     )
                 )
         else:
             hints = None
         try:
             run = load_field(_doc.get(
-                'run'), uri_union_of_strtype_or_CommandLineToolLoader_or_ExpressionToolLoader_or_WorkflowLoader_False_False_None, baseuri, loadingOptions)
+                'run'), union_of_strtype_or_CommandLineToolLoader_or_ExpressionToolLoader_or_WorkflowLoader, baseuri, loadingOptions)
         except ValidationException as e:
             _errors__.append(
                 ValidationException(
                     "the `run` field is not valid because:",
                     SourceLine(_doc, 'run', str),
                     [e]
                 )
@@ -10824,15 +10889,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `id`, `label`, `doc`, `in`, `out`, `requirements`, `hints`, `run`, `scatter`, `scatterMethod`" % (k),
+                            "invalid field `{}`, expected one of: `id`, `label`, `doc`, `in`, `out`, `requirements`, `hints`, `run`, `scatter`, `scatterMethod`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'WorkflowStep'", None, _errors__)
@@ -10896,22 +10961,19 @@
             r['hints'] = save(
                 self.hints,
                 top=False,
                 base_url=self.id,
                 relative_uris=relative_uris)
 
         if self.run is not None:
-            u = save_relative_uri(
+            r['run'] = save(
                 self.run,
-                self.id,
-                False,
-                None,
-                relative_uris)
-            if u:
-                r['run'] = u
+                top=False,
+                base_url=self.id,
+                relative_uris=relative_uris)
 
         if self.scatter is not None:
             u = save_relative_uri(
                 self.scatter,
                 self.id,
                 False,
                 0,
@@ -11170,15 +11232,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `id`, `label`, `doc`, `inputs`, `outputs`, `requirements`, `hints`, `cwlVersion`, `class`, `steps`" % (k),
+                            "invalid field `{}`, expected one of: `id`, `label`, `doc`, `inputs`, `outputs`, `requirements`, `hints`, `cwlVersion`, `class`, `steps`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'Workflow'", None, _errors__)
@@ -11317,15 +11379,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`" % (k),
+                            "invalid field `{}`, expected one of: `class`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'SubworkflowFeatureRequirement'", None, _errors__)
@@ -11395,15 +11457,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`" % (k),
+                            "invalid field `{}`, expected one of: `class`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'ScatterFeatureRequirement'", None, _errors__)
@@ -11473,15 +11535,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`" % (k),
+                            "invalid field `{}`, expected one of: `class`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'MultipleInputFeatureRequirement'", None, _errors__)
@@ -11551,15 +11613,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`" % (k),
+                            "invalid field `{}`, expected one of: `class`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'StepInputExpressionRequirement'", None, _errors__)
@@ -11848,15 +11910,15 @@
 IdentifiedLoader = _RecordLoader(Identified)
 LoadListingEnumLoader = _EnumLoader(("no_listing", "shallow_listing", "deep_listing",))
 LoadContentsLoader = _RecordLoader(LoadContents)
 FieldBaseLoader = _RecordLoader(FieldBase)
 InputFormatLoader = _RecordLoader(InputFormat)
 OutputFormatLoader = _RecordLoader(OutputFormat)
 ParameterLoader = _RecordLoader(Parameter)
-ExpressionLoader = _EnumLoader(("ExpressionPlaceholder",))
+ExpressionLoader = _ExpressionLoader(str)
 InputBindingLoader = _RecordLoader(InputBinding)
 IOSchemaLoader = _RecordLoader(IOSchema)
 InputSchemaLoader = _RecordLoader(InputSchema)
 OutputSchemaLoader = _RecordLoader(OutputSchema)
 InputRecordFieldLoader = _RecordLoader(InputRecordField)
 InputRecordSchemaLoader = _RecordLoader(InputRecordSchema)
 InputEnumSchemaLoader = _RecordLoader(InputEnumSchema)
@@ -11941,21 +12003,23 @@
 uri_File_classLoader_False_True_None = _URILoader(File_classLoader, False, True, None)
 union_of_None_type_or_strtype = _UnionLoader((None_type, strtype,))
 uri_union_of_None_type_or_strtype_False_False_None = _URILoader(union_of_None_type_or_strtype, False, False, None)
 union_of_None_type_or_inttype = _UnionLoader((None_type, inttype,))
 union_of_FileLoader_or_DirectoryLoader = _UnionLoader((FileLoader, DirectoryLoader,))
 array_of_union_of_FileLoader_or_DirectoryLoader = _ArrayLoader(union_of_FileLoader_or_DirectoryLoader)
 union_of_None_type_or_array_of_union_of_FileLoader_or_DirectoryLoader = _UnionLoader((None_type, array_of_union_of_FileLoader_or_DirectoryLoader,))
+secondaryfilesdsl_union_of_None_type_or_array_of_union_of_FileLoader_or_DirectoryLoader = _SecondaryDSLLoader(union_of_None_type_or_array_of_union_of_FileLoader_or_DirectoryLoader)
 uri_union_of_None_type_or_strtype_True_False_None = _URILoader(union_of_None_type_or_strtype, True, False, None)
 Directory_classLoader = _EnumLoader(("Directory",))
 uri_Directory_classLoader_False_True_None = _URILoader(Directory_classLoader, False, True, None)
 union_of_None_type_or_booltype = _UnionLoader((None_type, booltype,))
 union_of_None_type_or_LoadListingEnumLoader = _UnionLoader((None_type, LoadListingEnumLoader,))
 array_of_SecondaryFileSchemaLoader = _ArrayLoader(SecondaryFileSchemaLoader)
 union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader = _UnionLoader((None_type, SecondaryFileSchemaLoader, array_of_SecondaryFileSchemaLoader,))
+secondaryfilesdsl_union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader = _SecondaryDSLLoader(union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader)
 union_of_None_type_or_strtype_or_array_of_strtype_or_ExpressionLoader = _UnionLoader((None_type, strtype, array_of_strtype, ExpressionLoader,))
 uri_union_of_None_type_or_strtype_or_array_of_strtype_or_ExpressionLoader_True_False_None = _URILoader(union_of_None_type_or_strtype_or_array_of_strtype_or_ExpressionLoader, True, False, None)
 union_of_None_type_or_strtype_or_ExpressionLoader = _UnionLoader((None_type, strtype, ExpressionLoader,))
 uri_union_of_None_type_or_strtype_or_ExpressionLoader_True_False_None = _URILoader(union_of_None_type_or_strtype_or_ExpressionLoader, True, False, None)
 union_of_CWLTypeLoader_or_InputRecordSchemaLoader_or_InputEnumSchemaLoader_or_InputArraySchemaLoader_or_strtype = _UnionLoader((CWLTypeLoader, InputRecordSchemaLoader, InputEnumSchemaLoader, InputArraySchemaLoader, strtype,))
 array_of_union_of_CWLTypeLoader_or_InputRecordSchemaLoader_or_InputEnumSchemaLoader_or_InputArraySchemaLoader_or_strtype = _ArrayLoader(union_of_CWLTypeLoader_or_InputRecordSchemaLoader_or_InputEnumSchemaLoader_or_InputArraySchemaLoader_or_strtype)
 union_of_CWLTypeLoader_or_InputRecordSchemaLoader_or_InputEnumSchemaLoader_or_InputArraySchemaLoader_or_strtype_or_array_of_union_of_CWLTypeLoader_or_InputRecordSchemaLoader_or_InputEnumSchemaLoader_or_InputArraySchemaLoader_or_strtype = _UnionLoader((CWLTypeLoader, InputRecordSchemaLoader, InputEnumSchemaLoader, InputArraySchemaLoader, strtype, array_of_union_of_CWLTypeLoader_or_InputRecordSchemaLoader_or_InputEnumSchemaLoader_or_InputArraySchemaLoader_or_strtype,))
@@ -12049,15 +12113,14 @@
 array_of_WorkflowStepInputLoader = _ArrayLoader(WorkflowStepInputLoader)
 idmap_in__array_of_WorkflowStepInputLoader = _IdMapLoader(array_of_WorkflowStepInputLoader, 'id', 'source')
 union_of_strtype_or_WorkflowStepOutputLoader = _UnionLoader((strtype, WorkflowStepOutputLoader,))
 array_of_union_of_strtype_or_WorkflowStepOutputLoader = _ArrayLoader(union_of_strtype_or_WorkflowStepOutputLoader)
 union_of_array_of_union_of_strtype_or_WorkflowStepOutputLoader = _UnionLoader((array_of_union_of_strtype_or_WorkflowStepOutputLoader,))
 uri_union_of_array_of_union_of_strtype_or_WorkflowStepOutputLoader_True_False_None = _URILoader(union_of_array_of_union_of_strtype_or_WorkflowStepOutputLoader, True, False, None)
 union_of_strtype_or_CommandLineToolLoader_or_ExpressionToolLoader_or_WorkflowLoader = _UnionLoader((strtype, CommandLineToolLoader, ExpressionToolLoader, WorkflowLoader,))
-uri_union_of_strtype_or_CommandLineToolLoader_or_ExpressionToolLoader_or_WorkflowLoader_False_False_None = _URILoader(union_of_strtype_or_CommandLineToolLoader_or_ExpressionToolLoader_or_WorkflowLoader, False, False, None)
 union_of_None_type_or_ScatterMethodLoader = _UnionLoader((None_type, ScatterMethodLoader,))
 uri_union_of_None_type_or_ScatterMethodLoader_False_True_None = _URILoader(union_of_None_type_or_ScatterMethodLoader, False, True, None)
 array_of_WorkflowOutputParameterLoader = _ArrayLoader(WorkflowOutputParameterLoader)
 idmap_outputs_array_of_WorkflowOutputParameterLoader = _IdMapLoader(array_of_WorkflowOutputParameterLoader, 'id', 'type')
 array_of_WorkflowStepLoader = _ArrayLoader(WorkflowStepLoader)
 union_of_array_of_WorkflowStepLoader = _UnionLoader((array_of_WorkflowStepLoader,))
 idmap_steps_union_of_array_of_WorkflowStepLoader = _IdMapLoader(union_of_array_of_WorkflowStepLoader, 'id', 'None')
@@ -12081,7 +12144,21 @@
     add_lc_filename(result, uri)
 
     if loadingOptions is None:
         loadingOptions = LoadingOptions(fileuri=uri)
     loadingOptions.idx[uri] = result
 
     return _document_load(union_of_CommandLineToolLoader_or_ExpressionToolLoader_or_WorkflowLoader_or_array_of_union_of_CommandLineToolLoader_or_ExpressionToolLoader_or_WorkflowLoader, result, uri, loadingOptions)
+
+
+def load_document_by_yaml(yaml, uri, loadingOptions=None):
+    # type: (Any, str, Optional[LoadingOptions]) -> Any
+    '''Shortcut to load via a YAML object.
+    yaml: must be from ruamel.yaml.main.round_trip_load with preserve_quotes=True
+    '''
+    add_lc_filename(yaml, uri)
+
+    if loadingOptions is None:
+        loadingOptions = LoadingOptions(fileuri=uri)
+    loadingOptions.idx[uri] = yaml
+
+    return _document_load(union_of_CommandLineToolLoader_or_ExpressionToolLoader_or_WorkflowLoader_or_array_of_union_of_CommandLineToolLoader_or_ExpressionToolLoader_or_WorkflowLoader, yaml, uri, loadingOptions)
```

### Comparing `cwl-utils-0.8/cwl_utils/parser_v1_2.py` & `cwl-utils-0.9/cwl_utils/parser_v1_2.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,34 +21,35 @@
     Union,
 )
 from urllib.parse import quote, urlsplit, urlunsplit
 from urllib.request import pathname2url
 
 from ruamel import yaml
 from ruamel.yaml.comments import CommentedMap
+
 from schema_salad.exceptions import SchemaSaladException, ValidationException
 from schema_salad.fetcher import DefaultFetcher, Fetcher
 from schema_salad.sourceline import SourceLine, add_lc_filename
 
 _vocab = {}  # type: Dict[str, str]
 _rvocab = {}  # type: Dict[str, str]
 
 
-class Savable(object):
+class Savable:
     @classmethod
     def fromDoc(cls, _doc, baseuri, loadingOptions, docRoot=None):
         # type: (Any, str, LoadingOptions, Optional[str]) -> Savable
         pass
 
     def save(self, top=False, base_url="", relative_uris=True):
         # type: (bool, str, bool) -> Dict[str, str]
         pass
 
 
-class LoadingOptions(object):
+class LoadingOptions:
     def __init__(
         self,
         fetcher=None,  # type: Optional[Fetcher]
         namespaces=None,  # type: Optional[Dict[str, str]]
         schemas=None,  # type: Optional[Dict[str, str]]
         fileuri=None,  # type: Optional[str]
         copyfrom=None,  # type: Optional[LoadingOptions]
@@ -68,16 +69,16 @@
             if namespaces is None:
                 self.namespaces = copyfrom.namespaces
             if schemas is None:
                 self.schemas = copyfrom.schemas
 
         if fetcher is None:
             import requests
-            from cachecontrol.wrapper import CacheControl
             from cachecontrol.caches import FileCache
+            from cachecontrol.wrapper import CacheControl
 
             if "HOME" in os.environ:
                 session = CacheControl(
                     requests.Session(),
                     cache=FileCache(
                         os.path.join(os.environ["HOME"], ".cache", "salad")
                     ),
@@ -214,20 +215,20 @@
 
     if vocab_term:
         split = urlsplit(url)
         if bool(split.scheme):
             if url in loadingOptions.rvocab:
                 return loadingOptions.rvocab[url]
         else:
-            raise ValidationException("Term '{}' not in vocabulary".format(url))
+            raise ValidationException(f"Term '{url}' not in vocabulary")
 
     return url
 
 
-class _Loader(object):
+class _Loader:
     def load(self, doc, baseuri, loadingOptions, docRoot=None):
         # type: (Any, str, LoadingOptions, Optional[str]) -> Any
         pass
 
 
 class _AnyLoader(_Loader):
     def load(self, doc, baseuri, loadingOptions, docRoot=None):
@@ -279,28 +280,78 @@
             except ValidationException as e:
                 errors.append(e.with_sourceline(SourceLine(doc, i, str)))
         if errors:
             raise ValidationException("", None, errors)
         return r
 
     def __repr__(self):  # type: () -> str
-        return "array<{}>".format(self.items)
+        return f"array<{self.items}>"
 
 
 class _EnumLoader(_Loader):
     def __init__(self, symbols):
         # type: (Sequence[str]) -> None
         self.symbols = symbols
 
     def load(self, doc, baseuri, loadingOptions, docRoot=None):
         # type: (Any, str, LoadingOptions, Optional[str]) -> Any
         if doc in self.symbols:
             return doc
         else:
-            raise ValidationException("Expected one of {}".format(self.symbols))
+            raise ValidationException(f"Expected one of {self.symbols}")
+
+
+class _SecondaryDSLLoader(_Loader):
+    def __init__(self, inner):
+        # type: (_Loader) -> None
+        self.inner = inner
+
+    def load(self, doc, baseuri, loadingOptions, docRoot=None):
+        # type: (Any, str, LoadingOptions, Optional[str]) -> Any
+        r: List[Dict[str, Any]] = []
+        if isinstance(doc, MutableSequence):
+            for d in doc:
+                if isinstance(d, str):
+                    if d.endswith("?"):
+                        r.append({"pattern": d[:-1], "required": False})
+                    else:
+                        r.append({"pattern": d})
+                elif isinstance(d, dict):
+                    new_dict: Dict[str, Any] = {}
+                    if "pattern" in d:
+                        new_dict["pattern"] = d.pop("pattern")
+                    else:
+                        raise ValidationException(
+                            "Missing pattern in secondaryFiles specification entry: {}".format(
+                                d
+                            )
+                        )
+                    new_dict["required"] = (
+                        d.pop("required") if "required" in d else None
+                    )
+
+                    if len(d):
+                        raise ValidationException(
+                            "Unallowed values in secondaryFiles specification entry: {}".format(
+                                d
+                            )
+                        )
+
+                else:
+                    raise ValidationException(
+                        "Expected a string or sequence of (strings or mappings)."
+                    )
+        elif isinstance(doc, str):
+            if doc.endswith("?"):
+                r.append({"pattern": doc[:-1], "required": False})
+            else:
+                r.append({"pattern": doc})
+        else:
+            raise ValidationException("Expected str or sequence of str")
+        return self.inner.load(r, baseuri, loadingOptions, docRoot)
 
 
 class _RecordLoader(_Loader):
     def __init__(self, classtype):
         # type: (Type[Savable]) -> None
         self.classtype = classtype
 
@@ -310,30 +361,39 @@
             raise ValidationException("Expected a dict")
         return self.classtype.fromDoc(doc, baseuri, loadingOptions, docRoot=docRoot)
 
     def __repr__(self):  # type: () -> str
         return str(self.classtype)
 
 
+class _ExpressionLoader(_Loader):
+    def __init__(self, items: Type[str]) -> None:
+        self.items = items
+
+    def load(self, doc, baseuri, loadingOptions, docRoot=None):
+        # type: (Any, str, LoadingOptions, Optional[str]) -> Any
+        if not isinstance(doc, str):
+            raise ValidationException("Expected a str")
+        return doc
+
+
 class _UnionLoader(_Loader):
     def __init__(self, alternates):
         # type: (Sequence[_Loader]) -> None
         self.alternates = alternates
 
     def load(self, doc, baseuri, loadingOptions, docRoot=None):
         # type: (Any, str, LoadingOptions, Optional[str]) -> Any
         errors = []
         for t in self.alternates:
             try:
                 return t.load(doc, baseuri, loadingOptions, docRoot=docRoot)
             except ValidationException as e:
                 errors.append(
-                    ValidationException(
-                        "tried {} but".format(t.__class__.__name__), None, [e]
-                    )
+                    ValidationException(f"tried {t.__class__.__name__} but", None, [e])
                 )
         raise ValidationException("", None, errors, "-")
 
     def __repr__(self):  # type: () -> str
         return " | ".join(str(a) for a in self.alternates)
 
 
@@ -344,26 +404,31 @@
         self.scoped_id = scoped_id
         self.vocab_term = vocab_term
         self.scoped_ref = scoped_ref
 
     def load(self, doc, baseuri, loadingOptions, docRoot=None):
         # type: (Any, str, LoadingOptions, Optional[str]) -> Any
         if isinstance(doc, MutableSequence):
-            doc = [
-                expand_url(
-                    i,
-                    baseuri,
-                    loadingOptions,
-                    self.scoped_id,
-                    self.vocab_term,
-                    self.scoped_ref,
-                )
-                for i in doc
-            ]
-        if isinstance(doc, str):
+            newdoc = []
+            for i in doc:
+                if isinstance(i, str):
+                    newdoc.append(
+                        expand_url(
+                            i,
+                            baseuri,
+                            loadingOptions,
+                            self.scoped_id,
+                            self.vocab_term,
+                            self.scoped_ref,
+                        )
+                    )
+                else:
+                    newdoc.append(i)
+            doc = newdoc
+        elif isinstance(doc, str):
             doc = expand_url(
                 doc,
                 baseuri,
                 loadingOptions,
                 self.scoped_id,
                 self.vocab_term,
                 self.scoped_ref,
@@ -525,17 +590,17 @@
         pathsp = path.split("#", 2)
         frag = "#" + quote(str(pathsp[1])) if len(pathsp) == 2 else ""
         urlpath = pathname2url(str(pathsp[0]))
     else:
         urlpath = pathname2url(path)
         frag = ""
     if urlpath.startswith("//"):
-        return "file:{}{}".format(urlpath, frag)
+        return f"file:{urlpath}{frag}"
     else:
-        return "file://{}{}".format(urlpath, frag)
+        return f"file://{urlpath}{frag}"
 
 
 def prefix_url(url, namespaces):  # type: (str, Dict[str, str]) -> str
     for k, v in namespaces.items():
         if url.startswith(v):
             return k + ":" + url[len(v) :]
     return url
@@ -672,15 +737,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `doc`, `name`, `type`" % (k),
+                            "invalid field `{}`, expected one of: `doc`, `name`, `type`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'RecordField'", None, _errors__)
@@ -791,15 +856,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `fields`, `type`" % (k),
+                            "invalid field `{}`, expected one of: `fields`, `type`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'RecordSchema'", None, _errors__)
@@ -901,15 +966,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `symbols`, `type`" % (k),
+                            "invalid field `{}`, expected one of: `symbols`, `type`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'EnumSchema'", None, _errors__)
@@ -1010,15 +1075,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `items`, `type`" % (k),
+                            "invalid field `{}`, expected one of: `items`, `type`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'ArraySchema'", None, _errors__)
@@ -1290,15 +1355,15 @@
                     )
                 )
         else:
             size = None
         if 'secondaryFiles' in _doc:
             try:
                 secondaryFiles = load_field(_doc.get(
-                    'secondaryFiles'), union_of_None_type_or_array_of_union_of_FileLoader_or_DirectoryLoader, baseuri, loadingOptions)
+                    'secondaryFiles'), secondaryfilesdsl_union_of_None_type_or_array_of_union_of_FileLoader_or_DirectoryLoader, baseuri, loadingOptions)
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
                         "the `secondaryFiles` field is not valid because:",
                         SourceLine(_doc, 'secondaryFiles', str),
                         [e]
                     )
@@ -1343,15 +1408,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `location`, `path`, `basename`, `dirname`, `nameroot`, `nameext`, `checksum`, `size`, `secondaryFiles`, `format`, `contents`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `location`, `path`, `basename`, `dirname`, `nameroot`, `nameext`, `checksum`, `size`, `secondaryFiles`, `format`, `contents`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'File'", None, _errors__)
@@ -1612,15 +1677,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `location`, `path`, `basename`, `listing`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `location`, `path`, `basename`, `listing`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'Directory'", None, _errors__)
@@ -1762,15 +1827,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `loadContents`" % (k),
+                            "invalid field `{}`, expected one of: `loadContents`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'InputBinding'", None, _errors__)
@@ -1914,15 +1979,15 @@
                     )
                 )
         else:
             label = None
         if 'secondaryFiles' in _doc:
             try:
                 secondaryFiles = load_field(_doc.get(
-                    'secondaryFiles'), union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
+                    'secondaryFiles'), secondaryfilesdsl_union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
                         "the `secondaryFiles` field is not valid because:",
                         SourceLine(_doc, 'secondaryFiles', str),
                         [e]
                     )
@@ -1995,15 +2060,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `doc`, `name`, `type`, `label`, `secondaryFiles`, `streamable`, `format`, `loadContents`, `loadListing`" % (k),
+                            "invalid field `{}`, expected one of: `doc`, `name`, `type`, `label`, `secondaryFiles`, `streamable`, `format`, `loadContents`, `loadListing`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'InputRecordField'", None, _errors__)
@@ -2214,15 +2279,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `fields`, `type`, `label`, `doc`, `name`" % (k),
+                            "invalid field `{}`, expected one of: `fields`, `type`, `label`, `doc`, `name`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'InputRecordSchema'", None, _errors__)
@@ -2399,15 +2464,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `symbols`, `type`, `label`, `doc`, `name`" % (k),
+                            "invalid field `{}`, expected one of: `symbols`, `type`, `label`, `doc`, `name`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'InputEnumSchema'", None, _errors__)
@@ -2587,15 +2652,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `items`, `type`, `label`, `doc`, `name`" % (k),
+                            "invalid field `{}`, expected one of: `items`, `type`, `label`, `doc`, `name`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'InputArraySchema'", None, _errors__)
@@ -2757,15 +2822,15 @@
                     )
                 )
         else:
             label = None
         if 'secondaryFiles' in _doc:
             try:
                 secondaryFiles = load_field(_doc.get(
-                    'secondaryFiles'), union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
+                    'secondaryFiles'), secondaryfilesdsl_union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
                         "the `secondaryFiles` field is not valid because:",
                         SourceLine(_doc, 'secondaryFiles', str),
                         [e]
                     )
@@ -2810,15 +2875,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `doc`, `name`, `type`, `label`, `secondaryFiles`, `streamable`, `format`" % (k),
+                            "invalid field `{}`, expected one of: `doc`, `name`, `type`, `label`, `secondaryFiles`, `streamable`, `format`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'OutputRecordField'", None, _errors__)
@@ -3015,15 +3080,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `fields`, `type`, `label`, `doc`, `name`" % (k),
+                            "invalid field `{}`, expected one of: `fields`, `type`, `label`, `doc`, `name`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'OutputRecordSchema'", None, _errors__)
@@ -3200,15 +3265,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `symbols`, `type`, `label`, `doc`, `name`" % (k),
+                            "invalid field `{}`, expected one of: `symbols`, `type`, `label`, `doc`, `name`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'OutputEnumSchema'", None, _errors__)
@@ -3388,15 +3453,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `items`, `type`, `label`, `doc`, `name`" % (k),
+                            "invalid field `{}`, expected one of: `items`, `type`, `label`, `doc`, `name`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'OutputArraySchema'", None, _errors__)
@@ -3554,15 +3619,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `expressionLib`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `expressionLib`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'InlineJavascriptRequirement'", None, _errors__)
@@ -3666,15 +3731,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `types`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `types`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'SchemaDefRequirement'", None, _errors__)
@@ -3786,15 +3851,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `pattern`, `required`" % (k),
+                            "invalid field `{}`, expected one of: `pattern`, `required`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'SecondaryFileSchema'", None, _errors__)
@@ -3892,15 +3957,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `loadListing`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `loadListing`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'LoadListingRequirement'", None, _errors__)
@@ -3999,15 +4064,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `envName`, `envValue`" % (k),
+                            "invalid field `{}`, expected one of: `envName`, `envValue`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'EnvironmentDef'", None, _errors__)
@@ -4229,15 +4294,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `loadContents`, `position`, `prefix`, `separate`, `itemSeparator`, `valueFrom`, `shellQuote`" % (k),
+                            "invalid field `{}`, expected one of: `loadContents`, `position`, `prefix`, `separate`, `itemSeparator`, `valueFrom`, `shellQuote`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandLineBinding'", None, _errors__)
@@ -4421,15 +4486,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `loadContents`, `loadListing`, `glob`, `outputEval`" % (k),
+                            "invalid field `{}`, expected one of: `loadContents`, `loadListing`, `glob`, `outputEval`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandOutputBinding'", None, _errors__)
@@ -4531,15 +4596,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `inputBinding`" % (k),
+                            "invalid field `{}`, expected one of: `inputBinding`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandLineBindable'", None, _errors__)
@@ -4673,15 +4738,15 @@
                     )
                 )
         else:
             label = None
         if 'secondaryFiles' in _doc:
             try:
                 secondaryFiles = load_field(_doc.get(
-                    'secondaryFiles'), union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
+                    'secondaryFiles'), secondaryfilesdsl_union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
                         "the `secondaryFiles` field is not valid because:",
                         SourceLine(_doc, 'secondaryFiles', str),
                         [e]
                     )
@@ -4768,15 +4833,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `doc`, `name`, `type`, `label`, `secondaryFiles`, `streamable`, `format`, `loadContents`, `loadListing`, `inputBinding`" % (k),
+                            "invalid field `{}`, expected one of: `doc`, `name`, `type`, `label`, `secondaryFiles`, `streamable`, `format`, `loadContents`, `loadListing`, `inputBinding`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandInputRecordField'", None, _errors__)
@@ -5010,15 +5075,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `fields`, `type`, `label`, `doc`, `name`, `inputBinding`" % (k),
+                            "invalid field `{}`, expected one of: `fields`, `type`, `label`, `doc`, `name`, `inputBinding`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandInputRecordSchema'", None, _errors__)
@@ -5218,15 +5283,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `symbols`, `type`, `label`, `doc`, `name`, `inputBinding`" % (k),
+                            "invalid field `{}`, expected one of: `symbols`, `type`, `label`, `doc`, `name`, `inputBinding`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandInputEnumSchema'", None, _errors__)
@@ -5429,15 +5494,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `items`, `type`, `label`, `doc`, `name`, `inputBinding`" % (k),
+                            "invalid field `{}`, expected one of: `items`, `type`, `label`, `doc`, `name`, `inputBinding`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandInputArraySchema'", None, _errors__)
@@ -5608,15 +5673,15 @@
                     )
                 )
         else:
             label = None
         if 'secondaryFiles' in _doc:
             try:
                 secondaryFiles = load_field(_doc.get(
-                    'secondaryFiles'), union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
+                    'secondaryFiles'), secondaryfilesdsl_union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
                         "the `secondaryFiles` field is not valid because:",
                         SourceLine(_doc, 'secondaryFiles', str),
                         [e]
                     )
@@ -5675,15 +5740,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `doc`, `name`, `type`, `label`, `secondaryFiles`, `streamable`, `format`, `outputBinding`" % (k),
+                            "invalid field `{}`, expected one of: `doc`, `name`, `type`, `label`, `secondaryFiles`, `streamable`, `format`, `outputBinding`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandOutputRecordField'", None, _errors__)
@@ -5887,15 +5952,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `fields`, `type`, `label`, `doc`, `name`" % (k),
+                            "invalid field `{}`, expected one of: `fields`, `type`, `label`, `doc`, `name`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandOutputRecordSchema'", None, _errors__)
@@ -6072,15 +6137,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `symbols`, `type`, `label`, `doc`, `name`" % (k),
+                            "invalid field `{}`, expected one of: `symbols`, `type`, `label`, `doc`, `name`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandOutputEnumSchema'", None, _errors__)
@@ -6260,15 +6325,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `items`, `type`, `label`, `doc`, `name`" % (k),
+                            "invalid field `{}`, expected one of: `items`, `type`, `label`, `doc`, `name`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandOutputArraySchema'", None, _errors__)
@@ -6416,15 +6481,15 @@
                     )
                 )
         else:
             label = None
         if 'secondaryFiles' in _doc:
             try:
                 secondaryFiles = load_field(_doc.get(
-                    'secondaryFiles'), union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
+                    'secondaryFiles'), secondaryfilesdsl_union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
                         "the `secondaryFiles` field is not valid because:",
                         SourceLine(_doc, 'secondaryFiles', str),
                         [e]
                     )
@@ -6550,15 +6615,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `label`, `secondaryFiles`, `streamable`, `doc`, `id`, `format`, `loadContents`, `loadListing`, `default`, `type`, `inputBinding`" % (k),
+                            "invalid field `{}`, expected one of: `label`, `secondaryFiles`, `streamable`, `doc`, `id`, `format`, `loadContents`, `loadListing`, `default`, `type`, `inputBinding`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandInputParameter'", None, _errors__)
@@ -6742,15 +6807,15 @@
                     )
                 )
         else:
             label = None
         if 'secondaryFiles' in _doc:
             try:
                 secondaryFiles = load_field(_doc.get(
-                    'secondaryFiles'), union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
+                    'secondaryFiles'), secondaryfilesdsl_union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
                         "the `secondaryFiles` field is not valid because:",
                         SourceLine(_doc, 'secondaryFiles', str),
                         [e]
                     )
@@ -6834,15 +6899,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `label`, `secondaryFiles`, `streamable`, `doc`, `id`, `format`, `type`, `outputBinding`" % (k),
+                            "invalid field `{}`, expected one of: `label`, `secondaryFiles`, `streamable`, `doc`, `id`, `format`, `type`, `outputBinding`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandOutputParameter'", None, _errors__)
@@ -7244,15 +7309,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `id`, `label`, `doc`, `inputs`, `outputs`, `requirements`, `hints`, `cwlVersion`, `intent`, `class`, `baseCommand`, `arguments`, `stdin`, `stderr`, `stdout`, `successCodes`, `temporaryFailCodes`, `permanentFailCodes`" % (k),
+                            "invalid field `{}`, expected one of: `id`, `label`, `doc`, `inputs`, `outputs`, `requirements`, `hints`, `cwlVersion`, `intent`, `class`, `baseCommand`, `arguments`, `stdin`, `stderr`, `stdout`, `successCodes`, `temporaryFailCodes`, `permanentFailCodes`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'CommandLineTool'", None, _errors__)
@@ -7595,15 +7660,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `dockerPull`, `dockerLoad`, `dockerFile`, `dockerImport`, `dockerImageId`, `dockerOutputDirectory`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `dockerPull`, `dockerLoad`, `dockerFile`, `dockerImport`, `dockerImageId`, `dockerOutputDirectory`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'DockerRequirement'", None, _errors__)
@@ -7728,15 +7793,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `packages`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `packages`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'SoftwareRequirement'", None, _errors__)
@@ -7848,15 +7913,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `package`, `version`, `specs`" % (k),
+                            "invalid field `{}`, expected one of: `package`, `version`, `specs`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'SoftwarePackage'", None, _errors__)
@@ -7994,15 +8059,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `entryname`, `entry`, `writable`" % (k),
+                            "invalid field `{}`, expected one of: `entryname`, `entry`, `writable`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'Dirent'", None, _errors__)
@@ -8103,15 +8168,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `listing`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `listing`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'InitialWorkDirRequirement'", None, _errors__)
@@ -8201,15 +8266,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `envDef`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `envDef`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'EnvVarRequirement'", None, _errors__)
@@ -8291,15 +8356,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`" % (k),
+                            "invalid field `{}`, expected one of: `class`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'ShellCommandRequirement'", None, _errors__)
@@ -8520,15 +8585,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `coresMin`, `coresMax`, `ramMin`, `ramMax`, `tmpdirMin`, `tmpdirMax`, `outdirMin`, `outdirMax`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `coresMin`, `coresMax`, `ramMin`, `ramMax`, `tmpdirMin`, `tmpdirMax`, `outdirMin`, `outdirMax`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'ResourceRequirement'", None, _errors__)
@@ -8674,15 +8739,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `enableReuse`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `enableReuse`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'WorkReuse'", None, _errors__)
@@ -8785,15 +8850,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `networkAccess`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `networkAccess`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'NetworkAccess'", None, _errors__)
@@ -8911,15 +8976,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `inplaceUpdate`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `inplaceUpdate`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'InplaceUpdateRequirement'", None, _errors__)
@@ -9014,15 +9079,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`, `timelimit`" % (k),
+                            "invalid field `{}`, expected one of: `class`, `timelimit`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'ToolTimeLimit'", None, _errors__)
@@ -9127,15 +9192,15 @@
                     )
                 )
         else:
             label = None
         if 'secondaryFiles' in _doc:
             try:
                 secondaryFiles = load_field(_doc.get(
-                    'secondaryFiles'), union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
+                    'secondaryFiles'), secondaryfilesdsl_union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
                         "the `secondaryFiles` field is not valid because:",
                         SourceLine(_doc, 'secondaryFiles', str),
                         [e]
                     )
@@ -9205,15 +9270,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `label`, `secondaryFiles`, `streamable`, `doc`, `id`, `format`, `type`" % (k),
+                            "invalid field `{}`, expected one of: `label`, `secondaryFiles`, `streamable`, `doc`, `id`, `format`, `type`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'ExpressionToolOutputParameter'", None, _errors__)
@@ -9372,15 +9437,15 @@
                     )
                 )
         else:
             label = None
         if 'secondaryFiles' in _doc:
             try:
                 secondaryFiles = load_field(_doc.get(
-                    'secondaryFiles'), union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
+                    'secondaryFiles'), secondaryfilesdsl_union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
                         "the `secondaryFiles` field is not valid because:",
                         SourceLine(_doc, 'secondaryFiles', str),
                         [e]
                     )
@@ -9506,15 +9571,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `label`, `secondaryFiles`, `streamable`, `doc`, `id`, `format`, `loadContents`, `loadListing`, `default`, `type`, `inputBinding`" % (k),
+                            "invalid field `{}`, expected one of: `label`, `secondaryFiles`, `streamable`, `doc`, `id`, `format`, `loadContents`, `loadListing`, `default`, `type`, `inputBinding`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'WorkflowInputParameter'", None, _errors__)
@@ -9828,15 +9893,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `id`, `label`, `doc`, `inputs`, `outputs`, `requirements`, `hints`, `cwlVersion`, `intent`, `class`, `expression`" % (k),
+                            "invalid field `{}`, expected one of: `id`, `label`, `doc`, `inputs`, `outputs`, `requirements`, `hints`, `cwlVersion`, `intent`, `class`, `expression`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'ExpressionTool'", None, _errors__)
@@ -10029,15 +10094,15 @@
                     )
                 )
         else:
             label = None
         if 'secondaryFiles' in _doc:
             try:
                 secondaryFiles = load_field(_doc.get(
-                    'secondaryFiles'), union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
+                    'secondaryFiles'), secondaryfilesdsl_union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
                         "the `secondaryFiles` field is not valid because:",
                         SourceLine(_doc, 'secondaryFiles', str),
                         [e]
                     )
@@ -10149,15 +10214,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `label`, `secondaryFiles`, `streamable`, `doc`, `id`, `format`, `outputSource`, `linkMerge`, `pickValue`, `type`" % (k),
+                            "invalid field `{}`, expected one of: `label`, `secondaryFiles`, `streamable`, `doc`, `id`, `format`, `outputSource`, `linkMerge`, `pickValue`, `type`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'WorkflowOutputParameter'", None, _errors__)
@@ -10560,15 +10625,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `id`, `source`, `linkMerge`, `pickValue`, `loadContents`, `loadListing`, `label`, `default`, `valueFrom`" % (k),
+                            "invalid field `{}`, expected one of: `id`, `source`, `linkMerge`, `pickValue`, `loadContents`, `loadListing`, `label`, `default`, `valueFrom`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'WorkflowStepInput'", None, _errors__)
@@ -10729,15 +10794,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `id`" % (k),
+                            "invalid field `{}`, expected one of: `id`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'WorkflowStepOutput'", None, _errors__)
@@ -10996,15 +11061,15 @@
                         [e]
                     )
                 )
         else:
             hints = None
         try:
             run = load_field(_doc.get(
-                'run'), uri_union_of_strtype_or_CommandLineToolLoader_or_ExpressionToolLoader_or_WorkflowLoader_or_OperationLoader_False_False_None, baseuri, loadingOptions)
+                'run'), union_of_strtype_or_CommandLineToolLoader_or_ExpressionToolLoader_or_WorkflowLoader_or_OperationLoader, baseuri, loadingOptions)
         except ValidationException as e:
             _errors__.append(
                 ValidationException(
                     "the `run` field is not valid because:",
                     SourceLine(_doc, 'run', str),
                     [e]
                 )
@@ -11061,15 +11126,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `id`, `label`, `doc`, `in`, `out`, `requirements`, `hints`, `run`, `when`, `scatter`, `scatterMethod`" % (k),
+                            "invalid field `{}`, expected one of: `id`, `label`, `doc`, `in`, `out`, `requirements`, `hints`, `run`, `when`, `scatter`, `scatterMethod`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'WorkflowStep'", None, _errors__)
@@ -11133,22 +11198,19 @@
             r['hints'] = save(
                 self.hints,
                 top=False,
                 base_url=self.id,
                 relative_uris=relative_uris)
 
         if self.run is not None:
-            u = save_relative_uri(
+            r['run'] = save(
                 self.run,
-                self.id,
-                False,
-                None,
-                relative_uris)
-            if u:
-                r['run'] = u
+                top=False,
+                base_url=self.id,
+                relative_uris=relative_uris)
 
         if self.when is not None:
             r['when'] = save(
                 self.when,
                 top=False,
                 base_url=self.id,
                 relative_uris=relative_uris)
@@ -11436,15 +11498,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `id`, `label`, `doc`, `inputs`, `outputs`, `requirements`, `hints`, `cwlVersion`, `intent`, `class`, `steps`" % (k),
+                            "invalid field `{}`, expected one of: `id`, `label`, `doc`, `inputs`, `outputs`, `requirements`, `hints`, `cwlVersion`, `intent`, `class`, `steps`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'Workflow'", None, _errors__)
@@ -11593,15 +11655,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`" % (k),
+                            "invalid field `{}`, expected one of: `class`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'SubworkflowFeatureRequirement'", None, _errors__)
@@ -11671,15 +11733,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`" % (k),
+                            "invalid field `{}`, expected one of: `class`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'ScatterFeatureRequirement'", None, _errors__)
@@ -11749,15 +11811,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`" % (k),
+                            "invalid field `{}`, expected one of: `class`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'MultipleInputFeatureRequirement'", None, _errors__)
@@ -11827,15 +11889,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `class`" % (k),
+                            "invalid field `{}`, expected one of: `class`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'StepInputExpressionRequirement'", None, _errors__)
@@ -11943,15 +12005,15 @@
                     )
                 )
         else:
             label = None
         if 'secondaryFiles' in _doc:
             try:
                 secondaryFiles = load_field(_doc.get(
-                    'secondaryFiles'), union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
+                    'secondaryFiles'), secondaryfilesdsl_union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
                         "the `secondaryFiles` field is not valid because:",
                         SourceLine(_doc, 'secondaryFiles', str),
                         [e]
                     )
@@ -12063,15 +12125,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `label`, `secondaryFiles`, `streamable`, `doc`, `id`, `format`, `loadContents`, `loadListing`, `default`, `type`" % (k),
+                            "invalid field `{}`, expected one of: `label`, `secondaryFiles`, `streamable`, `doc`, `id`, `format`, `loadContents`, `loadListing`, `default`, `type`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'OperationInputParameter'", None, _errors__)
@@ -12247,15 +12309,15 @@
                     )
                 )
         else:
             label = None
         if 'secondaryFiles' in _doc:
             try:
                 secondaryFiles = load_field(_doc.get(
-                    'secondaryFiles'), union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
+                    'secondaryFiles'), secondaryfilesdsl_union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader, baseuri, loadingOptions)
             except ValidationException as e:
                 _errors__.append(
                     ValidationException(
                         "the `secondaryFiles` field is not valid because:",
                         SourceLine(_doc, 'secondaryFiles', str),
                         [e]
                     )
@@ -12325,15 +12387,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `label`, `secondaryFiles`, `streamable`, `doc`, `id`, `format`, `type`" % (k),
+                            "invalid field `{}`, expected one of: `label`, `secondaryFiles`, `streamable`, `doc`, `id`, `format`, `type`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'OperationOutputParameter'", None, _errors__)
@@ -12606,15 +12668,15 @@
                                     loadingOptions,
                                     scoped_id=False,
                                     vocab_term=False)
                     extension_fields[ex] = _doc[k]
                 else:
                     _errors__.append(
                         ValidationException(
-                            "invalid field `%s`, expected one of: `id`, `label`, `doc`, `inputs`, `outputs`, `requirements`, `hints`, `cwlVersion`, `intent`, `class`" % (k),
+                            "invalid field `{}`, expected one of: `id`, `label`, `doc`, `inputs`, `outputs`, `requirements`, `hints`, `cwlVersion`, `intent`, `class`".format(k),
                             SourceLine(_doc, k, str)
                         )
                     )
                     break
 
         if _errors__:
             raise ValidationException("Trying 'Operation'", None, _errors__)
@@ -13001,15 +13063,15 @@
 IdentifiedLoader = _RecordLoader(Identified)
 LoadListingEnumLoader = _EnumLoader(("no_listing", "shallow_listing", "deep_listing",))
 LoadContentsLoader = _RecordLoader(LoadContents)
 FieldBaseLoader = _RecordLoader(FieldBase)
 InputFormatLoader = _RecordLoader(InputFormat)
 OutputFormatLoader = _RecordLoader(OutputFormat)
 ParameterLoader = _RecordLoader(Parameter)
-ExpressionLoader = _EnumLoader(("ExpressionPlaceholder",))
+ExpressionLoader = _ExpressionLoader(str)
 InputBindingLoader = _RecordLoader(InputBinding)
 IOSchemaLoader = _RecordLoader(IOSchema)
 InputSchemaLoader = _RecordLoader(InputSchema)
 OutputSchemaLoader = _RecordLoader(OutputSchema)
 InputRecordFieldLoader = _RecordLoader(InputRecordField)
 InputRecordSchemaLoader = _RecordLoader(InputRecordSchema)
 InputEnumSchemaLoader = _RecordLoader(InputEnumSchema)
@@ -13098,21 +13160,23 @@
 uri_File_classLoader_False_True_None = _URILoader(File_classLoader, False, True, None)
 union_of_None_type_or_strtype = _UnionLoader((None_type, strtype,))
 uri_union_of_None_type_or_strtype_False_False_None = _URILoader(union_of_None_type_or_strtype, False, False, None)
 union_of_None_type_or_inttype = _UnionLoader((None_type, inttype,))
 union_of_FileLoader_or_DirectoryLoader = _UnionLoader((FileLoader, DirectoryLoader,))
 array_of_union_of_FileLoader_or_DirectoryLoader = _ArrayLoader(union_of_FileLoader_or_DirectoryLoader)
 union_of_None_type_or_array_of_union_of_FileLoader_or_DirectoryLoader = _UnionLoader((None_type, array_of_union_of_FileLoader_or_DirectoryLoader,))
+secondaryfilesdsl_union_of_None_type_or_array_of_union_of_FileLoader_or_DirectoryLoader = _SecondaryDSLLoader(union_of_None_type_or_array_of_union_of_FileLoader_or_DirectoryLoader)
 uri_union_of_None_type_or_strtype_True_False_None = _URILoader(union_of_None_type_or_strtype, True, False, None)
 Directory_classLoader = _EnumLoader(("Directory",))
 uri_Directory_classLoader_False_True_None = _URILoader(Directory_classLoader, False, True, None)
 union_of_None_type_or_booltype = _UnionLoader((None_type, booltype,))
 union_of_None_type_or_LoadListingEnumLoader = _UnionLoader((None_type, LoadListingEnumLoader,))
 array_of_SecondaryFileSchemaLoader = _ArrayLoader(SecondaryFileSchemaLoader)
 union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader = _UnionLoader((None_type, SecondaryFileSchemaLoader, array_of_SecondaryFileSchemaLoader,))
+secondaryfilesdsl_union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader = _SecondaryDSLLoader(union_of_None_type_or_SecondaryFileSchemaLoader_or_array_of_SecondaryFileSchemaLoader)
 union_of_None_type_or_strtype_or_array_of_strtype_or_ExpressionLoader = _UnionLoader((None_type, strtype, array_of_strtype, ExpressionLoader,))
 uri_union_of_None_type_or_strtype_or_array_of_strtype_or_ExpressionLoader_True_False_None = _URILoader(union_of_None_type_or_strtype_or_array_of_strtype_or_ExpressionLoader, True, False, None)
 union_of_None_type_or_strtype_or_ExpressionLoader = _UnionLoader((None_type, strtype, ExpressionLoader,))
 uri_union_of_None_type_or_strtype_or_ExpressionLoader_True_False_None = _URILoader(union_of_None_type_or_strtype_or_ExpressionLoader, True, False, None)
 union_of_CWLTypeLoader_or_InputRecordSchemaLoader_or_InputEnumSchemaLoader_or_InputArraySchemaLoader_or_strtype = _UnionLoader((CWLTypeLoader, InputRecordSchemaLoader, InputEnumSchemaLoader, InputArraySchemaLoader, strtype,))
 array_of_union_of_CWLTypeLoader_or_InputRecordSchemaLoader_or_InputEnumSchemaLoader_or_InputArraySchemaLoader_or_strtype = _ArrayLoader(union_of_CWLTypeLoader_or_InputRecordSchemaLoader_or_InputEnumSchemaLoader_or_InputArraySchemaLoader_or_strtype)
 union_of_CWLTypeLoader_or_InputRecordSchemaLoader_or_InputEnumSchemaLoader_or_InputArraySchemaLoader_or_strtype_or_array_of_union_of_CWLTypeLoader_or_InputRecordSchemaLoader_or_InputEnumSchemaLoader_or_InputArraySchemaLoader_or_strtype = _UnionLoader((CWLTypeLoader, InputRecordSchemaLoader, InputEnumSchemaLoader, InputArraySchemaLoader, strtype, array_of_union_of_CWLTypeLoader_or_InputRecordSchemaLoader_or_InputEnumSchemaLoader_or_InputArraySchemaLoader_or_strtype,))
@@ -13209,15 +13273,14 @@
 array_of_WorkflowStepInputLoader = _ArrayLoader(WorkflowStepInputLoader)
 idmap_in__array_of_WorkflowStepInputLoader = _IdMapLoader(array_of_WorkflowStepInputLoader, 'id', 'source')
 union_of_strtype_or_WorkflowStepOutputLoader = _UnionLoader((strtype, WorkflowStepOutputLoader,))
 array_of_union_of_strtype_or_WorkflowStepOutputLoader = _ArrayLoader(union_of_strtype_or_WorkflowStepOutputLoader)
 union_of_array_of_union_of_strtype_or_WorkflowStepOutputLoader = _UnionLoader((array_of_union_of_strtype_or_WorkflowStepOutputLoader,))
 uri_union_of_array_of_union_of_strtype_or_WorkflowStepOutputLoader_True_False_None = _URILoader(union_of_array_of_union_of_strtype_or_WorkflowStepOutputLoader, True, False, None)
 union_of_strtype_or_CommandLineToolLoader_or_ExpressionToolLoader_or_WorkflowLoader_or_OperationLoader = _UnionLoader((strtype, CommandLineToolLoader, ExpressionToolLoader, WorkflowLoader, OperationLoader,))
-uri_union_of_strtype_or_CommandLineToolLoader_or_ExpressionToolLoader_or_WorkflowLoader_or_OperationLoader_False_False_None = _URILoader(union_of_strtype_or_CommandLineToolLoader_or_ExpressionToolLoader_or_WorkflowLoader_or_OperationLoader, False, False, None)
 union_of_None_type_or_ScatterMethodLoader = _UnionLoader((None_type, ScatterMethodLoader,))
 uri_union_of_None_type_or_ScatterMethodLoader_False_True_None = _URILoader(union_of_None_type_or_ScatterMethodLoader, False, True, None)
 array_of_WorkflowOutputParameterLoader = _ArrayLoader(WorkflowOutputParameterLoader)
 idmap_outputs_array_of_WorkflowOutputParameterLoader = _IdMapLoader(array_of_WorkflowOutputParameterLoader, 'id', 'type')
 array_of_WorkflowStepLoader = _ArrayLoader(WorkflowStepLoader)
 union_of_array_of_WorkflowStepLoader = _UnionLoader((array_of_WorkflowStepLoader,))
 idmap_steps_union_of_array_of_WorkflowStepLoader = _IdMapLoader(union_of_array_of_WorkflowStepLoader, 'id', 'None')
@@ -13245,7 +13308,21 @@
     add_lc_filename(result, uri)
 
     if loadingOptions is None:
         loadingOptions = LoadingOptions(fileuri=uri)
     loadingOptions.idx[uri] = result
 
     return _document_load(union_of_CommandLineToolLoader_or_ExpressionToolLoader_or_WorkflowLoader_or_OperationLoader_or_array_of_union_of_CommandLineToolLoader_or_ExpressionToolLoader_or_WorkflowLoader_or_OperationLoader, result, uri, loadingOptions)
+
+
+def load_document_by_yaml(yaml, uri, loadingOptions=None):
+    # type: (Any, str, Optional[LoadingOptions]) -> Any
+    '''Shortcut to load via a YAML object.
+    yaml: must be from ruamel.yaml.main.round_trip_load with preserve_quotes=True
+    '''
+    add_lc_filename(yaml, uri)
+
+    if loadingOptions is None:
+        loadingOptions = LoadingOptions(fileuri=uri)
+    loadingOptions.idx[uri] = yaml
+
+    return _document_load(union_of_CommandLineToolLoader_or_ExpressionToolLoader_or_WorkflowLoader_or_OperationLoader_or_array_of_union_of_CommandLineToolLoader_or_ExpressionToolLoader_or_WorkflowLoader_or_OperationLoader, yaml, uri, loadingOptions)
```

### Comparing `cwl-utils-0.8/cwl_utils.egg-info/SOURCES.txt` & `cwl-utils-0.9/cwl_utils.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 setup.cfg
 setup.py
 test-requirements.txt
 cwl_utils/__init__.py
 cwl_utils/__meta__.py
 cwl_utils/cite_extract.py
 cwl_utils/cwl_expression_refactor.py
+cwl_utils/cwl_v1_0_expression_refactor.py
+cwl_utils/cwl_v1_1_expression_refactor.py
+cwl_utils/cwl_v1_2_expression_refactor.py
 cwl_utils/docker_extract.py
 cwl_utils/first_tool.py
 cwl_utils/graph_split.py
 cwl_utils/image_puller.py
 cwl_utils/parser_v1_0.py
 cwl_utils/parser_v1_1.py
 cwl_utils/parser_v1_2.py
@@ -28,14 +31,20 @@
 cwl_utils.egg-info/top_level.txt
 cwl_utils/parser/__init__.py
 testdata/dockstore-tool-md5sum.cwl
 testdata/md5sum.cwl
 testdata/md5sum.input
 testdata/md5sum.json
 testdata/workflow_input_format_expr.cwl
+testdata/workflow_input_format_expr_v1_1.cwl
+testdata/workflow_input_format_expr_v1_2.cwl
 testdata/workflow_input_sf_expr.cwl
 testdata/workflow_input_sf_expr_array.cwl
+testdata/workflow_input_sf_expr_array_v1_1.cwl
+testdata/workflow_input_sf_expr_array_v1_2.cwl
+testdata/workflow_input_sf_expr_v1_1.cwl
+testdata/workflow_input_sf_expr_v1_2.cwl
 tests/__init__.py
 tests/test_cite_extract.py
 tests/test_docker_extract.py
 tests/test_etools_to_clt.py
 tests/test_graph_split.py
```

### Comparing `cwl-utils-0.8/setup.py` & `cwl-utils-0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     include_package_data=True,
     python_requires=">=3.6",
     install_requires=[
         "ruamel.yaml<=0.16.5,>=0.12.4",
         "requests",
         "schema-salad >= 7, < 8",
         "typing_extensions",
-        "cwltool",
+        "cwltool >= 3.0.20201113183607",
         "cwlformat",
     ],
     setup_requires=[] + pytest_runner,
     tests_require=["pytest<7", "cwltool"],
     test_suite="tests",
     scripts=[
         "cwl_utils/docker_extract.py",
```

### Comparing `cwl-utils-0.8/testdata/dockstore-tool-md5sum.cwl` & `cwl-utils-0.9/testdata/dockstore-tool-md5sum.cwl`

 * *Files identical despite different names*

### Comparing `cwl-utils-0.8/testdata/workflow_input_format_expr.cwl` & `cwl-utils-0.9/testdata/workflow_input_format_expr.cwl`

 * *Files identical despite different names*

### Comparing `cwl-utils-0.8/testdata/workflow_input_sf_expr.cwl` & `cwl-utils-0.9/testdata/workflow_input_sf_expr.cwl`

 * *Files identical despite different names*

### Comparing `cwl-utils-0.8/testdata/workflow_input_sf_expr_array.cwl` & `cwl-utils-0.9/testdata/workflow_input_sf_expr_array.cwl`

 * *Files identical despite different names*

### Comparing `cwl-utils-0.8/tests/test_docker_extract.py` & `cwl-utils-0.9/tests/test_docker_extract.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from os import environ
 from pathlib import Path
 from tempfile import TemporaryDirectory
-from unittest import skipIf
 
 import pytest
+
 import cwl_utils.parser_v1_0 as parser
 from cwl_utils.docker_extract import traverse
 from cwl_utils.image_puller import DockerImagePuller, SingularityImagePuller
 
 HERE = Path(__file__).resolve().parent
 TEST_CWL = HERE / "../testdata/md5sum.cwl"
 TRAVIS = environ.get("TRAVIS", "false") == "true"
@@ -20,14 +20,15 @@
 
     with TemporaryDirectory() as tmpdir:
         for req in set(traverse(loaded)):
             image_puller = DockerImagePuller(req.dockerPull, tmpdir)
             image_puller.save_docker_image()
             _ = image_puller.generate_udocker_loading_command()
 
+
 @pytest.mark.skipif(TRAVIS, reason="travis cannot run singularity in docker")
 def test_traverse_workflow_singularity() -> None:
     """Test container extraction tool using Singularity."""
     loaded = parser.load_document(str(TEST_CWL.resolve()))
 
     with TemporaryDirectory() as tmpdir:
         for req in set(traverse(loaded)):
```

### Comparing `cwl-utils-0.8/tests/test_graph_split.py` & `cwl-utils-0.9/tests/test_graph_split.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Test the CWL $graph document splitter tool."""
 import os
 from io import StringIO
 from pathlib import Path
-from unittest import TestCase
 
 import requests
 
 from cwl_utils.graph_split import run
 
 URI = "https://gist.githubusercontent.com/altairwei/6a0097db95cad23de36f825ed3b9f4b0/raw/83f332931c3093ee73554cd7f60054ce17d03239/rhapsody_wta_1.8.packed.cwl"
```

