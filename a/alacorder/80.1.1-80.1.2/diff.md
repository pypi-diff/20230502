# Comparing `tmp/alacorder-80.1.1.tar.gz` & `tmp/alacorder-80.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.1.1.tar", max compression
+gzip compressed data, was "alacorder-80.1.2.tar", max compression
```

## Comparing `alacorder-80.1.1.tar` & `alacorder-80.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.1.1/LICENSE
--rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.1.1/README.md
--rw-r--r--   0        0        0      697 2023-05-01 17:53:02.479122 alacorder-80.1.1/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-01 17:53:03.320152 alacorder-80.1.1/src/alacorder/.DS_Store
--rw-r--r--   0        0        0     1784 2023-04-21 19:12:38.269775 alacorder-80.1.1/src/alacorder/__init__.py
--rw-r--r--   0        0        0   212262 2023-05-01 17:52:48.932648 alacorder-80.1.1/src/alacorder/__main__.py
--rw-r--r--   0        0        0   212262 2023-05-01 17:52:43.729760 alacorder-80.1.1/src/alacorder/alac.py
--rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.1.2/LICENSE
+-rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.1.2/README.md
+-rw-r--r--   0        0        0      697 2023-05-02 14:23:36.762018 alacorder-80.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-02 14:23:56.879572 alacorder-80.1.2/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0     1784 2023-04-21 19:12:38.269775 alacorder-80.1.2/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   213086 2023-05-02 14:23:45.359435 alacorder-80.1.2/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   213086 2023-05-02 14:23:13.445437 alacorder-80.1.2/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.1.2/PKG-INFO
```

### Comparing `alacorder-80.1.1/LICENSE` & `alacorder-80.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.1.1/README.md` & `alacorder-80.1.2/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.1.1/pyproject.toml` & `alacorder-80.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.1.1"
+version = "80.1.2"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.1.1/src/alacorder/.DS_Store` & `alacorder-80.1.2/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-80.1.1/src/alacorder/__init__.py` & `alacorder-80.1.2/src/alacorder/__init__.py`

 * *Files identical despite different names*

### Comparing `alacorder-80.1.1/src/alacorder/__main__.py` & `alacorder-80.1.2/src/alacorder/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,35 +7,36 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.1.1"
+version = "80.1.2"
 
 autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import Select
 from selenium.webdriver.chrome.options import Options
 
 
-#   #   #   #               LOGS                 #   #   #   #
+#   #   #   #                LOGS                #   #   #   #
 
 
 pl.Config.set_tbl_rows(20)
 pl.Config.set_fmt_str_lengths(100)
 pl.Config.set_tbl_width_chars(90)
 pl.Config.set_tbl_formatting("NOTHING")
+pl.Config.set_tbl_dataframe_shape_below(True)
 pl.Config.set_tbl_hide_column_data_types(True)
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
 fname = f"{name} {version}"
 fshort_name = f"{name} {'.'.join(version.split('.')[0:-1])}"
 
 prt = print
@@ -95,14 +96,15 @@
     message = ""
     for m in msg:
         message += f"{m} "
     message = message.strip()
     if cf:
         if cf["WINDOW"]:
             cf["WINDOW"].write_event_value("POPUP", message)
+            cf["WINDOW"].write_event_value("ERROR", message)
         elif cf["FORCE"]:
             print(message)
         else:
             raise Exception(message)
     else:
         raise Exception(message)
 
