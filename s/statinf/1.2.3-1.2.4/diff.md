# Comparing `tmp/statinf-1.2.3.tar.gz` & `tmp/statinf-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statinf-1.2.3.tar", last modified: Sat Apr 29 17:49:44 2023, max compression
+gzip compressed data, was "statinf-1.2.4.tar", last modified: Tue May  2 11:44:34 2023, max compression
```

## Comparing `statinf-1.2.3.tar` & `statinf-1.2.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-29 17:49:44.373417 statinf-1.2.3/
--rw-r--r--   0 florian   (1000) florian   (1000)     1070 2020-10-01 18:31:13.000000 statinf-1.2.3/LICENSE
--rw-r--r--   0 florian   (1000) florian   (1000)     8825 2023-04-29 17:49:44.373417 statinf-1.2.3/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)     8337 2020-10-01 18:31:13.000000 statinf-1.2.3/README.md
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-04-29 17:49:44.373417 statinf-1.2.3/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)      781 2020-10-01 18:31:13.000000 statinf-1.2.3/setup.py
--rw-r--r--   0 florian   (1000) florian   (1000)      889 2023-04-29 17:49:43.000000 statinf-1.2.3/setup_new.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-29 17:49:44.363417 statinf-1.2.3/statinf/
--rw-r--r--   0 florian   (1000) florian   (1000)       22 2023-04-29 17:49:43.000000 statinf-1.2.3/statinf/__init__.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-29 17:49:44.363417 statinf-1.2.3/statinf/data/
--rw-r--r--   0 florian   (1000) florian   (1000)     2701 2023-02-03 18:48:52.000000 statinf-1.2.3/statinf/data/GenerateData.py
--rw-r--r--   0 florian   (1000) florian   (1000)    27132 2021-03-24 14:33:31.000000 statinf-1.2.3/statinf/data/ProcessData.py
--rw-r--r--   0 florian   (1000) florian   (1000)       55 2020-10-01 18:31:13.000000 statinf-1.2.3/statinf/data/__init__.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-29 17:49:44.363417 statinf-1.2.3/statinf/distributions/
--rw-r--r--   0 florian   (1000) florian   (1000)       24 2023-02-03 18:27:09.000000 statinf-1.2.3/statinf/distributions/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)    20379 2023-04-29 16:28:26.000000 statinf-1.2.3/statinf/distributions/discrete.py
--rw-r--r--   0 florian   (1000) florian   (1000)       26 2021-06-27 12:48:10.000000 statinf-1.2.3/statinf/init_template.py
--rw-r--r--   0 florian   (1000) florian   (1000)     5107 2021-06-27 13:22:48.000000 statinf-1.2.3/statinf/misc.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-29 17:49:44.373417 statinf-1.2.3/statinf/ml/
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2020-10-01 18:31:13.000000 statinf-1.2.3/statinf/ml/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)     2522 2021-03-07 06:24:49.000000 statinf-1.2.3/statinf/ml/activations.py
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2020-10-17 16:20:51.000000 statinf-1.2.3/statinf/ml/generative.py
--rw-r--r--   0 florian   (1000) florian   (1000)     2892 2021-03-07 06:09:35.000000 statinf-1.2.3/statinf/ml/initializations.py
--rw-r--r--   0 florian   (1000) florian   (1000)     3152 2021-03-07 06:45:42.000000 statinf-1.2.3/statinf/ml/losses.py
--rw-r--r--   0 florian   (1000) florian   (1000)    16863 2022-08-21 10:47:32.000000 statinf-1.2.3/statinf/ml/neuralnetwork.py
--rw-r--r--   0 florian   (1000) florian   (1000)    11152 2021-03-07 08:40:43.000000 statinf-1.2.3/statinf/ml/optimizers.py
--rw-r--r--   0 florian   (1000) florian   (1000)     6141 2021-06-27 13:22:59.000000 statinf-1.2.3/statinf/ml/performance.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-29 17:49:44.373417 statinf-1.2.3/statinf/nonparametrics/
--rw-r--r--   0 florian   (1000) florian   (1000)       23 2020-11-01 11:38:35.000000 statinf-1.2.3/statinf/nonparametrics/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)      842 2020-11-01 18:05:22.000000 statinf-1.2.3/statinf/nonparametrics/kernels.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-29 17:49:44.373417 statinf-1.2.3/statinf/regressions/
--rw-r--r--   0 florian   (1000) florian   (1000)    19249 2021-03-24 15:58:55.000000 statinf-1.2.3/statinf/regressions/LinearModels.py
--rw-r--r--   0 florian   (1000) florian   (1000)       51 2023-02-03 18:26:31.000000 statinf-1.2.3/statinf/regressions/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)    18168 2021-03-24 15:54:37.000000 statinf-1.2.3/statinf/regressions/glm.py
--rw-r--r--   0 florian   (1000) florian   (1000)     7060 2020-10-01 18:31:13.000000 statinf-1.2.3/statinf/regressions/glm_test.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-29 17:49:44.373417 statinf-1.2.3/statinf/stats/
--rw-r--r--   0 florian   (1000) florian   (1000)      126 2020-11-01 12:20:16.000000 statinf-1.2.3/statinf/stats/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)     6950 2020-11-01 18:03:36.000000 statinf-1.2.3/statinf/stats/bayesian.py
--rw-r--r--   0 florian   (1000) florian   (1000)     4185 2020-10-01 18:31:13.000000 statinf-1.2.3/statinf/stats/descriptive.py
--rw-r--r--   0 florian   (1000) florian   (1000)    21520 2023-02-03 18:58:48.000000 statinf-1.2.3/statinf/stats/tests.py
--rw-r--r--   0 florian   (1000) florian   (1000)    11524 2020-10-27 02:35:31.000000 statinf-1.2.3/statinf/stats/timeseries.py
--rw-r--r--   0 florian   (1000) florian   (1000)    10469 2020-11-01 18:02:58.000000 statinf-1.2.3/statinf/stats/unsupervised.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-29 17:49:44.363417 statinf-1.2.3/statinf.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     8825 2023-04-29 17:49:44.000000 statinf-1.2.3/statinf.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      966 2023-04-29 17:49:44.000000 statinf-1.2.3/statinf.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-04-29 17:49:44.000000 statinf-1.2.3/statinf.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)      101 2023-04-29 17:49:44.000000 statinf-1.2.3/statinf.egg-info/requires.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-04-29 17:49:44.000000 statinf-1.2.3/statinf.egg-info/top_level.txt
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-02 11:44:34.114357 statinf-1.2.4/
+-rw-r--r--   0 florian   (1000) florian   (1000)     1070 2020-10-01 18:31:13.000000 statinf-1.2.4/LICENSE
+-rw-r--r--   0 florian   (1000) florian   (1000)     8825 2023-05-02 11:44:34.114357 statinf-1.2.4/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     8337 2020-10-01 18:31:13.000000 statinf-1.2.4/README.md
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-05-02 11:44:34.114357 statinf-1.2.4/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)      781 2020-10-01 18:31:13.000000 statinf-1.2.4/setup.py
+-rw-r--r--   0 florian   (1000) florian   (1000)      889 2023-05-02 11:44:33.000000 statinf-1.2.4/setup_new.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-02 11:44:34.071023 statinf-1.2.4/statinf/
+-rw-r--r--   0 florian   (1000) florian   (1000)       22 2023-05-02 11:44:33.000000 statinf-1.2.4/statinf/__init__.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-02 11:44:34.081857 statinf-1.2.4/statinf/data/
+-rw-r--r--   0 florian   (1000) florian   (1000)     2701 2023-02-03 18:48:52.000000 statinf-1.2.4/statinf/data/GenerateData.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    27132 2021-03-24 14:33:31.000000 statinf-1.2.4/statinf/data/ProcessData.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       55 2020-10-01 18:31:13.000000 statinf-1.2.4/statinf/data/__init__.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-02 11:44:34.081857 statinf-1.2.4/statinf/distributions/
+-rw-r--r--   0 florian   (1000) florian   (1000)       24 2023-02-03 18:27:09.000000 statinf-1.2.4/statinf/distributions/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    20390 2023-05-02 09:53:55.000000 statinf-1.2.4/statinf/distributions/discrete.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       26 2021-06-27 12:48:10.000000 statinf-1.2.4/statinf/init_template.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     5107 2021-06-27 13:22:48.000000 statinf-1.2.4/statinf/misc.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-02 11:44:34.092690 statinf-1.2.4/statinf/ml/
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2020-10-01 18:31:13.000000 statinf-1.2.4/statinf/ml/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     2522 2021-03-07 06:24:49.000000 statinf-1.2.4/statinf/ml/activations.py
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2020-10-17 16:20:51.000000 statinf-1.2.4/statinf/ml/generative.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     2892 2021-03-07 06:09:35.000000 statinf-1.2.4/statinf/ml/initializations.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     3152 2021-03-07 06:45:42.000000 statinf-1.2.4/statinf/ml/losses.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    16863 2022-08-21 10:47:32.000000 statinf-1.2.4/statinf/ml/neuralnetwork.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    11152 2021-03-07 08:40:43.000000 statinf-1.2.4/statinf/ml/optimizers.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     6141 2021-06-27 13:22:59.000000 statinf-1.2.4/statinf/ml/performance.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-02 11:44:34.092690 statinf-1.2.4/statinf/nonparametrics/
+-rw-r--r--   0 florian   (1000) florian   (1000)       23 2020-11-01 11:38:35.000000 statinf-1.2.4/statinf/nonparametrics/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)      842 2020-11-01 18:05:22.000000 statinf-1.2.4/statinf/nonparametrics/kernels.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-02 11:44:34.103523 statinf-1.2.4/statinf/regressions/
+-rw-r--r--   0 florian   (1000) florian   (1000)    19249 2021-03-24 15:58:55.000000 statinf-1.2.4/statinf/regressions/LinearModels.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       51 2023-02-03 18:26:31.000000 statinf-1.2.4/statinf/regressions/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    18168 2021-03-24 15:54:37.000000 statinf-1.2.4/statinf/regressions/glm.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     7060 2020-10-01 18:31:13.000000 statinf-1.2.4/statinf/regressions/glm_test.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-02 11:44:34.114357 statinf-1.2.4/statinf/stats/
+-rw-r--r--   0 florian   (1000) florian   (1000)      126 2020-11-01 12:20:16.000000 statinf-1.2.4/statinf/stats/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     6950 2020-11-01 18:03:36.000000 statinf-1.2.4/statinf/stats/bayesian.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     4185 2020-10-01 18:31:13.000000 statinf-1.2.4/statinf/stats/descriptive.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    21520 2023-02-03 18:58:48.000000 statinf-1.2.4/statinf/stats/tests.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    11524 2020-10-27 02:35:31.000000 statinf-1.2.4/statinf/stats/timeseries.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    10469 2020-11-01 18:02:58.000000 statinf-1.2.4/statinf/stats/unsupervised.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-02 11:44:34.081857 statinf-1.2.4/statinf.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     8825 2023-05-02 11:44:34.000000 statinf-1.2.4/statinf.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      966 2023-05-02 11:44:34.000000 statinf-1.2.4/statinf.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-05-02 11:44:34.000000 statinf-1.2.4/statinf.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)      101 2023-05-02 11:44:34.000000 statinf-1.2.4/statinf.egg-info/requires.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-05-02 11:44:34.000000 statinf-1.2.4/statinf.egg-info/top_level.txt
```

### Comparing `statinf-1.2.3/LICENSE` & `statinf-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `statinf-1.2.3/PKG-INFO` & `statinf-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statinf
-Version: 1.2.3
+Version: 1.2.4
 Summary: A library for statistics and causal inference
 Home-page: https://www.florianfelice.com/statinf
 Author: Florian Felice
 Author-email: florian.felice@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `statinf-1.2.3/README.md` & `statinf-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `statinf-1.2.3/setup.py` & `statinf-1.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.3/setup_new.py` & `statinf-1.2.4/setup_new.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="statinf",
-    version="1.2.3",
+    version="1.2.4",
     author="Florian Felice",
     author_email="florian.felice@outlook.com",
     description="A library for statistics and causal inference",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.florianfelice.com/statinf",
     packages=setuptools.find_packages(),
```

