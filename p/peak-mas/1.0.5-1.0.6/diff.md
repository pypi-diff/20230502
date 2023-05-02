# Comparing `tmp/peak-mas-1.0.5.tar.gz` & `tmp/peak-mas-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peak-mas-1.0.5.tar", last modified: Thu Apr 20 14:28:00 2023, max compression
+gzip compressed data, was "peak-mas-1.0.6.tar", last modified: Tue May  2 13:06:26 2023, max compression
```

## Comparing `peak-mas-1.0.5.tar` & `peak-mas-1.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2023-04-20 14:28:00.929259 peak-mas-1.0.5/
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)    35148 2022-11-16 18:35:26.000000 peak-mas-1.0.5/LICENSE
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     6792 2023-04-20 14:28:00.929259 peak-mas-1.0.5/PKG-INFO
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     5843 2022-11-16 18:35:26.000000 peak-mas-1.0.5/README.md
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     1664 2023-04-20 14:27:36.000000 peak-mas-1.0.5/pyproject.toml
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)       38 2023-04-20 14:28:00.929259 peak-mas-1.0.5/setup.cfg
-drwxr-xr-x   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2023-04-20 14:28:00.925259 peak-mas-1.0.5/src/
-drwxr-xr-x   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2023-04-20 14:28:00.927260 peak-mas-1.0.5/src/peak/
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)      669 2023-04-20 14:27:36.000000 peak-mas-1.0.5/src/peak/__init__.py
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     3299 2023-04-20 14:25:32.000000 peak-mas-1.0.5/src/peak/__main__.py
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)    17766 2023-04-20 14:25:38.000000 peak-mas-1.0.5/src/peak/agents.py
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     3519 2023-04-20 14:25:45.000000 peak-mas-1.0.5/src/peak/behaviours.py
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     3657 2023-04-20 13:30:25.000000 peak-mas-1.0.5/src/peak/bootloader.py
-drwxr-xr-x   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2023-04-20 14:28:00.927260 peak-mas-1.0.5/src/peak/cli/
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2022-11-16 18:35:26.000000 peak-mas-1.0.5/src/peak/cli/__init__.py
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)      845 2023-04-20 14:25:17.000000 peak-mas-1.0.5/src/peak/cli/df.py
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     2837 2023-04-20 14:25:25.000000 peak-mas-1.0.5/src/peak/cli/mas.py
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     6776 2023-04-20 13:30:25.000000 peak-mas-1.0.5/src/peak/core.py
-drwxr-xr-x   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2023-04-20 14:28:00.929259 peak-mas-1.0.5/src/peak_mas.egg-info/
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     6792 2023-04-20 14:28:00.000000 peak-mas-1.0.5/src/peak_mas.egg-info/PKG-INFO
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)      438 2023-04-20 14:28:00.000000 peak-mas-1.0.5/src/peak_mas.egg-info/SOURCES.txt
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)        1 2023-04-20 14:28:00.000000 peak-mas-1.0.5/src/peak_mas.egg-info/dependency_links.txt
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)       44 2023-04-20 14:28:00.000000 peak-mas-1.0.5/src/peak_mas.egg-info/entry_points.txt
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)      119 2023-04-20 14:28:00.000000 peak-mas-1.0.5/src/peak_mas.egg-info/requires.txt
--rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)        5 2023-04-20 14:28:00.000000 peak-mas-1.0.5/src/peak_mas.egg-info/top_level.txt
+drwxr-xr-x   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2023-05-02 13:06:26.483331 peak-mas-1.0.6/
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)    35148 2022-11-16 18:35:26.000000 peak-mas-1.0.6/LICENSE
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     6792 2023-05-02 13:06:26.483331 peak-mas-1.0.6/PKG-INFO
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     5843 2022-11-16 18:35:26.000000 peak-mas-1.0.6/README.md
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     1664 2023-05-02 13:06:10.000000 peak-mas-1.0.6/pyproject.toml
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)       38 2023-05-02 13:06:26.483331 peak-mas-1.0.6/setup.cfg
+drwxr-xr-x   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2023-05-02 13:06:26.480331 peak-mas-1.0.6/src/
+drwxr-xr-x   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2023-05-02 13:06:26.482331 peak-mas-1.0.6/src/peak/
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)      603 2023-05-02 13:06:10.000000 peak-mas-1.0.6/src/peak/__init__.py
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     3299 2023-04-20 14:45:48.000000 peak-mas-1.0.6/src/peak/__main__.py
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)    17777 2023-05-02 11:06:09.000000 peak-mas-1.0.6/src/peak/agents.py
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     3519 2023-04-20 14:36:05.000000 peak-mas-1.0.6/src/peak/behaviours.py
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     3608 2023-04-20 14:39:46.000000 peak-mas-1.0.6/src/peak/bootloader.py
+drwxr-xr-x   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2023-05-02 13:06:26.482331 peak-mas-1.0.6/src/peak/cli/
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2022-11-16 18:35:26.000000 peak-mas-1.0.6/src/peak/cli/__init__.py
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)      845 2023-04-20 14:39:59.000000 peak-mas-1.0.6/src/peak/cli/df.py
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     2837 2023-04-20 14:45:48.000000 peak-mas-1.0.6/src/peak/cli/mas.py
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     6727 2023-04-20 14:39:52.000000 peak-mas-1.0.6/src/peak/core.py
+drwxr-xr-x   0 brunus-reberes  (1000) brunus-reberes  (1000)        0 2023-05-02 13:06:26.483331 peak-mas-1.0.6/src/peak_mas.egg-info/
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)     6792 2023-05-02 13:06:26.000000 peak-mas-1.0.6/src/peak_mas.egg-info/PKG-INFO
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)      438 2023-05-02 13:06:26.000000 peak-mas-1.0.6/src/peak_mas.egg-info/SOURCES.txt
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)        1 2023-05-02 13:06:26.000000 peak-mas-1.0.6/src/peak_mas.egg-info/dependency_links.txt
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)       44 2023-05-02 13:06:26.000000 peak-mas-1.0.6/src/peak_mas.egg-info/entry_points.txt
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)      119 2023-05-02 13:06:26.000000 peak-mas-1.0.6/src/peak_mas.egg-info/requires.txt
+-rw-r--r--   0 brunus-reberes  (1000) brunus-reberes  (1000)        5 2023-05-02 13:06:26.000000 peak-mas-1.0.6/src/peak_mas.egg-info/top_level.txt
```

### Comparing `peak-mas-1.0.5/LICENSE` & `peak-mas-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `peak-mas-1.0.5/PKG-INFO` & `peak-mas-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peak-mas
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python-based framework for heterogeneous agent communities
 Author-email: Bruno Ribeiro <brgri@isep.ipp.pt>
 Project-URL: Homepage, https://www.gecad.isep.ipp.pt/peak
 Project-URL: Github, https://github.com/gecad-group/peak-mas
 Keywords: framework,multiagent,agent-based,ecosystem,spade,xmpp
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `peak-mas-1.0.5/README.md` & `peak-mas-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `peak-mas-1.0.5/pyproject.toml` & `peak-mas-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "peak-mas"
-version = "1.0.5"
+version = "1.0.6"
 description = "Python-based framework for heterogeneous agent communities"
 readme = "README.md"
 authors = [{ name = "Bruno Ribeiro", email = "brgri@isep.ipp.pt" }]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -38,15 +38,15 @@
 Homepage = "https://www.gecad.isep.ipp.pt/peak"
 Github = "https://github.com/gecad-group/peak-mas"
 
 [project.scripts]
 peak = "peak.__main__:main"
 
 [tool.bumpver]
-current_version = "1.0.5"
+current_version = "1.0.6"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "chore: bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `peak-mas-1.0.5/src/peak/__init__.py` & `peak-mas-1.0.6/src/peak/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,24 +3,21 @@
 PEAK is a framework for developing communities of heterogeneous agents. 
 This communities are multi-agent systems that can coexist and exchange 
 resources and information with each other easly. 
 
 isort: skip_file
 """
 
-# Standard library imports
 import logging
 
-# Third party imports
 from spade.message import Message
 from spade.template import Template
 
-# Reader imports
 from peak.core import *
 from peak.agents import *
 from peak.behaviours import *
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 __author__ = "Bruno Ribeiro"
 __email__ = "brgri@isep.ipp.pt"
-__version__ = "1.0.5"
+__version__ = "1.0.6"
```

### Comparing `peak-mas-1.0.5/src/peak/__main__.py` & `peak-mas-1.0.6/src/peak/__main__.py`

 * *Files identical despite different names*

### Comparing `peak-mas-1.0.5/src/peak/agents.py` & `peak-mas-1.0.6/src/peak/agents.py`

 * *Files 0% similar despite different names*

```diff
@@ -442,15 +442,15 @@
         )
 
         # Configure CORS on all routes.
         for route in list(self.web.app.router.routes()):
             cors.add(route)
 
         # Start web API
-        self.web.start(port=self.port)
+        self.web.start("0.0.0.0", port=self.port)
         self.logger.info("REST API running on port " + self.port)
 
     async def get_groups(self, request):
         return {
             "nodes": list(self.ecosystemhierarchy_data["nodes"]),
             "links": list(self.ecosystemhierarchy_data["links"]),
             "categories": list(self.ecosystemhierarchy_data["categories"]),
```

### Comparing `peak-mas-1.0.5/src/peak/behaviours.py` & `peak-mas-1.0.6/src/peak/behaviours.py`

 * *Files identical despite different names*

### Comparing `peak-mas-1.0.5/src/peak/bootloader.py` & `peak-mas-1.0.6/src/peak/bootloader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-# Standard library imports
 import asyncio
 import importlib
 import logging
 import os
 import sys
 import time
 from multiprocessing import Process
 from pathlib import Path
 from typing import List, Type
 
-# Third party imports
 from aioxmpp import JID
 from spade import quit_spade
 
 logger = logging.getLogger(__name__)
 
 
 async def _wait_for_processes(processes):
```

### Comparing `peak-mas-1.0.5/src/peak/cli/df.py` & `peak-mas-1.0.6/src/peak/cli/df.py`

 * *Files identical despite different names*

### Comparing `peak-mas-1.0.5/src/peak/cli/mas.py` & `peak-mas-1.0.6/src/peak/cli/mas.py`

 * *Files identical despite different names*

### Comparing `peak-mas-1.0.5/src/peak/core.py` & `peak-mas-1.0.6/src/peak/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-# Standard library imports
 import logging as _logging
 from abc import ABCMeta as _ABCMeta
 from typing import Dict, List
 
-# Third party imports
 import aioxmpp as _aioxmpp
 import spade as _spade
 from aioxmpp import JID
 from aioxmpp.callbacks import first_signal
 
 _module_logger = _logging.getLogger(__name__)
```

### Comparing `peak-mas-1.0.5/src/peak_mas.egg-info/PKG-INFO` & `peak-mas-1.0.6/src/peak_mas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peak-mas
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python-based framework for heterogeneous agent communities
 Author-email: Bruno Ribeiro <brgri@isep.ipp.pt>
 Project-URL: Homepage, https://www.gecad.isep.ipp.pt/peak
 Project-URL: Github, https://github.com/gecad-group/peak-mas
 Keywords: framework,multiagent,agent-based,ecosystem,spade,xmpp
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

