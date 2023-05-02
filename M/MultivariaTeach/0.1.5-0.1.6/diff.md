# Comparing `tmp/MultivariaTeach-0.1.5.tar.gz` & `tmp/MultivariaTeach-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MultivariaTeach-0.1.5.tar", last modified: Tue May  2 21:22:32 2023, max compression
+gzip compressed data, was "MultivariaTeach-0.1.6.tar", last modified: Tue May  2 21:32:47 2023, max compression
```

## Comparing `MultivariaTeach-0.1.5.tar` & `MultivariaTeach-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwx------   0 ben        (501) staff       (20)        0 2023-05-02 21:22:32.421158 MultivariaTeach-0.1.5/
--rw-------   0 ben        (501) staff       (20)      743 2023-04-25 22:03:04.000000 MultivariaTeach-0.1.5/LICENSE
-drwx------   0 ben        (501) staff       (20)        0 2023-05-02 21:22:32.419844 MultivariaTeach-0.1.5/MultivariaTeach.egg-info/
--rw-------   0 ben        (501) staff       (20)    15366 2023-05-02 21:22:32.000000 MultivariaTeach-0.1.5/MultivariaTeach.egg-info/PKG-INFO
--rw-------   0 ben        (501) staff       (20)      330 2023-05-02 21:22:32.000000 MultivariaTeach-0.1.5/MultivariaTeach.egg-info/SOURCES.txt
--rw-------   0 ben        (501) staff       (20)        1 2023-05-02 21:22:32.000000 MultivariaTeach-0.1.5/MultivariaTeach.egg-info/dependency_links.txt
--rw-------   0 ben        (501) staff       (20)       41 2023-05-02 21:22:32.000000 MultivariaTeach-0.1.5/MultivariaTeach.egg-info/requires.txt
--rw-------   0 ben        (501) staff       (20)       22 2023-05-02 21:22:32.000000 MultivariaTeach-0.1.5/MultivariaTeach.egg-info/top_level.txt
--rw-------   0 ben        (501) staff       (20)    15366 2023-05-02 21:22:32.421013 MultivariaTeach-0.1.5/PKG-INFO
--rw-------   0 ben        (501) staff       (20)    14698 2023-05-02 21:22:03.000000 MultivariaTeach-0.1.5/README.md
-drwx------   0 ben        (501) staff       (20)        0 2023-05-02 21:22:32.420164 MultivariaTeach-0.1.5/multivariateach/
--rw-------   0 ben        (501) staff       (20)       31 2023-05-02 20:33:56.000000 MultivariaTeach-0.1.5/multivariateach/__init__.py
--rw-------   0 ben        (501) staff       (20)    11161 2023-05-01 19:52:12.000000 MultivariaTeach-0.1.5/multivariateach/multivariateach.py
--rw-------   0 ben        (501) staff       (20)       38 2023-05-02 21:22:32.421193 MultivariaTeach-0.1.5/setup.cfg
--rw-------   0 ben        (501) staff       (20)      932 2023-05-02 21:22:26.000000 MultivariaTeach-0.1.5/setup.py
-drwx------   0 ben        (501) staff       (20)        0 2023-05-02 21:22:32.420628 MultivariaTeach-0.1.5/tests/
--rw-------   0 ben        (501) staff       (20)        0 2023-04-25 22:05:08.000000 MultivariaTeach-0.1.5/tests/__init__.py
--rw-------   0 ben        (501) staff       (20)     7016 2023-05-01 22:22:43.000000 MultivariaTeach-0.1.5/tests/test_multivariteach.py
+drwx------   0 ben        (501) staff       (20)        0 2023-05-02 21:32:47.749146 MultivariaTeach-0.1.6/
+-rw-------   0 ben        (501) staff       (20)      743 2023-04-25 22:03:04.000000 MultivariaTeach-0.1.6/LICENSE
+drwx------   0 ben        (501) staff       (20)        0 2023-05-02 21:32:47.747702 MultivariaTeach-0.1.6/MultivariaTeach.egg-info/
+-rw-------   0 ben        (501) staff       (20)    15366 2023-05-02 21:32:47.000000 MultivariaTeach-0.1.6/MultivariaTeach.egg-info/PKG-INFO
+-rw-------   0 ben        (501) staff       (20)      330 2023-05-02 21:32:47.000000 MultivariaTeach-0.1.6/MultivariaTeach.egg-info/SOURCES.txt
+-rw-------   0 ben        (501) staff       (20)        1 2023-05-02 21:32:47.000000 MultivariaTeach-0.1.6/MultivariaTeach.egg-info/dependency_links.txt
+-rw-------   0 ben        (501) staff       (20)       41 2023-05-02 21:32:47.000000 MultivariaTeach-0.1.6/MultivariaTeach.egg-info/requires.txt
+-rw-------   0 ben        (501) staff       (20)       22 2023-05-02 21:32:47.000000 MultivariaTeach-0.1.6/MultivariaTeach.egg-info/top_level.txt
+-rw-------   0 ben        (501) staff       (20)    15366 2023-05-02 21:32:47.748999 MultivariaTeach-0.1.6/PKG-INFO
+-rw-------   0 ben        (501) staff       (20)    14698 2023-05-02 21:32:06.000000 MultivariaTeach-0.1.6/README.md
+drwx------   0 ben        (501) staff       (20)        0 2023-05-02 21:32:47.748102 MultivariaTeach-0.1.6/multivariateach/
+-rw-------   0 ben        (501) staff       (20)       31 2023-05-02 20:33:56.000000 MultivariaTeach-0.1.6/multivariateach/__init__.py
+-rw-------   0 ben        (501) staff       (20)    11161 2023-05-01 19:52:12.000000 MultivariaTeach-0.1.6/multivariateach/multivariateach.py
+-rw-------   0 ben        (501) staff       (20)       38 2023-05-02 21:32:47.749182 MultivariaTeach-0.1.6/setup.cfg
+-rw-------   0 ben        (501) staff       (20)      932 2023-05-02 21:32:38.000000 MultivariaTeach-0.1.6/setup.py
+drwx------   0 ben        (501) staff       (20)        0 2023-05-02 21:32:47.748569 MultivariaTeach-0.1.6/tests/
+-rw-------   0 ben        (501) staff       (20)        0 2023-04-25 22:05:08.000000 MultivariaTeach-0.1.6/tests/__init__.py
+-rw-------   0 ben        (501) staff       (20)     7016 2023-05-01 22:22:43.000000 MultivariaTeach-0.1.6/tests/test_multivariteach.py
```

### Comparing `MultivariaTeach-0.1.5/LICENSE` & `MultivariaTeach-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `MultivariaTeach-0.1.5/MultivariaTeach.egg-info/PKG-INFO` & `MultivariaTeach-0.1.6/MultivariaTeach.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MultivariaTeach
-Version: 0.1.5
+Version: 0.1.6
 Summary: A collection of tools intended for students of multivariate analysis
 Home-page: https://github.com/Ben-Goren/MultivariaTeach
 Author: Ben Goren
 Author-email: bgoren@asu.edu
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: ISC License (ISCL)
@@ -121,15 +121,15 @@
 
 Unlike with most other software, you are not presented with a pretty-formatted table of results; instead, the `results` object can now be itself queried for … well, for anything and everything. So, for example, a simple-but-complete test might look like this:
 
 ```python
 import numpy as np
 import pandas as pd
 from sklearn import datasets
