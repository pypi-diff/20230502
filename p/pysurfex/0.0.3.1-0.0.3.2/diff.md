# Comparing `tmp/pysurfex-0.0.3.1.tar.gz` & `tmp/pysurfex-0.0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysurfex-0.0.3.1.tar", max compression
+gzip compressed data, was "pysurfex-0.0.3.2.tar", max compression
```

## Comparing `pysurfex-0.0.3.1.tar` & `pysurfex-0.0.3.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     2532 2023-04-26 06:09:39.281463 pysurfex-0.0.3.1/README.rst
--rw-r--r--   0        0        0     5233 2023-04-26 06:09:39.289463 pysurfex-0.0.3.1/pyproject.toml
--rw-r--r--   0        0        0      142 2023-04-26 06:09:39.289463 pysurfex-0.0.3.1/pysurfex/__init__.py
--rw-r--r--   0        0        0    30965 2023-04-26 06:09:39.289463 pysurfex-0.0.3.1/pysurfex/binary_input.py
--rw-r--r--   0        0        0    18837 2023-04-26 06:09:39.289463 pysurfex-0.0.3.1/pysurfex/bufr.py
--rw-r--r--   0        0        0    10460 2023-04-26 06:09:39.289463 pysurfex-0.0.3.1/pysurfex/cache.py
--rw-r--r--   0        0        0    19335 2023-04-26 06:09:39.289463 pysurfex-0.0.3.1/pysurfex/cfg/config.yml
--rw-r--r--   0        0        0     8985 2023-04-26 06:09:39.289463 pysurfex-0.0.3.1/pysurfex/cfg/config_exp_surfex.toml
--rw-r--r--   0        0        0      135 2023-04-26 06:09:39.289463 pysurfex-0.0.3.1/pysurfex/cfg/default_thredds.cfg
--rw-r--r--   0        0        0     5253 2023-04-26 06:09:39.289463 pysurfex-0.0.3.1/pysurfex/cfg/first_guess.yml
--rw-r--r--   0        0        0      192 2023-04-26 06:09:39.289463 pysurfex-0.0.3.1/pysurfex/cfg/qc_codes.json
--rw-r--r--   0        0        0      370 2023-04-26 06:09:39.289463 pysurfex-0.0.3.1/pysurfex/cfg/user.yml
--rw-r--r--   0        0        0    62279 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/cli.py
--rw-r--r--   0        0        0    61762 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/cmd_parsing.py
--rw-r--r--   0        0        0    32663 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/configuration.py
--rw-r--r--   0        0        0     1291 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/datetime_utils.py
--rw-r--r--   0        0        0     8511 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/ecoclimap.py
--rw-r--r--   0        0        0     3891 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/fa.py
--rw-r--r--   0        0        0    58096 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/file.py
--rw-r--r--   0        0        0    35668 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/forcing.py
--rw-r--r--   0        0        0    33675 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/geo.py
--rw-r--r--   0        0        0    22471 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/grib.py
--rw-r--r--   0        0        0    14928 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/input_methods.py
--rw-r--r--   0        0        0    18924 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/interpolation.py
--rw-r--r--   0        0        0   100050 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/namelist.py
--rw-r--r--   0        0        0    34770 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/netcdf.py
--rw-r--r--   0        0        0    37729 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/obs.py
--rw-r--r--   0        0        0     4483 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/observation.py
--rw-r--r--   0        0        0    12016 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/obsmon.py
--rw-r--r--   0        0        0     6415 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/obsoul.py
--rw-r--r--   0        0        0    16227 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/platform.py
--rw-r--r--   0        0        0       20 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/plot.py
--rw-r--r--   0        0        0    17168 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/read.py
--rw-r--r--   0        0        0    11682 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/run.py
--rw-r--r--   0        0        0     2254 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/settings/assimilation.json
--rw-r--r--   0        0        0        0 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/settings/filetype.json
--rw-r--r--   0        0        0     1075 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/settings/forecast.json
--rw-r--r--   0        0        0     1305 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/settings/pgd.json
--rw-r--r--   0        0        0      952 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/settings/prep.json
--rw-r--r--   0        0        0     3499 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/timeseries.py
--rw-r--r--   0        0        0    67688 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/titan.py
--rw-r--r--   0        0        0     3463 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/util.py
--rw-r--r--   0        0        0    19977 2023-04-26 06:09:39.293463 pysurfex-0.0.3.1/pysurfex/variable.py
--rw-r--r--   0        0        0     3868 1970-01-01 00:00:00.000000 pysurfex-0.0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     3318 2023-05-02 18:57:12.959139 pysurfex-0.0.3.2/README.rst
+-rw-r--r--   0        0        0     5202 2023-05-02 18:57:12.963139 pysurfex-0.0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      142 2023-05-02 18:57:12.963139 pysurfex-0.0.3.2/pysurfex/__init__.py
+-rw-r--r--   0        0        0    30965 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/binary_input.py
+-rw-r--r--   0        0        0    18837 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/bufr.py
+-rw-r--r--   0        0        0    10460 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/cache.py
+-rw-r--r--   0        0        0    19335 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/cfg/config.yml
+-rw-r--r--   0        0        0     8985 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/cfg/config_exp_surfex.toml
+-rw-r--r--   0        0        0      135 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/cfg/default_thredds.cfg
+-rw-r--r--   0        0        0     5253 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/cfg/first_guess.yml
+-rw-r--r--   0        0        0      192 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/cfg/qc_codes.json
+-rw-r--r--   0        0        0      370 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/cfg/user.yml
+-rw-r--r--   0        0        0    62389 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/cli.py
+-rw-r--r--   0        0        0    62271 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/cmd_parsing.py
+-rw-r--r--   0        0        0    32663 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/configuration.py
+-rw-r--r--   0        0        0     1291 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/datetime_utils.py
+-rw-r--r--   0        0        0     8511 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/ecoclimap.py
+-rw-r--r--   0        0        0     3891 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/fa.py
+-rw-r--r--   0        0        0    58096 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/file.py
+-rw-r--r--   0        0        0    35668 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/forcing.py
+-rw-r--r--   0        0        0    33675 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/geo.py
+-rw-r--r--   0        0        0    22471 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/grib.py
+-rw-r--r--   0        0        0    14928 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/input_methods.py
+-rw-r--r--   0        0        0    18924 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/interpolation.py
+-rw-r--r--   0        0        0   100050 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/namelist.py
+-rw-r--r--   0        0        0    34770 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/netcdf.py
+-rw-r--r--   0        0        0    37729 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/obs.py
+-rw-r--r--   0        0        0     4483 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/observation.py
+-rw-r--r--   0        0        0    12016 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/obsmon.py
+-rw-r--r--   0        0        0     6415 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/obsoul.py
+-rw-r--r--   0        0        0    16227 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/platform.py
+-rw-r--r--   0        0        0       20 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/plot.py
+-rw-r--r--   0        0        0    17168 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/read.py
+-rw-r--r--   0        0        0    11682 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/run.py
+-rw-r--r--   0        0        0     2254 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/settings/assimilation.json
+-rw-r--r--   0        0        0        0 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/settings/filetype.json
+-rw-r--r--   0        0        0     1075 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/settings/forecast.json
+-rw-r--r--   0        0        0     1305 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/settings/pgd.json
+-rw-r--r--   0        0        0      952 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/settings/prep.json
+-rw-r--r--   0        0        0     3499 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/timeseries.py
+-rw-r--r--   0        0        0    67688 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/titan.py
+-rw-r--r--   0        0        0     3463 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/util.py
+-rw-r--r--   0        0        0    19977 2023-05-02 18:57:12.967139 pysurfex-0.0.3.2/pysurfex/variable.py
+-rw-r--r--   0        0        0     4606 1970-01-01 00:00:00.000000 pysurfex-0.0.3.2/PKG-INFO
```

### Comparing `pysurfex-0.0.3.1/README.rst` & `pysurfex-0.0.3.2/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,75 +1,79 @@
-.. _README:
 
 .. image:: https://coveralls.io/repos/github/metno/pysurfex/badge.svg?branch=master
 
