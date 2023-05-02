# Comparing `tmp/ConcurrentDatabase-0.0.2.tar.gz` & `tmp/ConcurrentDatabase-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ConcurrentDatabase-0.0.2.tar", last modified: Tue May  2 16:56:09 2023, max compression
+gzip compressed data, was "ConcurrentDatabase-0.0.3.tar", last modified: Tue May  2 17:03:39 2023, max compression
```

## Comparing `ConcurrentDatabase-0.0.2.tar` & `ConcurrentDatabase-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:56:09.800910 ConcurrentDatabase-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:56:09.796910 ConcurrentDatabase-0.0.2/ConcurrentDatabase/
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-02 16:55:58.000000 ConcurrentDatabase-0.0.2/ConcurrentDatabase/ColumnWrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-05-02 16:55:58.000000 ConcurrentDatabase-0.0.2/ConcurrentDatabase/Database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8849 2023-05-02 16:55:58.000000 ConcurrentDatabase-0.0.2/ConcurrentDatabase/DynamicEntry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-05-02 16:55:58.000000 ConcurrentDatabase-0.0.2/ConcurrentDatabase/DynamicTable.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-02 16:55:58.000000 ConcurrentDatabase-0.0.2/ConcurrentDatabase/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:56:09.800910 ConcurrentDatabase-0.0.2/ConcurrentDatabase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-02 16:56:09.000000 ConcurrentDatabase-0.0.2/ConcurrentDatabase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-02 16:56:09.000000 ConcurrentDatabase-0.0.2/ConcurrentDatabase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 16:56:09.000000 ConcurrentDatabase-0.0.2/ConcurrentDatabase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 16:56:09.000000 ConcurrentDatabase-0.0.2/ConcurrentDatabase.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-02 16:56:09.800910 ConcurrentDatabase-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-02 16:55:58.000000 ConcurrentDatabase-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-02 16:55:58.000000 ConcurrentDatabase-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 16:56:09.800910 ConcurrentDatabase-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-02 16:55:58.000000 ConcurrentDatabase-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:03:39.855767 ConcurrentDatabase-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:03:39.851767 ConcurrentDatabase-0.0.3/ConcurrentDatabase/
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-05-02 17:03:26.000000 ConcurrentDatabase-0.0.3/ConcurrentDatabase/ColumnWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-05-02 17:03:26.000000 ConcurrentDatabase-0.0.3/ConcurrentDatabase/Database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-05-02 17:03:26.000000 ConcurrentDatabase-0.0.3/ConcurrentDatabase/DynamicEntry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-05-02 17:03:26.000000 ConcurrentDatabase-0.0.3/ConcurrentDatabase/DynamicTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-02 17:03:26.000000 ConcurrentDatabase-0.0.3/ConcurrentDatabase/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:03:39.851767 ConcurrentDatabase-0.0.3/ConcurrentDatabase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-02 17:03:39.000000 ConcurrentDatabase-0.0.3/ConcurrentDatabase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-02 17:03:39.000000 ConcurrentDatabase-0.0.3/ConcurrentDatabase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 17:03:39.000000 ConcurrentDatabase-0.0.3/ConcurrentDatabase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 17:03:39.000000 ConcurrentDatabase-0.0.3/ConcurrentDatabase.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-02 17:03:39.851767 ConcurrentDatabase-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-02 17:03:26.000000 ConcurrentDatabase-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-02 17:03:26.000000 ConcurrentDatabase-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 17:03:39.855767 ConcurrentDatabase-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-02 17:03:26.000000 ConcurrentDatabase-0.0.3/setup.py
```

### Comparing `ConcurrentDatabase-0.0.2/ConcurrentDatabase/ColumnWrapper.py` & `ConcurrentDatabase-0.0.3/ConcurrentDatabase/ColumnWrapper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from loguru import logger as logging
+
+
 class ColumnWrapper:
 
     def __init__(self, table, pragma):
         self.table = table
         self.position = pragma[0]  # type: int
         self.name = pragma[1]  # type: str
         self.type = pragma[2].upper()  # type: str
@@ -9,16 +12,20 @@
         self.default_value = pragma[4]  # type: str
         self.primary_key = pragma[5]  # type: int
 
         if self.primary_key:
             self.table.primary_keys.append(self)
 
     def validate(self, value):
-        if self.not_null and value is None and self.default_value is None:
+
+        if (self.not_null and value is None) and self.default_value == "":
             raise ValueError(f"Column {self.name} cannot be null")
+        elif value is None:
+            return
+
         if isinstance(value, list):  # If the value is a range of values then validate each value in the range
             for item in value:
                 self.validate(item)
             return
         # Validate the duck type of the column is correct (aka if it is a string of an integer its still an integer)
         if self.type == "INTEGER":
             try:
