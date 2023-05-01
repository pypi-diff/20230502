# Comparing `tmp/database_knotinfo-21.7.tar.gz` & `tmp/database_knotinfo-21.7.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/database_knotinfo/database_knotinfo/dist/tmp0mbxm01k/database_knotinfo-21.7.tar", last modified: Thu Jul  1 14:38:36 2021, max compression
+gzip compressed data, was "/home/runner/work/database_knotinfo/database_knotinfo/dist/tmpsb79pfa7/database_knotinfo-21.7.15.tar", last modified: Thu Jul 15 16:21:03 2021, max compression
```

## Comparing `database_knotinfo-21.7.tar` & `database_knotinfo-21.7.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 14:38:36.000000 database_knotinfo-21.7/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 14:38:36.000000 database_knotinfo-21.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 14:38:36.000000 database_knotinfo-21.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     3022 2021-07-01 14:38:26.000000 database_knotinfo-21.7/.github/workflows/check_version_changed.yml
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2021-07-01 14:38:26.000000 database_knotinfo-21.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-07-01 14:38:26.000000 database_knotinfo-21.7/MANIFEST
--rw-r--r--   0 runner    (1001) docker     (121)       41 2021-07-01 14:38:26.000000 database_knotinfo-21.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2720 2021-07-01 14:38:36.000000 database_knotinfo-21.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2189 2021-07-01 14:38:26.000000 database_knotinfo-21.7/README.md
--rwxr-xr-x   0 runner    (1001) docker     (121)     3705 2021-07-01 14:38:26.000000 database_knotinfo-21.7/create_knotinfo_csv.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 14:38:36.000000 database_knotinfo-21.7/database_knotinfo/
--rw-r--r--   0 runner    (1001) docker     (121)     2686 2021-07-01 14:38:26.000000 database_knotinfo-21.7/database_knotinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2322 2021-07-01 14:38:26.000000 database_knotinfo-21.7/database_knotinfo/__init__.pyc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 14:38:36.000000 database_knotinfo-21.7/database_knotinfo/csv_data/
--rw-r--r--   0 runner    (1001) docker     (121)  8985808 2021-07-01 14:38:27.000000 database_knotinfo-21.7/database_knotinfo/csv_data/knotinfo_data_complete.csv
--rw-r--r--   0 runner    (1001) docker     (121) 15323687 2021-07-01 14:38:26.000000 database_knotinfo-21.7/database_knotinfo/csv_data/linkinfo_data_complete.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 14:38:36.000000 database_knotinfo-21.7/database_knotinfo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2720 2021-07-01 14:38:36.000000 database_knotinfo-21.7/database_knotinfo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      495 2021-07-01 14:38:36.000000 database_knotinfo-21.7/database_knotinfo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-01 14:38:36.000000 database_knotinfo-21.7/database_knotinfo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-07-01 14:38:36.000000 database_knotinfo-21.7/database_knotinfo.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)      469 2021-07-01 14:38:26.000000 database_knotinfo-21.7/get_release_tag.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      888 2021-07-01 14:38:26.000000 database_knotinfo-21.7/new_version_tag.sh
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-07-01 14:38:36.000000 database_knotinfo-21.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1399 2021-07-01 14:38:26.000000 database_knotinfo-21.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-15 16:21:03.000000 database_knotinfo-21.7.15/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-15 16:21:03.000000 database_knotinfo-21.7.15/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-15 16:21:03.000000 database_knotinfo-21.7.15/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     3022 2021-07-15 16:20:51.000000 database_knotinfo-21.7.15/.github/workflows/check_version_changed.yml
+-rw-r--r--   0 runner    (1001) docker     (121)    35149 2021-07-15 16:20:51.000000 database_knotinfo-21.7.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2021-07-15 16:20:51.000000 database_knotinfo-21.7.15/MANIFEST
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2021-07-15 16:20:51.000000 database_knotinfo-21.7.15/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2938 2021-07-15 16:21:03.000000 database_knotinfo-21.7.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2404 2021-07-15 16:20:51.000000 database_knotinfo-21.7.15/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3705 2021-07-15 16:20:51.000000 database_knotinfo-21.7.15/create_knotinfo_csv.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-15 16:21:03.000000 database_knotinfo-21.7.15/database_knotinfo/
+-rw-r--r--   0 runner    (1001) docker     (121)     2951 2021-07-15 16:20:51.000000 database_knotinfo-21.7.15/database_knotinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2021-07-15 16:20:52.000000 database_knotinfo-21.7.15/database_knotinfo/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-15 16:21:03.000000 database_knotinfo-21.7.15/database_knotinfo/csv_data/
+-rw-r--r--   0 runner    (1001) docker     (121)  8985808 2021-07-15 16:20:52.000000 database_knotinfo-21.7.15/database_knotinfo/csv_data/knotinfo_data_complete.csv
+-rw-r--r--   0 runner    (1001) docker     (121) 15323687 2021-07-15 16:20:51.000000 database_knotinfo-21.7.15/database_knotinfo/csv_data/linkinfo_data_complete.csv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-15 16:21:03.000000 database_knotinfo-21.7.15/database_knotinfo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2938 2021-07-15 16:21:03.000000 database_knotinfo-21.7.15/database_knotinfo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2021-07-15 16:21:03.000000 database_knotinfo-21.7.15/database_knotinfo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-15 16:21:03.000000 database_knotinfo-21.7.15/database_knotinfo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2021-07-15 16:21:03.000000 database_knotinfo-21.7.15/database_knotinfo.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)      430 2021-07-15 16:20:51.000000 database_knotinfo-21.7.15/get_release_tag.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)      978 2021-07-15 16:20:51.000000 database_knotinfo-21.7.15/new_version_tag.sh
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2021-07-15 16:21:03.000000 database_knotinfo-21.7.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1399 2021-07-15 16:20:51.000000 database_knotinfo-21.7.15/setup.py
```

### Comparing `database_knotinfo-21.7/.github/workflows/check_version_changed.yml` & `database_knotinfo-21.7.15/.github/workflows/check_version_changed.yml`

 * *Files identical despite different names*

### Comparing `database_knotinfo-21.7/LICENSE` & `database_knotinfo-21.7.15/LICENSE`

 * *Files identical despite different names*

### Comparing `database_knotinfo-21.7/PKG-INFO` & `database_knotinfo-21.7.15/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database_knotinfo
-Version: 21.7
+Version: 21.7.15
 Summary: The KnotInfo and LinkInfo databases as lists of dictionaries
 Home-page: https://github.com/soehms/database_knotinfo
 Author: Sebastian Oehms
 Author-email: seb.oehms@gmail.com
 License: GPL
 Keywords: KnotInfo,LinkInfo,SageMath,database,knot,link,mathematics,topology,invariants
 Platform: UNKNOWN
