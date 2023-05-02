# Comparing `tmp/matgl-0.2.0.tar.gz` & `tmp/matgl-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matgl-0.2.0.tar", last modified: Thu Apr 27 02:35:27 2023, max compression
+gzip compressed data, was "matgl-0.2.1.tar", last modified: Tue May  2 14:06:49 2023, max compression
```

## Comparing `matgl-0.2.0.tar` & `matgl-0.2.1.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-04-27 02:35:27.734976 matgl-0.2.0/
--rw-r--r--   0 shyue      (501) staff       (20)     1529 2023-03-24 21:11:48.000000 matgl-0.2.0/LICENSE
--rw-r--r--   0 shyue      (501) staff       (20)     6907 2023-04-27 02:35:27.735064 matgl-0.2.0/PKG-INFO
--rw-r--r--   0 shyue      (501) staff       (20)     5756 2023-04-27 02:19:29.000000 matgl-0.2.0/README.md
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-04-27 02:35:27.726853 matgl-0.2.0/matgl/
--rw-r--r--   0 shyue      (501) staff       (20)      128 2023-04-27 02:34:19.000000 matgl-0.2.0/matgl/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     1694 2023-04-27 02:11:40.000000 matgl-0.2.0/matgl/config.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-04-27 02:35:27.728318 matgl-0.2.0/matgl/dataloader/
--rw-r--r--   0 shyue      (501) staff       (20)       53 2023-03-22 18:49:07.000000 matgl-0.2.0/matgl/dataloader/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    11085 2023-04-22 15:03:50.000000 matgl-0.2.0/matgl/dataloader/dataset.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-04-27 02:35:27.729465 matgl-0.2.0/matgl/graph/
--rw-r--r--   0 shyue      (501) staff       (20)       54 2023-03-22 18:49:07.000000 matgl-0.2.0/matgl/graph/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     5358 2023-04-27 02:12:23.000000 matgl-0.2.0/matgl/graph/compute.py
--rw-r--r--   0 shyue      (501) staff       (20)     6797 2023-03-24 14:22:00.000000 matgl-0.2.0/matgl/graph/converters.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-04-27 02:35:27.732149 matgl-0.2.0/matgl/layers/
--rw-r--r--   0 shyue      (501) staff       (20)       60 2023-03-22 18:49:07.000000 matgl-0.2.0/matgl/layers/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     2099 2023-04-22 15:03:50.000000 matgl-0.2.0/matgl/layers/activations.py
--rw-r--r--   0 shyue      (501) staff       (20)     3586 2023-04-27 02:11:52.000000 matgl-0.2.0/matgl/layers/atom_ref.py
--rw-r--r--   0 shyue      (501) staff       (20)     2168 2023-04-26 23:53:15.000000 matgl-0.2.0/matgl/layers/bond_expansion.py
--rw-r--r--   0 shyue      (501) staff       (20)     6124 2023-04-26 23:56:19.000000 matgl-0.2.0/matgl/layers/core.py
--rw-r--r--   0 shyue      (501) staff       (20)      809 2023-03-22 18:49:07.000000 matgl-0.2.0/matgl/layers/cutoff_functions.py
--rw-r--r--   0 shyue      (501) staff       (20)     3144 2023-04-27 00:46:37.000000 matgl-0.2.0/matgl/layers/embedding_block.py
--rw-r--r--   0 shyue      (501) staff       (20)    16058 2023-04-26 23:57:55.000000 matgl-0.2.0/matgl/layers/graph_conv.py
--rw-r--r--   0 shyue      (501) staff       (20)     3972 2023-04-27 00:48:04.000000 matgl-0.2.0/matgl/layers/readout_block.py
--rw-r--r--   0 shyue      (501) staff       (20)     3726 2023-04-27 00:53:44.000000 matgl-0.2.0/matgl/layers/three_body.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-04-27 02:35:27.733730 matgl-0.2.0/matgl/models/
--rw-r--r--   0 shyue      (501) staff       (20)      124 2023-03-22 18:49:07.000000 matgl-0.2.0/matgl/models/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    12940 2023-03-24 14:41:18.000000 matgl-0.2.0/matgl/models/ase_interface.py
--rw-r--r--   0 shyue      (501) staff       (20)    12293 2023-04-27 00:53:44.000000 matgl-0.2.0/matgl/models/m3gnet.py
--rw-r--r--   0 shyue      (501) staff       (20)     9328 2023-04-27 02:31:12.000000 matgl-0.2.0/matgl/models/megnet.py
--rw-r--r--   0 shyue      (501) staff       (20)     3089 2023-03-24 14:22:00.000000 matgl-0.2.0/matgl/models/potential.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-04-27 02:35:27.734724 matgl-0.2.0/matgl/utils/
--rw-r--r--   0 shyue      (501) staff       (20)       63 2023-03-22 18:49:07.000000 matgl-0.2.0/matgl/utils/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    17703 2023-04-27 02:13:46.000000 matgl-0.2.0/matgl/utils/maths.py
--rw-r--r--   0 shyue      (501) staff       (20)   131200 2023-03-22 18:49:07.000000 matgl-0.2.0/matgl/utils/sb_roots.npy
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-04-27 02:35:27.727858 matgl-0.2.0/matgl.egg-info/
--rw-r--r--   0 shyue      (501) staff       (20)     6907 2023-04-27 02:35:27.000000 matgl-0.2.0/matgl.egg-info/PKG-INFO
--rw-r--r--   0 shyue      (501) staff       (20)      835 2023-04-27 02:35:27.000000 matgl-0.2.0/matgl.egg-info/SOURCES.txt
--rw-r--r--   0 shyue      (501) staff       (20)        1 2023-04-27 02:35:27.000000 matgl-0.2.0/matgl.egg-info/dependency_links.txt
--rw-r--r--   0 shyue      (501) staff       (20)       10 2023-04-27 02:35:27.000000 matgl-0.2.0/matgl.egg-info/requires.txt
--rw-r--r--   0 shyue      (501) staff       (20)        6 2023-04-27 02:35:27.000000 matgl-0.2.0/matgl.egg-info/top_level.txt
--rw-r--r--   0 shyue      (501) staff       (20)     3121 2023-03-24 14:22:00.000000 matgl-0.2.0/pyproject.toml
--rw-r--r--   0 shyue      (501) staff       (20)      603 2023-04-27 02:35:27.735378 matgl-0.2.0/setup.cfg
--rw-r--r--   0 shyue      (501) staff       (20)     2075 2023-03-24 21:13:05.000000 matgl-0.2.0/setup.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-05-02 14:06:49.759614 matgl-0.2.1/
+-rw-r--r--   0 shyue      (501) staff       (20)     1529 2023-03-24 21:11:48.000000 matgl-0.2.1/LICENSE
+-rw-r--r--   0 shyue      (501) staff       (20)     8113 2023-05-02 14:06:49.759712 matgl-0.2.1/PKG-INFO
+-rw-r--r--   0 shyue      (501) staff       (20)     6963 2023-04-30 16:12:51.000000 matgl-0.2.1/README.md
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-05-02 14:06:49.752371 matgl-0.2.1/matgl/
+-rw-r--r--   0 shyue      (501) staff       (20)      128 2023-05-02 13:55:59.000000 matgl-0.2.1/matgl/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1937 2023-05-02 13:54:04.000000 matgl-0.2.1/matgl/config.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-05-02 14:06:49.753846 matgl-0.2.1/matgl/dataloader/
+-rw-r--r--   0 shyue      (501) staff       (20)       53 2023-03-22 18:49:07.000000 matgl-0.2.1/matgl/dataloader/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    11497 2023-05-02 13:08:40.000000 matgl-0.2.1/matgl/dataloader/dataset.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-05-02 14:06:49.754617 matgl-0.2.1/matgl/graph/
+-rw-r--r--   0 shyue      (501) staff       (20)       54 2023-03-22 18:49:07.000000 matgl-0.2.1/matgl/graph/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     5323 2023-05-02 13:08:40.000000 matgl-0.2.1/matgl/graph/compute.py
+-rw-r--r--   0 shyue      (501) staff       (20)     6802 2023-05-02 13:08:40.000000 matgl-0.2.1/matgl/graph/converters.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-05-02 14:06:49.757342 matgl-0.2.1/matgl/layers/
+-rw-r--r--   0 shyue      (501) staff       (20)       60 2023-03-22 18:49:07.000000 matgl-0.2.1/matgl/layers/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2099 2023-04-29 13:55:25.000000 matgl-0.2.1/matgl/layers/activations.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3586 2023-04-29 13:55:25.000000 matgl-0.2.1/matgl/layers/atom_ref.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2168 2023-04-29 13:55:25.000000 matgl-0.2.1/matgl/layers/bond_expansion.py
+-rw-r--r--   0 shyue      (501) staff       (20)     6124 2023-04-29 13:55:25.000000 matgl-0.2.1/matgl/layers/core.py
+-rw-r--r--   0 shyue      (501) staff       (20)      809 2023-03-22 18:49:07.000000 matgl-0.2.1/matgl/layers/cutoff_functions.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3144 2023-04-29 13:55:25.000000 matgl-0.2.1/matgl/layers/embedding_block.py
+-rw-r--r--   0 shyue      (501) staff       (20)    16058 2023-04-29 13:55:25.000000 matgl-0.2.1/matgl/layers/graph_conv.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3972 2023-04-29 13:55:25.000000 matgl-0.2.1/matgl/layers/readout_block.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3726 2023-04-29 13:55:25.000000 matgl-0.2.1/matgl/layers/three_body.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-05-02 14:06:49.758509 matgl-0.2.1/matgl/models/
+-rw-r--r--   0 shyue      (501) staff       (20)      124 2023-03-22 18:49:07.000000 matgl-0.2.1/matgl/models/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    12940 2023-03-24 14:41:18.000000 matgl-0.2.1/matgl/models/ase_interface.py
+-rw-r--r--   0 shyue      (501) staff       (20)    12307 2023-04-29 13:55:25.000000 matgl-0.2.1/matgl/models/m3gnet.py
+-rw-r--r--   0 shyue      (501) staff       (20)    12878 2023-05-02 13:54:32.000000 matgl-0.2.1/matgl/models/megnet.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3089 2023-03-24 14:22:00.000000 matgl-0.2.1/matgl/models/potential.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-05-02 14:06:49.759407 matgl-0.2.1/matgl/utils/
+-rw-r--r--   0 shyue      (501) staff       (20)       63 2023-03-22 18:49:07.000000 matgl-0.2.1/matgl/utils/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1451 2023-05-02 14:06:01.000000 matgl-0.2.1/matgl/utils/data.py
+-rw-r--r--   0 shyue      (501) staff       (20)    17700 2023-05-02 13:08:40.000000 matgl-0.2.1/matgl/utils/maths.py
+-rw-r--r--   0 shyue      (501) staff       (20)   131200 2023-03-22 18:49:07.000000 matgl-0.2.1/matgl/utils/sb_roots.npy
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-05-02 14:06:49.753390 matgl-0.2.1/matgl.egg-info/
+-rw-r--r--   0 shyue      (501) staff       (20)     8113 2023-05-02 14:06:49.000000 matgl-0.2.1/matgl.egg-info/PKG-INFO
+-rw-r--r--   0 shyue      (501) staff       (20)      855 2023-05-02 14:06:49.000000 matgl-0.2.1/matgl.egg-info/SOURCES.txt
+-rw-r--r--   0 shyue      (501) staff       (20)        1 2023-05-02 14:06:49.000000 matgl-0.2.1/matgl.egg-info/dependency_links.txt
+-rw-r--r--   0 shyue      (501) staff       (20)       10 2023-05-02 14:06:49.000000 matgl-0.2.1/matgl.egg-info/requires.txt
+-rw-r--r--   0 shyue      (501) staff       (20)        6 2023-05-02 14:06:49.000000 matgl-0.2.1/matgl.egg-info/top_level.txt
+-rw-r--r--   0 shyue      (501) staff       (20)     3121 2023-03-24 14:22:00.000000 matgl-0.2.1/pyproject.toml
+-rw-r--r--   0 shyue      (501) staff       (20)      603 2023-05-02 14:06:49.760017 matgl-0.2.1/setup.cfg
+-rw-r--r--   0 shyue      (501) staff       (20)     2074 2023-05-02 13:08:40.000000 matgl-0.2.1/setup.py
```

### Comparing `matgl-0.2.0/LICENSE` & `matgl-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `matgl-0.2.0/PKG-INFO` & `matgl-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: matgl
-Version: 0.2.0
-Summary: MatGL (Materials Graph Library) is a framework for graph deep learning for materials science. 
+Version: 0.2.1
+Summary: MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.
 Author: Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Shyue Ping Ong
 Author-email: ongsp@eng.ucsd.edu
 Maintainer: Shyue Ping Ong
 Maintainer-email: ongsp@eng.ucsd.edu
 Keywords: materials,interatomic potential,force field,science,property prediction,AI,machine learning,graph,deep learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -26,14 +26,15 @@
 [![Linting](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)
 [![Testing](https://github.com/materialsvirtuallab/matgl/workflows/Testing%20-%20main/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Testing/badge.svg)
 [![Downloads](https://pepy.tech/badge/matgl)](https://pepy.tech/project/matgl)
 
 # Table of Contents
 * [Introduction](#introduction)
 * [Status](#status)
+* [Architectures](#architectures)
 * [Installation](#installation)
 * [Usage](#usage)
 * [Documentation](#documentation)
 * [References](#references)
 
 <a name="introduction"></a>
 # Introduction
@@ -49,40 +50,55 @@
 
 This effort is a collaboration between the [Materials Virtual Lab](http://materialsvirtuallab.org) and Intel Labs
 (Santiago Miret, Marcel Nassar, Carmelo Gonzales).
 
 <a name="status"></a>
 # Status
 
-Feb 16 2023: Both initial implementations of M3GNet and MEGNet architectures have been completed. Expect bugs!
+- Apr 26 2023: Pre-trained MEGNet models now available for formation energies and band gaps!
+- Feb 16 2023: Both initial implementations of M3GNet and MEGNet architectures have been completed. Expect bugs!
+
+<a name="architectures"></a>
+# Architectures
+
+## MEGNet
+
+<img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MEGNet.png?raw=true"  width="50%">
+
+The MatErials Graph Network (MEGNet) is an implementation of DeepMind's graph networks for universal machine
+learning in materials science. We have demonstrated its success in achieving very low prediction errors in a broad
+array of properties in both molecules and crystals (see "Graph Networks as a Universal Machine Learning Framework for
+Molecules and Crystals"). New releases have included our recent work on multi-fidelity materials property modeling
+(See "Learning properties of ordered and disordered materials from multi-fidelity data").
+
+Briefly, Figure 1 shows the sequential update steps of the graph network, whereby bonds, atoms, and global state
+attributes are updated using information from each other, generating an output graph.
 
 ## M3GNet
 
-<img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/M3GNet_schematic.png?raw=true"  width="50%">
+<img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/M3GNet.png?raw=true"  width="50%">
 
 [M3GNet](https://www.nature.com/articles/s43588-022-00349-3) is a new materials graph neural network architecture that
-incorporates 3-body interactions. A key difference with prior materials graph implementations such as
-[MEGNet](https://github.com/materialsvirtuallab/megnet) is the addition of the coordinates for atoms and the 3×3
-lattice matrix in crystals, which are necessary for obtaining tensorial quantities such as forces and stresses via
-auto-differentiation.
+incorporates 3-body interactions in MEGNet. An additional difference is the addition of the coordinates for atoms and
+the 3×3 lattice matrix in crystals, which are necessary for obtaining tensorial quantities such as forces and
+stresses via auto-differentiation.
 
 As a framework, M3GNet has diverse applications, including:
 
 - **Interatomic potential development.** With the same training data, M3GNet performs similarly to state-of-the-art
   machine learning interatomic potentials (ML-IAPs). However, a key feature of a graph representation is its
   flexibility to scale to diverse chemical spaces. One of the key accomplishments of M3GNet is the development of a
   *universal IAP* that can work across the entire periodic table of the elements by training on relaxations performed
   in the [Materials Project](http://materialsproject.org).
 - **Surrogate models for property predictions.** Like the previous MEGNet architecture, M3GNet can be used to develop
   surrogate models for property predictions, achieving in many cases accuracies that better or similar to other
   state-of-the-art ML models.
 
 For detailed performance benchmarks, please refer to the publication in the [References](#references) section.
 
-
 <a name="installation"></a>
 # Installation
 
 Matgl can be installed via pip for the latest stable version:
 
 ```bash
 pip install matgl
