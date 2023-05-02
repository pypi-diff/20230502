# Comparing `tmp/causalforge-0.0.6.tar.gz` & `tmp/causalforge-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causalforge-0.0.6.tar", last modified: Mon May  1 23:41:36 2023, max compression
+gzip compressed data, was "causalforge-0.0.7.tar", last modified: Tue May  2 00:17:13 2023, max compression
```

## Comparing `causalforge-0.0.6.tar` & `causalforge-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-05-01 23:41:36.446056 causalforge-0.0.6/
--rw-r--r--   0 AG62216    (501) staff       (20)     1065 2023-04-22 02:11:58.000000 causalforge-0.0.6/LICENSE
--rw-r--r--   0 AG62216    (501) staff       (20)     2895 2023-05-01 23:41:36.446198 causalforge-0.0.6/PKG-INFO
--rw-r--r--   0 AG62216    (501) staff       (20)     2444 2023-04-27 01:40:40.000000 causalforge-0.0.6/README.md
-drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-05-01 23:41:36.441402 causalforge-0.0.6/causalforge/
--rw-r--r--   0 AG62216    (501) staff       (20)       62 2023-05-01 23:40:20.000000 causalforge-0.0.6/causalforge/__init__.py
-drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-05-01 23:41:36.445576 causalforge-0.0.6/causalforge/tests/
--rw-r--r--   0 AG62216    (501) staff       (20)        0 2023-04-22 02:11:58.000000 causalforge-0.0.6/causalforge/tests/__init__.py
-drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-05-01 23:41:36.444895 causalforge-0.0.6/causalforge.egg-info/
--rw-r--r--   0 AG62216    (501) staff       (20)     2895 2023-05-01 23:41:36.000000 causalforge-0.0.6/causalforge.egg-info/PKG-INFO
--rw-r--r--   0 AG62216    (501) staff       (20)      264 2023-05-01 23:41:36.000000 causalforge-0.0.6/causalforge.egg-info/SOURCES.txt
--rw-r--r--   0 AG62216    (501) staff       (20)        1 2023-05-01 23:41:36.000000 causalforge-0.0.6/causalforge.egg-info/dependency_links.txt
--rw-r--r--   0 AG62216    (501) staff       (20)      134 2023-05-01 23:41:36.000000 causalforge-0.0.6/causalforge.egg-info/requires.txt
--rw-r--r--   0 AG62216    (501) staff       (20)       12 2023-05-01 23:41:36.000000 causalforge-0.0.6/causalforge.egg-info/top_level.txt
--rw-r--r--   0 AG62216    (501) staff       (20)      102 2023-05-01 23:41:36.447001 causalforge-0.0.6/setup.cfg
--rw-r--r--   0 AG62216    (501) staff       (20)     1659 2023-04-26 23:15:59.000000 causalforge-0.0.6/setup.py
+drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-05-02 00:17:13.008997 causalforge-0.0.7/
+-rw-r--r--   0 AG62216    (501) staff       (20)     1065 2023-04-22 02:11:58.000000 causalforge-0.0.7/LICENSE
+-rw-r--r--   0 AG62216    (501) staff       (20)     2942 2023-05-02 00:17:13.009132 causalforge-0.0.7/PKG-INFO
+-rw-r--r--   0 AG62216    (501) staff       (20)     2491 2023-05-01 23:55:39.000000 causalforge-0.0.7/README.md
+drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-05-02 00:17:13.004813 causalforge-0.0.7/causalforge/
+-rw-r--r--   0 AG62216    (501) staff       (20)       62 2023-05-02 00:16:22.000000 causalforge-0.0.7/causalforge/__init__.py
+drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-05-02 00:17:13.008553 causalforge-0.0.7/causalforge/tests/
+-rw-r--r--   0 AG62216    (501) staff       (20)        0 2023-04-22 02:11:58.000000 causalforge-0.0.7/causalforge/tests/__init__.py
+drwxr-xr-x   0 AG62216    (501) staff       (20)        0 2023-05-02 00:17:13.007871 causalforge-0.0.7/causalforge.egg-info/
+-rw-r--r--   0 AG62216    (501) staff       (20)     2942 2023-05-02 00:17:12.000000 causalforge-0.0.7/causalforge.egg-info/PKG-INFO
+-rw-r--r--   0 AG62216    (501) staff       (20)      264 2023-05-02 00:17:12.000000 causalforge-0.0.7/causalforge.egg-info/SOURCES.txt
+-rw-r--r--   0 AG62216    (501) staff       (20)        1 2023-05-02 00:17:12.000000 causalforge-0.0.7/causalforge.egg-info/dependency_links.txt
+-rw-r--r--   0 AG62216    (501) staff       (20)      128 2023-05-02 00:17:12.000000 causalforge-0.0.7/causalforge.egg-info/requires.txt
+-rw-r--r--   0 AG62216    (501) staff       (20)       12 2023-05-02 00:17:12.000000 causalforge-0.0.7/causalforge.egg-info/top_level.txt
+-rw-r--r--   0 AG62216    (501) staff       (20)      102 2023-05-02 00:17:13.009783 causalforge-0.0.7/setup.cfg
+-rw-r--r--   0 AG62216    (501) staff       (20)     1659 2023-04-26 23:15:59.000000 causalforge-0.0.7/setup.py
```

### Comparing `causalforge-0.0.6/LICENSE` & `causalforge-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `causalforge-0.0.6/PKG-INFO` & `causalforge-0.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,72 +1,71 @@
 Metadata-Version: 2.1
 Name: causalforge
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python Package for Causal Inference
 Home-page: https://github.com/anthem-ai/causalflow
 Author: Gino Tesei, Jey Kottalam
 Author-email: 
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<img alt="causalforge-logo" class="causalforge-logo"  height="250" width="300"  src="https://raw.githubusercontent.com/anthem-ai/causalflow/main/logo.png">
+<img alt="causalforge-logo" class="causalforge-logo"  height="250" width="300"  src="https://raw.githubusercontent.com/anthem-ai/causalflow/main/logo.png?token=GHSAT0AAAAAAB6UCMRK6JN5QVPWHF2GO3XSZCQL25A">
 
 # CausalFlow
 
 [![PyPI version](https://badge.fury.io/py/causalforge.svg)](https://badge.fury.io/py/causalforge)
 [![Documentation Status](https://readthedocs.org/projects/causalforge/badge/?version=latest)](https://causalforge.readthedocs.io/en/latest/?badge=latest)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
 [![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
 
 
-CausalFlow is a Python package that provides a suite of modeling & causal inference methods using machine learning algorithms based on Elevence Health recent research. It provides convenient APIs that allow to estimate Propensity Score, Average Treatment Effect (ATE), Conditional Average Treatment Effect (CATE) or Individual Treatment Effect (ITE) 
+CausalForge is a Python package that provides a suite of modeling & causal inference methods using machine learning algorithms based on Elevence Health recent research. It provides convenient APIs that allow to estimate Propensity Score, Average Treatment Effect (ATE), Conditional Average Treatment Effect (CATE) or Individual Treatment Effect (ITE) 
 from experimental or observational data.
 
 <details>
   <summary> <H3>Installing Python Package</H3>  </summary>
 
 We recommend to create a proper enviroment with tensorflow and pytorch 
 installed. For example, for a local Mac enviroment without GPUs: 
 
 ```sh
 conda env create -f env_mac.yml
