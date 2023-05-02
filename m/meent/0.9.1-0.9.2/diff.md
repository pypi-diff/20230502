# Comparing `tmp/meent-0.9.1.tar.gz` & `tmp/meent-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meent-0.9.1.tar", last modified: Thu Apr 27 05:56:38 2023, max compression
+gzip compressed data, was "meent-0.9.2.tar", last modified: Tue May  2 14:35:52 2023, max compression
```

## Comparing `meent-0.9.1.tar` & `meent-0.9.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:38.059154 meent-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-27 05:56:27.000000 meent-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-27 05:56:38.059154 meent-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-04-27 05:56:27.000000 meent-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:38.051154 meent-0.9.1/meent/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-27 05:56:27.000000 meent-0.9.1/meent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-27 05:56:27.000000 meent-0.9.1/meent/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:38.051154 meent-0.9.1/meent/nk_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:38.055154 meent-0.9.1/meent/nk_data/filmetrics/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-27 05:56:27.000000 meent-0.9.1/meent/nk_data/filmetrics/Al2O3.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-04-27 05:56:27.000000 meent-0.9.1/meent/nk_data/filmetrics/Si.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-04-27 05:56:27.000000 meent-0.9.1/meent/nk_data/filmetrics/Si3N4.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-04-27 05:56:27.000000 meent-0.9.1/meent/nk_data/filmetrics/SiO2.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:38.055154 meent-0.9.1/meent/nk_data/matlab/
--rw-r--r--   0 runner    (1001) docker     (123)    11222 2023-04-27 05:56:27.000000 meent-0.9.1/meent/nk_data/matlab/p_Si.mat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:38.055154 meent-0.9.1/meent/on_jax/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_jax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:38.055154 meent-0.9.1/meent/on_jax/emsolver/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_jax/emsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16856 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_jax/emsolver/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_jax/emsolver/convolution_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    38784 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_jax/emsolver/field_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_jax/emsolver/primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)    13965 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_jax/emsolver/rcwa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_jax/emsolver/scattering_method.py
--rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_jax/emsolver/smm_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    14577 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_jax/emsolver/transfer_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_jax/mee.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:38.055154 meent-0.9.1/meent/on_jax/modeler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_jax/modeler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_jax/modeler/modeling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:38.055154 meent-0.9.1/meent/on_jax/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_jax/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_jax/optimizer/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_jax/optimizer/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:38.055154 meent-0.9.1/meent/on_numpy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:38.055154 meent-0.9.1/meent/on_numpy/emsolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_numpy/emsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_numpy/emsolver/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_numpy/emsolver/convolution_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    27387 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_numpy/emsolver/field_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_numpy/emsolver/rcwa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_numpy/emsolver/scattering_method.py
--rw-r--r--   0 runner    (1001) docker     (123)    10530 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_numpy/emsolver/smm_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_numpy/emsolver/transfer_method.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_numpy/mee.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:38.055154 meent-0.9.1/meent/on_numpy/modeler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_numpy/modeler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_numpy/modeler/modeling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:38.055154 meent-0.9.1/meent/on_torch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:38.059154 meent-0.9.1/meent/on_torch/emsolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_torch/emsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18368 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_torch/emsolver/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13174 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_torch/emsolver/convolution_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    28821 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_torch/emsolver/field_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_torch/emsolver/primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)    11741 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_torch/emsolver/rcwa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_torch/emsolver/scattering_method.py
--rw-r--r--   0 runner    (1001) docker     (123)    10516 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_torch/emsolver/smm_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    14085 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_torch/emsolver/transfer_method.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_torch/mee.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:38.059154 meent-0.9.1/meent/on_torch/modeler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_torch/modeler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_torch/modeler/modeling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:38.059154 meent-0.9.1/meent/on_torch/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_torch/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_torch/optimizer/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-27 05:56:27.000000 meent-0.9.1/meent/on_torch/optimizer/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 05:56:38.051154 meent-0.9.1/meent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-27 05:56:38.000000 meent-0.9.1/meent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-27 05:56:38.000000 meent-0.9.1/meent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 05:56:38.000000 meent-0.9.1/meent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-27 05:56:38.000000 meent-0.9.1/meent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 05:56:38.000000 meent-0.9.1/meent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 05:56:38.059154 meent-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-27 05:56:27.000000 meent-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:52.947544 meent-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-02 14:35:37.000000 meent-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-02 14:35:52.947544 meent-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-05-02 14:35:37.000000 meent-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:52.939544 meent-0.9.2/meent/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-02 14:35:37.000000 meent-0.9.2/meent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-05-02 14:35:37.000000 meent-0.9.2/meent/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:52.939544 meent-0.9.2/meent/nk_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:52.943544 meent-0.9.2/meent/nk_data/filmetrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-02 14:35:37.000000 meent-0.9.2/meent/nk_data/filmetrics/Al2O3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-05-02 14:35:37.000000 meent-0.9.2/meent/nk_data/filmetrics/Si.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-02 14:35:37.000000 meent-0.9.2/meent/nk_data/filmetrics/Si3N4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-05-02 14:35:37.000000 meent-0.9.2/meent/nk_data/filmetrics/SiO2.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:52.943544 meent-0.9.2/meent/nk_data/matlab/
+-rw-r--r--   0 runner    (1001) docker     (123)    11222 2023-05-02 14:35:37.000000 meent-0.9.2/meent/nk_data/matlab/p_Si.mat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:52.943544 meent-0.9.2/meent/on_jax/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_jax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:52.943544 meent-0.9.2/meent/on_jax/emsolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_jax/emsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16856 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_jax/emsolver/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_jax/emsolver/convolution_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38784 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_jax/emsolver/field_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_jax/emsolver/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13965 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_jax/emsolver/rcwa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_jax/emsolver/scattering_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_jax/emsolver/smm_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14577 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_jax/emsolver/transfer_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_jax/mee.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:52.943544 meent-0.9.2/meent/on_jax/modeler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_jax/modeler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_jax/modeler/modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:52.943544 meent-0.9.2/meent/on_jax/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_jax/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_jax/optimizer/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_jax/optimizer/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:52.943544 meent-0.9.2/meent/on_numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:52.947544 meent-0.9.2/meent/on_numpy/emsolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_numpy/emsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_numpy/emsolver/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_numpy/emsolver/convolution_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27387 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_numpy/emsolver/field_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_numpy/emsolver/rcwa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_numpy/emsolver/scattering_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10530 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_numpy/emsolver/smm_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_numpy/emsolver/transfer_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_numpy/mee.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:52.947544 meent-0.9.2/meent/on_numpy/modeler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_numpy/modeler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_numpy/modeler/modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:52.947544 meent-0.9.2/meent/on_torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:52.947544 meent-0.9.2/meent/on_torch/emsolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_torch/emsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18368 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_torch/emsolver/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13557 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_torch/emsolver/convolution_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29243 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_torch/emsolver/field_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_torch/emsolver/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11858 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_torch/emsolver/rcwa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_torch/emsolver/scattering_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10516 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_torch/emsolver/smm_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14085 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_torch/emsolver/transfer_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_torch/mee.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:52.947544 meent-0.9.2/meent/on_torch/modeler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_torch/modeler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_torch/modeler/modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:52.947544 meent-0.9.2/meent/on_torch/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_torch/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_torch/optimizer/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-02 14:35:37.000000 meent-0.9.2/meent/on_torch/optimizer/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:35:52.943544 meent-0.9.2/meent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-02 14:35:52.000000 meent-0.9.2/meent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-02 14:35:52.000000 meent-0.9.2/meent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:35:52.000000 meent-0.9.2/meent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-02 14:35:52.000000 meent-0.9.2/meent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 14:35:52.000000 meent-0.9.2/meent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 14:35:52.947544 meent-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-02 14:35:37.000000 meent-0.9.2/setup.py
```

### Comparing `meent-0.9.1/LICENSE` & `meent-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/README.md` & `meent-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/meent/main.py` & `meent-0.9.2/meent/main.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/meent/nk_data/filmetrics/Al2O3.txt` & `meent-0.9.2/meent/nk_data/filmetrics/Al2O3.txt`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/meent/nk_data/filmetrics/Si.txt` & `meent-0.9.2/meent/nk_data/filmetrics/Si.txt`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/meent/nk_data/filmetrics/Si3N4.txt` & `meent-0.9.2/meent/nk_data/filmetrics/Si3N4.txt`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/meent/nk_data/filmetrics/SiO2.txt` & `meent-0.9.2/meent/nk_data/filmetrics/SiO2.txt`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/meent/nk_data/matlab/p_Si.mat` & `meent-0.9.2/meent/nk_data/matlab/p_Si.mat`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/meent/on_jax/emsolver/_base.py` & `meent-0.9.2/meent/on_jax/emsolver/_base.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/meent/on_jax/emsolver/convolution_matrix.py` & `meent-0.9.2/meent/on_jax/emsolver/convolution_matrix.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/meent/on_jax/emsolver/field_distribution.py` & `meent-0.9.2/meent/on_jax/emsolver/field_distribution.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/meent/on_jax/emsolver/primitives.py` & `meent-0.9.2/meent/on_jax/emsolver/primitives.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/meent/on_jax/emsolver/rcwa.py` & `meent-0.9.2/meent/on_jax/emsolver/rcwa.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/meent/on_jax/emsolver/scattering_method.py` & `meent-0.9.2/meent/on_jax/emsolver/scattering_method.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/meent/on_jax/emsolver/smm_util.py` & `meent-0.9.2/meent/on_jax/emsolver/smm_util.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/meent/on_jax/emsolver/transfer_method.py` & `meent-0.9.2/meent/on_jax/emsolver/transfer_method.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/meent/on_jax/mee.py` & `meent-0.9.2/meent/on_jax/mee.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/meent/on_jax/modeler/modeling.py` & `meent-0.9.2/meent/on_jax/modeler/modeling.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/meent/on_jax/optimizer/loss.py` & `meent-0.9.2/meent/on_jax/optimizer/loss.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/meent/on_jax/optimizer/optimizer.py` & `meent-0.9.2/meent/on_jax/optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/meent/on_numpy/emsolver/_base.py` & `meent-0.9.2/meent/on_numpy/emsolver/_base.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/meent/on_numpy/emsolver/convolution_matrix.py` & `meent-0.9.2/meent/on_numpy/emsolver/convolution_matrix.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/meent/on_numpy/emsolver/field_distribution.py` & `meent-0.9.2/meent/on_numpy/emsolver/field_distribution.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/meent/on_numpy/emsolver/rcwa.py` & `meent-0.9.2/meent/on_numpy/emsolver/rcwa.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/meent/on_numpy/emsolver/scattering_method.py` & `meent-0.9.2/meent/on_numpy/emsolver/scattering_method.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/meent/on_numpy/emsolver/smm_util.py` & `meent-0.9.2/meent/on_numpy/emsolver/smm_util.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/meent/on_numpy/emsolver/transfer_method.py` & `meent-0.9.2/meent/on_numpy/emsolver/transfer_method.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/meent/on_numpy/mee.py` & `meent-0.9.2/meent/on_numpy/mee.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/meent/on_numpy/modeler/modeling.py` & `meent-0.9.2/meent/on_numpy/modeler/modeling.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/meent/on_torch/emsolver/_base.py` & `meent-0.9.2/meent/on_torch/emsolver/_base.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/meent/on_torch/emsolver/convolution_matrix.py` & `meent-0.9.2/meent/on_torch/emsolver/convolution_matrix.py`

 * *Files 3% similar despite different names*

