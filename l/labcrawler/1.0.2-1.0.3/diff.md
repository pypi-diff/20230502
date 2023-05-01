# Comparing `tmp/labcrawler-1.0.2.tar.gz` & `tmp/labcrawler-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labcrawler-1.0.2.tar", last modified: Mon Apr 24 02:39:45 2023, max compression
+gzip compressed data, was "labcrawler-1.0.3.tar", last modified: Mon May  1 22:18:46 2023, max compression
```

## Comparing `labcrawler-1.0.2.tar` & `labcrawler-1.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-24 02:39:45.849878 labcrawler-1.0.2/
--rw-r--r--   0 francispotter   (501) staff       (20)     1071 2023-03-20 17:28:47.000000 labcrawler-1.0.2/LICENSE
--rw-r--r--   0 francispotter   (501) staff       (20)       30 2023-04-22 03:09:31.000000 labcrawler-1.0.2/MANIFEST.in
--rw-r--r--   0 francispotter   (501) staff       (20)    13869 2023-04-24 02:39:45.847777 labcrawler-1.0.2/PKG-INFO
--rw-r--r--   0 francispotter   (501) staff       (20)    13587 2023-04-24 02:38:57.000000 labcrawler-1.0.2/README.md
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-24 02:39:45.812782 labcrawler-1.0.2/labcrawler/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-04-05 15:51:26.000000 labcrawler-1.0.2/labcrawler/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)       90 2023-04-22 03:09:31.000000 labcrawler-1.0.2/labcrawler/__main__.py
--rw-r--r--   0 francispotter   (501) staff       (20)     4267 2023-04-22 03:09:31.000000 labcrawler-1.0.2/labcrawler/_legacy.py
--rw-r--r--   0 francispotter   (501) staff       (20)     3573 2023-04-24 01:27:34.000000 labcrawler-1.0.2/labcrawler/analysis.py
--rw-r--r--   0 francispotter   (501) staff       (20)     5351 2023-04-24 00:51:06.000000 labcrawler-1.0.2/labcrawler/cli.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1101 2023-04-05 15:42:21.000000 labcrawler-1.0.2/labcrawler/gitlab_ci_config.py
--rw-r--r--   0 francispotter   (501) staff       (20)     3131 2023-04-24 00:56:03.000000 labcrawler-1.0.2/labcrawler/gitlab_ci_data_loader.py
--rw-r--r--   0 francispotter   (501) staff       (20)     2388 2023-04-05 15:46:57.000000 labcrawler-1.0.2/labcrawler/gitlab_repository_files_extractor.py
--rw-r--r--   0 francispotter   (501) staff       (20)      451 2023-04-22 03:09:31.000000 labcrawler-1.0.2/labcrawler/project_data_file.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-24 02:39:45.844832 labcrawler-1.0.2/labcrawler/templates/
--rw-r--r--   0 francispotter   (501) staff       (20)       51 2023-04-22 03:09:31.000000 labcrawler-1.0.2/labcrawler/templates/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)      264 2023-04-22 03:09:31.000000 labcrawler-1.0.2/labcrawler/templates/labcrawler.json.template
--rw-r--r--   0 francispotter   (501) staff       (20)     1003 2023-04-22 03:09:31.000000 labcrawler-1.0.2/labcrawler/templates/meltano.yml
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-24 02:39:45.842778 labcrawler-1.0.2/labcrawler.egg-info/
--rw-r--r--   0 francispotter   (501) staff       (20)    13869 2023-04-24 02:39:45.000000 labcrawler-1.0.2/labcrawler.egg-info/PKG-INFO
--rw-r--r--   0 francispotter   (501) staff       (20)      656 2023-04-24 02:39:45.000000 labcrawler-1.0.2/labcrawler.egg-info/SOURCES.txt
--rw-r--r--   0 francispotter   (501) staff       (20)        1 2023-04-24 02:39:45.000000 labcrawler-1.0.2/labcrawler.egg-info/dependency_links.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       87 2023-04-24 02:39:45.000000 labcrawler-1.0.2/labcrawler.egg-info/entry_points.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       64 2023-04-24 02:39:45.000000 labcrawler-1.0.2/labcrawler.egg-info/requires.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       11 2023-04-24 02:39:45.000000 labcrawler-1.0.2/labcrawler.egg-info/top_level.txt
--rw-r--r--   0 francispotter   (501) staff       (20)      689 2023-04-22 03:09:31.000000 labcrawler-1.0.2/pyproject.toml
--rw-r--r--   0 francispotter   (501) staff       (20)       38 2023-04-24 02:39:45.850089 labcrawler-1.0.2/setup.cfg
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-24 02:39:45.845609 labcrawler-1.0.2/test/
--rw-r--r--   0 francispotter   (501) staff       (20)     1721 2023-04-05 15:42:37.000000 labcrawler-1.0.2/test/test_gitlab_ci_config.py
--rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-04-24 02:39:33.000000 labcrawler-1.0.2/version
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-05-01 22:18:46.958523 labcrawler-1.0.3/
+-rw-r--r--   0 francispotter   (501) staff       (20)     1071 2023-03-20 17:28:47.000000 labcrawler-1.0.3/LICENSE
+-rw-r--r--   0 francispotter   (501) staff       (20)       30 2023-04-22 03:09:31.000000 labcrawler-1.0.3/MANIFEST.in
+-rw-r--r--   0 francispotter   (501) staff       (20)    14416 2023-05-01 22:18:46.957861 labcrawler-1.0.3/PKG-INFO
+-rw-r--r--   0 francispotter   (501) staff       (20)    14134 2023-05-01 22:16:55.000000 labcrawler-1.0.3/README.md
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-05-01 22:18:46.613164 labcrawler-1.0.3/labcrawler/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-04-05 15:51:26.000000 labcrawler-1.0.3/labcrawler/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)       90 2023-04-22 03:09:31.000000 labcrawler-1.0.3/labcrawler/__main__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     4267 2023-04-22 03:09:31.000000 labcrawler-1.0.3/labcrawler/_legacy.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     3710 2023-05-01 22:16:55.000000 labcrawler-1.0.3/labcrawler/analysis.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     5431 2023-05-01 22:16:55.000000 labcrawler-1.0.3/labcrawler/cli.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     1101 2023-04-05 15:42:21.000000 labcrawler-1.0.3/labcrawler/gitlab_ci_config.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     3131 2023-05-01 22:16:51.000000 labcrawler-1.0.3/labcrawler/gitlab_ci_data_loader.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     2388 2023-04-05 15:46:57.000000 labcrawler-1.0.3/labcrawler/gitlab_repository_files_extractor.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      451 2023-04-22 03:09:31.000000 labcrawler-1.0.3/labcrawler/project_data_file.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-05-01 22:18:46.951966 labcrawler-1.0.3/labcrawler/templates/
+-rw-r--r--   0 francispotter   (501) staff       (20)       51 2023-04-22 03:09:31.000000 labcrawler-1.0.3/labcrawler/templates/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      264 2023-04-22 03:09:31.000000 labcrawler-1.0.3/labcrawler/templates/labcrawler.json.template
+-rw-r--r--   0 francispotter   (501) staff       (20)     1003 2023-04-22 03:09:31.000000 labcrawler-1.0.3/labcrawler/templates/meltano.yml
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-05-01 22:18:46.903715 labcrawler-1.0.3/labcrawler.egg-info/
+-rw-r--r--   0 francispotter   (501) staff       (20)    14416 2023-05-01 22:18:46.000000 labcrawler-1.0.3/labcrawler.egg-info/PKG-INFO
+-rw-r--r--   0 francispotter   (501) staff       (20)      656 2023-05-01 22:18:46.000000 labcrawler-1.0.3/labcrawler.egg-info/SOURCES.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)        1 2023-05-01 22:18:46.000000 labcrawler-1.0.3/labcrawler.egg-info/dependency_links.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)       87 2023-05-01 22:18:46.000000 labcrawler-1.0.3/labcrawler.egg-info/entry_points.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)       80 2023-05-01 22:18:46.000000 labcrawler-1.0.3/labcrawler.egg-info/requires.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)       11 2023-05-01 22:18:46.000000 labcrawler-1.0.3/labcrawler.egg-info/top_level.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)      714 2023-05-01 22:16:55.000000 labcrawler-1.0.3/pyproject.toml
+-rw-r--r--   0 francispotter   (501) staff       (20)       38 2023-05-01 22:18:46.958665 labcrawler-1.0.3/setup.cfg
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-05-01 22:18:46.956537 labcrawler-1.0.3/test/
+-rw-r--r--   0 francispotter   (501) staff       (20)     1721 2023-04-05 15:42:37.000000 labcrawler-1.0.3/test/test_gitlab_ci_config.py
+-rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-05-01 22:18:21.000000 labcrawler-1.0.3/version
```

### Comparing `labcrawler-1.0.2/LICENSE` & `labcrawler-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `labcrawler-1.0.2/PKG-INFO` & `labcrawler-1.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labcrawler
-Version: 1.0.2
+Version: 1.0.3
 Summary: Analysis tool for GitLab project and CI configurations
 Author-email: Steampunk Wizard <labcrawler@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.6.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -199,14 +199,26 @@
 
 If you want to see all of the rows when performing queries, rather than just a sample, try:
 
 ``` python
 pandas.set_option('display.max_rows', None)
 ```
 
+For prettier output, we've added a `neat()` function.
+
+```python
+>>> neat(projects[['name_with_namespace','merge_method']])
+name_with_namespace                                          merge_method
+-----------------------------------------------------------  --------------
+Steampunk Wizard / WizLib                                    merge
+Steampunk Wizard / FileWiz                                   merge
+Steampunk Wizard / LabCrawler                                merge
+Steampunk Wizard / Busy                                      merge
+```
+
 Roadmap
 -------
 
 We maintain an informal roadmap of future functionality. Development of such functionality depends on contributions from the community, a generous donation, or us simply finding the time ;-).
 
 - Put all these roadmap items into GitLab issues for visibility and sharing
 - Fix the bug where users are being loaded into the CSV multiple times (possible Meltano tap-gitlab fix?)
```

