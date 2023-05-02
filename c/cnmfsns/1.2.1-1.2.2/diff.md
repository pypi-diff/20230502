# Comparing `tmp/cnmfsns-1.2.1.tar.gz` & `tmp/cnmfsns-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnmfsns-1.2.1.tar", last modified: Tue May  2 18:38:23 2023, max compression
+gzip compressed data, was "cnmfsns-1.2.2.tar", last modified: Tue May  2 19:38:16 2023, max compression
```

## Comparing `cnmfsns-1.2.1.tar` & `cnmfsns-1.2.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 18:38:23.423009 cnmfsns-1.2.1/
--rw-rw-rw-   0        0        0     1090 2023-04-24 20:31:27.000000 cnmfsns-1.2.1/LICENSE
--rw-rw-rw-   0        0        0     3897 2023-05-02 18:38:23.423009 cnmfsns-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     3382 2023-05-02 18:34:45.000000 cnmfsns-1.2.1/README.md
--rw-rw-rw-   0        0        0       86 2023-04-24 20:31:27.000000 cnmfsns-1.2.1/pyproject.toml
--rw-rw-rw-   0        0        0      926 2023-05-02 18:38:23.423009 cnmfsns-1.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-02 18:38:23.375611 cnmfsns-1.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-02 18:38:23.407376 cnmfsns-1.2.1/src/cnmfsns/
--rw-rw-rw-   0        0        0     1570 2023-04-24 20:31:27.000000 cnmfsns-1.2.1/src/cnmfsns/__init__.py
--rw-rw-rw-   0        0        0    56210 2023-04-24 20:31:27.000000 cnmfsns-1.2.1/src/cnmfsns/cli.py
--rw-rw-rw-   0        0        0    46157 2023-04-24 20:31:27.000000 cnmfsns-1.2.1/src/cnmfsns/cnmf.py
--rw-rw-rw-   0        0        0    16061 2023-04-24 20:31:27.000000 cnmfsns-1.2.1/src/cnmfsns/colors.py
--rw-rw-rw-   0        0        0     3257 2023-04-24 20:31:27.000000 cnmfsns-1.2.1/src/cnmfsns/config.py
--rw-rw-rw-   0        0        0    24347 2023-05-02 18:34:53.000000 cnmfsns-1.2.1/src/cnmfsns/dataset.py
--rw-rw-rw-   0        0        0    13863 2023-05-02 18:34:54.000000 cnmfsns-1.2.1/src/cnmfsns/integration.py
--rw-rw-rw-   0        0        0    57568 2023-04-25 21:29:53.000000 cnmfsns-1.2.1/src/cnmfsns/plots.py
--rw-rw-rw-   0        0        0    23331 2023-04-25 17:52:38.000000 cnmfsns-1.2.1/src/cnmfsns/sns.py
--rw-rw-rw-   0        0        0     2767 2023-04-24 20:31:27.000000 cnmfsns-1.2.1/src/cnmfsns/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 18:38:23.423009 cnmfsns-1.2.1/src/cnmfsns.egg-info/
--rw-rw-rw-   0        0        0     3897 2023-05-02 18:38:23.000000 cnmfsns-1.2.1/src/cnmfsns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      472 2023-05-02 18:38:23.000000 cnmfsns-1.2.1/src/cnmfsns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 18:38:23.000000 cnmfsns-1.2.1/src/cnmfsns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-02 18:38:23.000000 cnmfsns-1.2.1/src/cnmfsns.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      145 2023-05-02 18:38:23.000000 cnmfsns-1.2.1/src/cnmfsns.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-02 18:38:23.000000 cnmfsns-1.2.1/src/cnmfsns.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 19:38:16.041359 cnmfsns-1.2.2/
+-rw-rw-rw-   0        0        0     1090 2023-04-24 20:31:27.000000 cnmfsns-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0     3897 2023-05-02 19:38:16.041359 cnmfsns-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3382 2023-05-02 19:36:59.000000 cnmfsns-1.2.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-24 20:31:27.000000 cnmfsns-1.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0      941 2023-05-02 19:38:16.041359 cnmfsns-1.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-02 19:38:15.987656 cnmfsns-1.2.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 19:38:16.018918 cnmfsns-1.2.2/src/cnmfsns/
+-rw-rw-rw-   0        0        0     1570 2023-04-24 20:31:27.000000 cnmfsns-1.2.2/src/cnmfsns/__init__.py
+-rw-rw-rw-   0        0        0    56210 2023-04-24 20:31:27.000000 cnmfsns-1.2.2/src/cnmfsns/cli.py
+-rw-rw-rw-   0        0        0    46157 2023-04-24 20:31:27.000000 cnmfsns-1.2.2/src/cnmfsns/cnmf.py
+-rw-rw-rw-   0        0        0    16061 2023-04-24 20:31:27.000000 cnmfsns-1.2.2/src/cnmfsns/colors.py
+-rw-rw-rw-   0        0        0     3257 2023-04-24 20:31:27.000000 cnmfsns-1.2.2/src/cnmfsns/config.py
+-rw-rw-rw-   0        0        0    24347 2023-05-02 18:34:53.000000 cnmfsns-1.2.2/src/cnmfsns/dataset.py
+-rw-rw-rw-   0        0        0    13863 2023-05-02 19:06:07.000000 cnmfsns-1.2.2/src/cnmfsns/integration.py
+-rw-rw-rw-   0        0        0    57568 2023-04-25 21:29:53.000000 cnmfsns-1.2.2/src/cnmfsns/plots.py
+-rw-rw-rw-   0        0        0    23331 2023-04-25 17:52:38.000000 cnmfsns-1.2.2/src/cnmfsns/sns.py
+-rw-rw-rw-   0        0        0     2767 2023-04-24 20:31:27.000000 cnmfsns-1.2.2/src/cnmfsns/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:38:16.041359 cnmfsns-1.2.2/src/cnmfsns.egg-info/
+-rw-rw-rw-   0        0        0     3897 2023-05-02 19:38:15.000000 cnmfsns-1.2.2/src/cnmfsns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      472 2023-05-02 19:38:15.000000 cnmfsns-1.2.2/src/cnmfsns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 19:38:15.000000 cnmfsns-1.2.2/src/cnmfsns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-02 19:38:15.000000 cnmfsns-1.2.2/src/cnmfsns.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      158 2023-05-02 19:38:15.000000 cnmfsns-1.2.2/src/cnmfsns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-02 19:38:15.000000 cnmfsns-1.2.2/src/cnmfsns.egg-info/top_level.txt
```

### Comparing `cnmfsns-1.2.1/LICENSE` & `cnmfsns-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.2.1/PKG-INFO` & `cnmfsns-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnmfsns
-Version: 1.2.1
+Version: 1.2.2
 Summary: cNMF Solution Network Space
 Home-page: https://github.com/MorrissyLab/cNMF-SNS
 Author: Ted Verhey
 Author-email: tbverhey@ucalgary.ca
 Project-URL: Bug Tracker, https://github.com/MorrissyLab/cNMF-SNS/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,15 @@
 
 ![cNMF-SNS logo](logo.png)
 
 -----------------
 
 # cNMF-SNS: powerful factorization-based multi-omics integration toolkit
 