```diff
@@ -141,14 +141,15 @@
 
         f_coeffs = fft_piecewise_constant_vector(ucell_layer, x_list, y_list,
                                                  fourier_order_x, fourier_order_y, type_complex=type_complex)
         o_f_coeffs = fft_piecewise_constant_vector(1/ucell_layer, x_list, y_list,
                                                  fourier_order_x, fourier_order_y, type_complex=type_complex)
 
         center = torch.div(torch.tensor(f_coeffs.shape, device=device), 2, rounding_mode='trunc')
+        center = torch.tensor(center, device=device)
 
         conv_idx_y = torch.arange(-ff_y + 1, ff_y, 1, device=device)
         conv_idx_y = circulant(conv_idx_y, device=device)
         conv_i = conv_idx_y.repeat_interleave(ff_x, dim=1)
         conv_i = conv_i.repeat_interleave(ff_x, dim=0)
 
         conv_idx_x = torch.arange(-ff_x + 1, ff_x, 1, device=device)
@@ -173,14 +174,15 @@
         e_conv_all = torch.zeros((ucell_pmt.shape[0], ff, ff), device=device).type(type_complex)
         o_e_conv_all = torch.zeros((ucell_pmt.shape[0], ff, ff), device=device).type(type_complex)
 
         for i, layer in enumerate(ucell_pmt):
             f_coeffs = fft_piecewise_constant(layer, fourier_order_x, fourier_order_y, device=device, type_complex=type_complex)
             o_f_coeffs = fft_piecewise_constant(1/layer, fourier_order_x, fourier_order_y, device=device, type_complex=type_complex)
             center = torch.div(torch.tensor(f_coeffs.shape, device=device), 2, rounding_mode='trunc')
+            center = torch.tensor(center, device=device)
             conv_idx = torch.arange(-ff + 1, ff, 1, device=device)
             conv_idx = circulant(conv_idx, device=device)
             e_conv = f_coeffs[center[0], center[1] + conv_idx]
             o_e_conv = o_f_coeffs[center[0], center[1] + conv_idx]
             e_conv_all[i] = e_conv
             o_e_conv_all[i] = o_e_conv
     else:  # 2D
@@ -190,14 +192,15 @@
         e_conv_all = torch.zeros((ucell_pmt.shape[0], ff_x * ff_y,  ff_x * ff_y), device=device).type(type_complex)
         o_e_conv_all = torch.zeros((ucell_pmt.shape[0], ff_x * ff_y,  ff_x * ff_y), device=device).type(type_complex)
 
         for i, layer in enumerate(ucell_pmt):
             f_coeffs = fft_piecewise_constant(layer, fourier_order_x, fourier_order_y, device=device, type_complex=type_complex)
             o_f_coeffs = fft_piecewise_constant(1/layer, fourier_order_x, fourier_order_y, device=device, type_complex=type_complex)
             center = torch.div(torch.tensor(f_coeffs.shape, device=device), 2, rounding_mode='trunc')
+            center = torch.tensor(center, device=device)
 
             conv_idx_y = torch.arange(-ff_y + 1, ff_y, 1, device=device)
             conv_idx_y = circulant(conv_idx_y, device=device)
             conv_i = conv_idx_y.repeat_interleave(ff_x, dim=1)
             conv_i = conv_i.repeat_interleave(ff_x, dim=0)
 
             conv_idx_x = torch.arange(-ff_x + 1, ff_x, 1, device=device)
@@ -226,14 +229,15 @@
 
         for i, layer in enumerate(ucell_pmt):
             n = minimum_pattern_size // layer.shape[1]
             layer = layer.repeat_interleave(n + 1, axis=1)
             f_coeffs = torch.fft.fftshift(torch.fft.fft(layer / layer.numel()))
             o_f_coeffs = torch.fft.fftshift(torch.fft.fft(1/layer / layer.numel()))
             center = torch.div(torch.tensor(f_coeffs.shape, device=device), 2, rounding_mode='trunc')
+            center = torch.tensor(center, device=device)
             conv_idx = torch.arange(-ff + 1, ff, 1, device=device)
             conv_idx = circulant(conv_idx, device=device)
             e_conv = f_coeffs[center[0], center[1] + conv_idx]
             o_e_conv = o_f_coeffs[center[0], center[1] + conv_idx]
             e_conv_all[i] = e_conv
             o_e_conv_all[i] = o_e_conv
 
@@ -251,22 +255,25 @@
             minimum_pattern_size_y = 2 * ff_y
             minimum_pattern_size_x = 2 * ff_x
         # e.g., 8 bytes * (40*500) * (40*500) / 1E6 = 3200 MB = 3.2 GB
 
         for i, layer in enumerate(ucell_pmt):
             if layer.shape[0] < minimum_pattern_size_y:
                 n = torch.div(minimum_pattern_size_y, layer.shape[0], rounding_mode='trunc')
+                n = torch.tensor(n, device=device)
                 layer = layer.repeat_interleave(n + 1, axis=0)
             if layer.shape[1] < minimum_pattern_size_x:
                 n = torch.div(minimum_pattern_size_x, layer.shape[1], rounding_mode='trunc')
+                n = torch.tensor(n, device=device)
                 layer = layer.repeat_interleave(n + 1, axis=1)
 
             f_coeffs = torch.fft.fftshift(torch.fft.fft2(layer / layer.numel()))
             o_f_coeffs = torch.fft.fftshift(torch.fft.fft2(1/layer / layer.numel()))
             center = torch.div(torch.tensor(f_coeffs.shape, device=device), 2, rounding_mode='trunc')
+            center = torch.tensor(center, device=device)
 
             conv_idx_y = torch.arange(-ff_y + 1, ff_y, 1, device=device)
             conv_idx_y = circulant(conv_idx_y, device=device)
             conv_i = conv_idx_y.repeat_interleave(ff_x, dim=1)
             conv_i = conv_i.repeat_interleave(ff_x, dim=0)
 
             conv_idx_x = torch.arange(-ff_x + 1, ff_x, 1, device=device)
```