### Comparing `statinf-1.2.3/statinf/data/GenerateData.py` & `statinf-1.2.4/statinf/data/GenerateData.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.3/statinf/data/ProcessData.py` & `statinf-1.2.4/statinf/data/ProcessData.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.3/statinf/distributions/discrete.py` & `statinf-1.2.4/statinf/distributions/discrete.py`

 * *Files 4% similar despite different names*

```diff
@@ -342,39 +342,27 @@
         :type log: :obj:`bool`
 
         :return: Normalizing factor :math:`Z`
         :rtype: :obj:`float`
         """
         j = j if j else self.j
 
-        # ## Almost exact form
-        z_i = - np.inf
-        z_last = 0
-        current_j = 0
-
-        while (np.abs(z_i - z_last) > self.eps) & (current_j < j):
-            z_last = z_i
-            _log_fact = np.sum(np.log(range(1, current_j)))
-            z_i = self._log_sum(z_i, current_j * math.log(lambda_) - nu_ * _log_fact)
-            current_j += 1
-
-        if not log:
-            z_i = math.exp(z_i)
-
-        return float(np.sum(z_i))
-
-    def _log_sum(self, x, y):
-        if x == -np.inf:
-            return y
-        elif y == -np.inf:
-            return x
-        elif x > y:
-            return x + math.log(1 + math.exp(y - x))
-        else:
-            return y + math.log(1 + math.exp(x - y))
+        try:
+            _num = [np.exp(_j * np.log(lambda_)) for _j in range(j)]
+            _denom = [np.exp(nu_ * np.sum(np.log(range(1, _j + 1)))) for _j in range(j)]
+        except RuntimeWarning:
+            _num = [np.exp(Decimal(_j) * Decimal(np.log(lambda_))) for _j in range(j)]
+            _denom = [np.exp(Decimal(nu_) * Decimal(np.sum(np.log(range(1, _j + 1))))) for _j in range(j)]
+
+        z_i = float(np.sum([_n / _d for _n, _d in zip(_num, _denom) if (_n < np.inf) & (_d < np.inf)]))
+
+        if log:
+            z_i = math.log(z_i)
+
+        return z_i
 
     def pmf(self, x) -> float:
         """Computes the probability mass function for selected value :obj:`x`.
 
         :formula: The probability mass function (pmf) is computed by
 
             .. math:: \\mathbb{P}(X = x | \\lambda, \\nu) = \\dfrac{\\lambda^{x}}{(x!)^{\\nu}} \\dfrac{1}{Z(\\lambda, \\nu)}
@@ -398,15 +386,17 @@
         except OverflowError:
             # Inf the integers to compute are too large, we use decimal format
             # Ref: https://stackoverflow.com/questions/16174399/overflowerror-long-int-too-large-to-convert-to-float-in-python
             _pow = [Decimal(p) for p in _pow]
             _dec = True
 
         # Compute $(x!)^{\nu}$
-        _fact = [pow(np.exp(np.sum(np.log(range(1, _x)))), self.nu_) for _x in x]
+        _fact = [np.exp(self.nu_ * np.sum(np.log(range(1, _x + 1)))) for _x in x]
+        if _dec:
+            _fact = [Decimal(f) for f in _fact]
 
         a = np.array([float(p / f) for p, f in zip(_pow, _fact)])
         return a * (1 / self._Z)
 
     @staticmethod
     def nloglike(params, data, Z, j=100) -> float:
         """Static method to estumate the negative likelihood (used in :meth:`statinf.distributions.discrete.CMPoisson.fit` method).
@@ -430,18 +420,20 @@
         X = np.asarray(data)
         n = len(X)
 
         # Compute log(Z)
         log_Z = Z(lambda_=lambda_, nu_=nu_, j=j, log=True)
 
         _log_fact = np.asarray([math.log(math.factorial(_x)) for _x in X])
-        ll = (math.log(lambda_) * np.sum(X)) - (nu_ * np.sum(_log_fact)) - (n * log_Z)
+        ll = math.log(lambda_) * np.sum(X)
+        ll += - (nu_ * np.sum(_log_fact))
+        ll += - (n * log_Z)
         return -ll
 
-    def fit(self, data, method='L-BFGS-B', init_params='auto', j=None) -> dict:
+    def fit(self, data, method='L-BFGS-B', init_params='auto', j=None, bounds=None) -> dict:
         """Estimates the parameters :math:`\\lambda` and :math:`\\nu` of the distribution from empirical data based on Maximum Likelihood Estimation.
 
         .. note::
 
             There is no close form to estimate the parameters nor a direct relation between the empirical moments (:math:`\\bar{X}`) and the theoretical ones.
             Therefore, only MLE is available (no fast method).
 
@@ -453,25 +445,26 @@
         :type init_params: :obj:`numpy.array`, optional
 
         :return: Estimated parameters
         :rtype: :obj:`dict`
         """
         # We transform warnings as error (for overflow) to handle in try / except: https://stackoverflow.com/questions/5644836/
         j = j if j else self.j
-        bounds = [(self.eps, None), (self.eps, None)]
+        if bounds is None:
+            bounds = [(self.eps, None), (self.eps, None)]
         if init_params == 'auto':
-            _disp = data.std() / data.mean()
-            init_params = np.array([1., _disp])
+            _disp = data.var() / data.mean()
+            init_params = np.array([data.mean(), _disp])
 
         res = self._fit(data=data, bounds=bounds, method=method, init_params=init_params, args=(j,))
         self.lambda_ = res.x[0]
         self.nu_ = res.x[1]
         warnings.filterwarnings("error")
         self._Z = self.Z(lambda_=self.lambda_, nu_=self.nu_, j=j)
         warnings.resetwarnings()
 
         out = {'lambda_': self.lambda_, 'nu_': self.nu_, 'convergence': res.success}
 
         if method in scipy_methods:
-            out.update({'nll': self.nll})
+            out.update({'loglikelihood': -self.nll})
 
         return out
```

