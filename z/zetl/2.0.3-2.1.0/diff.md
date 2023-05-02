# Comparing `tmp/zetl-2.0.3.tar.gz` & `tmp/zetl-2.1.0.tar.gz`

## Comparing `zetl-2.0.3.tar` & `zetl-2.1.0.tar`

### file list

```diff
@@ -1,48 +1,50 @@
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 zetl-2.0.3/src/zetl/.schemawiz_config3
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 zetl-2.0.3/src/zetl/1.CURRENT_DATE.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zetl-2.0.3/src/zetl/__init__.py
--rw-r--r--   0        0        0    40960 2020-02-02 00:00:00.000000 zetl-2.0.3/src/zetl/local_sqlite_db
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 zetl-2.0.3/src/zetl/mysql_export.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 zetl-2.0.3/src/zetl/mysql_extract.py
--rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 zetl-2.0.3/src/zetl/mysql_import.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 zetl-2.0.3/src/zetl/postgres_export.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 zetl-2.0.3/src/zetl/postgres_extract.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 zetl-2.0.3/src/zetl/postgres_import.py
--rw-r--r--   0        0        0    26189 2020-02-02 00:00:00.000000 zetl-2.0.3/src/zetl/run.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zetl-2.0.3/src/zetl/sample.csv
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 zetl-2.0.3/src/zetl/sqlite_export.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 zetl-2.0.3/src/zetl/sqlite_extract.py
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 zetl-2.0.3/src/zetl/sqlite_import.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 zetl-2.0.3/src/zetl/view.py
--rw-r--r--   0        0        0    32768 2020-02-02 00:00:00.000000 zetl-2.0.3/src/zetl/zetl.db
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 zetl-2.0.3/src/zetl/zetl_this_file.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 zetl-2.0.3/src/zetl/zetl_this_folder.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 zetl-2.0.3/src/zetl/zetl_scripts/test/1.check.sql
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 zetl-2.0.3/src/zetl/zetl_scripts/test/another_mysqlcheck.sql
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 zetl-2.0.3/src/zetl/zetl_scripts/test/another_postgrescheck.sql
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 zetl-2.0.3/src/zetl/zetl_scripts/test/postgrescheck.sql
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 zetl-2.0.3/src/zetl/zetl_scripts/test/z_etl.csv
--rwxr-xr-x   0        0        0       69 2020-02-02 00:00:00.000000 zetl-2.0.3/tests/chk_zetl.bat
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 zetl-2.0.3/tests/floats.csv
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zetl-2.0.3/tests/sample.csv
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 zetl-2.0.3/tests/sample.tsv
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 zetl-2.0.3/tests/sampletable.ddl
--rw-r--r--   0        0        0    50392 2020-02-02 00:00:00.000000 zetl-2.0.3/tests/tesla.csv
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 zetl-2.0.3/tests/zetl.db
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 zetl-2.0.3/tests/zetl_scripts/demo1/1.hello.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 zetl-2.0.3/tests/zetl_scripts/demo1/2.somethings.sql
--rwxr-xr-x   0        0        0      212 2020-02-02 00:00:00.000000 zetl-2.0.3/tests/zetl_scripts/demo1/3.hello.bat
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 zetl-2.0.3/tests/zetl_scripts/demo1/z_etl.csv
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 zetl-2.0.3/tests/zetl_scripts/demo2/1.somethings.sql
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 zetl-2.0.3/tests/zetl_scripts/demo2/z_etl.csv
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 zetl-2.0.3/tests/zetl_scripts/demo3/1.tms.sql
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 zetl-2.0.3/tests/zetl_scripts/demo3/z_etl.csv
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 zetl-2.0.3/tests/zetl_scripts/empty_log/1.truncate_zlog.sql
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 zetl-2.0.3/tests/zetl_scripts/empty_log/z_etl.csv
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 zetl-2.0.3/tests/zetl_scripts/view_log/1.latest_log_view.sql
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 zetl-2.0.3/tests/zetl_scripts/view_log/z_etl.csv
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 zetl-2.0.3/.gitignore
--rw-r--r--   0        0        0    18431 2020-02-02 00:00:00.000000 zetl-2.0.3/LICENSE
--rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 zetl-2.0.3/README.md
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 zetl-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 zetl-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 zetl-2.1.0/src/zetl/.schemawiz_config3
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 zetl-2.1.0/src/zetl/1.CURRENT_DATE.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zetl-2.1.0/src/zetl/__init__.py
+-rw-r--r--   0        0        0    40960 2020-02-02 00:00:00.000000 zetl-2.1.0/src/zetl/local_sqlite_db
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 zetl-2.1.0/src/zetl/mysql_export.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 zetl-2.1.0/src/zetl/mysql_extract.py
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 zetl-2.1.0/src/zetl/mysql_import.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 zetl-2.1.0/src/zetl/postgres_export.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 zetl-2.1.0/src/zetl/postgres_extract.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 zetl-2.1.0/src/zetl/postgres_import.py
+-rw-r--r--   0        0        0    26189 2020-02-02 00:00:00.000000 zetl-2.1.0/src/zetl/run.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zetl-2.1.0/src/zetl/sample.csv
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 zetl-2.1.0/src/zetl/sample7.csv
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 zetl-2.1.0/src/zetl/sqlite_export.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 zetl-2.1.0/src/zetl/sqlite_extract.py
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 zetl-2.1.0/src/zetl/sqlite_import.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 zetl-2.1.0/src/zetl/view.py
+-rw-r--r--   0        0        0    32768 2020-02-02 00:00:00.000000 zetl-2.1.0/src/zetl/zetl.db
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 zetl-2.1.0/src/zetl/zetl_this_file.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 zetl-2.1.0/src/zetl/zetl_this_folder.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 zetl-2.1.0/src/zetl/zetl_scripts/test/1.check.sql
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 zetl-2.1.0/src/zetl/zetl_scripts/test/another_mysqlcheck.sql
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 zetl-2.1.0/src/zetl/zetl_scripts/test/another_postgrescheck.sql
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 zetl-2.1.0/src/zetl/zetl_scripts/test/postgrescheck.sql
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 zetl-2.1.0/src/zetl/zetl_scripts/test/z_etl.csv
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 zetl-2.1.0/tests/.schemawiz_config3
+-rwxr-xr-x   0        0        0      316 2020-02-02 00:00:00.000000 zetl-2.1.0/tests/backup.bat
+-rwxr-xr-x   0        0        0       69 2020-02-02 00:00:00.000000 zetl-2.1.0/tests/chk_zetl.bat
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 zetl-2.1.0/tests/floats.csv
+-rw-r--r--   0        0        0    24576 2020-02-02 00:00:00.000000 zetl-2.1.0/tests/local_sqlite_db
+-rwxr-xr-x   0        0        0      295 2020-02-02 00:00:00.000000 zetl-2.1.0/tests/restore.bat
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zetl-2.1.0/tests/sample.csv
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 zetl-2.1.0/tests/sample.tsv
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 zetl-2.1.0/tests/sampletable.ddl
+-rw-r--r--   0        0        0    50392 2020-02-02 00:00:00.000000 zetl-2.1.0/tests/tesla.csv
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 zetl-2.1.0/tests/z_etl.csv
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 zetl-2.1.0/tests/z_log.csv
+-rwxr-xr-x   0        0        0      237 2020-02-02 00:00:00.000000 zetl-2.1.0/tests/zetl_scripts/backup/15.extract_csv_files.bat
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 zetl-2.1.0/tests/zetl_scripts/backup/z_etl.csv
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 zetl-2.1.0/tests/zetl_scripts/demo2/1.somethings.sql
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 zetl-2.1.0/tests/zetl_scripts/demo3/1.tms.sql
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 zetl-2.1.0/tests/zetl_scripts/empty_log/1.truncate_zlog.sql
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-2.1.0/tests/zetl_scripts/empty_log/z_etl.csv
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 zetl-2.1.0/tests/zetl_scripts/view_log/1.latest_log_view.sql
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 zetl-2.1.0/tests/zetl_scripts/view_log/z_etl.csv
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 zetl-2.1.0/.gitignore
+-rw-r--r--   0        0        0    18431 2020-02-02 00:00:00.000000 zetl-2.1.0/LICENSE
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 zetl-2.1.0/README.md
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 zetl-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 zetl-2.1.0/PKG-INFO
```

