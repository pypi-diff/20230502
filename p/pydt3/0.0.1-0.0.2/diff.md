# Comparing `tmp/pydt3-0.0.1.tar.gz` & `tmp/pydt3-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydt3-0.0.1.tar", last modified: Mon May  1 21:46:07 2023, max compression
+gzip compressed data, was "pydt3-0.0.2.tar", last modified: Tue May  2 09:58:38 2023, max compression
```

## Comparing `pydt3-0.0.1.tar` & `pydt3-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 koc        (501) staff       (20)        0 2023-05-01 21:46:07.335149 pydt3-0.0.1/
--rw-r--r--   0 koc        (501) staff       (20)     1057 2023-05-01 21:26:29.000000 pydt3-0.0.1/LICENSE.txt
--rw-r--r--   0 koc        (501) staff       (20)     2589 2023-05-01 21:46:07.334734 pydt3-0.0.1/PKG-INFO
--rw-r--r--   0 koc        (501) staff       (20)     2179 2023-05-01 21:42:45.000000 pydt3-0.0.1/README.md
-drwxr-xr-x   0 koc        (501) staff       (20)        0 2023-05-01 21:46:07.314158 pydt3-0.0.1/pydt3/
--rw-r--r--   0 koc        (501) staff       (20)       75 2023-05-01 16:57:05.000000 pydt3-0.0.1/pydt3/__init__.py
--rw-r--r--   0 koc        (501) staff       (20)    12818 2023-05-01 20:52:52.000000 pydt3-0.0.1/pydt3/devonthink.py
--rw-r--r--   0 koc        (501) staff       (20)     4750 2023-05-01 18:37:35.000000 pydt3-0.0.1/pydt3/jxa_helper.scpt
-drwxr-xr-x   0 koc        (501) staff       (20)        0 2023-05-01 21:46:07.333414 pydt3-0.0.1/pydt3/models/
--rw-r--r--   0 koc        (501) staff       (20)        0 2023-05-01 19:54:18.000000 pydt3-0.0.1/pydt3/models/__init__.py
--rw-r--r--   0 koc        (501) staff       (20)     3643 2023-05-01 20:20:12.000000 pydt3-0.0.1/pydt3/models/database.py
--rw-r--r--   0 koc        (501) staff       (20)      254 2023-05-01 13:05:27.000000 pydt3-0.0.1/pydt3/models/item.py
--rw-r--r--   0 koc        (501) staff       (20)    20714 2023-05-01 20:20:15.000000 pydt3-0.0.1/pydt3/models/record.py
--rw-r--r--   0 koc        (501) staff       (20)     2272 2023-04-29 13:54:14.000000 pydt3-0.0.1/pydt3/models/reminder.py
--rw-r--r--   0 koc        (501) staff       (20)     1372 2023-05-01 14:40:42.000000 pydt3-0.0.1/pydt3/models/smartgroup.py
--rw-r--r--   0 koc        (501) staff       (20)        0 2023-04-29 15:08:38.000000 pydt3-0.0.1/pydt3/models/tab.py
--rw-r--r--   0 koc        (501) staff       (20)     1916 2023-05-01 20:20:12.000000 pydt3-0.0.1/pydt3/models/text.py
--rw-r--r--   0 koc        (501) staff       (20)     6074 2023-05-01 20:20:12.000000 pydt3-0.0.1/pydt3/models/windows.py
--rw-r--r--   0 koc        (501) staff       (20)     7492 2023-05-01 18:34:27.000000 pydt3-0.0.1/pydt3/osascript.py
--rw-r--r--   0 koc        (501) staff       (20)        0 2023-04-29 05:42:20.000000 pydt3-0.0.1/pydt3/utils.py
-drwxr-xr-x   0 koc        (501) staff       (20)        0 2023-05-01 21:46:07.316587 pydt3-0.0.1/pydt3.egg-info/
--rw-r--r--   0 koc        (501) staff       (20)     2589 2023-05-01 21:46:07.000000 pydt3-0.0.1/pydt3.egg-info/PKG-INFO
--rw-r--r--   0 koc        (501) staff       (20)      485 2023-05-01 21:46:07.000000 pydt3-0.0.1/pydt3.egg-info/SOURCES.txt
--rw-r--r--   0 koc        (501) staff       (20)        1 2023-05-01 21:46:07.000000 pydt3-0.0.1/pydt3.egg-info/dependency_links.txt
--rw-r--r--   0 koc        (501) staff       (20)       77 2023-05-01 21:46:07.000000 pydt3-0.0.1/pydt3.egg-info/requires.txt
--rw-r--r--   0 koc        (501) staff       (20)        6 2023-05-01 21:46:07.000000 pydt3-0.0.1/pydt3.egg-info/top_level.txt
--rw-r--r--   0 koc        (501) staff       (20)      714 2023-05-01 21:22:15.000000 pydt3-0.0.1/pyproject.toml
--rw-r--r--   0 koc        (501) staff       (20)       38 2023-05-01 21:46:07.335286 pydt3-0.0.1/setup.cfg
+drwxr-xr-x   0 koc        (501) staff       (20)        0 2023-05-02 09:58:38.566415 pydt3-0.0.2/
+-rw-r--r--   0 koc        (501) staff       (20)     1057 2023-05-01 21:26:29.000000 pydt3-0.0.2/LICENSE.txt
+-rw-r--r--   0 koc        (501) staff       (20)     2592 2023-05-02 09:58:38.565089 pydt3-0.0.2/PKG-INFO
+-rw-r--r--   0 koc        (501) staff       (20)     2182 2023-05-02 09:46:56.000000 pydt3-0.0.2/README.md
+drwxr-xr-x   0 koc        (501) staff       (20)        0 2023-05-02 09:58:38.545025 pydt3-0.0.2/pydt3/
+-rw-r--r--   0 koc        (501) staff       (20)       75 2023-05-01 16:57:05.000000 pydt3-0.0.2/pydt3/__init__.py
+-rw-r--r--   0 koc        (501) staff       (20)    13572 2023-05-02 09:46:43.000000 pydt3-0.0.2/pydt3/devonthink.py
+-rw-r--r--   0 koc        (501) staff       (20)     4780 2023-05-02 09:35:29.000000 pydt3-0.0.2/pydt3/jxa_helper.scpt
+drwxr-xr-x   0 koc        (501) staff       (20)        0 2023-05-02 09:58:38.563463 pydt3-0.0.2/pydt3/models/
+-rw-r--r--   0 koc        (501) staff       (20)        0 2023-05-01 19:54:18.000000 pydt3-0.0.2/pydt3/models/__init__.py
+-rw-r--r--   0 koc        (501) staff       (20)     3643 2023-05-01 20:20:12.000000 pydt3-0.0.2/pydt3/models/database.py
+-rw-r--r--   0 koc        (501) staff       (20)      254 2023-05-01 13:05:27.000000 pydt3-0.0.2/pydt3/models/item.py
+-rw-r--r--   0 koc        (501) staff       (20)    20714 2023-05-01 20:20:15.000000 pydt3-0.0.2/pydt3/models/record.py
+-rw-r--r--   0 koc        (501) staff       (20)     2272 2023-04-29 13:54:14.000000 pydt3-0.0.2/pydt3/models/reminder.py
+-rw-r--r--   0 koc        (501) staff       (20)     1372 2023-05-01 14:40:42.000000 pydt3-0.0.2/pydt3/models/smartgroup.py
+-rw-r--r--   0 koc        (501) staff       (20)        0 2023-04-29 15:08:38.000000 pydt3-0.0.2/pydt3/models/tab.py
+-rw-r--r--   0 koc        (501) staff       (20)     1916 2023-05-01 20:20:12.000000 pydt3-0.0.2/pydt3/models/text.py
+-rw-r--r--   0 koc        (501) staff       (20)     6074 2023-05-01 20:20:12.000000 pydt3-0.0.2/pydt3/models/windows.py
+-rw-r--r--   0 koc        (501) staff       (20)     7492 2023-05-01 18:34:27.000000 pydt3-0.0.2/pydt3/osascript.py
+-rw-r--r--   0 koc        (501) staff       (20)        0 2023-04-29 05:42:20.000000 pydt3-0.0.2/pydt3/utils.py
+drwxr-xr-x   0 koc        (501) staff       (20)        0 2023-05-02 09:58:38.550332 pydt3-0.0.2/pydt3.egg-info/
+-rw-r--r--   0 koc        (501) staff       (20)     2592 2023-05-02 09:58:38.000000 pydt3-0.0.2/pydt3.egg-info/PKG-INFO
+-rw-r--r--   0 koc        (501) staff       (20)      485 2023-05-02 09:58:38.000000 pydt3-0.0.2/pydt3.egg-info/SOURCES.txt
+-rw-r--r--   0 koc        (501) staff       (20)        1 2023-05-02 09:58:38.000000 pydt3-0.0.2/pydt3.egg-info/dependency_links.txt
+-rw-r--r--   0 koc        (501) staff       (20)       77 2023-05-02 09:58:38.000000 pydt3-0.0.2/pydt3.egg-info/requires.txt
+-rw-r--r--   0 koc        (501) staff       (20)        6 2023-05-02 09:58:38.000000 pydt3-0.0.2/pydt3.egg-info/top_level.txt
+-rw-r--r--   0 koc        (501) staff       (20)      714 2023-05-02 09:58:03.000000 pydt3-0.0.2/pyproject.toml
+-rw-r--r--   0 koc        (501) staff       (20)       38 2023-05-02 09:58:38.566946 pydt3-0.0.2/setup.cfg
```

### Comparing `pydt3-0.0.1/LICENSE.txt` & `pydt3-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydt3-0.0.1/PKG-INFO` & `pydt3-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pydt3
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python API for Devonthink 3 utilizes AppleScript (JXA) and PyObjC.
 Author-email: astrosheep <astrosheepthesheep@outlook.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # PyDT3 - The Python API For DEVONthink 3
 
