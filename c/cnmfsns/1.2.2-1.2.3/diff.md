# Comparing `tmp/cnmfsns-1.2.2.tar.gz` & `tmp/cnmfsns-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnmfsns-1.2.2.tar", last modified: Tue May  2 19:38:16 2023, max compression
+gzip compressed data, was "cnmfsns-1.2.3.tar", last modified: Tue May  2 20:25:20 2023, max compression
```

## Comparing `cnmfsns-1.2.2.tar` & `cnmfsns-1.2.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 19:38:16.041359 cnmfsns-1.2.2/
--rw-rw-rw-   0        0        0     1090 2023-04-24 20:31:27.000000 cnmfsns-1.2.2/LICENSE
--rw-rw-rw-   0        0        0     3897 2023-05-02 19:38:16.041359 cnmfsns-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     3382 2023-05-02 19:36:59.000000 cnmfsns-1.2.2/README.md
--rw-rw-rw-   0        0        0       86 2023-04-24 20:31:27.000000 cnmfsns-1.2.2/pyproject.toml
--rw-rw-rw-   0        0        0      941 2023-05-02 19:38:16.041359 cnmfsns-1.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-02 19:38:15.987656 cnmfsns-1.2.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-02 19:38:16.018918 cnmfsns-1.2.2/src/cnmfsns/
--rw-rw-rw-   0        0        0     1570 2023-04-24 20:31:27.000000 cnmfsns-1.2.2/src/cnmfsns/__init__.py
--rw-rw-rw-   0        0        0    56210 2023-04-24 20:31:27.000000 cnmfsns-1.2.2/src/cnmfsns/cli.py
--rw-rw-rw-   0        0        0    46157 2023-04-24 20:31:27.000000 cnmfsns-1.2.2/src/cnmfsns/cnmf.py
--rw-rw-rw-   0        0        0    16061 2023-04-24 20:31:27.000000 cnmfsns-1.2.2/src/cnmfsns/colors.py
--rw-rw-rw-   0        0        0     3257 2023-04-24 20:31:27.000000 cnmfsns-1.2.2/src/cnmfsns/config.py
--rw-rw-rw-   0        0        0    24347 2023-05-02 18:34:53.000000 cnmfsns-1.2.2/src/cnmfsns/dataset.py
--rw-rw-rw-   0        0        0    13863 2023-05-02 19:06:07.000000 cnmfsns-1.2.2/src/cnmfsns/integration.py
--rw-rw-rw-   0        0        0    57568 2023-04-25 21:29:53.000000 cnmfsns-1.2.2/src/cnmfsns/plots.py
--rw-rw-rw-   0        0        0    23331 2023-04-25 17:52:38.000000 cnmfsns-1.2.2/src/cnmfsns/sns.py
--rw-rw-rw-   0        0        0     2767 2023-04-24 20:31:27.000000 cnmfsns-1.2.2/src/cnmfsns/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 19:38:16.041359 cnmfsns-1.2.2/src/cnmfsns.egg-info/
--rw-rw-rw-   0        0        0     3897 2023-05-02 19:38:15.000000 cnmfsns-1.2.2/src/cnmfsns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      472 2023-05-02 19:38:15.000000 cnmfsns-1.2.2/src/cnmfsns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 19:38:15.000000 cnmfsns-1.2.2/src/cnmfsns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-02 19:38:15.000000 cnmfsns-1.2.2/src/cnmfsns.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      158 2023-05-02 19:38:15.000000 cnmfsns-1.2.2/src/cnmfsns.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-02 19:38:15.000000 cnmfsns-1.2.2/src/cnmfsns.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 20:25:20.484247 cnmfsns-1.2.3/
+-rw-rw-rw-   0        0        0     1090 2023-04-24 20:31:27.000000 cnmfsns-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0     3886 2023-05-02 20:25:20.484247 cnmfsns-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3371 2023-05-02 20:24:10.000000 cnmfsns-1.2.3/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-24 20:31:27.000000 cnmfsns-1.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0      964 2023-05-02 20:25:20.486246 cnmfsns-1.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-02 20:25:20.445261 cnmfsns-1.2.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 20:25:20.467244 cnmfsns-1.2.3/src/cnmfsns/
+-rw-rw-rw-   0        0        0     1570 2023-04-24 20:31:27.000000 cnmfsns-1.2.3/src/cnmfsns/__init__.py
+-rw-rw-rw-   0        0        0    56210 2023-04-24 20:31:27.000000 cnmfsns-1.2.3/src/cnmfsns/cli.py
+-rw-rw-rw-   0        0        0    46157 2023-04-24 20:31:27.000000 cnmfsns-1.2.3/src/cnmfsns/cnmf.py
+-rw-rw-rw-   0        0        0    16061 2023-04-24 20:31:27.000000 cnmfsns-1.2.3/src/cnmfsns/colors.py
+-rw-rw-rw-   0        0        0     3257 2023-04-24 20:31:27.000000 cnmfsns-1.2.3/src/cnmfsns/config.py
+-rw-rw-rw-   0        0        0    24347 2023-05-02 18:34:53.000000 cnmfsns-1.2.3/src/cnmfsns/dataset.py
+-rw-rw-rw-   0        0        0    13863 2023-05-02 19:06:07.000000 cnmfsns-1.2.3/src/cnmfsns/integration.py
+-rw-rw-rw-   0        0        0    57568 2023-04-25 21:29:53.000000 cnmfsns-1.2.3/src/cnmfsns/plots.py
+-rw-rw-rw-   0        0        0    23331 2023-04-25 17:52:38.000000 cnmfsns-1.2.3/src/cnmfsns/sns.py
+-rw-rw-rw-   0        0        0     2767 2023-04-24 20:31:27.000000 cnmfsns-1.2.3/src/cnmfsns/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 20:25:20.484247 cnmfsns-1.2.3/src/cnmfsns.egg-info/
+-rw-rw-rw-   0        0        0     3886 2023-05-02 20:25:20.000000 cnmfsns-1.2.3/src/cnmfsns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      472 2023-05-02 20:25:20.000000 cnmfsns-1.2.3/src/cnmfsns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 20:25:20.000000 cnmfsns-1.2.3/src/cnmfsns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-02 20:25:20.000000 cnmfsns-1.2.3/src/cnmfsns.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      177 2023-05-02 20:25:20.000000 cnmfsns-1.2.3/src/cnmfsns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-02 20:25:20.000000 cnmfsns-1.2.3/src/cnmfsns.egg-info/top_level.txt
```

### Comparing `cnmfsns-1.2.2/LICENSE` & `cnmfsns-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.2.2/PKG-INFO` & `cnmfsns-1.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnmfsns
-Version: 1.2.2
+Version: 1.2.3
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
 
