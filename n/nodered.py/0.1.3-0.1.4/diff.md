# Comparing `tmp/nodered.py-0.1.3.tar.gz` & `tmp/nodered.py-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodered.py-0.1.3.tar", last modified: Mon May  1 13:26:39 2023, max compression
+gzip compressed data, was "nodered.py-0.1.4.tar", last modified: Tue May  2 11:31:07 2023, max compression
```

## Comparing `nodered.py-0.1.3.tar` & `nodered.py-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-01 13:26:39.570000 nodered.py-0.1.3/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1065 2023-04-28 05:27:55.000000 nodered.py-0.1.3/LICENSE
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2074 2023-05-01 13:26:39.670000 nodered.py-0.1.3/PKG-INFO
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1758 2023-04-30 04:58:00.000000 nodered.py-0.1.3/README.md
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-01 13:26:39.570000 nodered.py-0.1.3/nodered.py.egg-info/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2074 2023-05-01 13:26:39.000000 nodered.py-0.1.3/nodered.py.egg-info/PKG-INFO
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      543 2023-05-01 13:26:39.000000 nodered.py-0.1.3/nodered.py.egg-info/SOURCES.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-05-01 13:26:39.000000 nodered.py-0.1.3/nodered.py.egg-info/dependency_links.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      163 2023-05-01 13:26:39.000000 nodered.py-0.1.3/nodered.py.egg-info/requires.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       57 2023-05-01 13:26:39.000000 nodered.py-0.1.3/nodered.py.egg-info/top_level.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-04-28 03:54:24.000000 nodered.py-0.1.3/nodered.py.egg-info/zip-safe
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-01 13:26:39.570000 nodered.py-0.1.3/noderedpy/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      466 2023-05-01 12:55:57.000000 nodered.py-0.1.3/noderedpy/__init__.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     5580 2023-05-01 13:06:41.000000 nodered.py-0.1.3/noderedpy/_nodered.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     3457 2023-05-01 13:22:01.000000 nodered.py-0.1.3/noderedpy/_property.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     6410 2023-04-30 03:53:02.000000 nodered.py-0.1.3/noderedpy/_server.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      805 2023-04-30 03:52:23.000000 nodered.py-0.1.3/noderedpy/decorator.py
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-01 13:26:39.570000 nodered.py-0.1.3/noderedpy/node-red-starter/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2398 2023-04-29 01:58:51.000000 nodered.py-0.1.3/noderedpy/node-red-starter/index.js
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      296 2023-04-27 11:00:04.000000 nodered.py-0.1.3/noderedpy/node-red-starter/package.json
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-01 13:26:39.570000 nodered.py-0.1.3/noderedpy/templates/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     7123 2023-05-01 13:22:31.000000 nodered.py-0.1.3/noderedpy/templates/__init__.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      971 2023-05-01 13:00:37.000000 nodered.py-0.1.3/noderedpy/templates/template.html
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     3212 2023-05-01 13:01:59.000000 nodered.py-0.1.3/noderedpy/templates/template.js
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      269 2023-05-01 13:03:04.000000 nodered.py-0.1.3/noderedpy/templates/template.json
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       38 2023-05-01 13:26:39.670000 nodered.py-0.1.3/setup.cfg
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1077 2023-05-01 12:49:35.000000 nodered.py-0.1.3/setup.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-02 11:31:07.310000 nodered.py-0.1.4/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1065 2023-04-28 05:27:55.000000 nodered.py-0.1.4/LICENSE
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2074 2023-05-02 11:31:07.400000 nodered.py-0.1.4/PKG-INFO
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1758 2023-04-30 04:58:00.000000 nodered.py-0.1.4/README.md
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-02 11:31:07.310000 nodered.py-0.1.4/nodered.py.egg-info/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2074 2023-05-02 11:31:07.000000 nodered.py-0.1.4/nodered.py.egg-info/PKG-INFO
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      543 2023-05-02 11:31:07.000000 nodered.py-0.1.4/nodered.py.egg-info/SOURCES.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-05-02 11:31:07.000000 nodered.py-0.1.4/nodered.py.egg-info/dependency_links.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      163 2023-05-02 11:31:07.000000 nodered.py-0.1.4/nodered.py.egg-info/requires.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       57 2023-05-02 11:31:07.000000 nodered.py-0.1.4/nodered.py.egg-info/top_level.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-04-28 03:54:24.000000 nodered.py-0.1.4/nodered.py.egg-info/zip-safe
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-02 11:31:07.310000 nodered.py-0.1.4/noderedpy/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      496 2023-05-02 10:41:48.000000 nodered.py-0.1.4/noderedpy/__init__.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     5580 2023-05-01 13:06:41.000000 nodered.py-0.1.4/noderedpy/_nodered.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     4006 2023-05-02 10:42:51.000000 nodered.py-0.1.4/noderedpy/_property.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     6410 2023-04-30 03:53:02.000000 nodered.py-0.1.4/noderedpy/_server.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      805 2023-04-30 03:52:23.000000 nodered.py-0.1.4/noderedpy/decorator.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-02 11:31:07.320000 nodered.py-0.1.4/noderedpy/node-red-starter/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2398 2023-04-29 01:58:51.000000 nodered.py-0.1.4/noderedpy/node-red-starter/index.js
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      296 2023-04-27 11:00:04.000000 nodered.py-0.1.4/noderedpy/node-red-starter/package.json
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-05-02 11:31:07.320000 nodered.py-0.1.4/noderedpy/templates/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     7470 2023-05-02 10:45:53.000000 nodered.py-0.1.4/noderedpy/templates/__init__.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      971 2023-05-01 13:00:37.000000 nodered.py-0.1.4/noderedpy/templates/template.html
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     3212 2023-05-01 13:01:59.000000 nodered.py-0.1.4/noderedpy/templates/template.js
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      269 2023-05-01 13:03:04.000000 nodered.py-0.1.4/noderedpy/templates/template.json
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       38 2023-05-02 11:31:07.400000 nodered.py-0.1.4/setup.cfg
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1077 2023-05-01 12:49:35.000000 nodered.py-0.1.4/setup.py
```

### Comparing `nodered.py-0.1.3/LICENSE` & `nodered.py-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nodered.py-0.1.3/PKG-INFO` & `nodered.py-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodered.py
-Version: 0.1.3
+Version: 0.1.4
 Summary: make python function to Node-RED node
 Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev
 Author-email: this.dev.somehit@gmail.com
 License: MIT license
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nodered.py Version: 0.1.3 Summary: make python
+Metadata-Version: 2.1 Name: nodered.py Version: 0.1.4 Summary: make python
 function to Node-RED node Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev Author-email: this.dev.somehit@gmail.com License: MIT license
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE
                            ****** NodeRED.py ******
                      make python function to Node-RED node
