# Comparing `tmp/pyVIA-0.1.82.tar.gz` & `tmp/pyVIA-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyVIA-0.1.82.tar", last modified: Tue May  2 02:00:06 2023, max compression
+gzip compressed data, was "dist/pyVIA-0.1.9.tar", last modified: Tue Jan 19 04:52:20 2021, max compression
```

## Comparing `pyVIA-0.1.82.tar` & `pyVIA-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,14 @@
-drwxrwxr-x   0 shobi     (1001) shobi     (1001)        0 2023-05-02 02:00:06.000000 pyVIA-0.1.82/
--rw-rw-r--   0 shobi     (1001) shobi     (1001)       38 2023-05-02 02:00:06.000000 pyVIA-0.1.82/setup.cfg
--rw-rw-r--   0 shobi     (1001) shobi     (1001)      900 2023-05-02 01:59:01.000000 pyVIA-0.1.82/setup.py
--rw-rw-r--   0 shobi     (1001) shobi     (1001)    19436 2021-04-06 08:42:30.000000 pyVIA-0.1.82/README.md
--rw-rw-r--   0 shobi     (1001) shobi     (1001)    21668 2023-05-02 02:00:06.000000 pyVIA-0.1.82/PKG-INFO
-drwxrwxr-x   0 shobi     (1001) shobi     (1001)        0 2023-05-02 02:00:06.000000 pyVIA-0.1.82/pyVIA.egg-info/
--rw-rw-r--   0 shobi     (1001) shobi     (1001)      193 2023-05-02 02:00:05.000000 pyVIA-0.1.82/pyVIA.egg-info/requires.txt
--rw-rw-r--   0 shobi     (1001) shobi     (1001)        1 2023-05-02 02:00:05.000000 pyVIA-0.1.82/pyVIA.egg-info/dependency_links.txt
--rw-rw-r--   0 shobi     (1001) shobi     (1001)        6 2023-05-02 02:00:05.000000 pyVIA-0.1.82/pyVIA.egg-info/top_level.txt
--rw-rw-r--   0 shobi     (1001) shobi     (1001)      292 2023-05-02 02:00:05.000000 pyVIA-0.1.82/pyVIA.egg-info/SOURCES.txt
--rw-rw-r--   0 shobi     (1001) shobi     (1001)    21668 2023-05-02 02:00:05.000000 pyVIA-0.1.82/pyVIA.egg-info/PKG-INFO
-drwxrwxr-x   0 shobi     (1001) shobi     (1001)        0 2023-05-02 02:00:06.000000 pyVIA-0.1.82/pyVIA/
--rw-rw-r--   0 shobi     (1001) shobi     (1001)      143 2022-08-26 05:48:14.000000 pyVIA-0.1.82/pyVIA/__init__.py
--rw-rw-r--   0 shobi     (1001) shobi     (1001)    75009 2023-04-24 08:14:12.000000 pyVIA-0.1.82/pyVIA/utils_via.py
--rw-rw-r--   0 shobi     (1001) shobi     (1001)     7987 2022-03-16 04:16:24.000000 pyVIA-0.1.82/pyVIA/windmap.py
--rw-rw-r--   0 shobi     (1001) shobi     (1001)   149975 2023-05-02 01:57:31.000000 pyVIA-0.1.82/pyVIA/plotting_via.py
--rw-rw-r--   0 shobi     (1001) shobi     (1001)   160718 2023-02-22 09:50:18.000000 pyVIA-0.1.82/pyVIA/examples.py
--rw-rw-r--   0 shobi     (1001) shobi     (1001)   195116 2023-05-02 01:58:38.000000 pyVIA-0.1.82/pyVIA/core.py
--rw-rw-r--   0 shobi     (1001) shobi     (1001)     9598 2022-12-12 04:55:33.000000 pyVIA-0.1.82/pyVIA/datasets_via.py
+drwxrwxr-x   0 shobi     (1001) shobi     (1001)        0 2021-01-19 04:52:20.000000 pyVIA-0.1.9/
+-rw-rw-r--   0 shobi     (1001) shobi     (1001)       38 2021-01-19 04:52:20.000000 pyVIA-0.1.9/setup.cfg
+-rw-rw-r--   0 shobi     (1001) shobi     (1001)      831 2021-01-19 04:50:44.000000 pyVIA-0.1.9/setup.py
+-rw-rw-r--   0 shobi     (1001) shobi     (1001)    15408 2021-01-19 04:51:47.000000 pyVIA-0.1.9/README.md
+-rw-rw-r--   0 shobi     (1001) shobi     (1001)    17255 2021-01-19 04:52:20.000000 pyVIA-0.1.9/PKG-INFO
+drwxrwxr-x   0 shobi     (1001) shobi     (1001)        0 2021-01-19 04:52:20.000000 pyVIA-0.1.9/pyVIA.egg-info/
+-rw-rw-r--   0 shobi     (1001) shobi     (1001)      138 2021-01-19 04:52:19.000000 pyVIA-0.1.9/pyVIA.egg-info/requires.txt
+-rw-rw-r--   0 shobi     (1001) shobi     (1001)        1 2021-01-19 04:52:19.000000 pyVIA-0.1.9/pyVIA.egg-info/dependency_links.txt
+-rw-rw-r--   0 shobi     (1001) shobi     (1001)        6 2021-01-19 04:52:19.000000 pyVIA-0.1.9/pyVIA.egg-info/top_level.txt
+-rw-rw-r--   0 shobi     (1001) shobi     (1001)      194 2021-01-19 04:52:19.000000 pyVIA-0.1.9/pyVIA.egg-info/SOURCES.txt
+-rw-rw-r--   0 shobi     (1001) shobi     (1001)    17255 2021-01-19 04:52:19.000000 pyVIA-0.1.9/pyVIA.egg-info/PKG-INFO
+drwxrwxr-x   0 shobi     (1001) shobi     (1001)        0 2021-01-19 04:52:20.000000 pyVIA-0.1.9/pyVIA/
+-rw-rw-r--   0 shobi     (1001) shobi     (1001)       19 2020-09-15 07:09:22.000000 pyVIA-0.1.9/pyVIA/__init__.py
+-rw-rw-r--   0 shobi     (1001) shobi     (1001)   293535 2021-01-19 04:50:36.000000 pyVIA-0.1.9/pyVIA/core.py
```

### Comparing `pyVIA-0.1.82/setup.py` & `pyVIA-0.1.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='pyVIA',
-    version='0.1.82', #May-2-2023
+    version='0.1.9', #18-Jan-2021
     packages=['pyVIA',],
     license='MIT',
     author_email = 'shobana.venkat88@gmail.com',
     url = 'https://github.com/ShobiStassen/VIA',
     setup_requires = ['numpy>=1.17','pybind11'],
-    install_requires=['pybind11','numpy>=1.17','scipy','pandas>=0.25','hnswlib','igraph','leidenalg>=0.7.0', 'scikit-learn', 'termcolor','pygam', 'matplotlib','scanpy','umap-learn>=0.5.0','phate','datashader', 'scikit-image', 'pillow','wget','gdown','seaborn'],
+    install_requires=['pybind11','numpy>=1.17','scipy','pandas>=0.25','hnswlib','python-igraph','leidenalg>=0.7.0', 'sklearn', 'termcolor','pygam', 'matplotlib','scanpy','umap-learn','phate'],
     long_description=long_description,
     long_description_content_type='text/markdown'
 )