@@ -3962,32 +3964,34 @@
                 size=[39, 10],
                 key="TB-OUTPUTPATH",
             ),
         ],
         [
             sg.Radio("All Tables (.xlsx, .xls)", "TABLE", key="TB-ALL", default=True),
             sg.Radio("Cases", "TABLE", key="TB-CASES", default=False),
-            sg.Radio("Charges", "TABLE", key="TB-CHARGES", default=False),
+            sg.Radio("Sentences", "TABLE", key="TB-SENTENCES", default=False),
             sg.Radio("Fees", "TABLE", key="TB-FEES", default=False),
         ],
         [
             sg.Radio("Case Action Summary", "TABLE", key="TB-CAS", default=False),
             sg.Radio("Witnesses", "TABLE", key="TB-WITNESSES", default=False),
             sg.Radio("Images", "TABLE", key="TB-IMAGES", default=False),
         ],
         [
             sg.Radio("Attorneys", "TABLE", key="TB-ATTORNEYS", default=False),
             sg.Radio("Settings", "TABLE", key="TB-SETTINGS", default=False),
             sg.Radio("Financial History", "TABLE", key="TB-HISTORY", default=False),
         ],
         [
+            sg.Radio("All Charges", "TABLE", key="TB-CHARGES", default=False),
             sg.Radio(
                 "Disposition Charges", "TABLE", key="TB-DISPOSITION", default=False
             ),
             sg.Radio("Filing Charges", "TABLE", key="TB-FILING", default=False),
+
         ],
         [
             sg.Text("Max cases: "),
             sg.Input(key="TB-COUNT", default_text="0", size=[5, 1]),
             sg.Checkbox("Allow Overwrite", key="TB-OVERWRITE", default=True),
         ],
         [
@@ -4070,23 +4074,31 @@
     window = sg.Window(
         title=name,
         layout=layout,
         grab_anywhere=True,
         resizable=WINDOW_RESIZE,
         size=WINDOW_SIZE,
     )
+    thread = False
     while True:
         event, values = window.read()
         if event in ("Exit", "Quit", sg.WIN_CLOSED):
             window.close()
             break
         elif "TOTAL" in event and "PROGRESS" in event:
             window["PROGRESS"].update(max=values[event], current_count=0)
         elif "PROGRESS" in event and "TOTAL" not in event:
             window["PROGRESS"].update(current_count=values[event])
+        elif "ERROR" in event:
+            window["AA"].update(disabled=False)
+            window["SQ"].update(disabled=False)
+            window["MA"].update(disabled=False)
+            window["TB"].update(disabled=False)
+            window["MA"].update(disabled=False)
+            window["SUM"].update(disabled=False)
         elif "COMPLETE" in event:
             print("Alacorder completed the task.")
             window["AA"].update(disabled=False)
             window["SQ"].update(disabled=False)
             window["MA"].update(disabled=False)
             window["TB"].update(disabled=False)
             window["MA"].update(disabled=False)
@@ -4112,15 +4124,15 @@
                 window["SUM-PAIRS"].get(),
                 pairs=window["SUM-PAIRS"].get(),
                 log=True,
                 no_write=False,
                 overwrite=True,
                 window=window,
             )
-            threading.Thread(target=pairs, args=[cf], daemon=True).start()
+            thread = threading.Thread(target=pairs, args=[cf], daemon=True).start()
             print("Creating AIS / Unique ID pairs template...")
             window["MT"].update(disabled=True)
         elif event == "SUM":
             cf = set(
                 window["SUM-INPUTPATH"].get(),
                 window["SUM-OUTPUTPATH"].get(),
                 pairs=window["SUM-PAIRS"].get(),
@@ -4129,31 +4141,33 @@
                 convictions_summary=window["SUM-CONV"].get(),
                 log=True,
                 no_write=False,
                 overwrite=True,
                 window=window,
             )
             print("Making voting rights summary table...")
-            threading.Thread(target=init, args=[cf], daemon=True).start()
+            thread = threading.Thread(target=init, args=[cf], daemon=True).start()
             window["SUM"].update(disabled=True)
         elif event == "POPUP":
             sg.popup(values["POPUP"])
         elif event == "TB":
             table = ""
             table = "all" if window["TB-ALL"].get() else table
+            table = "cases" if window["TB-CASES"].get() else table
             table = "charges" if window["TB-CHARGES"].get() else table
             table = "fees" if window["TB-FEES"].get() else table
             table = "case-action-summary" if window["TB-CAS"].get() else table
             table = "witnesses" if window["TB-WITNESSES"].get() else table
             table = "images" if window["TB-IMAGES"].get() else table
             table = "attorneys" if window["TB-ATTORNEYS"].get() else table
             table = "settings" if window["TB-SETTINGS"].get() else table
             table = "disposition" if window["TB-DISPOSITION"].get() else table
             table = "filing" if window["TB-FILING"].get() else table
             table = "financial-history" if window["TB-HISTORY"].get() else table
