# Comparing `tmp/voprov-0.0.2.tar.gz` & `tmp/voprov-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/voprov-0.0.2.tar", last modified: Mon Oct 26 15:36:13 2020, max compression
+gzip compressed data, was "voprov-0.0.3.tar", last modified: Tue May  2 09:41:57 2023, max compression
```

## Comparing `voprov-0.0.2.tar` & `voprov-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 15:36:13.862513 voprov-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (116)     2081 2020-10-26 15:36:13.862513 voprov-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      720 2020-10-26 15:36:04.000000 voprov-0.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-10-26 15:36:13.862513 voprov-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1855 2020-10-26 15:36:04.000000 voprov-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 15:36:13.862513 voprov-0.0.2/voprov/
--rw-r--r--   0 runner    (1001) docker     (116)     1524 2020-10-26 15:36:04.000000 voprov-0.0.2/voprov/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 15:36:13.862513 voprov-0.0.2/voprov/models/
--rw-r--r--   0 runner    (1001) docker     (116)      235 2020-10-26 15:36:04.000000 voprov-0.0.2/voprov/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    13035 2020-10-26 15:36:04.000000 voprov-0.0.2/voprov/models/constants.py
--rw-r--r--   0 runner    (1001) docker     (116)   104891 2020-10-26 15:36:04.000000 voprov-0.0.2/voprov/models/model.py
--rw-r--r--   0 runner    (1001) docker     (116)      996 2020-10-26 15:36:04.000000 voprov-0.0.2/voprov/models/voprovConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (116)    13752 2020-10-26 15:36:04.000000 voprov-0.0.2/voprov/models/voprovDescriptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     1795 2020-10-26 15:36:04.000000 voprov-0.0.2/voprov/models/voprovRelations.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 15:36:13.862513 voprov-0.0.2/voprov/serializers/
--rw-r--r--   0 runner    (1001) docker     (116)     1631 2020-10-26 15:36:04.000000 voprov-0.0.2/voprov/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      821 2020-10-26 15:36:04.000000 voprov-0.0.2/voprov/serializers/provn.py
--rw-r--r--   0 runner    (1001) docker     (116)    10303 2020-10-26 15:36:04.000000 voprov-0.0.2/voprov/serializers/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 15:36:13.862513 voprov-0.0.2/voprov/visualization/
--rw-r--r--   0 runner    (1001) docker     (116)      214 2020-10-26 15:36:04.000000 voprov-0.0.2/voprov/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6664 2020-10-26 15:36:04.000000 voprov-0.0.2/voprov/visualization/dot.py
--rw-r--r--   0 runner    (1001) docker     (116)     1263 2020-10-26 15:36:04.000000 voprov-0.0.2/voprov/visualization/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-26 15:36:13.862513 voprov-0.0.2/voprov.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2081 2020-10-26 15:36:13.000000 voprov-0.0.2/voprov.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      575 2020-10-26 15:36:13.000000 voprov-0.0.2/voprov.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-26 15:36:13.000000 voprov-0.0.2/voprov.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-26 15:36:13.000000 voprov-0.0.2/voprov.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       32 2020-10-26 15:36:13.000000 voprov-0.0.2/voprov.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2020-10-26 15:36:13.000000 voprov-0.0.2/voprov.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:41:57.992111 voprov-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-02 09:41:42.000000 voprov-0.0.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-02 09:41:42.000000 voprov-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-02 09:41:57.992111 voprov-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-02 09:41:42.000000 voprov-0.0.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 09:41:57.996111 voprov-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-02 09:41:42.000000 voprov-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:41:57.992111 voprov-0.0.3/voprov/
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-02 09:41:42.000000 voprov-0.0.3/voprov/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:41:57.992111 voprov-0.0.3/voprov/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-02 09:41:42.000000 voprov-0.0.3/voprov/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-05-02 09:41:42.000000 voprov-0.0.3/voprov/models/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105183 2023-05-02 09:41:42.000000 voprov-0.0.3/voprov/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-02 09:41:42.000000 voprov-0.0.3/voprov/models/voprovConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13687 2023-05-02 09:41:42.000000 voprov-0.0.3/voprov/models/voprovDescriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-02 09:41:42.000000 voprov-0.0.3/voprov/models/voprovRelations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:41:57.992111 voprov-0.0.3/voprov/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-02 09:41:42.000000 voprov-0.0.3/voprov/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11514 2023-05-02 09:41:42.000000 voprov-0.0.3/voprov/serializers/provjson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-02 09:41:42.000000 voprov-0.0.3/voprov/serializers/provn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9987 2023-05-02 09:41:42.000000 voprov-0.0.3/voprov/serializers/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:41:57.992111 voprov-0.0.3/voprov/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-02 09:41:42.000000 voprov-0.0.3/voprov/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-05-02 09:41:42.000000 voprov-0.0.3/voprov/visualization/dot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-02 09:41:42.000000 voprov-0.0.3/voprov/visualization/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:41:57.992111 voprov-0.0.3/voprov.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-02 09:41:57.000000 voprov-0.0.3/voprov.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-02 09:41:57.000000 voprov-0.0.3/voprov.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 09:41:57.000000 voprov-0.0.3/voprov.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 09:41:57.000000 voprov-0.0.3/voprov.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-02 09:41:57.000000 voprov-0.0.3/voprov.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 09:41:57.000000 voprov-0.0.3/voprov.egg-info/top_level.txt
```

### Comparing `voprov-0.0.2/README.rst` & `voprov-0.0.3/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Introduction
 ============
 
 A library for IVOA Provenance Data Model supporting PROV-N, PROV-XML, PROV-JSON export
 
