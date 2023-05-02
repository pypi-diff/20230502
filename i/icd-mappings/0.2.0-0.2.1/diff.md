# Comparing `tmp/icd_mappings-0.2.0.tar.gz` & `tmp/icd_mappings-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icd_mappings-0.2.0.tar", max compression
+gzip compressed data, was "icd_mappings-0.2.1.tar", max compression
```

## Comparing `icd_mappings-0.2.0.tar` & `icd_mappings-0.2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1992 2023-04-26 11:33:59.681730 icd_mappings-0.2.0/README.md
--rw-r--r--   0        0        0       31 2023-03-15 14:37:28.554849 icd_mappings-0.2.0/icdmappings/__init__.py
--rw-r--r--   0        0        0   106285 2021-07-12 11:47:18.000000 icd_mappings-0.2.0/icdmappings/data_files/CCS-SingleDiagnosisGrouper.txt
--rw-r--r--   0        0        0   897559 2023-04-26 11:30:37.278877 icd_mappings-0.2.0/icdmappings/data_files/ICD_9_CM_v32_master_descriptions/CMS32_DESC_LONG_DX.txt
--rw-r--r--   0        0        0   182309 2023-03-31 16:11:55.490825 icd_mappings-0.2.0/icdmappings/data_files/ICD_9_CM_v32_master_descriptions/CMS32_DESC_LONG_SG.txt
--rw-r--r--   0        0        0   418158 2013-06-13 10:42:38.000000 icd_mappings-0.2.0/icdmappings/data_files/ICD_9_CM_v32_master_descriptions/CMS32_DESC_SHORT_DX.txt
--rw-r--r--   0        0        0   107145 2013-06-26 12:34:24.000000 icd_mappings-0.2.0/icdmappings/data_files/ICD_9_CM_v32_master_descriptions/CMS32_DESC_SHORT_SG.txt
--rw-r--r--   0        0        0        0 2023-04-27 16:29:57.530715 icd_mappings-0.2.0/icdmappings/data_files/ICD_9_CM_v32_master_descriptions/__init__.py
--rw-r--r--   0        0        0      311 2023-03-13 09:49:16.855619 icd_mappings-0.2.0/icdmappings/data_files/ICD_9_CM_v32_master_descriptions/readme.md
--rw-r--r--   0        0        0        0 2023-03-13 11:37:06.004050 icd_mappings-0.2.0/icdmappings/data_files/__init__.py
--rw-r--r--   0        0        0   629547 2022-06-20 16:29:42.984515 icd_mappings-0.2.0/icdmappings/data_files/cci2015.csv
--rw-r--r--   0        0        0  2766948 2022-09-21 16:12:43.000000 icd_mappings-0.2.0/icdmappings/data_files/icd10cmtoicd9gem.csv
--rw-r--r--   0        0        0     1087 2021-07-19 15:30:56.000000 icd_mappings-0.2.0/icdmappings/data_files/icd9-CM-code-chapter-en=PT.csv
--rw-r--r--   0        0        0  1427817 2022-06-23 13:00:01.514335 icd_mappings-0.2.0/icdmappings/data_files/icd9dx2015.csv
--rw-r--r--   0        0        0   821109 2022-06-21 13:09:55.045319 icd_mappings-0.2.0/icdmappings/data_files/icd9toicd10cmgem.csv
--rw-r--r--   0        0        0     2132 2023-04-26 14:04:37.870674 icd_mappings-0.2.0/icdmappings/icdmappings.py
--rw-r--r--   0        0        0      448 2023-04-28 14:13:01.025512 icd_mappings-0.2.0/icdmappings/mappers/__init__.py
--rw-r--r--   0        0        0     1807 2023-04-27 16:25:13.969388 icd_mappings-0.2.0/icdmappings/mappers/icd10_to_icd9.py
--rw-r--r--   0        0        0     2341 2023-04-27 16:33:49.924682 icd_mappings-0.2.0/icdmappings/mappers/icd9_to_cci.py
--rw-r--r--   0        0        0     4639 2023-04-27 16:23:09.059449 icd_mappings-0.2.0/icdmappings/mappers/icd9_to_ccs.py
--rw-r--r--   0        0        0     3157 2023-04-27 16:23:57.508814 icd_mappings-0.2.0/icdmappings/mappers/icd9_to_chapters.py
--rw-r--r--   0        0        0     1819 2023-04-27 16:24:45.052915 icd_mappings-0.2.0/icdmappings/mappers/icd9_to_icd10.py
--rw-r--r--   0        0        0      760 2023-04-27 15:23:41.254667 icd_mappings-0.2.0/icdmappings/mappers/icd9_to_level3.py
--rw-r--r--   0        0        0     4903 2023-04-28 14:15:34.482740 icd_mappings-0.2.0/icdmappings/mappers/icd9level3_to_ccs.py
--rw-r--r--   0        0        0      491 2023-04-26 14:00:22.255137 icd_mappings-0.2.0/icdmappings/mappers/mapper_interface.py
--rw-r--r--   0        0        0      100 2023-03-14 10:04:00.087660 icd_mappings-0.2.0/icdmappings/validators/__init__.py
--rw-r--r--   0        0        0     3015 2023-04-27 16:32:08.174950 icd_mappings-0.2.0/icdmappings/validators/icd9_validator.py
--rw-r--r--   0        0        0      735 2023-04-26 14:39:04.763355 icd_mappings-0.2.0/icdmappings/validators/icd_validator_interface.py
--rw-r--r--   0        0        0      661 2023-04-28 14:22:37.525825 icd_mappings-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2822 1970-01-01 00:00:00.000000 icd_mappings-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2002 2023-04-28 14:23:08.766954 icd_mappings-0.2.1/README.md
+-rw-r--r--   0        0        0       45 2023-04-28 14:33:52.698035 icd_mappings-0.2.1/icdmappings/__init__.py
+-rw-r--r--   0        0        0   106285 2021-07-12 11:47:18.000000 icd_mappings-0.2.1/icdmappings/data_files/CCS-SingleDiagnosisGrouper.txt
+-rw-r--r--   0        0        0   897559 2023-04-26 11:30:37.278877 icd_mappings-0.2.1/icdmappings/data_files/ICD_9_CM_v32_master_descriptions/CMS32_DESC_LONG_DX.txt
+-rw-r--r--   0        0        0   182309 2023-03-31 16:11:55.490825 icd_mappings-0.2.1/icdmappings/data_files/ICD_9_CM_v32_master_descriptions/CMS32_DESC_LONG_SG.txt
+-rw-r--r--   0        0        0   418158 2013-06-13 10:42:38.000000 icd_mappings-0.2.1/icdmappings/data_files/ICD_9_CM_v32_master_descriptions/CMS32_DESC_SHORT_DX.txt
+-rw-r--r--   0        0        0   107145 2013-06-26 12:34:24.000000 icd_mappings-0.2.1/icdmappings/data_files/ICD_9_CM_v32_master_descriptions/CMS32_DESC_SHORT_SG.txt
+-rw-r--r--   0        0        0        0 2023-04-27 16:29:57.530715 icd_mappings-0.2.1/icdmappings/data_files/ICD_9_CM_v32_master_descriptions/__init__.py
+-rw-r--r--   0        0        0      311 2023-03-13 09:49:16.855619 icd_mappings-0.2.1/icdmappings/data_files/ICD_9_CM_v32_master_descriptions/readme.md
+-rw-r--r--   0        0        0        0 2023-03-13 11:37:06.004050 icd_mappings-0.2.1/icdmappings/data_files/__init__.py
+-rw-r--r--   0        0        0   629547 2022-06-20 16:29:42.984515 icd_mappings-0.2.1/icdmappings/data_files/cci2015.csv
+-rw-r--r--   0        0        0  2766948 2022-09-21 16:12:43.000000 icd_mappings-0.2.1/icdmappings/data_files/icd10cmtoicd9gem.csv
+-rw-r--r--   0        0        0     1087 2021-07-19 15:30:56.000000 icd_mappings-0.2.1/icdmappings/data_files/icd9-CM-code-chapter-en=PT.csv
+-rw-r--r--   0        0        0  1427817 2022-06-23 13:00:01.514335 icd_mappings-0.2.1/icdmappings/data_files/icd9dx2015.csv
+-rw-r--r--   0        0        0   821109 2022-06-21 13:09:55.045319 icd_mappings-0.2.1/icdmappings/data_files/icd9toicd10cmgem.csv
+-rw-r--r--   0        0        0     2238 2023-05-02 12:00:27.079365 icd_mappings-0.2.1/icdmappings/icdmappings.py
+-rw-r--r--   0        0        0      448 2023-04-28 14:13:01.025512 icd_mappings-0.2.1/icdmappings/mappers/__init__.py
+-rw-r--r--   0        0        0     1807 2023-04-27 16:25:13.969388 icd_mappings-0.2.1/icdmappings/mappers/icd10_to_icd9.py
+-rw-r--r--   0        0        0     2341 2023-04-27 16:33:49.924682 icd_mappings-0.2.1/icdmappings/mappers/icd9_to_cci.py
+-rw-r--r--   0        0        0     4639 2023-04-27 16:23:09.059449 icd_mappings-0.2.1/icdmappings/mappers/icd9_to_ccs.py
+-rw-r--r--   0        0        0     3157 2023-04-27 16:23:57.508814 icd_mappings-0.2.1/icdmappings/mappers/icd9_to_chapters.py
+-rw-r--r--   0        0        0     1819 2023-04-27 16:24:45.052915 icd_mappings-0.2.1/icdmappings/mappers/icd9_to_icd10.py
+-rw-r--r--   0        0        0      760 2023-04-27 15:23:41.254667 icd_mappings-0.2.1/icdmappings/mappers/icd9_to_level3.py
+-rw-r--r--   0        0        0     4903 2023-04-28 14:15:34.482740 icd_mappings-0.2.1/icdmappings/mappers/icd9level3_to_ccs.py
+-rw-r--r--   0        0        0      491 2023-04-26 14:00:22.255137 icd_mappings-0.2.1/icdmappings/mappers/mapper_interface.py
+-rw-r--r--   0        0        0      129 2023-04-28 14:32:58.827845 icd_mappings-0.2.1/icdmappings/validators/__init__.py
+-rw-r--r--   0        0        0     3015 2023-04-28 15:26:10.584568 icd_mappings-0.2.1/icdmappings/validators/icd9_validator.py
+-rw-r--r--   0        0        0      735 2023-04-26 14:39:04.763355 icd_mappings-0.2.1/icdmappings/validators/icd_validator_interface.py
+-rw-r--r--   0        0        0      661 2023-05-02 12:01:08.776443 icd_mappings-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2832 1970-01-01 00:00:00.000000 icd_mappings-0.2.1/PKG-INFO
```

### Comparing `icd_mappings-0.2.0/README.md` & `icd_mappings-0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,10 @@
 # ICDMappings
