# Comparing `tmp/cnmfsns-1.2.0.tar.gz` & `tmp/cnmfsns-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnmfsns-1.2.0.tar", last modified: Tue May  2 17:37:08 2023, max compression
+gzip compressed data, was "cnmfsns-1.2.1.tar", last modified: Tue May  2 18:38:23 2023, max compression
```

## Comparing `cnmfsns-1.2.0.tar` & `cnmfsns-1.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 17:37:08.635242 cnmfsns-1.2.0/
--rw-rw-rw-   0        0        0     1090 2023-04-24 20:31:27.000000 cnmfsns-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     3901 2023-05-02 17:37:08.636238 cnmfsns-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3386 2023-05-02 17:17:56.000000 cnmfsns-1.2.0/README.md
--rw-rw-rw-   0        0        0       86 2023-04-24 20:31:27.000000 cnmfsns-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      938 2023-05-02 17:37:08.637257 cnmfsns-1.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-02 17:37:08.581988 cnmfsns-1.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-02 17:37:08.610650 cnmfsns-1.2.0/src/cnmfsns/
--rw-rw-rw-   0        0        0     1570 2023-04-24 20:31:27.000000 cnmfsns-1.2.0/src/cnmfsns/__init__.py
--rw-rw-rw-   0        0        0    56210 2023-04-24 20:31:27.000000 cnmfsns-1.2.0/src/cnmfsns/cli.py
--rw-rw-rw-   0        0        0    46157 2023-04-24 20:31:27.000000 cnmfsns-1.2.0/src/cnmfsns/cnmf.py
--rw-rw-rw-   0        0        0    16061 2023-04-24 20:31:27.000000 cnmfsns-1.2.0/src/cnmfsns/colors.py
--rw-rw-rw-   0        0        0     3257 2023-04-24 20:31:27.000000 cnmfsns-1.2.0/src/cnmfsns/config.py
--rw-rw-rw-   0        0        0    24347 2023-05-01 22:10:41.000000 cnmfsns-1.2.0/src/cnmfsns/dataset.py
--rw-rw-rw-   0        0        0    13795 2023-04-25 16:36:26.000000 cnmfsns-1.2.0/src/cnmfsns/integration.py
--rw-rw-rw-   0        0        0    57568 2023-04-25 21:29:53.000000 cnmfsns-1.2.0/src/cnmfsns/plots.py
--rw-rw-rw-   0        0        0    23331 2023-04-25 17:52:38.000000 cnmfsns-1.2.0/src/cnmfsns/sns.py
--rw-rw-rw-   0        0        0     2767 2023-04-24 20:31:27.000000 cnmfsns-1.2.0/src/cnmfsns/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 17:37:08.634257 cnmfsns-1.2.0/src/cnmfsns.egg-info/
--rw-rw-rw-   0        0        0     3901 2023-05-02 17:37:08.000000 cnmfsns-1.2.0/src/cnmfsns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      472 2023-05-02 17:37:08.000000 cnmfsns-1.2.0/src/cnmfsns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 17:37:08.000000 cnmfsns-1.2.0/src/cnmfsns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-02 17:37:08.000000 cnmfsns-1.2.0/src/cnmfsns.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      155 2023-05-02 17:37:08.000000 cnmfsns-1.2.0/src/cnmfsns.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-02 17:37:08.000000 cnmfsns-1.2.0/src/cnmfsns.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 18:38:23.423009 cnmfsns-1.2.1/
+-rw-rw-rw-   0        0        0     1090 2023-04-24 20:31:27.000000 cnmfsns-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     3897 2023-05-02 18:38:23.423009 cnmfsns-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3382 2023-05-02 18:34:45.000000 cnmfsns-1.2.1/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-24 20:31:27.000000 cnmfsns-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0      926 2023-05-02 18:38:23.423009 cnmfsns-1.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-02 18:38:23.375611 cnmfsns-1.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 18:38:23.407376 cnmfsns-1.2.1/src/cnmfsns/
+-rw-rw-rw-   0        0        0     1570 2023-04-24 20:31:27.000000 cnmfsns-1.2.1/src/cnmfsns/__init__.py
+-rw-rw-rw-   0        0        0    56210 2023-04-24 20:31:27.000000 cnmfsns-1.2.1/src/cnmfsns/cli.py
+-rw-rw-rw-   0        0        0    46157 2023-04-24 20:31:27.000000 cnmfsns-1.2.1/src/cnmfsns/cnmf.py
+-rw-rw-rw-   0        0        0    16061 2023-04-24 20:31:27.000000 cnmfsns-1.2.1/src/cnmfsns/colors.py
+-rw-rw-rw-   0        0        0     3257 2023-04-24 20:31:27.000000 cnmfsns-1.2.1/src/cnmfsns/config.py
+-rw-rw-rw-   0        0        0    24347 2023-05-02 18:34:53.000000 cnmfsns-1.2.1/src/cnmfsns/dataset.py
+-rw-rw-rw-   0        0        0    13863 2023-05-02 18:34:54.000000 cnmfsns-1.2.1/src/cnmfsns/integration.py
+-rw-rw-rw-   0        0        0    57568 2023-04-25 21:29:53.000000 cnmfsns-1.2.1/src/cnmfsns/plots.py
+-rw-rw-rw-   0        0        0    23331 2023-04-25 17:52:38.000000 cnmfsns-1.2.1/src/cnmfsns/sns.py
+-rw-rw-rw-   0        0        0     2767 2023-04-24 20:31:27.000000 cnmfsns-1.2.1/src/cnmfsns/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:38:23.423009 cnmfsns-1.2.1/src/cnmfsns.egg-info/
+-rw-rw-rw-   0        0        0     3897 2023-05-02 18:38:23.000000 cnmfsns-1.2.1/src/cnmfsns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      472 2023-05-02 18:38:23.000000 cnmfsns-1.2.1/src/cnmfsns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 18:38:23.000000 cnmfsns-1.2.1/src/cnmfsns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-02 18:38:23.000000 cnmfsns-1.2.1/src/cnmfsns.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      145 2023-05-02 18:38:23.000000 cnmfsns-1.2.1/src/cnmfsns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-02 18:38:23.000000 cnmfsns-1.2.1/src/cnmfsns.egg-info/top_level.txt
```

### Comparing `cnmfsns-1.2.0/LICENSE` & `cnmfsns-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.2.0/PKG-INFO` & `cnmfsns-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnmfsns
-Version: 1.2.0
+Version: 1.2.1
 Summary: cNMF Solution Network Space
 Home-page: https://github.com/MorrissyLab/cNMF-SNS
 Author: Ted Verhey
 Author-email: tbverhey@ucalgary.ca
 Project-URL: Bug Tracker, https://github.com/MorrissyLab/cNMF-SNS/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,22 +16,20 @@
 
 ![cNMF-SNS logo](logo.png)
 
 -----------------
 
 # cNMF-SNS: powerful factorization-based multi-omics integration toolkit
 
