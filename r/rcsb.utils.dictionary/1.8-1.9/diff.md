# Comparing `tmp/rcsb.utils.dictionary-1.8.tar.gz` & `tmp/rcsb.utils.dictionary-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.utils.dictionary-1.8.tar", last modified: Thu Apr  6 11:55:17 2023, max compression
+gzip compressed data, was "rcsb.utils.dictionary-1.9.tar", last modified: Tue May  2 14:54:04 2023, max compression
```

## Comparing `rcsb.utils.dictionary-1.8.tar` & `rcsb.utils.dictionary-1.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-06 11:55:17.240972 rcsb.utils.dictionary-1.8/
--rw-r--r--   0 vsts      (1001) docker     (122)    10293 2023-04-06 11:49:17.000000 rcsb.utils.dictionary-1.8/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-04-06 11:49:17.000000 rcsb.utils.dictionary-1.8/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      113 2023-04-06 11:49:17.000000 rcsb.utils.dictionary-1.8/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     1674 2023-04-06 11:55:17.240972 rcsb.utils.dictionary-1.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      986 2023-04-06 11:49:17.000000 rcsb.utils.dictionary-1.8/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-06 11:55:17.232972 rcsb.utils.dictionary-1.8/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-04-06 11:49:17.000000 rcsb.utils.dictionary-1.8/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-06 11:55:17.236972 rcsb.utils.dictionary-1.8/rcsb/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-04-06 11:49:17.000000 rcsb.utils.dictionary-1.8/rcsb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-06 11:55:17.240972 rcsb.utils.dictionary-1.8/rcsb/utils/dictionary/
--rw-r--r--   0 vsts      (1001) docker     (122)    38239 2023-04-06 11:49:17.000000 rcsb.utils.dictionary-1.8/rcsb/utils/dictionary/DictMethodAssemblyHelper.py
--rw-r--r--   0 vsts      (1001) docker     (122)    46584 2023-04-06 11:49:17.000000 rcsb.utils.dictionary-1.8/rcsb/utils/dictionary/DictMethodChemRefHelper.py
--rw-r--r--   0 vsts      (1001) docker     (122)   200580 2023-04-06 11:49:17.000000 rcsb.utils.dictionary-1.8/rcsb/utils/dictionary/DictMethodCommonUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)    20846 2023-04-06 11:49:17.000000 rcsb.utils.dictionary-1.8/rcsb/utils/dictionary/DictMethodCompModelHelper.py
--rw-r--r--   0 vsts      (1001) docker     (122)   138579 2023-04-06 11:49:17.000000 rcsb.utils.dictionary-1.8/rcsb/utils/dictionary/DictMethodEntityHelper.py
--rw-r--r--   0 vsts      (1001) docker     (122)   143571 2023-04-06 11:49:17.000000 rcsb.utils.dictionary-1.8/rcsb/utils/dictionary/DictMethodEntityInstanceHelper.py
--rw-r--r--   0 vsts      (1001) docker     (122)    65391 2023-04-06 11:49:17.000000 rcsb.utils.dictionary-1.8/rcsb/utils/dictionary/DictMethodEntryHelper.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6094 2023-04-06 11:49:17.000000 rcsb.utils.dictionary-1.8/rcsb/utils/dictionary/DictMethodResourceCacheWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)    35595 2023-04-06 11:49:17.000000 rcsb.utils.dictionary-1.8/rcsb/utils/dictionary/DictMethodResourceProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9779 2023-04-06 11:49:17.000000 rcsb.utils.dictionary-1.8/rcsb/utils/dictionary/DictMethodRunner.py
--rw-r--r--   0 vsts      (1001) docker     (122)    48393 2023-04-06 11:49:17.000000 rcsb.utils.dictionary-1.8/rcsb/utils/dictionary/DictMethodSecStructUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4097 2023-04-06 11:49:17.000000 rcsb.utils.dictionary-1.8/rcsb/utils/dictionary/DictionaryApiProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3783 2023-04-06 11:49:17.000000 rcsb.utils.dictionary-1.8/rcsb/utils/dictionary/DictionaryApiProviderWrapper.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13373 2023-04-06 11:49:17.000000 rcsb.utils.dictionary-1.8/rcsb/utils/dictionary/NeighborInteractionProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4196 2023-04-06 11:49:17.000000 rcsb.utils.dictionary-1.8/rcsb/utils/dictionary/NeighborInteractionWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-04-06 11:49:17.000000 rcsb.utils.dictionary-1.8/rcsb/utils/dictionary/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-06 11:55:17.236972 rcsb.utils.dictionary-1.8/rcsb.utils.dictionary.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1674 2023-04-06 11:55:17.000000 rcsb.utils.dictionary-1.8/rcsb.utils.dictionary.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1175 2023-04-06 11:55:17.000000 rcsb.utils.dictionary-1.8/rcsb.utils.dictionary.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-06 11:55:17.000000 rcsb.utils.dictionary-1.8/rcsb.utils.dictionary.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-06 11:55:14.000000 rcsb.utils.dictionary-1.8/rcsb.utils.dictionary.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      385 2023-04-06 11:55:17.000000 rcsb.utils.dictionary-1.8/rcsb.utils.dictionary.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-04-06 11:55:17.000000 rcsb.utils.dictionary-1.8/rcsb.utils.dictionary.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      374 2023-04-06 11:49:17.000000 rcsb.utils.dictionary-1.8/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-04-06 11:55:17.240972 rcsb.utils.dictionary-1.8/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (122)     2242 2023-04-06 11:49:17.000000 rcsb.utils.dictionary-1.8/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-02 14:54:04.709210 rcsb.utils.dictionary-1.9/
+-rw-r--r--   0 vsts      (1001) docker     (122)    10366 2023-05-02 14:47:55.000000 rcsb.utils.dictionary-1.9/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-05-02 14:47:55.000000 rcsb.utils.dictionary-1.9/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      113 2023-05-02 14:47:55.000000 rcsb.utils.dictionary-1.9/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     1674 2023-05-02 14:54:04.709210 rcsb.utils.dictionary-1.9/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      986 2023-05-02 14:47:55.000000 rcsb.utils.dictionary-1.9/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-02 14:54:04.697210 rcsb.utils.dictionary-1.9/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-02 14:47:55.000000 rcsb.utils.dictionary-1.9/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-02 14:54:04.701210 rcsb.utils.dictionary-1.9/rcsb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-02 14:47:55.000000 rcsb.utils.dictionary-1.9/rcsb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-02 14:54:04.709210 rcsb.utils.dictionary-1.9/rcsb/utils/dictionary/
+-rw-r--r--   0 vsts      (1001) docker     (122)    38239 2023-05-02 14:47:55.000000 rcsb.utils.dictionary-1.9/rcsb/utils/dictionary/DictMethodAssemblyHelper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    46584 2023-05-02 14:47:55.000000 rcsb.utils.dictionary-1.9/rcsb/utils/dictionary/DictMethodChemRefHelper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)   200580 2023-05-02 14:47:55.000000 rcsb.utils.dictionary-1.9/rcsb/utils/dictionary/DictMethodCommonUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    20846 2023-05-02 14:47:55.000000 rcsb.utils.dictionary-1.9/rcsb/utils/dictionary/DictMethodCompModelHelper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)   138413 2023-05-02 14:47:55.000000 rcsb.utils.dictionary-1.9/rcsb/utils/dictionary/DictMethodEntityHelper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)   143571 2023-05-02 14:47:55.000000 rcsb.utils.dictionary-1.9/rcsb/utils/dictionary/DictMethodEntityInstanceHelper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    65391 2023-05-02 14:47:55.000000 rcsb.utils.dictionary-1.9/rcsb/utils/dictionary/DictMethodEntryHelper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6094 2023-05-02 14:47:55.000000 rcsb.utils.dictionary-1.9/rcsb/utils/dictionary/DictMethodResourceCacheWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    35595 2023-05-02 14:47:55.000000 rcsb.utils.dictionary-1.9/rcsb/utils/dictionary/DictMethodResourceProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9779 2023-05-02 14:47:55.000000 rcsb.utils.dictionary-1.9/rcsb/utils/dictionary/DictMethodRunner.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    48393 2023-05-02 14:47:55.000000 rcsb.utils.dictionary-1.9/rcsb/utils/dictionary/DictMethodSecStructUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4097 2023-05-02 14:47:55.000000 rcsb.utils.dictionary-1.9/rcsb/utils/dictionary/DictionaryApiProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3783 2023-05-02 14:47:55.000000 rcsb.utils.dictionary-1.9/rcsb/utils/dictionary/DictionaryApiProviderWrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13373 2023-05-02 14:47:55.000000 rcsb.utils.dictionary-1.9/rcsb/utils/dictionary/NeighborInteractionProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4196 2023-05-02 14:47:55.000000 rcsb.utils.dictionary-1.9/rcsb/utils/dictionary/NeighborInteractionWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-05-02 14:47:55.000000 rcsb.utils.dictionary-1.9/rcsb/utils/dictionary/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-02 14:54:04.697210 rcsb.utils.dictionary-1.9/rcsb.utils.dictionary.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1674 2023-05-02 14:54:04.000000 rcsb.utils.dictionary-1.9/rcsb.utils.dictionary.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1175 2023-05-02 14:54:04.000000 rcsb.utils.dictionary-1.9/rcsb.utils.dictionary.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-02 14:54:04.000000 rcsb.utils.dictionary-1.9/rcsb.utils.dictionary.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-02 14:54:03.000000 rcsb.utils.dictionary-1.9/rcsb.utils.dictionary.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      385 2023-05-02 14:54:04.000000 rcsb.utils.dictionary-1.9/rcsb.utils.dictionary.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-05-02 14:54:04.000000 rcsb.utils.dictionary-1.9/rcsb.utils.dictionary.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      374 2023-05-02 14:47:55.000000 rcsb.utils.dictionary-1.9/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-05-02 14:54:04.709210 rcsb.utils.dictionary-1.9/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     2242 2023-05-02 14:47:55.000000 rcsb.utils.dictionary-1.9/setup.py
```

### Comparing `rcsb.utils.dictionary-1.8/HISTORY.txt` & `rcsb.utils.dictionary-1.9/HISTORY.txt`

 * *Files 1% similar despite different names*

```diff
@@ -105,8 +105,9 @@
 07-Mar-2023 - V1.04 Bug fix in DictMethodChemRefHelper;
                     Stop loading CARD data to rcsb_polymer_entity_feature
 14-Mar-2023 - V1.05 Load CARD annotation data to rcsb_polymer_entity_annotation
 16-Mar-2023 - V1.06 Update configuration of DictMethodResourceCacheWorkflow() and NeighborInteractionWorkflow() to use HERE and CACHE folder
 20-Mar-2023 - V1.07 Fix formula weight calculation of CSM polymer entities
  5-Apr-2023 - V1.08 Update population of provenance_source attributes for taxonomy/organism and gene categories;
                     Correct attribute name for rcsb_chem_comp_target provenance;
