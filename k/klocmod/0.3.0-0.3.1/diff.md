# Comparing `tmp/klocmod-0.3.0.tar.gz` & `tmp/klocmod-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klocmod-0.3.0.tar", max compression
+gzip compressed data, was "klocmod-0.3.1.tar", max compression
```

## Comparing `klocmod-0.3.0.tar` & `klocmod-0.3.1.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1054 2023-02-12 20:05:26.759907 klocmod-0.3.0/LICENSE
--rw-r--r--   0        0        0     2597 2023-02-12 20:05:26.759907 klocmod-0.3.0/README.md
--rw-r--r--   0        0        0    13019 2023-02-12 20:05:55.040197 klocmod-0.3.0/klocmod/__init__.py
--rw-r--r--   0        0        0     1063 2023-02-12 20:05:26.759907 klocmod-0.3.0/klocmod/internals.py
--rw-r--r--   0        0        0     1405 2023-02-12 20:05:55.040197 klocmod-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3418 1970-01-01 00:00:00.000000 klocmod-0.3.0/setup.py
--rw-r--r--   0        0        0     3804 1970-01-01 00:00:00.000000 klocmod-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1054 2023-05-02 07:29:04.712121 klocmod-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2597 2023-05-02 07:29:04.712121 klocmod-0.3.1/README.md
+-rw-r--r--   0        0        0    13356 2023-05-02 07:29:23.520138 klocmod-0.3.1/klocmod/__init__.py
+-rw-r--r--   0        0        0     1063 2023-05-02 07:29:04.712121 klocmod-0.3.1/klocmod/internals.py
+-rw-r--r--   0        0        0     1405 2023-05-02 07:29:23.520138 klocmod-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3804 1970-01-01 00:00:00.000000 klocmod-0.3.1/PKG-INFO
```

### Comparing `klocmod-0.3.0/LICENSE` & `klocmod-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `klocmod-0.3.0/README.md` & `klocmod-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `klocmod-0.3.0/klocmod/__init__.py` & `klocmod-0.3.1/klocmod/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 import json
 import configparser
 from typing import *
 from pathlib import PurePath, Path
 
 from .internals import swap_keys, check_missing_non_regional_languages
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 __all__ = ['LanguageDictionary', 'SpecificLanguageDictionary', 'LocalizationsContainer', 'InvalidLocalizationFileError']
 _logger = logging.getLogger(__name__)
 
 
 class LanguageDictionary:
     """
     The base class for dict-like objects containing phrases for a particular language. Usually used as a fallback since
@@ -157,14 +157,17 @@
         return self._name
 
     def __eq__(self, other) -> bool:
         if not isinstance(other, LanguageDictionary):
             raise TypeError("Incomparable types!")
         return self._name == other._name
 
+    def __hash__(self) -> int:
+        return hash(self.name)
+
 
 class SpecificLanguageDictionary(LanguageDictionary):
     """
     A concrete implementation of :py:class:`LanguageDictionary` that consists of two dicts: one of them is considered as
     primary one and the other as spare. When you're trying to get some localized phrase by a key, the primary dict is
     used for searching first. If there is no such a key there, the search continues in the spare dict. Finally, if there
     is no such a phrase, the key itself is returned by the base class.
@@ -197,15 +200,20 @@
             return super()[item]
 
     def __eq__(self, other) -> bool:
         if not isinstance(other, LanguageDictionary):
             raise TypeError("Incomparable types!")
         if not isinstance(other, SpecificLanguageDictionary):
             return False
-        return self._primary_dict == other._primary_dict and self._spare_lang_dict == other._spare_lang_dict
+        return super().__eq__(other) \
+            and self._primary_dict == other._primary_dict \
+            and self._spare_lang_dict == other._spare_lang_dict
+
+    def __hash__(self) -> int:
+        return hash((self.name, tuple(sorted(self._primary_dict.items())), self._spare_lang_dict))
 
 
 class LocalizationsContainer:
     """
     A factory of :py:class:`LanguageDictionary` instances. Call the :py:meth:`LocalizationContainer.from_file` static
     method to get the instance of the container. Then you can use the :py:meth:`LocalizationContainer.get_lang` method
     to create instances of specific languages (:py:class:`LanguageDictionary`).
@@ -319,14 +327,17 @@
         return self.get_lang(lang_tag)
 
     def __eq__(self, other) -> bool:
         if not isinstance(other, LocalizationsContainer):
             raise TypeError("Incomparable types!")
         return self._primary_dict == other._primary_dict and self._spare_lang_dct == other._spare_lang_dct
 
+    def __iter__(self) -> Iterable:
+        return iter(self._primary_dict.items())
+    
 
 class InvalidLocalizationFileError(Exception):
     """
     An exception that is thrown when any error occurred while parsing some localization file.
 
     :param message: a human-readable message describing the error
     :param file_path: a path to the localization file
```

### Comparing `klocmod-0.3.0/klocmod/internals.py` & `klocmod-0.3.1/klocmod/internals.py`

 * *Files identical despite different names*

### Comparing `klocmod-0.3.0/pyproject.toml` & `klocmod-0.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "klocmod"
-version = "0.3.0"
+version = "0.3.1"
 description = "A simple module providing facilities to localize small programs via textual files."
 authors = ["Leonid Kozarin <kozalo@sadbot.ru>"]
 license = "MIT"
 readme = "README.md"
 include = ["LICENSE", "README.md"]
 homepage = "https://kozalo.ru/#post-1541257200"
 repository = "https://github.com/kozalosev/klocmod"
```

### Comparing `klocmod-0.3.0/PKG-INFO` & `klocmod-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klocmod
-Version: 0.3.0
+Version: 0.3.1
 Summary: A simple module providing facilities to localize small programs via textual files.
 Home-page: https://kozalo.ru/#post-1541257200
 License: MIT
 Keywords: localization library
 Author: Leonid Kozarin
 Author-email: kozalo@sadbot.ru
 Requires-Python: >=3.8,<4.0
```