-https://coveralls.io/github/metno/pysurfex
 
 Python API to SURFEX (pysurfex)
 =======================================================
 
 An API in python to the external surface model SURFEX.
     - Prepare input and namelists to a SURFEX binary
     - Create atmospheric forcing for offline SURFEX runs
     - Read SURFEX output
-    - A scheduler setup to run offline SURFEX experiments
     - Quality control of observations with titanlib
     - Optimal interpolation with gridpp
     - Monitor the observations usage
 
 See online documentation in https://metno.github.io/pysurfex/
 
 Installation of pregenerated packages from pypi (pip)
 ---------------------------------------------------------
 
+All releases will trigger an autmomatic pre-built package on pypi which can be installed by pip
+
 .. code-block:: bash
 
-    pip3 install pysurfex
+  pip3 install pysurfex
 
 User installation:
 
 .. code-block:: bash
 
-    pip3 install pysurfex --user
+  pip3 install pysurfex --user
+
 
+Run pysurfex from pre-built container
+-------------------------------------------
 
+Releases also trigger an update of the pysurfex container in the github container registry. Below is an example to run pgd without any arguments.
+
+.. code-block:: bash
+
+  podman run -it ghcr.io/metno/pysurfex:latest poetry run pgd
 
 
 Installation on debian based Linux system
 --------------------------------------------
 
 Install the required pacakges (some might be obsolete if the pip packages contain the needed depedencies):
 
 .. code-block:: bash
 
   sudo apt-get update
