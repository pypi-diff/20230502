# Comparing `tmp/schemawizard_package-2.4.0.tar.gz` & `tmp/schemawizard_package-2.5.0.tar.gz`

## Comparing `schemawizard_package-2.4.0.tar` & `schemawizard_package-2.5.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/dateformat_readme.md
--rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/methods.md
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/src/schemawizard_package/.schemawiz_config1
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/src/schemawizard_package/.schemawiz_config2
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/src/schemawizard_package/.schemawiz_config3
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/src/schemawizard_package/__init__.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/src/schemawizard_package/a.csv
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/src/schemawizard_package/floats.csv
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/src/schemawizard_package/postgres_data.tsv
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/src/schemawizard_package/sample7.csv
--rw-r--r--   0        0        0    34587 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/src/schemawizard_package/schemawizard.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/src/schemawizard_package/sqlite.station_years.ddl
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/src/schemawizard_package/sqlite.tablea.ddl
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/src/schemawizard_package/sqlite.tablec.ddl
--rw-r--r--   0        0        0   106414 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/src/schemawizard_package/station_months.tsv
--rw-r--r--   0        0        0   503697 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/src/schemawizard_package/station_years.tsv
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/src/schemawizard_package/z.canweather.station_years.ddl
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/tests/chk_ddl.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/tests/create_and_load.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/tests/create_and_load_mysql.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/tests/create_and_load_postgres.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/tests/csv_load.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/tests/floats.csv
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/tests/generate_bigqueryddl.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/tests/generate_ddl_knowing_delimiter.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/tests/generate_externalbigqueryddl.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/tests/generate_mysqlddl.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/tests/generate_postgresddl.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/tests/load_mysql.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/tests/load_postgres.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/tests/sample.csv
--rw-r--r--   0        0        0    50392 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/tests/tesla.csv
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/tests/tester.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/LICENSE
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/README.md
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/pyproject.toml
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 schemawizard_package-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/dateformat_readme.md
+-rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/methods.md
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/src/schemawizard_package/.schemawiz_config1
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/src/schemawizard_package/.schemawiz_config2
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/src/schemawizard_package/.schemawiz_config3
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/src/schemawizard_package/__init__.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/src/schemawizard_package/a.csv
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/src/schemawizard_package/floats.csv
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/src/schemawizard_package/postgres_data.tsv
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/src/schemawizard_package/sample7.csv
+-rw-r--r--   0        0        0    35077 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/src/schemawizard_package/schemawizard.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/src/schemawizard_package/sqlite.station_years.ddl
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/src/schemawizard_package/sqlite.tablea.ddl
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/src/schemawizard_package/sqlite.tablec.ddl
+-rw-r--r--   0        0        0   106414 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/src/schemawizard_package/station_months.tsv
+-rw-r--r--   0        0        0   503697 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/src/schemawizard_package/station_years.tsv
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/src/schemawizard_package/testcase1.csv
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/src/schemawizard_package/z.canweather.station_years.ddl
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/tests/chk_ddl.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/tests/create_and_load.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/tests/create_and_load_mysql.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/tests/create_and_load_postgres.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/tests/csv_load.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/tests/floats.csv
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/tests/generate_bigqueryddl.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/tests/generate_ddl_knowing_delimiter.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/tests/generate_externalbigqueryddl.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/tests/generate_mysqlddl.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/tests/generate_postgresddl.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/tests/load_mysql.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/tests/load_postgres.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/tests/sample.csv
+-rw-r--r--   0        0        0    50392 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/tests/tesla.csv
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/tests/tester.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/LICENSE
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/README.md
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 schemawizard_package-2.5.0/PKG-INFO
```

### Comparing `schemawizard_package-2.4.0/dateformat_readme.md` & `schemawizard_package-2.5.0/dateformat_readme.md`

 * *Files identical despite different names*

### Comparing `schemawizard_package-2.4.0/methods.md` & `schemawizard_package-2.5.0/methods.md`

 * *Files identical despite different names*

### Comparing `schemawizard_package-2.4.0/src/schemawizard_package/schemawizard.py` & `schemawizard_package-2.5.0/src/schemawizard_package/schemawizard.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from sqlitedave_package.sqlitedave import sqlite_db
 from postgresdave_package.postgresdave import postgres_db 
 from mysqldave_package.mysqldave import mysql_db 
 from garbledave_package.garbledave import garbledave 
 
 def main():
 	obj = schemawiz()
