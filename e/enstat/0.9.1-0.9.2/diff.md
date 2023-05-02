# Comparing `tmp/enstat-0.9.1.tar.gz` & `tmp/enstat-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enstat-0.9.1.tar", last modified: Mon Apr 24 14:28:06 2023, max compression
+gzip compressed data, was "enstat-0.9.2.tar", last modified: Tue May  2 10:19:22 2023, max compression
```

## Comparing `enstat-0.9.1.tar` & `enstat-0.9.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:06.883530 enstat-0.9.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:06.879530 enstat-0.9.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:06.879530 enstat-0.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-24 14:27:57.000000 enstat-0.9.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-24 14:27:57.000000 enstat-0.9.1/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-24 14:27:57.000000 enstat-0.9.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-24 14:27:57.000000 enstat-0.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-24 14:27:57.000000 enstat-0.9.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-24 14:27:57.000000 enstat-0.9.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-24 14:27:57.000000 enstat-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-24 14:28:06.883530 enstat-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-24 14:27:57.000000 enstat-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:06.879530 enstat-0.9.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-24 14:27:57.000000 enstat-0.9.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-24 14:27:57.000000 enstat-0.9.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-24 14:27:57.000000 enstat-0.9.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-24 14:27:57.000000 enstat-0.9.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-24 14:27:57.000000 enstat-0.9.1/docs/module.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:06.879530 enstat-0.9.1/enstat/
--rw-r--r--   0 runner    (1001) docker     (123)    26261 2023-04-24 14:27:57.000000 enstat-0.9.1/enstat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-24 14:28:06.000000 enstat-0.9.1/enstat/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-04-24 14:27:57.000000 enstat-0.9.1/enstat/detail.py
--rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-04-24 14:27:57.000000 enstat-0.9.1/enstat/mean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:06.883530 enstat-0.9.1/enstat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-24 14:28:06.000000 enstat-0.9.1/enstat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-24 14:28:06.000000 enstat-0.9.1/enstat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 14:28:06.000000 enstat-0.9.1/enstat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 14:28:06.000000 enstat-0.9.1/enstat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 14:28:06.000000 enstat-0.9.1/enstat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-24 14:27:57.000000 enstat-0.9.1/environment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-24 14:27:57.000000 enstat-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 14:28:06.883530 enstat-0.9.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:28:06.883530 enstat-0.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:27:57.000000 enstat-0.9.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-04-24 14:27:57.000000 enstat-0.9.1/tests/test_binned.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-04-24 14:27:57.000000 enstat-0.9.1/tests/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-04-24 14:27:57.000000 enstat-0.9.1/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:19:22.800221 enstat-0.9.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:19:22.796221 enstat-0.9.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:19:22.800221 enstat-0.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-02 10:19:14.000000 enstat-0.9.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-02 10:19:14.000000 enstat-0.9.2/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-02 10:19:14.000000 enstat-0.9.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-02 10:19:14.000000 enstat-0.9.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-02 10:19:14.000000 enstat-0.9.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-02 10:19:14.000000 enstat-0.9.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-02 10:19:14.000000 enstat-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-05-02 10:19:22.800221 enstat-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-02 10:19:14.000000 enstat-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:19:22.800221 enstat-0.9.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-02 10:19:14.000000 enstat-0.9.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-02 10:19:14.000000 enstat-0.9.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-02 10:19:14.000000 enstat-0.9.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-02 10:19:14.000000 enstat-0.9.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-02 10:19:14.000000 enstat-0.9.2/docs/module.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:19:22.800221 enstat-0.9.2/enstat/
+-rw-r--r--   0 runner    (1001) docker     (123)    27159 2023-05-02 10:19:14.000000 enstat-0.9.2/enstat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-02 10:19:22.000000 enstat-0.9.2/enstat/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-05-02 10:19:14.000000 enstat-0.9.2/enstat/detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-05-02 10:19:14.000000 enstat-0.9.2/enstat/mean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:19:22.800221 enstat-0.9.2/enstat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-05-02 10:19:22.000000 enstat-0.9.2/enstat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-02 10:19:22.000000 enstat-0.9.2/enstat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 10:19:22.000000 enstat-0.9.2/enstat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 10:19:22.000000 enstat-0.9.2/enstat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 10:19:22.000000 enstat-0.9.2/enstat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-02 10:19:14.000000 enstat-0.9.2/environment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-02 10:19:14.000000 enstat-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 10:19:22.800221 enstat-0.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:19:22.800221 enstat-0.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 10:19:14.000000 enstat-0.9.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-05-02 10:19:14.000000 enstat-0.9.2/tests/test_binned.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-05-02 10:19:14.000000 enstat-0.9.2/tests/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-05-02 10:19:14.000000 enstat-0.9.2/tests/test_main.py
```

### Comparing `enstat-0.9.1/.github/workflows/pre-commit.yml` & `enstat-0.9.2/.github/workflows/pre-commit.yml`

 * *Files identical despite different names*

### Comparing `enstat-0.9.1/.gitignore` & `enstat-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `enstat-0.9.1/.pre-commit-config.yaml` & `enstat-0.9.2/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
   - id: autoflake
     args: [--in-place, --remove-unused-variable, --remove-all-unused-imports]
 - repo: https://github.com/asottile/reorder_python_imports
   rev: v3.9.0
   hooks:
   - id: reorder-python-imports
 - repo: https://github.com/asottile/pyupgrade
-  rev: v3.3.1
+  rev: v3.3.2
   hooks:
   - id: pyupgrade
     args: [--py36-plus]
 - repo: https://github.com/PyCQA/flake8
   rev: 6.0.0
   hooks:
   - id: flake8
```