-* Free software: MIT license
+* Free software: MIT license (https://opensource.org/licenses/MIT)
 * Documentation: (incoming).
 
 Features
 --------
 
 * An implementation of the `IVOA Provenance Data Model <http://www.ivoa.net/documents/ProvenanceDM/>`_ in Python.
 * Serialization support: `PROV-N <http://www.w3.org/TR/prov-n/>`_, `PROV-XML <http://www.w3.org/TR/prov-xml/>`_ and `PROV-JSON <http://www.w3.org/Submission/prov-json/>`_.
 * Exporting VOPROV documents into various graphical formats (e.g. PDF, PNG, SVG).
 * Convert a VOPROV document to a `Prov Document <https://github.com/trungdong/prov>`_.
 
 
 Uses
 ----
 
-A short tutorial for using this package is in development.
+A short tutorial for using this package is available here:
+
+https://github.com/mservillat/voprov/blob/master/tutorials/voprov_tutorial.ipynb
```

### Comparing `voprov-0.0.2/setup.py` & `voprov-0.0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     readme = f.read()
 
 requirements = [
-    'prov>=1.5.3',
+    'prov>=2.0',
 ]
 
 test_requirements = [
     'pydot>=1.2.0'
 ]
 
 setup(
     name='voprov',
-    version='0.0.2',
+    version='0.0.3',
     description='A library for IVOA Provenance Data Model supporting PROV-JSON, '
                 'PROV-XML and PROV-N',
     long_description=readme,
-    author='Jean-Francois Sornay',
-    author_email='jeanfrancois.sornay@gmail.com',
+    author='Benjamin Parciany',
+    author_email='benjamin.parciany@obspm.fr',
     url='https://github.com/sanguillon/voprov/',
     packages=find_packages(),
     include_package_data=True,
     install_requires=requirements,
     extras_require={
         'dot': ['pydot>=1.2.0'],
     },
@@ -43,19 +43,18 @@
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Intended Audience :: Information Technology',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: French',
         'Operating System :: OS Independent',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Scientific/Engineering :: Information Analysis',
     ],
     tests_require=test_requirements,
-    python_requires='>=2',
+    python_requires='>=3',
 )
```

### Comparing `voprov-0.0.2/voprov/__init__.py` & `voprov-0.0.3/voprov/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # -*- coding: utf-8 -*-
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
 from prov import Error
 
 __author__ = 'Jean-Francois Sornay'
 __email__ = 'jeanfrancois.sornay@gmail.com'
 
 __all__ = ["Error", "models", "read"]
```

### Comparing `voprov-0.0.2/voprov/models/constants.py` & `voprov-0.0.3/voprov/models/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 # -*- coding: utf-8 -*-
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-
 from prov.constants import *
 from prov.model import Literal
 
 __author__ = 'Jean-Francois Sornay'
 __email__ = 'jeanfrancois.sornay@gmail.com'
 
 
@@ -168,46 +165,46 @@
     VOPROV_CONFIGURATION_RELATION:      VOPROV_CONFIGURATION_RELATION,
     VOPROV_REFERENCE_RELATION:          VOPROV_REFERENCE_RELATION,
 })
 
 
 # Part 3 : Identifier for voprov's attributes
 #   Adaptation of identifiers for PROV's attributes
-VOPROV_ATTR_ENTITY =                    VOPROV['entity']
-VOPROV_ATTR_ACTIVITY =                  VOPROV['activity']
-VOPROV_ATTR_TRIGGER =                   VOPROV['trigger']
-VOPROV_ATTR_INFORMED =                  VOPROV['informed']
-VOPROV_ATTR_INFORMANT =                 VOPROV['informant']
-VOPROV_ATTR_STARTER =                   VOPROV['starter']
-VOPROV_ATTR_ENDER =                     VOPROV['ender']
-VOPROV_ATTR_AGENT =                     VOPROV['agent']
-VOPROV_ATTR_PLAN =                      VOPROV['plan']
-VOPROV_ATTR_DELEGATE =                  VOPROV['delegate']
-VOPROV_ATTR_RESPONSIBLE =               VOPROV['responsible']
-VOPROV_ATTR_GENERATED_ENTITY =          VOPROV['generatedEntity']
-VOPROV_ATTR_USED_ENTITY =               VOPROV['usedEntity']
-VOPROV_ATTR_GENERATION =                VOPROV['generation']
-VOPROV_ATTR_USAGE =                     VOPROV['usage']
-VOPROV_ATTR_SPECIFIC_ENTITY =           VOPROV['specificEntity']
-VOPROV_ATTR_GENERAL_ENTITY =            VOPROV['generalEntity']
-VOPROV_ATTR_ALTERNATE1 =                VOPROV['alternate1']
-VOPROV_ATTR_ALTERNATE2 =                VOPROV['alternate2']
-VOPROV_ATTR_BUNDLE =                    VOPROV['bundle']
-VOPROV_ATTR_INFLUENCEE =                VOPROV['influencee']
-VOPROV_ATTR_INFLUENCER =                VOPROV['influencer']
-VOPROV_ATTR_COLLECTION =                VOPROV['collection']
+VOPROV_ATTR_ENTITY =                    PROV['entity']
+VOPROV_ATTR_ACTIVITY =                  PROV['activity']
+VOPROV_ATTR_TRIGGER =                   PROV['trigger']
+VOPROV_ATTR_INFORMED =                  PROV['informed']
+VOPROV_ATTR_INFORMANT =                 PROV['informant']
+VOPROV_ATTR_STARTER =                   PROV['starter']
+VOPROV_ATTR_ENDER =                     PROV['ender']
+VOPROV_ATTR_AGENT =                     PROV['agent']
+VOPROV_ATTR_PLAN =                      PROV['plan']
+VOPROV_ATTR_DELEGATE =                  PROV['delegate']
+VOPROV_ATTR_RESPONSIBLE =               PROV['responsible']
+VOPROV_ATTR_GENERATED_ENTITY =          PROV['generatedEntity']
+VOPROV_ATTR_USED_ENTITY =               PROV['usedEntity']
+VOPROV_ATTR_GENERATION =                PROV['generation']
+VOPROV_ATTR_USAGE =                     PROV['usage']
+VOPROV_ATTR_SPECIFIC_ENTITY =           PROV['specificEntity']
+VOPROV_ATTR_GENERAL_ENTITY =            PROV['generalEntity']
+VOPROV_ATTR_ALTERNATE1 =                PROV['alternate1']
+VOPROV_ATTR_ALTERNATE2 =                PROV['alternate2']
+VOPROV_ATTR_BUNDLE =                    PROV['bundle']
+VOPROV_ATTR_INFLUENCEE =                PROV['influencee']
+VOPROV_ATTR_INFLUENCER =                PROV['influencer']
+VOPROV_ATTR_COLLECTION =                PROV['collection']
 #   (some is used in description and configuration element, so in this case, they only appear in description part)
 #   voprov description
