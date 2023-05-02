# Comparing `tmp/clophfit-0.4.7.tar.gz` & `tmp/clophfit-0.4.8.tar.gz`

## Comparing `clophfit-0.4.7.tar` & `clophfit-0.4.8.tar`

### file list

```diff
@@ -1,200 +1,200 @@
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 clophfit-0.4.7/.codespellrc
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 clophfit-0.4.7/.darglint
--rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 clophfit-0.4.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 clophfit-0.4.7/.python-version
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 clophfit-0.4.7/.readthedocs.yml
--rw-r--r--   0        0        0    11049 2020-02-02 00:00:00.000000 clophfit-0.4.7/CHANGELOG.md
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 clophfit-0.4.7/CONTRIBUTING.md
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 clophfit-0.4.7/bandit.yml
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 clophfit-0.4.7/cz_customize_info.txt
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 clophfit-0.4.7/.github/dependabot.yml
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 clophfit-0.4.7/.github/workflows/cd.yml
--rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 clophfit-0.4.7/.github/workflows/ci.yml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 clophfit-0.4.7/.github/workflows/constraints.txt
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 clophfit-0.4.7/.github/workflows/docs.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/Makefile
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/conf.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/make.bat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/.gitkeep
--rw-r--r--   0        0        0    49846 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/bs_pd_f1.png
--rw-r--r--   0        0        0    55458 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/bs_pd_f2.png
--rw-r--r--   0        0        0    16105 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/bs_pd_f3.png
--rw-r--r--   0        0        0    36779 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/bs_pd_f4.png
--rw-r--r--   0        0        0    16293 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/bs_pd_f5.png
--rw-r--r--   0        0        0    23529 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/bs_pd_f6.png
--rw-r--r--   0        0        0    41234 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/bs_pd_f7.png
--rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/csvtable.png
--rw-r--r--   0        0        0    20158 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/emcee-01.png
--rw-r--r--   0        0        0   109446 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/emcee-02.png
--rw-r--r--   0        0        0    18582 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/emcee-11.png
--rw-r--r--   0        0        0   420822 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/emcee-12.png
--rw-r--r--   0        0        0    14293 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/f01.png
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/file.png
--rw-r--r--   0        0        0     7787 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/gR_fit1.png
--rw-r--r--   0        0        0    32629 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/gR_fit2.png
--rw-r--r--   0        0        0   117478 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/gR_fit3.png
--rw-r--r--   0        0        0    42999 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/gR_fit4.png
--rw-r--r--   0        0        0    83505 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/gR_fit5.png
--rw-r--r--   0        0        0    12423 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/gR_fit6.png
--rw-r--r--   0        0        0    14823 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/gR_fit7.png
--rw-r--r--   0        0        0    18894 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/glmfit0.png
--rw-r--r--   0        0        0    21702 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/glmfit1.png
--rw-r--r--   0        0        0    33541 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/glmfit2.png
--rw-r--r--   0        0        0    10655 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/glmfit3.png
--rw-r--r--   0        0        0    34747 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/glmfit_np.r_.png
--rw-r--r--   0        0        0    16358 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/lmfit1.png
--rw-r--r--   0        0        0    29012 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/lmfit2.png
--rw-r--r--   0        0        0    45332 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/lmfit3.png
--rw-r--r--   0        0        0    48655 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/lmfit4.png
--rw-r--r--   0        0        0    16400 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/lmfit5.png
--rw-r--r--   0        0        0    21693 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/lmodel1.png
--rw-r--r--   0        0        0    28428 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/lmodel2.png
--rw-r--r--   0        0        0    11916 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/lmodel3.png
--rw-r--r--   0        0        0    29389 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/lmodel4.png
--rw-r--r--   0        0        0    23708 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/lmodel5.png
--rw-r--r--   0        0        0   187683 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/lmodel6.png
--rw-r--r--   0        0        0    24709 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/lmodel_H04.png
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/note_file.png
--rw-r--r--   0        0        0   101706 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/r_bs.png
--rw-r--r--   0        0        0    24754 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/ratio2P-lmodel1.png
--rw-r--r--   0        0        0    63411 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/ratio2P-lmodel2.png
--rw-r--r--   0        0        0    31838 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/ratio2P_R1.png
--rw-r--r--   0        0        0   114443 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/ratio2P_R2.png
--rw-r--r--   0        0        0    43555 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/ratio2P_R3.png
--rw-r--r--   0        0        0    94094 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/ratio2P_R4.png
--rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/ratio2P_R5.png
--rw-r--r--   0        0        0    14971 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/ratio2P_R6.png
--rw-r--r--   0        0        0   101706 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/_static/rpy_bs.png
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/api/api.rst
--rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/api/prtecan.uml.rst
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/misc/CHANGELOG.md -> ../../CHANGELOG.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/misc/CONTRIBUTING.md -> ../../CONTRIBUTING.md
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/misc/license.rst
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/misc/misc.rst
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/references/description.rst
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/references/references.rst
--rw-r--r--   0        0        0  1966192 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/tutorials/prtecan.ipynb
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/tutorials/tutorials.rst
--rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/tutorials/usage.org
--rw-r--r--   0        0        0    14299 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/tutorials/usage.rst
--rw-r--r--   0        0        0    30911 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/tutorials/usage2.org
--rw-r--r--   0        0        0    58554 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/tutorials/usage2.rst
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 clophfit-0.4.7/src/clophfit/__init__.py
--rw-r--r--   0        0        0     7325 2020-02-02 00:00:00.000000 clophfit-0.4.7/src/clophfit/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.4.7/src/clophfit/py.typed
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 clophfit-0.4.7/src/clophfit/binding/__init__.py
--rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 clophfit-0.4.7/src/clophfit/binding/fitting.py
--rwxr-xr-x   0        0        0     1386 2020-02-02 00:00:00.000000 clophfit-0.4.7/src/clophfit/old/dil_buffer.py
--rwxr-xr-x   0        0        0     1320 2020-02-02 00:00:00.000000 clophfit-0.4.7/src/clophfit/old/dil_correction.py
--rwxr-xr-x   0        0        0     5639 2020-02-02 00:00:00.000000 clophfit-0.4.7/src/clophfit/old/fit_rpy.py
--rwxr-xr-x   0        0        0     7936 2020-02-02 00:00:00.000000 clophfit-0.4.7/src/clophfit/old/fit_titration.py
--rwxr-xr-x   0        0        0     6060 2020-02-02 00:00:00.000000 clophfit-0.4.7/src/clophfit/old/fit_titration_global.py
--rwxr-xr-x   0        0        0      634 2020-02-02 00:00:00.000000 clophfit-0.4.7/src/clophfit/old/merge.py
--rwxr-xr-x   0        0        0      891 2020-02-02 00:00:00.000000 clophfit-0.4.7/src/clophfit/old/plot_tecan.py
--rwxr-xr-x   0        0        0      119 2020-02-02 00:00:00.000000 clophfit-0.4.7/src/clophfit/old/bash/fit.tecan
--rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 clophfit-0.4.7/src/clophfit/old/bash/fit.tecan.cl
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 clophfit-0.4.7/src/clophfit/old/bash/new_sort_K.sh
--rwxr-xr-x   0        0        0      222 2020-02-02 00:00:00.000000 clophfit-0.4.7/src/clophfit/old/bash/sum_all
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.4.7/src/clophfit/old/bash/sum_e2
--rwxr-xr-x   0        0        0      352 2020-02-02 00:00:00.000000 clophfit-0.4.7/src/clophfit/old/bash/sum_lib
--rwxr-xr-x   0        0        0      427 2020-02-02 00:00:00.000000 clophfit-0.4.7/src/clophfit/old/bash/sum_lib2
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.4.7/src/clophfit/old/bash/sum_s202n
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.4.7/src/clophfit/old/bash/sum_v224q
--rwxr-xr-x   0        0        0      572 2020-02-02 00:00:00.000000 clophfit-0.4.7/src/clophfit/old/bash/w_ave.sh
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 clophfit-0.4.7/src/clophfit/prtecan/__init__.py
--rw-r--r--   0        0        0    51759 2020-02-02 00:00:00.000000 clophfit-0.4.7/src/clophfit/prtecan/prtecan.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/conftest.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/test_binding.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/test_cli.py
--rw-r--r--   0        0        0     5895 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/test_oldscripts.py
--rw-r--r--   0        0        0    26316 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/test_prtecan.py
--rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/290212_100.xls
--rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/290212_150.xls
--rw-r--r--   0        0        0    12069 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/290212_20.xls
--rw-r--r--   0        0        0    13122 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/290212_5.78.xls
--rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/290212_50.xls
--rw-r--r--   0        0        0    13140 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/290212_6.38.xls
--rw-r--r--   0        0        0    13137 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/290212_6.83.xls
--rw-r--r--   0        0        0    13146 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/290212_7.24.xls
--rw-r--r--   0        0        0    13141 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/290212_7.67.xls
--rw-r--r--   0        0        0    13173 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/290212_8.23.xls
--rw-r--r--   0        0        0    13171 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/290212_8.82.xls
--rw-r--r--   0        0        0    13152 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/290212_9.31.xls
--rw-r--r--   0        0        0    12930 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/290513_5.5.xls
--rw-r--r--   0        0        0    11262 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/290513_5.5_bad.xls
--rw-r--r--   0        0        0    12946 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/290513_7.2.xls
--rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/290513_8.8.xls
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/list.cl
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/list.cl20
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/list.pH
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/list.pH2
--rw-r--r--   0        0        0    14438 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/140220/200214 pH data.ods
--rw-r--r--   0        0        0    12835 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/140220/NaCl1_200214.xls
--rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/140220/NaCl2_200214.xls
--rw-r--r--   0        0        0    12802 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/140220/NaCl3_200214.xls
--rw-r--r--   0        0        0    12799 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/140220/NaCl4_200214.xls
--rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/140220/NaCl5_200214.xls
--rw-r--r--   0        0        0    12773 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/140220/NaCl6_200214.xls
--rw-r--r--   0        0        0    12783 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/140220/NaCl7_200214.xls
--rw-r--r--   0        0        0    12790 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/140220/NaCl8_200214.xls
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/140220/additions.cl
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/140220/additions.pH
--rw-r--r--   0        0        0    21877 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/140220/fit0-1.csv
--rw-r--r--   0        0        0    21592 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/140220/fit0.csv
--rw-r--r--   0        0        0    23056 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/140220/fit1-1.csv
--rw-r--r--   0        0        0    23182 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/140220/fit1.csv
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/140220/list.cl
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/140220/list.pH
--rw-r--r--   0        0        0    12865 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/140220/pH5.0_200214.xls
--rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/140220/pH5.8_200214.xls
--rw-r--r--   0        0        0    12889 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/140220/pH6.5_200214.xls
--rw-r--r--   0        0        0    12914 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/140220/pH7.1_200214.xls
--rw-r--r--   0        0        0    12934 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/140220/pH7.6_200214.xls
--rw-r--r--   0        0        0    12939 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/140220/pH8.3_200214.xls
--rw-r--r--   0        0        0    12937 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/140220/pH9.1_200214.xls
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/140220/scheme.txt
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/140220/scheme0.txt
--rw-r--r--   0        0        0     9176 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/exceptions/0_Labelblocks_290513_5.5.xlsx
--rw-r--r--   0        0        0    12275 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/exceptions/290212_7.67_repeated_lb.xls
--rw-r--r--   0        0        0    10209 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/exceptions/84wells_290212_20.xlsx
--rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/Tecan/exceptions/88wells_290212_20.xlsx
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/data/A01-20140311a.dat
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/data/A01.dat
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/data/A11.dat
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/data/B01.dat
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/data/H04.dat
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/data/NTT-A04-Cl_note
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/data/copyIP.txt
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/data/ratio2P.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/data/w.txt
--rw-r--r--   0        0        0    43486 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/data/Meas/A04 Cl_A.csv
--rw-r--r--   0        0        0   138192 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/data/Meas/A04 Cl_A.png
--rw-r--r--   0        0        0    29087 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/data/Meas/A04 Cl_B.csv
--rw-r--r--   0        0        0    97762 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/data/Meas/A04 Cl_B.png
--rw-r--r--   0        0        0    35910 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/data/Meas/A04 Cl_C.csv
--rw-r--r--   0        0        0   138239 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/data/Meas/A04 Cl_C.png
--rw-r--r--   0        0        0    29248 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/data/Meas/A04 Cl_D.csv
--rw-r--r--   0        0        0    84749 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/data/Meas/A04 Cl_D.png
--rw-r--r--   0        0        0    35312 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/data/Meas/A04 Cl_E.csv
--rw-r--r--   0        0        0   145114 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/data/Meas/A04 Cl_E.png
--rw-r--r--   0        0        0    43756 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/data/Meas/A04 Cl_F.csv
--rw-r--r--   0        0        0   126442 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/data/Meas/A04 Cl_F.png
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/data/global/Cl/A11-failed.dat
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/data/global/Cl/B05-20130628-cor.dat
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/data/global/pH/B01-failed.dat
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/data/global/pH/D05.dat
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/data/global/pH/H04-with_nan.dat
--rw-r--r--   0        0        0   235947 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/data/k/D05.dat-bs.png
--rw-r--r--   0        0        0    28093 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/data/k/D05.dat.png
--rw-r--r--   0        0        0    12506 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/data/output/band_A04 Cl_A_NTT-A04-Cl_note.pdf
--rw-r--r--   0        0        0    12433 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/data/output/band_A04 Cl_B_NTT-A04-Cl_note.pdf
--rw-r--r--   0        0        0    66713 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/data/output/svd_A04 Cl_A_NTT-A04-Cl_note.pdf
--rw-r--r--   0        0        0    39832 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/data/output/svd_A04 Cl_B_NTT-A04-Cl_note.pdf
--rw-r--r--   0        0        0    32564 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/data/output/global/Cl/B05-20130628-cor.dat.png
--rw-r--r--   0        0        0    36956 2020-02-02 00:00:00.000000 clophfit-0.4.7/tests/data/output/global/pH/D05.dat.png
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 clophfit-0.4.7/.gitignore
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 clophfit-0.4.7/LICENSE.txt
--rw-r--r--   0        0        0    11373 2020-02-02 00:00:00.000000 clophfit-0.4.7/pyproject.toml
--rw-r--r--   0        0        0     5590 2020-02-02 00:00:00.000000 clophfit-0.4.7/docs/README.md
--rw-r--r--   0        0        0     8431 2020-02-02 00:00:00.000000 clophfit-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 clophfit-0.4.8/.codespellrc
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 clophfit-0.4.8/.darglint
+-rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 clophfit-0.4.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 clophfit-0.4.8/.python-version
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 clophfit-0.4.8/.readthedocs.yml
+-rw-r--r--   0        0        0    13095 2020-02-02 00:00:00.000000 clophfit-0.4.8/CHANGELOG.md
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 clophfit-0.4.8/CONTRIBUTING.md
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 clophfit-0.4.8/bandit.yml
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 clophfit-0.4.8/cz_customize_info.txt
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 clophfit-0.4.8/.github/dependabot.yml
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 clophfit-0.4.8/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 clophfit-0.4.8/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 clophfit-0.4.8/.github/workflows/constraints.txt
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 clophfit-0.4.8/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/Makefile
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/conf.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/make.bat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/.gitkeep
+-rw-r--r--   0        0        0    49846 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/bs_pd_f1.png
+-rw-r--r--   0        0        0    55458 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/bs_pd_f2.png
+-rw-r--r--   0        0        0    16105 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/bs_pd_f3.png
+-rw-r--r--   0        0        0    36779 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/bs_pd_f4.png
+-rw-r--r--   0        0        0    16293 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/bs_pd_f5.png
+-rw-r--r--   0        0        0    23529 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/bs_pd_f6.png
+-rw-r--r--   0        0        0    41234 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/bs_pd_f7.png
+-rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/csvtable.png
+-rw-r--r--   0        0        0    20158 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/emcee-01.png
+-rw-r--r--   0        0        0   109446 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/emcee-02.png
+-rw-r--r--   0        0        0    18582 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/emcee-11.png
+-rw-r--r--   0        0        0   420822 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/emcee-12.png
+-rw-r--r--   0        0        0    14293 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/f01.png
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/file.png
+-rw-r--r--   0        0        0     7787 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/gR_fit1.png
+-rw-r--r--   0        0        0    32629 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/gR_fit2.png
+-rw-r--r--   0        0        0   117478 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/gR_fit3.png
+-rw-r--r--   0        0        0    42999 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/gR_fit4.png
+-rw-r--r--   0        0        0    83505 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/gR_fit5.png
+-rw-r--r--   0        0        0    12423 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/gR_fit6.png
+-rw-r--r--   0        0        0    14823 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/gR_fit7.png
+-rw-r--r--   0        0        0    18894 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/glmfit0.png
+-rw-r--r--   0        0        0    21702 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/glmfit1.png
+-rw-r--r--   0        0        0    33541 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/glmfit2.png
+-rw-r--r--   0        0        0    10655 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/glmfit3.png
+-rw-r--r--   0        0        0    34747 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/glmfit_np.r_.png
+-rw-r--r--   0        0        0    16358 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/lmfit1.png
+-rw-r--r--   0        0        0    29012 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/lmfit2.png
+-rw-r--r--   0        0        0    45332 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/lmfit3.png
+-rw-r--r--   0        0        0    48655 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/lmfit4.png
+-rw-r--r--   0        0        0    16400 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/lmfit5.png
+-rw-r--r--   0        0        0    21693 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/lmodel1.png
+-rw-r--r--   0        0        0    28428 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/lmodel2.png
+-rw-r--r--   0        0        0    11916 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/lmodel3.png
+-rw-r--r--   0        0        0    29389 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/lmodel4.png
+-rw-r--r--   0        0        0    23708 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/lmodel5.png
+-rw-r--r--   0        0        0   187683 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/lmodel6.png
+-rw-r--r--   0        0        0    24709 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/lmodel_H04.png
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/note_file.png
+-rw-r--r--   0        0        0   101706 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/r_bs.png
+-rw-r--r--   0        0        0    24754 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/ratio2P-lmodel1.png
+-rw-r--r--   0        0        0    63411 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/ratio2P-lmodel2.png
+-rw-r--r--   0        0        0    31838 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/ratio2P_R1.png
+-rw-r--r--   0        0        0   114443 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/ratio2P_R2.png
+-rw-r--r--   0        0        0    43555 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/ratio2P_R3.png
+-rw-r--r--   0        0        0    94094 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/ratio2P_R4.png
+-rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/ratio2P_R5.png
+-rw-r--r--   0        0        0    14971 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/ratio2P_R6.png
+-rw-r--r--   0        0        0   101706 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/_static/rpy_bs.png
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/api/api.rst
+-rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/api/prtecan.uml.rst
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/misc/CHANGELOG.md -> ../../CHANGELOG.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/misc/CONTRIBUTING.md -> ../../CONTRIBUTING.md
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/misc/license.rst
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/misc/misc.rst
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/references/description.rst
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/references/references.rst
+-rw-r--r--   0        0        0  1966192 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/tutorials/prtecan.ipynb
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/tutorials/tutorials.rst
+-rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/tutorials/usage.org
+-rw-r--r--   0        0        0    14299 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/tutorials/usage.rst
+-rw-r--r--   0        0        0    30911 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/tutorials/usage2.org
+-rw-r--r--   0        0        0    58554 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/tutorials/usage2.rst
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/__init__.py
+-rw-r--r--   0        0        0     7325 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/py.typed
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/binding/__init__.py
+-rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/binding/fitting.py
+-rwxr-xr-x   0        0        0     1386 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/old/dil_buffer.py
+-rwxr-xr-x   0        0        0     1320 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/old/dil_correction.py
+-rwxr-xr-x   0        0        0     5639 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/old/fit_rpy.py
+-rwxr-xr-x   0        0        0     7936 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/old/fit_titration.py
+-rwxr-xr-x   0        0        0     6060 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/old/fit_titration_global.py
+-rwxr-xr-x   0        0        0      634 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/old/merge.py
+-rwxr-xr-x   0        0        0      891 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/old/plot_tecan.py
+-rwxr-xr-x   0        0        0      119 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/old/bash/fit.tecan
+-rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/old/bash/fit.tecan.cl
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/old/bash/new_sort_K.sh
+-rwxr-xr-x   0        0        0      222 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/old/bash/sum_all
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/old/bash/sum_e2
+-rwxr-xr-x   0        0        0      352 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/old/bash/sum_lib
+-rwxr-xr-x   0        0        0      427 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/old/bash/sum_lib2
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/old/bash/sum_s202n
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/old/bash/sum_v224q
+-rwxr-xr-x   0        0        0      572 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/old/bash/w_ave.sh
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/prtecan/__init__.py
+-rw-r--r--   0        0        0    51805 2020-02-02 00:00:00.000000 clophfit-0.4.8/src/clophfit/prtecan/prtecan.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/conftest.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/test_binding.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/test_cli.py
+-rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/test_oldscripts.py
+-rw-r--r--   0        0        0    26316 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/test_prtecan.py
+-rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/290212_100.xls
+-rw-r--r--   0        0        0    12073 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/290212_150.xls
+-rw-r--r--   0        0        0    12069 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/290212_20.xls
+-rw-r--r--   0        0        0    13122 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/290212_5.78.xls
+-rw-r--r--   0        0        0    12062 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/290212_50.xls
+-rw-r--r--   0        0        0    13140 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/290212_6.38.xls
+-rw-r--r--   0        0        0    13137 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/290212_6.83.xls
+-rw-r--r--   0        0        0    13146 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/290212_7.24.xls
+-rw-r--r--   0        0        0    13141 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/290212_7.67.xls
+-rw-r--r--   0        0        0    13173 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/290212_8.23.xls
+-rw-r--r--   0        0        0    13171 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/290212_8.82.xls
+-rw-r--r--   0        0        0    13152 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/290212_9.31.xls
+-rw-r--r--   0        0        0    12930 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/290513_5.5.xls
+-rw-r--r--   0        0        0    11262 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/290513_5.5_bad.xls
+-rw-r--r--   0        0        0    12946 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/290513_7.2.xls
+-rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/290513_8.8.xls
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/list.cl
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/list.cl20
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/list.pH
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/list.pH2
+-rw-r--r--   0        0        0    14438 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/200214 pH data.ods
+-rw-r--r--   0        0        0    12835 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/NaCl1_200214.xls
+-rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/NaCl2_200214.xls
+-rw-r--r--   0        0        0    12802 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/NaCl3_200214.xls
+-rw-r--r--   0        0        0    12799 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/NaCl4_200214.xls
+-rw-r--r--   0        0        0    12812 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/NaCl5_200214.xls
+-rw-r--r--   0        0        0    12773 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/NaCl6_200214.xls
+-rw-r--r--   0        0        0    12783 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/NaCl7_200214.xls
+-rw-r--r--   0        0        0    12790 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/NaCl8_200214.xls
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/additions.cl
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/additions.pH
+-rw-r--r--   0        0        0    21877 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/fit0-1.csv
+-rw-r--r--   0        0        0    21592 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/fit0.csv
+-rw-r--r--   0        0        0    23056 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/fit1-1.csv
+-rw-r--r--   0        0        0    23182 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/fit1.csv
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/list.cl
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/list.pH
+-rw-r--r--   0        0        0    12865 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/pH5.0_200214.xls
+-rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/pH5.8_200214.xls
+-rw-r--r--   0        0        0    12889 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/pH6.5_200214.xls
+-rw-r--r--   0        0        0    12914 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/pH7.1_200214.xls
+-rw-r--r--   0        0        0    12934 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/pH7.6_200214.xls
+-rw-r--r--   0        0        0    12939 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/pH8.3_200214.xls
+-rw-r--r--   0        0        0    12937 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/pH9.1_200214.xls
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/scheme.txt
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/140220/scheme0.txt
+-rw-r--r--   0        0        0     9176 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/exceptions/0_Labelblocks_290513_5.5.xlsx
+-rw-r--r--   0        0        0    12275 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/exceptions/290212_7.67_repeated_lb.xls
+-rw-r--r--   0        0        0    10209 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/exceptions/84wells_290212_20.xlsx
+-rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/Tecan/exceptions/88wells_290212_20.xlsx
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/A01-20140311a.dat
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/A01.dat
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/A11.dat
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/B01.dat
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/H04.dat
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/NTT-A04-Cl_note
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/copyIP.txt
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/ratio2P.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/w.txt
+-rw-r--r--   0        0        0    43486 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/Meas/A04 Cl_A.csv
+-rw-r--r--   0        0        0   138192 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/Meas/A04 Cl_A.png
+-rw-r--r--   0        0        0    29087 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/Meas/A04 Cl_B.csv
+-rw-r--r--   0        0        0    97762 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/Meas/A04 Cl_B.png
+-rw-r--r--   0        0        0    35910 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/Meas/A04 Cl_C.csv
+-rw-r--r--   0        0        0   138239 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/Meas/A04 Cl_C.png
+-rw-r--r--   0        0        0    29248 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/Meas/A04 Cl_D.csv
+-rw-r--r--   0        0        0    84749 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/Meas/A04 Cl_D.png
+-rw-r--r--   0        0        0    35312 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/Meas/A04 Cl_E.csv
+-rw-r--r--   0        0        0   145114 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/Meas/A04 Cl_E.png
+-rw-r--r--   0        0        0    43756 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/Meas/A04 Cl_F.csv
+-rw-r--r--   0        0        0   126442 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/Meas/A04 Cl_F.png
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/global/Cl/A11-failed.dat
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/global/Cl/B05-20130628-cor.dat
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/global/pH/B01-failed.dat
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/global/pH/D05.dat
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/global/pH/H04-with_nan.dat
+-rw-r--r--   0        0        0   235947 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/k/D05.dat-bs.png
+-rw-r--r--   0        0        0    28093 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/k/D05.dat.png
+-rw-r--r--   0        0        0    12506 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/output/band_A04 Cl_A_NTT-A04-Cl_note.pdf
+-rw-r--r--   0        0        0    12433 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/output/band_A04 Cl_B_NTT-A04-Cl_note.pdf
+-rw-r--r--   0        0        0    66713 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/output/svd_A04 Cl_A_NTT-A04-Cl_note.pdf
+-rw-r--r--   0        0        0    39832 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/output/svd_A04 Cl_B_NTT-A04-Cl_note.pdf
+-rw-r--r--   0        0        0    32564 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/output/global/Cl/B05-20130628-cor.dat.png
+-rw-r--r--   0        0        0    36956 2020-02-02 00:00:00.000000 clophfit-0.4.8/tests/data/output/global/pH/D05.dat.png
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 clophfit-0.4.8/.gitignore
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 clophfit-0.4.8/LICENSE.txt
+-rw-r--r--   0        0        0    11370 2020-02-02 00:00:00.000000 clophfit-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0     5625 2020-02-02 00:00:00.000000 clophfit-0.4.8/docs/README.md
+-rw-r--r--   0        0        0     8467 2020-02-02 00:00:00.000000 clophfit-0.4.8/PKG-INFO
```