-                    Stop loading rcsb_chem_comp_synonyms for type 'Brand Name'
+                    Stop loading rcsb_chem_comp_synonyms for type 'Brand Name'
+ 2-May-2023 - V1.09 Stop loading depth data for CARD lineage annotations
```

### Comparing `rcsb.utils.dictionary-1.8/LICENSE` & `rcsb.utils.dictionary-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.utils.dictionary-1.8/PKG-INFO` & `rcsb.utils.dictionary-1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.dictionary
-Version: 1.8
+Version: 1.9
 Summary: RCSB Python Dictionary Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_utils_dictionary
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.dictionary-1.8/README.md` & `rcsb.utils.dictionary-1.9/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.utils.dictionary-1.8/rcsb/utils/dictionary/DictMethodAssemblyHelper.py` & `rcsb.utils.dictionary-1.9/rcsb/utils/dictionary/DictMethodAssemblyHelper.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.dictionary-1.8/rcsb/utils/dictionary/DictMethodChemRefHelper.py` & `rcsb.utils.dictionary-1.9/rcsb/utils/dictionary/DictMethodChemRefHelper.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.dictionary-1.8/rcsb/utils/dictionary/DictMethodCommonUtils.py` & `rcsb.utils.dictionary-1.9/rcsb/utils/dictionary/DictMethodCommonUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.dictionary-1.8/rcsb/utils/dictionary/DictMethodCompModelHelper.py` & `rcsb.utils.dictionary-1.9/rcsb/utils/dictionary/DictMethodCompModelHelper.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.dictionary-1.8/rcsb/utils/dictionary/DictMethodEntityHelper.py` & `rcsb.utils.dictionary-1.9/rcsb/utils/dictionary/DictMethodEntityHelper.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #   3-May-2022 dwp Use internal computed-model identifiers for 'entry_id' in containter_identifiers
 #  23-Jun-2022 bv  Use ma_target_ref_db_details to populate rcsb_polymer_entity_container_identifiers.reference_sequence_identifiers for MA models
 #  29-Jun-2022 dwp Use internal computed-model identifiers everywhere (in same manner as experimental models)
 #  21-Jul-2022 dwp Fix logic for assigning reference sequence identifiers for computed models
 #   6-Mar-2023 dwp Stop loading CARD data to rcsb_polymer_entity_feature
 #  14-Mar-2023 dwp Load CARD data to rcsb_polymer_entity_annotation
 #  28-Mar-2023 dwp Populate 'rcsb_entity_source_organism.provenance_source' with transient value from 'entity_src_nat.rcsb_provenance_source' (applicable to CSMs only)
