# Comparing `tmp/se_lib-0.26.tar.gz` & `tmp/se_lib-0.26.1.tar.gz`

## Comparing `se_lib-0.26.tar` & `se_lib-0.26.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 se_lib-0.26/.DS_Store
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 se_lib-0.26/.gitattributes
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 se_lib-0.26/selib/.DS_Store
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 se_lib-0.26/selib/__init__.py
--rw-r--r--   0        0        0    66120 2020-02-02 00:00:00.000000 se_lib-0.26/selib/selib.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 se_lib-0.26/LICENSE
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 se_lib-0.26/README.md
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 se_lib-0.26/pyproject.toml
--rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 se_lib-0.26/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 se_lib-0.26.1/.DS_Store
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 se_lib-0.26.1/.gitattributes
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 se_lib-0.26.1/selib/.DS_Store
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 se_lib-0.26.1/selib/__init__.py
+-rw-r--r--   0        0        0    66122 2020-02-02 00:00:00.000000 se_lib-0.26.1/selib/selib.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 se_lib-0.26.1/LICENSE
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 se_lib-0.26.1/README.md
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 se_lib-0.26.1/pyproject.toml
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 se_lib-0.26.1/PKG-INFO
```

### Comparing `se_lib-0.26/.DS_Store` & `se_lib-0.26.1/.DS_Store`

 * *Files identical despite different names*

### Comparing `se_lib-0.26/selib/.DS_Store` & `se_lib-0.26.1/selib/.DS_Store`

 * *Files identical despite different names*

### Comparing `se_lib-0.26/selib/selib.py` & `se_lib-0.26.1/selib/selib.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-se-lib Version .26
+se-lib Version .26.1
 
 Copyright (c) 2022-2023 Ray Madachy
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `se_lib-0.26/LICENSE` & `se_lib-0.26.1/LICENSE`

 * *Files identical despite different names*

### Comparing `se_lib-0.26/README.md` & `se_lib-0.26.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Systems Engineering Library (se-lib)
-Version .26
+Version .26.1
 
 Copyright (c) 2022-2023 se-lib Development Team
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `se_lib-0.26/pyproject.toml` & `se_lib-0.26.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "se-lib"
-version = "0.26"
+version = "0.26.1"
 authors = [
   { name="se-lib Development Team", email="info@se-lib.org" },
 ]
 description = "Systems Engineering Library (se-lib)"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `se_lib-0.26/PKG-INFO` & `se_lib-0.26.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: se-lib
-Version: 0.26
+Version: 0.26.1
 Summary: Systems Engineering Library (se-lib)
 Project-URL: Homepage, http://se-lib.org
 Author-email: se-lib Development Team <info@se-lib.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Requires-Dist: matplotlib
 Requires-Dist: netcdf4
 Requires-Dist: pandas
 Requires-Dist: pysd
 Description-Content-Type: text/markdown
 
 # Systems Engineering Library (se-lib)
-Version .26
+Version .26.1
 
 Copyright (c) 2022-2023 se-lib Development Team
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