-  sudo apt-get install -y libudunits2-dev libproj-dev libeccodes0 libeccodes-dev libnetcdf-dev netcdf-bin
+  sudo apt-get install -y libudunits2-dev libproj-dev libeccodes0 libeccodes-dev libnetcdf-dev netcdf-bin ca-certificates
 
 The following depencies are needed. Install the non-standard ones e.g. with pip or your system installation system.
 
 General dependencies (from pypi)
 ---------------------------------
 
 .. code-block:: bash
 
   numpy
-  netCDF4
-  cfunits
   pyproj
   pyyaml
   toml
-  netCDF4
   f90nml
-  requests
 
 To read NetCDF files:
 
 .. code-block:: bash
 
   NetCDF4
+  cfunits
 
 To read grib files:
 
 .. code-block:: bash
 
   eccodes
 
@@ -88,44 +92,66 @@
   requests
 
 For Quality control of observations
 
 .. code-block:: bash
 
   titanlib
-  db-sqlite3
 
 For optimal interpolation and observation operators
 
 .. code-block:: bash
 
   gridpp
 
 For testing:
 
 .. code-block:: bash
 
   pytest
 
-Download the source code, then install ``pysurfex`` by executing the following inside the extracted
-folder:
 
 Install pysurfex
 -------------------------------------------
+
+Download the source code, then install ``pysurfex`` by executing the following inside the extracted
+folder:
+
 .. code-block:: bash
 
   poetry install
 
-Create documentation
----------------------------------------------
+
+This will install ``pysurfex`` in a poetry environment and this environment can be activated interactively by:
 
 .. code-block:: bash
 
-  cd docs
-  # Create html documentation
-  make html
+  poetry shell
+
+or
+
+Run pysurfex client applications
+-------------------------------------------
+
+.. code-block:: bash
+
+  poetry run [command]
+  # e.g.
+  poetry run python # will run python inside the pysurfex poetry environment
+
+
+Run pysurfex client applications
+-------------------------------------------
+.. code-block:: python
+
+  import sys
+  from pysurfex.cli import parse_args_surfex_binary, run_surfex_binary
+
+  argv = sys.argv[1:]
+  kwargs = parse_args_surfex_binary(argv, "pgd")
+  run_surfex_binary("pgd", **kwargs)
 
 
 Examples
 -----------------------
 
 See https://metno.github.io/pysurfex/#examples
```

### Comparing `pysurfex-0.0.3.1/pyproject.toml` & `pysurfex-0.0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
     name = "pysurfex"
-    version = "0.0.3.1"
+    version = "0.0.3.2"
     description = "Python API to SURFEX"
     authors = ["Trygve Aspelien"]
     license = "MIT"
     readme = "README.rst"
     repository = "https://github.com/metno/pysurfex"
     documentation = "https://metno.github.io/pysurfex/"
 