### Comparing `enstat-0.9.1/LICENSE` & `enstat-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `enstat-0.9.1/PKG-INFO` & `enstat-0.9.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: enstat
-Version: 0.9.1
+Version: 0.9.2
+Summary: Ensemble averages
 Author-email: Tom de Geus <tom@geus.me>
 Project-URL: Source, https://github.com/tdegeus/enstat
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `enstat-0.9.1/README.md` & `enstat-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `enstat-0.9.1/docs/Makefile` & `enstat-0.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `enstat-0.9.1/docs/make.bat` & `enstat-0.9.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `enstat-0.9.1/docs/module.rst` & `enstat-0.9.2/docs/module.rst`

 * *Files identical despite different names*

### Comparing `enstat-0.9.1/enstat/__init__.py` & `enstat-0.9.2/enstat/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,19 +44,31 @@
 
         ret = cls()
         ret.first = first
         ret.second = second
         ret.norm = norm
         return ret
 
-    def __add__(self, datum: float):
+    def __add__(self, datum: float | ArrayLike):
         self.add_sample(datum)
         return self
 
-    def add_sample(self, datum: float):
+    def __itruediv__(self, factor: float):
+        assert not hasattr(factor, "__len__")
+        self.first /= factor
+        self.second /= factor**2
+        return self
+
+    def __imul__(self, factor: float):
+        assert not hasattr(factor, "__len__")
+        self.first *= factor
+        self.second *= factor**2
+        return self
+
+    def add_sample(self, datum: float | ArrayLike):
         """
         Add a sample.
         Internally changes the sums of the first and second statistical moments and normalisation.
 
         :param datum: Sample.
         """
 
@@ -226,14 +238,30 @@
             norm=np.sum(self.norm),
         )
 
     def __add__(self, data: ArrayLike):
         self.add_sample(data)
         return self
 