@@ -58,16 +58,18 @@
 >>> l2 = l[2]
 >>> l2['name']
 'L2a1{1}'
 >>> l2['homflypt_polynomial']
 'v/z-v^3/z + v*z'
 ```
 
-To build a new release, the `CSV` files can be upgraded
-with the `create_knotinfo_csv.py` script.
+To build a new release, the `CSV` files can be upgraded with the
+`create_knotinfo_csv.py` script. A [cronjob](https://github.com/soehms/database_knotinfo/blob/main/.github/workflows/check_version_changed.yml)
+executes it on the first day of every month and creates a new
+release if differences are detected.
 
 ## Installation
 
 ### Python
 
 ```bash
 pip install database_knotinfo
@@ -89,20 +91,20 @@
 ```
 
 ## Versioning
 
 Version numbers are automatically generated every month if differences to the
 original databases are detected. They follow the scheme
 
-\<year of the century\>.\<month\>
+\<year of the century\>.\<month\>.\<day\>
 
 ## Help
 
-If you note an divergence between this repository and the original data in case
-the the current release is older as a month please create an issue about that.
+If you note a divergence between this repository and the original data in case
+the current release is older than a month please create an issue about that.
 
 ## Credits
 
 Many thanks to Chuck Livingston and Allison Moore for making the data
 available. For further acknowledgments see the corresponding homepages.
```

### Comparing `database_knotinfo-21.7/README.md` & `database_knotinfo-21.7.15/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -43,16 +43,18 @@
 >>> l2 = l[2]
 >>> l2['name']
 'L2a1{1}'
 >>> l2['homflypt_polynomial']
 'v/z-v^3/z + v*z'
 ```
 
-To build a new release, the `CSV` files can be upgraded
-with the `create_knotinfo_csv.py` script.
+To build a new release, the `CSV` files can be upgraded with the
+`create_knotinfo_csv.py` script. A [cronjob](https://github.com/soehms/database_knotinfo/blob/main/.github/workflows/check_version_changed.yml)
+executes it on the first day of every month and creates a new
+release if differences are detected.
 
 ## Installation
 
 ### Python
 
 ```bash
 pip install database_knotinfo
@@ -74,18 +76,18 @@
 ```
 
 ## Versioning
 
 Version numbers are automatically generated every month if differences to the
 original databases are detected. They follow the scheme
 
-\<year of the century\>.\<month\>
+\<year of the century\>.\<month\>.\<day\>
 
 ## Help
 
-If you note an divergence between this repository and the original data in case
-the the current release is older as a month please create an issue about that.
+If you note a divergence between this repository and the original data in case
+the current release is older than a month please create an issue about that.
 
 ## Credits
 
 Many thanks to Chuck Livingston and Allison Moore for making the data
 available. For further acknowledgments see the corresponding homepages.
```