@@ -28,26 +35,27 @@
         elif self.type == "REAL":
             try:
                 float(value)
             except ValueError:
                 raise ValueError(f"Column {self.name} must of duck type {self.type}")
         elif self.type == "TEXT":
             if not isinstance(value, str) and not isinstance(value, int) and not isinstance(value, float):
-                raise ValueError(f"Column {self.name} must of duck type {self.type}")
+                raise ValueError(f"Column {self.name} must of duck type {self.type} not {type(value)}")
         elif self.type == "BLOB":
             if not isinstance(value, bytes):
                 raise ValueError(f"Column {self.name} must of exact type {self.type}")
         elif self.type == "BOOLEAN":
             if not isinstance(value, bool):
                 raise ValueError(f"Column {self.name} must of exact type {self.type}")
         else:
-            raise ValueError(f"Column {self.name} has an unknown type {self.type}")
+            logging.warning(f"Unknown column type {self.type}")
 
     def __str__(self):
-        return f"[{self.position}]-{self.name}-{self.type}-{'NOT NULL' if self.not_null else 'NULL'}-{'PRIMARY KEY' if self.primary_key else ''}"
+        return f"[{self.position}]{'-PRIMARY KEY' if self.primary_key else ''}-{self.name}-({self.type})-" \
+               f"{'NOT NULL' if self.not_null else ''}-{'DEFAULT ' + self.default_value if self.default_value else ''}"
 
     def __repr__(self):
         return self.__str__()
 
     def __eq__(self, other):
         if isinstance(other, ColumnWrapper):
             return self.name == other.name
@@ -83,8 +91,9 @@
         elif self.type == "BOOLEAN":
             return str(value)
         elif self.type == "REAL":
             return str(value)
         elif self.type == "BLOB":
             return str(value)
         else:
-            raise TypeError(f"Unknown column type {self.type}")
+            logging.warning(f"Unknown column type {self.type}")
+            return str(value)
```

### Comparing `ConcurrentDatabase-0.0.2/ConcurrentDatabase/Database.py` & `ConcurrentDatabase-0.0.3/ConcurrentDatabase/Database.py`

 * *Files 12% similar despite different names*

```diff
@@ -88,17 +88,20 @@
         :param table_name: The name of the table to update.
         :param version: The version of the table to update.
         :param update_query: A custom update query if table elements need to be updated in a specific way.
         """
         # Check if the table is already up to date
         if self.table_version_table.get_row(table_name=table_name)["version"] == version:
             return
-        # Check if the revision increment is valid
-        if self.table_version_table.get_row(table_name=table_name)["version"] + 1 != version:
-            raise ValueError(f"Invalid revision increment for table {table_name} max increment is 1")
+        elif self.table_version_table.get_row(table_name=table_name)["version"] > version:
+            return
+        # Check if the revision increment is only 1 more than the current version
+        elif self.table_version_table.get_row(table_name=table_name)["version"] + 1 != version:
+            raise ValueError(f"Table {table_name} version {version} is not 1 more than the current version "
+                             f"{self.table_version_table.get_row(table_name=table_name)['version']}")
         # Check if the table exists
         if table_name not in self.tables:
             raise KeyError(f"Table {table_name} not found in database {self.database_name}")
 
         # Update the table
         if update_query:
             for query in update_query:
```

### Comparing `ConcurrentDatabase-0.0.2/ConcurrentDatabase/DynamicEntry.py` & `ConcurrentDatabase-0.0.3/ConcurrentDatabase/DynamicEntry.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,19 @@
 
         for key in kwargs:
             if key in self.columns:
                 self._values[key] = kwargs[key]
             else:
                 raise KeyError(f"Column {key} does not exist in table {self.table.table_name}")
 
+        # Add columns that were not specified and have a default value
+        for column in self.columns:
+            if column.name not in self._values and column.default_value is not None:
+                self._values[column.name] = column.default_value
+
         self._previous_values = self._values.copy()
 
     def __getitem__(self, item):
         # This form of item setting does not access the database and is only in memory
         if isinstance(item, int):  # Select by index
             if len(self.columns) > item >= 0:
                 return self._values[self.columns[item].name]
@@ -89,15 +94,17 @@
         Flushes the changes to the database if there are any
         :return:
         """
         if self._dirty:
             # Build the query
             changed_values = {}
             for key in self._values:
-                if self._values[key] != self._previous_values[key]:
+                if key in self._previous_values and self._values[key] != self._previous_values[key]:
+                    changed_values[key] = self._values[key]
+                elif key not in self._previous_values:
                     changed_values[key] = self._values[key]
             if len(changed_values) == 0:
                 return
             sql = f"UPDATE {self.table.table_name} SET "
             for key in changed_values:
                 sql += f"{key} = ?, "
             sql = sql[:-2] if sql.endswith(", ") else sql  # Remove the trailing comma and space if there is one