@@ -94,26 +110,25 @@
 python setup.py -e .
 ```
 
 
 <a name="usage"></a>
 # Usage
 
-The pre-trained MEGNet models for the Materials Project formation energy and band gap are now available. The following
-is an example of a prediction of the formation energy for CsCl.
+The pre-trained MEGNet models for the Materials Project formation energy and multi-fidelity band gap are now available.
+The following is an example of a prediction of the formation energy for CsCl.
 
 ```python
 from pymatgen.core import Structure, Lattice
 from matgl.models.megnet import MEGNet
 
-# load the pre-trained MEGNet model. By default, it is the formation energy model.
-model = MEGNet.load()
+# load the pre-trained MEGNet model for formation energy model.
+model = MEGNet.load("MEGNet-MP-2018.6.1-Eform")
 # This is the structure obtained from the Materials Project.
 struct = Structure.from_spacegroup("Pm-3m", Lattice.cubic(4.14), ["Cs", "Cl"], [[0, 0, 0], [0.5, 0.5, 0.5]])
-# define MEGNet calculator
 eform = model.predict_structure(struct)
 print(f"The predicted formation energy for CsCl is {float(eform.numpy()):5f} eV/atom.")
 ```
 
 A full example is in [here](examples/Using%20MEGNet%20Pre-trained%20Models%20for%20Property%20Predictions.ipynb).
 
 
@@ -123,24 +138,29 @@
 - [API documentation](https://materialsvirtuallab.github.io/matgl/modules.html)
 
 <a name="references"></a>
 # References
 
 Please cite the following works:
 
+- MEGNet
+    ```txt
+    Chen, C.; Ye, W.; Zuo, Y.; Zheng, C.; Ong, S. P. Graph Networks as a Universal Machine Learning Framework for
+    Molecules and Crystals. Chem. Mater. 2019, 31 (9), 3564–3572. https://doi.org/10.1021/acs.chemmater.9b01294.
+    ```
+- Multi-fidelity MEGNet
+    ```txt
+    Chen, C.; Zuo, Y.; Ye, W.; Li, X.; Ong, S. P. Learning Properties of Ordered and Disordered Materials from
+    Multi-Fidelity Data. Nature Computational Science 2021, 1, 46–53. https://doi.org/10.1038/s43588-020-00002-x.
+    ```
 - M3GNet
     ```txt
     Chen, C., Ong, S.P. A universal graph deep learning interatomic potential for the periodic table. Nat Comput Sci,
     2, 718–728 (2022). https://doi.org/10.1038/s43588-022-00349-3.
     ```
-- MEGNET
-    ```txt
-    Chen, C.; Ye, W.; Zuo, Y.; Zheng, C.; Ong, S. P. Graph Networks as a Universal Machine Learning Framework for
-    Molecules and Crystals. Chem. Mater. 2019, 31 (9), 3564–3572. https://doi.org/10.1021/acs.chemmater.9b01294.
-    ```
 
 # Acknowledgements
 
 This work was primarily supported by the Materials Project, funded by the U.S. Department of Energy, Office of Science,
 Office of Basic Energy Sciences, Materials Sciences and Engineering Division under contract no.
 DE-AC02-05-CH11231: Materials Project program KC23MP. This work used the Expanse supercomputing cluster at the Extreme
 Science and Engineering Discovery Environment (XSEDE), which is supported by National Science Foundation grant number
```

