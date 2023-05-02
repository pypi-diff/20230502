# Comparing `tmp/parsigs-0.0.1.tar.gz` & `tmp/parsigs-0.0.1b0.tar.gz`

## Comparing `parsigs-0.0.1.tar` & `parsigs-0.0.1b0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 parsigs-0.0.1/contributing.md
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 parsigs-0.0.1/playground.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 parsigs-0.0.1/requirements.txt
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 parsigs-0.0.1/.github/workflows/starter-workflow.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parsigs-0.0.1/parsigs/__init__.py
--rw-r--r--   0        0        0     7668 2020-02-02 00:00:00.000000 parsigs-0.0.1/parsigs/parse_sig_api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parsigs-0.0.1/research/__init__.py
--rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 parsigs-0.0.1/research/dosage_instructions_ner.ipynb
--rw-r--r--   0        0        0    10695 2020-02-02 00:00:00.000000 parsigs-0.0.1/research/dosage_instructions_ner_bert.ipynb
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 parsigs-0.0.1/research/pre_process_data.py
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 parsigs-0.0.1/research/config/config.cfg
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 parsigs-0.0.1/research/config/config_bert.cfg
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 parsigs-0.0.1/research/config/config_compact_bert.cfg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parsigs-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 parsigs-0.0.1/tests/test_parsig_api.py
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 parsigs-0.0.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 parsigs-0.0.1/LICENSE
--rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 parsigs-0.0.1/README.md
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 parsigs-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 parsigs-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 parsigs-0.0.1b0/contributing.md
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 parsigs-0.0.1b0/playground.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 parsigs-0.0.1b0/requirements.txt
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 parsigs-0.0.1b0/.github/workflows/starter-workflow.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parsigs-0.0.1b0/parsigs/__init__.py
+-rw-r--r--   0        0        0     7668 2020-02-02 00:00:00.000000 parsigs-0.0.1b0/parsigs/parse_sig_api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parsigs-0.0.1b0/research/__init__.py
+-rw-r--r--   0        0        0     8664 2020-02-02 00:00:00.000000 parsigs-0.0.1b0/research/dosage_instructions_ner.ipynb
+-rw-r--r--   0        0        0    10695 2020-02-02 00:00:00.000000 parsigs-0.0.1b0/research/dosage_instructions_ner_bert.ipynb
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 parsigs-0.0.1b0/research/pre_process_data.py
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 parsigs-0.0.1b0/research/config/config.cfg
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 parsigs-0.0.1b0/research/config/config_bert.cfg
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 parsigs-0.0.1b0/research/config/config_compact_bert.cfg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parsigs-0.0.1b0/tests/__init__.py
+-rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 parsigs-0.0.1b0/tests/test_parsig_api.py
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 parsigs-0.0.1b0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 parsigs-0.0.1b0/LICENSE
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 parsigs-0.0.1b0/README.md
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 parsigs-0.0.1b0/pyproject.toml
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 parsigs-0.0.1b0/PKG-INFO
```

### Comparing `parsigs-0.0.1/.github/workflows/starter-workflow.yaml` & `parsigs-0.0.1b0/.github/workflows/starter-workflow.yaml`

 * *Files identical despite different names*

### Comparing `parsigs-0.0.1/parsigs/parse_sig_api.py` & `parsigs-0.0.1b0/parsigs/parse_sig_api.py`

 * *Files identical despite different names*

### Comparing `parsigs-0.0.1/research/dosage_instructions_ner.ipynb` & `parsigs-0.0.1b0/research/dosage_instructions_ner.ipynb`

 * *Files identical despite different names*

### Comparing `parsigs-0.0.1/research/dosage_instructions_ner_bert.ipynb` & `parsigs-0.0.1b0/research/dosage_instructions_ner_bert.ipynb`

 * *Files identical despite different names*

### Comparing `parsigs-0.0.1/research/pre_process_data.py` & `parsigs-0.0.1b0/research/pre_process_data.py`

 * *Files identical despite different names*

### Comparing `parsigs-0.0.1/research/config/config.cfg` & `parsigs-0.0.1b0/research/config/config.cfg`

 * *Files identical despite different names*

### Comparing `parsigs-0.0.1/research/config/config_bert.cfg` & `parsigs-0.0.1b0/research/config/config_bert.cfg`

 * *Files identical despite different names*

### Comparing `parsigs-0.0.1/research/config/config_compact_bert.cfg` & `parsigs-0.0.1b0/research/config/config_compact_bert.cfg`

 * *Files identical despite different names*

### Comparing `parsigs-0.0.1/tests/test_parsig_api.py` & `parsigs-0.0.1b0/tests/test_parsig_api.py`

 * *Files identical despite different names*

### Comparing `parsigs-0.0.1/.gitignore` & `parsigs-0.0.1b0/.gitignore`

 * *Files identical despite different names*

### Comparing `parsigs-0.0.1/LICENSE` & `parsigs-0.0.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `parsigs-0.0.1/README.md` & `parsigs-0.0.1b0/README.md`

 * *Files identical despite different names*

### Comparing `parsigs-0.0.1/pyproject.toml` & `parsigs-0.0.1b0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "parsigs"
-version = "0.0.1"
+version = "0.0.1_beta"
 authors = [
-  { name="Roy Ashcenazi", email="royashcenazi@gmail.com" },
+    { name = "Roy Ashcenazi", email = "royashcenazi@gmail.com" },
 ]
 description = "The private, smart and easy Sig (Dosage Instructions) text-parser"
 readme = "README.md"
+dependencies = [
+    "spacy",
+    "word2number"
+]
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `parsigs-0.0.1/PKG-INFO` & `parsigs-0.0.1b0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: parsigs
-Version: 0.0.1
+Version: 0.0.1b0
 Summary: The private, smart and easy Sig (Dosage Instructions) text-parser
 Project-URL: Homepage, https://github.com/royashcenazi/parsigs
 Project-URL: Bug Tracker, https://github.com/royashcenazi/parsigs/issues
 Author-email: Roy Ashcenazi <royashcenazi@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: spacy
+Requires-Dist: word2number
 Description-Content-Type: text/markdown
 
 # Parsigs - the private, smart and easy Sig (Dosage Instructions) text-parser 
 
 Parsigs is an open-source project that aims to extract relevant information from doctors' signature text without compromising privacy and PHI (Protected Health Information) using Natural Language Processing.
 
 ## Features
```

