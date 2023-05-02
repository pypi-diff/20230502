# Comparing `tmp/unisci-1.4.4.tar.gz` & `tmp/unisci-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unisci-1.4.4.tar", last modified: Tue May  2 02:21:07 2023, max compression
+gzip compressed data, was "unisci-1.4.5.tar", last modified: Tue May  2 02:27:52 2023, max compression
```

## Comparing `unisci-1.4.4.tar` & `unisci-1.4.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-02 02:21:07.938977 unisci-1.4.4/
--rw-r--r--   0 vivaan     (501) staff       (20)     1071 2023-04-17 11:50:57.000000 unisci-1.4.4/LICENSE
--rw-r--r--   0 vivaan     (501) staff       (20)      188 2023-04-27 04:25:20.000000 unisci-1.4.4/MANIFEST.in
--rw-r--r--   0 vivaan     (501) staff       (20)     1614 2023-05-02 02:21:07.938662 unisci-1.4.4/PKG-INFO
--rw-r--r--   0 vivaan     (501) staff       (20)     1286 2023-04-28 05:01:19.000000 unisci-1.4.4/README.md
--rw-r--r--   0 vivaan     (501) staff       (20)       38 2023-05-02 02:21:07.939069 unisci-1.4.4/setup.cfg
--rw-r--r--   0 vivaan     (501) staff       (20)      679 2023-05-01 22:47:51.000000 unisci-1.4.4/setup.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-02 02:21:07.932860 unisci-1.4.4/unisci/
--rw-r--r--   0 vivaan     (501) staff       (20)       87 2023-05-01 22:47:55.000000 unisci-1.4.4/unisci/__init__.py
--rw-r--r--   0 vivaan     (501) staff       (20)     1503 2023-05-01 22:47:16.000000 unisci-1.4.4/unisci/_conversion_factors.py
--rw-r--r--   0 vivaan     (501) staff       (20)      607 2023-04-23 05:14:17.000000 unisci-1.4.4/unisci/_error.py
--rw-r--r--   0 vivaan     (501) staff       (20)      386 2023-04-26 16:06:26.000000 unisci-1.4.4/unisci/constants.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-02 02:21:07.935131 unisci-1.4.4/unisci/formulas/
--rw-r--r--   0 vivaan     (501) staff       (20)        0 2023-04-25 22:04:55.000000 unisci-1.4.4/unisci/formulas/__init__.py
--rw-r--r--   0 vivaan     (501) staff       (20)     2264 2023-04-30 22:55:51.000000 unisci-1.4.4/unisci/formulas/_validation.py
--rw-r--r--   0 vivaan     (501) staff       (20)    14458 2023-04-30 22:56:45.000000 unisci-1.4.4/unisci/formulas/chemistry.py
--rw-r--r--   0 vivaan     (501) staff       (20)     1842 2023-04-30 22:59:28.000000 unisci-1.4.4/unisci/metric.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-02 02:21:07.938266 unisci-1.4.4/unisci/periodic/
--rw-r--r--   0 vivaan     (501) staff       (20)   259692 2023-04-21 14:28:34.000000 unisci-1.4.4/unisci/periodic/periodic-table-lookup.json
--rw-r--r--   0 vivaan     (501) staff       (20)     2257 2023-04-21 14:47:26.000000 unisci-1.4.4/unisci/periodic/periodic-table-numbers.json
--rw-r--r--   0 vivaan     (501) staff       (20)     2233 2023-04-21 14:30:16.000000 unisci-1.4.4/unisci/periodic/periodic-table-symbols.json
--rw-r--r--   0 vivaan     (501) staff       (20)    38865 2023-04-30 22:56:45.000000 unisci-1.4.4/unisci/types.py
-drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-02 02:21:07.934302 unisci-1.4.4/unisci.egg-info/
--rw-r--r--   0 vivaan     (501) staff       (20)     1614 2023-05-02 02:21:07.000000 unisci-1.4.4/unisci.egg-info/PKG-INFO
--rw-r--r--   0 vivaan     (501) staff       (20)      525 2023-05-02 02:21:07.000000 unisci-1.4.4/unisci.egg-info/SOURCES.txt
--rw-r--r--   0 vivaan     (501) staff       (20)        1 2023-05-02 02:21:07.000000 unisci-1.4.4/unisci.egg-info/dependency_links.txt
--rw-r--r--   0 vivaan     (501) staff       (20)       30 2023-05-02 02:21:07.000000 unisci-1.4.4/unisci.egg-info/requires.txt
--rw-r--r--   0 vivaan     (501) staff       (20)        7 2023-05-02 02:21:07.000000 unisci-1.4.4/unisci.egg-info/top_level.txt
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-02 02:27:52.465433 unisci-1.4.5/
+-rw-r--r--   0 vivaan     (501) staff       (20)     1071 2023-04-17 11:50:57.000000 unisci-1.4.5/LICENSE
+-rw-r--r--   0 vivaan     (501) staff       (20)      188 2023-04-27 04:25:20.000000 unisci-1.4.5/MANIFEST.in
+-rw-r--r--   0 vivaan     (501) staff       (20)     1614 2023-05-02 02:27:52.465139 unisci-1.4.5/PKG-INFO
+-rw-r--r--   0 vivaan     (501) staff       (20)     1286 2023-04-28 05:01:19.000000 unisci-1.4.5/README.md
+-rw-r--r--   0 vivaan     (501) staff       (20)       38 2023-05-02 02:27:52.465535 unisci-1.4.5/setup.cfg
+-rw-r--r--   0 vivaan     (501) staff       (20)      679 2023-05-02 02:26:41.000000 unisci-1.4.5/setup.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-02 02:27:52.461114 unisci-1.4.5/unisci/
+-rw-r--r--   0 vivaan     (501) staff       (20)       87 2023-05-02 02:26:46.000000 unisci-1.4.5/unisci/__init__.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     1503 2023-05-01 22:47:16.000000 unisci-1.4.5/unisci/_conversion_factors.py
+-rw-r--r--   0 vivaan     (501) staff       (20)      607 2023-04-23 05:14:17.000000 unisci-1.4.5/unisci/_error.py
+-rw-r--r--   0 vivaan     (501) staff       (20)      386 2023-04-26 16:06:26.000000 unisci-1.4.5/unisci/constants.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-02 02:27:52.463446 unisci-1.4.5/unisci/formulas/
+-rw-r--r--   0 vivaan     (501) staff       (20)        0 2023-04-25 22:04:55.000000 unisci-1.4.5/unisci/formulas/__init__.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     2264 2023-04-30 22:55:51.000000 unisci-1.4.5/unisci/formulas/_validation.py
+-rw-r--r--   0 vivaan     (501) staff       (20)    14458 2023-04-30 22:56:45.000000 unisci-1.4.5/unisci/formulas/chemistry.py
+-rw-r--r--   0 vivaan     (501) staff       (20)     1842 2023-04-30 22:59:28.000000 unisci-1.4.5/unisci/metric.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-02 02:27:52.464754 unisci-1.4.5/unisci/periodic/
+-rw-r--r--   0 vivaan     (501) staff       (20)   259692 2023-04-21 14:28:34.000000 unisci-1.4.5/unisci/periodic/periodic-table-lookup.json
+-rw-r--r--   0 vivaan     (501) staff       (20)     2257 2023-04-21 14:47:26.000000 unisci-1.4.5/unisci/periodic/periodic-table-numbers.json
+-rw-r--r--   0 vivaan     (501) staff       (20)     2233 2023-04-21 14:30:16.000000 unisci-1.4.5/unisci/periodic/periodic-table-symbols.json
+-rw-r--r--   0 vivaan     (501) staff       (20)    39019 2023-05-02 02:25:51.000000 unisci-1.4.5/unisci/types.py
+drwxr-xr-x   0 vivaan     (501) staff       (20)        0 2023-05-02 02:27:52.462618 unisci-1.4.5/unisci.egg-info/
+-rw-r--r--   0 vivaan     (501) staff       (20)     1614 2023-05-02 02:27:52.000000 unisci-1.4.5/unisci.egg-info/PKG-INFO
+-rw-r--r--   0 vivaan     (501) staff       (20)      525 2023-05-02 02:27:52.000000 unisci-1.4.5/unisci.egg-info/SOURCES.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)        1 2023-05-02 02:27:52.000000 unisci-1.4.5/unisci.egg-info/dependency_links.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)       30 2023-05-02 02:27:52.000000 unisci-1.4.5/unisci.egg-info/requires.txt
+-rw-r--r--   0 vivaan     (501) staff       (20)        7 2023-05-02 02:27:52.000000 unisci-1.4.5/unisci.egg-info/top_level.txt
```

### Comparing `unisci-1.4.4/LICENSE` & `unisci-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `unisci-1.4.4/PKG-INFO` & `unisci-1.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unisci
-Version: 1.4.4
+Version: 1.4.5
 Summary: Units Conversions, and Science Package
 Author: Vivaan Singhvi
 Author-email: singhvi.vivaan@gmail.com
 License: MIT
 Project-URL: Documentation, https://unisci.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `unisci-1.4.4/README.md` & `unisci-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `unisci-1.4.4/setup.py` & `unisci-1.4.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     description = f.read()
 
 with open("requirements.txt") as f:
     requirements = f.readlines()
 
 setup(
     name='unisci',
-    version='1.4.4',
+    version='1.4.5',
     author='Vivaan Singhvi',
     author_email='singhvi.vivaan@gmail.com',
     description='Units Conversions, and Science Package',
     long_description=description,
     long_description_content_type="text/markdown",
     license='MIT',
     packages=find_packages(),
```

