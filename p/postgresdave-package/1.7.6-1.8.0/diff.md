# Comparing `tmp/postgresdave_package-1.7.6.tar.gz` & `tmp/postgresdave_package-1.8.0.tar.gz`

## Comparing `postgresdave_package-1.7.6.tar` & `postgresdave_package-1.8.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 postgresdave_package-1.7.6/QuickStart.md
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 postgresdave_package-1.7.6/methods.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 postgresdave_package-1.7.6/src/postgresdave_package/__init__.py
--rw-r--r--   0        0        0    15642 2020-02-02 00:00:00.000000 postgresdave_package-1.7.6/src/postgresdave_package/postgresdave.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 postgresdave_package-1.7.6/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 postgresdave_package-1.7.6/LICENSE
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 postgresdave_package-1.7.6/README.md
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 postgresdave_package-1.7.6/pyproject.toml
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 postgresdave_package-1.7.6/PKG-INFO
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 postgresdave_package-1.8.0/QuickStart.md
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 postgresdave_package-1.8.0/methods.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 postgresdave_package-1.8.0/src/postgresdave_package/__init__.py
+-rw-r--r--   0        0        0    16115 2020-02-02 00:00:00.000000 postgresdave_package-1.8.0/src/postgresdave_package/postgresdave.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 postgresdave_package-1.8.0/src/postgresdave_package/testcase1.csv
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 postgresdave_package-1.8.0/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 postgresdave_package-1.8.0/LICENSE
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 postgresdave_package-1.8.0/README.md
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 postgresdave_package-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 postgresdave_package-1.8.0/PKG-INFO
```

### Comparing `postgresdave_package-1.7.6/QuickStart.md` & `postgresdave_package-1.8.0/QuickStart.md`

 * *Files identical despite different names*

### Comparing `postgresdave_package-1.7.6/methods.md` & `postgresdave_package-1.8.0/methods.md`

 * *Files identical despite different names*

### Comparing `postgresdave_package-1.7.6/src/postgresdave_package/postgresdave.py` & `postgresdave_package-1.8.0/src/postgresdave_package/postgresdave.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,14 +66,16 @@
 		self.data_type = ''
 		self.Need_Quotes = ''
 		self.ordinal_position = -1
 		self.comment = '' # dateformat in csv [%Y/%m/%d]
 
 class postgres_db:
 	def __init__(self,DB_USERPWD='no-password-supplied',DB_SCHEMA='no-schema-supplied'):
+		self.delimiter = ''
+		self.delimiter_replace = '^~^'
 		self.enable_logging = False
 		self.max_loglines = 500
 		self.db_conn_dets = dbconnection_details()
 		self.dbconn = None
 		self.cur = None
 
 		if DB_USERPWD != 'no-password-supplied':
@@ -153,26 +155,24 @@
 	def dbstr(self):
 		return 'usr=' + self.db_conn_dets.DB_USERNAME + '; svr=' + self.db_conn_dets.DB_HOST + '; port=' + self.db_conn_dets.DB_PORT + '; Database=' + self.db_conn_dets.DB_NAME + '; Schema=' + self.db_conn_dets.DB_SCHEMA 
 
 	def dbversion(self):
 		return self.queryone('SELECT VERSION()')
 
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
@@ -293,15 +293,37 @@
 			this_schema = self.db_conn_dets.DB_SCHEMA
 			this_table = tblname.split('.')[0]
 
 		qualified_table = this_schema + '.' + this_table
 
 		self.export_query_to_csv('SELECT * FROM ' + qualified_table,csvfile,szdelimiter)
 
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
 		this_schema = tblname.split('.')[0]
 		try:
 			this_table = tblname.split('.')[1]
 		except:
 			this_schema = self.db_conn_dets.DB_SCHEMA
 			this_table = tblname.split('.')[0]
 
@@ -334,15 +356,16 @@
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
 							if row[j].lower() == 'none' or row[j].lower() == 'null':
 								newline += "NULL,"
@@ -358,17 +381,17 @@
 									dt_fmt = self.getbetween(table_fields[j].comment,'[',']')
 									if dt_fmt.strip() != '':
 										newline += "to_timestamp('" + self.clean_text(row[j]) + "','" + dt_fmt + "'),"
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
@@ -497,11 +520,11 @@
 	#print('Connected to ' + mydb.dbversion())
 	#qry = """
 	#SELECT DISTINCT table_catalog as database_name, table_schema as schema 
 	#FROM INFORMATION_SCHEMA.TABLES
 	#"""
 	#print(mydb.export_query_to_str(qry,'\t'))
 
-	#mydb.load_csv_to_table('CanadianPostalCodes.csv','canweather.canadianpostalcodes',True,',')
+	#mydb.load_csv_to_table('testcase1.csv','testcase1',True,',')
 
 	mydb.close()
```

### Comparing `postgresdave_package-1.7.6/LICENSE` & `postgresdave_package-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `postgresdave_package-1.7.6/PKG-INFO` & `postgresdave_package-1.8.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: postgresdave_package
-Version: 1.7.6
+Version: 1.8.0
 Summary: A wrapper for simplified Postgres usage using psycopg2.
 Project-URL: Homepage, https://github.com/daveskura/postgresdave
 Project-URL: Author Linkedin, https://www.linkedin.com/in/2166883
 Author-email: Dave Skura <dskura@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: garbledave-package>=1.0.0
+Requires-Dist: psycopg2>=2.9.5
 Description-Content-Type: text/markdown
 
 # postgresdave
 A simple wrapper on psycopg2 to access Postgres
 
 ### install with pip
 pip install postgresdave_package
```