-VOPROV_ATTR_NAME =                      VOPROV['name']
-VOPROV_ATTR_ROLE =                      VOPROV['role']
+VOPROV_ATTR_NAME =                      PROV['name']
+VOPROV_ATTR_ROLE =                      PROV['role']
 VOPROV_ATTR_VALUE_TYPE =                VOPROV['valueType']
 VOPROV_ATTR_CONTENT_TYPE =              VOPROV['contentType']
 #   voprov configuration
-VOPROV_ATTR_LOCATION =                  VOPROV['location']
-VOPROV_ATTR_VALUE =                     VOPROV['value']
+VOPROV_ATTR_LOCATION =                  PROV['location']
+VOPROV_ATTR_VALUE =                     PROV['value']
 VOPROV_ATTR_ARTEFACT_TYPE =             VOPROV['artefactType']
 
 #   voprov relation
 VOPROV_ATTR_DESCRIBED =                 VOPROV['described']
 VOPROV_ATTR_DESCRIPTOR =                VOPROV['descriptor']
 VOPROV_ATTR_RELATED =                   VOPROV['related']
 VOPROV_ATTR_RELATOR =                   VOPROV['relator']
@@ -250,17 +247,17 @@
     VOPROV_ATTR_RELATOR,
     VOPROV_ATTR_CONFIGURED,
     VOPROV_ATTR_CONFIGURATOR,
     VOPROV_ATTR_REFERENCED,
     VOPROV_ATTR_REFERRER,
 })
 
-VOPROV_ATTR_TIME = VOPROV['time']
-VOPROV_ATTR_STARTTIME = VOPROV['startTime']
-VOPROV_ATTR_ENDTIME = VOPROV['endTime']
+VOPROV_ATTR_TIME = PROV['time']
+VOPROV_ATTR_STARTTIME = PROV['startTime']
+VOPROV_ATTR_ENDTIME = PROV['endTime']
 
 #   adding the voprov identifier for the literals attribute
 PROV_ATTRIBUTE_LITERALS.update({
     # update of prov literals to voprov literals
     VOPROV_ATTR_TIME,
     VOPROV_ATTR_STARTTIME,
     VOPROV_ATTR_ENDTIME,
@@ -273,15 +270,29 @@
 
     # voprov configuration
     Literal(VOPROV_ATTR_LOCATION),
     Literal(VOPROV_ATTR_VALUE),
     Literal(VOPROV_ATTR_ARTEFACT_TYPE),
 })
 
+# Set of formal attributes of PROV records
+PROV_ATTRIBUTES = PROV_ATTRIBUTE_QNAMES | PROV_ATTRIBUTE_LITERALS
+PROV_RECORD_ATTRIBUTES = list((attr, str(attr)) for attr in PROV_ATTRIBUTES)
+
+PROV_RECORD_IDS_MAP = dict(
+    (PROV_N_MAP[rec_type_id], rec_type_id) for rec_type_id in PROV_N_MAP
+)
+PROV_ID_ATTRIBUTES_MAP = dict(
+    (prov_id, attribute) for (prov_id, attribute) in PROV_RECORD_ATTRIBUTES
+)
+PROV_ATTRIBUTES_ID_MAP = dict(
+    (attribute, prov_id) for (prov_id, attribute) in PROV_RECORD_ATTRIBUTES
+)
+
 # Extra definition for convenience
-VOPROV_TYPE = VOPROV['type']
-VOPROV_LABEL = VOPROV['label']
-VOPROV_VALUE = VOPROV['value']
-VOPROV_LOCATION = VOPROV['location']
-VOPROV_ROLE = VOPROV['role']
+VOPROV_TYPE = PROV['type']
+VOPROV_LABEL = PROV['label']
+VOPROV_VALUE = PROV['value']
+VOPROV_LOCATION = PROV['location']
+VOPROV_ROLE = PROV['role']
 
