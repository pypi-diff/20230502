# Comparing `tmp/q_random_number_generator-0.0.5.tar.gz` & `tmp/q_random_number_generator-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "q_random_number_generator-0.0.5.tar", last modified: Tue May  2 13:32:02 2023, max compression
+gzip compressed data, was "q_random_number_generator-0.0.6.tar", last modified: Tue May  2 14:29:50 2023, max compression
```

## Comparing `q_random_number_generator-0.0.5.tar` & `q_random_number_generator-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 13:32:02.942980 q_random_number_generator-0.0.5/
--rw-rw-rw-   0        0        0     1065 2023-05-02 11:39:46.000000 q_random_number_generator-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      522 2023-05-02 13:32:02.941062 q_random_number_generator-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       78 2023-05-02 12:16:38.000000 q_random_number_generator-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 13:32:02.923876 q_random_number_generator-0.0.5/q_random_number_generator/
--rw-rw-rw-   0        0        0     1432 2023-05-02 13:26:10.000000 q_random_number_generator-0.0.5/q_random_number_generator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:32:02.937936 q_random_number_generator-0.0.5/q_random_number_generator.egg-info/
--rw-rw-rw-   0        0        0      522 2023-05-02 13:32:02.000000 q_random_number_generator-0.0.5/q_random_number_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-05-02 13:32:02.000000 q_random_number_generator-0.0.5/q_random_number_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 13:32:02.000000 q_random_number_generator-0.0.5/q_random_number_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-05-02 13:32:02.000000 q_random_number_generator-0.0.5/q_random_number_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 13:32:02.943975 q_random_number_generator-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      667 2023-05-02 13:31:56.000000 q_random_number_generator-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 14:29:50.100030 q_random_number_generator-0.0.6/
+-rw-rw-rw-   0        0        0     1065 2023-05-02 11:39:46.000000 q_random_number_generator-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      675 2023-05-02 14:29:50.098029 q_random_number_generator-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2023-05-02 14:29:13.000000 q_random_number_generator-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 14:29:50.079510 q_random_number_generator-0.0.6/q_random_number_generator/
+-rw-rw-rw-   0        0        0     1454 2023-05-02 14:26:30.000000 q_random_number_generator-0.0.6/q_random_number_generator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 14:29:50.094033 q_random_number_generator-0.0.6/q_random_number_generator.egg-info/
+-rw-rw-rw-   0        0        0      675 2023-05-02 14:29:49.000000 q_random_number_generator-0.0.6/q_random_number_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-05-02 14:29:49.000000 q_random_number_generator-0.0.6/q_random_number_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 14:29:49.000000 q_random_number_generator-0.0.6/q_random_number_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-05-02 14:29:49.000000 q_random_number_generator-0.0.6/q_random_number_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 14:29:50.100030 q_random_number_generator-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      667 2023-05-02 14:26:39.000000 q_random_number_generator-0.0.6/setup.py
```

### Comparing `q_random_number_generator-0.0.5/LICENSE` & `q_random_number_generator-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `q_random_number_generator-0.0.5/PKG-INFO` & `q_random_number_generator-0.0.6/q_random_number_generator.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,26 @@
 Metadata-Version: 2.1
-Name: q_random_number_generator
-Version: 0.0.5
+Name: q-random-number-generator
+Version: 0.0.6
 Summary: Using qiskit to realize random number generator
 Home-page: https://github.com/allen91wu/q_random_number_generator
 Author: Allen Wu
 Author-email: allen91.wu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # q_random_number_generator
+
+## Description
 Using qiskit to realize quantum number generator.
+
+## Example
+```python
+import q_rand_number_generator as qrng
+
+random_int = qrng.randint(-50, 50, 10)
+```
+## Author
+- Allen Wu
```

### Comparing `q_random_number_generator-0.0.5/q_random_number_generator/__init__.py` & `q_random_number_generator-0.0.6/q_random_number_generator/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     QC = QuantumCircuit(qr, cr)
     QC.h(range(q_counts))
     QC.measure(qr, cr)
     return QC
 
 
 def generate(start, end, total):
-    maximum = end
+    maximum = max(abs(start), abs(end))
     collected = 0
     qbits = 0
 
     # decision qubits counts
     isInt = int(math.log2(maximum)) == math.log2(maximum)
     if isInt is True:
         qbits = math.ceil(math.log2(maximum)) + 2
```

### Comparing `q_random_number_generator-0.0.5/q_random_number_generator.egg-info/PKG-INFO` & `q_random_number_generator-0.0.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,26 @@
 Metadata-Version: 2.1
-Name: q-random-number-generator
-Version: 0.0.5
+Name: q_random_number_generator
+Version: 0.0.6
 Summary: Using qiskit to realize random number generator
 Home-page: https://github.com/allen91wu/q_random_number_generator
 Author: Allen Wu
 Author-email: allen91.wu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # q_random_number_generator
+
+## Description
 Using qiskit to realize quantum number generator.
+
+## Example
+```python
+import q_rand_number_generator as qrng
+
+random_int = qrng.randint(-50, 50, 10)
+```
+## Author
+- Allen Wu
```

### Comparing `q_random_number_generator-0.0.5/setup.py` & `q_random_number_generator-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="q_random_number_generator",
-    version="0.0.5",
+    version="0.0.6",
     author="Allen Wu",
     author_email="allen91.wu@gmail.com",
     description="Using qiskit to realize random number generator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/allen91wu/q_random_number_generator",
     packages=setuptools.find_packages(),
```