@@ -40,26 +40,25 @@
 [build-system]
     build-backend = "poetry.core.masonry.api"
     requires = ["poetry-core > 1.2.0"]
 
 [tool.poetry.dependencies]
     python = "^3.8"
     dateutils = "^0.6.12"
-    fastjsonschema = "2.16.2"
     f90nml = "^1.4.3"
     humanize = "^3.14.0"
     numexpr = "^2.8.4"
     numpy = "^1.22.4"
     pandas = "^1.4.0"
     pyproj = "^3.3.0"
     pyyaml = "^6.0"
     toml = "^0.10.2"
 
 #[tool.poetry.group.formats.dependencies]
-    netcdf4 = "^1.6.3"
+    netcdf4 = "1.5.7"
     cfunits = "^3.3.5"
     eccodes = "^1.5.1"
 
 #[tool.poetry.group.points.dependencies]
     requests = "^2.28.2"
     gridpp = "^0.6.0"
     titanlib = "^0.3.3"
```

### Comparing `pysurfex-0.0.3.1/pysurfex/binary_input.py` & `pysurfex-0.0.3.2/pysurfex/binary_input.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.1/pysurfex/bufr.py` & `pysurfex-0.0.3.2/pysurfex/bufr.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.1/pysurfex/cache.py` & `pysurfex-0.0.3.2/pysurfex/cache.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.1/pysurfex/cfg/config.yml` & `pysurfex-0.0.3.2/pysurfex/cfg/config.yml`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.1/pysurfex/cfg/config_exp_surfex.toml` & `pysurfex-0.0.3.2/pysurfex/cfg/config_exp_surfex.toml`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.1/pysurfex/cfg/first_guess.yml` & `pysurfex-0.0.3.2/pysurfex/cfg/first_guess.yml`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.1/pysurfex/cli.py` & `pysurfex-0.0.3.2/pysurfex/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     SodaInputData,
 )
 from .cache import Cache
 from .cmd_parsing import (
     parse_args_bufr2json,
     parse_args_create_forcing,
     parse_args_create_namelist,
+    parse_args_dump_environ,
     parse_args_first_guess_for_oi,
     parse_args_gridpp,
     parse_args_hm2pysurfex,
     parse_args_lsm_file_assim,
     parse_args_masterodb,
     parse_args_merge_qc_data,
     parse_args_modify_forcing,
@@ -1540,15 +1541,17 @@
     """Command line interface.
 
     Args:
         argv(list, optional): Arguments. Defaults to None.
     """
     if argv is None:
         argv = sys.argv[1:]
-    with open("rte.json", mode="w", encoding="utf-8") as file_handler:
+    kwargs = parse_args_dump_environ(argv)
+    outputfile = kwargs["outputfile"]
+    with open(outputfile, mode="w", encoding="utf-8") as file_handler:
         json.dump(os.environ.copy(), file_handler)
 
 
 def first_guess_for_oi(argv=None):
     """Command line interface.
 
     Args:
```

### Comparing `pysurfex-0.0.3.1/pysurfex/cmd_parsing.py` & `pysurfex-0.0.3.2/pysurfex/cmd_parsing.py`

 * *Files 0% similar despite different names*

```diff
@@ -500,14 +500,36 @@
     args = parser.parse_args(argv)
     kwargs = {}
     for arg in vars(args):
         kwargs.update({arg: getattr(args, arg)})
     return kwargs
 
 
+def parse_args_dump_environ(argv):
+    """Parse arguments for dum environ.
+
+    Args:
+        argv (list): List with arguments.
+
+    Returns:
+        dict: Parsed arguments.
+
+    """
+    parser = ArgumentParser(description="Dump environment")
+    parser.add_argument(
+        "-o", "--outputfile", type=str, default="rte.json", help="Default output file"
+    )
+
+    args = parser.parse_args(argv)
+    kwargs = {}
+    for arg in vars(args):
+        kwargs.update({arg: getattr(args, arg)})
+    return kwargs
+
+
 def parse_args_first_guess_for_oi(argv):
     """Parse arguments for firstguess4oi.
 
     Args:
         argv (list): List with arguments.
 
     Returns:
```