-This Python API for Devonthink 3 utilizes AppleScript (JXA) and PyObjC.
+The Python API for Devonthink 3 utilizes AppleScript (JXA) and PyObjC.
 
 Most of the APIs are directly mapped to AppleScript (JXA).
 For example, these two are equivalent:
 
 ```python
 from pydt3 import DEVONthink3
 dt3 = DEVONthink3()
@@ -44,18 +44,18 @@
 
 ## Quick Start
 
 ```python
 from pydt3 import DEVONthink3
 dtp3 = DEVONthink3()
 
-inbox = dtp3.ext.inbox
+inbox = dtp3.inbox
 
 # create a new folder in inbox
-dtp3.create_location('hello-from-pydt3', inbox)
+dtp3.create_location('new-group-from-pydt3', inbox)
 
 # get selected records
 records = dtp3.selected_records
 
 # get the first selected record and print its information
 if records:
     first = records[0]
@@ -70,15 +70,15 @@
     'type': 'markdown',
     'plain text': '# Hello from pydt3',
 }, inbox)
 ```
 
 ## Documentation
 
-Unlike many other API wrapper projects, PyDT3 is well documented thanks to the detailed AppleScript dictionary by DEVONthink team and code generation ability of ChatGTP.
+Unlike many other API wrapper projects, PyDT3 is well documented thanks to the detailed AppleScript dictionary by DEVONthink team and the code generation ability of ChatGTP.
 
 You can check the documentation either in source code (`docstring`), code editor (if properly configured), or the documentation site (not available at the time).
 
 ![documentation-in-editor](images/create_record_with_doc.png)
 
 ## Requirements
```

### Comparing `pydt3-0.0.1/README.md` & `pydt3-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # PyDT3 - The Python API For DEVONthink 3
 
-This Python API for Devonthink 3 utilizes AppleScript (JXA) and PyObjC.
+The Python API for Devonthink 3 utilizes AppleScript (JXA) and PyObjC.
 
 Most of the APIs are directly mapped to AppleScript (JXA).
 For example, these two are equivalent:
 
 ```python
 from pydt3 import DEVONthink3
 dt3 = DEVONthink3()
@@ -32,18 +32,18 @@
 
 ## Quick Start
 
 ```python
 from pydt3 import DEVONthink3
 dtp3 = DEVONthink3()
 
-inbox = dtp3.ext.inbox
+inbox = dtp3.inbox
 
 # create a new folder in inbox
-dtp3.create_location('hello-from-pydt3', inbox)
+dtp3.create_location('new-group-from-pydt3', inbox)
 
 # get selected records
 records = dtp3.selected_records
 
 # get the first selected record and print its information
 if records:
     first = records[0]
@@ -58,15 +58,15 @@
     'type': 'markdown',
     'plain text': '# Hello from pydt3',
 }, inbox)
 ```
 
 ## Documentation
 
-Unlike many other API wrapper projects, PyDT3 is well documented thanks to the detailed AppleScript dictionary by DEVONthink team and code generation ability of ChatGTP.
+Unlike many other API wrapper projects, PyDT3 is well documented thanks to the detailed AppleScript dictionary by DEVONthink team and the code generation ability of ChatGTP.
 
 You can check the documentation either in source code (`docstring`), code editor (if properly configured), or the documentation site (not available at the time).
 
 ![documentation-in-editor](images/create_record_with_doc.png)
 
 ## Requirements
```

### Comparing `pydt3-0.0.1/pydt3/devonthink.py` & `pydt3-0.0.2/pydt3/devonthink.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,70 +48,70 @@
     def viewer_windows(self) -> List[ViewerWindow]:
         return self.get_property_native('viewerWindows')
 
     # properties
     @property
     def bates_number(self) -> int:
         """Current bates number."""
-        return self.window.get_property('bates number')
+        return self.get_property_native('batesNumber')
 
     @property
     def cancelled_progress(self) -> bool:
         """Specifies if a process with visible progress indicator should be cancelled."""
-        return self.window.get_property('cancelled progress')
+        return self.get_property_native('cancelledProgress')
 
     @property
     def content_record(self) -> Record:
         """The record of the visible document in the frontmost think window."""
-        return self.window.get_property('content record')
+        return self.get_property_native('contentRecord')
 
     @property
     def current_database(self) -> Database:
         """The currently used database."""
-        return self.window.get_property('current database')
+        return self.get_property_native('currentDatabase')
 
     @property
     def current_group(self) -> Record:
         """The (selected) group of the frontmost window of the current database. Returns root of current database if no current group exists."""
-        return self.window.get_property('current group')
+        return self.get_property_native('currentGroup')
 
     @property
     def current_workspace(self) -> str:
         """The name of the currently used workspace."""
-        return self.window.get_property('current workspace')
+        return self.get_property_native('currentWorkspace')
 
     @property
     def inbox(self) -> Database:
         """The global inbox."""
-        return self.window.get_property('inbox')
+        return self.get_property_native('inbox')
 
     @property
     def incoming_group(self) -> Record:
         """The default group for new notes. Either global inbox or incoming group of current database if global inbox isn't available."""
-        return self.window.get_property('incoming group')
+        return self.get_property_native('incomingGroup')
 
     @property
     def last_downloaded_URL(self) -> str:
         """The actual URL of the last download."""
-        return self.window.get_property('last downloaded URL')
+        return self.get_property_native('lastDownloadedURL')
 
     @property
     def last_downloaded_response(self) -> Record:
         """HTTP-Status, Last-Modified, Content-Type, Content-Length and Charset of last HTTP(S) response."""
-        return self.window.get_property('last downloaded response')
+        return self.get_property_native('lastDownloadedResponse')
 
     @property
     def preferred_import_destination(self) -> Record:
         """The default destination for data from external sources. See Preferences > Import > Destination."""
-        return self.window.get_property('preferred import destination')
+        return self.get_property_native('preferredImportDestination')
 
     @property
     def reading_list(self) -> List[dict]:
         """The items of the reading list."""
-        return self.window.get_property('reading list')
+        return self.get_property_native('readingList')
 
     @property
     def selection(self) -> list:
         """Not implemented due to the poor document. Plus it's 
         officially not recommanded:
 
             selection (list, r/o) : The current selection of
@@ -122,17 +122,41 @@
 
         """
         raise NotImplementedError()
 
     @property
     def workspaces(self) -> List[str]:
         """The names of all available workspaces."""
-        return self.window.get_property('workspaces')
+        return self.get_property_native('workspaces')
     
     # methods
