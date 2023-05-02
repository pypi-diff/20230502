# Comparing `tmp/smartsheet-pydantic-1.4.0.tar.gz` & `tmp/smartsheet-pydantic-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartsheet-pydantic-1.4.0.tar", last modified: Mon May  1 22:50:21 2023, max compression
+gzip compressed data, was "smartsheet-pydantic-1.4.1.tar", last modified: Tue May  2 02:40:40 2023, max compression
```

## Comparing `smartsheet-pydantic-1.4.0.tar` & `smartsheet-pydantic-1.4.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 agile     (1000) agile     (1000)        0 2023-05-01 22:50:21.665284 smartsheet-pydantic-1.4.0/
--rw-rw-r--   0 agile     (1000) agile     (1000)     1091 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.0/LICENSE
--rw-rw-r--   0 agile     (1000) agile     (1000)     8575 2023-05-01 22:50:21.665284 smartsheet-pydantic-1.4.0/PKG-INFO
--rw-rw-r--   0 agile     (1000) agile     (1000)     6925 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.0/README.md
--rw-rw-r--   0 agile     (1000) agile     (1000)      811 2023-05-01 22:46:50.000000 smartsheet-pydantic-1.4.0/pyproject.toml
--rw-rw-r--   0 agile     (1000) agile     (1000)       38 2023-05-01 22:50:21.665284 smartsheet-pydantic-1.4.0/setup.cfg
-drwxrwxr-x   0 agile     (1000) agile     (1000)        0 2023-05-01 22:50:21.665284 smartsheet-pydantic-1.4.0/src/
-drwxrwxr-x   0 agile     (1000) agile     (1000)        0 2023-05-01 22:50:21.665284 smartsheet-pydantic-1.4.0/src/smartsheet_pydantic/
--rw-rw-r--   0 agile     (1000) agile     (1000)        0 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.0/src/smartsheet_pydantic/__init__.py
--rw-rw-r--   0 agile     (1000) agile     (1000)     6740 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.0/src/smartsheet_pydantic/controller.py
--rw-rw-r--   0 agile     (1000) agile     (1000)      493 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.0/src/smartsheet_pydantic/debug_logger.py
--rw-rw-r--   0 agile     (1000) agile     (1000)     2816 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.0/src/smartsheet_pydantic/filters.py
--rw-rw-r--   0 agile     (1000) agile     (1000)    12396 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.0/src/smartsheet_pydantic/smartmodels.py
--rw-rw-r--   0 agile     (1000) agile     (1000)     3087 2023-05-01 22:41:52.000000 smartsheet-pydantic-1.4.0/src/smartsheet_pydantic/sources.py
--rw-rw-r--   0 agile     (1000) agile     (1000)     2329 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.0/src/smartsheet_pydantic/transformer.py
-drwxrwxr-x   0 agile     (1000) agile     (1000)        0 2023-05-01 22:50:21.665284 smartsheet-pydantic-1.4.0/src/smartsheet_pydantic.egg-info/
--rw-rw-r--   0 agile     (1000) agile     (1000)     8575 2023-05-01 22:50:21.000000 smartsheet-pydantic-1.4.0/src/smartsheet_pydantic.egg-info/PKG-INFO
--rw-rw-r--   0 agile     (1000) agile     (1000)      622 2023-05-01 22:50:21.000000 smartsheet-pydantic-1.4.0/src/smartsheet_pydantic.egg-info/SOURCES.txt
--rw-rw-r--   0 agile     (1000) agile     (1000)        1 2023-05-01 22:50:21.000000 smartsheet-pydantic-1.4.0/src/smartsheet_pydantic.egg-info/dependency_links.txt
--rw-rw-r--   0 agile     (1000) agile     (1000)      102 2023-05-01 22:50:21.000000 smartsheet-pydantic-1.4.0/src/smartsheet_pydantic.egg-info/requires.txt
--rw-rw-r--   0 agile     (1000) agile     (1000)       20 2023-05-01 22:50:21.000000 smartsheet-pydantic-1.4.0/src/smartsheet_pydantic.egg-info/top_level.txt
-drwxrwxr-x   0 agile     (1000) agile     (1000)        0 2023-05-01 22:50:21.665284 smartsheet-pydantic-1.4.0/tests/
--rw-rw-r--   0 agile     (1000) agile     (1000)     4686 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.0/tests/test_controller.py
--rw-rw-r--   0 agile     (1000) agile     (1000)     3527 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.0/tests/test_filters.py
--rw-rw-r--   0 agile     (1000) agile     (1000)    13872 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.0/tests/test_smartmodel.py
--rw-rw-r--   0 agile     (1000) agile     (1000)     1714 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.0/tests/test_sources.py
+drwxrwxr-x   0 agile     (1000) agile     (1000)        0 2023-05-02 02:40:40.064898 smartsheet-pydantic-1.4.1/
+-rw-rw-r--   0 agile     (1000) agile     (1000)     1091 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.1/LICENSE
+-rw-rw-r--   0 agile     (1000) agile     (1000)     8575 2023-05-02 02:40:40.064898 smartsheet-pydantic-1.4.1/PKG-INFO
+-rw-rw-r--   0 agile     (1000) agile     (1000)     6925 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.1/README.md
+-rw-rw-r--   0 agile     (1000) agile     (1000)      811 2023-05-02 02:38:43.000000 smartsheet-pydantic-1.4.1/pyproject.toml
+-rw-rw-r--   0 agile     (1000) agile     (1000)       38 2023-05-02 02:40:40.064898 smartsheet-pydantic-1.4.1/setup.cfg
+drwxrwxr-x   0 agile     (1000) agile     (1000)        0 2023-05-02 02:40:40.064898 smartsheet-pydantic-1.4.1/src/
+drwxrwxr-x   0 agile     (1000) agile     (1000)        0 2023-05-02 02:40:40.064898 smartsheet-pydantic-1.4.1/src/smartsheet_pydantic/
+-rw-rw-r--   0 agile     (1000) agile     (1000)        0 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.1/src/smartsheet_pydantic/__init__.py
+-rw-rw-r--   0 agile     (1000) agile     (1000)     7370 2023-05-02 02:38:26.000000 smartsheet-pydantic-1.4.1/src/smartsheet_pydantic/controller.py
+-rw-rw-r--   0 agile     (1000) agile     (1000)      493 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.1/src/smartsheet_pydantic/debug_logger.py
+-rw-rw-r--   0 agile     (1000) agile     (1000)     2816 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.1/src/smartsheet_pydantic/filters.py
+-rw-rw-r--   0 agile     (1000) agile     (1000)    12396 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.1/src/smartsheet_pydantic/smartmodels.py
+-rw-rw-r--   0 agile     (1000) agile     (1000)     3087 2023-05-01 22:53:34.000000 smartsheet-pydantic-1.4.1/src/smartsheet_pydantic/sources.py
+-rw-rw-r--   0 agile     (1000) agile     (1000)     2329 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.1/src/smartsheet_pydantic/transformer.py
+drwxrwxr-x   0 agile     (1000) agile     (1000)        0 2023-05-02 02:40:40.064898 smartsheet-pydantic-1.4.1/src/smartsheet_pydantic.egg-info/
+-rw-rw-r--   0 agile     (1000) agile     (1000)     8575 2023-05-02 02:40:40.000000 smartsheet-pydantic-1.4.1/src/smartsheet_pydantic.egg-info/PKG-INFO
+-rw-rw-r--   0 agile     (1000) agile     (1000)      622 2023-05-02 02:40:40.000000 smartsheet-pydantic-1.4.1/src/smartsheet_pydantic.egg-info/SOURCES.txt
+-rw-rw-r--   0 agile     (1000) agile     (1000)        1 2023-05-02 02:40:40.000000 smartsheet-pydantic-1.4.1/src/smartsheet_pydantic.egg-info/dependency_links.txt
+-rw-rw-r--   0 agile     (1000) agile     (1000)      102 2023-05-02 02:40:40.000000 smartsheet-pydantic-1.4.1/src/smartsheet_pydantic.egg-info/requires.txt
+-rw-rw-r--   0 agile     (1000) agile     (1000)       20 2023-05-02 02:40:40.000000 smartsheet-pydantic-1.4.1/src/smartsheet_pydantic.egg-info/top_level.txt
+drwxrwxr-x   0 agile     (1000) agile     (1000)        0 2023-05-02 02:40:40.064898 smartsheet-pydantic-1.4.1/tests/
+-rw-rw-r--   0 agile     (1000) agile     (1000)     4686 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.1/tests/test_controller.py
+-rw-rw-r--   0 agile     (1000) agile     (1000)     3527 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.1/tests/test_filters.py
+-rw-rw-r--   0 agile     (1000) agile     (1000)    13872 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.1/tests/test_smartmodel.py
+-rw-rw-r--   0 agile     (1000) agile     (1000)     1714 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.1/tests/test_sources.py
```

### Comparing `smartsheet-pydantic-1.4.0/LICENSE` & `smartsheet-pydantic-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.4.0/PKG-INFO` & `smartsheet-pydantic-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartsheet-pydantic
-Version: 1.4.0
+Version: 1.4.1
 Summary: Smartsheet Python SDK and Pydantic Wrapper
 Author: Takahiro Watanabe
 License: The MIT License (MIT)
         Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `smartsheet-pydantic-1.4.0/README.md` & `smartsheet-pydantic-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.4.0/pyproject.toml` & `smartsheet-pydantic-1.4.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=67.7.1", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "smartsheet-pydantic"
-version = "1.4.0"
+version = "1.4.1"
 description = "Smartsheet Python SDK and Pydantic Wrapper"
 readme = "README.md"
 authors = [{ name = "Takahiro Watanabe" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `smartsheet-pydantic-1.4.0/src/smartsheet_pydantic/controller.py` & `smartsheet-pydantic-1.4.1/src/smartsheet_pydantic/controller.py`

 * *Files 17% similar despite different names*

```diff
@@ -111,28 +111,43 @@
         return list(result)
 
     @debug_logger
     def extract_as_smartmodels(self) -> set[SmartModel]:
         rows = self.extract_row_objects()
         return self.target_transformer.fit(rows)
 
