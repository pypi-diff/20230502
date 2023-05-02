# Comparing `tmp/bs_python_utils-0.0.3.tar.gz` & `tmp/bs_python_utils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs_python_utils-0.0.3.tar", max compression
+gzip compressed data, was "bs_python_utils-0.0.4.tar", max compression
```

## Comparing `bs_python_utils-0.0.3.tar` & `bs_python_utils-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1073 2023-04-21 14:06:07.415664 bs_python_utils-0.0.3/LICENSE
--rw-r--r--   0        0        0     1119 2023-04-24 22:47:51.485025 bs_python_utils-0.0.3/README.md
--rw-r--r--   0        0        0     1799 2023-04-24 19:42:58.427840 bs_python_utils-0.0.3/bs_python_utils/Timer.py
--rw-r--r--   0        0        0        0 2023-04-24 19:42:58.429294 bs_python_utils-0.0.3/bs_python_utils/__init__.py
--rw-r--r--   0        0        0    28473 2023-04-24 22:57:44.859499 bs_python_utils-0.0.3/bs_python_utils/bs_altair.py
--rw-r--r--   0        0        0     2976 2023-04-24 20:25:24.489951 bs_python_utils-0.0.3/bs_python_utils/bs_logging.py
--rw-r--r--   0        0        0     3577 2023-04-24 19:42:58.433666 bs_python_utils-0.0.3/bs_python_utils/bs_mathstr.py
--rw-r--r--   0        0        0     4338 2023-04-24 21:45:53.142922 bs_python_utils-0.0.3/bs_python_utils/bs_mem.py
--rw-r--r--   0        0        0    13696 2023-04-24 22:48:26.403984 bs_python_utils-0.0.3/bs_python_utils/bs_opt.py
--rw-r--r--   0        0        0       36 2023-04-24 19:42:58.438686 bs_python_utils-0.0.3/bs_python_utils/bs_plots.py
--rw-r--r--   0        0        0     4507 2023-04-24 20:32:13.556809 bs_python_utils-0.0.3/bs_python_utils/bs_seaborn.py
--rw-r--r--   0        0        0     1391 2023-04-24 22:48:26.302214 bs_python_utils-0.0.3/bs_python_utils/bs_sparse_gaussian.py
--rw-r--r--   0        0        0      905 2023-04-24 19:42:58.441367 bs_python_utils-0.0.3/bs_python_utils/bsmplutils.py
--rw-r--r--   0        0        0    29170 2023-04-24 20:25:24.806746 bs_python_utils-0.0.3/bs_python_utils/bsnputils.py
--rw-r--r--   0        0        0     2132 2023-04-24 20:25:24.253141 bs_python_utils-0.0.3/bs_python_utils/bssputils.py
--rw-r--r--   0        0        0    15489 2023-04-24 20:25:24.644930 bs_python_utils-0.0.3/bs_python_utils/bsstats.py
--rw-r--r--   0        0        0     9199 2023-04-24 20:25:24.587557 bs_python_utils-0.0.3/bs_python_utils/bsutils.py
--rw-r--r--   0        0        0     7801 2023-04-24 21:45:53.165270 bs_python_utils-0.0.3/bs_python_utils/distance_covariances.py
--rw-r--r--   0        0        0     1350 2023-04-24 22:36:28.733299 bs_python_utils-0.0.3/bs_python_utils/example_opt.py
--rw-r--r--   0        0        0     3833 2023-04-24 22:48:26.344134 bs_python_utils-0.0.3/bs_python_utils/examples_altair.py
--rw-r--r--   0        0        0     1013 2023-04-24 22:36:28.733372 bs_python_utils-0.0.3/bs_python_utils/examples_distance_covariances.py
--rw-r--r--   0        0        0      552 2023-04-24 22:36:28.733335 bs_python_utils-0.0.3/bs_python_utils/examples_mem.py
--rw-r--r--   0        0        0      771 2023-04-24 21:45:53.146924 bs_python_utils-0.0.3/bs_python_utils/examples_seaborn.py
--rw-r--r--   0        0        0      786 2023-04-24 22:36:28.733292 bs_python_utils-0.0.3/bs_python_utils/examples_sklearn.py
--rw-r--r--   0        0        0     7426 2023-04-24 20:25:24.576148 bs_python_utils-0.0.3/bs_python_utils/pandas_utils.py
--rw-r--r--   0        0        0     1872 2023-04-24 21:46:50.361114 bs_python_utils-0.0.3/bs_python_utils/sklearn_utils.py
--rw-r--r--   0        0        0     1871 2023-04-24 22:47:22.264599 bs_python_utils-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2091 1970-01-01 00:00:00.000000 bs_python_utils-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-21 14:06:07.415664 bs_python_utils-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1210 2023-05-02 17:34:41.331375 bs_python_utils-0.0.4/README.md
+-rw-r--r--   0        0        0     1799 2023-04-24 19:42:58.427840 bs_python_utils-0.0.4/bs_python_utils/Timer.py
+-rw-r--r--   0        0        0        0 2023-04-24 19:42:58.429294 bs_python_utils-0.0.4/bs_python_utils/__init__.py
+-rw-r--r--   0        0        0    28473 2023-04-24 22:57:44.859499 bs_python_utils-0.0.4/bs_python_utils/bs_altair.py
+-rw-r--r--   0        0        0     2976 2023-04-24 20:25:24.489951 bs_python_utils-0.0.4/bs_python_utils/bs_logging.py
+-rw-r--r--   0        0        0     3577 2023-04-24 19:42:58.433666 bs_python_utils-0.0.4/bs_python_utils/bs_mathstr.py
+-rw-r--r--   0        0        0     4338 2023-04-24 21:45:53.142922 bs_python_utils-0.0.4/bs_python_utils/bs_mem.py
+-rw-r--r--   0        0        0    13696 2023-04-24 22:48:26.403984 bs_python_utils-0.0.4/bs_python_utils/bs_opt.py
+-rw-r--r--   0        0        0       36 2023-04-24 19:42:58.438686 bs_python_utils-0.0.4/bs_python_utils/bs_plots.py
+-rw-r--r--   0        0        0     4507 2023-04-24 20:32:13.556809 bs_python_utils-0.0.4/bs_python_utils/bs_seaborn.py
+-rw-r--r--   0        0        0     1391 2023-04-24 22:48:26.302214 bs_python_utils-0.0.4/bs_python_utils/bs_sparse_gaussian.py
+-rw-r--r--   0        0        0      905 2023-04-24 19:42:58.441367 bs_python_utils-0.0.4/bs_python_utils/bsmplutils.py
+-rw-r--r--   0        0        0    31781 2023-05-02 17:31:44.506884 bs_python_utils-0.0.4/bs_python_utils/bsnputils.py
+-rw-r--r--   0        0        0     2132 2023-04-24 20:25:24.253141 bs_python_utils-0.0.4/bs_python_utils/bssputils.py
+-rw-r--r--   0        0        0    15489 2023-04-24 20:25:24.644930 bs_python_utils-0.0.4/bs_python_utils/bsstats.py
+-rw-r--r--   0        0        0     9199 2023-04-24 20:25:24.587557 bs_python_utils-0.0.4/bs_python_utils/bsutils.py
+-rw-r--r--   0        0        0     7801 2023-04-24 21:45:53.165270 bs_python_utils-0.0.4/bs_python_utils/distance_covariances.py
+-rw-r--r--   0        0        0     1350 2023-04-24 22:36:28.733299 bs_python_utils-0.0.4/bs_python_utils/example_opt.py
+-rw-r--r--   0        0        0     3833 2023-04-24 22:48:26.344134 bs_python_utils-0.0.4/bs_python_utils/examples_altair.py
+-rw-r--r--   0        0        0     1013 2023-04-24 22:36:28.733372 bs_python_utils-0.0.4/bs_python_utils/examples_distance_covariances.py
+-rw-r--r--   0        0        0      552 2023-04-24 22:36:28.733335 bs_python_utils-0.0.4/bs_python_utils/examples_mem.py
+-rw-r--r--   0        0        0      771 2023-04-24 21:45:53.146924 bs_python_utils-0.0.4/bs_python_utils/examples_seaborn.py
+-rw-r--r--   0        0        0      786 2023-04-24 22:36:28.733292 bs_python_utils-0.0.4/bs_python_utils/examples_sklearn.py
+-rw-r--r--   0        0        0     7426 2023-04-24 20:25:24.576148 bs_python_utils-0.0.4/bs_python_utils/pandas_utils.py
+-rw-r--r--   0        0        0     1872 2023-04-24 21:46:50.361114 bs_python_utils-0.0.4/bs_python_utils/sklearn_utils.py
+-rw-r--r--   0        0        0     1871 2023-05-02 17:33:54.399911 bs_python_utils-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2182 1970-01-01 00:00:00.000000 bs_python_utils-0.0.4/PKG-INFO
```

### Comparing `bs_python_utils-0.0.3/LICENSE` & `bs_python_utils-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.3/README.md` & `bs_python_utils-0.0.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -10,12 +10,15 @@
 
 - **Github repository**: <https://github.com/bsalanie/bs-python-utils/>
 - **Documentation** <https://bsalanie.github.io/bs-python-utils/>
 
 
 ### Release notes
 