### Comparing `meent-0.9.1/meent/on_torch/emsolver/field_distribution.py` & `meent-0.9.2/meent/on_torch/emsolver/field_distribution.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import torch
 
 
 def field_dist_1d_vectorized_ji(wavelength, kx_vector, T1, layer_info_list, period,
-                                pol, res_x=20, res_y=20, res_z=20, type_complex=torch.complex128, type_float=torch.float64):
+                                pol, res_x=20, res_y=20, res_z=20,  device='cpu',
+                                type_complex=torch.complex128, type_float=torch.float64):
 
     k0 = 2 * torch.pi / wavelength
     Kx = torch.diag(kx_vector / k0)
 
     field_cell = torch.zeros((res_z * len(layer_info_list), res_y, res_x, 3), dtype=type_complex)
 
     T_layer = T1
@@ -31,15 +32,15 @@
             z = k / res_z * d
 
             if pol == 0:
                 Sy = W @ (diag_exp(-k0 * Q * z) @ c1 + diag_exp(k0 * Q * (z - d)) @ c2)
                 Ux = V @ (-diag_exp(-k0 * Q * z) @ c1 + diag_exp(k0 * Q * (z - d)) @ c2)
                 C = Kx @ Sy
 
-                x_1d = torch.arange(res_x, dtype=type_float).reshape((1, -1, 1))
+                x_1d = torch.arange(res_x, dtype=type_float, device=device).reshape((1, -1, 1))
                 x_1d = -1j * x_1d * period[0] / res_x
                 x_2d = torch.tile(x_1d, (res_y, 1, 1))
                 x_2d = x_2d * kx_vector
                 x_2d = x_2d.reshape((res_y, res_x, 1, len(kx_vector)))
 
                 exp_K = torch.exp(x_2d)
                 exp_K = exp_K.reshape((res_y, res_x, -1))