@@ -116,15 +123,17 @@
         Called by this entry's table to flush all entries in the table in one transaction
         :return:
         """
         if self._dirty:
             # Build the query
             changed_values = {}
             for key in self._values:
-                if self._values[key] != self._previous_values[key]:
+                if key in self._previous_values and self._values[key] != self._previous_values[key]:
+                    changed_values[key] = self._values[key]
+                elif key not in self._previous_values:
                     changed_values[key] = self._values[key]
             if len(changed_values) == 0:
                 return ""
             sql = f"UPDATE {self.table.table_name} SET "
             for key, value in changed_values.items():
                 column = self.columns[self.columns.index(key)]
                 sql += f"{key} = {column.safe_value(value)}, "
```

### Comparing `ConcurrentDatabase-0.0.2/ConcurrentDatabase/DynamicTable.py` & `ConcurrentDatabase-0.0.3/ConcurrentDatabase/DynamicTable.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,14 +55,24 @@
         """
         Update the schema of the table.
         :return: None
         """
         self.columns = []
         self._load_columns()
 
+    def get_entry_by_row(self, row_num: int):
+        """
+        Get an entry by the row number.
+        """
+        result = self.database.get(f"SELECT * FROM {self.table_name} LIMIT 1 OFFSET {row_num}")
+        if result:
+            return DynamicEntry(self, load_tuple=result[0])
+        else:
+            return None
+
     def get_row(self, **kwargs) -> typing.Optional[DynamicEntry]:
         """
         Get a row from the table.
         :param kwargs: The filters to apply to the query.
         :return: The row.
         """
         self._validate_columns(**kwargs)
@@ -110,27 +120,35 @@
         if result:
             entries = [DynamicEntry(self, load_tuple=row) for row in result]
             self.entries.extend(entries)
             return entries
         else:
             return []
 
-    def get_all(self) -> List[DynamicEntry]:
+    def get_all(self, reverse=False) -> List[DynamicEntry]:
         """
         Get all rows from the table. This is not recommended for large tables.
         :return: The rows.
         """
-        result = self.database.get(f"SELECT * FROM {self.table_name}")
+        result = self.database.get(f"SELECT * FROM {self.table_name} ORDER BY rowid {'DESC' if reverse else 'ASC'}")
         if result:
             entries = [DynamicEntry(self, load_tuple=row) for row in result]
             self.entries.extend(entries)
             return entries
         else:
             return []
 
+    def custom_query(self, sql: str):
+        """
+        Run a custom query on the table.
+        :param sql: The query to run.
+        :return: The result of the query.
+        """
+        return self.database.get(sql)
+
     def add(self, **kwargs) -> DynamicEntry:
         """
         Add a row to the table.
         :param kwargs: The values of the entry
         :return: A DynamicEntry object representing the row.
         """
         # For each column validate that it is a valid column
@@ -264,21 +282,28 @@
         if key in self.columns:
             self.database.run(f"ALTER TABLE {self.table_name} DROP COLUMN {key}")
             self.columns.remove(key)
         else:
             raise KeyError(f"Column {key} not found in table {self.table_name}")
 
     def __iter__(self):
-        for column in self.columns:
-            yield column
+        """
+        Iterate over the entries in the table.
+        """
+        # Load all entries
+        return self.get_all()
 
     def __len__(self):
-        return len(self.columns)
+        """
+        Get the number of entries in the table.
+        """
+        sql = f"SELECT COUNT(*) FROM {self.table_name}"
+        return self.database.get(sql)[0][0]
 
     def __contains__(self, key):
         return key in self.columns
 
     def __repr__(self):
         return f"DynamicTable({self.table_name}, {self.database})"
 
     def __str__(self):
-        return f"DynamicTable({self.table_name}, {self.database})"
+        return f"DynamicTable({self.table_name}, {self.database})"
```

### Comparing `ConcurrentDatabase-0.0.2/ConcurrentDatabase.egg-info/PKG-INFO` & `ConcurrentDatabase-0.0.3/ConcurrentDatabase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ConcurrentDatabase
-Version: 0.0.2
+Version: 0.0.3
 Summary: A SQLite wrapper that allows for object oriented database access.
 Home-page: 
 Author: Jay S
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
```

### Comparing `ConcurrentDatabase-0.0.2/PKG-INFO` & `ConcurrentDatabase-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ConcurrentDatabase
-Version: 0.0.2
+Version: 0.0.3
 Summary: A SQLite wrapper that allows for object oriented database access.
 Home-page: 
 Author: Jay S
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
```

### Comparing `ConcurrentDatabase-0.0.2/README.md` & `ConcurrentDatabase-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ConcurrentDatabase-0.0.2/pyproject.toml` & `ConcurrentDatabase-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ConcurrentDatabase-0.0.2/setup.py` & `ConcurrentDatabase-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ConcurrentDatabase",
-    version="0.0.2",
+    version="0.0.3",
     author="Jay S",
     author_email="",
     description="A SQLite wrapper that allows for object oriented database access.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