-![version badge](https://img.shields.io/badge/version-1.2.2-blue)
+![version badge](https://img.shields.io/badge/version-1.2.3-blue)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/cnmfsns.svg)](https://pypi.org/project/cnmfsns/)
 [![Conda Latest Release](https://anaconda.org/conda-forge/cnmfsns/badges/version.svg)](https://anaconda.org/anaconda/cnmfsns/)
 [![Package Status](https://img.shields.io/pypi/status/cnmfsns.svg)](https://pypi.org/project/cnmfsns/)
 [![Downloads](https://static.pepy.tech/personalized-badge/cnmfsns?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/cnmfsns)
 [![License](https://img.shields.io/pypi/l/cnmfsns.svg)](https://github.com/MorrissyLab/cNMF-SNS/blob/main/LICENSE)
 <details>
   <summary> </summary>
@@ -69,15 +69,15 @@
 ```
 
 ### ✨ Latest version from GitHub
 
 Before installing cNMF-SNS using pip, it is recommended to first set up a separate conda environment and have conda manage as many dependencies as possible.
 
 ```bash
-conda create --name cnmfsns -c conda-forge python=3.10 anndata pandas numpy scipy matplotlib upsetplot httplib2 tomli tomli-w click pygraphviz python-igraph semantic_version yaml scikit-learn fastcluster scanpy pyyaml gseapy=1.0.3
+conda create --name cnmfsns -c conda-forge python=3.10 anndata pandas numpy scipy matplotlib upsetplot httplib2 tomli tomli-w click pygraphviz python-igraph semantic_version pyyaml scikit-learn fastcluster scanpy pyyaml
 conda activate cnmfsns
 pip install git+https://github.com/MorrissyLab/cNMF-SNS.git
 ```
 
 ## 📖 Documentation
 
 ### 📓 Python interface tutorial
```

### Comparing `cnmfsns-1.2.2/README.md` & `cnmfsns-1.2.3/README.md`

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
-000000b0: 6572 7369 6f6e 2d31 2e32 2e32 2d62 6c75  ersion-1.2.2-blu
+000000b0: 6572 7369 6f6e 2d31 2e32 2e33 2d62 6c75  ersion-1.2.3-blu
 000000c0: 6529 0d0a 5b21 5b50 7950 4920 4c61 7465  e)..[![PyPI Late
 000000d0: 7374 2052 656c 6561 7365 5d28 6874 7470  st Release](http
 000000e0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
 000000f0: 696f 2f70 7970 692f 762f 636e 6d66 736e  io/pypi/v/cnmfsn
 00000100: 732e 7376 6729 5d28 6874 7470 733a 2f2f  s.svg)](https://
 00000110: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
 00000120: 2f63 6e6d 6673 6e73 2f29 0d0a 5b21 5b43  /cnmfsns/)..[![C
@@ -168,45 +168,44 @@
 00000a70: 3020 616e 6e64 6174 6120 7061 6e64 6173  0 anndata pandas
 00000a80: 206e 756d 7079 2073 6369 7079 206d 6174   numpy scipy mat
 00000a90: 706c 6f74 6c69 6220 7570 7365 7470 6c6f  plotlib upsetplo
 00000aa0: 7420 6874 7470 6c69 6232 2074 6f6d 6c69  t httplib2 tomli
 00000ab0: 2074 6f6d 6c69 2d77 2063 6c69 636b 2070   tomli-w click p
 00000ac0: 7967 7261 7068 7669 7a20 7079 7468 6f6e  ygraphviz python
 00000ad0: 2d69 6772 6170 6820 7365 6d61 6e74 6963  -igraph semantic
-00000ae0: 5f76 6572 7369 6f6e 2079 616d 6c20 7363  _version yaml sc
-00000af0: 696b 6974 2d6c 6561 726e 2066 6173 7463  ikit-learn fastc
-00000b00: 6c75 7374 6572 2073 6361 6e70 7920 7079  luster scanpy py
-00000b10: 7961 6d6c 2067 7365 6170 793d 312e 302e  yaml gseapy=1.0.
-00000b20: 330d 0a63 6f6e 6461 2061 6374 6976 6174  3..conda activat
-00000b30: 6520 636e 6d66 736e 730d 0a70 6970 2069  e cnmfsns..pip i
-00000b40: 6e73 7461 6c6c 2067 6974 2b68 7474 7073  nstall git+https
-00000b50: 3a2f 2f67 6974 6875 622e 636f 6d2f 4d6f  ://github.com/Mo
-00000b60: 7272 6973 7379 4c61 622f 634e 4d46 2d53  rrissyLab/cNMF-S
-00000b70: 4e53 2e67 6974 0d0a 6060 600d 0a0d 0a23  NS.git..```....#
-00000b80: 2320 f09f 9396 2044 6f63 756d 656e 7461  # .... Documenta
-00000b90: 7469 6f6e 0d0a 0d0a 2323 2320 f09f 9393  tion....### ....
-00000ba0: 2050 7974 686f 6e20 696e 7465 7266 6163   Python interfac
-00000bb0: 6520 7475 746f 7269 616c 0d0a 0d0a 546f  e tutorial....To
-00000bc0: 2067 6574 2073 7461 7274 6564 2c20 7361   get started, sa
-00000bd0: 6d70 6c65 2070 726f 7465 6f6d 6963 7320  mple proteomics 
-00000be0: 6461 7461 7365 7473 2061 6e64 2061 204a  datasets and a J
-00000bf0: 7570 7974 6572 206e 6f74 6562 6f6f 6b20  upyter notebook 
-00000c00: 7475 746f 7269 616c 2069 7320 6176 6169  tutorial is avai
-00000c10: 6c61 626c 6520 5b68 6572 655d 282f 7475  lable [here](/tu
-00000c20: 746f 7269 616c 292e 0d0a 0d0a 2323 2320  torial).....### 
-00000c30: e28c a8ef b88f 2043 6f6d 6d61 6e64 206c  ...... Command l
-00000c40: 696e 6520 696e 7465 7266 6163 650d 0a0d  ine interface...
-00000c50: 0a53 6565 2074 6865 205b 636f 6d6d 616e  .See the [comman
-00000c60: 6420 6c69 6e65 2069 6e74 6572 6661 6365  d line interface
-00000c70: 2064 6f63 756d 656e 7461 7469 6f6e 5d28   documentation](
-00000c80: 2f43 4c49 2e6d 6429 2e0d 0a0d 0a23 2320  /CLI.md).....## 
-00000c90: f09f 92ad 2047 6574 7469 6e67 2048 656c  .... Getting Hel
-00000ca0: 700d 0a0d 0a46 6f72 2065 7272 6f72 7320  p....For errors 
-00000cb0: 6172 6973 696e 6720 6475 7269 6e67 2075  arising during u
-00000cc0: 7365 206f 6620 634e 4d46 2d53 4e53 2c20  se of cNMF-SNS, 
-00000cd0: 6372 6561 7465 2061 6e64 2062 726f 7773  create and brows
-00000ce0: 6520 6973 7375 6573 2069 6e20 7468 6520  e issues in the 
-00000cf0: 5b47 6974 4875 6220 2269 7373 7565 7322  [GitHub "issues"
-00000d00: 2074 6162 5d28 6874 7470 733a 2f2f 6769   tab](https://gi
-00000d10: 7468 7562 2e63 6f6d 2f4d 6f72 7269 7373  thub.com/Morriss
-00000d20: 794c 6162 2f63 4e4d 462d 534e 532f 6973  yLab/cNMF-SNS/is
-00000d30: 7375 6573 292e                           sues).
+00000ae0: 5f76 6572 7369 6f6e 2070 7979 616d 6c20  _version pyyaml 
+00000af0: 7363 696b 6974 2d6c 6561 726e 2066 6173  scikit-learn fas
+00000b00: 7463 6c75 7374 6572 2073 6361 6e70 7920  tcluster scanpy 
+00000b10: 7079 7961 6d6c 0d0a 636f 6e64 6120 6163  pyyaml..conda ac
+00000b20: 7469 7661 7465 2063 6e6d 6673 6e73 0d0a  tivate cnmfsns..
+00000b30: 7069 7020 696e 7374 616c 6c20 6769 742b  pip install git+
+00000b40: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000b50: 6f6d 2f4d 6f72 7269 7373 794c 6162 2f63  om/MorrissyLab/c
+00000b60: 4e4d 462d 534e 532e 6769 740d 0a60 6060  NMF-SNS.git..```
+00000b70: 0d0a 0d0a 2323 20f0 9f93 9620 446f 6375  ....## .... Docu
+00000b80: 6d65 6e74 6174 696f 6e0d 0a0d 0a23 2323  mentation....###
+00000b90: 20f0 9f93 9320 5079 7468 6f6e 2069 6e74   .... Python int
+00000ba0: 6572 6661 6365 2074 7574 6f72 6961 6c0d  erface tutorial.
+00000bb0: 0a0d 0a54 6f20 6765 7420 7374 6172 7465  ...To get starte
+00000bc0: 642c 2073 616d 706c 6520 7072 6f74 656f  d, sample proteo
+00000bd0: 6d69 6373 2064 6174 6173 6574 7320 616e  mics datasets an
+00000be0: 6420 6120 4a75 7079 7465 7220 6e6f 7465  d a Jupyter note
+00000bf0: 626f 6f6b 2074 7574 6f72 6961 6c20 6973  book tutorial is
+00000c00: 2061 7661 696c 6162 6c65 205b 6865 7265   available [here
+00000c10: 5d28 2f74 7574 6f72 6961 6c29 2e0d 0a0d  ](/tutorial)....
+00000c20: 0a23 2323 20e2 8ca8 efb8 8f20 436f 6d6d  .### ...... Comm
+00000c30: 616e 6420 6c69 6e65 2069 6e74 6572 6661  and line interfa
+00000c40: 6365 0d0a 0d0a 5365 6520 7468 6520 5b63  ce....See the [c
+00000c50: 6f6d 6d61 6e64 206c 696e 6520 696e 7465  ommand line inte
+00000c60: 7266 6163 6520 646f 6375 6d65 6e74 6174  rface documentat
+00000c70: 696f 6e5d 282f 434c 492e 6d64 292e 0d0a  ion](/CLI.md)...
+00000c80: 0d0a 2323 20f0 9f92 ad20 4765 7474 696e  ..## .... Gettin
+00000c90: 6720 4865 6c70 0d0a 0d0a 466f 7220 6572  g Help....For er
+00000ca0: 726f 7273 2061 7269 7369 6e67 2064 7572  rors arising dur
+00000cb0: 696e 6720 7573 6520 6f66 2063 4e4d 462d  ing use of cNMF-
+00000cc0: 534e 532c 2063 7265 6174 6520 616e 6420  SNS, create and 
+00000cd0: 6272 6f77 7365 2069 7373 7565 7320 696e  browse issues in
+00000ce0: 2074 6865 205b 4769 7448 7562 2022 6973   the [GitHub "is
+00000cf0: 7375 6573 2220 7461 625d 2868 7474 7073  sues" tab](https
+00000d00: 3a2f 2f67 6974 6875 622e 636f 6d2f 4d6f  ://github.com/Mo
+00000d10: 7272 6973 7379 4c61 622f 634e 4d46 2d53  rrissyLab/cNMF-S
+00000d20: 4e53 2f69 7373 7565 7329 2e              NS/issues).
```

### Comparing `cnmfsns-1.2.2/setup.cfg` & `cnmfsns-1.2.3/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6e6d 6673 6e73 0d0a 7665 7273   = cnmfsns..vers
-00000020: 696f 6e20 3d20 312e 322e 320d 0a61 7574  ion = 1.2.2..aut
+00000020: 696f 6e20 3d20 312e 322e 330d 0a61 7574  ion = 1.2.3..aut
 00000030: 686f 7220 3d20 5465 6420 5665 7268 6579  hor = Ted Verhey
 00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000050: 2074 6276 6572 6865 7940 7563 616c 6761   tbverhey@ucalga
 00000060: 7279 2e63 610d 0a64 6573 6372 6970 7469  ry.ca..descripti
 00000070: 6f6e 203d 2063 4e4d 4620 536f 6c75 7469  on = cNMF Soluti
 00000080: 6f6e 204e 6574 776f 726b 2053 7061 6365  on Network Space
 00000090: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
@@ -41,19 +41,21 @@
 00000280: 0d0a 0968 7474 706c 6962 320d 0a09 746f  ...httplib2...to
 00000290: 6d6c 690d 0a09 746f 6d6c 692d 770d 0a09  mli...tomli-w...
 000002a0: 6469 7374 696e 6374 6970 790d 0a09 636c  distinctipy...cl
 000002b0: 6963 6b0d 0a09 7079 6772 6170 6876 697a  ick...pygraphviz
 000002c0: 0d0a 0969 6772 6170 680d 0a09 7365 6d61  ...igraph...sema
 000002d0: 6e74 6963 5f76 6572 7369 6f6e 0d0a 0970  ntic_version...p
 000002e0: 7979 616d 6c0d 0a09 7363 696b 6974 2d6c  yyaml...scikit-l
-000002f0: 6561 726e 0d0a 7079 7468 6f6e 5f72 6571  earn..python_req
-00000300: 7569 7265 7320 3d20 3e3d 332e 390d 0a0d  uires = >=3.9...
-00000310: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
-00000320: 6573 2e66 696e 645d 0d0a 7768 6572 6520  es.find]..where 
-00000330: 3d20 7372 630d 0a0d 0a5b 6f70 7469 6f6e  = src....[option
-00000340: 732e 656e 7472 795f 706f 696e 7473 5d0d  s.entry_points].
-00000350: 0a63 6f6e 736f 6c65 5f73 6372 6970 7473  .console_scripts
-00000360: 203d 200d 0a09 636e 6d66 736e 7320 3d20   = ...cnmfsns = 
-00000370: 636e 6d66 736e 732e 636c 693a 636c 690d  cnmfsns.cli:cli.
-00000380: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
-00000390: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
-000003a0: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
+000002f0: 6561 726e 0d0a 0966 6173 7463 6c75 7374  earn...fastclust
+00000300: 6572 0d0a 0973 6361 6e70 790d 0a70 7974  er...scanpy..pyt
+00000310: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
+00000320: 3d33 2e39 0d0a 0d0a 5b6f 7074 696f 6e73  =3.9....[options
+00000330: 2e70 6163 6b61 6765 732e 6669 6e64 5d0d  .packages.find].
+00000340: 0a77 6865 7265 203d 2073 7263 0d0a 0d0a  .where = src....
+00000350: 5b6f 7074 696f 6e73 2e65 6e74 7279 5f70  [options.entry_p
+00000360: 6f69 6e74 735d 0d0a 636f 6e73 6f6c 655f  oints]..console_
+00000370: 7363 7269 7074 7320 3d20 0d0a 0963 6e6d  scripts = ...cnm
+00000380: 6673 6e73 203d 2063 6e6d 6673 6e73 2e63  fsns = cnmfsns.c
+00000390: 6c69 3a63 6c69 0d0a 0d0a 5b65 6767 5f69  li:cli....[egg_i
+000003a0: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
+000003b0: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
+000003c0: 0d0a 0d0a                                ....
```

### Comparing `cnmfsns-1.2.2/src/cnmfsns/__init__.py` & `cnmfsns-1.2.3/src/cnmfsns/__init__.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.2.2/src/cnmfsns/cli.py` & `cnmfsns-1.2.3/src/cnmfsns/cli.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.2.2/src/cnmfsns/cnmf.py` & `cnmfsns-1.2.3/src/cnmfsns/cnmf.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.2.2/src/cnmfsns/colors.py` & `cnmfsns-1.2.3/src/cnmfsns/colors.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.2.2/src/cnmfsns/config.py` & `cnmfsns-1.2.3/src/cnmfsns/config.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.2.2/src/cnmfsns/dataset.py` & `cnmfsns-1.2.3/src/cnmfsns/dataset.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.2.2/src/cnmfsns/integration.py` & `cnmfsns-1.2.3/src/cnmfsns/integration.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.2.2/src/cnmfsns/plots.py` & `cnmfsns-1.2.3/src/cnmfsns/plots.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.2.2/src/cnmfsns/sns.py` & `cnmfsns-1.2.3/src/cnmfsns/sns.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.2.2/src/cnmfsns/utils.py` & `cnmfsns-1.2.3/src/cnmfsns/utils.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.2.2/src/cnmfsns.egg-info/PKG-INFO` & `cnmfsns-1.2.3/src/cnmfsns.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnmfsns
-Version: 1.2.2
+Version: 1.2.3
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
 
-![version badge](https://img.shields.io/badge/version-1.2.2-blue)
+![version badge](https://img.shields.io/badge/version-1.2.3-blue)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/cnmfsns.svg)](https://pypi.org/project/cnmfsns/)
 [![Conda Latest Release](https://anaconda.org/conda-forge/cnmfsns/badges/version.svg)](https://anaconda.org/anaconda/cnmfsns/)
 [![Package Status](https://img.shields.io/pypi/status/cnmfsns.svg)](https://pypi.org/project/cnmfsns/)
 [![Downloads](https://static.pepy.tech/personalized-badge/cnmfsns?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/cnmfsns)
 [![License](https://img.shields.io/pypi/l/cnmfsns.svg)](https://github.com/MorrissyLab/cNMF-SNS/blob/main/LICENSE)
 <details>
   <summary> </summary>
@@ -69,15 +69,15 @@
 ```
 
 ### ✨ Latest version from GitHub
 
 Before installing cNMF-SNS using pip, it is recommended to first set up a separate conda environment and have conda manage as many dependencies as possible.
 
 ```bash
-conda create --name cnmfsns -c conda-forge python=3.10 anndata pandas numpy scipy matplotlib upsetplot httplib2 tomli tomli-w click pygraphviz python-igraph semantic_version yaml scikit-learn fastcluster scanpy pyyaml gseapy=1.0.3
+conda create --name cnmfsns -c conda-forge python=3.10 anndata pandas numpy scipy matplotlib upsetplot httplib2 tomli tomli-w click pygraphviz python-igraph semantic_version pyyaml scikit-learn fastcluster scanpy pyyaml
 conda activate cnmfsns
 pip install git+https://github.com/MorrissyLab/cNMF-SNS.git
 ```
 
 ## 📖 Documentation
 
 ### 📓 Python interface tutorial
```

