# Comparing `tmp/lmfit-1.2.0.tar.gz` & `tmp/lmfit-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmfit-1.2.0.tar", last modified: Sat Apr  8 19:48:27 2023, max compression
+gzip compressed data, was "lmfit-1.2.1.tar", last modified: Tue May  2 17:52:43 2023, max compression
```

## Comparing `lmfit-1.2.0.tar` & `lmfit-1.2.1.tar`

### file list

```diff
@@ -1,203 +1,203 @@
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-04-08 19:48:27.419321 lmfit-1.2.0/
--rw-r--r--   0 Newville   (501) staff       (20)      308 2023-02-23 19:14:07.000000 lmfit-1.2.0/.codecov.yml
--rw-r--r--   0 Newville   (501) staff       (20)      393 2023-02-23 19:14:07.000000 lmfit-1.2.0/.gitattributes
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-04-08 19:48:27.388061 lmfit-1.2.0/.github/
--rw-r--r--   0 Newville   (501) staff       (20)     5158 2023-02-23 19:14:07.000000 lmfit-1.2.0/.github/CONTRIBUTING.md
--rw-r--r--   0 Newville   (501) staff       (20)     2465 2023-02-23 19:14:07.000000 lmfit-1.2.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 Newville   (501) staff       (20)     2211 2023-02-23 19:14:07.000000 lmfit-1.2.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 Newville   (501) staff       (20)      502 2023-02-23 19:14:07.000000 lmfit-1.2.0/.github/dependabot.yml
--rw-r--r--   0 Newville   (501) staff       (20)      323 2023-03-30 18:04:00.000000 lmfit-1.2.0/.gitignore
--rw-r--r--   0 Newville   (501) staff       (20)     1676 2023-03-30 18:04:00.000000 lmfit-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 Newville   (501) staff       (20)     3015 2023-02-23 19:14:07.000000 lmfit-1.2.0/AUTHORS.txt
--rw-r--r--   0 Newville   (501) staff       (20)     3670 2023-02-23 19:14:07.000000 lmfit-1.2.0/LICENSE
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-04-08 19:48:27.392814 lmfit-1.2.0/NIST_STRD/
--rw-r--r--   0 Newville   (501) staff       (20)     6869 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Bennett5.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1713 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/BoxBOD.dat
--rw-r--r--   0 Newville   (501) staff       (20)     7558 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Chwirut1.dat
--rw-r--r--   0 Newville   (501) staff       (20)     3060 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Chwirut2.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1990 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/DanWood.dat
--rw-r--r--   0 Newville   (501) staff       (20)     6761 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/ENSO.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2773 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Eckerle4.dat
--rw-r--r--   0 Newville   (501) staff       (20)     8098 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Gauss1.dat
--rw-r--r--   0 Newville   (501) staff       (20)     8100 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Gauss2.dat
--rw-r--r--   0 Newville   (501) staff       (20)     8102 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Gauss3.dat
--rw-r--r--   0 Newville   (501) staff       (20)     9276 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Hahn1.dat
--rw-r--r--   0 Newville   (501) staff       (20)     5858 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Kirby2.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2945 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Lanczos1.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2601 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Lanczos2.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2574 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Lanczos3.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2305 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/MGH09.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2335 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/MGH10.dat
--rw-r--r--   0 Newville   (501) staff       (20)     3078 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/MGH17.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1853 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Misra1a.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1845 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Misra1b.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1839 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Misra1c.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1843 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Misra1d.dat
--rw-r--r--   0 Newville   (501) staff       (20)     6401 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Models
--rw-r--r--   0 Newville   (501) staff       (20)     7001 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Nelson.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1873 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Rat42.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2072 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Rat43.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2486 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Roszman1.dat
--rw-r--r--   0 Newville   (501) staff       (20)     3026 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Thurber.dat
--rw-r--r--   0 Newville   (501) staff       (20)     5721 2023-04-08 19:48:27.419483 lmfit-1.2.0/PKG-INFO
--rw-r--r--   0 Newville   (501) staff       (20)     4220 2023-02-23 19:14:07.000000 lmfit-1.2.0/README.rst
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-04-08 19:48:27.393340 lmfit-1.2.0/asv_benchmarking/
--rw-r--r--   0 Newville   (501) staff       (20)       43 2023-02-23 19:14:07.000000 lmfit-1.2.0/asv_benchmarking/README.md
--rw-r--r--   0 Newville   (501) staff       (20)     2793 2023-02-23 19:14:07.000000 lmfit-1.2.0/asv_benchmarking/asv.conf.json
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-04-08 19:48:27.393653 lmfit-1.2.0/asv_benchmarking/benchmarks/
--rw-r--r--   0 Newville   (501) staff       (20)        0 2023-02-23 19:14:07.000000 lmfit-1.2.0/asv_benchmarking/benchmarks/__init__.py
--rw-r--r--   0 Newville   (501) staff       (20)     4394 2023-02-23 19:14:07.000000 lmfit-1.2.0/asv_benchmarking/benchmarks/benchmarks.py
--rw-r--r--   0 Newville   (501) staff       (20)      350 2023-02-23 19:14:07.000000 lmfit-1.2.0/asv_benchmarking/run_benchmark_code.py
--rw-r--r--   0 Newville   (501) staff       (20)    12176 2023-03-26 20:21:53.000000 lmfit-1.2.0/azure-pipelines.yml
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-04-08 19:48:27.397899 lmfit-1.2.0/doc/
--rw-r--r--   0 Newville   (501) staff       (20)     4386 2023-04-04 03:22:28.000000 lmfit-1.2.0/doc/Makefile
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-04-08 19:48:27.398268 lmfit-1.2.0/doc/_static/
--rw-r--r--   0 Newville   (501) staff       (20)        0 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/_static/empty
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-04-08 19:48:27.398392 lmfit-1.2.0/doc/_templates/
--rw-r--r--   0 Newville   (501) staff       (20)      756 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/_templates/indexsidebar.html
--rw-r--r--   0 Newville   (501) staff       (20)     3499 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/bounds.rst
--rw-r--r--   0 Newville   (501) staff       (20)    30647 2023-03-30 18:04:00.000000 lmfit-1.2.0/doc/builtin_models.rst
--rw-r--r--   0 Newville   (501) staff       (20)     6527 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/conf.py
--rw-r--r--   0 Newville   (501) staff       (20)    15659 2023-03-30 18:04:00.000000 lmfit-1.2.0/doc/confidence.rst
--rw-r--r--   0 Newville   (501) staff       (20)     8110 2023-03-30 18:04:00.000000 lmfit-1.2.0/doc/constraints.rst
--rw-r--r--   0 Newville   (501) staff       (20)      223 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/contents.rst
--rwxr-xr-x   0 Newville   (501) staff       (20)     1943 2023-04-04 02:11:28.000000 lmfit-1.2.0/doc/doc_examples_to_gallery.py
--rw-r--r--   0 Newville   (501) staff       (20)    12177 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/faq.rst
--rwxr-xr-x   0 Newville   (501) staff       (20)      660 2023-04-04 02:10:04.000000 lmfit-1.2.0/doc/filter_spurious_link_from_html.py
--rw-r--r--   0 Newville   (501) staff       (20)    34852 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/fitting.rst
--rw-r--r--   0 Newville   (501) staff       (20)     2915 2023-03-30 18:04:00.000000 lmfit-1.2.0/doc/index.rst
--rw-r--r--   0 Newville   (501) staff       (20)     5102 2023-03-30 18:04:00.000000 lmfit-1.2.0/doc/installation.rst
--rw-r--r--   0 Newville   (501) staff       (20)     9268 2023-03-30 18:04:00.000000 lmfit-1.2.0/doc/intro.rst
--rw-r--r--   0 Newville   (501) staff       (20)      941 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/make.bat
--rw-r--r--   0 Newville   (501) staff       (20)    43359 2023-04-04 03:22:28.000000 lmfit-1.2.0/doc/model.rst
--rw-r--r--   0 Newville   (501) staff       (20)     4611 2023-03-30 18:04:00.000000 lmfit-1.2.0/doc/parameters.rst
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-04-08 19:48:27.398767 lmfit-1.2.0/doc/sphinx/
--rw-r--r--   0 Newville   (501) staff       (20)      460 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/sphinx/ext_imgmath.py
--rw-r--r--   0 Newville   (501) staff       (20)      407 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/sphinx/ext_mathjax.py
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-04-08 19:48:27.384628 lmfit-1.2.0/doc/sphinx/theme/
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-04-08 19:48:27.399235 lmfit-1.2.0/doc/sphinx/theme/sphinx13/
--rw-r--r--   0 Newville   (501) staff       (20)     7546 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/sphinx/theme/sphinx13/basic_layout.html
--rw-r--r--   0 Newville   (501) staff       (20)     3080 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/sphinx/theme/sphinx13/layout.html
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-04-08 19:48:27.400444 lmfit-1.2.0/doc/sphinx/theme/sphinx13/static/
--rw-r--r--   0 Newville   (501) staff       (20)      429 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/sphinx/theme/sphinx13/static/bodybg.png
--rw-r--r--   0 Newville   (501) staff       (20)      180 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/sphinx/theme/sphinx13/static/footerbg.png
--rw-r--r--   0 Newville   (501) staff       (20)      189 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/sphinx/theme/sphinx13/static/headerbg.png
--rw-r--r--   0 Newville   (501) staff       (20)      149 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/sphinx/theme/sphinx13/static/listitem.png
--rw-r--r--   0 Newville   (501) staff       (20)     9907 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/sphinx/theme/sphinx13/static/lmfitheader.png
--rw-r--r--   0 Newville   (501) staff       (20)      183 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/sphinx/theme/sphinx13/static/relbg.png
--rw-r--r--   0 Newville   (501) staff       (20)     7978 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/sphinx/theme/sphinx13/static/sphinx13.css
--rw-r--r--   0 Newville   (501) staff       (20)       72 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/sphinx/theme/sphinx13/theme.conf
--rw-r--r--   0 Newville   (501) staff       (20)     1500 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/support.rst
--rw-r--r--   0 Newville   (501) staff       (20)    25910 2023-04-07 18:31:26.000000 lmfit-1.2.0/doc/whatsnew.rst
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-04-08 19:48:27.408328 lmfit-1.2.0/examples/
--rw-r--r--   0 Newville   (501) staff       (20)     8195 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/NIST_Gauss2.dat
--rw-r--r--   0 Newville   (501) staff       (20)      419 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/README.txt
--rw-r--r--   0 Newville   (501) staff       (20)     1419 2023-04-01 13:56:41.000000 lmfit-1.2.0/examples/doc_builtinmodels_nistgauss.py
--rw-r--r--   0 Newville   (501) staff       (20)     1010 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/doc_builtinmodels_nistgauss2.py
--rw-r--r--   0 Newville   (501) staff       (20)     1364 2023-04-07 18:31:26.000000 lmfit-1.2.0/examples/doc_builtinmodels_peakmodels.py
--rw-r--r--   0 Newville   (501) staff       (20)     1961 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/doc_builtinmodels_splinemodel.py
--rw-r--r--   0 Newville   (501) staff       (20)      784 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/doc_builtinmodels_stepmodel.py
--rw-r--r--   0 Newville   (501) staff       (20)     1964 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/doc_confidence_advanced.py
--rw-r--r--   0 Newville   (501) staff       (20)      481 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/doc_confidence_basic.py
--rw-r--r--   0 Newville   (501) staff       (20)     3850 2023-04-01 13:56:41.000000 lmfit-1.2.0/examples/doc_confidence_chi2_maps.py
--rw-r--r--   0 Newville   (501) staff       (20)     3359 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/doc_fitting_emcee.py
--rw-r--r--   0 Newville   (501) staff       (20)      969 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/doc_fitting_withreport.py
--rw-r--r--   0 Newville   (501) staff       (20)     1953 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/doc_model_composite.py
--rw-r--r--   0 Newville   (501) staff       (20)      651 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/doc_model_gaussian.py
--rw-r--r--   0 Newville   (501) staff       (20)      774 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/doc_model_loadmodel.py
--rw-r--r--   0 Newville   (501) staff       (20)      531 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/doc_model_loadmodelresult.py
--rw-r--r--   0 Newville   (501) staff       (20)      537 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/doc_model_loadmodelresult2.py
--rw-r--r--   0 Newville   (501) staff       (20)      337 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/doc_model_savemodel.py
--rw-r--r--   0 Newville   (501) staff       (20)      423 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/doc_model_savemodelresult.py
--rw-r--r--   0 Newville   (501) staff       (20)      996 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/doc_model_savemodelresult2.py
--rw-r--r--   0 Newville   (501) staff       (20)      862 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/doc_model_two_components.py
--rw-r--r--   0 Newville   (501) staff       (20)      834 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/doc_model_uncertainty.py
--rw-r--r--   0 Newville   (501) staff       (20)     3148 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/doc_model_uncertainty2.py
--rw-r--r--   0 Newville   (501) staff       (20)     1051 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/doc_model_with_iter_callback.py
--rw-r--r--   0 Newville   (501) staff       (20)      775 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/doc_model_with_nan_policy.py
--rw-r--r--   0 Newville   (501) staff       (20)     1499 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/doc_parameters_basic.py
--rw-r--r--   0 Newville   (501) staff       (20)     1252 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/doc_parameters_valuesdict.py
--rw-r--r--   0 Newville   (501) staff       (20)     7666 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/example_Model_interface.py
--rw-r--r--   0 Newville   (501) staff       (20)    17926 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/example_brute.py
--rw-r--r--   0 Newville   (501) staff       (20)     4731 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/example_complex_resonator_model.py
--rw-r--r--   0 Newville   (501) staff       (20)     4378 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/example_confidence_interval.py
--rw-r--r--   0 Newville   (501) staff       (20)     3331 2023-03-25 15:55:57.000000 lmfit-1.2.0/examples/example_detect_outliers.py
--rw-r--r--   0 Newville   (501) staff       (20)     1795 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/example_diffev.py
--rw-r--r--   0 Newville   (501) staff       (20)     4098 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/example_emcee_Model_interface.py
--rw-r--r--   0 Newville   (501) staff       (20)     1273 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/example_expression_model.py
--rw-r--r--   0 Newville   (501) staff       (20)     2716 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/example_fit_multi_datasets.py
--rw-r--r--   0 Newville   (501) staff       (20)     1417 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/example_fit_with_algebraic_constraint.py
--rw-r--r--   0 Newville   (501) staff       (20)     2161 2023-04-01 13:56:41.000000 lmfit-1.2.0/examples/example_fit_with_bounds.py
--rw-r--r--   0 Newville   (501) staff       (20)     2666 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/example_fit_with_derivfunc.py
--rw-r--r--   0 Newville   (501) staff       (20)     2190 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/example_fit_with_inequality.py
--rw-r--r--   0 Newville   (501) staff       (20)     2378 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/example_reduce_fcn.py
--rw-r--r--   0 Newville   (501) staff       (20)     2915 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/example_sympy.py
--rw-r--r--   0 Newville   (501) staff       (20)     6112 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/example_two_dimensional_peak.py
--rw-r--r--   0 Newville   (501) staff       (20)      851 2023-04-04 02:16:59.000000 lmfit-1.2.0/examples/example_use_pandas.py
--rw-r--r--   0 Newville   (501) staff       (20)     7776 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/lmfit_emcee_model_selection.py
--rw-r--r--   0 Newville   (501) staff       (20)     2373 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/model1d_gauss.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1987 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/peak.csv
--rw-r--r--   0 Newville   (501) staff       (20)     2464 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/sinedata.dat
--rw-r--r--   0 Newville   (501) staff       (20)     9496 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/test_peak.dat
--rw-r--r--   0 Newville   (501) staff       (20)    11611 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/test_splinepeak.dat
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-04-08 19:48:27.411539 lmfit-1.2.0/lmfit/
--rw-r--r--   0 Newville   (501) staff       (20)     1956 2023-03-30 18:04:00.000000 lmfit-1.2.0/lmfit/__init__.py
--rw-r--r--   0 Newville   (501) staff       (20)    10016 2023-02-23 19:14:07.000000 lmfit-1.2.0/lmfit/_ampgo.py
--rw-r--r--   0 Newville   (501) staff       (20)    15312 2023-04-01 13:56:41.000000 lmfit-1.2.0/lmfit/confidence.py
--rw-r--r--   0 Newville   (501) staff       (20)     4808 2023-02-23 19:14:07.000000 lmfit-1.2.0/lmfit/jsonutils.py
--rw-r--r--   0 Newville   (501) staff       (20)    16911 2023-02-23 19:14:07.000000 lmfit-1.2.0/lmfit/lineshapes.py
--rw-r--r--   0 Newville   (501) staff       (20)   105393 2023-04-01 13:56:41.000000 lmfit-1.2.0/lmfit/minimizer.py
--rw-r--r--   0 Newville   (501) staff       (20)    84175 2023-04-01 14:38:49.000000 lmfit-1.2.0/lmfit/model.py
--rw-r--r--   0 Newville   (501) staff       (20)    65998 2023-02-24 16:55:16.000000 lmfit-1.2.0/lmfit/models.py
--rw-r--r--   0 Newville   (501) staff       (20)    36709 2023-04-07 18:31:26.000000 lmfit-1.2.0/lmfit/parameter.py
--rw-r--r--   0 Newville   (501) staff       (20)    15394 2023-04-01 13:56:41.000000 lmfit-1.2.0/lmfit/printfuncs.py
--rw-r--r--   0 Newville   (501) staff       (20)      160 2023-04-08 19:48:27.000000 lmfit-1.2.0/lmfit/version.py
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-04-08 19:48:27.412183 lmfit-1.2.0/lmfit.egg-info/
--rw-r--r--   0 Newville   (501) staff       (20)     5721 2023-04-08 19:48:27.000000 lmfit-1.2.0/lmfit.egg-info/PKG-INFO
--rw-r--r--   0 Newville   (501) staff       (20)     4971 2023-04-08 19:48:27.000000 lmfit-1.2.0/lmfit.egg-info/SOURCES.txt
--rw-r--r--   0 Newville   (501) staff       (20)        1 2023-04-08 19:48:27.000000 lmfit-1.2.0/lmfit.egg-info/dependency_links.txt
--rw-r--r--   0 Newville   (501) staff       (20)      685 2023-04-08 19:48:27.000000 lmfit-1.2.0/lmfit.egg-info/requires.txt
--rw-r--r--   0 Newville   (501) staff       (20)        6 2023-04-08 19:48:27.000000 lmfit-1.2.0/lmfit.egg-info/top_level.txt
--rwxr-xr-x   0 Newville   (501) staff       (20)     1010 2023-02-23 19:14:07.000000 lmfit-1.2.0/publish_docs.sh
--rw-r--r--   0 Newville   (501) staff       (20)      202 2023-02-23 19:14:07.000000 lmfit-1.2.0/pyproject.toml
--rw-r--r--   0 Newville   (501) staff       (20)     2456 2023-04-08 19:48:27.420089 lmfit-1.2.0/setup.cfg
--rw-r--r--   0 Newville   (501) staff       (20)       92 2023-02-23 19:14:07.000000 lmfit-1.2.0/setup.py
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-04-08 19:48:27.419186 lmfit-1.2.0/tests/
--rw-r--r--   0 Newville   (501) staff       (20)     6109 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/NISTModels.py
--rw-r--r--   0 Newville   (501) staff       (20)        0 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/__init__.py
--rw-r--r--   0 Newville   (501) staff       (20)      893 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/conftest.py
--rw-r--r--   0 Newville   (501) staff       (20)     5656 2023-03-30 18:04:00.000000 lmfit-1.2.0/tests/gauss_modelresult_lmfit100.sav
--rw-r--r--   0 Newville   (501) staff       (20)     1374 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_1variable.py
--rw-r--r--   0 Newville   (501) staff       (20)     7097 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_NIST_Strd.py
--rw-r--r--   0 Newville   (501) staff       (20)     3951 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_algebraic_constraint.py
--rw-r--r--   0 Newville   (501) staff       (20)     5193 2023-03-30 18:04:00.000000 lmfit-1.2.0/tests/test_ampgo.py
--rw-r--r--   0 Newville   (501) staff       (20)     1238 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_basicfit.py
--rw-r--r--   0 Newville   (501) staff       (20)     3911 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_basinhopping.py
--rw-r--r--   0 Newville   (501) staff       (20)     1900 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_bounded_jacobian.py
--rw-r--r--   0 Newville   (501) staff       (20)     1413 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_bounds.py
--rw-r--r--   0 Newville   (501) staff       (20)    11428 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_brute.py
--rw-r--r--   0 Newville   (501) staff       (20)    11953 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_builtin_models.py
--rw-r--r--   0 Newville   (501) staff       (20)     9251 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_confidence.py
--rw-r--r--   0 Newville   (501) staff       (20)     9987 2023-04-01 13:56:41.000000 lmfit-1.2.0/tests/test_covariance_matrix.py
--rw-r--r--   0 Newville   (501) staff       (20)     1235 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_custom_independentvar.py
--rw-r--r--   0 Newville   (501) staff       (20)      612 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_default_kws.py
--rw-r--r--   0 Newville   (501) staff       (20)     2595 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_dual_annealing.py
--rw-r--r--   0 Newville   (501) staff       (20)     4364 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_itercb.py
--rw-r--r--   0 Newville   (501) staff       (20)     3066 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_jsonutils.py
--rw-r--r--   0 Newville   (501) staff       (20)     6266 2023-03-30 18:04:00.000000 lmfit-1.2.0/tests/test_least_squares.py
--rw-r--r--   0 Newville   (501) staff       (20)     4804 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_lineshapes.py
--rw-r--r--   0 Newville   (501) staff       (20)      781 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_manypeaks_speed.py
--rw-r--r--   0 Newville   (501) staff       (20)     3689 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_max_nfev.py
--rw-r--r--   0 Newville   (501) staff       (20)      545 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_minimizer.py
--rw-r--r--   0 Newville   (501) staff       (20)    51749 2023-03-30 18:04:00.000000 lmfit-1.2.0/tests/test_model.py
--rw-r--r--   0 Newville   (501) staff       (20)    10484 2023-03-30 18:04:00.000000 lmfit-1.2.0/tests/test_model_saveload.py
--rw-r--r--   0 Newville   (501) staff       (20)     4354 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_model_uncertainties.py
--rw-r--r--   0 Newville   (501) staff       (20)     4965 2023-03-30 18:04:00.000000 lmfit-1.2.0/tests/test_models.py
--rw-r--r--   0 Newville   (501) staff       (20)     2181 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_multidatasets.py
--rw-r--r--   0 Newville   (501) staff       (20)    24031 2023-04-01 13:56:41.000000 lmfit-1.2.0/tests/test_nose.py
--rw-r--r--   0 Newville   (501) staff       (20)     1168 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_pandas.py
--rw-r--r--   0 Newville   (501) staff       (20)    19779 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_parameter.py
--rw-r--r--   0 Newville   (501) staff       (20)    21287 2023-04-07 18:31:26.000000 lmfit-1.2.0/tests/test_parameters.py
--rw-r--r--   0 Newville   (501) staff       (20)    14990 2023-04-01 13:56:41.000000 lmfit-1.2.0/tests/test_printfuncs.py
--rw-r--r--   0 Newville   (501) staff       (20)     4784 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_shgo.py
--rw-r--r--   0 Newville   (501) staff       (20)     1503 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_stepmodel.py
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-02 17:52:43.183141 lmfit-1.2.1/
+-rw-r--r--   0 Newville   (501) staff       (20)      308 2023-04-18 14:52:43.000000 lmfit-1.2.1/.codecov.yml
+-rw-r--r--   0 Newville   (501) staff       (20)      393 2023-04-18 14:52:43.000000 lmfit-1.2.1/.gitattributes
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-02 17:52:43.150931 lmfit-1.2.1/.github/
+-rw-r--r--   0 Newville   (501) staff       (20)     5158 2023-04-18 14:52:43.000000 lmfit-1.2.1/.github/CONTRIBUTING.md
+-rw-r--r--   0 Newville   (501) staff       (20)     2465 2023-04-18 14:52:43.000000 lmfit-1.2.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 Newville   (501) staff       (20)     2211 2023-04-18 14:52:43.000000 lmfit-1.2.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 Newville   (501) staff       (20)      502 2023-04-18 14:52:43.000000 lmfit-1.2.1/.github/dependabot.yml
+-rw-r--r--   0 Newville   (501) staff       (20)      323 2023-04-18 14:52:43.000000 lmfit-1.2.1/.gitignore
+-rw-r--r--   0 Newville   (501) staff       (20)     1676 2023-05-02 16:08:38.000000 lmfit-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 Newville   (501) staff       (20)     3015 2023-04-18 14:52:43.000000 lmfit-1.2.1/AUTHORS.txt
+-rw-r--r--   0 Newville   (501) staff       (20)     3670 2023-04-18 14:52:43.000000 lmfit-1.2.1/LICENSE
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-02 17:52:43.158832 lmfit-1.2.1/NIST_STRD/
+-rw-r--r--   0 Newville   (501) staff       (20)     6869 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Bennett5.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1713 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/BoxBOD.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     7558 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Chwirut1.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     3060 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Chwirut2.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1990 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/DanWood.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     6761 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/ENSO.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2773 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Eckerle4.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     8098 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Gauss1.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     8100 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Gauss2.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     8102 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Gauss3.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     9276 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Hahn1.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     5858 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Kirby2.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2945 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Lanczos1.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2601 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Lanczos2.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2574 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Lanczos3.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2305 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/MGH09.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2335 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/MGH10.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     3078 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/MGH17.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1853 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Misra1a.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1845 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Misra1b.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1839 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Misra1c.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1843 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Misra1d.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     6401 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Models
+-rw-r--r--   0 Newville   (501) staff       (20)     7001 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Nelson.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1873 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Rat42.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2072 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Rat43.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2486 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Roszman1.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     3026 2023-04-18 14:52:43.000000 lmfit-1.2.1/NIST_STRD/Thurber.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     7730 2023-05-02 17:52:43.183287 lmfit-1.2.1/PKG-INFO
+-rw-r--r--   0 Newville   (501) staff       (20)     6229 2023-04-22 17:52:19.000000 lmfit-1.2.1/README.rst
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-02 17:52:43.159329 lmfit-1.2.1/asv_benchmarking/
+-rw-r--r--   0 Newville   (501) staff       (20)       43 2023-04-18 14:52:43.000000 lmfit-1.2.1/asv_benchmarking/README.md
+-rw-r--r--   0 Newville   (501) staff       (20)     2793 2023-04-18 14:52:43.000000 lmfit-1.2.1/asv_benchmarking/asv.conf.json
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-02 17:52:43.159580 lmfit-1.2.1/asv_benchmarking/benchmarks/
+-rw-r--r--   0 Newville   (501) staff       (20)        0 2023-04-18 14:52:43.000000 lmfit-1.2.1/asv_benchmarking/benchmarks/__init__.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4394 2023-04-18 14:52:43.000000 lmfit-1.2.1/asv_benchmarking/benchmarks/benchmarks.py
+-rw-r--r--   0 Newville   (501) staff       (20)      350 2023-04-18 14:52:43.000000 lmfit-1.2.1/asv_benchmarking/run_benchmark_code.py
+-rw-r--r--   0 Newville   (501) staff       (20)    12176 2023-05-02 16:08:38.000000 lmfit-1.2.1/azure-pipelines.yml
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-02 17:52:43.162399 lmfit-1.2.1/doc/
+-rw-r--r--   0 Newville   (501) staff       (20)     4386 2023-05-02 17:31:02.000000 lmfit-1.2.1/doc/Makefile
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-02 17:52:43.162548 lmfit-1.2.1/doc/_static/
+-rw-r--r--   0 Newville   (501) staff       (20)        0 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/_static/empty
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-02 17:52:43.162675 lmfit-1.2.1/doc/_templates/
+-rw-r--r--   0 Newville   (501) staff       (20)      756 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/_templates/indexsidebar.html
+-rw-r--r--   0 Newville   (501) staff       (20)     3499 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/bounds.rst
+-rw-r--r--   0 Newville   (501) staff       (20)    30647 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/builtin_models.rst
+-rw-r--r--   0 Newville   (501) staff       (20)     6527 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/conf.py
+-rw-r--r--   0 Newville   (501) staff       (20)    15659 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/confidence.rst
+-rw-r--r--   0 Newville   (501) staff       (20)     8110 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/constraints.rst
+-rw-r--r--   0 Newville   (501) staff       (20)      223 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/contents.rst
+-rwxr-xr-x   0 Newville   (501) staff       (20)     1943 2023-05-02 17:29:24.000000 lmfit-1.2.1/doc/doc_examples_to_gallery.py
+-rw-r--r--   0 Newville   (501) staff       (20)    12177 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/faq.rst
+-rw-r--r--   0 Newville   (501) staff       (20)    34852 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/fitting.rst
+-rw-r--r--   0 Newville   (501) staff       (20)     2915 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/index.rst
+-rw-r--r--   0 Newville   (501) staff       (20)     5102 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/installation.rst
+-rw-r--r--   0 Newville   (501) staff       (20)     9268 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/intro.rst
+-rw-r--r--   0 Newville   (501) staff       (20)      941 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/make.bat
+-rw-r--r--   0 Newville   (501) staff       (20)    43609 2023-05-02 17:45:23.000000 lmfit-1.2.1/doc/model.rst
+-rw-r--r--   0 Newville   (501) staff       (20)     4611 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/parameters.rst
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-02 17:52:43.162956 lmfit-1.2.1/doc/sphinx/
+-rw-r--r--   0 Newville   (501) staff       (20)      460 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/sphinx/ext_imgmath.py
+-rw-r--r--   0 Newville   (501) staff       (20)      407 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/sphinx/ext_mathjax.py
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-02 17:52:43.145809 lmfit-1.2.1/doc/sphinx/theme/
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-02 17:52:43.163376 lmfit-1.2.1/doc/sphinx/theme/sphinx13/
+-rw-r--r--   0 Newville   (501) staff       (20)     7546 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/sphinx/theme/sphinx13/basic_layout.html
+-rw-r--r--   0 Newville   (501) staff       (20)     3080 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/sphinx/theme/sphinx13/layout.html
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-02 17:52:43.164427 lmfit-1.2.1/doc/sphinx/theme/sphinx13/static/
+-rw-r--r--   0 Newville   (501) staff       (20)      429 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/sphinx/theme/sphinx13/static/bodybg.png
+-rw-r--r--   0 Newville   (501) staff       (20)      180 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/sphinx/theme/sphinx13/static/footerbg.png
+-rw-r--r--   0 Newville   (501) staff       (20)      189 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/sphinx/theme/sphinx13/static/headerbg.png
+-rw-r--r--   0 Newville   (501) staff       (20)      149 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/sphinx/theme/sphinx13/static/listitem.png
+-rw-r--r--   0 Newville   (501) staff       (20)     9907 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/sphinx/theme/sphinx13/static/lmfitheader.png
+-rw-r--r--   0 Newville   (501) staff       (20)      183 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/sphinx/theme/sphinx13/static/relbg.png
+-rw-r--r--   0 Newville   (501) staff       (20)     7978 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/sphinx/theme/sphinx13/static/sphinx13.css
+-rw-r--r--   0 Newville   (501) staff       (20)       72 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/sphinx/theme/sphinx13/theme.conf
+-rw-r--r--   0 Newville   (501) staff       (20)     1500 2023-04-18 14:52:43.000000 lmfit-1.2.1/doc/support.rst
+-rw-r--r--   0 Newville   (501) staff       (20)    26325 2023-05-02 16:14:37.000000 lmfit-1.2.1/doc/whatsnew.rst
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-02 17:52:43.172295 lmfit-1.2.1/examples/
+-rw-r--r--   0 Newville   (501) staff       (20)     8195 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/NIST_Gauss2.dat
+-rw-r--r--   0 Newville   (501) staff       (20)      419 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/README.txt
+-rw-r--r--   0 Newville   (501) staff       (20)     1419 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_builtinmodels_nistgauss.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1010 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_builtinmodels_nistgauss2.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1364 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_builtinmodels_peakmodels.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1961 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_builtinmodels_splinemodel.py
+-rw-r--r--   0 Newville   (501) staff       (20)      784 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_builtinmodels_stepmodel.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1964 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_confidence_advanced.py
+-rw-r--r--   0 Newville   (501) staff       (20)      481 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_confidence_basic.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3850 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_confidence_chi2_maps.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3359 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_fitting_emcee.py
+-rw-r--r--   0 Newville   (501) staff       (20)      969 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_fitting_withreport.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1953 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_model_composite.py
+-rw-r--r--   0 Newville   (501) staff       (20)      651 2023-04-30 01:28:00.000000 lmfit-1.2.1/examples/doc_model_gaussian.py
+-rw-r--r--   0 Newville   (501) staff       (20)      774 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_model_loadmodel.py
+-rw-r--r--   0 Newville   (501) staff       (20)      531 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_model_loadmodelresult.py
+-rw-r--r--   0 Newville   (501) staff       (20)      537 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_model_loadmodelresult2.py
+-rw-r--r--   0 Newville   (501) staff       (20)      337 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_model_savemodel.py
+-rw-r--r--   0 Newville   (501) staff       (20)      423 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_model_savemodelresult.py
+-rw-r--r--   0 Newville   (501) staff       (20)      996 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_model_savemodelresult2.py
+-rw-r--r--   0 Newville   (501) staff       (20)      862 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_model_two_components.py
+-rw-r--r--   0 Newville   (501) staff       (20)      834 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_model_uncertainty.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3148 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_model_uncertainty2.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1051 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_model_with_iter_callback.py
+-rw-r--r--   0 Newville   (501) staff       (20)      775 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_model_with_nan_policy.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1499 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_parameters_basic.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1252 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/doc_parameters_valuesdict.py
+-rw-r--r--   0 Newville   (501) staff       (20)     7666 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/example_Model_interface.py
+-rw-r--r--   0 Newville   (501) staff       (20)    17926 2023-05-02 16:08:13.000000 lmfit-1.2.1/examples/example_brute.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4731 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/example_complex_resonator_model.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4378 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/example_confidence_interval.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3331 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/example_detect_outliers.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1795 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/example_diffev.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4098 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/example_emcee_Model_interface.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1273 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/example_expression_model.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2716 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/example_fit_multi_datasets.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1417 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/example_fit_with_algebraic_constraint.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2161 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/example_fit_with_bounds.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2666 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/example_fit_with_derivfunc.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2190 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/example_fit_with_inequality.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2378 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/example_reduce_fcn.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2915 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/example_sympy.py
+-rw-r--r--   0 Newville   (501) staff       (20)     6112 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/example_two_dimensional_peak.py
+-rw-r--r--   0 Newville   (501) staff       (20)      851 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/example_use_pandas.py
+-rw-r--r--   0 Newville   (501) staff       (20)     7776 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/lmfit_emcee_model_selection.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2373 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/model1d_gauss.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1987 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/peak.csv
+-rw-r--r--   0 Newville   (501) staff       (20)     2464 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/sinedata.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     9496 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/test_peak.dat
+-rw-r--r--   0 Newville   (501) staff       (20)    11611 2023-04-18 14:52:43.000000 lmfit-1.2.1/examples/test_splinepeak.dat
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-02 17:52:43.175604 lmfit-1.2.1/lmfit/
+-rw-r--r--   0 Newville   (501) staff       (20)     1956 2023-04-18 14:52:43.000000 lmfit-1.2.1/lmfit/__init__.py
+-rw-r--r--   0 Newville   (501) staff       (20)    10016 2023-04-18 14:52:43.000000 lmfit-1.2.1/lmfit/_ampgo.py
+-rw-r--r--   0 Newville   (501) staff       (20)    21034 2023-04-26 01:48:37.000000 lmfit-1.2.1/lmfit/conf_emcee.py
+-rw-r--r--   0 Newville   (501) staff       (20)    15312 2023-04-18 14:52:43.000000 lmfit-1.2.1/lmfit/confidence.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4808 2023-04-18 14:52:43.000000 lmfit-1.2.1/lmfit/jsonutils.py
+-rw-r--r--   0 Newville   (501) staff       (20)    16911 2023-04-18 14:52:43.000000 lmfit-1.2.1/lmfit/lineshapes.py
+-rw-r--r--   0 Newville   (501) staff       (20)   105487 2023-05-02 16:07:56.000000 lmfit-1.2.1/lmfit/minimizer.py
+-rw-r--r--   0 Newville   (501) staff       (20)    84462 2023-05-02 16:08:38.000000 lmfit-1.2.1/lmfit/model.py
+-rw-r--r--   0 Newville   (501) staff       (20)    65998 2023-04-18 14:52:43.000000 lmfit-1.2.1/lmfit/models.py
+-rw-r--r--   0 Newville   (501) staff       (20)    36709 2023-04-18 14:52:43.000000 lmfit-1.2.1/lmfit/parameter.py
+-rw-r--r--   0 Newville   (501) staff       (20)    15394 2023-04-18 14:52:43.000000 lmfit-1.2.1/lmfit/printfuncs.py
+-rw-r--r--   0 Newville   (501) staff       (20)      160 2023-05-02 17:52:43.000000 lmfit-1.2.1/lmfit/version.py
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-02 17:52:43.176207 lmfit-1.2.1/lmfit.egg-info/
+-rw-r--r--   0 Newville   (501) staff       (20)     7730 2023-05-02 17:52:43.000000 lmfit-1.2.1/lmfit.egg-info/PKG-INFO
+-rw-r--r--   0 Newville   (501) staff       (20)     4953 2023-05-02 17:52:43.000000 lmfit-1.2.1/lmfit.egg-info/SOURCES.txt
+-rw-r--r--   0 Newville   (501) staff       (20)        1 2023-05-02 17:52:43.000000 lmfit-1.2.1/lmfit.egg-info/dependency_links.txt
+-rw-r--r--   0 Newville   (501) staff       (20)      669 2023-05-02 17:52:43.000000 lmfit-1.2.1/lmfit.egg-info/requires.txt
+-rw-r--r--   0 Newville   (501) staff       (20)        6 2023-05-02 17:52:43.000000 lmfit-1.2.1/lmfit.egg-info/top_level.txt
+-rwxr-xr-x   0 Newville   (501) staff       (20)     1010 2023-04-18 14:52:43.000000 lmfit-1.2.1/publish_docs.sh
+-rw-r--r--   0 Newville   (501) staff       (20)      202 2023-04-18 14:52:43.000000 lmfit-1.2.1/pyproject.toml
+-rw-r--r--   0 Newville   (501) staff       (20)     2447 2023-05-02 17:52:43.183892 lmfit-1.2.1/setup.cfg
+-rw-r--r--   0 Newville   (501) staff       (20)       92 2023-04-18 14:52:43.000000 lmfit-1.2.1/setup.py
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-05-02 17:52:43.183000 lmfit-1.2.1/tests/
+-rw-r--r--   0 Newville   (501) staff       (20)     6109 2023-04-18 14:52:43.000000 lmfit-1.2.1/tests/NISTModels.py
+-rw-r--r--   0 Newville   (501) staff       (20)        0 2023-04-18 14:52:43.000000 lmfit-1.2.1/tests/__init__.py
+-rw-r--r--   0 Newville   (501) staff       (20)      893 2023-04-18 14:52:43.000000 lmfit-1.2.1/tests/conftest.py
+-rw-r--r--   0 Newville   (501) staff       (20)     5656 2023-04-18 14:52:43.000000 lmfit-1.2.1/tests/gauss_modelresult_lmfit100.sav
+-rw-r--r--   0 Newville   (501) staff       (20)     1374 2023-04-18 14:52:43.000000 lmfit-1.2.1/tests/test_1variable.py
+-rw-r--r--   0 Newville   (501) staff       (20)     7097 2023-04-18 14:52:43.000000 lmfit-1.2.1/tests/test_NIST_Strd.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3951 2023-04-18 14:52:43.000000 lmfit-1.2.1/tests/test_algebraic_constraint.py
+-rw-r--r--   0 Newville   (501) staff       (20)     5063 2023-05-02 16:08:38.000000 lmfit-1.2.1/tests/test_ampgo.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1238 2023-04-18 14:52:43.000000 lmfit-1.2.1/tests/test_basicfit.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3911 2023-04-18 14:52:43.000000 lmfit-1.2.1/tests/test_basinhopping.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1900 2023-04-18 14:52:43.000000 lmfit-1.2.1/tests/test_bounded_jacobian.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1413 2023-04-18 14:52:43.000000 lmfit-1.2.1/tests/test_bounds.py
+-rw-r--r--   0 Newville   (501) staff       (20)    11428 2023-04-18 14:52:43.000000 lmfit-1.2.1/tests/test_brute.py
+-rw-r--r--   0 Newville   (501) staff       (20)    11953 2023-04-18 14:52:43.000000 lmfit-1.2.1/tests/test_builtin_models.py
+-rw-r--r--   0 Newville   (501) staff       (20)     9251 2023-04-18 14:52:43.000000 lmfit-1.2.1/tests/test_confidence.py
+-rw-r--r--   0 Newville   (501) staff       (20)     9987 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_covariance_matrix.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1235 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_custom_independentvar.py
+-rw-r--r--   0 Newville   (501) staff       (20)      612 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_default_kws.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2595 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_dual_annealing.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4364 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_itercb.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3066 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_jsonutils.py
+-rw-r--r--   0 Newville   (501) staff       (20)     6266 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_least_squares.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4804 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_lineshapes.py
+-rw-r--r--   0 Newville   (501) staff       (20)      781 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_manypeaks_speed.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3689 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_max_nfev.py
+-rw-r--r--   0 Newville   (501) staff       (20)      545 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_minimizer.py
+-rw-r--r--   0 Newville   (501) staff       (20)    52838 2023-05-02 16:08:38.000000 lmfit-1.2.1/tests/test_model.py
+-rw-r--r--   0 Newville   (501) staff       (20)    10484 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_model_saveload.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4354 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_model_uncertainties.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4965 2023-04-30 00:05:44.000000 lmfit-1.2.1/tests/test_models.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2181 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_multidatasets.py
+-rw-r--r--   0 Newville   (501) staff       (20)    24031 2023-05-02 16:26:12.000000 lmfit-1.2.1/tests/test_nose.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1168 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_pandas.py
+-rw-r--r--   0 Newville   (501) staff       (20)    19779 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_parameter.py
+-rw-r--r--   0 Newville   (501) staff       (20)    21287 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_parameters.py
+-rw-r--r--   0 Newville   (501) staff       (20)    14990 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_printfuncs.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4784 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_shgo.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1503 2023-04-18 14:52:44.000000 lmfit-1.2.1/tests/test_stepmodel.py
```

### Comparing `lmfit-1.2.0/.github/CONTRIBUTING.md` & `lmfit-1.2.1/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/.github/ISSUE_TEMPLATE.md` & `lmfit-1.2.1/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/.github/PULL_REQUEST_TEMPLATE.md` & `lmfit-1.2.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/.pre-commit-config.yaml` & `lmfit-1.2.1/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 exclude: 'doc/conf.py'
 
 repos:
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.3.2
     hooks:
     -   id: pyupgrade
         args: [--py37-plus]
 
 -   repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
