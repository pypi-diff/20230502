# Comparing `tmp/hkfdb-2.76.tar.gz` & `tmp/hkfdb-2.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hkfdb-2.76.tar", last modified: Tue May  2 16:08:53 2023, max compression
+gzip compressed data, was "hkfdb-2.77.tar", last modified: Tue May  2 16:14:02 2023, max compression
```

## Comparing `hkfdb-2.76.tar` & `hkfdb-2.77.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 16:08:53.281451 hkfdb-2.76/
--rw-rw-rw-   0        0        0    35149 2021-07-30 00:33:11.000000 hkfdb-2.76/LICENSE
--rw-rw-rw-   0        0        0     1652 2023-05-02 16:08:53.281451 hkfdb-2.76/PKG-INFO
--rw-rw-rw-   0        0        0     1243 2023-03-30 03:29:25.000000 hkfdb-2.76/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 16:08:53.275156 hkfdb-2.76/hkfdb/
--rw-rw-rw-   0        0        0    90857 2023-05-02 16:08:15.000000 hkfdb-2.76/hkfdb/Database.py
--rw-rw-rw-   0        0        0       23 2021-09-12 13:30:45.000000 hkfdb-2.76/hkfdb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 16:08:53.280212 hkfdb-2.76/hkfdb.egg-info/
--rw-rw-rw-   0        0        0     1652 2023-05-02 16:08:53.000000 hkfdb-2.76/hkfdb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-05-02 16:08:53.000000 hkfdb-2.76/hkfdb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 16:08:53.000000 hkfdb-2.76/hkfdb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-02 16:08:53.000000 hkfdb-2.76/hkfdb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-02 16:08:53.000000 hkfdb-2.76/hkfdb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 16:08:53.281451 hkfdb-2.76/setup.cfg
--rw-rw-rw-   0        0        0      762 2023-05-02 16:08:30.000000 hkfdb-2.76/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 16:14:02.933984 hkfdb-2.77/
+-rw-rw-rw-   0        0        0    35149 2021-07-30 00:33:11.000000 hkfdb-2.77/LICENSE
+-rw-rw-rw-   0        0        0     1652 2023-05-02 16:14:02.933984 hkfdb-2.77/PKG-INFO
+-rw-rw-rw-   0        0        0     1243 2023-03-30 03:29:25.000000 hkfdb-2.77/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 16:14:02.933984 hkfdb-2.77/hkfdb/
+-rw-rw-rw-   0        0        0    91011 2023-05-02 16:13:10.000000 hkfdb-2.77/hkfdb/Database.py
+-rw-rw-rw-   0        0        0       23 2021-09-12 13:30:45.000000 hkfdb-2.77/hkfdb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 16:14:02.933984 hkfdb-2.77/hkfdb.egg-info/
+-rw-rw-rw-   0        0        0     1652 2023-05-02 16:14:02.000000 hkfdb-2.77/hkfdb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2023-05-02 16:14:02.000000 hkfdb-2.77/hkfdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 16:14:02.000000 hkfdb-2.77/hkfdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-02 16:14:02.000000 hkfdb-2.77/hkfdb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-02 16:14:02.000000 hkfdb-2.77/hkfdb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 16:14:02.933984 hkfdb-2.77/setup.cfg
+-rw-rw-rw-   0        0        0      762 2023-05-02 16:13:52.000000 hkfdb-2.77/setup.py
```

### Comparing `hkfdb-2.76/LICENSE` & `hkfdb-2.77/LICENSE`

 * *Files identical despite different names*

### Comparing `hkfdb-2.76/PKG-INFO` & `hkfdb-2.77/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkfdb
-Version: 2.76
+Version: 2.77
 Summary: Hong Kong Finance Database.
 Home-page: https://www.hkfdb.net
 Author: Hong Kong Finance Database Team
 Author-email: info@hkfdb.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hkfdb-2.76/README.md` & `hkfdb-2.77/README.md`

 * *Files identical despite different names*

### Comparing `hkfdb-2.76/hkfdb/Database.py` & `hkfdb-2.77/hkfdb/Database.py`

 * *Files 0% similar despite different names*

```diff
@@ -1473,14 +1473,16 @@
                             df = pd.DataFrame(content, columns=columns)
                             df['date'] = pd.to_datetime(df['date'], format='%Y%m%d')
                             df['listing_date'] = pd.to_datetime(df['listing_date'], format='%Y%m%d')
                             df_list.append(df)
 
                 df = pd.concat(df_list)
                 df = df.sort_values('date')
+                df['num_of_cbbc_sold'] = df['num_of_cbbc_sold'].abs()
+                df['avg_price_per_cbbc_sold'] = df['avg_price_per_cbbc_sold'].abs()
                 df['bull_bear'] = df['bull_bear'].str.replace(' ','')
                 df = df.set_index('unique_id')
                 # df = df.drop('index', axis=1)
 
                 return df
 
         else:
```

### Comparing `hkfdb-2.76/hkfdb.egg-info/PKG-INFO` & `hkfdb-2.77/hkfdb.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkfdb
-Version: 2.76
+Version: 2.77
 Summary: Hong Kong Finance Database.
 Home-page: https://www.hkfdb.net
 Author: Hong Kong Finance Database Team
 Author-email: info@hkfdb.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hkfdb-2.76/setup.py` & `hkfdb-2.77/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hkfdb",
-    version="2.76",
+    version="2.77",
     author="Hong Kong Finance Database Team",
     author_email="info@hkfdb.net",
     description="Hong Kong Finance Database.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.hkfdb.net",
     packages=setuptools.find_packages(),
```