-![version badge](https://img.shields.io/badge/version-1.2.0-blue)
+![version badge](https://img.shields.io/badge/version-1.2.1-blue)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/cnmfsns.svg)](https://pypi.org/project/cnmfsns/)
 [![Conda Latest Release](https://anaconda.org/conda-forge/cnmfsns/badges/version.svg)](https://anaconda.org/anaconda/cnmfsns/)
 [![Package Status](https://img.shields.io/pypi/status/cnmfsns.svg)](https://pypi.org/project/cnmfsns/)
 [![Downloads](https://static.pepy.tech/personalized-badge/cnmfsns?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/cnmfsns)
 [![License](https://img.shields.io/pypi/l/cnmfsns.svg)](https://github.com/MorrissyLab/cNMF-SNS/blob/main/LICENSE)
-
-
 <details>
   <summary> </summary>
 
 ```md
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3509134.svg)](https://doi.org/10.5281/zenodo.3509134)
```

### Comparing `cnmfsns-1.2.0/README.md` & `cnmfsns-1.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 00000040: 2070 6f77 6572 6675 6c20 6661 6374 6f72   powerful factor
 00000050: 697a 6174 696f 6e2d 6261 7365 6420 6d75  ization-based mu
 00000060: 6c74 692d 6f6d 6963 7320 696e 7465 6772  lti-omics integr
 00000070: 6174 696f 6e20 746f 6f6c 6b69 740d 0a0d  ation toolkit...
 00000080: 0a21 5b76 6572 7369 6f6e 2062 6164 6765  .![version badge
 00000090: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
 000000a0: 6965 6c64 732e 696f 2f62 6164 6765 2f76  ields.io/badge/v
-000000b0: 6572 7369 6f6e 2d31 2e32 2e30 2d62 6c75  ersion-1.2.0-blu
+000000b0: 6572 7369 6f6e 2d31 2e32 2e31 2d62 6c75  ersion-1.2.1-blu
 000000c0: 6529 0d0a 5b21 5b50 7950 4920 4c61 7465  e)..[![PyPI Late
 000000d0: 7374 2052 656c 6561 7365 5d28 6874 7470  st Release](http
 000000e0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
 000000f0: 696f 2f70 7970 692f 762f 636e 6d66 736e  io/pypi/v/cnmfsn
 00000100: 732e 7376 6729 5d28 6874 7470 733a 2f2f  s.svg)](https://
 00000110: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
 00000120: 2f63 6e6d 6673 6e73 2f29 0d0a 5b21 5b43  /cnmfsns/)..[![C
@@ -48,165 +48,165 @@
 000002f0: 0a5b 215b 4c69 6365 6e73 655d 2868 7474  .[![License](htt
 00000300: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
 00000310: 2e69 6f2f 7079 7069 2f6c 2f63 6e6d 6673  .io/pypi/l/cnmfs
 00000320: 6e73 2e73 7667 295d 2868 7474 7073 3a2f  ns.svg)](https:/
 00000330: 2f67 6974 6875 622e 636f 6d2f 4d6f 7272  /github.com/Morr
 00000340: 6973 7379 4c61 622f 634e 4d46 2d53 4e53  issyLab/cNMF-SNS
 00000350: 2f62 6c6f 622f 6d61 696e 2f4c 4943 454e  /blob/main/LICEN
-00000360: 5345 290d 0a0d 0a0d 0a3c 6465 7461 696c  SE)......<detail
-00000370: 733e 0d0a 2020 3c73 756d 6d61 7279 3e20  s>..  <summary> 
-00000380: 3c2f 7375 6d6d 6172 793e 0d0a 0d0a 6060  </summary>....``
-00000390: 606d 640d 0a0d 0a5b 215b 444f 495d 2868  `md....[![DOI](h
-000003a0: 7474 7073 3a2f 2f7a 656e 6f64 6f2e 6f72  ttps://zenodo.or
-000003b0: 672f 6261 6467 652f 444f 492f 3130 2e35  g/badge/DOI/10.5
-000003c0: 3238 312f 7a65 6e6f 646f 2e33 3530 3931  281/zenodo.35091
-000003d0: 3334 2e73 7667 295d 2868 7474 7073 3a2f  34.svg)](https:/
-000003e0: 2f64 6f69 2e6f 7267 2f31 302e 3532 3831  /doi.org/10.5281
-000003f0: 2f7a 656e 6f64 6f2e 3335 3039 3133 3429  /zenodo.3509134)
-00000400: 0d0a 0d0a 6060 600d 0a0d 0a3c 2f64 6574  ....```....</det
-00000410: 6169 6c73 3e0d 0a0d 0a2a 2a63 4e4d 462d  ails>....**cNMF-
-00000420: 534e 532a 2a20 2863 6f6e 7365 6e73 7573  SNS** (consensus
-00000430: 204e 6f6e 2d6e 6567 6174 6976 6520 4d61   Non-negative Ma
-00000440: 7472 6978 2046 6163 746f 7269 7a61 7469  trix Factorizati
-00000450: 6f6e 2053 6f6c 7574 696f 6e20 4e65 7477  on Solution Netw
-00000460: 6f72 6b20 5370 6163 6529 2069 7320 6120  ork Space) is a 
-00000470: 5079 7468 6f6e 2070 6163 6b61 6765 2065  Python package e
-00000480: 6e61 626c 696e 6720 696e 7465 6772 6174  nabling integrat
-00000490: 696f 6e20 6f66 2062 756c 6b2c 2073 696e  ion of bulk, sin
-000004a0: 676c 652d 6365 6c6c 2c20 616e 640d 0a73  gle-cell, and..s
-000004b0: 7061 7469 616c 2065 7870 7265 7373 696f  patial expressio
-000004c0: 6e20 6461 7461 2062 6574 7765 656e 2061  n data between a
-000004d0: 6e64 2077 6974 6869 6e20 6461 7461 7365  nd within datase
-000004e0: 7473 2e20 634e 4d46 2070 726f 7669 6465  ts. cNMF provide
-000004f0: 7320 6120 2a2a 726f 6275 7374 2c20 0d0a  s a **robust, ..
-00000500: 756e 7375 7065 7276 6973 6564 2a2a 2064  unsupervised** d
-00000510: 6563 6f6e 766f 6c75 7469 6f6e 206f 6620  econvolution of 
-00000520: 6561 6368 2064 6174 6173 6574 2069 6e74  each dataset int
-00000530: 6f20 6765 6e65 2065 7870 7265 7373 696f  o gene expressio
-00000540: 6e20 7072 6f67 7261 6d73 2028 4745 5073  n programs (GEPs
-00000550: 292e 0d0a 2a2a 4e65 7477 6f72 6b2d 6261  )...**Network-ba
-00000560: 7365 6420 696e 7465 6772 6174 696f 6e2a  sed integration*
-00000570: 2a20 6f66 2047 4550 7320 656e 6162 6c65  * of GEPs enable
-00000580: 7320 666c 6578 6962 6c65 2069 6e74 6567  s flexible integ
-00000590: 7261 7469 6f6e 206f 6620 6d61 6e79 2064  ration of many d
-000005a0: 6174 6173 6574 730d 0a61 6372 6f73 7320  atasets..across 
-000005b0: 6173 7361 7973 2028 6567 2e20 5072 6f74  assays (eg. Prot
-000005c0: 6569 6e2c 2052 4e41 2d53 6571 2920 616e  ein, RNA-Seq) an
-000005d0: 6420 7061 7469 656e 7420 636f 686f 7274  d patient cohort
-000005e0: 732e 0d0a 0d0a 436f 6d6d 756e 6974 6965  s.....Communitie
-000005f0: 7320 7769 7468 2047 4550 7320 6672 6f6d  s with GEPs from
-00000600: 206d 756c 7469 706c 6520 6461 7461 7365   multiple datase
-00000610: 7473 2063 616e 2062 6520 616e 6e6f 7461  ts can be annota
-00000620: 7465 6420 7769 7468 2064 6174 6173 6574  ted with dataset
-00000630: 2d73 7065 6369 6669 630d 0a61 6e6e 6f74  -specific..annot
-00000640: 6174 696f 6e73 2074 6f20 6661 6369 6c69  ations to facili
-00000650: 7461 7465 2069 6e74 6572 7072 6574 6174  tate interpretat
-00000660: 696f 6e2e 0d0a 0d0a 2323 20e2 9aa1 4d61  ion.....## ...Ma
-00000670: 696e 2046 6561 7475 7265 730d 0a0d 0a48  in Features....H
-00000680: 6572 6520 6172 6520 6a75 7374 2061 2066  ere are just a f
-00000690: 6577 206f 6620 7468 6520 7468 696e 6773  ew of the things
-000006a0: 2074 6861 7420 634e 4d46 2d53 4e53 2064   that cNMF-SNS d
-000006b0: 6f65 7320 7765 6c6c 3a0d 0a0d 0a2d 2049  oes well:....- I
-000006c0: 6e74 6567 7261 7469 6f6e 206f 6620 6578  ntegration of ex
-000006d0: 7072 6573 7369 6f6e 2064 6174 6120 646f  pression data do
-000006e0: 6573 206e 6f74 2072 6571 7569 7265 2073  es not require s
-000006f0: 7562 7365 7474 696e 6720 6665 6174 7572  ubsetting featur
-00000700: 6573 2f67 656e 6573 2074 6f0d 0a20 2061  es/genes to..  a
-00000710: 2073 6861 7265 6420 6f72 2027 6f76 6572   shared or 'over
-00000720: 6469 7370 6572 7365 6427 2073 7562 7365  dispersed' subse
-00000730: 740d 0a2d 2049 6465 616c 2066 6f72 2069  t..- Ideal for i
-00000740: 6e63 7265 6d65 6e74 616c 2069 6e74 6567  ncremental integ
-00000750: 7261 7469 6f6e 2028 6164 6469 6e67 2064  ration (adding d
-00000760: 6174 6173 6574 7320 6f6e 6520 6174 2061  atasets one at a
-00000770: 2074 696d 6529 2073 696e 6365 0d0a 2020   time) since..  
-00000780: 6465 636f 6e76 6f6c 7574 696f 6e20 6973  deconvolution is
-00000790: 2070 6572 666f 726d 6564 2069 6e64 6570   performed indep
-000007a0: 656e 6465 6e74 6c79 206f 6e20 6561 6368  endently on each
-000007b0: 2064 6174 6173 6574 2067 656e 6572 6174   dataset generat
-000007c0: 696e 6720 696e 7661 7269 616e 7420 4745  ing invariant GE
-000007d0: 5073 0d0a 2d20 446f 6573 206e 6f74 2061  Ps..- Does not a
-000007e0: 7373 756d 6520 7468 6520 7361 6d65 206c  ssume the same l
-000007f0: 6576 656c 206f 6620 7370 6172 7369 7479  evel of sparsity
-00000800: 2f64 6570 7468 2028 7369 6e67 6c65 2d63  /depth (single-c
-00000810: 656c 6c2c 2062 756c 6b29 0d0a 2d20 4964  ell, bulk)..- Id
-00000820: 656e 7469 6669 6573 2069 6e74 6572 7072  entifies interpr
-00000830: 6574 6162 6c65 2c20 6164 6469 7469 7665  etable, additive
-00000840: 206e 6f6e 2d6e 6567 6174 6976 6520 6765   non-negative ge
-00000850: 6e65 2065 7870 7265 7373 696f 6e20 7072  ne expression pr
-00000860: 6f67 7261 6d73 0d0a 2d20 5477 6f20 696e  ograms..- Two in
-00000870: 7465 7266 6163 6573 3a20 636f 6d6d 616e  terfaces: comman
-00000880: 642d 6c69 6e65 2069 6e74 6572 6661 6365  d-line interface
-00000890: 2066 6f72 2072 6170 6964 2064 6174 6120   for rapid data 
-000008a0: 6578 706c 6f72 6174 696f 6e20 616e 6420  exploration and 
-000008b0: 7079 7468 6f6e 0d0a 2020 696e 7465 7266  python..  interf
-000008c0: 6163 6520 666f 7220 6578 7465 6e73 6962  ace for extensib
-000008d0: 696c 6974 7920 616e 6420 666c 6578 6962  ility and flexib
-000008e0: 696c 6974 790d 0a0d 0a23 2320 f09f 94a7  ility....## ....
-000008f0: 2049 6e73 7461 6c6c 0d0a 0d0a 2323 2320   Install....### 
-00000900: e298 81ef b88f 2050 7562 6c69 6320 5265  ...... Public Re
-00000910: 6c65 6173 650d 0a0d 0a49 6e73 7461 6c6c  lease....Install
-00000920: 2074 6865 2070 6163 6b61 6765 2077 6974   the package wit
-00000930: 6820 636f 6e64 613a 0d0a 6060 6062 6173  h conda:..```bas
-00000940: 680d 0a63 6f6e 6461 2069 6e73 7461 6c6c  h..conda install
-00000950: 202d 6320 636f 6e64 612d 666f 7267 6520   -c conda-forge 
-00000960: 636e 6d66 736e 730d 0a60 6060 0d0a 0d0a  cnmfsns..```....
-00000970: 2323 2320 e29c a820 4c61 7465 7374 2076  ### ... Latest v
-00000980: 6572 7369 6f6e 2066 726f 6d20 4769 7448  ersion from GitH
-00000990: 7562 0d0a 0d0a 4265 666f 7265 2069 6e73  ub....Before ins
-000009a0: 7461 6c6c 696e 6720 634e 4d46 2d53 4e53  talling cNMF-SNS
-000009b0: 2075 7369 6e67 2070 6970 2c20 6974 2069   using pip, it i
-000009c0: 7320 7265 636f 6d6d 656e 6465 6420 746f  s recommended to
-000009d0: 2066 6972 7374 2073 6574 2075 7020 6120   first set up a 
-000009e0: 7365 7061 7261 7465 2063 6f6e 6461 2065  separate conda e
-000009f0: 6e76 6972 6f6e 6d65 6e74 2061 6e64 2068  nvironment and h
-00000a00: 6176 6520 636f 6e64 6120 6d61 6e61 6765  ave conda manage
-00000a10: 2061 7320 6d61 6e79 2064 6570 656e 6465   as many depende
-00000a20: 6e63 6965 7320 6173 2070 6f73 7369 626c  ncies as possibl
-00000a30: 652e 0d0a 0d0a 6060 6062 6173 680d 0a63  e.....```bash..c
-00000a40: 6f6e 6461 2063 7265 6174 6520 2d2d 6e61  onda create --na
-00000a50: 6d65 2063 6e6d 6673 6e73 202d 6320 636f  me cnmfsns -c co
-00000a60: 6e64 612d 666f 7267 6520 7079 7468 6f6e  nda-forge python
-00000a70: 3d33 2e31 3020 616e 6e64 6174 6120 7061  =3.10 anndata pa
-00000a80: 6e64 6173 206e 756d 7079 2073 6369 7079  ndas numpy scipy
-00000a90: 206d 6174 706c 6f74 6c69 6220 7570 7365   matplotlib upse
-00000aa0: 7470 6c6f 7420 6874 7470 6c69 6232 2074  tplot httplib2 t
-00000ab0: 6f6d 6c69 2074 6f6d 6c69 2d77 2063 6c69  omli tomli-w cli
-00000ac0: 636b 2070 7967 7261 7068 7669 7a20 7079  ck pygraphviz py
-00000ad0: 7468 6f6e 2d69 6772 6170 6820 7365 6d61  thon-igraph sema
-00000ae0: 6e74 6963 5f76 6572 7369 6f6e 2079 616d  ntic_version yam
-00000af0: 6c20 7363 696b 6974 2d6c 6561 726e 2066  l scikit-learn f
-00000b00: 6173 7463 6c75 7374 6572 2073 6361 6e70  astcluster scanp
-00000b10: 7920 7079 7961 6d6c 2067 7365 6170 793d  y pyyaml gseapy=
-00000b20: 312e 302e 330d 0a63 6f6e 6461 2061 6374  1.0.3..conda act
-00000b30: 6976 6174 6520 636e 6d66 736e 730d 0a70  ivate cnmfsns..p
-00000b40: 6970 2069 6e73 7461 6c6c 2067 6974 2b68  ip install git+h
-00000b50: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000b60: 6d2f 4d6f 7272 6973 7379 4c61 622f 634e  m/MorrissyLab/cN
-00000b70: 4d46 2d53 4e53 2e67 6974 0d0a 6060 600d  MF-SNS.git..```.
-00000b80: 0a0d 0a23 2320 f09f 9396 2044 6f63 756d  ...## .... Docum
-00000b90: 656e 7461 7469 6f6e 0d0a 0d0a 2323 2320  entation....### 
-00000ba0: f09f 9393 2050 7974 686f 6e20 696e 7465  .... Python inte
-00000bb0: 7266 6163 6520 7475 746f 7269 616c 0d0a  rface tutorial..
-00000bc0: 0d0a 546f 2067 6574 2073 7461 7274 6564  ..To get started
-00000bd0: 2c20 7361 6d70 6c65 2070 726f 7465 6f6d  , sample proteom
-00000be0: 6963 7320 6461 7461 7365 7473 2061 6e64  ics datasets and
-00000bf0: 2061 204a 7570 7974 6572 206e 6f74 6562   a Jupyter noteb
-00000c00: 6f6f 6b20 7475 746f 7269 616c 2069 7320  ook tutorial is 
-00000c10: 6176 6169 6c61 626c 6520 5b68 6572 655d  available [here]
-00000c20: 282f 7475 746f 7269 616c 292e 0d0a 0d0a  (/tutorial).....
-00000c30: 2323 2320 e28c a8ef b88f 2043 6f6d 6d61  ### ...... Comma
-00000c40: 6e64 206c 696e 6520 696e 7465 7266 6163  nd line interfac
-00000c50: 650d 0a0d 0a53 6565 2074 6865 205b 636f  e....See the [co
-00000c60: 6d6d 616e 6420 6c69 6e65 2069 6e74 6572  mmand line inter
-00000c70: 6661 6365 2064 6f63 756d 656e 7461 7469  face documentati
-00000c80: 6f6e 5d28 2f43 4c49 2e6d 6429 2e0d 0a0d  on](/CLI.md)....
-00000c90: 0a23 2320 f09f 92ad 2047 6574 7469 6e67  .## .... Getting
-00000ca0: 2048 656c 700d 0a0d 0a46 6f72 2065 7272   Help....For err
-00000cb0: 6f72 7320 6172 6973 696e 6720 6475 7269  ors arising duri
-00000cc0: 6e67 2075 7365 206f 6620 634e 4d46 2d53  ng use of cNMF-S
-00000cd0: 4e53 2c20 6372 6561 7465 2061 6e64 2062  NS, create and b
-00000ce0: 726f 7773 6520 6973 7375 6573 2069 6e20  rowse issues in 
-00000cf0: 7468 6520 5b47 6974 4875 6220 2269 7373  the [GitHub "iss
-00000d00: 7565 7322 2074 6162 5d28 6874 7470 733a  ues" tab](https:
-00000d10: 2f2f 6769 7468 7562 2e63 6f6d 2f4d 6f72  //github.com/Mor
-00000d20: 7269 7373 794c 6162 2f63 4e4d 462d 534e  rissyLab/cNMF-SN
-00000d30: 532f 6973 7375 6573 292e                 S/issues).
+00000360: 5345 290d 0a3c 6465 7461 696c 733e 0d0a  SE)..<details>..
+00000370: 2020 3c73 756d 6d61 7279 3e20 3c2f 7375    <summary> </su
+00000380: 6d6d 6172 793e 0d0a 0d0a 6060 606d 640d  mmary>....```md.
+00000390: 0a0d 0a5b 215b 444f 495d 2868 7474 7073  ...[![DOI](https
+000003a0: 3a2f 2f7a 656e 6f64 6f2e 6f72 672f 6261  ://zenodo.org/ba
+000003b0: 6467 652f 444f 492f 3130 2e35 3238 312f  dge/DOI/10.5281/
+000003c0: 7a65 6e6f 646f 2e33 3530 3931 3334 2e73  zenodo.3509134.s
+000003d0: 7667 295d 2868 7474 7073 3a2f 2f64 6f69  vg)](https://doi
+000003e0: 2e6f 7267 2f31 302e 3532 3831 2f7a 656e  .org/10.5281/zen
+000003f0: 6f64 6f2e 3335 3039 3133 3429 0d0a 0d0a  odo.3509134)....
+00000400: 6060 600d 0a0d 0a3c 2f64 6574 6169 6c73  ```....</details
+00000410: 3e0d 0a0d 0a2a 2a63 4e4d 462d 534e 532a  >....**cNMF-SNS*
+00000420: 2a20 2863 6f6e 7365 6e73 7573 204e 6f6e  * (consensus Non
+00000430: 2d6e 6567 6174 6976 6520 4d61 7472 6978  -negative Matrix
+00000440: 2046 6163 746f 7269 7a61 7469 6f6e 2053   Factorization S
+00000450: 6f6c 7574 696f 6e20 4e65 7477 6f72 6b20  olution Network 
+00000460: 5370 6163 6529 2069 7320 6120 5079 7468  Space) is a Pyth
+00000470: 6f6e 2070 6163 6b61 6765 2065 6e61 626c  on package enabl
+00000480: 696e 6720 696e 7465 6772 6174 696f 6e20  ing integration 
+00000490: 6f66 2062 756c 6b2c 2073 696e 676c 652d  of bulk, single-
+000004a0: 6365 6c6c 2c20 616e 640d 0a73 7061 7469  cell, and..spati
+000004b0: 616c 2065 7870 7265 7373 696f 6e20 6461  al expression da
+000004c0: 7461 2062 6574 7765 656e 2061 6e64 2077  ta between and w
+000004d0: 6974 6869 6e20 6461 7461 7365 7473 2e20  ithin datasets. 
+000004e0: 634e 4d46 2070 726f 7669 6465 7320 6120  cNMF provides a 
+000004f0: 2a2a 726f 6275 7374 2c20 0d0a 756e 7375  **robust, ..unsu
+00000500: 7065 7276 6973 6564 2a2a 2064 6563 6f6e  pervised** decon
+00000510: 766f 6c75 7469 6f6e 206f 6620 6561 6368  volution of each
+00000520: 2064 6174 6173 6574 2069 6e74 6f20 6765   dataset into ge
+00000530: 6e65 2065 7870 7265 7373 696f 6e20 7072  ne expression pr
+00000540: 6f67 7261 6d73 2028 4745 5073 292e 0d0a  ograms (GEPs)...
+00000550: 2a2a 4e65 7477 6f72 6b2d 6261 7365 6420  **Network-based 
+00000560: 696e 7465 6772 6174 696f 6e2a 2a20 6f66  integration** of
+00000570: 2047 4550 7320 656e 6162 6c65 7320 666c   GEPs enables fl
+00000580: 6578 6962 6c65 2069 6e74 6567 7261 7469  exible integrati
+00000590: 6f6e 206f 6620 6d61 6e79 2064 6174 6173  on of many datas
+000005a0: 6574 730d 0a61 6372 6f73 7320 6173 7361  ets..across assa
+000005b0: 7973 2028 6567 2e20 5072 6f74 6569 6e2c  ys (eg. Protein,
+000005c0: 2052 4e41 2d53 6571 2920 616e 6420 7061   RNA-Seq) and pa
+000005d0: 7469 656e 7420 636f 686f 7274 732e 0d0a  tient cohorts...
+000005e0: 0d0a 436f 6d6d 756e 6974 6965 7320 7769  ..Communities wi
+000005f0: 7468 2047 4550 7320 6672 6f6d 206d 756c  th GEPs from mul
+00000600: 7469 706c 6520 6461 7461 7365 7473 2063  tiple datasets c
+00000610: 616e 2062 6520 616e 6e6f 7461 7465 6420  an be annotated 
+00000620: 7769 7468 2064 6174 6173 6574 2d73 7065  with dataset-spe
+00000630: 6369 6669 630d 0a61 6e6e 6f74 6174 696f  cific..annotatio
+00000640: 6e73 2074 6f20 6661 6369 6c69 7461 7465  ns to facilitate
+00000650: 2069 6e74 6572 7072 6574 6174 696f 6e2e   interpretation.
+00000660: 0d0a 0d0a 2323 20e2 9aa1 4d61 696e 2046  ....## ...Main F
+00000670: 6561 7475 7265 730d 0a0d 0a48 6572 6520  eatures....Here 
+00000680: 6172 6520 6a75 7374 2061 2066 6577 206f  are just a few o
+00000690: 6620 7468 6520 7468 696e 6773 2074 6861  f the things tha
+000006a0: 7420 634e 4d46 2d53 4e53 2064 6f65 7320  t cNMF-SNS does 
+000006b0: 7765 6c6c 3a0d 0a0d 0a2d 2049 6e74 6567  well:....- Integ
+000006c0: 7261 7469 6f6e 206f 6620 6578 7072 6573  ration of expres
+000006d0: 7369 6f6e 2064 6174 6120 646f 6573 206e  sion data does n
+000006e0: 6f74 2072 6571 7569 7265 2073 7562 7365  ot require subse
+000006f0: 7474 696e 6720 6665 6174 7572 6573 2f67  tting features/g
+00000700: 656e 6573 2074 6f0d 0a20 2061 2073 6861  enes to..  a sha
+00000710: 7265 6420 6f72 2027 6f76 6572 6469 7370  red or 'overdisp
+00000720: 6572 7365 6427 2073 7562 7365 740d 0a2d  ersed' subset..-
+00000730: 2049 6465 616c 2066 6f72 2069 6e63 7265   Ideal for incre
+00000740: 6d65 6e74 616c 2069 6e74 6567 7261 7469  mental integrati
+00000750: 6f6e 2028 6164 6469 6e67 2064 6174 6173  on (adding datas
+00000760: 6574 7320 6f6e 6520 6174 2061 2074 696d  ets one at a tim
+00000770: 6529 2073 696e 6365 0d0a 2020 6465 636f  e) since..  deco
+00000780: 6e76 6f6c 7574 696f 6e20 6973 2070 6572  nvolution is per
+00000790: 666f 726d 6564 2069 6e64 6570 656e 6465  formed independe
+000007a0: 6e74 6c79 206f 6e20 6561 6368 2064 6174  ntly on each dat
+000007b0: 6173 6574 2067 656e 6572 6174 696e 6720  aset generating 
+000007c0: 696e 7661 7269 616e 7420 4745 5073 0d0a  invariant GEPs..
+000007d0: 2d20 446f 6573 206e 6f74 2061 7373 756d  - Does not assum
+000007e0: 6520 7468 6520 7361 6d65 206c 6576 656c  e the same level
+000007f0: 206f 6620 7370 6172 7369 7479 2f64 6570   of sparsity/dep
+00000800: 7468 2028 7369 6e67 6c65 2d63 656c 6c2c  th (single-cell,
+00000810: 2062 756c 6b29 0d0a 2d20 4964 656e 7469   bulk)..- Identi
+00000820: 6669 6573 2069 6e74 6572 7072 6574 6162  fies interpretab
+00000830: 6c65 2c20 6164 6469 7469 7665 206e 6f6e  le, additive non
+00000840: 2d6e 6567 6174 6976 6520 6765 6e65 2065  -negative gene e
+00000850: 7870 7265 7373 696f 6e20 7072 6f67 7261  xpression progra
+00000860: 6d73 0d0a 2d20 5477 6f20 696e 7465 7266  ms..- Two interf
+00000870: 6163 6573 3a20 636f 6d6d 616e 642d 6c69  aces: command-li
+00000880: 6e65 2069 6e74 6572 6661 6365 2066 6f72  ne interface for
+00000890: 2072 6170 6964 2064 6174 6120 6578 706c   rapid data expl
+000008a0: 6f72 6174 696f 6e20 616e 6420 7079 7468  oration and pyth
+000008b0: 6f6e 0d0a 2020 696e 7465 7266 6163 6520  on..  interface 
+000008c0: 666f 7220 6578 7465 6e73 6962 696c 6974  for extensibilit
+000008d0: 7920 616e 6420 666c 6578 6962 696c 6974  y and flexibilit
+000008e0: 790d 0a0d 0a23 2320 f09f 94a7 2049 6e73  y....## .... Ins
+000008f0: 7461 6c6c 0d0a 0d0a 2323 2320 e298 81ef  tall....### ....
+00000900: b88f 2050 7562 6c69 6320 5265 6c65 6173  .. Public Releas
+00000910: 650d 0a0d 0a49 6e73 7461 6c6c 2074 6865  e....Install the
+00000920: 2070 6163 6b61 6765 2077 6974 6820 636f   package with co
+00000930: 6e64 613a 0d0a 6060 6062 6173 680d 0a63  nda:..```bash..c
+00000940: 6f6e 6461 2069 6e73 7461 6c6c 202d 6320  onda install -c 
+00000950: 636f 6e64 612d 666f 7267 6520 636e 6d66  conda-forge cnmf
+00000960: 736e 730d 0a60 6060 0d0a 0d0a 2323 2320  sns..```....### 
+00000970: e29c a820 4c61 7465 7374 2076 6572 7369  ... Latest versi
+00000980: 6f6e 2066 726f 6d20 4769 7448 7562 0d0a  on from GitHub..
+00000990: 0d0a 4265 666f 7265 2069 6e73 7461 6c6c  ..Before install
+000009a0: 696e 6720 634e 4d46 2d53 4e53 2075 7369  ing cNMF-SNS usi
+000009b0: 6e67 2070 6970 2c20 6974 2069 7320 7265  ng pip, it is re
+000009c0: 636f 6d6d 656e 6465 6420 746f 2066 6972  commended to fir
+000009d0: 7374 2073 6574 2075 7020 6120 7365 7061  st set up a sepa
+000009e0: 7261 7465 2063 6f6e 6461 2065 6e76 6972  rate conda envir
+000009f0: 6f6e 6d65 6e74 2061 6e64 2068 6176 6520  onment and have 
+00000a00: 636f 6e64 6120 6d61 6e61 6765 2061 7320  conda manage as 
+00000a10: 6d61 6e79 2064 6570 656e 6465 6e63 6965  many dependencie
+00000a20: 7320 6173 2070 6f73 7369 626c 652e 0d0a  s as possible...
+00000a30: 0d0a 6060 6062 6173 680d 0a63 6f6e 6461  ..```bash..conda
+00000a40: 2063 7265 6174 6520 2d2d 6e61 6d65 2063   create --name c
+00000a50: 6e6d 6673 6e73 202d 6320 636f 6e64 612d  nmfsns -c conda-
+00000a60: 666f 7267 6520 7079 7468 6f6e 3d33 2e31  forge python=3.1
+00000a70: 3020 616e 6e64 6174 6120 7061 6e64 6173  0 anndata pandas
+00000a80: 206e 756d 7079 2073 6369 7079 206d 6174   numpy scipy mat
+00000a90: 706c 6f74 6c69 6220 7570 7365 7470 6c6f  plotlib upsetplo
+00000aa0: 7420 6874 7470 6c69 6232 2074 6f6d 6c69  t httplib2 tomli
+00000ab0: 2074 6f6d 6c69 2d77 2063 6c69 636b 2070   tomli-w click p
+00000ac0: 7967 7261 7068 7669 7a20 7079 7468 6f6e  ygraphviz python
+00000ad0: 2d69 6772 6170 6820 7365 6d61 6e74 6963  -igraph semantic
+00000ae0: 5f76 6572 7369 6f6e 2079 616d 6c20 7363  _version yaml sc
+00000af0: 696b 6974 2d6c 6561 726e 2066 6173 7463  ikit-learn fastc
+00000b00: 6c75 7374 6572 2073 6361 6e70 7920 7079  luster scanpy py
+00000b10: 7961 6d6c 2067 7365 6170 793d 312e 302e  yaml gseapy=1.0.
+00000b20: 330d 0a63 6f6e 6461 2061 6374 6976 6174  3..conda activat
+00000b30: 6520 636e 6d66 736e 730d 0a70 6970 2069  e cnmfsns..pip i
+00000b40: 6e73 7461 6c6c 2067 6974 2b68 7474 7073  nstall git+https
+00000b50: 3a2f 2f67 6974 6875 622e 636f 6d2f 4d6f  ://github.com/Mo
+00000b60: 7272 6973 7379 4c61 622f 634e 4d46 2d53  rrissyLab/cNMF-S
+00000b70: 4e53 2e67 6974 0d0a 6060 600d 0a0d 0a23  NS.git..```....#
+00000b80: 2320 f09f 9396 2044 6f63 756d 656e 7461  # .... Documenta
+00000b90: 7469 6f6e 0d0a 0d0a 2323 2320 f09f 9393  tion....### ....
+00000ba0: 2050 7974 686f 6e20 696e 7465 7266 6163   Python interfac
+00000bb0: 6520 7475 746f 7269 616c 0d0a 0d0a 546f  e tutorial....To
+00000bc0: 2067 6574 2073 7461 7274 6564 2c20 7361   get started, sa
+00000bd0: 6d70 6c65 2070 726f 7465 6f6d 6963 7320  mple proteomics 
+00000be0: 6461 7461 7365 7473 2061 6e64 2061 204a  datasets and a J
+00000bf0: 7570 7974 6572 206e 6f74 6562 6f6f 6b20  upyter notebook 
+00000c00: 7475 746f 7269 616c 2069 7320 6176 6169  tutorial is avai
+00000c10: 6c61 626c 6520 5b68 6572 655d 282f 7475  lable [here](/tu
+00000c20: 746f 7269 616c 292e 0d0a 0d0a 2323 2320  torial).....### 
+00000c30: e28c a8ef b88f 2043 6f6d 6d61 6e64 206c  ...... Command l
+00000c40: 696e 6520 696e 7465 7266 6163 650d 0a0d  ine interface...
+00000c50: 0a53 6565 2074 6865 205b 636f 6d6d 616e  .See the [comman
+00000c60: 6420 6c69 6e65 2069 6e74 6572 6661 6365  d line interface
+00000c70: 2064 6f63 756d 656e 7461 7469 6f6e 5d28   documentation](
+00000c80: 2f43 4c49 2e6d 6429 2e0d 0a0d 0a23 2320  /CLI.md).....## 
+00000c90: f09f 92ad 2047 6574 7469 6e67 2048 656c  .... Getting Hel
+00000ca0: 700d 0a0d 0a46 6f72 2065 7272 6f72 7320  p....For errors 
+00000cb0: 6172 6973 696e 6720 6475 7269 6e67 2075  arising during u
+00000cc0: 7365 206f 6620 634e 4d46 2d53 4e53 2c20  se of cNMF-SNS, 
+00000cd0: 6372 6561 7465 2061 6e64 2062 726f 7773  create and brows
+00000ce0: 6520 6973 7375 6573 2069 6e20 7468 6520  e issues in the 
+00000cf0: 5b47 6974 4875 6220 2269 7373 7565 7322  [GitHub "issues"
+00000d00: 2074 6162 5d28 6874 7470 733a 2f2f 6769   tab](https://gi
+00000d10: 7468 7562 2e63 6f6d 2f4d 6f72 7269 7373  thub.com/Morriss
+00000d20: 794c 6162 2f63 4e4d 462d 534e 532f 6973  yLab/cNMF-SNS/is
+00000d30: 7375 6573 292e                           sues).
```

### Comparing `cnmfsns-1.2.0/setup.cfg` & `cnmfsns-1.2.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6e6d 6673 6e73 0d0a 7665 7273   = cnmfsns..vers
-00000020: 696f 6e20 3d20 312e 322e 300d 0a61 7574  ion = 1.2.0..aut
+00000020: 696f 6e20 3d20 312e 322e 310d 0a61 7574  ion = 1.2.1..aut
 00000030: 686f 7220 3d20 5465 6420 5665 7268 6579  hor = Ted Verhey
 00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000050: 2074 6276 6572 6865 7940 7563 616c 6761   tbverhey@ucalga
 00000060: 7279 2e63 610d 0a64 6573 6372 6970 7469  ry.ca..descripti
 00000070: 6f6e 203d 2063 4e4d 4620 536f 6c75 7469  on = cNMF Soluti
 00000080: 6f6e 204e 6574 776f 726b 2053 7061 6365  on Network Space
 00000090: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
@@ -36,24 +36,23 @@
 00000230: 3d20 0d0a 0961 6e6e 6461 7461 203e 3d20  = ...anndata >= 
 00000240: 302e 382e 300d 0a09 7061 6e64 6173 0d0a  0.8.0...pandas..
 00000250: 096e 756d 7079 0d0a 0973 6369 7079 203e  .numpy...scipy >
 00000260: 3d20 312e 392e 300d 0a09 6d61 7470 6c6f  = 1.9.0...matplo
 00000270: 746c 6962 0d0a 0975 7073 6574 706c 6f74  tlib...upsetplot
 00000280: 0d0a 0968 7474 706c 6962 320d 0a09 746f  ...httplib2...to
 00000290: 6d6c 690d 0a09 746f 6d6c 692d 770d 0a09  mli...tomli-w...
-000002a0: 6469 7374 696e 6374 6970 790d 0a09 6e61  distinctipy...na
-000002b0: 6e63 6f72 726d 700d 0a09 636c 6963 6b0d  ncorrmp...click.
-000002c0: 0a09 7079 6772 6170 6876 697a 0d0a 0969  ..pygraphviz...i
-000002d0: 6772 6170 680d 0a09 7365 6d61 6e74 6963  graph...semantic
-000002e0: 5f76 6572 7369 6f6e 0d0a 0970 7979 616d  _version...pyyam
-000002f0: 6c0d 0a70 7974 686f 6e5f 7265 7175 6972  l..python_requir
-00000300: 6573 203d 203e 3d33 2e39 0d0a 0d0a 5b6f  es = >=3.9....[o
-00000310: 7074 696f 6e73 2e70 6163 6b61 6765 732e  ptions.packages.
-00000320: 6669 6e64 5d0d 0a77 6865 7265 203d 2073  find]..where = s
-00000330: 7263 0d0a 0d0a 5b6f 7074 696f 6e73 2e65  rc....[options.e
-00000340: 6e74 7279 5f70 6f69 6e74 735d 0d0a 636f  ntry_points]..co
-00000350: 6e73 6f6c 655f 7363 7269 7074 7320 3d20  nsole_scripts = 
-00000360: 0d0a 0963 6e6d 6673 6e73 203d 2063 6e6d  ...cnmfsns = cnm
-00000370: 6673 6e73 2e63 6c69 3a63 6c69 0d0a 0d0a  fsns.cli:cli....
-00000380: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
-00000390: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
-000003a0: 7465 203d 2030 0d0a 0d0a                 te = 0....
+000002a0: 6469 7374 696e 6374 6970 790d 0a09 636c  distinctipy...cl
+000002b0: 6963 6b0d 0a09 7079 6772 6170 6876 697a  ick...pygraphviz
+000002c0: 0d0a 0969 6772 6170 680d 0a09 7365 6d61  ...igraph...sema
+000002d0: 6e74 6963 5f76 6572 7369 6f6e 0d0a 0970  ntic_version...p
+000002e0: 7979 616d 6c0d 0a70 7974 686f 6e5f 7265  yyaml..python_re
+000002f0: 7175 6972 6573 203d 203e 3d33 2e39 0d0a  quires = >=3.9..
+00000300: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
+00000310: 6765 732e 6669 6e64 5d0d 0a77 6865 7265  ges.find]..where
+00000320: 203d 2073 7263 0d0a 0d0a 5b6f 7074 696f   = src....[optio
+00000330: 6e73 2e65 6e74 7279 5f70 6f69 6e74 735d  ns.entry_points]
+00000340: 0d0a 636f 6e73 6f6c 655f 7363 7269 7074  ..console_script
+00000350: 7320 3d20 0d0a 0963 6e6d 6673 6e73 203d  s = ...cnmfsns =
+00000360: 2063 6e6d 6673 6e73 2e63 6c69 3a63 6c69   cnmfsns.cli:cli
+00000370: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
+00000380: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
+00000390: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
```

### Comparing `cnmfsns-1.2.0/src/cnmfsns/__init__.py` & `cnmfsns-1.2.1/src/cnmfsns/__init__.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.2.0/src/cnmfsns/cli.py` & `cnmfsns-1.2.1/src/cnmfsns/cli.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.2.0/src/cnmfsns/cnmf.py` & `cnmfsns-1.2.1/src/cnmfsns/cnmf.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.2.0/src/cnmfsns/colors.py` & `cnmfsns-1.2.1/src/cnmfsns/colors.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.2.0/src/cnmfsns/config.py` & `cnmfsns-1.2.1/src/cnmfsns/config.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.2.0/src/cnmfsns/dataset.py` & `cnmfsns-1.2.1/src/cnmfsns/dataset.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.2.0/src/cnmfsns/integration.py` & `cnmfsns-1.2.1/src/cnmfsns/integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         return usages
     
     def compute_corr(self, method="pearson", cpus=cpus_available):
         if method == "pearson":
             try:
                 from nancorrmp.nancorrmp import NaNCorrMp
             except ImportError:
-                logging.info(f"nancorrmp not installed. Calculating Pearson correlation matrix using 1 CPU.")
+                logging.info(f"nancorrmp not installed. To improve computation time, install using `pip install nancorrmp`. Calculating Pearson correlation matrix using 1 CPU.")
                 corr = self.get_geps().corr(method)
             else:
                 cpu_string = "all" if cpus == -1 else str(cpus)
                 logging.info(f"nancorrmp found. Calculating Pearson correlation matrix using {cpu_string} CPUs.")
                 corr = NaNCorrMp.calculate(self.get_geps(), n_jobs=cpus)
         elif method == "spearman":
             logging.info(f"Calculating Spearman correlation matrix using 1 CPU.")
```

### Comparing `cnmfsns-1.2.0/src/cnmfsns/plots.py` & `cnmfsns-1.2.1/src/cnmfsns/plots.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.2.0/src/cnmfsns/sns.py` & `cnmfsns-1.2.1/src/cnmfsns/sns.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.2.0/src/cnmfsns/utils.py` & `cnmfsns-1.2.1/src/cnmfsns/utils.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.2.0/src/cnmfsns.egg-info/PKG-INFO` & `cnmfsns-1.2.1/src/cnmfsns.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnmfsns
-Version: 1.2.0
+Version: 1.2.1
 Summary: cNMF Solution Network Space
 Home-page: https://github.com/MorrissyLab/cNMF-SNS
 Author: Ted Verhey
 Author-email: tbverhey@ucalgary.ca
 Project-URL: Bug Tracker, https://github.com/MorrissyLab/cNMF-SNS/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,22 +16,20 @@
 
 ![cNMF-SNS logo](logo.png)
 
 -----------------
 
 # cNMF-SNS: powerful factorization-based multi-omics integration toolkit
 
-![version badge](https://img.shields.io/badge/version-1.2.0-blue)
+![version badge](https://img.shields.io/badge/version-1.2.1-blue)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/cnmfsns.svg)](https://pypi.org/project/cnmfsns/)
 [![Conda Latest Release](https://anaconda.org/conda-forge/cnmfsns/badges/version.svg)](https://anaconda.org/anaconda/cnmfsns/)
 [![Package Status](https://img.shields.io/pypi/status/cnmfsns.svg)](https://pypi.org/project/cnmfsns/)
 [![Downloads](https://static.pepy.tech/personalized-badge/cnmfsns?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/cnmfsns)
 [![License](https://img.shields.io/pypi/l/cnmfsns.svg)](https://github.com/MorrissyLab/cNMF-SNS/blob/main/LICENSE)
-
-
 <details>
   <summary> </summary>
 
 ```md
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3509134.svg)](https://doi.org/10.5281/zenodo.3509134)
```