### Comparing `matgl-0.2.0/README.md` & `matgl-0.2.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 [![Linting](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)
 [![Testing](https://github.com/materialsvirtuallab/matgl/workflows/Testing%20-%20main/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Testing/badge.svg)
 [![Downloads](https://pepy.tech/badge/matgl)](https://pepy.tech/project/matgl)
 
 # Table of Contents
 * [Introduction](#introduction)
 * [Status](#status)
+* [Architectures](#architectures)
 * [Installation](#installation)
 * [Usage](#usage)
 * [Documentation](#documentation)
 * [References](#references)
 
 <a name="introduction"></a>
 # Introduction
@@ -25,40 +26,55 @@
 
 This effort is a collaboration between the [Materials Virtual Lab](http://materialsvirtuallab.org) and Intel Labs
 (Santiago Miret, Marcel Nassar, Carmelo Gonzales).
 
 <a name="status"></a>
 # Status
 
-Feb 16 2023: Both initial implementations of M3GNet and MEGNet architectures have been completed. Expect bugs!
+- Apr 26 2023: Pre-trained MEGNet models now available for formation energies and band gaps!
+- Feb 16 2023: Both initial implementations of M3GNet and MEGNet architectures have been completed. Expect bugs!
+
+<a name="architectures"></a>
+# Architectures
+
+## MEGNet
+
+<img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MEGNet.png?raw=true"  width="50%">
+
+The MatErials Graph Network (MEGNet) is an implementation of DeepMind's graph networks for universal machine
+learning in materials science. We have demonstrated its success in achieving very low prediction errors in a broad
+array of properties in both molecules and crystals (see "Graph Networks as a Universal Machine Learning Framework for
+Molecules and Crystals"). New releases have included our recent work on multi-fidelity materials property modeling
+(See "Learning properties of ordered and disordered materials from multi-fidelity data").
+
+Briefly, Figure 1 shows the sequential update steps of the graph network, whereby bonds, atoms, and global state
+attributes are updated using information from each other, generating an output graph.
 
 ## M3GNet
 
-<img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/M3GNet_schematic.png?raw=true"  width="50%">
+<img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/M3GNet.png?raw=true"  width="50%">
 
 [M3GNet](https://www.nature.com/articles/s43588-022-00349-3) is a new materials graph neural network architecture that
-incorporates 3-body interactions. A key difference with prior materials graph implementations such as
-[MEGNet](https://github.com/materialsvirtuallab/megnet) is the addition of the coordinates for atoms and the 3×3
-lattice matrix in crystals, which are necessary for obtaining tensorial quantities such as forces and stresses via
-auto-differentiation.
+incorporates 3-body interactions in MEGNet. An additional difference is the addition of the coordinates for atoms and
+the 3×3 lattice matrix in crystals, which are necessary for obtaining tensorial quantities such as forces and
+stresses via auto-differentiation.
 
 As a framework, M3GNet has diverse applications, including:
 
 - **Interatomic potential development.** With the same training data, M3GNet performs similarly to state-of-the-art
   machine learning interatomic potentials (ML-IAPs). However, a key feature of a graph representation is its
   flexibility to scale to diverse chemical spaces. One of the key accomplishments of M3GNet is the development of a
   *universal IAP* that can work across the entire periodic table of the elements by training on relaxations performed
   in the [Materials Project](http://materialsproject.org).
 - **Surrogate models for property predictions.** Like the previous MEGNet architecture, M3GNet can be used to develop
   surrogate models for property predictions, achieving in many cases accuracies that better or similar to other
   state-of-the-art ML models.
 
 For detailed performance benchmarks, please refer to the publication in the [References](#references) section.
 
-
 <a name="installation"></a>
 # Installation
 
 Matgl can be installed via pip for the latest stable version:
 
 ```bash
 pip install matgl
@@ -70,26 +86,25 @@
 python setup.py -e .
 ```
 
 
 <a name="usage"></a>
 # Usage
 
-The pre-trained MEGNet models for the Materials Project formation energy and band gap are now available. The following
-is an example of a prediction of the formation energy for CsCl.
+The pre-trained MEGNet models for the Materials Project formation energy and multi-fidelity band gap are now available.
+The following is an example of a prediction of the formation energy for CsCl.
 
 ```python
 from pymatgen.core import Structure, Lattice
 from matgl.models.megnet import MEGNet
 
-# load the pre-trained MEGNet model. By default, it is the formation energy model.
-model = MEGNet.load()
+# load the pre-trained MEGNet model for formation energy model.
+model = MEGNet.load("MEGNet-MP-2018.6.1-Eform")
 # This is the structure obtained from the Materials Project.
 struct = Structure.from_spacegroup("Pm-3m", Lattice.cubic(4.14), ["Cs", "Cl"], [[0, 0, 0], [0.5, 0.5, 0.5]])
-# define MEGNet calculator
 eform = model.predict_structure(struct)
 print(f"The predicted formation energy for CsCl is {float(eform.numpy()):5f} eV/atom.")
 ```
 
 A full example is in [here](examples/Using%20MEGNet%20Pre-trained%20Models%20for%20Property%20Predictions.ipynb).
 
 
@@ -99,24 +114,29 @@
 - [API documentation](https://materialsvirtuallab.github.io/matgl/modules.html)
 
 <a name="references"></a>
 # References
 
 Please cite the following works:
 
+- MEGNet
+    ```txt
+    Chen, C.; Ye, W.; Zuo, Y.; Zheng, C.; Ong, S. P. Graph Networks as a Universal Machine Learning Framework for
+    Molecules and Crystals. Chem. Mater. 2019, 31 (9), 3564–3572. https://doi.org/10.1021/acs.chemmater.9b01294.
+    ```
+- Multi-fidelity MEGNet
+    ```txt
+    Chen, C.; Zuo, Y.; Ye, W.; Li, X.; Ong, S. P. Learning Properties of Ordered and Disordered Materials from
+    Multi-Fidelity Data. Nature Computational Science 2021, 1, 46–53. https://doi.org/10.1038/s43588-020-00002-x.
+    ```
 - M3GNet
     ```txt
     Chen, C., Ong, S.P. A universal graph deep learning interatomic potential for the periodic table. Nat Comput Sci,
     2, 718–728 (2022). https://doi.org/10.1038/s43588-022-00349-3.
     ```
-- MEGNET
-    ```txt
-    Chen, C.; Ye, W.; Zuo, Y.; Zheng, C.; Ong, S. P. Graph Networks as a Universal Machine Learning Framework for
-    Molecules and Crystals. Chem. Mater. 2019, 31 (9), 3564–3572. https://doi.org/10.1021/acs.chemmater.9b01294.
-    ```
 
 # Acknowledgements
 
 This work was primarily supported by the Materials Project, funded by the U.S. Department of Energy, Office of Science,
 Office of Basic Energy Sciences, Materials Sciences and Engineering Division under contract no.
 DE-AC02-05-CH11231: Materials Project program KC23MP. This work used the Expanse supercomputing cluster at the Extreme
 Science and Engineering Discovery Environment (XSEDE), which is supported by National Science Foundation grant number
```

### Comparing `matgl-0.2.0/matgl/config.py` & `matgl-0.2.1/matgl/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 """Global configuration variables for matgl."""
 from __future__ import annotations
 
-import numpy as np
+import os
+from pathlib import Path
 
-# import tensorflow as tf
+import numpy as np
 import torch
 
+# CWD = os.path.dirname(os.path.abspath(__file__))
+
 DTYPES = {
     "float32": {"numpy": np.float32, "torch": torch.float32},
     "float16": {"numpy": np.float16, "torch": torch.float16},
     "int32": {"numpy": np.int32, "torch": torch.int32},
     "int16": {"numpy": np.int16, "torch": torch.int16},
 }
 
+PRETRAINED_MODELS_PATH = Path(os.path.expanduser("~")) / ".matgl" / "models"
+PRETRAINED_MODELS_BASE_URL = "https://github.com/materialsvirtuallab/matgl/raw/main/pretrained_models/"
+
 
 class DataType:
     """
     Tensorflow and numpy data types. Used to choose between float16 and float32
     """
 
     # np_float = tf.keras.mixed_precision.global_policy().compute_dtype
```

### Comparing `matgl-0.2.0/matgl/dataloader/dataset.py` & `matgl-0.2.1/matgl/dataloader/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,17 @@
 def MGLDataLoader(
     train_data: dgl.data.utils.Subset,
     val_data: dgl.data.utils.Subset,
     collate_fn: Callable,
     batch_size: int,
     num_workers: int,
     use_ddp: bool = False,
+    pin_memory: bool = False,
     test_data: dgl.data.utils.Subset | None = None,
+    generator: torch.Generator | None = None,
 ):
     """
     Dataloader for MEGNet training
     Args:
     train_data: training data
     val_data: validation data
     test_data: testing data
@@ -65,34 +67,35 @@
     """
     train_loader = GraphDataLoader(
         train_data,
         batch_size=batch_size,
         shuffle=True,
         collate_fn=collate_fn,
         num_workers=num_workers,
-        pin_memory=True,
+        pin_memory=pin_memory,
         use_ddp=use_ddp,
+        generator=generator,
     )
 
     val_loader = GraphDataLoader(
         val_data,
         batch_size=batch_size,
         shuffle=False,
         collate_fn=collate_fn,
         num_workers=num_workers,
-        pin_memory=True,
+        pin_memory=pin_memory,
     )
     if test_data is not None:
         test_loader = GraphDataLoader(
             test_data,
             batch_size=batch_size,
             shuffle=False,
             collate_fn=collate_fn,
             num_workers=num_workers,
-            pin_memory=True,
+            pin_memory=pin_memory,
         )
         return train_loader, val_loader, test_loader
     else:
         return train_loader, val_loader
 
 
 class MEGNetDataset(DGLDataset):
@@ -101,32 +104,34 @@
     """
 
     def __init__(
         self,
         structures: list,
         labels: list,
         label_name: str,
-        converter,
+        converter: Pmg2Graph,
         initial: float = 0.0,
         final: float = 5.0,
-        num_centers: int = 20,
+        num_centers: int = 100,
         width: float = 0.5,
         name: str = "MEGNETDataset",
         graph_labels: list | None = None,
     ):
         """
         Args:
         structures: Pymatgen strutcure
         labels: property values
         label: label name
         converter: Transformer for converting structures to DGL graphs, e.g., Pmg2Graph.
         initial: initial distance for Gaussian expansions
         final: final distance for Gaussian expansions
         num_centers: number of Gaussian functions
         width: width of Gaussian functions
+        name: Name of dataset
+        graph_labels: graph attributes either integers and floating point numbers
         """
         self.converter = converter
         self.structures = structures
         self.labels = torch.FloatTensor(labels)
         self.label_name = label_name
         self.initial = initial
         self.final = final
@@ -162,15 +167,18 @@
             else:
                 graph, state_attr = self.converter.get_graph_from_molecule(mol=structure)
             bond_vec, bond_dist = compute_pair_vector_and_distance(graph)
             graph.edata["edge_attr"] = bond_expansion(bond_dist)
             self.graphs.append(graph)
             self.graph_attr.append(state_attr)
         if self.graph_labels is not None:
-            self.graph_attr = torch.tensor(self.graph_labels).long()  # type: ignore
+            if np.array(self.graph_labels).dtype == "int64":
+                self.graph_attr = torch.tensor(self.graph_labels).long()  # type: ignore
+            else:
+                self.graph_attr = torch.tensor(self.graph_labels)  # type: ignore
         else:
             self.graph_attr = torch.tensor(self.graph_attr)  # type: ignore
 
         return self.graphs, self.graph_attr
 
     def save(self, filename: str = "dgl_graph.bin", filename_graph_attr: str = "graph_attr.pt"):
         """
```

### Comparing `matgl-0.2.0/matgl/graph/compute.py` & `matgl-0.2.1/matgl/graph/compute.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,20 +81,20 @@
 
     Returns:
     bond_vec (torch.tensor): bond distance between two atoms
     bond_dist (torch.tensor): vector from src node to dst node
     """
     bond_vec = torch.zeros(g.num_edges(), 3)
     bond_dist = torch.zeros(g.num_edges())
-    for i in range(g.num_edges()):
-        bond_vec[i, :] = (
-            g.ndata["pos"][g.edges()[1][i], :]
-            + torch.sum(torch.squeeze(g.edata["pbc_offset"][i][:] * g.edata["lattice"][i][:, None]), dim=0)
-            - g.ndata["pos"][g.edges()[0][i], :]
-        )
+    bond_vec[:, :] = (
+        g.ndata["pos"][g.edges()[1][:].long(), :]
+        + torch.squeeze(torch.matmul(g.edata["pbc_offset"].unsqueeze(1), torch.squeeze(g.edata["lattice"])))
+        - g.ndata["pos"][g.edges()[0][:].long(), :]
+    )
+
     bond_dist = torch.norm(bond_vec, dim=1)
 
     return bond_vec, bond_dist
 
 
 def compute_theta_and_phi(edges: dgl.udf.EdgeBatch):
     """
```

### Comparing `matgl-0.2.0/matgl/graph/converters.py` & `matgl-0.2.1/matgl/graph/converters.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 class Pmg2Graph:
     """
     Construct a DGL graph from Pymatgen Molecules or Structures, ASE atoms is also added.
     """
 
     def __init__(
         self,
-        element_types: tuple[str],
+        element_types: tuple[str, ...],
         cutoff: float = 5.0,
     ):
         """
         Parameters
         ----------
         element_types: List of elements present in dataset for graph conversion. This ensures all graphs are
             constructed with the same dimensionality of features.
```

### Comparing `matgl-0.2.0/matgl/layers/activations.py` & `matgl-0.2.1/matgl/layers/activations.py`

 * *Files identical despite different names*

### Comparing `matgl-0.2.0/matgl/layers/atom_ref.py` & `matgl-0.2.1/matgl/layers/atom_ref.py`

 * *Files identical despite different names*

### Comparing `matgl-0.2.0/matgl/layers/bond_expansion.py` & `matgl-0.2.1/matgl/layers/bond_expansion.py`

 * *Files identical despite different names*

### Comparing `matgl-0.2.0/matgl/layers/core.py` & `matgl-0.2.1/matgl/layers/core.py`

 * *Files identical despite different names*

### Comparing `matgl-0.2.0/matgl/layers/cutoff_functions.py` & `matgl-0.2.1/matgl/layers/cutoff_functions.py`

 * *Files identical despite different names*

### Comparing `matgl-0.2.0/matgl/layers/embedding_block.py` & `matgl-0.2.1/matgl/layers/embedding_block.py`

 * *Files identical despite different names*

### Comparing `matgl-0.2.0/matgl/layers/graph_conv.py` & `matgl-0.2.1/matgl/layers/graph_conv.py`

 * *Files identical despite different names*

### Comparing `matgl-0.2.0/matgl/layers/readout_block.py` & `matgl-0.2.1/matgl/layers/readout_block.py`

 * *Files identical despite different names*

### Comparing `matgl-0.2.0/matgl/layers/three_body.py` & `matgl-0.2.1/matgl/layers/three_body.py`

 * *Files identical despite different names*

### Comparing `matgl-0.2.0/matgl/models/ase_interface.py` & `matgl-0.2.1/matgl/models/ase_interface.py`

 * *Files identical despite different names*

### Comparing `matgl-0.2.0/matgl/models/m3gnet.py` & `matgl-0.2.1/matgl/models/m3gnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from matgl.layers.three_body import SphericalBesselWithHarmonics, ThreeBodyInteractions
 
 logger = logging.getLogger(__file__)
 CWD = os.path.dirname(os.path.abspath(__file__))
 
 MODEL_NAME = "m3gnet"
 
-MODEL_PATHS = {"MP-2021.2.8-EFS": os.path.join(CWD, "..", "..", "pretrained", "MP-2021.2.8-EFS")}
+MODEL_PATHS = {"MP-2021.2.8-EFS": os.path.join(CWD, "..", "..", "pretrained_models", "MP-2021.2.8-EFS")}
 
 
 class M3GNet(nn.Module):
     """
     The main M3GNet model
     """
 
@@ -237,15 +237,15 @@
         """
         if model_dir in MODEL_PATHS:
             return cls.from_dir(MODEL_PATHS[model_dir])
 
         if os.path.isdir(model_dir) and "m3gnet.pt" in os.listdir(model_dir):
             return cls.from_dir(model_dir)
 
-        raise ValueError(f"{model_dir} not found in available pretrained {list(MODEL_PATHS.keys())}")
+        raise ValueError(f"{model_dir} not found in available pretrained_models {list(MODEL_PATHS.keys())}")
 
     def forward(self, g: dgl.DGLGraph, state_attr: torch.tensor | None = None, l_g: dgl.DGLGraph | None = None):
         """Performs message passing and updates node representations.
 
         Parameters
         ----------
         g : DGLGraph
```

### Comparing `matgl-0.2.0/matgl/models/potential.py` & `matgl-0.2.1/matgl/models/potential.py`

 * *Files identical despite different names*

### Comparing `matgl-0.2.0/matgl/utils/maths.py` & `matgl-0.2.1/matgl/utils/maths.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
         self.cutoff = cutoff
         self.smooth = smooth
         if smooth:
             self.funcs = self._calculate_smooth_symbolic_funcs()
         else:
             self.funcs = self._calculate_symbolic_funcs()
 
-        self.zeros = torch.from_numpy(SPHERICAL_BESSEL_ROOTS).type(DataType.torch_float)
+        self.zeros = torch.tensor(SPHERICAL_BESSEL_ROOTS, dtype=DataType.torch_float)
 
     @lru_cache(maxsize=128)
     def _calculate_symbolic_funcs(self) -> list:
         """
         Spherical basis functions based on Rayleigh formula. This function
         generates
         symbolic formula.
```

### Comparing `matgl-0.2.0/matgl/utils/sb_roots.npy` & `matgl-0.2.1/matgl/utils/sb_roots.npy`

 * *Files identical despite different names*

### Comparing `matgl-0.2.0/matgl.egg-info/PKG-INFO` & `matgl-0.2.1/matgl.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: matgl
-Version: 0.2.0
-Summary: MatGL (Materials Graph Library) is a framework for graph deep learning for materials science. 
+Version: 0.2.1
+Summary: MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.
 Author: Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Shyue Ping Ong
 Author-email: ongsp@eng.ucsd.edu
 Maintainer: Shyue Ping Ong
 Maintainer-email: ongsp@eng.ucsd.edu
 Keywords: materials,interatomic potential,force field,science,property prediction,AI,machine learning,graph,deep learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -26,14 +26,15 @@
 [![Linting](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)
 [![Testing](https://github.com/materialsvirtuallab/matgl/workflows/Testing%20-%20main/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Testing/badge.svg)
 [![Downloads](https://pepy.tech/badge/matgl)](https://pepy.tech/project/matgl)
 
 # Table of Contents
 * [Introduction](#introduction)
 * [Status](#status)
+* [Architectures](#architectures)
 * [Installation](#installation)
 * [Usage](#usage)
 * [Documentation](#documentation)
 * [References](#references)
 
 <a name="introduction"></a>
 # Introduction
@@ -49,40 +50,55 @@
 
 This effort is a collaboration between the [Materials Virtual Lab](http://materialsvirtuallab.org) and Intel Labs
 (Santiago Miret, Marcel Nassar, Carmelo Gonzales).
 
 <a name="status"></a>
 # Status
 
-Feb 16 2023: Both initial implementations of M3GNet and MEGNet architectures have been completed. Expect bugs!
+- Apr 26 2023: Pre-trained MEGNet models now available for formation energies and band gaps!
+- Feb 16 2023: Both initial implementations of M3GNet and MEGNet architectures have been completed. Expect bugs!
+
+<a name="architectures"></a>
+# Architectures
+
+## MEGNet
+
+<img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MEGNet.png?raw=true"  width="50%">
+
+The MatErials Graph Network (MEGNet) is an implementation of DeepMind's graph networks for universal machine
+learning in materials science. We have demonstrated its success in achieving very low prediction errors in a broad
+array of properties in both molecules and crystals (see "Graph Networks as a Universal Machine Learning Framework for
+Molecules and Crystals"). New releases have included our recent work on multi-fidelity materials property modeling
+(See "Learning properties of ordered and disordered materials from multi-fidelity data").
+
+Briefly, Figure 1 shows the sequential update steps of the graph network, whereby bonds, atoms, and global state
+attributes are updated using information from each other, generating an output graph.
 
 ## M3GNet
 
-<img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/M3GNet_schematic.png?raw=true"  width="50%">
+<img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/M3GNet.png?raw=true"  width="50%">
 
 [M3GNet](https://www.nature.com/articles/s43588-022-00349-3) is a new materials graph neural network architecture that
-incorporates 3-body interactions. A key difference with prior materials graph implementations such as
-[MEGNet](https://github.com/materialsvirtuallab/megnet) is the addition of the coordinates for atoms and the 3×3
-lattice matrix in crystals, which are necessary for obtaining tensorial quantities such as forces and stresses via
-auto-differentiation.
+incorporates 3-body interactions in MEGNet. An additional difference is the addition of the coordinates for atoms and
+the 3×3 lattice matrix in crystals, which are necessary for obtaining tensorial quantities such as forces and
+stresses via auto-differentiation.
 
 As a framework, M3GNet has diverse applications, including:
 
 - **Interatomic potential development.** With the same training data, M3GNet performs similarly to state-of-the-art
   machine learning interatomic potentials (ML-IAPs). However, a key feature of a graph representation is its
   flexibility to scale to diverse chemical spaces. One of the key accomplishments of M3GNet is the development of a
   *universal IAP* that can work across the entire periodic table of the elements by training on relaxations performed
   in the [Materials Project](http://materialsproject.org).
 - **Surrogate models for property predictions.** Like the previous MEGNet architecture, M3GNet can be used to develop
   surrogate models for property predictions, achieving in many cases accuracies that better or similar to other
   state-of-the-art ML models.
 
 For detailed performance benchmarks, please refer to the publication in the [References](#references) section.
 
-
 <a name="installation"></a>
 # Installation
 
 Matgl can be installed via pip for the latest stable version:
 
 ```bash
 pip install matgl
@@ -94,26 +110,25 @@
 python setup.py -e .
 ```
 
 
 <a name="usage"></a>
 # Usage
 
-The pre-trained MEGNet models for the Materials Project formation energy and band gap are now available. The following
-is an example of a prediction of the formation energy for CsCl.
+The pre-trained MEGNet models for the Materials Project formation energy and multi-fidelity band gap are now available.
+The following is an example of a prediction of the formation energy for CsCl.
 
 ```python
 from pymatgen.core import Structure, Lattice
 from matgl.models.megnet import MEGNet
 
-# load the pre-trained MEGNet model. By default, it is the formation energy model.
-model = MEGNet.load()
+# load the pre-trained MEGNet model for formation energy model.
+model = MEGNet.load("MEGNet-MP-2018.6.1-Eform")
 # This is the structure obtained from the Materials Project.
 struct = Structure.from_spacegroup("Pm-3m", Lattice.cubic(4.14), ["Cs", "Cl"], [[0, 0, 0], [0.5, 0.5, 0.5]])
-# define MEGNet calculator
 eform = model.predict_structure(struct)
 print(f"The predicted formation energy for CsCl is {float(eform.numpy()):5f} eV/atom.")
 ```
 
 A full example is in [here](examples/Using%20MEGNet%20Pre-trained%20Models%20for%20Property%20Predictions.ipynb).
 
 
@@ -123,24 +138,29 @@
 - [API documentation](https://materialsvirtuallab.github.io/matgl/modules.html)
 
 <a name="references"></a>
 # References
 
 Please cite the following works:
 
+- MEGNet
+    ```txt
+    Chen, C.; Ye, W.; Zuo, Y.; Zheng, C.; Ong, S. P. Graph Networks as a Universal Machine Learning Framework for
+    Molecules and Crystals. Chem. Mater. 2019, 31 (9), 3564–3572. https://doi.org/10.1021/acs.chemmater.9b01294.
+    ```
+- Multi-fidelity MEGNet
+    ```txt
+    Chen, C.; Zuo, Y.; Ye, W.; Li, X.; Ong, S. P. Learning Properties of Ordered and Disordered Materials from
+    Multi-Fidelity Data. Nature Computational Science 2021, 1, 46–53. https://doi.org/10.1038/s43588-020-00002-x.
+    ```
 - M3GNet
     ```txt
     Chen, C., Ong, S.P. A universal graph deep learning interatomic potential for the periodic table. Nat Comput Sci,
     2, 718–728 (2022). https://doi.org/10.1038/s43588-022-00349-3.
     ```
-- MEGNET
-    ```txt
-    Chen, C.; Ye, W.; Zuo, Y.; Zheng, C.; Ong, S. P. Graph Networks as a Universal Machine Learning Framework for
-    Molecules and Crystals. Chem. Mater. 2019, 31 (9), 3564–3572. https://doi.org/10.1021/acs.chemmater.9b01294.
-    ```
 
 # Acknowledgements
 
 This work was primarily supported by the Materials Project, funded by the U.S. Department of Energy, Office of Science,
 Office of Basic Energy Sciences, Materials Sciences and Engineering Division under contract no.
 DE-AC02-05-CH11231: Materials Project program KC23MP. This work used the Expanse supercomputing cluster at the Extreme
 Science and Engineering Discovery Environment (XSEDE), which is supported by National Science Foundation grant number
```

### Comparing `matgl-0.2.0/matgl.egg-info/SOURCES.txt` & `matgl-0.2.1/matgl.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,9 +27,10 @@
 matgl/layers/three_body.py
 matgl/models/__init__.py
 matgl/models/ase_interface.py
 matgl/models/m3gnet.py
 matgl/models/megnet.py
 matgl/models/potential.py
 matgl/utils/__init__.py
+matgl/utils/data.py
 matgl/utils/maths.py
 matgl/utils/sb_roots.npy
```

### Comparing `matgl-0.2.0/pyproject.toml` & `matgl-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `matgl-0.2.0/setup.cfg` & `matgl-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `matgl-0.2.0/setup.py` & `matgl-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 setup(
     name="matgl",
     version=version,
     author="Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Shyue Ping Ong",
     author_email="ongsp@eng.ucsd.edu",
     maintainer="Shyue Ping Ong",
     maintainer_email="ongsp@eng.ucsd.edu",
-    description="MatGL (Materials Graph Library) is a framework for graph deep learning for materials science. ",
+    description="MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=[
         "materials",
         "interatomic potential",
         "force field",
         "science",
```