+            table = "sentences" if window["TB-SENTENCES"].get() else table
             if (
                 window["TB-INPUTPATH"].get() == ""
                 or window["TB-OUTPUTPATH"].get() == ""
             ):
                 sg.popup("Check configuration and try again.")
             else:
                 cf = set(
@@ -4162,18 +4176,17 @@
                     count=int(window["TB-COUNT"].get()),
                     table=table,
                     log=True,
                     overwrite=window["TB-OVERWRITE"].get(),
                     no_prompt=True,
                     archive=False,
                     window=window,
-                )
-                # except:
+                )                
+                thread = threading.Thread(target=init, args=[cf], daemon=True).start()
                 window["TB"].update(disabled=True)
-                threading.Thread(target=init, args=[cf], daemon=True).start()
                 continue
         elif event == "MA":
             if (
                 window["MA-INPUTPATH"].get() == ""
                 or window["MA-OUTPUTPATH"].get() == ""
             ):
                 sg.popup("Check configuration and try again.")
@@ -4195,16 +4208,17 @@
                     no_prompt=True,
                     window=window,
                 )
             except:
                 sg.popup("Check configuration and try again.")
                 window["MA"].update(disabled=False)
                 continue
-            window["MA"].update(disabled=True)
-            threading.Thread(target=archive, args=[cf], daemon=True).start()
+            if os.path.splitext(window["MA-OUTPUTPATH"].get())[1] in (".parquet", ".json", ".csv"):
+                thread = threading.Thread(target=archive, args=[cf], daemon=True).start()
+                window["MA"].update(disabled=True)
             continue
         elif event == "SQ":
             if (
                 window["SQ-INPUTPATH"].get() == ""
                 or window["SQ-OUTPUTPATH"].get() == ""
             ):
                 sg.popup("Check configuration and try again.")
@@ -4213,15 +4227,15 @@
                 try:
                     sq_max = int(window["SQ-MAX"].get().strip())
                     sq_skip = int(window["SQ-SKIP"].get().strip())
                 except:
                     sq_max = 0
                     sq_skip = 0
                 window["SQ"].update(disabled=True)
