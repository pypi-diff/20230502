# Comparing `tmp/vdna-0.1.0b0.tar.gz` & `tmp/vdna-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdna-0.1.0b0.tar", last modified: Thu Apr 20 05:17:45 2023, max compression
+gzip compressed data, was "vdna-0.1.1.tar", last modified: Tue May  2 02:32:27 2023, max compression
```

## Comparing `vdna-0.1.0b0.tar` & `vdna-0.1.1.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxrwx---   0 mattwidojo  (1005) jattias   (1005)        0 2023-04-20 05:17:45.759664 vdna-0.1.0b0/
--rw-rw----   0 mattwidojo  (1005) jattias   (1005)     1074 2023-04-20 04:52:55.000000 vdna-0.1.0b0/LICENSE
--rw-rw----   0 mattwidojo  (1005) jattias   (1005)    10082 2023-04-20 05:17:45.759664 vdna-0.1.0b0/PKG-INFO
--rw-rw----   0 mattwidojo  (1005) jattias   (1005)     9529 2023-04-20 04:52:55.000000 vdna-0.1.0b0/README.md
--rw-rw----   0 mattwidojo  (1005) jattias   (1005)      787 2023-04-20 05:17:01.000000 vdna-0.1.0b0/pyproject.toml
--rw-rw----   0 mattwidojo  (1005) jattias   (1005)       38 2023-04-20 05:17:45.763664 vdna-0.1.0b0/setup.cfg
-drwxrwx---   0 mattwidojo  (1005) jattias   (1005)        0 2023-04-20 05:17:45.651660 vdna-0.1.0b0/src/
-drwxrwx---   0 mattwidojo  (1005) jattias   (1005)        0 2023-04-20 05:17:45.683661 vdna-0.1.0b0/src/vdna/
--rw-rw----   0 mattwidojo  (1005) jattias   (1005)      208 2023-04-20 04:52:56.000000 vdna-0.1.0b0/src/vdna/__init__.py
--rw-rw----   0 mattwidojo  (1005) jattias   (1005)    14691 2023-04-20 04:52:56.000000 vdna-0.1.0b0/src/vdna/distances.py
-drwxrwx---   0 mattwidojo  (1005) jattias   (1005)        0 2023-04-20 05:17:45.719663 vdna-0.1.0b0/src/vdna/networks/
--rw-rw----   0 mattwidojo  (1005) jattias   (1005)     2234 2023-04-20 04:52:56.000000 vdna-0.1.0b0/src/vdna/networks/__init__.py
--rw-rw----   0 mattwidojo  (1005) jattias   (1005)    23479 2023-04-20 04:52:56.000000 vdna-0.1.0b0/src/vdna/networks/clip.py
--rw-rw----   0 mattwidojo  (1005) jattias   (1005)    14815 2023-04-20 04:52:56.000000 vdna-0.1.0b0/src/vdna/networks/dino_resnet50.py
--rw-rw----   0 mattwidojo  (1005) jattias   (1005)    16122 2023-04-20 04:52:56.000000 vdna-0.1.0b0/src/vdna/networks/dino_vit.py
--rw-rw----   0 mattwidojo  (1005) jattias   (1005)    11773 2023-04-20 04:52:56.000000 vdna-0.1.0b0/src/vdna/networks/feature_extraction_model.py
--rw-rw----   0 mattwidojo  (1005) jattias   (1005)    12980 2023-04-20 04:52:56.000000 vdna-0.1.0b0/src/vdna/networks/inception_pytorch.py
--rw-rw----   0 mattwidojo  (1005) jattias   (1005)    16862 2023-04-20 04:52:56.000000 vdna-0.1.0b0/src/vdna/networks/mugs_vit.py
--rw-rw----   0 mattwidojo  (1005) jattias   (1005)    14565 2023-04-20 04:52:56.000000 vdna-0.1.0b0/src/vdna/networks/random_resnet50.py
--rw-rw----   0 mattwidojo  (1005) jattias   (1005)     7860 2023-04-20 04:52:56.000000 vdna-0.1.0b0/src/vdna/networks/vgg16.py
-drwxrwx---   0 mattwidojo  (1005) jattias   (1005)        0 2023-04-20 05:17:45.735663 vdna-0.1.0b0/src/vdna/utils/
--rw-rw----   0 mattwidojo  (1005) jattias   (1005)     8470 2023-04-20 04:52:56.000000 vdna-0.1.0b0/src/vdna/utils/im.py
--rw-rw----   0 mattwidojo  (1005) jattias   (1005)      843 2023-04-20 04:52:56.000000 vdna-0.1.0b0/src/vdna/utils/io.py
--rw-rw----   0 mattwidojo  (1005) jattias   (1005)     1514 2023-04-20 04:52:56.000000 vdna-0.1.0b0/src/vdna/utils/settings.py
--rw-rw----   0 mattwidojo  (1005) jattias   (1005)     3886 2023-04-20 04:52:56.000000 vdna-0.1.0b0/src/vdna/utils/stats.py
--rw-rw----   0 mattwidojo  (1005) jattias   (1005)      942 2023-04-20 04:52:56.000000 vdna-0.1.0b0/src/vdna/utils/utils.py
--rw-rw----   0 mattwidojo  (1005) jattias   (1005)     5843 2023-04-20 04:52:56.000000 vdna-0.1.0b0/src/vdna/vdna_processor.py
-drwxrwx---   0 mattwidojo  (1005) jattias   (1005)        0 2023-04-20 05:17:45.751664 vdna-0.1.0b0/src/vdna/vdnas/
--rw-rw----   0 mattwidojo  (1005) jattias   (1005)      535 2023-04-20 05:17:36.000000 vdna-0.1.0b0/src/vdna/vdnas/__init__.py
--rw-rw----   0 mattwidojo  (1005) jattias   (1005)     4206 2023-04-20 04:52:56.000000 vdna-0.1.0b0/src/vdna/vdnas/vdna_base.py
--rw-rw----   0 mattwidojo  (1005) jattias   (1005)     2892 2023-04-20 04:52:56.000000 vdna-0.1.0b0/src/vdna/vdnas/vdna_gauss.py
--rw-rw----   0 mattwidojo  (1005) jattias   (1005)     2304 2023-04-20 04:52:56.000000 vdna-0.1.0b0/src/vdna/vdnas/vdna_hist.py
--rw-rw----   0 mattwidojo  (1005) jattias   (1005)     2443 2023-04-20 04:52:56.000000 vdna-0.1.0b0/src/vdna/vdnas/vdna_layer_gauss.py
--rw-rw----   0 mattwidojo  (1005) jattias   (1005)       37 2023-04-20 05:17:07.000000 vdna-0.1.0b0/src/vdna/version.py
-drwxrwx---   0 mattwidojo  (1005) jattias   (1005)        0 2023-04-20 05:17:45.695662 vdna-0.1.0b0/src/vdna.egg-info/
--rw-rw----   0 mattwidojo  (1005) jattias   (1005)    10082 2023-04-20 05:17:45.000000 vdna-0.1.0b0/src/vdna.egg-info/PKG-INFO
--rw-rw----   0 mattwidojo  (1005) jattias   (1005)      863 2023-04-20 05:17:45.000000 vdna-0.1.0b0/src/vdna.egg-info/SOURCES.txt
--rw-rw----   0 mattwidojo  (1005) jattias   (1005)        1 2023-04-20 05:17:45.000000 vdna-0.1.0b0/src/vdna.egg-info/dependency_links.txt
--rw-rw----   0 mattwidojo  (1005) jattias   (1005)       86 2023-04-20 05:17:45.000000 vdna-0.1.0b0/src/vdna.egg-info/requires.txt
--rw-rw----   0 mattwidojo  (1005) jattias   (1005)        5 2023-04-20 05:17:45.000000 vdna-0.1.0b0/src/vdna.egg-info/top_level.txt
-drwxrwx---   0 mattwidojo  (1005) jattias   (1005)        0 2023-04-20 05:17:45.755664 vdna-0.1.0b0/tests/
--rw-rw----   0 mattwidojo  (1005) jattias   (1005)    12739 2023-04-20 04:52:56.000000 vdna-0.1.0b0/tests/test_all.py
+drwxrwx---   0 mattwidojo  (1005) jattias   (1005)        0 2023-05-02 02:32:27.080179 vdna-0.1.1/
+-rw-rw----   0 mattwidojo  (1005) jattias   (1005)     1074 2023-04-20 04:52:55.000000 vdna-0.1.1/LICENSE
+-rw-rw----   0 mattwidojo  (1005) jattias   (1005)    10781 2023-05-02 02:32:27.072178 vdna-0.1.1/PKG-INFO
+-rw-rw----   0 mattwidojo  (1005) jattias   (1005)    10230 2023-05-02 02:31:04.000000 vdna-0.1.1/README.md
+-rw-rw----   0 mattwidojo  (1005) jattias   (1005)      786 2023-05-02 02:32:04.000000 vdna-0.1.1/pyproject.toml
+-rw-rw----   0 mattwidojo  (1005) jattias   (1005)       38 2023-05-02 02:32:27.080179 vdna-0.1.1/setup.cfg
+drwxrwx---   0 mattwidojo  (1005) jattias   (1005)        0 2023-05-02 02:32:26.672163 vdna-0.1.1/src/
+drwxrwx---   0 mattwidojo  (1005) jattias   (1005)        0 2023-05-02 02:32:26.788167 vdna-0.1.1/src/vdna/
+-rw-rw----   0 mattwidojo  (1005) jattias   (1005)      208 2023-04-20 04:52:56.000000 vdna-0.1.1/src/vdna/__init__.py
+-rw-rw----   0 mattwidojo  (1005) jattias   (1005)    14691 2023-04-20 04:52:56.000000 vdna-0.1.1/src/vdna/distances.py
+drwxrwx---   0 mattwidojo  (1005) jattias   (1005)        0 2023-05-02 02:32:26.944173 vdna-0.1.1/src/vdna/networks/
+-rw-rw----   0 mattwidojo  (1005) jattias   (1005)     2234 2023-04-20 04:52:56.000000 vdna-0.1.1/src/vdna/networks/__init__.py
+-rw-rw----   0 mattwidojo  (1005) jattias   (1005)    23479 2023-04-20 04:52:56.000000 vdna-0.1.1/src/vdna/networks/clip.py
+-rw-rw----   0 mattwidojo  (1005) jattias   (1005)    14815 2023-04-20 04:52:56.000000 vdna-0.1.1/src/vdna/networks/dino_resnet50.py
+-rw-rw----   0 mattwidojo  (1005) jattias   (1005)    16122 2023-04-20 04:52:56.000000 vdna-0.1.1/src/vdna/networks/dino_vit.py
+-rw-rw----   0 mattwidojo  (1005) jattias   (1005)    11773 2023-04-20 04:52:56.000000 vdna-0.1.1/src/vdna/networks/feature_extraction_model.py
+-rw-rw----   0 mattwidojo  (1005) jattias   (1005)    12980 2023-04-20 04:52:56.000000 vdna-0.1.1/src/vdna/networks/inception_pytorch.py
+-rw-rw----   0 mattwidojo  (1005) jattias   (1005)    16862 2023-04-20 04:52:56.000000 vdna-0.1.1/src/vdna/networks/mugs_vit.py
+-rw-rw----   0 mattwidojo  (1005) jattias   (1005)    14565 2023-04-20 04:52:56.000000 vdna-0.1.1/src/vdna/networks/random_resnet50.py
+-rw-rw----   0 mattwidojo  (1005) jattias   (1005)     7860 2023-04-20 04:52:56.000000 vdna-0.1.1/src/vdna/networks/vgg16.py
+drwxrwx---   0 mattwidojo  (1005) jattias   (1005)        0 2023-05-02 02:32:26.996175 vdna-0.1.1/src/vdna/utils/
+-rw-rw----   0 mattwidojo  (1005) jattias   (1005)     8470 2023-04-20 04:52:56.000000 vdna-0.1.1/src/vdna/utils/im.py
+-rw-rw----   0 mattwidojo  (1005) jattias   (1005)      843 2023-04-20 04:52:56.000000 vdna-0.1.1/src/vdna/utils/io.py
+-rw-rw----   0 mattwidojo  (1005) jattias   (1005)     1514 2023-04-20 04:52:56.000000 vdna-0.1.1/src/vdna/utils/settings.py
+-rw-rw----   0 mattwidojo  (1005) jattias   (1005)     3886 2023-04-20 04:52:56.000000 vdna-0.1.1/src/vdna/utils/stats.py
+-rw-rw----   0 mattwidojo  (1005) jattias   (1005)      942 2023-04-20 04:52:56.000000 vdna-0.1.1/src/vdna/utils/utils.py
+-rw-rw----   0 mattwidojo  (1005) jattias   (1005)     5843 2023-04-20 04:52:56.000000 vdna-0.1.1/src/vdna/vdna_processor.py
+drwxrwx---   0 mattwidojo  (1005) jattias   (1005)        0 2023-05-02 02:32:27.044177 vdna-0.1.1/src/vdna/vdnas/
+-rw-rw----   0 mattwidojo  (1005) jattias   (1005)      673 2023-05-02 02:31:05.000000 vdna-0.1.1/src/vdna/vdnas/__init__.py
+-rw-rw----   0 mattwidojo  (1005) jattias   (1005)     2887 2023-05-02 02:31:05.000000 vdna-0.1.1/src/vdna/vdnas/vdna_activation_ranges.py
+-rw-rw----   0 mattwidojo  (1005) jattias   (1005)     4206 2023-04-20 04:52:56.000000 vdna-0.1.1/src/vdna/vdnas/vdna_base.py
+-rw-rw----   0 mattwidojo  (1005) jattias   (1005)     2892 2023-04-20 04:52:56.000000 vdna-0.1.1/src/vdna/vdnas/vdna_gauss.py
+-rw-rw----   0 mattwidojo  (1005) jattias   (1005)     2304 2023-04-20 04:52:56.000000 vdna-0.1.1/src/vdna/vdnas/vdna_hist.py
+-rw-rw----   0 mattwidojo  (1005) jattias   (1005)     2443 2023-04-20 04:52:56.000000 vdna-0.1.1/src/vdna/vdnas/vdna_layer_gauss.py
+-rw-rw----   0 mattwidojo  (1005) jattias   (1005)       36 2023-05-02 02:32:13.000000 vdna-0.1.1/src/vdna/version.py
+drwxrwx---   0 mattwidojo  (1005) jattias   (1005)        0 2023-05-02 02:32:26.820168 vdna-0.1.1/src/vdna.egg-info/
+-rw-rw----   0 mattwidojo  (1005) jattias   (1005)    10781 2023-05-02 02:32:26.000000 vdna-0.1.1/src/vdna.egg-info/PKG-INFO
+-rw-rw----   0 mattwidojo  (1005) jattias   (1005)      904 2023-05-02 02:32:26.000000 vdna-0.1.1/src/vdna.egg-info/SOURCES.txt
+-rw-rw----   0 mattwidojo  (1005) jattias   (1005)        1 2023-05-02 02:32:26.000000 vdna-0.1.1/src/vdna.egg-info/dependency_links.txt
+-rw-rw----   0 mattwidojo  (1005) jattias   (1005)       86 2023-05-02 02:32:26.000000 vdna-0.1.1/src/vdna.egg-info/requires.txt
+-rw-rw----   0 mattwidojo  (1005) jattias   (1005)        5 2023-05-02 02:32:26.000000 vdna-0.1.1/src/vdna.egg-info/top_level.txt
+drwxrwx---   0 mattwidojo  (1005) jattias   (1005)        0 2023-05-02 02:32:27.060178 vdna-0.1.1/tests/
+-rw-rw----   0 mattwidojo  (1005) jattias   (1005)     6652 2023-05-02 02:31:05.000000 vdna-0.1.1/tests/test_all.py
```

### Comparing `vdna-0.1.0b0/LICENSE` & `vdna-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vdna-0.1.0b0/PKG-INFO` & `vdna-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdna
-Version: 0.1.0b0
+Version: 0.1.1
 Summary: A package to compute and compare Visual DNAs, an approach to represent images.
 Author-email: Benjamin Ramtoula <benjamin@robots.ox.ac.uk>
 Project-URL: Homepage, https://github.com/bramtoula/vdna
 Project-URL: Bug Tracker, https://github.com/bramtoula/vdna/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,42 +15,52 @@
 # Visual DNA 🧬
 ## Introduction
 This repository provides a library to compute and compare Visual Distribution of Neuron Activations (VDNAs).
 Visuals DNAs allow comparing datasets or images using distributions of neuron activations throughout layers of a feature extractor.
 They can be used as an alternative to FID and provide more holistic and granular comparisons.
 
 <p align="center">