-	#obj.loadcsvfile('floats.csv')
-	#print(obj.guess_postgres_ddl())
+	obj.loadcsvfile('testcase1.csv')
+	print(obj.guess_sqlite_ddl('testcase1'))
 	
 	#tbl = obj.createload_postgres_from_csv('projects.tsv','gcp_projects')
 
 """	
 	csvfilename = 'a.csv'
 	ddl = obj.guess_postgres_ddl(csvfilename.replace('.','_'))
 	print(ddl)
@@ -341,14 +341,15 @@
 class schemawiz:	
 	def __init__(self,csvfilename=''):
 		self.version=2.0
 		self.dbthings = dbthinger()
 		self.force_delimiter = ''
 		self.lastcall_tablename = ''
 		self.delimiter = ''
+		self.delimiter_replace = '^~^'
 		self.logging_on = False
 		self.SomeFileContents = []
 		self.column_names = []
 		self.column_datatypes = []
 		self.BigQuery_datatypes = []
 		self.mysql_datatypes = []
 		self.sqlite_datatypes = []
@@ -578,15 +579,17 @@
 					if (linecount>100):
 						break
 			
 			#self.logger('file has ' + str(len(self.SomeFileContents)) + ' lines')
 			#self.logger('line size is ' + str(self.datalinesize) + ' ytes')
 			#self.logger('file size is ' + str(file_stats.st_size) + ' bytes')
 			self.get_column_names()
+
 			self.get_column_types(thisdatabase_type)
+			
 			self.analyzed = True
 
 	def get_just_filename(self):
 		justfilename=''
 		if self.csvfilename.find('\\') > -1: # have a path and dirs
 			fileparts = self.csvfilename.split('\\')
 			justfilename = fileparts[len(fileparts)-1]
@@ -682,32 +685,53 @@
 		elif self.dbthings.match_integer_type(data) :
 			lookslike = 'bigint'
 
 		else:
 			lookslike = 'text'
 
 		return lookslike,dtformat
+	def handledblquotes(self,rowwithquotes):
+		newstr = ''
+		quotecount = 0
+		cvtmode = False
+		for i in range (0,len(rowwithquotes)-1):
+			if rowwithquotes[i] == '"':
+				quotecount += 1
+			
+			if (quotecount % 2) == 1:
+				cvtmode = True 
+			else:
+				cvtmode = False
+
+			if cvtmode and rowwithquotes[i] == self.delimiter:
+				newstr += self.delimiter_replace
+			elif rowwithquotes[i] != '"':
+				newstr += rowwithquotes[i]
+			
+		return newstr
 
 	def get_column_types(self,thisdatabase_type):
 		found_datatypes = {}
 		found_datavalues = {}
 		found_datefomat = {}
 		for i in range(1,len(self.SomeFileContents)):
-			dataline = self.SomeFileContents[i].strip().split(self.delimiter)
+			cvted_str = self.handledblquotes(self.SomeFileContents[i])
+			dataline = cvted_str.strip().split(self.delimiter)
 			for j in range(0,len(dataline)):
+				fld = dataline[j].replace(self.delimiter_replace,self.delimiter)
 
 				if self.column_names[j].lower().endswith('_text'):
 					thisdatatype = 'text'
 					dtformat = ''
 				else:
-					thisdatatype,dtformat = self.get_datatype(dataline[j],thisdatabase_type)
+					thisdatatype,dtformat = self.get_datatype(fld,thisdatabase_type)
 				#print(thisdatatype)
 				if self.column_names[j] not in found_datatypes:
 					found_datatypes[self.column_names[j]] = thisdatatype
-					found_datavalues[self.column_names[j]] = dataline[j]
+					found_datavalues[self.column_names[j]] = fld
 					found_datefomat[self.column_names[j]]	= dtformat
 				else:
 					if found_datatypes[self.column_names[j]] == 'date' and thisdatatype =='date' and found_datefomat[self.column_names[j]] != dtformat:
 						found_datatypes[self.column_names[j]] == 'text'
 					elif found_datatypes[self.column_names[j]] == 'timestamp' and thisdatatype =='timestamp' and found_datefomat[self.column_names[j]] != dtformat:
 						found_datatypes[self.column_names[j]] == 'text'
 					elif found_datatypes[self.column_names[j]] != thisdatatype:
@@ -778,22 +802,19 @@
 		text = ptext.strip()
 		if (text[:1] == '"' and text[-1:] == '"'):
 			return text[1:-1]
 		else:
 			return text
 
 	def clean_column_name(self,col_name):
-
-		new_column_name = col_name
-		chardict = self.count_chars(col_name)
-		alphacount = self.count_alpha(chardict)
-		nbrcount = self.count_nbr(chardict)
-		if ((len(col_name)-2) == (alphacount + nbrcount)) and '1234567890'.find(col_name[:1]) == -1:
-			new_column_name = self.clean_text(col_name) # .replace('"','').strip()
-
+		col = col_name.replace(' ','_')
+		new_column_name = ''
+		for i in range(0,len(col)):
+			if 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ_'.find(col[i]) > -1:
+				new_column_name += col[i]
 
 		return new_column_name
 
 	def get_column_names(self):
 		self.delimiter = self.GuessDelimiter(self.SomeFileContents[0])
 		self.logger('file delimiter is ' + self.delimiter)
 		self.column_names = self.SomeFileContents[0].strip().split(self.delimiter)
```

### Comparing `schemawizard_package-2.4.0/src/schemawizard_package/sqlite.tablea.ddl` & `schemawizard_package-2.5.0/src/schemawizard_package/sqlite.tablea.ddl`

 * *Files identical despite different names*

### Comparing `schemawizard_package-2.4.0/src/schemawizard_package/station_months.tsv` & `schemawizard_package-2.5.0/src/schemawizard_package/station_months.tsv`

 * *Files identical despite different names*

### Comparing `schemawizard_package-2.4.0/src/schemawizard_package/station_years.tsv` & `schemawizard_package-2.5.0/src/schemawizard_package/station_years.tsv`

 * *Files identical despite different names*

### Comparing `schemawizard_package-2.4.0/tests/create_and_load.py` & `schemawizard_package-2.5.0/tests/create_and_load.py`

 * *Files identical despite different names*

### Comparing `schemawizard_package-2.4.0/tests/tesla.csv` & `schemawizard_package-2.5.0/tests/tesla.csv`

 * *Files identical despite different names*

### Comparing `schemawizard_package-2.4.0/tests/tester.py` & `schemawizard_package-2.5.0/tests/tester.py`

 * *Files identical despite different names*

### Comparing `schemawizard_package-2.4.0/LICENSE` & `schemawizard_package-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `schemawizard_package-2.4.0/pyproject.toml` & `schemawizard_package-2.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling","postgresdave_package","mysqldave_package","sqlitedave_package","garbledave_package"]
 
 build-backend = "hatchling.build"
 
 [project]
 name = "schemawizard_package"
-version = "2.4.0"
+version = "2.5.0"
 dependencies = [
   'postgresdave_package >= 1.7.6',
   'mysqldave_package >= 1.3.7',
   'sqlitedave_package >= 1.2.6',
   'garbledave_package >= 1.0.0 '
 ]
 authors = [
```

### Comparing `schemawizard_package-2.4.0/PKG-INFO` & `schemawizard_package-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schemawizard_package
-Version: 2.4.0
+Version: 2.5.0
 Summary: Reads a csv and generates a table design for Postgres, MySQL, sqlite or BigQuery
 Project-URL: Homepage, https://github.com/daveskura/schemawizard
 Project-URL: Author Linkedin, https://www.linkedin.com/in/2166883
 Author-email: Dave Skura <dskura@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

