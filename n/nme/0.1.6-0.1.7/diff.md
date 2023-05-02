# Comparing `tmp/nme-0.1.6.tar.gz` & `tmp/nme-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nme-0.1.6.tar", last modified: Wed Sep 28 13:36:27 2022, max compression
+gzip compressed data, was "nme-0.1.7.tar", last modified: Tue May  2 18:27:16 2023, max compression
```

## Comparing `nme-0.1.6.tar` & `nme-0.1.7.tar`

### file list

```diff
@@ -1,44 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 13:36:27.904050 nme-0.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 13:36:27.900050 nme-0.1.6/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-09-28 13:36:12.000000 nme-0.1.6/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 13:36:27.900050 nme-0.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1804 2022-09-28 13:36:12.000000 nme-0.1.6/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (121)     5296 2022-09-28 13:36:12.000000 nme-0.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1446 2022-09-28 13:36:12.000000 nme-0.1.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      536 2022-09-28 13:36:12.000000 nme-0.1.6/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-09-28 13:36:12.000000 nme-0.1.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5962 2022-09-28 13:36:27.904050 nme-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4958 2022-09-28 13:36:12.000000 nme-0.1.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 13:36:27.900050 nme-0.1.6/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-09-28 13:36:12.000000 nme-0.1.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-09-28 13:36:12.000000 nme-0.1.6/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2335 2022-09-28 13:36:12.000000 nme-0.1.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     3660 2022-09-28 13:36:12.000000 nme-0.1.6/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-09-28 13:36:12.000000 nme-0.1.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      800 2022-09-28 13:36:12.000000 nme-0.1.6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-09-28 13:36:12.000000 nme-0.1.6/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 13:36:27.900050 nme-0.1.6/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      419 2022-09-28 13:36:12.000000 nme-0.1.6/examples/base_cbor_example.py
--rw-r--r--   0 runner    (1001) docker     (121)      390 2022-09-28 13:36:12.000000 nme-0.1.6/examples/base_example.py
--rw-r--r--   0 runner    (1001) docker     (121)     2099 2022-09-28 13:36:12.000000 nme-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-28 13:36:27.904050 nme-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 13:36:27.900050 nme-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 13:36:27.900050 nme-0.1.6/src/nme/
--rw-r--r--   0 runner    (1001) docker     (121)     1488 2022-09-28 13:36:12.000000 nme-0.1.6/src/nme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13719 2022-09-28 13:36:12.000000 nme-0.1.6/src/nme/_class_register.py
--rw-r--r--   0 runner    (1001) docker     (121)     5370 2022-09-28 13:36:12.000000 nme-0.1.6/src/nme/_serialize_hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-09-28 13:36:12.000000 nme-0.1.6/src/nme/_testsupport.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-09-28 13:36:27.000000 nme-0.1.6/src/nme/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 13:36:27.904050 nme-0.1.6/src/nme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5962 2022-09-28 13:36:27.000000 nme-0.1.6/src/nme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      752 2022-09-28 13:36:27.000000 nme-0.1.6/src/nme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-28 13:36:27.000000 nme-0.1.6/src/nme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-09-28 13:36:27.000000 nme-0.1.6/src/nme.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-09-28 13:36:27.000000 nme-0.1.6/src/nme.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-09-28 13:36:27.000000 nme-0.1.6/src/nme.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 13:36:27.904050 nme-0.1.6/src/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-09-28 13:36:12.000000 nme-0.1.6/src/tests/class_register_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     3675 2022-09-28 13:36:12.000000 nme-0.1.6/src/tests/test_cbor_hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)     5135 2022-09-28 13:36:12.000000 nme-0.1.6/src/tests/test_class_register.py
--rw-r--r--   0 runner    (1001) docker     (121)    10315 2022-09-28 13:36:12.000000 nme-0.1.6/src/tests/test_json_hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)      433 2022-09-28 13:36:12.000000 nme-0.1.6/tox.ini
+drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-05-02 18:27:16.299731 nme-0.1.7/
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     3101 2023-05-02 15:28:06.000000 nme-0.1.7/.gitignore
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1072 2023-05-02 14:34:16.000000 nme-0.1.7/LICENSE
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1040 2023-05-02 18:27:16.299731 nme-0.1.7/PKG-INFO
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)       88 2023-05-02 14:43:09.000000 nme-0.1.7/README.md
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1232 2023-05-02 17:22:16.000000 nme-0.1.7/pyproject.toml
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)       38 2023-05-02 18:27:16.299731 nme-0.1.7/setup.cfg
+drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-05-02 18:27:16.299731 nme-0.1.7/src/
+drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-05-02 18:27:16.299731 nme-0.1.7/src/nme.egg-info/
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     1040 2023-05-02 18:27:16.000000 nme-0.1.7/src/nme.egg-info/PKG-INFO
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)      340 2023-05-02 18:27:16.000000 nme-0.1.7/src/nme.egg-info/SOURCES.txt
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)        1 2023-05-02 18:27:16.000000 nme-0.1.7/src/nme.egg-info/dependency_links.txt
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)       73 2023-05-02 18:27:16.000000 nme-0.1.7/src/nme.egg-info/requires.txt
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)       10 2023-05-02 18:27:16.000000 nme-0.1.7/src/nme.egg-info/top_level.txt
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)      730 2023-05-02 18:22:27.000000 nme-0.1.7/src/nme.py
+drwxr-xr-x   0 czaki     (1000) grzegorz  (1000)        0 2023-05-02 18:27:16.299731 nme-0.1.7/src/tests/
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)       78 2022-09-28 12:57:55.000000 nme-0.1.7/src/tests/class_register_util.py
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     3644 2023-05-02 15:21:01.000000 nme-0.1.7/src/tests/test_cbor_hooks.py
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     5104 2023-05-02 15:21:01.000000 nme-0.1.7/src/tests/test_class_register.py
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)     9430 2023-05-02 15:21:55.000000 nme-0.1.7/src/tests/test_json_hooks.py
+-rw-r--r--   0 czaki     (1000) grzegorz  (1000)      441 2023-05-02 15:24:32.000000 nme-0.1.7/tox.ini
```

### Comparing `nme-0.1.6/LICENSE.txt` & `nme-0.1.7/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Grzegorz Bokota
+Copyright (c) 2023 Grzegorz Bokota
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `nme-0.1.6/src/tests/test_cbor_hooks.py` & `nme-0.1.7/src/tests/test_cbor_hooks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from dataclasses import dataclass
 from enum import Enum
 
 import cbor2
 import pytest
 from pydantic import BaseModel
 
-from nme import nme_cbor_decoder, nme_cbor_encoder, register_class, rename_key
-from nme._class_register import class_to_str
+from nme import nme_cbor_decoder, nme_cbor_encoder, register_class, rename_key, class_to_str
 
 
 class RadiusType(Enum):
     NO = 0
     R2D = 1
     R3D = 2
```

