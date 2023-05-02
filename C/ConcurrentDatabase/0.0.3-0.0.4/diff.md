# Comparing `tmp/ConcurrentDatabase-0.0.3.tar.gz` & `tmp/ConcurrentDatabase-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ConcurrentDatabase-0.0.3.tar", last modified: Tue May  2 17:03:39 2023, max compression
+gzip compressed data, was "ConcurrentDatabase-0.0.4.tar", last modified: Tue May  2 21:09:45 2023, max compression
```

## Comparing `ConcurrentDatabase-0.0.3.tar` & `ConcurrentDatabase-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:03:39.855767 ConcurrentDatabase-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:03:39.851767 ConcurrentDatabase-0.0.3/ConcurrentDatabase/
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-05-02 17:03:26.000000 ConcurrentDatabase-0.0.3/ConcurrentDatabase/ColumnWrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-05-02 17:03:26.000000 ConcurrentDatabase-0.0.3/ConcurrentDatabase/Database.py
--rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-05-02 17:03:26.000000 ConcurrentDatabase-0.0.3/ConcurrentDatabase/DynamicEntry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-05-02 17:03:26.000000 ConcurrentDatabase-0.0.3/ConcurrentDatabase/DynamicTable.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-02 17:03:26.000000 ConcurrentDatabase-0.0.3/ConcurrentDatabase/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:03:39.851767 ConcurrentDatabase-0.0.3/ConcurrentDatabase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-02 17:03:39.000000 ConcurrentDatabase-0.0.3/ConcurrentDatabase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-02 17:03:39.000000 ConcurrentDatabase-0.0.3/ConcurrentDatabase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 17:03:39.000000 ConcurrentDatabase-0.0.3/ConcurrentDatabase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 17:03:39.000000 ConcurrentDatabase-0.0.3/ConcurrentDatabase.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-02 17:03:39.851767 ConcurrentDatabase-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-02 17:03:26.000000 ConcurrentDatabase-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-02 17:03:26.000000 ConcurrentDatabase-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 17:03:39.855767 ConcurrentDatabase-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-02 17:03:26.000000 ConcurrentDatabase-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:09:45.753652 ConcurrentDatabase-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:09:45.753652 ConcurrentDatabase-0.0.4/ConcurrentDatabase/
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-02 21:09:31.000000 ConcurrentDatabase-0.0.4/ConcurrentDatabase/ColumnWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-05-02 21:09:31.000000 ConcurrentDatabase-0.0.4/ConcurrentDatabase/Database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-05-02 21:09:31.000000 ConcurrentDatabase-0.0.4/ConcurrentDatabase/DynamicEntry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-05-02 21:09:31.000000 ConcurrentDatabase-0.0.4/ConcurrentDatabase/DynamicTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-02 21:09:31.000000 ConcurrentDatabase-0.0.4/ConcurrentDatabase/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:09:45.753652 ConcurrentDatabase-0.0.4/ConcurrentDatabase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-02 21:09:45.000000 ConcurrentDatabase-0.0.4/ConcurrentDatabase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-02 21:09:45.000000 ConcurrentDatabase-0.0.4/ConcurrentDatabase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:09:45.000000 ConcurrentDatabase-0.0.4/ConcurrentDatabase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 21:09:45.000000 ConcurrentDatabase-0.0.4/ConcurrentDatabase.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-02 21:09:45.753652 ConcurrentDatabase-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-02 21:09:31.000000 ConcurrentDatabase-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-02 21:09:31.000000 ConcurrentDatabase-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 21:09:45.753652 ConcurrentDatabase-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-02 21:09:31.000000 ConcurrentDatabase-0.0.4/setup.py
```

### Comparing `ConcurrentDatabase-0.0.3/ConcurrentDatabase/ColumnWrapper.py` & `ConcurrentDatabase-0.0.4/ConcurrentDatabase/ColumnWrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,25 +23,25 @@
             return
 
         if isinstance(value, list):  # If the value is a range of values then validate each value in the range
             for item in value:
                 self.validate(item)
             return
         # Validate the duck type of the column is correct (aka if it is a string of an integer its still an integer)