### Comparing `zetl-2.0.3/src/zetl/local_sqlite_db` & `zetl-2.1.0/src/zetl/local_sqlite_db`

 * *Files identical despite different names*

### Comparing `zetl-2.0.3/src/zetl/mysql_export.py` & `zetl-2.1.0/src/zetl/mysql_export.py`

 * *Files identical despite different names*

### Comparing `zetl-2.0.3/src/zetl/mysql_extract.py` & `zetl-2.1.0/src/zetl/mysql_extract.py`

 * *Files identical despite different names*

### Comparing `zetl-2.0.3/src/zetl/mysql_import.py` & `zetl-2.1.0/src/zetl/mysql_import.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,12 +64,12 @@
 				newfile += partlist[i] + filedelimiter
 
 		newfile += ddl_output_filename
 		return newfile
 
 if __name__ == '__main__':
 	# myexp = dbimport('sample.csv','sample8',True)
-	# tbl = schemawiz().createload_mysql_from_csv('CanadianPostalCodes.csv','thistbl')
-
+	#tbl = schemawiz().createload_mysql_from_csv('sample7.csv','restored_sample7')
+ 
 	main()
```

### Comparing `zetl-2.0.3/src/zetl/postgres_export.py` & `zetl-2.1.0/src/zetl/postgres_export.py`

 * *Files identical despite different names*

### Comparing `zetl-2.0.3/src/zetl/postgres_extract.py` & `zetl-2.1.0/src/zetl/postgres_extract.py`

 * *Files identical despite different names*

### Comparing `zetl-2.0.3/src/zetl/postgres_import.py` & `zetl-2.1.0/src/zetl/postgres_import.py`

 * *Files identical despite different names*

### Comparing `zetl-2.0.3/src/zetl/run.py` & `zetl-2.1.0/src/zetl/run.py`

 * *Files identical despite different names*

### Comparing `zetl-2.0.3/src/zetl/sqlite_export.py` & `zetl-2.1.0/src/zetl/sqlite_export.py`

 * *Files identical despite different names*

### Comparing `zetl-2.0.3/src/zetl/sqlite_extract.py` & `zetl-2.1.0/src/zetl/sqlite_extract.py`

 * *Files identical despite different names*

### Comparing `zetl-2.0.3/src/zetl/sqlite_import.py` & `zetl-2.1.0/src/zetl/sqlite_import.py`

 * *Files identical despite different names*

### Comparing `zetl-2.0.3/src/zetl/view.py` & `zetl-2.1.0/src/zetl/view.py`

 * *Files identical despite different names*

### Comparing `zetl-2.0.3/src/zetl/zetl.db` & `zetl-2.1.0/src/zetl/zetl.db`

 * *Files identical despite different names*

### Comparing `zetl-2.0.3/src/zetl/zetl_this_file.py` & `zetl-2.1.0/src/zetl/zetl_this_file.py`

 * *Files identical despite different names*

### Comparing `zetl-2.0.3/src/zetl/zetl_this_folder.py` & `zetl-2.1.0/src/zetl/zetl_this_folder.py`

 * *Files identical despite different names*

### Comparing `zetl-2.0.3/tests/tesla.csv` & `zetl-2.1.0/tests/tesla.csv`

 * *Files identical despite different names*

### Comparing `zetl-2.0.3/LICENSE` & `zetl-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zetl-2.0.3/README.md` & `zetl-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `zetl-2.0.3/pyproject.toml` & `zetl-2.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [build-system]
 requires = ["hatchling","schemawizard_package","postgresdave_package","mysqldave_package","garbledave_package"]
 
 build-backend = "hatchling.build"
 
 [project]
 name = "zetl"
-version = "2.0.3"
+version = "2.1.0"
 dependencies = [
-  'schemawizard_package >= 2.2.9',
-  'postgresdave_package >= 1.7.6',
-  'mysqldave_package >= 1.3.7',
+  'schemawizard_package >= 2.5.1',
+  'postgresdave_package >= 1.8.0',
+  'mysqldave_package >= 1.5.0',
+  'sqlitedave_package >= 1.3.0',
   'garbledave_package >= 1.0.0 '
 ]
 authors = [
   { name="Dave Skura", email="dskura@gmail.com" },
 ]
 description = "A simple ETL framework for Python, SQL and BAT files which uses a Postgres database for activity logging."
 readme = "README.md"
```

### Comparing `zetl-2.0.3/PKG-INFO` & `zetl-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: zetl
-Version: 2.0.3
+Version: 2.1.0
 Summary: A simple ETL framework for Python, SQL and BAT files which uses a Postgres database for activity logging.
 Project-URL: Homepage, https://github.com/daveskura/zetl
 Project-URL: Author Linkedin, https://www.linkedin.com/in/2166883
 Author-email: Dave Skura <dskura@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: garbledave-package>=1.0.0
-Requires-Dist: mysqldave-package>=1.3.7
-Requires-Dist: postgresdave-package>=1.7.6
-Requires-Dist: schemawizard-package>=2.2.9
+Requires-Dist: mysqldave-package>=1.5.0
+Requires-Dist: postgresdave-package>=1.8.0
+Requires-Dist: schemawizard-package>=2.5.1
+Requires-Dist: sqlitedave-package>=1.3.0
 Description-Content-Type: text/markdown
 
 A simple ETL framework for Python, SQL and BAT files which uses a Postgres database for activity logging.
 the zetl framework requires python and Postgres to run.
 
 ---
```

