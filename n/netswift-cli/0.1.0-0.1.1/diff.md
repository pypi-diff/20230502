# Comparing `tmp/netswift_cli-0.1.0.tar.gz` & `tmp/netswift_cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netswift_cli-0.1.0.tar", max compression
+gzip compressed data, was "netswift_cli-0.1.1.tar", max compression
```

## Comparing `netswift_cli-0.1.0.tar` & `netswift_cli-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0      149 2023-05-02 08:35:12.064627 netswift_cli-0.1.0/netswift_cli/README.md
--rw-r--r--   0        0        0     2883 2023-05-02 08:46:05.134384 netswift_cli-0.1.0/netswift_cli/netswift_cli.py
--rw-r--r--   0        0        0      861 2023-05-02 08:52:26.285750 netswift_cli-0.1.0/netswift_cli/requirements.txt
--rw-r--r--   0        0        0      418 2023-05-02 08:57:54.344365 netswift_cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      591 1970-01-01 00:00:00.000000 netswift_cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      149 2023-05-02 08:35:12.064627 netswift_cli-0.1.1/netswift_cli/README.md
+-rw-r--r--   0        0        0    16384 2023-05-02 10:12:39.593378 netswift_cli-0.1.1/netswift_cli/employee_absent.db
+-rw-r--r--   0        0        0     5043 2023-05-02 10:13:25.232133 netswift_cli-0.1.1/netswift_cli/netswift_cli.py
+-rw-r--r--   0        0        0      861 2023-05-02 08:52:26.285750 netswift_cli-0.1.1/netswift_cli/requirements.txt
+-rw-r--r--   0        0        0      418 2023-05-02 10:18:47.277783 netswift_cli-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      591 1970-01-01 00:00:00.000000 netswift_cli-0.1.1/PKG-INFO
```

### Comparing `netswift_cli-0.1.0/netswift_cli/requirements.txt` & `netswift_cli-0.1.1/netswift_cli/requirements.txt`

 * *Files identical despite different names*

### Comparing `netswift_cli-0.1.0/PKG-INFO` & `netswift_cli-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netswift-cli
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple CLI application to manage NetSwift employee attendance
 Author: Rehmat Alam
 Author-email: rehmat@netswift.pk
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