### Comparing `database_knotinfo-21.7/create_knotinfo_csv.py` & `database_knotinfo-21.7.15/create_knotinfo_csv.py`

 * *Files identical despite different names*

### Comparing `database_knotinfo-21.7/database_knotinfo/__init__.py` & `database_knotinfo-21.7.15/database_knotinfo/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,7 +86,20 @@
     csv_path = os.path.join(package_path, Names.csv_path.value)
 
     link_csv = open(os.path.join(csv_path, filename))
     link_dict = csv.DictReader(link_csv, delimiter=Names.delimiter.value)
     link_list = list(link_dict)
     link_csv.close()
     return link_list
+
+def version():
+    r"""
+    Return the current version of the databases.
+
+    EXAMPLES::
+
+        >>> from database_knotinfo import version
+        >>> version()
+        '21.07.15'
+    """
+    from database_knotinfo import __version__
+    return __version__.value
```

### Comparing `database_knotinfo-21.7/database_knotinfo/csv_data/knotinfo_data_complete.csv` & `database_knotinfo-21.7.15/database_knotinfo/csv_data/knotinfo_data_complete.csv`

 * *Files identical despite different names*

### Comparing `database_knotinfo-21.7/database_knotinfo/csv_data/linkinfo_data_complete.csv` & `database_knotinfo-21.7.15/database_knotinfo/csv_data/linkinfo_data_complete.csv`

 * *Files identical despite different names*

### Comparing `database_knotinfo-21.7/database_knotinfo.egg-info/PKG-INFO` & `database_knotinfo-21.7.15/database_knotinfo.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-knotinfo
-Version: 21.7
+Version: 21.7.15
 Summary: The KnotInfo and LinkInfo databases as lists of dictionaries
 Home-page: https://github.com/soehms/database_knotinfo
 Author: Sebastian Oehms
 Author-email: seb.oehms@gmail.com
 License: GPL
 Keywords: KnotInfo,LinkInfo,SageMath,database,knot,link,mathematics,topology,invariants
 Platform: UNKNOWN
@@ -58,16 +58,18 @@
 >>> l2 = l[2]
 >>> l2['name']
 'L2a1{1}'
 >>> l2['homflypt_polynomial']
 'v/z-v^3/z + v*z'
 ```
 
-To build a new release, the `CSV` files can be upgraded
-with the `create_knotinfo_csv.py` script.
+To build a new release, the `CSV` files can be upgraded with the
+`create_knotinfo_csv.py` script. A [cronjob](https://github.com/soehms/database_knotinfo/blob/main/.github/workflows/check_version_changed.yml)
+executes it on the first day of every month and creates a new
+release if differences are detected.
 
 ## Installation
 
 ### Python
 
 ```bash
 pip install database_knotinfo
@@ -89,20 +91,20 @@
 ```
 
 ## Versioning
 
 Version numbers are automatically generated every month if differences to the
 original databases are detected. They follow the scheme
 
-\<year of the century\>.\<month\>
+\<year of the century\>.\<month\>.\<day\>
 
 ## Help
 
-If you note an divergence between this repository and the original data in case
-the the current release is older as a month please create an issue about that.
+If you note a divergence between this repository and the original data in case
+the current release is older than a month please create an issue about that.
 
 ## Credits
 
 Many thanks to Chuck Livingston and Allison Moore for making the data
 available. For further acknowledgments see the corresponding homepages.
```

### Comparing `database_knotinfo-21.7/new_version_tag.sh` & `database_knotinfo-21.7.15/new_version_tag.sh`

 * *Files 10% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 # This script is used by GitHub Action .github/workflows/check_version_changed.yml
 # It checks if create_knotinfo_csv.py did find new content in the databases.
 # In that case the changes are commited and a new version tag is created.
 # Please don't use this scrip for other purpose!
 GIT_DIFF=`git diff`
 if [ -n "$GIT_DIFF" ]
 then
+    DAY=$(date +%d)
     MONTH=$(date +%m)
     YEAR=$(date +%g)
-    TAG=$YEAR"."$MONTH
+    TAG=$YEAR"."$MONTH"."$DAY
     COMMIT_MSG="automatic upgrade to version "$TAG" on "$(date +%F)
+    echo "value = '"$TAG"'" > database_knotinfo/__version__.py
     git config user.email "seb.oehms@gmail.com"
     git config user.name "Sebastian Oehms"
     git commit -m "$COMMIT_MSG" .
     echo "New version "$TAG" commited"
     git push
     echo "New database content pushed to repository"
     git tag -a -m "$COMMIT_MSG" $TAG
```

### Comparing `database_knotinfo-21.7/setup.py` & `database_knotinfo-21.7.15/setup.py`

 * *Files identical despite different names*

