# Comparing `tmp/promsoft_weight_calc_interface-0.1.5.tar.gz` & `tmp/promsoft_weight_calc_interface-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promsoft_weight_calc_interface-0.1.5.tar", max compression
+gzip compressed data, was "promsoft_weight_calc_interface-0.1.6.tar", max compression
```

## Comparing `promsoft_weight_calc_interface-0.1.5.tar` & `promsoft_weight_calc_interface-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      392 2023-04-14 07:41:57.164500 promsoft_weight_calc_interface-0.1.5/README.md
--rw-r--r--   0        0        0       68 2023-04-07 05:47:16.006748 promsoft_weight_calc_interface-0.1.5/promsoft_weight_calc_interface/__init__.py
--rw-r--r--   0        0        0     1575 2023-04-19 05:24:09.630483 promsoft_weight_calc_interface-0.1.5/promsoft_weight_calc_interface/models.py
--rw-r--r--   0        0        0      521 2023-04-19 05:24:09.630483 promsoft_weight_calc_interface-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      851 1970-01-01 00:00:00.000000 promsoft_weight_calc_interface-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      392 2023-04-14 07:41:57.164500 promsoft_weight_calc_interface-0.1.6/README.md
+-rw-r--r--   0        0        0       68 2023-04-07 05:47:16.006748 promsoft_weight_calc_interface-0.1.6/promsoft_weight_calc_interface/__init__.py
+-rw-r--r--   0        0        0     1660 2023-05-02 10:53:32.038228 promsoft_weight_calc_interface-0.1.6/promsoft_weight_calc_interface/models.py
+-rw-r--r--   0        0        0      505 2023-05-02 10:53:32.042228 promsoft_weight_calc_interface-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 promsoft_weight_calc_interface-0.1.6/PKG-INFO
```

### Comparing `promsoft_weight_calc_interface-0.1.5/promsoft_weight_calc_interface/models.py` & `promsoft_weight_calc_interface-0.1.6/promsoft_weight_calc_interface/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 from pydantic import BaseModel, validator, Field
 
 
+V2_RESULT_DICT = {
+    "detail": "",
+    "dimensions": {},
+    "items_sizes": {}
+}
+
+
 class Entry(BaseModel):
     """
     Класс для входных данных о товарах
     """
 
     id: int = Field(
         default=0,
```

### Comparing `promsoft_weight_calc_interface-0.1.5/PKG-INFO` & `promsoft_weight_calc_interface-0.1.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: promsoft-weight-calc-interface
-Version: 0.1.5
-Summary: Интерфейс для сервиса weight_calc.
+Version: 0.1.6
+Summary: An interface for weight_calc service.
 Author: Alena Chegodaikina
 Author-email: alena@promsoft.ru
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