### Comparing `nme-0.1.6/src/tests/test_class_register.py` & `nme-0.1.7/src/tests/test_class_register.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from enum import Enum
 from typing import Any, Dict
 
 import pytest
 
-from nme import REGISTER, register_class, rename_key, update_argument
-from nme._class_register import class_to_str
+from nme import REGISTER, register_class, rename_key, update_argument, class_to_str
 
 
 @register_class
 class SampleClass1:
     pass
```

### Comparing `nme-0.1.6/src/tests/test_json_hooks.py` & `nme-0.1.7/src/tests/test_json_hooks.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 from pathlib import Path
 
 import numpy as np
 import pytest
 from pydantic import BaseModel, Extra, dataclasses
 
 from nme import NMEEncoder, nme_object_hook, register_class, rename_key
-from nme._class_register import class_to_str
-from nme._serialize_hooks import add_class_info
 
 try:
     from napari.utils import Colormap
     from napari.utils.notifications import NotificationSeverity
 except ImportError:
     Colormap = None
     NotificationSeverity = None
@@ -151,40 +149,14 @@
             json.dump(ob, f_p, cls=NMEEncoder)
         with (tmp_path / "test.json").open("r") as f_p:
             ob2 = json.load(f_p, object_hook=nme_object_hook)
         assert ob2.data1 == 1
         assert ob2.data2 == 2
 
 
-def test_add_class_info_pydantic(clean_register):
-    @register_class
-    class SampleClass(BaseModel):
-        field: int = 1
-
-    dkt = {}
-    dkt = add_class_info(SampleClass(), dkt)
-    assert "__class__" in dkt
-    assert class_to_str(SampleClass) == dkt["__class__"]
-    assert len(dkt["__class_version_dkt__"]) == 1
-    assert dkt["__class_version_dkt__"][class_to_str(SampleClass)] == "0.0.0"
-
-
-def test_add_class_info_enum(clean_register):
-    @register_class
-    class SampleEnum(Enum):
-        field = 1
-
-    dkt = {}
-    dkt = add_class_info(SampleEnum.field, dkt)
-    assert "__class__" in dkt
-    assert class_to_str(SampleEnum) == dkt["__class__"]
-    assert len(dkt["__class_version_dkt__"]) == 1
-    assert dkt["__class_version_dkt__"][class_to_str(SampleEnum)] == "0.0.0"
-
-
 def test_path_serialization(tmp_path):
     with (tmp_path / "test.json").open("w") as f_p:
         json.dump(Path(), f_p, cls=NMEEncoder)
     with (tmp_path / "test.json").open("r") as f_p:
         data = json.load(f_p, object_hook=nme_object_hook)
     assert str(Path()) == data
```