### Comparing `unisci-1.4.4/unisci/_conversion_factors.py` & `unisci-1.4.5/unisci/_conversion_factors.py`

 * *Files identical despite different names*

### Comparing `unisci-1.4.4/unisci/_error.py` & `unisci-1.4.5/unisci/_error.py`

 * *Files identical despite different names*

### Comparing `unisci-1.4.4/unisci/formulas/_validation.py` & `unisci-1.4.5/unisci/formulas/_validation.py`

 * *Files identical despite different names*

### Comparing `unisci-1.4.4/unisci/formulas/chemistry.py` & `unisci-1.4.5/unisci/formulas/chemistry.py`

 * *Files identical despite different names*

### Comparing `unisci-1.4.4/unisci/metric.py` & `unisci-1.4.5/unisci/metric.py`

 * *Files identical despite different names*

### Comparing `unisci-1.4.4/unisci/periodic/periodic-table-lookup.json` & `unisci-1.4.5/unisci/periodic/periodic-table-lookup.json`

 * *Files identical despite different names*

### Comparing `unisci-1.4.4/unisci/periodic/periodic-table-numbers.json` & `unisci-1.4.5/unisci/periodic/periodic-table-numbers.json`

 * *Files identical despite different names*

### Comparing `unisci-1.4.4/unisci/periodic/periodic-table-symbols.json` & `unisci-1.4.5/unisci/periodic/periodic-table-symbols.json`

 * *Files identical despite different names*