### Comparing `pysurfex-0.0.3.1/pysurfex/configuration.py` & `pysurfex-0.0.3.2/pysurfex/configuration.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.1/pysurfex/datetime_utils.py` & `pysurfex-0.0.3.2/pysurfex/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.1/pysurfex/ecoclimap.py` & `pysurfex-0.0.3.2/pysurfex/ecoclimap.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.1/pysurfex/fa.py` & `pysurfex-0.0.3.2/pysurfex/fa.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.1/pysurfex/file.py` & `pysurfex-0.0.3.2/pysurfex/file.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.1/pysurfex/forcing.py` & `pysurfex-0.0.3.2/pysurfex/forcing.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.1/pysurfex/geo.py` & `pysurfex-0.0.3.2/pysurfex/geo.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.1/pysurfex/grib.py` & `pysurfex-0.0.3.2/pysurfex/grib.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.1/pysurfex/input_methods.py` & `pysurfex-0.0.3.2/pysurfex/input_methods.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.1/pysurfex/interpolation.py` & `pysurfex-0.0.3.2/pysurfex/interpolation.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.1/pysurfex/namelist.py` & `pysurfex-0.0.3.2/pysurfex/namelist.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.1/pysurfex/netcdf.py` & `pysurfex-0.0.3.2/pysurfex/netcdf.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.1/pysurfex/obs.py` & `pysurfex-0.0.3.2/pysurfex/obs.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.1/pysurfex/observation.py` & `pysurfex-0.0.3.2/pysurfex/observation.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.1/pysurfex/obsmon.py` & `pysurfex-0.0.3.2/pysurfex/obsmon.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.1/pysurfex/obsoul.py` & `pysurfex-0.0.3.2/pysurfex/obsoul.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.1/pysurfex/platform.py` & `pysurfex-0.0.3.2/pysurfex/platform.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.1/pysurfex/read.py` & `pysurfex-0.0.3.2/pysurfex/read.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.1/pysurfex/run.py` & `pysurfex-0.0.3.2/pysurfex/run.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.1/pysurfex/settings/assimilation.json` & `pysurfex-0.0.3.2/pysurfex/settings/assimilation.json`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.1/pysurfex/settings/forecast.json` & `pysurfex-0.0.3.2/pysurfex/settings/forecast.json`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.1/pysurfex/settings/pgd.json` & `pysurfex-0.0.3.2/pysurfex/settings/pgd.json`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.1/pysurfex/settings/prep.json` & `pysurfex-0.0.3.2/pysurfex/settings/prep.json`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.1/pysurfex/timeseries.py` & `pysurfex-0.0.3.2/pysurfex/timeseries.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.1/pysurfex/titan.py` & `pysurfex-0.0.3.2/pysurfex/titan.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.1/pysurfex/util.py` & `pysurfex-0.0.3.2/pysurfex/util.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.1/pysurfex/variable.py` & `pysurfex-0.0.3.2/pysurfex/variable.py`

 * *Files identical despite different names*

### Comparing `pysurfex-0.0.3.1/PKG-INFO` & `pysurfex-0.0.3.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysurfex
-Version: 0.0.3.1
+Version: 0.0.3.2
 Summary: Python API to SURFEX
 Home-page: https://github.com/metno/pysurfex
 License: MIT
 Author: Trygve Aspelien
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,99 +12,102 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cfunits (>=3.3.5,<4.0.0)
 Requires-Dist: dateutils (>=0.6.12,<0.7.0)
 Requires-Dist: eccodes (>=1.5.1,<2.0.0)
 Requires-Dist: f90nml (>=1.4.3,<2.0.0)