```

### Comparing `lmfit-1.2.0/AUTHORS.txt` & `lmfit-1.2.1/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/LICENSE` & `lmfit-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/NIST_STRD/Bennett5.dat` & `lmfit-1.2.1/NIST_STRD/Bennett5.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/NIST_STRD/BoxBOD.dat` & `lmfit-1.2.1/NIST_STRD/BoxBOD.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/NIST_STRD/Chwirut1.dat` & `lmfit-1.2.1/NIST_STRD/Chwirut1.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/NIST_STRD/Chwirut2.dat` & `lmfit-1.2.1/NIST_STRD/Chwirut2.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/NIST_STRD/DanWood.dat` & `lmfit-1.2.1/NIST_STRD/DanWood.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/NIST_STRD/ENSO.dat` & `lmfit-1.2.1/NIST_STRD/ENSO.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/NIST_STRD/Eckerle4.dat` & `lmfit-1.2.1/NIST_STRD/Eckerle4.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/NIST_STRD/Gauss1.dat` & `lmfit-1.2.1/NIST_STRD/Gauss1.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/NIST_STRD/Gauss2.dat` & `lmfit-1.2.1/NIST_STRD/Gauss2.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/NIST_STRD/Gauss3.dat` & `lmfit-1.2.1/NIST_STRD/Gauss3.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/NIST_STRD/Hahn1.dat` & `lmfit-1.2.1/NIST_STRD/Hahn1.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/NIST_STRD/Kirby2.dat` & `lmfit-1.2.1/NIST_STRD/Kirby2.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/NIST_STRD/Lanczos1.dat` & `lmfit-1.2.1/NIST_STRD/Lanczos1.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/NIST_STRD/Lanczos2.dat` & `lmfit-1.2.1/NIST_STRD/Lanczos2.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/NIST_STRD/Lanczos3.dat` & `lmfit-1.2.1/NIST_STRD/Lanczos3.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/NIST_STRD/MGH09.dat` & `lmfit-1.2.1/NIST_STRD/MGH09.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/NIST_STRD/MGH10.dat` & `lmfit-1.2.1/NIST_STRD/MGH10.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/NIST_STRD/MGH17.dat` & `lmfit-1.2.1/NIST_STRD/MGH17.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/NIST_STRD/Misra1a.dat` & `lmfit-1.2.1/NIST_STRD/Misra1a.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/NIST_STRD/Misra1b.dat` & `lmfit-1.2.1/NIST_STRD/Misra1b.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/NIST_STRD/Misra1c.dat` & `lmfit-1.2.1/NIST_STRD/Misra1c.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/NIST_STRD/Misra1d.dat` & `lmfit-1.2.1/NIST_STRD/Misra1d.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/NIST_STRD/Models` & `lmfit-1.2.1/NIST_STRD/Models`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/NIST_STRD/Nelson.dat` & `lmfit-1.2.1/NIST_STRD/Nelson.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/NIST_STRD/Rat42.dat` & `lmfit-1.2.1/NIST_STRD/Rat42.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/NIST_STRD/Rat43.dat` & `lmfit-1.2.1/NIST_STRD/Rat43.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/NIST_STRD/Roszman1.dat` & `lmfit-1.2.1/NIST_STRD/Roszman1.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/NIST_STRD/Thurber.dat` & `lmfit-1.2.1/NIST_STRD/Thurber.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/README.rst` & `lmfit-1.2.1/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -13,61 +13,78 @@
 .. image:: https://img.shields.io/pypi/dm/lmfit.svg
    :target: https://pypi.org/project/lmfit
 
 .. image:: https://img.shields.io/badge/docs-read-brightgreen
    :target: https://lmfit.github.io/lmfit-py/
 
 .. image:: https://zenodo.org/badge/4185/lmfit/lmfit-py.svg
-   :target: https://zenodo.org/badge/latestdoi/4185/lmfit/lmfit-py
+   :target: https://doi.org/10.5281/zenodo.598352
 
-.. _LMfit mailing list: https://groups.google.com/group/lmfit-py
+.. _LMfit google mailing list: https://groups.google.com/group/lmfit-py
+.. _Github Discussions: https://github.com/lmfit/lmfit-py/discussions
+.. _Github Issues: https://github.com/lmfit/lmfit-py/issues
+
+
+..
+   Note: the Zenodo target should be
+   https://zenodo.org/badge/latestdoi/4185/lmfit/lmfit-py
+   but see https://github.com/lmfit/lmfit-py/discussions/862
 
 
 Overview
 ---------
 
-LMfit-py provides a Least-Squares Minimization routine and class with a simple,
-flexible approach to parameterizing a model for fitting to data.
+The lmfit Python library supports provides tools for non-linear least-squares
+minimization and curve fitting.  The goal is to make these optimization
+algorithms more flexible, more comprehensible, and easier to use well, with the
+key feature of casting variables in minimization and fitting routines as named
+parameters that can have many attributes beside just a current value.
+
+LMfit is a pure Python package, built on top of Scipy and Numpy, and so easy to
+install with ``pip install lmfit``.
+
+For questions, comments, and suggestions, please use the `LMfit google mailing
+list`_ or `Github discussions`_.  For software issues and bugs, use `Github
+Issues`_, but please read `Contributing.md <.github/CONTRIBUTING.md>`_ before
+creating an Issue.
+
+
+Parameters and Minimization
+------------------------------
+
+LMfit provides optimization routines similar to (and based on) those from
+``scipy.optimize``, but with a simple, flexible approach to parameterizing a
+model for fitting to data using named parameters. These named Parameters can be
+held fixed or freely adjusted in the fit, or held between lower and upper
+bounds. Parameters can also be constrained as a simple mathematical expression
+of other Parameters.
+
+A Parameters object (which acts like a Python dictionary) contains named
+parameters, and can be built as with::
+
+    import lmfit
+    fit_params = lmfit.Parameters()
+    fit_params['amp'] = lmfit.Parameter(value=1.2)
+    fit_params['cen'] = lmfit.Parameter(value=40.0, vary=False)
+    fit_params['wid'] = lmfit.Parameter(value=4, min=0)
+    fit_params['fwhm'] = lmfit.Parameter(expr='wid*2.355')
 
-LMfit is a pure Python package, and so easy to install from source or with
-``pip install lmfit``.
+or using the equivalent::
 
-For questions, comments, and suggestions, please use the `LMfit mailing list`_.
-Using the bug tracking software in GitHub Issues is encouraged for known
-problems and bug reports. Please read
-`Contributing.md <.github/CONTRIBUTING.md>`_ before creating an Issue.
-
-
-Parameters and Fitting
--------------------------
-
-LMfit-py provides a Least-Squares Minimization routine and class with a simple,
-flexible approach to parameterizing a model for fitting to data. Named
-Parameters can be held fixed or freely adjusted in the fit, or held between
-lower and upper bounds. In addition, parameters can be constrained as a simple
-mathematical expression of other Parameters.
-
-To do this, the programmer defines a Parameters object, an enhanced dictionary,
-containing named parameters::
-
-    fit_params = Parameters()
-    fit_params['amp'] = Parameter(value=1.2, min=0.1, max=1000)
-    fit_params['cen'] = Parameter(value=40.0, vary=False)
-    fit_params['wid'] = Parameter(value=4, min=0)
+    fit_params = lmfit.create_params(amp=1.2,
+                                     cen={'value':40, 'vary':False},
+                                     wid={'value': 4, 'min':0},
+                                     fwhm={'expr': 'wid*2.355'})
 
-or using the equivalent::
 
-    fit_params = Parameters()
-    fit_params.add('amp', value=1.2, min=0.1, max=1000)
-    fit_params.add('cen', value=40.0, vary=False)
-    fit_params.add('wid', value=4, min=0)
-
-The programmer will also write a function to be minimized (in the least-squares
-sense) with its first argument being this Parameters object, and additional
-positional and keyword arguments as desired::
+
+In the general minimization case (see below for Curve-fitting), the user will
+also write an objective function to be minimized (in the least-squares sense)
+with its first argument being this Parameters object, and additional positional
+and keyword arguments as desired::
 
     def myfunc(params, x, data, someflag=True):
         amp = params['amp'].value
         cen = params['cen'].value
         wid = params['wid'].value
         ...
         return residual_array
@@ -83,19 +100,44 @@
 actually varied in the fit. In addition, which parameters are adjusted and which
 are fixed happens at run-time, so that changing what is varied and what
 constraints are placed on the parameters can easily be modified by the user in
 real-time data analysis.
 
 To perform the fit, the user calls::
 
-    result = minimize(myfunc, fit_params, args=(x, data), kws={'someflag':True}, ....)
+    result = lmfit.minimize(myfunc, fit_params, args=(x, data), kws={'someflag':True}, ....)
 
 After the fit, a ``MinimizerResult`` class is returned that holds the results
 the fit (e.g., fitting statistics and optimized parameters). The dictionary
 ``result.params`` contains the best-fit values, estimated standard deviations,
 and correlations with other variables in the fit.
 
 By default, the underlying fit algorithm is the Levenberg-Marquardt algorithm
 with numerically-calculated derivatives from MINPACK's lmdif function, as used
 by ``scipy.optimize.leastsq``. Most other solvers that are present in ``scipy``
-(e.g., Nelder-Mead, differential_evolution, basinhopping, etctera) are also
+(e.g., Nelder-Mead, differential_evolution, basin-hopping, and more) are also
 supported.
+
+
+Curve-Fitting with lmfit.Model
+----------------------------------
+
+One of the most common use of least-squares minimization is for curve fitting,
+where minimization of ``data-model``, or ``(data-model)*weights``.  Using
+``lmfit.minimize`` as above, the objective function would take ``data`` and
+``weights`` and effectively calculated the model and then return the value of
+``(data-model)*weights``.
+
+To simplify this, and make curve-fitting more flexible, lmfit provides a Model
+class that wraps a *model function* that represents the model (without the data
+or weights).  Parameters are then automatically found from the named arguments
+of the model function.  In addition, simple model functions can be readily
+combined and reused, and several common model functions are included in lmfit.
+
+Exploration of Confidence Intervals
+-------------------------------------
+
+Lmfit tries to always estimate uncertainties in fitting parameters and
+correlations between them.  It does this even for those methods where the
+corresponding ``scipy.optimize`` routines do not estimate uncertainties.  Lmfit
+also provides methods to explicitly explore and evaluate the confidence
+intervals in fit results.
```