-conda activate causalflow
+conda activate causalforge
 ```
 
 You can install it after cloning this repository, i.e.
 
 ```sh
-git clone https://gitlab.com/gtesei/causalflow.git
-cd causalflow
+git clone https://github.com/anthem-ai/causalforge
+cd causalforge
 [sudo] pip install -e . [--trusted-host pypi.org --trusted-host files.pythonhosted.org]
 ```
 
 or directly from the repository (development), i.e.
 
 ```sh
-pip install --upgrade git+https://gitlab.com/gtesei/causalflow.git [--trusted-host pypi.org --trusted-host files.pythonhosted.org]
+pip install --upgrade git+https://github.com/anthem-ai/causalforge [--trusted-host pypi.org --trusted-host files.pythonhosted.org]
 ```
 
 or directly from PyPI, i.e.
 
 ```sh
-pip install causalflow
+pip install causalforge
 ```
 
 After installing you can import classes and methods, e.g.
 
 ```python
-import causalflow
-causalflow.__version__
-'0.0.1'
+import causalforge
+causalforge.__version__
 ```
 </details>
 
 <details>
   <summary> <H3>Testing</H3>  </summary>
   
 ```bash
```

### Comparing `causalforge-0.0.6/README.md` & `causalforge-0.0.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,56 @@
-<img alt="causalforge-logo" class="causalforge-logo"  height="250" width="300"  src="https://raw.githubusercontent.com/anthem-ai/causalflow/main/logo.png">
+<img alt="causalforge-logo" class="causalforge-logo"  height="250" width="300"  src="https://raw.githubusercontent.com/anthem-ai/causalflow/main/logo.png?token=GHSAT0AAAAAAB6UCMRK6JN5QVPWHF2GO3XSZCQL25A">
 
 # CausalFlow
 
 [![PyPI version](https://badge.fury.io/py/causalforge.svg)](https://badge.fury.io/py/causalforge)
 [![Documentation Status](https://readthedocs.org/projects/causalforge/badge/?version=latest)](https://causalforge.readthedocs.io/en/latest/?badge=latest)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
 [![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
 
 
-CausalFlow is a Python package that provides a suite of modeling & causal inference methods using machine learning algorithms based on Elevence Health recent research. It provides convenient APIs that allow to estimate Propensity Score, Average Treatment Effect (ATE), Conditional Average Treatment Effect (CATE) or Individual Treatment Effect (ITE) 
+CausalForge is a Python package that provides a suite of modeling & causal inference methods using machine learning algorithms based on Elevence Health recent research. It provides convenient APIs that allow to estimate Propensity Score, Average Treatment Effect (ATE), Conditional Average Treatment Effect (CATE) or Individual Treatment Effect (ITE) 
 from experimental or observational data.
 
 <details>
   <summary> <H3>Installing Python Package</H3>  </summary>
 
 We recommend to create a proper enviroment with tensorflow and pytorch 
 installed. For example, for a local Mac enviroment without GPUs: 
 
 ```sh
 conda env create -f env_mac.yml
-conda activate causalflow
+conda activate causalforge
 ```
 
 You can install it after cloning this repository, i.e.
 
 ```sh
-git clone https://gitlab.com/gtesei/causalflow.git
-cd causalflow
+git clone https://github.com/anthem-ai/causalforge
+cd causalforge
 [sudo] pip install -e . [--trusted-host pypi.org --trusted-host files.pythonhosted.org]
 ```
 
 or directly from the repository (development), i.e.
 
 ```sh
-pip install --upgrade git+https://gitlab.com/gtesei/causalflow.git [--trusted-host pypi.org --trusted-host files.pythonhosted.org]
+pip install --upgrade git+https://github.com/anthem-ai/causalforge [--trusted-host pypi.org --trusted-host files.pythonhosted.org]
 ```
 
 or directly from PyPI, i.e.
 
 ```sh
-pip install causalflow
+pip install causalforge
 ```
 
 After installing you can import classes and methods, e.g.
 
 ```python
-import causalflow
-causalflow.__version__
-'0.0.1'
+import causalforge
+causalforge.__version__
 ```
 </details>
 
 <details>
   <summary> <H3>Testing</H3>  </summary>
   
 ```bash
```

### Comparing `causalforge-0.0.6/causalforge.egg-info/PKG-INFO` & `causalforge-0.0.7/causalforge.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,72 +1,71 @@
 Metadata-Version: 2.1
 Name: causalforge
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python Package for Causal Inference
 Home-page: https://github.com/anthem-ai/causalflow
 Author: Gino Tesei, Jey Kottalam
 Author-email: 
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<img alt="causalforge-logo" class="causalforge-logo"  height="250" width="300"  src="https://raw.githubusercontent.com/anthem-ai/causalflow/main/logo.png">
+<img alt="causalforge-logo" class="causalforge-logo"  height="250" width="300"  src="https://raw.githubusercontent.com/anthem-ai/causalflow/main/logo.png?token=GHSAT0AAAAAAB6UCMRK6JN5QVPWHF2GO3XSZCQL25A">
 
 # CausalFlow
 
 [![PyPI version](https://badge.fury.io/py/causalforge.svg)](https://badge.fury.io/py/causalforge)
 [![Documentation Status](https://readthedocs.org/projects/causalforge/badge/?version=latest)](https://causalforge.readthedocs.io/en/latest/?badge=latest)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
 [![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/release/python-380/)
 
 
-CausalFlow is a Python package that provides a suite of modeling & causal inference methods using machine learning algorithms based on Elevence Health recent research. It provides convenient APIs that allow to estimate Propensity Score, Average Treatment Effect (ATE), Conditional Average Treatment Effect (CATE) or Individual Treatment Effect (ITE) 
+CausalForge is a Python package that provides a suite of modeling & causal inference methods using machine learning algorithms based on Elevence Health recent research. It provides convenient APIs that allow to estimate Propensity Score, Average Treatment Effect (ATE), Conditional Average Treatment Effect (CATE) or Individual Treatment Effect (ITE) 
 from experimental or observational data.
 
 <details>
   <summary> <H3>Installing Python Package</H3>  </summary>
 
 We recommend to create a proper enviroment with tensorflow and pytorch 
 installed. For example, for a local Mac enviroment without GPUs: 
 
 ```sh
 conda env create -f env_mac.yml
-conda activate causalflow
+conda activate causalforge
 ```
 
 You can install it after cloning this repository, i.e.
 
 ```sh
-git clone https://gitlab.com/gtesei/causalflow.git
-cd causalflow
+git clone https://github.com/anthem-ai/causalforge
+cd causalforge
 [sudo] pip install -e . [--trusted-host pypi.org --trusted-host files.pythonhosted.org]
 ```
 
 or directly from the repository (development), i.e.
 
 ```sh
-pip install --upgrade git+https://gitlab.com/gtesei/causalflow.git [--trusted-host pypi.org --trusted-host files.pythonhosted.org]
+pip install --upgrade git+https://github.com/anthem-ai/causalforge [--trusted-host pypi.org --trusted-host files.pythonhosted.org]
 ```
 
 or directly from PyPI, i.e.
 
 ```sh
-pip install causalflow
+pip install causalforge
 ```
 
 After installing you can import classes and methods, e.g.
 
 ```python
-import causalflow
-causalflow.__version__
-'0.0.1'
+import causalforge
+causalforge.__version__
 ```
 </details>
 
 <details>
   <summary> <H3>Testing</H3>  </summary>
   
 ```bash
```

### Comparing `causalforge-0.0.6/setup.py` & `causalforge-0.0.7/setup.py`

 * *Files identical despite different names*