-Requires-Dist: fastjsonschema (==2.16.2)
 Requires-Dist: gridpp (>=0.6.0,<0.7.0)
 Requires-Dist: humanize (>=3.14.0,<4.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
-Requires-Dist: netcdf4 (>=1.6.3,<2.0.0)
+Requires-Dist: netcdf4 (==1.5.7)
 Requires-Dist: numexpr (>=2.8.4,<3.0.0)
 Requires-Dist: numpy (>=1.22.4,<2.0.0)
 Requires-Dist: pandas (>=1.4.0,<2.0.0)
 Requires-Dist: pyproj (>=3.3.0,<4.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: titanlib (>=0.3.3,<0.4.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Documentation, https://metno.github.io/pysurfex/
 Project-URL: Repository, https://github.com/metno/pysurfex
 Description-Content-Type: text/x-rst
 
-.. _README:
 
 .. image:: https://coveralls.io/repos/github/metno/pysurfex/badge.svg?branch=master
 
-https://coveralls.io/github/metno/pysurfex
 
 Python API to SURFEX (pysurfex)
 =======================================================
 
 An API in python to the external surface model SURFEX.
     - Prepare input and namelists to a SURFEX binary
     - Create atmospheric forcing for offline SURFEX runs
     - Read SURFEX output
-    - A scheduler setup to run offline SURFEX experiments
     - Quality control of observations with titanlib
     - Optimal interpolation with gridpp
     - Monitor the observations usage
 
 See online documentation in https://metno.github.io/pysurfex/
 
 Installation of pregenerated packages from pypi (pip)
 ---------------------------------------------------------
 
+All releases will trigger an autmomatic pre-built package on pypi which can be installed by pip
+
 .. code-block:: bash
 
-    pip3 install pysurfex
+  pip3 install pysurfex
 
 User installation:
 
 .. code-block:: bash
 
-    pip3 install pysurfex --user
+  pip3 install pysurfex --user
+
 
+Run pysurfex from pre-built container
+-------------------------------------------
 
+Releases also trigger an update of the pysurfex container in the github container registry. Below is an example to run pgd without any arguments.
+
+.. code-block:: bash
+
+  podman run -it ghcr.io/metno/pysurfex:latest poetry run pgd
 
 
 Installation on debian based Linux system
 --------------------------------------------
 
 Install the required pacakges (some might be obsolete if the pip packages contain the needed depedencies):
 
 .. code-block:: bash
 
   sudo apt-get update
-  sudo apt-get install -y libudunits2-dev libproj-dev libeccodes0 libeccodes-dev libnetcdf-dev netcdf-bin
+  sudo apt-get install -y libudunits2-dev libproj-dev libeccodes0 libeccodes-dev libnetcdf-dev netcdf-bin ca-certificates
 
 The following depencies are needed. Install the non-standard ones e.g. with pip or your system installation system.
 
 General dependencies (from pypi)
 ---------------------------------
 
 .. code-block:: bash
 
   numpy
-  netCDF4
-  cfunits
   pyproj
   pyyaml
   toml
-  netCDF4
   f90nml
-  requests
 
 To read NetCDF files:
 
 .. code-block:: bash
 
   NetCDF4
+  cfunits
 
 To read grib files:
 
 .. code-block:: bash
 
   eccodes
 
@@ -123,45 +126,67 @@
   requests
 
 For Quality control of observations
 
 .. code-block:: bash
 
   titanlib
-  db-sqlite3
 
 For optimal interpolation and observation operators
 
 .. code-block:: bash
 
   gridpp
 
 For testing:
 
 .. code-block:: bash
 
   pytest
 
-Download the source code, then install ``pysurfex`` by executing the following inside the extracted
-folder:
 
 Install pysurfex
 -------------------------------------------
+
+Download the source code, then install ``pysurfex`` by executing the following inside the extracted
+folder:
+
 .. code-block:: bash
 
   poetry install
 
-Create documentation
----------------------------------------------
+
+This will install ``pysurfex`` in a poetry environment and this environment can be activated interactively by:
 
 .. code-block:: bash
 
-  cd docs
-  # Create html documentation
-  make html
+  poetry shell
+
+or
+
+Run pysurfex client applications
+-------------------------------------------
+
+.. code-block:: bash
+
+  poetry run [command]
+  # e.g.
+  poetry run python # will run python inside the pysurfex poetry environment
+
+
+Run pysurfex client applications
+-------------------------------------------
+.. code-block:: python
+
+  import sys
+  from pysurfex.cli import parse_args_surfex_binary, run_surfex_binary
+
+  argv = sys.argv[1:]
+  kwargs = parse_args_surfex_binary(argv, "pgd")
+  run_surfex_binary("pgd", **kwargs)
 
 
 Examples
 -----------------------
 
 See https://metno.github.io/pysurfex/#examples
```