### Comparing `lmfit-1.2.0/asv_benchmarking/asv.conf.json` & `lmfit-1.2.1/asv_benchmarking/asv.conf.json`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/asv_benchmarking/benchmarks/benchmarks.py` & `lmfit-1.2.1/asv_benchmarking/benchmarks/benchmarks.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/azure-pipelines.yml` & `lmfit-1.2.1/azure-pipelines.yml`

 * *Files 0% similar despite different names*

```diff
@@ -257,27 +257,27 @@
             ##curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
             ##python3.12 get-pip.py --user
             python3.12 -m ensurepip --upgrade
             pip3.12 install -U build pip setuptools wheel pybind11 cython || echo -e "\043#vso[task.logissue type=warning;] Allowed failure for development version!!"
           displayName: 'Install build, pip, setuptools, wheel, pybind11, and cython'
         - script: |
             export PATH=/home/vsts/.local/bin:$PATH
-            export numpy_version=1.24.1
+            export numpy_version=1.24.3
             wget https://github.com/numpy/numpy/releases/download/v${numpy_version}/numpy-${numpy_version}.tar.gz
             tar xzvf numpy-${numpy_version}.tar.gz
             cd numpy-${numpy_version}
             python3.12 setup.py install --user || echo -e "\043#vso[task.logissue type=warning;] Allowed failure for development version!!"
           displayName: 'Install latest available version of NumPy'
         - script: |
             export PATH=/home/vsts/.local/bin:$PATH
             pip3.12 install -U pythran || echo -e "\043#vso[task.logissue type=warning;] Allowed failure for development version!!"
           displayName: 'Install pythran'
         - script: |
             export PATH=/home/vsts/.local/bin:$PATH
-            export scipy_version=1.10.0
+            export scipy_version=1.10.1
             wget https://github.com/scipy/scipy/releases/download/v${scipy_version}/scipy-${scipy_version}.tar.gz
             tar xzvf scipy-${scipy_version}.tar.gz
             cd scipy-${scipy_version}
             python3.12 setup.py install --user || echo -e "\043#vso[task.logissue type=warning;] Allowed failure for development version!!"
           displayName: 'Install latest available version of SciPy'
         - script: |
             export PATH=/home/vsts/.local/bin:$PATH
```