### Comparing `labcrawler-1.0.2/README.md` & `labcrawler-1.0.3/labcrawler.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: labcrawler
+Version: 1.0.3
+Summary: Analysis tool for GitLab project and CI configurations
+Author-email: Steampunk Wizard <labcrawler@steampunkwizard.ca>
+License: MIT
+Requires-Python: >=3.6.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 
 Summary
 -------
 
 LabCrawler by [Francis Potter](https://www.linkedin.com/in/francispotter/) using [Meltano](https://meltano.com/) and [Pandas](https://pandas.pydata.org/).
 
 Examine a set of GitLab projects for usage of governance processes such as CI/CD, merge requests, merge request approvals, security scanning, and code review. This tool pulls project and group configuration and recent history data from GitLab and returns it in a CSV that can be imported to a spreadsheet.
@@ -189,14 +199,26 @@
 
 If you want to see all of the rows when performing queries, rather than just a sample, try:
 
 ``` python
 pandas.set_option('display.max_rows', None)
 ```
 
+For prettier output, we've added a `neat()` function.
+
+```python
+>>> neat(projects[['name_with_namespace','merge_method']])
+name_with_namespace                                          merge_method
+-----------------------------------------------------------  --------------
+Steampunk Wizard / WizLib                                    merge
+Steampunk Wizard / FileWiz                                   merge
+Steampunk Wizard / LabCrawler                                merge
+Steampunk Wizard / Busy                                      merge
+```
+
 Roadmap
 -------
 
 We maintain an informal roadmap of future functionality. Development of such functionality depends on contributions from the community, a generous donation, or us simply finding the time ;-).
 
 - Put all these roadmap items into GitLab issues for visibility and sharing
 - Fix the bug where users are being loaded into the CSV multiple times (possible Meltano tap-gitlab fix?)