-                threading.Thread(
+                thread = threading.Thread(
                     target=fetch,
                     args=(
                         window["SQ-INPUTPATH"].get(),
                         window["SQ-OUTPUTPATH"].get(),
                         window["SQ-CUSTOMERID"].get(),
                         window["SQ-USERID"].get(),
                         pwd,
@@ -4244,15 +4258,15 @@
                 window["AA-INPUTPATH"].get() == ""
                 or window["AA-OUTPUTPATH"].get() == ""
             ):
                 sg.popup("Check configuration and try again.")
                 continue
             try:
                 window["AA"].update(disabled=True)
-                threading.Thread(
+                thread = threading.Thread(
                     target=append_archive,
                     args=(
                         window["AA-INPUTPATH"].get(),
                         window["AA-OUTPUTPATH"].get(),
                     ),
                     kwargs={"window": window},
                     daemon=True,
```

### Comparing `alacorder-80.1.1/src/alacorder/alac.py` & `alacorder-80.1.2/src/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,35 +7,36 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.1.1"
+version = "80.1.2"
 
 autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import Select
 from selenium.webdriver.chrome.options import Options
 
 
-#   #   #   #               LOGS                 #   #   #   #
+#   #   #   #                LOGS                #   #   #   #
 
 
 pl.Config.set_tbl_rows(20)
 pl.Config.set_fmt_str_lengths(100)
 pl.Config.set_tbl_width_chars(90)
 pl.Config.set_tbl_formatting("NOTHING")
+pl.Config.set_tbl_dataframe_shape_below(True)
 pl.Config.set_tbl_hide_column_data_types(True)
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
 fname = f"{name} {version}"
 fshort_name = f"{name} {'.'.join(version.split('.')[0:-1])}"
 
 prt = print
@@ -95,14 +96,15 @@
     message = ""
     for m in msg:
         message += f"{m} "
     message = message.strip()
     if cf:
         if cf["WINDOW"]:
             cf["WINDOW"].write_event_value("POPUP", message)
+            cf["WINDOW"].write_event_value("ERROR", message)
         elif cf["FORCE"]:
             print(message)
         else:
             raise Exception(message)
     else:
         raise Exception(message)
 
@@ -3962,32 +3964,34 @@
                 size=[39, 10],
                 key="TB-OUTPUTPATH",
             ),
         ],
         [
             sg.Radio("All Tables (.xlsx, .xls)", "TABLE", key="TB-ALL", default=True),
             sg.Radio("Cases", "TABLE", key="TB-CASES", default=False),
-            sg.Radio("Charges", "TABLE", key="TB-CHARGES", default=False),
+            sg.Radio("Sentences", "TABLE", key="TB-SENTENCES", default=False),
             sg.Radio("Fees", "TABLE", key="TB-FEES", default=False),
         ],
         [
             sg.Radio("Case Action Summary", "TABLE", key="TB-CAS", default=False),
             sg.Radio("Witnesses", "TABLE", key="TB-WITNESSES", default=False),
             sg.Radio("Images", "TABLE", key="TB-IMAGES", default=False),
         ],
         [
             sg.Radio("Attorneys", "TABLE", key="TB-ATTORNEYS", default=False),
             sg.Radio("Settings", "TABLE", key="TB-SETTINGS", default=False),
             sg.Radio("Financial History", "TABLE", key="TB-HISTORY", default=False),
         ],
         [
+            sg.Radio("All Charges", "TABLE", key="TB-CHARGES", default=False),
             sg.Radio(
                 "Disposition Charges", "TABLE", key="TB-DISPOSITION", default=False
             ),
             sg.Radio("Filing Charges", "TABLE", key="TB-FILING", default=False),
+
         ],
         [
             sg.Text("Max cases: "),
             sg.Input(key="TB-COUNT", default_text="0", size=[5, 1]),
             sg.Checkbox("Allow Overwrite", key="TB-OVERWRITE", default=True),
         ],
         [
@@ -4070,23 +4074,31 @@
     window = sg.Window(
         title=name,
         layout=layout,
         grab_anywhere=True,
         resizable=WINDOW_RESIZE,
         size=WINDOW_SIZE,
     )
+    thread = False
     while True:
         event, values = window.read()
         if event in ("Exit", "Quit", sg.WIN_CLOSED):
             window.close()
             break
         elif "TOTAL" in event and "PROGRESS" in event:
             window["PROGRESS"].update(max=values[event], current_count=0)
         elif "PROGRESS" in event and "TOTAL" not in event:
             window["PROGRESS"].update(current_count=values[event])
+        elif "ERROR" in event:
+            window["AA"].update(disabled=False)
+            window["SQ"].update(disabled=False)
+            window["MA"].update(disabled=False)
+            window["TB"].update(disabled=False)
+            window["MA"].update(disabled=False)
+            window["SUM"].update(disabled=False)
         elif "COMPLETE" in event:
             print("Alacorder completed the task.")
             window["AA"].update(disabled=False)
             window["SQ"].update(disabled=False)
             window["MA"].update(disabled=False)
             window["TB"].update(disabled=False)
             window["MA"].update(disabled=False)
@@ -4112,15 +4124,15 @@
                 window["SUM-PAIRS"].get(),
                 pairs=window["SUM-PAIRS"].get(),
                 log=True,
                 no_write=False,
                 overwrite=True,
                 window=window,
             )
-            threading.Thread(target=pairs, args=[cf], daemon=True).start()
+            thread = threading.Thread(target=pairs, args=[cf], daemon=True).start()
             print("Creating AIS / Unique ID pairs template...")
             window["MT"].update(disabled=True)
         elif event == "SUM":
             cf = set(
                 window["SUM-INPUTPATH"].get(),
                 window["SUM-OUTPUTPATH"].get(),
                 pairs=window["SUM-PAIRS"].get(),
@@ -4129,31 +4141,33 @@
                 convictions_summary=window["SUM-CONV"].get(),
                 log=True,
                 no_write=False,
                 overwrite=True,
                 window=window,
             )
             print("Making voting rights summary table...")
-            threading.Thread(target=init, args=[cf], daemon=True).start()
+            thread = threading.Thread(target=init, args=[cf], daemon=True).start()
             window["SUM"].update(disabled=True)
         elif event == "POPUP":
             sg.popup(values["POPUP"])
         elif event == "TB":
             table = ""
             table = "all" if window["TB-ALL"].get() else table
+            table = "cases" if window["TB-CASES"].get() else table
             table = "charges" if window["TB-CHARGES"].get() else table
             table = "fees" if window["TB-FEES"].get() else table
             table = "case-action-summary" if window["TB-CAS"].get() else table
             table = "witnesses" if window["TB-WITNESSES"].get() else table
             table = "images" if window["TB-IMAGES"].get() else table
             table = "attorneys" if window["TB-ATTORNEYS"].get() else table
             table = "settings" if window["TB-SETTINGS"].get() else table
             table = "disposition" if window["TB-DISPOSITION"].get() else table
             table = "filing" if window["TB-FILING"].get() else table
             table = "financial-history" if window["TB-HISTORY"].get() else table
+            table = "sentences" if window["TB-SENTENCES"].get() else table
             if (
                 window["TB-INPUTPATH"].get() == ""
                 or window["TB-OUTPUTPATH"].get() == ""
             ):
                 sg.popup("Check configuration and try again.")
             else:
                 cf = set(
@@ -4162,18 +4176,17 @@
                     count=int(window["TB-COUNT"].get()),
                     table=table,
                     log=True,
                     overwrite=window["TB-OVERWRITE"].get(),
                     no_prompt=True,
                     archive=False,
                     window=window,
-                )
-                # except:
+                )                
+                thread = threading.Thread(target=init, args=[cf], daemon=True).start()
                 window["TB"].update(disabled=True)
-                threading.Thread(target=init, args=[cf], daemon=True).start()
                 continue
         elif event == "MA":
             if (
                 window["MA-INPUTPATH"].get() == ""
                 or window["MA-OUTPUTPATH"].get() == ""
             ):
                 sg.popup("Check configuration and try again.")
@@ -4195,16 +4208,17 @@
                     no_prompt=True,
                     window=window,
                 )
             except:
                 sg.popup("Check configuration and try again.")
                 window["MA"].update(disabled=False)
                 continue
