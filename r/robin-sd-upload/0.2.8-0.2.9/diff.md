# Comparing `tmp/robin_sd_upload-0.2.8.tar.gz` & `tmp/robin_sd_upload-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/robin_sd_upload-0.2.8.tar", last modified: Wed Feb 15 15:28:51 2023, max compression
+gzip compressed data, was "dist/robin_sd_upload-0.2.9.tar", last modified: Wed Feb 15 15:33:30 2023, max compression
```

## Comparing `robin_sd_upload-0.2.8.tar` & `robin_sd_upload-0.2.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 15:28:51.000000 robin_sd_upload-0.2.8/
--rw-r--r--   0 root         (0) root         (0)      633 2023-02-15 15:28:51.000000 robin_sd_upload-0.2.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-02-15 15:28:36.000000 robin_sd_upload-0.2.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 15:28:51.000000 robin_sd_upload-0.2.8/robin_sd_upload/
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-02-15 15:28:36.000000 robin_sd_upload-0.2.8/robin_sd_upload/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      185 2023-02-15 15:28:36.000000 robin_sd_upload-0.2.8/robin_sd_upload/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-02-15 15:28:36.000000 robin_sd_upload-0.2.8/robin_sd_upload/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 15:28:51.000000 robin_sd_upload-0.2.8/robin_sd_upload/api_interaction/
--rw-rw-rw-   0 root         (0) root         (0)       48 2023-02-15 15:28:36.000000 robin_sd_upload-0.2.8/robin_sd_upload/api_interaction/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1537 2023-02-15 15:28:36.000000 robin_sd_upload-0.2.8/robin_sd_upload/api_interaction/get_bearer_token.py
--rw-rw-rw-   0 root         (0) root         (0)     1749 2023-02-15 15:28:36.000000 robin_sd_upload-0.2.8/robin_sd_upload/api_interaction/push_software.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 15:28:51.000000 robin_sd_upload-0.2.8/robin_sd_upload/slack_interaction/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-02-15 15:28:36.000000 robin_sd_upload-0.2.8/robin_sd_upload/slack_interaction/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2002 2023-02-15 15:28:36.000000 robin_sd_upload-0.2.8/robin_sd_upload/slack_interaction/slack_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 15:28:51.000000 robin_sd_upload-0.2.8/robin_sd_upload/supportive_scripts/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-02-15 15:28:36.000000 robin_sd_upload-0.2.8/robin_sd_upload/supportive_scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3640 2023-02-15 15:28:36.000000 robin_sd_upload-0.2.8/robin_sd_upload/supportive_scripts/arg_parse.py
--rw-rw-rw-   0 root         (0) root         (0)     1264 2023-02-15 15:28:36.000000 robin_sd_upload-0.2.8/robin_sd_upload/supportive_scripts/check_upload_file.py
--rw-rw-rw-   0 root         (0) root         (0)      644 2023-02-15 15:28:36.000000 robin_sd_upload-0.2.8/robin_sd_upload/supportive_scripts/create_folder.py
--rw-rw-rw-   0 root         (0) root         (0)      875 2023-02-15 15:28:36.000000 robin_sd_upload-0.2.8/robin_sd_upload/supportive_scripts/create_zip.py
--rw-rw-rw-   0 root         (0) root         (0)     2261 2023-02-15 15:28:36.000000 robin_sd_upload-0.2.8/robin_sd_upload/supportive_scripts/logger.py
--rw-rw-rw-   0 root         (0) root         (0)      567 2023-02-15 15:28:36.000000 robin_sd_upload-0.2.8/robin_sd_upload/supportive_scripts/remove_zip.py
--rw-rw-rw-   0 root         (0) root         (0)     1574 2023-02-15 15:28:36.000000 robin_sd_upload-0.2.8/robin_sd_upload/supportive_scripts/sudo_file.py
--rw-rw-rw-   0 root         (0) root         (0)     1389 2023-02-15 15:28:36.000000 robin_sd_upload-0.2.8/robin_sd_upload/supportive_scripts/validate.py
--rw-rw-rw-   0 root         (0) root         (0)     1229 2023-02-15 15:28:36.000000 robin_sd_upload-0.2.8/robin_sd_upload/supportive_scripts/version_checker.py
--rw-rw-rw-   0 root         (0) root         (0)     2758 2023-02-15 15:28:36.000000 robin_sd_upload-0.2.8/robin_sd_upload/supportive_scripts/yaml_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 15:28:51.000000 robin_sd_upload-0.2.8/robin_sd_upload.egg-info/
--rw-r--r--   0 root         (0) root         (0)      633 2023-02-15 15:28:51.000000 robin_sd_upload-0.2.8/robin_sd_upload.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1157 2023-02-15 15:28:51.000000 robin_sd_upload-0.2.8/robin_sd_upload.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-15 15:28:51.000000 robin_sd_upload-0.2.8/robin_sd_upload.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       67 2023-02-15 15:28:51.000000 robin_sd_upload-0.2.8/robin_sd_upload.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-02-15 15:28:51.000000 robin_sd_upload-0.2.8/robin_sd_upload.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-02-15 15:28:51.000000 robin_sd_upload-0.2.8/robin_sd_upload.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-15 15:28:51.000000 robin_sd_upload-0.2.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1051 2023-02-15 15:28:36.000000 robin_sd_upload-0.2.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 15:28:51.000000 robin_sd_upload-0.2.8/tests/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-02-15 15:28:36.000000 robin_sd_upload-0.2.8/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       17 2023-02-15 15:28:36.000000 robin_sd_upload-0.2.8/tests/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 15:33:30.000000 robin_sd_upload-0.2.9/
+-rw-r--r--   0 root         (0) root         (0)      633 2023-02-15 15:33:30.000000 robin_sd_upload-0.2.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-02-15 15:33:08.000000 robin_sd_upload-0.2.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 15:33:30.000000 robin_sd_upload-0.2.9/robin_sd_upload/
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-02-15 15:33:08.000000 robin_sd_upload-0.2.9/robin_sd_upload/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-02-15 15:33:08.000000 robin_sd_upload-0.2.9/robin_sd_upload/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-02-15 15:33:08.000000 robin_sd_upload-0.2.9/robin_sd_upload/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 15:33:30.000000 robin_sd_upload-0.2.9/robin_sd_upload/api_interaction/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2023-02-15 15:33:08.000000 robin_sd_upload-0.2.9/robin_sd_upload/api_interaction/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1537 2023-02-15 15:33:08.000000 robin_sd_upload-0.2.9/robin_sd_upload/api_interaction/get_bearer_token.py
+-rw-rw-rw-   0 root         (0) root         (0)     1749 2023-02-15 15:33:08.000000 robin_sd_upload-0.2.9/robin_sd_upload/api_interaction/push_software.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 15:33:30.000000 robin_sd_upload-0.2.9/robin_sd_upload/slack_interaction/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-02-15 15:33:08.000000 robin_sd_upload-0.2.9/robin_sd_upload/slack_interaction/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2002 2023-02-15 15:33:08.000000 robin_sd_upload-0.2.9/robin_sd_upload/slack_interaction/slack_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 15:33:30.000000 robin_sd_upload-0.2.9/robin_sd_upload/supportive_scripts/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-02-15 15:33:08.000000 robin_sd_upload-0.2.9/robin_sd_upload/supportive_scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3640 2023-02-15 15:33:08.000000 robin_sd_upload-0.2.9/robin_sd_upload/supportive_scripts/arg_parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     1264 2023-02-15 15:33:08.000000 robin_sd_upload-0.2.9/robin_sd_upload/supportive_scripts/check_upload_file.py
+-rw-rw-rw-   0 root         (0) root         (0)      644 2023-02-15 15:33:08.000000 robin_sd_upload-0.2.9/robin_sd_upload/supportive_scripts/create_folder.py
+-rw-rw-rw-   0 root         (0) root         (0)      875 2023-02-15 15:33:08.000000 robin_sd_upload-0.2.9/robin_sd_upload/supportive_scripts/create_zip.py
+-rw-rw-rw-   0 root         (0) root         (0)     2261 2023-02-15 15:33:08.000000 robin_sd_upload-0.2.9/robin_sd_upload/supportive_scripts/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)      567 2023-02-15 15:33:08.000000 robin_sd_upload-0.2.9/robin_sd_upload/supportive_scripts/remove_zip.py
+-rw-rw-rw-   0 root         (0) root         (0)     1574 2023-02-15 15:33:08.000000 robin_sd_upload-0.2.9/robin_sd_upload/supportive_scripts/sudo_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     1389 2023-02-15 15:33:08.000000 robin_sd_upload-0.2.9/robin_sd_upload/supportive_scripts/validate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1229 2023-02-15 15:33:08.000000 robin_sd_upload-0.2.9/robin_sd_upload/supportive_scripts/version_checker.py
+-rw-rw-rw-   0 root         (0) root         (0)     2827 2023-02-15 15:33:08.000000 robin_sd_upload-0.2.9/robin_sd_upload/supportive_scripts/yaml_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 15:33:30.000000 robin_sd_upload-0.2.9/robin_sd_upload.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      633 2023-02-15 15:33:30.000000 robin_sd_upload-0.2.9/robin_sd_upload.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1157 2023-02-15 15:33:30.000000 robin_sd_upload-0.2.9/robin_sd_upload.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-15 15:33:30.000000 robin_sd_upload-0.2.9/robin_sd_upload.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-02-15 15:33:30.000000 robin_sd_upload-0.2.9/robin_sd_upload.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-02-15 15:33:30.000000 robin_sd_upload-0.2.9/robin_sd_upload.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-02-15 15:33:30.000000 robin_sd_upload-0.2.9/robin_sd_upload.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-02-15 15:33:30.000000 robin_sd_upload-0.2.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2023-02-15 15:33:08.000000 robin_sd_upload-0.2.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 15:33:30.000000 robin_sd_upload-0.2.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-02-15 15:33:08.000000 robin_sd_upload-0.2.9/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-02-15 15:33:08.000000 robin_sd_upload-0.2.9/tests/test.py
```

### Comparing `robin_sd_upload-0.2.8/PKG-INFO` & `robin_sd_upload-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robin_sd_upload
-Version: 0.2.8
+Version: 0.2.9
 Summary: Package to upload files to the Robin Radar API
 Home-page: https://bitbucket.org/robin-radar-systems/sd-api-upload-pip-package.git
 Author: Robin Radar Systems
 Author-email: it-team@robinradar.com
 License: MIT
 Description: # robin-sd-upload
