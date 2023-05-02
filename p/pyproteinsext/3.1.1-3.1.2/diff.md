# Comparing `tmp/pyproteinsext-3.1.1.tar.gz` & `tmp/pyproteinsext-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproteinsext-3.1.1.tar", max compression
+gzip compressed data, was "pyproteinsext-3.1.2.tar", max compression
```

## Comparing `pyproteinsext-3.1.1.tar` & `pyproteinsext-3.1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    35141 2023-03-16 13:44:31.227660 pyproteinsext-3.1.1/LICENSE
--rw-r--r--   0        0        0      431 2023-03-22 13:59:26.473722 pyproteinsext-3.1.1/pyproject.toml
--rw-r--r--   0        0        0        6 2023-03-16 13:45:07.939948 pyproteinsext-3.1.1/pyproteinsext/.gitignore
--rw-r--r--   0        0        0    35141 2023-03-16 13:45:07.939948 pyproteinsext-3.1.1/pyproteinsext/LICENSE
--rw-r--r--   0        0        0        0 2023-03-16 13:45:07.939948 pyproteinsext-3.1.1/pyproteinsext/__init__.py
--rw-r--r--   0        0        0     1030 2023-03-16 13:45:07.939948 pyproteinsext-3.1.1/pyproteinsext/__main__.py
--rw-r--r--   0        0        0     9824 2023-03-16 13:45:07.939948 pyproteinsext-3.1.1/pyproteinsext/annotators.py
--rw-r--r--   0        0        0    14237 2023-03-16 13:45:07.939948 pyproteinsext-3.1.1/pyproteinsext/biogrid.py
--rw-r--r--   0        0        0        0 2023-03-16 13:45:07.939948 pyproteinsext-3.1.1/pyproteinsext/database/__init__.py
--rw-r--r--   0        0        0    18015 2023-03-16 13:45:07.939948 pyproteinsext-3.1.1/pyproteinsext/database/uniprotFastaFS.py
--rw-r--r--   0        0        0     9091 2023-03-16 13:45:07.939948 pyproteinsext-3.1.1/pyproteinsext/ena.py
--rw-r--r--   0        0        0     2084 2023-03-16 13:45:07.939948 pyproteinsext-3.1.1/pyproteinsext/fastaContainerFactory.py
--rw-r--r--   0        0        0    16636 2023-03-16 13:45:07.939948 pyproteinsext-3.1.1/pyproteinsext/hmmrContainerFactory.py
--rw-r--r--   0        0        0     1622 2023-03-16 13:45:07.939948 pyproteinsext-3.1.1/pyproteinsext/matrisome.py
--rw-r--r--   0        0        0   114987 2023-03-16 13:45:07.939948 pyproteinsext-3.1.1/pyproteinsext/notebooks/.ipynb_checkpoints/HMMR_wrapper-checkpoint.ipynb
--rw-r--r--   0        0        0     2748 2023-03-16 13:45:07.939948 pyproteinsext-3.1.1/pyproteinsext/notebooks/.ipynb_checkpoints/uniprotWrapper-checkpoint.ipynb
--rw-r--r--   0        0        0   114987 2023-03-16 13:45:07.939948 pyproteinsext-3.1.1/pyproteinsext/notebooks/HMMR_wrapper.ipynb
--rwxr-xr-x   0        0        0  2114556 2023-03-16 13:45:07.951948 pyproteinsext-3.1.1/pyproteinsext/notebooks/data/example_hmmscan.out.gz
--rw-r--r--   0        0        0    82252 2023-03-16 13:45:07.951948 pyproteinsext-3.1.1/pyproteinsext/notebooks/psicquic_demo.ipynb
--rw-r--r--   0        0        0     2748 2023-03-16 13:45:07.951948 pyproteinsext-3.1.1/pyproteinsext/notebooks/uniprotWrapper.ipynb
--rw-r--r--   0        0        0    13715 2023-03-16 13:45:07.951948 pyproteinsext-3.1.1/pyproteinsext/ontology.py
--rw-r--r--   0        0        0     3004 2023-03-16 13:45:07.951948 pyproteinsext-3.1.1/pyproteinsext/pfam.py
--rw-r--r--   0        0        0     2414 2023-03-16 13:45:07.951948 pyproteinsext-3.1.1/pyproteinsext/pfamCutter.py
--rw-r--r--   0        0        0      741 2023-03-16 13:45:07.951948 pyproteinsext-3.1.1/pyproteinsext/proteinContainer.py
--rw-r--r--   0        0        0    27750 2023-03-16 13:45:07.951948 pyproteinsext-3.1.1/pyproteinsext/psicquic.py
--rw-r--r--   0        0        0     4674 2023-03-16 13:45:07.951948 pyproteinsext-3.1.1/pyproteinsext/refseq.py
--rw-r--r--   0        0        0     4662 2023-03-16 13:45:07.951948 pyproteinsext-3.1.1/pyproteinsext/services/uniprot/__init__.py
--rw-r--r--   0        0        0     3868 2023-03-16 13:45:07.951948 pyproteinsext-3.1.1/pyproteinsext/services/uniprot/collectionProxy.py
--rw-r--r--   0        0        0     2115 2023-03-16 13:45:07.951948 pyproteinsext-3.1.1/pyproteinsext/services/uniprot/entryProxy.py
--rw-r--r--   0        0        0     1028 2023-03-16 13:45:07.951948 pyproteinsext-3.1.1/pyproteinsext/services/uniprot/redisClient.py
--rw-r--r--   0        0        0     1480 2023-03-16 13:45:07.951948 pyproteinsext-3.1.1/pyproteinsext/setup.py
--rw-r--r--   0        0        0     4013 2023-03-16 13:45:07.951948 pyproteinsext-3.1.1/pyproteinsext/tmhmmContainerFactory.py
--rw-r--r--   0        0        0    23939 2023-03-16 13:45:07.951948 pyproteinsext-3.1.1/pyproteinsext/topology.py
--rw-r--r--   0        0        0    27203 2023-03-17 11:00:42.061529 pyproteinsext-3.1.1/pyproteinsext/uniprot.py
--rw-r--r--   0        0        0     5484 2023-03-16 13:45:07.951948 pyproteinsext-3.1.1/pyproteinsext/uniprotAnnotator.py
--rw-r--r--   0        0        0      909 2023-03-22 13:59:34.825456 pyproteinsext-3.1.1/setup.py
--rw-r--r--   0        0        0      669 2023-03-22 13:59:34.825780 pyproteinsext-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35141 2023-05-02 15:15:54.566691 pyproteinsext-3.1.2/LICENSE
+-rw-r--r--   0        0        0      417 2023-05-02 15:20:24.942432 pyproteinsext-3.1.2/pyproject.toml
+-rw-r--r--   0        0        0        6 2023-05-02 15:16:09.296365 pyproteinsext-3.1.2/pyproteinsext/.gitignore
+-rw-r--r--   0        0        0    35141 2023-05-02 15:16:09.296762 pyproteinsext-3.1.2/pyproteinsext/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-02 15:16:09.296885 pyproteinsext-3.1.2/pyproteinsext/__init__.py
+-rw-r--r--   0        0        0     1030 2023-05-02 15:16:09.297090 pyproteinsext-3.1.2/pyproteinsext/__main__.py
+-rw-r--r--   0        0        0     9824 2023-05-02 15:16:09.297288 pyproteinsext-3.1.2/pyproteinsext/annotators.py
+-rw-r--r--   0        0        0    14237 2023-05-02 15:16:09.297487 pyproteinsext-3.1.2/pyproteinsext/biogrid.py
+-rw-r--r--   0        0        0        0 2023-05-02 15:16:09.297637 pyproteinsext-3.1.2/pyproteinsext/database/__init__.py
+-rw-r--r--   0        0        0    18015 2023-05-02 15:16:09.297897 pyproteinsext-3.1.2/pyproteinsext/database/uniprotFastaFS.py
+-rw-r--r--   0        0        0     9091 2023-05-02 15:16:09.298123 pyproteinsext-3.1.2/pyproteinsext/ena.py
+-rw-r--r--   0        0        0     2084 2023-05-02 15:16:09.298379 pyproteinsext-3.1.2/pyproteinsext/fastaContainerFactory.py
+-rw-r--r--   0        0        0    16636 2023-05-02 15:16:09.298649 pyproteinsext-3.1.2/pyproteinsext/hmmrContainerFactory.py
+-rw-r--r--   0        0        0     1622 2023-05-02 15:16:09.298870 pyproteinsext-3.1.2/pyproteinsext/matrisome.py
+-rw-r--r--   0        0        0   114987 2023-05-02 15:16:09.299592 pyproteinsext-3.1.2/pyproteinsext/notebooks/.ipynb_checkpoints/HMMR_wrapper-checkpoint.ipynb
+-rw-r--r--   0        0        0     2748 2023-05-02 15:16:09.299785 pyproteinsext-3.1.2/pyproteinsext/notebooks/.ipynb_checkpoints/uniprotWrapper-checkpoint.ipynb
+-rw-r--r--   0        0        0   114987 2023-05-02 15:16:09.300269 pyproteinsext-3.1.2/pyproteinsext/notebooks/HMMR_wrapper.ipynb
+-rwxr-xr-x   0        0        0  2114556 2023-05-02 15:16:09.307978 pyproteinsext-3.1.2/pyproteinsext/notebooks/data/example_hmmscan.out.gz
+-rw-r--r--   0        0        0    82252 2023-05-02 15:16:09.308746 pyproteinsext-3.1.2/pyproteinsext/notebooks/psicquic_demo.ipynb
+-rw-r--r--   0        0        0     2748 2023-05-02 15:16:09.308999 pyproteinsext-3.1.2/pyproteinsext/notebooks/uniprotWrapper.ipynb
+-rw-r--r--   0        0        0    13715 2023-05-02 15:16:09.309223 pyproteinsext-3.1.2/pyproteinsext/ontology.py
+-rw-r--r--   0        0        0     3004 2023-05-02 15:16:09.309399 pyproteinsext-3.1.2/pyproteinsext/pfam.py
+-rw-r--r--   0        0        0     2414 2023-05-02 15:16:09.309563 pyproteinsext-3.1.2/pyproteinsext/pfamCutter.py
+-rw-r--r--   0        0        0      741 2023-05-02 15:16:09.309727 pyproteinsext-3.1.2/pyproteinsext/proteinContainer.py
+-rw-r--r--   0        0        0    27750 2023-05-02 15:16:09.310037 pyproteinsext-3.1.2/pyproteinsext/psicquic.py
+-rw-r--r--   0        0        0     4674 2023-05-02 15:16:09.310247 pyproteinsext-3.1.2/pyproteinsext/refseq.py
+-rw-r--r--   0        0        0     4662 2023-05-02 15:16:09.310777 pyproteinsext-3.1.2/pyproteinsext/services/uniprot/__init__.py
+-rw-r--r--   0        0        0     3868 2023-05-02 15:16:09.311053 pyproteinsext-3.1.2/pyproteinsext/services/uniprot/collectionProxy.py
+-rw-r--r--   0        0        0     2115 2023-05-02 15:16:09.311223 pyproteinsext-3.1.2/pyproteinsext/services/uniprot/entryProxy.py
+-rw-r--r--   0        0        0     1028 2023-05-02 15:16:09.311396 pyproteinsext-3.1.2/pyproteinsext/services/uniprot/redisClient.py
+-rw-r--r--   0        0        0     1480 2023-05-02 15:16:09.311627 pyproteinsext-3.1.2/pyproteinsext/setup.py
+-rw-r--r--   0        0        0     4013 2023-05-02 15:16:09.311842 pyproteinsext-3.1.2/pyproteinsext/tmhmmContainerFactory.py
+-rw-r--r--   0        0        0    23939 2023-05-02 15:16:09.312225 pyproteinsext-3.1.2/pyproteinsext/topology.py
+-rw-r--r--   0        0        0    27203 2023-05-02 15:16:09.312715 pyproteinsext-3.1.2/pyproteinsext/uniprot.py
+-rw-r--r--   0        0        0     5484 2023-05-02 15:16:09.313102 pyproteinsext-3.1.2/pyproteinsext/uniprotAnnotator.py
+-rw-r--r--   0        0        0      880 2023-05-02 15:20:35.347130 pyproteinsext-3.1.2/setup.py
+-rw-r--r--   0        0        0      578 2023-05-02 15:20:35.347411 pyproteinsext-3.1.2/PKG-INFO
```

### Comparing `pyproteinsext-3.1.1/LICENSE` & `pyproteinsext-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproteinsext-3.1.1/pyproteinsext/LICENSE` & `pyproteinsext-3.1.2/pyproteinsext/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproteinsext-3.1.1/pyproteinsext/__main__.py` & `pyproteinsext-3.1.2/pyproteinsext/__main__.py`

 * *Files identical despite different names*

### Comparing `pyproteinsext-3.1.1/pyproteinsext/annotators.py` & `pyproteinsext-3.1.2/pyproteinsext/annotators.py`

 * *Files identical despite different names*

### Comparing `pyproteinsext-3.1.1/pyproteinsext/biogrid.py` & `pyproteinsext-3.1.2/pyproteinsext/biogrid.py`

 * *Files identical despite different names*

### Comparing `pyproteinsext-3.1.1/pyproteinsext/database/uniprotFastaFS.py` & `pyproteinsext-3.1.2/pyproteinsext/database/uniprotFastaFS.py`

 * *Files identical despite different names*

### Comparing `pyproteinsext-3.1.1/pyproteinsext/ena.py` & `pyproteinsext-3.1.2/pyproteinsext/ena.py`

 * *Files identical despite different names*

### Comparing `pyproteinsext-3.1.1/pyproteinsext/fastaContainerFactory.py` & `pyproteinsext-3.1.2/pyproteinsext/fastaContainerFactory.py`

 * *Files identical despite different names*

### Comparing `pyproteinsext-3.1.1/pyproteinsext/hmmrContainerFactory.py` & `pyproteinsext-3.1.2/pyproteinsext/hmmrContainerFactory.py`

 * *Files identical despite different names*

### Comparing `pyproteinsext-3.1.1/pyproteinsext/matrisome.py` & `pyproteinsext-3.1.2/pyproteinsext/matrisome.py`

 * *Files identical despite different names*

### Comparing `pyproteinsext-3.1.1/pyproteinsext/notebooks/.ipynb_checkpoints/HMMR_wrapper-checkpoint.ipynb` & `pyproteinsext-3.1.2/pyproteinsext/notebooks/.ipynb_checkpoints/HMMR_wrapper-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `pyproteinsext-3.1.1/pyproteinsext/notebooks/.ipynb_checkpoints/uniprotWrapper-checkpoint.ipynb` & `pyproteinsext-3.1.2/pyproteinsext/notebooks/.ipynb_checkpoints/uniprotWrapper-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `pyproteinsext-3.1.1/pyproteinsext/notebooks/HMMR_wrapper.ipynb` & `pyproteinsext-3.1.2/pyproteinsext/notebooks/HMMR_wrapper.ipynb`

 * *Files identical despite different names*

### Comparing `pyproteinsext-3.1.1/pyproteinsext/notebooks/data/example_hmmscan.out.gz` & `pyproteinsext-3.1.2/pyproteinsext/notebooks/data/example_hmmscan.out.gz`

 * *Files identical despite different names*

### Comparing `pyproteinsext-3.1.1/pyproteinsext/notebooks/psicquic_demo.ipynb` & `pyproteinsext-3.1.2/pyproteinsext/notebooks/psicquic_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pyproteinsext-3.1.1/pyproteinsext/notebooks/uniprotWrapper.ipynb` & `pyproteinsext-3.1.2/pyproteinsext/notebooks/uniprotWrapper.ipynb`

 * *Files identical despite different names*

### Comparing `pyproteinsext-3.1.1/pyproteinsext/ontology.py` & `pyproteinsext-3.1.2/pyproteinsext/ontology.py`

 * *Files identical despite different names*

### Comparing `pyproteinsext-3.1.1/pyproteinsext/pfam.py` & `pyproteinsext-3.1.2/pyproteinsext/pfam.py`

 * *Files identical despite different names*

### Comparing `pyproteinsext-3.1.1/pyproteinsext/pfamCutter.py` & `pyproteinsext-3.1.2/pyproteinsext/pfamCutter.py`

 * *Files identical despite different names*

### Comparing `pyproteinsext-3.1.1/pyproteinsext/proteinContainer.py` & `pyproteinsext-3.1.2/pyproteinsext/proteinContainer.py`

 * *Files identical despite different names*

### Comparing `pyproteinsext-3.1.1/pyproteinsext/psicquic.py` & `pyproteinsext-3.1.2/pyproteinsext/psicquic.py`

 * *Files identical despite different names*

### Comparing `pyproteinsext-3.1.1/pyproteinsext/refseq.py` & `pyproteinsext-3.1.2/pyproteinsext/refseq.py`

 * *Files identical despite different names*

### Comparing `pyproteinsext-3.1.1/pyproteinsext/services/uniprot/__init__.py` & `pyproteinsext-3.1.2/pyproteinsext/services/uniprot/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproteinsext-3.1.1/pyproteinsext/services/uniprot/collectionProxy.py` & `pyproteinsext-3.1.2/pyproteinsext/services/uniprot/collectionProxy.py`

 * *Files identical despite different names*

### Comparing `pyproteinsext-3.1.1/pyproteinsext/services/uniprot/entryProxy.py` & `pyproteinsext-3.1.2/pyproteinsext/services/uniprot/entryProxy.py`

 * *Files identical despite different names*

### Comparing `pyproteinsext-3.1.1/pyproteinsext/services/uniprot/redisClient.py` & `pyproteinsext-3.1.2/pyproteinsext/services/uniprot/redisClient.py`

 * *Files identical despite different names*

### Comparing `pyproteinsext-3.1.1/pyproteinsext/setup.py` & `pyproteinsext-3.1.2/pyproteinsext/setup.py`

 * *Files identical despite different names*

### Comparing `pyproteinsext-3.1.1/pyproteinsext/tmhmmContainerFactory.py` & `pyproteinsext-3.1.2/pyproteinsext/tmhmmContainerFactory.py`

 * *Files identical despite different names*

### Comparing `pyproteinsext-3.1.1/pyproteinsext/topology.py` & `pyproteinsext-3.1.2/pyproteinsext/topology.py`

 * *Files identical despite different names*

### Comparing `pyproteinsext-3.1.1/pyproteinsext/uniprot.py` & `pyproteinsext-3.1.2/pyproteinsext/uniprot.py`

 * *Files identical despite different names*

### Comparing `pyproteinsext-3.1.1/pyproteinsext/uniprotAnnotator.py` & `pyproteinsext-3.1.2/pyproteinsext/uniprotAnnotator.py`

 * *Files identical despite different names*

### Comparing `pyproteinsext-3.1.1/setup.py` & `pyproteinsext-3.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,30 +7,27 @@
 package_data = \
 {'': ['*'],
  'pyproteinsext': ['notebooks/*',
                    'notebooks/.ipynb_checkpoints/*',
                    'notebooks/data/*']}
 
 install_requires = \
-['biopython>=1.79,<2.0',
- 'bs4>=0.0.1,<0.0.2',
- 'networkx>=2.6.3,<3.0.0',
- 'pyproteins>=2.0.0,<3.0.0']
+['biopython>=1.79,<2.0', 'bs4>=0.0.1,<0.0.2', 'pyproteins>=2.0.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'pyproteinsext',
-    'version': '3.1.1',
+    'version': '3.1.2',
     'description': "'Extending pyproteins for bioinformatics tools&services'",
     'long_description': None,
     'author': 'glaunay',
     'author_email': 'pitooon@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `pyproteinsext-3.1.1/PKG-INFO` & `pyproteinsext-3.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: pyproteinsext
-Version: 3.1.1
+Version: 3.1.2
 Summary: 'Extending pyproteins for bioinformatics tools&services'
 License: BSD
 Author: glaunay
 Author-email: pitooon@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: biopython (>=1.79,<2.0)
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
-Requires-Dist: networkx (>=2.6.3,<3.0.0)
 Requires-Dist: pyproteins (>=2.0.0,<3.0.0)
```

