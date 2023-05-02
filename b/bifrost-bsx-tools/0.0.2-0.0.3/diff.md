# Comparing `tmp/bifrost_bsx_tools-0.0.2.tar.gz` & `tmp/bifrost_bsx_tools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bifrost_bsx_tools-0.0.2.tar", last modified: Mon Apr  3 12:15:14 2023, max compression
+gzip compressed data, was "bifrost_bsx_tools-0.0.3.tar", last modified: Tue May  2 16:10:55 2023, max compression
```

## Comparing `bifrost_bsx_tools-0.0.2.tar` & `bifrost_bsx_tools-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 vbauer    (1000) vbauer    (1000)        0 2023-04-03 12:15:14.629804 bifrost_bsx_tools-0.0.2/
--rw-rw-r--   0 vbauer    (1000) vbauer    (1000)     1058 2023-03-20 10:05:51.000000 bifrost_bsx_tools-0.0.2/LICENSE.txt
--rw-rw-r--   0 vbauer    (1000) vbauer    (1000)     4309 2023-04-03 12:15:14.629804 bifrost_bsx_tools-0.0.2/PKG-INFO
--rw-rw-r--   0 vbauer    (1000) vbauer    (1000)     2395 2023-03-20 16:10:52.000000 bifrost_bsx_tools-0.0.2/README.md
--rw-rw-r--   0 vbauer    (1000) vbauer    (1000)      858 2023-04-03 12:13:49.000000 bifrost_bsx_tools-0.0.2/pyproject.toml
--rw-rw-r--   0 vbauer    (1000) vbauer    (1000)       38 2023-04-03 12:15:14.629804 bifrost_bsx_tools-0.0.2/setup.cfg
-drwxrwxr-x   0 vbauer    (1000) vbauer    (1000)        0 2023-04-03 12:15:14.625804 bifrost_bsx_tools-0.0.2/src/
-drwxrwxr-x   0 vbauer    (1000) vbauer    (1000)        0 2023-04-03 12:15:14.629804 bifrost_bsx_tools-0.0.2/src/bifrost_bsx_tools/
--rw-rw-r--   0 vbauer    (1000) vbauer    (1000)       91 2023-03-20 13:18:07.000000 bifrost_bsx_tools-0.0.2/src/bifrost_bsx_tools/__init__.py
--rw-rw-r--   0 vbauer    (1000) vbauer    (1000)     9524 2023-03-20 15:47:41.000000 bifrost_bsx_tools-0.0.2/src/bifrost_bsx_tools/core.py
-drwxrwxr-x   0 vbauer    (1000) vbauer    (1000)        0 2023-04-03 12:15:14.629804 bifrost_bsx_tools-0.0.2/src/bifrost_bsx_tools.egg-info/
--rw-rw-r--   0 vbauer    (1000) vbauer    (1000)     4309 2023-04-03 12:15:14.000000 bifrost_bsx_tools-0.0.2/src/bifrost_bsx_tools.egg-info/PKG-INFO
--rw-rw-r--   0 vbauer    (1000) vbauer    (1000)      324 2023-04-03 12:15:14.000000 bifrost_bsx_tools-0.0.2/src/bifrost_bsx_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 vbauer    (1000) vbauer    (1000)        1 2023-04-03 12:15:14.000000 bifrost_bsx_tools-0.0.2/src/bifrost_bsx_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 vbauer    (1000) vbauer    (1000)       32 2023-04-03 12:15:14.000000 bifrost_bsx_tools-0.0.2/src/bifrost_bsx_tools.egg-info/requires.txt
--rw-rw-r--   0 vbauer    (1000) vbauer    (1000)       18 2023-04-03 12:15:14.000000 bifrost_bsx_tools-0.0.2/src/bifrost_bsx_tools.egg-info/top_level.txt
+drwxrwxr-x   0 vbauer    (1000) vbauer    (1000)        0 2023-05-02 16:10:55.138226 bifrost_bsx_tools-0.0.3/
+-rw-rw-r--   0 vbauer    (1000) vbauer    (1000)     1058 2023-03-20 10:05:51.000000 bifrost_bsx_tools-0.0.3/LICENSE.txt
+-rw-rw-r--   0 vbauer    (1000) vbauer    (1000)     4309 2023-05-02 16:10:55.138226 bifrost_bsx_tools-0.0.3/PKG-INFO
+-rw-rw-r--   0 vbauer    (1000) vbauer    (1000)     2395 2023-03-20 16:10:52.000000 bifrost_bsx_tools-0.0.3/README.md
+-rw-rw-r--   0 vbauer    (1000) vbauer    (1000)      858 2023-05-02 16:09:43.000000 bifrost_bsx_tools-0.0.3/pyproject.toml
+-rw-rw-r--   0 vbauer    (1000) vbauer    (1000)       38 2023-05-02 16:10:55.138226 bifrost_bsx_tools-0.0.3/setup.cfg
+drwxrwxr-x   0 vbauer    (1000) vbauer    (1000)        0 2023-05-02 16:10:55.134226 bifrost_bsx_tools-0.0.3/src/
+drwxrwxr-x   0 vbauer    (1000) vbauer    (1000)        0 2023-05-02 16:10:55.134226 bifrost_bsx_tools-0.0.3/src/bifrost_bsx_tools/
+-rw-rw-r--   0 vbauer    (1000) vbauer    (1000)       91 2023-03-20 13:18:07.000000 bifrost_bsx_tools-0.0.3/src/bifrost_bsx_tools/__init__.py
+-rw-rw-r--   0 vbauer    (1000) vbauer    (1000)    10794 2023-05-02 16:07:11.000000 bifrost_bsx_tools-0.0.3/src/bifrost_bsx_tools/core.py
+drwxrwxr-x   0 vbauer    (1000) vbauer    (1000)        0 2023-05-02 16:10:55.134226 bifrost_bsx_tools-0.0.3/src/bifrost_bsx_tools.egg-info/
+-rw-rw-r--   0 vbauer    (1000) vbauer    (1000)     4309 2023-05-02 16:10:55.000000 bifrost_bsx_tools-0.0.3/src/bifrost_bsx_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 vbauer    (1000) vbauer    (1000)      324 2023-05-02 16:10:55.000000 bifrost_bsx_tools-0.0.3/src/bifrost_bsx_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 vbauer    (1000) vbauer    (1000)        1 2023-05-02 16:10:55.000000 bifrost_bsx_tools-0.0.3/src/bifrost_bsx_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 vbauer    (1000) vbauer    (1000)       32 2023-05-02 16:10:55.000000 bifrost_bsx_tools-0.0.3/src/bifrost_bsx_tools.egg-info/requires.txt
+-rw-rw-r--   0 vbauer    (1000) vbauer    (1000)       18 2023-05-02 16:10:55.000000 bifrost_bsx_tools-0.0.3/src/bifrost_bsx_tools.egg-info/top_level.txt
```

### Comparing `bifrost_bsx_tools-0.0.2/LICENSE.txt` & `bifrost_bsx_tools-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bifrost_bsx_tools-0.0.2/PKG-INFO` & `bifrost_bsx_tools-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bifrost_bsx_tools
-Version: 0.0.2
+Version: 0.0.3
 Summary: Extract time series from Bifrost BSX files as pandas DataFrame.
 Author-email: Valentin Bauer <valentin.bauer@tuwien.ac.at>
 License: Copyright (c) 2023 Valentin Bauer
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
```

### Comparing `bifrost_bsx_tools-0.0.2/README.md` & `bifrost_bsx_tools-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `bifrost_bsx_tools-0.0.2/pyproject.toml` & `bifrost_bsx_tools-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bifrost_bsx_tools"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Valentin Bauer", email="valentin.bauer@tuwien.ac.at" },
 ]
 description = "Extract time series from Bifrost BSX files as pandas DataFrame."
 readme = "README.md"
 license = { file = "LICENSE.txt" }
 requires-python = ">=3.7"
```