```

### Comparing `labcrawler-1.0.2/labcrawler/_legacy.py` & `labcrawler-1.0.3/labcrawler/_legacy.py`

 * *Files identical despite different names*

### Comparing `labcrawler-1.0.2/labcrawler/analysis.py` & `labcrawler-1.0.3/labcrawler/analysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from pathlib import Path
 from dataclasses import dataclass
 from sys import argv
 from inspect import get_annotations
 
 from pandas import DataFrame
 from pandas import read_csv
+from tabulate import tabulate
 
 @dataclass
 class DataSet:
     access_levels:DataFrame = None
     groups:DataFrame = None
     projects:DataFrame = None
     branches:DataFrame = None
@@ -72,7 +73,9 @@
                         join(self.projects[['name','path_with_namespace']].add_prefix('project_'), on='project_id', how='right')
         
         for datatype in DATATYPES:
             df = getattr(self, datatype)
             if df is not None:
                 df.index.name = 'id'
 
+def output_neat(dataframe):
+        print(tabulate(dataframe, showindex=False, headers=dataframe.columns))
```

### Comparing `labcrawler-1.0.2/labcrawler/cli.py` & `labcrawler-1.0.3/labcrawler/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from platformdirs import user_data_dir
 from platformdirs import user_documents_dir
 
 from labcrawler.analysis import RawDataSet
 from labcrawler.analysis import AssembledDataSet
 from labcrawler.analysis import DATATYPES
 from labcrawler.gitlab_ci_data_loader import GitLabCIDataLoader
