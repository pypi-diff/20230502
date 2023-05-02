# Comparing `tmp/mysqldave_package-1.4.0.tar.gz` & `tmp/mysqldave_package-1.5.0.tar.gz`

## Comparing `mysqldave_package-1.4.0.tar` & `mysqldave_package-1.5.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 mysqldave_package-1.4.0/QuickStart.md
--rwxr-xr-x   0        0        0      538 2020-02-02 00:00:00.000000 mysqldave_package-1.4.0/export_to_csv.bat
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 mysqldave_package-1.4.0/methods.md
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 mysqldave_package-1.4.0/src/mysqldave_package/.schemawiz_config2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysqldave_package-1.4.0/src/mysqldave_package/__init__.py
--rw-r--r--   0        0        0    13788 2020-02-02 00:00:00.000000 mysqldave_package-1.4.0/src/mysqldave_package/mysqldave.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 mysqldave_package-1.4.0/src/mysqldave_package/restored_sample.ddl
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 mysqldave_package-1.4.0/src/mysqldave_package/sample.csv
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 mysqldave_package-1.4.0/tests/.schemawiz_config2
--rwxr-xr-x   0        0        0      316 2020-02-02 00:00:00.000000 mysqldave_package-1.4.0/tests/backup.bat
--rwxr-xr-x   0        0        0      303 2020-02-02 00:00:00.000000 mysqldave_package-1.4.0/tests/restore.bat
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 mysqldave_package-1.4.0/tests/sample7.csv
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 mysqldave_package-1.4.0/tests/sample8.csv
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 mysqldave_package-1.4.0/tests/tester.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 mysqldave_package-1.4.0/tests/thistbl.csv
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 mysqldave_package-1.4.0/tests/z.new_sample7.ddl
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 mysqldave_package-1.4.0/tests/z.new_sample8.ddl
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 mysqldave_package-1.4.0/tests/z.new_thistbl.ddl
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 mysqldave_package-1.4.0/tests/z.restored_1sample7.ddl
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 mysqldave_package-1.4.0/tests/z.restored_sample7.ddl
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 mysqldave_package-1.4.0/tests/z.restored_sample8.ddl
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 mysqldave_package-1.4.0/tests/z.restored_thistbl.ddl
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 mysqldave_package-1.4.0/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 mysqldave_package-1.4.0/LICENSE
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 mysqldave_package-1.4.0/README.md
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 mysqldave_package-1.4.0/pyproject.toml
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 mysqldave_package-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/QuickStart.md
+-rwxr-xr-x   0        0        0      538 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/export_to_csv.bat
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/methods.md
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/src/mysqldave_package/.schemawiz_config2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/src/mysqldave_package/__init__.py
+-rw-r--r--   0        0        0    14301 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/src/mysqldave_package/mysqldave.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/src/mysqldave_package/restored_sample.ddl
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/src/mysqldave_package/sample.csv
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/src/mysqldave_package/testcase1.csv
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/tests/.schemawiz_config2
+-rwxr-xr-x   0        0        0      316 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/tests/backup.bat
+-rwxr-xr-x   0        0        0      300 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/tests/restore.bat
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/tests/sample7.csv
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/tests/sample8.csv
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/tests/tester.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/tests/thistbl.csv
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/tests/z.new_sample7.ddl
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/tests/z.new_sample8.ddl
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/tests/z.new_thistbl.ddl
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/tests/z.restored_1sample7.ddl
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/tests/z.restored_sample7.ddl
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/tests/z.restored_sample8.ddl
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/tests/z.restored_thistbl.ddl
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/LICENSE
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/README.md
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 mysqldave_package-1.5.0/PKG-INFO
```

### Comparing `mysqldave_package-1.4.0/QuickStart.md` & `mysqldave_package-1.5.0/QuickStart.md`

 * *Files identical despite different names*

### Comparing `mysqldave_package-1.4.0/export_to_csv.bat` & `mysqldave_package-1.5.0/export_to_csv.bat`

 * *Files identical despite different names*

### Comparing `mysqldave_package-1.4.0/methods.md` & `mysqldave_package-1.5.0/methods.md`

 * *Files identical despite different names*

### Comparing `mysqldave_package-1.4.0/src/mysqldave_package/mysqldave.py` & `mysqldave_package-1.5.0/src/mysqldave_package/mysqldave.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 from garbledave_package.garbledave import garbledave 
 
 def main():
 	mydb = mysql_db()
 	mydb.connect()
 	print(mydb.dbstr())
 
-	#csvfilename = 'sample.csv'
-	#tblname = 'sample7'
+	#csvfilename = 'testcase1.csv'
+	#tblname = 'testcase1'
 	#mydb.load_csv_to_table(csvfilename,tblname,True,',')
 
 	mydb.close()
 
 
 class dbconnection_details: 
 	def __init__(self): 
@@ -78,14 +78,16 @@
 		self.data_type = ''
 		self.Need_Quotes = ''
 		self.ordinal_position = -1
 		self.comment = '' # dateformat in csv [%Y/%m/%d]
 
 class mysql_db:
 	def __init__(self,DB_USERPWD='no-password-supplied',DB_SCHEMA='no-schema-supplied'):
+		self.delimiter = ''
+		self.delimiter_replace = '^~^'
 		self.enable_logging = False
 		self.max_loglines = 500
 		self.db_conn_dets = dbconnection_details()
 		self.dbconn = None
 		self.cur = None
 
 		if DB_USERPWD != 'no-password-supplied':
