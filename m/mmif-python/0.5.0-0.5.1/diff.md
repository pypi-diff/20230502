# Comparing `tmp/mmif-python-0.5.0.tar.gz` & `tmp/mmif-python-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmif-python-0.5.0.tar", last modified: Sun Apr 30 04:04:27 2023, max compression
+gzip compressed data, was "mmif-python-0.5.1.tar", last modified: Tue May  2 02:25:15 2023, max compression
```

## Comparing `mmif-python-0.5.0.tar` & `mmif-python-0.5.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 04:04:27.509018 mmif-python-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-04-30 04:03:52.000000 mmif-python-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-30 04:03:52.000000 mmif-python-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-30 04:04:27.509018 mmif-python-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-30 04:03:52.000000 mmif-python-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 04:03:53.000000 mmif-python-0.5.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 04:04:27.505018 mmif-python-0.5.0/mmif/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-30 04:03:52.000000 mmif-python-0.5.0/mmif/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 04:04:27.505018 mmif-python-0.5.0/mmif/res/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 04:04:27.000000 mmif-python-0.5.0/mmif/res/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-04-30 04:04:27.000000 mmif-python-0.5.0/mmif/res/clams.vocabulary.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-30 04:04:27.000000 mmif-python-0.5.0/mmif/res/do-not-edit.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-04-30 04:04:27.000000 mmif-python-0.5.0/mmif/res/mmif.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 04:04:27.509018 mmif-python-0.5.0/mmif/serialize/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-30 04:03:52.000000 mmif-python-0.5.0/mmif/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14052 2023-04-30 04:03:52.000000 mmif-python-0.5.0/mmif/serialize/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19125 2023-04-30 04:03:52.000000 mmif-python-0.5.0/mmif/serialize/mmif.py
--rw-r--r--   0 runner    (1001) docker     (123)    18396 2023-04-30 04:03:52.000000 mmif-python-0.5.0/mmif/serialize/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-04-30 04:03:52.000000 mmif-python-0.5.0/mmif/serialize/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 04:04:27.509018 mmif-python-0.5.0/mmif/ver/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-30 04:04:27.000000 mmif-python-0.5.0/mmif/ver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-30 04:04:27.000000 mmif-python-0.5.0/mmif/ver/do-not-edit.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 04:04:27.509018 mmif-python-0.5.0/mmif/vocabulary/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-30 04:04:27.000000 mmif-python-0.5.0/mmif/vocabulary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-30 04:04:27.000000 mmif-python-0.5.0/mmif/vocabulary/annotation_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-04-30 04:04:27.000000 mmif-python-0.5.0/mmif/vocabulary/base_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-30 04:04:27.000000 mmif-python-0.5.0/mmif/vocabulary/do-not-edit.txt
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-30 04:04:27.000000 mmif-python-0.5.0/mmif/vocabulary/document_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 04:04:27.509018 mmif-python-0.5.0/mmif_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-30 04:04:27.000000 mmif-python-0.5.0/mmif_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-30 04:04:27.000000 mmif-python-0.5.0/mmif_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 04:04:27.000000 mmif-python-0.5.0/mmif_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-30 04:04:27.000000 mmif-python-0.5.0/mmif_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-30 04:04:27.000000 mmif-python-0.5.0/mmif_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-30 04:03:52.000000 mmif-python-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 04:04:27.509018 mmif-python-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-04-30 04:03:52.000000 mmif-python-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 02:25:15.922579 mmif-python-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-05-02 02:24:47.000000 mmif-python-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-02 02:24:47.000000 mmif-python-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-02 02:25:15.922579 mmif-python-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-02 02:24:47.000000 mmif-python-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 02:24:47.000000 mmif-python-0.5.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 02:25:15.918579 mmif-python-0.5.1/mmif/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-02 02:24:47.000000 mmif-python-0.5.1/mmif/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 02:25:15.922579 mmif-python-0.5.1/mmif/res/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 02:25:15.000000 mmif-python-0.5.1/mmif/res/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-05-02 02:25:15.000000 mmif-python-0.5.1/mmif/res/clams.vocabulary.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-02 02:25:15.000000 mmif-python-0.5.1/mmif/res/do-not-edit.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-05-02 02:25:15.000000 mmif-python-0.5.1/mmif/res/mmif.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 02:25:15.922579 mmif-python-0.5.1/mmif/serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-02 02:24:47.000000 mmif-python-0.5.1/mmif/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14052 2023-05-02 02:24:47.000000 mmif-python-0.5.1/mmif/serialize/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20102 2023-05-02 02:24:47.000000 mmif-python-0.5.1/mmif/serialize/mmif.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18396 2023-05-02 02:24:47.000000 mmif-python-0.5.1/mmif/serialize/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16014 2023-05-02 02:24:47.000000 mmif-python-0.5.1/mmif/serialize/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 02:25:15.922579 mmif-python-0.5.1/mmif/ver/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-02 02:25:15.000000 mmif-python-0.5.1/mmif/ver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-02 02:25:15.000000 mmif-python-0.5.1/mmif/ver/do-not-edit.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 02:25:15.922579 mmif-python-0.5.1/mmif/vocabulary/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-02 02:25:15.000000 mmif-python-0.5.1/mmif/vocabulary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-02 02:25:15.000000 mmif-python-0.5.1/mmif/vocabulary/annotation_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-05-02 02:25:15.000000 mmif-python-0.5.1/mmif/vocabulary/base_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-02 02:25:15.000000 mmif-python-0.5.1/mmif/vocabulary/do-not-edit.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-02 02:25:15.000000 mmif-python-0.5.1/mmif/vocabulary/document_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 02:25:15.922579 mmif-python-0.5.1/mmif_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-02 02:25:15.000000 mmif-python-0.5.1/mmif_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-02 02:25:15.000000 mmif-python-0.5.1/mmif_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 02:25:15.000000 mmif-python-0.5.1/mmif_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-02 02:25:15.000000 mmif-python-0.5.1/mmif_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-02 02:25:15.000000 mmif-python-0.5.1/mmif_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-02 02:24:47.000000 mmif-python-0.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 02:25:15.922579 mmif-python-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    12299 2023-05-02 02:24:47.000000 mmif-python-0.5.1/setup.py
```

### Comparing `mmif-python-0.5.0/LICENSE` & `mmif-python-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mmif-python-0.5.0/PKG-INFO` & `mmif-python-0.5.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmif-python
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python implementation of MultiMedia Interchange Format specification. (https://mmif.clams.ai)
 Home-page: https://mmif.clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 License: UNKNOWN
 Description: # MMIF for python
```

### Comparing `mmif-python-0.5.0/README.md` & `mmif-python-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `mmif-python-0.5.0/mmif/res/clams.vocabulary.yaml` & `mmif-python-0.5.1/mmif/res/clams.vocabulary.yaml`

 * *Files identical despite different names*

### Comparing `mmif-python-0.5.0/mmif/res/mmif.json` & `mmif-python-0.5.1/mmif/res/mmif.json`

 * *Files identical despite different names*

### Comparing `mmif-python-0.5.0/mmif/serialize/annotation.py` & `mmif-python-0.5.1/mmif/serialize/annotation.py`

 * *Files identical despite different names*

### Comparing `mmif-python-0.5.0/mmif/serialize/mmif.py` & `mmif-python-0.5.1/mmif/serialize/mmif.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,14 +64,39 @@
         if isinstance(json_str, bytes):
             json_str = json_str.decode('utf8')
         schema = json.loads(mmif.get_mmif_json_schema())
         if isinstance(json_str, str):
             json_str = json.loads(json_str)
         jsonschema.validators.validate(json_str, schema)
 
+    def serialize(self, pretty: bool = False, sanitize: bool = False) -> str:
+        if sanitize:
+            self.sanitize()
+        return super().serialize(pretty)
+
+    def sanitize(self):
+        """
+        Sanitizes a Mmif object by running some safeguards.
+        Concretely, it performs the following before returning the JSON string.
+        
+        #. validating output using built-in MMIF jsonschema
+        #. remove non-existing annotation types from ``contains`` metadata
+    
+        """
+        for view in self.views:
+            existing_at_types = set(annotation.at_type for annotation in view.annotations)
+            to_pop = set()
+            for contains_at_type in view.metadata.contains.keys():
+                if contains_at_type not in existing_at_types:
+                    to_pop.add(contains_at_type)
+            for key in to_pop:
+                view.metadata.contains.pop(key)
+        serialized = self.serialize()
+        self.validate(serialized)
+
     def new_view_id(self) -> str:
         """
         Fetches an ID for a new view.
 
         :return: the ID
         """
         index = len(self.views)
@@ -237,22 +262,22 @@
     def get_alignments(self, at_type1: Union[str, ThingTypesBase], at_type2: Union[str, ThingTypesBase]) -> Dict[str, List[Annotation]]:
         """
         Finds views where alignments between two given annotation types occurred.
 
         :return: a dict that keyed by view IDs (str) and has lists of alignment Annotation objects as values.
         """
         v_and_a = {}
-        at_type1 = ThingTypesBase.from_str(at_type1) if isinstance(at_type1, str) else at_type1
-        at_type2 = ThingTypesBase.from_str(at_type2) if isinstance(at_type2, str) else at_type2
+        at_type1, at_type2 = [ThingTypesBase.from_str(x) if isinstance(x, str) else x for x in (at_type1, at_type2)]
         assert at_type1 != at_type2, f"Alignment must be between two different types, given only one: {at_type1}"
         for alignment_view in self.get_all_views_contain(AnnotationTypes.Alignment):
             alignments = []
             contains_meta = alignment_view.metadata.contains[AnnotationTypes.Alignment]
             if 'sourceType' in contains_meta and 'targetType' in contains_meta:
-                aligned_types = list({contains_meta['sourceType'], contains_meta['targetType']})
+                aligned_types = [ThingTypesBase.from_str(x) 
+                                 for x in {contains_meta['sourceType'], contains_meta['targetType']}]
                 if len(aligned_types) == 2 and at_type1 in aligned_types and at_type2 in aligned_types:
                     alignments.extend(alignment_view.annotations)
             else:
                 for alignment in alignment_view.get_annotations(AnnotationTypes.Alignment):
                     aligned_types = set()
                     for ann_id in [alignment.properties['target'], alignment.properties['source']]:
                         ann_id = cast(str, ann_id)
```

### Comparing `mmif-python-0.5.0/mmif/serialize/model.py` & `mmif-python-0.5.1/mmif/serialize/model.py`

 * *Files identical despite different names*

### Comparing `mmif-python-0.5.0/mmif/serialize/view.py` & `mmif-python-0.5.1/mmif/serialize/view.py`

 * *Files 4% similar despite different names*

```diff
@@ -242,20 +242,29 @@
         self.error: Union[dict, ErrorDict] = {}
         self.warnings: List[str] = []
         self._required_attributes = ["app"]
         self._attribute_classes = {
             'error': ErrorDict,
             'contains': ContainsDict
         }
-        # in theory, either `contains` or `error` should appear in a `view`
+        # in theory, *oneOf* `contains`, `error`, or `warnings` should appear in a `view`
         # but with current implementation, there's no easy way to set a condition 
         # for `oneOf` requirement 
         # see MmifObject::_required_attributes in model.py 
+        # also see this class' `_serialize()` override implementation
         super().__init__(viewmetadata_obj)
 
+    def _serialize(self, alt_container: Optional[Dict] = None) -> dict:
+        serialized = super()._serialize()
+        # `_serialize()` eliminates any *empty* attributes, so 
+        # when no "contains", "errors", nor "warnings", at least add an empty contains back
+        if not (self.contains.items() or self.error or self.warnings):
+            serialized['contains'] = {}
+        return serialized
+
     def new_contain(self, at_type: Union[str, ThingTypesBase], **contains_metadata) -> Optional['Contain']:
         """
         Adds a new element to the ``contains`` dictionary.
 
         :param at_type: the ``@type`` of the annotation type being added
         :param contains_metadata: any metadata associated with the annotation type
         :return: the generated :class:`Contain` object
@@ -360,8 +369,11 @@
             
     def get(self, key: Union[str, ThingTypesBase], default=None):
         if isinstance(key, str):
             key = ThingTypesBase.from_str(key)
         return self._items.get(key, default)
     
     def __contains__(self, item: Union[str, ThingTypesBase]):
-        return item in list(self._items.keys())
+        return item in self._items
+
+    def pop(self, key):
+        self._items.pop(key)
```

### Comparing `mmif-python-0.5.0/mmif/vocabulary/annotation_types.py` & `mmif-python-0.5.1/mmif/vocabulary/annotation_types.py`

 * *Files identical despite different names*

### Comparing `mmif-python-0.5.0/mmif/vocabulary/base_types.py` & `mmif-python-0.5.1/mmif/vocabulary/base_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 # This file is auto-generated by setup.py
+import warnings
 from typing import ClassVar
 
+
 class TypesBase(object):
     """
     Base class for arbitrary vocabulary type. 
     This class provides bisic initializer, comparators, 
     and (de-)serialization methods. 
     """
     _prefixes = {}
     base_uri: str
     shortname: str
-    
+    fuzzy_eq: bool
+
     def __init__(self, type_uri: str):
+        self.fuzzy_eq = False
         self.parse_names(type_uri)
         if self.__repr__() not in self.__class__._prefixes:
             # prepare auto-inferred prefix for Annotations.[].id field
             self.__class__._prefixes[self.__repr__()] \
                 = self.__class__._create_prefix(self.shortname,
                                                 self.__class__._prefixes.values()
                                                 )
@@ -105,14 +109,18 @@
     Base class for CLAMS vocabulary types. Main 
     This class adds handling of MMIF specification versions 
     in initializer and comparators. 
     """
     version: str
     dev_version: ClassVar[str] = 'develop'
     
+    def __init__(self, type_uri, fuzzymode=True):
+        super().__init__(type_uri)
+        self.fuzzy_eq = fuzzymode
+    
     def parse_names(self, type_uri:str):
         if not type_uri:
             self.base_uri, self.shortname, self.version = "", "", ""
         elif 'mmif.clams.ai' not in type_uri:
             raise ValueError(f'Cannot process "{type_uri}"!: not a CLAMS vocabulary URI')
         elif type_uri[-1].isdigit():  # new versioning
             self.base_uri, _, self.shortname, self.version = type_uri.rsplit('/', 3)
@@ -126,35 +134,46 @@
                              f'longer supported with this app.')
         if legacy_ver > '0.4.2':
             raise ValueError(f'Cannot process "{self}"!: Invalid CLAMS vocabulary type URI.')
         return True
 
     def __hash__(self):
         return hash(str(self))
