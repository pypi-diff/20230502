# Comparing `tmp/polynomiograpy-0.2.0a1.tar.gz` & `tmp/polynomiograpy-0.2.0a1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polynomiograpy-0.2.0a1.tar", max compression
+gzip compressed data, was "polynomiograpy-0.2.0a1.post1.tar", max compression
```

## Comparing `polynomiograpy-0.2.0a1.tar` & `polynomiograpy-0.2.0a1.post1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-05-01 01:47:51.256690 polynomiograpy-0.2.0a1/LICENSE
--rw-r--r--   0        0        0       68 2023-05-01 01:39:06.537562 polynomiograpy-0.2.0a1/README.md
--rw-r--r--   0        0        0      414 2023-05-02 08:46:19.553798 polynomiograpy-0.2.0a1/polynomiograpy/__init__.py
--rw-r--r--   0        0        0     4851 2023-05-02 08:45:57.985613 polynomiograpy-0.2.0a1/polynomiograpy/cli/__init__.py
--rw-r--r--   0        0        0      970 2023-05-02 08:39:43.286847 polynomiograpy-0.2.0a1/polynomiograpy/common/finite_field.py
--rw-r--r--   0        0        0     1458 2023-05-01 02:13:32.052248 polynomiograpy-0.2.0a1/polynomiograpy/common/polynomial.py
--rw-r--r--   0        0        0     1991 2023-05-02 08:14:34.251805 polynomiograpy-0.2.0a1/polynomiograpy/iterations/__init__.py
--rw-r--r--   0        0        0     1266 2023-05-02 07:52:35.745113 polynomiograpy-0.2.0a1/polynomiograpy/iterations/helpers.py
--rw-r--r--   0        0        0     2279 2023-05-02 07:44:10.901452 polynomiograpy-0.2.0a1/polynomiograpy/iterations/methods.py
--rw-r--r--   0        0        0      915 2023-05-02 08:43:46.491492 polynomiograpy-0.2.0a1/polynomiograpy/roots/__init__.py
--rw-r--r--   0        0        0      931 2023-05-02 08:15:06.208942 polynomiograpy-0.2.0a1/polynomiograpy/roots/helpers.py
--rw-r--r--   0        0        0      738 2023-05-02 08:46:46.725578 polynomiograpy-0.2.0a1/pyproject.toml
--rw-r--r--   0        0        0      738 1970-01-01 00:00:00.000000 polynomiograpy-0.2.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-01 01:47:51.256690 polynomiograpy-0.2.0a1.post1/LICENSE
+-rw-r--r--   0        0        0       68 2023-05-01 01:39:06.537562 polynomiograpy-0.2.0a1.post1/README.md
+-rw-r--r--   0        0        0      420 2023-05-02 08:57:40.472153 polynomiograpy-0.2.0a1.post1/polynomiograpy/__init__.py
+-rw-r--r--   0        0        0     4797 2023-05-02 08:54:25.623761 polynomiograpy-0.2.0a1.post1/polynomiograpy/cli/__init__.py
+-rw-r--r--   0        0        0      970 2023-05-02 08:39:43.286847 polynomiograpy-0.2.0a1.post1/polynomiograpy/common/finite_field.py
+-rw-r--r--   0        0        0     1458 2023-05-01 02:13:32.052248 polynomiograpy-0.2.0a1.post1/polynomiograpy/common/polynomial.py
+-rw-r--r--   0        0        0     1991 2023-05-02 08:14:34.251805 polynomiograpy-0.2.0a1.post1/polynomiograpy/iterations/__init__.py
+-rw-r--r--   0        0        0     1266 2023-05-02 07:52:35.745113 polynomiograpy-0.2.0a1.post1/polynomiograpy/iterations/helpers.py
+-rw-r--r--   0        0        0     2279 2023-05-02 07:44:10.901452 polynomiograpy-0.2.0a1.post1/polynomiograpy/iterations/methods.py
+-rw-r--r--   0        0        0      915 2023-05-02 08:43:46.491492 polynomiograpy-0.2.0a1.post1/polynomiograpy/roots/__init__.py
+-rw-r--r--   0        0        0      931 2023-05-02 08:15:06.208942 polynomiograpy-0.2.0a1.post1/polynomiograpy/roots/helpers.py
+-rw-r--r--   0        0        0      744 2023-05-02 08:56:30.404622 polynomiograpy-0.2.0a1.post1/pyproject.toml
+-rw-r--r--   0        0        0      744 1970-01-01 00:00:00.000000 polynomiograpy-0.2.0a1.post1/PKG-INFO
```

### Comparing `polynomiograpy-0.2.0a1/LICENSE` & `polynomiograpy-0.2.0a1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `polynomiograpy-0.2.0a1/polynomiograpy/cli/__init__.py` & `polynomiograpy-0.2.0a1.post1/polynomiograpy/cli/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,22 +84,20 @@
 def run_iter():
     print("** Complex Plane Setup **")
     min_real = int(input_with_default("Min Real (-3): ", "-3"))
     max_real = int(input_with_default("Max Real (3): ", "3"))
     min_imag = int(input_with_default("Min Imag (-3): ", "-3"))
     max_imag = int(input_with_default("Max Imag (3): ", "3"))
     print("** Polynomial **")
-    poly_degree = int(input("Degree of the polynomial: "))
-    coeffs = []
-    for i in range(poly_degree + 1):
-        coeffs.append(
-            int(input_with_default(f"Int coefficient of x^{poly_degree-i} (1): ", "1"))
-        )
-    coeffs.reverse()
-    poly = Polynomial(coeffs=coeffs)
+    coeffs: str = input_with_default(
+        "Coefficients from degree d to 0 (1,0,0,1): ", "1,0,0,1"
+    )
+    parsed_coeffs = [int(e) for e in coeffs.split(",")]
+    parsed_coeffs.reverse()
+    poly = Polynomial(coeffs=parsed_coeffs)
     print(f"Polynomial: {poly}")
     print("** Method **")
     print(f"Available methods: {available_methods}")
     method = input_with_default("Method (newton): ", "newton")
     delta = float(input_with_default("convergence threshold (0.1): ", "0.1"))
     max_iter = int(input_with_default("Max iteration (16): ", "16"))
     print("** Output Setup **")
```