-        if self.type == "INTEGER":
+        if self.type == "INTEGER" or self.type == "INT":
             try:
                 int(value)
             except ValueError:
                 raise ValueError(f"Column {self.name} must of duck type {self.type}")
         elif self.type == "REAL":
             try:
                 float(value)
             except ValueError:
                 raise ValueError(f"Column {self.name} must of duck type {self.type}")
-        elif self.type == "TEXT":
+        elif self.type == "TEXT" or self.type == "STRING":
             if not isinstance(value, str) and not isinstance(value, int) and not isinstance(value, float):
                 raise ValueError(f"Column {self.name} must of duck type {self.type} not {type(value)}")
         elif self.type == "BLOB":
             if not isinstance(value, bytes):
                 raise ValueError(f"Column {self.name} must of exact type {self.type}")
         elif self.type == "BOOLEAN":
             if not isinstance(value, bool):
@@ -80,20 +80,20 @@
         Returns a value that is safe to be inserted into a SQL statement
         :param column: The column that the value is for
         :param value: The value to be inserted
         :return:
         """
         if value is None:
             return "NULL"
-        elif self.type == "TEXT":
+        elif self.type == "TEXT" or self.type == "STRING":
             return f"'{value}'"
-        elif self.type == "INTEGER":
+        elif self.type == "INTEGER" or self.type == "INT":
             return str(value)
         elif self.type == "BOOLEAN":
             return str(value)
         elif self.type == "REAL":
             return str(value)
         elif self.type == "BLOB":
             return str(value)
         else:
-            logging.warning(f"Unknown column type {self.type}")
-            return str(value)
+            logging.warning(f"Unknown column type {self.type}, assuming TEXT")
+            return f"'{value}'"
```

### Comparing `ConcurrentDatabase-0.0.3/ConcurrentDatabase/Database.py` & `ConcurrentDatabase-0.0.4/ConcurrentDatabase/Database.py`

 * *Files identical despite different names*

### Comparing `ConcurrentDatabase-0.0.3/ConcurrentDatabase/DynamicEntry.py` & `ConcurrentDatabase-0.0.4/ConcurrentDatabase/DynamicEntry.py`

 * *Files identical despite different names*

### Comparing `ConcurrentDatabase-0.0.3/ConcurrentDatabase/DynamicTable.py` & `ConcurrentDatabase-0.0.4/ConcurrentDatabase/DynamicTable.py`

 * *Files identical despite different names*

### Comparing `ConcurrentDatabase-0.0.3/ConcurrentDatabase.egg-info/PKG-INFO` & `ConcurrentDatabase-0.0.4/ConcurrentDatabase.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ConcurrentDatabase
-Version: 0.0.3
+Version: 0.0.4
 Summary: A SQLite wrapper that allows for object oriented database access.
 Home-page: 
 Author: Jay S
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
```

### Comparing `ConcurrentDatabase-0.0.3/PKG-INFO` & `ConcurrentDatabase-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ConcurrentDatabase
-Version: 0.0.3
+Version: 0.0.4
 Summary: A SQLite wrapper that allows for object oriented database access.
 Home-page: 
 Author: Jay S
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
```

### Comparing `ConcurrentDatabase-0.0.3/README.md` & `ConcurrentDatabase-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ConcurrentDatabase-0.0.3/pyproject.toml` & `ConcurrentDatabase-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ConcurrentDatabase-0.0.3/setup.py` & `ConcurrentDatabase-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ConcurrentDatabase",
-    version="0.0.3",
+    version="0.0.4",
     author="Jay S",
     author_email="",
     description="A SQLite wrapper that allows for object oriented database access.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