@@ -52,15 +53,15 @@
 
             else:
                 Uy = W @ (diag_exp(-k0 * Q * z) @ c1 + diag_exp(k0 * Q * (z - d)) @ c2)
                 Sx = V @ (-diag_exp(-k0 * Q * z) @ c1 + diag_exp(k0 * Q * (z - d)) @ c2)
 
                 C = EKx @ Uy  # there is a better option for convergence
 
-                x_1d = torch.arange(res_x, dtype=type_float).reshape((1, -1, 1))
+                x_1d = torch.arange(res_x, dtype=type_float, device=device).reshape((1, -1, 1))
                 x_1d = -1j * x_1d * period[0] / res_x
                 x_2d = torch.tile(x_1d, (res_y, 1, 1))
                 x_2d = x_2d * kx_vector
                 x_2d = x_2d.reshape((res_y, res_x, 1, len(kx_vector)))
 
                 exp_K = torch.exp(x_2d)
                 exp_K = exp_K.reshape((res_y, res_x, -1))
@@ -75,15 +76,16 @@
 
         T_layer = a_i @ X @ T_layer
 
     return field_cell
 
 
 def field_dist_1d_conical_vectorized_ji(wavelength, kx_vector, n_I, theta, phi, T1, layer_info_list, period,
-                                        res_x=20, res_y=20, res_z=20, device='cpu', type_complex=torch.complex128, type_float=torch.float64):
+                                        res_x=20, res_y=20, res_z=20, device='cpu',
+                                        type_complex=torch.complex128, type_float=torch.float64):
 
     k0 = 2 * torch.pi / wavelength
     ky = k0 * n_I * torch.sin(theta) * torch.sin(phi)
     Kx = torch.diag(kx_vector / k0)
 
     field_cell = torch.zeros((res_z * len(layer_info_list), res_y, res_x, 6), dtype=type_complex)
 