-
+from labcrawler.analysis import output_neat
 
 APPNAME = "LabCrawler"
 APPAUTHOR = "SteampunkWizard"
 
 class LabCrawlerCLI:
 
     def __init__(self):
@@ -145,8 +145,9 @@
     def analyze(self):
         raw = RawDataSet(self.config['output_dir'])
         assembled = AssembledDataSet(raw)
         values = vars(assembled)
         banner = "\n".join([f"{len(values[t].index)} {t}" for t in values])
         banner = f"LabCrawler analysis\n{banner}\nPython {python_version()}"
         values['raw'] = raw
+        values['neat'] = output_neat
         interact(local=values, banner=banner)
```

### Comparing `labcrawler-1.0.2/labcrawler/gitlab_ci_config.py` & `labcrawler-1.0.3/labcrawler/gitlab_ci_config.py`

 * *Files identical despite different names*

### Comparing `labcrawler-1.0.2/labcrawler/gitlab_ci_data_loader.py` & `labcrawler-1.0.3/labcrawler/gitlab_ci_data_loader.py`

 * *Files identical despite different names*

### Comparing `labcrawler-1.0.2/labcrawler/gitlab_repository_files_extractor.py` & `labcrawler-1.0.3/labcrawler/gitlab_repository_files_extractor.py`

 * *Files identical despite different names*

### Comparing `labcrawler-1.0.2/labcrawler/templates/meltano.yml` & `labcrawler-1.0.3/labcrawler/templates/meltano.yml`

 * *Files identical despite different names*

### Comparing `labcrawler-1.0.2/labcrawler.egg-info/PKG-INFO` & `labcrawler-1.0.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: labcrawler
-Version: 1.0.2
-Summary: Analysis tool for GitLab project and CI configurations
-Author-email: Steampunk Wizard <labcrawler@steampunkwizard.ca>
-License: MIT
-Requires-Python: >=3.6.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 Summary
 -------
 
 LabCrawler by [Francis Potter](https://www.linkedin.com/in/francispotter/) using [Meltano](https://meltano.com/) and [Pandas](https://pandas.pydata.org/).
 
 Examine a set of GitLab projects for usage of governance processes such as CI/CD, merge requests, merge request approvals, security scanning, and code review. This tool pulls project and group configuration and recent history data from GitLab and returns it in a CSV that can be imported to a spreadsheet.
@@ -199,14 +189,26 @@
 
 If you want to see all of the rows when performing queries, rather than just a sample, try:
 
 ``` python
 pandas.set_option('display.max_rows', None)
 ```
 
+For prettier output, we've added a `neat()` function.
+
+```python
+>>> neat(projects[['name_with_namespace','merge_method']])
+name_with_namespace                                          merge_method
+-----------------------------------------------------------  --------------
+Steampunk Wizard / WizLib                                    merge
+Steampunk Wizard / FileWiz                                   merge
+Steampunk Wizard / LabCrawler                                merge
+Steampunk Wizard / Busy                                      merge
+```
+
 Roadmap
 -------
 
 We maintain an informal roadmap of future functionality. Development of such functionality depends on contributions from the community, a generous donation, or us simply finding the time ;-).
 
 - Put all these roadmap items into GitLab issues for visibility and sharing
 - Fix the bug where users are being loaded into the CSV multiple times (possible Meltano tap-gitlab fix?)
```

### Comparing `labcrawler-1.0.2/labcrawler.egg-info/SOURCES.txt` & `labcrawler-1.0.3/labcrawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `labcrawler-1.0.2/pyproject.toml` & `labcrawler-1.0.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 readme = "README.md"
 requires-python = ">=3.6.5"
 license = {text = "MIT"}
 dependencies = [
     "platformdirs >=3.2.0",
     "wizlib >=0.2.2",
     "meltano >= 2.17.1",
-    "pandas >= 2.0.0"
+    "pandas >= 2.0.0",
+    "tabulate >= 0.9.0"
 ]
 dynamic = ["version"]
 
 [tool.setuptools.package-dir]
 labcrawler = "labcrawler"
 
 [project.scripts]
```

### Comparing `labcrawler-1.0.2/test/test_gitlab_ci_config.py` & `labcrawler-1.0.3/test/test_gitlab_ci_config.py`

 * *Files identical despite different names*

