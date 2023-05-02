# Comparing `tmp/aiida-phonopy-1.0.0.tar.gz` & `tmp/aiida-phonopy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida-phonopy-1.0.0.tar", last modified: Wed Nov 23 11:20:46 2022, max compression
+gzip compressed data, was "aiida-phonopy-1.1.0.tar", last modified: Tue May  2 13:41:29 2023, max compression
```

## Comparing `aiida-phonopy-1.0.0.tar` & `aiida-phonopy-1.1.0.tar`

### file list

```diff
@@ -1,39 +1,46 @@
--rw-r--r--   0        0        0     3575 2022-10-25 10:53:20.497744 aiida-phonopy-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     1085 2022-10-25 10:53:20.499745 aiida-phonopy-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0     2003 2022-10-25 12:18:09.423923 aiida-phonopy-1.0.0/README.md
--rw-r--r--   0        0        0    52380 2022-10-25 10:53:20.513744 aiida-phonopy-1.0.0/examples/BaTiO3/FORCE_SETS
--rw-r--r--   0        0        0    21945 2022-10-25 10:53:20.515744 aiida-phonopy-1.0.0/examples/BaTiO3/phonopy.yaml
--rw-r--r--   0        0        0    52380 2022-10-25 10:53:20.521744 aiida-phonopy-1.0.0/examples/BaTiO3/ref_out/FORCE_SETS
--rw-r--r--   0        0        0       41 2022-10-25 10:53:20.523744 aiida-phonopy-1.0.0/examples/BaTiO3/ref_out/aiida.in
--rw-r--r--   0        0        0     1538 2022-10-25 10:53:20.525744 aiida-phonopy-1.0.0/examples/BaTiO3/ref_out/aiida.out
--rw-r--r--   0        0        0    58620 2022-10-25 10:53:20.527744 aiida-phonopy-1.0.0/examples/BaTiO3/ref_out/band.hdf5
--rw-r--r--   0        0        0    43797 2022-10-25 10:53:20.530744 aiida-phonopy-1.0.0/examples/BaTiO3/ref_out/force_constants.hdf5
--rw-r--r--   0        0        0     2445 2022-10-25 10:53:20.532744 aiida-phonopy-1.0.0/examples/BaTiO3/ref_out/irreps.yaml
--rw-r--r--   0        0        0    39220 2022-10-25 10:53:20.534744 aiida-phonopy-1.0.0/examples/BaTiO3/ref_out/mesh.hdf5
--rw-r--r--   0        0        0    21837 2022-10-25 10:53:20.537744 aiida-phonopy-1.0.0/examples/BaTiO3/ref_out/phonopy.yaml
--rw-r--r--   0        0        0     2336 2022-10-25 10:53:20.539744 aiida-phonopy-1.0.0/examples/BaTiO3/ref_out/qpoints.hdf5
--rw-r--r--   0        0        0    33644 2022-10-25 10:53:20.542744 aiida-phonopy-1.0.0/examples/BaTiO3/ref_out/thermal_properties.yaml
--rw-r--r--   0        0        0     1254 2022-11-23 11:10:02.227907 aiida-phonopy-1.0.0/examples/BaTiO3/script.py
--rw-r--r--   0        0        0     3318 2022-11-23 11:10:02.229907 aiida-phonopy-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       91 2022-11-23 11:10:02.231907 aiida-phonopy-1.0.0/src/aiida_phonopy/__init__.py
--rw-r--r--   0        0        0        0 2022-11-21 14:49:58.336931 aiida-phonopy-1.0.0/src/aiida_phonopy/calculations/__init__.py
--rw-r--r--   0        0        0       62 2022-11-21 14:49:58.187932 aiida-phonopy-1.0.0/src/aiida_phonopy/calculations/functions/__init__.py
--rw-r--r--   0        0        0    10852 2022-11-21 14:49:58.281931 aiida-phonopy-1.0.0/src/aiida_phonopy/calculations/functions/data_utils.py
--rw-r--r--   0        0        0     3591 2022-11-21 14:49:58.333931 aiida-phonopy-1.0.0/src/aiida_phonopy/calculations/functions/link_structures.py
--rw-r--r--   0        0        0    18545 2022-11-21 14:49:58.571929 aiida-phonopy-1.0.0/src/aiida_phonopy/calculations/phonopy.py
--rw-r--r--   0        0        0      271 2022-11-21 14:49:59.015927 aiida-phonopy-1.0.0/src/aiida_phonopy/data/__init__.py
--rw-r--r--   0        0        0     2884 2022-11-21 18:20:28.978564 aiida-phonopy-1.0.0/src/aiida_phonopy/data/force_constants.py
--rw-r--r--   0        0        0     5592 2022-11-21 14:49:59.105926 aiida-phonopy-1.0.0/src/aiida_phonopy/data/phonopy.py
--rw-r--r--   0        0        0     9448 2022-11-23 11:10:02.233907 aiida-phonopy-1.0.0/src/aiida_phonopy/data/preprocess.py
--rw-r--r--   0        0        0    19024 2022-11-23 11:10:02.235907 aiida-phonopy-1.0.0/src/aiida_phonopy/data/raw.py
--rw-r--r--   0        0        0       65 2022-11-21 14:49:58.597929 aiida-phonopy-1.0.0/src/aiida_phonopy/parsers/__init__.py
--rw-r--r--   0        0        0     2450 2022-11-21 14:49:58.615929 aiida-phonopy-1.0.0/src/aiida_phonopy/parsers/base.py
--rw-r--r--   0        0        0    17951 2022-11-23 11:10:02.238907 aiida-phonopy-1.0.0/src/aiida_phonopy/parsers/phonopy.py
--rw-r--r--   0        0        0        0 2022-11-21 14:49:58.576929 aiida-phonopy-1.0.0/src/aiida_phonopy/parsers/raw_parsers/__init__.py
--rw-r--r--   0        0        0     1080 2022-11-21 14:49:58.595929 aiida-phonopy-1.0.0/src/aiida_phonopy/parsers/raw_parsers/phonopy.py
--rw-r--r--   0        0        0        0 2022-11-21 14:49:58.975927 aiida-phonopy-1.0.0/src/aiida_phonopy/utils/__init__.py
--rw-r--r--   0        0        0     1879 2022-11-21 14:49:59.001927 aiida-phonopy-1.0.0/src/aiida_phonopy/utils/mapping.py
--rw-r--r--   0        0        0      688 2022-11-21 14:49:59.008927 aiida-phonopy-1.0.0/src/aiida_phonopy/utils/resources.py
--rw-r--r--   0        0        0        0 2022-11-21 14:49:58.848928 aiida-phonopy-1.0.0/src/aiida_phonopy/workflows/__init__.py
--rw-r--r--   0        0        0    15642 2022-11-21 14:49:58.971927 aiida-phonopy-1.0.0/src/aiida_phonopy/workflows/phonopy.py
--rw-r--r--   0        0        0     3526 1970-01-01 00:00:00.000000 aiida-phonopy-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3718 2023-05-02 11:10:46.800256 aiida-phonopy-1.1.0/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     2397 2023-05-02 11:10:46.822256 aiida-phonopy-1.1.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1512 2023-05-02 11:10:46.868255 aiida-phonopy-1.1.0/.github/workflows/validate_release_tag.py
+-rw-r--r--   0        0        0      392 2022-10-25 11:13:01.498840 aiida-phonopy-1.1.0/.gitignore
+-rw-r--r--   0        0        0      781 2023-05-02 11:30:11.383556 aiida-phonopy-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      239 2022-10-25 10:53:20.495745 aiida-phonopy-1.1.0/.readthedocs.yml
+-rw-r--r--   0        0        0     4028 2023-05-02 11:42:38.288260 aiida-phonopy-1.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1085 2022-10-25 10:53:20.499745 aiida-phonopy-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     2003 2022-10-25 12:18:09.423923 aiida-phonopy-1.1.0/README.md
+-rw-r--r--   0        0        0      155 2022-01-27 11:33:53.420852 aiida-phonopy-1.1.0/docker-compose.yml
+-rw-r--r--   0        0        0    52380 2022-10-25 10:53:20.513744 aiida-phonopy-1.1.0/examples/BaTiO3/FORCE_SETS
+-rw-r--r--   0        0        0    21945 2022-10-25 10:53:20.515744 aiida-phonopy-1.1.0/examples/BaTiO3/phonopy.yaml
+-rw-r--r--   0        0        0    52380 2022-10-25 10:53:20.521744 aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/FORCE_SETS
+-rw-r--r--   0        0        0       41 2022-10-25 10:53:20.523744 aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/aiida.in
+-rw-r--r--   0        0        0     1538 2022-10-25 10:53:20.525744 aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/aiida.out
+-rw-r--r--   0        0        0    58620 2022-10-25 10:53:20.527744 aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/band.hdf5
+-rw-r--r--   0        0        0    43797 2022-10-25 10:53:20.530744 aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/force_constants.hdf5
+-rw-r--r--   0        0        0     2445 2022-10-25 10:53:20.532744 aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/irreps.yaml
+-rw-r--r--   0        0        0    39220 2022-10-25 10:53:20.534744 aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/mesh.hdf5
+-rw-r--r--   0        0        0    21837 2022-10-25 10:53:20.537744 aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/phonopy.yaml
+-rw-r--r--   0        0        0     2336 2022-10-25 10:53:20.539744 aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/qpoints.hdf5
+-rw-r--r--   0        0        0    33644 2022-10-25 10:53:20.542744 aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/thermal_properties.yaml
+-rw-r--r--   0        0        0     1254 2023-05-02 11:10:46.944255 aiida-phonopy-1.1.0/examples/BaTiO3/script.py
+-rw-r--r--   0        0        0     3220 2023-05-02 11:21:44.224474 aiida-phonopy-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       91 2023-05-02 11:13:04.579463 aiida-phonopy-1.1.0/src/aiida_phonopy/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-21 14:49:58.336931 aiida-phonopy-1.1.0/src/aiida_phonopy/calculations/__init__.py
+-rw-r--r--   0        0        0       62 2022-11-21 14:49:58.187932 aiida-phonopy-1.1.0/src/aiida_phonopy/calculations/functions/__init__.py
+-rw-r--r--   0        0        0    10382 2023-02-20 17:13:17.220510 aiida-phonopy-1.1.0/src/aiida_phonopy/calculations/functions/data_utils.py
+-rw-r--r--   0        0        0     3591 2022-11-21 14:49:58.333931 aiida-phonopy-1.1.0/src/aiida_phonopy/calculations/functions/link_structures.py
+-rw-r--r--   0        0        0    18063 2023-05-02 11:02:32.280097 aiida-phonopy-1.1.0/src/aiida_phonopy/calculations/phonopy.py
+-rw-r--r--   0        0        0      271 2022-11-21 14:49:59.015927 aiida-phonopy-1.1.0/src/aiida_phonopy/data/__init__.py
+-rw-r--r--   0        0        0     3026 2023-05-02 11:02:03.694261 aiida-phonopy-1.1.0/src/aiida_phonopy/data/force_constants.py
+-rw-r--r--   0        0        0     9265 2023-05-02 10:59:59.422975 aiida-phonopy-1.1.0/src/aiida_phonopy/data/phonopy.py
+-rw-r--r--   0        0        0    11504 2023-05-02 11:14:43.966892 aiida-phonopy-1.1.0/src/aiida_phonopy/data/preprocess.py
+-rw-r--r--   0        0        0    19358 2023-05-02 11:10:47.202254 aiida-phonopy-1.1.0/src/aiida_phonopy/data/raw.py
+-rw-r--r--   0        0        0       65 2022-11-21 14:49:58.597929 aiida-phonopy-1.1.0/src/aiida_phonopy/parsers/__init__.py
+-rw-r--r--   0        0        0     2450 2022-11-21 14:49:58.615929 aiida-phonopy-1.1.0/src/aiida_phonopy/parsers/base.py
+-rw-r--r--   0        0        0    18362 2023-05-02 11:10:47.175254 aiida-phonopy-1.1.0/src/aiida_phonopy/parsers/phonopy.py
+-rw-r--r--   0        0        0        0 2022-11-21 14:49:58.576929 aiida-phonopy-1.1.0/src/aiida_phonopy/parsers/raw_parsers/__init__.py
+-rw-r--r--   0        0        0     1080 2023-02-10 21:29:51.740132 aiida-phonopy-1.1.0/src/aiida_phonopy/parsers/raw_parsers/phonopy.py
+-rw-r--r--   0        0        0        0 2022-11-21 14:49:58.975927 aiida-phonopy-1.1.0/src/aiida_phonopy/utils/__init__.py
+-rw-r--r--   0        0        0     1879 2022-11-21 14:49:59.001927 aiida-phonopy-1.1.0/src/aiida_phonopy/utils/mapping.py
+-rw-r--r--   0        0        0      688 2022-11-21 14:49:59.008927 aiida-phonopy-1.1.0/src/aiida_phonopy/utils/resources.py
+-rw-r--r--   0        0        0        0 2022-11-21 14:49:58.848928 aiida-phonopy-1.1.0/src/aiida_phonopy/workflows/__init__.py
+-rw-r--r--   0        0        0    15627 2023-05-02 11:05:35.530044 aiida-phonopy-1.1.0/src/aiida_phonopy/workflows/phonopy.py
+-rw-r--r--   0        0        0     3585 1970-01-01 00:00:00.000000 aiida-phonopy-1.1.0/PKG-INFO
```

### Comparing `aiida-phonopy-1.0.0/CHANGELOG.md` & `aiida-phonopy-1.1.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,22 @@
 # Changelog
 