@@ -96,15 +98,15 @@
             in enumerate(layer_info_list[::-1]):
 
         c = torch.cat([big_I, big_B @ big_A_i @ big_X])  @ T_layer
 
         for k in range(res_z):
             Sx, Sy, Ux, Uy, Sz, Uz = z_loop_1d_conical(k, c, k0, Kx, ky, res_z, E_conv_i, q_1, q_2, W_1, W_2, V_11, V_12, V_21, V_22, d)
 
-            x_1d = torch.arange(res_x, dtype=type_float).reshape((1, -1, 1))
+            x_1d = torch.arange(res_x, dtype=type_float, device=device).reshape((1, -1, 1))
             x_1d = -1j * x_1d * period[0] / res_x
             x_2d = torch.tile(x_1d, (res_y, 1, 1))
             x_2d = x_2d * kx_vector
             x_2d = x_2d.reshape((res_y, res_x, 1, len(kx_vector)))
 
             exp_K = torch.exp(x_2d)
             exp_K = exp_K.reshape((res_y, res_x, -1))
@@ -127,15 +129,15 @@
 
 
 def field_dist_2d_vectorized_ji(wavelength, kx_vector, n_I, theta, phi, fourier_order_x, fourier_order_y, T1, layer_info_list, period,
                                 res_x=20, res_y=20, res_z=20, device='cpu', type_complex=torch.complex128, type_float=torch.float64):
 
     k0 = 2 * torch.pi / wavelength
 
-    fourier_indices_y = torch.arange(-fourier_order_y, fourier_order_y + 1, dtype=type_float)
+    fourier_indices_y = torch.arange(-fourier_order_y, fourier_order_y + 1, dtype=type_float, device=device)
     ff_x = fourier_order_x * 2 + 1
     ff_y = fourier_order_y * 2 + 1
     ky_vector = k0 * (n_I * torch.sin(theta) * torch.sin(phi) + fourier_indices_y * (
             wavelength / period[1])).type(type_complex)
 
     Kx = torch.diag(torch.tile(kx_vector, (ff_y, )).flatten()) / k0
     Ky = torch.diag(torch.tile(ky_vector.reshape((-1, 1)), (ff_x, )).flatten()) / k0
@@ -151,16 +153,16 @@
             in enumerate(layer_info_list[::-1]):
 
         c = torch.cat([big_I, big_B @ big_A_i @ big_X])  @ T_layer
 
         for k in range(res_z):
             Sx, Sy, Ux, Uy, Sz, Uz = z_loop_2d(k, c, k0, Kx, Ky, res_z, E_conv_i, q, W_11, W_12, W_21, W_22, V_11, V_12, V_21, V_22, d)
 
-            x_1d = torch.arange(res_x, dtype=type_float).reshape((1, -1, 1))
-            y_1d = torch.arange(res_y, dtype=type_float).reshape((-1, 1, 1))
+            x_1d = torch.arange(res_x, dtype=type_float, device=device).reshape((1, -1, 1))
+            y_1d = torch.arange(res_y, dtype=type_float, device=device).reshape((-1, 1, 1))
 
             x_1d = -1j * x_1d * period[0] / res_x
             y_1d = -1j * y_1d * period[1] / res_y
 
             x_2d = torch.tile(x_1d, (res_y, 1, 1))
             y_2d = torch.tile(y_1d, (1, res_x, 1))
 
@@ -187,15 +189,16 @@
 
         T_layer = big_A_i @ big_X @ T_layer
 
     return field_cell
 
 
 def field_dist_1d_vectorized_kji(wavelength, kx_vector, T1, layer_info_list, period,
-                                 pol, res_x=20, res_y=20, res_z=20, type_complex=torch.complex128, type_float=torch.float64):
+                                 pol, res_x=20, res_y=20, res_z=20,  device='cpu',
+                                 type_complex=torch.complex128, type_float=torch.float64):
 
     k0 = 2 * torch.pi / wavelength
     Kx = torch.diag(kx_vector / k0)
 
     field_cell = torch.zeros((res_z * len(layer_info_list), res_y, res_x, 3), dtype=type_complex)
 
     T_layer = T1
