# Comparing `tmp/causalforge-0.0.5.tar.gz` & `tmp/causalforge-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causalforge-0.0.5.tar", last modified: Wed Apr 26 23:22:24 2023, max compression
+gzip compressed data, was "causalforge-0.0.6.tar", last modified: Mon May  1 23:41:36 2023, max compression
```

## Comparing `causalforge-0.0.5.tar` & `causalforge-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-04-26 23:22:24.868419 causalforge-0.0.5/
--rw-r--r--   0 AG62216    (501) staff       (20)     1065 2023-04-22 02:11:58.000000 causalforge-0.0.5/LICENSE
--rw-r--r--   0 AG62216    (501) staff       (20)     2499 2023-04-26 23:22:24.868624 causalforge-0.0.5/PKG-INFO
--rw-r--r--   0 AG62216    (501) staff       (20)     2048 2023-04-26 23:21:19.000000 causalforge-0.0.5/README.md
-drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-04-26 23:22:24.863670 causalforge-0.0.5/causalforge/
--rw-r--r--   0 AG62216    (501) staff       (20)       62 2023-04-26 23:21:33.000000 causalforge-0.0.5/causalforge/__init__.py
-drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-04-26 23:22:24.867959 causalforge-0.0.5/causalforge/tests/
--rw-r--r--   0 AG62216    (501) staff       (20)        0 2023-04-22 02:11:58.000000 causalforge-0.0.5/causalforge/tests/__init__.py
-drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-04-26 23:22:24.867195 causalforge-0.0.5/causalforge.egg-info/
--rw-r--r--   0 AG62216    (501) staff       (20)     2499 2023-04-26 23:22:24.000000 causalforge-0.0.5/causalforge.egg-info/PKG-INFO
--rw-r--r--   0 AG62216    (501) staff       (20)      264 2023-04-26 23:22:24.000000 causalforge-0.0.5/causalforge.egg-info/SOURCES.txt
--rw-r--r--   0 AG62216    (501) staff       (20)        1 2023-04-26 23:22:24.000000 causalforge-0.0.5/causalforge.egg-info/dependency_links.txt
--rw-r--r--   0 AG62216    (501) staff       (20)      134 2023-04-26 23:22:24.000000 causalforge-0.0.5/causalforge.egg-info/requires.txt
--rw-r--r--   0 AG62216    (501) staff       (20)       12 2023-04-26 23:22:24.000000 causalforge-0.0.5/causalforge.egg-info/top_level.txt
--rw-r--r--   0 AG62216    (501) staff       (20)      102 2023-04-26 23:22:24.869594 causalforge-0.0.5/setup.cfg
--rw-r--r--   0 AG62216    (501) staff       (20)     1659 2023-04-26 23:15:59.000000 causalforge-0.0.5/setup.py
+drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-05-01 23:41:36.446056 causalforge-0.0.6/
+-rw-r--r--   0 AG62216    (501) staff       (20)     1065 2023-04-22 02:11:58.000000 causalforge-0.0.6/LICENSE
+-rw-r--r--   0 AG62216    (501) staff       (20)     2895 2023-05-01 23:41:36.446198 causalforge-0.0.6/PKG-INFO
+-rw-r--r--   0 AG62216    (501) staff       (20)     2444 2023-04-27 01:40:40.000000 causalforge-0.0.6/README.md
+drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-05-01 23:41:36.441402 causalforge-0.0.6/causalforge/
+-rw-r--r--   0 AG62216    (501) staff       (20)       62 2023-05-01 23:40:20.000000 causalforge-0.0.6/causalforge/__init__.py
+drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-05-01 23:41:36.445576 causalforge-0.0.6/causalforge/tests/
+-rw-r--r--   0 AG62216    (501) staff       (20)        0 2023-04-22 02:11:58.000000 causalforge-0.0.6/causalforge/tests/__init__.py
+drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-05-01 23:41:36.444895 causalforge-0.0.6/causalforge.egg-info/
+-rw-r--r--   0 AG62216    (501) staff       (20)     2895 2023-05-01 23:41:36.000000 causalforge-0.0.6/causalforge.egg-info/PKG-INFO
+-rw-r--r--   0 AG62216    (501) staff       (20)      264 2023-05-01 23:41:36.000000 causalforge-0.0.6/causalforge.egg-info/SOURCES.txt
+-rw-r--r--   0 AG62216    (501) staff       (20)        1 2023-05-01 23:41:36.000000 causalforge-0.0.6/causalforge.egg-info/dependency_links.txt
+-rw-r--r--   0 AG62216    (501) staff       (20)      134 2023-05-01 23:41:36.000000 causalforge-0.0.6/causalforge.egg-info/requires.txt
+-rw-r--r--   0 AG62216    (501) staff       (20)       12 2023-05-01 23:41:36.000000 causalforge-0.0.6/causalforge.egg-info/top_level.txt
+-rw-r--r--   0 AG62216    (501) staff       (20)      102 2023-05-01 23:41:36.447001 causalforge-0.0.6/setup.cfg
+-rw-r--r--   0 AG62216    (501) staff       (20)     1659 2023-04-26 23:15:59.000000 causalforge-0.0.6/setup.py
```

### Comparing `causalforge-0.0.5/LICENSE` & `causalforge-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `causalforge-0.0.5/PKG-INFO` & `causalforge-0.0.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causalforge
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python Package for Causal Inference
 Home-page: https://github.com/anthem-ai/causalflow
 Author: Gino Tesei, Jey Kottalam
 Author-email: 
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
@@ -72,8 +72,21 @@
 ```bash
 cd tests
 pytest --disable-warnings 
 ```
 
 </details>
 
+## Citation
+
+```bibtex
+@article{tesei2023learning,
+  title={Learning end-to-end patient representations through self-supervised covariate balancing for causal treatment effect estimation},
+  author={Tesei, Gino and Giampanis, Stefanos and Shi, Jingpu and Norgeot, Beau},
+  journal={Journal of Biomedical Informatics},
+  volume={140},
+  pages={104339},
+  year={2023},
+  publisher={Elsevier}
+}
+```
```

### Comparing `causalforge-0.0.5/causalforge.egg-info/PKG-INFO` & `causalforge-0.0.6/causalforge.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causalforge
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python Package for Causal Inference
 Home-page: https://github.com/anthem-ai/causalflow
 Author: Gino Tesei, Jey Kottalam
 Author-email: 
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
@@ -72,8 +72,21 @@
 ```bash
 cd tests
 pytest --disable-warnings 
 ```
 
 </details>
 
+## Citation
+
+```bibtex
+@article{tesei2023learning,
+  title={Learning end-to-end patient representations through self-supervised covariate balancing for causal treatment effect estimation},
+  author={Tesei, Gino and Giampanis, Stefanos and Shi, Jingpu and Norgeot, Beau},
+  journal={Journal of Biomedical Informatics},
+  volume={140},
+  pages={104339},
+  year={2023},
+  publisher={Elsevier}
+}
+```
```

### Comparing `causalforge-0.0.5/setup.py` & `causalforge-0.0.6/setup.py`

 * *Files identical despite different names*

