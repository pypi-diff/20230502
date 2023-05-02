# Comparing `tmp/py4vasp-0.7.2.tar.gz` & `tmp/py4vasp-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py4vasp-0.7.2.tar", max compression
+gzip compressed data, was "py4vasp-0.7.3.tar", max compression
```

## Comparing `py4vasp-0.7.2.tar` & `py4vasp-0.7.3.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0    10178 2022-05-09 07:25:59.189847 py4vasp-0.7.2/LICENSE.txt
--rw-r--r--   0        0        0     2854 2023-03-23 13:12:04.886569 py4vasp-0.7.2/README.md
--rw-r--r--   0        0        0     2315 2023-04-03 11:22:19.616383 py4vasp-0.7.2/pyproject.toml
--rw-r--r--   0        0        0      326 2023-04-03 11:22:19.616383 py4vasp-0.7.2/src/py4vasp/__init__.py
--rw-r--r--   0        0        0     5246 2023-02-15 07:55:50.680586 py4vasp-0.7.2/src/py4vasp/_calculation.py
--rw-r--r--   0        0        0      259 2022-12-16 14:54:49.948020 py4vasp-0.7.2/src/py4vasp/_config.py
--rw-r--r--   0        0        0        0 2022-11-29 09:40:19.980354 py4vasp-0.7.2/src/py4vasp/_control/__init__.py
--rw-r--r--   0        0        0     1780 2022-11-29 09:40:19.986354 py4vasp-0.7.2/src/py4vasp/_control/base.py
--rw-r--r--   0        0        0      427 2022-11-29 09:40:19.990354 py4vasp-0.7.2/src/py4vasp/_control/incar.py
--rw-r--r--   0        0        0      436 2022-11-29 09:40:19.998354 py4vasp-0.7.2/src/py4vasp/_control/kpoints.py
--rw-r--r--   0        0        0      944 2022-11-29 09:40:20.005354 py4vasp-0.7.2/src/py4vasp/_control/poscar.py
--rw-r--r--   0        0        0        0 2022-11-29 09:40:20.011354 py4vasp-0.7.2/src/py4vasp/_data/__init__.py
--rw-r--r--   0        0        0     6622 2023-04-03 11:08:32.372990 py4vasp-0.7.2/src/py4vasp/_data/band.py
--rw-r--r--   0        0        0     9504 2023-02-15 07:55:50.687586 py4vasp-0.7.2/src/py4vasp/_data/base.py
--rw-r--r--   0        0        0     1831 2022-11-29 09:40:20.026353 py4vasp-0.7.2/src/py4vasp/_data/born_effective_charge.py
--rw-r--r--   0        0        0     3891 2022-12-02 11:01:28.568650 py4vasp-0.7.2/src/py4vasp/_data/density.py
--rw-r--r--   0        0        0     5755 2023-04-03 11:08:32.373991 py4vasp-0.7.2/src/py4vasp/_data/dielectric_function.py
--rw-r--r--   0        0        0     2243 2023-04-03 11:08:32.373991 py4vasp-0.7.2/src/py4vasp/_data/dielectric_tensor.py
--rw-r--r--   0        0        0     4331 2022-11-29 09:40:20.054353 py4vasp-0.7.2/src/py4vasp/_data/dispersion.py
--rw-r--r--   0        0        0     4848 2023-01-10 11:26:59.831495 py4vasp-0.7.2/src/py4vasp/_data/dos.py
--rw-r--r--   0        0        0     1864 2022-11-29 09:40:20.069353 py4vasp-0.7.2/src/py4vasp/_data/elastic_modulus.py
--rw-r--r--   0        0        0     6911 2023-03-23 13:12:04.917569 py4vasp-0.7.2/src/py4vasp/_data/energy.py
--rw-r--r--   0        0        0     1931 2022-11-29 09:40:20.091353 py4vasp-0.7.2/src/py4vasp/_data/fatband.py
--rw-r--r--   0        0        0     3408 2023-01-10 11:26:59.840495 py4vasp-0.7.2/src/py4vasp/_data/force.py
--rw-r--r--   0        0        0     1948 2022-11-29 09:40:20.108353 py4vasp-0.7.2/src/py4vasp/_data/force_constant.py
--rw-r--r--   0        0        0     1573 2022-11-29 09:40:20.115353 py4vasp-0.7.2/src/py4vasp/_data/internal_strain.py
--rw-r--r--   0        0        0     8792 2023-01-10 11:26:59.845495 py4vasp-0.7.2/src/py4vasp/_data/kpoint.py
--rw-r--r--   0        0        0     7477 2023-01-10 11:26:59.850495 py4vasp-0.7.2/src/py4vasp/_data/magnetism.py
--rw-r--r--   0        0        0     4915 2023-01-10 11:26:59.854495 py4vasp-0.7.2/src/py4vasp/_data/pair_correlation.py
--rw-r--r--   0        0        0     3158 2022-12-13 15:12:47.154456 py4vasp-0.7.2/src/py4vasp/_data/phonon_band.py
--rw-r--r--   0        0        0     3030 2022-12-13 15:12:47.154456 py4vasp-0.7.2/src/py4vasp/_data/phonon_dos.py
--rw-r--r--   0        0        0     4562 2022-11-29 09:40:20.160353 py4vasp-0.7.2/src/py4vasp/_data/phonon_projector.py
--rw-r--r--   0        0        0     2094 2022-11-29 09:40:20.166353 py4vasp-0.7.2/src/py4vasp/_data/piezoelectric_tensor.py
--rw-r--r--   0        0        0     1317 2022-11-29 09:40:20.173353 py4vasp-0.7.2/src/py4vasp/_data/polarization.py
--rw-r--r--   0        0        0    12065 2023-01-10 11:26:59.858495 py4vasp-0.7.2/src/py4vasp/_data/projector.py
--rw-r--r--   0        0        0      430 2023-01-18 07:23:08.908927 py4vasp-0.7.2/src/py4vasp/_data/selection.py
--rw-r--r--   0        0        0     2362 2022-11-29 09:40:20.193353 py4vasp-0.7.2/src/py4vasp/_data/slice_.py
--rw-r--r--   0        0        0     2906 2023-01-10 11:26:59.863494 py4vasp-0.7.2/src/py4vasp/_data/stress.py
--rw-r--r--   0        0        0    10593 2023-01-18 07:23:08.913926 py4vasp-0.7.2/src/py4vasp/_data/structure.py
--rw-r--r--   0        0        0      514 2022-11-29 09:40:20.210353 py4vasp-0.7.2/src/py4vasp/_data/system.py
--rw-r--r--   0        0        0     6299 2023-01-18 07:23:08.917927 py4vasp-0.7.2/src/py4vasp/_data/topology.py
--rw-r--r--   0        0        0     3180 2022-12-16 14:54:49.950020 py4vasp-0.7.2/src/py4vasp/_data/velocity.py
--rw-r--r--   0        0        0     6460 2022-11-29 09:40:20.220353 py4vasp-0.7.2/src/py4vasp/_data/viewer3d.py
--rw-r--r--   0        0        0     4897 2022-12-13 15:12:47.154456 py4vasp-0.7.2/src/py4vasp/_raw/access.py
--rw-r--r--   0        0        0    14651 2023-03-23 13:12:04.925569 py4vasp-0.7.2/src/py4vasp/_raw/data.py
--rw-r--r--   0        0        0     2636 2022-11-29 09:40:20.234352 py4vasp-0.7.2/src/py4vasp/_raw/data_wrapper.py
--rw-r--r--   0        0        0    11798 2022-12-16 14:54:49.958020 py4vasp-0.7.2/src/py4vasp/_raw/definition.py
--rw-r--r--   0        0        0     7049 2022-12-13 15:12:47.155456 py4vasp-0.7.2/src/py4vasp/_raw/schema.py
--rw-r--r--   0        0        0        0 2022-12-13 15:12:47.155456 py4vasp-0.7.2/src/py4vasp/_third_party/__init__.py
--rw-r--r--   0        0        0      437 2023-02-10 10:58:50.268810 py4vasp-0.7.2/src/py4vasp/_third_party/graph/__init__.py
--rw-r--r--   0        0        0     6647 2022-12-16 14:54:49.966020 py4vasp-0.7.2/src/py4vasp/_third_party/graph/graph.py
--rw-r--r--   0        0        0     2474 2022-12-13 15:12:47.155456 py4vasp-0.7.2/src/py4vasp/_third_party/graph/mixin.py
--rw-r--r--   0        0        0     1727 2022-12-13 15:12:47.155456 py4vasp-0.7.2/src/py4vasp/_third_party/graph/plot.py
--rw-r--r--   0        0        0     4177 2022-12-13 15:12:47.156456 py4vasp-0.7.2/src/py4vasp/_third_party/graph/series.py
--rw-r--r--   0        0        0      395 2022-11-29 09:40:20.256352 py4vasp-0.7.2/src/py4vasp/_third_party/interactive.py
--rw-r--r--   0        0        0      882 2022-11-29 09:40:20.261352 py4vasp-0.7.2/src/py4vasp/_util/check.py
--rw-r--r--   0        0        0     1380 2022-12-16 14:54:49.969020 py4vasp-0.7.2/src/py4vasp/_util/convert.py
--rw-r--r--   0        0        0      422 2023-01-10 11:26:59.872495 py4vasp-0.7.2/src/py4vasp/_util/documentation.py
--rw-r--r--   0        0        0      911 2022-11-29 09:40:20.274352 py4vasp-0.7.2/src/py4vasp/_util/reader.py
--rw-r--r--   0        0        0     3526 2022-12-13 15:12:47.156456 py4vasp-0.7.2/src/py4vasp/_util/select.py
--rw-r--r--   0        0        0      501 2022-11-29 09:40:20.287352 py4vasp-0.7.2/src/py4vasp/control.py
--rw-r--r--   0        0        0     2503 2022-12-16 14:54:49.973020 py4vasp-0.7.2/src/py4vasp/data.py
--rw-r--r--   0        0        0     1660 2023-03-23 13:12:04.945569 py4vasp-0.7.2/src/py4vasp/exception.py
--rw-r--r--   0        0        0      869 2022-12-13 15:12:47.156456 py4vasp-0.7.2/src/py4vasp/raw.py
--rw-r--r--   0        0        0        0 2022-09-13 09:54:26.819128 py4vasp-0.7.2/src/py4vasp/scripts/__init__.py
--rw-r--r--   0        0        0    24796 2023-03-23 13:12:04.953569 py4vasp-0.7.2/src/py4vasp/scripts/error_analysis.py
--rw-r--r--   0        0        0     4114 1970-01-01 00:00:00.000000 py4vasp-0.7.2/setup.py
--rw-r--r--   0        0        0     3935 1970-01-01 00:00:00.000000 py4vasp-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0    10178 2022-05-09 07:25:59.189847 py4vasp-0.7.3/LICENSE.txt
+-rw-r--r--   0        0        0     2854 2023-03-23 13:12:04.886569 py4vasp-0.7.3/README.md
+-rw-r--r--   0        0        0     2333 2023-05-02 08:11:36.358402 py4vasp-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0      326 2023-05-02 08:11:36.358402 py4vasp-0.7.3/src/py4vasp/__init__.py
+-rw-r--r--   0        0        0     5246 2023-02-15 07:55:50.680586 py4vasp-0.7.3/src/py4vasp/_calculation.py
+-rw-r--r--   0        0        0      259 2022-12-16 14:54:49.948020 py4vasp-0.7.3/src/py4vasp/_config.py
+-rw-r--r--   0        0        0        0 2022-11-29 09:40:19.980354 py4vasp-0.7.3/src/py4vasp/_control/__init__.py
+-rw-r--r--   0        0        0     1780 2022-11-29 09:40:19.986354 py4vasp-0.7.3/src/py4vasp/_control/base.py
+-rw-r--r--   0        0        0      427 2022-11-29 09:40:19.990354 py4vasp-0.7.3/src/py4vasp/_control/incar.py
+-rw-r--r--   0        0        0      436 2022-11-29 09:40:19.998354 py4vasp-0.7.3/src/py4vasp/_control/kpoints.py
+-rw-r--r--   0        0        0      944 2022-11-29 09:40:20.005354 py4vasp-0.7.3/src/py4vasp/_control/poscar.py
+-rw-r--r--   0        0        0        0 2022-11-29 09:40:20.011354 py4vasp-0.7.3/src/py4vasp/_data/__init__.py
+-rw-r--r--   0        0        0     6622 2023-05-02 08:11:36.364402 py4vasp-0.7.3/src/py4vasp/_data/band.py
+-rw-r--r--   0        0        0     9504 2023-02-15 07:55:50.687586 py4vasp-0.7.3/src/py4vasp/_data/base.py
+-rw-r--r--   0        0        0     1831 2022-11-29 09:40:20.026353 py4vasp-0.7.3/src/py4vasp/_data/born_effective_charge.py
+-rw-r--r--   0        0        0     3891 2023-05-02 08:11:36.366402 py4vasp-0.7.3/src/py4vasp/_data/density.py
+-rw-r--r--   0        0        0     5755 2023-05-02 08:11:36.368402 py4vasp-0.7.3/src/py4vasp/_data/dielectric_function.py
+-rw-r--r--   0        0        0     2243 2023-05-02 08:11:36.368402 py4vasp-0.7.3/src/py4vasp/_data/dielectric_tensor.py
+-rw-r--r--   0        0        0     4331 2022-11-29 09:40:20.054353 py4vasp-0.7.3/src/py4vasp/_data/dispersion.py
+-rw-r--r--   0        0        0     4848 2023-01-10 11:26:59.831495 py4vasp-0.7.3/src/py4vasp/_data/dos.py
+-rw-r--r--   0        0        0     1864 2022-11-29 09:40:20.069353 py4vasp-0.7.3/src/py4vasp/_data/elastic_modulus.py
+-rw-r--r--   0        0        0     6911 2023-03-23 13:12:04.917569 py4vasp-0.7.3/src/py4vasp/_data/energy.py
+-rw-r--r--   0        0        0     1931 2022-11-29 09:40:20.091353 py4vasp-0.7.3/src/py4vasp/_data/fatband.py
+-rw-r--r--   0        0        0     3408 2023-01-10 11:26:59.840495 py4vasp-0.7.3/src/py4vasp/_data/force.py
+-rw-r--r--   0        0        0     1948 2022-11-29 09:40:20.108353 py4vasp-0.7.3/src/py4vasp/_data/force_constant.py
+-rw-r--r--   0        0        0     1573 2022-11-29 09:40:20.115353 py4vasp-0.7.3/src/py4vasp/_data/internal_strain.py
+-rw-r--r--   0        0        0     8792 2023-01-10 11:26:59.845495 py4vasp-0.7.3/src/py4vasp/_data/kpoint.py
+-rw-r--r--   0        0        0     7477 2023-05-02 08:11:36.370402 py4vasp-0.7.3/src/py4vasp/_data/magnetism.py
+-rw-r--r--   0        0        0     4915 2023-01-10 11:26:59.854495 py4vasp-0.7.3/src/py4vasp/_data/pair_correlation.py
+-rw-r--r--   0        0        0     3158 2022-12-13 15:12:47.154456 py4vasp-0.7.3/src/py4vasp/_data/phonon_band.py
+-rw-r--r--   0        0        0     3030 2022-12-13 15:12:47.154456 py4vasp-0.7.3/src/py4vasp/_data/phonon_dos.py
+-rw-r--r--   0        0        0     4562 2022-11-29 09:40:20.160353 py4vasp-0.7.3/src/py4vasp/_data/phonon_projector.py
+-rw-r--r--   0        0        0     2094 2022-11-29 09:40:20.166353 py4vasp-0.7.3/src/py4vasp/_data/piezoelectric_tensor.py
+-rw-r--r--   0        0        0     1317 2022-11-29 09:40:20.173353 py4vasp-0.7.3/src/py4vasp/_data/polarization.py
+-rw-r--r--   0        0        0    12065 2023-05-02 08:11:36.371402 py4vasp-0.7.3/src/py4vasp/_data/projector.py
+-rw-r--r--   0        0        0      430 2023-01-18 07:23:08.908927 py4vasp-0.7.3/src/py4vasp/_data/selection.py
+-rw-r--r--   0        0        0     2362 2022-11-29 09:40:20.193353 py4vasp-0.7.3/src/py4vasp/_data/slice_.py
+-rw-r--r--   0        0        0     2906 2023-05-02 08:11:36.371402 py4vasp-0.7.3/src/py4vasp/_data/stress.py
+-rw-r--r--   0        0        0    10593 2023-05-02 08:11:36.371402 py4vasp-0.7.3/src/py4vasp/_data/structure.py
+-rw-r--r--   0        0        0      514 2022-11-29 09:40:20.210353 py4vasp-0.7.3/src/py4vasp/_data/system.py
+-rw-r--r--   0        0        0     6299 2023-01-18 07:23:08.917927 py4vasp-0.7.3/src/py4vasp/_data/topology.py
+-rw-r--r--   0        0        0     3180 2022-12-16 14:54:49.950020 py4vasp-0.7.3/src/py4vasp/_data/velocity.py
+-rw-r--r--   0        0        0     6460 2022-11-29 09:40:20.220353 py4vasp-0.7.3/src/py4vasp/_data/viewer3d.py
+-rw-r--r--   0        0        0     4897 2022-12-13 15:12:47.154456 py4vasp-0.7.3/src/py4vasp/_raw/access.py
+-rw-r--r--   0        0        0    14651 2023-03-23 13:12:04.925569 py4vasp-0.7.3/src/py4vasp/_raw/data.py
+-rw-r--r--   0        0        0     2636 2023-05-02 08:11:36.372402 py4vasp-0.7.3/src/py4vasp/_raw/data_wrapper.py
+-rw-r--r--   0        0        0    11798 2023-05-02 08:11:36.372402 py4vasp-0.7.3/src/py4vasp/_raw/definition.py
+-rw-r--r--   0        0        0     7049 2022-12-13 15:12:47.155456 py4vasp-0.7.3/src/py4vasp/_raw/schema.py
+-rw-r--r--   0        0        0        0 2022-12-13 15:12:47.155456 py4vasp-0.7.3/src/py4vasp/_third_party/__init__.py
+-rw-r--r--   0        0        0      437 2023-02-10 10:58:50.268810 py4vasp-0.7.3/src/py4vasp/_third_party/graph/__init__.py
+-rw-r--r--   0        0        0     6647 2022-12-16 14:54:49.966020 py4vasp-0.7.3/src/py4vasp/_third_party/graph/graph.py
+-rw-r--r--   0        0        0     2474 2022-12-13 15:12:47.155456 py4vasp-0.7.3/src/py4vasp/_third_party/graph/mixin.py
+-rw-r--r--   0        0        0     1727 2022-12-13 15:12:47.155456 py4vasp-0.7.3/src/py4vasp/_third_party/graph/plot.py
+-rw-r--r--   0        0        0     4177 2022-12-13 15:12:47.156456 py4vasp-0.7.3/src/py4vasp/_third_party/graph/series.py
+-rw-r--r--   0        0        0      395 2022-11-29 09:40:20.256352 py4vasp-0.7.3/src/py4vasp/_third_party/interactive.py
+-rw-r--r--   0        0        0      882 2022-11-29 09:40:20.261352 py4vasp-0.7.3/src/py4vasp/_util/check.py
+-rw-r--r--   0        0        0     1380 2022-12-16 14:54:49.969020 py4vasp-0.7.3/src/py4vasp/_util/convert.py
+-rw-r--r--   0        0        0      422 2023-01-10 11:26:59.872495 py4vasp-0.7.3/src/py4vasp/_util/documentation.py
+-rw-r--r--   0        0        0      911 2023-05-02 08:11:36.373402 py4vasp-0.7.3/src/py4vasp/_util/reader.py
+-rw-r--r--   0        0        0     3526 2023-05-02 08:11:36.375402 py4vasp-0.7.3/src/py4vasp/_util/select.py
+-rw-r--r--   0        0        0      501 2022-11-29 09:40:20.287352 py4vasp-0.7.3/src/py4vasp/control.py
+-rw-r--r--   0        0        0     2503 2022-12-16 14:54:49.973020 py4vasp-0.7.3/src/py4vasp/data.py
+-rw-r--r--   0        0        0     1660 2023-05-02 08:11:36.375402 py4vasp-0.7.3/src/py4vasp/exception.py
+-rw-r--r--   0        0        0      869 2022-12-13 15:12:47.156456 py4vasp-0.7.3/src/py4vasp/raw.py
+-rw-r--r--   0        0        0        0 2022-09-13 09:54:26.819128 py4vasp-0.7.3/src/py4vasp/scripts/__init__.py
+-rw-r--r--   0        0        0    24796 2023-03-23 13:12:04.953569 py4vasp-0.7.3/src/py4vasp/scripts/error_analysis.py
+-rw-r--r--   0        0        0     4137 1970-01-01 00:00:00.000000 py4vasp-0.7.3/setup.py
+-rw-r--r--   0        0        0     3972 1970-01-01 00:00:00.000000 py4vasp-0.7.3/PKG-INFO
```

### Comparing `py4vasp-0.7.2/LICENSE.txt` & `py4vasp-0.7.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/README.md` & `py4vasp-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/pyproject.toml` & `py4vasp-0.7.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py4vasp"
-version = "0.7.2"
+version = "0.7.3"
 description = "Tool for assisting with the analysis and setup of VASP calculations."
 authors = [
     "VASP Software GmbH <py4vasp@vasp.at>",
     "Martin Schlipf <martin.schlipf@gmail.com>",
     "Henrique Miranda <miranda.henrique@gmail.com>",
     "Orest Dubay <orest-d@users.noreply.github.com>",
     "Jonathan Lahnsteiner <jonathan.lahnsteiner@gmx.at>",
@@ -32,14 +32,15 @@
 # nglview should be excluded
 ipywidgets = "^7.7"
 ase = ">=3.22.1"
 mdtraj = ">=1.9.6"
 mrcfile = ">=1.3.0"
 plotly = ">=5.9.0"
 kaleido = "!=0.2.1.post1,>=0.2.1"
+ipython = "^8.12"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=7.1.2"
 pytest-cov = ">=3.0.0"
 pylint = ">=2.14.3"
 Sphinx = ">=5.0.2"
 black = ">=22.6.0"
```

### Comparing `py4vasp-0.7.2/src/py4vasp/_calculation.py` & `py4vasp-0.7.3/src/py4vasp/_calculation.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_control/base.py` & `py4vasp-0.7.3/src/py4vasp/_control/base.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_control/poscar.py` & `py4vasp-0.7.3/src/py4vasp/_control/poscar.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_data/band.py` & `py4vasp-0.7.3/src/py4vasp/_data/band.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_data/base.py` & `py4vasp-0.7.3/src/py4vasp/_data/base.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_data/born_effective_charge.py` & `py4vasp-0.7.3/src/py4vasp/_data/born_effective_charge.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_data/density.py` & `py4vasp-0.7.3/src/py4vasp/_data/density.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_data/dielectric_function.py` & `py4vasp-0.7.3/src/py4vasp/_data/dielectric_function.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_data/dielectric_tensor.py` & `py4vasp-0.7.3/src/py4vasp/_data/dielectric_tensor.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_data/dispersion.py` & `py4vasp-0.7.3/src/py4vasp/_data/dispersion.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_data/dos.py` & `py4vasp-0.7.3/src/py4vasp/_data/dos.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_data/elastic_modulus.py` & `py4vasp-0.7.3/src/py4vasp/_data/elastic_modulus.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_data/energy.py` & `py4vasp-0.7.3/src/py4vasp/_data/energy.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_data/fatband.py` & `py4vasp-0.7.3/src/py4vasp/_data/fatband.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_data/force.py` & `py4vasp-0.7.3/src/py4vasp/_data/force.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_data/force_constant.py` & `py4vasp-0.7.3/src/py4vasp/_data/force_constant.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_data/internal_strain.py` & `py4vasp-0.7.3/src/py4vasp/_data/internal_strain.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_data/kpoint.py` & `py4vasp-0.7.3/src/py4vasp/_data/kpoint.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_data/magnetism.py` & `py4vasp-0.7.3/src/py4vasp/_data/magnetism.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_data/pair_correlation.py` & `py4vasp-0.7.3/src/py4vasp/_data/pair_correlation.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_data/phonon_band.py` & `py4vasp-0.7.3/src/py4vasp/_data/phonon_band.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_data/phonon_dos.py` & `py4vasp-0.7.3/src/py4vasp/_data/phonon_dos.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_data/phonon_projector.py` & `py4vasp-0.7.3/src/py4vasp/_data/phonon_projector.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_data/piezoelectric_tensor.py` & `py4vasp-0.7.3/src/py4vasp/_data/piezoelectric_tensor.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_data/polarization.py` & `py4vasp-0.7.3/src/py4vasp/_data/polarization.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_data/projector.py` & `py4vasp-0.7.3/src/py4vasp/_data/projector.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_data/slice_.py` & `py4vasp-0.7.3/src/py4vasp/_data/slice_.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_data/stress.py` & `py4vasp-0.7.3/src/py4vasp/_data/stress.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_data/structure.py` & `py4vasp-0.7.3/src/py4vasp/_data/structure.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_data/system.py` & `py4vasp-0.7.3/src/py4vasp/_data/system.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_data/topology.py` & `py4vasp-0.7.3/src/py4vasp/_data/topology.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_data/velocity.py` & `py4vasp-0.7.3/src/py4vasp/_data/velocity.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_data/viewer3d.py` & `py4vasp-0.7.3/src/py4vasp/_data/viewer3d.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_raw/access.py` & `py4vasp-0.7.3/src/py4vasp/_raw/access.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_raw/data.py` & `py4vasp-0.7.3/src/py4vasp/_raw/data.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_raw/data_wrapper.py` & `py4vasp-0.7.3/src/py4vasp/_raw/data_wrapper.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_raw/definition.py` & `py4vasp-0.7.3/src/py4vasp/_raw/definition.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_raw/schema.py` & `py4vasp-0.7.3/src/py4vasp/_raw/schema.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_third_party/graph/graph.py` & `py4vasp-0.7.3/src/py4vasp/_third_party/graph/graph.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_third_party/graph/mixin.py` & `py4vasp-0.7.3/src/py4vasp/_third_party/graph/mixin.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_third_party/graph/plot.py` & `py4vasp-0.7.3/src/py4vasp/_third_party/graph/plot.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_third_party/graph/series.py` & `py4vasp-0.7.3/src/py4vasp/_third_party/graph/series.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_util/check.py` & `py4vasp-0.7.3/src/py4vasp/_util/check.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_util/convert.py` & `py4vasp-0.7.3/src/py4vasp/_util/convert.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_util/reader.py` & `py4vasp-0.7.3/src/py4vasp/_util/reader.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/_util/select.py` & `py4vasp-0.7.3/src/py4vasp/_util/select.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/data.py` & `py4vasp-0.7.3/src/py4vasp/data.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/exception.py` & `py4vasp-0.7.3/src/py4vasp/exception.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/raw.py` & `py4vasp-0.7.3/src/py4vasp/raw.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/src/py4vasp/scripts/error_analysis.py` & `py4vasp-0.7.3/src/py4vasp/scripts/error_analysis.py`

 * *Files identical despite different names*

### Comparing `py4vasp-0.7.2/setup.py` & `py4vasp-0.7.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,29 +16,30 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['ase>=3.22.1',
  'h5py>=3.7.0',
+ 'ipython>=8.12,<9.0',
  'ipywidgets>=7.7,<8.0',
  'kaleido!=0.2.1.post1,>=0.2.1',
  'mdtraj>=1.9.6',
  'mrcfile>=1.3.0',
  'nglview>=3.0.3',
  'numpy>=1.23.0',
  'pandas>=1.4.3',
  'plotly>=5.9.0']
 
 entry_points = \
 {'console_scripts': ['error-analysis = py4vasp.scripts.error_analysis:main']}
 
 setup_kwargs = {
     'name': 'py4vasp',
-    'version': '0.7.2',
+    'version': '0.7.3',
     'description': 'Tool for assisting with the analysis and setup of VASP calculations.',
     'long_description': '# py4vasp\n\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![tests](https://github.com/vasp-dev/py4vasp/actions/workflows/test.yml/badge.svg)](https://github.com/vasp-dev/py4vasp/actions/workflows/test.yml)\n\n> Please note that this document is intended mostly for developers that want to use\n> the version of py4vasp provided on Github. If you just want to install py4vasp to\n> use it, please follow the [official documentation](https://vasp.at/py4vasp/latest).\n\n## Installation\n\nWe use the [poetry dependency manager](https://python-poetry.org/) which takes care of\nall dependencies and maintains a virtual environment to check the code. If you want to\ntest something in the virtual environment, just use e.g. ```poetry run jupyter-notebook```.\n\nUsing poetry installing and the code requires the following steps. The last step will\ntest whether everything worked\n~~~shell\ngit clone git@github.com:vasp-dev/py4vasp.git\npip install poetry\npoetry install\npoetry run pytest\n~~~\nNote that this will install py4vasp into a virtual environment managed by poetry. This\nisolates the code from all other packages you have installed and makes sure that when\nyou modify the code all the relevant dependencies are tracked.\n\nOccasionally, we encountered errors when installing the *mdtraj* dependency in this\nfashion, in particular on MacOS and Windows. If you notice the same behavior, we\nrecommend to manage your environment with *conda* and install *py4vasp* in the\nfollowing manner\n~~~shell\ngit clone git@github.com:vasp-dev/py4vasp.git\nconda create --name py4vasp-env python=3.8\nconda activate py4vasp-env\nconda install -c conda-forge poetry\nconda install -c conda-forge mdtraj\npoetry config virtualenvs.create false --local\npoetry install\npoetry run pytest\n~~~\n\n## Code style\n\nCode style is enforced, but is not something the developer should spend time on, so we\ndecided on using the black formatter. Please run ```black .``` before committing the code.\n\n## Contributing to py4vasp\n\nWe welcome contributions to py4vasp. To improve the code please follow this workflow\n\n* Create an issue for the bugfix or feature you plan to work on, this gives the option\n  to provide some input before work is invested.\n* Implement your work in a fork of the repository and create a pull request for it.\n  Please make sure to test your code thoroughly and commit the tests in the pull\n  request in the tests directory.\n* In the message to your merge request mention the issue the code attempts to solve.\n* We will try to include your merge request rapidly when all the tests pass and your\n  code is covered by tests.\n\nPlease limit the size of a pull request to approximately 200 lines of code\notherwise reviewing the changes gets unwieldy. Prefer splitting the work into\nmultiple smaller chunks if necessary.\n',
     'author': 'VASP Software GmbH',
     'author_email': 'py4vasp@vasp.at',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://vasp.at/py4vasp/latest',
```

### Comparing `py4vasp-0.7.2/PKG-INFO` & `py4vasp-0.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: py4vasp
-Version: 0.7.2
+Version: 0.7.3
 Summary: Tool for assisting with the analysis and setup of VASP calculations.
 Home-page: https://vasp.at/py4vasp/latest
 License: Apache-2.0
 Author: VASP Software GmbH
 Author-email: py4vasp@vasp.at
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ase (>=3.22.1)
 Requires-Dist: h5py (>=3.7.0)
+Requires-Dist: ipython (>=8.12,<9.0)
 Requires-Dist: ipywidgets (>=7.7,<8.0)
 Requires-Dist: kaleido (!=0.2.1.post1,>=0.2.1)
 Requires-Dist: mdtraj (>=1.9.6)
 Requires-Dist: mrcfile (>=1.3.0)
 Requires-Dist: nglview (>=3.0.3)
 Requires-Dist: numpy (>=1.23.0)
 Requires-Dist: pandas (>=1.4.3)
```