+    def __itruediv__(self, factor: float | ArrayLike):
+        if hasattr(factor, "__len__"):
+            assert factor.shape == self.first.shape
+        self.first /= factor
+        if self.second is not None:
+            self.second /= factor**2
+        return self
+
+    def __imul__(self, factor: float | ArrayLike):
+        if hasattr(factor, "__len__"):
+            assert factor.shape == self.first.shape
+        self.first *= factor
+        if self.second is not None:
+            self.second *= factor**2
+        return self
+
     def add_sample(self, data: ArrayLike, mask: ArrayLike = None):
         r"""
         Add a sample.
         Internally changes the sums of the first and second statistical moments and normalisation.
 
         :param data: The sample.
         :param mask: Mask entries (boolean array).
```

### Comparing `enstat-0.9.1/enstat/detail.py` & `enstat-0.9.2/enstat/detail.py`

 * *Files identical despite different names*

### Comparing `enstat-0.9.1/enstat/mean.py` & `enstat-0.9.2/enstat/mean.py`

 * *Files identical despite different names*

### Comparing `enstat-0.9.1/enstat.egg-info/PKG-INFO` & `enstat-0.9.2/enstat.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: enstat
-Version: 0.9.1
+Version: 0.9.2
+Summary: Ensemble averages
 Author-email: Tom de Geus <tom@geus.me>
 Project-URL: Source, https://github.com/tdegeus/enstat
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `enstat-0.9.1/enstat.egg-info/SOURCES.txt` & `enstat-0.9.2/enstat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enstat-0.9.1/tests/test_binned.py` & `enstat-0.9.2/tests/test_binned.py`

 * *Files identical despite different names*

### Comparing `enstat-0.9.1/tests/test_histogram.py` & `enstat-0.9.2/tests/test_histogram.py`

 * *Files identical despite different names*

### Comparing `enstat-0.9.1/tests/test_main.py` & `enstat-0.9.2/tests/test_main.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,29 +24,65 @@
         self.assertTrue(np.isnan(average.std()))
 
         average += np.array(1.0)
 
         self.assertFalse(np.isnan(average.mean()))
         self.assertFalse(np.isnan(average.std()))
 
-    def test_scalar_division(self):
+    def test_scalar_zero_division(self):
         """
         Check for zero division.
         """
 
         average = enstat.scalar()
 
         a = np.random.random(50 * 20).reshape(50, 20)
 
         for i in range(a.shape[0]):
             average += a[i, :]
 
         self.assertTrue(np.isclose(average.mean(), np.mean(a)))
         self.assertTrue(np.isclose(average.std(), np.std(a), rtol=1e-3))
 
+    def test_scalar_units_div(self):
+        """
+        Change units.
+        """
+
+        average = enstat.scalar()
+
+        a = np.random.random(50 * 20).reshape(50, 20)
+        factor = np.random.random() + 0.1
+        aprime = a / factor
+
+        for i in range(a.shape[0]):
+            average += a[i, :]
+
+        average /= factor
+        self.assertTrue(np.isclose(average.mean(), np.mean(aprime)))
+        self.assertTrue(np.isclose(average.std(), np.std(aprime), rtol=1e-3))
+
+    def test_scalar_units_mul(self):
+        """
+        Change units.
+        """
+
+        average = enstat.scalar()
+
+        a = np.random.random(50 * 20).reshape(50, 20)
+        factor = np.random.random() + 0.1
+        aprime = a * factor
+
+        for i in range(a.shape[0]):
+            average += a[i, :]
+
+        average *= factor
+        self.assertTrue(np.isclose(average.mean(), np.mean(aprime)))
+        self.assertTrue(np.isclose(average.std(), np.std(aprime), rtol=1e-3))
+
     def test_static(self):
         """
         Basic test of "mean" and "std" using a random sample.
         """
 
         average = enstat.static()
 
@@ -56,14 +92,56 @@
             average += a[i, :, :]
 
         self.assertTrue(np.allclose(average.mean(), np.mean(a, axis=0)))
         self.assertTrue(np.allclose(average.std(), np.std(a, axis=0), rtol=5e-1, atol=1e-3))
         self.assertTrue(average.shape == a.shape[1:])
         self.assertTrue(average.size == np.prod(a.shape[1:]))
 
+    def test_static_units_div(self):
+        """
+        Change units.
+        """
+
+        average = enstat.static()
+
+        a = np.random.random(35 * 50 * 20).reshape(35, 50, 20)
+        factor = np.random.random() + 0.1
+        aprime = a / factor
+
+        for i in range(a.shape[0]):
+            average += a[i, :, :]
+
+        average /= factor
+
+        self.assertTrue(np.allclose(average.mean(), np.mean(aprime, axis=0)))
+        self.assertTrue(np.allclose(average.std(), np.std(aprime, axis=0), rtol=5e-1, atol=1e-3))
+        self.assertTrue(average.shape == a.shape[1:])
+        self.assertTrue(average.size == np.prod(a.shape[1:]))
+
+    def test_static_units_mul(self):
+        """
+        Change units.
+        """
+
+        average = enstat.static()
+
+        a = np.random.random(35 * 50 * 20).reshape(35, 50, 20)
+        factor = np.random.random() + 0.1
+        aprime = a * factor
+
+        for i in range(a.shape[0]):
+            average += a[i, :, :]
+
+        average *= factor
+
+        self.assertTrue(np.allclose(average.mean(), np.mean(aprime, axis=0)))
+        self.assertTrue(np.allclose(average.std(), np.std(aprime, axis=0), rtol=5e-1, atol=1e-3))
+        self.assertTrue(average.shape == a.shape[1:])
+        self.assertTrue(average.size == np.prod(a.shape[1:]))
+
     def test_static_ravel(self):
         """
         Like :py:func:`test_static` but with a test of `ravel`.
         """
 
         arraylike = enstat.static()
         scalar = enstat.scalar()
```