+    
+    def normalize_attype_vers(self):
+        if '.' in self.version and self._check_legacy_version(self.version):
+            # legacy mapping: see https://github.com/clamsproject/mmif/issues/14#issuecomment-1504439497
+            if self.version == '0.4.2' and self.shortname == 'Annotation':
+                return 'v2'
+            elif self.version.startswith('0.4.'):
+                return 'v1'
+        else:
+            return self.version
 
-    def __eq__(self, other):
-        if isinstance(other, str):
-            other = ThingTypesBase.from_str(other)
+    def _eq_internal(self, other, fuzzy):
         if isinstance(other, ClamsTypesBase):
-            vers = []
-            for o in (self, other):
-                if '.' in o.version and self._check_legacy_version(o.version):
-                    # legacy mapping: see https://github.com/clamsproject/mmif/issues/14#issuecomment-1504439497
-                    if o.version == '0.4.2' and o.shortname == 'Annotation':
-                        vers.append('v2')
-                    elif o.version.startswith('0.4.'):
-                        vers.append('v1')
-                else:
-                    vers.append(o.version)
-            return self.base_uri == other.base_uri \
-                and self.shortname == other.shortname \
-                and vers[0] == vers[1]
+            if fuzzy:
+                vers = [x.normalize_attype_vers() for x in (self, other)]
+                if self.base_uri == other.base_uri and self.shortname == other.shortname:
+                    if vers[0] != vers[1]:
+                        warnings.warn(f'version difference detected: {self.version}&{other.version}@{self.shortname}')
+                    return True
+                return False
+            else:
+                return self.base_uri == other.base_uri \
+                    and self.shortname == other.shortname \
+                    and self.version == other.version
         else:
             return False
     