@@ -212,22 +215,22 @@
             V = W @ Q
             EKx = None
 
         else:
             V = E_conv_i @ W @ Q
             EKx = E_conv_i @ Kx
 
-        z_1d = torch.arange(res_z, dtype=type_float).reshape((-1, 1, 1)) / res_z * d
+        z_1d = torch.arange(res_z, dtype=type_float, device=device).reshape((-1, 1, 1)) / res_z * d
 
         if pol == 0:
             Sy = W @ (diag_exp_batch(-k0 * Q * z_1d) @ c1 + diag_exp_batch(k0 * Q * (z_1d - d)) @ c2)
             Ux = V @ (-diag_exp_batch(-k0 * Q * z_1d) @ c1 + diag_exp_batch(k0 * Q * (z_1d - d)) @ c2)
             C = Kx @ Sy
 
-            x_1d = torch.arange(res_x, dtype=type_float).reshape((1, -1, 1))
+            x_1d = torch.arange(res_x, dtype=type_float, device=device).reshape((1, -1, 1))
             x_1d = -1j * x_1d * period[0] / res_x
             x_2d = torch.tile(x_1d, (res_y, 1, 1))
             x_2d = x_2d * kx_vector
             x_2d = x_2d.reshape((res_y, res_x, 1, len(kx_vector)))
 
             exp_K = torch.exp(x_2d)
             exp_K = exp_K.reshape((res_y, res_x, -1))
@@ -240,15 +243,15 @@
 
         else:
             Uy = W @ (diag_exp_batch(-k0 * Q * z_1d) @ c1 + diag_exp_batch(k0 * Q * (z_1d - d)) @ c2)
             Sx = V @ (-diag_exp_batch(-k0 * Q * z_1d) @ c1 + diag_exp_batch(k0 * Q * (z_1d - d)) @ c2)
 
             C = EKx @ Uy  # there is a better option for convergence
 
-            x_1d = torch.arange(res_x, dtype=type_float).reshape((1, -1, 1))
+            x_1d = torch.arange(res_x, dtype=type_float, device=device).reshape((1, -1, 1))
             x_1d = -1j * x_1d * period[0] / res_x
             x_2d = torch.tile(x_1d, (res_y, 1, 1))
             x_2d = x_2d * kx_vector
             x_2d = x_2d.reshape((res_y, res_x, 1, len(kx_vector)))
 
             exp_K = torch.exp(x_2d)
             exp_K = exp_K.reshape((res_y, res_x, -1))
@@ -281,15 +284,15 @@
 
     # From the first layer
     for idx_layer, [E_conv_i, q_1, q_2, W_1, W_2, V_11, V_12, V_21, V_22, big_X, big_A_i, big_B, d] \
             in enumerate(layer_info_list[::-1]):
 
         c = torch.cat([big_I, big_B @ big_A_i @ big_X])  @ T_layer
 
-        z_1d = torch.arange(res_z, dtype=type_float).reshape((-1, 1, 1)) / res_z * d
+        z_1d = torch.arange(res_z, dtype=type_float, device=device).reshape((-1, 1, 1)) / res_z * d
 
         ff = len(c) // 4
 
         c1_plus = c[0 * ff:1 * ff]
         c2_plus = c[1 * ff:2 * ff]
         c1_minus = c[2 * ff:3 * ff]
         c2_minus = c[3 * ff:4 * ff]
@@ -306,15 +309,15 @@
 
         Uy = V_21 @ (-diag_exp_batch(-k0 * big_Q1 * z_1d) @ c1_plus + diag_exp_batch(k0 * big_Q1 * (z_1d - d)) @ c1_minus) \
              + V_22 @ (-diag_exp_batch(-k0 * big_Q2 * z_1d) @ c2_plus + diag_exp_batch(k0 * big_Q2 * (z_1d - d)) @ c2_minus)
 
         Sz = -1j * E_conv_i @ (Kx @ Uy - ky * Ux)
         Uz = -1j * (Kx @ Sy - ky * Sx)
 
-        x_1d = torch.arange(res_x, dtype=type_float).reshape((1, -1, 1))
+        x_1d = torch.arange(res_x, dtype=type_float, device=device).reshape((1, -1, 1))
         x_1d = -1j * x_1d * period[0] / res_x
         x_2d = torch.tile(x_1d, (res_y, 1, 1))
         x_2d = x_2d * kx_vector
         x_2d = x_2d.reshape((res_y, res_x, 1, len(kx_vector)))
 
         exp_K = torch.exp(x_2d)
         exp_K = exp_K.reshape((res_y, res_x, -1))
@@ -336,15 +339,15 @@
 
 
 def field_dist_2d_vectorized_kji(wavelength, kx_vector, n_I, theta, phi, fourier_order_x, fourier_order_y, T1, layer_info_list, period,
                                  res_x=20, res_y=20, res_z=20, device='cpu', type_complex=torch.complex128, type_float=torch.float64):
 
     k0 = 2 * torch.pi / wavelength
 