-![version badge](https://img.shields.io/badge/version-1.2.1-blue)
+![version badge](https://img.shields.io/badge/version-1.2.2-blue)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/cnmfsns.svg)](https://pypi.org/project/cnmfsns/)
 [![Conda Latest Release](https://anaconda.org/conda-forge/cnmfsns/badges/version.svg)](https://anaconda.org/anaconda/cnmfsns/)
 [![Package Status](https://img.shields.io/pypi/status/cnmfsns.svg)](https://pypi.org/project/cnmfsns/)
 [![Downloads](https://static.pepy.tech/personalized-badge/cnmfsns?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/cnmfsns)
 [![License](https://img.shields.io/pypi/l/cnmfsns.svg)](https://github.com/MorrissyLab/cNMF-SNS/blob/main/LICENSE)
 <details>
   <summary> </summary>
```

### Comparing `cnmfsns-1.2.1/README.md` & `cnmfsns-1.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 00000040: 2070 6f77 6572 6675 6c20 6661 6374 6f72   powerful factor
 00000050: 697a 6174 696f 6e2d 6261 7365 6420 6d75  ization-based mu
 00000060: 6c74 692d 6f6d 6963 7320 696e 7465 6772  lti-omics integr
 00000070: 6174 696f 6e20 746f 6f6c 6b69 740d 0a0d  ation toolkit...
 00000080: 0a21 5b76 6572 7369 6f6e 2062 6164 6765  .![version badge
 00000090: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
 000000a0: 6965 6c64 732e 696f 2f62 6164 6765 2f76  ields.io/badge/v
-000000b0: 6572 7369 6f6e 2d31 2e32 2e31 2d62 6c75  ersion-1.2.1-blu
+000000b0: 6572 7369 6f6e 2d31 2e32 2e32 2d62 6c75  ersion-1.2.2-blu
 000000c0: 6529 0d0a 5b21 5b50 7950 4920 4c61 7465  e)..[![PyPI Late
 000000d0: 7374 2052 656c 6561 7365 5d28 6874 7470  st Release](http
 000000e0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
 000000f0: 696f 2f70 7970 692f 762f 636e 6d66 736e  io/pypi/v/cnmfsn
 00000100: 732e 7376 6729 5d28 6874 7470 733a 2f2f  s.svg)](https://
 00000110: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
 00000120: 2f63 6e6d 6673 6e73 2f29 0d0a 5b21 5b43  /cnmfsns/)..[![C
```

### Comparing `cnmfsns-1.2.1/setup.cfg` & `cnmfsns-1.2.2/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6e6d 6673 6e73 0d0a 7665 7273   = cnmfsns..vers
-00000020: 696f 6e20 3d20 312e 322e 310d 0a61 7574  ion = 1.2.1..aut
+00000020: 696f 6e20 3d20 312e 322e 320d 0a61 7574  ion = 1.2.2..aut
 00000030: 686f 7220 3d20 5465 6420 5665 7268 6579  hor = Ted Verhey
 00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000050: 2074 6276 6572 6865 7940 7563 616c 6761   tbverhey@ucalga
 00000060: 7279 2e63 610d 0a64 6573 6372 6970 7469  ry.ca..descripti
 00000070: 6f6e 203d 2063 4e4d 4620 536f 6c75 7469  on = cNMF Soluti
 00000080: 6f6e 204e 6574 776f 726b 2053 7061 6365  on Network Space
 00000090: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
@@ -40,19 +40,20 @@
 00000270: 746c 6962 0d0a 0975 7073 6574 706c 6f74  tlib...upsetplot
 00000280: 0d0a 0968 7474 706c 6962 320d 0a09 746f  ...httplib2...to
 00000290: 6d6c 690d 0a09 746f 6d6c 692d 770d 0a09  mli...tomli-w...
 000002a0: 6469 7374 696e 6374 6970 790d 0a09 636c  distinctipy...cl
 000002b0: 6963 6b0d 0a09 7079 6772 6170 6876 697a  ick...pygraphviz
 000002c0: 0d0a 0969 6772 6170 680d 0a09 7365 6d61  ...igraph...sema
 000002d0: 6e74 6963 5f76 6572 7369 6f6e 0d0a 0970  ntic_version...p
-000002e0: 7979 616d 6c0d 0a70 7974 686f 6e5f 7265  yyaml..python_re
-000002f0: 7175 6972 6573 203d 203e 3d33 2e39 0d0a  quires = >=3.9..
-00000300: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
-00000310: 6765 732e 6669 6e64 5d0d 0a77 6865 7265  ges.find]..where
-00000320: 203d 2073 7263 0d0a 0d0a 5b6f 7074 696f   = src....[optio
-00000330: 6e73 2e65 6e74 7279 5f70 6f69 6e74 735d  ns.entry_points]
-00000340: 0d0a 636f 6e73 6f6c 655f 7363 7269 7074  ..console_script
-00000350: 7320 3d20 0d0a 0963 6e6d 6673 6e73 203d  s = ...cnmfsns =
-00000360: 2063 6e6d 6673 6e73 2e63 6c69 3a63 6c69   cnmfsns.cli:cli
-00000370: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
-00000380: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
-00000390: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
+000002e0: 7979 616d 6c0d 0a09 7363 696b 6974 2d6c  yyaml...scikit-l
+000002f0: 6561 726e 0d0a 7079 7468 6f6e 5f72 6571  earn..python_req
+00000300: 7569 7265 7320 3d20 3e3d 332e 390d 0a0d  uires = >=3.9...
+00000310: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
+00000320: 6573 2e66 696e 645d 0d0a 7768 6572 6520  es.find]..where 
+00000330: 3d20 7372 630d 0a0d 0a5b 6f70 7469 6f6e  = src....[option
+00000340: 732e 656e 7472 795f 706f 696e 7473 5d0d  s.entry_points].
+00000350: 0a63 6f6e 736f 6c65 5f73 6372 6970 7473  .console_scripts
+00000360: 203d 200d 0a09 636e 6d66 736e 7320 3d20   = ...cnmfsns = 
+00000370: 636e 6d66 736e 732e 636c 693a 636c 690d  cnmfsns.cli:cli.
+00000380: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
+00000390: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
+000003a0: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
```

### Comparing `cnmfsns-1.2.1/src/cnmfsns/__init__.py` & `cnmfsns-1.2.2/src/cnmfsns/__init__.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.2.1/src/cnmfsns/cli.py` & `cnmfsns-1.2.2/src/cnmfsns/cli.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.2.1/src/cnmfsns/cnmf.py` & `cnmfsns-1.2.2/src/cnmfsns/cnmf.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.2.1/src/cnmfsns/colors.py` & `cnmfsns-1.2.2/src/cnmfsns/colors.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.2.1/src/cnmfsns/config.py` & `cnmfsns-1.2.2/src/cnmfsns/config.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.2.1/src/cnmfsns/dataset.py` & `cnmfsns-1.2.2/src/cnmfsns/dataset.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.2.1/src/cnmfsns/integration.py` & `cnmfsns-1.2.2/src/cnmfsns/integration.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.2.1/src/cnmfsns/plots.py` & `cnmfsns-1.2.2/src/cnmfsns/plots.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.2.1/src/cnmfsns/sns.py` & `cnmfsns-1.2.2/src/cnmfsns/sns.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.2.1/src/cnmfsns/utils.py` & `cnmfsns-1.2.2/src/cnmfsns/utils.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.2.1/src/cnmfsns.egg-info/PKG-INFO` & `cnmfsns-1.2.2/src/cnmfsns.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnmfsns
-Version: 1.2.1
+Version: 1.2.2
 Summary: cNMF Solution Network Space
 Home-page: https://github.com/MorrissyLab/cNMF-SNS
 Author: Ted Verhey
 Author-email: tbverhey@ucalgary.ca
 Project-URL: Bug Tracker, https://github.com/MorrissyLab/cNMF-SNS/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,15 @@
 
 ![cNMF-SNS logo](logo.png)
 
 -----------------
 
 # cNMF-SNS: powerful factorization-based multi-omics integration toolkit
 
-![version badge](https://img.shields.io/badge/version-1.2.1-blue)
+![version badge](https://img.shields.io/badge/version-1.2.2-blue)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/cnmfsns.svg)](https://pypi.org/project/cnmfsns/)
 [![Conda Latest Release](https://anaconda.org/conda-forge/cnmfsns/badges/version.svg)](https://anaconda.org/anaconda/cnmfsns/)
 [![Package Status](https://img.shields.io/pypi/status/cnmfsns.svg)](https://pypi.org/project/cnmfsns/)
 [![Downloads](https://static.pepy.tech/personalized-badge/cnmfsns?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/cnmfsns)
 [![License](https://img.shields.io/pypi/l/cnmfsns.svg)](https://github.com/MorrissyLab/cNMF-SNS/blob/main/LICENSE)
 <details>
   <summary> </summary>
```