+#### 0.0.4 (May 2, 2023)
+Added Legendre polynomials and quantile routines in `bsnputils`.
+
 #### 0.0.3  (April 24, 2023)
 Satisfied mypy.
 
 #### 0.0.2  (April 24, 2023)
 Fixed main PyPI page.
```

### Comparing `bs_python_utils-0.0.3/bs_python_utils/Timer.py` & `bs_python_utils-0.0.4/bs_python_utils/Timer.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.3/bs_python_utils/bs_altair.py` & `bs_python_utils-0.0.4/bs_python_utils/bs_altair.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.3/bs_python_utils/bs_logging.py` & `bs_python_utils-0.0.4/bs_python_utils/bs_logging.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.3/bs_python_utils/bs_mathstr.py` & `bs_python_utils-0.0.4/bs_python_utils/bs_mathstr.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.3/bs_python_utils/bs_mem.py` & `bs_python_utils-0.0.4/bs_python_utils/bs_mem.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.3/bs_python_utils/bs_opt.py` & `bs_python_utils-0.0.4/bs_python_utils/bs_opt.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.3/bs_python_utils/bs_seaborn.py` & `bs_python_utils-0.0.4/bs_python_utils/bs_seaborn.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.3/bs_python_utils/bs_sparse_gaussian.py` & `bs_python_utils-0.0.4/bs_python_utils/bs_sparse_gaussian.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.3/bs_python_utils/bsmplutils.py` & `bs_python_utils-0.0.4/bs_python_utils/bsmplutils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.3/bs_python_utils/bsnputils.py` & `bs_python_utils-0.0.4/bs_python_utils/bsnputils.py`

 * *Files 2% similar despite different names*

```diff
@@ -951,7 +951,95 @@
         else:
             # to ensure integral_val has the same shape as f
             integral_val = weights[0] * f(nodes[0], pars)
             for i in range(1, n_nodes):
                 integral_val += weights[i] * f(nodes[i], pars)
 
     return cast(np.ndarray, integral_vec) if vectorized else cast(float, integral_val)