+#   2-May-2023 dwp Stop loading depth data for CARD lineage annotations
 ##
 """
 Helper class implements methods supporting entity-level item and category methods in the RCSB dictionary extension.
 
 """
 __docformat__ = "google en"
 __author__ = "John Westbrook"
@@ -2657,15 +2658,14 @@
                             addPropTupL.append(("CARD_ARO_CVTERM_ID", fD["card_aro_cvterm_id"]))
                             cObj.setValue(";".join([str(tup[0]) for tup in addPropTupL]), "additional_properties_name", ii)
                             cObj.setValue(";".join([str(tup[1]) for tup in addPropTupL]), "additional_properties_values", ii)
                             #
                             idLinL = fD["annotation_lineage"]
                             cObj.setValue(";".join([str(lD["id"]) for lD in idLinL]), "annotation_lineage_id", ii)
                             cObj.setValue(";".join([str(lD["name"]) for lD in idLinL]), "annotation_lineage_name", ii)
-                            cObj.setValue(";".join([str(lD["depth"]) for lD in idLinL]), "annotation_lineage_depth", ii)
                             #
                             ii += 1
                         # Now add "AMR Gene Family" annotation (applicable for all entities)
                         cObj.setValue(ii + 1, "ordinal", ii)
                         cObj.setValue(entryId, "entry_id", ii)
                         cObj.setValue(entityId, "entity_id", ii)
                         cObj.setValue("CARD", "type", ii)