+    ## standard additions
+    def display_dialog(self, text: str, place_holder: str = None, buttons: List[str]=None, default_button: str = None, with_icon: str = None) -> str:
+        """Display a dialog.
+
+        Args:
+            text (str): The text to display.
+            place_holder (str): The placeholder text.
+            with_icon (str): The icon to display.
+            buttons (List[str]): The buttons to display.
+            default_button (str): The default button.
+
+        Returns:
+            str: The selected button.
+        """
+        kwargs = {
+            'defaultAnswer': place_holder,
+            'buttons': buttons,
+            'defaultButton': default_button,
+            'withIcon': with_icon,
+        }
+
+        kwargs = {k: v for k, v in kwargs.items() if v is not None}
+        return self.run_method('displayDialog', [text], kwargs)
+    
     def search(self, text: str, comparision: str = 'no case', excludeSubgroups: bool = False) -> List[Record]:
         """Search for records in specified group or all databases.
 
         Args:
             text (str): The search string.
             comparision (str, optional):  The comparison to use (default `'no case'`). One of fuzzy/‌no case/‌no umlauts.
             excludeSubgroups (bool, optional): Don't search in subgroups of the specified group. (default `false`).
@@ -318,12 +342,8 @@
     def __init__(self, app: DEVONthink3):
         self.app = app
     
     def db_by_name(self, name: str) -> Optional[Database]:
         dbs = self.app.databases
         for db in dbs:
             if db.name == name:
-                return db
-    
-    @property
-    def inbox(self) -> Optional[Database]:
-        return self.db_by_name('Inbox')
+                return db
```

### Comparing `pydt3-0.0.1/pydt3/jxa_helper.scpt` & `pydt3-0.0.2/pydt3/jxa_helper.scpt`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4a73 4f73 6144 4153 312e 3030 312e 3030  JsOsaDAS1.001.00
 00000010: 6270 6c69 7374 3030 d101 0256 7363 7269  bplist00...Vscri
-00000020: 7074 5f11 1236 636f 6e73 7420 6765 744f  pt_..6const getO
+00000020: 7074 5f11 1254 636f 6e73 7420 6765 744f  pt_..Tconst getO
 00000030: 626a 6563 7449 6420 3d20 2828 2920 3d3e  bjectId = (() =>
 00000040: 207b 0a20 2020 206c 6574 2063 6f75 6e74   {.    let count
 00000050: 203d 2030 3b0a 2020 2020 636f 6e73 7420   = 0;.    const 
 00000060: 6f62 6a49 644d 6170 203d 206e 6577 2057  objIdMap = new W
 00000070: 6561 6b4d 6170 2829 3b0a 2020 2020 7265  eakMap();.    re
 00000080: 7475 726e 2028 6f62 6a65 6374 2920 3d3e  turn (object) =>
 00000090: 207b 0a20 2020 2020 2063 6f6e 7374 206f   {.      const o
@@ -49,249 +49,251 @@
 00000300: 2920 7b0a 2020 2020 7265 7475 726e 206f  ) {.    return o
 00000310: 626a 203d 3d3d 206e 756c 6c20 7c7c 205b  bj === null || [
 00000320: 2775 6e64 6566 696e 6564 272c 2027 7374  'undefined', 'st
 00000330: 7269 6e67 272c 2027 6e75 6d62 6572 272c  ring', 'number',
 00000340: 2027 626f 6f6c 6561 6e27 5d2e 696e 636c   'boolean'].incl
 00000350: 7564 6573 2874 7970 656f 6620 6f62 6a29  udes(typeof obj)
 00000360: 3b0a 7d0a 0a66 756e 6374 696f 6e20 6973  ;.}..function is
-00000370: 506c 6169 6e4a 736f 6e28 6f62 6a29 207b  PlainJson(obj) {
-00000380: 0a20 2020 2069 6620 2869 734a 736f 6e4e  .    if (isJsonN
-00000390: 6f64 6556 616c 7565 286f 626a 2929 207b  odeValue(obj)) {
-000003a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000003b0: 7472 7565 3b0a 2020 2020 7d20 656c 7365  true;.    } else
-000003c0: 2069 6620 2874 7970 656f 6620 6f62 6a20   if (typeof obj 
-000003d0: 3d3d 3d20 276f 626a 6563 7427 2920 7b0a  === 'object') {.
-000003e0: 2020 2020 2020 2020 666f 7220 286c 6574          for (let
-000003f0: 206b 2069 6e20 6f62 6a29 207b 0a20 2020   k in obj) {.   
-00000400: 2020 2020 2020 2020 2069 6620 2821 6973           if (!is
-00000410: 4a73 6f6e 4e6f 6465 5661 6c75 6528 6f62  JsonNodeValue(ob
-00000420: 6a5b 6b5d 2929 207b 0a20 2020 2020 2020  j[k])) {.       
-00000430: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00000440: 6661 6c73 653b 0a20 2020 2020 2020 2020  false;.         
-00000450: 2020 207d 0a20 2020 2020 2020 207d 0a20     }.        }. 
-00000460: 2020 2020 2020 2072 6574 7572 6e20 7472         return tr
-00000470: 7565 3b0a 2020 2020 7d20 656c 7365 2069  ue;.    } else i
-00000480: 6620 2874 7970 656f 6620 6f62 6a20 3d3d  f (typeof obj ==
-00000490: 3d20 2766 756e 6374 696f 6e27 2920 7b0a  = 'function') {.
-000004a0: 2020 2020 2020 2020 7265 7475 726e 2066          return f
-000004b0: 616c 7365 3b0a 2020 2020 7d0a 7d0a 0a66  alse;.    }.}..f
-000004c0: 756e 6374 696f 6e20 7772 6170 4f62 6a53  unction wrapObjS
-000004d0: 7065 6354 6f4a 736f 6e28 6f62 6a53 7065  pecToJson(objSpe
-000004e0: 6329 207b 0a20 2020 206c 6574 2065 7661  c) {.    let eva
-000004f0: 6c75 6174 6564 203d 206f 626a 5370 6563  luated = objSpec
-00000500: 2829 3b0a 0a20 2020 206c 6574 2063 6c61  ();..    let cla
-00000510: 7373 4f66 203d 204f 626a 6563 7453 7065  ssOf = ObjectSpe
-00000520: 6369 6669 6572 2e63 6c61 7373 4f66 286f  cifier.classOf(o
-00000530: 626a 5370 6563 293b 0a20 2020 2069 6620  bjSpec);.    if 
-00000540: 2863 6c61 7373 4f66 203d 3d3d 2027 6170  (classOf === 'ap
-00000550: 706c 6963 6174 696f 6e27 2920 7b0a 2020  plication') {.  
-00000560: 2020 2020 2020 7265 7475 726e 207b 0a20        return {. 
-00000570: 2020 2020 2020 2020 2020 206e 616d 653a             name:
-00000580: 206f 626a 5370 6563 2e6e 616d 6528 292c   objSpec.name(),
-00000590: 0a20 2020 2020 2020 2020 2020 2074 7970  .            typ
-000005a0: 653a 2027 7265 6665 7265 6e63 6527 2c0a  e: 'reference',.
-000005b0: 2020 2020 2020 2020 2020 2020 7261 7749              rawI
-000005c0: 643a 2067 6574 4f62 6a65 6374 4964 286f  d: getObjectId(o
-000005d0: 626a 5370 6563 292c 0a20 2020 2020 2020  bjSpec),.       
-000005e0: 2020 2020 206f 626a 4964 3a20 6361 6368       objId: cach
-000005f0: 654f 626a 6374 286f 626a 5370 6563 292c  eObjct(objSpec),
-00000600: 0a20 2020 2020 2020 2020 2020 2063 6c61  .            cla
-00000610: 7373 4e61 6d65 3a20 636c 6173 734f 660a  ssName: classOf.
-00000620: 2020 2020 2020 2020 7d0a 2020 2020 7d0a          }.    }.
-00000630: 2020 2020 6966 2028 6973 506c 6169 6e4a      if (isPlainJ
-00000640: 736f 6e28 6576 616c 7561 7465 6429 2920  son(evaluated)) 
-00000650: 7b0a 2020 2020 2020 2020 6966 2028 6f62  {.        if (ob
-00000660: 6a53 7065 6320 696e 7374 616e 6365 6f66  jSpec instanceof
-00000670: 2044 6174 6529 207b 0a20 2020 2020 2020   Date) {.       
-00000680: 2020 2020 2072 6574 7572 6e20 7b0a 2020       return {.  
-00000690: 2020 2020 2020 2020 2020 2020 2020 7479                ty
-000006a0: 7065 3a20 2776 616c 7565 272c 0a20 2020  pe: 'value',.   
-000006b0: 2020 2020 2020 2020 2020 2020 2064 6174               dat
-000006c0: 613a 206f 626a 5370 6563 2e74 6f49 534f  a: objSpec.toISO
-000006d0: 5374 7269 6e67 2829 0a20 2020 2020 2020  String().       
-000006e0: 2020 2020 207d 0a20 2020 2020 2020 207d       }.        }
-000006f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00000700: 7b0a 2020 2020 2020 2020 2020 2020 7479  {.            ty
-00000710: 7065 3a20 2776 616c 7565 272c 0a20 2020  pe: 'value',.   
-00000720: 2020 2020 2020 2020 2064 6174 613a 2065           data: e
-00000730: 7661 6c75 6174 6564 0a20 2020 2020 2020  valuated.       
-00000740: 207d 0a20 2020 207d 0a0a 2020 2020 6966   }.    }..    if
-00000750: 2028 7479 7065 6f66 2065 7661 6c75 6174   (typeof evaluat
-00000760: 6564 203d 3d3d 2027 6f62 6a65 6374 2729  ed === 'object')
-00000770: 207b 0a20 2020 2020 2020 2066 6f72 2028   {.        for (
-00000780: 6c65 7420 6b20 696e 2065 7661 6c75 6174  let k in evaluat
-00000790: 6564 2920 7b0a 2020 2020 2020 2020 2020  ed) {.          
-000007a0: 2020 6576 616c 7561 7465 645b 6b5d 203d    evaluated[k] =
-000007b0: 2077 7261 704f 626a 5370 6563 546f 4a73   wrapObjSpecToJs
-000007c0: 6f6e 286f 626a 5370 6563 5b6b 5d29 3b0a  on(objSpec[k]);.
-000007d0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-000007e0: 2020 7265 7475 726e 207b 0a20 2020 2020    return {.     
-000007f0: 2020 2020 2020 2074 7970 653a 2027 636f         type: 'co
-00000800: 6e74 6169 6e65 7227 2c0a 2020 2020 2020  ntainer',.      
-00000810: 2020 2020 2020 6461 7461 3a20 6576 616c        data: eval
-00000820: 7561 7465 642c 0a20 2020 2020 2020 207d  uated,.        }
-00000830: 3b0a 2020 2020 7d20 0a20 2020 200a 2020  ;.    } .    .  
-00000840: 2020 6966 2028 636c 6173 734f 6620 213d    if (classOf !=
-00000850: 3d20 756e 6465 6669 6e65 6429 207b 0a20  = undefined) {. 
-00000860: 2020 2020 2020 202f 2f20 7468 726f 7720         // throw 
-00000870: 6e65 7720 4572 726f 7228 6055 6e6b 6e6f  new Error(`Unkno
-00000880: 776e 2074 7970 653a 2024 7b74 7970 656f  wn type: ${typeo
-00000890: 6620 6f62 6a53 7063 7d60 293b 0a20 2020  f objSpc}`);.   
-000008a0: 2020 2020 2072 6574 7572 6e20 7b0a 2020       return {.  
-000008b0: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
-000008c0: 2772 6566 6572 656e 6365 272c 0a20 2020  'reference',.   
-000008d0: 2020 2020 2020 2020 206f 626a 4964 3a20           objId: 
-000008e0: 6361 6368 654f 626a 6374 286f 626a 5370  cacheObjct(objSp
-000008f0: 6563 292c 0a20 2020 2020 2020 2020 2020  ec),.           
-00000900: 2063 6c61 7373 4e61 6d65 3a20 636c 6173   className: clas
-00000910: 734f 660a 2020 2020 2020 2020 7d0a 2020  sOf.        }.  
-00000920: 2020 7d20 0a20 2020 200a 2020 2020 0a20    } .    .    . 
-00000930: 2020 2074 6872 6f77 206e 6577 2045 7272     throw new Err
-00000940: 6f72 2860 556e 6b6e 6f77 6e20 7479 7065  or(`Unknown type
-00000950: 3a20 247b 7479 7065 6f66 206f 626a 5370  : ${typeof objSp
-00000960: 6563 7d60 293b 0a7d 0a0a 6675 6e63 7469  ec}`);.}..functi
-00000970: 6f6e 2075 6e77 7261 704f 626a 4672 6f6d  on unwrapObjFrom
-00000980: 4a73 6f6e 286f 626a 2920 7b0a 2020 2020  Json(obj) {.    
-00000990: 6966 2028 6f62 6a2e 7479 7065 203d 3d3d  if (obj.type ===
-000009a0: 2027 7661 6c75 6527 2920 7b0a 2020 2020   'value') {.    
-000009b0: 2020 2020 7265 7475 726e 206f 626a 2e64      return obj.d
-000009c0: 6174 613b 0a20 2020 207d 2065 6c73 6520  ata;.    } else 
-000009d0: 6966 2028 6f62 6a2e 7479 7065 203d 3d3d  if (obj.type ===
-000009e0: 2027 636f 6e74 6169 6e65 7227 2920 7b0a   'container') {.
-000009f0: 2020 2020 2020 2020 666f 7220 286c 6574          for (let
-00000a00: 206b 2069 6e20 6f62 6a2e 6461 7461 2920   k in obj.data) 
-00000a10: 7b0a 2020 2020 2020 2020 2020 2020 6f62  {.            ob
-00000a20: 6a2e 6461 7461 5b6b 5d20 3d20 756e 7772  j.data[k] = unwr
-00000a30: 6170 4f62 6a46 726f 6d4a 736f 6e28 6f62  apObjFromJson(ob
-00000a40: 6a2e 6461 7461 5b6b 5d29 3b0a 2020 2020  j.data[k]);.    
-00000a50: 2020 2020 7d0a 2020 2020 2020 2020 7265      }.        re
-00000a60: 7475 726e 206f 626a 2e64 6174 613b 0a20  turn obj.data;. 
-00000a70: 2020 207d 2065 6c73 6520 6966 2028 6f62     } else if (ob
-00000a80: 6a2e 7479 7065 203d 3d3d 2027 7265 6665  j.type === 'refe
-00000a90: 7265 6e63 6527 2920 7b0a 2020 2020 2020  rence') {.      
-00000aa0: 2020 7265 7475 726e 2067 6574 4361 6368    return getCach
-00000ab0: 6564 4f62 6a65 6374 286f 626a 2e6f 626a  edObject(obj.obj
-00000ac0: 4964 293b 0a20 2020 207d 0a7d 0a0a 6675  Id);.    }.}..fu
-00000ad0: 6e63 7469 6f6e 2067 6574 4170 706c 6963  nction getApplic
-00000ae0: 6174 696f 6e28 7061 7261 6d73 2920 7b0a  ation(params) {.
-00000af0: 2020 2020 6c65 7420 6e61 6d65 203d 2070      let name = p
-00000b00: 6172 616d 732e 6e61 6d65 3b0a 2020 2020  arams.name;.    
-00000b10: 6c65 7420 6170 7020 3d20 4170 706c 6963  let app = Applic
-00000b20: 6174 696f 6e28 6e61 6d65 293b 0a20 2020  ation(name);.   
-00000b30: 2072 6574 7572 6e20 7772 6170 4f62 6a53   return wrapObjS
-00000b40: 7065 6354 6f4a 736f 6e28 6170 7029 3b0a  pecToJson(app);.
-00000b50: 7d0a 6765 7441 7070 6c69 6361 7469 6f6e  }.getApplication
-00000b60: 203d 206a 736f 6e49 4f57 7261 7070 6572   = jsonIOWrapper
-00000b70: 2867 6574 4170 706c 6963 6174 696f 6e29  (getApplication)
-00000b80: 3b0a 0a66 756e 6374 696f 6e20 6765 7450  ;..function getP
-00000b90: 726f 7065 7274 6965 7328 7061 7261 6d73  roperties(params
-00000ba0: 2920 7b0a 2020 2020 6c65 7420 6f62 6a49  ) {.    let objI
-00000bb0: 6420 3d20 7061 7261 6d73 2e6f 626a 4964  d = params.objId
-00000bc0: 3b0a 2020 2020 6c65 7420 6e61 6d65 7320  ;.    let names 
-00000bd0: 3d20 7061 7261 6d73 2e6e 616d 6573 3b0a  = params.names;.
-00000be0: 2020 2020 6c65 7420 6f62 6a20 3d20 6f62      let obj = ob
-00000bf0: 6a65 6374 4361 6368 654d 6170 5b6f 626a  jectCacheMap[obj
-00000c00: 4964 5d3b 0a20 2020 206c 6574 2064 6174  Id];.    let dat
-00000c10: 6120 3d20 7b7d 3b0a 2020 2020 666f 7220  a = {};.    for 
-00000c20: 286c 6574 206e 206f 6620 6e61 6d65 7329  (let n of names)
-00000c30: 207b 0a20 2020 2020 2020 206c 6574 2070   {.        let p
-00000c40: 726f 7065 7274 7920 3d20 6f62 6a5b 6e5d  roperty = obj[n]
-00000c50: 3b0a 2020 2020 2020 2020 6461 7461 5b6e  ;.        data[n
-00000c60: 5d20 3d20 7772 6170 4f62 6a53 7065 6354  ] = wrapObjSpecT
-00000c70: 6f4a 736f 6e28 7072 6f70 6572 7479 293b  oJson(property);
-00000c80: 0a20 2020 207d 0a20 2020 2072 6574 7572  .    }.    retur
-00000c90: 6e20 6461 7461 3b0a 7d0a 6765 7450 726f  n data;.}.getPro
-00000ca0: 7065 7274 6965 7320 3d20 6a73 6f6e 494f  perties = jsonIO
-00000cb0: 5772 6170 7065 7228 6765 7450 726f 7065  Wrapper(getPrope
-00000cc0: 7274 6965 7329 3b0a 0a0a 6675 6e63 7469  rties);...functi
-00000cd0: 6f6e 2073 6574 5072 6f70 6572 7479 5661  on setPropertyVa
-00000ce0: 6c75 6573 2870 6172 616d 7329 207b 0a20  lues(params) {. 
-00000cf0: 2020 206c 6574 206f 626a 4964 203d 2070     let objId = p
-00000d00: 6172 616d 732e 6f62 6a49 643b 0a20 2020  arams.objId;.   
-00000d10: 206c 6574 2070 726f 7065 7274 6965 7320   let properties 
-00000d20: 3d20 7061 7261 6d73 2e70 726f 7065 7274  = params.propert
-00000d30: 6965 733b 0a0a 2020 2020 6c65 7420 6f62  ies;..    let ob
-00000d40: 6a20 3d20 6f62 6a65 6374 4361 6368 654d  j = objectCacheM
-00000d50: 6170 5b6f 626a 4964 5d3b 0a0a 2020 2020  ap[objId];..    
-00000d60: 666f 7220 286c 6574 206e 2069 6e20 7072  for (let n in pr
-00000d70: 6f70 6572 7469 6573 2920 7b0a 2020 2020  operties) {.    
-00000d80: 2020 2020 6c65 7420 7661 6c75 6520 3d20      let value = 
-00000d90: 7072 6f70 6572 7469 6573 5b6e 5d3b 0a20  properties[n];. 
-00000da0: 2020 2020 2020 206f 626a 5b6e 5d20 3d20         obj[n] = 
-00000db0: 7661 6c75 653b 0a20 2020 207d 0a20 2020  value;.    }.   
-00000dc0: 2072 6574 7572 6e20 7b7d 3b0a 7d0a 7365   return {};.}.se
-00000dd0: 7450 726f 7065 7274 7956 616c 7565 7320  tPropertyValues 
-00000de0: 3d20 6a73 6f6e 494f 5772 6170 7065 7228  = jsonIOWrapper(
-00000df0: 7365 7450 726f 7065 7274 7956 616c 7565  setPropertyValue
-00000e00: 7329 3b0a 0a66 756e 6374 696f 6e20 7275  s);..function ru
-00000e10: 6e4d 6574 686f 6428 7061 7261 6d73 2920  nMethod(params) 
-00000e20: 7b0a 2020 2020 6c65 7420 6f62 6a49 6420  {.    let objId 
-00000e30: 3d20 7061 7261 6d73 2e6f 626a 4964 3b0a  = params.objId;.
-00000e40: 2020 2020 6c65 7420 6e61 6d65 203d 2070      let name = p
-00000e50: 6172 616d 732e 6e61 6d65 3b0a 2020 2020  arams.name;.    
-00000e60: 6c65 7420 6172 6773 203d 2070 6172 616d  let args = param
-00000e70: 732e 6172 6773 3b0a 2020 2020 666f 7220  s.args;.    for 
-00000e80: 286c 6574 2069 203d 2030 3b20 6920 3c20  (let i = 0; i < 
-00000e90: 6172 6773 2e6c 656e 6774 683b 2069 2b2b  args.length; i++
-00000ea0: 2920 7b0a 2020 2020 2020 2020 6172 6773  ) {.        args
-00000eb0: 5b69 5d20 3d20 756e 7772 6170 4f62 6a46  [i] = unwrapObjF
-00000ec0: 726f 6d4a 736f 6e28 6172 6773 5b69 5d29  romJson(args[i])
-00000ed0: 3b0a 2020 2020 7d0a 2020 2020 6c65 7420  ;.    }.    let 
-00000ee0: 6b77 6172 6773 203d 207b 7d3b 0a20 2020  kwargs = {};.   
-00000ef0: 2066 6f72 2028 6c65 7420 6b20 696e 2070   for (let k in p
-00000f00: 6172 616d 732e 6b77 6172 6773 2920 7b0a  arams.kwargs) {.
-00000f10: 2020 2020 2020 2020 6b77 6172 6773 5b6b          kwargs[k
-00000f20: 5d20 3d20 756e 7772 6170 4f62 6a46 726f  ] = unwrapObjFro
-00000f30: 6d4a 736f 6e28 7061 7261 6d73 2e6b 7761  mJson(params.kwa
-00000f40: 7267 735b 6b5d 293b 0a20 2020 207d 0a0a  rgs[k]);.    }..
-00000f50: 2020 2020 6c65 7420 6f62 6a20 3d20 6f62      let obj = ob
-00000f60: 6a65 6374 4361 6368 654d 6170 5b6f 626a  jectCacheMap[obj
-00000f70: 4964 5d3b 0a20 2020 206c 6574 2072 6573  Id];.    let res
-00000f80: 756c 7420 3d20 6f62 6a5b 6e61 6d65 5d28  ult = obj[name](
-00000f90: 2e2e 2e61 7267 732c 206b 7761 7267 7329  ...args, kwargs)
-00000fa0: 3b0a 2020 2020 7265 7475 726e 2077 7261  ;.    return wra
-00000fb0: 704f 626a 5370 6563 546f 4a73 6f6e 2872  pObjSpecToJson(r
-00000fc0: 6573 756c 7429 3b0a 7d0a 7275 6e4d 6574  esult);.}.runMet
-00000fd0: 686f 6420 3d20 6a73 6f6e 494f 5772 6170  hod = jsonIOWrap
-00000fe0: 7065 7228 7275 6e4d 6574 686f 6429 3b0a  per(runMethod);.
-00000ff0: 0a0a 6675 6e63 7469 6f6e 2072 656c 6561  ..function relea
-00001000: 7365 4f62 6a65 6374 2870 6172 616d 7329  seObject(params)
-00001010: 207b 0a20 2020 206c 6574 206f 626a 4964   {.    let objId
-00001020: 203d 2070 6172 616d 732e 6f62 6a49 643b   = params.objId;
-00001030: 0a20 2020 2064 656c 6574 6520 6f62 6a65  .    delete obje
-00001040: 6374 4361 6368 654d 6170 5b6f 626a 4964  ctCacheMap[objId
-00001050: 5d3b 0a20 2020 2072 6574 7572 6e20 7b7d  ];.    return {}
-00001060: 3b0a 7d0a 7265 6c65 6173 654f 626a 6563  ;.}.releaseObjec
-00001070: 7420 3d20 6a73 6f6e 494f 5772 6170 7065  t = jsonIOWrappe
-00001080: 7228 7265 6c65 6173 654f 626a 6563 7429  r(releaseObject)
-00001090: 3b0a 0a66 756e 6374 696f 6e20 6361 6c6c  ;..function call
-000010a0: 5365 6c66 2870 6172 616d 7329 207b 0a20  Self(params) {. 
-000010b0: 2020 206c 6574 206f 626a 4964 203d 2070     let objId = p
-000010c0: 6172 616d 732e 6f62 6a49 643b 0a20 2020  arams.objId;.   
-000010d0: 206c 6574 2061 7267 7320 3d20 7061 7261   let args = para
-000010e0: 6d73 2e61 7267 733b 0a20 2020 200a 2020  ms.args;.    .  
-000010f0: 2020 666f 7220 286c 6574 2069 203d 2030    for (let i = 0
-00001100: 3b20 6920 3c20 6172 6773 2e6c 656e 6774  ; i < args.lengt
-00001110: 683b 2069 2b2b 2920 7b0a 2020 2020 2020  h; i++) {.      
-00001120: 2020 6172 6773 5b69 5d20 3d20 756e 7772    args[i] = unwr
-00001130: 6170 4f62 6a46 726f 6d4a 736f 6e28 6172  apObjFromJson(ar
-00001140: 6773 5b69 5d29 3b0a 2020 2020 7d0a 2020  gs[i]);.    }.  
-00001150: 2020 6c65 7420 6b77 6172 6773 203d 207b    let kwargs = {
-00001160: 7d3b 0a20 2020 2066 6f72 2028 6c65 7420  };.    for (let 
-00001170: 6b20 696e 2070 6172 616d 732e 6b77 6172  k in params.kwar
-00001180: 6773 2920 7b0a 2020 2020 2020 2020 6b77  gs) {.        kw
-00001190: 6172 6773 5b6b 5d20 3d20 756e 7772 6170  args[k] = unwrap
-000011a0: 4f62 6a46 726f 6d4a 736f 6e28 7061 7261  ObjFromJson(para
-000011b0: 6d73 2e6b 7761 7267 735b 6b5d 293b 0a20  ms.kwargs[k]);. 
-000011c0: 2020 207d 0a20 2020 206c 6574 206f 626a     }.    let obj
-000011d0: 203d 206f 626a 6563 7443 6163 6865 4d61   = objectCacheMa
-000011e0: 705b 6f62 6a49 645d 3b0a 2020 2020 6c65  p[objId];.    le
-000011f0: 7420 7265 7375 6c74 203d 206f 626a 282e  t result = obj(.
-00001200: 2e2e 6172 6773 2c20 6b77 6172 6773 293b  ..args, kwargs);
-00001210: 0a20 2020 2072 6574 7572 6e20 7772 6170  .    return wrap
-00001220: 4f62 6a53 7065 6354 6f4a 736f 6e28 7265  ObjSpecToJson(re
-00001230: 7375 6c74 293b 0a7d 0a63 616c 6c53 656c  sult);.}.callSel
-00001240: 6620 3d20 6a73 6f6e 494f 5772 6170 7065  f = jsonIOWrappe
-00001250: 7228 6361 6c6c 5365 6c66 293b 0008 000b  r(callSelf);....
-00001260: 0012 0000 0000 0000 0201 0000 0000 0000  ................
-00001270: 0003 0000 0000 0000 0000 0000 0000 0000  ................
-00001280: 124c 6a73 6372 0001 000c fade dead       .Ljscr........
+00000370: 506c 6169 6e4f 626a 286f 626a 2920 7b0a  PlainObj(obj) {.
+00000380: 2020 2020 6966 2028 6973 4a73 6f6e 4e6f      if (isJsonNo
+00000390: 6465 5661 6c75 6528 6f62 6a29 2920 7b0a  deValue(obj)) {.
+000003a0: 2020 2020 2020 2020 7265 7475 726e 2074          return t
+000003b0: 7275 653b 0a20 2020 207d 2065 6c73 6520  rue;.    } else 
+000003c0: 6966 2028 7479 7065 6f66 206f 626a 203d  if (typeof obj =
+000003d0: 3d3d 2027 6f62 6a65 6374 2729 207b 0a20  == 'object') {. 
+000003e0: 2020 2020 2020 2066 6f72 2028 6c65 7420         for (let 
+000003f0: 6b20 696e 206f 626a 2920 7b0a 2020 2020  k in obj) {.    
+00000400: 2020 2020 2020 2020 6966 2028 2169 734a          if (!isJ
+00000410: 736f 6e4e 6f64 6556 616c 7565 286f 626a  sonNodeValue(obj
+00000420: 5b6b 5d29 2920 7b0a 2020 2020 2020 2020  [k])) {.        
+00000430: 2020 2020 2020 2020 7265 7475 726e 2066          return f
+00000440: 616c 7365 3b0a 2020 2020 2020 2020 2020  alse;.          
+00000450: 2020 7d0a 2020 2020 2020 2020 7d0a 2020    }.        }.  
+00000460: 2020 2020 2020 7265 7475 726e 2074 7275        return tru
+00000470: 653b 0a20 2020 207d 2065 6c73 6520 6966  e;.    } else if
+00000480: 2028 7479 7065 6f66 206f 626a 203d 3d3d   (typeof obj ===
+00000490: 2027 6675 6e63 7469 6f6e 2729 207b 0a20   'function') {. 
+000004a0: 2020 2020 2020 2072 6574 7572 6e20 6661         return fa
+000004b0: 6c73 653b 0a20 2020 207d 0a7d 0a0a 0a66  lse;.    }.}...f
+000004c0: 756e 6374 696f 6e20 7772 6170 4f62 6a54  unction wrapObjT
+000004d0: 6f4a 736f 6e28 6f62 6a29 207b 0a0a 2020  oJson(obj) {..  
+000004e0: 2020 6966 2028 6973 4a73 6f6e 4e6f 6465    if (isJsonNode
+000004f0: 5661 6c75 6528 6f62 6a29 2920 7b0a 2020  Value(obj)) {.  
+00000500: 2020 2020 2020 7265 7475 726e 207b 0a20        return {. 
+00000510: 2020 2020 2020 2020 2020 2074 7970 653a             type:
+00000520: 2027 7661 6c75 6527 2c0a 2020 2020 2020   'value',.      
+00000530: 2020 2020 2020 6461 7461 3a20 6f62 6a0a        data: obj.
+00000540: 2020 2020 2020 2020 7d0a 2020 2020 7d0a          }.    }.
+00000550: 0a20 2020 2069 6620 2874 7970 656f 6620  .    if (typeof 
+00000560: 6f62 6a20 3d3d 3d20 276f 626a 6563 7427  obj === 'object'
+00000570: 2920 7b0a 2020 2020 2020 2020 6966 2028  ) {.        if (
+00000580: 6f62 6a20 696e 7374 616e 6365 6f66 2044  obj instanceof D
+00000590: 6174 6529 207b 0a20 2020 2020 2020 2020  ate) {.         
+000005a0: 2020 2072 6574 7572 6e20 7b0a 2020 2020     return {.    
+000005b0: 2020 2020 2020 2020 2020 2020 7479 7065              type
+000005c0: 3a20 2776 616c 7565 272c 0a20 2020 2020  : 'value',.     
+000005d0: 2020 2020 2020 2020 2020 2064 6174 613a             data:
+000005e0: 206f 626a 2e74 6f49 534f 5374 7269 6e67   obj.toISOString
+000005f0: 2829 0a20 2020 2020 2020 2020 2020 207d  ().            }
+00000600: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
+00000610: 2020 202f 2f20 4966 2069 7427 7320 6172     // If it's ar
+00000620: 7261 7920 6f72 2064 6963 740a 2020 2020  ray or dict.    
+00000630: 2020 2020 6966 2028 4172 7261 792e 6973      if (Array.is
+00000640: 4172 7261 7928 6f62 6a29 207c 7c20 6f62  Array(obj) || ob
+00000650: 6a2e 636f 6e73 7472 7563 746f 722e 6e61  j.constructor.na
+00000660: 6d65 203d 3d3d 2027 4f62 6a65 6374 2729  me === 'Object')
+00000670: 207b 0a20 2020 2020 2020 2020 2020 206c   {.            l
+00000680: 6574 2064 6174 6120 3d20 7b7d 3b0a 2020  et data = {};.  
+00000690: 2020 2020 2020 2020 2020 666f 7220 286c            for (l
+000006a0: 6574 2069 2069 6e20 6f62 6a29 207b 0a20  et i in obj) {. 
+000006b0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+000006c0: 6174 615b 695d 203d 2077 7261 704f 626a  ata[i] = wrapObj
+000006d0: 546f 4a73 6f6e 286f 626a 5b69 5d29 3b0a  ToJson(obj[i]);.
+000006e0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+000006f0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00000700: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00000710: 2020 2074 7970 653a 2027 636f 6e74 6169     type: 'contai
+00000720: 6e65 7227 2c0a 2020 2020 2020 2020 2020  ner',.          
+00000730: 2020 2020 2020 6461 7461 3a20 6461 7461        data: data
+00000740: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
+00000750: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
+00000760: 2020 7468 726f 7720 6e65 7720 4572 726f    throw new Erro
+00000770: 7228 6077 7261 704f 626a 546f 4a73 6f6e  r(`wrapObjToJson
+00000780: 3a20 556e 6b6e 6f77 6e20 7479 7065 3a20  : Unknown type: 
+00000790: 247b 7479 7065 6f66 206f 626a 7d60 293b  ${typeof obj}`);
+000007a0: 0a20 2020 207d 0a0a 2020 2020 6966 2028  .    }..    if (
+000007b0: 4f62 6a65 6374 5370 6563 6966 6965 722e  ObjectSpecifier.
+000007c0: 6861 7349 6e73 7461 6e63 6528 6f62 6a29  hasInstance(obj)
+000007d0: 2920 7b0a 2020 2020 2020 2020 6c65 7420  ) {.        let 
+000007e0: 636c 6173 734f 6620 3d20 4f62 6a65 6374  classOf = Object
+000007f0: 5370 6563 6966 6965 722e 636c 6173 734f  Specifier.classO
+00000800: 6628 6f62 6a29 3b0a 2020 2020 2020 2020  f(obj);.        
+00000810: 6c65 7420 6576 616c 7561 7465 6420 3d20  let evaluated = 
+00000820: 6f62 6a28 293b 0a20 2020 2020 2020 2069  obj();.        i
+00000830: 6620 2865 7661 6c75 6174 6564 2021 3d3d  f (evaluated !==
+00000840: 2075 6e64 6566 696e 6564 2026 2620 214f   undefined && !O
+00000850: 626a 6563 7453 7065 6369 6669 6572 2e68  bjectSpecifier.h
+00000860: 6173 496e 7374 616e 6365 2865 7661 6c75  asInstance(evalu
+00000870: 6174 6564 2929 207b 0a20 2020 2020 2020  ated)) {.       
+00000880: 2020 2020 2072 6574 7572 6e20 7772 6170       return wrap
+00000890: 4f62 6a54 6f4a 736f 6e28 6576 616c 7561  ObjToJson(evalua
+000008a0: 7465 6429 3b0a 2020 2020 2020 2020 7d0a  ted);.        }.
+000008b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000008c0: 7b0a 2020 2020 2020 2020 2020 2020 7479  {.            ty
+000008d0: 7065 3a20 2772 6566 6572 656e 6365 272c  pe: 'reference',
+000008e0: 0a20 2020 2020 2020 2020 2020 206f 626a  .            obj
+000008f0: 4964 3a20 6361 6368 654f 626a 6374 286f  Id: cacheObjct(o
+00000900: 626a 292c 0a20 2020 2020 2020 2020 2020  bj),.           
+00000910: 2063 6c61 7373 4e61 6d65 3a20 636c 6173   className: clas
+00000920: 734f 660a 2020 2020 2020 2020 7d0a 2020  sOf.        }.  
+00000930: 2020 7d0a 2020 2020 0a20 2020 2074 6872    }.    .    thr
+00000940: 6f77 206e 6577 2045 7272 6f72 2860 556e  ow new Error(`Un
+00000950: 6b6e 6f77 6e20 7479 7065 3a20 247b 7479  known type: ${ty
+00000960: 7065 6f66 206f 626a 7d60 293b 0a7d 0a0a  peof obj}`);.}..
+00000970: 6675 6e63 7469 6f6e 2075 6e77 7261 704f  function unwrapO
+00000980: 626a 4672 6f6d 4a73 6f6e 286f 626a 2920  bjFromJson(obj) 
+00000990: 7b0a 2020 2020 6966 2028 6f62 6a2e 7479  {.    if (obj.ty
+000009a0: 7065 203d 3d3d 2027 7661 6c75 6527 2920  pe === 'value') 
+000009b0: 7b0a 2020 2020 2020 2020 7265 7475 726e  {.        return
+000009c0: 206f 626a 2e64 6174 613b 0a20 2020 207d   obj.data;.    }
+000009d0: 2065 6c73 6520 6966 2028 6f62 6a2e 7479   else if (obj.ty
+000009e0: 7065 203d 3d3d 2027 636f 6e74 6169 6e65  pe === 'containe
+000009f0: 7227 2920 7b0a 2020 2020 2020 2020 666f  r') {.        fo
+00000a00: 7220 286c 6574 206b 2069 6e20 6f62 6a2e  r (let k in obj.
+00000a10: 6461 7461 2920 7b0a 2020 2020 2020 2020  data) {.        
+00000a20: 2020 2020 6f62 6a2e 6461 7461 5b6b 5d20      obj.data[k] 
+00000a30: 3d20 756e 7772 6170 4f62 6a46 726f 6d4a  = unwrapObjFromJ
+00000a40: 736f 6e28 6f62 6a2e 6461 7461 5b6b 5d29  son(obj.data[k])
+00000a50: 3b0a 2020 2020 2020 2020 7d0a 2020 2020  ;.        }.    
+00000a60: 2020 2020 7265 7475 726e 206f 626a 2e64      return obj.d
+00000a70: 6174 613b 0a20 2020 207d 2065 6c73 6520  ata;.    } else 
+00000a80: 6966 2028 6f62 6a2e 7479 7065 203d 3d3d  if (obj.type ===
+00000a90: 2027 7265 6665 7265 6e63 6527 2920 7b0a   'reference') {.
+00000aa0: 2020 2020 2020 2020 7265 7475 726e 2067          return g
+00000ab0: 6574 4361 6368 6564 4f62 6a65 6374 286f  etCachedObject(o
+00000ac0: 626a 2e6f 626a 4964 293b 0a20 2020 207d  bj.objId);.    }
+00000ad0: 0a7d 0a0a 6675 6e63 7469 6f6e 2067 6574  .}..function get
+00000ae0: 4170 706c 6963 6174 696f 6e28 7061 7261  Application(para
+00000af0: 6d73 2920 7b0a 2020 2020 6c65 7420 6e61  ms) {.    let na
+00000b00: 6d65 203d 2070 6172 616d 732e 6e61 6d65  me = params.name
+00000b10: 3b0a 2020 2020 6c65 7420 6170 7020 3d20  ;.    let app = 
+00000b20: 4170 706c 6963 6174 696f 6e28 6e61 6d65  Application(name
+00000b30: 293b 0a20 2020 2061 7070 2e69 6e63 6c75  );.    app.inclu
+00000b40: 6465 5374 616e 6461 7264 4164 6469 7469  deStandardAdditi
+00000b50: 6f6e 7320 3d20 7472 7565 0a20 2020 2072  ons = true.    r
+00000b60: 6574 7572 6e20 7772 6170 4f62 6a54 6f4a  eturn wrapObjToJ
+00000b70: 736f 6e28 6170 7029 3b0a 7d0a 6765 7441  son(app);.}.getA
+00000b80: 7070 6c69 6361 7469 6f6e 203d 206a 736f  pplication = jso
+00000b90: 6e49 4f57 7261 7070 6572 2867 6574 4170  nIOWrapper(getAp
+00000ba0: 706c 6963 6174 696f 6e29 3b0a 0a66 756e  plication);..fun
+00000bb0: 6374 696f 6e20 6765 7450 726f 7065 7274  ction getPropert
+00000bc0: 6965 7328 7061 7261 6d73 2920 7b0a 2020  ies(params) {.  
+00000bd0: 2020 6c65 7420 6f62 6a49 6420 3d20 7061    let objId = pa
+00000be0: 7261 6d73 2e6f 626a 4964 3b0a 2020 2020  rams.objId;.    
+00000bf0: 6c65 7420 6e61 6d65 7320 3d20 7061 7261  let names = para
+00000c00: 6d73 2e6e 616d 6573 3b0a 2020 2020 6c65  ms.names;.    le
+00000c10: 7420 6f62 6a20 3d20 6f62 6a65 6374 4361  t obj = objectCa
+00000c20: 6368 654d 6170 5b6f 626a 4964 5d3b 0a20  cheMap[objId];. 
+00000c30: 2020 206c 6574 2064 6174 6120 3d20 7b7d     let data = {}
+00000c40: 3b0a 2020 2020 666f 7220 286c 6574 206e  ;.    for (let n
+00000c50: 206f 6620 6e61 6d65 7329 207b 0a20 2020   of names) {.   
+00000c60: 2020 2020 206c 6574 2070 726f 7065 7274       let propert
+00000c70: 7920 3d20 6f62 6a5b 6e5d 3b0a 2020 2020  y = obj[n];.    
+00000c80: 2020 2020 6461 7461 5b6e 5d20 3d20 7772      data[n] = wr
+00000c90: 6170 4f62 6a54 6f4a 736f 6e28 7072 6f70  apObjToJson(prop
+00000ca0: 6572 7479 293b 0a20 2020 207d 0a20 2020  erty);.    }.   
+00000cb0: 2072 6574 7572 6e20 6461 7461 3b0a 7d0a   return data;.}.
+00000cc0: 6765 7450 726f 7065 7274 6965 7320 3d20  getProperties = 
+00000cd0: 6a73 6f6e 494f 5772 6170 7065 7228 6765  jsonIOWrapper(ge
+00000ce0: 7450 726f 7065 7274 6965 7329 3b0a 0a0a  tProperties);...
+00000cf0: 6675 6e63 7469 6f6e 2073 6574 5072 6f70  function setProp
+00000d00: 6572 7479 5661 6c75 6573 2870 6172 616d  ertyValues(param
+00000d10: 7329 207b 0a20 2020 206c 6574 206f 626a  s) {.    let obj
+00000d20: 4964 203d 2070 6172 616d 732e 6f62 6a49  Id = params.objI
+00000d30: 643b 0a20 2020 206c 6574 2070 726f 7065  d;.    let prope
+00000d40: 7274 6965 7320 3d20 7061 7261 6d73 2e70  rties = params.p
+00000d50: 726f 7065 7274 6965 733b 0a0a 2020 2020  roperties;..    
+00000d60: 6c65 7420 6f62 6a20 3d20 6f62 6a65 6374  let obj = object
+00000d70: 4361 6368 654d 6170 5b6f 626a 4964 5d3b  CacheMap[objId];
+00000d80: 0a0a 2020 2020 666f 7220 286c 6574 206e  ..    for (let n
+00000d90: 2069 6e20 7072 6f70 6572 7469 6573 2920   in properties) 
+00000da0: 7b0a 2020 2020 2020 2020 6c65 7420 7661  {.        let va
+00000db0: 6c75 6520 3d20 7072 6f70 6572 7469 6573  lue = properties
+00000dc0: 5b6e 5d3b 0a20 2020 2020 2020 206f 626a  [n];.        obj
+00000dd0: 5b6e 5d20 3d20 7661 6c75 653b 0a20 2020  [n] = value;.   
+00000de0: 207d 0a20 2020 2072 6574 7572 6e20 7b7d   }.    return {}
+00000df0: 3b0a 7d0a 7365 7450 726f 7065 7274 7956  ;.}.setPropertyV
+00000e00: 616c 7565 7320 3d20 6a73 6f6e 494f 5772  alues = jsonIOWr
+00000e10: 6170 7065 7228 7365 7450 726f 7065 7274  apper(setPropert
+00000e20: 7956 616c 7565 7329 3b0a 0a66 756e 6374  yValues);..funct
+00000e30: 696f 6e20 7275 6e4d 6574 686f 6428 7061  ion runMethod(pa
+00000e40: 7261 6d73 2920 7b0a 2020 2020 6c65 7420  rams) {.    let 
+00000e50: 6f62 6a49 6420 3d20 7061 7261 6d73 2e6f  objId = params.o
+00000e60: 626a 4964 3b0a 2020 2020 6c65 7420 6e61  bjId;.    let na
+00000e70: 6d65 203d 2070 6172 616d 732e 6e61 6d65  me = params.name
+00000e80: 3b0a 2020 2020 6c65 7420 6172 6773 203d  ;.    let args =
+00000e90: 2070 6172 616d 732e 6172 6773 3b0a 2020   params.args;.  
+00000ea0: 2020 666f 7220 286c 6574 2069 203d 2030    for (let i = 0
+00000eb0: 3b20 6920 3c20 6172 6773 2e6c 656e 6774  ; i < args.lengt
+00000ec0: 683b 2069 2b2b 2920 7b0a 2020 2020 2020  h; i++) {.      
+00000ed0: 2020 6172 6773 5b69 5d20 3d20 756e 7772    args[i] = unwr
+00000ee0: 6170 4f62 6a46 726f 6d4a 736f 6e28 6172  apObjFromJson(ar
+00000ef0: 6773 5b69 5d29 3b0a 2020 2020 7d0a 2020  gs[i]);.    }.  
+00000f00: 2020 6c65 7420 6b77 6172 6773 203d 207b    let kwargs = {
+00000f10: 7d3b 0a20 2020 2066 6f72 2028 6c65 7420  };.    for (let 
+00000f20: 6b20 696e 2070 6172 616d 732e 6b77 6172  k in params.kwar
+00000f30: 6773 2920 7b0a 2020 2020 2020 2020 6b77  gs) {.        kw
+00000f40: 6172 6773 5b6b 5d20 3d20 756e 7772 6170  args[k] = unwrap
+00000f50: 4f62 6a46 726f 6d4a 736f 6e28 7061 7261  ObjFromJson(para
+00000f60: 6d73 2e6b 7761 7267 735b 6b5d 293b 0a20  ms.kwargs[k]);. 
+00000f70: 2020 207d 0a0a 2020 2020 6c65 7420 6f62     }..    let ob
+00000f80: 6a20 3d20 6f62 6a65 6374 4361 6368 654d  j = objectCacheM
+00000f90: 6170 5b6f 626a 4964 5d3b 0a20 2020 206c  ap[objId];.    l
+00000fa0: 6574 2072 6573 756c 7420 3d20 6f62 6a5b  et result = obj[
+00000fb0: 6e61 6d65 5d28 2e2e 2e61 7267 732c 206b  name](...args, k
+00000fc0: 7761 7267 7329 3b0a 2020 2020 7265 7475  wargs);.    retu
+00000fd0: 726e 2077 7261 704f 626a 546f 4a73 6f6e  rn wrapObjToJson
+00000fe0: 2872 6573 756c 7429 3b0a 7d0a 7275 6e4d  (result);.}.runM
+00000ff0: 6574 686f 6420 3d20 6a73 6f6e 494f 5772  ethod = jsonIOWr
+00001000: 6170 7065 7228 7275 6e4d 6574 686f 6429  apper(runMethod)
+00001010: 3b0a 0a0a 6675 6e63 7469 6f6e 2072 656c  ;...function rel
+00001020: 6561 7365 4f62 6a65 6374 2870 6172 616d  easeObject(param
+00001030: 7329 207b 0a20 2020 206c 6574 206f 626a  s) {.    let obj
+00001040: 4964 203d 2070 6172 616d 732e 6f62 6a49  Id = params.objI
+00001050: 643b 0a20 2020 2064 656c 6574 6520 6f62  d;.    delete ob
+00001060: 6a65 6374 4361 6368 654d 6170 5b6f 626a  jectCacheMap[obj
+00001070: 4964 5d3b 0a20 2020 2072 6574 7572 6e20  Id];.    return 
+00001080: 7b7d 3b0a 7d0a 7265 6c65 6173 654f 626a  {};.}.releaseObj
+00001090: 6563 7420 3d20 6a73 6f6e 494f 5772 6170  ect = jsonIOWrap
+000010a0: 7065 7228 7265 6c65 6173 654f 626a 6563  per(releaseObjec
+000010b0: 7429 3b0a 0a66 756e 6374 696f 6e20 6361  t);..function ca
+000010c0: 6c6c 5365 6c66 2870 6172 616d 7329 207b  llSelf(params) {
+000010d0: 0a20 2020 206c 6574 206f 626a 4964 203d  .    let objId =
+000010e0: 2070 6172 616d 732e 6f62 6a49 643b 0a20   params.objId;. 
+000010f0: 2020 206c 6574 2061 7267 7320 3d20 7061     let args = pa
+00001100: 7261 6d73 2e61 7267 733b 0a20 2020 200a  rams.args;.    .
+00001110: 2020 2020 666f 7220 286c 6574 2069 203d      for (let i =
+00001120: 2030 3b20 6920 3c20 6172 6773 2e6c 656e   0; i < args.len
+00001130: 6774 683b 2069 2b2b 2920 7b0a 2020 2020  gth; i++) {.    
+00001140: 2020 2020 6172 6773 5b69 5d20 3d20 756e      args[i] = un
+00001150: 7772 6170 4f62 6a46 726f 6d4a 736f 6e28  wrapObjFromJson(
+00001160: 6172 6773 5b69 5d29 3b0a 2020 2020 7d0a  args[i]);.    }.
+00001170: 2020 2020 6c65 7420 6b77 6172 6773 203d      let kwargs =
+00001180: 207b 7d3b 0a20 2020 2066 6f72 2028 6c65   {};.    for (le
+00001190: 7420 6b20 696e 2070 6172 616d 732e 6b77  t k in params.kw
+000011a0: 6172 6773 2920 7b0a 2020 2020 2020 2020  args) {.        
+000011b0: 6b77 6172 6773 5b6b 5d20 3d20 756e 7772  kwargs[k] = unwr
+000011c0: 6170 4f62 6a46 726f 6d4a 736f 6e28 7061  apObjFromJson(pa
+000011d0: 7261 6d73 2e6b 7761 7267 735b 6b5d 293b  rams.kwargs[k]);
+000011e0: 0a20 2020 207d 0a20 2020 206c 6574 206f  .    }.    let o
+000011f0: 626a 203d 206f 626a 6563 7443 6163 6865  bj = objectCache
+00001200: 4d61 705b 6f62 6a49 645d 3b0a 2020 2020  Map[objId];.    
+00001210: 6c65 7420 7265 7375 6c74 203d 206f 626a  let result = obj
+00001220: 282e 2e2e 6172 6773 2c20 6b77 6172 6773  (...args, kwargs
+00001230: 293b 0a20 2020 2072 6574 7572 6e20 7772  );.    return wr
+00001240: 6170 4f62 6a54 6f4a 736f 6e28 7265 7375  apObjToJson(resu
+00001250: 6c74 293b 0a7d 0a63 616c 6c53 656c 6620  lt);.}.callSelf 
+00001260: 3d20 6a73 6f6e 494f 5772 6170 7065 7228  = jsonIOWrapper(
+00001270: 6361 6c6c 5365 6c66 293b 0008 000b 0012  callSelf);......
+00001280: 0000 0000 0000 0201 0000 0000 0000 0003  ................
+00001290: 0000 0000 0000 0000 0000 0000 0000 126a  ...............j
+000012a0: 6a73 6372 0001 000c fade dead            jscr........
```

### Comparing `pydt3-0.0.1/pydt3/models/database.py` & `pydt3-0.0.2/pydt3/models/database.py`

 * *Files identical despite different names*

### Comparing `pydt3-0.0.1/pydt3/models/record.py` & `pydt3-0.0.2/pydt3/models/record.py`

 * *Files identical despite different names*

### Comparing `pydt3-0.0.1/pydt3/models/reminder.py` & `pydt3-0.0.2/pydt3/models/reminder.py`

 * *Files identical despite different names*

### Comparing `pydt3-0.0.1/pydt3/models/smartgroup.py` & `pydt3-0.0.2/pydt3/models/smartgroup.py`

 * *Files identical despite different names*

### Comparing `pydt3-0.0.1/pydt3/models/text.py` & `pydt3-0.0.2/pydt3/models/text.py`

 * *Files identical despite different names*

### Comparing `pydt3-0.0.1/pydt3/models/windows.py` & `pydt3-0.0.2/pydt3/models/windows.py`

 * *Files identical despite different names*

### Comparing `pydt3-0.0.1/pydt3/osascript.py` & `pydt3-0.0.2/pydt3/osascript.py`

 * *Files identical despite different names*

### Comparing `pydt3-0.0.1/pydt3.egg-info/PKG-INFO` & `pydt3-0.0.2/pydt3.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pydt3
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python API for Devonthink 3 utilizes AppleScript (JXA) and PyObjC.
 Author-email: astrosheep <astrosheepthesheep@outlook.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # PyDT3 - The Python API For DEVONthink 3
 
-This Python API for Devonthink 3 utilizes AppleScript (JXA) and PyObjC.
+The Python API for Devonthink 3 utilizes AppleScript (JXA) and PyObjC.
 
 Most of the APIs are directly mapped to AppleScript (JXA).
 For example, these two are equivalent:
 
 ```python
 from pydt3 import DEVONthink3
 dt3 = DEVONthink3()
@@ -44,18 +44,18 @@
 
 ## Quick Start
 
 ```python
 from pydt3 import DEVONthink3
 dtp3 = DEVONthink3()
 
-inbox = dtp3.ext.inbox
+inbox = dtp3.inbox
 
 # create a new folder in inbox
-dtp3.create_location('hello-from-pydt3', inbox)
+dtp3.create_location('new-group-from-pydt3', inbox)
 
 # get selected records
 records = dtp3.selected_records
 
 # get the first selected record and print its information
 if records:
     first = records[0]
@@ -70,15 +70,15 @@
     'type': 'markdown',
     'plain text': '# Hello from pydt3',
 }, inbox)
 ```
 
 ## Documentation
 
-Unlike many other API wrapper projects, PyDT3 is well documented thanks to the detailed AppleScript dictionary by DEVONthink team and code generation ability of ChatGTP.
+Unlike many other API wrapper projects, PyDT3 is well documented thanks to the detailed AppleScript dictionary by DEVONthink team and the code generation ability of ChatGTP.
 
 You can check the documentation either in source code (`docstring`), code editor (if properly configured), or the documentation site (not available at the time).
 
 ![documentation-in-editor](images/create_record_with_doc.png)
 
 ## Requirements
```

### Comparing `pydt3-0.0.1/pyproject.toml` & `pydt3-0.0.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "pydt3"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="astrosheep", email="astrosheepthesheep@outlook.com" },
 ]
 description = "Python API for Devonthink 3 utilizes AppleScript (JXA) and PyObjC."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = ["pyobjc-core", "pyobjc-framework-AppleScriptKit", "pyobjc-framework-AppleScriptObjC"]
```