### Comparing `clophfit-0.4.7/.pre-commit-config.yaml` & `clophfit-0.4.8/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -31,34 +31,34 @@
     hooks:
       - id: pretty-format-ini
         args: [--autofix]
       - id: pretty-format-toml
         args: [--autofix]
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.257
+    rev: v0.0.263
     hooks:
       - id: ruff
 
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black-jupyter
       - id: black
         require_serial: true
 
   - repo: https://github.com/asottile/blacken-docs
     rev: 1.13.0
     hooks:
       - id: blacken-docs
         additional_dependencies: [black]
         exclude: docs/tutorials/usage.*.rst
 
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.0.0-alpha.6
+    rev: v3.0.0-alpha.9-for-vscode
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript, json]
         args: [--prose-wrap=always]
 
   - repo: https://github.com/pre-commit/pygrep-hooks
     rev: v1.10.0
@@ -67,20 +67,14 @@
       # - id: python-check-blanket-type-ignore # same as ruff PGH
       - id: python-no-eval
       - id: python-use-type-annotations
       - id: rst-backticks
       - id: rst-directive-colons
       - id: rst-inline-touching-normal
 
-  - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
-    hooks:
-      - id: pyupgrade
-        args: [--py38-plus]
-
   - repo: https://github.com/PyCQA/bandit
     rev: 1.7.5 # Update me!
     hooks:
       - id: bandit
         args: ["-c", "bandit.yml"]
         # additional_dependencies: ["bandit[toml]"]
 
