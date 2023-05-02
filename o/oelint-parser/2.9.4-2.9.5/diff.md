# Comparing `tmp/oelint_parser-2.9.4.tar.gz` & `tmp/oelint_parser-2.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oelint_parser-2.9.4.tar", last modified: Thu Dec  1 13:51:05 2022, max compression
+gzip compressed data, was "oelint_parser-2.9.5.tar", last modified: Mon Dec  5 09:12:39 2022, max compression
```

## Comparing `oelint_parser-2.9.4.tar` & `oelint_parser-2.9.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 13:51:05.089592 oelint_parser-2.9.4/
--rw-r--r--   0 runner    (1001) docker     (122)     1325 2022-12-01 13:50:38.000000 oelint_parser-2.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       59 2022-12-01 13:50:38.000000 oelint_parser-2.9.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7163 2022-12-01 13:51:05.089592 oelint_parser-2.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5374 2022-12-01 13:50:38.000000 oelint_parser-2.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 13:51:05.085592 oelint_parser-2.9.4/oelint_parser/
--rw-r--r--   0 runner    (1001) docker     (122)       81 2022-12-01 13:50:38.000000 oelint_parser-2.9.4/oelint_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    27064 2022-12-01 13:50:38.000000 oelint_parser-2.9.4/oelint_parser/cls_item.py
--rw-r--r--   0 runner    (1001) docker     (122)    10905 2022-12-01 13:50:38.000000 oelint_parser-2.9.4/oelint_parser/cls_stash.py
--rw-r--r--   0 runner    (1001) docker     (122)      360 2022-12-01 13:50:38.000000 oelint_parser-2.9.4/oelint_parser/const_func.py
--rw-r--r--   0 runner    (1001) docker     (122)     2517 2022-12-01 13:50:38.000000 oelint_parser-2.9.4/oelint_parser/const_vars.py
--rw-r--r--   0 runner    (1001) docker     (122)     6674 2022-12-01 13:50:38.000000 oelint_parser-2.9.4/oelint_parser/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 13:51:05.085592 oelint_parser-2.9.4/oelint_parser/data/
--rw-r--r--   0 runner    (1001) docker     (122)    45045 2022-12-01 13:50:38.000000 oelint_parser-2.9.4/oelint_parser/data/const-default.json
--rw-r--r--   0 runner    (1001) docker     (122)     9772 2022-12-01 13:50:38.000000 oelint_parser-2.9.4/oelint_parser/helper_files.py
--rw-r--r--   0 runner    (1001) docker     (122)     1167 2022-12-01 13:50:38.000000 oelint_parser-2.9.4/oelint_parser/inlinerep.py
--rw-r--r--   0 runner    (1001) docker     (122)    12044 2022-12-01 13:50:38.000000 oelint_parser-2.9.4/oelint_parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     3361 2022-12-01 13:50:38.000000 oelint_parser-2.9.4/oelint_parser/rpl_regex.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 13:51:05.085592 oelint_parser-2.9.4/oelint_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7163 2022-12-01 13:51:05.000000 oelint_parser-2.9.4/oelint_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      557 2022-12-01 13:51:05.000000 oelint_parser-2.9.4/oelint_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-01 13:51:05.000000 oelint_parser-2.9.4/oelint_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       30 2022-12-01 13:51:05.000000 oelint_parser-2.9.4/oelint_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2022-12-01 13:51:05.000000 oelint_parser-2.9.4/oelint_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       34 2022-12-01 13:50:38.000000 oelint_parser-2.9.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      461 2022-12-01 13:51:05.089592 oelint_parser-2.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1351 2022-12-01 13:51:04.000000 oelint_parser-2.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 09:12:39.699755 oelint_parser-2.9.5/
+-rw-r--r--   0 runner    (1001) docker     (122)     1325 2022-12-05 09:12:17.000000 oelint_parser-2.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2022-12-05 09:12:17.000000 oelint_parser-2.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7163 2022-12-05 09:12:39.699755 oelint_parser-2.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5374 2022-12-05 09:12:17.000000 oelint_parser-2.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 09:12:39.699755 oelint_parser-2.9.5/oelint_parser/
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2022-12-05 09:12:17.000000 oelint_parser-2.9.5/oelint_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27240 2022-12-05 09:12:17.000000 oelint_parser-2.9.5/oelint_parser/cls_item.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10905 2022-12-05 09:12:17.000000 oelint_parser-2.9.5/oelint_parser/cls_stash.py
+-rw-r--r--   0 runner    (1001) docker     (122)      360 2022-12-05 09:12:17.000000 oelint_parser-2.9.5/oelint_parser/const_func.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2517 2022-12-05 09:12:17.000000 oelint_parser-2.9.5/oelint_parser/const_vars.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6674 2022-12-05 09:12:17.000000 oelint_parser-2.9.5/oelint_parser/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 09:12:39.699755 oelint_parser-2.9.5/oelint_parser/data/
+-rw-r--r--   0 runner    (1001) docker     (122)    45045 2022-12-05 09:12:17.000000 oelint_parser-2.9.5/oelint_parser/data/const-default.json
+-rw-r--r--   0 runner    (1001) docker     (122)     9772 2022-12-05 09:12:17.000000 oelint_parser-2.9.5/oelint_parser/helper_files.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1167 2022-12-05 09:12:17.000000 oelint_parser-2.9.5/oelint_parser/inlinerep.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12044 2022-12-05 09:12:17.000000 oelint_parser-2.9.5/oelint_parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3361 2022-12-05 09:12:17.000000 oelint_parser-2.9.5/oelint_parser/rpl_regex.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 09:12:39.699755 oelint_parser-2.9.5/oelint_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7163 2022-12-05 09:12:39.000000 oelint_parser-2.9.5/oelint_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      557 2022-12-05 09:12:39.000000 oelint_parser-2.9.5/oelint_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-05 09:12:39.000000 oelint_parser-2.9.5/oelint_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2022-12-05 09:12:39.000000 oelint_parser-2.9.5/oelint_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2022-12-05 09:12:39.000000 oelint_parser-2.9.5/oelint_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2022-12-05 09:12:17.000000 oelint_parser-2.9.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      461 2022-12-05 09:12:39.699755 oelint_parser-2.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1351 2022-12-05 09:12:39.000000 oelint_parser-2.9.5/setup.py
```

### Comparing `oelint_parser-2.9.4/LICENSE` & `oelint_parser-2.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `oelint_parser-2.9.4/PKG-INFO` & `oelint_parser-2.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oelint_parser
-Version: 2.9.4
+Version: 2.9.5
 Summary: Alternative parser for bitbake recipes
 Home-page: https://github.com/priv-kweihmann/oelint-parser
 Author: Konrad Weihmann
 Author-email: kweihmann@outlook.com
 License: UNKNOWN
 Description: # oelint-parser
```