+
+
+def legendre_polynomials(
+    x: np.ndarray,
+    max_deg: int,
+    a: float = -1.0,
+    b: float = 1.0,
+    no_constant: bool = False,
+) -> np.ndarray:
+    """evaluates the Legendre polynomials over x in the interval [a, b]
+
+    Args:
+        x: the points where the polynomials are to be evaluated
+        max_deg: the maximum degree
+        a: the start of the interval, classically -1
+        b: the end of the interval, classically 1
+        no_constant: if True, delete the constant polynomial
+
+    Returns:
+        an array of (max_deg+1) arrays of the shape of x
+    """
+    sx = check_vector(x)
+    if a > np.min(x):
+        sys.exit("legendre_polynomials: points below start of interval")
+    if b < np.max(x):
+        sys.exit("legendre_polynomials: points above end of interval")
+    p = np.zeros((sx, max_deg + 1))
+    x_transf = 2.0 * (x - a) / (b - a) - 1.0
+    p[:, 0] = np.ones_like(x)
+    p[:, 1] = x_transf
+    for deg in range(2, max_deg + 1):
+        p2 = (2 * deg - 1) * (p[:, deg - 1] * x_transf) - (deg - 1) * p[:, deg - 2]
+        p[:, deg] = p2 / deg
+    polys_p = p[:, 1:] if no_constant else p
+    return polys_p
+
+
+def quantile_transform(v: np.ndarray) -> np.ndarray:
+    """transform a vector of counts into the corresponding quantiles
+
+    Args:
+        v:  a vector of counts
+
+    Returns:
+         the corresponding quantiles
+    """
+    n = check_vector(v)
+    q = np.zeros(n)
+    for i in range(n):
+        q[i] = np.sum(v <= v[i]) / (n + 1)
+    return q
+
+
+def print_quantiles(
+    v: np.ndarray | Iterable[np.ndarray], quantiles: np.ndarray
+) -> np.ndarray:
+    """print these quantiles of the array(s)
+
+    Args:
+        v:  a vector or an iterable of vectors
+        quantiles: quantiles in [0,1]
+
+    Returns:
+         the corresponding quantiles as a vector or a matrix
+    """
+    nq = check_vector(quantiles)
+    if isinstance(v, np.ndarray):
+        qvals = np.quantile(v, quantiles)
+        for q, qv in zip(quantiles, qvals, strict=True):
+            print(f"Quantile {q: .3f}: {qv: >10.3f}")
+    elif isinstance(v, Iterable):
+        v = list(v)
+        for v_i in v:
+            _ = check_vector(v_i)
+        nv = len(v)
+        qvals = np.zeros((nq, nv))
+        for i in range(nv):
+            qvals[:, i] = np.quantile(v[i], quantiles)
+        for iq, q in enumerate(quantiles):
+            s = f"Quantile {q: .3f}: "
+            qv = qvals[iq, :]
+            for i in range(nv):
+                s += f"  {qv[i]: >10.3f}"
+            print(f"{s}")
+    else:
+        bs_error_abort("v must be  a vector or a list of vectors")
+
+    return cast(np.ndarray, qvals)
```

### Comparing `bs_python_utils-0.0.3/bs_python_utils/bssputils.py` & `bs_python_utils-0.0.4/bs_python_utils/bssputils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.3/bs_python_utils/bsstats.py` & `bs_python_utils-0.0.4/bs_python_utils/bsstats.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.3/bs_python_utils/bsutils.py` & `bs_python_utils-0.0.4/bs_python_utils/bsutils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.3/bs_python_utils/distance_covariances.py` & `bs_python_utils-0.0.4/bs_python_utils/distance_covariances.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.3/bs_python_utils/example_opt.py` & `bs_python_utils-0.0.4/bs_python_utils/example_opt.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.3/bs_python_utils/examples_altair.py` & `bs_python_utils-0.0.4/bs_python_utils/examples_altair.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.3/bs_python_utils/examples_distance_covariances.py` & `bs_python_utils-0.0.4/bs_python_utils/examples_distance_covariances.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.3/bs_python_utils/examples_mem.py` & `bs_python_utils-0.0.4/bs_python_utils/examples_mem.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.3/bs_python_utils/examples_seaborn.py` & `bs_python_utils-0.0.4/bs_python_utils/examples_seaborn.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.3/bs_python_utils/examples_sklearn.py` & `bs_python_utils-0.0.4/bs_python_utils/examples_sklearn.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.3/bs_python_utils/pandas_utils.py` & `bs_python_utils-0.0.4/bs_python_utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.3/bs_python_utils/sklearn_utils.py` & `bs_python_utils-0.0.4/bs_python_utils/sklearn_utils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.3/pyproject.toml` & `bs_python_utils-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bs_python_utils"
-version = "0.0.3"
+version = "0.0.4"
 description = "my Python utilities"
 authors = ["Bernard Salanie <fbsalanie@columbia.edu>"]
 repository = "https://github.com/bsalanie/bs-python-utils"
 documentation = "https://bsalanie.github.io/bs-python-utils/"
 readme = "README.md"
 packages = [
   {include = "bs_python_utils"}
```

### Comparing `bs_python_utils-0.0.3/PKG-INFO` & `bs_python_utils-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bs-python-utils
-Version: 0.0.3
+Version: 0.0.4
 Summary: my Python utilities
 Home-page: https://github.com/bsalanie/bs-python-utils
 Author: Bernard Salanie
 Author-email: fbsalanie@columbia.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -34,13 +34,16 @@
 
 - **Github repository**: <https://github.com/bsalanie/bs-python-utils/>
 - **Documentation** <https://bsalanie.github.io/bs-python-utils/>
 
 
 ### Release notes
 
+#### 0.0.4 (May 2, 2023)
+Added Legendre polynomials and quantile routines in `bsnputils`.
+
 #### 0.0.3  (April 24, 2023)
 Satisfied mypy.
 
 #### 0.0.2  (April 24, 2023)
 Fixed main PyPI page.
```

