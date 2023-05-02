# Comparing `tmp/sqlitedave_package-1.2.6.tar.gz` & `tmp/sqlitedave_package-1.3.0.tar.gz`

## Comparing `sqlitedave_package-1.2.6.tar` & `sqlitedave_package-1.3.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 sqlitedave_package-1.2.6/src/sqlitedave_package/.schemawiz_config3
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlitedave_package-1.2.6/src/sqlitedave_package/__init__.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 sqlitedave_package-1.2.6/src/sqlitedave_package/a.csv
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 sqlitedave_package-1.2.6/src/sqlitedave_package/execute.py
--rw-r--r--   0        0        0   610304 2020-02-02 00:00:00.000000 sqlitedave_package-1.2.6/src/sqlitedave_package/local_sqlite_db
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 sqlitedave_package-1.2.6/src/sqlitedave_package/postgres_data.tsv
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 sqlitedave_package-1.2.6/src/sqlitedave_package/query.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 sqlitedave_package-1.2.6/src/sqlitedave_package/select.sql
--rw-r--r--   0        0        0    12252 2020-02-02 00:00:00.000000 sqlitedave_package-1.2.6/src/sqlitedave_package/sqlitedave.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 sqlitedave_package-1.2.6/tests/create_tables.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 sqlitedave_package-1.2.6/tests/create_tesla.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 sqlitedave_package-1.2.6/tests/select_from_sqlite_db.py
--rw-r--r--   0        0        0    50392 2020-02-02 00:00:00.000000 sqlitedave_package-1.2.6/tests/tesla.csv
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 sqlitedave_package-1.2.6/LICENSE
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 sqlitedave_package-1.2.6/README.md
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 sqlitedave_package-1.2.6/pyproject.toml
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 sqlitedave_package-1.2.6/PKG-INFO
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 sqlitedave_package-1.3.0/src/sqlitedave_package/.schemawiz_config3
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlitedave_package-1.3.0/src/sqlitedave_package/__init__.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 sqlitedave_package-1.3.0/src/sqlitedave_package/a.csv
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 sqlitedave_package-1.3.0/src/sqlitedave_package/complexdata.csv
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 sqlitedave_package-1.3.0/src/sqlitedave_package/execute.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 sqlitedave_package-1.3.0/src/sqlitedave_package/postgres_data.tsv
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 sqlitedave_package-1.3.0/src/sqlitedave_package/query.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 sqlitedave_package-1.3.0/src/sqlitedave_package/select.sql
+-rw-r--r--   0        0        0    13435 2020-02-02 00:00:00.000000 sqlitedave_package-1.3.0/src/sqlitedave_package/sqlitedave.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 sqlitedave_package-1.3.0/src/sqlitedave_package/testcase1.csv
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 sqlitedave_package-1.3.0/tests/create_tables.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 sqlitedave_package-1.3.0/tests/create_tesla.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 sqlitedave_package-1.3.0/tests/select_from_sqlite_db.py
+-rw-r--r--   0        0        0    50392 2020-02-02 00:00:00.000000 sqlitedave_package-1.3.0/tests/tesla.csv
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 sqlitedave_package-1.3.0/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 sqlitedave_package-1.3.0/LICENSE
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 sqlitedave_package-1.3.0/README.md
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 sqlitedave_package-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 sqlitedave_package-1.3.0/PKG-INFO
```

### Comparing `sqlitedave_package-1.2.6/src/sqlitedave_package/execute.py` & `sqlitedave_package-1.3.0/src/sqlitedave_package/execute.py`

 * *Files identical despite different names*

### Comparing `sqlitedave_package-1.2.6/src/sqlitedave_package/query.py` & `sqlitedave_package-1.3.0/src/sqlitedave_package/query.py`

 * *Files identical despite different names*

### Comparing `sqlitedave_package-1.2.6/src/sqlitedave_package/sqlitedave.py` & `sqlitedave_package-1.3.0/src/sqlitedave_package/sqlitedave.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,17 +23,20 @@
 	print('-- ')
 	print('py -m sqlitedave_package.execute [query or filename] ') 
 	print('-- ')
 
 	mydb = sqlite_db()
 	mydb.connect()
 	print(mydb.dbstr())
-	mydb.load_csv_to_table('postgres_data.tsv','tablec',True,'~')
+	#mydb.execute(qry)
+	
+	#mydb.load_csv_to_table('testcase1.csv','testcase1',True,',')
+	#print(mydb.queryone('SELECT COUNT(*) FROM testcase1'))
 
-	#print(mydb.export_query_to_str('SELECT CURRENT_DATE as d1,CURRENT_DATE as d2'))
+	#print(mydb.export_query_to_str('SELECT count(*) FROM testcase1'))
 
 	#csvfilename = 'Station.tsv'
 	#tblname = 'Station'
 	
 	#mydb.load_csv_to_table('a.csv','tablea',True,',')
 	#mydb.export_table_to_csv(csvfilename,tblname)
 