### Comparing `oelint_parser-2.9.4/README.md` & `oelint_parser-2.9.5/README.md`

 * *Files identical despite different names*

### Comparing `oelint_parser-2.9.4/oelint_parser/cls_item.py` & `oelint_parser-2.9.5/oelint_parser/cls_item.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         self.__Line = line
         self.__Raw = rawtext
         self.__Links = []
         self.__Origin = origin
         self.__InFileLine = infileline
         self.__IncludedFrom = []
         self.__RealRaw = realraw or rawtext
-        self._override_delimiter = "_"
+        self.__OverrideDelimiter = "_"
 
     @property
     def Line(self):
         """Overall line count
 
         Returns:
             int: overall line count of item
@@ -121,14 +121,23 @@
         """Item comes from a bbclass
 
         Returns:
             bool: if item was set in a bbclass
         """
         return self.__Origin.endswith(".bbclass")
 
+    @property
+    def OverrideDelimiter(self):
+        """Override delimiter
+
+        Returns:
+            str: Override delimiter
+        """
+        return self.__OverrideDelimiter
+
     @staticmethod
     def safe_linesplit(string):
         """Safely split an input line to chunks
 
         Args:
             string (str): raw input string
 
@@ -154,16 +163,16 @@
         Arguments:
             name {str} -- input string
 
         Returns:
             tuple -- clean variable name, modifiers, package specific modifiers
         """
         if ":" in name:
-            self._override_delimiter = ":"
-        chunks = name.split(self._override_delimiter)
+            self.__OverrideDelimiter = ":"
+        chunks = name.split(self.__OverrideDelimiter)
         _suffix = []
         _var = [chunks[0]]
         for i in chunks[1:]:
             tmp = ""
             if "-" in i:
                 # just use the prefix in case a dash is found
                 # that addresses things like FILES_${PN}-dev
@@ -173,41 +182,41 @@
                 _suffix.append(i + tmp)
             elif i in ["${PN}"]:
                 _suffix.append(i + tmp)
             else:
                 _var.append(i + tmp)
         _var = [x for x in _var if x]
         _suffix = [x for x in _suffix if x]
-        return (self._override_delimiter.join(_var), self._override_delimiter.join(_suffix))
+        return (self.__OverrideDelimiter.join(_var), self.__OverrideDelimiter.join(_suffix))
 
     def extract_sub_func(self, name):
         """Extract modifiers for functions
 
         Arguments:
             name {str} -- input value
 
         Returns:
             tuple -- clean function name, modifiers
         """
         if ":" in name:
-            self._override_delimiter = ":"
-        chunks = name.split(self._override_delimiter)
+            self.__OverrideDelimiter = ":"
+        chunks = name.split(self.__OverrideDelimiter)
         _marker = ["append", "prepend", "class-native",
                    "class-cross", "class-target", "remove"]
         _suffix = []
         _var = [chunks[0]]
         for i in chunks[1:]:
-            if i in _marker or self._override_delimiter.join(_var) in CONSTANTS.FunctionsKnown:
+            if i in _marker or self.__OverrideDelimiter.join(_var) in CONSTANTS.FunctionsKnown:
                 _suffix = chunks[chunks.index(i):]
                 break
             else:
                 _var.append(i)
         _var = [x for x in _var if x]
         _suffix = [x for x in _suffix if x]
-        return (self._override_delimiter.join(_var), self._override_delimiter.join(_suffix))
+        return (self.__OverrideDelimiter.join(_var), self.__OverrideDelimiter.join(_suffix))
 
     def IsFromAppend(self):
         """Item originates from a bbappend
 
         Returns:
             bool -- True if coming from a bbappend
         """
@@ -274,15 +283,15 @@
         if "inherit" != name and not flag:
             self.__VarName, self.__SubItem = self.extract_sub(
                 name)
         else:
             self.__VarName = name
             self.__SubItem = ""
         self.__SubItems = [x for x in self.SubItem.split(
-            self._override_delimiter) if x]
+            self.OverrideDelimiter) if x]
         self.__VarValue = value
         self.__VarOp = operator
         self.__Flag = flag or ""
         self.__RawVarName = "{name}[{flag}]".format(
             name=self.VarName, flag=self.Flag) if self.Flag else self.VarName
         self.__VarValueStripped = self.VarValue.strip().lstrip('"').rstrip('"')
 
@@ -347,15 +356,15 @@
     @property
     def VarNameComplete(self):
         """Complete variable name included overrides and flags
 
         Returns:
             str: complete variable name
         """
-        _var = self._override_delimiter.join([self.VarName] + self.SubItems)
+        _var = self.OverrideDelimiter.join([self.VarName] + self.SubItems)
         return "{name}[{flag}]".format(name=_var, flag=self.Flag) if self.Flag else _var
 
     @property
     def RawVarName(self):
         """Variable name and flags combined
 
         Returns:
@@ -595,15 +604,15 @@
         """
         super().__init__(origin, line, infileline, rawtext, realraw)
         self.__IsPython = python is not None
         self.__IsFakeroot = fakeroot is not None
         name = name or ""
         self.__FuncName, self.__SubItem = self.extract_sub_func(name.strip())
         self.__SubItems = [x for x in self.SubItem.split(
-            self._override_delimiter) if x]
+            self.OverrideDelimiter) if x]
         self.__FuncBody = body
         self.__FuncBodyStripped = body.replace(
             "{", "").replace("}", "").replace("\n", "").strip()
         self.__FuncBodyRaw = textwrap.dedent(
             rawtext[rawtext.find("{") + 1:].rstrip().rstrip("}"))
 
     @property
@@ -636,15 +645,15 @@
     @property
     def FuncNameComplete(self):
         """Complete function name (including overrides)
 
         Returns:
             str: complete name of function
         """
-        return self._override_delimiter.join([self.__FuncName] + self.__SubItems)
+        return self.OverrideDelimiter.join([self.__FuncName] + self.__SubItems)
 
     @property
     def SubItem(self):
         """Function modifiers
 
         Returns:
             str: function modifiers like packages, machines, appends, prepends
```

### Comparing `oelint_parser-2.9.4/oelint_parser/cls_stash.py` & `oelint_parser-2.9.5/oelint_parser/cls_stash.py`

 * *Files identical despite different names*

### Comparing `oelint_parser-2.9.4/oelint_parser/const_vars.py` & `oelint_parser-2.9.5/oelint_parser/const_vars.py`

 * *Files identical despite different names*

### Comparing `oelint_parser-2.9.4/oelint_parser/constants.py` & `oelint_parser-2.9.5/oelint_parser/constants.py`

 * *Files identical despite different names*

### Comparing `oelint_parser-2.9.4/oelint_parser/data/const-default.json` & `oelint_parser-2.9.5/oelint_parser/data/const-default.json`

 * *Files identical despite different names*

### Comparing `oelint_parser-2.9.4/oelint_parser/helper_files.py` & `oelint_parser-2.9.5/oelint_parser/helper_files.py`

 * *Files identical despite different names*

### Comparing `oelint_parser-2.9.4/oelint_parser/inlinerep.py` & `oelint_parser-2.9.5/oelint_parser/inlinerep.py`

 * *Files identical despite different names*

### Comparing `oelint_parser-2.9.4/oelint_parser/parser.py` & `oelint_parser-2.9.5/oelint_parser/parser.py`

 * *Files identical despite different names*

### Comparing `oelint_parser-2.9.4/oelint_parser/rpl_regex.py` & `oelint_parser-2.9.5/oelint_parser/rpl_regex.py`

 * *Files identical despite different names*

### Comparing `oelint_parser-2.9.4/oelint_parser.egg-info/PKG-INFO` & `oelint_parser-2.9.5/oelint_parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oelint-parser
-Version: 2.9.4
+Version: 2.9.5
 Summary: Alternative parser for bitbake recipes
 Home-page: https://github.com/priv-kweihmann/oelint-parser
 Author: Konrad Weihmann
 Author-email: kweihmann@outlook.com
 License: UNKNOWN
 Description: # oelint-parser
```

### Comparing `oelint_parser-2.9.4/oelint_parser.egg-info/SOURCES.txt` & `oelint_parser-2.9.5/oelint_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oelint_parser-2.9.4/setup.py` & `oelint_parser-2.9.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 requirements = []
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name='oelint_parser',
-    version='2.9.4',
+    version='2.9.5',
     author='Konrad Weihmann',
     author_email='kweihmann@outlook.com',
     description='Alternative parser for bitbake recipes',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/priv-kweihmann/oelint-parser',
     packages=setuptools.find_packages(),
```