### Comparing `polynomiograpy-0.2.0a1/polynomiograpy/common/finite_field.py` & `polynomiograpy-0.2.0a1.post1/polynomiograpy/common/finite_field.py`

 * *Files identical despite different names*

### Comparing `polynomiograpy-0.2.0a1/polynomiograpy/common/polynomial.py` & `polynomiograpy-0.2.0a1.post1/polynomiograpy/common/polynomial.py`

 * *Files identical despite different names*

### Comparing `polynomiograpy-0.2.0a1/polynomiograpy/iterations/__init__.py` & `polynomiograpy-0.2.0a1.post1/polynomiograpy/iterations/__init__.py`

 * *Files identical despite different names*

### Comparing `polynomiograpy-0.2.0a1/polynomiograpy/iterations/helpers.py` & `polynomiograpy-0.2.0a1.post1/polynomiograpy/iterations/helpers.py`

 * *Files identical despite different names*

### Comparing `polynomiograpy-0.2.0a1/polynomiograpy/iterations/methods.py` & `polynomiograpy-0.2.0a1.post1/polynomiograpy/iterations/methods.py`

 * *Files identical despite different names*

### Comparing `polynomiograpy-0.2.0a1/polynomiograpy/roots/__init__.py` & `polynomiograpy-0.2.0a1.post1/polynomiograpy/roots/__init__.py`

 * *Files identical despite different names*

### Comparing `polynomiograpy-0.2.0a1/polynomiograpy/roots/helpers.py` & `polynomiograpy-0.2.0a1.post1/polynomiograpy/roots/helpers.py`

 * *Files identical despite different names*

### Comparing `polynomiograpy-0.2.0a1/pyproject.toml` & `polynomiograpy-0.2.0a1.post1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polynomiograpy"
-version = "0.2.0.a1"
+version = "0.2.0.a1.post1"
 description = ""
 authors = ["İsmail Tapan <ismltpn@gmail.com>"]
 maintainers = ["İsmail Tapan <ismltpn@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = ""
 repository = "https://github.com/ismltpn/polynomiograpy/"
```

### Comparing `polynomiograpy-0.2.0a1/PKG-INFO` & `polynomiograpy-0.2.0a1.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polynomiograpy
-Version: 0.2.0a1
+Version: 0.2.0a1.post1
 Summary: 
 Home-page: https://github.com/ismltpn/polynomiograpy/
 License: MIT
 Keywords: Polynomiography,Polynomials,Visual Art
 Author: İsmail Tapan
 Author-email: ismltpn@gmail.com
 Maintainer: İsmail Tapan
```