-VOPROV_QUALIFIEDNAME = VOPROV['QUALIFIED_NAME']
+VOPROV_QUALIFIEDNAME = PROV['QUALIFIED_NAME']
```

### Comparing `voprov-0.0.2/voprov/models/model.py` & `voprov-0.0.3/voprov/models/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 # -*- coding: utf-8 -*-
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-
 import io
 import itertools
 import os
 import logging
 import shutil
 import tempfile
 import dateutil.parser
 from prov.model import (ProvException, ProvDocument, ProvBundle, ProvActivity,
                         ProvUsage, ProvAgent, ProvGeneration, ProvAssociation, ProvEntity,
                         ProvCommunication, ProvStart, ProvEnd, ProvInvalidation, ProvDerivation,
                         ProvAttribution, ProvDelegation, ProvInfluence, ProvSpecialization,
                         ProvAlternate, ProvMention, ProvMembership,
                         PROV_REC_CLS, DEFAULT_NAMESPACES, NamespaceManager, first)
-from six.moves.urllib.parse import urlparse
+from urllib.parse import urlparse
 
 from voprov import serializers
 from voprov.models.voprovDescriptions import *
 from voprov.models.voprovConfigurations import *
 from voprov.models.voprovRelations import *
 
 __author__ = 'Jean-Francois Sornay'
@@ -27,15 +24,15 @@
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_NAMESPACES.update({'voprov': VOPROV})
 
 
 def _ensure_datetime(value):
-    if isinstance(value, six.string_types):
+    if isinstance(value, str):
         return dateutil.parser.parse(value)
     else:
         return value
 
 
 class VOProvEntity(ProvEntity):
     """Adaptation of prov Entity to VOProv Entity"""
@@ -77,15 +74,14 @@
 
         :param comment:                 Text containing specific comments on the entity.
         """
         self._attributes[VOPROV['comment']] = {comment}
 
     def isDescribedBy(self, activityDescription, identifier=None):
         """Link an activity description to this activity
-
         :param activityDescription:     Identifier for the activity description link to this activity.
         :param identifier:              Identifier of the description relation created.
         """
         return self._bundle.description(self, activityDescription, identifier)
 
     def wasGeneratedBy(self, activity, time=None, attributes=None):
         """
@@ -368,14 +364,21 @@
             if value:
                 for super_formal in super(VOProvActivity, self).FORMAL_ATTRIBUTES:
                     if local_part is super_formal.localpart:
                         activity.add_attributes({super_formal: value})
                         break
         return bundle.add_record(activity)
 
+    def add_parameter(self, idbundle, idparam, nameparam, valueparam):
+        """add a parameter to an activity"""
+        if self._bundle.valid_qualified_name(idbundle) not in self._bundle._bundles:
+            bundle_config = self._bundle.bundle(idbundle)
+            param = bundle_config.parameter(idparam, nameparam, valueparam)
+            self._bundle.wasConfiguredBy(self, param)
+
 
 class VOProvAgent(ProvAgent):
     """Adaptation of Prov Agent class"""
     _prov_type = VOPROV_AGENT
 
     def set_name(self, name):
         """Set the name of this activity.
@@ -1013,15 +1016,15 @@
             other_attributes = {}
         if name is not None:
             other_attributes.update({VOPROV_ATTR_NAME: name})
         if comment is not None:
             other_attributes.update({VOPROV['comment']: comment})
         if activityDescription is not None:
             self.description(identifier, activityDescription)
-        if len(other_attributes) is 0:
+        if len(other_attributes) == 0:
             other_attributes = None
         return self.new_record(
             VOPROV_ACTIVITY, identifier, {
                 VOPROV_ATTR_STARTTIME: startTime,
                 VOPROV_ATTR_ENDTIME: endTime
             },
             other_attributes
@@ -1054,15 +1057,15 @@
             other_attributes.update({VOPROV['generatedAtTime']: generatedAtTime})
         if invalidatedAtTime is not None:
             other_attributes.update({VOPROV['invalidatedAtTime']: invalidatedAtTime})
         if comment is not None:
             other_attributes.update({VOPROV['comment']: comment})
         if entityDescription is not None:
             self.description(identifier, entityDescription)
-        if len(other_attributes) is 0:
+        if len(other_attributes) == 0:
             other_attributes = None
         return self.new_record(
             VOPROV_ENTITY, identifier, None, other_attributes
         )
 
     def valueEntity(self, identifier, value, name=None, location=None, generatedAtTime=None, invalidatedAtTime=None,
                     comment=None, valueDescription=None, other_attributes=None):
@@ -1095,15 +1098,15 @@
             other_attributes.update({VOPROV['invalidatedAtTime']: invalidatedAtTime})
         if comment is not None:
             other_attributes.update({VOPROV['comment']: comment})
         if value is not None:
             other_attributes.update({VOPROV['value']: value})
         if valueDescription is not None:
             self.description(identifier, valueDescription)
-        if len(other_attributes) is 0:
+        if len(other_attributes) == 0:
             other_attributes = None
         return self.new_record(VOPROV_VALUE_ENTITY, identifier, None, other_attributes)
 
     def datasetEntity(self, identifier, name=None, location=None, generatedAtTime=None, invalidatedAtTime=None,
                       comment=None, datasetDescription=None, other_attributes=None):
         """
         Creates a new data set entity.