@@ -111,14 +114,16 @@
 		self.data_type = ''
 		self.Need_Quotes = ''
 		self.ordinal_position = -1
 		self.comment = '' # dateformat in csv [%Y/%m/%d]
 
 class sqlite_db:
 	def __init__(self,DB_NAME=''):
+		self.delimiter = ''
+		self.delimiter_replace = '^~^'
 		self.enable_logging = False
 		self.max_loglines = 500
 		self.db_conn_dets = dbconnection_details(DB_NAME)
 		self.dbconn = None
 		self.cur = None
 
 	def getbetween(self,srch_str,chr_strt,chr_end,srch_position=0):
@@ -161,26 +166,24 @@
 	def dbstr(self):
 		return 'Database=' + self.db_conn_dets.DB_NAME + '; version ' + self.dbversion()
 
 	def dbversion(self):
 		return self.queryone('select sqlite_version();')
 
 	def clean_column_name(self,col_name):
-
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
@@ -290,28 +293,73 @@
 
 	def export_table_to_csv(self,csvfile,tblname,szdelimiter=','):
 		if not self.does_table_exist(tblname):
 			raise Exception('Table does not exist.  Create table first')
 
 		self.export_query_to_csv('SELECT * FROM ' + tblname,csvfile,szdelimiter)
 
+	def readincsvfile(self,csvfile,szdelimiter):
+		f = open(csvfile,'r')
+		wholefile = f.read()
+		f.close()		
+		lines = []
+		hdr_row = wholefile.split('\n')[0]
+		lines.append(hdr_row)
+		colcount = len(hdr_row.split(szdelimiter))
+		content = wholefile[len(hdr_row):].split(szdelimiter)
+
+		j = 0
+		while j < (len(content)-colcount):
+			newline = ''
+			for i in range(0,colcount-1):
+				newline += content[j+i] + szdelimiter
+			lines.append(newline)
+			j = j + colcount-1
+
+
+		#print('\nlines[0] ',lines[0])
+		#print('\nlines[1] ',lines[1])
+		#print('\nlines[2] ',lines[2])
+		#sys.exit(1)
+		return lines
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
 	def load_csv_to_table(self,csvfile,tblname,withtruncate=True,szdelimiter=',',fields='',withextrafields={}):
+		self.delimiter = szdelimiter
+
 		table_fields = self.getfielddefs(tblname)
 
 		if not self.does_table_exist(tblname):
 			raise Exception('Table does not exist.  Create table first')
 
 		if withtruncate:
 			self.execute('DELETE FROM ' + tblname)
 
-		f = open(csvfile,'r')
-		lines = f.readlines()
+		lines = self.readincsvfile(csvfile,szdelimiter)
 
 		hdrs = lines[0].split(szdelimiter)
-		f.close()		
 
 		isqlhdr = 'INSERT INTO ' + tblname + '('
 
 		if fields != '':
 			isqlhdr += fields	+ ') VALUES '	
 		else:
 			for i in range(0,len(hdrs)):
@@ -325,15 +373,17 @@
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
+
 						newline = "("
 						for var in withextrafields:
 							newline += "'" + withextrafields[var]  + "',"
 
 						for j in range(0,len(row)):
 
 							if row[j].lower() == 'none' or row[j].lower() == 'null':
@@ -350,17 +400,17 @@
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

### Comparing `sqlitedave_package-1.2.6/tests/create_tables.py` & `sqlitedave_package-1.3.0/tests/create_tables.py`

 * *Files identical despite different names*

### Comparing `sqlitedave_package-1.2.6/tests/tesla.csv` & `sqlitedave_package-1.3.0/tests/tesla.csv`

 * *Files identical despite different names*

### Comparing `sqlitedave_package-1.2.6/LICENSE` & `sqlitedave_package-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlitedave_package-1.2.6/README.md` & `sqlitedave_package-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `sqlitedave_package-1.2.6/pyproject.toml` & `sqlitedave_package-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling","garbledave_package"]
 
 build-backend = "hatchling.build"
 
 [project]
 name = "sqlitedave_package"
-version = "1.2.6"
+version = "1.3.0"
 dependencies = [
   'garbledave_package >= 1.0.0'
 ]
 authors = [
   { name="Dave Skura", email="dskura@gmail.com" },
 ]
 description = "A wrapper for simplified sqlite usage using sqlite3."
```

### Comparing `sqlitedave_package-1.2.6/PKG-INFO` & `sqlitedave_package-1.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlitedave_package
-Version: 1.2.6
+Version: 1.3.0
 Summary: A wrapper for simplified sqlite usage using sqlite3.
 Project-URL: Homepage, https://github.com/daveskura/sqlitedave
 Project-URL: Author Linkedin, https://www.linkedin.com/in/2166883
 Author-email: Dave Skura <dskura@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

