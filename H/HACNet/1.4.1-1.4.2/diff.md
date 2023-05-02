# Comparing `tmp/HACNet-1.4.1.tar.gz` & `tmp/HACNet-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HACNet-1.4.1.tar", last modified: Tue May  2 17:31:27 2023, max compression
+gzip compressed data, was "HACNet-1.4.2.tar", last modified: Tue May  2 17:55:47 2023, max compression
```

## Comparing `HACNet-1.4.1.tar` & `HACNet-1.4.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 17:31:27.773800 HACNet-1.4.1/
-drwxrwxrwx   0        0        0        0 2023-05-02 17:31:27.707457 HACNet-1.4.1/HACNet/
--rw-rw-rw-   0        0        0    14950 2023-05-02 17:31:14.000000 HACNet-1.4.1/HACNet/CNN.py
--rw-rw-rw-   0        0        0    15340 2023-05-02 17:31:14.000000 HACNet-1.4.1/HACNet/GCN.py
--rw-rw-rw-   0        0        0     8898 2023-05-02 17:31:14.000000 HACNet-1.4.1/HACNet/MLP.py
--rw-rw-rw-   0        0        0        2 2023-05-02 17:31:14.000000 HACNet-1.4.1/HACNet/__init__.py
--rw-rw-rw-   0        0        0    55337 2023-05-02 17:31:14.000000 HACNet-1.4.1/HACNet/functions.py
-drwxrwxrwx   0        0        0        0 2023-05-02 17:31:27.767815 HACNet-1.4.1/HACNet.egg-info/
--rw-rw-rw-   0        0        0      373 2023-05-02 17:31:27.000000 HACNet-1.4.1/HACNet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-05-02 17:31:27.000000 HACNet-1.4.1/HACNet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 17:31:27.000000 HACNet-1.4.1/HACNet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-02 17:31:27.000000 HACNet-1.4.1/HACNet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1090 2023-05-02 17:31:16.000000 HACNet-1.4.1/LICENSE
--rw-rw-rw-   0        0        0      373 2023-05-02 17:31:27.773800 HACNet-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     3536 2023-05-02 17:31:16.000000 HACNet-1.4.1/README.md
--rw-rw-rw-   0        0        0       86 2023-05-02 17:31:27.778791 HACNet-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0      498 2023-05-02 17:31:16.000000 HACNet-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:55:47.716149 HACNet-1.4.2/
+drwxrwxrwx   0        0        0        0 2023-05-02 17:55:47.675258 HACNet-1.4.2/HACNet/
+-rw-rw-rw-   0        0        0    14950 2023-05-02 17:55:24.000000 HACNet-1.4.2/HACNet/CNN.py
+-rw-rw-rw-   0        0        0    15340 2023-05-02 17:55:24.000000 HACNet-1.4.2/HACNet/GCN.py
+-rw-rw-rw-   0        0        0     8898 2023-05-02 17:55:24.000000 HACNet-1.4.2/HACNet/MLP.py
+-rw-rw-rw-   0        0        0        2 2023-05-02 17:55:24.000000 HACNet-1.4.2/HACNet/__init__.py
+-rw-rw-rw-   0        0        0    55401 2023-05-02 17:55:24.000000 HACNet-1.4.2/HACNet/functions.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:55:47.710165 HACNet-1.4.2/HACNet.egg-info/
+-rw-rw-rw-   0        0        0      373 2023-05-02 17:55:47.000000 HACNet-1.4.2/HACNet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-05-02 17:55:47.000000 HACNet-1.4.2/HACNet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 17:55:47.000000 HACNet-1.4.2/HACNet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-02 17:55:47.000000 HACNet-1.4.2/HACNet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1090 2023-05-02 17:55:26.000000 HACNet-1.4.2/LICENSE
+-rw-rw-rw-   0        0        0      373 2023-05-02 17:55:47.716149 HACNet-1.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3536 2023-05-02 17:55:26.000000 HACNet-1.4.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-02 17:55:47.720139 HACNet-1.4.2/setup.cfg
+-rw-rw-rw-   0        0        0      498 2023-05-02 17:55:27.000000 HACNet-1.4.2/setup.py
```

### Comparing `HACNet-1.4.1/HACNet/CNN.py` & `HACNet-1.4.2/HACNet/CNN.py`

 * *Files identical despite different names*

### Comparing `HACNet-1.4.1/HACNet/GCN.py` & `HACNet-1.4.2/HACNet/GCN.py`

 * *Files identical despite different names*

### Comparing `HACNet-1.4.1/HACNet/MLP.py` & `HACNet-1.4.2/HACNet/MLP.py`

 * *Files identical despite different names*

### Comparing `HACNet-1.4.1/HACNet/functions.py` & `HACNet-1.4.2/HACNet/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -403,15 +403,15 @@
 		fc1 = self.fc1_bn(fc1_y) if fc1_y.shape[0]>1 else fc1_y
 		fc2_z = self.fc2(fc1)
 		return fc2_z, fc1_z
 
 
 	""" define a function to predict pkd for a single protein-ligand complex """
 
-def predict_pkd(protein_pdb, ligand_mol2, verbose=True): 
+def predict_pkd(protein_pdb, ligand_mol2, elements_xml, cnn_params, gcn0_params, gcn1_params, mlp_params, verbose=True): 
 
   """
   Inputs:
   1) protein_pdb: path to protein pdb file
   2) ligand_mol2: path to ligand mol2 file
   3) verbose: if True, will return pkd and image of protein-ligand complex.
       If False, will return float corresponding to predicted pkd. Default is True
```

### Comparing `HACNet-1.4.1/LICENSE` & `HACNet-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `HACNet-1.4.1/README.md` & `HACNet-1.4.2/README.md`

 * *Files identical despite different names*