+    def __eq__(self, other):
+        if isinstance(other, str):
+            other = ThingTypesBase.from_str(other)
+        return self._eq_internal(other, self.fuzzy_eq and other.fuzzy_eq)
+    
     def __repr__(self):
         if self.version[0] == 'v':
             return f'{self.base_uri}/vocabulary/{self.shortname}/{self.version}'
         else:
             return f'{self.base_uri}/{self.version}/vocabulary/{self.shortname}'
```

### Comparing `mmif-python-0.5.0/mmif/vocabulary/document_types.py` & `mmif-python-0.5.1/mmif/vocabulary/document_types.py`

 * *Files identical despite different names*

### Comparing `mmif-python-0.5.0/mmif_python.egg-info/PKG-INFO` & `mmif-python-0.5.1/mmif_python.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmif-python
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python implementation of MultiMedia Interchange Format specification. (https://mmif.clams.ai)
 Home-page: https://mmif.clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 License: UNKNOWN
 Description: # MMIF for python
```

### Comparing `mmif-python-0.5.0/mmif_python.egg-info/SOURCES.txt` & `mmif-python-0.5.1/mmif_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mmif-python-0.5.0/setup.py` & `mmif-python-0.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,15 @@
     }
     vocabulary_dir = generate_subpack(
         mmif_name, mmif_vocabulary_pkg,
         '\n'.join(
             f"from .{mod_name} import {class_name}"
             for mod_name, classes in types.items()
             for class_name in classes
-        )+'\n'
+        ) + '\n\n' + "typevers = {**ThingType.typevers, **AnnotationTypes.typevers, **DocumentTypes.typevers}" + '\n'
     )
     document_types = []
     annotation_types = []
     base_types = []
     
     for n, v in clams_types_vers.items():
         if n == 'Thing':