```

### Comparing `robin_sd_upload-0.2.8/robin_sd_upload/api_interaction/get_bearer_token.py` & `robin_sd_upload-0.2.9/robin_sd_upload/api_interaction/get_bearer_token.py`

 * *Files identical despite different names*

### Comparing `robin_sd_upload-0.2.8/robin_sd_upload/api_interaction/push_software.py` & `robin_sd_upload-0.2.9/robin_sd_upload/api_interaction/push_software.py`

 * *Files identical despite different names*

### Comparing `robin_sd_upload-0.2.8/robin_sd_upload/slack_interaction/slack_handler.py` & `robin_sd_upload-0.2.9/robin_sd_upload/slack_interaction/slack_handler.py`

 * *Files identical despite different names*

### Comparing `robin_sd_upload-0.2.8/robin_sd_upload/supportive_scripts/arg_parse.py` & `robin_sd_upload-0.2.9/robin_sd_upload/supportive_scripts/arg_parse.py`

 * *Files identical despite different names*

### Comparing `robin_sd_upload-0.2.8/robin_sd_upload/supportive_scripts/check_upload_file.py` & `robin_sd_upload-0.2.9/robin_sd_upload/supportive_scripts/check_upload_file.py`

 * *Files identical despite different names*

### Comparing `robin_sd_upload-0.2.8/robin_sd_upload/supportive_scripts/create_folder.py` & `robin_sd_upload-0.2.9/robin_sd_upload/supportive_scripts/create_folder.py`

 * *Files identical despite different names*

### Comparing `robin_sd_upload-0.2.8/robin_sd_upload/supportive_scripts/create_zip.py` & `robin_sd_upload-0.2.9/robin_sd_upload/supportive_scripts/create_zip.py`

 * *Files identical despite different names*

### Comparing `robin_sd_upload-0.2.8/robin_sd_upload/supportive_scripts/logger.py` & `robin_sd_upload-0.2.9/robin_sd_upload/supportive_scripts/logger.py`

 * *Files identical despite different names*

### Comparing `robin_sd_upload-0.2.8/robin_sd_upload/supportive_scripts/remove_zip.py` & `robin_sd_upload-0.2.9/robin_sd_upload/supportive_scripts/remove_zip.py`

 * *Files identical despite different names*

### Comparing `robin_sd_upload-0.2.8/robin_sd_upload/supportive_scripts/sudo_file.py` & `robin_sd_upload-0.2.9/robin_sd_upload/supportive_scripts/sudo_file.py`

 * *Files identical despite different names*

### Comparing `robin_sd_upload-0.2.8/robin_sd_upload/supportive_scripts/validate.py` & `robin_sd_upload-0.2.9/robin_sd_upload/supportive_scripts/validate.py`

 * *Files identical despite different names*

### Comparing `robin_sd_upload-0.2.8/robin_sd_upload/supportive_scripts/version_checker.py` & `robin_sd_upload-0.2.9/robin_sd_upload/supportive_scripts/version_checker.py`

 * *Files identical despite different names*

### Comparing `robin_sd_upload-0.2.8/robin_sd_upload/supportive_scripts/yaml_parser.py` & `robin_sd_upload-0.2.9/robin_sd_upload/supportive_scripts/yaml_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 
     # Set variable config_file to the first config file found
     for cfg_file in config_files:
         if os.path.isfile(cfg_file) and check_file_format(cfg_file):
             with open(cfg_file, 'r') as config_file:
                 config = yaml.safe_load(config_file)
                 file = cfg_file
+                print(f"Config file found in {cfg_file} directory.")
                 break
         else:
             print(f"Config file not found in {cfg_file} directory.")
             print(f"Checking next directory...")
     if not config:
         admin_interface = "https://software-api-admin.robinradar.systems"
         doc_pages = "https://robinradar.atlassian.net/wiki/spaces/DEV/pages/284033095/Software+Deployment+API"
```

### Comparing `robin_sd_upload-0.2.8/robin_sd_upload.egg-info/PKG-INFO` & `robin_sd_upload-0.2.9/robin_sd_upload.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robin-sd-upload
-Version: 0.2.8
+Version: 0.2.9
 Summary: Package to upload files to the Robin Radar API
 Home-page: https://bitbucket.org/robin-radar-systems/sd-api-upload-pip-package.git
 Author: Robin Radar Systems
 Author-email: it-team@robinradar.com
 License: MIT
 Description: # robin-sd-upload
```

### Comparing `robin_sd_upload-0.2.8/robin_sd_upload.egg-info/SOURCES.txt` & `robin_sd_upload-0.2.9/robin_sd_upload.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robin_sd_upload-0.2.8/setup.py` & `robin_sd_upload-0.2.9/setup.py`

 * *Files identical despite different names*

