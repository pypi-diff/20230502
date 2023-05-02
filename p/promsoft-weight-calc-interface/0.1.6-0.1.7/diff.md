# Comparing `tmp/promsoft_weight_calc_interface-0.1.6.tar.gz` & `tmp/promsoft_weight_calc_interface-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promsoft_weight_calc_interface-0.1.6.tar", max compression
+gzip compressed data, was "promsoft_weight_calc_interface-0.1.7.tar", max compression
```

## Comparing `promsoft_weight_calc_interface-0.1.6.tar` & `promsoft_weight_calc_interface-0.1.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      392 2023-04-14 07:41:57.164500 promsoft_weight_calc_interface-0.1.6/README.md
--rw-r--r--   0        0        0       68 2023-04-07 05:47:16.006748 promsoft_weight_calc_interface-0.1.6/promsoft_weight_calc_interface/__init__.py
--rw-r--r--   0        0        0     1660 2023-05-02 10:53:32.038228 promsoft_weight_calc_interface-0.1.6/promsoft_weight_calc_interface/models.py
--rw-r--r--   0        0        0      505 2023-05-02 10:53:32.042228 promsoft_weight_calc_interface-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 promsoft_weight_calc_interface-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      392 2023-04-14 07:41:57.164500 promsoft_weight_calc_interface-0.1.7/README.md
+-rw-r--r--   0        0        0       84 2023-05-02 11:04:37.319980 promsoft_weight_calc_interface-0.1.7/promsoft_weight_calc_interface/__init__.py
+-rw-r--r--   0        0        0     1660 2023-05-02 10:53:32.038228 promsoft_weight_calc_interface-0.1.7/promsoft_weight_calc_interface/models.py
+-rw-r--r--   0        0        0      505 2023-05-02 11:04:37.319980 promsoft_weight_calc_interface-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 promsoft_weight_calc_interface-0.1.7/PKG-INFO
```

### Comparing `promsoft_weight_calc_interface-0.1.6/promsoft_weight_calc_interface/models.py` & `promsoft_weight_calc_interface-0.1.7/promsoft_weight_calc_interface/models.py`

 * *Files identical despite different names*

### Comparing `promsoft_weight_calc_interface-0.1.6/PKG-INFO` & `promsoft_weight_calc_interface-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promsoft-weight-calc-interface
-Version: 0.1.6
+Version: 0.1.7
 Summary: An interface for weight_calc service.
 Author: Alena Chegodaikina
 Author-email: alena@promsoft.ru
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