### Comparing `unisci-1.4.4/unisci/types.py` & `unisci-1.4.5/unisci/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,30 +151,34 @@
 
         elif isinstance(other, Temperature):
 
             raise CompatabilityError("A Quantity (absolute temperature) is incompatible for addition with a Temperature (relative temperature)")
         
         elif isinstance(other, Quantity):
 
+            # convert both to base units
+            self_temp = self.to_base_units()
+            other = other.to_base_units()
+
             # automatically convert all the other's units to self's units
-            other = other.converted(list(self.unit_type.keys()))
+            other = other.converted(list(self_temp.unit_type.keys()))
 
             # check for incompatability
-            if len(self.unit_type) != len(other.unit_type):
+            if len(self_temp.unit_type) != len(other.unit_type):
                 raise CompatabilityError("Quantity addition requires units to be of the same type and order.")
             
             # checks that all powers are the same
-            for key in self.unit_type.keys():
+            for key in self_temp.unit_type.keys():
                 try:
-                    if other.unit_type[key] != self.unit_type[key]:
+                    if other.unit_type[key] != self_temp.unit_type[key]:
                         raise CompatabilityError("Quantity addition requires units to be of the same type and order.")
                 except:
                     raise CompatabilityError("Quantity addition requires units to be of the same type and order.")
                 
-            return Quantity(self.number + other.number, self.unit_type.copy())
+            return Quantity(self_temp.number + other.number, self.unit_type.copy())
         
         else:
             raise UnsupportedError("Type is not supported for addition with Quantity.")
         
     def __radd__(self, other: Union[int, float, Quantity]) -> Quantity:
 
         """
```

### Comparing `unisci-1.4.4/unisci.egg-info/PKG-INFO` & `unisci-1.4.5/unisci.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unisci
-Version: 1.4.4
+Version: 1.4.5
 Summary: Units Conversions, and Science Package
 Author: Vivaan Singhvi
 Author-email: singhvi.vivaan@gmail.com
 License: MIT
 Project-URL: Documentation, https://unisci.readthedocs.io/en/latest/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `unisci-1.4.4/unisci.egg-info/SOURCES.txt` & `unisci-1.4.5/unisci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