```

### Comparing `nodered.py-0.1.3/README.md` & `nodered.py-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `nodered.py-0.1.3/nodered.py.egg-info/PKG-INFO` & `nodered.py-0.1.4/nodered.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodered.py
-Version: 0.1.3
+Version: 0.1.4
 Summary: make python function to Node-RED node
 Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev
 Author-email: this.dev.somehit@gmail.com
 License: MIT license
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nodered.py Version: 0.1.3 Summary: make python
+Metadata-Version: 2.1 Name: nodered.py Version: 0.1.4 Summary: make python
 function to Node-RED node Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev Author-email: this.dev.somehit@gmail.com License: MIT license
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE
                            ****** NodeRED.py ******
                      make python function to Node-RED node
```

### Comparing `nodered.py-0.1.3/nodered.py.egg-info/SOURCES.txt` & `nodered.py-0.1.4/nodered.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nodered.py-0.1.3/noderedpy/_nodered.py` & `nodered.py-0.1.4/noderedpy/_nodered.py`

 * *Files identical despite different names*

### Comparing `nodered.py-0.1.3/noderedpy/_property.py` & `nodered.py-0.1.4/noderedpy/_property.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,14 +12,23 @@
     @property
     def display_name(self) -> str:
         return " ".join([
             item.capitalize()
             for item in self.name.split("_")
         ])
 
+class CodeProperty(Property):
+    def __init__(self, name:str, default:str = "", language:str = None, height:int = 250, required:bool = False, display_icon:str = None):
+        if not isinstance(default, str):
+            raise TypeError("CodeProperty can accept types: [ 'dict', 'json string' ]")
+        
+        super().__init__(name, default, required, display_icon if display_icon else "fa fa-code")
+        self.language, self.height =\
+            language, height
+
 class InputProperty(Property):
     def __init__(self, name:str, default:Union[int, float, str] = None, required:bool = False, display_icon:str = None):
         if not isinstance(default, (int, float, str)):
             raise TypeError("InputProperty can accept types: [ 'int', 'float', 'str' ]")
         
         if default is None:
             if isinstance(default, int):
@@ -43,30 +52,32 @@
     def __init__(self, name:str, default:list = [], height:int = 250, required:bool = False, display_icon:str = None):
         if not isinstance(default, list):
             raise TypeError("ListProperty can accept type: 'list'")
 
         super().__init__(name, default, required, display_icon if display_icon else "fa fa-list-ul")
         self.height = height
 
-class DictProperty(Property):
+class DictProperty(CodeProperty):
     def __init__(self, name:str, default:Union[dict, str] = {}, height:int = 250, required:bool = False, display_icon:str = None):
         if not isinstance(default, ( dict, str )):
             raise TypeError("DictProperty can accept types: [ 'dict', 'json string' ]")
         
         if isinstance(default, str):
             if not default.strip().startswith("{") or not default.strip().endswith("}"):
                 raise ValueError("DictProperty value must be 'dict' or 'json string'!")
 
             try:
                 json.loads(default)
             except:
                 raise ValueError("DictProperty value must be 'dict' or 'json string'!")