-  <img src=docs/demo.gif />
+  <img src=docs/vis/demo.gif />
 </p>
 
 VDNAs are generated by passing images to represent through a frozen pre-trained feature extractor network and monitoring activation values throughout the network.
 We can represent the images efficiently by fitting distributions such as histograms or Gaussians to the activations at each neuron.
 Because VDNAs keep neuron activations independent, we can compare VDNAs while focusing on neurons that are more relevant to the tasks at hand.
 
 <p align="center">
-  <img src=docs/dna-overview.svg  width="700"/>
+  <img src=docs/vis/dna-overview.svg  width="700"/>
 </p>
 
 For example, we can compare VDNAs to find similar datasets based on attributes of interest selected through specific combinations of neurons.
 
 <p align="center">
-  <img src=docs/usecase_overview_a.svg  width="400" />  
+  <img src=docs/vis/usecase_overview_a.svg  width="400" />  
 
 We can also represent individual images and check their similarity to datasets or other images.
 
 <p align="center">
-  <img src=docs/usecase_overview_b.svg  width="400"/>
+  <img src=docs/vis/usecase_overview_b.svg  width="400"/>
 </p>
 
 ## Resources
 This work was introduced in our paper:  
-Visual DNA: Representing and Comparing Images using Distributions of Neuron Activations  
+[Visual DNA: Representing and Comparing Images using Distributions of Neuron Activations](https://arxiv.org/abs/2304.10036)  
 [Benjamin Ramtoula](https://bramtoula.github.io), [Matthew Gadd](https://mttgdd.github.io/), [Paul Newman](https://www.ori.ox.ac.uk/people/paul-newman/), [Daniele de Martini](https://danieledema.github.io/)  
 CVPR 2023  
 
+Please consider citing our paper if you make use of this project in your research.
+```
+@article{ramtoula2023vdna,
+  author    = {Ramtoula, Benjamin and Gadd, Matthew and Newman, Paul and De Martini, Daniele},
+  title     = {Visual DNA: Representing and Comparing Images using Distributions of Neuron Activations},
+  journal   = {CVPR},
+  year      = {2023},
+}
+```
+
 You can also visit the [project website](https://bramtoula.github.io/vdna/).
 
 
 # Installation
 Visual DNA can be installed using pip:
 ```
 pip install vdna
@@ -201,14 +211,17 @@
 - `gaussian`: 
   - This uses a Gaussian for each neuron, as in the paper.
   - Can be compared with the neuron-wise Fréchet Distance: `from vdna import NFD`.
 - `layer-gaussian`:
   - This fits a multivariate Gaussian for each selected layer of the feature extractor.
   - Can be compared with the neuron-wise Fréchet Distance: `from vdna import NFD`.
   - Can be compared with the layer-wise Fréchet Distance (to reproduce FID for example): `from vdna import FD`.
+- `activation-ranges`:
+  - This keeps track of minimum and maximum activation values for each neuron.
+  - Can be useful to get neuron activation ranges used for normalisation for histograms (see [documentation about adding your feature extractor](docs/add_your_feature_extractor.md))
 
 
 ## FID computation
 The commonly used Fréchet Inception Distance (FID) can be computed by creating VDNAs with the `inception` feature extractor and the `layer-gaussian` distribution.
 It can then be computed using the `FD` function on layer `block_3`.
 
 For example:
```

### Comparing `vdna-0.1.0b0/README.md` & `vdna-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,52 @@
 # Visual DNA 🧬
 ## Introduction
 This repository provides a library to compute and compare Visual Distribution of Neuron Activations (VDNAs).
 Visuals DNAs allow comparing datasets or images using distributions of neuron activations throughout layers of a feature extractor.
 They can be used as an alternative to FID and provide more holistic and granular comparisons.
 
 <p align="center">
-  <img src=docs/demo.gif />
+  <img src=docs/vis/demo.gif />
 </p>
 
 VDNAs are generated by passing images to represent through a frozen pre-trained feature extractor network and monitoring activation values throughout the network.
 We can represent the images efficiently by fitting distributions such as histograms or Gaussians to the activations at each neuron.
 Because VDNAs keep neuron activations independent, we can compare VDNAs while focusing on neurons that are more relevant to the tasks at hand.
 
 <p align="center">
-  <img src=docs/dna-overview.svg  width="700"/>
+  <img src=docs/vis/dna-overview.svg  width="700"/>
 </p>
 
 For example, we can compare VDNAs to find similar datasets based on attributes of interest selected through specific combinations of neurons.
 
 <p align="center">
-  <img src=docs/usecase_overview_a.svg  width="400" />  
+  <img src=docs/vis/usecase_overview_a.svg  width="400" />  
 
 We can also represent individual images and check their similarity to datasets or other images.
 
 <p align="center">
-  <img src=docs/usecase_overview_b.svg  width="400"/>
+  <img src=docs/vis/usecase_overview_b.svg  width="400"/>
 </p>
 
 ## Resources
 This work was introduced in our paper:  
-Visual DNA: Representing and Comparing Images using Distributions of Neuron Activations  
+[Visual DNA: Representing and Comparing Images using Distributions of Neuron Activations](https://arxiv.org/abs/2304.10036)  
 [Benjamin Ramtoula](https://bramtoula.github.io), [Matthew Gadd](https://mttgdd.github.io/), [Paul Newman](https://www.ori.ox.ac.uk/people/paul-newman/), [Daniele de Martini](https://danieledema.github.io/)  
 CVPR 2023  
 
+Please consider citing our paper if you make use of this project in your research.
+```
+@article{ramtoula2023vdna,
+  author    = {Ramtoula, Benjamin and Gadd, Matthew and Newman, Paul and De Martini, Daniele},
+  title     = {Visual DNA: Representing and Comparing Images using Distributions of Neuron Activations},
+  journal   = {CVPR},
+  year      = {2023},
+}
+```
+
 You can also visit the [project website](https://bramtoula.github.io/vdna/).
 
 
 # Installation
 Visual DNA can be installed using pip:
 ```
 pip install vdna
@@ -187,14 +197,17 @@
 - `gaussian`: 
   - This uses a Gaussian for each neuron, as in the paper.
   - Can be compared with the neuron-wise Fréchet Distance: `from vdna import NFD`.
 - `layer-gaussian`:
   - This fits a multivariate Gaussian for each selected layer of the feature extractor.
   - Can be compared with the neuron-wise Fréchet Distance: `from vdna import NFD`.
   - Can be compared with the layer-wise Fréchet Distance (to reproduce FID for example): `from vdna import FD`.
+- `activation-ranges`:
+  - This keeps track of minimum and maximum activation values for each neuron.
+  - Can be useful to get neuron activation ranges used for normalisation for histograms (see [documentation about adding your feature extractor](docs/add_your_feature_extractor.md))
 
 
 ## FID computation
 The commonly used Fréchet Inception Distance (FID) can be computed by creating VDNAs with the `inception` feature extractor and the `layer-gaussian` distribution.
 It can then be computed using the `FD` function on layer `block_3`.
 
 For example:
```

### Comparing `vdna-0.1.0b0/pyproject.toml` & `vdna-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vdna"
-version = "0.1.0b"
+version = "0.1.1"
 authors = [
   { name="Benjamin Ramtoula", email="benjamin@robots.ox.ac.uk" },
 ]
 description = "A package to compute and compare Visual DNAs, an approach to represent images."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `vdna-0.1.0b0/src/vdna/distances.py` & `vdna-0.1.1/src/vdna/distances.py`

 * *Files identical despite different names*

### Comparing `vdna-0.1.0b0/src/vdna/networks/__init__.py` & `vdna-0.1.1/src/vdna/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `vdna-0.1.0b0/src/vdna/networks/clip.py` & `vdna-0.1.1/src/vdna/networks/clip.py`

 * *Files identical despite different names*

### Comparing `vdna-0.1.0b0/src/vdna/networks/dino_resnet50.py` & `vdna-0.1.1/src/vdna/networks/dino_resnet50.py`

 * *Files identical despite different names*

### Comparing `vdna-0.1.0b0/src/vdna/networks/dino_vit.py` & `vdna-0.1.1/src/vdna/networks/dino_vit.py`

 * *Files identical despite different names*

### Comparing `vdna-0.1.0b0/src/vdna/networks/feature_extraction_model.py` & `vdna-0.1.1/src/vdna/networks/feature_extraction_model.py`

 * *Files identical despite different names*

### Comparing `vdna-0.1.0b0/src/vdna/networks/inception_pytorch.py` & `vdna-0.1.1/src/vdna/networks/inception_pytorch.py`

 * *Files identical despite different names*

### Comparing `vdna-0.1.0b0/src/vdna/networks/mugs_vit.py` & `vdna-0.1.1/src/vdna/networks/mugs_vit.py`

 * *Files identical despite different names*

### Comparing `vdna-0.1.0b0/src/vdna/networks/random_resnet50.py` & `vdna-0.1.1/src/vdna/networks/random_resnet50.py`

 * *Files identical despite different names*

### Comparing `vdna-0.1.0b0/src/vdna/networks/vgg16.py` & `vdna-0.1.1/src/vdna/networks/vgg16.py`

 * *Files identical despite different names*

### Comparing `vdna-0.1.0b0/src/vdna/utils/im.py` & `vdna-0.1.1/src/vdna/utils/im.py`

 * *Files identical despite different names*

### Comparing `vdna-0.1.0b0/src/vdna/utils/io.py` & `vdna-0.1.1/src/vdna/utils/io.py`

 * *Files identical despite different names*

### Comparing `vdna-0.1.0b0/src/vdna/utils/settings.py` & `vdna-0.1.1/src/vdna/utils/settings.py`

 * *Files identical despite different names*

### Comparing `vdna-0.1.0b0/src/vdna/utils/stats.py` & `vdna-0.1.1/src/vdna/utils/stats.py`

 * *Files identical despite different names*

### Comparing `vdna-0.1.0b0/src/vdna/utils/utils.py` & `vdna-0.1.1/src/vdna/utils/utils.py`

 * *Files identical despite different names*

### Comparing `vdna-0.1.0b0/src/vdna/vdna_processor.py` & `vdna-0.1.1/src/vdna/vdna_processor.py`

 * *Files identical despite different names*

### Comparing `vdna-0.1.0b0/src/vdna/vdnas/__init__.py` & `vdna-0.1.1/src/vdna/vdnas/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from .vdna_activation_ranges import VDNAActivationRanges
 from .vdna_base import VDNA
 from .vdna_gauss import VDNAGauss
 from .vdna_hist import VDNAHist
 from .vdna_layer_gauss import VDNALayerGauss
 
 
 def get_vdna(dist_name):
@@ -9,9 +10,11 @@
         return VDNALayerGauss()
     elif dist_name == "gaussian":
         return VDNAGauss()
     elif "histogram" in dist_name:
         n_bins = int(dist_name.split("-")[1])
         assert n_bins
         return VDNAHist(hist_nb_bins=n_bins)
+    elif dist_name == "activation-ranges":
+        return VDNAActivationRanges()
     else:
         raise NotImplementedError("VDNA {} not implemented!".format(dist_name))
```

### Comparing `vdna-0.1.0b0/src/vdna/vdnas/vdna_base.py` & `vdna-0.1.1/src/vdna/vdnas/vdna_base.py`

 * *Files identical despite different names*

### Comparing `vdna-0.1.0b0/src/vdna/vdnas/vdna_gauss.py` & `vdna-0.1.1/src/vdna/vdnas/vdna_gauss.py`

 * *Files identical despite different names*

### Comparing `vdna-0.1.0b0/src/vdna/vdnas/vdna_hist.py` & `vdna-0.1.1/src/vdna/vdnas/vdna_hist.py`

 * *Files identical despite different names*

### Comparing `vdna-0.1.0b0/src/vdna/vdnas/vdna_layer_gauss.py` & `vdna-0.1.1/src/vdna/vdnas/vdna_layer_gauss.py`

 * *Files identical despite different names*

### Comparing `vdna-0.1.0b0/src/vdna.egg-info/PKG-INFO` & `vdna-0.1.1/src/vdna.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdna
-Version: 0.1.0b0
+Version: 0.1.1
 Summary: A package to compute and compare Visual DNAs, an approach to represent images.
 Author-email: Benjamin Ramtoula <benjamin@robots.ox.ac.uk>
 Project-URL: Homepage, https://github.com/bramtoula/vdna
 Project-URL: Bug Tracker, https://github.com/bramtoula/vdna/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,42 +15,52 @@
 # Visual DNA 🧬
 ## Introduction
 This repository provides a library to compute and compare Visual Distribution of Neuron Activations (VDNAs).
 Visuals DNAs allow comparing datasets or images using distributions of neuron activations throughout layers of a feature extractor.
 They can be used as an alternative to FID and provide more holistic and granular comparisons.
 
 <p align="center">
-  <img src=docs/demo.gif />
+  <img src=docs/vis/demo.gif />
 </p>
 
 VDNAs are generated by passing images to represent through a frozen pre-trained feature extractor network and monitoring activation values throughout the network.
 We can represent the images efficiently by fitting distributions such as histograms or Gaussians to the activations at each neuron.
 Because VDNAs keep neuron activations independent, we can compare VDNAs while focusing on neurons that are more relevant to the tasks at hand.
 
 <p align="center">
-  <img src=docs/dna-overview.svg  width="700"/>
+  <img src=docs/vis/dna-overview.svg  width="700"/>
 </p>
 
 For example, we can compare VDNAs to find similar datasets based on attributes of interest selected through specific combinations of neurons.
 
 <p align="center">
-  <img src=docs/usecase_overview_a.svg  width="400" />  
+  <img src=docs/vis/usecase_overview_a.svg  width="400" />  
 
 We can also represent individual images and check their similarity to datasets or other images.
 
 <p align="center">
-  <img src=docs/usecase_overview_b.svg  width="400"/>
+  <img src=docs/vis/usecase_overview_b.svg  width="400"/>
 </p>
 
 ## Resources
 This work was introduced in our paper:  
-Visual DNA: Representing and Comparing Images using Distributions of Neuron Activations  
+[Visual DNA: Representing and Comparing Images using Distributions of Neuron Activations](https://arxiv.org/abs/2304.10036)  
 [Benjamin Ramtoula](https://bramtoula.github.io), [Matthew Gadd](https://mttgdd.github.io/), [Paul Newman](https://www.ori.ox.ac.uk/people/paul-newman/), [Daniele de Martini](https://danieledema.github.io/)  
 CVPR 2023  
 
+Please consider citing our paper if you make use of this project in your research.
+```
+@article{ramtoula2023vdna,
+  author    = {Ramtoula, Benjamin and Gadd, Matthew and Newman, Paul and De Martini, Daniele},
+  title     = {Visual DNA: Representing and Comparing Images using Distributions of Neuron Activations},
+  journal   = {CVPR},
+  year      = {2023},
+}
+```
+
 You can also visit the [project website](https://bramtoula.github.io/vdna/).
 
 
 # Installation
 Visual DNA can be installed using pip:
 ```
 pip install vdna
@@ -201,14 +211,17 @@
 - `gaussian`: 
   - This uses a Gaussian for each neuron, as in the paper.
   - Can be compared with the neuron-wise Fréchet Distance: `from vdna import NFD`.
 - `layer-gaussian`:
   - This fits a multivariate Gaussian for each selected layer of the feature extractor.
   - Can be compared with the neuron-wise Fréchet Distance: `from vdna import NFD`.
   - Can be compared with the layer-wise Fréchet Distance (to reproduce FID for example): `from vdna import FD`.
+- `activation-ranges`:
+  - This keeps track of minimum and maximum activation values for each neuron.
+  - Can be useful to get neuron activation ranges used for normalisation for histograms (see [documentation about adding your feature extractor](docs/add_your_feature_extractor.md))
 
 
 ## FID computation
 The commonly used Fréchet Inception Distance (FID) can be computed by creating VDNAs with the `inception` feature extractor and the `layer-gaussian` distribution.
 It can then be computed using the `FD` function on layer `block_3`.
 
 For example:
```

### Comparing `vdna-0.1.0b0/src/vdna.egg-info/SOURCES.txt` & `vdna-0.1.1/src/vdna.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -21,12 +21,13 @@
 src/vdna/networks/vgg16.py
 src/vdna/utils/im.py
 src/vdna/utils/io.py
 src/vdna/utils/settings.py
 src/vdna/utils/stats.py
 src/vdna/utils/utils.py
 src/vdna/vdnas/__init__.py
+src/vdna/vdnas/vdna_activation_ranges.py
 src/vdna/vdnas/vdna_base.py
 src/vdna/vdnas/vdna_gauss.py
 src/vdna/vdnas/vdna_hist.py
 src/vdna/vdnas/vdna_layer_gauss.py
 tests/test_all.py
```

