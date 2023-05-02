# Comparing `tmp/aisdc-1.0.2.tar.gz` & `tmp/aisdc-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aisdc-1.0.2.tar", last modified: Mon Feb 27 14:43:39 2023, max compression
+gzip compressed data, was "aisdc-1.0.3.tar", last modified: Tue May  2 16:13:23 2023, max compression
```

## Comparing `aisdc-1.0.2.tar` & `aisdc-1.0.3.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-02-27 14:43:39.757035 aisdc-1.0.2/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1063 2022-12-04 22:46:52.000000 aisdc-1.0.2/LICENSE
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5041 2023-02-27 14:43:39.757035 aisdc-1.0.2/PKG-INFO
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3969 2023-02-27 14:08:40.000000 aisdc-1.0.2/README.md
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-02-27 14:43:39.749035 aisdc-1.0.2/aisdc/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2022-12-04 22:46:52.000000 aisdc-1.0.2/aisdc/__init__.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-02-27 14:43:39.753035 aisdc-1.0.2/aisdc/attacks/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2022-12-04 22:46:52.000000 aisdc-1.0.2/aisdc/attacks/__init__.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      395 2022-12-04 22:46:52.000000 aisdc-1.0.2/aisdc/attacks/attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    23679 2023-02-27 14:04:11.000000 aisdc-1.0.2/aisdc/attacks/attribute_attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2167 2022-12-12 15:48:01.000000 aisdc-1.0.2/aisdc/attacks/dataset.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    22222 2023-02-27 14:04:11.000000 aisdc-1.0.2/aisdc/attacks/likelihood_attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7539 2022-12-12 15:48:38.000000 aisdc-1.0.2/aisdc/attacks/metrics.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3114 2022-12-12 15:48:53.000000 aisdc-1.0.2/aisdc/attacks/mia_extremecase.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11910 2023-02-27 13:04:16.000000 aisdc-1.0.2/aisdc/attacks/report.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    21836 2023-02-27 13:04:16.000000 aisdc-1.0.2/aisdc/attacks/worst_case_attack.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-02-27 14:43:39.753035 aisdc-1.0.2/aisdc/preprocessing/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2022-12-04 22:46:52.000000 aisdc-1.0.2/aisdc/preprocessing/__init__.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    23420 2023-02-27 14:04:11.000000 aisdc-1.0.2/aisdc/preprocessing/loaders.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-02-27 14:43:39.753035 aisdc-1.0.2/aisdc/safemodel/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       61 2022-12-04 22:46:52.000000 aisdc-1.0.2/aisdc/safemodel/__init__.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-02-27 14:43:39.753035 aisdc-1.0.2/aisdc/safemodel/classifiers/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      310 2022-12-04 22:46:52.000000 aisdc-1.0.2/aisdc/safemodel/classifiers/__init__.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7491 2022-12-04 22:46:52.000000 aisdc-1.0.2/aisdc/safemodel/classifiers/dp_svc.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7595 2023-02-27 14:04:11.000000 aisdc-1.0.2/aisdc/safemodel/classifiers/new_model_template.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     7149 2022-12-04 22:46:52.000000 aisdc-1.0.2/aisdc/safemodel/classifiers/safedecisiontreeclassifier.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    20922 2023-02-27 14:04:11.000000 aisdc-1.0.2/aisdc/safemodel/classifiers/safekeras.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6287 2023-02-27 14:04:11.000000 aisdc-1.0.2/aisdc/safemodel/classifiers/saferandomforestclassifier.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1912 2022-12-04 22:46:52.000000 aisdc-1.0.2/aisdc/safemodel/classifiers/safesvc.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1212 2022-12-04 22:46:52.000000 aisdc-1.0.2/aisdc/safemodel/classifiers/safetf.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    10821 2022-12-04 22:46:52.000000 aisdc-1.0.2/aisdc/safemodel/reporting.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4984 2022-12-04 22:46:52.000000 aisdc-1.0.2/aisdc/safemodel/rules.json
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    29904 2023-02-27 14:04:11.000000 aisdc-1.0.2/aisdc/safemodel/safemodel.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-02-27 14:43:39.749035 aisdc-1.0.2/aisdc.egg-info/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5041 2023-02-27 14:43:39.000000 aisdc-1.0.2/aisdc.egg-info/PKG-INFO
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1421 2023-02-27 14:43:39.000000 aisdc-1.0.2/aisdc.egg-info/SOURCES.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        1 2023-02-27 14:43:39.000000 aisdc-1.0.2/aisdc.egg-info/dependency_links.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      170 2023-02-27 14:43:39.000000 aisdc-1.0.2/aisdc.egg-info/requires.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        6 2023-02-27 14:43:39.000000 aisdc-1.0.2/aisdc.egg-info/top_level.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       38 2023-02-27 14:43:39.757035 aisdc-1.0.2/setup.cfg
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1857 2023-02-27 14:37:53.000000 aisdc-1.0.2/setup.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-02-27 14:43:39.753035 aisdc-1.0.2/tests/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2209 2022-12-04 22:46:52.000000 aisdc-1.0.2/tests/test_attacks.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     2958 2023-02-27 14:04:11.000000 aisdc-1.0.2/tests/test_attacks_dataset.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     9109 2023-02-27 14:04:11.000000 aisdc-1.0.2/tests/test_attacks_via_safemodel.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3390 2022-12-04 22:46:52.000000 aisdc-1.0.2/tests/test_attribute_inference_attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1470 2022-12-04 22:46:52.000000 aisdc-1.0.2/tests/test_data_interface.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3661 2022-12-04 22:46:52.000000 aisdc-1.0.2/tests/test_lira_attack.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     6246 2022-12-04 22:46:52.000000 aisdc-1.0.2/tests/test_loaders.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     3991 2022-12-04 22:46:52.000000 aisdc-1.0.2/tests/test_metrics.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     8366 2022-12-04 22:46:52.000000 aisdc-1.0.2/tests/test_safedecisiontreeclassifier.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    27082 2022-12-04 22:46:52.000000 aisdc-1.0.2/tests/test_safekeras2.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    15852 2022-12-04 22:46:52.000000 aisdc-1.0.2/tests/test_safemodel.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11770 2022-12-04 22:46:52.000000 aisdc-1.0.2/tests/test_saferandomforestclassifier.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     4891 2022-12-04 22:46:52.000000 aisdc-1.0.2/tests/test_safesvc.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      365 2022-12-04 22:46:52.000000 aisdc-1.0.2/tests/test_safetf.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    11146 2023-02-27 13:04:16.000000 aisdc-1.0.2/tests/test_worst_case_attack.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-05-02 16:13:23.828295 aisdc-1.0.3/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1063 2022-12-04 22:46:52.000000 aisdc-1.0.3/LICENSE
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4999 2023-05-02 16:13:23.828295 aisdc-1.0.3/PKG-INFO
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3927 2023-05-02 15:24:23.000000 aisdc-1.0.3/README.md
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-05-02 16:13:23.824295 aisdc-1.0.3/aisdc/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-04-26 12:57:02.000000 aisdc-1.0.3/aisdc/__init__.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-05-02 16:13:23.824295 aisdc-1.0.3/aisdc/attacks/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-04-26 12:57:02.000000 aisdc-1.0.3/aisdc/attacks/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      395 2023-04-26 12:57:02.000000 aisdc-1.0.3/aisdc/attacks/attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    23679 2023-04-26 12:57:02.000000 aisdc-1.0.3/aisdc/attacks/attribute_attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2167 2023-05-02 10:18:16.000000 aisdc-1.0.3/aisdc/attacks/dataset.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    22027 2023-05-02 15:16:25.000000 aisdc-1.0.3/aisdc/attacks/likelihood_attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    12090 2023-05-02 15:16:25.000000 aisdc-1.0.3/aisdc/attacks/report.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    22656 2023-05-02 15:16:25.000000 aisdc-1.0.3/aisdc/attacks/worst_case_attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    10042 2023-05-02 15:24:23.000000 aisdc-1.0.3/aisdc/generate_report.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11752 2023-05-02 15:32:15.000000 aisdc-1.0.3/aisdc/metrics.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-05-02 16:13:23.824295 aisdc-1.0.3/aisdc/preprocessing/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2023-04-26 12:57:02.000000 aisdc-1.0.3/aisdc/preprocessing/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    23420 2023-04-26 12:57:02.000000 aisdc-1.0.3/aisdc/preprocessing/loaders.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-05-02 16:13:23.828295 aisdc-1.0.3/aisdc/safemodel/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       61 2023-04-26 12:57:02.000000 aisdc-1.0.3/aisdc/safemodel/__init__.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-05-02 16:13:23.828295 aisdc-1.0.3/aisdc/safemodel/classifiers/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      310 2023-04-26 12:57:02.000000 aisdc-1.0.3/aisdc/safemodel/classifiers/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7491 2023-04-26 12:57:02.000000 aisdc-1.0.3/aisdc/safemodel/classifiers/dp_svc.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7595 2023-04-26 12:57:02.000000 aisdc-1.0.3/aisdc/safemodel/classifiers/new_model_template.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     7149 2023-04-26 12:57:02.000000 aisdc-1.0.3/aisdc/safemodel/classifiers/safedecisiontreeclassifier.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    20882 2023-05-02 15:16:25.000000 aisdc-1.0.3/aisdc/safemodel/classifiers/safekeras.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6287 2023-04-26 12:57:02.000000 aisdc-1.0.3/aisdc/safemodel/classifiers/saferandomforestclassifier.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1912 2023-04-26 12:57:02.000000 aisdc-1.0.3/aisdc/safemodel/classifiers/safesvc.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1212 2023-04-26 12:57:02.000000 aisdc-1.0.3/aisdc/safemodel/classifiers/safetf.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    10821 2023-04-26 12:57:02.000000 aisdc-1.0.3/aisdc/safemodel/reporting.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4984 2023-04-26 12:57:02.000000 aisdc-1.0.3/aisdc/safemodel/rules.json
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    30719 2023-05-02 15:16:25.000000 aisdc-1.0.3/aisdc/safemodel/safemodel.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-05-02 16:13:23.824295 aisdc-1.0.3/aisdc.egg-info/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4999 2023-05-02 16:13:23.000000 aisdc-1.0.3/aisdc.egg-info/PKG-INFO
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1435 2023-05-02 16:13:23.000000 aisdc-1.0.3/aisdc.egg-info/SOURCES.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        1 2023-05-02 16:13:23.000000 aisdc-1.0.3/aisdc.egg-info/dependency_links.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      170 2023-05-02 16:13:23.000000 aisdc-1.0.3/aisdc.egg-info/requires.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        6 2023-05-02 16:13:23.000000 aisdc-1.0.3/aisdc.egg-info/top_level.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       38 2023-05-02 16:13:23.828295 aisdc-1.0.3/setup.cfg
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1857 2023-05-02 15:24:23.000000 aisdc-1.0.3/setup.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-05-02 16:13:23.828295 aisdc-1.0.3/tests/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1598 2023-05-02 15:16:25.000000 aisdc-1.0.3/tests/test_attacks.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2958 2023-04-26 12:57:02.000000 aisdc-1.0.3/tests/test_attacks_dataset.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     9109 2023-04-26 12:57:02.000000 aisdc-1.0.3/tests/test_attacks_via_safemodel.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3390 2023-04-26 12:57:02.000000 aisdc-1.0.3/tests/test_attribute_inference_attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1470 2023-04-26 12:57:02.000000 aisdc-1.0.3/tests/test_data_interface.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6065 2023-05-02 15:24:23.000000 aisdc-1.0.3/tests/test_generate_report.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3661 2023-04-26 12:57:02.000000 aisdc-1.0.3/tests/test_lira_attack.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6246 2023-04-26 12:57:02.000000 aisdc-1.0.3/tests/test_loaders.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     6804 2023-05-02 15:16:25.000000 aisdc-1.0.3/tests/test_metrics.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     8366 2023-04-26 12:57:02.000000 aisdc-1.0.3/tests/test_safedecisiontreeclassifier.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    27082 2023-04-26 12:57:02.000000 aisdc-1.0.3/tests/test_safekeras2.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    15852 2023-04-26 12:57:02.000000 aisdc-1.0.3/tests/test_safemodel.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11770 2023-04-26 12:57:02.000000 aisdc-1.0.3/tests/test_saferandomforestclassifier.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     4891 2023-04-26 12:57:02.000000 aisdc-1.0.3/tests/test_safesvc.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      365 2023-04-26 12:57:02.000000 aisdc-1.0.3/tests/test_safetf.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11146 2023-05-02 10:18:16.000000 aisdc-1.0.3/tests/test_worst_case_attack.py
```

### Comparing `aisdc-1.0.2/LICENSE` & `aisdc-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.2/PKG-INFO` & `aisdc-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aisdc
-Version: 1.0.2
+Version: 1.0.3
 Summary: Tools for the statistical disclosure control of machine learning models
 Home-page: https://github.com/AI-SDC/AI-SDC
 Maintainer: Jim Smith
 Maintainer-email: james.smith@uwe.ac.uk
 License: MIT
 Keywords: data-privacy,data-protection,machine-learning,privacy,privacy-tools,statistical-disclosure-control
 Classifier: Development Status :: 5 - Production/Stable