@@ -157,15 +157,15 @@
     for mod_name, type_ver_list in type_lists.items():
         enum_contents = generate_vocab_enum(spec_version, type_ver_list, mod_name)
         write_res_file(vocabulary_dir, mod_name+'.py', enum_contents)
 
     return vocabulary_dir
 
 
-def get_latest_mmif_gittag(version: str):
+def get_latest_mmif_gittag():
     # vmaj, vmin, vpat = version.split('.')[0:3]
     res = request.urlopen('https://api.github.com/repos/clamsproject/mmif/git/refs/tags')
     body = json.loads(res.read())
     tags = [os.path.basename(tag['ref']) for tag in body]
     # sort and return highest version
     mmif_ver_format = lambda x: re.match(r'\d+\.\d+\.\d$', x)
     return sorted([tag for tag in tags if mmif_ver_format(tag)])[-1]
@@ -196,15 +196,15 @@
 
 def prep_ext_files(setuptools_cmd):
     ori_run = setuptools_cmd.run
 
     def mod_run(self):
         # will infer the `spec_ver` from the latest git tag available either on GH or local `mmif` repository.
         # NOTE that when `make develop`, it will use specification files from upstream "develop" branch of `mmif` repo
-        latest_mmif_gittag = get_latest_mmif_gittag(version)
+        latest_mmif_gittag = get_latest_mmif_gittag()
         spec_file_gitref = latest_mmif_gittag if '.dev' not in version else 'develop'
         # legacy version tags were formatted as xx-a.b.c (e.g., vocab-0.0.1)
         spec_version = latest_mmif_gittag.split('-')[-1]
         # making resources into a python package so that `pkg_resources` can access resource files
         res_dir = generate_subpack(mmif_name, mmif_res_pkg)
 
         # the following will generate a new version value based on VERSION file
```