-    fourier_indices_y = torch.arange(-fourier_order_y, fourier_order_y + 1, dtype=type_float)
+    fourier_indices_y = torch.arange(-fourier_order_y, fourier_order_y + 1, dtype=type_float, device=device)
     ff_x = fourier_order_x * 2 + 1
     ff_y = fourier_order_y * 2 + 1
     ky_vector = k0 * (n_I * torch.sin(theta) * torch.sin(phi) + fourier_indices_y * (
             wavelength / period[1])).type(type_complex)
 
     Kx = torch.diag(torch.tile(kx_vector, (ff_y, )).flatten()) / k0
     Ky = torch.diag(torch.tile(ky_vector.reshape((-1, 1)), (ff_x, )).flatten()) / k0
@@ -356,28 +359,27 @@
     big_I = torch.eye((len(T1)), device=device).type(type_complex)
 
     # From the first layer
     for idx_layer, (E_conv_i, q, W_11, W_12, W_21, W_22, V_11, V_12, V_21, V_22, big_X, big_A_i, big_B, d)\
             in enumerate(layer_info_list[::-1]):
 
         c = torch.cat([big_I, big_B @ big_A_i @ big_X])  @ T_layer
-        z_1d = torch.arange(res_z, dtype=type_float).reshape((-1, 1, 1)) / res_z * d
+        z_1d = torch.arange(res_z, dtype=type_float, device=device).reshape((-1, 1, 1)) / res_z * d
 
         ff = len(c) // 4
 
         c1_plus = c[0 * ff:1 * ff]
         c2_plus = c[1 * ff:2 * ff]
         c1_minus = c[2 * ff:3 * ff]
         c2_minus = c[3 * ff:4 * ff]
 
         q1 = q[:len(q) // 2]
         q2 = q[len(q) // 2:]
         big_Q1 = torch.diag(q1)
         big_Q2 = torch.diag(q2)
-
         Sx = W_11 @ (diag_exp_batch(-k0 * big_Q1 * z_1d) @ c1_plus + diag_exp_batch(k0 * big_Q1 * (z_1d - d)) @ c1_minus) \
               + W_12 @ (diag_exp_batch(-k0 * big_Q2 * z_1d) @ c2_plus + diag_exp_batch(k0 * big_Q2 * (z_1d - d)) @ c2_minus)
 
         Sy = W_21 @ (diag_exp_batch(-k0 * big_Q1 * z_1d) @ c1_plus + diag_exp_batch(k0 * big_Q1 * (z_1d - d)) @ c1_minus) \
               + W_22 @ (diag_exp_batch(-k0 * big_Q2 * z_1d) @ c2_plus + diag_exp_batch(k0 * big_Q2 * (z_1d - d)) @ c2_minus)
 
         Ux = V_11 @ (-diag_exp_batch(-k0 * big_Q1 * z_1d) @ c1_plus + diag_exp_batch(k0 * big_Q1 * (z_1d - d)) @ c1_minus) \
@@ -385,16 +387,16 @@
 
         Uy = V_21 @ (-diag_exp_batch(-k0 * big_Q1 * z_1d) @ c1_plus + diag_exp_batch(k0 * big_Q1 * (z_1d - d)) @ c1_minus) \
               + V_22 @ (-diag_exp_batch(-k0 * big_Q2 * z_1d) @ c2_plus + diag_exp_batch(k0 * big_Q2 * (z_1d - d)) @ c2_minus)
 
         Sz = -1j * E_conv_i @ (Kx @ Uy - Ky @ Ux)
         Uz = -1j * (Kx @ Sy - Ky @ Sx)
 
-        x_1d = torch.arange(res_x, dtype=type_float).reshape((1, -1, 1))
-        y_1d = torch.arange(res_y, dtype=type_float).reshape((-1, 1, 1))
+        x_1d = torch.arange(res_x, dtype=type_float, device=device).reshape((1, -1, 1))
+        y_1d = torch.arange(res_y, dtype=type_float, device=device).reshape((-1, 1, 1))
 
         x_1d = -1j * x_1d * period[0] / res_x
         y_1d = -1j * y_1d * period[1] / res_y
 
         x_2d = torch.tile(x_1d, (res_y, 1, 1))
         y_2d = torch.tile(y_1d, (1, res_x, 1))
 
@@ -422,15 +424,15 @@
 
         T_layer = big_A_i @ big_X @ T_layer
 
     return field_cell
 
 
 def field_dist_1d_vanilla(wavelength, kx_vector, T1, layer_info_list, period, pol, res_x=20, res_y=20, res_z=20,
-                          type_complex=torch.complex128, *args, **kwargs):
+                          device='cpu', type_complex=torch.complex128, *args, **kwargs):
 
     k0 = 2 * torch.pi / wavelength
     Kx = torch.diag(kx_vector / k0)
 
     field_cell = torch.zeros((res_z * len(layer_info_list), res_y, res_x, 3)).type(type_complex)
 
     T_layer = T1
@@ -556,15 +558,15 @@
 
 def field_dist_2d_vanilla(wavelength, kx_vector, n_I, theta, phi, fourier_order_x, fourier_order_y, T1, layer_info_list,
                           period, res_x=20, res_y=20, res_z=20,
                           device='cpu', type_complex=torch.complex128, type_float=torch.float64):
 
     k0 = 2 * torch.pi / wavelength
 
-    fourier_indices_y = torch.arange(-fourier_order_y, fourier_order_y + 1, dtype=type_float)
+    fourier_indices_y = torch.arange(-fourier_order_y, fourier_order_y + 1, dtype=type_float, device=device)
     ff_x = fourier_order_x * 2 + 1
     ff_y = fourier_order_y * 2 + 1
     ky_vector = k0 * (n_I * torch.sin(theta) * torch.sin(phi) + fourier_indices_y * (
             wavelength / period[1])).type(type_complex)
 
     Kx = torch.diag(kx_vector.tile(ff_y).flatten()) / k0
     Ky = torch.diag(ky_vector.reshape((-1, 1)).tile(ff_x).flatten() / k0)
@@ -675,16 +677,16 @@
 
 
 def diag_exp(x):
     return torch.diag(torch.exp(torch.diag(x)))
 
 
 def diag_exp_batch(x):
-    res = torch.zeros(x.shape, dtype=x.dtype)
-    ix = torch.arange(x.shape[-1])
+    res = torch.zeros(x.shape, device=x.device, dtype=x.dtype)
+    ix = torch.arange(x.shape[-1], device=x.device)
     res[:, ix, ix] = torch.exp(x[:, ix, ix])
     return res
 
 
 def z_loop_1d_conical(k, c, k0, Kx, ky, res_z, E_conv_i, q_1, q_2, W_1, W_2, V_11, V_12, V_21, V_22, d):
 
     z = k / res_z * d
```

### Comparing `meent-0.9.1/meent/on_torch/emsolver/primitives.py` & `meent-0.9.2/meent/on_torch/emsolver/primitives.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/meent/on_torch/emsolver/rcwa.py` & `meent-0.9.2/meent/on_torch/emsolver/rcwa.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,24 +128,25 @@
     def calculate_field(self, res_x=20, res_y=20, res_z=20, field_algo=2):
         if self.grating_type == 0:
             res_y = 1
             if field_algo == 0:
                 field_cell = field_dist_1d_vanilla(self.wavelength, self.kx_vector,
                                                    self.T1, self.layer_info_list, self.period, self.pol,
                                                    res_x=res_x, res_y=res_y, res_z=res_z,
-                                                   type_complex=self.type_complex)
+                                                   device=self.device, type_complex=self.type_complex)
             elif field_algo == 1:
                 field_cell = field_dist_1d_vectorized_ji(self.wavelength, self.kx_vector, self.T1, self.layer_info_list,
                                                          self.period, self.pol, res_x=res_x, res_y=res_y, res_z=res_z,
-                                                         type_complex=self.type_complex, type_float=self.type_float)
+                                                         device=self.device, type_complex=self.type_complex,
+                                                         type_float=self.type_float)
             elif field_algo == 2:
                 field_cell = field_dist_1d_vectorized_kji(self.wavelength, self.kx_vector, self.T1,
                                                           self.layer_info_list, self.period, self.pol,
                                                           res_x=res_x, res_y=res_y, res_z=res_z,
-                                                          type_complex=self.type_complex,
+                                                          device=self.device, type_complex=self.type_complex,
                                                           type_float=self.type_float)
             else:
                 raise ValueError
         elif self.grating_type == 1:
             res_y = 1
             if field_algo == 0:
                 field_cell = field_dist_1d_conical_vanilla(self.wavelength, self.kx_vector, self.n_I, self.theta,
```

### Comparing `meent-0.9.1/meent/on_torch/emsolver/scattering_method.py` & `meent-0.9.2/meent/on_torch/emsolver/scattering_method.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/meent/on_torch/emsolver/smm_util.py` & `meent-0.9.2/meent/on_torch/emsolver/smm_util.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/meent/on_torch/emsolver/transfer_method.py` & `meent-0.9.2/meent/on_torch/emsolver/transfer_method.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/meent/on_torch/modeler/modeling.py` & `meent-0.9.2/meent/on_torch/modeler/modeling.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/meent/on_torch/optimizer/loss.py` & `meent-0.9.2/meent/on_torch/optimizer/loss.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/meent/on_torch/optimizer/optimizer.py` & `meent-0.9.2/meent/on_torch/optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/meent.egg-info/SOURCES.txt` & `meent-0.9.2/meent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meent-0.9.1/setup.py` & `meent-0.9.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
             ],
     'pytorch': ['torch>=2.0.0',
                 'tqdm>=4.64.1',
                 ],
 }
 setup(
     name='meent',
-    version='0.9.1',
+    version='0.9.2',
     url='https://github.com/kc-ml2/meent',
     author='KC ML2',
     author_email='yongha@kc-ml2.com',
     packages=['meent'] + find_packages(include=['meent.*']),
     install_requires=[
         'numpy>=1.23.3',
         'scipy>=1.9.1',
```