### Comparing `lmfit-1.2.0/doc/Makefile` & `lmfit-1.2.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/doc/_templates/indexsidebar.html` & `lmfit-1.2.1/doc/_templates/indexsidebar.html`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/doc/bounds.rst` & `lmfit-1.2.1/doc/bounds.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/doc/builtin_models.rst` & `lmfit-1.2.1/doc/builtin_models.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/doc/conf.py` & `lmfit-1.2.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/doc/confidence.rst` & `lmfit-1.2.1/doc/confidence.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/doc/constraints.rst` & `lmfit-1.2.1/doc/constraints.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/doc/doc_examples_to_gallery.py` & `lmfit-1.2.1/doc/doc_examples_to_gallery.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/doc/faq.rst` & `lmfit-1.2.1/doc/faq.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/doc/fitting.rst` & `lmfit-1.2.1/doc/fitting.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/doc/index.rst` & `lmfit-1.2.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/doc/installation.rst` & `lmfit-1.2.1/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/doc/intro.rst` & `lmfit-1.2.1/doc/intro.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/doc/make.bat` & `lmfit-1.2.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/doc/model.rst` & `lmfit-1.2.1/doc/model.rst`

 * *Files 1% similar despite different names*

```diff
@@ -912,14 +912,23 @@
 
    Boolean flag for whether to automatically scale covariance matrix.
 
 .. attribute:: success
 
    Boolean value of whether fit succeeded.
 
+.. attribute:: userargs
+
+   positional arguments passed to :meth:`Model.fit`, a tuple of (``y``, ``weights``)
+
+.. attribute:: userkws
+
+   keyword arguments passed to :meth:`Model.fit`, a dict, which will have independent data arrays such as ``x``.
+
+
 .. attribute:: weights
 
    numpy.ndarray (or ``None``) of weighting values to be used in fit. If not
    ``None``, it will be used as a multiplicative factor of the residual
    array, so that ``weights*(data - fit)`` is minimized in the
    least-squares sense.
```

