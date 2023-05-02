# Comparing `tmp/pypotlib-0.0.6.tar.gz` & `tmp/pypotlib-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypotlib-0.0.6.tar", last modified: Sat Apr 22 21:52:24 2023, max compression
+gzip compressed data, was "pypotlib-0.0.7.tar", last modified: Tue May  2 15:44:39 2023, max compression
```

## Comparing `pypotlib-0.0.6.tar` & `pypotlib-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,34 @@
--rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 pypotlib-0.0.6/.clang-format
--rw-r--r--   0        0        0      446 1970-01-01 00:00:00.000000 pypotlib-0.0.6/.github/workflows/build_test.yml
--rw-r--r--   0        0        0     2486 1970-01-01 00:00:00.000000 pypotlib-0.0.6/.github/workflows/build_wheels.yml
--rw-r--r--   0        0        0     5219 1970-01-01 00:00:00.000000 pypotlib-0.0.6/.gitignore
--rw-r--r--   0        0        0      547 1970-01-01 00:00:00.000000 pypotlib-0.0.6/CODEOWNERS
--rw-r--r--   0        0        0     5488 1970-01-01 00:00:00.000000 pypotlib-0.0.6/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1117 1970-01-01 00:00:00.000000 pypotlib-0.0.6/LICENSE
--rw-r--r--   0        0        0     2622 1970-01-01 00:00:00.000000 pypotlib-0.0.6/README.md
--rw-r--r--   0        0        0      326 1970-01-01 00:00:00.000000 pypotlib-0.0.6/environment.yml
--rw-r--r--   0        0        0     1785 1970-01-01 00:00:00.000000 pypotlib-0.0.6/meson.build
--rw-r--r--   0        0        0      223 1970-01-01 00:00:00.000000 pypotlib-0.0.6/pyb11_srcs/CuH2/py_cuh2pot.cc
--rw-r--r--   0        0        0     1223 1970-01-01 00:00:00.000000 pypotlib-0.0.6/pyb11_srcs/CuH2/py_cuh2pot.hpp
--rw-r--r--   0        0        0      211 1970-01-01 00:00:00.000000 pypotlib-0.0.6/pyb11_srcs/LennardJones/py_ljpot.cc
--rw-r--r--   0        0        0     1219 1970-01-01 00:00:00.000000 pypotlib-0.0.6/pyb11_srcs/LennardJones/py_ljpot.hpp
--rw-r--r--   0        0        0      231 1970-01-01 00:00:00.000000 pypotlib-0.0.6/pyb11_srcs/py_potential.cc
--rw-r--r--   0        0        0     1178 1970-01-01 00:00:00.000000 pypotlib-0.0.6/pyb11_srcs/py_potential.hpp
--rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 pypotlib-0.0.6/pyb11_srcs/py_pottypes.cc
--rw-r--r--   0        0        0      151 1970-01-01 00:00:00.000000 pypotlib-0.0.6/pyb11_srcs/py_wrapper.cc
--rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 pypotlib-0.0.6/pyb11_srcs/py_wrapper.hpp
--rw-r--r--   0        0        0       26 1970-01-01 00:00:00.000000 pypotlib-0.0.6/pypotlib/__init__.py
--rw-r--r--   0        0        0      944 1970-01-01 00:00:00.000000 pypotlib-0.0.6/pypotlib/ase_adapters.py
--rw-r--r--   0        0        0     1439 1970-01-01 00:00:00.000000 pypotlib-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      112 1970-01-01 00:00:00.000000 pypotlib-0.0.6/subprojects/potlib.wrap
--rw-r--r--   0        0        0     3040 1970-01-01 00:00:00.000000 pypotlib-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 pypotlib-0.0.7/.clang-format
+-rw-r--r--   0        0        0      446 1970-01-01 00:00:00.000000 pypotlib-0.0.7/.github/workflows/build_test.yml
+-rw-r--r--   0        0        0     2486 1970-01-01 00:00:00.000000 pypotlib-0.0.7/.github/workflows/build_wheels.yml
+-rw-r--r--   0        0        0     5227 1970-01-01 00:00:00.000000 pypotlib-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1242 1970-01-01 00:00:00.000000 pypotlib-0.0.7/.nb/aseCuH2slab.md
+-rw-r--r--   0        0        0     6534 1970-01-01 00:00:00.000000 pypotlib-0.0.7/.nb/data/cuh2/init.con
+-rw-r--r--   0        0        0    16761 1970-01-01 00:00:00.000000 pypotlib-0.0.7/.nb/data/cuh2/init_shift.con
+-rw-r--r--   0        0        0     6534 1970-01-01 00:00:00.000000 pypotlib-0.0.7/.nb/data/cuh2/min1_0Cu.con
+-rw-r--r--   0        0        0    16761 1970-01-01 00:00:00.000000 pypotlib-0.0.7/.nb/data/cuh2/min1_0Cu_shift.con
+-rw-r--r--   0        0        0     6534 1970-01-01 00:00:00.000000 pypotlib-0.0.7/.nb/data/cuh2/min2_0Cu.con
+-rw-r--r--   0        0        0    16761 1970-01-01 00:00:00.000000 pypotlib-0.0.7/.nb/data/cuh2/min2_0Cu_shift.con
+-rw-r--r--   0        0        0      547 1970-01-01 00:00:00.000000 pypotlib-0.0.7/CODEOWNERS
+-rw-r--r--   0        0        0     5488 1970-01-01 00:00:00.000000 pypotlib-0.0.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1117 1970-01-01 00:00:00.000000 pypotlib-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2978 1970-01-01 00:00:00.000000 pypotlib-0.0.7/README.md
+-rw-r--r--   0        0        0      358 1970-01-01 00:00:00.000000 pypotlib-0.0.7/environment.yml
+-rw-r--r--   0        0        0     1929 1970-01-01 00:00:00.000000 pypotlib-0.0.7/meson.build
+-rw-r--r--   0        0        0      223 1970-01-01 00:00:00.000000 pypotlib-0.0.7/pyb11_srcs/CuH2/py_cuh2pot.cc
+-rw-r--r--   0        0        0     1223 1970-01-01 00:00:00.000000 pypotlib-0.0.7/pyb11_srcs/CuH2/py_cuh2pot.hpp
+-rw-r--r--   0        0        0      211 1970-01-01 00:00:00.000000 pypotlib-0.0.7/pyb11_srcs/LennardJones/py_ljpot.cc
+-rw-r--r--   0        0        0     1219 1970-01-01 00:00:00.000000 pypotlib-0.0.7/pyb11_srcs/LennardJones/py_ljpot.hpp
+-rw-r--r--   0        0        0      231 1970-01-01 00:00:00.000000 pypotlib-0.0.7/pyb11_srcs/py_potential.cc
+-rw-r--r--   0        0        0     1178 1970-01-01 00:00:00.000000 pypotlib-0.0.7/pyb11_srcs/py_potential.hpp
+-rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 pypotlib-0.0.7/pyb11_srcs/py_pottypes.cc
+-rw-r--r--   0        0        0      151 1970-01-01 00:00:00.000000 pypotlib-0.0.7/pyb11_srcs/py_wrapper.cc
+-rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 pypotlib-0.0.7/pyb11_srcs/py_wrapper.hpp
+-rw-r--r--   0        0        0       26 1970-01-01 00:00:00.000000 pypotlib-0.0.7/pypotlib/__init__.py
+-rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 pypotlib-0.0.7/pypotlib/ase_adapters.py
+-rw-r--r--   0        0        0      350 1970-01-01 00:00:00.000000 pypotlib-0.0.7/pypotlib/aux.py
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:00.000000 pypotlib-0.0.7/pypotlib/systems/__init__.py
+-rw-r--r--   0        0        0     3488 1970-01-01 00:00:00.000000 pypotlib-0.0.7/pypotlib/systems/cu_slab_h2.py
+-rw-r--r--   0        0        0     1439 1970-01-01 00:00:00.000000 pypotlib-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      112 1970-01-01 00:00:00.000000 pypotlib-0.0.7/subprojects/potlib.wrap
+-rw-r--r--   0        0        0     3396 1970-01-01 00:00:00.000000 pypotlib-0.0.7/PKG-INFO
```

### Comparing `pypotlib-0.0.6/.clang-format` & `pypotlib-0.0.7/.clang-format`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.6/.github/workflows/build_wheels.yml` & `pypotlib-0.0.7/.github/workflows/build_wheels.yml`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.6/.gitignore` & `pypotlib-0.0.7/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Added
 subprojects/*
 !subprojects/potlib.wrap
 compile_commands.json
 pdm.lock
 wheelhouse/
+*.ipynb
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
```

### Comparing `pypotlib-0.0.6/CODEOWNERS` & `pypotlib-0.0.7/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.6/CODE_OF_CONDUCT.md` & `pypotlib-0.0.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.6/LICENSE` & `pypotlib-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.6/README.md` & `pypotlib-0.0.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,29 @@
-# `pypotlib` [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md) ![Builds](https://github.com/TheochemUI/pypotlib/actions/workflows/build_test.yml/badge.svg) ![Wheels](https://github.com/TheochemUI/pypotlib/actions/workflows/build_wheels.yml/badge.svg)
+# `pypotlib` [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](https://github.com/TheochemUI/pypotlib/blob/main/code_of_conduct.md) ![Builds](https://github.com/TheochemUI/pypotlib/actions/workflows/build_test.yml/badge.svg) ![Wheels](https://github.com/TheochemUI/pypotlib/actions/workflows/build_wheels.yml/badge.svg)
 
 Python bindings and ASE adapters for `potlib`.
 
 ## Details
 
 The library consists of thin wrappers to `potlib` under `cpot` and a
 `PyPotLibCalc` class which is an `ase` calculator under `ase_adapters`.
 
-## Builds
+## Installation
 
-### Local usage
+This is [on PyPI](https://pypi.org/project/pypotlib), with wheels, so usage is simply:
+
+``` bash
+pip install pypotlib
+```
+
+Users are advised to not try to build from source, since the underlying `potlib`
+code includes `fortran` and `cpp` dependencies which can be slightly tricky to
+work with.
+
+### Local Development
 
 The easiest way is to use the environment file, compatible with `conda`,
 `mamba`, `micromamba` etc.
 
 ```bash
 mamba env create -f environment.yml
 mamba activate rgpotpy
```

### Comparing `pypotlib-0.0.6/meson.build` & `pypotlib-0.0.7/meson.build`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 project('pypotlib', 'cpp',
-       version: '0.0.6',
+       version: '0.0.7',
   default_options : ['warning_level=2', 'cpp_std=c++17'])
 # IMPORTANT!! warning_level=3 passes -fimplicit-none
 # Many of the older Fortran codes need implicit typing
 
 host_system = host_machine.system()
 
 # Add C++ compiler options
@@ -62,11 +62,20 @@
   pure: false, # install next to compiled extension
   subdir: 'pypotlib'
 )
 
 # Adapters
 py.install_sources([
     'pypotlib/ase_adapters.py',
+    'pypotlib/aux.py',
   ],
   pure: false,
   subdir: 'pypotlib'
 )
+
+# Systems
+py.install_sources([
+    'pypotlib/systems/cu_slab_h2.py',
+  ],
+  pure: false,
+  subdir: 'pypotlib/systems'
+)
```

### Comparing `pypotlib-0.0.6/pyb11_srcs/CuH2/py_cuh2pot.hpp` & `pypotlib-0.0.7/pyb11_srcs/CuH2/py_cuh2pot.hpp`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.6/pyb11_srcs/LennardJones/py_ljpot.hpp` & `pypotlib-0.0.7/pyb11_srcs/LennardJones/py_ljpot.hpp`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.6/pyb11_srcs/py_potential.hpp` & `pypotlib-0.0.7/pyb11_srcs/py_potential.hpp`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.6/pyb11_srcs/py_wrapper.hpp` & `pypotlib-0.0.7/pyb11_srcs/py_wrapper.hpp`

 * *Files identical despite different names*

### Comparing `pypotlib-0.0.6/pypotlib/ase_adapters.py` & `pypotlib-0.0.7/pypotlib/ase_adapters.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,12 +17,12 @@
         self, atoms=None, properties=["energy"], system_changes=all_changes
     ):
         Calculator.calculate(self, atoms, properties, system_changes)
         positions = atoms.get_positions()
         atmtypes = atoms.get_atomic_numbers()
         box = atoms.get_cell()
         if np.all(box == np.zeros(3)):
-            warnings.warn("Box is zero, setting to rectangular 100, 100, 100")
+            warnings.warn("Box is zero, setting to diagonal(100, 100, 100)")
             box = np.eye(3) * 100
         energy, forces = self.cpot(positions, atmtypes, box)
         self.results["energy"] = energy
         self.results["forces"] = forces
```

### Comparing `pypotlib-0.0.6/pyproject.toml` & `pypotlib-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.pdm]
 
 [project]
 name = "pypotlib"
-version = "0.0.6"
+version = "0.0.7"
 description = "Python bindings and ASE adapters for potlib"
 authors = [
     {name = "Rohit Goswami", email = "rog32@hi.is"},
 ]
 # These are only if ase integration is requested, consider a group
 dependencies = [
     "numpy>=1.24.2",
```

### Comparing `pypotlib-0.0.6/PKG-INFO` & `pypotlib-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,42 @@
 Metadata-Version: 2.1
 Name: pypotlib
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python bindings and ASE adapters for potlib
 Author-Email: Rohit Goswami <rog32@hi.is>
 License: MIT
 Project-URL: Source code, https://github.com/TheochemUI/pypotlib
 Project-URL: Bug tracker, https://github.com/TheochemUI/pypotlib/issues
 Requires-Python: >=3.10
 Requires-Dist: numpy>=1.24.2
 Requires-Dist: ase>=3.22.1
 Description-Content-Type: text/markdown
 
-# `pypotlib` [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md) ![Builds](https://github.com/TheochemUI/pypotlib/actions/workflows/build_test.yml/badge.svg) ![Wheels](https://github.com/TheochemUI/pypotlib/actions/workflows/build_wheels.yml/badge.svg)
+# `pypotlib` [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](https://github.com/TheochemUI/pypotlib/blob/main/code_of_conduct.md) ![Builds](https://github.com/TheochemUI/pypotlib/actions/workflows/build_test.yml/badge.svg) ![Wheels](https://github.com/TheochemUI/pypotlib/actions/workflows/build_wheels.yml/badge.svg)
 
 Python bindings and ASE adapters for `potlib`.
 
 ## Details
 
 The library consists of thin wrappers to `potlib` under `cpot` and a
 `PyPotLibCalc` class which is an `ase` calculator under `ase_adapters`.
 
-## Builds
+## Installation
 
-### Local usage
+This is [on PyPI](https://pypi.org/project/pypotlib), with wheels, so usage is simply:
+
+``` bash
+pip install pypotlib
+```
+
+Users are advised to not try to build from source, since the underlying `potlib`
+code includes `fortran` and `cpp` dependencies which can be slightly tricky to
+work with.
+
+### Local Development
 
 The easiest way is to use the environment file, compatible with `conda`,
 `mamba`, `micromamba` etc.
 
 ```bash
 mamba env create -f environment.yml
 mamba activate rgpotpy
```