@@ -149,25 +151,24 @@
 		return 'usr=' + self.db_conn_dets.DB_USERNAME + '; svr=' + self.db_conn_dets.DB_HOST + '; port=' + self.db_conn_dets.DB_PORT + '; Database=' + self.db_conn_dets.DB_NAME
 
 	def dbversion(self):
 		return self.queryone('SELECT VERSION()')
 
 	def clean_column_name(self,col_name):
 
-		new_column_name = col_name
-		chardict = self.count_chars(col_name)
-		alphacount = self.count_alpha(chardict)
-		nbrcount = self.count_nbr(chardict)
-		if ((len(col_name)-2) == (alphacount + nbrcount)) and '1234567890'.find(col_name[:1]) == -1:
-			new_column_name = self.clean_text(col_name) # .replace('"','').strip()
+		col = col_name.replace(' ','_')
+		new_column_name = ''
+		for i in range(0,len(col)):
+			if 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ_'.find(col[i]) > -1:
+				new_column_name += col[i]
 
 		return new_column_name
 
 	def clean_text(self,ptext): # remove optional double quotes
-		text = ptext.strip()
+		text = ptext.replace(self.delimiter_replace,self.delimiter).strip()
 		if (text[:1] == '"' and text[-1:] == '"'):
 			return text[1:-1]
 		else:
 			return text
 
 	def count_chars(self,data,exceptchars=''):
 		chars_in_hdr = {}
@@ -283,15 +284,38 @@
 
 	def export_table_to_csv(self,csvfile,tblname,szdelimiter=','):
 		if not self.does_table_exist(tblname):
 			raise Exception('Table does not exist.  Create table first')
 
 		self.export_query_to_csv('SELECT * FROM ' + tblname,csvfile,szdelimiter)
 
+
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
+
+
 	def load_csv_to_table(self,csvfile,tblname,withtruncate=True,szdelimiter=',',fields='',withextrafields={}):
+		self.delimiter = szdelimiter
 		table_fields = self.getfielddefs(self.db_conn_dets.DB_NAME,tblname)
 
 		if not self.does_table_exist(tblname):
 			raise Exception('Table does not exist.  Create table first')
 
 
 		if withtruncate:
@@ -318,15 +342,16 @@
 		with open(csvfile) as myfile:
 			for line in myfile:
 				if line.strip()!='':
 					if skiprow1 == 0:
 						skiprow1 = 1
 					else:
 						batchcount += 1
-						row = line.rstrip("\n").split(szdelimiter)
+						unquotedline = self.handledblquotes(line.rstrip("\n"))
+						row = unquotedline.split(szdelimiter)
 						newline = "("
 						for var in withextrafields:
 							newline += "'" + withextrafields[var]  + "',"
 
 						for j in range(0,len(row)):
 							#print(table_fields[j].data_type.strip().lower())
 							#print(table_fields[j].comment)
@@ -346,17 +371,17 @@
 									dt_fmt = self.getbetween(table_fields[j].comment,'[',']')
 									if dt_fmt.strip() != '':
 										newline += "str_to_date('" + self.clean_text(row[j]) + "','" + dt_fmt + "'),"
 									else:
 										newline += "'" + self.clean_text(row[j]) + "',"
 
 								elif table_fields[j].Need_Quotes == 'QUOTE':
-									newline += "'" + self.clean_text(row[j]).replace(',','').replace("'",'').replace('"','') + "',"
+									newline += "'" + self.clean_text(row[j]).replace("'",'').replace('"','') + "',"
 								else:
-									val = self.clean_text(row[j]).replace(',','').replace("'",'').replace('"','')
+									val = self.clean_text(row[j]).replace("'",'').replace('"','')
 									if val == '':
 										newline += "NULL,"
 									else:
 										newline += val + ","
 
 							
 						ilines += newline[:-1] + '),'
```

### Comparing `mysqldave_package-1.4.0/src/mysqldave_package/restored_sample.ddl` & `mysqldave_package-1.5.0/src/mysqldave_package/restored_sample.ddl`

 * *Files identical despite different names*

### Comparing `mysqldave_package-1.4.0/tests/tester.py` & `mysqldave_package-1.5.0/tests/tester.py`

 * *Files identical despite different names*

### Comparing `mysqldave_package-1.4.0/LICENSE` & `mysqldave_package-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mysqldave_package-1.4.0/pyproject.toml` & `mysqldave_package-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling","mysql.connector","garbledave_package"]
 
 build-backend = "hatchling.build"
 
 [project]
 name = "mysqldave_package"
-version = "1.4.0"
+version = "1.5.0"
 dependencies = [
   'mysql-connector-python >= 8.0.32',
   'garbledave_package >= 1.0.0'
 ]
 authors = [
   { name="Dave Skura", email="dskura@gmail.com" },
 ]
```

### Comparing `mysqldave_package-1.4.0/PKG-INFO` & `mysqldave_package-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqldave_package
-Version: 1.4.0
+Version: 1.5.0
 Summary: A wrapper for simplified Postgres usage using mysql.connector.
 Project-URL: Homepage, https://github.com/daveskura/mysqldave
 Project-URL: Author Linkedin, https://www.linkedin.com/in/2166883
 Author-email: Dave Skura <dskura@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