+## v1.1.0 - 2023-05-02
+
+[full changelog](https://github.com/aiida-phonopy/aiida-phonopy/compare/v1.1.0...v1.0.0)
+
+In this release we apply some improvements in the way the data is stored, and refactor the calculation utils to make names shorter and more comprehensible.
+
+## v1.0.0 - 2022-11-0X
+
+[full changelog](https://github.com/aiida-phonopy/aiida-phonopy/compare/v1.0.0...v0.7.0)
+
+In this release the new version of AiiDA v2.x is fully supported.
+
+
 ## v0.7.0 - 2022-11-0X
 
 [full changelog](https://github.com/aiida-phonopy/aiida-phonopy/compare/v0.7.0...v0.6.0)
 
 This new release contains radical changes from the previous versions. The new changes have been made to encounter the request and the possibility
 to interface with more (possibly any) force calculator.
```

### Comparing `aiida-phonopy-1.0.0/LICENSE.txt` & `aiida-phonopy-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.0.0/README.md` & `aiida-phonopy-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.0.0/examples/BaTiO3/FORCE_SETS` & `aiida-phonopy-1.1.0/examples/BaTiO3/FORCE_SETS`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.0.0/examples/BaTiO3/phonopy.yaml` & `aiida-phonopy-1.1.0/examples/BaTiO3/phonopy.yaml`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.0.0/examples/BaTiO3/ref_out/FORCE_SETS` & `aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/FORCE_SETS`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.0.0/examples/BaTiO3/ref_out/aiida.out` & `aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/aiida.out`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.0.0/examples/BaTiO3/ref_out/band.hdf5` & `aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/band.hdf5`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.0.0/examples/BaTiO3/ref_out/force_constants.hdf5` & `aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/force_constants.hdf5`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.0.0/examples/BaTiO3/ref_out/irreps.yaml` & `aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/irreps.yaml`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.0.0/examples/BaTiO3/ref_out/mesh.hdf5` & `aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/mesh.hdf5`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.0.0/examples/BaTiO3/ref_out/phonopy.yaml` & `aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/phonopy.yaml`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.0.0/examples/BaTiO3/ref_out/qpoints.hdf5` & `aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/qpoints.hdf5`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.0.0/examples/BaTiO3/ref_out/thermal_properties.yaml` & `aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/thermal_properties.yaml`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.0.0/examples/BaTiO3/script.py` & `aiida-phonopy-1.1.0/examples/BaTiO3/script.py`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.0.0/pyproject.toml` & `aiida-phonopy-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -19,34 +19,35 @@
     'Operating System :: MacOS :: MacOS X',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Topic :: Scientific/Engineering :: Physics',
     'Topic :: Scientific/Engineering :: Chemistry',
 ]
-keywords = ['aiida', 'workflows']
+keywords = ['aiida', 'phonopy', 'workflows']
 requires-python = '>=3.8'
 dependencies = [
-    "aiida-core>=2.0.0",
+    "aiida-core>=2.0.0,<3.0.0",
     "phonopy>=2.14,<3.0.0",
 ]
 
 [project.urls]
 Source = "https://github.com/aiida-phonopy/aiida-phonopy"
 
 [project.optional-dependencies]
 pre-commit = [
     'pre-commit~=2.17',
-    'pylint==2.13.7',
+    'pylint==2.17.2',
     'pylint-aiida~=0.1.1',
+    'toml',
 ]
 tests = [
     'pgtest~=1.3',
-    'pytest~=6.2',
-    'pytest-regressions~=1.0',
+    'pytest~=6.0',
+    'pytest-regressions~=2.3',
 ]
 docs = [
     "Sphinx",
     "docutils",
     "sphinx-copybutton~=0.3.0",
     "sphinx-book-theme~=0.1.0",
     "sphinx-click~=2.7.1",
@@ -70,20 +71,14 @@
 [tool.flit.module]
 name = 'aiida_phonopy'
 
 [tool.flit.sdist]
 exclude = [
     'tests/',
     'docs/',
-    '.git/',
-    '.github/',
-    '.gitignore',
-    '.pre-commit-config.yaml',
-    '.readthedocs.yml',
-    'docker-compose.yml',
 ]
 
 [tool.flynt]
 line-length = 120
 fail-on-change = true
 
 [tool.isort]
```

### Comparing `aiida-phonopy-1.0.0/src/aiida_phonopy/calculations/functions/data_utils.py` & `aiida-phonopy-1.1.0/src/aiida_phonopy/calculations/functions/data_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,61 +4,59 @@
 from aiida.engine import calcfunction
 from aiida.plugins import DataFactory
 
 PreProcessData = DataFactory('phonopy.preprocess')
 PhonopyData = DataFactory('phonopy.phonopy')
 
 __all__ = (
-    'get_unitcell_from_distance', 'get_primitive_from_distance', 'get_supercell_from_distance',
-    'get_supercells_with_displacements_from_distance', 'get_displacements_from_distance',
-    'get_preprocess_with_new_displacements_from_distance', 'generate_preprocess_data_from_distance',
-    'generate_phonopy_data_full', 'CalcfunctionMixin'
+    'get_unitcell', 'get_primitive', 'get_supercell', 'get_supercells_with_displacements', 'get_displacements',
+    'get_preprocess_with_new_displacements', 'generate_preprocess_data', 'generate_phonopy_data', 'CalcfunctionMixin'
 )
 
 
 @calcfunction
-def get_unitcell_from_distance(preprocess_data: PreProcessData):
+def get_unitcell(preprocess_data: PreProcessData):
     """Get the unitcell of a PreProcessData as a StructureData."""
     structure_data = preprocess_data.get_unitcell()
     return structure_data
 
 
 @calcfunction
-def get_primitive_from_distance(preprocess_data: PreProcessData):
+def get_primitive(preprocess_data: PreProcessData):
     """Get the primitive cell of a PreProcessData as a StructureData."""
     structure_data = preprocess_data.get_primitive_cell()
     return structure_data
 
 
 @calcfunction
-def get_supercell_from_distance(preprocess_data: PreProcessData):
+def get_supercell(preprocess_data: PreProcessData):
     """Get the supercell (pristine) of a PreProcessData as a StructureData."""
     structure_data = preprocess_data.get_supercell()
     return structure_data
 
 
 @calcfunction
-def get_supercells_with_displacements_from_distance(preprocess_data: PreProcessData):
+def get_supercells_with_displacements(preprocess_data: PreProcessData):
     """Get the supercells with displacements of a PreProcessData as a StructureData."""
     structures_data = preprocess_data.get_supercells_with_displacements()
     return structures_data
 
 
 @calcfunction
-def get_displacements_from_distance(preprocess_data: PreProcessData):
+def get_displacements(preprocess_data: PreProcessData):
     """Get the displacements of a PreProcessData as an ArrayData with array name `displacements`."""
     displacements = preprocess_data.get_displacements()
     the_displacements = orm.ArrayData()
     the_displacements.set_array('displacements', displacements)
 
     return the_displacements
 
 
 @calcfunction
-def generate_preprocess_data_from_distance(
+def generate_preprocess_data(
     structure: orm.StructureData,
     displacement_generator=None,
     supercell_matrix=None,
     primitive_matrix=None,
     symprec=None,
     is_symmetry=None,
     distinguish_kinds=None,
@@ -124,17 +122,15 @@
 
     preprocess.set_displacements(**displ_generator)
 
     return preprocess
 
 
 @calcfunction
-def get_preprocess_with_new_displacements_from_distance(
-    preprocess_data: PreProcessData, displacement_generator: orm.Dict
-):
+def get_preprocess_with_new_displacements(preprocess_data: PreProcessData, displacement_generator: orm.Dict):
     """Get a new PreProcessData from an old one from new displacement generator settings."""
     displacement_dataset = preprocess_data.generate_displacement_dataset(**displacement_generator.get_dict())
 
     preprocess = PreProcessData(
         structure=preprocess_data.get_unitcell(),
         supercell_matrix=preprocess_data.supercell_matrix,
         primitive_matrix=preprocess_data.primitive_matrix,
@@ -145,64 +141,54 @@
 
     preprocess.set_displacements_from_dataset(displacement_dataset)
 
     return preprocess
 
 
 @calcfunction
-def generate_phonopy_data_full(preprocess_data: PreProcessData, nac_parameters=None, **forces_dict):
+def generate_phonopy_data(preprocess_data: PreProcessData, nac_parameters=None, forces_index=None, **forces_dict):
     """Create a PhonopyData node from a PreProcess(Phonopy)Data node, storing forces and (optionally)
         non-analytical constants.
 
         `Forces` must be passed as **kwargs**, since we are calling a calcfunction with a variable
         number of supercells forces.
 
         :param nac_parameters: ArrayData containing 'dielectric' and 'born_charges' as arrays
             with their correct shape
+        :param forces_index: Int if a TrajectoryData is given, in order to get the correct slice of the array.
         :param forces_dict: dictionary of supercells forces as ArrayData stored as `forces`, each Data
-            labelled in the dictionary in the format `{prefix}_{suffix}`.
+            labelled in the dictionary in the format `forces_{suffix}`.
             The prefix is common and the suffix corresponds to the suffix number of the supercell with
             displacement label given from the `get_supercells_with_displacements` method.
 
             For example:
                 {'forces_1':ArrayData, 'forces_2':ArrayData}
                 <==>
                 {'supercell_1':StructureData, 'supercell_2':StructureData}
                 and forces in each ArrayData stored as 'forces',
                 i.e. ArrayData.get_array('forces') must not raise error
 
             .. note: if residual forces would be stored, label it with 0 as suffix.
     """
-    import numpy as np
-
-    # Getting the prefix
-    for key in forces_dict:
-        try:
-            int(key.split('_')[-1])
-            # dumb way of getting the prefix including cases of multiple `_`, e.g. `force_calculation_001`
-            prefix = key[:-(len(key.split('_')[-1]) + 1)]
-        except ValueError as err:
-            raise ValueError(f'{key} is not an acceptable key, must finish with an int number.') from err
+    prefix = 'forces'
 
     forces_0 = forces_dict.pop(f'{prefix}_0', None)
+    # Setting the dictionary of forces
+    dict_of_forces = {}
 
-    # Setting force sets array
-    force_sets = [0 for _ in forces_dict]
-
-    # Filling arrays in numeric order determined by the key label
     for key, value in forces_dict.items():
-        index = int(key.split('_')[-1])
-        force_sets[index - 1] = value.get_array('forces')
+        if key.startswith(prefix):
+            dict_of_forces[key] = value.get_array('forces')
 
-    # Finilizing force sets array
-    sets_of_forces = np.array(force_sets)
+    if forces_index is not None:
+        forces_index = forces_index.value
 
     # Setting data on a new PhonopyData
     new_phonopy_data = PhonopyData(preprocess_data=preprocess_data)
-    new_phonopy_data.set_forces(sets_of_forces=sets_of_forces)
+    new_phonopy_data.set_forces(dict_of_forces=dict_of_forces, forces_index=forces_index)
 
     if forces_0 is not None:
         new_phonopy_data.set_residual_forces(forces=forces_0.get_array('forces'))
 
     if nac_parameters is not None:
         new_phonopy_data.set_dielectric(nac_parameters.get_array('dielectric'))
         new_phonopy_data.set_born_charges(nac_parameters.get_array('born_charges'))
@@ -214,54 +200,57 @@
     """Set of calcfunctions to be called from the aiida-phonopy DataTypes."""
 
     def __init__(self, data_node):
         self._data_node = data_node
 
     def get_unitcell(self):
         """Get the unitcell as a StructureData through a calfunction."""
-        return get_unitcell_from_distance(preprocess_data=self._data_node)
+        return get_unitcell(preprocess_data=self._data_node)
 
     def get_primitive_cell(self):
         """Get the primitive cell as a StructureData through a calfunction."""
-        return get_primitive_from_distance(preprocess_data=self._data_node)
+        return get_primitive(preprocess_data=self._data_node)
 
     def get_supercell(self):
         """Get the supercell (pristine) as a StructureData through a calfunction."""
-        return get_supercell_from_distance(preprocess_data=self._data_node)
+        return get_supercell(preprocess_data=self._data_node)
 
     def get_supercells_with_displacements(self):
         """Get the supercells with displacements as a StructureData through a calfunction."""
-        return get_supercells_with_displacements_from_distance(preprocess_data=self._data_node)
+        return get_supercells_with_displacements(preprocess_data=self._data_node)
 
     def get_displacements(self):
         """Get the displacements as an ArrayData through a calfunction."""
-        return get_displacements_from_distance(preprocess_data=self._data_node)
+        return get_displacements(preprocess_data=self._data_node)
 
     def get_preprocess_with_new_displacements(self, displacement_generator: orm.Dict):
         """Create a PreProcessData node from a PreProcess/PhonopyData with a new set of displacements.
 
         :param displacement_generator: a `storable` dictionary  """
-        return get_preprocess_with_new_displacements_from_distance(
+        return get_preprocess_with_new_displacements(
             preprocess_data=self._data_node, displacement_generator=displacement_generator
         )
 
-    def generate_full_phonopy_data(self, nac_parameters=None, **forces_dict):
+    def generate_phonopy_data(self, nac_parameters=None, forces_index=None, **forces_dict):
         """Create a PhonopyData node from a PreProcess(Phonopy)Data node, storing forces and (optionally)
         non-analytical constants.
 
         `Forces` must be passed as **kwargs**, since we are calling a calcfunction with a variable
         number of supercells forces.
 
         :param nac_parameters: ArrayData containing 'dielectric' and 'born_charges' as arrays
             with their correct shape
+        :param forces_index: Int if a TrajectoryData is given, in order to get the correct slice of the array.
         :param forces_dict: dictionary of supercells forces as ArrayData stored as `forces`, each Data
             labelled in the dictionary in the format `{prefix}_{suffix}`.
             The prefix is common and the suffix corresponds to the suffix number of the supercell with
             displacement label given from the `get_supercells_with_displacements` method
 
             For example:
                 {'forces_1':ArrayData, 'forces_2':ArrayData} goes along with
                 {'supercell_1':StructureData, 'supercell_2':StructureData}
                 and forces in each ArrayData stored as 'forces',
                 i.e. ArrayData.get_array('forces') must not raise error
         """
-        return generate_phonopy_data_full(preprocess_data=self._data_node, nac_parameters=nac_parameters, **forces_dict)
+        return generate_phonopy_data(
+            preprocess_data=self._data_node, nac_parameters=nac_parameters, forces_index=forces_index, **forces_dict
+        )
```

### Comparing `aiida-phonopy-1.0.0/src/aiida_phonopy/calculations/functions/link_structures.py` & `aiida-phonopy-1.1.0/src/aiida_phonopy/calculations/functions/link_structures.py`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.0.0/src/aiida_phonopy/calculations/phonopy.py` & `aiida-phonopy-1.1.0/src/aiida_phonopy/calculations/phonopy.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,14 @@
     ]
 
     @classmethod
     def define(cls, spec):
         """Define inputs, outputs, and outline."""
         super().define(spec)
 
-        # in v1.0 it will be a namespace of Dict
         spec.input(
             'parameters',
             valid_type=orm.Dict,
             required=True,
             help=(
                 'Phonopy parameters (`setting tags`) for post processing. '
                 'The following tags, along their type, are allowed:\n' +
@@ -164,15 +163,15 @@
         spec.input(
             'force_constants',
             valid_type=ForceConstantsData,
             required=False,
             help='Force constants of the input structure.'
         )
         spec.input('settings', valid_type=orm.Dict, required=False, help='Settings for phonopy calculation.')
-        spec.inputs.validator = cls._validate_inputs
+        # spec.inputs.validator = cls._validate_inputs
 
         spec.input('metadata.options.withmpi', valid_type=bool, default=False)
         spec.input('metadata.options.input_filename', valid_type=str, default=cls._DEFAULT_INPUT_FILE)
         spec.input('metadata.options.output_filename', valid_type=str, default=cls._DEFAULT_OUTPUT_FILE)
         spec.input('metadata.options.parser_name', valid_type=str, default='phonopy.phonopy')
         spec.inputs['metadata']['options']['resources'].default = lambda: {'num_machines': 1}
 
@@ -215,15 +214,15 @@
         )
         spec.exit_code(
             303,
             'ERROR_OUTPUT_PHONOPY_MISSING',
             message='The retrieved folder did not contain the required phonopy file.'
         )
         spec.exit_code(
-            303,
+            304,
             'ERROR_OUTPUT_FILES_MISSING',
             message='The retrieved folder did not contain one or more expected output files.'
         )
         spec.exit_code(
             305, 'ERROR_BAD_INPUTS', message='No run mode has been selected.'
         )  # maybe we should check this from the input too
 
@@ -263,23 +262,14 @@
             if invalid_values:
                 return f'Parameters tags must be of the correct type; got invalid values {invalid_values}.'
 
         if value:
             if isinstance(value, orm.Dict):
                 __validate_dict(value.get_dict())
 
-    @classmethod
-    def _validate_inputs(cls, value, _):
-        """Validate the top level namespace."""
-        if 'force_constants' in value or 'phonopy_data' in value:
-            if 'force_constants' in value and 'phonopy_data' in value:
-                return 'specify only one between `force_constants` and `phonopy_data`'
-        else:
-            return 'at least one between `force_constants` and `phonopy_data` must be specified'
-
     def prepare_for_submission(self, folder):
         """Prepare the calculation job for submission by transforming input nodes into input files.
 
         In addition to the input files being written to the sandbox folder, a `CalcInfo` instance will be returned that
         contains lists of files that need to be copied to the remote machine before job submission, as well as file
         lists that are to be retrieved after job completion.
 
@@ -380,15 +370,15 @@
             for key in ['symmetrize_nac', 'factor_nac', 'subtract_residual_forces']:
                 if key in the_settings:
                     kwargs.update({key: the_settings[key]})
 
         if 'phonopy_data' in self.inputs:
             ph = self.inputs.phonopy_data.get_phonopy_instance(**kwargs)
         elif 'force_constants' in self.inputs:
-            ph = self.force_constants.get_phonopy_instance(**kwargs)
+            ph = self.inputs.force_constants.get_phonopy_instance(**kwargs)
 
         # Setting the phonopy yaml obtject to produce yaml lines
         # .. note: this does not write the force constants
         phpy_yaml = PhonopyYaml()
         phpy_yaml.set_phonon_info(ph)
         phpy_yaml_txt = str(phpy_yaml)
```

### Comparing `aiida-phonopy-1.0.0/src/aiida_phonopy/data/force_constants.py` & `aiida-phonopy-1.1.0/src/aiida_phonopy/data/force_constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 # -*- coding: utf-8 -*-
 """
 This module defines the class for force constants data.
 """
-
-from aiida.orm import ArrayData
 import numpy as np
 
 from .raw import RawData
 
 
-class ForceConstantsData(RawData, ArrayData):  # pylint: disable=too-many-ancestors
+class ForceConstantsData(RawData):  # pylint: disable=too-many-ancestors
     """
     This class provides the force constants data, along with the non-analytical constants
     (optional) and the structure information (unitcell, supercell, ...).
     """
 
     def __init__(
         self,
@@ -33,21 +31,22 @@
         kwargs['is_symmetry'] = is_symmetry
 
         super().__init__(**kwargs)
 
     def get_phonopy_instance(self, **kwargs):
         """Return a `phonopy.Phonopy` object with force and nac parameters (if set).
 
-        :param kwargs: compatible keys with the super method in `RawData`
+        :param kwargs: see :func:`aiida_phonopy.data.preprocess.PreProcessData.get_phonopy_instance`
+            * symmetrize_nac: whether or not to symmetrize the nac parameters
+                using point group symmetry; bool, defaults to self.is_symmetry
+            * factor_nac: factor for non-analytical corrections;
+                float, defaults to Hartree*Bohr
         """
         ph_instance = super().get_phonopy_instance(**kwargs)
 
-        if self.displacement_dataset is not None:
-            ph_instance.dataset = self.displacement_dataset
-
         if self.force_constants is not None:
             ph_instance.set_force_constants(self.force_constants)
 
         return ph_instance
 
     @property
     def force_constants(self):
```

### Comparing `aiida-phonopy-1.0.0/src/aiida_phonopy/data/preprocess.py` & `aiida-phonopy-1.1.0/src/aiida_phonopy/data/preprocess.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 This module defines the class for managing the frozen phonon structure.
 """
 
 import copy
+import json
 
 from aiida import orm
 import numpy as np
 
 from aiida_phonopy.calculations.functions.link_structures import phonopy_atoms_to_structure
 
 from .raw import RawData
@@ -43,33 +44,41 @@
 
         if self.__class__.__name__ == 'PreProcessData':
             self.set_displacements()
 
     @property
     def displacement_dataset(self):
         """Get the dispacement dataset in a readible format for phonopy."""
+        message = '`displacement_dataset` stored in the database will be deprecated in v2.0.0'
         try:
-            the_displacement_dataset = self.base.attributes.get('displacement_dataset')
+            import warnings
+            the_dataset = self.base.attributes.get('displacement_dataset')
+            warnings.warn(message, DeprecationWarning)
+            return the_dataset
         except AttributeError:
-            the_displacement_dataset = None
-        return the_displacement_dataset
+            filename = 'displacement_dataset.json'
+
+            if filename in self.base.repository.list_object_names():
+                with self.base.repository.open(filename, mode='rb') as handle:
+                    return json.load(handle)
+
+            return None
 
     @property
     def displacements(self):
         """Get the displacements to apply to the supercell.
 
         :returns: array with displacements; can be type-I or type-II (see :func:`phonopy.Phonopy.displacements`)
         """
-        try:
-            ph = self.get_phonopy_instance()
-            ph.dataset = self.displacement_dataset
+        # For the time being, it is important to keep this implementation for the subclasses in the package,
+        # otherwise a loop is generated (i.e. in the PhonopyData class, when setting the forces).
+        ph = super().get_phonopy_instance()
+        ph.dataset = self.displacement_dataset
 
-            return ph.displacements
-        except (AttributeError, TypeError):
-            return None
+        return ph.displacements
 
     def get_displacements(self):
         """Get the displacements to apply to the supercell."""
         return self.displacements
 
     def set_displacements(
         self,
@@ -103,15 +112,24 @@
                 random_seed=random_seed,
                 temperature=temperature,
                 cutoff_frequency=cutoff_frequency,
             )
         except ValueError as err:
             raise ValueError('one or more input types are not accepted') from err
 
-        self.base.attributes.set('displacement_dataset', copy.deepcopy(ph.dataset))
+        self._set_displacements(copy.deepcopy(ph.dataset))
+
+    def _set_displacements(self, value):
+        """Put in the repository the displacement dataset in json format."""
+        try:
+            serialized = json.dumps(value)
+        except TypeError:
+            serialized = json.dumps(_serialize(value))
+
+        self.base.repository.put_object_from_bytes(serialized.encode('utf-8'), 'displacement_dataset.json')
 
     def set_displacements_from_dataset(self, dataset):
         """Set displacements for frozen phonon calculation from a dataset.
         Useful if you want to set displacements from a previously random generated
         displacement dataset, or for setting dataset for self-consistent harmonic
         approximation.
 
@@ -131,42 +149,52 @@
             try:
                 ph.displacements = dataset
             except RuntimeError as err:
                 raise ValueError('non compatible format') from err
         else:
             raise ValueError('type not accepted')
 
-        self.base.attributes.set('displacement_dataset', copy.deepcopy(ph.dataset))
+        self._set_displacements(_serialize(copy.deepcopy(ph.dataset)))
+
+    def get_phonopy_instance(self, symmetrize_nac=None, factor_nac=None, **kwargs):
+        """Return a `phonopy.Phonopy` object with the current values.
+
+        :param symmetrize_nac: whether or not to symmetrize the nac parameters using point group symmetry.
+        :type symmetrize_nac: bool, defaults to self.is_symmetry
+        :param factor_nac: factor for non-analytical corrections
+        :type factor_nac: float,defaults to Hartree*Bohr
+        :param kwargs: for internal use to set the primitive cell
+        """
+        ph = super().get_phonopy_instance(symmetrize_nac, factor_nac, **kwargs)
+        if self.displacement_dataset is not None:
+            ph.dataset = self.displacement_dataset
+        return ph
 
     def get_supercells_with_displacements(self):
         """Get the supercells with displacements for frozen phonon calculation.
 
         :returns: dictionary with StructureData nodes (note: not stored), None if
             the displacement dataset has not been set
         """
+        # Here we distinguish the kind, but only for mapping purposes.
+        # This does not affect the number of displacements, since they
+        # have been set with the correct flag of not distinguishing kinds.
         ph = self.get_phonopy_instance(**{'distinguish': True})
-        try:
-            ph.dataset = self.displacement_dataset
 
-            supercells = ph.supercells_with_displacements
-            mapping = self.kinds_map
-            structures_dict = {}
-
-            # this will make the labels more nice to read - not really needed though
-            digits = len(str(len(supercells)))
-
-            for i, scell in enumerate(supercells):
-                # start from 1 - better choice for gathering forces
-                # MAYBE JUST NUMBERS???
-                label = f'supercell_{str(i + 1).zfill(digits)}'
-                structures_dict.update({label: phonopy_atoms_to_structure(scell, mapping)})
+        supercells = ph.supercells_with_displacements
+        mapping = self.kinds_map
+        structures_dict = {}
 
-            return structures_dict
-        except AttributeError:
-            return None
+        digits = len(str(len(supercells)))  # this will make the labels more nice to read
+
+        for i, scell in enumerate(supercells):  # start from 1 - better choice for gathering forces
+            label = f'supercell_{str(i + 1).zfill(digits)}'
+            structures_dict.update({label: phonopy_atoms_to_structure(scell, mapping)})
+
+        return structures_dict
 
     def generate_displacement_dataset(
         self,
         distance=0.01,
         is_plusminus='auto',
         is_diagonal=True,
         is_trigonal=False,
@@ -230,15 +258,15 @@
         :type symprec: orm.Float, optional
         :param is_symmetry: if using space group symmetry, defaults to True
         :type is_symmetry: orm.Bool, optional
         :param distinguish_kinds: if distinguish names of same specie by symmetry, defaults to True
         :type distinguish_kinds: orm.Bool, optional
         :return: PreProcessData node
         """
-        from aiida_phonopy.calculations.functions.data_utils import generate_preprocess_data_from_distance
+        from aiida_phonopy.calculations.functions.data_utils import generate_preprocess_data
 
         kwargs = {}
 
         kwargs['structure'] = structure
 
         if displacement_generator is not None:
             kwargs['displacement_generator'] = displacement_generator
@@ -254,8 +282,26 @@
 
         if is_symmetry is not None:
             kwargs['is_symmetry'] = is_symmetry
 
         if distinguish_kinds is not None:
             kwargs['distinguish_kinds'] = distinguish_kinds
 
-        return generate_preprocess_data_from_distance(**kwargs)
+        return generate_preprocess_data(**kwargs)
+
+
+def _serialize(data):
+    """Serialize the data for displacement dataset, in case it contains numpy.ndarray."""
+    serialized = copy.deepcopy(data)
+
+    try:
+        for key, value in data.items():
+            serialized[key] = _serialize(value)
+    except AttributeError:
+        if isinstance(serialized, list):
+            for i, value in enumerate(data):
+                serialized[i] = _serialize(value)
+        else:
+            if isinstance(data, np.ndarray):
+                return copy.deepcopy(data.tolist())
+
+    return serialized
```

### Comparing `aiida-phonopy-1.0.0/src/aiida_phonopy/data/raw.py` & `aiida-phonopy-1.1.0/src/aiida_phonopy/data/raw.py`

 * *Files 0% similar despite different names*

```diff
@@ -331,15 +331,15 @@
 
     def get_phonopy_instance(self, symmetrize_nac=None, factor_nac=None, **kwargs) -> Phonopy:
         """Return a `phonopy.Phonopy` object with the current values.
 
         :param symmetrize_nac: whether or not to symmetrize the nac parameters using point group symmetry.
         :type symmetrize_nac: bool, defaults to self.is_symmetry
         :param factor_nac: factor for non-analytical corrections
-        :type factor_nac: float,defaults to Hartree*Bohr
+        :type factor_nac: float, defaults to Hartree*Bohr
         :param kwargs: for internal use to set the primitive cell
         """
         from phonopy.structure.symmetry import symmetrize_borns_and_epsilon
         from phonopy.units import Bohr, Hartree
 
         distinguish = kwargs.pop('distinguish', self.distinguish_kinds)
         unitcell = self._get_phonopy_atoms_unitcell(distinguish)
@@ -456,28 +456,40 @@
         if the_dielectric.shape == (3, 3):
             self.base.attributes.set('dielectric', the_dielectric.tolist())
         else:
             raise ValueError('the array is not of the correct shape')
 
     @property
     def born_charges(self):
-        """Get the effective Born charges tensors in Cartesian coordinates."""
+        """Get the effective Born charges tensors in Cartesian coordinates.
+
+        ..note:
+            The indecis refers to:
+                1. Atomic index.
+                2. Polarization index.
+                3. Atomic displacement index.
+
+        :returns: numpy.ndarray, shape (num primitive cell atoms, 3, 3)
+        """
         try:
             value = self.get_array('born_charges')
         except (KeyError, AttributeError):
             value = None
         return value
 
     def set_born_charges(self, born_charges):
-        """Set the `infinity` dielectric tensor in Cartesian coordinates.
-
-        .. note: it is assumed that the tensors have been computed on the primitive cell.
+        """Set the Born effective charge tensors in Cartesian coordinates.
 
-        :param dielectric: (number of atoms in the primitive cell, 3, 3) shape array like
+        ..note:
+            The indecis refers to:
+                1. Atomic index.
+                2. Polarization index.
+                3. Atomic displacement index.
 
+        :param born_charges: (number of atoms in the primitive cell, 3, 3) shape array like
         :raises:
             * TypeError: if the format is not compatible or of the correct type
             * ValueError: if the format is not compatible or of the correct type
         """
         self._if_can_modify()
 
         if not isinstance(born_charges, (list, np.ndarray)):
```

### Comparing `aiida-phonopy-1.0.0/src/aiida_phonopy/parsers/base.py` & `aiida-phonopy-1.1.0/src/aiida_phonopy/parsers/base.py`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.0.0/src/aiida_phonopy/parsers/phonopy.py` & `aiida-phonopy-1.1.0/src/aiida_phonopy/parsers/phonopy.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,19 +156,23 @@
             # Check for job completion, indicating that phonopy exited without interruption, even if there was an error.
             parsed_data, logs = parse_stdout_(stdout)
         except ValueError:
             logs.critical.append(traceback.format_exc())
             exit_code_stdout = self.exit_codes.ERROR_UNEXPECTED_PARSER_EXCEPTION
 
         # If the stdout was incomplete, most likely the job was interrupted before it could cleanly finish, so the
-        # output files are most likely corrupt and cannot be restarted from
+        # output files are most likely corrupt and cannot be restarted
         if 'ERROR_OUTPUT_STDOUT_INCOMPLETE' in logs['error']:
             exit_code_stdout = self.exit_codes.ERROR_OUTPUT_STDOUT_INCOMPLETE
+
         if 'ERROR_BAD_INPUTS' in logs['error']:
-            exit_code_stdout = self.exit_codes.ERROR_BAD_INPUTS
+            parameters = _uppercase_dict(self.node.inputs.parameters.get_dict(), dict_name='parameters')
+            if 'FORCE_CONSTANTS' in parameters:
+                if str.upper(parameters['FORCE_CONSTANTS']) != 'WRITE':
+                    exit_code_stdout = self.exit_codes.ERROR_BAD_INPUTS
 
         return parsed_data, logs, exit_code_stdout
 
     def get_expected_filenames_keys(self):
         """Return the retrieve file keys (that map to the filenames outputs) depending on the tags in `parameters`."""
         retrieved_set = set()
         parameters = _uppercase_dict(self.node.inputs.parameters.get_dict(), dict_name='parameters')
@@ -178,31 +182,34 @@
             'mesh': {'MESH', 'MP', 'MESH_NUMBERS', 'MP_SHIFT', 'GAMMA_CENTER', 'WRITE_MESH'},
             'dos': {'DOS'},
             'pdos': {'PDOS'},
             'tprop': {'TPROP'},
             'tdisp': {'TDISP'},
             'tdispmat': {'TDISPMAT'},
             'qpoints': {'QPOINTS', 'WRITEDM'},
-            'fc': {'WRITE_FORCE_CONSTANTS'},
+            'fc': {'WRITE_FORCE_CONSTANTS', 'FORCE_CONSTANTS'},
             'mod': {'MODULATION'},
             'irreps': {'IRREPS', 'SHOW_IRREPS', 'LITTLE_COGROUP'}
         }
 
         for tag, value in parameters.items():
             for key_map, tag_map in maps.items():
                 if tag in tag_map:
                     # Usually these tags are set only if one needs them, i.e. to TRUE,
                     # thus this further control is actually pointless. Nevertheless,
-                    # we want to avoid anyway to raise error when in inputs one of these
+                    # we want to avoid to raise error when in inputs one of these
                     # tags is set to FALSE, meaning there will be no output to parse.
                     if tag.startswith(('WRITE', 'DOS', 'TPROP', 'TDISP', 'TDISPMAT')):
                         if value:
                             retrieved_set.add(key_map)
                     else:
-                        retrieved_set.add(key_map)
+                        if tag != 'FORCE_CONSTANTS':
+                            retrieved_set.add(key_map)
+                        elif str.upper(value) == 'WRITE':
+                            retrieved_set.add(key_map)
 
         # Double check on mesh. The writing tag must have priority.
         if 'WRITE_MESH' in parameters.keys():
             if not parameters['WRITE_MESH']:
                 retrieved_set.remove('mesh')
 
         return retrieved_set
```

### Comparing `aiida-phonopy-1.0.0/src/aiida_phonopy/parsers/raw_parsers/phonopy.py` & `aiida-phonopy-1.1.0/src/aiida_phonopy/parsers/raw_parsers/phonopy.py`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.0.0/src/aiida_phonopy/utils/mapping.py` & `aiida-phonopy-1.1.0/src/aiida_phonopy/utils/mapping.py`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.0.0/src/aiida_phonopy/utils/resources.py` & `aiida-phonopy-1.1.0/src/aiida_phonopy/utils/resources.py`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.0.0/src/aiida_phonopy/workflows/phonopy.py` & `aiida-phonopy-1.1.0/src/aiida_phonopy/workflows/phonopy.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,20 +125,20 @@
         (e.g. if your code plugin stores  the forces in `TrajectoryData`, extract them with a `calcfunction`).
         Expose each `ArrayData` choosing a **common prefix**, while as **suffix use
         _{number}**, with `{number}` referring to the correspective supercell label suffix (that you are supposed to
         keep track somewhere, e.g. in the label of the code calculation/workchain).
         Now you can gather all the information in one data noe, i.e. in a `PhonopyData` node.
         To do so, you can simple run:
 
-        ```self.ctx.preprocess_data.calcfunctions.generate_full_phonopy_data(**self.outputs.supercells_forces)```
+        ```self.ctx.preprocess_data.calcfunctions.generate_phonopy_data(**self.outputs.supercells_forces)```
 
         and then expose it as output in the `output_phonopy_data` namespace.
 
         * Alternatively: instead of exposing the supercell forces as outputs, you can directly gather all the forces
-        in a dictionary and run directly to the `generate_full_phonopy_data` method using this dictionary (always using
+        in a dictionary and run directly to the `generate_phonopy_data` method using this dictionary (always using
         the double *).
 
         See the implementation in aiidateam/aiida-common-workflows for an example.
 
     4. (optional) Run the non-analytical constants on the primitive cell.
 
         Non-analytical constants should be run for polar insulators. These require usually a linear response code
@@ -148,15 +148,15 @@
         ```self.ctx.preprocess_data.calcfunctions.get_primitive_cell()```
 
         If you compute also these, collect the dielectric tensor and the effectic born charges in an ArrayData,
         with the arraynames `dielectric` and `born_charges` (in Cartesian coordinates!).
         Then, gather all the information of nac and forces in a unique `PhonopyData` via:
 
         ```
-        self.ctx.preprocess_data.calcfunctions.generate_full_phonopy_data(
+        self.ctx.preprocess_data.calcfunctions.generate_phonopy_data(
             nac_parameters=nac_paramters,
             **self.outputs.supercells_forces
             )
         ```
 
         and expose the output.
```

### Comparing `aiida-phonopy-1.0.0/PKG-INFO` & `aiida-phonopy-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: aiida-phonopy
-Version: 1.0.0
+Version: 1.1.0
 Summary: The official AiiDA plugin for Phonopy
-Keywords: aiida,workflows
+Keywords: aiida,phonopy,workflows
 Author-email: Lorenzo Bastonero <bastonero.lorenzo@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AiiDA
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
-Requires-Dist: aiida-core>=2.0.0
+Requires-Dist: aiida-core>=2.0.0,<3.0.0
 Requires-Dist: phonopy>=2.14,<3.0.0
 Requires-Dist: Sphinx ; extra == "docs"
 Requires-Dist: docutils ; extra == "docs"
 Requires-Dist: sphinx-copybutton~=0.3.0 ; extra == "docs"
 Requires-Dist: sphinx-book-theme~=0.1.0 ; extra == "docs"
 Requires-Dist: sphinx-click~=2.7.1 ; extra == "docs"
 Requires-Dist: pre-commit~=2.17 ; extra == "pre-commit"
-Requires-Dist: pylint==2.13.7 ; extra == "pre-commit"
+Requires-Dist: pylint==2.17.2 ; extra == "pre-commit"
 Requires-Dist: pylint-aiida~=0.1.1 ; extra == "pre-commit"
+Requires-Dist: toml ; extra == "pre-commit"
 Requires-Dist: pgtest~=1.3 ; extra == "tests"
-Requires-Dist: pytest~=6.2 ; extra == "tests"
-Requires-Dist: pytest-regressions~=1.0 ; extra == "tests"
+Requires-Dist: pytest~=6.0 ; extra == "tests"
+Requires-Dist: pytest-regressions~=2.3 ; extra == "tests"
 Project-URL: Source, https://github.com/aiida-phonopy/aiida-phonopy
 Provides-Extra: docs
 Provides-Extra: pre-commit
 Provides-Extra: tests
 
 # `aiida-phonopy`
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
```