### Comparing `statinf-1.2.3/statinf/misc.py` & `statinf-1.2.4/statinf/misc.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.3/statinf/ml/activations.py` & `statinf-1.2.4/statinf/ml/activations.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.3/statinf/ml/initializations.py` & `statinf-1.2.4/statinf/ml/initializations.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.3/statinf/ml/losses.py` & `statinf-1.2.4/statinf/ml/losses.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.3/statinf/ml/neuralnetwork.py` & `statinf-1.2.4/statinf/ml/neuralnetwork.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.3/statinf/ml/optimizers.py` & `statinf-1.2.4/statinf/ml/optimizers.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.3/statinf/ml/performance.py` & `statinf-1.2.4/statinf/ml/performance.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.3/statinf/nonparametrics/kernels.py` & `statinf-1.2.4/statinf/nonparametrics/kernels.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.3/statinf/regressions/LinearModels.py` & `statinf-1.2.4/statinf/regressions/LinearModels.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.3/statinf/regressions/glm.py` & `statinf-1.2.4/statinf/regressions/glm.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.3/statinf/regressions/glm_test.py` & `statinf-1.2.4/statinf/regressions/glm_test.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.3/statinf/stats/bayesian.py` & `statinf-1.2.4/statinf/stats/bayesian.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.3/statinf/stats/descriptive.py` & `statinf-1.2.4/statinf/stats/descriptive.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.3/statinf/stats/tests.py` & `statinf-1.2.4/statinf/stats/tests.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.3/statinf/stats/timeseries.py` & `statinf-1.2.4/statinf/stats/timeseries.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.3/statinf/stats/unsupervised.py` & `statinf-1.2.4/statinf/stats/unsupervised.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.3/statinf.egg-info/PKG-INFO` & `statinf-1.2.4/statinf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statinf
-Version: 1.2.3
+Version: 1.2.4
 Summary: A library for statistics and causal inference
 Home-page: https://www.florianfelice.com/statinf
 Author: Florian Felice
 Author-email: florian.felice@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `statinf-1.2.3/statinf.egg-info/SOURCES.txt` & `statinf-1.2.4/statinf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