@@ -98,12 +92,12 @@
   - repo: https://github.com/shellcheck-py/shellcheck-py
     rev: v0.9.0.2
     hooks:
       - id: shellcheck
         args: [-x]
 
   - repo: https://github.com/commitizen-tools/commitizen
-    rev: v2.42.1
+    rev: 3.2.0
     hooks:
       - id: commitizen
       - id: commitizen-branch
         stages: [push]
```

### Comparing `clophfit-0.4.7/CHANGELOG.md` & `clophfit-0.4.8/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,60 @@
 # Changelog
 
+## v0.4.8 (2023-05-02)
+
+### Docs
+
+- Lint README.md with markdownlint-cli
+
+### Build
+
+- update lmfit requirement from <1.1.1 to <1.2.1 (#213)
+- remove pyupgrade as ruff "UP" fully replaces it
+- bump pandas-stubs from 2.0.0.230412 to 2.0.1.230501 (#240)
+- update commitizen requirement from <3.1.1 to <3.2.1 (#239)
+- update coverage[toml] requirement from <7.2.4 to <7.2.6 (#238)
+- bump pip from 23.1.1 to 23.1.2 in /.github/workflows (#235)
+- update commitizen requirement from <2.42.2 to <3.1.1 (#234)
+- bump sphinx from 6.1.3 to 6.2.1 (#233)
+- bump ruff from 0.0.262 to 0.0.263 (#232)
+- update pandas requirement from <2.0.1 to <2.0.2 (#231)
+- bump pip from 23.1 to 23.1.1 in /.github/workflows (#229)
+- update numpy requirement from <1.24.3 to <1.24.4 (#227)
+- bump codecov/codecov-action from 3.1.2 to 3.1.3 (#225)
+- update corner requirement from <2.2.2 to <2.2.3 (#211)
+- update pygments requirement from <2.14.1 to <2.15.2 (#223)
+- bump pip from 23.0.1 to 23.1 in /.github/workflows (#222)
+- update pytest requirement from <7.2.3 to <7.3.2 (#220)
+- bump pandas-stubs from 1.5.3.230321 to 2.0.0.230412 (#218)
+- bump ruff from 0.0.260 to 0.0.262 (#224)
+- update rpy2 requirement from <3.5.11 to <3.5.12 (#221)
+- bump sphinx-autodoc-typehints from 1.22 to 1.23.0 (#219)
+- bump codecov/codecov-action from 3.1.1 to 3.1.2 (#217)
+- bump pip-deepfreeze from 1.1.0 to 1.2.0 in /.github/workflows (#216)
+- update mypy requirement from <1.2 to <1.3 (#210)
+- update coverage[toml] requirement from <7.2.3 to <7.2.4 (#209)
+- bump hatch from 1.6.3 to 1.7.0 in /.github/workflows (#207)
+- update pandas requirement from <1.5.4 to <2.0.1 (#205)
+- bump pydata-sphinx-theme from 0.13.1 to 0.13.3 (#204)
+- bump ruff from 0.0.259 to 0.0.260 (#203)
+- bump ruff from 0.0.258 to 0.0.259 (#201)
+- bump ruff from 0.0.257 to 0.0.258 (#199)
+- bump pandas-stubs from 1.5.3.230304 to 1.5.3.230321 (#198)
+
+### CI/CD
+
+- skip tests when only docs are changed
+
+### chore
+
+- update pre-commit hooks (#230)
+- update pre-commit hooks (#214)
+- update pre-commit hooks (#206)
+
 ## v0.4.7 (2023-03-21)
 
 ### Docs
 
 - Update Readme
 
 ### Build
```

### Comparing `clophfit-0.4.7/CONTRIBUTING.md` & `clophfit-0.4.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/cz_customize_info.txt` & `clophfit-0.4.8/cz_customize_info.txt`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/.github/workflows/cd.yml` & `clophfit-0.4.8/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/.github/workflows/ci.yml` & `clophfit-0.4.8/.github/workflows/ci.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Run lint, typeguard, mypy and xdoctest, and pytest which triggers coverage
 name: CI
 
 on:
   workflow_dispatch:
   pull_request:
+    paths-ignore:
+      - "docs/**"
+      - "*.md"
   push:
+    paths-ignore:
+      - "docs/**"
+      - "*.md"
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
 env:
   STABLE_PYTHON_VERSION: "3.11"
@@ -132,8 +138,8 @@
           name: coverage-data
       - name: Create coverage report
         run: |
           hatch run coverage:combine
           hatch run coverage:report
           hatch run coverage:xml
       - name: Upload coverage report
-        uses: codecov/codecov-action@v3.1.1
+        uses: codecov/codecov-action@v3.1.3
```

### Comparing `clophfit-0.4.7/.github/workflows/docs.yml` & `clophfit-0.4.8/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/Makefile` & `clophfit-0.4.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/conf.py` & `clophfit-0.4.8/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "ClopHfit"
 copyright = "2021, Daniele Arosio"  # noqa: A001
 author = "Daniele Arosio"
 
 # The full version, including alpha/beta/rc tags
-release = "0.4.7"
+release = "0.4.8"
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
```

### Comparing `clophfit-0.4.7/docs/make.bat` & `clophfit-0.4.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/bs_pd_f1.png` & `clophfit-0.4.8/docs/_static/bs_pd_f1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/bs_pd_f2.png` & `clophfit-0.4.8/docs/_static/bs_pd_f2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/bs_pd_f3.png` & `clophfit-0.4.8/docs/_static/bs_pd_f3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/bs_pd_f4.png` & `clophfit-0.4.8/docs/_static/bs_pd_f4.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/bs_pd_f5.png` & `clophfit-0.4.8/docs/_static/bs_pd_f5.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/bs_pd_f6.png` & `clophfit-0.4.8/docs/_static/bs_pd_f6.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/bs_pd_f7.png` & `clophfit-0.4.8/docs/_static/bs_pd_f7.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/csvtable.png` & `clophfit-0.4.8/docs/_static/csvtable.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/emcee-01.png` & `clophfit-0.4.8/docs/_static/emcee-01.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/emcee-02.png` & `clophfit-0.4.8/docs/_static/emcee-02.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/emcee-11.png` & `clophfit-0.4.8/docs/_static/emcee-11.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/emcee-12.png` & `clophfit-0.4.8/docs/_static/emcee-12.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/f01.png` & `clophfit-0.4.8/docs/_static/f01.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/file.png` & `clophfit-0.4.8/docs/_static/file.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/gR_fit1.png` & `clophfit-0.4.8/docs/_static/gR_fit1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/gR_fit2.png` & `clophfit-0.4.8/docs/_static/gR_fit2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/gR_fit3.png` & `clophfit-0.4.8/docs/_static/gR_fit3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/gR_fit4.png` & `clophfit-0.4.8/docs/_static/gR_fit4.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/gR_fit5.png` & `clophfit-0.4.8/docs/_static/gR_fit5.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/gR_fit6.png` & `clophfit-0.4.8/docs/_static/gR_fit6.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/gR_fit7.png` & `clophfit-0.4.8/docs/_static/gR_fit7.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/glmfit0.png` & `clophfit-0.4.8/docs/_static/glmfit0.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/glmfit1.png` & `clophfit-0.4.8/docs/_static/glmfit1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/glmfit2.png` & `clophfit-0.4.8/docs/_static/glmfit2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/glmfit3.png` & `clophfit-0.4.8/docs/_static/glmfit3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/glmfit_np.r_.png` & `clophfit-0.4.8/docs/_static/glmfit_np.r_.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/lmfit1.png` & `clophfit-0.4.8/docs/_static/lmfit1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/lmfit2.png` & `clophfit-0.4.8/docs/_static/lmfit2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/lmfit3.png` & `clophfit-0.4.8/docs/_static/lmfit3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/lmfit4.png` & `clophfit-0.4.8/docs/_static/lmfit4.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/lmfit5.png` & `clophfit-0.4.8/docs/_static/lmfit5.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/lmodel1.png` & `clophfit-0.4.8/docs/_static/lmodel1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/lmodel2.png` & `clophfit-0.4.8/docs/_static/lmodel2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/lmodel3.png` & `clophfit-0.4.8/docs/_static/lmodel3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/lmodel4.png` & `clophfit-0.4.8/docs/_static/lmodel4.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/lmodel5.png` & `clophfit-0.4.8/docs/_static/lmodel5.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/lmodel6.png` & `clophfit-0.4.8/docs/_static/lmodel6.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/lmodel_H04.png` & `clophfit-0.4.8/docs/_static/lmodel_H04.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/note_file.png` & `clophfit-0.4.8/docs/_static/note_file.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/r_bs.png` & `clophfit-0.4.8/docs/_static/r_bs.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/ratio2P-lmodel1.png` & `clophfit-0.4.8/docs/_static/ratio2P-lmodel1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/ratio2P-lmodel2.png` & `clophfit-0.4.8/docs/_static/ratio2P-lmodel2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/ratio2P_R1.png` & `clophfit-0.4.8/docs/_static/ratio2P_R1.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/ratio2P_R2.png` & `clophfit-0.4.8/docs/_static/ratio2P_R2.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/ratio2P_R3.png` & `clophfit-0.4.8/docs/_static/ratio2P_R3.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/ratio2P_R4.png` & `clophfit-0.4.8/docs/_static/ratio2P_R4.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/ratio2P_R5.png` & `clophfit-0.4.8/docs/_static/ratio2P_R5.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/ratio2P_R6.png` & `clophfit-0.4.8/docs/_static/ratio2P_R6.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/_static/rpy_bs.png` & `clophfit-0.4.8/docs/_static/rpy_bs.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/api/prtecan.uml.rst` & `clophfit-0.4.8/docs/api/prtecan.uml.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/references/description.rst` & `clophfit-0.4.8/docs/references/description.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/tutorials/prtecan.ipynb` & `clophfit-0.4.8/docs/tutorials/prtecan.ipynb`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/tutorials/usage.org` & `clophfit-0.4.8/docs/tutorials/usage.org`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/tutorials/usage.rst` & `clophfit-0.4.8/docs/tutorials/usage.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/tutorials/usage2.org` & `clophfit-0.4.8/docs/tutorials/usage2.org`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/docs/tutorials/usage2.rst` & `clophfit-0.4.8/docs/tutorials/usage2.rst`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/src/clophfit/__main__.py` & `clophfit-0.4.8/src/clophfit/__main__.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/src/clophfit/binding/fitting.py` & `clophfit-0.4.8/src/clophfit/binding/fitting.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/src/clophfit/old/dil_buffer.py` & `clophfit-0.4.8/src/clophfit/old/dil_buffer.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/src/clophfit/old/dil_correction.py` & `clophfit-0.4.8/src/clophfit/old/dil_correction.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/src/clophfit/old/fit_rpy.py` & `clophfit-0.4.8/src/clophfit/old/fit_rpy.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/src/clophfit/old/fit_titration.py` & `clophfit-0.4.8/src/clophfit/old/fit_titration.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/src/clophfit/old/fit_titration_global.py` & `clophfit-0.4.8/src/clophfit/old/fit_titration_global.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/src/clophfit/old/merge.py` & `clophfit-0.4.8/src/clophfit/old/merge.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/src/clophfit/old/plot_tecan.py` & `clophfit-0.4.8/src/clophfit/old/plot_tecan.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/src/clophfit/old/bash/w_ave.sh` & `clophfit-0.4.8/src/clophfit/old/bash/w_ave.sh`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/src/clophfit/prtecan/__init__.py` & `clophfit-0.4.8/src/clophfit/prtecan/__init__.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/src/clophfit/prtecan/prtecan.py` & `clophfit-0.4.8/src/clophfit/prtecan/prtecan.py`

 * *Files 1% similar despite different names*

```diff
@@ -350,15 +350,15 @@
                             stacklevel=2,
                         )
         except AssertionError as exc:
             msg = "Cannot extract data in Labelblock: not 96 wells?"
             raise ValueError(msg) from exc
         return data
 
-    _KEYS = [
+    _KEYS = [  # noqa: RUF008 "False positive for ClassVar"
         "Emission Bandwidth",
         "Emission Wavelength",
         "Excitation Bandwidth",
         "Excitation Wavelength",
         "Mode",
         "Integration Time",
         "Number of Flashes",
```

### Comparing `clophfit-0.4.7/tests/test_binding.py` & `clophfit-0.4.8/tests/test_binding.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/test_cli.py` & `clophfit-0.4.8/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/test_oldscripts.py` & `clophfit-0.4.8/tests/test_oldscripts.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         ],
     )
     def run_script(self, request: pytest.FixtureRequest) -> Iterator[Rscript]:
         """Run the script as class fixture."""
         cli = Path("../../src/clophfit/old/fit_titration.py")
         csv_file = request.param[0]
         with subprocess.Popen(  # nosec B603
-            [cli, csv_file, self.note_fp, "-t", "cl", "-d", "_tmpoutput"]
+            [cli, csv_file, self.note_fp, "-t", "cl", "-d", "_tmpoutput"]  # noqa: S603
             + request.param[2],
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             universal_newlines=True,
             cwd=_data,
         ) as process:
             yield request.param, process.communicate()
@@ -107,16 +107,16 @@
 SA2   11.0487   47.6023   76.2874     104.3   138.128
 SB2    491.64   534.936   571.809   611.045   664.602
   K   7.34376   7.51152   7.65166   7.80003   7.99971
 bootstrap:""",
         """SA1   26910.8   27072.2   27216.7   27361.3   27522.7
 SB1   916.697   1037.35   1144.64    1251.2   1369.35
 SA2   3813.97   3970.34   4110.42   4250.52   4406.96
-SB2      -INF   24.2754   87.1121   149.801   219.626
-  K   7.51099   7.78702   8.03882   8.29508   8.58663
+SB2      -INF   24.2754   87.1125   149.801   219.626
+  K   7.51099   7.78702   8.03881   8.29508   8.58663
 bootstrap:""",
     ]
 
     @pytest.fixture(
         scope="class",
         params=[
             (dat_files[0], res[0], ["--boot", "3"]),
@@ -129,15 +129,15 @@
         dat_file = request.param[0]
         with subprocess.Popen(  # nosec B603
             [cli, dat_file, "_tmpoutput"] + request.param[2],
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             universal_newlines=True,
             cwd=_data,
-            shell=False,
+            shell=False,  # noqa: S603
         ) as process:
             yield request.param, process.communicate()
 
     def test_stdout(self, run_script: Rscript) -> None:
         """It print out results."""
         expected = run_script[0][1]
         assert expected in run_script[1][0]
```

### Comparing `clophfit-0.4.7/tests/test_prtecan.py` & `clophfit-0.4.8/tests/test_prtecan.py`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/290212_100.xls` & `clophfit-0.4.8/tests/Tecan/290212_100.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/290212_150.xls` & `clophfit-0.4.8/tests/Tecan/290212_150.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/290212_20.xls` & `clophfit-0.4.8/tests/Tecan/290212_20.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/290212_5.78.xls` & `clophfit-0.4.8/tests/Tecan/290212_5.78.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/290212_50.xls` & `clophfit-0.4.8/tests/Tecan/290212_50.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/290212_6.38.xls` & `clophfit-0.4.8/tests/Tecan/290212_6.38.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/290212_6.83.xls` & `clophfit-0.4.8/tests/Tecan/290212_6.83.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/290212_7.24.xls` & `clophfit-0.4.8/tests/Tecan/290212_7.24.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/290212_7.67.xls` & `clophfit-0.4.8/tests/Tecan/290212_7.67.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/290212_8.23.xls` & `clophfit-0.4.8/tests/Tecan/290212_8.23.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/290212_8.82.xls` & `clophfit-0.4.8/tests/Tecan/290212_8.82.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/290212_9.31.xls` & `clophfit-0.4.8/tests/Tecan/290212_9.31.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/290513_5.5.xls` & `clophfit-0.4.8/tests/Tecan/290513_5.5.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/290513_5.5_bad.xls` & `clophfit-0.4.8/tests/Tecan/290513_5.5_bad.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/290513_7.2.xls` & `clophfit-0.4.8/tests/Tecan/290513_7.2.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/290513_8.8.xls` & `clophfit-0.4.8/tests/Tecan/290513_8.8.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/140220/200214 pH data.ods` & `clophfit-0.4.8/tests/Tecan/140220/200214 pH data.ods`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/140220/NaCl1_200214.xls` & `clophfit-0.4.8/tests/Tecan/140220/NaCl1_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/140220/NaCl2_200214.xls` & `clophfit-0.4.8/tests/Tecan/140220/NaCl2_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/140220/NaCl3_200214.xls` & `clophfit-0.4.8/tests/Tecan/140220/NaCl3_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/140220/NaCl4_200214.xls` & `clophfit-0.4.8/tests/Tecan/140220/NaCl4_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/140220/NaCl5_200214.xls` & `clophfit-0.4.8/tests/Tecan/140220/NaCl5_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/140220/NaCl6_200214.xls` & `clophfit-0.4.8/tests/Tecan/140220/NaCl6_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/140220/NaCl7_200214.xls` & `clophfit-0.4.8/tests/Tecan/140220/NaCl7_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/140220/NaCl8_200214.xls` & `clophfit-0.4.8/tests/Tecan/140220/NaCl8_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/140220/fit0-1.csv` & `clophfit-0.4.8/tests/Tecan/140220/fit0-1.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/140220/fit0.csv` & `clophfit-0.4.8/tests/Tecan/140220/fit0.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/140220/fit1-1.csv` & `clophfit-0.4.8/tests/Tecan/140220/fit1-1.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/140220/fit1.csv` & `clophfit-0.4.8/tests/Tecan/140220/fit1.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/140220/pH5.0_200214.xls` & `clophfit-0.4.8/tests/Tecan/140220/pH5.0_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/140220/pH5.8_200214.xls` & `clophfit-0.4.8/tests/Tecan/140220/pH5.8_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/140220/pH6.5_200214.xls` & `clophfit-0.4.8/tests/Tecan/140220/pH6.5_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/140220/pH7.1_200214.xls` & `clophfit-0.4.8/tests/Tecan/140220/pH7.1_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/140220/pH7.6_200214.xls` & `clophfit-0.4.8/tests/Tecan/140220/pH7.6_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/140220/pH8.3_200214.xls` & `clophfit-0.4.8/tests/Tecan/140220/pH8.3_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/140220/pH9.1_200214.xls` & `clophfit-0.4.8/tests/Tecan/140220/pH9.1_200214.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/exceptions/0_Labelblocks_290513_5.5.xlsx` & `clophfit-0.4.8/tests/Tecan/exceptions/0_Labelblocks_290513_5.5.xlsx`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/exceptions/290212_7.67_repeated_lb.xls` & `clophfit-0.4.8/tests/Tecan/exceptions/290212_7.67_repeated_lb.xls`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/exceptions/84wells_290212_20.xlsx` & `clophfit-0.4.8/tests/Tecan/exceptions/84wells_290212_20.xlsx`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/Tecan/exceptions/88wells_290212_20.xlsx` & `clophfit-0.4.8/tests/Tecan/exceptions/88wells_290212_20.xlsx`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/data/A01-20140311a.dat` & `clophfit-0.4.8/tests/data/A01-20140311a.dat`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/data/A01.dat` & `clophfit-0.4.8/tests/data/A01.dat`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/data/NTT-A04-Cl_note` & `clophfit-0.4.8/tests/data/NTT-A04-Cl_note`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/data/Meas/A04 Cl_A.csv` & `clophfit-0.4.8/tests/data/Meas/A04 Cl_A.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/data/Meas/A04 Cl_A.png` & `clophfit-0.4.8/tests/data/Meas/A04 Cl_A.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/data/Meas/A04 Cl_B.csv` & `clophfit-0.4.8/tests/data/Meas/A04 Cl_B.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/data/Meas/A04 Cl_B.png` & `clophfit-0.4.8/tests/data/Meas/A04 Cl_B.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/data/Meas/A04 Cl_C.csv` & `clophfit-0.4.8/tests/data/Meas/A04 Cl_C.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/data/Meas/A04 Cl_C.png` & `clophfit-0.4.8/tests/data/Meas/A04 Cl_C.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/data/Meas/A04 Cl_D.csv` & `clophfit-0.4.8/tests/data/Meas/A04 Cl_D.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/data/Meas/A04 Cl_D.png` & `clophfit-0.4.8/tests/data/Meas/A04 Cl_D.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/data/Meas/A04 Cl_E.csv` & `clophfit-0.4.8/tests/data/Meas/A04 Cl_E.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/data/Meas/A04 Cl_E.png` & `clophfit-0.4.8/tests/data/Meas/A04 Cl_E.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/data/Meas/A04 Cl_F.csv` & `clophfit-0.4.8/tests/data/Meas/A04 Cl_F.csv`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/data/Meas/A04 Cl_F.png` & `clophfit-0.4.8/tests/data/Meas/A04 Cl_F.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/data/k/D05.dat-bs.png` & `clophfit-0.4.8/tests/data/k/D05.dat-bs.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/data/k/D05.dat.png` & `clophfit-0.4.8/tests/data/k/D05.dat.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/data/output/band_A04 Cl_A_NTT-A04-Cl_note.pdf` & `clophfit-0.4.8/tests/data/output/band_A04 Cl_A_NTT-A04-Cl_note.pdf`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/data/output/band_A04 Cl_B_NTT-A04-Cl_note.pdf` & `clophfit-0.4.8/tests/data/output/band_A04 Cl_B_NTT-A04-Cl_note.pdf`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/data/output/svd_A04 Cl_A_NTT-A04-Cl_note.pdf` & `clophfit-0.4.8/tests/data/output/svd_A04 Cl_A_NTT-A04-Cl_note.pdf`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/data/output/svd_A04 Cl_B_NTT-A04-Cl_note.pdf` & `clophfit-0.4.8/tests/data/output/svd_A04 Cl_B_NTT-A04-Cl_note.pdf`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/data/output/global/Cl/B05-20130628-cor.dat.png` & `clophfit-0.4.8/tests/data/output/global/Cl/B05-20130628-cor.dat.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/tests/data/output/global/pH/D05.dat.png` & `clophfit-0.4.8/tests/data/output/global/pH/D05.dat.png`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/.gitignore` & `clophfit-0.4.8/.gitignore`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/LICENSE.txt` & `clophfit-0.4.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `clophfit-0.4.7/pyproject.toml` & `clophfit-0.4.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,22 +17,22 @@
   "Programming Language :: Unix Shell",
   "Intended Audience :: Science/Research",
   "Topic :: Scientific/Engineering",
   "Development Status :: 3 - Alpha"
 ]
 dependencies = [
   'click < 8.1.4',
-  'corner < 2.2.2',
+  'corner < 2.2.3',
   'emcee < 3.1.5',
-  'lmfit < 1.1.1',
+  'lmfit < 1.2.1',
   'matplotlib < 3.7.2',
-  'numpy < 1.24.3',
+  'numpy < 1.24.4',
   'openpyxl < 3.1.3',
-  'pandas < 1.5.4',
-  'rpy2 < 3.5.11',
+  'pandas < 2.0.2',
+  'rpy2 < 3.5.12',
   'scipy < 1.10.2',
   'seaborn < 0.12.3',
   'sympy < 1.11.2',
   'tqdm < 4.65.1',
   'xlrd < 2.0.2'
 ]
 description = "Cli for fitting macromolecule pH titration or binding assays data e.g. fluorescence spectra."
@@ -44,41 +44,41 @@
   "macromolecule binding"
 ]
 license = "BSD-3-Clause"
 license-files = {paths = ["LICENSE.txt"]}
 name = "clophfit"
 readme = "docs/README.md"
 requires-python = ">=3.8, <3.12"
-version = "0.4.7"
+version = "0.4.8"
 
 [project.optional-dependencies]
 dev = [
-  "commitizen < 2.42.2",
+  "commitizen < 3.2.1",
   "ipykernel",
   "jupyter",
-  "ruff == 0.0.257",
+  "ruff == 0.0.263",
   "pylsp-mypy",
   "python-lsp-ruff"
 ]
 docs = [
   "autodocsumm == 0.2.10",
   "myst-parser == 1.0.0",
   "nbsphinx == 0.9.1",
-  "pydata-sphinx-theme == 0.13.1",
-  "Sphinx == 6.1.3",
+  "pydata-sphinx-theme == 0.13.3",
+  "Sphinx == 6.2.1",
   "sphinx-click == 4.4.0",
-  "sphinx_autodoc_typehints == 1.22",
+  "sphinx_autodoc_typehints == 1.23.0",
   "sphinxcontrib-plantuml == 0.25"
 ]
 tests = [
-  "coverage[toml] < 7.2.3",
-  "mypy < 1.2",
-  "pandas-stubs == 1.5.3.230304",
-  "Pygments < 2.14.1",
-  "pytest < 7.2.3",
+  "coverage[toml] < 7.2.6",
+  "mypy < 1.3",
+  "pandas-stubs == 2.0.1.230501",
+  "Pygments < 2.15.2",
+  "pytest < 7.3.2",
   "typeguard < 2.13.4",
   "xdoctest < 1.1.2"
 ]
 
 [project.scripts]
 "clop" = "clophfit.__main__:clop"
 
@@ -106,15 +106,15 @@
 '''
 line-length = 88
 skip-string-normalization = false
 
 [tool.commitizen]
 name = "cz_customize"
 tag_format = "v$version"
-version = "0.4.7"
+version = "0.4.8"
 version_files = [
   "pyproject.toml:version",
   "docs/conf.py:release",
   "docs/README.md:Version"
 ]
 
 [tool.commitizen.customize]
@@ -377,15 +377,15 @@
   "PT",  # pytest-style
   "PTH",  # use-pathlib
   "Q",  # quotes
   "RUF",  # Ruff
   "S",  # bandit XXX
   "SIM",  # simplify
   "TID",  # tidy-imports
-  "UP",  # pyupgrade XXX
+  "UP",  # pyupgrade
   "YTT",  # 2020
   "W"  # pycodestyle
 ]
 
 [tool.ruff.isort]
 combine-as-imports = true
 force-single-line = true
```

### Comparing `clophfit-0.4.7/docs/README.md` & `clophfit-0.4.8/docs/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
+# ClopHfit
+
 [![PyPI](https://img.shields.io/pypi/v/ClopHfit.svg)](https://pypi.org/project/ClopHfit/)
 [![CI](https://github.com/darosio/ClopHfit/actions/workflows/ci.yml/badge.svg)](https://github.com/darosio/ClopHfit/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/darosio/ClopHfit/branch/main/graph/badge.svg?token=OU6F9VFUQ6)](https://codecov.io/gh/darosio/ClopHfit)
 [![RtD](https://readthedocs.org/projects/clophfit/badge/)](https://clophfit.readthedocs.io/)
 [![zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.6354112.svg)](https://doi.org/10.5281/zenodo.6354112)
 
-# ClopHfit
-
 Cli for fitting macromolecule pH titration or binding assay data, e.g.
 fluorescence spectra.
 
-- Version: "0.4.7"
+- Version: "0.4.8"
 
 ## Features
 
 - Plate Reader data Parser.
 - Perform non-linear least square fitting.
 - Extract and fit pH and chloride titrations of GFP libraries.
   - For 2 labelblocks (e.g. 400, 485 nm) fit data separately and globally.
@@ -28,23 +28,25 @@
 - Extract and fit titrations from a list of tecan files collected at various pH
   or chloride concentrations:
 
       clop prtecan --help
 
   For example:
 
-      clop prtecan list.pH -k ph --scheme ../scheme.txt --dil additions.pH --norm --out prova2 --Klim 6.8,8.4 --sel 7.6,20
+        clop prtecan list.pH -k ph --scheme ../scheme.txt --dil additions.pH \
+            --norm --out prova2 --Klim 6.8,8.4 --sel 7.6,20
 
   To reproduce older pr.tecan add `--no-weight` option:
 
-      clop prtecan list.pH -k ph --scheme ../scheme.txt --no-bg --no-weight --out 4old --Klim 6.8,8.4 --sel 7.6,20
+        clop prtecan list.pH -k ph --scheme ../scheme.txt --no-bg --no-weight \
+            --out 4old --Klim 6.8,8.4 --sel 7.6,20
 
 - Predict chloride dissociation constant `K_d` at given pH:
 
-      clop eq1 --help
+        clop eq1 --help
 
 To use clophfit in your python:
 
     from clophfit import prtecan, binding
 
 ## Installation
 
@@ -60,53 +62,48 @@
 You need the following requirements:
 
 - `hatch` for test automation and package dependency managements. If you don't
   have hatch, you can use `pipx run hatch` to run it without installing, or
   `pipx install hatch`. Dependencies are locked thanks to
   [pip-deepfreeze](https://pypi.org/project/pip-deepfreeze/). You can run
   `hatch env show` to list available environments and scripts.
-  ```bash
-  hatch run init  # init repo with pre-commit hooks
-  hatch run sync  # sync venv with deepfreeze
-  # other examples
-  hatch run lint:run
-  hatch run tests.py3.10:all
-  ```
+
+        hatch run init  # init repo with pre-commit hooks
+        hatch run sync  # sync venv with deepfreeze
+
+        hatch run lint:run
+        hatch run tests.py3.10:all
+
   Hatch handles everything for you, including setting up an temporary virtual
   environment for each run.
+
 - `pre-commit` for all style and consistency checking. While you can run it with
   nox, this is such an important tool that it deserves to be installed on its
   own. If pre-commit fails during pushing upstream then stage changes, Commit
   Extend (into previous commit), and repeat pushing.
 
 `pip`, `pip-deepfreeze` and `hatch` are pinned in
 .github/workflows/constraints.txt for consistency with CI/CD.
 
-```bash
-pipx install pre-commit
-pipx install hatch
-pipx runpip hatch install hatch-pip-deepfreeze
-```
+    pipx install pre-commit
+    pipx install hatch
+    pipx runpip hatch install hatch-pip-deepfreeze
 
 ### Setting up a development with direnv
 
-```bash
-echo "layout hatch" > .envrc
-hatch run init
-```
+    echo "layout hatch" > .envrc
+    hatch run init
 
 ### Setting up a development environment manually
 
 You can set up a development environment by running:
 
-```bash
-python3 -m venv .venv
-source ./.venv/bin/activate
-pip install -v -e .[dev,tests,docs]
-```
+    python3 -m venv .venv
+    source ./.venv/bin/activate
+    pip install -v -e .[dev,tests,docs]
 
 With direnv for using [Jupyter](https://jupyter.org/) during development:
 
     jupiter notebook
 
 And only in case you need a system wide easy accessible kernel:
 
@@ -144,25 +141,27 @@
     sphinx-apidoc -f -o docs/api/ src/clophfit/
 
 ### Bump and releasing
 
 To bump version and upload build to test.pypi using:
 
     hatch run bump
-    hatch run bump "--increment PATCH" "--files-only" ["--no-verify" to bypass pre-commit and commit-msg hooks]
+    hatch run bump "--increment PATCH" "--files-only" \
+        ["--no-verify" to bypass pre-commit and commit-msg hooks]
 
 while to update only the CHANGELOG.md file:
 
     hatch run ch
 
 Release will automatically occur after pushing.
 
-(Alternatively)
+(Otherwise)
 
-    pipx run --spec commitizen cz bump --changelog-to-stdout --files-only (--prerelease alpha) --increment MINOR
+    pipx run --spec commitizen cz bump --changelog-to-stdout --files-only \
+        (--prerelease alpha) --increment MINOR
 
 To keep clean development history use branches and pr:
 
     gh pr create --fill
     gh pr merge --squash --delete-branch [-t “fix|ci|feat: msg”]
 
 ### Configuration files
@@ -184,11 +183,9 @@
 - mypy configured in pyproject.toml (tests deps);
 - commitizen in pyproject.toml (dev deps and pinned in pre-commit).
 
 pip-df generates requirements[-dev,docs,tests].txt.
 
 Other manual actions:
 
-```bash
-pylint src/ tests/
-bandit -r src/
-```
+    pylint src/ tests/
+    bandit -r src/
```

### Comparing `clophfit-0.4.7/PKG-INFO` & `clophfit-0.4.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clophfit
-Version: 0.4.7
+Version: 0.4.8
 Summary: Cli for fitting macromolecule pH titration or binding assays data e.g. fluorescence spectra.
 Project-URL: Bug Tracker, https://github.com/darosio/ClopHfit/issues
 Project-URL: Changelog, https://darosio.github.io/ClopHfit/misc/CHANGELOG.html
 Project-URL: Discussions, https://github.com/darosio/ClopHfit/discussions
 Project-URL: Documentation, https://clophfit.readthedocs.io
 Project-URL: Github releases, https://github.com/darosio/ClopHfit/releases
 Project-URL: Homepage, https://github.com/darosio/ClopHfit
@@ -21,65 +21,65 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Unix Shell
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: <3.12,>=3.8
 Requires-Dist: click<8.1.4
-Requires-Dist: corner<2.2.2
+Requires-Dist: corner<2.2.3
 Requires-Dist: emcee<3.1.5
-Requires-Dist: lmfit<1.1.1
+Requires-Dist: lmfit<1.2.1
 Requires-Dist: matplotlib<3.7.2
-Requires-Dist: numpy<1.24.3
+Requires-Dist: numpy<1.24.4
 Requires-Dist: openpyxl<3.1.3
-Requires-Dist: pandas<1.5.4
-Requires-Dist: rpy2<3.5.11
+Requires-Dist: pandas<2.0.2
+Requires-Dist: rpy2<3.5.12
 Requires-Dist: scipy<1.10.2
 Requires-Dist: seaborn<0.12.3
 Requires-Dist: sympy<1.11.2
 Requires-Dist: tqdm<4.65.1
 Requires-Dist: xlrd<2.0.2
 Provides-Extra: dev
-Requires-Dist: commitizen<2.42.2; extra == 'dev'
+Requires-Dist: commitizen<3.2.1; extra == 'dev'
 Requires-Dist: ipykernel; extra == 'dev'
 Requires-Dist: jupyter; extra == 'dev'
 Requires-Dist: pylsp-mypy; extra == 'dev'
 Requires-Dist: python-lsp-ruff; extra == 'dev'
-Requires-Dist: ruff==0.0.257; extra == 'dev'
+Requires-Dist: ruff==0.0.263; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: autodocsumm==0.2.10; extra == 'docs'
 Requires-Dist: myst-parser==1.0.0; extra == 'docs'
 Requires-Dist: nbsphinx==0.9.1; extra == 'docs'
-Requires-Dist: pydata-sphinx-theme==0.13.1; extra == 'docs'
-Requires-Dist: sphinx-autodoc-typehints==1.22; extra == 'docs'
+Requires-Dist: pydata-sphinx-theme==0.13.3; extra == 'docs'
+Requires-Dist: sphinx-autodoc-typehints==1.23.0; extra == 'docs'
 Requires-Dist: sphinx-click==4.4.0; extra == 'docs'
-Requires-Dist: sphinx==6.1.3; extra == 'docs'
+Requires-Dist: sphinx==6.2.1; extra == 'docs'
 Requires-Dist: sphinxcontrib-plantuml==0.25; extra == 'docs'
 Provides-Extra: tests
-Requires-Dist: coverage[toml]<7.2.3; extra == 'tests'
-Requires-Dist: mypy<1.2; extra == 'tests'
-Requires-Dist: pandas-stubs==1.5.3.230304; extra == 'tests'
-Requires-Dist: pygments<2.14.1; extra == 'tests'
-Requires-Dist: pytest<7.2.3; extra == 'tests'
+Requires-Dist: coverage[toml]<7.2.6; extra == 'tests'
+Requires-Dist: mypy<1.3; extra == 'tests'
+Requires-Dist: pandas-stubs==2.0.1.230501; extra == 'tests'
+Requires-Dist: pygments<2.15.2; extra == 'tests'
+Requires-Dist: pytest<7.3.2; extra == 'tests'
 Requires-Dist: typeguard<2.13.4; extra == 'tests'
 Requires-Dist: xdoctest<1.1.2; extra == 'tests'
 Description-Content-Type: text/markdown
 
+# ClopHfit
+
 [![PyPI](https://img.shields.io/pypi/v/ClopHfit.svg)](https://pypi.org/project/ClopHfit/)
 [![CI](https://github.com/darosio/ClopHfit/actions/workflows/ci.yml/badge.svg)](https://github.com/darosio/ClopHfit/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/darosio/ClopHfit/branch/main/graph/badge.svg?token=OU6F9VFUQ6)](https://codecov.io/gh/darosio/ClopHfit)
 [![RtD](https://readthedocs.org/projects/clophfit/badge/)](https://clophfit.readthedocs.io/)
 [![zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.6354112.svg)](https://doi.org/10.5281/zenodo.6354112)
 
-# ClopHfit
-
 Cli for fitting macromolecule pH titration or binding assay data, e.g.
 fluorescence spectra.
 
-- Version: "0.4.7"
+- Version: "0.4.8"
 
 ## Features
 
 - Plate Reader data Parser.
 - Perform non-linear least square fitting.
 - Extract and fit pH and chloride titrations of GFP libraries.
   - For 2 labelblocks (e.g. 400, 485 nm) fit data separately and globally.
@@ -94,23 +94,25 @@
 - Extract and fit titrations from a list of tecan files collected at various pH
   or chloride concentrations:
 
       clop prtecan --help
 
   For example:
 
-      clop prtecan list.pH -k ph --scheme ../scheme.txt --dil additions.pH --norm --out prova2 --Klim 6.8,8.4 --sel 7.6,20
+        clop prtecan list.pH -k ph --scheme ../scheme.txt --dil additions.pH \
+            --norm --out prova2 --Klim 6.8,8.4 --sel 7.6,20
 
   To reproduce older pr.tecan add `--no-weight` option:
 
-      clop prtecan list.pH -k ph --scheme ../scheme.txt --no-bg --no-weight --out 4old --Klim 6.8,8.4 --sel 7.6,20
+        clop prtecan list.pH -k ph --scheme ../scheme.txt --no-bg --no-weight \
+            --out 4old --Klim 6.8,8.4 --sel 7.6,20
 
 - Predict chloride dissociation constant `K_d` at given pH:
 
-      clop eq1 --help
+        clop eq1 --help
 
 To use clophfit in your python:
 
     from clophfit import prtecan, binding
 
 ## Installation
 
@@ -126,53 +128,48 @@
 You need the following requirements:
 
 - `hatch` for test automation and package dependency managements. If you don't
   have hatch, you can use `pipx run hatch` to run it without installing, or
   `pipx install hatch`. Dependencies are locked thanks to
   [pip-deepfreeze](https://pypi.org/project/pip-deepfreeze/). You can run
   `hatch env show` to list available environments and scripts.
-  ```bash
-  hatch run init  # init repo with pre-commit hooks
-  hatch run sync  # sync venv with deepfreeze
-  # other examples
-  hatch run lint:run
-  hatch run tests.py3.10:all
-  ```
+
+        hatch run init  # init repo with pre-commit hooks
+        hatch run sync  # sync venv with deepfreeze
+
+        hatch run lint:run
+        hatch run tests.py3.10:all
+
   Hatch handles everything for you, including setting up an temporary virtual
   environment for each run.
+
 - `pre-commit` for all style and consistency checking. While you can run it with
   nox, this is such an important tool that it deserves to be installed on its
   own. If pre-commit fails during pushing upstream then stage changes, Commit
   Extend (into previous commit), and repeat pushing.
 
 `pip`, `pip-deepfreeze` and `hatch` are pinned in
 .github/workflows/constraints.txt for consistency with CI/CD.
 
-```bash
-pipx install pre-commit
-pipx install hatch
-pipx runpip hatch install hatch-pip-deepfreeze
-```
+    pipx install pre-commit
+    pipx install hatch
+    pipx runpip hatch install hatch-pip-deepfreeze
 
 ### Setting up a development with direnv
 
-```bash
-echo "layout hatch" > .envrc
-hatch run init
-```
+    echo "layout hatch" > .envrc
+    hatch run init
 
 ### Setting up a development environment manually
 
 You can set up a development environment by running:
 
-```bash
-python3 -m venv .venv
-source ./.venv/bin/activate
-pip install -v -e .[dev,tests,docs]
-```
+    python3 -m venv .venv
+    source ./.venv/bin/activate
+    pip install -v -e .[dev,tests,docs]
 
 With direnv for using [Jupyter](https://jupyter.org/) during development:
 
     jupiter notebook
 
 And only in case you need a system wide easy accessible kernel:
 
@@ -210,25 +207,27 @@
     sphinx-apidoc -f -o docs/api/ src/clophfit/
 
 ### Bump and releasing
 
 To bump version and upload build to test.pypi using:
 
     hatch run bump
-    hatch run bump "--increment PATCH" "--files-only" ["--no-verify" to bypass pre-commit and commit-msg hooks]
+    hatch run bump "--increment PATCH" "--files-only" \
+        ["--no-verify" to bypass pre-commit and commit-msg hooks]
 
 while to update only the CHANGELOG.md file:
 
     hatch run ch
 
 Release will automatically occur after pushing.
 
-(Alternatively)
+(Otherwise)
 
-    pipx run --spec commitizen cz bump --changelog-to-stdout --files-only (--prerelease alpha) --increment MINOR
+    pipx run --spec commitizen cz bump --changelog-to-stdout --files-only \
+        (--prerelease alpha) --increment MINOR
 
 To keep clean development history use branches and pr:
 
     gh pr create --fill
     gh pr merge --squash --delete-branch [-t “fix|ci|feat: msg”]
 
 ### Configuration files
@@ -250,11 +249,9 @@
 - mypy configured in pyproject.toml (tests deps);
 - commitizen in pyproject.toml (dev deps and pinned in pre-commit).
 
 pip-df generates requirements[-dev,docs,tests].txt.
 
 Other manual actions:
 
-```bash
-pylint src/ tests/
-bandit -r src/
-```
+    pylint src/ tests/
+    bandit -r src/
```