@@ -1130,15 +1133,15 @@
             other_attributes.update({VOPROV['generatedAtTime']: generatedAtTime})
         if invalidatedAtTime is not None:
             other_attributes.update({VOPROV['invalidatedAtTime']: invalidatedAtTime})
         if comment is not None:
             other_attributes.update({VOPROV['comment']: comment})
         if datasetDescription is not None:
             self.description(identifier, datasetDescription)
-        if len(other_attributes) is 0:
+        if len(other_attributes) == 0:
             other_attributes = None
         return self.new_record(VOPROV_DATASET_ENTITY, identifier, None, other_attributes)
 
     def configFile(self, identifier, name, location, comment=None, configFileDescription=None, other_attributes=None):
         """
         Creates a new config file.
 
@@ -1152,15 +1155,15 @@
         """
         if other_attributes is None:
             other_attributes = {}
         if comment is not None:
             other_attributes.update({VOPROV['comment']: comment})
         if configFileDescription is not None:
             self.description(identifier, configFileDescription)
-        if len(other_attributes) is 0:
+        if len(other_attributes) == 0:
             other_attributes = None
         return self.new_record(VOPROV_CONFIGURATION_FILE, identifier, {
             VOPROV_ATTR_NAME: name,
             VOPROV_ATTR_LOCATION: location
         }, other_attributes)
 
     def parameter(self, identifier, name, value, parameterDescription=None, other_attributes=None):
@@ -1175,15 +1178,16 @@
         :param other_attributes:        Optional other attributes as a dictionary or list
                                         of tuples to be added to the record optionally (default: None).
         """
         if parameterDescription is not None:
             self.description(identifier, parameterDescription)
         return self.new_record(VOPROV_CONFIGURATION_PARAMETER, identifier, {
             VOPROV_ATTR_NAME: name,
-            VOPROV_ATTR_VALUE: value
+            VOPROV_ATTR_VALUE: value,
+            PROV_LABEL: name + " = " + value
         }, other_attributes)
 
     def agent(self, identifier, name=None, type=None, comment=None, email=None, affiliation=None, phone=None,
               address=None, url=None, other_attributes=None):
         """
         Creates a new agent.
 
@@ -1213,15 +1217,15 @@
             other_attributes.update({VOPROV['affiliation']: affiliation})
         if phone is not None:
             other_attributes.update({VOPROV['phone']: phone})
         if address is not None:
             other_attributes.update({VOPROV['address']: address})
         if url is not None:
             other_attributes.update({VOPROV['url']: url})
-        if len(other_attributes) is 0:
+        if len(other_attributes) == 0:
             other_attributes = None
         return self.new_record(VOPROV_AGENT, identifier, None, other_attributes)
 
     def usage(self, activity, entity=None, usageDescription=None, role=None, time=None,
               identifier=None, other_attributes=None):
         """
         Creates a new usage record for an activity.
@@ -1240,15 +1244,15 @@
         """
         if other_attributes is None:
             other_attributes = {}
         if role is not None:
             other_attributes.update({VOPROV_ATTR_ROLE: role})
         if usageDescription is not None:
             other_attributes.update({VOPROV['descriptor']: usageDescription})