@@ -2681,15 +2681,14 @@
                         addPropTupL.append(("CARD_ARO_RESISTANCE_MECHANISM", fD["card_aro_resistance_mechanism"]))
                         cObj.setValue(";".join([str(tup[0]) for tup in addPropTupL]), "additional_properties_name", ii)
                         cObj.setValue(";".join([str(tup[1]) for tup in addPropTupL]), "additional_properties_values", ii)
                         #
                         idLinL = fD["family_annotation_lineage"]
                         cObj.setValue(";".join([str(lD["id"]) for lD in idLinL]), "annotation_lineage_id", ii)
                         cObj.setValue(";".join([str(lD["name"]) for lD in idLinL]), "annotation_lineage_name", ii)
-                        cObj.setValue(";".join([str(lD["depth"]) for lD in idLinL]), "annotation_lineage_depth", ii)
                         #
                         ii += 1
                         #
             # ---
             skipBird = True  # JDW added this in: https://github.com/rcsb/py-rcsb_db/commit/c3432f32859557042cfb77d69cb9e2fea1b4bfac
             if not skipBird:
                 # BIRD type and class
```

### Comparing `rcsb.utils.dictionary-1.8/rcsb/utils/dictionary/DictMethodEntityInstanceHelper.py` & `rcsb.utils.dictionary-1.9/rcsb/utils/dictionary/DictMethodEntityInstanceHelper.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.dictionary-1.8/rcsb/utils/dictionary/DictMethodEntryHelper.py` & `rcsb.utils.dictionary-1.9/rcsb/utils/dictionary/DictMethodEntryHelper.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.dictionary-1.8/rcsb/utils/dictionary/DictMethodResourceCacheWorkflow.py` & `rcsb.utils.dictionary-1.9/rcsb/utils/dictionary/DictMethodResourceCacheWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.dictionary-1.8/rcsb/utils/dictionary/DictMethodResourceProvider.py` & `rcsb.utils.dictionary-1.9/rcsb/utils/dictionary/DictMethodResourceProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.dictionary-1.8/rcsb/utils/dictionary/DictMethodRunner.py` & `rcsb.utils.dictionary-1.9/rcsb/utils/dictionary/DictMethodRunner.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.dictionary-1.8/rcsb/utils/dictionary/DictMethodSecStructUtils.py` & `rcsb.utils.dictionary-1.9/rcsb/utils/dictionary/DictMethodSecStructUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.dictionary-1.8/rcsb/utils/dictionary/DictionaryApiProvider.py` & `rcsb.utils.dictionary-1.9/rcsb/utils/dictionary/DictionaryApiProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.dictionary-1.8/rcsb/utils/dictionary/DictionaryApiProviderWrapper.py` & `rcsb.utils.dictionary-1.9/rcsb/utils/dictionary/DictionaryApiProviderWrapper.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.dictionary-1.8/rcsb/utils/dictionary/NeighborInteractionProvider.py` & `rcsb.utils.dictionary-1.9/rcsb/utils/dictionary/NeighborInteractionProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.dictionary-1.8/rcsb/utils/dictionary/NeighborInteractionWorkflow.py` & `rcsb.utils.dictionary-1.9/rcsb/utils/dictionary/NeighborInteractionWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.dictionary-1.8/rcsb.utils.dictionary.egg-info/PKG-INFO` & `rcsb.utils.dictionary-1.9/rcsb.utils.dictionary.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.dictionary
-Version: 1.8
+Version: 1.9
 Summary: RCSB Python Dictionary Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_utils_dictionary
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.dictionary-1.8/rcsb.utils.dictionary.egg-info/SOURCES.txt` & `rcsb.utils.dictionary-1.9/rcsb.utils.dictionary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.utils.dictionary-1.8/setup.py` & `rcsb.utils.dictionary-1.9/setup.py`

 * *Files identical despite different names*