-    def add_rows(self, dataset: set[SmartModel]) -> dict[str: int]:
+    def add_rows(self, dataset: set[SmartModel], partition_size=300) -> dict[str: int]:
         """
         Append the given set of SmartModels into the smartsheet.
         """
-        try:
-            logging.info(f"{len(dataset)} SmartModels prepared for addition")
+
+        def add_rows(dataset):
             rows = []
             for data in dataset:
-                row = \
-                    data.to_row(self.sheet)
+                row = data.to_row(self.sheet)
                 rows.append(row)
             response = self.sheet.add_rows(rows)
             if response.result_code != 0:
                 raise Exception(f"Row addition failed {response.data}")
+
+        try:
+            logging.info(f"{len(dataset)} SmartModels prepared for addition")
+            dataset = list(dataset)
+            partition_count = 0
+            while len(dataset) > 0:
+                if len(dataset) > partition_size:
+                    subset = dataset[:partition_size]
+                    dataset = dataset[partition_size:]
+                    add_rows(subset)
+                    partition_count += 1
+                else:
+                    add_rows(dataset)
+                    partition_count += 1
+                    dataset = 0
+            logging.info(f"Addition complete in {partition_count} partitions, with each partition size of {partition_size}")
             return {"status_code": 201}
         except Exception as e:
             raise Exception(f"Row addition failed {e}")
 
     @debug_logger
     def update_rows(self, dataset: set[SmartModel]) -> dict[str: int]:
         """
```

### Comparing `smartsheet-pydantic-1.4.0/src/smartsheet_pydantic/filters.py` & `smartsheet-pydantic-1.4.1/src/smartsheet_pydantic/filters.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.4.0/src/smartsheet_pydantic/smartmodels.py` & `smartsheet-pydantic-1.4.1/src/smartsheet_pydantic/smartmodels.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.4.0/src/smartsheet_pydantic/sources.py` & `smartsheet-pydantic-1.4.1/src/smartsheet_pydantic/sources.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.4.0/src/smartsheet_pydantic/transformer.py` & `smartsheet-pydantic-1.4.1/src/smartsheet_pydantic/transformer.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.4.0/src/smartsheet_pydantic.egg-info/PKG-INFO` & `smartsheet-pydantic-1.4.1/src/smartsheet_pydantic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartsheet-pydantic
-Version: 1.4.0
+Version: 1.4.1
 Summary: Smartsheet Python SDK and Pydantic Wrapper
 Author: Takahiro Watanabe
 License: The MIT License (MIT)
         Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `smartsheet-pydantic-1.4.0/src/smartsheet_pydantic.egg-info/SOURCES.txt` & `smartsheet-pydantic-1.4.1/src/smartsheet_pydantic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.4.0/tests/test_controller.py` & `smartsheet-pydantic-1.4.1/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.4.0/tests/test_filters.py` & `smartsheet-pydantic-1.4.1/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.4.0/tests/test_smartmodel.py` & `smartsheet-pydantic-1.4.1/tests/test_smartmodel.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.4.0/tests/test_sources.py` & `smartsheet-pydantic-1.4.1/tests/test_sources.py`

 * *Files identical despite different names*