### Comparing `bifrost_bsx_tools-0.0.2/src/bifrost_bsx_tools/core.py` & `bifrost_bsx_tools-0.0.3/src/bifrost_bsx_tools/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -247,19 +247,43 @@
         
         try:
             
             with self.bsx_archive.open(timeseries_path) as f:
             
                 try:
                     df = pd.read_csv(f, header=0)
-                    column_names = ['Timestep'] + [str(i) for i in range(len(df.columns) - 1)]
-                    df.columns = column_names
                     
+                    # rename the columns to keep only the index in the name
+                    pattern = r".*_(?P<idx>\d+)"
+                    replace = lambda m: m.group('idx')
+                    
+                    # replace the column names with the index
+                    df.columns = df.columns.str.replace(pattern, replace, regex=True)
+                    
+                    # rename the timestep column
+                    df.rename(columns={'SimulationTime[s]': 'Timestep'}, inplace=True)
                     df['Time'] = pd.to_datetime(df['Timestep'], unit='s')
                     df.set_index('Time', inplace=True)
+                    
+                    # sort the columns by their index
+                    # but the columns are strings so we need to convert to int first
+                    # but some columns are not integers, so we need to handle that
+                    
+                    # first, get the columns that are not integers
+                    non_integer_columns = [ c for c in df.columns if not c.isdigit() ]
+                    
+                    # then, get the columns that are integers
+                    integer_columns = [ c for c in df.columns if c.isdigit() ]
+                    
+                    # then, sort the integer columns
+                    integer_columns = sorted(integer_columns, key=lambda c: int(c))
+                    
+                    # then, put the columns back together
+                    df = df[non_integer_columns + integer_columns]
+                    
                     return df
                 
                 except pd.errors.EmptyDataError as e:
                     raise DynamicTimseriesParsingError(run_id, dynamic_id) from e
         
         except KeyError as e:
             raise DynamicTimeseriesNotFoundError(run_id, dynamic_id) from e
```

### Comparing `bifrost_bsx_tools-0.0.2/src/bifrost_bsx_tools.egg-info/PKG-INFO` & `bifrost_bsx_tools-0.0.3/src/bifrost_bsx_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bifrost-bsx-tools
-Version: 0.0.2
+Version: 0.0.3
 Summary: Extract time series from Bifrost BSX files as pandas DataFrame.
 Author-email: Valentin Bauer <valentin.bauer@tuwien.ac.at>
 License: Copyright (c) 2023 Valentin Bauer
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
```