-        if len(other_attributes) is 0:
+        if len(other_attributes) == 0:
             other_attributes = None
         return self.new_record(
             VOPROV_USAGE, identifier, {
                 VOPROV_ATTR_ACTIVITY: activity,
                 VOPROV_ATTR_ENTITY: entity,
                 VOPROV_ATTR_TIME: _ensure_datetime(time)},
             other_attributes
@@ -1273,15 +1277,15 @@
         """
         if other_attributes is None:
             other_attributes = {}
         if role is not None:
             other_attributes.update({VOPROV_ATTR_ROLE: role})
         if generationDescription is not None:
             other_attributes.update({VOPROV['descriptor']: generationDescription})
-        if len(other_attributes) is 0:
+        if len(other_attributes) == 0:
             other_attributes = None
         return self.new_record(
             VOPROV_GENERATION, identifier, {
                 VOPROV_ATTR_ENTITY: entity,
                 VOPROV_ATTR_ACTIVITY: activity,
                 VOPROV_ATTR_TIME: _ensure_datetime(time)
             },
@@ -1399,15 +1403,15 @@
         :param other_attributes:        Optional other attributes as a dictionary or list
                                         of tuples to be added to the record optionally (default: None).
         """
         if other_attributes is None:
             other_attributes = {}
         if role is not None:
             other_attributes.update({VOPROV_ATTR_ROLE: role})
-        if len(other_attributes) is 0:
+        if len(other_attributes) == 0:
             other_attributes = None
         return self.new_record(
             VOPROV_ATTRIBUTION, identifier, {
                 VOPROV_ATTR_ENTITY: entity,
                 VOPROV_ATTR_AGENT: agent
             },
             other_attributes
@@ -1428,15 +1432,15 @@
         :param other_attributes:        Optional other attributes as a dictionary or list
                                         of tuples to be added to the record optionally (default: None).
         """
         if other_attributes is None:
             other_attributes = {}
         if role is not None:
             other_attributes.update({VOPROV_ATTR_ROLE: role})
-        if len(other_attributes) is 0:
+        if len(other_attributes) == 0:
             other_attributes = None
         return self.new_record(
             VOPROV_ASSOCIATION, identifier, {
                 VOPROV_ATTR_ACTIVITY: activity,
                 VOPROV_ATTR_AGENT: agent,
                 VOPROV_ATTR_PLAN: plan
             },
@@ -1696,15 +1700,15 @@
             other_attributes.update({VOPROV['description']: description})
         if docurl is not None:
             other_attributes.update({VOPROV['docurl']: docurl})
         if type is not None:
             other_attributes.update({VOPROV['type']: type})
         if subtype is not None:
             other_attributes.update({VOPROV['subtype']: subtype})
-        if len(other_attributes) is 0:
+        if len(other_attributes) == 0:
             other_attributes = None
         return self.new_record(
             VOPROV_ACTIVITY_DESCRIPTION, identifier, {
                 VOPROV_ATTR_NAME: name
             },
             other_attributes
         )
@@ -1725,15 +1729,15 @@
             other_attributes = {}
         if description is not None:
             other_attributes.update({VOPROV['description']: description})
         if docurl is not None:
             other_attributes.update({VOPROV['docurl']: docurl})
         if type is not None:
             other_attributes.update({VOPROV['type']: type})
-        if len(other_attributes) is 0:
+        if len(other_attributes) == 0:
             other_attributes = None
         return self.new_record(
             VOPROV_ENTITY_DESCRIPTION, identifier, {
                 VOPROV_ATTR_NAME: name
             },
             other_attributes
         )
@@ -1769,15 +1773,15 @@
             other_attributes.update({VOPROV['type']: type})
         if unit is not None:
             other_attributes.update({VOPROV['unit']: unit})
         if ucd is not None:
             other_attributes.update({VOPROV['ucd']: ucd})
         if utype is not None:
             other_attributes.update({VOPROV['utype']: utype})
-        if len(other_attributes) is 0:
+        if len(other_attributes) == 0:
             other_attributes = None
         return self.new_record(
             VOPROV_VALUE_DESCRIPTION, identifier, {
                 VOPROV_ATTR_NAME: name,
                 VOPROV_ATTR_VALUE_TYPE: valueType
             },
             other_attributes
@@ -1801,15 +1805,15 @@
             other_attributes = {}
         if description is not None:
             other_attributes.update({VOPROV['description']: description})
         if docurl is not None:
             other_attributes.update({VOPROV['docurl']: docurl})
         if type is not None:
             other_attributes.update({VOPROV['type']: type})
-        if len(other_attributes) is 0:
+        if len(other_attributes) == 0:
             other_attributes = None
         return self.new_record(
             VOPROV_DATASET_DESCRIPTION, identifier, {
                 VOPROV_ATTR_NAME: name,
                 VOPROV_ATTR_CONTENT_TYPE: contentType
             },
             other_attributes
@@ -1835,15 +1839,15 @@
             other_attributes = {}
         if description is not None:
             other_attributes.update({VOPROV['description']: description})
         if type is not None:
             other_attributes.update({VOPROV['type']: type})
         if multiplicity is not None:
             other_attributes.update({VOPROV['multiplicity']: multiplicity})
-        if len(other_attributes) is 0:
+        if len(other_attributes) == 0:
             other_attributes = None
         self.relate(identifier, activityDescription)
         if entityDescription:
             if not isinstance(entityDescription, list):
                 entityDescription = [entityDescription]
             for ed_item in entityDescription:
                 self.relate(ed_item, identifier)
@@ -1875,15 +1879,15 @@
             other_attributes = {}
         if description is not None:
             other_attributes.update({VOPROV['description']: description})
         if type is not None:
             other_attributes.update({VOPROV['type']: type})
         if multiplicity is not None:
             other_attributes.update({VOPROV['multiplicity']: multiplicity})
-        if len(other_attributes) is 0:
+        if len(other_attributes) == 0:
             other_attributes = None
         self.relate(identifier, activityDescription)
         if entityDescription:
             if not isinstance(entityDescription, list):
                 entityDescription = [entityDescription]
             for ed_item in entityDescription:
                 self.relate(ed_item, identifier)
@@ -1908,15 +1912,15 @@
         :param other_attributes:        Optional other attributes as a dictionary or list
                                         of tuples to be added to the record optionally (default: None).
         """
         if other_attributes is None:
             other_attributes = {}
         if description is not None:
             other_attributes.update({VOPROV['description']: description})
-        if len(other_attributes) is 0:
+        if len(other_attributes) == 0:
             other_attributes = None
         self.relate(identifier, activityDescription)
         return self.new_record(
             VOPROV_CONFIG_FILE_DESCRIPTION, identifier, {
                 VOPROV_ATTR_NAME: name,
                 VOPROV_ATTR_CONTENT_TYPE: contentType
             },
@@ -1965,15 +1969,15 @@
             other_attributes.update({VOPROV['min']: min})
         if max is not None:
             other_attributes.update({VOPROV['max']: max})
         if options is not None:
             other_attributes.update({VOPROV['options']: options})
         if default is not None:
             other_attributes.update({VOPROV['default']: default})
-        if len(other_attributes) is 0:
+        if len(other_attributes) == 0:
             other_attributes = None
         self.relate(identifier, activityDescription)
         return self.new_record(
             VOPROV_PARAMETER_DESCRIPTION, identifier, {
                 VOPROV_ATTR_NAME: name,
                 VOPROV_ATTR_VALUE_TYPE: valueType
             },
@@ -2338,15 +2342,15 @@
         :return: :py:class:`ProvDocument`
         """
         serializer = serializers.get(format)()
 
         if content is not None:
             # io.StringIO only accepts unicode strings
             stream = io.StringIO(
-                content if not isinstance(content, six.binary_type)
+                content if not isinstance(content, bytes)
                 else content.decode()
             )
             return serializer.deserialize(stream, **args)
 
         if source is not None:
             if hasattr(source, "read"):
                 return serializer.deserialize(source, **args)
```

### Comparing `voprov-0.0.2/voprov/models/voprovConfigurations.py` & `voprov-0.0.3/voprov/models/voprovConfigurations.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 # -*- coding: utf-8 -*-
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-
 from prov.model import (ProvElement, ProvBundle, ProvEntity)
 from voprov.models.constants import *
 
 __author__ = 'Jean-Francois Sornay'
 __email__ = 'jeanfrancois.sornay@gmail.com'
```

### Comparing `voprov-0.0.2/voprov/models/voprovDescriptions.py` & `voprov-0.0.3/voprov/models/voprovDescriptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 # -*- coding: utf-8 -*-
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-
 from prov.model import (ProvElement, ProvBundle, ProvEntity)
 from voprov.models.constants import *
 
 __author__ = 'Jean-Francois Sornay'
 __email__ = 'jeanfrancois.sornay@gmail.com'
 
 
@@ -92,15 +89,16 @@
         :param description:             A descriptive text for this kind of usage (default: None).
         :param type:                    Type of relation (default: None).
         :param multiplicity:            Number of expected input entities to be used with the given role
                                         (default: None).
         :param other_attributes:        Optional other attributes as a dictionary or list
                                         of tuples to be added to the record optionally (default: None).
         """
-        return self._bundle.usageDescription(identifier, self, role, description, type, multiplicity, entityDescription, other_attributes)
+        return self._bundle.usageDescription(identifier, self, role, description, type, multiplicity, entityDescription,
+                                             other_attributes)
 
     def generationDescription(self, identifier, role, description=None, type=None,
                               multiplicity=None, entityDescription=None, other_attributes=None):
         """
         Creates a new generation description.
 
         :param identifier:              Identifier for new generation description.
```

### Comparing `voprov-0.0.2/voprov/models/voprovRelations.py` & `voprov-0.0.3/voprov/models/voprovRelations.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 # -*- coding: utf-8 -*-
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-
 from prov.model import (ProvRelation, ProvBundle, ProvInfluence)
 from voprov.models.constants import *
 
 __author__ = 'Jean-Francois Sornay'
 __email__ = 'jeanfrancois.sornay@gmail.com'
```

### Comparing `voprov-0.0.2/voprov/serializers/__init__.py` & `voprov-0.0.3/voprov/serializers/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # -*- coding: utf-8 -*-
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-
 from voprov.serializers.provn import VOProvNSerializer
 from voprov.serializers.xml import VOProvXMLSerializer
+from voprov.serializers.provjson import VOProvJSONSerializer
 from prov import Error
 
 __author__ = 'Jean-Francois Sornay'
 __email__ = 'jeanfrancois.sornay@gmail.com'
 __all__ = [
     'get'
 ]
@@ -23,21 +21,21 @@
 
     serializers = None
     """Property caching all available serializers in a dict."""
 
     @staticmethod
     def load_serializers():
         """Loads all available serializers into the registry."""
-        from prov.serializers.provjson import ProvJSONSerializer
+        from voprov.serializers.provjson import VOProvJSONSerializer
         from voprov.serializers.provn import VOProvNSerializer
         from voprov.serializers.xml import VOProvXMLSerializer
         from prov.serializers.provrdf import ProvRDFSerializer
 
         Registry.serializers = {
-            'json': ProvJSONSerializer,
+            'json': VOProvJSONSerializer,
             'rdf': ProvRDFSerializer,
             'provn': VOProvNSerializer,
             'xml': VOProvXMLSerializer
         }
 
 
 def get(format_name):
```

### Comparing `voprov-0.0.2/voprov/serializers/provn.py` & `voprov-0.0.3/voprov/serializers/provn.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 # -*- coding: utf-8 -*-
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-
 from prov.serializers.provn import *
 
 
 class VOProvNSerializer(ProvNSerializer):
     """PROV-N serializer for ProvDocument
 
     """
```

### Comparing `voprov-0.0.2/voprov/serializers/xml.py` & `voprov-0.0.3/voprov/serializers/xml.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 # -*- coding: utf-8 -*-
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-
 from prov.serializers.provxml import *
 from voprov.models.constants import *
 
 # Create a dictionary containing all top-level PROV XML elements for an easy
 # mapping.
 FULL_NAMES_MAP = dict(PROV_N_MAP)
 FULL_NAMES_MAP.update(ADDITIONAL_N_MAP)
@@ -24,15 +21,15 @@
 
         :param stream: Where to save the output.
         :type force_types: boolean, optional
         :param force_types: Will force xsd:types to be written for most
             attributes mainly PROV-"attributes", e.g. tags not in the
             PROV namespace. Off by default meaning xsd:type attributes will
             only be set for prov:type, prov:location, and prov:value as is
-            done in the official PROV-XML specification. Furthermore the
+            done in the official PROV-XML specification. Furthermore, the
             types will always be set if the Python type requires it. False
             is a good default and it should rarely require changing.
         """
         xml_root = self.serialize_bundle(bundle=self.document,
                                          force_types=force_types)
         for bundle in self.document.bundles:
             self.serialize_bundle(bundle=bundle, element=xml_root,
@@ -85,19 +82,19 @@
             xml_bundle_root = etree.SubElement(
                 element, _ns_prov("bundleContent"), nsmap=nsmap)
         else:
             xml_bundle_root = etree.Element(_ns_prov("document"), nsmap=nsmap)
 
         if bundle.identifier:
             xml_bundle_root.attrib[_ns_prov("id")] = \
-                six.text_type(bundle.identifier)
+                str(bundle.identifier)
 
         for record in bundle._records:
             rec_type = record.get_type()
-            identifier = six.text_type(record._identifier) \
+            identifier = str(record._identifier) \
                 if record._identifier else None
 
             if identifier:
                 attrs = {_ns_prov("id"): identifier}
             else:
                 attrs = None
 
@@ -120,19 +117,19 @@
                             value.datatype.localpart)
                     if value.langtag is not None:
                         subelem.attrib[_ns_xml("lang")] = value.langtag
                     v = value.value
                 elif isinstance(value, prov.model.QualifiedName):
                     if attr not in PROV_ATTRIBUTE_QNAMES:
                         subelem.attrib[_ns_xsi("type")] = "xsd:QName"
-                    v = six.text_type(value)
+                    v = str(value)
                 elif isinstance(value, datetime.datetime):
                     v = value.isoformat()
                 else:
-                    v = six.text_type(value)
+                    v = str(value)
 
                 # xsd type inference.
                 #
                 # This is a bit messy and there are all kinds of special
                 # rules but it appears to get the job done.
                 #
                 # If it is a type element and does not yet have an
@@ -140,34 +137,32 @@
                 # The not startswith("prov:") check is a little bit hacky to
                 # avoid type interference when the type is a standard prov
                 # type.
                 #
                 # To enable a mapping of Python types to XML and back,
                 # the XSD type must be written for these types.
                 ALWAYS_CHECK = [bool, datetime.datetime, float,
-                                prov.identifier.Identifier]
-                # Add long and int on Python 2, only int on Python 3.
-                ALWAYS_CHECK.extend(six.integer_types)
+                                prov.identifier.Identifier, int]
                 ALWAYS_CHECK = tuple(ALWAYS_CHECK)
                 if (force_types or
                         type(value) in ALWAYS_CHECK or
                         attr in [PROV_TYPE, PROV_LOCATION, PROV_VALUE]) and \
                         _ns_xsi("type") not in subelem.attrib and \
-                        not six.text_type(value).startswith("voprov:") and \
+                        not str(value).startswith("voprov:") and \
                         not (attr in PROV_ATTRIBUTE_QNAMES and v) and \
                         attr not in [PROV_ATTR_TIME, PROV_LABEL]:
                     xsd_type = None
                     if isinstance(value, bool):
                         xsd_type = XSD_BOOLEAN
                         v = v.lower()
-                    elif isinstance(value, six.string_types):
+                    elif isinstance(value, str):
                         xsd_type = XSD_STRING
                     elif isinstance(value, float):
                         xsd_type = XSD_DOUBLE
-                    elif isinstance(value, six.integer_types):
+                    elif isinstance(value, int):
                         xsd_type = XSD_INT
                     elif isinstance(value, datetime.datetime):
                         # Exception of the exception, while technically
                         # still correct, do not write XSD dateTime type for
                         # attributes in the PROV namespaces as the type is
                         # already declared in the XSD and PROV XML also does
                         # not specify it in the docs.
@@ -175,15 +170,15 @@
                                 or "time" not in attr.localpart.lower():
                             xsd_type = XSD_DATETIME
                     elif isinstance(value, prov.identifier.Identifier):
                         xsd_type = XSD_ANYURI
 
                     if xsd_type is not None:
                         subelem.attrib[_ns_xsi("type")] = \
-                            six.text_type(xsd_type)
+                            str(xsd_type)
 
                 if attr in PROV_ATTRIBUTE_QNAMES and v:
                     subelem.attrib[_ns_prov("ref")] = v
                 else:
                     subelem.text = v
         return xml_bundle_root
```

### Comparing `voprov-0.0.2/voprov/visualization/dot.py` & `voprov-0.0.3/voprov/visualization/dot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 # -*- coding: utf-8 -*-
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-
 from prov.dot import *
 from voprov.visualization.graph import *
 
 __author__ = 'Jean-Francois Sornay'
 __email__ = 'jeanfrancois.sornay@gmail.com'
 
 # updating the generic node style map which is used when the object used in a relation is not declared
```

### Comparing `voprov-0.0.2/voprov.egg-info/SOURCES.txt` & `voprov-0.0.3/voprov.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+AUTHORS.rst
+LICENSE
 README.rst
 setup.py
 voprov/__init__.py
 voprov.egg-info/PKG-INFO
 voprov.egg-info/SOURCES.txt
 voprov.egg-info/dependency_links.txt
 voprov.egg-info/not-zip-safe
@@ -10,12 +12,13 @@
 voprov/models/__init__.py
 voprov/models/constants.py
 voprov/models/model.py
 voprov/models/voprovConfigurations.py
 voprov/models/voprovDescriptions.py
 voprov/models/voprovRelations.py
 voprov/serializers/__init__.py
+voprov/serializers/provjson.py
 voprov/serializers/provn.py
 voprov/serializers/xml.py
 voprov/visualization/__init__.py
 voprov/visualization/dot.py
 voprov/visualization/graph.py
```