-            window["MA"].update(disabled=True)
-            threading.Thread(target=archive, args=[cf], daemon=True).start()
+            if os.path.splitext(window["MA-OUTPUTPATH"].get())[1] in (".parquet", ".json", ".csv"):
+                thread = threading.Thread(target=archive, args=[cf], daemon=True).start()
+                window["MA"].update(disabled=True)
             continue
         elif event == "SQ":
             if (
                 window["SQ-INPUTPATH"].get() == ""
                 or window["SQ-OUTPUTPATH"].get() == ""
             ):
                 sg.popup("Check configuration and try again.")
@@ -4213,15 +4227,15 @@
                 try:
                     sq_max = int(window["SQ-MAX"].get().strip())
                     sq_skip = int(window["SQ-SKIP"].get().strip())
                 except:
                     sq_max = 0
                     sq_skip = 0
                 window["SQ"].update(disabled=True)
-                threading.Thread(
+                thread = threading.Thread(
                     target=fetch,
                     args=(
                         window["SQ-INPUTPATH"].get(),
                         window["SQ-OUTPUTPATH"].get(),
                         window["SQ-CUSTOMERID"].get(),
                         window["SQ-USERID"].get(),
                         pwd,
@@ -4244,15 +4258,15 @@
                 window["AA-INPUTPATH"].get() == ""
                 or window["AA-OUTPUTPATH"].get() == ""
             ):
                 sg.popup("Check configuration and try again.")
                 continue
             try:
                 window["AA"].update(disabled=True)
-                threading.Thread(
+                thread = threading.Thread(
                     target=append_archive,
                     args=(
                         window["AA-INPUTPATH"].get(),
                         window["AA-OUTPUTPATH"].get(),
                     ),
                     kwargs={"window": window},
                     daemon=True,
```

### Comparing `alacorder-80.1.1/PKG-INFO` & `alacorder-80.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.1.1
+Version: 80.1.2
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

