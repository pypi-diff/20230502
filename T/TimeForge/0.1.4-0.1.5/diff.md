# Comparing `tmp/TimeForge-0.1.4.tar.gz` & `tmp/TimeForge-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TimeForge-0.1.4.tar", last modified: Mon Apr 24 12:48:29 2023, max compression
+gzip compressed data, was "TimeForge-0.1.5.tar", last modified: Tue May  2 12:38:00 2023, max compression
```

## Comparing `TimeForge-0.1.4.tar` & `TimeForge-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-24 12:48:29.403894 TimeForge-0.1.4/
--rw-r--r--   0 michael   (1000) michael   (1000)    34916 2023-04-04 11:47:23.000000 TimeForge-0.1.4/LICENSE.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1003 2023-04-24 12:48:29.403894 TimeForge-0.1.4/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      330 2023-04-05 15:25:59.000000 TimeForge-0.1.4/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)      935 2023-04-24 12:48:24.000000 TimeForge-0.1.4/pyproject.toml
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-04-24 12:48:29.403894 TimeForge-0.1.4/setup.cfg
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-24 12:48:29.403894 TimeForge-0.1.4/src/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-24 12:48:29.403894 TimeForge-0.1.4/src/TimeForge.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)     1003 2023-04-24 12:48:29.000000 TimeForge-0.1.4/src/TimeForge.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      271 2023-04-24 12:48:29.000000 TimeForge-0.1.4/src/TimeForge.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-04-24 12:48:29.000000 TimeForge-0.1.4/src/TimeForge.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      105 2023-04-24 12:48:29.000000 TimeForge-0.1.4/src/TimeForge.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       10 2023-04-24 12:48:29.000000 TimeForge-0.1.4/src/TimeForge.egg-info/top_level.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-24 12:48:29.403894 TimeForge-0.1.4/src/timeforge/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-24 11:15:53.000000 TimeForge-0.1.4/src/timeforge/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6626 2023-04-24 11:49:59.000000 TimeForge-0.1.4/src/timeforge/__main__.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-02 12:38:00.283803 TimeForge-0.1.5/
+-rw-r--r--   0 michael   (1000) michael   (1000)    34916 2023-04-04 11:47:23.000000 TimeForge-0.1.5/LICENSE.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1003 2023-05-02 12:38:00.283803 TimeForge-0.1.5/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)      330 2023-04-05 15:25:59.000000 TimeForge-0.1.5/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      935 2023-05-02 12:37:47.000000 TimeForge-0.1.5/pyproject.toml
+-rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-05-02 12:38:00.283803 TimeForge-0.1.5/setup.cfg
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-02 12:38:00.283803 TimeForge-0.1.5/src/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-02 12:38:00.283803 TimeForge-0.1.5/src/TimeForge.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1003 2023-05-02 12:38:00.000000 TimeForge-0.1.5/src/TimeForge.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)      271 2023-05-02 12:38:00.000000 TimeForge-0.1.5/src/TimeForge.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-05-02 12:38:00.000000 TimeForge-0.1.5/src/TimeForge.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      105 2023-05-02 12:38:00.000000 TimeForge-0.1.5/src/TimeForge.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       10 2023-05-02 12:38:00.000000 TimeForge-0.1.5/src/TimeForge.egg-info/top_level.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-02 12:38:00.283803 TimeForge-0.1.5/src/timeforge/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-24 11:15:53.000000 TimeForge-0.1.5/src/timeforge/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6834 2023-05-02 12:37:03.000000 TimeForge-0.1.5/src/timeforge/__main__.py
```

### Comparing `TimeForge-0.1.4/LICENSE.md` & `TimeForge-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `TimeForge-0.1.4/PKG-INFO` & `TimeForge-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TimeForge
-Version: 0.1.4
+Version: 0.1.5
 Summary: Create realistic looking but fake time documentation for your student job at KIT
 Author-email: Michael Hohenstein <michael@hohenste.in>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: German
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Scheduling
```