```

### Comparing `pyVIA-0.1.82/README.md` & `pyVIA-0.1.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,123 +1,75 @@
-# VIA
-VIA is a single-cell Trajectory Inference method that offers topology construction, pseudotimes, automated terminal state prediction and automated plotting of temporal gene dynamics along lineages. VIA combines lazy-teleporting random walks and Monte-Carlo Markov Chain simulations to overcome common challenges such as 1) accurate terminal state and lineage inference, 2) ability to capture combination of cyclic, disconnected and tree-like structures, 3) scalability in feature and sample space. 4) Generalizability to multi-omic analysis. In addition to transcriptomic data, VIA works on scATAC-seq, flow and imaging cytometry data. 
-Please refer to our [paper](https://www.biorxiv.org/content/10.1101/2021.02.10.430705v1) for more details.
+# Via
+VIA is a single-cell Trajectory Inference method that offers topology construction, pseudotimes, automated terminal state prediction and automated plotting of temporal gene dynamics along lineages. VIA combines lazy-teleporting random walks and Monte-Carlo Markov Chain simulations to overcome common challenges such as 1) accurate terminal state and lineage inference, 2) ability to capture combination of cyclic, disconnected and tree-like structures, 3) scalability in feature and sample space. It is also well-suited for multi-omic analysis. In addition to transcriptomic data, VIA works on scATAC-seq, flow and imaging cytometry data 
 
 ## Getting Started
-### Linux Ubuntu 16.04 and Windows 10 Installation
+### install using pip takes a few minutes on a clean environment
 We recommend setting up a new conda environment
 ```
-conda create --name ViaEnv python=3.7 
-pip install pyVIA // tested on linux Ubuntu 16.04 and Windows 10
+conda create --name ViaEnv pip 
+pip install pyVIA // tested on linux
 ```
 This usually tries to install hnswlib, produces an error and automatically corrects itself by first installing pybind11 followed by hnswlib. To get a smoother installation, consider installing in the following order after creating a new conda environment:
 ```
 pip install pybind11
 pip install hnswlib
 pip install pyVIA
 ```
 ### install by cloning repository and running setup.py (ensure dependencies are installed)
 ```
 git clone https://github.com/ShobiStassen/VIA.git 
-python3 setup.py install // cd into the directory of the cloned VIA folder containing setup.py and issue this command
+python3 setup.py install // cd into the directory of the cloned PARC folder containing setup.py and issue this command
 ```
 