-        
-        super().__init__(name, default, required, display_icon if display_icon else "fa fa-code")
-        self.height = height
+
+        if isinstance(default, dict):
+            default = json.dumps(default, indent = 4)
+
+        super().__init__(name, default, "json", height, required, display_icon if display_icon else "fa fa-code")
 
 class SpinnerProperty(Property):
     def __init__(self, name:str, default:float = 0, step:float = None, min:float = None, max:float = None, required:bool = False, display_icon:str = None):
         if not isinstance(default, (int, float)):
             raise TypeError("SpinnerProperty can accept types: [ 'int', 'float' ]")
 
         super().__init__(name, default, required, display_icon if display_icon else "fa fa-random")
```

### Comparing `nodered.py-0.1.3/noderedpy/_server.py` & `nodered.py-0.1.4/noderedpy/_server.py`

 * *Files identical despite different names*

### Comparing `nodered.py-0.1.3/noderedpy/decorator.py` & `nodered.py-0.1.4/noderedpy/decorator.py`

 * *Files identical despite different names*

### Comparing `nodered.py-0.1.3/noderedpy/node-red-starter/index.js` & `nodered.py-0.1.4/noderedpy/node-red-starter/index.js`

 * *Files identical despite different names*

### Comparing `nodered.py-0.1.3/noderedpy/templates/__init__.py` & `nodered.py-0.1.4/noderedpy/templates/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 import os, json, noderedpy
 from .._property import (
-    InputProperty, ListProperty, DictProperty,
-    SpinnerProperty, ComboBoxProperty
+    InputProperty, ListProperty,
+    SpinnerProperty, ComboBoxProperty, CodeProperty
 )
 from . import __path__
 
 
 def package_json(node:"noderedpy._nodered.Node") -> str:
     with open(os.path.join(__path__[0], "template.json"), "r", encoding = "utf-8") as tr:
         tt = tr.read()
@@ -57,41 +57,50 @@
             properties_js_save.append('''
             this.''' + property.name + ''' = [];
             $("#node-input-''' + property.name + '''-container").editableList("items").each((_, item) => {
                 this.''' + property.name + '''.push(item.find("input.input-list-item").val());
             });
 ''')
             default_value = str(property.default)
-        elif isinstance(property, DictProperty):
+        elif isinstance(property, CodeProperty):
             properties_html.append(f"""
     <div class="form-row" style="margin-bottom:0px;">
         <label><i class="{property.display_icon}"></i> <span>{property.display_name}</span></label>
     </div>
     <div class="form-row node-text-editor-row">
         <div style="height:{property.height}px;" class="node-text-editor" id="node-input-{property.name}"></div>
     </div>
 """)
-            properties_js_prepare.append('''
+            if property.language:
+                properties_js_prepare.append('''
+            this.''' + property.name + '''Editor = RED.editor.createEditor({
+                id: "node-input-''' + property.name + '''",
+                mode: "ace/mode/''' + property.language + '''",
+                value: this.''' + property.name + ''',
+                focus: true
+            });
+''')
+            else:
+                properties_js_prepare.append('''
             this.''' + property.name + '''Editor = RED.editor.createEditor({
                 id: "node-input-''' + property.name + '''",
-                mode: "ace/mode/json",
                 value: this.''' + property.name + ''',
                 focus: true
             });
 ''')
             properties_js_cancel.append(f"""
             this.{property.name}Editor.destroy();
             delete this.{property.name}Editor;
 """)
             properties_js_save.append(f"""
             $("#node-input-{property.name}").val(this.{property.name}Editor.getValue().trim());
             this.{property.name}Editor.destroy();
             delete this.{property.name}Editor;
 """)
-            default_value = f"`{json.dumps(property.default, indent = 4)}`"
+            default_value = f"`{property.default}`"
         elif isinstance(property, SpinnerProperty):
             properties_html.append(f"""
     <div class="form-row" style="margin-bottom:0px;">
         <label><i class="{property.display_icon}"></i> <span>{property.display_name}</span></label>
     </div>
     <div class="form-row">
         <input type="text" id="node-input-{property.name}" style="width:calc(100% - 22px);">
```

### Comparing `nodered.py-0.1.3/noderedpy/templates/template.html` & `nodered.py-0.1.4/noderedpy/templates/template.html`

 * *Files identical despite different names*

### Comparing `nodered.py-0.1.3/noderedpy/templates/template.js` & `nodered.py-0.1.4/noderedpy/templates/template.js`

 * *Files identical despite different names*

### Comparing `nodered.py-0.1.3/setup.py` & `nodered.py-0.1.4/setup.py`

 * *Files identical despite different names*