-import MultivariaTeach as mt
+import multivariateach as mt
 
 iris = datasets.load_iris() # Fisher's 1936 flower data
 
 data = pd.DataFrame(np.hstack([iris.target.reshape(-1, 1), iris.data])) # Extract the parts we want in the structure we need
 data.columns = ['group', 'x1', 'x2', 'x3', 'x4'] # Give names to the columns
 
 X = mt.create_design_matrix(data, 'group')
```

### Comparing `MultivariaTeach-0.1.5/PKG-INFO` & `MultivariaTeach-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MultivariaTeach
-Version: 0.1.5
+Version: 0.1.6
 Summary: A collection of tools intended for students of multivariate analysis
 Home-page: https://github.com/Ben-Goren/MultivariaTeach
 Author: Ben Goren
 Author-email: bgoren@asu.edu
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: ISC License (ISCL)
@@ -121,15 +121,15 @@
 
 Unlike with most other software, you are not presented with a pretty-formatted table of results; instead, the `results` object can now be itself queried for … well, for anything and everything. So, for example, a simple-but-complete test might look like this:
 
 ```python
 import numpy as np
 import pandas as pd
 from sklearn import datasets
-import MultivariaTeach as mt
+import multivariateach as mt
 
 iris = datasets.load_iris() # Fisher's 1936 flower data
 
 data = pd.DataFrame(np.hstack([iris.target.reshape(-1, 1), iris.data])) # Extract the parts we want in the structure we need
 data.columns = ['group', 'x1', 'x2', 'x3', 'x4'] # Give names to the columns
 
 X = mt.create_design_matrix(data, 'group')
```

### Comparing `MultivariaTeach-0.1.5/README.md` & `MultivariaTeach-0.1.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
 Unlike with most other software, you are not presented with a pretty-formatted table of results; instead, the `results` object can now be itself queried for … well, for anything and everything. So, for example, a simple-but-complete test might look like this:
 
 ```python
 import numpy as np
 import pandas as pd
 from sklearn import datasets
-import MultivariaTeach as mt
+import multivariateach as mt
 
 iris = datasets.load_iris() # Fisher's 1936 flower data
 
 data = pd.DataFrame(np.hstack([iris.target.reshape(-1, 1), iris.data])) # Extract the parts we want in the structure we need
 data.columns = ['group', 'x1', 'x2', 'x3', 'x4'] # Give names to the columns
 
 X = mt.create_design_matrix(data, 'group')
```

### Comparing `MultivariaTeach-0.1.5/multivariateach/multivariateach.py` & `MultivariaTeach-0.1.6/multivariateach/multivariateach.py`

 * *Files identical despite different names*

### Comparing `MultivariaTeach-0.1.5/setup.py` & `MultivariaTeach-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="MultivariaTeach",
-    version="0.1.5",
+    version="0.1.6",
     description="A collection of tools intended for students of multivariate analysis",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     author="Ben Goren",
     author_email="bgoren@asu.edu",
     url="https://github.com/Ben-Goren/MultivariaTeach",
     packages=find_packages(),
```

### Comparing `MultivariaTeach-0.1.5/tests/test_multivariteach.py` & `MultivariaTeach-0.1.6/tests/test_multivariteach.py`

 * *Files identical despite different names*