@@ -57,15 +57,15 @@
 ## Quick Start
 
 ### Development
 
 Clone the repository and install the dependencies (safest in a virtual env):
 
 ```
-$ git clone --recurse-submodules https://github.com/AI-SDC/AI-SDC.git
+$ git clone https://github.com/AI-SDC/AI-SDC.git
 $ cd AI-SDC
 $ pip install -r requirements.txt
 ```
 
 Then run the tests:
 
 ```
@@ -96,15 +96,15 @@
 ```
 
 Or start up `jupyter notebook` and run an example.
 
 Alternatively, you can clone the repo and install:
 
 ```
-$ git clone --recurse-submodules https://github.com/AI-SDC/AI-SDC.git
+$ git clone https://github.com/AI-SDC/AI-SDC.git
 $ cd AI-SDC
 $ pip install .
 ```
 
 ---
 
 This work was funded by UK Research and Innovation Grant Number MC_PC_21033 as part of Phase 1 of the DARE UK (Data and Analytics Research Environments UK) programme (https://dareuk.org.uk/), delivered in partnership with HDR UK and ADRUK. The specific project was Guidelines and Resources for AI Model Access from TrusTEd Research environments (GRAIMATTER).­ This project has also been supported by MRC and EPSRC [grant number MR/S010351/1]: PICTURES.
```

### Comparing `aisdc-1.0.2/README.md` & `aisdc-1.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 ## Quick Start
 
 ### Development
 
 Clone the repository and install the dependencies (safest in a virtual env):
 
 ```
-$ git clone --recurse-submodules https://github.com/AI-SDC/AI-SDC.git
+$ git clone https://github.com/AI-SDC/AI-SDC.git
 $ cd AI-SDC
 $ pip install -r requirements.txt
 ```
 
 Then run the tests:
 
 ```
@@ -71,15 +71,15 @@
 ```
 
 Or start up `jupyter notebook` and run an example.
 
 Alternatively, you can clone the repo and install:
 
 ```
-$ git clone --recurse-submodules https://github.com/AI-SDC/AI-SDC.git
+$ git clone https://github.com/AI-SDC/AI-SDC.git
 $ cd AI-SDC
 $ pip install .
 ```
 
 ---
 
 This work was funded by UK Research and Innovation Grant Number MC_PC_21033 as part of Phase 1 of the DARE UK (Data and Analytics Research Environments UK) programme (https://dareuk.org.uk/), delivered in partnership with HDR UK and ADRUK. The specific project was Guidelines and Resources for AI Model Access from TrusTEd Research environments (GRAIMATTER).­ This project has also been supported by MRC and EPSRC [grant number MR/S010351/1]: PICTURES.
```

### Comparing `aisdc-1.0.2/aisdc/attacks/attribute_attack.py` & `aisdc-1.0.3/aisdc/attacks/attribute_attack.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.2/aisdc/attacks/dataset.py` & `aisdc-1.0.3/aisdc/attacks/dataset.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.2/aisdc/attacks/likelihood_attack.py` & `aisdc-1.0.3/aisdc/attacks/likelihood_attack.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 import numpy as np
 import sklearn
 from scipy.stats import norm
 from sklearn.datasets import load_breast_cancer
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.model_selection import train_test_split
 
-from aisdc.attacks import metrics, report
+from aisdc import metrics
+from aisdc.attacks import report
 from aisdc.attacks.attack import Attack
 from aisdc.attacks.dataset import Data
 
 logging.basicConfig(level=logging.INFO)
 
 N_SHADOW_MODELS = 100  # Number of shadow models that should be trained
 EPS = 1e-16  # Used to avoid numerical issues in logit function
@@ -164,33 +165,24 @@
         dataset.y_test = np.array(y_test_new, int)
         print(
             f"new ytest has values and counts: {np.unique(dataset.y_test,return_counts=True)}"
         )
 
         return dataset
 
-    def run_scenario_from_preds(  # pylint: disable = too-many-statements
+    def run_scenario_from_preds(  # pylint: disable = too-many-statements, too-many-arguments, too-many-locals
         self,
         shadow_clf: sklearn.base.BaseEstimator,
         X_target_train: Iterable[float],
         y_target_train: Iterable[float],
         target_train_preds: Iterable[float],
         X_shadow_train: Iterable[float],
         y_shadow_train: Iterable[float],
         shadow_train_preds: Iterable[float],
     ) -> tuple[np.ndarray, np.ndarray, sklearn.base.BaseEstimator]:
-        # def run_scenario_from_preds( # pylint: disable = too-many-locals, too-many-arguments
-        #     shadow_clf,
-        #     X_target_train: Iterable[float],
-        #     y_target_train: Iterable[float],
-        #     target_train_preds: Iterable[float],
-        #     X_shadow_train: Iterable[float],
-        #     y_shadow_train: Iterable[float],
-        #     shadow_train_preds: Iterable[float],
-
         """Implements the likelihood test, using the "offline" version
         See p.6 (top of second column) for details
 
         Parameters
         ----------
         shadow_clf: sklearn.Model
             An sklearn classifier that will be trained to form the shadow model.
@@ -329,17 +321,21 @@
             var_null = max(null_scores.var(), EPS)  # var can be zeros in some cases
             prob = norm.cdf(true_score, loc=mean_null, scale=np.sqrt(var_null))
             mia_scores.append([1 - prob, prob])
             mia_labels.append(0)
 
         mia_clf = DummyClassifier()
         logger.info("Finished scenario")
-        self.attack_metrics = [
-            metrics.get_metrics(mia_clf, np.array(mia_scores), np.array(mia_labels))
-        ]
+
+        mia_scores = np.array(mia_scores)
+        mia_labels = np.array(mia_labels)
+        y_pred_proba, y_test = metrics.get_probabilities(
+            mia_clf, mia_scores, mia_labels, permute_rows=True
+        )
+        self.attack_metrics = [metrics.get_metrics(y_pred_proba, y_test)]
 
     def example(self) -> None:  # pylint: disable = too-many-locals
         """Runs an example attack using data from sklearn
 
         Generates example data, trains a classifier and tuns the attack
         """
         X, y = load_breast_cancer(return_X_y=True, as_frame=False)
```

### Comparing `aisdc-1.0.2/aisdc/attacks/report.py` & `aisdc-1.0.3/aisdc/attacks/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,17 +215,23 @@
     Returns
     -------
 
     pdf: fpdf.FPDF
         fpdf document object
 
     """
-
-    dummy_metrics = attack_output["dummy_attack_metrics"]
-    mia_metrics = attack_output["attack_metrics"]
+    # dummy_metrics = attack_output["dummy_attack_metrics"]
+    dummy_metrics = []
+    mia_metrics = [
+        v
+        for _, v in attack_output["attack_experiment_logger"][
+            "attack_instance_logger"
+        ].items()
+    ]
+    # mia_metrics = attack_output["attack_metrics"]
     metadata = attack_output["metadata"]
     if dummy_metrics is None or len(dummy_metrics) == 0:
         do_dummy = False
     else:
         do_dummy = True
 
     _roc_plot(mia_metrics, dummy_metrics, "log_roc.png")
```

### Comparing `aisdc-1.0.2/aisdc/attacks/worst_case_attack.py` & `aisdc-1.0.3/aisdc/attacks/worst_case_attack.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,27 @@
 Runs a worst case attack based upon predictive probabilities stored in two .csv files
 """
 
 from __future__ import annotations
 
 import argparse
 import logging
+import uuid
 from collections.abc import Hashable
+from datetime import datetime
 from typing import Any
 
 import numpy as np
 import sklearn
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.metrics import confusion_matrix
 from sklearn.model_selection import train_test_split
 
-from aisdc.attacks import metrics, report
+from aisdc import metrics
+from aisdc.attacks import report
 from aisdc.attacks.attack import Attack
 from aisdc.attacks.dataset import Data
 
 logging.basicConfig(level=logging.INFO)
 
 P_THRESH = 0.05
 
@@ -143,17 +146,17 @@
         self.attack_metrics = self.run_attack_reps(
             train_preds,
             test_preds,
             train_correct=train_correct,
             test_correct=test_correct,
         )
 
+        self.dummy_attack_metrics = []
         if self.args.n_dummy_reps > 0:
             logger.info("Running dummy attack reps")
-            self.dummy_attack_metrics = []
             n_train_rows = len(train_preds)
             n_test_rows = len(test_preds)
             for _ in range(self.args.n_dummy_reps):
                 d_train_preds, d_test_preds = self.generate_arrays(
                     n_train_rows, n_test_rows, self.args.train_beta, self.args.test_beta
                 )
                 temp_metrics = self.run_attack_reps(d_train_preds, d_test_preds)
@@ -223,19 +226,20 @@
             mi_train_x, mi_test_x, mi_train_y, mi_test_y = train_test_split(
                 mi_x, mi_y, test_size=self.args.test_prop, stratify=mi_y
             )
             attack_classifier = self.args.mia_attack_model(
                 **self.args.mia_attack_model_hyp
             )
             attack_classifier.fit(mi_train_x, mi_train_y)
-
-            mia_metrics.append(
-                metrics.get_metrics(attack_classifier, mi_test_x, mi_test_y)
+            y_pred_proba, y_test = metrics.get_probabilities(
+                attack_classifier, mi_test_x, mi_test_y, permute_rows=True
             )
 
+            mia_metrics.append(metrics.get_metrics(y_pred_proba, y_test))
+
             if self.args.include_model_correct_feature and train_correct is not None:
                 # Compute the Yeom TPR and FPR
                 yeom_preds = mi_test_x[:, -1]
                 tn, fp, fn, tp = confusion_matrix(mi_test_y, yeom_preds).ravel()
                 mia_metrics[-1]["yeom_tpr"] = tp / (tp + fn)
                 mia_metrics[-1]["yeom_fpr"] = fp / (fp + tn)
                 mia_metrics[-1]["yeom_advantage"] = (
@@ -264,14 +268,17 @@
         auc_p_vals = [
             metrics.auc_p_val(
                 m["AUC"], m["n_pos_test_examples"], m["n_neg_test_examples"]
             )[0]
             for m in attack_metrics
         ]
 
+        if len(attack_metrics) == 0:
+            return global_metrics
+
         m = attack_metrics[0]
         _, auc_std = metrics.auc_p_val(
             0.5, m["n_pos_test_examples"], m["n_neg_test_examples"]
         )
 
         global_metrics[
             "null_auc_3sd_range"
@@ -420,29 +427,44 @@
 
         # Global metrics
         self.metadata["global_metrics"] = self._get_global_metrics(self.attack_metrics)
         self.metadata["baseline_global_metrics"] = self._get_global_metrics(
             self.dummy_attack_metrics
         )
 
+    def _get_attack_metrics_instances(self) -> dict:
+        """Constructs the metadata object, after attacks"""
+        attack_metrics_experiment = {}
+        attack_metrics_instances = {}
+
+        for rep, _ in enumerate(self.attack_metrics):
+            attack_metrics_instances["instance_" + str(rep + 1)] = self.attack_metrics[
+                rep
+            ]
+
+        attack_metrics_experiment["attack_instance_logger"] = attack_metrics_instances
+        return attack_metrics_experiment
+
     def make_report(self) -> dict:
         """Creates output dictionary structure"""
         output = {}
-        output["attack_metrics"] = self.attack_metrics
-        output["dummy_attack_metrics"] = self.dummy_attack_metrics
+        output["log_id"] = str(uuid.uuid4())
+        output["log_time"] = datetime.now().strftime("%d/%m/%Y %H:%M:%S")
+
         self._construct_metadata()
         output["metadata"] = self.metadata
+
+        output["attack_experiment_logger"] = self._get_attack_metrics_instances()
+
         if self.args.report_name is not None:
             json_report = report.create_json_report(output)
             with open(f"{self.args.report_name}.json", "w", encoding="utf-8") as f:
                 f.write(json_report)
-
-            pdf = report.create_mia_report(output)
-            pdf.output(f"{self.args.report_name}.pdf", "F")
-
+            pdf_report = report.create_mia_report(output)
+            pdf_report.output(f"{self.args.report_name}.pdf", "F")
         return output
 
 
 def _make_dummy_data(args):
     """Initialise class and run dummy data creation"""
     wc_args = WorstCaseAttackArgs(**args.__dict__)
     wc_args.set_param("in_sample_filename", "train_preds.csv")
```

### Comparing `aisdc-1.0.2/aisdc/preprocessing/loaders.py` & `aisdc-1.0.3/aisdc/preprocessing/loaders.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.2/aisdc/safemodel/classifiers/dp_svc.py` & `aisdc-1.0.3/aisdc/safemodel/classifiers/dp_svc.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.2/aisdc/safemodel/classifiers/new_model_template.py` & `aisdc-1.0.3/aisdc/safemodel/classifiers/new_model_template.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.2/aisdc/safemodel/classifiers/safedecisiontreeclassifier.py` & `aisdc-1.0.3/aisdc/safemodel/classifiers/safedecisiontreeclassifier.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.2/aisdc/safemodel/classifiers/safekeras.py` & `aisdc-1.0.3/aisdc/safemodel/classifiers/safekeras.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import numpy as np
 
 # tensorflow imports
 import tensorflow as tf
 import tensorflow_privacy as tfp
 from dictdiffer import diff
 from tensorflow.keras import Model as KerasModel  # pylint: disable = import-error
-from tensorflow_privacy.privacy.analysis import compute_dp_sgd_privacy
+from tensorflow_privacy import compute_dp_sgd_privacy
 
 # safemodel superclass
 from ..reporting import get_reporting_string
 from ..safemodel import SafeModel
 
 # suppress numerous deprecatino warnings
 # shut tensorflow up
@@ -290,15 +290,15 @@
         super().preliminary_check(apply_constraints=True, verbose=True)
 
     def dp_epsilon_met(
         self, num_examples: int, batch_size: int = 0, epochs: int = 0
     ) -> Tuple[bool, str]:
         """Checks if epsilon is sufficient for Differential Privacy
         Provides feedback to user if epsilon is not sufficient"""
-        privacy = compute_dp_sgd_privacy.compute_dp_sgd_privacy(
+        privacy = compute_dp_sgd_privacy(
             n=num_examples,
             batch_size=batch_size,
             noise_multiplier=self.noise_multiplier,
             epochs=epochs,
             delta=self.delta,
         )
         ok = privacy[0] < self.min_epsilon
```

### Comparing `aisdc-1.0.2/aisdc/safemodel/classifiers/saferandomforestclassifier.py` & `aisdc-1.0.3/aisdc/safemodel/classifiers/saferandomforestclassifier.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.2/aisdc/safemodel/classifiers/safesvc.py` & `aisdc-1.0.3/aisdc/safemodel/classifiers/safesvc.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.2/aisdc/safemodel/classifiers/safetf.py` & `aisdc-1.0.3/aisdc/safemodel/classifiers/safetf.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.2/aisdc/safemodel/reporting.py` & `aisdc-1.0.3/aisdc/safemodel/reporting.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.2/aisdc/safemodel/rules.json` & `aisdc-1.0.3/aisdc/safemodel/rules.json`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.2/aisdc/safemodel/safemodel.py` & `aisdc-1.0.3/aisdc/safemodel/safemodel.py`

 * *Files 0% similar despite different names*

```diff
@@ -778,18 +778,37 @@
                         attack_name,
                         f"{os.path.splitext(filename)[0]}_{attack_name}_res",
                     )
 
             now = datetime.datetime.now()
             output["timestamp"] = str(now.strftime("%Y-%m-%d %H:%M:%S"))
 
-            json_str = json.dumps(output, indent=4, cls=report.NumpyArrayEncoder)
             outputfilename = self.researcher + "_checkfile.json"
-            with open(outputfilename, "a", encoding="utf-8") as file:
-                file.write(json_str)
+            data = [output]
+            # load existing results
+            if os.path.isfile(outputfilename):
+                with open(outputfilename, newline="", encoding="utf-8") as file:
+                    try:
+                        data = json.load(file)
+                        data.append(output)
+                    except json.decoder.JSONDecodeError:  # pragma: no cover
+                        logger.warning(
+                            "File %s could not be loaded - overwiting", outputfilename
+                        )
+
+            # write to disk
+            try:
+                with open(outputfilename, "w", newline="", encoding="utf-8") as file:
+                    json.dump(data, file, indent=4, cls=report.NumpyArrayEncoder)
+            except TypeError:  # pragma: no cover
+                logger.warning(
+                    "Error: safemodel could not write non-serialisable "
+                    " outputs to file %s",
+                    outputfilename,
+                )
 
     def run_attack(
         self,
         data_obj: dataset.Data = None,
         attack_name: str = "worst_case",
         filename: str = "undefined",
     ) -> dict:
```

### Comparing `aisdc-1.0.2/aisdc.egg-info/PKG-INFO` & `aisdc-1.0.3/aisdc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aisdc
-Version: 1.0.2
+Version: 1.0.3
 Summary: Tools for the statistical disclosure control of machine learning models
 Home-page: https://github.com/AI-SDC/AI-SDC
 Maintainer: Jim Smith
 Maintainer-email: james.smith@uwe.ac.uk
 License: MIT
 Keywords: data-privacy,data-protection,machine-learning,privacy,privacy-tools,statistical-disclosure-control
 Classifier: Development Status :: 5 - Production/Stable
@@ -57,15 +57,15 @@
 ## Quick Start
 
 ### Development
 
 Clone the repository and install the dependencies (safest in a virtual env):
 
 ```
-$ git clone --recurse-submodules https://github.com/AI-SDC/AI-SDC.git
+$ git clone https://github.com/AI-SDC/AI-SDC.git
 $ cd AI-SDC
 $ pip install -r requirements.txt
 ```
 
 Then run the tests:
 
 ```
@@ -96,15 +96,15 @@
 ```
 
 Or start up `jupyter notebook` and run an example.
 
 Alternatively, you can clone the repo and install:
 
 ```
-$ git clone --recurse-submodules https://github.com/AI-SDC/AI-SDC.git
+$ git clone https://github.com/AI-SDC/AI-SDC.git
 $ cd AI-SDC
 $ pip install .
 ```
 
 ---
 
 This work was funded by UK Research and Innovation Grant Number MC_PC_21033 as part of Phase 1 of the DARE UK (Data and Analytics Research Environments UK) programme (https://dareuk.org.uk/), delivered in partnership with HDR UK and ADRUK. The specific project was Guidelines and Resources for AI Model Access from TrusTEd Research environments (GRAIMATTER).­ This project has also been supported by MRC and EPSRC [grant number MR/S010351/1]: PICTURES.
```

### Comparing `aisdc-1.0.2/aisdc.egg-info/SOURCES.txt` & `aisdc-1.0.3/aisdc.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 LICENSE
 README.md
 setup.py
 aisdc/__init__.py
+aisdc/generate_report.py
+aisdc/metrics.py
 aisdc.egg-info/PKG-INFO
 aisdc.egg-info/SOURCES.txt
 aisdc.egg-info/dependency_links.txt
 aisdc.egg-info/requires.txt
 aisdc.egg-info/top_level.txt
 aisdc/attacks/__init__.py
 aisdc/attacks/attack.py
 aisdc/attacks/attribute_attack.py
 aisdc/attacks/dataset.py
 aisdc/attacks/likelihood_attack.py
-aisdc/attacks/metrics.py
-aisdc/attacks/mia_extremecase.py
 aisdc/attacks/report.py
 aisdc/attacks/worst_case_attack.py
 aisdc/preprocessing/__init__.py
 aisdc/preprocessing/loaders.py
 aisdc/safemodel/__init__.py
 aisdc/safemodel/reporting.py
 aisdc/safemodel/rules.json
@@ -31,14 +31,15 @@
 aisdc/safemodel/classifiers/safesvc.py
 aisdc/safemodel/classifiers/safetf.py
 tests/test_attacks.py
 tests/test_attacks_dataset.py
 tests/test_attacks_via_safemodel.py
 tests/test_attribute_inference_attack.py
 tests/test_data_interface.py
+tests/test_generate_report.py
 tests/test_lira_attack.py
 tests/test_loaders.py
 tests/test_metrics.py
 tests/test_safedecisiontreeclassifier.py
 tests/test_safekeras2.py
 tests/test_safemodel.py
 tests/test_saferandomforestclassifier.py
```

### Comparing `aisdc-1.0.2/setup.py` & `aisdc-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="aisdc",
-    version="1.0.2",
+    version="1.0.3",
     license="MIT",
     maintainer="Jim Smith",
     maintainer_email="james.smith@uwe.ac.uk",
     description="Tools for the statistical disclosure control of machine learning models",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AI-SDC/AI-SDC",
```

### Comparing `aisdc-1.0.2/tests/test_attacks.py` & `aisdc-1.0.3/tests/test_attacks.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """Jim Smith October 2022
 tests to pick up odd cases not otherwise covered
 in code in the attacks folder
 """
-import math
 
 import numpy as np
 import pytest
 from fpdf import FPDF
 
-from aisdc.attacks import attack, dataset, mia_extremecase, report
+from aisdc.attacks import attack, dataset, report
 from aisdc.safemodel.classifiers import SafeDecisionTreeClassifier
 
 BORDER = 0
 
 
 def test_superclass():
     """Test that the exceptions are raised if the superclass is called in error"""
@@ -21,34 +20,14 @@
     target_obj = SafeDecisionTreeClassifier()
     with pytest.raises(NotImplementedError):
         my_attack.attack(target_obj, dataset_obj)
     with pytest.raises(NotImplementedError):
         print(str(my_attack))  # .__str__()
 
 
-def test_mia_extremecase():
-    """test the extreme case mia in the file of the same name"""
-
-    # create actual values
-    y = np.zeros(50000)
-    y[:25] = 1
-    # exactly right and wrong predictions
-    right = np.zeros(50000)
-    right[:25] = 1
-    wrong = 1 - right
-
-    # right predictions - triggers override for very small logp
-    _, _, _, pval = mia_extremecase.min_max_disc(y, right)
-    assert pval == -115.13
-
-    # wrong predictions - probaility very close to 1 so logp=0
-    _, _, _, pval = mia_extremecase.min_max_disc(y, wrong)
-    assert math.isclose(pval, 0.0)
-
-
 def test_NumpyArrayEncoder():
     """conversion routine
     from reports.py
     """
 
     i32 = np.int32(2)
     i64 = np.int64(2)
```

### Comparing `aisdc-1.0.2/tests/test_attacks_dataset.py` & `aisdc-1.0.3/tests/test_attacks_dataset.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.2/tests/test_attacks_via_safemodel.py` & `aisdc-1.0.3/tests/test_attacks_via_safemodel.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.2/tests/test_attribute_inference_attack.py` & `aisdc-1.0.3/tests/test_attribute_inference_attack.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.2/tests/test_data_interface.py` & `aisdc-1.0.3/tests/test_data_interface.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.2/tests/test_lira_attack.py` & `aisdc-1.0.3/tests/test_lira_attack.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.2/tests/test_loaders.py` & `aisdc-1.0.3/tests/test_loaders.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.2/tests/test_safedecisiontreeclassifier.py` & `aisdc-1.0.3/tests/test_safedecisiontreeclassifier.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.2/tests/test_safekeras2.py` & `aisdc-1.0.3/tests/test_safekeras2.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.2/tests/test_safemodel.py` & `aisdc-1.0.3/tests/test_safemodel.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.2/tests/test_saferandomforestclassifier.py` & `aisdc-1.0.3/tests/test_saferandomforestclassifier.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.2/tests/test_safesvc.py` & `aisdc-1.0.3/tests/test_safesvc.py`

 * *Files identical despite different names*

### Comparing `aisdc-1.0.2/tests/test_worst_case_attack.py` & `aisdc-1.0.3/tests/test_worst_case_attack.py`

 * *Files identical despite different names*