-### MAC installation
-The pie-chart cluster-graph plot does not render correctly for MACs for the time-being. All other outputs are as expected. 
+### install dependencies separately if needed (linux)
+If the pip install doesn't work, it usually suffices to first install all the requirements (using pip) and subsequently install VIA (also using pip)
 ```
-conda create --name ViaEnv python=3.7 
-pip install pybind11
-conda install -c conda-forge hnswlib
-pip install pyVIA
-```
-
-### install dependencies separately if needed (linux ubuntu 16.04 and Windows 10)
-If the pip install doesn't work, it usually suffices to first install all the requirements (using pip) and subsequently install VIA (also using pip). 
-Note that on Windows if you do not have Visual C++ (required for hnswlib) you can install using [this link](https://www.scivision.dev/python-windows-visual-c-14-required/) . 
-```
-pip install pybind11, hnswlib, python-igraph, leidenalg>=0.7.0, umap-learn, numpy>=1.17, scipy, pandas>=0.25, sklearn, termcolor, pygam, phate, matplotlib,scanpy
+pip install python-igraph, leidenalg>=0.7.0, pybind11, hnswlib, umap-learn, numpy>=1.17, scipy, pandas>=0.25, sklearn, termcolor, pygam, phate
 pip install pyVIA
 ```
-## Jupyter Notebooks
-There are several [Jupyter Notebooks](https://github.com/ShobiStassen/VIA/tree/master/Jupyter%20Notebooks) with step-by-step code for real and simulated datasets. If you experience issues with opening the notebook from github, then copy the Jupyter Notebook URL and paste it into nb viewer https://nbviewer.jupyter.org/
-
-## Examples 
-Expected runtime will be a few minutes or less. Runtime on a "normal" laptop ~5 minutes for EB and less for smaller data.
-Data for the Jupyter Notebooks and Examples are available in the [Datasets folder](https://github.com/ShobiStassen/VIA/tree/master/Datasets) (smaller files) and larger datasets [here](https://drive.google.com/drive/folders/1WQSZeNixUAB1Sm0Xf68ZnSLQXyep936l?usp=sharing). 
-#### 1.a Toy Data (multifurcation) [Multifurcation Jupyter NB](https://github.com/ShobiStassen/VIA/blob/master/Jupyter%20Notebooks/ViaJupyter_Toy_Multifurcating.ipynb)
-#### 1.b Toy Data (disconnected) [Disconnected Jupyter NB](https://github.com/ShobiStassen/VIA/blob/master/Jupyter%20Notebooks/ViaJupyter_Toy_Disconnected.ipynb)
-#### 2.a Human Embryoid Bodies (wrapper function)
-#### 2.b Human Embryoid Bodies (Configuring VIA) [EB Jupyter NB](https://github.com/ShobiStassen/VIA/blob/master/Jupyter%20Notebooks/ViaJupyter_EmbryoidBody.ipynb)
-#### 3.a General input format and wrapper function
-#### 3.b General disconnected trajectories wrapper function
-#### More examples with additional code, outputs and details are available as [Jupyter Notebooks](https://github.com/ShobiStassen/VIA/tree/master/Jupyter%20Notebooks)
+## Examples (Expected runtime will be a few minutes or less. Runtime on a "normal" laptop ~5 minutes for EB and less for smaller data) 
+### 1.a Toy Data (multifurcation)
+### 1.b Toy Data (disconnected)
+### 2.a Human Embryoid Bodies (wrapper function)
+### 2.b Human Embryoid Bodies (Configuring VIA)
+### 3.a General input format and wrapper function
+### 3.b General disconnected trajectories wrapper function
 ------------------------------------------------------
 ### 1.a/b Toy data (Multifurcation and Disconnected)
-Two examples [toy datasets](https://github.com/ShobiStassen/VIA/tree/master/Datasets)  with annotations are generated using DynToy are provided. 
-
-### To run on Linux:
-All examples are shown according to Linux OS, small modifications are required to run on a Windows OS (see below)
+Two examples [toy datasets](https://drive.google.com/drive/folders/1WQSZeNixUAB1Sm0Xf68ZnSLQXyep936l?usp=sharing) with annotations are generated using DynToy are provided. 
 ```
 import pyVIA.core as via
-# ensure the data and label files are in csv format when you download/save them
 #multifurcation
 #the root is automatically set to  root_user = 'M1'
 via.main_Toy(ncomps=10, knn=30,dataset='Toy3', random_seed=2,foldername = ".../Trajectory/Datasets/") #multifurcation
 #disconnected trajectory
 #the root is automatically set as a list root_user = ['T1_M1', 'T2_M1'] # e.g. T2_M3 is a cell belonging to the 3rd Milestone (M3) of the second Trajectory (T2)
 via.main_Toy(ncomps=10, knn=30,dataset='Toy4',random_seed=2,foldername =".../Trajectory/Datasets/") #2 disconnected trajectories
 ```
-Windows (small modifications in calling the code due to the way multiprocessing works in Windows compared to Linux)
-### To run on Windows:
-A few additional lines are required:
-```
-#when running from an IDE you need to call the function in the following way to ensure the parallel processing works:
-import os
-import pyVIA.core as via
-f= os.path.join(r'C:\Users\...\Documents'+'\\')
-def main():
-    via.main_Toy(ncomps=10, knn=30,dataset='Toy3', random_seed=2,foldername= f)    
-if __name__ =='__main__':
-    main()
-    
-#when running directly from terminal:
-import os
-import pyVIA.core as via
-f= os.path.join(r'C:\Users\...\Documents'+'\\')
-via.main_Toy(ncomps=10, knn=30,dataset='Toy3', random_seed=2,foldername= f)    
-if __name__ =='__main__':
-```
-
 ## Output of Multifurcating toy dataset
 ![Output of VIA on multifurcating toy dataset](https://github.com/ShobiStassen/VIA/blob/master/Figures/Toy3_fig0.png?raw=true)
 ## Output of disconnected toy dataset
 ![Output of VIA on disconnected toy dataset](https://github.com/ShobiStassen/VIA/blob/master/Figures/Toy4_fig0.png?raw=true)
 
 ### 2.a Human Embryoid Bodies (wrapper function)
-Save the [Raw data](https://drive.google.com/file/d/1yz3zR1KAmghjYB_nLLUZoIlKN9Ew4RHf/view?usp=sharing) matrix as 'EBdata.mat'. The cells in this file have been filtered for too small/large libraries by [Moon et al. 2019](https://nbviewer.jupyter.org/github/KrishnaswamyLab/PHATE/blob/master/Python/tutorial/EmbryoidBody.ipynb). 
-
-Save the phate [embedding](https://github.com/ShobiStassen/VIA/tree/master/Datasets) which is required to run Example 2.a (since the phate operation is 
+save the [Raw data](https://drive.google.com/file/d/1yz3zR1KAmghjYB_nLLUZoIlKN9Ew4RHf/view?usp=sharing) matrix as 'EBdata.mat'. The cells in this file have been filtered for too small/large libraries by [Moon et al. 2019](https://nbviewer.jupyter.org/github/KrishnaswamyLab/PHATE/blob/master/Python/tutorial/EmbryoidBody.ipynb) 
 
 The function main_EB_clean() preprocesses the cells (normalized by library size, sqrt transformation). It then calls VIA to: plot the pseudotimes, terminal states, lineage pathways and gene-clustermap. The visualization method used in this function is PHATE.
 ```
-#runtime on single core, 8GB RAM 64bit Windows is about 8-10 minutes. This can be lowered by reducing the number of MCMC simulations (num_mcmc_simulations).
 import pyVIA.core as via
-#Windows example path for folder where EBdata.mat is saved: f= os.path.join(r'C:\Users\...\Documents'+'\\')
-via.main_EB_clean(ncomps=30, knn=20, v0_random_seed=24, foldername = f) # Most reasonable parameters of ncomps (10-200) and knn (15-50) work well
+via.main_EB_clean(ncomps=30, knn=20, p0_random_seed=20, foldername = '') # Most reasonable parameters of ncomps (10-200) and knn (15-50) work well
 ```
 ### 2.b Human Embryoid Bodies (Configuring VIA)
-If you wish to run the data using UMAP or TSNE (instead of PHATE), or require more control of the parameters/outputs, then use the following code. (See the Jupyter Notebook for detailed output and code). Expected runtime will be around 1-2 minutes using 5 cores, or ~8-10 on "normal" laptop. .
+If you wish to run the data using UMAP or TSNE (instead of PHATE), or require more control of the parameters/outputs, then use the following code:
+Expected runtime will be around 2 minutes
 ```
 import pyVIA.core as via
 #pre-process the data as needed and provide to via as a numpy array
 #root_user is the index of the cell corresponding to a suitable start/root cell
 
-v0_too_big = 0.3 #clusters comprising more than 30% of total cell population will be re-clustered by PARC
-v1_too_big = 0.05
-
 v0 = via.VIA(input_data, time_labels, jac_std_global=0.15, dist_std_local=1, knn=knn,
              too_big_factor=v0_too_big, root_user=[1], dataset='EB', random_seed=v0_random_seed,
              do_magic_bool=True, is_coarse=True, preserve_disconnected=True)  
 v0.run_VIA()
 
 
 tsi_list = get_loc_terminal_states(v0, input_data) #translate the terminal clusters found in v0 to the fine-grained run in v1
@@ -174,15 +126,15 @@
 
 # use UMAP or PHate to obtain embedding that is used for single-cell level visualization
 embedding = umap.UMAP(random_state=42, n_neighbors=15, init='random').fit_transform(data.values[:, 0:5])
 
 # list marker genes or genes of interest if known in advance. otherwise marker_genes = []
 marker_genes = ['Igll1', 'Myc', 'Slc7a5', 'Ldha', 'Foxo1', 'Lig4', 'Sp7']  # irf4 down-up
 # call VIA. We identify an early (suitable) start cell root = [42]. Can also set an arbitrary value
-via.via_wrapper(adata, true_label, embedding, knn=10, ncomps=20, jac_std_global=0.15, root=[42], dataset='',
+via.via_wrapper(adata, true_label, embedding, knn=20, ncomps=20, jac_std_global=0.15, root=[42], dataset='',
             random_seed=1,v0_toobig=0.3, v1_toobig=0.1, marker_genes=marker_genes)
 ```
 ### 3.b VIA wrapper for generic disconnected trajectory
 ```
 import scanpy as sc
 import pandas as pd
 
@@ -211,28 +163,28 @@
 ### Parameters
 
 | Input Parameter for class VIA | Description |
 | ---------- |----------|
 | `data` | (numpy.ndarray) n_samples x n_features. When using via_wrapper(), data is ANNdata object that has a PCA object adata.obsm['X_pca'][:, 0:ncomps] and ncomps is the number of components that will be used. |
 | `true_label` | (list) 'ground truth' annotations or placeholder|
 | `knn` |  (optional, default = 30) number of K-Nearest Neighbors for HNSWlib KNN graph |
-|`root_user`|When using one of the example datasets where there is a single root cell type, simply provide the index number of the cell corresponding to a sensible root: root_user = 1. When using the generic via wrapper, this input is in the form of a list containing roots corresponding to index (row number in cell matrix) of root cell. For most trajectories this is of the form [99], for multiple disconnected trajectories an arbitrary list of cells can be provided [1,506,1100] or VIA arbitratily chooses cells. If the root cells of disconnected trajectories are known in advance, then the cells should be annotated with similar syntax to that of Example Dataset in Disconnected Toy Example 1b.|
+|`root_user`|list containing roots corresponding to index (row number) of root cell. For most trajectories this is of the form [99], for multiple disconnected trajectories an arbitrary list of cells can be provided [1,506,1100] or VIA arbitratily chooses cells. If the root cells of disconnected trajectories are known in advance, then the cells should be annotated with similar syntax to that of Example Dataset in Disconnected Toy Example 1b.|
 | `dist_std_local` |  (optional, default = 1) local pruning threshold for PARC clustering stage: the number of standard deviations above the mean minkowski distance between neighbors of a given node. the higher the parameter, the more edges are retained|
 | `jac_std_global` |  (optional, default = 0.15) global level  graph pruning for PARC clustering stage. This threshold can also be set as the number of standard deviations below the network's mean-jaccard-weighted edges. 0.1-1 provide reasonable pruning. higher value means less pruning. e.g. a value of 0.15 means all edges that are above mean(edgeweight)-0.15*std(edge-weights) are retained. We find both 0.15 and 'median' to yield good results resulting in pruning away ~ 50-60% edges |
 | `too_big_factor` |  (optional, default = 0.4) if a cluster exceeds this share of the entire cell population, then the PARC will be run on the large cluster|
 |`x_lazy`| (optional, default = 0.95) 1-x = probability of staying in same node (lazy). Values between 0.9-0.99 are reasonable|
 |`alpha_teleport`| (optional, default = 0.99) 1-alpha is probability of jumping. Values between 0.95-0.99 are reasonable unless prior knowledge of teleportation 
 | `distance` |  (optional, default = 'l2' euclidean) 'ip','cosine'|
 | `random_seed` |  (optional, default = 42) The random seed to pass to Leiden|
 | `pseudotime_threshold_TS` |  (optional, default = 30) Percentile threshold for potential node to qualify as Terminal State|
 | `resolution_parameter` |  (optional, default = 1) Uses ModuliartyVP and RBConfigurationVertexPartition|
 | `preserve_disconnected_after_pruning` |  (optional, default = False) Cluster-graph pruning can occasionally cause fragmentation that can be repaired (by setting to True) by retaining select edges. |
 |`cluster_graph_pruning_std`| (optional, default =0.15) Usually set to the same value as the PARC clustering level of jac_std_global. To retain more connectivity in the graph underlying the trajectory computations, increase the value|
 |`visual_cluster_graph_pruning`| (optional, default = 0.15) Usually set to the same value as the PARC clustering level of jac_std_global. This does not impact computation of terminal states, pseudotime or lineage likelihoods. It controls the number of edges plotted for visual effect|
-|`num_sim_branch_probability`|(optional), default = 500. Number of MCMCs run per terminal state. This can be safely reduced to 100 when computational resources are limited|
+
 As shown in the examples, VIA is built to run on a single or double iteration. For extremely large datasets (>1M cells), a single pass is favourable. For mid-size it can be useful to run the double-pass mode which is shown in Example 2b and 3a,b. In the first pass VIA performs a coarser clustering which is useful for capturing terminal states. To increase the resolution of the pseudotime, lineage likelihood and gene trends, we re-run VIA in a second pass which produces a finer cluster-graph and transfers the lineages (terminal states) obtained in the first pass into the second pass. We therefore provide the second pass with the terminal_states obtained in the first pass. To speed up the computation, we also pass the original HNSW KNN graph. The following parameters are used for second passes.
 
 | Input Parameter | Description |
 | ---------- |----------|
 | `is_coarse` |  (optional, default = True) If running VIA in two steps, for the second fine-grained, set to "False'|
 |`super_cluster_labels`| Set this to v0.labels (clustering output of first pass "v0")|
 |`super_terminal_cells`| super_terminal_cells = via.get_loc_terminal_states(v0, data)|
@@ -242,9 +194,8 @@
 |`csr_array_locally_pruned`|csr_array_locally_pruned=v0.csr_array_locally_pruned. CSR matrix of the locally pruned KNN graph|
 
 | Attributes | Description |
 | ---------- |----------|
 | `labels` | (list) length n_samples of corresponding cluster labels |
 | `edgelist_maxout` | (list) used to draw trajectories on the 2D embedding |
 | `single_cell_pt_markov` | (list) computed pseudotime|
-|`single_cell_bp`|(array) computed single cell branch probabilities (lineage likelihoods). n_cells x n_terminal states. The columns each correspond to a terminal state, in the same order presented in the'terminal_clusters' attribute|
-| `terminal clusters` | (list) terminal clusters found by VIA|
+| `terminal clusters` | (list) terminal clusters found by VIA|
```

### Comparing `pyVIA-0.1.82/PKG-INFO` & `pyVIA-0.1.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,130 +1,82 @@
 Metadata-Version: 2.1
 Name: pyVIA
-Version: 0.1.82
+Version: 0.1.9
 Summary: UNKNOWN
 Home-page: https://github.com/ShobiStassen/VIA
 Author-email: shobana.venkat88@gmail.com
 License: MIT
-Description: # VIA
-        VIA is a single-cell Trajectory Inference method that offers topology construction, pseudotimes, automated terminal state prediction and automated plotting of temporal gene dynamics along lineages. VIA combines lazy-teleporting random walks and Monte-Carlo Markov Chain simulations to overcome common challenges such as 1) accurate terminal state and lineage inference, 2) ability to capture combination of cyclic, disconnected and tree-like structures, 3) scalability in feature and sample space. 4) Generalizability to multi-omic analysis. In addition to transcriptomic data, VIA works on scATAC-seq, flow and imaging cytometry data. 
-        Please refer to our [paper](https://www.biorxiv.org/content/10.1101/2021.02.10.430705v1) for more details.
+Description: # Via
+        VIA is a single-cell Trajectory Inference method that offers topology construction, pseudotimes, automated terminal state prediction and automated plotting of temporal gene dynamics along lineages. VIA combines lazy-teleporting random walks and Monte-Carlo Markov Chain simulations to overcome common challenges such as 1) accurate terminal state and lineage inference, 2) ability to capture combination of cyclic, disconnected and tree-like structures, 3) scalability in feature and sample space. It is also well-suited for multi-omic analysis. In addition to transcriptomic data, VIA works on scATAC-seq, flow and imaging cytometry data 
         
         ## Getting Started
-        ### Linux Ubuntu 16.04 and Windows 10 Installation
+        ### install using pip takes a few minutes on a clean environment
         We recommend setting up a new conda environment
         ```
-        conda create --name ViaEnv python=3.7 
-        pip install pyVIA // tested on linux Ubuntu 16.04 and Windows 10
+        conda create --name ViaEnv pip 
+        pip install pyVIA // tested on linux
         ```
         This usually tries to install hnswlib, produces an error and automatically corrects itself by first installing pybind11 followed by hnswlib. To get a smoother installation, consider installing in the following order after creating a new conda environment:
         ```
         pip install pybind11
         pip install hnswlib
         pip install pyVIA
         ```
         ### install by cloning repository and running setup.py (ensure dependencies are installed)
         ```
         git clone https://github.com/ShobiStassen/VIA.git 
-        python3 setup.py install // cd into the directory of the cloned VIA folder containing setup.py and issue this command
+        python3 setup.py install // cd into the directory of the cloned PARC folder containing setup.py and issue this command
         ```
         
-        ### MAC installation
-        The pie-chart cluster-graph plot does not render correctly for MACs for the time-being. All other outputs are as expected. 
+        ### install dependencies separately if needed (linux)
+        If the pip install doesn't work, it usually suffices to first install all the requirements (using pip) and subsequently install VIA (also using pip)
         ```
-        conda create --name ViaEnv python=3.7 
-        pip install pybind11
-        conda install -c conda-forge hnswlib
-        pip install pyVIA
-        ```
-        
-        ### install dependencies separately if needed (linux ubuntu 16.04 and Windows 10)
-        If the pip install doesn't work, it usually suffices to first install all the requirements (using pip) and subsequently install VIA (also using pip). 
-        Note that on Windows if you do not have Visual C++ (required for hnswlib) you can install using [this link](https://www.scivision.dev/python-windows-visual-c-14-required/) . 
-        ```
-        pip install pybind11, hnswlib, python-igraph, leidenalg>=0.7.0, umap-learn, numpy>=1.17, scipy, pandas>=0.25, sklearn, termcolor, pygam, phate, matplotlib,scanpy
+        pip install python-igraph, leidenalg>=0.7.0, pybind11, hnswlib, umap-learn, numpy>=1.17, scipy, pandas>=0.25, sklearn, termcolor, pygam, phate
         pip install pyVIA
         ```
-        ## Jupyter Notebooks
-        There are several [Jupyter Notebooks](https://github.com/ShobiStassen/VIA/tree/master/Jupyter%20Notebooks) with step-by-step code for real and simulated datasets. If you experience issues with opening the notebook from github, then copy the Jupyter Notebook URL and paste it into nb viewer https://nbviewer.jupyter.org/
-        
-        ## Examples 
-        Expected runtime will be a few minutes or less. Runtime on a "normal" laptop ~5 minutes for EB and less for smaller data.
-        Data for the Jupyter Notebooks and Examples are available in the [Datasets folder](https://github.com/ShobiStassen/VIA/tree/master/Datasets) (smaller files) and larger datasets [here](https://drive.google.com/drive/folders/1WQSZeNixUAB1Sm0Xf68ZnSLQXyep936l?usp=sharing). 
-        #### 1.a Toy Data (multifurcation) [Multifurcation Jupyter NB](https://github.com/ShobiStassen/VIA/blob/master/Jupyter%20Notebooks/ViaJupyter_Toy_Multifurcating.ipynb)
-        #### 1.b Toy Data (disconnected) [Disconnected Jupyter NB](https://github.com/ShobiStassen/VIA/blob/master/Jupyter%20Notebooks/ViaJupyter_Toy_Disconnected.ipynb)
-        #### 2.a Human Embryoid Bodies (wrapper function)
-        #### 2.b Human Embryoid Bodies (Configuring VIA) [EB Jupyter NB](https://github.com/ShobiStassen/VIA/blob/master/Jupyter%20Notebooks/ViaJupyter_EmbryoidBody.ipynb)
-        #### 3.a General input format and wrapper function
-        #### 3.b General disconnected trajectories wrapper function
-        #### More examples with additional code, outputs and details are available as [Jupyter Notebooks](https://github.com/ShobiStassen/VIA/tree/master/Jupyter%20Notebooks)
+        ## Examples (Expected runtime will be a few minutes or less. Runtime on a "normal" laptop ~5 minutes for EB and less for smaller data) 
+        ### 1.a Toy Data (multifurcation)
+        ### 1.b Toy Data (disconnected)
+        ### 2.a Human Embryoid Bodies (wrapper function)
+        ### 2.b Human Embryoid Bodies (Configuring VIA)
+        ### 3.a General input format and wrapper function
+        ### 3.b General disconnected trajectories wrapper function
         ------------------------------------------------------
         ### 1.a/b Toy data (Multifurcation and Disconnected)
-        Two examples [toy datasets](https://github.com/ShobiStassen/VIA/tree/master/Datasets)  with annotations are generated using DynToy are provided. 
-        
-        ### To run on Linux:
-        All examples are shown according to Linux OS, small modifications are required to run on a Windows OS (see below)
+        Two examples [toy datasets](https://drive.google.com/drive/folders/1WQSZeNixUAB1Sm0Xf68ZnSLQXyep936l?usp=sharing) with annotations are generated using DynToy are provided. 
         ```
         import pyVIA.core as via
-        # ensure the data and label files are in csv format when you download/save them
         #multifurcation
         #the root is automatically set to  root_user = 'M1'
         via.main_Toy(ncomps=10, knn=30,dataset='Toy3', random_seed=2,foldername = ".../Trajectory/Datasets/") #multifurcation
         #disconnected trajectory
         #the root is automatically set as a list root_user = ['T1_M1', 'T2_M1'] # e.g. T2_M3 is a cell belonging to the 3rd Milestone (M3) of the second Trajectory (T2)
         via.main_Toy(ncomps=10, knn=30,dataset='Toy4',random_seed=2,foldername =".../Trajectory/Datasets/") #2 disconnected trajectories
         ```
-        Windows (small modifications in calling the code due to the way multiprocessing works in Windows compared to Linux)
-        ### To run on Windows:
-        A few additional lines are required:
-        ```
-        #when running from an IDE you need to call the function in the following way to ensure the parallel processing works:
-        import os
-        import pyVIA.core as via
-        f= os.path.join(r'C:\Users\...\Documents'+'\\')
-        def main():
-            via.main_Toy(ncomps=10, knn=30,dataset='Toy3', random_seed=2,foldername= f)    
-        if __name__ =='__main__':
-            main()
-            
-        #when running directly from terminal:
-        import os
-        import pyVIA.core as via
-        f= os.path.join(r'C:\Users\...\Documents'+'\\')
-        via.main_Toy(ncomps=10, knn=30,dataset='Toy3', random_seed=2,foldername= f)    
-        if __name__ =='__main__':
-        ```
-        
         ## Output of Multifurcating toy dataset
         ![Output of VIA on multifurcating toy dataset](https://github.com/ShobiStassen/VIA/blob/master/Figures/Toy3_fig0.png?raw=true)
         ## Output of disconnected toy dataset
         ![Output of VIA on disconnected toy dataset](https://github.com/ShobiStassen/VIA/blob/master/Figures/Toy4_fig0.png?raw=true)
         
         ### 2.a Human Embryoid Bodies (wrapper function)
-        Save the [Raw data](https://drive.google.com/file/d/1yz3zR1KAmghjYB_nLLUZoIlKN9Ew4RHf/view?usp=sharing) matrix as 'EBdata.mat'. The cells in this file have been filtered for too small/large libraries by [Moon et al. 2019](https://nbviewer.jupyter.org/github/KrishnaswamyLab/PHATE/blob/master/Python/tutorial/EmbryoidBody.ipynb). 
-        
-        Save the phate [embedding](https://github.com/ShobiStassen/VIA/tree/master/Datasets) which is required to run Example 2.a (since the phate operation is 
+        save the [Raw data](https://drive.google.com/file/d/1yz3zR1KAmghjYB_nLLUZoIlKN9Ew4RHf/view?usp=sharing) matrix as 'EBdata.mat'. The cells in this file have been filtered for too small/large libraries by [Moon et al. 2019](https://nbviewer.jupyter.org/github/KrishnaswamyLab/PHATE/blob/master/Python/tutorial/EmbryoidBody.ipynb) 
         
         The function main_EB_clean() preprocesses the cells (normalized by library size, sqrt transformation). It then calls VIA to: plot the pseudotimes, terminal states, lineage pathways and gene-clustermap. The visualization method used in this function is PHATE.
         ```
-        #runtime on single core, 8GB RAM 64bit Windows is about 8-10 minutes. This can be lowered by reducing the number of MCMC simulations (num_mcmc_simulations).
         import pyVIA.core as via
-        #Windows example path for folder where EBdata.mat is saved: f= os.path.join(r'C:\Users\...\Documents'+'\\')
-        via.main_EB_clean(ncomps=30, knn=20, v0_random_seed=24, foldername = f) # Most reasonable parameters of ncomps (10-200) and knn (15-50) work well
+        via.main_EB_clean(ncomps=30, knn=20, p0_random_seed=20, foldername = '') # Most reasonable parameters of ncomps (10-200) and knn (15-50) work well
         ```
         ### 2.b Human Embryoid Bodies (Configuring VIA)
-        If you wish to run the data using UMAP or TSNE (instead of PHATE), or require more control of the parameters/outputs, then use the following code. (See the Jupyter Notebook for detailed output and code). Expected runtime will be around 1-2 minutes using 5 cores, or ~8-10 on "normal" laptop. .
+        If you wish to run the data using UMAP or TSNE (instead of PHATE), or require more control of the parameters/outputs, then use the following code:
+        Expected runtime will be around 2 minutes
         ```
         import pyVIA.core as via
         #pre-process the data as needed and provide to via as a numpy array
         #root_user is the index of the cell corresponding to a suitable start/root cell
         
-        v0_too_big = 0.3 #clusters comprising more than 30% of total cell population will be re-clustered by PARC
-        v1_too_big = 0.05
-        
         v0 = via.VIA(input_data, time_labels, jac_std_global=0.15, dist_std_local=1, knn=knn,
                      too_big_factor=v0_too_big, root_user=[1], dataset='EB', random_seed=v0_random_seed,
                      do_magic_bool=True, is_coarse=True, preserve_disconnected=True)  
         v0.run_VIA()
         
         
         tsi_list = get_loc_terminal_states(v0, input_data) #translate the terminal clusters found in v0 to the fine-grained run in v1
@@ -181,15 +133,15 @@
         
         # use UMAP or PHate to obtain embedding that is used for single-cell level visualization
         embedding = umap.UMAP(random_state=42, n_neighbors=15, init='random').fit_transform(data.values[:, 0:5])
         
         # list marker genes or genes of interest if known in advance. otherwise marker_genes = []
         marker_genes = ['Igll1', 'Myc', 'Slc7a5', 'Ldha', 'Foxo1', 'Lig4', 'Sp7']  # irf4 down-up
         # call VIA. We identify an early (suitable) start cell root = [42]. Can also set an arbitrary value
-        via.via_wrapper(adata, true_label, embedding, knn=10, ncomps=20, jac_std_global=0.15, root=[42], dataset='',
+        via.via_wrapper(adata, true_label, embedding, knn=20, ncomps=20, jac_std_global=0.15, root=[42], dataset='',
                     random_seed=1,v0_toobig=0.3, v1_toobig=0.1, marker_genes=marker_genes)
         ```
         ### 3.b VIA wrapper for generic disconnected trajectory
         ```
         import scanpy as sc
         import pandas as pd
         
@@ -218,28 +170,28 @@
         ### Parameters
         
         | Input Parameter for class VIA | Description |
         | ---------- |----------|
         | `data` | (numpy.ndarray) n_samples x n_features. When using via_wrapper(), data is ANNdata object that has a PCA object adata.obsm['X_pca'][:, 0:ncomps] and ncomps is the number of components that will be used. |
         | `true_label` | (list) 'ground truth' annotations or placeholder|
         | `knn` |  (optional, default = 30) number of K-Nearest Neighbors for HNSWlib KNN graph |
-        |`root_user`|When using one of the example datasets where there is a single root cell type, simply provide the index number of the cell corresponding to a sensible root: root_user = 1. When using the generic via wrapper, this input is in the form of a list containing roots corresponding to index (row number in cell matrix) of root cell. For most trajectories this is of the form [99], for multiple disconnected trajectories an arbitrary list of cells can be provided [1,506,1100] or VIA arbitratily chooses cells. If the root cells of disconnected trajectories are known in advance, then the cells should be annotated with similar syntax to that of Example Dataset in Disconnected Toy Example 1b.|
+        |`root_user`|list containing roots corresponding to index (row number) of root cell. For most trajectories this is of the form [99], for multiple disconnected trajectories an arbitrary list of cells can be provided [1,506,1100] or VIA arbitratily chooses cells. If the root cells of disconnected trajectories are known in advance, then the cells should be annotated with similar syntax to that of Example Dataset in Disconnected Toy Example 1b.|
         | `dist_std_local` |  (optional, default = 1) local pruning threshold for PARC clustering stage: the number of standard deviations above the mean minkowski distance between neighbors of a given node. the higher the parameter, the more edges are retained|
         | `jac_std_global` |  (optional, default = 0.15) global level  graph pruning for PARC clustering stage. This threshold can also be set as the number of standard deviations below the network's mean-jaccard-weighted edges. 0.1-1 provide reasonable pruning. higher value means less pruning. e.g. a value of 0.15 means all edges that are above mean(edgeweight)-0.15*std(edge-weights) are retained. We find both 0.15 and 'median' to yield good results resulting in pruning away ~ 50-60% edges |
         | `too_big_factor` |  (optional, default = 0.4) if a cluster exceeds this share of the entire cell population, then the PARC will be run on the large cluster|
         |`x_lazy`| (optional, default = 0.95) 1-x = probability of staying in same node (lazy). Values between 0.9-0.99 are reasonable|
         |`alpha_teleport`| (optional, default = 0.99) 1-alpha is probability of jumping. Values between 0.95-0.99 are reasonable unless prior knowledge of teleportation 
         | `distance` |  (optional, default = 'l2' euclidean) 'ip','cosine'|
         | `random_seed` |  (optional, default = 42) The random seed to pass to Leiden|
         | `pseudotime_threshold_TS` |  (optional, default = 30) Percentile threshold for potential node to qualify as Terminal State|
         | `resolution_parameter` |  (optional, default = 1) Uses ModuliartyVP and RBConfigurationVertexPartition|
         | `preserve_disconnected_after_pruning` |  (optional, default = False) Cluster-graph pruning can occasionally cause fragmentation that can be repaired (by setting to True) by retaining select edges. |
         |`cluster_graph_pruning_std`| (optional, default =0.15) Usually set to the same value as the PARC clustering level of jac_std_global. To retain more connectivity in the graph underlying the trajectory computations, increase the value|
         |`visual_cluster_graph_pruning`| (optional, default = 0.15) Usually set to the same value as the PARC clustering level of jac_std_global. This does not impact computation of terminal states, pseudotime or lineage likelihoods. It controls the number of edges plotted for visual effect|
-        |`num_sim_branch_probability`|(optional), default = 500. Number of MCMCs run per terminal state. This can be safely reduced to 100 when computational resources are limited|
+        
         As shown in the examples, VIA is built to run on a single or double iteration. For extremely large datasets (>1M cells), a single pass is favourable. For mid-size it can be useful to run the double-pass mode which is shown in Example 2b and 3a,b. In the first pass VIA performs a coarser clustering which is useful for capturing terminal states. To increase the resolution of the pseudotime, lineage likelihood and gene trends, we re-run VIA in a second pass which produces a finer cluster-graph and transfers the lineages (terminal states) obtained in the first pass into the second pass. We therefore provide the second pass with the terminal_states obtained in the first pass. To speed up the computation, we also pass the original HNSW KNN graph. The following parameters are used for second passes.
         
         | Input Parameter | Description |
         | ---------- |----------|
         | `is_coarse` |  (optional, default = True) If running VIA in two steps, for the second fine-grained, set to "False'|
         |`super_cluster_labels`| Set this to v0.labels (clustering output of first pass "v0")|
         |`super_terminal_cells`| super_terminal_cells = via.get_loc_terminal_states(v0, data)|
@@ -249,11 +201,11 @@
         |`csr_array_locally_pruned`|csr_array_locally_pruned=v0.csr_array_locally_pruned. CSR matrix of the locally pruned KNN graph|
         
         | Attributes | Description |
         | ---------- |----------|
         | `labels` | (list) length n_samples of corresponding cluster labels |
         | `edgelist_maxout` | (list) used to draw trajectories on the 2D embedding |
         | `single_cell_pt_markov` | (list) computed pseudotime|
-        |`single_cell_bp`|(array) computed single cell branch probabilities (lineage likelihoods). n_cells x n_terminal states. The columns each correspond to a terminal state, in the same order presented in the'terminal_clusters' attribute|
         | `terminal clusters` | (list) terminal clusters found by VIA|
+        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pyVIA-0.1.82/pyVIA.egg-info/PKG-INFO` & `pyVIA-0.1.9/pyVIA.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,130 +1,82 @@
 Metadata-Version: 2.1
 Name: pyVIA
-Version: 0.1.82
+Version: 0.1.9
 Summary: UNKNOWN
 Home-page: https://github.com/ShobiStassen/VIA
 Author-email: shobana.venkat88@gmail.com
 License: MIT
-Description: # VIA
-        VIA is a single-cell Trajectory Inference method that offers topology construction, pseudotimes, automated terminal state prediction and automated plotting of temporal gene dynamics along lineages. VIA combines lazy-teleporting random walks and Monte-Carlo Markov Chain simulations to overcome common challenges such as 1) accurate terminal state and lineage inference, 2) ability to capture combination of cyclic, disconnected and tree-like structures, 3) scalability in feature and sample space. 4) Generalizability to multi-omic analysis. In addition to transcriptomic data, VIA works on scATAC-seq, flow and imaging cytometry data. 
-        Please refer to our [paper](https://www.biorxiv.org/content/10.1101/2021.02.10.430705v1) for more details.
+Description: # Via
+        VIA is a single-cell Trajectory Inference method that offers topology construction, pseudotimes, automated terminal state prediction and automated plotting of temporal gene dynamics along lineages. VIA combines lazy-teleporting random walks and Monte-Carlo Markov Chain simulations to overcome common challenges such as 1) accurate terminal state and lineage inference, 2) ability to capture combination of cyclic, disconnected and tree-like structures, 3) scalability in feature and sample space. It is also well-suited for multi-omic analysis. In addition to transcriptomic data, VIA works on scATAC-seq, flow and imaging cytometry data 
         
         ## Getting Started
-        ### Linux Ubuntu 16.04 and Windows 10 Installation
+        ### install using pip takes a few minutes on a clean environment
         We recommend setting up a new conda environment
         ```
-        conda create --name ViaEnv python=3.7 
-        pip install pyVIA // tested on linux Ubuntu 16.04 and Windows 10
+        conda create --name ViaEnv pip 
+        pip install pyVIA // tested on linux
         ```
         This usually tries to install hnswlib, produces an error and automatically corrects itself by first installing pybind11 followed by hnswlib. To get a smoother installation, consider installing in the following order after creating a new conda environment:
         ```
         pip install pybind11
         pip install hnswlib
         pip install pyVIA
         ```
         ### install by cloning repository and running setup.py (ensure dependencies are installed)
         ```
         git clone https://github.com/ShobiStassen/VIA.git 
-        python3 setup.py install // cd into the directory of the cloned VIA folder containing setup.py and issue this command
+        python3 setup.py install // cd into the directory of the cloned PARC folder containing setup.py and issue this command
         ```
         
-        ### MAC installation
-        The pie-chart cluster-graph plot does not render correctly for MACs for the time-being. All other outputs are as expected. 
+        ### install dependencies separately if needed (linux)
+        If the pip install doesn't work, it usually suffices to first install all the requirements (using pip) and subsequently install VIA (also using pip)
         ```
-        conda create --name ViaEnv python=3.7 
-        pip install pybind11
-        conda install -c conda-forge hnswlib
-        pip install pyVIA
-        ```
-        
-        ### install dependencies separately if needed (linux ubuntu 16.04 and Windows 10)
-        If the pip install doesn't work, it usually suffices to first install all the requirements (using pip) and subsequently install VIA (also using pip). 
-        Note that on Windows if you do not have Visual C++ (required for hnswlib) you can install using [this link](https://www.scivision.dev/python-windows-visual-c-14-required/) . 
-        ```
-        pip install pybind11, hnswlib, python-igraph, leidenalg>=0.7.0, umap-learn, numpy>=1.17, scipy, pandas>=0.25, sklearn, termcolor, pygam, phate, matplotlib,scanpy
+        pip install python-igraph, leidenalg>=0.7.0, pybind11, hnswlib, umap-learn, numpy>=1.17, scipy, pandas>=0.25, sklearn, termcolor, pygam, phate
         pip install pyVIA
         ```
-        ## Jupyter Notebooks
-        There are several [Jupyter Notebooks](https://github.com/ShobiStassen/VIA/tree/master/Jupyter%20Notebooks) with step-by-step code for real and simulated datasets. If you experience issues with opening the notebook from github, then copy the Jupyter Notebook URL and paste it into nb viewer https://nbviewer.jupyter.org/
-        
-        ## Examples 
-        Expected runtime will be a few minutes or less. Runtime on a "normal" laptop ~5 minutes for EB and less for smaller data.
-        Data for the Jupyter Notebooks and Examples are available in the [Datasets folder](https://github.com/ShobiStassen/VIA/tree/master/Datasets) (smaller files) and larger datasets [here](https://drive.google.com/drive/folders/1WQSZeNixUAB1Sm0Xf68ZnSLQXyep936l?usp=sharing). 
-        #### 1.a Toy Data (multifurcation) [Multifurcation Jupyter NB](https://github.com/ShobiStassen/VIA/blob/master/Jupyter%20Notebooks/ViaJupyter_Toy_Multifurcating.ipynb)
-        #### 1.b Toy Data (disconnected) [Disconnected Jupyter NB](https://github.com/ShobiStassen/VIA/blob/master/Jupyter%20Notebooks/ViaJupyter_Toy_Disconnected.ipynb)
-        #### 2.a Human Embryoid Bodies (wrapper function)
-        #### 2.b Human Embryoid Bodies (Configuring VIA) [EB Jupyter NB](https://github.com/ShobiStassen/VIA/blob/master/Jupyter%20Notebooks/ViaJupyter_EmbryoidBody.ipynb)
-        #### 3.a General input format and wrapper function
-        #### 3.b General disconnected trajectories wrapper function
-        #### More examples with additional code, outputs and details are available as [Jupyter Notebooks](https://github.com/ShobiStassen/VIA/tree/master/Jupyter%20Notebooks)
+        ## Examples (Expected runtime will be a few minutes or less. Runtime on a "normal" laptop ~5 minutes for EB and less for smaller data) 
+        ### 1.a Toy Data (multifurcation)
+        ### 1.b Toy Data (disconnected)
+        ### 2.a Human Embryoid Bodies (wrapper function)
+        ### 2.b Human Embryoid Bodies (Configuring VIA)
+        ### 3.a General input format and wrapper function
+        ### 3.b General disconnected trajectories wrapper function
         ------------------------------------------------------
         ### 1.a/b Toy data (Multifurcation and Disconnected)
-        Two examples [toy datasets](https://github.com/ShobiStassen/VIA/tree/master/Datasets)  with annotations are generated using DynToy are provided. 
-        
-        ### To run on Linux:
-        All examples are shown according to Linux OS, small modifications are required to run on a Windows OS (see below)
+        Two examples [toy datasets](https://drive.google.com/drive/folders/1WQSZeNixUAB1Sm0Xf68ZnSLQXyep936l?usp=sharing) with annotations are generated using DynToy are provided. 
         ```
         import pyVIA.core as via
-        # ensure the data and label files are in csv format when you download/save them
         #multifurcation
         #the root is automatically set to  root_user = 'M1'
         via.main_Toy(ncomps=10, knn=30,dataset='Toy3', random_seed=2,foldername = ".../Trajectory/Datasets/") #multifurcation
         #disconnected trajectory
         #the root is automatically set as a list root_user = ['T1_M1', 'T2_M1'] # e.g. T2_M3 is a cell belonging to the 3rd Milestone (M3) of the second Trajectory (T2)
         via.main_Toy(ncomps=10, knn=30,dataset='Toy4',random_seed=2,foldername =".../Trajectory/Datasets/") #2 disconnected trajectories
         ```
-        Windows (small modifications in calling the code due to the way multiprocessing works in Windows compared to Linux)
-        ### To run on Windows:
-        A few additional lines are required:
-        ```
-        #when running from an IDE you need to call the function in the following way to ensure the parallel processing works:
-        import os
-        import pyVIA.core as via
-        f= os.path.join(r'C:\Users\...\Documents'+'\\')
-        def main():
-            via.main_Toy(ncomps=10, knn=30,dataset='Toy3', random_seed=2,foldername= f)    
-        if __name__ =='__main__':
-            main()
-            
-        #when running directly from terminal:
-        import os
-        import pyVIA.core as via
-        f= os.path.join(r'C:\Users\...\Documents'+'\\')
-        via.main_Toy(ncomps=10, knn=30,dataset='Toy3', random_seed=2,foldername= f)    
-        if __name__ =='__main__':
-        ```
-        
         ## Output of Multifurcating toy dataset
         ![Output of VIA on multifurcating toy dataset](https://github.com/ShobiStassen/VIA/blob/master/Figures/Toy3_fig0.png?raw=true)
         ## Output of disconnected toy dataset
         ![Output of VIA on disconnected toy dataset](https://github.com/ShobiStassen/VIA/blob/master/Figures/Toy4_fig0.png?raw=true)
         
         ### 2.a Human Embryoid Bodies (wrapper function)
-        Save the [Raw data](https://drive.google.com/file/d/1yz3zR1KAmghjYB_nLLUZoIlKN9Ew4RHf/view?usp=sharing) matrix as 'EBdata.mat'. The cells in this file have been filtered for too small/large libraries by [Moon et al. 2019](https://nbviewer.jupyter.org/github/KrishnaswamyLab/PHATE/blob/master/Python/tutorial/EmbryoidBody.ipynb). 
-        
-        Save the phate [embedding](https://github.com/ShobiStassen/VIA/tree/master/Datasets) which is required to run Example 2.a (since the phate operation is 
+        save the [Raw data](https://drive.google.com/file/d/1yz3zR1KAmghjYB_nLLUZoIlKN9Ew4RHf/view?usp=sharing) matrix as 'EBdata.mat'. The cells in this file have been filtered for too small/large libraries by [Moon et al. 2019](https://nbviewer.jupyter.org/github/KrishnaswamyLab/PHATE/blob/master/Python/tutorial/EmbryoidBody.ipynb) 
         
         The function main_EB_clean() preprocesses the cells (normalized by library size, sqrt transformation). It then calls VIA to: plot the pseudotimes, terminal states, lineage pathways and gene-clustermap. The visualization method used in this function is PHATE.
         ```
-        #runtime on single core, 8GB RAM 64bit Windows is about 8-10 minutes. This can be lowered by reducing the number of MCMC simulations (num_mcmc_simulations).
         import pyVIA.core as via
-        #Windows example path for folder where EBdata.mat is saved: f= os.path.join(r'C:\Users\...\Documents'+'\\')
-        via.main_EB_clean(ncomps=30, knn=20, v0_random_seed=24, foldername = f) # Most reasonable parameters of ncomps (10-200) and knn (15-50) work well
+        via.main_EB_clean(ncomps=30, knn=20, p0_random_seed=20, foldername = '') # Most reasonable parameters of ncomps (10-200) and knn (15-50) work well
         ```
         ### 2.b Human Embryoid Bodies (Configuring VIA)
-        If you wish to run the data using UMAP or TSNE (instead of PHATE), or require more control of the parameters/outputs, then use the following code. (See the Jupyter Notebook for detailed output and code). Expected runtime will be around 1-2 minutes using 5 cores, or ~8-10 on "normal" laptop. .
+        If you wish to run the data using UMAP or TSNE (instead of PHATE), or require more control of the parameters/outputs, then use the following code:
+        Expected runtime will be around 2 minutes
         ```
         import pyVIA.core as via
         #pre-process the data as needed and provide to via as a numpy array
         #root_user is the index of the cell corresponding to a suitable start/root cell
         
-        v0_too_big = 0.3 #clusters comprising more than 30% of total cell population will be re-clustered by PARC
-        v1_too_big = 0.05
-        
         v0 = via.VIA(input_data, time_labels, jac_std_global=0.15, dist_std_local=1, knn=knn,
                      too_big_factor=v0_too_big, root_user=[1], dataset='EB', random_seed=v0_random_seed,
                      do_magic_bool=True, is_coarse=True, preserve_disconnected=True)  
         v0.run_VIA()
         
         
         tsi_list = get_loc_terminal_states(v0, input_data) #translate the terminal clusters found in v0 to the fine-grained run in v1
@@ -181,15 +133,15 @@
         
         # use UMAP or PHate to obtain embedding that is used for single-cell level visualization
         embedding = umap.UMAP(random_state=42, n_neighbors=15, init='random').fit_transform(data.values[:, 0:5])
         
         # list marker genes or genes of interest if known in advance. otherwise marker_genes = []
         marker_genes = ['Igll1', 'Myc', 'Slc7a5', 'Ldha', 'Foxo1', 'Lig4', 'Sp7']  # irf4 down-up
         # call VIA. We identify an early (suitable) start cell root = [42]. Can also set an arbitrary value
-        via.via_wrapper(adata, true_label, embedding, knn=10, ncomps=20, jac_std_global=0.15, root=[42], dataset='',
+        via.via_wrapper(adata, true_label, embedding, knn=20, ncomps=20, jac_std_global=0.15, root=[42], dataset='',
                     random_seed=1,v0_toobig=0.3, v1_toobig=0.1, marker_genes=marker_genes)
         ```
         ### 3.b VIA wrapper for generic disconnected trajectory
         ```
         import scanpy as sc
         import pandas as pd
         
@@ -218,28 +170,28 @@
         ### Parameters
         
         | Input Parameter for class VIA | Description |
         | ---------- |----------|
         | `data` | (numpy.ndarray) n_samples x n_features. When using via_wrapper(), data is ANNdata object that has a PCA object adata.obsm['X_pca'][:, 0:ncomps] and ncomps is the number of components that will be used. |
         | `true_label` | (list) 'ground truth' annotations or placeholder|
         | `knn` |  (optional, default = 30) number of K-Nearest Neighbors for HNSWlib KNN graph |
-        |`root_user`|When using one of the example datasets where there is a single root cell type, simply provide the index number of the cell corresponding to a sensible root: root_user = 1. When using the generic via wrapper, this input is in the form of a list containing roots corresponding to index (row number in cell matrix) of root cell. For most trajectories this is of the form [99], for multiple disconnected trajectories an arbitrary list of cells can be provided [1,506,1100] or VIA arbitratily chooses cells. If the root cells of disconnected trajectories are known in advance, then the cells should be annotated with similar syntax to that of Example Dataset in Disconnected Toy Example 1b.|
+        |`root_user`|list containing roots corresponding to index (row number) of root cell. For most trajectories this is of the form [99], for multiple disconnected trajectories an arbitrary list of cells can be provided [1,506,1100] or VIA arbitratily chooses cells. If the root cells of disconnected trajectories are known in advance, then the cells should be annotated with similar syntax to that of Example Dataset in Disconnected Toy Example 1b.|
         | `dist_std_local` |  (optional, default = 1) local pruning threshold for PARC clustering stage: the number of standard deviations above the mean minkowski distance between neighbors of a given node. the higher the parameter, the more edges are retained|
         | `jac_std_global` |  (optional, default = 0.15) global level  graph pruning for PARC clustering stage. This threshold can also be set as the number of standard deviations below the network's mean-jaccard-weighted edges. 0.1-1 provide reasonable pruning. higher value means less pruning. e.g. a value of 0.15 means all edges that are above mean(edgeweight)-0.15*std(edge-weights) are retained. We find both 0.15 and 'median' to yield good results resulting in pruning away ~ 50-60% edges |
         | `too_big_factor` |  (optional, default = 0.4) if a cluster exceeds this share of the entire cell population, then the PARC will be run on the large cluster|
         |`x_lazy`| (optional, default = 0.95) 1-x = probability of staying in same node (lazy). Values between 0.9-0.99 are reasonable|
         |`alpha_teleport`| (optional, default = 0.99) 1-alpha is probability of jumping. Values between 0.95-0.99 are reasonable unless prior knowledge of teleportation 
         | `distance` |  (optional, default = 'l2' euclidean) 'ip','cosine'|
         | `random_seed` |  (optional, default = 42) The random seed to pass to Leiden|
         | `pseudotime_threshold_TS` |  (optional, default = 30) Percentile threshold for potential node to qualify as Terminal State|
         | `resolution_parameter` |  (optional, default = 1) Uses ModuliartyVP and RBConfigurationVertexPartition|
         | `preserve_disconnected_after_pruning` |  (optional, default = False) Cluster-graph pruning can occasionally cause fragmentation that can be repaired (by setting to True) by retaining select edges. |
         |`cluster_graph_pruning_std`| (optional, default =0.15) Usually set to the same value as the PARC clustering level of jac_std_global. To retain more connectivity in the graph underlying the trajectory computations, increase the value|
         |`visual_cluster_graph_pruning`| (optional, default = 0.15) Usually set to the same value as the PARC clustering level of jac_std_global. This does not impact computation of terminal states, pseudotime or lineage likelihoods. It controls the number of edges plotted for visual effect|
-        |`num_sim_branch_probability`|(optional), default = 500. Number of MCMCs run per terminal state. This can be safely reduced to 100 when computational resources are limited|
+        
         As shown in the examples, VIA is built to run on a single or double iteration. For extremely large datasets (>1M cells), a single pass is favourable. For mid-size it can be useful to run the double-pass mode which is shown in Example 2b and 3a,b. In the first pass VIA performs a coarser clustering which is useful for capturing terminal states. To increase the resolution of the pseudotime, lineage likelihood and gene trends, we re-run VIA in a second pass which produces a finer cluster-graph and transfers the lineages (terminal states) obtained in the first pass into the second pass. We therefore provide the second pass with the terminal_states obtained in the first pass. To speed up the computation, we also pass the original HNSW KNN graph. The following parameters are used for second passes.
         
         | Input Parameter | Description |
         | ---------- |----------|
         | `is_coarse` |  (optional, default = True) If running VIA in two steps, for the second fine-grained, set to "False'|
         |`super_cluster_labels`| Set this to v0.labels (clustering output of first pass "v0")|
         |`super_terminal_cells`| super_terminal_cells = via.get_loc_terminal_states(v0, data)|
@@ -249,11 +201,11 @@
         |`csr_array_locally_pruned`|csr_array_locally_pruned=v0.csr_array_locally_pruned. CSR matrix of the locally pruned KNN graph|
         
         | Attributes | Description |
         | ---------- |----------|
         | `labels` | (list) length n_samples of corresponding cluster labels |
         | `edgelist_maxout` | (list) used to draw trajectories on the 2D embedding |
         | `single_cell_pt_markov` | (list) computed pseudotime|
-        |`single_cell_bp`|(array) computed single cell branch probabilities (lineage likelihoods). n_cells x n_terminal states. The columns each correspond to a terminal state, in the same order presented in the'terminal_clusters' attribute|
         | `terminal clusters` | (list) terminal clusters found by VIA|
+        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