### Comparing `TimeForge-0.1.4/pyproject.toml` & `TimeForge-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TimeForge"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
 	{ name="Michael Hohenstein", email="michael@hohenste.in" },
 ]
 description = "Create realistic looking but fake time documentation for your student job at KIT"
 readme = "README.md"
 requires-python= ">=3.7"
 classifiers = [
```

### Comparing `TimeForge-0.1.4/src/TimeForge.egg-info/PKG-INFO` & `TimeForge-0.1.5/src/TimeForge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TimeForge
-Version: 0.1.4
+Version: 0.1.5
 Summary: Create realistic looking but fake time documentation for your student job at KIT
 Author-email: Michael Hohenstein <michael@hohenste.in>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: German
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Office/Business :: Scheduling
```

### Comparing `TimeForge-0.1.4/src/timeforge/__main__.py` & `TimeForge-0.1.5/src/timeforge/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,19 +36,22 @@
 parser.add_argument('-u', action='store_true',
                     help='the UB field in the form, default: False') # figure out what EB stands for
 
 parser.add_argument('-v', '--verbose', action='store_true',
                     help='more detailed information printing for debugging purpose')
 
 parser.add_argument('-i', '--input', type=str, required=True,
-                    help='the location of the input file')
+                    help='the location of the input file (The MiLoG-Arbeitszeitdokumentation.pdf from the PSE website)')
 
 parser.add_argument('-o', '--output', type=str, required=True,
                     help='Output File where the content will be written to')
 
+parser.add_argument('-j', '--job', type=str, required=True,
+                    help='description of the job task')
+
 argcomplete.autocomplete(parser)
 args = parser.parse_args()
 
 #########################################
 
 if args.verbose:
     from prettytable import PrettyTable
@@ -62,14 +65,15 @@
     tab.add_row(["Salary", str(args.salary) + '€'])
     tab.add_row(["Organisation unit", args.organisation])
     tab.add_row(["GF", args.low_income])
     tab.add_row(["UB", args.u])
     tab.add_row(["Verbose", args.verbose])
     tab.add_row(["Input File", args.input])
     tab.add_row(["Output-File", args.output])
+    tab.add_row(["Job-task", args.job])
     print(tab)
 
 #########################################
 
 # prevent autopep8 from moving these imports to the front
 if True:
     import sys, os
@@ -121,15 +125,15 @@
 # Generate the content for the PDF file
 date_day = 1
 table_row = 1
 work_hours_left = args.time
 while (work_hours_left > 0) and (date_day < 28): # February has 28 days and is therefore the shortest month of all
     if ( ( d := date( year=args.year, month=args.month, day=date_day) ).weekday() <= 5 ) and ( not d in feiertage_api_response ):
         worktime = timedelta( hours = ( h := min(work_hours_left, 4) ) ) # 4h maximum to work
-        form_data['Tätigkeit Stichwort ProjektRow'+str(table_row)] = "Arbeitstätigkeit"
+        form_data['Tätigkeit Stichwort ProjektRow'+str(table_row)] = args.job
         form_data["ttmmjjRow"+str(table_row)] = d.strftime("%d.%m.%y")
         form_data["hhmmRow"+str(table_row)] = ( start := time(hour=8) ).strftime("%H:%M" )  # beginning at 8am
         form_data["hhmmRow"+str(table_row)+"_2"] =( end := ( datetime.combine(d,start) + worktime ) ).time().strftime("%H:%M")
         form_data["hhmmRow"+str(table_row)+"_3"] ="00:00" #( (datetime.combine(d,start) + (worktime/2)) ).time().strftime("%H:%M")
         form_data["hhmmRow"+str(table_row)+"_4"] = time( hour=int(h), minute=int( (h % 1) * 60) ).strftime("%H:%M") #"0" + str(worktime) + ":00"
         work_hours_left -= h
         table_row += 1
```