### Comparing `lmfit-1.2.0/doc/parameters.rst` & `lmfit-1.2.1/doc/parameters.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/doc/sphinx/theme/sphinx13/basic_layout.html` & `lmfit-1.2.1/doc/sphinx/theme/sphinx13/basic_layout.html`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/doc/sphinx/theme/sphinx13/layout.html` & `lmfit-1.2.1/doc/sphinx/theme/sphinx13/layout.html`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/doc/sphinx/theme/sphinx13/static/lmfitheader.png` & `lmfit-1.2.1/doc/sphinx/theme/sphinx13/static/lmfitheader.png`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/doc/sphinx/theme/sphinx13/static/sphinx13.css` & `lmfit-1.2.1/doc/sphinx/theme/sphinx13/static/sphinx13.css`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/doc/support.rst` & `lmfit-1.2.1/doc/support.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/doc/whatsnew.rst` & `lmfit-1.2.1/doc/whatsnew.rst`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,27 @@
 .. _lmfit GitHub repository: https://github.com/lmfit/lmfit-py
 
 This section discusses changes between versions, especially changes
 significant to the use and behavior of the library. This is not meant
 to be a comprehensive list of changes. For such a complete record,
 consult the `lmfit GitHub repository`_.
 
+.. _whatsnew_121_label:
+
+Version 1.2.1 Release Notes (May 02, 2023)
+=================================================
+
+Bug fixes/enhancements:
+
+- fixed bug in ``Model.make_params()`` for initial parameter values that were
+  not recognized as floats such as ``np.Int64``.  (Issue #871; PR #872)
+
+- explicitly set ``maxfun`` for ``l-bfgs-b`` method when setting
+  ``maxiter``. (Issue #864; Discussion #865; PR #866)
+
 .. _whatsnew_120_label:
 
 Version 1.2.0 Release Notes (April 05, 2023)
 =================================================
 
 New features:
```

### Comparing `lmfit-1.2.0/examples/NIST_Gauss2.dat` & `lmfit-1.2.1/examples/NIST_Gauss2.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/doc_builtinmodels_nistgauss.py` & `lmfit-1.2.1/examples/doc_builtinmodels_nistgauss.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/doc_builtinmodels_nistgauss2.py` & `lmfit-1.2.1/examples/doc_builtinmodels_nistgauss2.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/doc_builtinmodels_peakmodels.py` & `lmfit-1.2.1/examples/doc_builtinmodels_peakmodels.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/doc_builtinmodels_splinemodel.py` & `lmfit-1.2.1/examples/doc_builtinmodels_splinemodel.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/doc_builtinmodels_stepmodel.py` & `lmfit-1.2.1/examples/doc_builtinmodels_stepmodel.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/doc_confidence_advanced.py` & `lmfit-1.2.1/examples/doc_confidence_advanced.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/doc_confidence_chi2_maps.py` & `lmfit-1.2.1/examples/doc_confidence_chi2_maps.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/doc_fitting_emcee.py` & `lmfit-1.2.1/examples/doc_fitting_emcee.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/doc_fitting_withreport.py` & `lmfit-1.2.1/examples/doc_fitting_withreport.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/doc_model_composite.py` & `lmfit-1.2.1/examples/doc_model_composite.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/doc_model_gaussian.py` & `lmfit-1.2.1/examples/doc_model_gaussian.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/doc_model_loadmodel.py` & `lmfit-1.2.1/examples/doc_model_loadmodel.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/doc_model_loadmodelresult.py` & `lmfit-1.2.1/examples/doc_model_loadmodelresult.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/doc_model_loadmodelresult2.py` & `lmfit-1.2.1/examples/doc_model_loadmodelresult2.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/doc_model_savemodelresult2.py` & `lmfit-1.2.1/examples/doc_model_savemodelresult2.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/doc_model_two_components.py` & `lmfit-1.2.1/examples/doc_model_two_components.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/doc_model_uncertainty.py` & `lmfit-1.2.1/examples/doc_model_uncertainty.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/doc_model_uncertainty2.py` & `lmfit-1.2.1/examples/doc_model_uncertainty2.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/doc_model_with_iter_callback.py` & `lmfit-1.2.1/examples/doc_model_with_iter_callback.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/doc_model_with_nan_policy.py` & `lmfit-1.2.1/examples/doc_model_with_nan_policy.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/doc_parameters_basic.py` & `lmfit-1.2.1/examples/doc_parameters_basic.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/doc_parameters_valuesdict.py` & `lmfit-1.2.1/examples/doc_parameters_valuesdict.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/example_Model_interface.py` & `lmfit-1.2.1/examples/example_Model_interface.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/example_brute.py` & `lmfit-1.2.1/examples/example_brute.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/example_complex_resonator_model.py` & `lmfit-1.2.1/examples/example_complex_resonator_model.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/example_confidence_interval.py` & `lmfit-1.2.1/examples/example_confidence_interval.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/example_detect_outliers.py` & `lmfit-1.2.1/examples/example_detect_outliers.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/example_diffev.py` & `lmfit-1.2.1/examples/example_diffev.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/example_emcee_Model_interface.py` & `lmfit-1.2.1/examples/example_emcee_Model_interface.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/example_expression_model.py` & `lmfit-1.2.1/examples/example_expression_model.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/example_fit_multi_datasets.py` & `lmfit-1.2.1/examples/example_fit_multi_datasets.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/example_fit_with_algebraic_constraint.py` & `lmfit-1.2.1/examples/example_fit_with_algebraic_constraint.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/example_fit_with_bounds.py` & `lmfit-1.2.1/examples/example_fit_with_bounds.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/example_fit_with_derivfunc.py` & `lmfit-1.2.1/examples/example_fit_with_derivfunc.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/example_fit_with_inequality.py` & `lmfit-1.2.1/examples/example_fit_with_inequality.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/example_reduce_fcn.py` & `lmfit-1.2.1/examples/example_reduce_fcn.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/example_sympy.py` & `lmfit-1.2.1/examples/example_sympy.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/example_two_dimensional_peak.py` & `lmfit-1.2.1/examples/example_two_dimensional_peak.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/example_use_pandas.py` & `lmfit-1.2.1/examples/example_use_pandas.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/lmfit_emcee_model_selection.py` & `lmfit-1.2.1/examples/lmfit_emcee_model_selection.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/model1d_gauss.dat` & `lmfit-1.2.1/examples/model1d_gauss.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/peak.csv` & `lmfit-1.2.1/examples/peak.csv`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/sinedata.dat` & `lmfit-1.2.1/examples/sinedata.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/test_peak.dat` & `lmfit-1.2.1/examples/test_peak.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/examples/test_splinepeak.dat` & `lmfit-1.2.1/examples/test_splinepeak.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/lmfit/__init__.py` & `lmfit-1.2.1/lmfit/__init__.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/lmfit/_ampgo.py` & `lmfit-1.2.1/lmfit/_ampgo.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/lmfit/confidence.py` & `lmfit-1.2.1/lmfit/confidence.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/lmfit/jsonutils.py` & `lmfit-1.2.1/lmfit/jsonutils.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/lmfit/lineshapes.py` & `lmfit-1.2.1/lmfit/lineshapes.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/lmfit/minimizer.py` & `lmfit-1.2.1/lmfit/minimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -961,14 +961,17 @@
         result = self.prepare_fit(params=params)
         result.method = method
         variables = result._init_vals_internal
         params = result.params
 
         self.set_max_nfev(max_nfev, 2000*(result.nvarys+1))
         fmin_kws = dict(method=method, options={'maxiter': 2*self.max_nfev})
+        if method == 'L-BFGS-B':
+            fmin_kws['options']['maxfun'] = 2*self.max_nfev
+
         # fmin_kws = dict(method=method, options={'maxfun': 2*self.max_nfev})
         fmin_kws.update(self.kws)
 
         if 'maxiter' in kws:
             warnings.warn(maxeval_warning.format('maxiter', thisfuncname()),
                           RuntimeWarning)
             kws.pop('maxiter')
```

### Comparing `lmfit-1.2.0/lmfit/model.py` & `lmfit-1.2.1/lmfit/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -661,17 +661,23 @@
         ...                    peak_amplitdue=dict(value=100, min=2),
         ...                    peak_sigma=dict(value=25, min=0, max=1000))
 
         """
         params = Parameters()
 
         def setpar(par, val):
-            if isinstance(val, (float, int)):
-                val = {'value': val}
-            par.set(**val)
+            # val is expected to be float-like or a dict: must have 'value' or 'expr' key
+            if isinstance(val, dict):
+                dval = val
+            else:
+                dval = {'value': float(val)}
+            if len(dval) < 1 or not ('value' in dval or 'expr' in dval):
+                raise TypeError(f'Invalid parameter value for {par}: {val}')
+
+            par.set(**dval)
 
         # make sure that all named parameters are in params
         for name in self.param_names:
             if name in params:
                 par = params[name]
             else:
                 par = Parameter(name=name)
```

### Comparing `lmfit-1.2.0/lmfit/models.py` & `lmfit-1.2.1/lmfit/models.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/lmfit/parameter.py` & `lmfit-1.2.1/lmfit/parameter.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/lmfit/printfuncs.py` & `lmfit-1.2.1/lmfit/printfuncs.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/lmfit.egg-info/SOURCES.txt` & `lmfit-1.2.1/lmfit.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 doc/builtin_models.rst
 doc/conf.py
 doc/confidence.rst
 doc/constraints.rst
 doc/contents.rst
 doc/doc_examples_to_gallery.py
 doc/faq.rst
-doc/filter_spurious_link_from_html.py
 doc/fitting.rst
 doc/index.rst
 doc/installation.rst
 doc/intro.rst
 doc/make.bat
 doc/model.rst
 doc/parameters.rst
@@ -128,14 +127,15 @@
 examples/model1d_gauss.dat
 examples/peak.csv
 examples/sinedata.dat
 examples/test_peak.dat
 examples/test_splinepeak.dat
 lmfit/__init__.py
 lmfit/_ampgo.py
+lmfit/conf_emcee.py
 lmfit/confidence.py
 lmfit/jsonutils.py
 lmfit/lineshapes.py
 lmfit/minimizer.py
 lmfit/model.py
 lmfit/models.py
 lmfit/parameter.py
```

### Comparing `lmfit-1.2.0/lmfit.egg-info/requires.txt` & `lmfit-1.2.1/lmfit.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 uncertainties>=3.1.4
 
 [all]
 build
 check-wheel-contents
 pre-commit
 twine
-codecov
 coverage
 flaky
 pytest
 pytest-cov
 cairosvg
 corner
 dill
@@ -53,12 +52,11 @@
 sphinxcontrib-svg2pdfconverter
 sympy
 
 [doc:platform_system == "Windows"]
 pycairo
 
 [test]
-codecov
 coverage
 flaky
 pytest
 pytest-cov
```

### Comparing `lmfit-1.2.0/publish_docs.sh` & `lmfit-1.2.1/publish_docs.sh`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/setup.cfg` & `lmfit-1.2.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,14 @@
 	Pillow
 	pycairo;platform_system=="Windows"
 	Sphinx
 	sphinx-gallery>=0.10
 	sphinxcontrib-svg2pdfconverter
 	sympy
 test = 
-	codecov
 	coverage
 	flaky
 	pytest
 	pytest-cov
 all = 
 	%(dev)s
 	%(test)s
```

### Comparing `lmfit-1.2.0/tests/NISTModels.py` & `lmfit-1.2.1/tests/NISTModels.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/tests/conftest.py` & `lmfit-1.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/tests/gauss_modelresult_lmfit100.sav` & `lmfit-1.2.1/tests/gauss_modelresult_lmfit100.sav`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/tests/test_1variable.py` & `lmfit-1.2.1/tests/test_1variable.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/tests/test_NIST_Strd.py` & `lmfit-1.2.1/tests/test_NIST_Strd.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/tests/test_algebraic_constraint.py` & `lmfit-1.2.1/tests/test_algebraic_constraint.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/tests/test_ampgo.py` & `lmfit-1.2.1/tests/test_ampgo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Tests for the AMPGO global minimization algorithm."""
-import sys
 
 import numpy as np
 from numpy.testing import assert_allclose
 import pytest
 from scipy import __version__ as scipy_version
 
 import lmfit
@@ -96,16 +95,14 @@
 def test_ampgo_invalid_tabustrategy(minimizer_Alpine02):
     """Test AMPGO algorithm with invalid tabustrategy."""
     kws = {'tabustrategy': 'unknown'}
     with pytest.raises(Exception, match=r'Invalid tabustrategy specified'):
         minimizer_Alpine02.minimize(method='ampgo', **kws)
 
 
-@pytest.mark.skipif(sys.version_info.major == 2,
-                    reason="does not throw an exception in Python 2")
 def test_ampgo_local_opts(minimizer_Alpine02):
     """Test AMPGO algorithm, pass local_opts to solver."""
     # use local_opts to pass maxfun to the local optimizer: providing a string
     # whereas an integer is required, this should throw an error.
     kws = {'local_opts': {'maxfun': 'string'}}
     with pytest.raises(TypeError):
         minimizer_Alpine02.minimize(method='ampgo', **kws)
```

### Comparing `lmfit-1.2.0/tests/test_basicfit.py` & `lmfit-1.2.1/tests/test_basicfit.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/tests/test_basinhopping.py` & `lmfit-1.2.1/tests/test_basinhopping.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/tests/test_bounded_jacobian.py` & `lmfit-1.2.1/tests/test_bounded_jacobian.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/tests/test_bounds.py` & `lmfit-1.2.1/tests/test_bounds.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/tests/test_brute.py` & `lmfit-1.2.1/tests/test_brute.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/tests/test_builtin_models.py` & `lmfit-1.2.1/tests/test_builtin_models.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/tests/test_confidence.py` & `lmfit-1.2.1/tests/test_confidence.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/tests/test_covariance_matrix.py` & `lmfit-1.2.1/tests/test_covariance_matrix.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/tests/test_custom_independentvar.py` & `lmfit-1.2.1/tests/test_custom_independentvar.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/tests/test_default_kws.py` & `lmfit-1.2.1/tests/test_default_kws.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/tests/test_dual_annealing.py` & `lmfit-1.2.1/tests/test_dual_annealing.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/tests/test_itercb.py` & `lmfit-1.2.1/tests/test_itercb.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/tests/test_jsonutils.py` & `lmfit-1.2.1/tests/test_jsonutils.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/tests/test_least_squares.py` & `lmfit-1.2.1/tests/test_least_squares.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/tests/test_lineshapes.py` & `lmfit-1.2.1/tests/test_lineshapes.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/tests/test_manypeaks_speed.py` & `lmfit-1.2.1/tests/test_manypeaks_speed.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/tests/test_max_nfev.py` & `lmfit-1.2.1/tests/test_max_nfev.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/tests/test_minimizer.py` & `lmfit-1.2.1/tests/test_minimizer.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/tests/test_model.py` & `lmfit-1.2.1/tests/test_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Tests for the Model, CompositeModel, and ModelResult classes."""
 
 import functools
-import sys
 import unittest
 import warnings
 
 import numpy as np
 from numpy.testing import assert_allclose
 import pytest
 from scipy import __version__ as scipy_version
@@ -1259,16 +1258,14 @@
         p = model.make_params(a1=4, t1=3, a2=4, t2=3)
         result = lambda: model.fit(data=y, params=p, x=x, method='Nelder',
                                    nan_policy='raise')
 
         msg = 'The model function generated NaN values and the fit aborted!'
         self.assertRaisesRegex(ValueError, msg, result)
 
-    @pytest.mark.skipif(sys.version_info.major == 2,
-                        reason="cannot use wrapped functions with Python 2")
     def test_wrapped_model_func(self):
         x = np.linspace(-1, 1, 51)
         y = 2.0*x + 3 + 0.0003 * x*x
         y += np.random.normal(size=len(x), scale=0.025)
         mod = Model(linear_func)
         pars = mod.make_params(a=1.5, b=2.5)
 
@@ -1398,7 +1395,41 @@
         params = comp_model.make_params(**self.guess())
 
         result = comp_model.fit(data, x=x, params=params)
         assert_results_close(result.values, true_values, rtol=0.01, atol=0.01)
 
         data_components = comp_model.eval_components(x=x)
         self.assertIn('exp', data_components)
+
+
+def test_make_params_valuetypes():
+    mod = lmfit.models.SineModel()
+
+    pars = mod.make_params(amplitude=1, frequency=1, shift=-0.2)
+
+    pars = mod.make_params(amplitude={'value': 0.9, 'min': 0},
+                           frequency=1.03,
+                           shift={'value': -0.2, 'vary': False})
+
+    val_i32 = np.arange(10, dtype=np.int32)
+    val_i64 = np.arange(10, dtype=np.int64)
+    # np.longdouble equals to np.float128 on Linux and macOS, np.float64 on Windows
+    val_ld = np.arange(10, dtype=np.longdouble)/3.0
+    val_c128 = np.arange(10, dtype=np.complex128)/3.0
+
+    pars = mod.make_params(amplitude=val_i64[2],
+                           frequency=val_i32[3],
+                           shift=-val_ld[4])
+
+    pars = mod.make_params(amplitude=val_c128[2],
+                           frequency=val_i32[3],
+                           shift=-val_ld[4])
+
+    assert pars is not None
+    with pytest.raises(ValueError):
+        pars = mod.make_params(amplitude='a string', frequency=2, shift=7)
+
+    with pytest.raises(TypeError):
+        pars = mod.make_params(amplitude={'v': 3}, frequency=2, shift=7)
+
+    with pytest.raises(TypeError):
+        pars = mod.make_params(amplitude={}, frequency=2, shift=7)
```

### Comparing `lmfit-1.2.0/tests/test_model_saveload.py` & `lmfit-1.2.1/tests/test_model_saveload.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/tests/test_model_uncertainties.py` & `lmfit-1.2.1/tests/test_model_uncertainties.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/tests/test_models.py` & `lmfit-1.2.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/tests/test_multidatasets.py` & `lmfit-1.2.1/tests/test_multidatasets.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/tests/test_nose.py` & `lmfit-1.2.1/tests/test_nose.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/tests/test_pandas.py` & `lmfit-1.2.1/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/tests/test_parameter.py` & `lmfit-1.2.1/tests/test_parameter.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/tests/test_parameters.py` & `lmfit-1.2.1/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/tests/test_printfuncs.py` & `lmfit-1.2.1/tests/test_printfuncs.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/tests/test_shgo.py` & `lmfit-1.2.1/tests/test_shgo.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.2.0/tests/test_stepmodel.py` & `lmfit-1.2.1/tests/test_stepmodel.py`

 * *Files identical despite different names*