-
 This tool helps working with ICD codes. It maps between ICD versions (such as between ICD9 and ICD10). Also maps to other codings such as CCS (Computer Software Classification), and CCI (Chronic Condition Indicator).
 
-List of all mappers:
-- [ICD9<->ICD10](https://www.nber.org/research/data/icd-9-cm-and-icd-10-cm-and-icd-10-pcs-crosswalk-or-general-equivalence-mappings): ICD9-CM and ICD10-CM (in both directions).
-- [ICD9->CCS](): ICD9-CM to CCS (Clinical Classification Software) codes;
-- [ICD9->ICD9Chapters](https://icd.codes/icd9cm): ICD9-CM diagnostic codes to the 19 Chapters;
-- [ICD9->CCI](https://www.hcup-us.ahrq.gov/toolssoftware/chronic/chronic.jsp) ICD9-CM diagnostics to CCI (Chronic Condition Indicator). True of False depending on whether a diagnostic is chronic or not;
-- ICD9->Level3: Gets the 3rd level of an ICD9-CM diagnostic code;
-
-
-Supports mapping either a `single code` at a time, or an `iterable of codes` (range, list, np.array, pd.Series, etc...).
-
-
-> :warning: When ICD9 or ICD10 is mentioned, it always refers to the American version aka ICD9-CM / ICD10-CM.
-
 # Installation
 
 `pip install icd-mappings`
 
 # Usage
 
 ```python
@@ -42,14 +28,29 @@
 >>> ['F0280', 'R111000', None, 'H269']
 
 # You can also check available mappers
 mapper.show_mappers()
 >>> ['icd9toccs', 'icd9toicd10', 'icd10toicd9', 'icd9tochapter', 'icd9tolevel3', 'icd9tocci']
 ```
 
+# Mappers
+
+List of all mappers:
+- [ICD9<->ICD10](https://www.nber.org/research/data/icd-9-cm-and-icd-10-cm-and-icd-10-pcs-crosswalk-or-general-equivalence-mappings): ICD9-CM and ICD10-CM (in both directions).
+- [ICD9->CCS](): ICD9-CM to CCS (Clinical Classification Software) codes;
+- [ICD9->ICD9Chapters](https://icd.codes/icd9cm): ICD9-CM diagnostic codes to the 19 Chapters;
+- [ICD9->CCI](https://www.hcup-us.ahrq.gov/toolssoftware/chronic/chronic.jsp) ICD9-CM diagnostics to CCI (Chronic Condition Indicator). True of False depending on whether a diagnostic is chronic or not;
+- ICD9->Level3: Gets the 3rd level of an ICD9-CM diagnostic code;
+
+
+Supports mapping either a `single code` at a time, or an `iterable of codes` (range, list, np.array, pd.Series, etc...).
+
+
+> :warning: When ICD9 or ICD10 is mentioned, it always refers to the American version aka ICD9-CM / ICD10-CM.
+
 # Feature requests
 
 Feel free to sugest feature requests under `Issues`, such as turning this into a script in case your pipeline does not use python.
 
 
 # Acknowledgments
```

### Comparing `icd_mappings-0.2.0/icdmappings/data_files/CCS-SingleDiagnosisGrouper.txt` & `icd_mappings-0.2.1/icdmappings/data_files/CCS-SingleDiagnosisGrouper.txt`

 * *Files identical despite different names*

### Comparing `icd_mappings-0.2.0/icdmappings/data_files/ICD_9_CM_v32_master_descriptions/CMS32_DESC_LONG_DX.txt` & `icd_mappings-0.2.1/icdmappings/data_files/ICD_9_CM_v32_master_descriptions/CMS32_DESC_LONG_DX.txt`

 * *Files identical despite different names*

### Comparing `icd_mappings-0.2.0/icdmappings/data_files/ICD_9_CM_v32_master_descriptions/CMS32_DESC_LONG_SG.txt` & `icd_mappings-0.2.1/icdmappings/data_files/ICD_9_CM_v32_master_descriptions/CMS32_DESC_LONG_SG.txt`

 * *Files identical despite different names*

### Comparing `icd_mappings-0.2.0/icdmappings/data_files/ICD_9_CM_v32_master_descriptions/CMS32_DESC_SHORT_DX.txt` & `icd_mappings-0.2.1/icdmappings/data_files/ICD_9_CM_v32_master_descriptions/CMS32_DESC_SHORT_DX.txt`

 * *Files identical despite different names*

### Comparing `icd_mappings-0.2.0/icdmappings/data_files/ICD_9_CM_v32_master_descriptions/CMS32_DESC_SHORT_SG.txt` & `icd_mappings-0.2.1/icdmappings/data_files/ICD_9_CM_v32_master_descriptions/CMS32_DESC_SHORT_SG.txt`

 * *Files identical despite different names*

### Comparing `icd_mappings-0.2.0/icdmappings/data_files/cci2015.csv` & `icd_mappings-0.2.1/icdmappings/data_files/cci2015.csv`

 * *Files identical despite different names*

### Comparing `icd_mappings-0.2.0/icdmappings/data_files/icd10cmtoicd9gem.csv` & `icd_mappings-0.2.1/icdmappings/data_files/icd10cmtoicd9gem.csv`

 * *Files identical despite different names*

### Comparing `icd_mappings-0.2.0/icdmappings/data_files/icd9-CM-code-chapter-en=PT.csv` & `icd_mappings-0.2.1/icdmappings/data_files/icd9-CM-code-chapter-en=PT.csv`

 * *Files identical despite different names*

### Comparing `icd_mappings-0.2.0/icdmappings/data_files/icd9dx2015.csv` & `icd_mappings-0.2.1/icdmappings/data_files/icd9dx2015.csv`

 * *Files identical despite different names*

### Comparing `icd_mappings-0.2.0/icdmappings/data_files/icd9toicd10cmgem.csv` & `icd_mappings-0.2.1/icdmappings/data_files/icd9toicd10cmgem.csv`

 * *Files identical despite different names*

### Comparing `icd_mappings-0.2.0/icdmappings/icdmappings.py` & `icd_mappings-0.2.1/icdmappings/icdmappings.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,24 @@
 
     def __init__(self):
 
         # mappers
         self.icd9_to_cci = ICD9toCCI()
         self.icd9_to_level3 = ICD9toLEVEL3()
         self.icd9_to_ccs = ICD9toCCS()
+        self.icd9level3_to_ccs = ICD9Level3toCCS()
         self.icd9_to_chapters = ICD9toChapters()
         self.icd9_to_icd10 = ICD9toICD10()
         self.icd10_to_icd9 = ICD10toICD9()
 
         self._internal_mapping = {
             'icd9tocci': self.icd9_to_cci,
             'icd9tolevel3': self.icd9_to_level3,
             'icd9toccs': self.icd9_to_ccs,
+            'icd9level3toccs': self.icd9level3_to_ccs,
             'icd9tochapter': self.icd9_to_chapters,
             'icd9toicd10': self.icd9_to_icd10,
             'icd10toicd9': self.icd10_to_icd9
         }
 
         # validators
```

### Comparing `icd_mappings-0.2.0/icdmappings/mappers/icd10_to_icd9.py` & `icd_mappings-0.2.1/icdmappings/mappers/icd10_to_icd9.py`

 * *Files identical despite different names*

### Comparing `icd_mappings-0.2.0/icdmappings/mappers/icd9_to_cci.py` & `icd_mappings-0.2.1/icdmappings/mappers/icd9_to_cci.py`

 * *Files identical despite different names*

### Comparing `icd_mappings-0.2.0/icdmappings/mappers/icd9_to_ccs.py` & `icd_mappings-0.2.1/icdmappings/mappers/icd9_to_ccs.py`

 * *Files identical despite different names*

### Comparing `icd_mappings-0.2.0/icdmappings/mappers/icd9_to_chapters.py` & `icd_mappings-0.2.1/icdmappings/mappers/icd9_to_chapters.py`

 * *Files identical despite different names*

### Comparing `icd_mappings-0.2.0/icdmappings/mappers/icd9_to_icd10.py` & `icd_mappings-0.2.1/icdmappings/mappers/icd9_to_icd10.py`

 * *Files identical despite different names*

### Comparing `icd_mappings-0.2.0/icdmappings/mappers/icd9_to_level3.py` & `icd_mappings-0.2.1/icdmappings/mappers/icd9_to_level3.py`

 * *Files identical despite different names*

### Comparing `icd_mappings-0.2.0/icdmappings/mappers/icd9level3_to_ccs.py` & `icd_mappings-0.2.1/icdmappings/mappers/icd9level3_to_ccs.py`

 * *Files identical despite different names*

### Comparing `icd_mappings-0.2.0/icdmappings/validators/icd9_validator.py` & `icd_mappings-0.2.1/icdmappings/validators/icd9_validator.py`

 * *Files identical despite different names*

### Comparing `icd_mappings-0.2.0/icdmappings/validators/icd_validator_interface.py` & `icd_mappings-0.2.1/icdmappings/validators/icd_validator_interface.py`

 * *Files identical despite different names*

### Comparing `icd_mappings-0.2.0/pyproject.toml` & `icd_mappings-0.2.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "icd-mappings"
-version = "0.2.0"
+version = "0.2.1"
 description = "This python tools allows you to map icd codes between versions (9 and 10) and also to other coding schemas such as CCS (Clinical Classification Software))"
 authors = ["Simao Novais <snovaisg.97@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 repository = "https://github.com/snovaisg/ICDMappings"
 packages = [{include = "icdmappings"}]
 include = ["data_sources/*"]
```

### Comparing `icd_mappings-0.2.0/PKG-INFO` & `icd_mappings-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icd-mappings
-Version: 0.2.0
+Version: 0.2.1
 Summary: This python tools allows you to map icd codes between versions (9 and 10) and also to other coding schemas such as CCS (Clinical Classification Software))
 Home-page: https://github.com/snovaisg/ICDMappings
 License: MIT
 Author: Simao Novais
 Author-email: snovaisg.97@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -14,30 +14,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: importlib-resources (>=5.12.0,<6.0.0)
 Project-URL: Repository, https://github.com/snovaisg/ICDMappings
 Description-Content-Type: text/markdown
 
 # ICDMappings
-
 This tool helps working with ICD codes. It maps between ICD versions (such as between ICD9 and ICD10). Also maps to other codings such as CCS (Computer Software Classification), and CCI (Chronic Condition Indicator).
 
-List of all mappers:
-- [ICD9<->ICD10](https://www.nber.org/research/data/icd-9-cm-and-icd-10-cm-and-icd-10-pcs-crosswalk-or-general-equivalence-mappings): ICD9-CM and ICD10-CM (in both directions).
-- [ICD9->CCS](): ICD9-CM to CCS (Clinical Classification Software) codes;
-- [ICD9->ICD9Chapters](https://icd.codes/icd9cm): ICD9-CM diagnostic codes to the 19 Chapters;
-- [ICD9->CCI](https://www.hcup-us.ahrq.gov/toolssoftware/chronic/chronic.jsp) ICD9-CM diagnostics to CCI (Chronic Condition Indicator). True of False depending on whether a diagnostic is chronic or not;
-- ICD9->Level3: Gets the 3rd level of an ICD9-CM diagnostic code;
-
-
-Supports mapping either a `single code` at a time, or an `iterable of codes` (range, list, np.array, pd.Series, etc...).
-
-
-> :warning: When ICD9 or ICD10 is mentioned, it always refers to the American version aka ICD9-CM / ICD10-CM.
-
 # Installation
 
 `pip install icd-mappings`
 
 # Usage
 
 ```python
@@ -61,14 +47,29 @@
 >>> ['F0280', 'R111000', None, 'H269']
 
 # You can also check available mappers
 mapper.show_mappers()
 >>> ['icd9toccs', 'icd9toicd10', 'icd10toicd9', 'icd9tochapter', 'icd9tolevel3', 'icd9tocci']
 ```
 
+# Mappers
+
+List of all mappers:
+- [ICD9<->ICD10](https://www.nber.org/research/data/icd-9-cm-and-icd-10-cm-and-icd-10-pcs-crosswalk-or-general-equivalence-mappings): ICD9-CM and ICD10-CM (in both directions).
+- [ICD9->CCS](): ICD9-CM to CCS (Clinical Classification Software) codes;
+- [ICD9->ICD9Chapters](https://icd.codes/icd9cm): ICD9-CM diagnostic codes to the 19 Chapters;
+- [ICD9->CCI](https://www.hcup-us.ahrq.gov/toolssoftware/chronic/chronic.jsp) ICD9-CM diagnostics to CCI (Chronic Condition Indicator). True of False depending on whether a diagnostic is chronic or not;
+- ICD9->Level3: Gets the 3rd level of an ICD9-CM diagnostic code;
+
+
+Supports mapping either a `single code` at a time, or an `iterable of codes` (range, list, np.array, pd.Series, etc...).
+
+
+> :warning: When ICD9 or ICD10 is mentioned, it always refers to the American version aka ICD9-CM / ICD10-CM.
+
 # Feature requests
 
 Feel free to sugest feature requests under `Issues`, such as turning this into a script in case your pipeline does not use python.
 
 
 # Acknowledgments
```

