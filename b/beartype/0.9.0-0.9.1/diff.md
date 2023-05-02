# Comparing `tmp/beartype-0.9.0.tar.gz` & `tmp/beartype-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beartype-0.9.0.tar", last modified: Fri Oct 22 07:49:33 2021, max compression
+gzip compressed data, was "beartype-0.9.1.tar", last modified: Sat Nov  6 06:22:34 2021, max compression
```

## Comparing `beartype-0.9.0.tar` & `beartype-0.9.1.tar`

### file list

```diff
@@ -1,429 +1,463 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.074188 beartype-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)     2392 2021-10-22 07:49:23.000000 beartype-0.9.0/.mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)     1140 2021-10-22 07:49:23.000000 beartype-0.9.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2021-10-22 07:49:23.000000 beartype-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1841 2021-10-22 07:49:23.000000 beartype-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)   230609 2021-10-22 07:49:33.074188 beartype-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)   228989 2021-10-22 07:49:23.000000 beartype-0.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.026188 beartype-0.9.0/beartype/
--rw-r--r--   0 runner    (1001) docker     (121)     9579 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.026188 beartype-0.9.0/beartype/_cave/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_cave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6290 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_cave/_caveabc.py
--rw-r--r--   0 runner    (1001) docker     (121)    52238 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_cave/_cavefast.py
--rw-r--r--   0 runner    (1001) docker     (121)    10240 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_cave/_cavemap.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.026188 beartype-0.9.0/beartype/_data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.026188 beartype-0.9.0/beartype/_data/cls/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_data/cls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2397 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_data/cls/datacls.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.026188 beartype-0.9.0/beartype/_data/func/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_data/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1901 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_data/func/datafunc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.026188 beartype-0.9.0/beartype/_data/hint/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_data/hint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.030188 beartype-0.9.0/beartype/_data/hint/pep/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_data/hint/pep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    28064 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_data/hint/pep/datapeprepr.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.030188 beartype-0.9.0/beartype/_data/hint/pep/sign/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_data/hint/pep/sign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2717 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_data/hint/pep/sign/datapepsigncls.py
--rw-r--r--   0 runner    (1001) docker     (121)     9525 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_data/hint/pep/sign/datapepsigns.py
--rw-r--r--   0 runner    (1001) docker     (121)    16548 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_data/hint/pep/sign/datapepsignset.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.030188 beartype-0.9.0/beartype/_data/mod/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_data/mod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1989 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_data/mod/datamod.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.030188 beartype-0.9.0/beartype/_decor/
--rw-r--r--   0 runner    (1001) docker     (121)     7639 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_decor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.030188 beartype-0.9.0/beartype/_decor/_cache/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_decor/_cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16796 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_decor/_cache/cachetype.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.030188 beartype-0.9.0/beartype/_decor/_code/
--rw-r--r--   0 runner    (1001) docker     (121)    35282 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_decor/_code/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.030188 beartype-0.9.0/beartype/_decor/_code/_pep/
--rw-r--r--   0 runner    (1001) docker     (121)    92720 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_decor/_code/_pep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   119812 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_decor/_code/_pep/_pephint.py
--rw-r--r--   0 runner    (1001) docker     (121)     5852 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_decor/_code/_pep/_pepmagic.py
--rw-r--r--   0 runner    (1001) docker     (121)    21260 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_decor/_code/_pep/_pepscope.py
--rw-r--r--   0 runner    (1001) docker     (121)    23177 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_decor/_code/_pep/_pepsnip.py
--rw-r--r--   0 runner    (1001) docker     (121)    14095 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_decor/_code/_pep/pepcode.py
--rw-r--r--   0 runner    (1001) docker     (121)    21062 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_decor/_code/codemain.py
--rw-r--r--   0 runner    (1001) docker     (121)    10889 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_decor/_code/codesnip.py
--rw-r--r--   0 runner    (1001) docker     (121)    13684 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_decor/_data.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.034188 beartype-0.9.0/beartype/_decor/_error/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_decor/_error/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17029 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_decor/_error/_errorsleuth.py
--rw-r--r--   0 runner    (1001) docker     (121)    10010 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_decor/_error/_errortype.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.034188 beartype-0.9.0/beartype/_decor/_error/_pep/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_decor/_error/_pep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4720 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_decor/_error/_pep/_errorpep586.py
--rw-r--r--   0 runner    (1001) docker     (121)     4279 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_decor/_error/_pep/_errorpep593.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.034188 beartype-0.9.0/beartype/_decor/_error/_pep/_pep484/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_decor/_error/_pep/_pep484/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1934 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_decor/_error/_pep/_pep484/_errornoreturn.py
--rw-r--r--   0 runner    (1001) docker     (121)     9696 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_decor/_error/_pep/_pep484/_errorunion.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.034188 beartype-0.9.0/beartype/_decor/_error/_pep/_pep484585/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_decor/_error/_pep/_pep484585/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5751 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_decor/_error/_pep/_pep484585/_errorgeneric.py
--rw-r--r--   0 runner    (1001) docker     (121)    13984 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_decor/_error/_pep/_pep484585/_errorsequence.py
--rw-r--r--   0 runner    (1001) docker     (121)    18761 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_decor/_error/errormain.py
--rw-r--r--   0 runner    (1001) docker     (121)    28338 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_decor/_pep563.py
--rw-r--r--   0 runner    (1001) docker     (121)    13940 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_decor/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.034188 beartype-0.9.0/beartype/_util/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.034188 beartype-0.9.0/beartype/_util/cache/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/cache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.034188 beartype-0.9.0/beartype/_util/cache/map/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/cache/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8884 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/cache/map/utilmapbig.py
--rw-r--r--   0 runner    (1001) docker     (121)     8711 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/cache/map/utilmaplru.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.034188 beartype-0.9.0/beartype/_util/cache/pool/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/cache/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10391 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/cache/pool/utilcachepool.py
--rw-r--r--   0 runner    (1001) docker     (121)    14177 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/cache/pool/utilcachepoollistfixed.py
--rw-r--r--   0 runner    (1001) docker     (121)     4268 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/cache/pool/utilcachepoolobjecttyped.py
--rw-r--r--   0 runner    (1001) docker     (121)    16321 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/cache/utilcachecall.py
--rw-r--r--   0 runner    (1001) docker     (121)    10013 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/cache/utilcacheerror.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.034188 beartype-0.9.0/beartype/_util/cls/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/cls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.038188 beartype-0.9.0/beartype/_util/cls/pep/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/cls/pep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    27282 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/cls/pep/utilpep3119.py
--rw-r--r--   0 runner    (1001) docker     (121)     8604 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/cls/utilclstest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.038188 beartype-0.9.0/beartype/_util/func/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20691 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/func/utilfuncarg.py
--rw-r--r--   0 runner    (1001) docker     (121)    32110 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/func/utilfunccode.py
--rw-r--r--   0 runner    (1001) docker     (121)    12617 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/func/utilfunccodeobj.py
--rw-r--r--   0 runner    (1001) docker     (121)     7079 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/func/utilfuncfile.py
--rw-r--r--   0 runner    (1001) docker     (121)    12462 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/func/utilfuncmake.py
--rw-r--r--   0 runner    (1001) docker     (121)    27901 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/func/utilfuncscope.py
--rw-r--r--   0 runner    (1001) docker     (121)     2408 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/func/utilfuncstack.py
--rw-r--r--   0 runner    (1001) docker     (121)    13631 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/func/utilfunctest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2132 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/func/utilfuncwrap.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.038188 beartype-0.9.0/beartype/_util/hint/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/hint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.038188 beartype-0.9.0/beartype/_util/hint/nonpep/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/hint/nonpep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    23408 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/hint/nonpep/utilnonpeptest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.038188 beartype-0.9.0/beartype/_util/hint/pep/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/hint/pep/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.038188 beartype-0.9.0/beartype/_util/hint/pep/mod/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/hint/pep/mod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16171 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/hint/pep/mod/utilmodnumpy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.042188 beartype-0.9.0/beartype/_util/hint/pep/proposal/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/hint/pep/proposal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.042188 beartype-0.9.0/beartype/_util/hint/pep/proposal/pep484/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/hint/pep/proposal/pep484/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8032 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/hint/pep/proposal/pep484/utilpep484.py
--rw-r--r--   0 runner    (1001) docker     (121)    21106 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/hint/pep/proposal/pep484/utilpep484generic.py
--rw-r--r--   0 runner    (1001) docker     (121)     6487 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/hint/pep/proposal/pep484/utilpep484newtype.py
--rw-r--r--   0 runner    (1001) docker     (121)     4877 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/hint/pep/proposal/pep484/utilpep484ref.py
--rw-r--r--   0 runner    (1001) docker     (121)     5242 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/hint/pep/proposal/pep484/utilpep484typevar.py
--rw-r--r--   0 runner    (1001) docker     (121)     1902 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/hint/pep/proposal/pep484/utilpep484union.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.042188 beartype-0.9.0/beartype/_util/hint/pep/proposal/pep484585/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/hint/pep/proposal/pep484585/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3119 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/hint/pep/proposal/pep484585/utilpep484585.py
--rw-r--r--   0 runner    (1001) docker     (121)     5515 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/hint/pep/proposal/pep484585/utilpep484585arg.py
--rw-r--r--   0 runner    (1001) docker     (121)     7703 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/hint/pep/proposal/pep484585/utilpep484585func.py
--rw-r--r--   0 runner    (1001) docker     (121)    19726 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/hint/pep/proposal/pep484585/utilpep484585generic.py
--rw-r--r--   0 runner    (1001) docker     (121)    12753 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/hint/pep/proposal/pep484585/utilpep484585ref.py
--rw-r--r--   0 runner    (1001) docker     (121)    12540 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/hint/pep/proposal/pep484585/utilpep484585type.py
--rw-r--r--   0 runner    (1001) docker     (121)    18455 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/hint/pep/proposal/utilpep544.py
--rw-r--r--   0 runner    (1001) docker     (121)    12380 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/hint/pep/proposal/utilpep585.py
--rw-r--r--   0 runner    (1001) docker     (121)     9655 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/hint/pep/proposal/utilpep586.py
--rw-r--r--   0 runner    (1001) docker     (121)     7298 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/hint/pep/proposal/utilpep589.py
--rw-r--r--   0 runner    (1001) docker     (121)    11437 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/hint/pep/proposal/utilpep593.py
--rw-r--r--   0 runner    (1001) docker     (121)     2172 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/hint/pep/utilpepattr.py
--rw-r--r--   0 runner    (1001) docker     (121)    38455 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/hint/pep/utilpepget.py
--rw-r--r--   0 runner    (1001) docker     (121)    38662 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/hint/pep/utilpeptest.py
--rw-r--r--   0 runner    (1001) docker     (121)    36988 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/hint/utilhintconv.py
--rw-r--r--   0 runner    (1001) docker     (121)      677 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/hint/utilhintget.py
--rw-r--r--   0 runner    (1001) docker     (121)     7208 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/hint/utilhinttest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.042188 beartype-0.9.0/beartype/_util/kind/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/kind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13988 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/kind/utilkinddict.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.046188 beartype-0.9.0/beartype/_util/mod/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/mod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7486 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/mod/utilmoddeprecate.py
--rw-r--r--   0 runner    (1001) docker     (121)    19437 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/mod/utilmodimport.py
--rw-r--r--   0 runner    (1001) docker     (121)    15861 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/mod/utilmodtest.py
--rw-r--r--   0 runner    (1001) docker     (121)     5394 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/mod/utilmodule.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.046188 beartype-0.9.0/beartype/_util/os/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/os/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1027 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/os/utilostest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.046188 beartype-0.9.0/beartype/_util/py/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      910 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/py/utilpyinterpreter.py
--rw-r--r--   0 runner    (1001) docker     (121)     3173 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/py/utilpyversion.py
--rw-r--r--   0 runner    (1001) docker     (121)     2412 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/py/utilpyword.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.046188 beartype-0.9.0/beartype/_util/text/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3729 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/text/utiltextget.py
--rw-r--r--   0 runner    (1001) docker     (121)     3617 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/text/utiltextident.py
--rw-r--r--   0 runner    (1001) docker     (121)     6883 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/text/utiltextjoin.py
--rw-r--r--   0 runner    (1001) docker     (121)    13642 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/text/utiltextlabel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1490 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/text/utiltextmagic.py
--rw-r--r--   0 runner    (1001) docker     (121)     5520 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/text/utiltextmunge.py
--rw-r--r--   0 runner    (1001) docker     (121)    10110 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/text/utiltextrepr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1674 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/text/utiltexttest.py
--rw-r--r--   0 runner    (1001) docker     (121)    12264 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/utilobject.py
--rw-r--r--   0 runner    (1001) docker     (121)     2321 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/_util/utiltyping.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.046188 beartype-0.9.0/beartype/cave/
--rw-r--r--   0 runner    (1001) docker     (121)    17656 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/cave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11300 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/cave/_cavelib.py
--rw-r--r--   0 runner    (1001) docker     (121)    21454 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/meta.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.046188 beartype-0.9.0/beartype/roar/
--rw-r--r--   0 runner    (1001) docker     (121)     7031 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/roar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    30588 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/roar/_roarexc.py
--rw-r--r--   0 runner    (1001) docker     (121)    11764 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/roar/_roarwarn.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.046188 beartype-0.9.0/beartype/vale/
--rw-r--r--   0 runner    (1001) docker     (121)     5848 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/vale/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.050188 beartype-0.9.0/beartype/vale/_factory/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/vale/_factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14862 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/vale/_factory/_valeis.py
--rw-r--r--   0 runner    (1001) docker     (121)     6403 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/vale/_factory/_valeisabc.py
--rw-r--r--   0 runner    (1001) docker     (121)    10496 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/vale/_factory/_valeiscls.py
--rw-r--r--   0 runner    (1001) docker     (121)    18303 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/vale/_factory/_valeisobj.py
--rw-r--r--   0 runner    (1001) docker     (121)    12083 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/vale/_factory/_valeisoper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.050188 beartype-0.9.0/beartype/vale/_util/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/vale/_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4249 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/vale/_util/_valeutilsnip.py
--rw-r--r--   0 runner    (1001) docker     (121)      617 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/vale/_util/_valeutiltest.py
--rw-r--r--   0 runner    (1001) docker     (121)    21503 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype/vale/_valevale.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.026188 beartype-0.9.0/beartype.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)   230609 2021-10-22 07:49:32.000000 beartype-0.9.0/beartype.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14486 2021-10-22 07:49:32.000000 beartype-0.9.0/beartype.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-22 07:49:32.000000 beartype-0.9.0/beartype.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-22 07:49:32.000000 beartype-0.9.0/beartype.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      278 2021-10-22 07:49:32.000000 beartype-0.9.0/beartype.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-10-22 07:49:32.000000 beartype-0.9.0/beartype.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.050188 beartype-0.9.0/beartype_test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.050188 beartype-0.9.0/beartype_test/a00_unit/
--rw-r--r--   0 runner    (1001) docker     (121)      489 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.050188 beartype-0.9.0/beartype_test/a00_unit/a00_util/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.050188 beartype-0.9.0/beartype_test/a00_unit/a00_util/cache/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.050188 beartype-0.9.0/beartype_test/a00_unit/a00_util/cache/map/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/cache/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2634 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/cache/map/test_utilmapbig.py
--rw-r--r--   0 runner    (1001) docker     (121)     5007 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/cache/map/test_utilmaplru.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.050188 beartype-0.9.0/beartype_test/a00_unit/a00_util/cache/pool/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/cache/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5703 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/cache/pool/test_utilcachepool.py
--rw-r--r--   0 runner    (1001) docker     (121)     8057 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/cache/pool/test_utilcachepoollistfixed.py
--rw-r--r--   0 runner    (1001) docker     (121)     4661 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/cache/pool/test_utilcachepoolobjecttyped.py
--rw-r--r--   0 runner    (1001) docker     (121)     5027 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/cache/test_utilcachecall.py
--rw-r--r--   0 runner    (1001) docker     (121)     4779 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/cache/test_utilcacheerror.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.050188 beartype-0.9.0/beartype_test/a00_unit/a00_util/cls/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/cls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.050188 beartype-0.9.0/beartype_test/a00_unit/a00_util/cls/pep/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/cls/pep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2854 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/cls/pep/test_utilpep3119.py
--rw-r--r--   0 runner    (1001) docker     (121)     3472 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/cls/test_utilclstest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.054188 beartype-0.9.0/beartype_test/a00_unit/a00_util/func/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6687 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/func/test_utilfuncarg.py
--rw-r--r--   0 runner    (1001) docker     (121)     4827 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/func/test_utilfunccode.py
--rw-r--r--   0 runner    (1001) docker     (121)     7703 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/func/test_utilfunccodeobj.py
--rw-r--r--   0 runner    (1001) docker     (121)     1711 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/func/test_utilfuncfile.py
--rw-r--r--   0 runner    (1001) docker     (121)      808 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/func/test_utilfuncget.py
--rw-r--r--   0 runner    (1001) docker     (121)     8451 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/func/test_utilfuncmake.py
--rw-r--r--   0 runner    (1001) docker     (121)     8907 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/func/test_utilfuncscope.py
--rw-r--r--   0 runner    (1001) docker     (121)     1154 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/func/test_utilfuncstack.py
--rw-r--r--   0 runner    (1001) docker     (121)     9076 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/func/test_utilfunctest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1855 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/func/test_utilfuncwrap.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.054188 beartype-0.9.0/beartype_test/a00_unit/a00_util/hint/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/hint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.054188 beartype-0.9.0/beartype_test/a00_unit/a00_util/hint/a00_pep/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/hint/a00_pep/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.054188 beartype-0.9.0/beartype_test/a00_unit/a00_util/hint/a00_pep/proposal/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/hint/a00_pep/proposal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.054188 beartype-0.9.0/beartype_test/a00_unit/a00_util/hint/a00_pep/proposal/pep484/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/hint/a00_pep/proposal/pep484/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2299 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/hint/a00_pep/proposal/pep484/test_utilpep484typevar.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.054188 beartype-0.9.0/beartype_test/a00_unit/a00_util/hint/a00_pep/proposal/pep484585/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/hint/a00_pep/proposal/pep484585/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6115 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/hint/a00_pep/proposal/pep484585/test_utilpepgeneric.py
--rw-r--r--   0 runner    (1001) docker     (121)     5772 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/hint/a00_pep/proposal/pep484585/test_utilpepsubclass.py
--rw-r--r--   0 runner    (1001) docker     (121)     3790 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/hint/a00_pep/proposal/test_utilpep586.py
--rw-r--r--   0 runner    (1001) docker     (121)     2697 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/hint/a00_pep/proposal/test_utilpep593.py
--rw-r--r--   0 runner    (1001) docker     (121)     7420 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/hint/a00_pep/test_a00_utilpepget.py
--rw-r--r--   0 runner    (1001) docker     (121)    11346 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/hint/a00_pep/test_a90_utilpeptest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.054188 beartype-0.9.0/beartype_test/a00_unit/a00_util/hint/a10_nonpep/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/hint/a10_nonpep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3907 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/hint/a10_nonpep/test_utilhintnonpeptest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.058188 beartype-0.9.0/beartype_test/a00_unit/a00_util/hint/a90_core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/hint/a90_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4511 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/hint/a90_core/test_a00_utilhinttest.py
--rw-r--r--   0 runner    (1001) docker     (121)     9029 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/hint/a90_core/test_a50_utilhintconv.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.058188 beartype-0.9.0/beartype_test/a00_unit/a00_util/kind/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/kind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10257 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/kind/test_utilkinddict.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.058188 beartype-0.9.0/beartype_test/a00_unit/a00_util/mod/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/mod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4530 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/mod/test_utilmoddeprecate.py
--rw-r--r--   0 runner    (1001) docker     (121)     8898 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/mod/test_utilmodimport.py
--rw-r--r--   0 runner    (1001) docker     (121)     3270 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/mod/test_utilmodtest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.058188 beartype-0.9.0/beartype_test/a00_unit/a00_util/os/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/os/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1107 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/os/test_utilostest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.058188 beartype-0.9.0/beartype_test/a00_unit/a00_util/py/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1125 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/py/test_utilpyinterpreter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1099 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/py/test_utilpyword.py
--rw-r--r--   0 runner    (1001) docker     (121)     2736 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/test_utilobject.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.058188 beartype-0.9.0/beartype_test/a00_unit/a00_util/text/
--rw-r--r--   0 runner    (1001) docker     (121)     1777 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/text/test_utiltextident.py
--rw-r--r--   0 runner    (1001) docker     (121)     4267 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/text/test_utiltextjoin.py
--rw-r--r--   0 runner    (1001) docker     (121)     2331 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/text/test_utiltextlabel.py
--rw-r--r--   0 runner    (1001) docker     (121)     4421 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/text/test_utiltextmunge.py
--rw-r--r--   0 runner    (1001) docker     (121)     2774 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a00_util/text/test_utiltextrepr.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.062188 beartype-0.9.0/beartype_test/a00_unit/a10_pep/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a10_pep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9470 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a10_pep/test_pep484.py
--rw-r--r--   0 runner    (1001) docker     (121)    10175 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a10_pep/test_pep484585.py
--rw-r--r--   0 runner    (1001) docker     (121)     8375 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a10_pep/test_pep544.py
--rw-r--r--   0 runner    (1001) docker     (121)     2628 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a10_pep/test_pep561.py
--rw-r--r--   0 runner    (1001) docker     (121)    14405 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a10_pep/test_pep563.py
--rw-r--r--   0 runner    (1001) docker     (121)     3562 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a10_pep/test_pep585.py
--rw-r--r--   0 runner    (1001) docker     (121)     3546 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a10_pep/test_pep589.py
--rw-r--r--   0 runner    (1001) docker     (121)     4811 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a10_pep/test_pep593.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.062188 beartype-0.9.0/beartype_test/a00_unit/a20_api/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a20_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2947 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a20_api/test_api_beartype.py
--rw-r--r--   0 runner    (1001) docker     (121)    27757 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a20_api/test_api_cave.py
--rw-r--r--   0 runner    (1001) docker     (121)     2148 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a20_api/test_api_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.062188 beartype-0.9.0/beartype_test/a00_unit/a20_api/vale/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a20_api/vale/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.062188 beartype-0.9.0/beartype_test/a00_unit/a20_api/vale/_factory/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a20_api/vale/_factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8233 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a20_api/vale/_factory/test_valeis.py
--rw-r--r--   0 runner    (1001) docker     (121)     6163 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a20_api/vale/_factory/test_valeiscls.py
--rw-r--r--   0 runner    (1001) docker     (121)     9706 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a20_api/vale/_factory/test_valeisobj.py
--rw-r--r--   0 runner    (1001) docker     (121)     4245 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a20_api/vale/_factory/test_valeisoper.py
--rw-r--r--   0 runner    (1001) docker     (121)     6910 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a20_api/vale/test_valevale.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.062188 beartype-0.9.0/beartype_test/a00_unit/a50_error/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a50_error/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4908 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a50_error/test_errormain.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.062188 beartype-0.9.0/beartype_test/a00_unit/a90_decor/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a90_decor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.062188 beartype-0.9.0/beartype_test/a00_unit/a90_decor/cache/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a90_decor/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4854 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a90_decor/cache/test_cachetype.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.062188 beartype-0.9.0/beartype_test/a00_unit/a90_decor/code/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a90_decor/code/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.066188 beartype-0.9.0/beartype_test/a00_unit/a90_decor/code/nonpep/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a90_decor/code/nonpep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5699 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a90_decor/code/nonpep/test_codemypy.py
--rw-r--r--   0 runner    (1001) docker     (121)     8114 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a90_decor/code/nonpep/test_codenonpep.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.066188 beartype-0.9.0/beartype_test/a00_unit/a90_decor/code/pep/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a90_decor/code/pep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5232 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a90_decor/code/pep/test_codepep.py
--rw-r--r--   0 runner    (1001) docker     (121)    15243 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a90_decor/code/pep/test_pepscope.py
--rw-r--r--   0 runner    (1001) docker     (121)    11406 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a90_decor/code/test_codeforwardref.py
--rw-r--r--   0 runner    (1001) docker     (121)    11342 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a90_decor/code/test_codemain.py
--rw-r--r--   0 runner    (1001) docker     (121)     7587 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a90_decor/code/test_codenoop.py
--rw-r--r--   0 runner    (1001) docker     (121)     5867 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a90_decor/test_decor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1173 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/a90_decor/test_decordata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.066188 beartype-0.9.0/beartype_test/a00_unit/data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11752 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/data/data_type.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.066188 beartype-0.9.0/beartype_test/a00_unit/data/hint/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/data/hint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6276 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/data/hint/data_hint.py
--rw-r--r--   0 runner    (1001) docker     (121)     6169 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/data/hint/data_hintref.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.066188 beartype-0.9.0/beartype_test/a00_unit/data/hint/nonpep/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/data/hint/nonpep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2567 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/data/hint/nonpep/data_nonpep.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.066188 beartype-0.9.0/beartype_test/a00_unit/data/hint/nonpep/mod/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/data/hint/nonpep/mod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9219 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/data/hint/nonpep/mod/_data_nonpepbeartype.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.066188 beartype-0.9.0/beartype_test/a00_unit/data/hint/nonpep/proposal/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/data/hint/nonpep/proposal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3424 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/data/hint/nonpep/proposal/_data_nonpep484.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.066188 beartype-0.9.0/beartype_test/a00_unit/data/hint/pep/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/data/hint/pep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5762 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/data/hint/pep/data_pep.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.066188 beartype-0.9.0/beartype_test/a00_unit/data/hint/pep/mod/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/data/hint/pep/mod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9799 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/data/hint/pep/mod/_data_hintmodnumpy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.066188 beartype-0.9.0/beartype_test/a00_unit/data/hint/pep/proposal/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/data/hint/pep/proposal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14939 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/data/hint/pep/proposal/_data_pep544.py
--rw-r--r--   0 runner    (1001) docker     (121)    46163 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/data/hint/pep/proposal/_data_pep585.py
--rw-r--r--   0 runner    (1001) docker     (121)    16562 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/data/hint/pep/proposal/_data_pep586.py
--rw-r--r--   0 runner    (1001) docker     (121)    14410 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/data/hint/pep/proposal/_data_pep589.py
--rw-r--r--   0 runner    (1001) docker     (121)    20690 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/data/hint/pep/proposal/_data_pep593.py
--rw-r--r--   0 runner    (1001) docker     (121)    76780 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/data/hint/pep/proposal/data_pep484.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.070188 beartype-0.9.0/beartype_test/a00_unit/data/hint/util/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/data/hint/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19343 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/data/hint/util/data_hintmetacls.py
--rw-r--r--   0 runner    (1001) docker     (121)     4960 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/data/hint/util/data_hintmetatyping.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.070188 beartype-0.9.0/beartype_test/a00_unit/data/pep/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/data/pep/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.070188 beartype-0.9.0/beartype_test/a00_unit/data/pep/pep563/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/data/pep/pep563/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4415 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/data/pep/pep563/data_pep563_club.py
--rw-r--r--   0 runner    (1001) docker     (121)    21697 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/data/pep/pep563/data_pep563_poem.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.070188 beartype-0.9.0/beartype_test/a00_unit/data/util/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/data/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.070188 beartype-0.9.0/beartype_test/a00_unit/data/util/func/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/data/util/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2076 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/data/util/func/data_utilfunccode.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.070188 beartype-0.9.0/beartype_test/a00_unit/data/util/mod/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/data/util/mod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      631 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/data/util/mod/data_utilmodule_bad.py
--rw-r--r--   0 runner    (1001) docker     (121)     1118 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a00_unit/data/util/mod/data_utilmodule_good.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.070188 beartype-0.9.0/beartype_test/a90_func/
--rw-r--r--   0 runner    (1001) docker     (121)      477 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a90_func/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a90_func/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.070188 beartype-0.9.0/beartype_test/a90_func/doc/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a90_func/doc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4261 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a90_func/doc/test_docreadme.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.070188 beartype-0.9.0/beartype_test/a90_func/pep/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a90_func/pep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6063 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/a90_func/pep/test_pep561_static.py
--rw-r--r--   0 runner    (1001) docker     (121)     7555 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.070188 beartype-0.9.0/beartype_test/util/
--rw-r--r--   0 runner    (1001) docker     (121)      482 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/util/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.070188 beartype-0.9.0/beartype_test/util/fixture/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/util/fixture/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.070188 beartype-0.9.0/beartype_test/util/mark/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/util/mark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3449 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/util/mark/pytmark.py
--rw-r--r--   0 runner    (1001) docker     (121)    11861 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/util/mark/pytskip.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.074188 beartype-0.9.0/beartype_test/util/mod/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/util/mod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2989 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/util/mod/pytmodimport.py
--rw-r--r--   0 runner    (1001) docker     (121)     4157 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/util/mod/pytmodtest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.074188 beartype-0.9.0/beartype_test/util/os/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/util/os/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.074188 beartype-0.9.0/beartype_test/util/os/command/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/util/os/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1577 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/util/os/command/pytcmdexit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.074188 beartype-0.9.0/beartype_test/util/path/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/util/path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10156 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/util/path/pytpathproject.py
--rw-r--r--   0 runner    (1001) docker     (121)      896 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/util/pytcontext.py
--rw-r--r--   0 runner    (1001) docker     (121)     4073 2021-10-22 07:49:23.000000 beartype-0.9.0/beartype_test/util/pytroar.py
--rw-r--r--   0 runner    (1001) docker     (121)    14797 2021-10-22 07:49:23.000000 beartype-0.9.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.074188 beartype-0.9.0/doc/
--rw-r--r--   0 runner    (1001) docker     (121)      638 2021-10-22 07:49:23.000000 beartype-0.9.0/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)    21477 2021-10-22 07:49:23.000000 beartype-0.9.0/doc/RELEASE.rst
--rw-r--r--   0 runner    (1001) docker     (121)      799 2021-10-22 07:49:23.000000 beartype-0.9.0/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 07:49:33.074188 beartype-0.9.0/doc/source/
--rw-r--r--   0 runner    (1001) docker     (121)      227 2021-10-22 07:49:23.000000 beartype-0.9.0/doc/source/404.rst
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-10-22 07:49:23.000000 beartype-0.9.0/doc/source/changes.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8279 2021-10-22 07:49:23.000000 beartype-0.9.0/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1481 2021-10-22 07:49:23.000000 beartype-0.9.0/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      166 2021-10-22 07:49:23.000000 beartype-0.9.0/doc/source/reference.rst
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-10-22 07:49:23.000000 beartype-0.9.0/doc/source/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8036 2021-10-22 07:49:23.000000 beartype-0.9.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)      167 2021-10-22 07:49:33.078188 beartype-0.9.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)    15649 2021-10-22 07:49:23.000000 beartype-0.9.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    12746 2021-10-22 07:49:23.000000 beartype-0.9.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.996060 beartype-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)     2392 2021-11-06 06:22:24.000000 beartype-0.9.1/.mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (121)     1140 2021-11-06 06:22:24.000000 beartype-0.9.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1079 2021-11-06 06:22:24.000000 beartype-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1841 2021-11-06 06:22:24.000000 beartype-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)   239513 2021-11-06 06:22:33.996060 beartype-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)   237842 2021-11-06 06:22:24.000000 beartype-0.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.928060 beartype-0.9.1/beartype/
+-rw-r--r--   0 runner    (1001) docker     (121)     8774 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.932060 beartype-0.9.1/beartype/_cave/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_cave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6290 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_cave/_caveabc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    52121 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_cave/_cavefast.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10240 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_cave/_cavemap.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.932060 beartype-0.9.1/beartype/_data/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.932060 beartype-0.9.1/beartype/_data/cls/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_data/cls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2397 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_data/cls/datacls.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.932060 beartype-0.9.1/beartype/_data/func/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_data/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1901 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_data/func/datafunc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.932060 beartype-0.9.1/beartype/_data/hint/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_data/hint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.932060 beartype-0.9.1/beartype/_data/hint/pep/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_data/hint/pep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28064 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_data/hint/pep/datapeprepr.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.936060 beartype-0.9.1/beartype/_data/hint/pep/sign/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_data/hint/pep/sign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2717 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_data/hint/pep/sign/datapepsigncls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9525 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_data/hint/pep/sign/datapepsigns.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18896 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_data/hint/pep/sign/datapepsignset.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.936060 beartype-0.9.1/beartype/_data/mod/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_data/mod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1989 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_data/mod/datamod.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.936060 beartype-0.9.1/beartype/_decor/
+-rw-r--r--   0 runner    (1001) docker     (121)     7639 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_decor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.936060 beartype-0.9.1/beartype/_decor/_cache/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_decor/_cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16796 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_decor/_cache/cachetype.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.936060 beartype-0.9.1/beartype/_decor/_code/
+-rw-r--r--   0 runner    (1001) docker     (121)    35282 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_decor/_code/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.936060 beartype-0.9.1/beartype/_decor/_code/_pep/
+-rw-r--r--   0 runner    (1001) docker     (121)    92720 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_decor/_code/_pep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   121346 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_decor/_code/_pep/_pephint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6153 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_decor/_code/_pep/_pepmagic.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21280 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_decor/_code/_pep/_pepscope.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23177 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_decor/_code/_pep/_pepsnip.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14095 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_decor/_code/_pep/pepcode.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21062 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_decor/_code/codemain.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10889 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_decor/_code/codesnip.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13684 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_decor/_data.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.940060 beartype-0.9.1/beartype/_decor/_error/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_decor/_error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17029 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_decor/_error/_errorsleuth.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10010 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_decor/_error/_errortype.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.940060 beartype-0.9.1/beartype/_decor/_error/_pep/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_decor/_error/_pep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4720 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_decor/_error/_pep/_errorpep586.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4279 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_decor/_error/_pep/_errorpep593.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.940060 beartype-0.9.1/beartype/_decor/_error/_pep/_pep484/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_decor/_error/_pep/_pep484/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1934 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_decor/_error/_pep/_pep484/_errornoreturn.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9696 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_decor/_error/_pep/_pep484/_errorunion.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.940060 beartype-0.9.1/beartype/_decor/_error/_pep/_pep484585/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_decor/_error/_pep/_pep484585/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5751 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_decor/_error/_pep/_pep484585/_errorgeneric.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14024 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_decor/_error/_pep/_pep484585/_errorsequence.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18761 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_decor/_error/errormain.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28338 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_decor/_pep563.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13547 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_decor/main.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.940060 beartype-0.9.1/beartype/_util/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.940060 beartype-0.9.1/beartype/_util/cache/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/cache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.944060 beartype-0.9.1/beartype/_util/cache/map/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/cache/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8884 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/cache/map/utilmapbig.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8711 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/cache/map/utilmaplru.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.944060 beartype-0.9.1/beartype/_util/cache/pool/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/cache/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10391 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/cache/pool/utilcachepool.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14177 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/cache/pool/utilcachepoollistfixed.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4268 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/cache/pool/utilcachepoolobjecttyped.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16321 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/cache/utilcachecall.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10013 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/cache/utilcacheerror.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.944060 beartype-0.9.1/beartype/_util/cls/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/cls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.944060 beartype-0.9.1/beartype/_util/cls/pep/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/cls/pep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27282 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/cls/pep/utilpep3119.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8604 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/cls/utilclstest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.948060 beartype-0.9.1/beartype/_util/func/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/func/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.948060 beartype-0.9.1/beartype/_util/func/lib/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/func/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4166 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/func/lib/utilbeartypefunc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.948060 beartype-0.9.1/beartype/_util/func/pep/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/func/pep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1580 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/func/pep/utilpep484func.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20677 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/func/utilfuncarg.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32110 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/func/utilfunccode.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12617 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/func/utilfunccodeobj.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7079 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/func/utilfuncfile.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12462 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/func/utilfuncmake.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27393 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/func/utilfuncscope.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8147 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/func/utilfuncstack.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13631 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/func/utilfunctest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2132 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/func/utilfuncwrap.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.948060 beartype-0.9.1/beartype/_util/hint/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/hint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.948060 beartype-0.9.1/beartype/_util/hint/nonpep/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/hint/nonpep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23408 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/hint/nonpep/utilnonpeptest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.948060 beartype-0.9.1/beartype/_util/hint/pep/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/hint/pep/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.948060 beartype-0.9.1/beartype/_util/hint/pep/mod/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/hint/pep/mod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16171 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/hint/pep/mod/utilmodnumpy.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.952060 beartype-0.9.1/beartype/_util/hint/pep/proposal/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/hint/pep/proposal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.952060 beartype-0.9.1/beartype/_util/hint/pep/proposal/pep484/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/hint/pep/proposal/pep484/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8032 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/hint/pep/proposal/pep484/utilpep484.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21106 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/hint/pep/proposal/pep484/utilpep484generic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6487 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/hint/pep/proposal/pep484/utilpep484newtype.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4877 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/hint/pep/proposal/pep484/utilpep484ref.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5242 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/hint/pep/proposal/pep484/utilpep484typevar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1902 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/hint/pep/proposal/pep484/utilpep484union.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.952060 beartype-0.9.1/beartype/_util/hint/pep/proposal/pep484585/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/hint/pep/proposal/pep484585/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3119 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/hint/pep/proposal/pep484585/utilpep484585.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5641 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/hint/pep/proposal/pep484585/utilpep484585arg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8623 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/hint/pep/proposal/pep484585/utilpep484585func.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19726 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/hint/pep/proposal/pep484585/utilpep484585generic.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12834 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/hint/pep/proposal/pep484585/utilpep484585ref.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12540 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/hint/pep/proposal/pep484585/utilpep484585type.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18455 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/hint/pep/proposal/utilpep544.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12380 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/hint/pep/proposal/utilpep585.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9655 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/hint/pep/proposal/utilpep586.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7298 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/hint/pep/proposal/utilpep589.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11437 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/hint/pep/proposal/utilpep593.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2172 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/hint/pep/utilpepattr.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38455 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/hint/pep/utilpepget.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38662 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/hint/pep/utilpeptest.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36988 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/hint/utilhintconv.py
+-rw-r--r--   0 runner    (1001) docker     (121)      677 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/hint/utilhintget.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7208 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/hint/utilhinttest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.952060 beartype-0.9.1/beartype/_util/kind/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/kind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13988 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/kind/utilkinddict.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.956060 beartype-0.9.1/beartype/_util/mod/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/mod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.956060 beartype-0.9.1/beartype/_util/mod/lib/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/mod/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4523 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/mod/lib/utilsphinx.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7486 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/mod/utilmoddeprecate.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19437 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/mod/utilmodimport.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15861 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/mod/utilmodtest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5394 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/mod/utilmodule.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.956060 beartype-0.9.1/beartype/_util/os/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/os/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1027 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/os/utilostest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.956060 beartype-0.9.1/beartype/_util/py/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      910 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/py/utilpyinterpreter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3173 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/py/utilpyversion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2412 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/py/utilpyword.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.956060 beartype-0.9.1/beartype/_util/text/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3729 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/text/utiltextget.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3617 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/text/utiltextident.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6883 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/text/utiltextjoin.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14057 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/text/utiltextlabel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1490 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/text/utiltextmagic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5520 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/text/utiltextmunge.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11319 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/text/utiltextrepr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1674 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/text/utiltexttest.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12264 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/utilobject.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2321 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/_util/utiltyping.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.956060 beartype-0.9.1/beartype/cave/
+-rw-r--r--   0 runner    (1001) docker     (121)    17656 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/cave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11300 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/cave/_cavelib.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22496 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/meta.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.956060 beartype-0.9.1/beartype/roar/
+-rw-r--r--   0 runner    (1001) docker     (121)     7031 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/roar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31009 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/roar/_roarexc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11764 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/roar/_roarwarn.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.960060 beartype-0.9.1/beartype/vale/
+-rw-r--r--   0 runner    (1001) docker     (121)     5848 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/vale/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.960060 beartype-0.9.1/beartype/vale/_factory/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/vale/_factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14862 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/vale/_factory/_valeis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6403 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/vale/_factory/_valeisabc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10496 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/vale/_factory/_valeiscls.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18303 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/vale/_factory/_valeisobj.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12083 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/vale/_factory/_valeisoper.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.960060 beartype-0.9.1/beartype/vale/_util/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/vale/_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4249 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/vale/_util/_valeutilsnip.py
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/vale/_util/_valeutiltest.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21503 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype/vale/_valevale.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.932060 beartype-0.9.1/beartype.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)   239513 2021-11-06 06:22:33.000000 beartype-0.9.1/beartype.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    15506 2021-11-06 06:22:33.000000 beartype-0.9.1/beartype.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-06 06:22:33.000000 beartype-0.9.1/beartype.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-06 06:22:33.000000 beartype-0.9.1/beartype.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      292 2021-11-06 06:22:33.000000 beartype-0.9.1/beartype.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2021-11-06 06:22:33.000000 beartype-0.9.1/beartype.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.960060 beartype-0.9.1/beartype_test/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.960060 beartype-0.9.1/beartype_test/a00_unit/
+-rw-r--r--   0 runner    (1001) docker     (121)      489 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.960060 beartype-0.9.1/beartype_test/a00_unit/a00_util/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.960060 beartype-0.9.1/beartype_test/a00_unit/a00_util/cache/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.964060 beartype-0.9.1/beartype_test/a00_unit/a00_util/cache/map/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/cache/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2634 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/cache/map/test_utilmapbig.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5007 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/cache/map/test_utilmaplru.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.964060 beartype-0.9.1/beartype_test/a00_unit/a00_util/cache/pool/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/cache/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5703 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/cache/pool/test_utilcachepool.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8057 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/cache/pool/test_utilcachepoollistfixed.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4661 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/cache/pool/test_utilcachepoolobjecttyped.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5027 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/cache/test_utilcachecall.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4779 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/cache/test_utilcacheerror.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.964060 beartype-0.9.1/beartype_test/a00_unit/a00_util/cls/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/cls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.964060 beartype-0.9.1/beartype_test/a00_unit/a00_util/cls/pep/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/cls/pep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2854 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/cls/pep/test_utilpep3119.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3472 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/cls/test_utilclstest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.964060 beartype-0.9.1/beartype_test/a00_unit/a00_util/func/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/func/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.964060 beartype-0.9.1/beartype_test/a00_unit/a00_util/func/lib/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/func/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3127 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/func/lib/test_utilbeartypefunc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.968060 beartype-0.9.1/beartype_test/a00_unit/a00_util/func/pep/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/func/pep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1793 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/func/pep/test_utilpep484func.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6687 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/func/test_utilfuncarg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4827 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/func/test_utilfunccode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7703 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/func/test_utilfunccodeobj.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1711 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/func/test_utilfuncfile.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8451 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/func/test_utilfuncmake.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8905 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/func/test_utilfuncscope.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1154 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/func/test_utilfuncstack.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9076 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/func/test_utilfunctest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1855 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/func/test_utilfuncwrap.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.968060 beartype-0.9.1/beartype_test/a00_unit/a00_util/hint/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/hint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.968060 beartype-0.9.1/beartype_test/a00_unit/a00_util/hint/a00_pep/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/hint/a00_pep/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.968060 beartype-0.9.1/beartype_test/a00_unit/a00_util/hint/a00_pep/proposal/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/hint/a00_pep/proposal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.968060 beartype-0.9.1/beartype_test/a00_unit/a00_util/hint/a00_pep/proposal/pep484/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/hint/a00_pep/proposal/pep484/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2299 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/hint/a00_pep/proposal/pep484/test_utilpep484typevar.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.968060 beartype-0.9.1/beartype_test/a00_unit/a00_util/hint/a00_pep/proposal/pep484585/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/hint/a00_pep/proposal/pep484585/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6115 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/hint/a00_pep/proposal/pep484585/test_utilpepgeneric.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5772 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/hint/a00_pep/proposal/pep484585/test_utilpepsubclass.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3790 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/hint/a00_pep/proposal/test_utilpep586.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2697 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/hint/a00_pep/proposal/test_utilpep593.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7420 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/hint/a00_pep/test_a00_utilpepget.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11346 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/hint/a00_pep/test_a90_utilpeptest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.968060 beartype-0.9.1/beartype_test/a00_unit/a00_util/hint/a10_nonpep/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/hint/a10_nonpep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3907 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/hint/a10_nonpep/test_utilhintnonpeptest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.968060 beartype-0.9.1/beartype_test/a00_unit/a00_util/hint/a90_core/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/hint/a90_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4511 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/hint/a90_core/test_a00_utilhinttest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9029 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/hint/a90_core/test_a50_utilhintconv.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.972060 beartype-0.9.1/beartype_test/a00_unit/a00_util/kind/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/kind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10257 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/kind/test_utilkinddict.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.972060 beartype-0.9.1/beartype_test/a00_unit/a00_util/mod/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/mod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4530 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/mod/test_utilmoddeprecate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8898 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/mod/test_utilmodimport.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3270 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/mod/test_utilmodtest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.972060 beartype-0.9.1/beartype_test/a00_unit/a00_util/os/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/os/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1107 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/os/test_utilostest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.972060 beartype-0.9.1/beartype_test/a00_unit/a00_util/py/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1125 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/py/test_utilpyinterpreter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1099 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/py/test_utilpyword.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2736 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/test_utilobject.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.972060 beartype-0.9.1/beartype_test/a00_unit/a00_util/text/
+-rw-r--r--   0 runner    (1001) docker     (121)     1777 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/text/test_utiltextident.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4267 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/text/test_utiltextjoin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2331 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/text/test_utiltextlabel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4421 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/text/test_utiltextmunge.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2774 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a00_util/text/test_utiltextrepr.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.976060 beartype-0.9.1/beartype_test/a00_unit/a10_pep/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a10_pep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9470 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a10_pep/test_pep484.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15906 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a10_pep/test_pep484585.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8375 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a10_pep/test_pep544.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2625 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a10_pep/test_pep561.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14405 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a10_pep/test_pep563.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3562 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a10_pep/test_pep585.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3546 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a10_pep/test_pep589.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4811 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a10_pep/test_pep593.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.976060 beartype-0.9.1/beartype_test/a00_unit/a20_api/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a20_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2947 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a20_api/test_api_beartype.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27757 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a20_api/test_api_cave.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2148 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a20_api/test_api_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.976060 beartype-0.9.1/beartype_test/a00_unit/a20_api/vale/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a20_api/vale/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.980060 beartype-0.9.1/beartype_test/a00_unit/a20_api/vale/_factory/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a20_api/vale/_factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8233 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a20_api/vale/_factory/test_valeis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6163 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a20_api/vale/_factory/test_valeiscls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9706 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a20_api/vale/_factory/test_valeisobj.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4245 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a20_api/vale/_factory/test_valeisoper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6910 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a20_api/vale/test_valevale.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.980060 beartype-0.9.1/beartype_test/a00_unit/a50_error/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a50_error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4908 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a50_error/test_errormain.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.980060 beartype-0.9.1/beartype_test/a00_unit/a90_decor/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a90_decor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.980060 beartype-0.9.1/beartype_test/a00_unit/a90_decor/cache/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a90_decor/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4854 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a90_decor/cache/test_cachetype.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.980060 beartype-0.9.1/beartype_test/a00_unit/a90_decor/code/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a90_decor/code/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.980060 beartype-0.9.1/beartype_test/a00_unit/a90_decor/code/nonpep/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a90_decor/code/nonpep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5699 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a90_decor/code/nonpep/test_codemypy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8114 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a90_decor/code/nonpep/test_codenonpep.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.980060 beartype-0.9.1/beartype_test/a00_unit/a90_decor/code/pep/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a90_decor/code/pep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5232 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a90_decor/code/pep/test_codepep.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15243 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a90_decor/code/pep/test_pepscope.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11833 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a90_decor/code/test_codeforwardref.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11342 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a90_decor/code/test_codemain.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7587 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a90_decor/code/test_codenoop.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5867 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a90_decor/test_decor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1173 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/a90_decor/test_decordata.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.980060 beartype-0.9.1/beartype_test/a00_unit/data/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11752 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/data/data_type.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.984060 beartype-0.9.1/beartype_test/a00_unit/data/hint/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/data/hint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6276 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/data/hint/data_hint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6169 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/data/hint/data_hintref.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.984060 beartype-0.9.1/beartype_test/a00_unit/data/hint/nonpep/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/data/hint/nonpep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2567 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/data/hint/nonpep/data_nonpep.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.984060 beartype-0.9.1/beartype_test/a00_unit/data/hint/nonpep/mod/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/data/hint/nonpep/mod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3794 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/data/hint/nonpep/mod/_data_nonpepbeartype.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.984060 beartype-0.9.1/beartype_test/a00_unit/data/hint/nonpep/proposal/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/data/hint/nonpep/proposal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11267 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/data/hint/nonpep/proposal/_data_nonpep484.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.984060 beartype-0.9.1/beartype_test/a00_unit/data/hint/pep/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/data/hint/pep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5762 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/data/hint/pep/data_pep.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.984060 beartype-0.9.1/beartype_test/a00_unit/data/hint/pep/mod/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/data/hint/pep/mod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9799 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/data/hint/pep/mod/_data_hintmodnumpy.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.984060 beartype-0.9.1/beartype_test/a00_unit/data/hint/pep/proposal/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/data/hint/pep/proposal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14972 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/data/hint/pep/proposal/_data_pep544.py
+-rw-r--r--   0 runner    (1001) docker     (121)    46300 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/data/hint/pep/proposal/_data_pep585.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16562 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/data/hint/pep/proposal/_data_pep586.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14410 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/data/hint/pep/proposal/_data_pep589.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20690 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/data/hint/pep/proposal/_data_pep593.py
+-rw-r--r--   0 runner    (1001) docker     (121)    77051 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/data/hint/pep/proposal/data_pep484.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.988060 beartype-0.9.1/beartype_test/a00_unit/data/hint/util/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/data/hint/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20117 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/data/hint/util/data_hintmetacls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4960 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/data/hint/util/data_hintmetatyping.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.988060 beartype-0.9.1/beartype_test/a00_unit/data/pep/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/data/pep/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.988060 beartype-0.9.1/beartype_test/a00_unit/data/pep/pep563/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/data/pep/pep563/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4415 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/data/pep/pep563/data_pep563_club.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21697 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/data/pep/pep563/data_pep563_poem.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.988060 beartype-0.9.1/beartype_test/a00_unit/data/util/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/data/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.988060 beartype-0.9.1/beartype_test/a00_unit/data/util/func/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/data/util/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2076 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/data/util/func/data_utilfunccode.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.988060 beartype-0.9.1/beartype_test/a00_unit/data/util/mod/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/data/util/mod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      631 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/data/util/mod/data_utilmodule_bad.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1118 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a00_unit/data/util/mod/data_utilmodule_good.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.988060 beartype-0.9.1/beartype_test/a90_func/
+-rw-r--r--   0 runner    (1001) docker     (121)      477 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a90_func/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a90_func/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.988060 beartype-0.9.1/beartype_test/a90_func/data/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a90_func/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.988060 beartype-0.9.1/beartype_test/a90_func/data/lib/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a90_func/data/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.988060 beartype-0.9.1/beartype_test/a90_func/data/lib/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (121)      634 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a90_func/data/lib/sphinx/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.988060 beartype-0.9.1/beartype_test/a90_func/data/lib/sphinx/_build/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a90_func/data/lib/sphinx/_build/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.988060 beartype-0.9.1/beartype_test/a90_func/data/lib/sphinx/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a90_func/data/lib/sphinx/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.992060 beartype-0.9.1/beartype_test/a90_func/data/lib/sphinx/_templates/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a90_func/data/lib/sphinx/_templates/.gitkeep
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2161 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a90_func/data/lib/sphinx/beartype_sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2650 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a90_func/data/lib/sphinx/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      510 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a90_func/data/lib/sphinx/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.992060 beartype-0.9.1/beartype_test/a90_func/doc/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a90_func/doc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4252 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a90_func/doc/test_docreadme.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.992060 beartype-0.9.1/beartype_test/a90_func/lib/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a90_func/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5808 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a90_func/lib/test_sphinx.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.992060 beartype-0.9.1/beartype_test/a90_func/pep/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a90_func/pep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6048 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/a90_func/pep/test_pep561_static.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7555 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.992060 beartype-0.9.1/beartype_test/util/
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/util/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.992060 beartype-0.9.1/beartype_test/util/fixture/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/util/fixture/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.992060 beartype-0.9.1/beartype_test/util/mark/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/util/mark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3449 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/util/mark/pytmark.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11861 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/util/mark/pytskip.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.992060 beartype-0.9.1/beartype_test/util/mod/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/util/mod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2989 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/util/mod/pytmodimport.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4619 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/util/mod/pytmodtest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.992060 beartype-0.9.1/beartype_test/util/os/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/util/os/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.992060 beartype-0.9.1/beartype_test/util/os/command/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/util/os/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1577 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/util/os/command/pytcmdexit.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.996060 beartype-0.9.1/beartype_test/util/path/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/util/path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4970 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/util/path/pytpathlib.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3437 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/util/path/pytpathmain.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3385 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/util/path/pytpathtest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      896 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/util/pytcontext.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4073 2021-11-06 06:22:24.000000 beartype-0.9.1/beartype_test/util/pytroar.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14797 2021-11-06 06:22:24.000000 beartype-0.9.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.996060 beartype-0.9.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (121)      638 2021-11-06 06:22:24.000000 beartype-0.9.1/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)    21477 2021-11-06 06:22:24.000000 beartype-0.9.1/doc/RELEASE.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      799 2021-11-06 06:22:24.000000 beartype-0.9.1/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-06 06:22:33.996060 beartype-0.9.1/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2021-11-06 06:22:24.000000 beartype-0.9.1/doc/source/404.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-11-06 06:22:24.000000 beartype-0.9.1/doc/source/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    10077 2021-11-06 06:22:24.000000 beartype-0.9.1/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1481 2021-11-06 06:22:24.000000 beartype-0.9.1/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      166 2021-11-06 06:22:24.000000 beartype-0.9.1/doc/source/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2021-11-06 06:22:24.000000 beartype-0.9.1/doc/source/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     8036 2021-11-06 06:22:24.000000 beartype-0.9.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (121)      167 2021-11-06 06:22:33.996060 beartype-0.9.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)    15649 2021-11-06 06:22:24.000000 beartype-0.9.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14489 2021-11-06 06:22:24.000000 beartype-0.9.1/tox.ini
```

### Comparing `beartype-0.9.0/.mypy.ini` & `beartype-0.9.1/.mypy.ini`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/.readthedocs.yml` & `beartype-0.9.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/LICENSE` & `beartype-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/MANIFEST.in` & `beartype-0.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/PKG-INFO` & `beartype-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: beartype
-Version: 0.9.0
+Version: 0.9.1
 Summary: Unbearably fast runtime type checking in pure Python.
 Home-page: https://github.com/beartype/beartype
 Author: Cecil Curry, et al.
 Author-email: leycec@gmail.com
 Maintainer: Cecil Curry, et al.
 Maintainer-email: leycec@gmail.com
 License: MIT
-Download-URL: https://github.com/beartype/beartype/archive/0.9.0.tar.gz
+Download-URL: https://github.com/beartype/beartype/archive/0.9.1.tar.gz
 Project-URL: Source, https://github.com/beartype/beartype
 Project-URL: Issues, https://github.com/beartype/beartype/issues
 Project-URL: Releases, https://github.com/beartype/beartype/issues
 Keywords: type checking,type hints,PEP 484
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -25,14 +25,15 @@
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Typing :: Typed
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6.0
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: all
 Provides-Extra: dev
 Provides-Extra: doc-rtd
 Provides-Extra: test-tox
 Provides-Extra: test-tox-coverage
@@ -52,15 +53,17 @@
 
 .. # ------------------( SYNOPSIS                           )------------------
 
 =================
 |beartype-banner|
 =================
 
-|ci-badge| |rtd-badge| |codecov-badge|
+|ci-badge| |codecov-badge|
+
+.. #FIXME: Add "|rtd-badge|" back above *AFTER* resolving Sphinx build issues.
 
 .. parsed-literal::
 
    Look for the bare necessities,
      the simple bare necessities.
    Forget about your worries and your strife.
 
@@ -143,14 +146,19 @@
 Actions`_ **+** tox_ **+** pytest_ **+** Codecov_, and `permissively
 distributed <beartype license_>`__ under the `MIT license`_. Beartype has *no*
 runtime dependencies, `only one test-time dependency <pytest_>`__, and `only
 one documentation-time dependency <Sphinx_>`__. Beartype supports `all actively
 developed Python versions <Python status_>`__, `all Python package managers
 <Install_>`__, and `multiple platform-specific package managers <Install_>`__.
 
+    Beartype `powers quality assurance across the Python ecosystem <beartype
+    dependents_>`__.
+
+    |icon-graspologic| |icon-hydrazen| |icon-pycrisp| |icon-sentipy|
+
 .. # ------------------( TABLE OF CONTENTS                  )------------------
 .. # Blank line. By default, Docutils appears to only separate the subsequent
 .. # table of contents heading from the prior paragraph by less than a single
 .. # blank line, hampering this table's readability and aesthetic comeliness.
 
 |
 
@@ -755,15 +763,15 @@
 
 If you don't know `type hints <PEP 484_>`__, this is your moment to go deep on
 the hardest hammer in Python's SQA_ toolbox. Here are a few friendly primers to
 guide you on your maiden voyage through the misty archipelagos of type hinting:
 
 * `"Python Type Checking (Guide)" <RealPython_>`__, a comprehensive third-party
   introduction to the subject. Like most existing articles, this guide predates
-  `O(1)` runtime type checkers and thus discusses only static type checking.
+  ``O(1)`` runtime type checkers and thus discusses only static type checking.
   Thankfully, the underlying syntax and semantics cleanly translate to runtime
   type checking.
 * `"PEP 484 -- Type Hints" <PEP 484_>`__, the defining standard, holy grail,
   and first testament of type hinting `personally authored by Python's former
   Benevolent Dictator for Life (BDFL) himself, Guido van Rossum <Guido van
   Rossum_>`__. Since it's surprisingly approachable and covers all the core
   conceits in detail, we recommend reading at least a few sections of interest.
@@ -1081,16 +1089,16 @@
     Wherever you can, prefer type_ and typing.Type_. Sure, they're
     inflexible, but they're inflexibly standardized across type checkers.
     Everywhere else, default to ``beartype.vale.IsSubclass``.
 
     See ``help(beartype.vale.IsSubclass)`` for further details.
 
 .. [#enum_type]
-   You don't want to know the type of enum.Enum_ members. No... seriously. You
-   don't. You do? Oh, very well. It's enum.Enum_. :superscript:`mic drop`
+   You don't want to know the type of enum.Enum_ members. No... srsly. You
+   don't. You do? Very well. It's enum.Enum_. :superscript:`mic drop`
 
 Validator Syntax
 ~~~~~~~~~~~~~~~~
 
 Beartype validators support a rich domain-specific language (DSL) leveraging
 familiar Python operators. Dynamically create new validators on-the-fly from
 existing validators, fueling reuse and preserving DRY_:
@@ -1190,17 +1198,206 @@
   class first introduced with Python 3.9.0 and since backported to older Python
   versions by the `third-party "typing_extensions" package
   <typing_extensions_>`__, which beartype also transparently supports.
 
 Validator Showcase
 ~~~~~~~~~~~~~~~~~~
 
-Let's unbox beartype validators with a sleazy slo-mo click-bait YouTube video.
+Observe the disturbing (yet alluring) utility of beartype validators in action
+as they unshackle type hints from the fetters of PEP compliance. Begone,
+foulest standards!
+
+Type Hint Connectives
++++++++++++++++++++++
+
+    **Subtitle:** *From Set Theory They Shall Grow*
+
+`PEP 484`_ standardized the typing.Union_ factory `disjunctively
+<disjunction_>`__ matching any of several equally permissible type hints ala
+Python's builtin ``or`` operator or the overloaded ``|`` operator for sets.
+That's great, because set theory is the beating heart behind type theory.
+
+But that's just disjunction_. What about intersection_ (e.g., ``and``, ``&``),
+`complementation <relative set complement_>`__ (e.g., ``not``, ``~``), or any
+of the vast multitude of *other* set theoretic operations? Can we logically
+connect simple type hints validating trivial constraints into complex type
+hints validating non-trivial constraints via PEP-standardized analogues of
+unary and binary operators?
+
+**Nope.** They don't exist yet. But that's okay. You use beartype, which means
+you don't have to wait for official Python developers to get there first.
+You're already there. :superscript:`...woah`
+
+Type Hint Elision
+^^^^^^^^^^^^^^^^^
+
+Python's core type hierarchy conceals an ugly history of secretive backward
+compatibility. In this subsection, we uncover the two filthiest, flea-infested,
+backwater corners of the otherwise well-lit atrium that is the Python language
+– and how exactly you can finalize them. Both obstruct type-checking, readable
+APIs, and quality assurance in the post-Python 2.7 era.
+
+Guido doesn't want you to know. But you want to know, don't you? You are about
+to enter another dimension, a dimension not only of syntax and semantics but of
+shame. A journey into a hideous land of annotation wrangling. Next stop... *the
+Beartype Zone.* Because guess what?
+
+* **Booleans are integers.** They shouldn't be. Booleans aren't integers in
+  most high-level languages. Wait. Are you telling me booleans are
+  literally integers in Python? Surely you jest. That can't be. You can't *add*
+  booleans, can you? What would that even mean if you could? Observe and cower,
+  rigorous data engineers.
+
+  .. code-block:: python
+
+     >>> True + 3.1415
+     4.141500000000001    # <-- oh. by. god.
+     >>> isinstance(False, int)
+     True                 # <-- when nothing is true, everything is true
+
+* **Strings are infinitely recursive sequences of...** yup, it's strings. They
+  shouldn't be. Strings aren't infinitely recursive data structures in any
+  other language devised by incautious mortals – high-level or not. Wait. Are
+  you telling me strings are both indistinguishable from full-blown immutable
+  sequences containing arbitrary items *and* infinitely recurse into themselves
+  like that sickening non-Euclidean Hall of Mirrors I puked all over when I was
+  a kid? Surely you kid. That can't be. You can't infinitely index into strings
+  *and* pass and return the results to and from callables expecting either
+  ``Sequence[Any]`` or ``Sequence[str]`` type hints, can you? Witness and
+  tremble, stricter-than-thou QA evangelists.
+
+  .. code-block:: python
+
+     >>> 'yougottabekiddi—'[0][0][0][0][0][0][0][0][0][0][0][0][0][0][0]
+     'y'                 # <-- pretty sure we just broke the world
+     >>> from collections.abc import Sequence
+     >>> isinstance("Ph'nglui mglw'nafh Cthu—"[0][0][0][0][0], Sequence)
+     True                # <-- ...curse you, curse you to heck and back
+
+When we annotate a callable as accepting an ``int``, we *never* want that
+callable to also silently accept a ``bool``. Likewise, when we annotate another
+callable as accepting a ``Sequence[Any]`` or ``Sequence[str]``, we *never* want
+that callable to also silently accept a ``str``. These are sensible
+expectations – just not in Python, where madness prevails.
+
+To resolve these counter-intuitive concerns, we need the equivalent of the
+`relative set complement (or difference) <relative set complement_>`__. We now
+call this thing... **type elision!** Sounds pretty hot, right? We know.
+
+Let's first validate **non-boolean integers** with a beartype validator
+effectively declaring a new ``int - bool`` class (i.e., the subclass of all
+integers that are *not* booleans):
+
+.. code-block:: python
+
+   # Import the requisite machinery.
+   from beartype import beartype
+   from beartype.vale import Is
+   from typing import Annotated   # <--------------- if Python ≥ 3.9.0
+   #from typing_extensions import Annotated   # <--- if Python < 3.9.0
+
+   # Type hint matching any non-boolean integer. This day all errata die.
+   IntNonbool = Annotated[int, Is[
+       lambda number: not isinstance(number, bool)]]
+
+   # Type-check a list of non-boolean integers summing to a non-boolean
+   # integer. Beartype wills it. So it shall be.
+   @beartype
+   def sum_intlist(my_list: list[IntNonbool]) -> IntNonbool:
+       '''
+       I cast thee out, mangy booleans!
+
+       You plague these shores no more.
+       '''
+
+       return sum(my_list)
+
+Let's next validate **non-string sequences** with beartype validators
+effectively declaring a new ``Sequence - str`` class (i.e., the subclass of all
+sequences that are *not* strings):
+
+.. code-block:: python
+
+   # Import the requisite machinery.
+   from beartype import beartype
+   from beartype.vale import Is
+   from collections.abc import Sequence
+   from typing import Annotated   # <--------------- if Python ≥ 3.9.0
+   #from typing_extensions import Annotated   # <--- if Python < 3.9.0
+
+   # Type hint matching any non-string sequence. Your day has finally come.
+   SequenceNonstr = Annotated[Sequence, Is[
+       lambda sequence: not isinstance(sequence, str)]]
+
+   # Type hint matching any non-string sequence *WHOSE ITEMS ARE ALL STRINGS.*
+   SequenceNonstrOfStr = Annotated[Sequence[str], Is[
+       lambda sequence: not isinstance(sequence, str)]]
+
+   # Type-check a non-string sequence of arbitrary items coerced into strings
+   # and then joined on newline to a new string. (Beartype got your back, bro.)
+   @beartype
+   def join_objects(my_sequence: SequenceNonstr) -> str:
+       '''
+       Your tide of disease ends here, "str" class!
+       '''
+
+       return '\n'.join(map(str, my_sequence))  # <-- no idea how that works
+
+   # Type-check a non-string sequence whose items are all strings joined on
+   # newline to a new string. It isn't much, but it's all you ask.
+   @beartype
+   def join_strs(my_sequence: SequenceNonstrOfStr) -> str:
+       '''
+       I expectorate thee up, sequence of strings.
+       '''
+
+       return '\n'.join(my_sequence)  # <-- do *NOT* do this to a string
+
+Full-Fat O(n) Matching
+++++++++++++++++++++++
+
+Let's validate **all integers in a list of integers in O(n) time**, because
+validators mean you no longer have to accept the QA scraps we feed you:
+
+.. code-block:: python
 
-:superscript:`Just kidding! It's just real-world industrial-strength examples.`
+   # Import the requisite machinery.
+   from beartype import beartype
+   from beartype.vale import Is
+   from typing import Annotated   # <--------------- if Python ≥ 3.9.0
+   #from typing_extensions import Annotated   # <--- if Python < 3.9.0
+
+   # Type hint matching all integers in a list of integers in O(n) time. Please
+   # never do this. You now want to, don't you? Why? You know the price! Why?!?
+   IntList = Annotated[list[int], Is[lambda lst: all(
+       isinstance(item, int) for item in lst)]]
+
+   # Type-check all integers in a list of integers in O(n) time. How could you?
+   @beartype
+   def sum_intlist(my_list: IntList) -> int:
+       '''
+       The slowest possible integer summation over the passed list of integers.
+
+       There goes your whole data science pipeline. Yikes! So much cringe.
+       '''
+
+       return sum(my_list)  # oh, gods what have you done
+
+Welcome to **full-fat type-checking.** In `our disastrous roadmap to beartype
+1.0.0 <beartype 1.0.0_>`__, we reluctantly admit that we'd like to augment the
+``@beartype`` decorator with a new parameter enabling full-fat type-checking.
+But don't wait on us. Force the issue now by just doing it yourself and then
+mocking us all over Gitter! *Fight the bear, man.*
+
+There are good reasons to believe that `O(1) type-checking is preferable <What
+does beartype do?_>`__. Violating that core precept exposes your codebase to
+scalability and security concerns. But you're the Big Boss, you swear you know
+best, and (in any case) we can't stop you because we already let the unneutered
+tomcat out of his trash bin by `publishing this API into the badlands of PyPI
+<beartype PyPI_>`__.
 
 Tensor Property Matching
 ++++++++++++++++++++++++
 
 Let's validate `the same two-dimensional NumPy array of floats of arbitrary
 precision as in the lead example above <Beartype Validators_>`__ with an
 efficient declarative validator avoiding the additional stack frame imposed by
@@ -1295,57 +1492,14 @@
        '''
        Strip the suffixing character from a string that is lengthy and/or a
        quoted sentence, because your web app deserves only the best data.
        '''
 
        return text[:-1]  # this is frankly outrageous
 
-Full-Fat O(n) Matching
-++++++++++++++++++++++
-
-Let's validate **all integers in a list of integers in O(n) time**, because
-validators mean you no longer have to accept the QA scraps we feed you:
-
-.. code-block:: python
-
-   # Import the requisite machinery.
-   from beartype import beartype
-   from beartype.vale import Is
-   from typing import Annotated   # <--------------- if Python ≥ 3.9.0
-   #from typing_extensions import Annotated   # <--- if Python < 3.9.0
-
-   # Type hint matching all integers in a list of integers in O(n) time. Please
-   # never do this. You now want to, don't you? Why? You know the price! Why?!?
-   IntList = Annotated[list[int], Is[lambda lst: all(
-       isinstance(item, int) for item in lst)]]
-
-   # Type-check all integers in a list of integers in O(n) time. How could you?
-   @beartype
-   def sum_intlist(my_list: IntList) -> int:
-       '''
-       The slowest possible integer summation over the passed list of integers.
-
-       There goes your whole data science pipeline. Yikes! So much cringe.
-       '''
-
-       return sum(my_list)  # oh, gods what have you done
-
-Welcome to **full-fat type-checking.** In `our disastrous roadmap to beartype
-1.0.0 <beartype 1.0.0_>`__, we reluctantly admit that we'd like to augment the
-``@beartype`` decorator with a new parameter enabling full-fat type-checking.
-But don't wait on us. Force the issue now by just doing it yourself and then
-mocking us all over Gitter! *Fight the bear, man.*
-
-There are good reasons to believe that `O(1) type-checking is preferable <What
-does beartype do?_>`__. Violating that core precept exposes your codebase to
-scalability and security concerns. But you're the Big Boss, you swear you know
-best, and (in any case) we can't stop you because we already let the unneutered
-tomcat out of his trash bin by `publishing this API into the badlands of PyPI
-<beartype PyPI_>`__.
-
 Validator Alternatives
 ~~~~~~~~~~~~~~~~~~~~~~
 
 If the unbridled power of beartype validators leaves you variously queasy,
 uneasy, and suspicious of our core worldview, beartype also supports
 third-party type hints like `typed NumPy arrays <NumPy Type Hints_>`__.
 
@@ -2242,14 +2396,16 @@
 +--------------------+-----------------------------------------+-------------------------------+---------------------------+
 |                    | `612 <PEP 612_>`__                      | *none*                        | *none*                    |
 +--------------------+-----------------------------------------+-------------------------------+---------------------------+
 |                    | `647 <PEP 647_>`__                      | *none*                        | *none*                    |
 +--------------------+-----------------------------------------+-------------------------------+---------------------------+
 |                    | `3119 <PEP 3119_>`__                    | **0.7.0**\ —\ *current*       | **0.9.0**\ —\ *current*   |
 +--------------------+-----------------------------------------+-------------------------------+---------------------------+
+|                    | `3141 <PEP 3141_>`__                    | **0.1.0**\ —\ *current*       | **0.1.0**\ —\ *current*   |
++--------------------+-----------------------------------------+-------------------------------+---------------------------+
 | packages           | `PyPI <beartype PyPI_>`__               | **0.1.0**\ —\ *current*       | —                         |
 +--------------------+-----------------------------------------+-------------------------------+---------------------------+
 |                    | `Anaconda <beartype Anaconda_>`__       | **0.1.0**\ —\ *current*       | —                         |
 +--------------------+-----------------------------------------+-------------------------------+---------------------------+
 |                    | `Gentoo Linux <beartype Gentoo_>`__     | **0.2.0**\ —\ *current*       | —                         |
 +--------------------+-----------------------------------------+-------------------------------+---------------------------+
 |                    | `macOS Homebrew <beartype Homebrew_>`__ | **0.5.1**\ —\ *current*       | —                         |
@@ -2264,14 +2420,16 @@
 +--------------------+-----------------------------------------+-------------------------------+---------------------------+
 |                    | 3.8                                     | **0.1.0**\ —\ *current*       | —                         |
 +--------------------+-----------------------------------------+-------------------------------+---------------------------+
 |                    | 3.9                                     | **0.3.2**\ —\ *current*       | —                         |
 +--------------------+-----------------------------------------+-------------------------------+---------------------------+
 |                    | 3.10                                    | **0.7.0**\ —\ *current*       | —                         |
 +--------------------+-----------------------------------------+-------------------------------+---------------------------+
+|                    | 3.11                                    | *none*                        | *none*                    |
++--------------------+-----------------------------------------+-------------------------------+---------------------------+
 
 Timings
 =======
 
 Let's profile ``beartype`` against other runtime type-checkers with `a battery
 of surely fair, impartial, and unbiased use cases <beartype profiler_>`__:
 
@@ -2585,14 +2743,15 @@
 * `PEP 572 -- Assignment Expressions <PEP 572_>`__.
 * `PEP 585 -- Type Hinting Generics In Standard Collections <PEP 585_>`__.
 * `PEP 586 -- Literal Types <PEP 586_>`__.
 * `PEP 589 -- TypedDict: Type Hints for Dictionaries with a Fixed Set of Keys
   <PEP 589_>`__, subject to `caveats detailed below <Partial Compliance_>`__
 * `PEP 593 -- Flexible function and variable annotations <PEP 593_>`__.
 * `PEP 604 -- Allow writing union types as X | Y <PEP 604_>`__.
+* `PEP 3141 -- A Type Hierarchy for Numbers <PEP 3141_>`__.
 
 Beartype is currently *not* compliant whatsoever with these PEPs:
 
 * `PEP 526 -- Syntax for Variable Annotations <PEP 526_>`__.
 * `PEP 591 -- Adding a final qualifier to typing <PEP 591_>`__.
 * `PEP 612 -- Parameter Specification Variables <PEP 612_>`__.
 
@@ -4105,14 +4264,28 @@
 .. |codecov-badge| image:: https://codecov.io/gh/beartype/beartype/branch/main/graph/badge.svg?token=E6F4YSY9ZQ
    :target: https://codecov.io/gh/beartype/beartype
    :alt: beartype test coverage status
 .. |rtd-badge| image:: https://readthedocs.org/projects/beartype/badge/?version=latest
    :target: https://beartype.readthedocs.io/en/latest/?badge=latest
    :alt: beartype Read The Docs (RTD) status
 
+.. # ------------------( IMAGES ~ downstream                )------------------
+.. |icon-graspologic| image:: https://user-images.githubusercontent.com/217028/138580730-dcb3ee22-6372-4a2d-93bf-d1a3c97e67cf.png
+   :target: https://github.com/microsoft/graspologic
+   :alt: Graspologic: Python package for graph statistical algorithms
+.. |icon-hydrazen| image:: https://user-images.githubusercontent.com/217028/139522423-d987d484-425b-4e70-a0e7-7390593471f1.png
+   :target: https://github.com/mit-ll-responsible-ai/hydra-zen
+   :alt: Hydra-Zen: Reproducible Pythonic CLI<->config APIs via Hydra
+.. |icon-pycrisp| image:: https://user-images.githubusercontent.com/217028/138580797-1f09f0b4-bced-4651-82c9-6dae50afe883.png
+   :target: https://gitlab.com/pycrisp/pycrisp
+   :alt: PyCrisp: Typed Python interactions with the Crisp API
+.. |icon-sentipy| image:: https://user-images.githubusercontent.com/217028/138581059-6e3218d0-2a2e-42b7-b15c-7e2759fa2399.png
+   :target: https://github.com/sentimentinvestor/sentipy
+   :alt: SentiPy: Typed Python interactions with the Sentiment Investor API
+
 .. # ------------------( LINKS ~ beartype : funding         )------------------
 .. _BETSE:
    https://gitlab.com/betse/betse
 .. _BETSEE:
    https://gitlab.com/betse/betsee
 .. _Paul Allen:
    https://en.wikipedia.org/wiki/Paul_Allen
@@ -4263,14 +4436,26 @@
    https://en.wikipedia.org/wiki/Shere_Khan
 
 .. # ------------------( LINKS ~ math                       )------------------
 .. _Euler–Mascheroni constant:
    https://en.wikipedia.org/wiki/Euler%E2%80%93Mascheroni_constant
 .. _coupon collector's problem:
    https://en.wikipedia.org/wiki/Coupon_collector%27s_problem
+
+.. # ------------------( LINKS ~ math : set                 )------------------
+.. _conjunction:
+   https://en.wikipedia.org/wiki/Logical_conjunction
+.. _disjunction:
+   https://en.wikipedia.org/wiki/Logical_disjunction
+.. _intersection:
+   https://en.wikipedia.org/wiki/Intersection_(set_theory)
+.. _relative set complement:
+   https://en.wikipedia.org/wiki/Complement_(set_theory)#Relative_complement
+
+.. # ------------------( LINKS ~ math : type                )------------------
 .. _covariance:
    https://en.wikipedia.org/wiki/Covariance_and_contravariance_(computer_science)
 
 .. # ------------------( LINKS ~ meme                       )------------------
 .. _RNGesus:
    https://knowyourmeme.com/memes/rngesus
 .. _goes up to eleven:
```

### Comparing `beartype-0.9.0/README.rst` & `beartype-0.9.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 
 .. # ------------------( SYNOPSIS                           )------------------
 
 =================
 |beartype-banner|
 =================
 
-|ci-badge| |rtd-badge| |codecov-badge|
+|ci-badge| |codecov-badge|
+
+.. #FIXME: Add "|rtd-badge|" back above *AFTER* resolving Sphinx build issues.
 
 .. parsed-literal::
 
    Look for the bare necessities,
      the simple bare necessities.
    Forget about your worries and your strife.
 
@@ -103,14 +105,19 @@
 Actions`_ **+** tox_ **+** pytest_ **+** Codecov_, and `permissively
 distributed <beartype license_>`__ under the `MIT license`_. Beartype has *no*
 runtime dependencies, `only one test-time dependency <pytest_>`__, and `only
 one documentation-time dependency <Sphinx_>`__. Beartype supports `all actively
 developed Python versions <Python status_>`__, `all Python package managers
 <Install_>`__, and `multiple platform-specific package managers <Install_>`__.
 
+    Beartype `powers quality assurance across the Python ecosystem <beartype
+    dependents_>`__.
+
+    |icon-graspologic| |icon-hydrazen| |icon-pycrisp| |icon-sentipy|
+
 .. # ------------------( TABLE OF CONTENTS                  )------------------
 .. # Blank line. By default, Docutils appears to only separate the subsequent
 .. # table of contents heading from the prior paragraph by less than a single
 .. # blank line, hampering this table's readability and aesthetic comeliness.
 
 |
 
@@ -715,15 +722,15 @@
 
 If you don't know `type hints <PEP 484_>`__, this is your moment to go deep on
 the hardest hammer in Python's SQA_ toolbox. Here are a few friendly primers to
 guide you on your maiden voyage through the misty archipelagos of type hinting:
 
 * `"Python Type Checking (Guide)" <RealPython_>`__, a comprehensive third-party
   introduction to the subject. Like most existing articles, this guide predates
-  `O(1)` runtime type checkers and thus discusses only static type checking.
+  ``O(1)`` runtime type checkers and thus discusses only static type checking.
   Thankfully, the underlying syntax and semantics cleanly translate to runtime
   type checking.
 * `"PEP 484 -- Type Hints" <PEP 484_>`__, the defining standard, holy grail,
   and first testament of type hinting `personally authored by Python's former
   Benevolent Dictator for Life (BDFL) himself, Guido van Rossum <Guido van
   Rossum_>`__. Since it's surprisingly approachable and covers all the core
   conceits in detail, we recommend reading at least a few sections of interest.
@@ -1041,16 +1048,16 @@
     Wherever you can, prefer type_ and typing.Type_. Sure, they're
     inflexible, but they're inflexibly standardized across type checkers.
     Everywhere else, default to ``beartype.vale.IsSubclass``.
 
     See ``help(beartype.vale.IsSubclass)`` for further details.
 
 .. [#enum_type]
-   You don't want to know the type of enum.Enum_ members. No... seriously. You
-   don't. You do? Oh, very well. It's enum.Enum_. :superscript:`mic drop`
+   You don't want to know the type of enum.Enum_ members. No... srsly. You
+   don't. You do? Very well. It's enum.Enum_. :superscript:`mic drop`
 
 Validator Syntax
 ~~~~~~~~~~~~~~~~
 
 Beartype validators support a rich domain-specific language (DSL) leveraging
 familiar Python operators. Dynamically create new validators on-the-fly from
 existing validators, fueling reuse and preserving DRY_:
@@ -1150,17 +1157,206 @@
   class first introduced with Python 3.9.0 and since backported to older Python
   versions by the `third-party "typing_extensions" package
   <typing_extensions_>`__, which beartype also transparently supports.
 
 Validator Showcase
 ~~~~~~~~~~~~~~~~~~
 
-Let's unbox beartype validators with a sleazy slo-mo click-bait YouTube video.
+Observe the disturbing (yet alluring) utility of beartype validators in action
+as they unshackle type hints from the fetters of PEP compliance. Begone,
+foulest standards!
+
+Type Hint Connectives
++++++++++++++++++++++
+
+    **Subtitle:** *From Set Theory They Shall Grow*
+
+`PEP 484`_ standardized the typing.Union_ factory `disjunctively
+<disjunction_>`__ matching any of several equally permissible type hints ala
+Python's builtin ``or`` operator or the overloaded ``|`` operator for sets.
+That's great, because set theory is the beating heart behind type theory.
+
+But that's just disjunction_. What about intersection_ (e.g., ``and``, ``&``),
+`complementation <relative set complement_>`__ (e.g., ``not``, ``~``), or any
+of the vast multitude of *other* set theoretic operations? Can we logically
+connect simple type hints validating trivial constraints into complex type
+hints validating non-trivial constraints via PEP-standardized analogues of
+unary and binary operators?
+
+**Nope.** They don't exist yet. But that's okay. You use beartype, which means
+you don't have to wait for official Python developers to get there first.
+You're already there. :superscript:`...woah`
+
+Type Hint Elision
+^^^^^^^^^^^^^^^^^
+
+Python's core type hierarchy conceals an ugly history of secretive backward
+compatibility. In this subsection, we uncover the two filthiest, flea-infested,
+backwater corners of the otherwise well-lit atrium that is the Python language
+– and how exactly you can finalize them. Both obstruct type-checking, readable
+APIs, and quality assurance in the post-Python 2.7 era.
+
+Guido doesn't want you to know. But you want to know, don't you? You are about
+to enter another dimension, a dimension not only of syntax and semantics but of
+shame. A journey into a hideous land of annotation wrangling. Next stop... *the
+Beartype Zone.* Because guess what?
+
+* **Booleans are integers.** They shouldn't be. Booleans aren't integers in
+  most high-level languages. Wait. Are you telling me booleans are
+  literally integers in Python? Surely you jest. That can't be. You can't *add*
+  booleans, can you? What would that even mean if you could? Observe and cower,
+  rigorous data engineers.
+
+  .. code-block:: python
+
+     >>> True + 3.1415
+     4.141500000000001    # <-- oh. by. god.
+     >>> isinstance(False, int)
+     True                 # <-- when nothing is true, everything is true
+
+* **Strings are infinitely recursive sequences of...** yup, it's strings. They
+  shouldn't be. Strings aren't infinitely recursive data structures in any
+  other language devised by incautious mortals – high-level or not. Wait. Are
+  you telling me strings are both indistinguishable from full-blown immutable
+  sequences containing arbitrary items *and* infinitely recurse into themselves
+  like that sickening non-Euclidean Hall of Mirrors I puked all over when I was
+  a kid? Surely you kid. That can't be. You can't infinitely index into strings
+  *and* pass and return the results to and from callables expecting either
+  ``Sequence[Any]`` or ``Sequence[str]`` type hints, can you? Witness and
+  tremble, stricter-than-thou QA evangelists.
+
+  .. code-block:: python
+
+     >>> 'yougottabekiddi—'[0][0][0][0][0][0][0][0][0][0][0][0][0][0][0]
+     'y'                 # <-- pretty sure we just broke the world
+     >>> from collections.abc import Sequence
+     >>> isinstance("Ph'nglui mglw'nafh Cthu—"[0][0][0][0][0], Sequence)
+     True                # <-- ...curse you, curse you to heck and back
+
+When we annotate a callable as accepting an ``int``, we *never* want that
+callable to also silently accept a ``bool``. Likewise, when we annotate another
+callable as accepting a ``Sequence[Any]`` or ``Sequence[str]``, we *never* want
+that callable to also silently accept a ``str``. These are sensible
+expectations – just not in Python, where madness prevails.
+
+To resolve these counter-intuitive concerns, we need the equivalent of the
+`relative set complement (or difference) <relative set complement_>`__. We now
+call this thing... **type elision!** Sounds pretty hot, right? We know.
+
+Let's first validate **non-boolean integers** with a beartype validator
+effectively declaring a new ``int - bool`` class (i.e., the subclass of all
+integers that are *not* booleans):
+
+.. code-block:: python
+
+   # Import the requisite machinery.
+   from beartype import beartype
+   from beartype.vale import Is
+   from typing import Annotated   # <--------------- if Python ≥ 3.9.0
+   #from typing_extensions import Annotated   # <--- if Python < 3.9.0
+
+   # Type hint matching any non-boolean integer. This day all errata die.
+   IntNonbool = Annotated[int, Is[
+       lambda number: not isinstance(number, bool)]]
+
+   # Type-check a list of non-boolean integers summing to a non-boolean
+   # integer. Beartype wills it. So it shall be.
+   @beartype
+   def sum_intlist(my_list: list[IntNonbool]) -> IntNonbool:
+       '''
+       I cast thee out, mangy booleans!
+
+       You plague these shores no more.
+       '''
+
+       return sum(my_list)
+
+Let's next validate **non-string sequences** with beartype validators
+effectively declaring a new ``Sequence - str`` class (i.e., the subclass of all
+sequences that are *not* strings):
+
+.. code-block:: python
+
+   # Import the requisite machinery.
+   from beartype import beartype
+   from beartype.vale import Is
+   from collections.abc import Sequence
+   from typing import Annotated   # <--------------- if Python ≥ 3.9.0
+   #from typing_extensions import Annotated   # <--- if Python < 3.9.0
+
+   # Type hint matching any non-string sequence. Your day has finally come.
+   SequenceNonstr = Annotated[Sequence, Is[
+       lambda sequence: not isinstance(sequence, str)]]
+
+   # Type hint matching any non-string sequence *WHOSE ITEMS ARE ALL STRINGS.*
+   SequenceNonstrOfStr = Annotated[Sequence[str], Is[
+       lambda sequence: not isinstance(sequence, str)]]
+
+   # Type-check a non-string sequence of arbitrary items coerced into strings
+   # and then joined on newline to a new string. (Beartype got your back, bro.)
+   @beartype
+   def join_objects(my_sequence: SequenceNonstr) -> str:
+       '''
+       Your tide of disease ends here, "str" class!
+       '''
+
+       return '\n'.join(map(str, my_sequence))  # <-- no idea how that works
+
+   # Type-check a non-string sequence whose items are all strings joined on
+   # newline to a new string. It isn't much, but it's all you ask.
+   @beartype
+   def join_strs(my_sequence: SequenceNonstrOfStr) -> str:
+       '''
+       I expectorate thee up, sequence of strings.
+       '''
+
+       return '\n'.join(my_sequence)  # <-- do *NOT* do this to a string
+
+Full-Fat O(n) Matching
+++++++++++++++++++++++
+
+Let's validate **all integers in a list of integers in O(n) time**, because
+validators mean you no longer have to accept the QA scraps we feed you:
+
+.. code-block:: python
 
-:superscript:`Just kidding! It's just real-world industrial-strength examples.`
+   # Import the requisite machinery.
+   from beartype import beartype
+   from beartype.vale import Is
+   from typing import Annotated   # <--------------- if Python ≥ 3.9.0
+   #from typing_extensions import Annotated   # <--- if Python < 3.9.0
+
+   # Type hint matching all integers in a list of integers in O(n) time. Please
+   # never do this. You now want to, don't you? Why? You know the price! Why?!?
+   IntList = Annotated[list[int], Is[lambda lst: all(
+       isinstance(item, int) for item in lst)]]
+
+   # Type-check all integers in a list of integers in O(n) time. How could you?
+   @beartype
+   def sum_intlist(my_list: IntList) -> int:
+       '''
+       The slowest possible integer summation over the passed list of integers.
+
+       There goes your whole data science pipeline. Yikes! So much cringe.
+       '''
+
+       return sum(my_list)  # oh, gods what have you done
+
+Welcome to **full-fat type-checking.** In `our disastrous roadmap to beartype
+1.0.0 <beartype 1.0.0_>`__, we reluctantly admit that we'd like to augment the
+``@beartype`` decorator with a new parameter enabling full-fat type-checking.
+But don't wait on us. Force the issue now by just doing it yourself and then
+mocking us all over Gitter! *Fight the bear, man.*
+
+There are good reasons to believe that `O(1) type-checking is preferable <What
+does beartype do?_>`__. Violating that core precept exposes your codebase to
+scalability and security concerns. But you're the Big Boss, you swear you know
+best, and (in any case) we can't stop you because we already let the unneutered
+tomcat out of his trash bin by `publishing this API into the badlands of PyPI
+<beartype PyPI_>`__.
 
 Tensor Property Matching
 ++++++++++++++++++++++++
 
 Let's validate `the same two-dimensional NumPy array of floats of arbitrary
 precision as in the lead example above <Beartype Validators_>`__ with an
 efficient declarative validator avoiding the additional stack frame imposed by
@@ -1255,57 +1451,14 @@
        '''
        Strip the suffixing character from a string that is lengthy and/or a
        quoted sentence, because your web app deserves only the best data.
        '''
 
        return text[:-1]  # this is frankly outrageous
 
-Full-Fat O(n) Matching
-++++++++++++++++++++++
-
-Let's validate **all integers in a list of integers in O(n) time**, because
-validators mean you no longer have to accept the QA scraps we feed you:
-
-.. code-block:: python
-
-   # Import the requisite machinery.
-   from beartype import beartype
-   from beartype.vale import Is
-   from typing import Annotated   # <--------------- if Python ≥ 3.9.0
-   #from typing_extensions import Annotated   # <--- if Python < 3.9.0
-
-   # Type hint matching all integers in a list of integers in O(n) time. Please
-   # never do this. You now want to, don't you? Why? You know the price! Why?!?
-   IntList = Annotated[list[int], Is[lambda lst: all(
-       isinstance(item, int) for item in lst)]]
-
-   # Type-check all integers in a list of integers in O(n) time. How could you?
-   @beartype
-   def sum_intlist(my_list: IntList) -> int:
-       '''
-       The slowest possible integer summation over the passed list of integers.
-
-       There goes your whole data science pipeline. Yikes! So much cringe.
-       '''
-
-       return sum(my_list)  # oh, gods what have you done
-
-Welcome to **full-fat type-checking.** In `our disastrous roadmap to beartype
-1.0.0 <beartype 1.0.0_>`__, we reluctantly admit that we'd like to augment the
-``@beartype`` decorator with a new parameter enabling full-fat type-checking.
-But don't wait on us. Force the issue now by just doing it yourself and then
-mocking us all over Gitter! *Fight the bear, man.*
-
-There are good reasons to believe that `O(1) type-checking is preferable <What
-does beartype do?_>`__. Violating that core precept exposes your codebase to
-scalability and security concerns. But you're the Big Boss, you swear you know
-best, and (in any case) we can't stop you because we already let the unneutered
-tomcat out of his trash bin by `publishing this API into the badlands of PyPI
-<beartype PyPI_>`__.
-
 Validator Alternatives
 ~~~~~~~~~~~~~~~~~~~~~~
 
 If the unbridled power of beartype validators leaves you variously queasy,
 uneasy, and suspicious of our core worldview, beartype also supports
 third-party type hints like `typed NumPy arrays <NumPy Type Hints_>`__.
 
@@ -2202,14 +2355,16 @@
 +--------------------+-----------------------------------------+-------------------------------+---------------------------+
 |                    | `612 <PEP 612_>`__                      | *none*                        | *none*                    |
 +--------------------+-----------------------------------------+-------------------------------+---------------------------+
 |                    | `647 <PEP 647_>`__                      | *none*                        | *none*                    |
 +--------------------+-----------------------------------------+-------------------------------+---------------------------+
 |                    | `3119 <PEP 3119_>`__                    | **0.7.0**\ —\ *current*       | **0.9.0**\ —\ *current*   |
 +--------------------+-----------------------------------------+-------------------------------+---------------------------+
+|                    | `3141 <PEP 3141_>`__                    | **0.1.0**\ —\ *current*       | **0.1.0**\ —\ *current*   |
++--------------------+-----------------------------------------+-------------------------------+---------------------------+
 | packages           | `PyPI <beartype PyPI_>`__               | **0.1.0**\ —\ *current*       | —                         |
 +--------------------+-----------------------------------------+-------------------------------+---------------------------+
 |                    | `Anaconda <beartype Anaconda_>`__       | **0.1.0**\ —\ *current*       | —                         |
 +--------------------+-----------------------------------------+-------------------------------+---------------------------+
 |                    | `Gentoo Linux <beartype Gentoo_>`__     | **0.2.0**\ —\ *current*       | —                         |
 +--------------------+-----------------------------------------+-------------------------------+---------------------------+
 |                    | `macOS Homebrew <beartype Homebrew_>`__ | **0.5.1**\ —\ *current*       | —                         |
@@ -2224,14 +2379,16 @@
 +--------------------+-----------------------------------------+-------------------------------+---------------------------+
 |                    | 3.8                                     | **0.1.0**\ —\ *current*       | —                         |
 +--------------------+-----------------------------------------+-------------------------------+---------------------------+
 |                    | 3.9                                     | **0.3.2**\ —\ *current*       | —                         |
 +--------------------+-----------------------------------------+-------------------------------+---------------------------+
 |                    | 3.10                                    | **0.7.0**\ —\ *current*       | —                         |
 +--------------------+-----------------------------------------+-------------------------------+---------------------------+
+|                    | 3.11                                    | *none*                        | *none*                    |
++--------------------+-----------------------------------------+-------------------------------+---------------------------+
 
 Timings
 =======
 
 Let's profile ``beartype`` against other runtime type-checkers with `a battery
 of surely fair, impartial, and unbiased use cases <beartype profiler_>`__:
 
@@ -2545,14 +2702,15 @@
 * `PEP 572 -- Assignment Expressions <PEP 572_>`__.
 * `PEP 585 -- Type Hinting Generics In Standard Collections <PEP 585_>`__.
 * `PEP 586 -- Literal Types <PEP 586_>`__.
 * `PEP 589 -- TypedDict: Type Hints for Dictionaries with a Fixed Set of Keys
   <PEP 589_>`__, subject to `caveats detailed below <Partial Compliance_>`__
 * `PEP 593 -- Flexible function and variable annotations <PEP 593_>`__.
 * `PEP 604 -- Allow writing union types as X | Y <PEP 604_>`__.
+* `PEP 3141 -- A Type Hierarchy for Numbers <PEP 3141_>`__.
 
 Beartype is currently *not* compliant whatsoever with these PEPs:
 
 * `PEP 526 -- Syntax for Variable Annotations <PEP 526_>`__.
 * `PEP 591 -- Adding a final qualifier to typing <PEP 591_>`__.
 * `PEP 612 -- Parameter Specification Variables <PEP 612_>`__.
 
@@ -4065,14 +4223,28 @@
 .. |codecov-badge| image:: https://codecov.io/gh/beartype/beartype/branch/main/graph/badge.svg?token=E6F4YSY9ZQ
    :target: https://codecov.io/gh/beartype/beartype
    :alt: beartype test coverage status
 .. |rtd-badge| image:: https://readthedocs.org/projects/beartype/badge/?version=latest
    :target: https://beartype.readthedocs.io/en/latest/?badge=latest
    :alt: beartype Read The Docs (RTD) status
 
+.. # ------------------( IMAGES ~ downstream                )------------------
+.. |icon-graspologic| image:: https://user-images.githubusercontent.com/217028/138580730-dcb3ee22-6372-4a2d-93bf-d1a3c97e67cf.png
+   :target: https://github.com/microsoft/graspologic
+   :alt: Graspologic: Python package for graph statistical algorithms
+.. |icon-hydrazen| image:: https://user-images.githubusercontent.com/217028/139522423-d987d484-425b-4e70-a0e7-7390593471f1.png
+   :target: https://github.com/mit-ll-responsible-ai/hydra-zen
+   :alt: Hydra-Zen: Reproducible Pythonic CLI<->config APIs via Hydra
+.. |icon-pycrisp| image:: https://user-images.githubusercontent.com/217028/138580797-1f09f0b4-bced-4651-82c9-6dae50afe883.png
+   :target: https://gitlab.com/pycrisp/pycrisp
+   :alt: PyCrisp: Typed Python interactions with the Crisp API
+.. |icon-sentipy| image:: https://user-images.githubusercontent.com/217028/138581059-6e3218d0-2a2e-42b7-b15c-7e2759fa2399.png
+   :target: https://github.com/sentimentinvestor/sentipy
+   :alt: SentiPy: Typed Python interactions with the Sentiment Investor API
+
 .. # ------------------( LINKS ~ beartype : funding         )------------------
 .. _BETSE:
    https://gitlab.com/betse/betse
 .. _BETSEE:
    https://gitlab.com/betse/betsee
 .. _Paul Allen:
    https://en.wikipedia.org/wiki/Paul_Allen
@@ -4223,14 +4395,26 @@
    https://en.wikipedia.org/wiki/Shere_Khan
 
 .. # ------------------( LINKS ~ math                       )------------------
 .. _Euler–Mascheroni constant:
    https://en.wikipedia.org/wiki/Euler%E2%80%93Mascheroni_constant
 .. _coupon collector's problem:
    https://en.wikipedia.org/wiki/Coupon_collector%27s_problem
+
+.. # ------------------( LINKS ~ math : set                 )------------------
+.. _conjunction:
+   https://en.wikipedia.org/wiki/Logical_conjunction
+.. _disjunction:
+   https://en.wikipedia.org/wiki/Logical_disjunction
+.. _intersection:
+   https://en.wikipedia.org/wiki/Intersection_(set_theory)
+.. _relative set complement:
+   https://en.wikipedia.org/wiki/Complement_(set_theory)#Relative_complement
+
+.. # ------------------( LINKS ~ math : type                )------------------
 .. _covariance:
    https://en.wikipedia.org/wiki/Covariance_and_contravariance_(computer_science)
 
 .. # ------------------( LINKS ~ meme                       )------------------
 .. _RNGesus:
    https://knowyourmeme.com/memes/rngesus
 .. _goes up to eleven:
```

### Comparing `beartype-0.9.0/beartype/__init__.py` & `beartype-0.9.1/beartype/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,32 +11,14 @@
 constants are commonly inspected (and thus expected) by external automation.
 '''
 
 # ....................{ TODO                              }....................
 #FIXME: Consider significantly expanding the above module docstring, assuming
 #Sphinx presents this module in its generated frontmatter.
 
-#FIXME: *SHALLOWLY TYPE-CHECK BOUND TYPE VARIABLES.* While deep type-checking
-#for type variables remains but a distant new hope, we *SHOULD* at least be
-#able to trivially shallowly type-check bound type variables (i.e., "TypeVar"
-#instances parametrized by the "bound=" parameter). For example:
-#    # Given this PEP 484-compliant type hint...
-#    hint = TypeVar('CallableT', bound=Callable[..., Any])
-#
-#    # ...we can meaningfully reduce this hint to this PEP 484-compliant type
-#    # hint.
-#    hint = Callable[..., Any]
-#Trivial, now that we consider it. Welp! Happily, given any arbitrary bound
-#type variable "T", runtime introspection readily yields that bound:
-#    >>> from typing import TypeVar
-#    >>> TypeVar('T', bound=str).__bound__
-#    str
-#    >>> TypeVar('T').__bound__
-#    None
-
 #FIXME: [NEW PROJECT] Consider creating a new private "beartype._bearable"
 #subpackage to enable arbitrary O(1) runtime type checking. By "arbitrary," we
 #mean just that: O(1) runtime type checking that anyone can perform in any
 #arbitrary expression without having to isolate that checking to a callable
 #signature.
 #
 #First, let's spec the public API. Fortunately, that's trivial. Just as with
```

### Comparing `beartype-0.9.0/beartype/_cave/_caveabc.py` & `beartype-0.9.1/beartype/_cave/_caveabc.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_cave/_cavefast.py` & `beartype-0.9.1/beartype/_cave/_cavefast.py`

 * *Files 1% similar despite different names*

```diff
@@ -864,48 +864,43 @@
 )
 '''
 C-based type of all subscripted generics if the active Python interpreter
 targets Python >= 3.9 *or* :class:`UnavailableType` otherwise.
 
 Subscripted generics include:
 
-* `PEP 585`_-compliant **builtin type hints** (i.e., C-based type hints
+* :pep:`585`-compliant **builtin type hints** (i.e., C-based type hints
   instantiated by subscripting either a concrete builtin container class like
   :class:`list` or :class:`tuple` *or* an abstract base class (ABC) declared by
   the :mod:`collections.abc` submodule like :class:`collections.abc.Iterable`
-  or :class:`collections.abc.Sequence`). Since *all* `PEP 585`_-compliant
+  or :class:`collections.abc.Sequence`). Since *all* :pep:`585`-compliant
   builtin type hints are classes, this C-based type is the class of those
   classes and thus effectively itself a metaclass. It's probably best not to
   think about that.
-* `PEP 484`_-compliant **subscripted generics** (i.e., user-defined classes
-  subclassing one or more `PEP 484`_-compliant type hints subsequently
+* :pep:`484`-compliant **subscripted generics** (i.e., user-defined classes
+  subclassing one or more :pep:`484`-compliant type hints subsequently
   subscripted by one or more PEP-compliant type hints).
-* `PEP 585`_-compliant **subscripted generics** (i.e., user-defined classes
-  subclassing one or more `PEP 585`_-compliant type hints subsequently
+* :pep:`585`-compliant **subscripted generics** (i.e., user-defined classes
+  subclassing one or more :pep:`585`-compliant type hints subsequently
   subscripted by one or more PEP-compliant type hints).
 
 Caveats
 ----------
 **This low-level type ambiguously matches semantically unrelated PEP-compliant
 type hints,** rendering this type all but useless for most practical purposes.
 To distinguish between the various semantic types of hints ambiguously matched
 by this type, higher-level PEP-specific functions *must* be called instead.
 These include:
 
-* :func:`beartype._util.hint.pep.proposal.pep484.utilpep484.is_hint_pep484_generic`.
-  detecting `PEP 484`_-compliant generic type hints.
-* :func:`beartype._util.hint.pep.proposal.utilpep585.is_hint_pep585_builtin`.
-  detecting `PEP 585`_-compliant builtin type hints.
-* :func:`beartype._util.hint.pep.proposal.utilpep585.is_hint_pep585_generic`.
-  detecting `PEP 585`_-compliant generic type hints.
-
-.. _PEP 484:
-    https://www.python.org/dev/peps/pep-0484
-.. _PEP 585:
-    https://www.python.org/dev/peps/pep-0585
+* :func:`beartype._util.hint.pep.proposal.pep484.utilpep484.is_hint_pep484_generic`,
+  detecting :pep:`484`-compliant generic type hints.
+* :func:`beartype._util.hint.pep.proposal.utilpep585.is_hint_pep585_builtin`,
+  detecting :pep:`585`-compliant builtin type hints.
+* :func:`beartype._util.hint.pep.proposal.utilpep585.is_hint_pep585_generic`,
+  detecting :pep:`585`-compliant generic type hints.
 '''
 
 # ....................{ TYPES ~ scalar                    }....................
 StrType = str    # Well, isn't that special.
 '''
 Type of all **unencoded Unicode strings** (i.e., instances of the builtin
 :class:`str` class; sequences of abstract Unicode codepoints that have yet to
```

### Comparing `beartype-0.9.0/beartype/_cave/_cavemap.py` & `beartype-0.9.1/beartype/_cave/_cavemap.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_data/cls/datacls.py` & `beartype-0.9.1/beartype/_data/cls/datacls.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_data/func/datafunc.py` & `beartype-0.9.1/beartype/_data/func/datafunc.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_data/hint/pep/datapeprepr.py` & `beartype-0.9.1/beartype/_data/hint/pep/datapeprepr.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_data/hint/pep/sign/datapepsigncls.py` & `beartype-0.9.1/beartype/_data/hint/pep/sign/datapepsigncls.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_data/hint/pep/sign/datapepsigns.py` & `beartype-0.9.1/beartype/_data/hint/pep/sign/datapepsigns.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_data/hint/pep/sign/datapepsignset.py` & `beartype-0.9.1/beartype/_data/hint/pep/sign/datapepsignset.py`

 * *Files 11% similar despite different names*

```diff
@@ -146,14 +146,76 @@
 ))
 '''
 Frozen set of all **bare ignorable signs** (i.e., arbitrary objects uniquely
 identifying unsubscripted type hints that are unconditionally ignorable by the
 :func:`beartype.beartype` decorator).
 '''
 
+# ....................{ SIGNS ~ return                    }....................
+HINT_SIGNS_RETURN_GENERATOR_ASYNC = frozenset((
+    # ..................{ PEP (484|585)                     }..................
+    HintSignAsyncGenerator,
+    HintSignAsyncIterable,
+    HintSignAsyncIterator,
+))
+'''
+Frozen set of all signs uniquely identifying **PEP-compliant asynchronous
+generator return type hints** (i.e., hints permissible as the return
+annotations of asynchronous generators).
+
+See Also
+----------
+:data:`HINT_SIGNS_RETURN_GENERATOR_SYNC`
+    Further discussion.
+'''
+
+
+HINT_SIGNS_RETURN_GENERATOR_SYNC = frozenset((
+    # ..................{ PEP (484|585)                     }..................
+    HintSignGenerator,
+    HintSignIterable,
+    HintSignIterator,
+))
+'''
+Frozen set of all signs uniquely identifying **PEP-compliant synchronous
+generator return type hints** (i.e., hints permissible as the return
+annotations of synchronous generators).
+
+Generator callables are simply syntactic sugar for non-generator callables
+returning generator objects. For this reason, generator callables *must* be
+annotated as returning a type compatible with generator objects -- including:
+
+* :data:`HintSignGenerator`, the narrowest abstract base class (ABC) to which
+  all generator objects necessarily conform.
+* :data:`HintSignIterator`, the immediate superclass of
+  :data:`HintSignGenerator`.
+* :data:`HintSignIterable`, the immediate superclass of
+  :data:`HintSignIterator`.
+
+Technically, :pep:`484` states that generator callables may only be annotated
+as only returning a subscription of the :attr:`typing.Generator` factory:
+
+    The return type of generator functions can be annotated by the generic type
+    ``Generator[yield_type, send_type, return_type]`` provided by ``typing.py``
+    module:
+
+Pragmatically, official documentation for the :mod:`typing` module seemingly
+*never* standardized by an existing PEP additionally states that generator
+callables may be annotated as also returning a subscription of either the
+:attr:`typing.Iterable` or :attr:`typing.Iterator` factories:
+
+    Alternatively, annotate your generator as having a return type of either
+    ``Iterable[YieldType]`` or ``Iterator[YieldType]``:
+
+See Also
+----------
+https://github.com/beartype/beartype/issues/65#issuecomment-954468111
+    Further discussion.
+'''
+
 # ....................{ SIGNS ~ type                      }....................
 HINT_SIGNS_ORIGIN_ISINSTANCEABLE = frozenset((
     # ..................{ PEP (484|585)                     }..................
     HintSignAbstractSet,
     HintSignAsyncContextManager,
     HintSignAsyncGenerator,
     HintSignAsyncIterable,
```

### Comparing `beartype-0.9.0/beartype/_data/mod/datamod.py` & `beartype-0.9.1/beartype/_data/mod/datamod.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_decor/__init__.py` & `beartype-0.9.1/beartype/_decor/__init__.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_decor/_cache/cachetype.py` & `beartype-0.9.1/beartype/_decor/_cache/cachetype.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_decor/_code/__init__.py` & `beartype-0.9.1/beartype/_decor/_code/__init__.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_decor/_code/_pep/__init__.py` & `beartype-0.9.1/beartype/_decor/_code/_pep/__init__.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_decor/_code/_pep/_pephint.py` & `beartype-0.9.1/beartype/_decor/_code/_pep/_pephint.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     ARG_NAME_GETRANDBITS,
     VAR_NAME_PREFIX_PITH,
     VAR_NAME_PITH_ROOT as PITH_ROOT_VAR_NAME,
 )
 from beartype._decor._code._pep._pepmagic import (
     EXCEPTION_PREFIX_FUNC_WRAPPER_LOCAL,
     EXCEPTION_PREFIX_HINT_ROOT,
+    EXCEPTION_PREFIX_HINT_ROOT_GENERIC,
     HINT_META_INDEX_HINT,
     HINT_META_INDEX_PLACEHOLDER,
     HINT_META_INDEX_PITH_EXPR,
     HINT_META_INDEX_PITH_VAR_NAME,
     HINT_META_INDEX_INDENT,
 )
 from beartype._decor._code._pep._pepscope import (
@@ -184,14 +185,15 @@
     _ARG_NAME_GETRANDBITS=ARG_NAME_GETRANDBITS,
     _CODE_INDENT_1=CODE_INDENT_1,
     _CODE_INDENT_2=CODE_INDENT_2,
 
     # "beartype._decor._code._pep._pepmagic" globals.
     _EXCEPTION_PREFIX_FUNC_WRAPPER_LOCAL=EXCEPTION_PREFIX_FUNC_WRAPPER_LOCAL,
     _EXCEPTION_PREFIX_HINT_ROOT=EXCEPTION_PREFIX_HINT_ROOT,
+    _EXCEPTION_PREFIX_HINT_ROOT_GENERIC=EXCEPTION_PREFIX_HINT_ROOT_GENERIC,
     _HINT_META_INDEX_HINT=HINT_META_INDEX_HINT,
     _HINT_META_INDEX_PLACEHOLDER=HINT_META_INDEX_PLACEHOLDER,
     _HINT_META_INDEX_PITH_EXPR=HINT_META_INDEX_PITH_EXPR,
     _HINT_META_INDEX_PITH_VAR_NAME=HINT_META_INDEX_PITH_VAR_NAME,
     _HINT_META_INDEX_INDENT=HINT_META_INDEX_INDENT,
     _LINE_RSTRIP_INDEX_AND=LINE_RSTRIP_INDEX_AND,
     _LINE_RSTRIP_INDEX_OR=LINE_RSTRIP_INDEX_OR,
@@ -496,32 +498,51 @@
     pith_curr_assign_expr_name_counter = 0
 
     # Python >= 3.8-specific assignment expression assigning this full Python
     # expression to the local variable assigned the value of this expression.
     pith_curr_assign_expr: str = None  # type: ignore[assignment]
 
     # ..................{ HINT ~ label                      }..................
-    # Human-readable label prefixing the machine-readable representation of the
-    # currently visited type hint if this hint is nested (i.e., any hint
-    # *except* the root type hint) in exception and warning messages.
+    # Human-readable substring prefixing the machine-readable representation of
+    # the currently visited type hint in exception and warning messages if this
+    # hint is nested (i.e., any hint *EXCEPT* the root type hint).
     #
-    # Note that "hint_curr_exception_prefix" should almost *ALWAYS* be used instead.
+    # Note that "hint_curr_exception_prefix" should typically be referenced
+    # instead.
     _EXCEPTION_PREFIX_HINT_CHILD = (
-        f'{_EXCEPTION_PREFIX_HINT_ROOT}{repr(hint_root)} nested ')
+        f'{_EXCEPTION_PREFIX_HINT_ROOT_GENERIC}{repr(hint_root)} nested ')
 
-    # Human-readable label prefixing the machine-readable representation of the
-    # currently visited type hint in exception and warning messages,
-    # initialized to the label describing the root type hint.
+    # Human-readable substring prefixing the machine-readable representation of
+    # the currently visited type hint in exception and warning messages if this
+    # hint is both nested (i.e., any hint *EXCEPT* the root type hint) *AND*
+    # being described generically (i.e., *WITHOUT* respect to the specific PEP
+    # to which this hint conforms).
     #
-    # Note that this label intentionally only describes the root and currently
-    # iterated child hints rather than the root hint, the currently iterated
-    # child hint, and all interim child hints leading from the former to the
-    # latter. The latter approach would be non-human-readable and insane.
+    # Note that "hint_curr_exception_prefix_generic" should typically be
+    # referenced instead.
+    _EXCEPTION_PREFIX_HINT_CHILD_GENERIC = (
+        f'{_EXCEPTION_PREFIX_HINT_CHILD}type hint ')
+
+    # Human-readable substring prefixing the machine-readable representation of
+    # the currently visited type hint in exception and warning messages,
+    # initialized to the string describing the root type hint.
+    #
+    # Note that this string intentionally only describes the root and currently
+    # iterated child hint rather than all of the root hint, the currently
+    # iterated child hint, and all interim child hints leading from the former
+    # to the latter. Although both feasible and less ambiguous, implementing
+    # the latter approach would be non-human-readable, complex, and insane.
     hint_curr_exception_prefix = _EXCEPTION_PREFIX_HINT_ROOT
 
+    # Human-readable substring prefixing the machine-readable representation of
+    # the currently visited type hint in exception and warning messages
+    # generically (i.e., *WITHOUT* respect to the specific PEP to which this
+    # hint conforms), initialized to the string describing the root type hint.
+    hint_curr_exception_prefix_generic = _EXCEPTION_PREFIX_HINT_ROOT_GENERIC
+
     # ..................{ METADATA                          }..................
     # Tuple of metadata describing the currently visited hint, appended by
     # the previously visited parent hint to the "hints_meta" stack.
     hint_curr_meta: tuple = None  # type: ignore[assignment]
 
     # Fixed list of all metadata describing all visitable hints currently
     # discovered by the breadth-first search (BFS) below. This list acts as a
@@ -882,15 +903,15 @@
                     # Python expression evaluating to this origin type.
                     hint_curr_expr=add_func_scope_type(
                         # Origin type of this hint if any *OR* raise an
                         # exception -- which should *NEVER* happen, as this
                         # hint was validated above to be supported.
                         cls=get_hint_pep_origin_type_isinstanceable(hint_curr),
                         func_scope=func_wrapper_locals,
-                        exception_prefix=_EXCEPTION_PREFIX_FUNC_WRAPPER_LOCAL,
+                        exception_prefix=hint_curr_exception_prefix_generic,
                     ),
                 )
             # Else, this hint is either subscripted, not shallowly
             # type-checkable, *OR* deeply type-checkable.
             #
             # ..............{ FORWARDREF                        }..............
             # If this hint is a forward reference...
@@ -908,15 +929,15 @@
                 #   preserves this local set as is.
                 hint_curr_expr, hint_forwardrefs_class_basename = (
                     express_func_scope_type_forwardref(
                         forwardref=hint_curr,
                         forwardrefs_class_basename=(
                             hint_forwardrefs_class_basename),
                         func_scope=func_wrapper_locals,
-                        exception_prefix=hint_curr_exception_prefix,
+                        exception_prefix=hint_curr_exception_prefix_generic,
                     ))
 
                 # Code type-checking the current pith against this class.
                 func_curr_code = PEP484_CODE_HINT_INSTANCE_format(
                     pith_curr_expr=pith_curr_expr,
                     hint_curr_expr=hint_curr_expr,
                 )
@@ -1178,16 +1199,16 @@
                     # * The "typing" module explicitly prohibits empty union
                     #   subscription: e.g.,
                     #       >>> typing.Union[]
                     #       SyntaxError: invalid syntax
                     #       >>> typing.Union[()]
                     #       TypeError: Cannot take a Union of no types.
                     assert hint_childs, (
-                        f'{hint_curr_exception_prefix}union type hint {repr(hint_curr)} '
-                        f'unsubscripted.')
+                        f'{hint_curr_exception_prefix}union type hint '
+                        f'{repr(hint_curr)} unsubscripted.')
                     # Else, this union is subscripted by two or more arguments.
                     # Why two rather than one? Because the "typing" module
                     # reduces unions of one argument to that argument: e.g.,
                     #     >>> import typing
                     #     >>> typing.Union[int]
                     #     int
 
@@ -1260,15 +1281,16 @@
                                 pith_curr_expr=(
                                     # If this union is subscripted by one or
                                     # more PEP-compliant child hints, prefer
                                     # the expression assigning this value to a
                                     # local variable efficiently reused by
                                     # subsequent code generated for
                                     # PEP-compliant child hints.
-                                    pith_curr_assign_expr if hint_childs_pep else
+                                    pith_curr_assign_expr
+                                    if hint_childs_pep else
                                     # Else, this union is *NOT* subscripted by
                                     # one or more PEP-compliant child hints.
                                     # Since this is the first and only test
                                     # generated for this union, prefer the
                                     # expression yielding the value of the
                                     # current pith *WITHOUT* assigning this
                                     # value to a local variable, which would
@@ -1297,15 +1319,15 @@
                                 # usual approach. See also this relevant
                                 # self-StackOverflow post:
                                 #       https://stackoverflow.com/a/40054478/2809027
                                 hint_curr_expr=add_func_scope_types(
                                     types=hint_childs_nonpep,
                                     func_scope=func_wrapper_locals,
                                     exception_prefix=(
-                                        _EXCEPTION_PREFIX_FUNC_WRAPPER_LOCAL),
+                                        hint_curr_exception_prefix_generic),
                                 ),
                             ))
 
                     # For each PEP-compliant child hint of this union, generate
                     # and append code type-checking this child hint.
                     for hint_child_index, hint_child in enumerate(
                         hint_childs_pep):
@@ -1401,15 +1423,15 @@
                 # ignorable arguments.
 
                     # Python expression evaluating to this origin type.
                     hint_curr_expr = add_func_scope_type(
                         # Origin type of this sequence.
                         cls=get_hint_pep_origin_type_isinstanceable(hint_curr),
                         func_scope=func_wrapper_locals,
-                        exception_prefix=_EXCEPTION_PREFIX_FUNC_WRAPPER_LOCAL,
+                        exception_prefix=hint_curr_exception_prefix_generic,
                     )
                     # print(f'Sequence type hint {hint_curr} origin type scoped: {hint_curr_expr}')
 
                     # If this hint is a fixed-length tuple, the parent "if"
                     # statement above has already validated the contents of
                     # this tuple. In this case, efficiently get the lone child
                     # hint of this parent hint *WITHOUT* validation.
@@ -1417,15 +1439,16 @@
                         hint_child = hint_childs[0]
                     # Else, this hint is a single-argument sequence, in which
                     # case the contents of this sequence have yet to be
                     # validated. In this case, inefficiently get the lone child
                     # hint of this parent hint *WITH* validation.
                     else:
                         hint_child = get_hint_pep484585_args_1(
-                            hint=hint_curr, exception_prefix=hint_curr_exception_prefix)
+                            hint=hint_curr,
+                            exception_prefix=hint_curr_exception_prefix)
 
                     # If this child hint is *NOT* ignorable, deeply type-check
                     # both the type of the current pith *AND* a randomly
                     # indexed item of this pith. Specifically...
                     if not is_hint_ignorable(hint_child):
                         # Record that a pseudo-random integer is now required.
                         is_var_random_int_needed = True
@@ -1677,45 +1700,43 @@
                     #* Add that detection logic to one or more
                     #  is_hint_*_ignorable() testers elsewhere.
                     #* Call is_hint_ignorable() below.
                     #* Unit test such type hints to indeed be ignorable.
 
                     # Superclass this pith is required to be a subclass of.
                     hint_child = get_hint_pep484585_subclass_superclass(
-                        hint=hint_curr, exception_prefix=hint_curr_exception_prefix)
-
-                    #FIXME: Unit test us up, please.
+                        hint=hint_curr,
+                        exception_prefix=hint_curr_exception_prefix)
 
                     # If this superclass is either a class *OR* tuple of
                     # classes...
                     if isinstance(hint_child, TestableTypes):
                         # Python expression evaluating to this superclass.
                         hint_curr_expr = add_func_scope_type_or_types(
                             type_or_types=hint_child,  # type: ignore[arg-type]
                             func_scope=func_wrapper_locals,
                             exception_prefix=(
-                                _EXCEPTION_PREFIX_FUNC_WRAPPER_LOCAL),
+                                hint_curr_exception_prefix_generic),
                         )
-
-                    #FIXME: *UNIT TEST THIS PLEASE.*
-
                     # Else, this superclass is *NOT* actually a class. By
                     # process of elimination and the validation already
                     # performed above by the
                     # get_hint_pep484585_subclass_superclass() getter, this
                     # superclass *MUST* be a forward reference to a class.
                     else:
                         # Render this forward reference accessible to the body
                         # of this wrapper function. See above for commentary.
                         hint_curr_expr, hint_forwardrefs_class_basename = (
                             express_func_scope_type_forwardref(
                                 forwardref=hint_child,
                                 forwardrefs_class_basename=(
                                     hint_forwardrefs_class_basename),
                                 func_scope=func_wrapper_locals,
+                                exception_prefix=(
+                                    hint_curr_exception_prefix_generic),
                             ))
 
                     # Code type-checking this pith against this superclass.
                     func_curr_code = PEP484585_CODE_HINT_SUBCLASS_format(
                         pith_curr_assign_expr=pith_curr_assign_expr,
                         pith_curr_var_name=pith_curr_var_name,
                         hint_curr_expr=hint_curr_expr,
@@ -1904,15 +1925,15 @@
                         indent_curr=indent_curr,
                         pith_curr_assign_expr=pith_curr_assign_expr,
                         # Python expression evaluating to this generic type.
                         hint_curr_expr=add_func_scope_type(
                             cls=hint_curr,
                             func_scope=func_wrapper_locals,
                             exception_prefix=(
-                                _EXCEPTION_PREFIX_FUNC_WRAPPER_LOCAL),
+                                hint_curr_exception_prefix_generic),
                         ),
                     )
                     # print(f'{hint_curr_exception_prefix} PEP generic {repr(hint)} handled.')
                 # Else, this hint is *NOT* a generic.
                 #
                 # ............{ LITERAL                           }............
                 # If this hint is a PEP 586-compliant type hint (i.e., the
@@ -1944,50 +1965,50 @@
 
                     # Initialize the code type-checking this pith against this
                     # hint to the substring prefixing all such code.
                     func_curr_code = PEP586_CODE_HINT_PREFIX_format(
                         pith_curr_assign_expr=pith_curr_assign_expr,
 
                         #FIXME: If "typing.Literal" is ever extended to support
-                        #substantially more types (and thus actually become
+                        #substantially more types (and thus actually becomes
                         #useful), optimize the construction of the "types" set
                         #below to instead leverage a similar
                         #"acquire_object_typed(set)" caching solution as that
                         #currently employed for unions. For now, we only shrug.
 
                         # Python expression evaluating to a tuple of the unique
                         # types of all literal objects subscripting this hint.
                         hint_child_types_expr=add_func_scope_types(
-                            types=set(
+                            # Set comprehension of all unique literal objects
+                            # subscripting this hint, implicitly discarding all
+                            # duplicate such objects.
+                            types={
                                 type(hint_child)
                                 for hint_child in hint_childs
-                            ),
+                            },
                             func_scope=func_wrapper_locals,
                             exception_prefix=(
-                                _EXCEPTION_PREFIX_FUNC_WRAPPER_LOCAL),
+                                hint_curr_exception_prefix_generic),
                         ),
                     )
 
                     # For each literal object subscripting this hint...
                     for hint_child in hint_childs:
                         # Generate and append efficient code type-checking
                         # this data validator by embedding this code as is.
-                        func_curr_code += (
-                            PEP586_CODE_HINT_LITERAL_format(
-                                pith_curr_var_name=(
-                                    pith_curr_var_name),
-                                # Python expression evaluating to this literal
-                                # object.
-                                hint_child_expr=add_func_scope_attr(
-                                    attr=hint_child,
-                                    func_scope=func_wrapper_locals,
-                                    exception_prefix=(
-                                        _EXCEPTION_PREFIX_FUNC_WRAPPER_LOCAL),
-                                ),
-                            ))
+                        func_curr_code += PEP586_CODE_HINT_LITERAL_format(
+                            pith_curr_var_name=pith_curr_var_name,
+                            # Python expression evaluating to this object.
+                            hint_child_expr=add_func_scope_attr(
+                                attr=hint_child,
+                                func_scope=func_wrapper_locals,
+                                exception_prefix=(
+                                    _EXCEPTION_PREFIX_FUNC_WRAPPER_LOCAL),
+                            ),
+                        )
 
                     # Munge this code to...
                     func_curr_code = (
                         # Strip the erroneous " or" suffix appended by the last
                         # child hint from this code.
                         f'{func_curr_code[:_LINE_RSTRIP_INDEX_OR]}'
                         # Suffix this code by the appropriate substring.
@@ -2005,15 +2026,15 @@
                         f'{hint_curr_exception_prefix}{repr(hint_curr)} unsupported but '
                         f'erroneously detected as supported.'
                     )
 
         # ................{ NON-PEP                           }................
         # Else, this hint is *NOT* PEP-compliant.
         #
-        # ................{ INSTANCES                         }................
+        # ................{ NON-PEP ~ type                    }................
         # If this hint is a non-"typing" class...
         #
         # Note that:
         # * This test is intentionally performed *AFTER* that testing whether
         #   this hint is PEP-compliant, thus guaranteeing this hint to be a
         #   PEP-noncompliant non-"typing" class rather than a PEP-compliant
         #   type hint originating from such a class. Since many hints are both
@@ -2032,33 +2053,33 @@
             # Code type-checking the current pith against this type.
             func_curr_code = PEP484_CODE_HINT_INSTANCE_format(
                 pith_curr_expr=pith_curr_expr,
                 # Python expression evaluating to this type.
                 hint_curr_expr=add_func_scope_type(
                     cls=hint_curr,
                     func_scope=func_wrapper_locals,
-                    exception_prefix=_EXCEPTION_PREFIX_FUNC_WRAPPER_LOCAL,
+                    exception_prefix=hint_curr_exception_prefix_generic,
                 ),
             )
-
+        # ................{ NON-PEP ~ bad                     }................
         # Else, this hint is neither PEP-compliant *NOR* a class. In this case,
         # raise an exception. Note that:
         # * This should *NEVER* happen, as the "typing" module goes to great
         #   lengths to validate the integrity of PEP-compliant types at
         #   declaration time.
         # * The higher-level die_unless_hint_nonpep() validator is
         #   intentionally *NOT* called here, as doing so would permit both:
         #   * PEP-noncompliant forward references, which could admittedly be
         #     disabled by passing "is_str_valid=False" to that call.
         #   * PEP-noncompliant tuple unions, which currently *CANNOT* be
         #     disabled by passing such an option to that call.
         else:
             raise BeartypeDecorHintPepException(
-                f'{hint_curr_exception_prefix}type hint {repr(hint_curr)} '
-                f'not PEP-compliant.'
+                f'{hint_curr_exception_prefix_generic}{repr(hint_curr)} '
+                f'unrecognized (i.e., neither PEP-compliant nor class).'
             )
 
         # ................{ CLEANUP                           }................
         # Inject this code into the body of this wrapper.
         func_wrapper_code = replace_str_substrs(
             text=func_wrapper_code,
             old=hint_curr_placeholder,
@@ -2070,17 +2091,19 @@
         hints_meta[hints_meta_index_curr] = None
 
         # Set the following *BEFORE* visiting the next visited hint but *AFTER*
         # performing all other logic for the currently visited hint, implying
         # these should be the last statements of this iteration:
         # * Increment the 0-based index of metadata describing the next visited
         #   hint in the "hints_meta" list.
-        # * Label prefixing the representation of the next visited hint.
+        # * Substrings prefixing the representation of the next visited hint.
         hints_meta_index_curr += 1
         hint_curr_exception_prefix = _EXCEPTION_PREFIX_HINT_CHILD
+        hint_curr_exception_prefix_generic = (
+            _EXCEPTION_PREFIX_HINT_CHILD_GENERIC)
 
     # ..................{ CLEANUP                           }..................
     # Release the fixed list of all such metadata.
     release_fixed_list(hints_meta)
 
     # If the Python code snippet to be returned remains unchanged from its
     # initial value, the breadth-first search above failed to generate code. In
@@ -2088,16 +2111,16 @@
     #
     # Note that this test is inexpensive, as the third character of the
     # "func_root_code" code snippet is guaranteed to differ from that of
     # "func_wrapper_code" code snippet if this function behaved as expected,
     # which it should have... but may not have, which is why we're testing.
     if func_wrapper_code == func_root_code:
         raise BeartypeDecorHintPepException(
-            f'{_EXCEPTION_PREFIX_HINT_ROOT}{repr(hint_root)} '
-            f'not type-checked.'
+            f'{_EXCEPTION_PREFIX_HINT_ROOT_GENERIC}{repr(hint_root)} '
+            f'unchecked.'
         )
     # Else, the breadth-first search above successfully generated code.
 
     # ..................{ CODE ~ locals                     }..................
     # PEP-compliant code snippet passing the value of the random integer
     # previously generated for the current call to the exception-handling
     # function call embedded in the "PEP_CODE_HINT_ROOT_SUFFIX" snippet,
```

### Comparing `beartype-0.9.0/beartype/_decor/_code/_pep/_pepmagic.py` & `beartype-0.9.1/beartype/_decor/_code/_pep/_pepmagic.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,21 +21,31 @@
 __all__ = ['STAR_IMPORTS_CONSIDERED_HARMFUL']
 
 # ....................{ CONSTANTS ~ exception             }....................
 EXCEPTION_PREFIX_FUNC_WRAPPER_LOCAL = (
     f'{EXCEPTION_CACHED_PLACEHOLDER} wrapper parameter ')
 '''
 Human-readable substring describing a new wrapper parameter required by the
-root hint in exception messages.
+current root type hint in exception messages.
 '''
 
 
 EXCEPTION_PREFIX_HINT_ROOT = EXCEPTION_CACHED_PLACEHOLDER
 '''
-Human-readable label describing the root hint in exception messages.
+Human-readable substring describing the current root type hint in exception
+messages.
+'''
+
+
+EXCEPTION_PREFIX_HINT_ROOT_GENERIC = (
+    f'{EXCEPTION_CACHED_PLACEHOLDER} type hint ')
+'''
+Human-readable substring describing the current root type hint generically
+(i.e., *without* respect to the specific PEP to which this hint conforms) in
+exception messages.
 '''
 
 # ....................{ CONSTANTS ~ hint : meta           }....................
 # Iterator yielding the next integer incrementation starting at 0, to be safely
 # deleted *AFTER* defining the following 0-based indices via this iterator.
 __hint_meta_index_counter = count(start=0, step=1)
```

### Comparing `beartype-0.9.0/beartype/_decor/_code/_pep/_pepscope.py` & `beartype-0.9.1/beartype/_decor/_code/_pep/_pepscope.py`

 * *Files 2% similar despite different names*

```diff
@@ -333,18 +333,19 @@
     # Else, this object is either a set or tuple.
     #
     # If this collection is empty, raise an exception.
     elif not types:
         raise BeartypeDecorHintNonpepException(f'{exception_prefix}empty.')
     # Else, this collection is non-empty.
 
-    # If any item in this collection is *NOT* a standard class, raise an
+    # If any item in this collection is *NOT* an isinstanceable class, raise an
     # exception.
     for cls in types:
-        die_unless_hint_nonpep_type(hint=cls, exception_prefix=exception_prefix)
+        die_unless_hint_nonpep_type(
+            hint=cls, exception_prefix=exception_prefix)
     # Else, all items of this collection are standard classes.
 
     # If this tuple only contains one type, register only this type.
     if len(types) == 1:
         return add_func_scope_type(
             # The first and only item of this collection, accessed as either:
             # * If this collection is a tuple, that item with fast indexing.
```

### Comparing `beartype-0.9.0/beartype/_decor/_code/_pep/_pepsnip.py` & `beartype-0.9.1/beartype/_decor/_code/_pep/_pepsnip.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_decor/_code/_pep/pepcode.py` & `beartype-0.9.1/beartype/_decor/_code/_pep/pepcode.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_decor/_code/codemain.py` & `beartype-0.9.1/beartype/_decor/_code/codemain.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_decor/_code/codesnip.py` & `beartype-0.9.1/beartype/_decor/_code/codesnip.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_decor/_data.py` & `beartype-0.9.1/beartype/_decor/_data.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_decor/_error/_errorsleuth.py` & `beartype-0.9.1/beartype/_decor/_error/_errorsleuth.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_decor/_error/_errortype.py` & `beartype-0.9.1/beartype/_decor/_error/_errortype.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_decor/_error/_pep/_errorpep586.py` & `beartype-0.9.1/beartype/_decor/_error/_pep/_errorpep586.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_decor/_error/_pep/_errorpep593.py` & `beartype-0.9.1/beartype/_decor/_error/_pep/_errorpep593.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_decor/_error/_pep/_pep484/_errornoreturn.py` & `beartype-0.9.1/beartype/_decor/_error/_pep/_pep484/_errornoreturn.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_decor/_error/_pep/_pep484/_errorunion.py` & `beartype-0.9.1/beartype/_decor/_error/_pep/_pep484/_errorunion.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_decor/_error/_pep/_pep484585/_errorgeneric.py` & `beartype-0.9.1/beartype/_decor/_error/_pep/_pep484585/_errorgeneric.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_decor/_error/_pep/_pep484585/_errorsequence.py` & `beartype-0.9.1/beartype/_decor/_error/_pep/_pep484585/_errorsequence.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,31 +17,32 @@
     get_cause_or_none_type_instance_origin)
 from beartype._data.hint.pep.sign.datapepsigns import HintSignTuple
 from beartype._data.hint.pep.sign.datapepsignset import (
     HINT_SIGNS_SEQUENCE_ARGS_1)
 from beartype._util.hint.pep.proposal.pep484585.utilpep484585 import (
     is_hint_pep484585_tuple_empty)
 from beartype._util.hint.utilhinttest import is_hint_ignorable
+from beartype._util.text.utiltextlabel import label_obj_type
 from beartype._util.text.utiltextrepr import represent_object
 from typing import Optional
 
 # See the "beartype.cave" submodule for further commentary.
 __all__ = ['STAR_IMPORTS_CONSIDERED_HARMFUL']
 
 # ....................{ GETTERS ~ sequence                }....................
 def get_cause_or_none_sequence_args_1(sleuth: CauseSleuth) -> Optional[str]:
     '''
     Human-readable string describing the failure of the passed arbitrary object
-    to satisfy the passed **PEP-compliant standard sequence type hint** (i.e.,
-    PEP-compliant type hint accepting exactly one subscripted type hint
-    argument constraining *all* items of this object, which necessarily
-    satisfies the :class:`collections.abc.Sequence` protocol with guaranteed
-    ``O(1)`` indexation across all sequence items) if this object actually
-    fails to satisfy this hint *or* ``None`` otherwise (i.e., if this object
-    satisfies this hint).
+    to satisfy the passed **PEP-compliant single-argument variadic sequence
+    type hint** (i.e., PEP-compliant type hint accepting exactly one
+    subscripted argument constraining *all* items of this object, which
+    necessarily satisfies the :class:`collections.abc.Sequence` protocol with
+    guaranteed ``O(1)`` indexation across all sequence items) if this object
+    actually fails to satisfy this hint *or* ``None`` otherwise (i.e., if this
+    object satisfies this hint).
 
     Parameters
     ----------
     sleuth : CauseSleuth
         Type-checking error cause sleuth.
     '''
     assert isinstance(sleuth, CauseSleuth), f'{repr(sleuth)} not cause sleuth.'
@@ -69,21 +70,20 @@
         _get_cause_or_none_sequence(sleuth)
     )
 
 
 def get_cause_or_none_tuple(sleuth: CauseSleuth) -> Optional[str]:
     '''
     Human-readable string describing the failure of the passed arbitrary object
-    to satisfy the passed **PEP-compliant standard sequence type hint** (i.e.,
-    PEP-compliant type hint accepting exactly one subscripted type hint
-    argument constraining *all* items of this object, which necessarily
-    satisfies the :class:`collections.abc.Sequence` protocol with guaranteed
-    ``O(1)`` indexation across all sequence items) if this object actually
-    fails to satisfy this hint *or* ``None`` otherwise (i.e., if this object
-    satisfies this hint).
+    to satisfy the passed **PEP-compliant tuple type hint** (i.e.,
+    PEP-compliant type hint accepting either zero or more subscripted arguments
+    iteratively constraining each item of this fixed-length tuple *or* exactly
+    one subscripted arguments constraining *all* items of this variadic tuple)
+    if this object actually fails to satisfy this hint *or* ``None`` otherwise
+    (i.e., if this object satisfies this hint).
 
     Parameters
     ----------
     sleuth : CauseSleuth
         Type-checking error cause sleuth.
     '''
     assert isinstance(sleuth, CauseSleuth), f'{repr(sleuth)} not cause sleuth.'
@@ -133,15 +133,15 @@
         if len(sleuth.pith) != len(sleuth.hint_childs):
             # Truncated representation of this tuple.
             pith_repr = represent_object(sleuth.pith)
 
             # Return a substring describing this failure.
             return (
                 f'tuple {pith_repr} length '
-                f'{len(sleuth.pith)} not {len(sleuth.hint_childs)}'
+                f'{len(sleuth.pith)} != {len(sleuth.hint_childs)}'
             )
         # Else, this pith and hint are of the same length.
 
         # For each enumerated item of this tuple...
         for pith_item_index, pith_item in enumerate(sleuth.pith):
             # Child hint corresponding to this tuple item. Since this pith and
             # hint are of the same length, this child hint exists.
@@ -162,33 +162,33 @@
                 pith=pith_item, hint=hint_child).get_cause_or_none()
 
             # If this item is the cause of this failure, return a substring
             # describing this failure by embedding this failure (itself
             # intended to be embedded in a longer string).
             if pith_item_cause is not None:
                 # print(f'tuple pith: {sleuth_copy.pith}\ntuple hint child: {sleuth_copy.hint}\ncause: {pith_item_cause}')
-                return f'tuple item {pith_item_index} {pith_item_cause}'
+                return f'tuple index {pith_item_index} item {pith_item_cause}'
             # Else, this item is *NOT* the cause of this failure. Silently
             # continue to the next.
 
     # Return "None", as all items of this fixed-length tuple are valid,
     # implying this pith to deeply satisfy this hint.
     return None
 
 # ....................{ GETTERS ~ private                 }....................
 def _get_cause_or_none_sequence(sleuth: CauseSleuth) -> Optional[str]:
     '''
     Human-readable string describing the failure of the passed arbitrary object
     to satisfy the passed **PEP-compliant variadic sequence type hint** (i.e.,
-    PEP-compliant type hint accepting one or more subscripted type hint
-    arguments constraining *all* items of this object, which necessarily
-    satisfies the :class:`collections.abc.Sequence` protocol with guaranteed
-    ``O(1)`` indexation across all sequence items) if this object actually
-    fails to satisfy this hint *or* ``None`` otherwise (i.e., if this object
-    satisfies this hint).
+    PEP-compliant type hint accepting one or more subscripted arguments
+    constraining *all* items of this object, which necessarily satisfies the
+    :class:`collections.abc.Sequence` protocol with guaranteed ``O(1)``
+    indexation across all sequence items) if this object actually fails to
+    satisfy this hint *or* ``None`` otherwise (i.e., if this object satisfies
+    this hint).
 
     Parameters
     ----------
     sleuth : CauseSleuth
         Type-checking error cause sleuth.
     '''
     # Assert this type hint to describe a variadic sequence. See the parent
@@ -267,16 +267,17 @@
                     pith=pith_item, hint=hint_child).get_cause_or_none()
 
                 # If this item is the cause of this failure, return a substring
                 # describing this failure by embedding this failure (itself
                 # intended to be embedded in a longer string).
                 if pith_item_cause is not None:
                     return (
-                        f'{sleuth.pith.__class__.__name__} item '
-                        f'{pith_item_index} {pith_item_cause}')
+                        f'{label_obj_type(sleuth.pith)} '
+                        f'index {pith_item_index} item {pith_item_cause}'
+                    )
                 # Else, this item is *NOT* the cause of this failure. Silently
                 # continue to the next.
         # Else, this child hint is ignorable.
     # Else, this sequence is empty, in which case all items of this sequence
     # (of which there are none) are valid. Just go with it, people.
 
     # Return "None", as all items of this sequence are valid, implying this
```

### Comparing `beartype-0.9.0/beartype/_decor/_error/errormain.py` & `beartype-0.9.1/beartype/_decor/_error/errormain.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_decor/_pep563.py` & `beartype-0.9.1/beartype/_decor/_pep563.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_decor/main.py` & `beartype-0.9.1/beartype/_decor/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,18 @@
     BeartypeDecorWrappeeException,
     BeartypeDecorWrapperException,
 )
 from beartype._decor._code.codemain import generate_code
 from beartype._decor._data import BeartypeData
 from beartype._util.cache.pool.utilcachepoolobjecttyped import (
     acquire_object_typed, release_object_typed)
+from beartype._util.func.lib.utilbeartypefunc import (
+    is_func_unbeartypeable,
+    set_func_beartyped,
+)
 from beartype._util.func.utilfuncmake import make_func
 from typing import Any, Callable, TypeVar, TYPE_CHECKING
 
 # See the "beartype.cave" submodule for further commentary.
 __all__ = ['STAR_IMPORTS_CONSIDERED_HARMFUL']
 
 # ....................{ GLOBALS                           }....................
@@ -82,26 +86,26 @@
     ----------
     BeartypeDecorHintException
         If any annotation on this callable is neither:
 
         * A **PEP-compliant type** (i.e., instance or class complying with a
           PEP supported by :mod:`beartype`), including:
 
-          * `PEP 484`_ types (i.e., instance or class declared by the stdlib
+          * :pep:`484` types (i.e., instance or class declared by the stdlib
             :mod:`typing` module).
 
         * A **PEP-noncompliant type** (i.e., instance or class complying with
           :mod:`beartype`-specific semantics rather than a PEP), including:
 
           * **Fully-qualified forward references** (i.e., strings specified as
             fully-qualified classnames).
           * **Tuple unions** (i.e., tuples containing one or more classes
             and/or forward references).
     BeartypeDecorHintPep563Exception
-        If `PEP 563`_ is active for this callable and evaluating a **postponed
+        If :pep:`563` is active for this callable and evaluating a **postponed
         annotation** (i.e., annotation whose value is a string) on this
         callable raises an exception (e.g., due to that annotation referring to
         local state no longer accessible from this deferred evaluation).
     BeartypeDecorParamNameException
         If the name of any parameter declared on this callable is prefixed by
         the reserved substring ``__beartype_``.
     BeartypeDecorWrappeeException
@@ -111,19 +115,14 @@
         * A class, which :mod:`beartype` currently fails to support.
         * A C-based callable (e.g., builtin, third-party C extension).
     BeartypeDecorWrapperException
         If this decorator erroneously generates a syntactically invalid wrapper
         function. This should *never* happen, but here we are, so this probably
         happened. Please submit an upstream issue with our issue tracker if you
         ever see this. (Thanks and abstruse apologies!)
-
-    .. _PEP 484:
-       https://www.python.org/dev/peps/pep-0484
-    .. _PEP 563:
-       https://www.python.org/dev/peps/pep-0563
     '''
 
     # Validate the type of the decorated object *BEFORE* performing any work
     # assuming this object to define attributes (e.g., "func.__name__").
     #
     # If this object is uncallable, raise an exception.
     if not callable(func):
@@ -132,27 +131,18 @@
     elif isinstance(func, type):
         raise BeartypeDecorWrappeeException(
             f'{repr(func)} unsupported, '
             f'as classes currently unsupported by @beartype.'
         )
     # Else, this object is a non-class callable. Let's do this, folks.
 
-    # If either...
-    if (
-        # This callable is unannotated *OR*...
-        not func.__annotations__ or
-        # This callable is decorated by the @typing.no_type_check decorator
-        # defining this dunder instance variable on this callable *OR*...
-        getattr(func, '__no_type_check__', False) is True or
-        # This callable is a @beartype-specific wrapper previously generated by
-        # this decorator...
-        hasattr(func, '__beartype_wrapper')
-    ):
-        # Efficiently reduce to a noop (i.e., the identity decorator) by
-        # returning this callable as is.
+    # If that callable is unbeartypeable (i.e., if this decorator should
+    # preserve that callable as is rather than wrap that callable with
+    # constant-time type-checking), silently reduce to the identity decorator.
+    if is_func_unbeartypeable(func):
         return func
 
     # Previously cached callable metadata reinitialized from this callable.
     func_data = acquire_object_typed(BeartypeData)
     func_data.reinit(func)
 
     # Generate the raw string of Python statements implementing this wrapper.
@@ -249,15 +239,15 @@
         func_wrapped=func,
         exception_cls=BeartypeDecorWrapperException,
     )
 
     # Declare this wrapper to be generated by @beartype, which tests for the
     # existence of this attribute above to avoid re-decorating callables
     # already decorated by @beartype by efficiently reducing to a noop.
-    func_wrapper.__beartype_wrapper = True  # type: ignore[attr-defined]
+    set_func_beartyped(func_wrapper)
 
     # Release this callable metadata back to its object pool.
     release_object_typed(func_data)
 
     # Return this wrapper.
     return func_wrapper  # type: ignore[return-value]
```

### Comparing `beartype-0.9.0/beartype/_util/cache/map/utilmapbig.py` & `beartype-0.9.1/beartype/_util/cache/map/utilmapbig.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/cache/map/utilmaplru.py` & `beartype-0.9.1/beartype/_util/cache/map/utilmaplru.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/cache/pool/utilcachepool.py` & `beartype-0.9.1/beartype/_util/cache/pool/utilcachepool.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/cache/pool/utilcachepoollistfixed.py` & `beartype-0.9.1/beartype/_util/cache/pool/utilcachepoollistfixed.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/cache/pool/utilcachepoolobjecttyped.py` & `beartype-0.9.1/beartype/_util/cache/pool/utilcachepoolobjecttyped.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/cache/utilcachecall.py` & `beartype-0.9.1/beartype/_util/cache/utilcachecall.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/cache/utilcacheerror.py` & `beartype-0.9.1/beartype/_util/cache/utilcacheerror.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/cls/pep/utilpep3119.py` & `beartype-0.9.1/beartype/_util/cls/pep/utilpep3119.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/cls/utilclstest.py` & `beartype-0.9.1/beartype/_util/cls/utilclstest.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/func/utilfuncarg.py` & `beartype-0.9.1/beartype/_util/func/utilfuncarg.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 )
 from enum import Enum as EnumMemberType
 from inspect import (
     CO_VARARGS,
     CO_VARKEYWORDS,
     Parameter,
 )
-from typing import Any, Generator, Tuple, Type
+from typing import Any, Iterable, Tuple, Type
 
 # See the "beartype.cave" submodule for further commentary.
 __all__ = ['STAR_IMPORTS_CONSIDERED_HARMFUL']
 
 # ....................{ VALIDATORS                        }....................
 #FIXME: Uncomment as needed.
 # def die_unless_func_argless(
@@ -369,16 +369,16 @@
     # Return the number of flexible parameters accepted by this callable.
     return func_codeobj.co_argcount
 
 # ....................{ GENERATORS                        }....................
 #FIXME: Unit test us up, please.
 #FIXME: Replace all existing usage of inspect.signature() throughout the
 #codebase with usage of this supremely fast generator instead.
-def iter_func_args(func: CallableCodeObjable) -> Generator[
-    Tuple[str, EnumMemberType, Any], None, None]:
+def iter_func_args(func: CallableCodeObjable) -> Iterable[
+    Tuple[str, EnumMemberType, Any]]:
     '''
     Generator yielding one 3-tuple ``(arg_name, arg_kind, arg_default)`` for
     each parameter accepted by the passed pure-Python callable.
 
     Specifically, this function dynamically creates and returns a new one-shot
     generator yielding for each callable parameter one 3-tuple containing:
```

### Comparing `beartype-0.9.0/beartype/_util/func/utilfunccode.py` & `beartype-0.9.1/beartype/_util/func/utilfunccode.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/func/utilfunccodeobj.py` & `beartype-0.9.1/beartype/_util/func/utilfunccodeobj.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/func/utilfuncfile.py` & `beartype-0.9.1/beartype/_util/func/utilfuncfile.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/func/utilfuncmake.py` & `beartype-0.9.1/beartype/_util/func/utilfuncmake.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/func/utilfuncscope.py` & `beartype-0.9.1/beartype/_util/func/utilfuncscope.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 
 This private submodule is *not* intended for importation by downstream callers.
 '''
 
 # ....................{ IMPORTS                           }....................
 from beartype.roar._roarexc import _BeartypeUtilCallableException
 from beartype._util.utilobject import get_object_basename_scoped
+from beartype._util.utiltyping import TypeException
 from collections.abc import Callable
 from types import CodeType
-from typing import Any, Dict, Optional, Type
+from typing import Any, Dict, Optional
 
 # See the "beartype.cave" submodule for further commentary.
 __all__ = ['STAR_IMPORTS_CONSIDERED_HARMFUL']
 
 # ....................{ HINTS                             }....................
 CallableScope = Dict[str, Any]
 '''
@@ -121,15 +122,15 @@
 # ....................{ GETTERS                           }....................
 #FIXME: Unit test us up, please.
 def get_func_globals(
     # Mandatory parameters.
     func: Callable,
 
     # Optional parameters.
-    exception_cls: Type[Exception] = _BeartypeUtilCallableException,
+    exception_cls: TypeException = _BeartypeUtilCallableException,
 ) -> CallableScope:
     '''
     **Global scope** (i.e., a dictionary mapping from the name to value of each
     globally scoped attribute declared by the module transitively declaring
     the passed pure-Python callable) for this callable.
 
     This getter transparently supports **wrapper callables** (i.e.,
@@ -143,15 +144,15 @@
     func : Callable
         Callable to be inspected.
     func_stack_frames_ignore : int, optional
         Number of frames on the call stack to be ignored (i.e., silently
         incremented past), such that the next non-ignored frame following the
         last ignored frame is the parent callable or module directly declaring
         the passed callable. Defaults to 0.
-    exception_cls : type, optional
+    exception_cls : Type[Exception], optional
         Type of exception to be raised in the event of a fatal error. Defaults
         to :class:`_BeartypeUtilCallableException`.
 
     Returns
     ----------
     Dict[str, Any]
         Global scope for this callable.
@@ -187,15 +188,15 @@
 
 def get_func_locals(
     # Mandatory parameters.
     func: Callable,
 
     # Optional parameters.
     func_stack_frames_ignore: int = 0,
-    exception_cls: Type[Exception] = _BeartypeUtilCallableException,
+    exception_cls: TypeException = _BeartypeUtilCallableException,
 ) -> CallableScope:
     '''
     **Local scope** for the passed callable.
 
     This getter returns either:
 
     * If this callable is **nested** (i.e., is a method *or* is a non-method
@@ -249,15 +250,15 @@
     func : Callable
         Callable to be inspected.
     func_stack_frames_ignore : int, optional
         Number of frames on the call stack to be ignored (i.e., silently
         incremented past), such that the next non-ignored frame following the
         last ignored frame is the parent callable or module directly declaring
         the passed callable. Defaults to 0.
-    exception_cls : type, optional
+    exception_cls : Type[Exception], optional
         Type of exception to be raised in the event of a fatal error. Defaults
         to :class:`_BeartypeUtilCallableException`.
 
     Returns
     ----------
     Dict[str, Any]
         Local scope for this callable.
@@ -274,15 +275,15 @@
     assert func_stack_frames_ignore >= 0, (
         f'{func_stack_frames_ignore} negative.')
     # print(f'\n--------- Capturing nested {func.__qualname__}() local scope...')
 
     # ..................{ IMPORTS                           }..................
     # Avoid circular import dependencies.
     from beartype._util.func.utilfunccodeobj import get_func_codeobj_or_none
-    from beartype._util.func.utilfuncstack import get_func_stack_frame
+    from beartype._util.func.utilfuncstack import iter_func_stack_frames
 
     # ..................{ NOOP                              }..................
     # Fully-qualified name of the module declaring the passed callable if that
     # callable was physically declared by an on-disk module *OR* "None"
     # otherwise (i.e., if that callable was dynamically declared in-memory).
     func_module_name = func.__module__
 
@@ -298,26 +299,22 @@
     # originally had no lexical access to. That's bad. So, we don't do that.
     #
     # If either...
     if (
         # The passed callable is dynamically declared in-memory...
         func_module_name is None or
         # The passed callable is unnested *OR*...
-        not is_func_nested(func) or
-        # The active Python interpreter fails to declare the private
-        # sys._getframe() getter...
-        get_func_stack_frame is None
+        not is_func_nested(func)
     ):
         # Then silently reduce to a noop by treating this nested callable as
         # module-scoped by preserving "func_locals" as the empty dictionary.
         return {}
     # Else, all of the following constraints hold:
     # * The passed callable is physically declared on-disk.
     # * The passed callable is nested.
-    # * The active Python interpreter declares the sys._getframe() getter.
 
     # ..................{ LOCALS ~ scope                    }..................
     # Local scope of the passed callable to be returned.
     func_scope: CallableScope = {}
 
     # ..................{ LOCALS ~ scope : name             }..................
     # Unqualified name of this nested callable.
@@ -405,18 +402,14 @@
 
         # Skip over this placeholder to the unqualified name of the parent
         # callable lexically containing the passed callable.
         func_scope_name = func_scope_names[-3]
     # print(f'Searching for parent {func_scope_name}() local scope...')
 
     # ..................{ LOCALS ~ frame                    }..................
-    # Next non-ignored frame following the last ignored frame, ignoring an
-    # additional frame embodying the current call to this getter.
-    func_frame = get_func_stack_frame(func_stack_frames_ignore + 1)
-
     # Code object underlying the parent callable associated with the current
     # stack frame if that callable is pure-Python *OR* "None".
     func_frame_codeobj: Optional[CodeType] = None
 
     # Fully-qualified name of that callable's module.
     func_frame_module_name = ''
 
@@ -426,104 +419,103 @@
     # ..................{ SEARCH                            }..................
     # While at least one frame remains on the call stack, iteratively search up
     # the call stack for a stack frame embodying the parent callable directly
     # declaring this nested callable, whereupon that parent callable's local
     # runtime scope is returned as is.
     #
     # Note this also implicitly skips past all other decorators applied *AFTER*
-    # (i.e., lexically above) @beartype to this nested callable: e.g.,
+    # @beartype (and thus residing lexically above @beartype) in caller code to
+    # this nested callable: e.g.,
     #     @the_way_of_kings   <--- skipped past
     #     @words_of_radiance  <--- skipped past
     #     @oathbringer        <--- skipped past
     #     @rhythm_of_war      <--- skipped past
     #     @beartype
     #     def the_stormlight_archive(bruh: str) -> str:
     #         return bruh
-    while func_frame:
+    for func_frame in iter_func_stack_frames(
+        # 0-based index of the first non-ignored frame following the last
+        # ignored frame, ignoring an additional frame embodying the current
+        # call to this getter.
+        func_stack_frames_ignore=func_stack_frames_ignore + 1,
+    ):
         # Code object underlying this frame's scope if that scope is
         # pure-Python *OR* "None" otherwise.
         func_frame_codeobj = get_func_codeobj_or_none(func_frame)
 
-        # If that scope is pure-Python, that code object exists. In this
-        # case...
-        if func_frame_codeobj is not None:
-            # Fully-qualified name of that scope's module.
-            func_frame_module_name = func_frame.f_globals['__name__']
-
-            # Unqualified name of that scope.
-            func_frame_name = func_frame_codeobj.co_name
+        # If this code object does *NOT* exist, this scope is C-based. In this
+        # case, silently ignore this scope and proceed to the next frame.
+        if func_frame_codeobj is None:
+            continue
+        # Else, this code object exists, implying this scope is pure-Python.
+
+        # Fully-qualified name of that scope's module.
+        func_frame_module_name = func_frame.f_globals['__name__']
+
+        # Unqualified name of that scope.
+        func_frame_name = func_frame_codeobj.co_name
+        # print(f'{func_frame_name}() locals: {repr(func_frame.f_locals)}')
+
+        # If that scope is the placeholder string assigned by the active Python
+        # interpreter to all scopes encapsulating the top-most lexical scope of
+        # a module in the current call stack, this search has just crossed a
+        # module boundary and is thus no longer searching within the module
+        # declaring this nested callable and has thus failed to find the
+        # lexical scope of the parent declaring this nested callable. Why?
+        # Because that scope *MUST* necessarily be in the same module as that
+        # of this nested callable. In this case, raise an exception.
+        if func_frame_name == '<module>':
+            raise exception_cls(
+                f'{get_object_basename_scoped(func)}() parent lexical scope '
+                f'{func_scope_name}() not found on call stack.'
+            )
+        # Else, that scope is *NOT* a module.
+        #
+        # If...
+        elif (
+            # That callable's name is that of the current lexical scope to be
+            # found *AND*...
+            func_frame_name == func_scope_name and
+            # That callable's module is that of this nested callable's and thus
+            # resides in the same lexical scope...
+            func_frame_module_name == func_module_name
+        ):
+        # Then that callable embodies the lexical scope to be found. In this
+        # case, that callable is the parent callable directly declaring this
+        # nested callable.
+        #
+        # Note that this scope *CANNOT* be validated to declare this nested
+        # callable. Why? Because this getter function is called by the
+        # @beartype decorator when decorating this nested callable, which has
+        # yet to be declared until @beartype creates and returns a new wrapper
+        # function and is thus unavailable from this scope: e.g.,
+        #     # This conditional *ALWAYS* raises an exception, because this
+        #     # nested callable has yet to be declared.
+        #     if func_name not in func_locals:
+        #         raise exception_cls(
+        #             f'{func_label} not declared by lexically scoped parent '
+        #             f'callable(s) that declared local variables:\n{repr(func_locals)}'
+        #         )
+        #
+        # Ergo, we have *NO* alternative but to blindly assume the above
+        # algorithm correctly collected this scope, which we only do because we
+        # have exhaustively tested this with *ALL* edge cases.
             # print(f'{func_frame_name}() locals: {repr(func_frame.f_locals)}')
 
-            # If that scope is the placeholder string assigned by the active
-            # Python interpreter to all scopes encapsulating the top-most
-            # lexical scope of a module in the current call stack, halt
-            # searching.
-            #
-            # If that scope is a module, this search has just crossed a module
-            # boundary and is thus no longer searching within the module
-            # declaring this nested callable and has thus failed to find the
-            # lexical scope of the parent declaring this nested callable. Why?
-            # Because that scope *MUST* necessarily be in the same module as
-            # that of this nested callable. In this case, immediately break and
-            # raise an exception.
-            if func_frame_name == '<module>':
-                raise exception_cls(
-                    f'{get_object_basename_scoped(func)}() parent lexical scope '
-                    f'{func_scope_name}() not found on call stack.'
-                )
-            # Else, that scope is *NOT* a module.
-            #
-            # If...
-            elif (
-                # That callable's name is that of the current lexical scope to
-                # be found *AND*...
-                func_frame_name == func_scope_name and
-                # That callable's module is that of this nested callable's and
-                # thus resides in the same lexical scope...
-                func_frame_module_name == func_module_name
-            ):
-            # Then that callable embodies the lexical scope to be found. In
-            # this case, that callable is the parent callable directly
-            # declaring this nested callable.
-            #
-            # Note that this scope *CANNOT* be validated to declare this nested
-            # callable. Why? Because this getter function is called by the
-            # @beartype decorator when decorating this nested callable, which
-            # has yet to be declared until @beartype creates and returns a new
-            # wrapper function and is thus unavailable from this scope: e.g.,
-            #     # This conditional *ALWAYS* raises an exception, because this
-            #     # nested callable has yet to be declared.
-            #     if func_name not in func_locals:
-            #         raise exception_cls(
-            #             f'{func_label} not declared by lexically scoped parent '
-            #             f'callable(s) that declared local variables:\n{repr(func_locals)}'
-            #         )
-            #
-            # Ergo, we have *NO* alternative but to blindly assume the above
-            # algorithm correctly collected this scope, which we only do
-            # because we have exhaustively tested this with *ALL* edge cases.
-                # print(f'{func_frame_name}() locals: {repr(func_frame.f_locals)}')
-
-                # Local scope of the passed callable. Since this nested
-                # callable is directly declared in the body of this parent
-                # callable, the local scope of this nested callable is
-                # *EXACTLY* the local scope of the body of this parent
-                # callable. Well, isn't that special?
-                func_scope = func_frame.f_locals
-
-                # Halt iteration.
-                break
-            # Else, that callable does *NOT* embody the current lexical scope
-            # to be found. In this case, silently ignore that callable and
-            # proceed to the next frame in the call stack.
-        # Else, that callable is C-based. In this case, silently ignore that
-        # callable and proceed to the next frame in the call stack.
-
-        # Iterate to the next frame on the call stack.
-        func_frame = func_frame.f_back
+            # Local scope of the passed callable. Since this nested callable is
+            # directly declared in the body of this parent callable, the local
+            # scope of this nested callable is *EXACTLY* the local scope of the
+            # body of this parent callable. Well, isn't that special?
+            func_scope = func_frame.f_locals
+
+            # Halt iteration.
+            break
+        # Else, that callable does *NOT* embody the current lexical scope to be
+        # found. In this case, silently ignore that callable and proceed to the
+        # next frame in the call stack.
 
     # Return the local scope of the passed callable.
     return func_scope
 
 # ....................{ ADDERS                            }....................
 def add_func_scope_attr(
     # Mandatory parameters.
```

### Comparing `beartype-0.9.0/beartype/_util/func/utilfunctest.py` & `beartype-0.9.1/beartype/_util/func/utilfunctest.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/func/utilfuncwrap.py` & `beartype-0.9.1/beartype/_util/func/utilfuncwrap.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/hint/nonpep/utilnonpeptest.py` & `beartype-0.9.1/beartype/_util/hint/nonpep/utilnonpeptest.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/hint/pep/mod/utilmodnumpy.py` & `beartype-0.9.1/beartype/_util/hint/pep/mod/utilmodnumpy.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/hint/pep/proposal/pep484/utilpep484.py` & `beartype-0.9.1/beartype/_util/hint/pep/proposal/pep484/utilpep484.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,16 +144,16 @@
 
         # print(f'Testing generic hint {repr(hint)} deep ignorability...')
         # If this generic is the "typing.Generic" superclass directly
         # parametrized by one or more type variables (e.g.,
         # "typing.Generic[T]"), return true.
         #
         # Note that we intentionally avoid calling the
-        # get_hint_pep_type_isinstanceable_or_none() function here, which has been
-        # intentionally designed to exclude PEP-compliant type hints
+        # get_hint_pep_type_isinstanceable_or_none() function here, which has
+        # been intentionally designed to exclude PEP-compliant type hints
         # originating from "typing" type origins for stability reasons.
         if get_hint_pep_origin_or_none(hint) is Generic:
             # print(f'Testing generic hint {repr(hint)} deep ignorability... True')
             return True
         # Else, this generic is *NOT* the "typing.Generic" superclass directly
         # parametrized by one or more type variables and thus *NOT* an
         # ignorable non-protocol.
```

### Comparing `beartype-0.9.0/beartype/_util/hint/pep/proposal/pep484/utilpep484generic.py` & `beartype-0.9.1/beartype/_util/hint/pep/proposal/pep484/utilpep484generic.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/hint/pep/proposal/pep484/utilpep484newtype.py` & `beartype-0.9.1/beartype/_util/hint/pep/proposal/pep484/utilpep484newtype.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/hint/pep/proposal/pep484/utilpep484ref.py` & `beartype-0.9.1/beartype/_util/hint/pep/proposal/pep484/utilpep484ref.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/hint/pep/proposal/pep484/utilpep484typevar.py` & `beartype-0.9.1/beartype/_util/hint/pep/proposal/pep484/utilpep484typevar.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/hint/pep/proposal/pep484/utilpep484union.py` & `beartype-0.9.1/beartype/_util/hint/pep/proposal/pep484/utilpep484union.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/hint/pep/proposal/pep484585/utilpep484585.py` & `beartype-0.9.1/beartype/_util/hint/pep/proposal/pep484585/utilpep484585.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/hint/pep/proposal/pep484585/utilpep484585arg.py` & `beartype-0.9.1/beartype/_util/hint/pep/proposal/pep484585/utilpep484585arg.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,15 +84,16 @@
 
     # If this hint is *NOT* subscripted by one argument, raise an exception.
     if len(hint_args) != 1:
         assert isinstance(exception_prefix, str), (
             f'{repr(exception_prefix)} not string.')
         raise BeartypeDecorHintPep585Exception(
             f'{exception_prefix}PEP 585 type hint {repr(hint)} '
-            f'not subscripted (indexed) by exactly one argument.'
+            f'not subscripted (indexed) by one argument (i.e., '
+            f'subscripted by {len(hint_args)} != 1 arguments).'
         )
     # Else, this hint is subscripted by one argument.
 
     # Return this argument as is.
     return hint_args[0]
 
 
@@ -148,13 +149,14 @@
 
     # If this hint is *NOT* subscripted by three arguments, raise an exception.
     if len(hint_args) != 3:
         assert isinstance(exception_prefix, str), (
             f'{repr(exception_prefix)} not string.')
         raise BeartypeDecorHintPep585Exception(
             f'{exception_prefix}PEP 585 type hint {repr(hint)} '
-            f'not subscripted (indexed) by exactly three arguments.'
+            f'not subscripted (indexed) by three arguments (i.e., '
+            f'subscripted by {len(hint_args)} != 3 arguments).'
         )
     # Else, this hint is subscripted by one argument.
 
     # Return this tuple of arguments as is.
     return hint_args  # type: ignore[return-value]
```

### Comparing `beartype-0.9.0/beartype/_util/hint/pep/proposal/pep484585/utilpep484585func.py` & `beartype-0.9.1/beartype/_util/hint/pep/proposal/pep484585/utilpep484585func.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 callable currently being decorated by :func:`beartype.beartype`).
 
 This private submodule is *not* intended for importation by downstream callers.
 '''
 
 # ....................{ IMPORTS                           }....................
 from beartype.roar import BeartypeDecorHintPep484585Exception
-from beartype._data.hint.pep.sign.datapepsigns import (
-    HintSignAsyncGenerator,
-    HintSignCoroutine,
-    HintSignGenerator,
+from beartype._data.hint.pep.sign.datapepsigns import HintSignCoroutine
+from beartype._data.hint.pep.sign.datapepsignset import (
+    HINT_SIGNS_RETURN_GENERATOR_ASYNC,
+    HINT_SIGNS_RETURN_GENERATOR_SYNC,
 )
 from beartype._util.func.utilfunctest import (
     is_func_async_coroutine,
     is_func_async_generator,
     is_func_sync_generator,
 )
 from beartype._util.hint.pep.proposal.pep484585.utilpep484585arg import (
@@ -31,16 +31,15 @@
     prefix_callable_decorated_return)
 from beartype._util.utiltyping import TypeException
 from collections.abc import Callable
 
 # See the "beartype.cave" submodule for further commentary.
 __all__ = ['STAR_IMPORTS_CONSIDERED_HARMFUL']
 
-# ....................{ GETTERS                           }....................
-#FIXME: Unit test us up, please.
+# ....................{ REDUCERS ~ return                 }....................
 def reduce_hint_pep484585_func_return(func: Callable) -> object:
     '''
     Reduce the possibly PEP-noncompliant type hint annotating the return of the
     passed callable if any to a simpler form to generate
     optimally efficient type-checking by the :func:`beartype.beartype`
     decorator.
 
@@ -58,17 +57,18 @@
         Single argument subscripting this hint.
 
     Raises
     ----------
     :exc:`BeartypeDecorHintPep484585Exception`
         If this callable is either:
 
-        * A generator *not* annotated by a :attr:`typing.Generator` type hint.
-        * An asynchronous generator *not* annotated by a
-          :attr:`typing.AsyncGenerator` type hint.
+        * A synchronous generator *not* annotated by a type hint identified by
+          a sign in the :data:`HINT_SIGNS_RETURN_GENERATOR_SYNC` set.
+        * An asynchronous generator *not* annotated by a type hint identified
+          by a sign in the :data:`HINT_SIGNS_RETURN_GENERATOR_ASYNC` set.
     '''
 
     # Type hint annotating this callable's return, which the caller has already
     # explicitly guaranteed to exist.
     hint = func.__annotations__['return']
 
     # Sign uniquely identifying this hint if any *OR* "None" otherwise (e.g.,
@@ -103,42 +103,54 @@
         # accept this hint as if this hint had instead been expanded to the
         # semantically equivalent PEP 484- or 585-compliant coroutine hint
         # "Coroutine[None, None, {hint}]".
     # Else, the decorated callable is *NOT* a coroutine.
     #
     # If the decorated callable is an asynchronous generator...
     elif is_func_async_generator(func):
-        # If this hint is *NOT* "AsyncGenerator[...]", this type hint is
-        # invalid. In this case, raise an exception.
-        if hint_sign is not HintSignAsyncGenerator:
+        #FIXME: Unit test this up, please!
+        # If this hint is semantically invalid as the return annotation of this
+        # callable, raise an exception.
+        if hint_sign not in HINT_SIGNS_RETURN_GENERATOR_ASYNC:
             _die_of_hint_return_invalid(
                 func=func,
                 exception_suffix=(
                     ' (i.e., expected either '
-                    'collections.abc.AsyncGenerator[...] or '
-                    'typing.AsyncGenerator[...] type hint).'
+                    'collections.abc.AsyncGenerator[YieldType, SendType], '
+                    'collections.abc.AsyncIterable[YieldType], '
+                    'collections.abc.AsyncIterator[YieldType], '
+                    'typing.AsyncGenerator[YieldType, SendType], '
+                    'typing.AsyncIterable[YieldType], or '
+                    'typing.AsyncIterator[YieldType] '
+                    'type hint).'
                 ),
             )
-        # Else, this hint is "AsyncGenerator[...]".
+        # Else, this hint is valid as the return annotation of this callable.
     # Else, the decorated callable is *NOT* an asynchronous generator.
     #
     # If the decorated callable is a synchronous generator...
     elif is_func_sync_generator(func):
-        # If this hint is *NOT* "Generator[...]", this type hint is invalid.
-        # In this case, raise an exception.
-        if hint_sign is not HintSignGenerator:
+        #FIXME: Unit test this up, please!
+        # If this hint is semantically invalid as the return annotation of this
+        # callable, raise an exception.
+        if hint_sign not in HINT_SIGNS_RETURN_GENERATOR_SYNC:
             _die_of_hint_return_invalid(
                 func=func,
                 exception_suffix=(
                     ' (i.e., expected either '
-                    'collections.abc.Generator[...] or '
-                    'typing.Generator[...] type hint).'
+                    'collections.abc.Generator[YieldType, SendType, ReturnType], '
+                    'collections.abc.Iterable[YieldType], '
+                    'collections.abc.Iterator[YieldType], '
+                    'typing.Generator[YieldType, SendType, ReturnType], '
+                    'typing.Iterable[YieldType], or '
+                    'typing.Iterator[YieldType] '
+                    'type hint).'
                 ),
             )
-        # Else, this hint is "Generator[...]".
+        # Else, this hint is valid as the return annotation of this callable.
     # Else, the decorated callable is none of the kinds detected above.
 
     # Return this possibly reduced hint.
     return hint
 
 # ....................{ PRIVATE ~ validators              }....................
 def _die_of_hint_return_invalid(
```

### Comparing `beartype-0.9.0/beartype/_util/hint/pep/proposal/pep484585/utilpep484585generic.py` & `beartype-0.9.1/beartype/_util/hint/pep/proposal/pep484585/utilpep484585generic.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/hint/pep/proposal/pep484585/utilpep484585ref.py` & `beartype-0.9.1/beartype/_util/hint/pep/proposal/pep484585/utilpep484585ref.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,17 @@
     :exc:`BeartypeDecorHintForwardRefException`
         If this object is *not* a forward reference type hint.
     '''
 
     # If this is *NOT* a forward reference type hint, raise an exception.
     if not isinstance(hint, HINT_PEP484585_FORWARDREF_TYPES):
         raise BeartypeDecorHintForwardRefException(
-            f'{exception_prefix}{repr(hint)} not forward reference.')
+            f'{exception_prefix}{repr(hint)} not forward reference '
+            f'(i.e., neither string nor "typing.ForwardRef" instance).'
+        )
 
 # ....................{ GETTERS ~ kind : forwardref       }....................
 #FIXME: Unit test against nested classes.
 #FIXME: Validate that this forward reference string is *NOT* the empty string.
 #FIXME: Validate that this forward reference string is a syntactically valid
 #"."-delimited concatenation of Python identifiers. We already have logic
 #performing that validation somewhere, so let's reuse that here, please.
```

### Comparing `beartype-0.9.0/beartype/_util/hint/pep/proposal/pep484585/utilpep484585type.py` & `beartype-0.9.1/beartype/_util/hint/pep/proposal/pep484585/utilpep484585type.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/hint/pep/proposal/utilpep544.py` & `beartype-0.9.1/beartype/_util/hint/pep/proposal/utilpep544.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/hint/pep/proposal/utilpep585.py` & `beartype-0.9.1/beartype/_util/hint/pep/proposal/utilpep585.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/hint/pep/proposal/utilpep586.py` & `beartype-0.9.1/beartype/_util/hint/pep/proposal/utilpep586.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/hint/pep/proposal/utilpep589.py` & `beartype-0.9.1/beartype/_util/hint/pep/proposal/utilpep589.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/hint/pep/proposal/utilpep593.py` & `beartype-0.9.1/beartype/_util/hint/pep/proposal/utilpep593.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/hint/pep/utilpepattr.py` & `beartype-0.9.1/beartype/_util/hint/pep/utilpepattr.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/hint/pep/utilpepget.py` & `beartype-0.9.1/beartype/_util/hint/pep/utilpepget.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/hint/pep/utilpeptest.py` & `beartype-0.9.1/beartype/_util/hint/pep/utilpeptest.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/hint/utilhintconv.py` & `beartype-0.9.1/beartype/_util/hint/utilhintconv.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/hint/utilhintget.py` & `beartype-0.9.1/beartype/_util/hint/utilhintget.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/hint/utilhinttest.py` & `beartype-0.9.1/beartype/_util/hint/utilhinttest.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/kind/utilkinddict.py` & `beartype-0.9.1/beartype/_util/kind/utilkinddict.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/mod/utilmoddeprecate.py` & `beartype-0.9.1/beartype/_util/mod/utilmoddeprecate.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/mod/utilmodimport.py` & `beartype-0.9.1/beartype/_util/mod/utilmodimport.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/mod/utilmodtest.py` & `beartype-0.9.1/beartype/_util/mod/utilmodtest.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/mod/utilmodule.py` & `beartype-0.9.1/beartype/_util/mod/utilmodule.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/os/utilostest.py` & `beartype-0.9.1/beartype/_util/os/utilostest.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/py/utilpyinterpreter.py` & `beartype-0.9.1/beartype/_util/py/utilpyinterpreter.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/py/utilpyversion.py` & `beartype-0.9.1/beartype/_util/py/utilpyversion.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/py/utilpyword.py` & `beartype-0.9.1/beartype/_util/py/utilpyword.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/text/utiltextget.py` & `beartype-0.9.1/beartype/_util/text/utiltextget.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/text/utiltextident.py` & `beartype-0.9.1/beartype/_util/text/utiltextident.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/text/utiltextjoin.py` & `beartype-0.9.1/beartype/_util/text/utiltextjoin.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/text/utiltextlabel.py` & `beartype-0.9.1/beartype/_util/text/utiltextlabel.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,14 +103,33 @@
         func_label_prefix = 'asynchronous generator '
     # Else, that callable is *NOT* an asynchronous generator.
 
     # Return the fully-qualified name of this callable preceded by this prefix.
     return f'{func_label_prefix}{get_object_basename_scoped(func)}()'
 
 # ....................{ LABELLERS ~ type                  }....................
+def label_obj_type(obj: object) -> str:
+    '''
+    Human-readable label describing the class of the passed object.
+
+    Parameters
+    ----------
+    obj : object
+        Object whose class is to be labelled.
+
+    Returns
+    ----------
+    str
+        Human-readable label describing the class of this object.
+    '''
+
+    # Tell me why, why, why I curse the sky! ...no, srsly.
+    return label_type(type(obj))
+
+
 def label_type(cls: type) -> str:
     '''
     Human-readable label describing the passed class.
 
     Parameters
     ----------
     cls : type
```

### Comparing `beartype-0.9.0/beartype/_util/text/utiltextmagic.py` & `beartype-0.9.1/beartype/_util/text/utiltextmagic.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/text/utiltextmunge.py` & `beartype-0.9.1/beartype/_util/text/utiltextmunge.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/text/utiltextrepr.py` & `beartype-0.9.1/beartype/_util/text/utiltextrepr.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,23 +8,52 @@
 transforming strings into new derivative strings) utilities.
 
 This private submodule is *not* intended for importation by downstream callers.
 """
 
 # ....................{ IMPORTS                           }....................
 from beartype.roar._roarwarn import _BeartypeUtilCallableWarning
+from beartype._cave._cavefast import NumberType
 from beartype._util.utilobject import get_object_basename_scoped
 from collections.abc import Callable
 from pprint import saferepr
 from re import (
     DOTALL,
     sub as re_sub
 )
 from string import punctuation
 
+# ....................{ PRIVATE                           }....................
+_CHARS_PUNCTUATION = frozenset(punctuation)
+'''
+Frozen set of all **ASCII punctuation characters** (i.e., non-Unicode
+characters satisfying the conventional definition of English punctuation).
+
+Note that the :attr:`string.punctuation` object is actually an inefficient
+string of these characters rather than an efficient collection. Ergo, this set
+should *ALWAYS* be accessed in lieu of that string.
+'''
+
+
+_TYPES_UNQUOTABLE = (
+    # Byte strings, whose representations are already quoted as "b'...'".
+    bytes,
+    # Numbers, whose representations are guaranteed to both contain *NO*
+    # whitespace and be sufficiently terse as to benefit from *NO* quoting.
+    NumberType,
+)
+'''
+**Unquotable tuple union** (i.e., isinstancable tuple of all classes such that
+the :func:`represent_object` function intentionally avoids double-quoting the
+machine-readable representations all instances of these classes, typically due
+to these representations either being effectively quoted already *or*
+sufficiently terse as to not benefit from being quoted).
+'''
+
+
 # ....................{ REPRESENTERS                      }....................
 def represent_object(
     # Mandatory parameters.
     obj: object,
 
     # Optional parameters.
     max_len: int = 96,
@@ -107,18 +136,18 @@
     if not obj_repr:
         return '""'
     # Else, this representation is non-empty.
     #
     # If this representation is neither...
     elif not (
         # Prefixed by punctuation *NOR*...
-        obj_repr[0] in punctuation or
-        # A byte-string, in which case this representation is instead prefixed
-        # by "b'".
-        isinstance(obj, bytes)
+        obj_repr[0] in _CHARS_PUNCTUATION or
+        # An instance of a class whose representations do *NOT* benefit from
+        # explicit quoting...
+        isinstance(obj, _TYPES_UNQUOTABLE)
     ):
     # Then this representation is *NOT* demarcated from preceding characters in
     # the parent string embedding this representation. In this case,
     # double-quote this representation for disambiguity with preceding
     # characters (e.g., sequence indices).
         obj_repr = f'"{obj_repr}"'
```

### Comparing `beartype-0.9.0/beartype/_util/text/utiltexttest.py` & `beartype-0.9.1/beartype/_util/text/utiltexttest.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/utilobject.py` & `beartype-0.9.1/beartype/_util/utilobject.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/_util/utiltyping.py` & `beartype-0.9.1/beartype/_util/utiltyping.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/cave/__init__.py` & `beartype-0.9.1/beartype/cave/__init__.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/cave/_cavelib.py` & `beartype-0.9.1/beartype/cave/_cavelib.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/meta.py` & `beartype-0.9.1/beartype/meta.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 See Also
 ----------
 "Python Version" section of this submodule's docstring for a detailed
 justification of this constant's current value.
 '''
 
 
-PYTHON_VERSION_MINOR_MAX = 10
+PYTHON_VERSION_MINOR_MAX = 11
 '''
 Maximum minor stable version of this major version of Python currently released
 (e.g., ``5`` if Python 3.5 is the most recent stable version of Python 3.x).
 '''
 
 
 def _convert_version_str_to_tuple(version_str: str) -> _Tuple[int, ...]:
@@ -196,15 +196,15 @@
 # * "{patch}" specifies the patch version, incremented only when correcting
 #   outstanding issues in a manner preserving such compatibility.
 #
 # When in doubt, increment only the minor version and reset the patch version.
 # For further details, see http://semver.org.
 #!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 
-VERSION = '0.9.0'
+VERSION = '0.9.1'
 '''
 Human-readable package version as a ``.``-delimited string.
 '''
 
 
 VERSION_PARTS = _convert_version_str_to_tuple(VERSION)
 '''
@@ -323,34 +323,57 @@
   enables forward compatibility with all future versions of this dependency
   known *not* to break backward compatibility, but should only be applied to
   dependencies strictly following the semantic versioning contract.
 * ``{version1}`` and ``{version1}`` are arbitrary version strings (e.g.,
   ``2020.2.16``, ``0.75a2``).
 '''
 
-# ....................{ METADATA ~ libs : test            }....................
+# ....................{ METADATA ~ libs : test : optional }....................
 #!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 # CAUTION: Avoid constraining optional test-time dependencies to version
 # ranges, which commonly fail for edge-case test environments -- including:
 # * The oldest Python version still supported by @beartype, which typically is
 #   *NOT* supported by newer versions of these dependencies.
 #!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
-LIBS_TESTTIME_OPTIONAL = (
-    'typing_extensions',
-) + (
+def _make_libs_testtime_optional() -> _Tuple[str, ...]:
+    '''
+    Create and return **optional test-time package dependencies** (i.e.,
+    dependencies recommended to test this package with :mod:`tox` as a
+    developer at the command line) as a tuple of :mod:`setuptools`-specific
+    requirements strings of the format ``{project_name} {comparison1}{version1},
+    ...,{comparisonN}{versionN}``.
+    '''
+
+    # List of unconditional optional test-time package dependencies.
+    libs_testtime_optional = [
+        # Required by our optional "test_sphinx" functional test.
+        'sphinx',
+
+        # Required to exercise beartype validators and thus functionality
+        # requiring beartype validators (e.g., "numpy.typing.NDArray" type
+        # hints) under Python < 3.9.
+        'typing_extensions',
+    ]
+
     # If the active Python interpreter is *NOT* PyPy...
-    (
-        # mypy >= 0.800, a reasonably recent version known to behave well. Even
-        # less reasonably recent versions of mypy are significantly deficient
-        # with respect to error reporting and *MUST* thus be blacklisted.
-        'mypy >=0.800' ,
+    if not _is_py_pypy():
+        # Require a reasonably recent version of mypy known to behave well.
+        # Less recent versions are significantly deficient with respect to
+        # error reporting and *MUST* thus be blacklisted.
+        #
+        # Note that PyPy currently fails to support mypy. See also this
+        # official documentation discussing this regrettable incompatibility:
+        #     https://mypy.readthedocs.io/en/stable/faq.html#does-it-run-on-pypy
+        libs_testtime_optional.append('mypy >=0.800')
+
         # If the current platform is *NOT* macOS...
-        (
-            # NumPy. NumPy has become *EXTREMELY* non-trivial to install under
-            # macOS with "pip", due to the conjunction of multiple issues:
+        if not _is_os_macos():
+            # Require NumPy. NumPy has become *EXTREMELY* non-trivial to
+            # install under macOS with "pip", due to the conjunction of
+            # multiple issues. These include:
             # * NumPy > 1.18.0, whose initial importation now implicitly
             #   detects whether the BLAS implementation NumPy was linked
             #   against is sane and raises a "RuntimeError" exception if that
             #   implementation is insane resembling:
             #       RuntimeError: Polyfit sanity test emitted a warning, most
             #       likely due to using a buggy Accelerate backend. If you
             #       compiled yourself, more information is available at
@@ -364,39 +387,36 @@
             #   install NumPy even when the "--force-reinstall" option is
             #   explicitly passed to "pip". Oddly, passing that option to "pip"
             #   under CPython resolves this issue -- which is why we only
             #   selectively disable NumPy installation under macOS + PyPy.
             #
             # See also this upstream NumPy issue:
             #     https://github.com/numpy/numpy/issues/15947
-            'numpy',
-        ) if not _is_os_macos() else
-        # Else, the active Python interpreter is PyPy under macOS and thus
-        # fails to support NumPy. In this case, avoid requiring NumPy.
-        ()
-    ) if not _is_py_pypy() else
-    # Else, the active Python interpreter is PyPy and thus fails to support
-    # mypy. In this case, avoid requiring mypy. See also this official
-    # documentation discussing mypy's current incompatibility with PyPy:
-    #     https://mypy.readthedocs.io/en/stable/faq.html#does-it-run-on-pypy
-    ()
-)
+            libs_testtime_optional.append('numpy')
+        # Else, the current platform is macOS.
+    # Else, the active Python interpreter is PyPy.
+
+    # Return a tuple coerced from this list.
+    return tuple(libs_testtime_optional)
+
+
+LIBS_TESTTIME_OPTIONAL = _make_libs_testtime_optional()
 '''
 **Optional developer test-time package dependencies** (i.e., dependencies
 recommended to test this package with :mod:`tox` as a developer at the command
 line) as a tuple of :mod:`setuptools`-specific requirements strings of the
 format ``{project_name} {comparison1}{version1},...,{comparisonN}{versionN}``.
 
 See Also
 ----------
 :data:`LIBS_RUNTIME_OPTIONAL`
     Further details.
 '''
 
-
+# ....................{ METADATA ~ libs : test : mandatory}....................
 LIBS_TESTTIME_MANDATORY_COVERAGE = (
     'coverage >=5.5',
 )
 '''
 **Mandatory test-time coverage package dependencies** (i.e., dependencies
 required to measure test coverage for this package) as a tuple of
 :mod:`setuptools`-specific requirements strings of the format ``{project_name}
@@ -446,36 +466,36 @@
 See Also
 ----------
 :data:`LIBS_RUNTIME_OPTIONAL`
     Further details.
 '''
 
 # ....................{ METADATA ~ libs : doc             }....................
-_LIB_VERSION_MIN_SPHINX = '4.1.0'
+_LIB_DOCTIME_MANDATORY_VERSION_MINIMUM_SPHINX = '4.1.0'
 '''
 Human-readable minimum version as a ``.``-delimited string of :mod:`sphinx`
 required to build package documentation.
 
 Specifically, this project requires:
 
 * :mod:sphinx` >= 4.1.0, which first supported the
   ``autodoc_typehints = 'both'`` option.
 '''
 
 
-_LIB_VERSION_MIN_SPHINX_RTD_THEME = '0.5.1'
+_LIB_DOCTIME_MANDATORY_VERSION_MINIMUM_SPHINX_RTD_THEME = '0.5.1'
 '''
 Human-readable minimum version as a ``.``-delimited string of the **Read The
 Docs (RTD)-flavoured Sphinx theme** (i.e., :mod:`sphinx_rtd_theme`) optionally
 leveraged when building package documentation.
 '''
 
 
 LIBS_DOCTIME_MANDATORY = (
-    f'sphinx >={_LIB_VERSION_MIN_SPHINX}',
+    f'sphinx >={_LIB_DOCTIME_MANDATORY_VERSION_MINIMUM_SPHINX}',
 )
 '''
 **Mandatory developer documentation build-time package dependencies** (i.e.,
 dependencies required to manually build documentation for this package as a
 developer at the command line) as a tuple of :mod:`setuptools`-specific
 requirements strings of the format ``{project_name}
 {comparison1}{version1},...,{comparisonN}{versionN}``.
@@ -491,16 +511,19 @@
 ----------
 :data:`LIBS_RUNTIME_OPTIONAL`
     Further details.
 '''
 
 
 LIBS_DOCTIME_MANDATORY_RTD = (
-    f'sphinx =={_LIB_VERSION_MIN_SPHINX}',
-    f'sphinx-rtd-theme =={_LIB_VERSION_MIN_SPHINX_RTD_THEME}',
+    f'sphinx =={_LIB_DOCTIME_MANDATORY_VERSION_MINIMUM_SPHINX}',
+    (
+        f'sphinx-rtd-theme '
+        f'=={_LIB_DOCTIME_MANDATORY_VERSION_MINIMUM_SPHINX_RTD_THEME}'
+    ),
 )
 '''
 **Mandatory Read The Docs (RTD) documentation build-time package dependencies**
 (i.e., dependencies required to automatically build documentation for this
 package from the third-party RTD hosting service) as a tuple of
 :mod:`setuptools`-specific requirements strings of the format ``{project_name}
 {comparison1}{version1},...,{comparisonN}{versionN}``.
```

### Comparing `beartype-0.9.0/beartype/roar/__init__.py` & `beartype-0.9.1/beartype/roar/__init__.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/roar/_roarexc.py` & `beartype-0.9.1/beartype/roar/_roarexc.py`

 * *Files 1% similar despite different names*

```diff
@@ -605,38 +605,38 @@
     This exception denotes a critical internal issue and should thus *never* be
     raised -- let alone allowed to percolate up the call stack to end users.
     '''
 
     pass
 
 
-class _BeartypeUtilTypeException(_BeartypeUtilException):
+class _BeartypeUtilModuleException(_BeartypeUtilException):
     '''
-    **Beartype class utility exception.**
+    **Beartype module utility exception.**
 
     This exception is raised by public functions of the private
-    :mod:`beartype._util.cls.utilclstest` subpackage.
+    :mod:`beartype._util.mod.utilmodule` subpackage when dynamically importing
+    an unimportable external user-defined module, typically due to a
+    **PEP-compliant forward reference type hint** (i.e., string whose value is
+    the name of a user-defined class that has yet to be defined) erroneously
+    referencing a non-existent module or module attribute.
 
     This exception denotes a critical internal issue and should thus *never* be
     raised -- let alone allowed to percolate up the call stack to end users.
     '''
 
     pass
 
 
-class _BeartypeUtilModuleException(_BeartypeUtilException):
+class _BeartypeUtilPathException(_BeartypeUtilException):
     '''
-    **Beartype module utility exception.**
+    **Beartype path utility exception.**
 
     This exception is raised by public functions of the private
-    :mod:`beartype._util.mod.utilmodule` subpackage when dynamically importing
-    an unimportable external user-defined module, typically due to a
-    **PEP-compliant forward reference type hint** (i.e., string whose value is
-    the name of a user-defined class that has yet to be defined) erroneously
-    referencing a non-existent module or module attribute.
+    :mod:`beartype._util.path` subpackage on various fatal edge cases.
 
     This exception denotes a critical internal issue and should thus *never* be
     raised -- let alone allowed to percolate up the call stack to end users.
     '''
 
     pass
 
@@ -650,14 +650,28 @@
 
     This exception denotes a critical internal issue and should thus *never* be
     raised -- let alone allowed to percolate up the call stack to end users.
     '''
 
     pass
 
+
+class _BeartypeUtilTypeException(_BeartypeUtilException):
+    '''
+    **Beartype class utility exception.**
+
+    This exception is raised by public functions of the private
+    :mod:`beartype._util.cls.utilclstest` subpackage.
+
+    This exception denotes a critical internal issue and should thus *never* be
+    raised -- let alone allowed to percolate up the call stack to end users.
+    '''
+
+    pass
+
 # ....................{ PRIVATE ~ util : call               }..................
 class _BeartypeCallHintRaiseException(_BeartypeUtilException):
     '''
     Abstract base class of all **beartype human-readable exception raiser
     exceptions.**
 
     Instances of subclasses of this exception are raised by private utility
```

### Comparing `beartype-0.9.0/beartype/roar/_roarwarn.py` & `beartype-0.9.1/beartype/roar/_roarwarn.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/vale/__init__.py` & `beartype-0.9.1/beartype/vale/__init__.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/vale/_factory/_valeis.py` & `beartype-0.9.1/beartype/vale/_factory/_valeis.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/vale/_factory/_valeisabc.py` & `beartype-0.9.1/beartype/vale/_factory/_valeisabc.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/vale/_factory/_valeiscls.py` & `beartype-0.9.1/beartype/vale/_factory/_valeiscls.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/vale/_factory/_valeisobj.py` & `beartype-0.9.1/beartype/vale/_factory/_valeisobj.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/vale/_factory/_valeisoper.py` & `beartype-0.9.1/beartype/vale/_factory/_valeisoper.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/vale/_util/_valeutilsnip.py` & `beartype-0.9.1/beartype/vale/_util/_valeutilsnip.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/vale/_util/_valeutiltest.py` & `beartype-0.9.1/beartype/vale/_util/_valeutiltest.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype/vale/_valevale.py` & `beartype-0.9.1/beartype/vale/_valevale.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype.egg-info/PKG-INFO` & `beartype-0.9.1/beartype.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: beartype
-Version: 0.9.0
+Version: 0.9.1
 Summary: Unbearably fast runtime type checking in pure Python.
 Home-page: https://github.com/beartype/beartype
 Author: Cecil Curry, et al.
 Author-email: leycec@gmail.com
 Maintainer: Cecil Curry, et al.
 Maintainer-email: leycec@gmail.com
 License: MIT
-Download-URL: https://github.com/beartype/beartype/archive/0.9.0.tar.gz
+Download-URL: https://github.com/beartype/beartype/archive/0.9.1.tar.gz
 Project-URL: Source, https://github.com/beartype/beartype
 Project-URL: Issues, https://github.com/beartype/beartype/issues
 Project-URL: Releases, https://github.com/beartype/beartype/issues
 Keywords: type checking,type hints,PEP 484
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -25,14 +25,15 @@
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Typing :: Typed
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6.0
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: all
 Provides-Extra: dev
 Provides-Extra: doc-rtd
 Provides-Extra: test-tox
 Provides-Extra: test-tox-coverage
@@ -52,15 +53,17 @@
 
 .. # ------------------( SYNOPSIS                           )------------------
 
 =================
 |beartype-banner|
 =================
 
-|ci-badge| |rtd-badge| |codecov-badge|
+|ci-badge| |codecov-badge|
+
+.. #FIXME: Add "|rtd-badge|" back above *AFTER* resolving Sphinx build issues.
 
 .. parsed-literal::
 
    Look for the bare necessities,
      the simple bare necessities.
    Forget about your worries and your strife.
 
@@ -143,14 +146,19 @@
 Actions`_ **+** tox_ **+** pytest_ **+** Codecov_, and `permissively
 distributed <beartype license_>`__ under the `MIT license`_. Beartype has *no*
 runtime dependencies, `only one test-time dependency <pytest_>`__, and `only
 one documentation-time dependency <Sphinx_>`__. Beartype supports `all actively
 developed Python versions <Python status_>`__, `all Python package managers
 <Install_>`__, and `multiple platform-specific package managers <Install_>`__.
 
+    Beartype `powers quality assurance across the Python ecosystem <beartype
+    dependents_>`__.
+
+    |icon-graspologic| |icon-hydrazen| |icon-pycrisp| |icon-sentipy|
+
 .. # ------------------( TABLE OF CONTENTS                  )------------------
 .. # Blank line. By default, Docutils appears to only separate the subsequent
 .. # table of contents heading from the prior paragraph by less than a single
 .. # blank line, hampering this table's readability and aesthetic comeliness.
 
 |
 
@@ -755,15 +763,15 @@
 
 If you don't know `type hints <PEP 484_>`__, this is your moment to go deep on
 the hardest hammer in Python's SQA_ toolbox. Here are a few friendly primers to
 guide you on your maiden voyage through the misty archipelagos of type hinting:
 
 * `"Python Type Checking (Guide)" <RealPython_>`__, a comprehensive third-party
   introduction to the subject. Like most existing articles, this guide predates
-  `O(1)` runtime type checkers and thus discusses only static type checking.
+  ``O(1)`` runtime type checkers and thus discusses only static type checking.
   Thankfully, the underlying syntax and semantics cleanly translate to runtime
   type checking.
 * `"PEP 484 -- Type Hints" <PEP 484_>`__, the defining standard, holy grail,
   and first testament of type hinting `personally authored by Python's former
   Benevolent Dictator for Life (BDFL) himself, Guido van Rossum <Guido van
   Rossum_>`__. Since it's surprisingly approachable and covers all the core
   conceits in detail, we recommend reading at least a few sections of interest.
@@ -1081,16 +1089,16 @@
     Wherever you can, prefer type_ and typing.Type_. Sure, they're
     inflexible, but they're inflexibly standardized across type checkers.
     Everywhere else, default to ``beartype.vale.IsSubclass``.
 
     See ``help(beartype.vale.IsSubclass)`` for further details.
 
 .. [#enum_type]
-   You don't want to know the type of enum.Enum_ members. No... seriously. You
-   don't. You do? Oh, very well. It's enum.Enum_. :superscript:`mic drop`
+   You don't want to know the type of enum.Enum_ members. No... srsly. You
+   don't. You do? Very well. It's enum.Enum_. :superscript:`mic drop`
 
 Validator Syntax
 ~~~~~~~~~~~~~~~~
 
 Beartype validators support a rich domain-specific language (DSL) leveraging
 familiar Python operators. Dynamically create new validators on-the-fly from
 existing validators, fueling reuse and preserving DRY_:
@@ -1190,17 +1198,206 @@
   class first introduced with Python 3.9.0 and since backported to older Python
   versions by the `third-party "typing_extensions" package
   <typing_extensions_>`__, which beartype also transparently supports.
 
 Validator Showcase
 ~~~~~~~~~~~~~~~~~~
 
-Let's unbox beartype validators with a sleazy slo-mo click-bait YouTube video.
+Observe the disturbing (yet alluring) utility of beartype validators in action
+as they unshackle type hints from the fetters of PEP compliance. Begone,
+foulest standards!
+
+Type Hint Connectives
++++++++++++++++++++++
+
+    **Subtitle:** *From Set Theory They Shall Grow*
+
+`PEP 484`_ standardized the typing.Union_ factory `disjunctively
+<disjunction_>`__ matching any of several equally permissible type hints ala
+Python's builtin ``or`` operator or the overloaded ``|`` operator for sets.
+That's great, because set theory is the beating heart behind type theory.
+
+But that's just disjunction_. What about intersection_ (e.g., ``and``, ``&``),
+`complementation <relative set complement_>`__ (e.g., ``not``, ``~``), or any
+of the vast multitude of *other* set theoretic operations? Can we logically
+connect simple type hints validating trivial constraints into complex type
+hints validating non-trivial constraints via PEP-standardized analogues of
+unary and binary operators?
+
+**Nope.** They don't exist yet. But that's okay. You use beartype, which means
+you don't have to wait for official Python developers to get there first.
+You're already there. :superscript:`...woah`
+
+Type Hint Elision
+^^^^^^^^^^^^^^^^^
+
+Python's core type hierarchy conceals an ugly history of secretive backward
+compatibility. In this subsection, we uncover the two filthiest, flea-infested,
+backwater corners of the otherwise well-lit atrium that is the Python language
+– and how exactly you can finalize them. Both obstruct type-checking, readable
+APIs, and quality assurance in the post-Python 2.7 era.
+
+Guido doesn't want you to know. But you want to know, don't you? You are about
+to enter another dimension, a dimension not only of syntax and semantics but of
+shame. A journey into a hideous land of annotation wrangling. Next stop... *the
+Beartype Zone.* Because guess what?
+
+* **Booleans are integers.** They shouldn't be. Booleans aren't integers in
+  most high-level languages. Wait. Are you telling me booleans are
+  literally integers in Python? Surely you jest. That can't be. You can't *add*
+  booleans, can you? What would that even mean if you could? Observe and cower,
+  rigorous data engineers.
+
+  .. code-block:: python
+
+     >>> True + 3.1415
+     4.141500000000001    # <-- oh. by. god.
+     >>> isinstance(False, int)
+     True                 # <-- when nothing is true, everything is true
+
+* **Strings are infinitely recursive sequences of...** yup, it's strings. They
+  shouldn't be. Strings aren't infinitely recursive data structures in any
+  other language devised by incautious mortals – high-level or not. Wait. Are
+  you telling me strings are both indistinguishable from full-blown immutable
+  sequences containing arbitrary items *and* infinitely recurse into themselves
+  like that sickening non-Euclidean Hall of Mirrors I puked all over when I was
+  a kid? Surely you kid. That can't be. You can't infinitely index into strings
+  *and* pass and return the results to and from callables expecting either
+  ``Sequence[Any]`` or ``Sequence[str]`` type hints, can you? Witness and
+  tremble, stricter-than-thou QA evangelists.
+
+  .. code-block:: python
+
+     >>> 'yougottabekiddi—'[0][0][0][0][0][0][0][0][0][0][0][0][0][0][0]
+     'y'                 # <-- pretty sure we just broke the world
+     >>> from collections.abc import Sequence
+     >>> isinstance("Ph'nglui mglw'nafh Cthu—"[0][0][0][0][0], Sequence)
+     True                # <-- ...curse you, curse you to heck and back
+
+When we annotate a callable as accepting an ``int``, we *never* want that
+callable to also silently accept a ``bool``. Likewise, when we annotate another
+callable as accepting a ``Sequence[Any]`` or ``Sequence[str]``, we *never* want
+that callable to also silently accept a ``str``. These are sensible
+expectations – just not in Python, where madness prevails.
+
+To resolve these counter-intuitive concerns, we need the equivalent of the
+`relative set complement (or difference) <relative set complement_>`__. We now
+call this thing... **type elision!** Sounds pretty hot, right? We know.
+
+Let's first validate **non-boolean integers** with a beartype validator
+effectively declaring a new ``int - bool`` class (i.e., the subclass of all
+integers that are *not* booleans):
+
+.. code-block:: python
+
+   # Import the requisite machinery.
+   from beartype import beartype
+   from beartype.vale import Is
+   from typing import Annotated   # <--------------- if Python ≥ 3.9.0
+   #from typing_extensions import Annotated   # <--- if Python < 3.9.0
+
+   # Type hint matching any non-boolean integer. This day all errata die.
+   IntNonbool = Annotated[int, Is[
+       lambda number: not isinstance(number, bool)]]
+
+   # Type-check a list of non-boolean integers summing to a non-boolean
+   # integer. Beartype wills it. So it shall be.
+   @beartype
+   def sum_intlist(my_list: list[IntNonbool]) -> IntNonbool:
+       '''
+       I cast thee out, mangy booleans!
+
+       You plague these shores no more.
+       '''
+
+       return sum(my_list)
+
+Let's next validate **non-string sequences** with beartype validators
+effectively declaring a new ``Sequence - str`` class (i.e., the subclass of all
+sequences that are *not* strings):
+
+.. code-block:: python
+
+   # Import the requisite machinery.
+   from beartype import beartype
+   from beartype.vale import Is
+   from collections.abc import Sequence
+   from typing import Annotated   # <--------------- if Python ≥ 3.9.0
+   #from typing_extensions import Annotated   # <--- if Python < 3.9.0
+
+   # Type hint matching any non-string sequence. Your day has finally come.
+   SequenceNonstr = Annotated[Sequence, Is[
+       lambda sequence: not isinstance(sequence, str)]]
+
+   # Type hint matching any non-string sequence *WHOSE ITEMS ARE ALL STRINGS.*
+   SequenceNonstrOfStr = Annotated[Sequence[str], Is[
+       lambda sequence: not isinstance(sequence, str)]]
+
+   # Type-check a non-string sequence of arbitrary items coerced into strings
+   # and then joined on newline to a new string. (Beartype got your back, bro.)
+   @beartype
+   def join_objects(my_sequence: SequenceNonstr) -> str:
+       '''
+       Your tide of disease ends here, "str" class!
+       '''
+
+       return '\n'.join(map(str, my_sequence))  # <-- no idea how that works
+
+   # Type-check a non-string sequence whose items are all strings joined on
+   # newline to a new string. It isn't much, but it's all you ask.
+   @beartype
+   def join_strs(my_sequence: SequenceNonstrOfStr) -> str:
+       '''
+       I expectorate thee up, sequence of strings.
+       '''
+
+       return '\n'.join(my_sequence)  # <-- do *NOT* do this to a string
+
+Full-Fat O(n) Matching
+++++++++++++++++++++++
+
+Let's validate **all integers in a list of integers in O(n) time**, because
+validators mean you no longer have to accept the QA scraps we feed you:
+
+.. code-block:: python
 
-:superscript:`Just kidding! It's just real-world industrial-strength examples.`
+   # Import the requisite machinery.
+   from beartype import beartype
+   from beartype.vale import Is
+   from typing import Annotated   # <--------------- if Python ≥ 3.9.0
+   #from typing_extensions import Annotated   # <--- if Python < 3.9.0
+
+   # Type hint matching all integers in a list of integers in O(n) time. Please
+   # never do this. You now want to, don't you? Why? You know the price! Why?!?
+   IntList = Annotated[list[int], Is[lambda lst: all(
+       isinstance(item, int) for item in lst)]]
+
+   # Type-check all integers in a list of integers in O(n) time. How could you?
+   @beartype
+   def sum_intlist(my_list: IntList) -> int:
+       '''
+       The slowest possible integer summation over the passed list of integers.
+
+       There goes your whole data science pipeline. Yikes! So much cringe.
+       '''
+
+       return sum(my_list)  # oh, gods what have you done
+
+Welcome to **full-fat type-checking.** In `our disastrous roadmap to beartype
+1.0.0 <beartype 1.0.0_>`__, we reluctantly admit that we'd like to augment the
+``@beartype`` decorator with a new parameter enabling full-fat type-checking.
+But don't wait on us. Force the issue now by just doing it yourself and then
+mocking us all over Gitter! *Fight the bear, man.*
+
+There are good reasons to believe that `O(1) type-checking is preferable <What
+does beartype do?_>`__. Violating that core precept exposes your codebase to
+scalability and security concerns. But you're the Big Boss, you swear you know
+best, and (in any case) we can't stop you because we already let the unneutered
+tomcat out of his trash bin by `publishing this API into the badlands of PyPI
+<beartype PyPI_>`__.
 
 Tensor Property Matching
 ++++++++++++++++++++++++
 
 Let's validate `the same two-dimensional NumPy array of floats of arbitrary
 precision as in the lead example above <Beartype Validators_>`__ with an
 efficient declarative validator avoiding the additional stack frame imposed by
@@ -1295,57 +1492,14 @@
        '''
        Strip the suffixing character from a string that is lengthy and/or a
        quoted sentence, because your web app deserves only the best data.
        '''
 
        return text[:-1]  # this is frankly outrageous
 
-Full-Fat O(n) Matching
-++++++++++++++++++++++
-
-Let's validate **all integers in a list of integers in O(n) time**, because
-validators mean you no longer have to accept the QA scraps we feed you:
-
-.. code-block:: python
-
-   # Import the requisite machinery.
-   from beartype import beartype
-   from beartype.vale import Is
-   from typing import Annotated   # <--------------- if Python ≥ 3.9.0
-   #from typing_extensions import Annotated   # <--- if Python < 3.9.0
-
-   # Type hint matching all integers in a list of integers in O(n) time. Please
-   # never do this. You now want to, don't you? Why? You know the price! Why?!?
-   IntList = Annotated[list[int], Is[lambda lst: all(
-       isinstance(item, int) for item in lst)]]
-
-   # Type-check all integers in a list of integers in O(n) time. How could you?
-   @beartype
-   def sum_intlist(my_list: IntList) -> int:
-       '''
-       The slowest possible integer summation over the passed list of integers.
-
-       There goes your whole data science pipeline. Yikes! So much cringe.
-       '''
-
-       return sum(my_list)  # oh, gods what have you done
-
-Welcome to **full-fat type-checking.** In `our disastrous roadmap to beartype
-1.0.0 <beartype 1.0.0_>`__, we reluctantly admit that we'd like to augment the
-``@beartype`` decorator with a new parameter enabling full-fat type-checking.
-But don't wait on us. Force the issue now by just doing it yourself and then
-mocking us all over Gitter! *Fight the bear, man.*
-
-There are good reasons to believe that `O(1) type-checking is preferable <What
-does beartype do?_>`__. Violating that core precept exposes your codebase to
-scalability and security concerns. But you're the Big Boss, you swear you know
-best, and (in any case) we can't stop you because we already let the unneutered
-tomcat out of his trash bin by `publishing this API into the badlands of PyPI
-<beartype PyPI_>`__.
-
 Validator Alternatives
 ~~~~~~~~~~~~~~~~~~~~~~
 
 If the unbridled power of beartype validators leaves you variously queasy,
 uneasy, and suspicious of our core worldview, beartype also supports
 third-party type hints like `typed NumPy arrays <NumPy Type Hints_>`__.
 
@@ -2242,14 +2396,16 @@
 +--------------------+-----------------------------------------+-------------------------------+---------------------------+
 |                    | `612 <PEP 612_>`__                      | *none*                        | *none*                    |
 +--------------------+-----------------------------------------+-------------------------------+---------------------------+
 |                    | `647 <PEP 647_>`__                      | *none*                        | *none*                    |
 +--------------------+-----------------------------------------+-------------------------------+---------------------------+
 |                    | `3119 <PEP 3119_>`__                    | **0.7.0**\ —\ *current*       | **0.9.0**\ —\ *current*   |
 +--------------------+-----------------------------------------+-------------------------------+---------------------------+
+|                    | `3141 <PEP 3141_>`__                    | **0.1.0**\ —\ *current*       | **0.1.0**\ —\ *current*   |
++--------------------+-----------------------------------------+-------------------------------+---------------------------+
 | packages           | `PyPI <beartype PyPI_>`__               | **0.1.0**\ —\ *current*       | —                         |
 +--------------------+-----------------------------------------+-------------------------------+---------------------------+
 |                    | `Anaconda <beartype Anaconda_>`__       | **0.1.0**\ —\ *current*       | —                         |
 +--------------------+-----------------------------------------+-------------------------------+---------------------------+
 |                    | `Gentoo Linux <beartype Gentoo_>`__     | **0.2.0**\ —\ *current*       | —                         |
 +--------------------+-----------------------------------------+-------------------------------+---------------------------+
 |                    | `macOS Homebrew <beartype Homebrew_>`__ | **0.5.1**\ —\ *current*       | —                         |
@@ -2264,14 +2420,16 @@
 +--------------------+-----------------------------------------+-------------------------------+---------------------------+
 |                    | 3.8                                     | **0.1.0**\ —\ *current*       | —                         |
 +--------------------+-----------------------------------------+-------------------------------+---------------------------+
 |                    | 3.9                                     | **0.3.2**\ —\ *current*       | —                         |
 +--------------------+-----------------------------------------+-------------------------------+---------------------------+
 |                    | 3.10                                    | **0.7.0**\ —\ *current*       | —                         |
 +--------------------+-----------------------------------------+-------------------------------+---------------------------+
+|                    | 3.11                                    | *none*                        | *none*                    |
++--------------------+-----------------------------------------+-------------------------------+---------------------------+
 
 Timings
 =======
 
 Let's profile ``beartype`` against other runtime type-checkers with `a battery
 of surely fair, impartial, and unbiased use cases <beartype profiler_>`__:
 
@@ -2585,14 +2743,15 @@
 * `PEP 572 -- Assignment Expressions <PEP 572_>`__.
 * `PEP 585 -- Type Hinting Generics In Standard Collections <PEP 585_>`__.
 * `PEP 586 -- Literal Types <PEP 586_>`__.
 * `PEP 589 -- TypedDict: Type Hints for Dictionaries with a Fixed Set of Keys
   <PEP 589_>`__, subject to `caveats detailed below <Partial Compliance_>`__
 * `PEP 593 -- Flexible function and variable annotations <PEP 593_>`__.
 * `PEP 604 -- Allow writing union types as X | Y <PEP 604_>`__.
+* `PEP 3141 -- A Type Hierarchy for Numbers <PEP 3141_>`__.
 
 Beartype is currently *not* compliant whatsoever with these PEPs:
 
 * `PEP 526 -- Syntax for Variable Annotations <PEP 526_>`__.
 * `PEP 591 -- Adding a final qualifier to typing <PEP 591_>`__.
 * `PEP 612 -- Parameter Specification Variables <PEP 612_>`__.
 
@@ -4105,14 +4264,28 @@
 .. |codecov-badge| image:: https://codecov.io/gh/beartype/beartype/branch/main/graph/badge.svg?token=E6F4YSY9ZQ
    :target: https://codecov.io/gh/beartype/beartype
    :alt: beartype test coverage status
 .. |rtd-badge| image:: https://readthedocs.org/projects/beartype/badge/?version=latest
    :target: https://beartype.readthedocs.io/en/latest/?badge=latest
    :alt: beartype Read The Docs (RTD) status
 
+.. # ------------------( IMAGES ~ downstream                )------------------
+.. |icon-graspologic| image:: https://user-images.githubusercontent.com/217028/138580730-dcb3ee22-6372-4a2d-93bf-d1a3c97e67cf.png
+   :target: https://github.com/microsoft/graspologic
+   :alt: Graspologic: Python package for graph statistical algorithms
+.. |icon-hydrazen| image:: https://user-images.githubusercontent.com/217028/139522423-d987d484-425b-4e70-a0e7-7390593471f1.png
+   :target: https://github.com/mit-ll-responsible-ai/hydra-zen
+   :alt: Hydra-Zen: Reproducible Pythonic CLI<->config APIs via Hydra
+.. |icon-pycrisp| image:: https://user-images.githubusercontent.com/217028/138580797-1f09f0b4-bced-4651-82c9-6dae50afe883.png
+   :target: https://gitlab.com/pycrisp/pycrisp
+   :alt: PyCrisp: Typed Python interactions with the Crisp API
+.. |icon-sentipy| image:: https://user-images.githubusercontent.com/217028/138581059-6e3218d0-2a2e-42b7-b15c-7e2759fa2399.png
+   :target: https://github.com/sentimentinvestor/sentipy
+   :alt: SentiPy: Typed Python interactions with the Sentiment Investor API
+
 .. # ------------------( LINKS ~ beartype : funding         )------------------
 .. _BETSE:
    https://gitlab.com/betse/betse
 .. _BETSEE:
    https://gitlab.com/betse/betsee
 .. _Paul Allen:
    https://en.wikipedia.org/wiki/Paul_Allen
@@ -4263,14 +4436,26 @@
    https://en.wikipedia.org/wiki/Shere_Khan
 
 .. # ------------------( LINKS ~ math                       )------------------
 .. _Euler–Mascheroni constant:
    https://en.wikipedia.org/wiki/Euler%E2%80%93Mascheroni_constant
 .. _coupon collector's problem:
    https://en.wikipedia.org/wiki/Coupon_collector%27s_problem
+
+.. # ------------------( LINKS ~ math : set                 )------------------
+.. _conjunction:
+   https://en.wikipedia.org/wiki/Logical_conjunction
+.. _disjunction:
+   https://en.wikipedia.org/wiki/Logical_disjunction
+.. _intersection:
+   https://en.wikipedia.org/wiki/Intersection_(set_theory)
+.. _relative set complement:
+   https://en.wikipedia.org/wiki/Complement_(set_theory)#Relative_complement
+
+.. # ------------------( LINKS ~ math : type                )------------------
 .. _covariance:
    https://en.wikipedia.org/wiki/Covariance_and_contravariance_(computer_science)
 
 .. # ------------------( LINKS ~ meme                       )------------------
 .. _RNGesus:
    https://knowyourmeme.com/memes/rngesus
 .. _goes up to eleven:
```

### Comparing `beartype-0.9.0/beartype.egg-info/SOURCES.txt` & `beartype-0.9.1/beartype.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -86,14 +86,18 @@
 beartype/_util/func/utilfunccodeobj.py
 beartype/_util/func/utilfuncfile.py
 beartype/_util/func/utilfuncmake.py
 beartype/_util/func/utilfuncscope.py
 beartype/_util/func/utilfuncstack.py
 beartype/_util/func/utilfunctest.py
 beartype/_util/func/utilfuncwrap.py
+beartype/_util/func/lib/__init__.py
+beartype/_util/func/lib/utilbeartypefunc.py
+beartype/_util/func/pep/__init__.py
+beartype/_util/func/pep/utilpep484func.py
 beartype/_util/hint/__init__.py
 beartype/_util/hint/utilhintconv.py
 beartype/_util/hint/utilhintget.py
 beartype/_util/hint/utilhinttest.py
 beartype/_util/hint/nonpep/__init__.py
 beartype/_util/hint/nonpep/utilnonpeptest.py
 beartype/_util/hint/pep/__init__.py
@@ -125,14 +129,16 @@
 beartype/_util/kind/__init__.py
 beartype/_util/kind/utilkinddict.py
 beartype/_util/mod/__init__.py
 beartype/_util/mod/utilmoddeprecate.py
 beartype/_util/mod/utilmodimport.py
 beartype/_util/mod/utilmodtest.py
 beartype/_util/mod/utilmodule.py
+beartype/_util/mod/lib/__init__.py
+beartype/_util/mod/lib/utilsphinx.py
 beartype/_util/os/__init__.py
 beartype/_util/os/utilostest.py
 beartype/_util/py/__init__.py
 beartype/_util/py/utilpyinterpreter.py
 beartype/_util/py/utilpyversion.py
 beartype/_util/py/utilpyword.py
 beartype/_util/text/__init__.py
@@ -180,20 +186,23 @@
 beartype_test/a00_unit/a00_util/cls/pep/__init__.py
 beartype_test/a00_unit/a00_util/cls/pep/test_utilpep3119.py
 beartype_test/a00_unit/a00_util/func/__init__.py
 beartype_test/a00_unit/a00_util/func/test_utilfuncarg.py
 beartype_test/a00_unit/a00_util/func/test_utilfunccode.py
 beartype_test/a00_unit/a00_util/func/test_utilfunccodeobj.py
 beartype_test/a00_unit/a00_util/func/test_utilfuncfile.py
-beartype_test/a00_unit/a00_util/func/test_utilfuncget.py
 beartype_test/a00_unit/a00_util/func/test_utilfuncmake.py
 beartype_test/a00_unit/a00_util/func/test_utilfuncscope.py
 beartype_test/a00_unit/a00_util/func/test_utilfuncstack.py
 beartype_test/a00_unit/a00_util/func/test_utilfunctest.py
 beartype_test/a00_unit/a00_util/func/test_utilfuncwrap.py
+beartype_test/a00_unit/a00_util/func/lib/__init__.py
+beartype_test/a00_unit/a00_util/func/lib/test_utilbeartypefunc.py
+beartype_test/a00_unit/a00_util/func/pep/__init__.py
+beartype_test/a00_unit/a00_util/func/pep/test_utilpep484func.py
 beartype_test/a00_unit/a00_util/hint/__init__.py
 beartype_test/a00_unit/a00_util/hint/a00_pep/__init__.py
 beartype_test/a00_unit/a00_util/hint/a00_pep/test_a00_utilpepget.py
 beartype_test/a00_unit/a00_util/hint/a00_pep/test_a90_utilpeptest.py
 beartype_test/a00_unit/a00_util/hint/a00_pep/proposal/__init__.py
 beartype_test/a00_unit/a00_util/hint/a00_pep/proposal/test_utilpep586.py
 beartype_test/a00_unit/a00_util/hint/a00_pep/proposal/test_utilpep593.py
@@ -293,16 +302,27 @@
 beartype_test/a00_unit/data/util/func/__init__.py
 beartype_test/a00_unit/data/util/func/data_utilfunccode.py
 beartype_test/a00_unit/data/util/mod/__init__.py
 beartype_test/a00_unit/data/util/mod/data_utilmodule_bad.py
 beartype_test/a00_unit/data/util/mod/data_utilmodule_good.py
 beartype_test/a90_func/README.rst
 beartype_test/a90_func/__init__.py
+beartype_test/a90_func/data/__init__.py
+beartype_test/a90_func/data/lib/__init__.py
+beartype_test/a90_func/data/lib/sphinx/Makefile
+beartype_test/a90_func/data/lib/sphinx/beartype_sphinx.py
+beartype_test/a90_func/data/lib/sphinx/conf.py
+beartype_test/a90_func/data/lib/sphinx/index.rst
+beartype_test/a90_func/data/lib/sphinx/_build/.gitkeep
+beartype_test/a90_func/data/lib/sphinx/_static/.gitkeep
+beartype_test/a90_func/data/lib/sphinx/_templates/.gitkeep
 beartype_test/a90_func/doc/__init__.py
 beartype_test/a90_func/doc/test_docreadme.py
+beartype_test/a90_func/lib/__init__.py
+beartype_test/a90_func/lib/test_sphinx.py
 beartype_test/a90_func/pep/__init__.py
 beartype_test/a90_func/pep/test_pep561_static.py
 beartype_test/util/README.rst
 beartype_test/util/__init__.py
 beartype_test/util/pytcontext.py
 beartype_test/util/pytroar.py
 beartype_test/util/fixture/__init__.py
@@ -312,15 +332,17 @@
 beartype_test/util/mod/__init__.py
 beartype_test/util/mod/pytmodimport.py
 beartype_test/util/mod/pytmodtest.py
 beartype_test/util/os/__init__.py
 beartype_test/util/os/command/__init__.py
 beartype_test/util/os/command/pytcmdexit.py
 beartype_test/util/path/__init__.py
-beartype_test/util/path/pytpathproject.py
+beartype_test/util/path/pytpathlib.py
+beartype_test/util/path/pytpathmain.py
+beartype_test/util/path/pytpathtest.py
 doc/Makefile
 doc/RELEASE.rst
 doc/make.bat
 doc/source/404.rst
 doc/source/changes.rst
 doc/source/conf.py
 doc/source/index.rst
```

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/cache/map/test_utilmapbig.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/cache/map/test_utilmapbig.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/cache/map/test_utilmaplru.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/cache/map/test_utilmaplru.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/cache/pool/test_utilcachepool.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/cache/pool/test_utilcachepool.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/cache/pool/test_utilcachepoollistfixed.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/cache/pool/test_utilcachepoollistfixed.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/cache/pool/test_utilcachepoolobjecttyped.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/cache/pool/test_utilcachepoolobjecttyped.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/cache/test_utilcachecall.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/cache/test_utilcachecall.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/cache/test_utilcacheerror.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/cache/test_utilcacheerror.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/cls/pep/test_utilpep3119.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/cls/pep/test_utilpep3119.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/cls/test_utilclstest.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/cls/test_utilclstest.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/func/test_utilfuncarg.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/func/test_utilfuncarg.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/func/test_utilfunccode.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/func/test_utilfunccode.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/func/test_utilfunccodeobj.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/func/test_utilfunccodeobj.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/func/test_utilfuncfile.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/func/test_utilfuncfile.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/func/test_utilfuncget.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/py/test_utilpyinterpreter.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 #!/usr/bin/env python3
 # --------------------( LICENSE                           )--------------------
 # Copyright (c) 2014-2021 Beartype authors.
 # See "LICENSE" for further details.
 
 '''
-**Callable utility getter unit tests.**
+Project-wide **Python interpreter** unit tests.
 
 This submodule unit tests the public API of the private
-:mod:`beartype._util.utilfunc.utilfuncget` submodule.
+:mod:`beartype._util.py.utilpyinterpreter` submodule.
 '''
 
 # ....................{ IMPORTS                           }....................
 #!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 # WARNING: To raise human-readable test errors, avoid importing from
 # package-specific submodules at module scope.
 #!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
-from pytest import raises
 
-# ....................{ TESTS                             }....................
+# ....................{ TESTS ~ tester                    }....................
+def test_is_py_pypy() -> None:
+    '''
+    Test the :func:`beartype._util.py.utilpyinterpreter.is_py_pypy` tester.
+    '''
+
+    # Defer heavyweight imports.
+    from beartype._util.py.utilpyinterpreter import is_py_pypy
+
+    # Assert this tester returns a boolean.
+    IS_PY_PYPY = is_py_pypy()
+    assert isinstance(IS_PY_PYPY, bool)
```

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/func/test_utilfuncmake.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/func/test_utilfuncmake.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/func/test_utilfuncscope.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/func/test_utilfuncscope.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     # Return this nested callable.
     return when_the_trees_are_crowned_with_leaves
 
 # ....................{ TESTS ~ tester                    }....................
 def test_is_func_nested() -> None:
     '''
     Test the
-    :func:`beartype._util.func.utilfuncscope.is_func_nested` function.
+    :func:`beartype._util.func.utilfuncscope.is_func_nested` tester.
     '''
 
     # Defer heavyweight imports.
     from beartype._util.func.utilfuncscope import is_func_nested
 
     # Nested callable returned by the above callable.
     when_the_ash_and_oak_and_the_birch_and_yew = (
```

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/func/test_utilfuncstack.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/func/test_utilfuncstack.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/func/test_utilfunctest.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/func/test_utilfunctest.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/func/test_utilfuncwrap.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/func/test_utilfuncwrap.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/hint/a00_pep/proposal/pep484/test_utilpep484typevar.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/hint/a00_pep/proposal/pep484/test_utilpep484typevar.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/hint/a00_pep/proposal/pep484585/test_utilpepgeneric.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/hint/a00_pep/proposal/pep484585/test_utilpepgeneric.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/hint/a00_pep/proposal/pep484585/test_utilpepsubclass.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/hint/a00_pep/proposal/pep484585/test_utilpepsubclass.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/hint/a00_pep/proposal/test_utilpep586.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/hint/a00_pep/proposal/test_utilpep586.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/hint/a00_pep/proposal/test_utilpep593.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/hint/a00_pep/proposal/test_utilpep593.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/hint/a00_pep/test_a00_utilpepget.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/hint/a00_pep/test_a00_utilpepget.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/hint/a00_pep/test_a90_utilpeptest.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/hint/a00_pep/test_a90_utilpeptest.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/hint/a10_nonpep/test_utilhintnonpeptest.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/hint/a10_nonpep/test_utilhintnonpeptest.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/hint/a90_core/test_a00_utilhinttest.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/hint/a90_core/test_a00_utilhinttest.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/hint/a90_core/test_a50_utilhintconv.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/hint/a90_core/test_a50_utilhintconv.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/kind/test_utilkinddict.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/kind/test_utilkinddict.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/mod/test_utilmoddeprecate.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/mod/test_utilmoddeprecate.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/mod/test_utilmodimport.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/mod/test_utilmodimport.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/mod/test_utilmodtest.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/mod/test_utilmodtest.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/os/test_utilostest.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/os/test_utilostest.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/py/test_utilpyword.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/py/test_utilpyword.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/test_utilobject.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/test_utilobject.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/text/test_utiltextident.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/text/test_utiltextident.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/text/test_utiltextjoin.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/text/test_utiltextjoin.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/text/test_utiltextlabel.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/text/test_utiltextlabel.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/text/test_utiltextmunge.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/text/test_utiltextmunge.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a00_util/text/test_utiltextrepr.py` & `beartype-0.9.1/beartype_test/a00_unit/a00_util/text/test_utiltextrepr.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a10_pep/test_pep484.py` & `beartype-0.9.1/beartype_test/a00_unit/a10_pep/test_pep484.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a10_pep/test_pep484585.py` & `beartype-0.9.1/beartype_test/a00_unit/a90_decor/code/test_codemain.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,229 +1,223 @@
 #!/usr/bin/env python3
 # --------------------( LICENSE                           )--------------------
 # Copyright (c) 2014-2021 Beartype authors.
 # See "LICENSE" for further details.
 
 '''
-Beartype decorator :pep:`484`- and :pep:`585`-compliant type hint unit tests.
+**Beartype decorator type hint code generation unit tests.**
 
 This submodule unit tests the :func:`beartype.beartype` decorator with respect
-to :pep:`484`- and :pep:`585`-compliant type hints.
+to type-checking code dynamically generated by the
+:mod:`beartype._decor._code.codemain` submodule.
 '''
 
 # ....................{ IMPORTS                           }....................
 #!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 # WARNING: To raise human-readable test errors, avoid importing from
 # package-specific submodules at module scope.
 #!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 from beartype.roar import BeartypeDecorHintPep585DeprecationWarning
 from beartype_test.util.mark.pytmark import ignore_warnings
 
-# ....................{ TESTS ~ decor : async             }....................
+# ....................{ TESTS                             }....................
 # Prevent pytest from capturing and displaying all expected non-fatal
 # beartype-specific warnings emitted by the @beartype decorator below. Urgh!
 @ignore_warnings(BeartypeDecorHintPep585DeprecationWarning)
-async def test_decor_async_coroutine() -> None:
+def test_codemain() -> None:
     '''
-    Test decorating coroutines with the :func:`beartype.beartype` decorator.
-    '''
-
-    # Defer heavyweight imports.
-    from asyncio import sleep
-    from beartype import beartype
-    from beartype.roar import BeartypeDecorHintPep484585Exception
-    from beartype._util.py.utilpyversion import IS_PYTHON_AT_LEAST_3_9
-    from beartype_test.util.pytroar import raises_uncached
-    from collections.abc import Coroutine as Pep585Coroutine
-    from typing import Union, Coroutine as Pep484Coroutine
+    Test the :func:`beartype.beartype` decorator with respect to type-checking
+    code dynamically generated by the :mod:`beartype._decor._code.codemain`
+    submodule.
+
+    This unit test effectively acts as a functional test and is thus the core
+    test exercising decorator functionality from the end user perspective --
+    the only perspective that matters in the end. Unsurprisingly, this test is
+    mildly more involved than most. *Whatevah.*
+
+    This test additionally attempts to avoid similar issues to a `prior issue
+    <issue #5_>`__ of this decorator induced by repeated
+    :func:`beartype.beartype` decorations of different callables annotated by
+    one or more of the same PEP-compliant type hints.
 
-    # Decorated coroutine whose return is annotated with an arbitrary
-    # PEP-compliant type hint.
-    @beartype
-    async def control_the_car(
-        said_the: Union[str, int],
-        biggest_greenest_bat: Union[str, float],
-    ) -> Union[str, float]:
-        await sleep(0)
-        return said_the + biggest_greenest_bat
-
-    # Assert awaiting this coroutine returns the expected value.
-    assert await control_the_car(
-        'I saw the big green bat bat a green big eye. ',
-        'Suddenly I knew I had gone too far.') == (
-        'I saw the big green bat bat a green big eye. '
-        'Suddenly I knew I had gone too far.')
-
-    # Decorated coroutine whose return is annotated with a PEP 484-compliant
-    # coroutine type hint.
-    @beartype
-    async def universal_love(
-        said_the: Union[str, int], cactus_person: Union[str, float]) -> (
-        Pep484Coroutine[None, None, Union[str, float]]):
-        await sleep(0)
-        return said_the + cactus_person
-
-    # Assert awaiting this coroutine returns the expected value.
-    assert await universal_love(
-        'The sea was made of strontium; ', 'the beach was made of rye.') == (
-        'The sea was made of strontium; the beach was made of rye.')
-
-    # If the active Python interpreter targets Python >= 3.9 and thus supports
-    # PEP 585...
-    if IS_PYTHON_AT_LEAST_3_9:
-        # Decorated coroutine whose return is annotated with a PEP
-        # 585-compliant coroutine type hint.
-        @beartype
-        async def transcendent_joy(
-            said_the: Union[str, float], big_green_bat: Union[str, int]) -> (
-            Pep585Coroutine[None, None, Union[str, float]]):
-            await sleep(0)
-            return said_the + big_green_bat
-
-        # Assert awaiting this coroutine returns the expected value.
-        assert await transcendent_joy(
-            'A thousand stars of sertraline ',
-            'whirled round quetiapine moons'
-        ) == 'A thousand stars of sertraline whirled round quetiapine moons'
-
-        #FIXME: Assert this decorator raises the expected exception when
-        #decorating an asynchronous callable annotating its return as
-        #"Pep585Coroutine[...]" accepting an invalid number of arguments.
-
-
-# Prevent pytest from capturing and displaying all expected non-fatal
-# beartype-specific warnings emitted by the @beartype decorator below. Hurk!
-@ignore_warnings(BeartypeDecorHintPep585DeprecationWarning)
-async def test_decor_async_generator() -> None:
-    '''
-    Test decorating asynchronous generators with the :func:`beartype.beartype`
-    decorator.
+    .. _issue #5:
+       https://github.com/beartype/beartype/issues/5
     '''
 
     # Defer heavyweight imports.
-    from asyncio import sleep
     from beartype import beartype
-    from beartype.roar import BeartypeDecorHintPep484585Exception
-    from beartype._util.py.utilpyversion import IS_PYTHON_AT_LEAST_3_9
+    from beartype.roar import (
+        BeartypeCallHintPepException,
+        # BeartypeDecorHintPep585DeprecationWarning,
+    )
+    from beartype._util.utilobject import is_object_context_manager
+    from beartype_test.a00_unit.data.hint.util.data_hintmetacls import (
+        HintPithSatisfiedMetadata,
+        HintPithUnsatisfiedMetadata,
+    )
+    from beartype_test.a00_unit.data.hint.nonpep.data_nonpep import (
+        HINTS_NONPEP_META)
+    from beartype_test.a00_unit.data.hint.pep.data_pep import HINTS_PEP_META
     from beartype_test.util.pytroar import raises_uncached
-    from collections.abc import AsyncGenerator as Pep585AsyncGenerator
-    from typing import Union, AsyncGenerator as Pep484AsyncGenerator
+    from re import search
 
-    # Decorated asynchronous generator whose return is annotated with a PEP
-    # 484-compliant asynchronous generator type hint.
-    @beartype
-    async def not_splitting_numbers(
-        said_the: Union[str, int], bigger_greener_bat: Union[str, float]) -> (
-        Pep484AsyncGenerator[Union[str, float], None]):
-        await sleep(0)
-        yield said_the + bigger_greener_bat
-
-    # Assert awaiting this asynchronous generator returns the expected value.
-    # Unlike synchronous generators, asynchronous generators are *NOT* actually
-    # iterators and thus have *NO* clean analogue to the iter() and next()
-    # builtins. The closest approximation is this rather unclean hack:
-    #     await not_splitting_number.__anext__()
-    # See also this relevant StackOvelflow post:
-    #     https://stackoverflow.com/a/42561322/2809027
-    async for not_splitting_number in not_splitting_numbers(
-        'the sand sizzled sharp like cooking oil that hissed and sang and ',
-        'threatened to boil the octahedral dunes.',
-    ):
-        # await sleep(0)
-        assert not_splitting_number == (
-            'the sand sizzled sharp like cooking oil that hissed and sang and '
-            'threatened to boil the octahedral dunes.'
-        )
-
-    # If the active Python interpreter targets Python >= 3.9 and thus supports
-    # PEP 585...
-    if IS_PYTHON_AT_LEAST_3_9:
-        # Decorated asynchronous generator whose return is annotated with a PEP
-        # 585-compliant asynchronous generator type hint.
-        @beartype
-        async def but_joining_mind(
-            said_the: Union[str, float],
-            bigger_greener_bat: Union[str, int],
-        ) -> Pep585AsyncGenerator[Union[str, float], None]:
-            await sleep(0)
-            yield said_the + bigger_greener_bat
-
-        # Assert awaiting this asynchronous generator returns the expected value.
-        async for but_joining_time in but_joining_mind(
-            'A meteorite of pure delight ', 'struck the sea without a sound.'):
-            assert but_joining_time == (
-                'A meteorite of pure delight struck the sea without a sound.')
-
-    # Assert this decorator raises the expected exception when decorating an
-    # asynchronous generator annotating its return as anything *EXCEPT*
-    # "AsyncGenerator[...]".
-    with raises_uncached(BeartypeDecorHintPep484585Exception):
-        @beartype
-        async def upside_down_trees(
-            roots_in_the_breeze: str, branches_underground: str) -> str:
-            await sleep(0)
-            yield roots_in_the_breeze + branches_underground
-
-# ....................{ TESTS ~ decor : sync              }....................
-# Prevent pytest from capturing and displaying all expected non-fatal
-# beartype-specific warnings emitted by the @beartype decorator below. Blargh!
-@ignore_warnings(BeartypeDecorHintPep585DeprecationWarning)
-def test_decor_sync_generator() -> None:
-    '''
-    Test decorating synchronous generators with the :func:`beartype.beartype`
-    decorator.
-    '''
-
-    # Defer heavyweight imports.
-    from beartype import beartype
-    from beartype.roar import BeartypeDecorHintPep484585Exception
-    from beartype._util.py.utilpyversion import IS_PYTHON_AT_LEAST_3_9
-    from beartype_test.util.pytroar import raises_uncached
-    from collections.abc import Generator as Pep585Generator
-    from typing import Union, Generator as Pep484Generator
+    # Tuple of all PEP-compliant type hint metadata to be tested -- regardless
+    # of whether those hints are uniquely identifiable by a sign or not.
+    HINTS_META = HINTS_PEP_META + HINTS_NONPEP_META
+
+    # Tuple of two arbitrary values used to trivially iterate twice below.
+    RANGE_2 = (None, None)
+
+    # For each predefined PEP-compliant type hint and associated metadata...
+    for hint_meta in HINTS_META:
+        # print(f'Type-checking PEP type hint {repr(hint_meta.hint)}...')
+
+        # If this hint is currently unsupported, continue to the next.
+        if not hint_meta.is_supported:
+            continue
+        # Else, this hint is currently supported.
+
+        # Repeat the following logic twice. Why? To exercise memoization across
+        # repeated @beartype decorations on different callables annotated by
+        # the same PEP hints.
+        for _ in RANGE_2:
+            # Undecorated callable both accepting a single parameter and
+            # returning a value annotated by this hint whose implementation
+            # trivially reduces to the identity function.
+            def func_untyped(hint_param: hint_meta.hint) -> hint_meta.hint:
+                return hint_param
+
+            # Decorated callable declared below.
+            func_typed = None
+
+            #FIXME: For unknown and probably uninteresting reasons, the
+            #pytest.warns() context manager appears to be broken on our
+            #local machine. We have no recourse but to unconditionally
+            #ignore this warning at the module level. So much rage!
+            #FIXME: It's likely this has something to do with the fact that
+            #Python filters deprecation warnings by default. This is almost
+            #certainly a pytest issue. Since this has become fairly
+            #unctuous, we should probably submit a pytest issue report.
+            #FIXME: Actually, pytest now appears to have explicit support for
+            #testing that a code block emits a deprecation warning:
+            #    with pytest.deprecated_call():
+            #        myfunction(17)
+            #See also: https://docs.pytest.org/en/6.2.x/warnings.html#ensuring-code-triggers-a-deprecation-warning
+
+            # # If this is a deprecated PEP-compliant type hint, declare this
+            # # decorated callable under a context manager asserting this
+            # # declaration to emit non-fatal deprecation warnings.
+            # if (
+            #     isinstance(hint_meta, HintPepMetadata) and
+            #     hint_meta.pep_sign in HINT_PEP_ATTRS_DEPRECATED
+            # ):
+            #     with pytest.warns(BeartypeDecorHintPep585DeprecationWarning):
+            #         func_typed = beartype(func_untyped)
+            # # Else, this is *NOT* a deprecated PEP-compliant type hint. In this
+            # # case, declare this decorated callable as is.
+            # else:
+            #     func_typed = beartype(func_untyped)
+
+            # @beartype-generated wrapper function type-checking this callable.
+            func_typed = beartype(func_untyped)
+
+            # For each pith satisfying this hint...
+            for pith_satisfied_meta in hint_meta.piths_satisfied_meta:
+                # Assert this metadata is an instance of the desired dataclass.
+                assert isinstance(
+                    pith_satisfied_meta, HintPithSatisfiedMetadata)
+
+                # Pith to be type-checked against this hint, defined as...
+                pith = (
+                    # If this pith is actually a pith factory (i.e., callable
+                    # accepting *NO* parameters and dynamically creating and
+                    # returning the value to be used as the desired pith), call
+                    # this factory and localize its return value.
+                    pith_satisfied_meta.pith()
+                    if pith_satisfied_meta.is_pith_factory else
+                    # Else, localize this pith as is.
+                    pith_satisfied_meta.pith
+                )
+                # print(f'Type-checking PEP type hint {repr(hint_meta.hint)} against {repr(pith)}...')
+
+                # If...
+                if (
+                    # This pith is a context manager *AND*...
+                    is_object_context_manager(pith) and
+                    # This pith should be safely opened and closed as a
+                    # context rather than preserved as a context manager...
+                    not pith_satisfied_meta.is_context_manager
+                # Then with this pith safely opened and closed as a context...
+                ):
+                    with pith as pith_context:
+                        # Assert this wrapper function successfully type-checks
+                        # this context against this hint *WITHOUT* modifying
+                        # this context.
+                        assert func_typed(pith_context) is pith_context
+                # Else, this object is *NOT* a context manager and thus safely
+                # passable and returnable as is.
+                else:
+                    # Assert this wrapper function successfully type-checks
+                    # this object against this hint *WITHOUT* modifying this
+                    # object.
+                    assert func_typed(pith) is pith
+
+            # For each pith *NOT* satisfying this hint...
+            for pith_unsatisfied_meta in hint_meta.piths_unsatisfied_meta:
+                # Assert this metadata is an instance of the desired dataclass.
+                assert isinstance(
+                    pith_unsatisfied_meta, HintPithUnsatisfiedMetadata)
+
+                # Assert that iterables of uncompiled regular expression
+                # expected to match and *NOT* match this message are *NOT*
+                # strings, as commonly occurs when accidentally omitting a
+                # trailing comma in tuples containing only one string: e.g.,
+                # * "('This is a tuple, yo.',)" is a 1-tuple containing one
+                #   string.
+                # * "('This is a string, bro.')" is a string *NOT* contained in
+                #   a 1-tuple.
+                assert not isinstance(
+                    pith_unsatisfied_meta.exception_str_match_regexes, str)
+                assert not isinstance(
+                    pith_unsatisfied_meta.exception_str_not_match_regexes, str)
+
+                # Assert this wrapper function raises the expected exception
+                # when type-checking this pith against this hint.
+                with raises_uncached(BeartypeCallHintPepException) as (
+                    exception_info):
+                    func_typed(pith_unsatisfied_meta.pith)
+
+                # Exception message raised by this wrapper function.
+                exception_str = str(exception_info.value)
+                # print('exception message: {}'.format(exception_str))
+
+                # Exception type localized for debuggability. Sadly, the
+                # pytest.ExceptionInfo.__repr__() dunder method fails to
+                # usefully describe its exception metadata.
+                exception_type = exception_info.type
+
+                # Assert this exception metadata describes the expected
+                # exception as a sanity check against upstream pytest issues
+                # and/or issues with our raises_uncached() context manager.
+                assert issubclass(exception_type, BeartypeCallHintPepException)
+
+                # For each uncompiled regular expression expected to match this
+                # message, assert this expression actually does so.
+                #
+                # Note that the re.search() rather than re.match() function is
+                # called. The latter is rooted at the start of the string and
+                # thus *ONLY* matches prefixes, while the former is *NOT*
+                # rooted at any string position and thus matches arbitrary
+                # substrings as desired.
+                for exception_str_match_regex in (
+                    pith_unsatisfied_meta.exception_str_match_regexes):
+                    assert search(
+                        exception_str_match_regex, exception_str) is not None
+
+                # For each uncompiled regular expression expected to *NOT*
+                # match this message, assert this expression actually does so.
+                for exception_str_not_match_regex in (
+                    pith_unsatisfied_meta.exception_str_not_match_regexes):
+                    assert search(
+                        exception_str_not_match_regex, exception_str) is None
 
-    # Decorated synchronous generator whose return is annotated with a PEP
-    # 484-compliant synchronous generator type hint.
-    @beartype
-    def not_facts_or_factors_or_factories(
-        said_the: Union[str, int],
-        bigger_greener_bat: Union[str, float],
-    ) -> Pep484Generator[Union[str, float], None, None]:
-        yield said_the + bigger_greener_bat
-
-    # Assert this synchronous generator yields the expected value when
-    # iterated.
-    assert next(not_facts_or_factors_or_factories(
-        'The watery sun began to run ',
-        'and it fell on the ground as rain.',
-    )) == 'The watery sun began to run and it fell on the ground as rain.'
-
-    # If the active Python interpreter targets Python >= 3.9 and thus supports
-    # PEP 585...
-    if IS_PYTHON_AT_LEAST_3_9:
-        # Decorated synchronous generator whose return is annotated with a PEP
-        # 585-compliant synchronous generator type hint.
-        @beartype
-        def contact_with_the_abstract_attractor(
-            said_the: Union[str, float],
-            bigger_greener_bat: Union[str, int],
-        ) -> Pep585Generator[Union[str, float], None, None]:
-            yield said_the + bigger_greener_bat
-
-        # Assert this synchronous generator yields the expected value when
-        # iterated.
-        assert next(contact_with_the_abstract_attractor(
-            'Then tree and beast all fled due east and ',
-            'the moon and stars shot south.',
-        )) == (
-            'Then tree and beast all fled due east and '
-            'the moon and stars shot south.'
-        )
-
-    # Assert this decorator raises the expected exception when decorating a
-    # synchronous generator annotating its return as anything *EXCEPT*
-    # "Generator[...]".
-    with raises_uncached(BeartypeDecorHintPep484585Exception):
-        @beartype
-        def GET_OUT_OF_THE_CAR(
-            FOR_THE_LOVE_OF_GOD: str, FACTOR_THE_NUMBER: str) -> str:
-            yield FOR_THE_LOVE_OF_GOD + FACTOR_THE_NUMBER
+            # assert False is True
```

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a10_pep/test_pep544.py` & `beartype-0.9.1/beartype_test/a00_unit/a10_pep/test_pep544.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a10_pep/test_pep561.py` & `beartype-0.9.1/beartype_test/a00_unit/a10_pep/test_pep561.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     from beartype._util.mod.utilmodule import get_module_filename
     from pathlib import Path
 
     # Concrete platform-agnostic path encapsulating the absolute filename of
     # the "beartype.__init__" submodule.
     #
     # Note that we intentionally do *NOT* obtain this file via the
-    # test-specific "beartype_test._util.path.pytpathproject" submodule. Why?
+    # test-specific "beartype_test._util.path.pytpathmain" submodule. Why?
     # Because we want to test that the "py.typed" file is actually being
     # installed with the "beartype" package, wherever that package may
     # currently be installed (e.g., to a "tox"-isolated venv).
     BEARTYPE_INIT_FILENAME = Path(get_module_filename(beartype))
 
     # Concrete platform-agnostic path encapsulating the absolute dirname of
     # the "beartype" package.
```

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a10_pep/test_pep563.py` & `beartype-0.9.1/beartype_test/a00_unit/a10_pep/test_pep563.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a10_pep/test_pep585.py` & `beartype-0.9.1/beartype_test/a00_unit/a10_pep/test_pep585.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a10_pep/test_pep589.py` & `beartype-0.9.1/beartype_test/a00_unit/a10_pep/test_pep589.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a10_pep/test_pep593.py` & `beartype-0.9.1/beartype_test/a00_unit/a10_pep/test_pep593.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a20_api/test_api_beartype.py` & `beartype-0.9.1/beartype_test/a00_unit/a20_api/test_api_beartype.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a20_api/test_api_cave.py` & `beartype-0.9.1/beartype_test/a00_unit/a20_api/test_api_cave.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a20_api/test_api_meta.py` & `beartype-0.9.1/beartype_test/a00_unit/a20_api/test_api_meta.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a20_api/vale/_factory/test_valeis.py` & `beartype-0.9.1/beartype_test/a00_unit/a20_api/vale/_factory/test_valeis.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a20_api/vale/_factory/test_valeiscls.py` & `beartype-0.9.1/beartype_test/a00_unit/a20_api/vale/_factory/test_valeiscls.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a20_api/vale/_factory/test_valeisobj.py` & `beartype-0.9.1/beartype_test/a00_unit/a20_api/vale/_factory/test_valeisobj.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a20_api/vale/_factory/test_valeisoper.py` & `beartype-0.9.1/beartype_test/a00_unit/a20_api/vale/_factory/test_valeisoper.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a20_api/vale/test_valevale.py` & `beartype-0.9.1/beartype_test/a00_unit/a20_api/vale/test_valevale.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a50_error/test_errormain.py` & `beartype-0.9.1/beartype_test/a00_unit/a50_error/test_errormain.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a90_decor/cache/test_cachetype.py` & `beartype-0.9.1/beartype_test/a00_unit/a90_decor/cache/test_cachetype.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a90_decor/code/nonpep/test_codemypy.py` & `beartype-0.9.1/beartype_test/a00_unit/a90_decor/code/nonpep/test_codemypy.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a90_decor/code/nonpep/test_codenonpep.py` & `beartype-0.9.1/beartype_test/a00_unit/a90_decor/code/nonpep/test_codenonpep.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a90_decor/code/pep/test_codepep.py` & `beartype-0.9.1/beartype_test/a00_unit/a90_decor/code/pep/test_codepep.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a90_decor/code/pep/test_pepscope.py` & `beartype-0.9.1/beartype_test/a00_unit/a90_decor/code/pep/test_pepscope.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a90_decor/code/test_codeforwardref.py` & `beartype-0.9.1/beartype_test/a00_unit/a90_decor/code/test_codeforwardref.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,30 +104,38 @@
     Test unsuccessful decorator-time usage of the :func:`beartype.beartype`
     decorator with respect to both PEP-compliant and -noncompliant forward
     references.
     '''
 
     # Defer heavyweight imports.
     from beartype import beartype
-    from beartype.roar import (
-        BeartypeDecorHintForwardRefException,
-        BeartypeDecorHintPep563Exception,
-    )
-    from beartype._util.py.utilpyversion import IS_PYTHON_AT_LEAST_3_10
+    from beartype.roar import BeartypeDecorHintForwardRefException
+
+    #FIXME: Uncomment if and when a future Python release unconditionally
+    #enables some variant of PEP 563... yet again.
+    # from beartype.roar import (
+    #     BeartypeDecorHintForwardRefException,
+    #     BeartypeDecorHintPep563Exception,
+    # )
+    # from beartype._util.py.utilpyversion import IS_PYTHON_AT_LEAST_3_10
+    #
+    # # Type of exception raised by @beartype when decorating callables annotated
+    # # by syntactically invalid forward reference type hints. Due to ambiguities
+    # # in PEP 563 unconditionally enabled under Python >= 3.10, @beartype is
+    # # unable to reliably differentiate forward references from non-forward
+    # # references and thus treats the former as the latter here.
+    # exception_cls = (
+    #     BeartypeDecorHintPep563Exception
+    #     if IS_PYTHON_AT_LEAST_3_10 else
+    #     BeartypeDecorHintForwardRefException
+    # )
 
     # Type of exception raised by @beartype when decorating callables annotated
-    # by syntactically invalid forward reference type hints. Due to ambiguities
-    # in PEP 563 unconditionally enabled under Python >= 3.10, @beartype is
-    # unable to reliably differentiate forward references from non-forward
-    # references and thus treats the former as the latter here.
-    exception_cls = (
-        BeartypeDecorHintPep563Exception
-        if IS_PYTHON_AT_LEAST_3_10 else
-        BeartypeDecorHintForwardRefException
-    )
+    # by syntactically invalid forward reference type hints.
+    exception_cls = BeartypeDecorHintForwardRefException
 
     # Assert @beartype raises the expected exception when decorating a callable
     # annotated by a syntactically invalid forward reference type hint.
     with raises_uncached(exception_cls):
         @beartype
         def linnets_wings(evening_full: (
             "There midnight’s all a glimmer, and noon a purple glow,")):
```

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a90_decor/code/test_codenoop.py` & `beartype-0.9.1/beartype_test/a00_unit/a90_decor/code/test_codenoop.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a90_decor/test_decor.py` & `beartype-0.9.1/beartype_test/a00_unit/a90_decor/test_decor.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/a90_decor/test_decordata.py` & `beartype-0.9.1/beartype_test/a00_unit/a90_decor/test_decordata.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/data/data_type.py` & `beartype-0.9.1/beartype_test/a00_unit/data/data_type.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/data/hint/data_hint.py` & `beartype-0.9.1/beartype_test/a00_unit/data/hint/data_hint.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/data/hint/data_hintref.py` & `beartype-0.9.1/beartype_test/a00_unit/data/hint/data_hintref.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/data/hint/nonpep/data_nonpep.py` & `beartype-0.9.1/beartype_test/a00_unit/data/hint/nonpep/data_nonpep.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/data/hint/nonpep/mod/_data_nonpepbeartype.py` & `beartype-0.9.1/beartype_test/a00_unit/data/hint/nonpep/proposal/_data_nonpep484.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,148 +1,180 @@
 #!/usr/bin/env python3
 # --------------------( LICENSE                           )--------------------
 # Copyright (c) 2014-2021 Beartype authors.
 # See "LICENSE" for further details.
 
 '''
-**Beartype-specific PEP-noncompliant type hints** (i.e., unofficial type hints
-supported *only* by the :mod:`beartype.beartype` decorator) test data.
+Project-wide :pep:`484`-compliant PEP-noncompliant type hint test data.
 
-These hints include:
+:pep:`484`-compliant type hints *mostly* indistinguishable from
+PEP-noncompliant type hints include:
 
-* **Fake builtin types** (i.e., types that are *not* builtin but which
-  nonetheless erroneously masquerade as being builtin).
-* **Tuple unions** (i.e., tuples containing *only* standard classes and
-  forward references to standard classes).
+* :func:`typing.NamedTuple`, a high-level factory function deferring to the
+  lower-level :func:`collections.namedtuple` factory function creating and
+  returning :class:`tuple` instances annotated by PEP-compliant type hints.
+* :func:`typing.TypedDict`, a high-level factory function creating and
+  returning :class:`dict` instances annotated by PEP-compliant type hints.
 '''
 
 # ....................{ IMPORTS                           }....................
 import sys
-from beartype_test.a00_unit.data.hint.util.data_hintmetacls import (
-    HintNonpepMetadata,
-    HintPithSatisfiedMetadata,
-    HintPithUnsatisfiedMetadata,
-)
 from beartype._cave._cavefast import (
     EllipsisType,
     FunctionType,
     FunctionOrMethodCType,
     MethodBoundInstanceOrClassType,
     ModuleType,
     NoneType,
     NotImplementedType,
 )
+from beartype_test.a00_unit.data.data_type import Class
+from beartype_test.a00_unit.data.hint.util.data_hintmetacls import (
+    HintNonpepMetadata,
+    HintPithSatisfiedMetadata,
+    HintPithUnsatisfiedMetadata,
+)
+from typing import (
+    NamedTuple,
+)
 
-# ....................{ CLASSES                           }....................
-class ThankfulStrumpet(object):
-    '''
-    Arbitrary class.
-    '''
-
-    def empirism_trumpeted(self) -> None:
-        '''
-        Arbitrary method.
-        '''
-
-        pass
+# ....................{ GLOBALS                           }....................
+NamedTupleType = NamedTuple(
+    'NamedTupleType', [('fumarole', str), ('enrolled', int)])
+'''
+PEP-compliant user-defined :func:`collections.namedtuple` instance typed with
+PEP-compliant annotations.
+'''
 
 # ....................{ ADDERS                            }....................
 def add_data(data_module: 'ModuleType') -> None:
     '''
-    Add :mod:`beartype`-specific PEP-noncompliant type hint test data to
-    various global containers declared by the passed module.
+    Add :pep:`484`**-compliant PEP-noncompliant type hint test data to various
+    global containers declared by the passed module.
 
     Parameters
     ----------
     data_module : ModuleType
         Module to be added to.
     '''
 
-    # Arbitrary instance of an arbitrary class.
-    manky_crumpet = ThankfulStrumpet()
-
     # ..................{ TUPLES                            }..................
-    # Add beartype-specific PEP-noncompliant test type hints to this dictionary
+    # Add PEP 484-specific PEP-noncompliant test type hints to this dictionary
     # global.
     data_module.HINTS_NONPEP_META.extend((
-        # ................{ TUPLE UNION                       }................
-        # Beartype-specific tuple unions (i.e., tuples containing one or more
-        # isinstanceable classes).
-
-        # Tuple union of one isinstanceable class.
+        # ................{ NAMEDTUPLE                        }................
+        # "NamedTuple" instances transparently reduce to standard tuples and
+        # *MUST* thus be handled as non-"typing" type hints.
         HintNonpepMetadata(
-            hint=(str,),
+            hint=NamedTupleType,
             piths_satisfied_meta=(
+                # Named tuple containing correctly typed items.
+                HintPithSatisfiedMetadata(
+                    NamedTupleType(fumarole='Leviathan', enrolled=37)),
+            ),
+            piths_unsatisfied_meta=(
                 # String constant.
-                HintPithSatisfiedMetadata('Pinioned coin tokens'),
+                HintPithUnsatisfiedMetadata('Of ͼarthen concordance that'),
+
+                #FIXME: Uncomment after implementing "NamedTuple" support.
+                # # Named tuple containing incorrectly typed items.
+                # HintPithUnsatisfiedMetadata(
+                #     pith=NamedTupleType(fumarole='Leviathan', enrolled=37),
+                #     # Match that the exception message raised for this object...
+                #     exception_str_match_regexes=(
+                #         # Declares the name of this tuple's problematic item.
+                #         r'\s[Ll]ist item 0\s',
+                #     ),
+                # ),
+            ),
+        ),
+
+        # ................{ TYPEDDICT                         }................
+        # "TypedDict" instances transparently reduce to dicts.
+        #FIXME: Implement us up, but note when doing so that:
+        #* We currently unconditionally reduce "TypeDict" to "Mapping".
+        #* "TypedDict" was first introduced with Python 3.8.
+
+        # ................{ TYPE ~ builtin                    }................
+        # Integer.
+        HintNonpepMetadata(
+            hint=int,
+            piths_satisfied_meta=(
+                # Integer constant.
+                HintPithSatisfiedMetadata(42),  # <-- we went there, folks
             ),
             piths_unsatisfied_meta=(
-                # Byte-string constant.
+                # String constant.
                 HintPithUnsatisfiedMetadata(
-                    pith=b'Murkily',
+                    pith='Introspectively ‘allein,’ dealigning consangui-',
                     # Match that the exception message raised for this pith
-                    # declares the types *NOT* satisfied by this object.
+                    # contains...
                     exception_str_match_regexes=(
-                        r'\bstr\b',
+                        # The type *NOT* satisfied by this object.
+                        r'\bint\b',
                     ),
                     # Match that the exception message raised for this pith
-                    # does *NOT* contain a newline or bullet delimiter.
+                    # does *NOT* contain...
                     exception_str_not_match_regexes=(
+                        # A newline.
                         r'\n',
+                        # A bullet delimiter.
                         r'\*',
+                        # Descriptive terms applied only to non-builtin types.
+                        r'\bprotocol\b',
+                        # The double-quoted name of this builtin type.
+                        r'"int"',
                     ),
                 ),
             ),
         ),
 
-        # Tuple union of two or more isinstanceable classes.
+        # Unicode string.
         HintNonpepMetadata(
-            hint=(int, str),
+            hint=str,
             piths_satisfied_meta=(
-                # Integer constant.
-                HintPithSatisfiedMetadata(12),
                 # String constant.
-                HintPithSatisfiedMetadata('Smirk‐opined — openly'),
+                HintPithSatisfiedMetadata('Glassily lassitudinal bȴood-'),
             ),
             piths_unsatisfied_meta=(
                 # Byte-string constant.
                 HintPithUnsatisfiedMetadata(
-                    pith=b'Betokening',
-                    # Match that the exception message raised for this object
-                    # declares the types *NOT* satisfied by this object.
+                    pith=b'Stains, disdain-fully ("...up-stairs!"),',
+                    # Match that the exception message raised for this pith
+                    # contains...
                     exception_str_match_regexes=(
-                        r'\bint\b',
+                        # The type *NOT* satisfied by this object.
                         r'\bstr\b',
+                        # The representation of this object preserved as is.
+                        r'\sb\'Stains, disdain-fully \("...up-stairs!"\),\'\s',
                     ),
-                    # Match that the exception message raised for this object
-                    # does *NOT* contain a newline or bullet delimiter.
+                    # Match that the exception message raised for this pith
+                    # does *NOT* contain...
                     exception_str_not_match_regexes=(
+                        # A newline.
                         r'\n',
+                        # A bullet delimiter.
                         r'\*',
+                        # Descriptive terms applied only to non-builtin types.
+                        r'\bprotocol\b',
+                        # The double-quoted name of this builtin type.
+                        r'"str"',
                     ),
                 ),
-            ),
-        ),
 
-        # ................{ TYPE ~ builtin                    }................
-        # Builtin type.
-        HintNonpepMetadata(
-            hint=str,
-            piths_satisfied_meta=(
-                # String constant.
-                HintPithSatisfiedMetadata('Glassily lassitudinal bȴood-'),
-            ),
-            piths_unsatisfied_meta=(
-                # Byte-string constant.
+                # Integer constant.
                 HintPithUnsatisfiedMetadata(
-                    pith=b'Stains, disdain-fully ("...up-stairs!"),',
+                    pith=666,  # <-- number of the beast, yo
                     # Match that the exception message raised for this pith
-                    # declares the types *NOT* satisfied by this object.
+                    # contains...
                     exception_str_match_regexes=(
+                        # The type *NOT* satisfied by this object.
                         r'\bstr\b',
+                        # The representation of this object preserved as is.
+                        r'\s666\s',
                     ),
                     # Match that the exception message raised for this pith
                     # does *NOT* contain...
                     exception_str_not_match_regexes=(
                         # A newline.
                         r'\n',
                         # A bullet delimiter.
@@ -204,15 +236,15 @@
         ),
 
         # Fake builtin bound method type.
         HintNonpepMetadata(
             hint=MethodBoundInstanceOrClassType,
             piths_satisfied_meta=(
                 # Bound method.
-                HintPithSatisfiedMetadata(manky_crumpet.empirism_trumpeted),
+                HintPithSatisfiedMetadata(Class().instance_method),
             ),
             piths_unsatisfied_meta=(
                 # String constant.
                 HintPithUnsatisfiedMetadata(
                     'ç‐omically gnomical whitebellied burden’s empathy of'),
             ),
         ),
```

### Comparing `beartype-0.9.0/beartype_test/a00_unit/data/hint/pep/data_pep.py` & `beartype-0.9.1/beartype_test/a00_unit/data/hint/pep/data_pep.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/data/hint/pep/mod/_data_hintmodnumpy.py` & `beartype-0.9.1/beartype_test/a00_unit/data/hint/pep/mod/_data_hintmodnumpy.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/data/hint/pep/proposal/_data_pep544.py` & `beartype-0.9.1/beartype_test/a00_unit/data/hint/pep/proposal/_data_pep544.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,15 @@
             pep_sign=HintSignGeneric,
             generic_type=SupportsAbs,
             # Oddly, some but *NOT* all "typing.Supports*" ABCs are
             # parametrized by type variables. *shrug*
             is_typevars=True,
             piths_satisfied_meta=(
                 # Integer constant.
-                HintPithSatisfiedMetadata(73),
+                HintPithSatisfiedMetadata(777),  # <-- what can this mean!?!?!?
             ),
             piths_unsatisfied_meta=(
                 # String constant.
                 HintPithUnsatisfiedMetadata('Scour Our flowering'),
             ),
         ),
```

### Comparing `beartype-0.9.0/beartype_test/a00_unit/data/hint/pep/proposal/_data_pep585.py` & `beartype-0.9.1/beartype_test/a00_unit/data/hint/pep/proposal/_data_pep585.py`

 * *Files 1% similar despite different names*

```diff
@@ -591,26 +591,27 @@
                     'Ously overmoist, ov‐ertly',
                     'Deverginating vertigo‐originating',
                 ]),
             ),
             piths_unsatisfied_meta=(
                 # String constant.
                 HintPithUnsatisfiedMetadata('Devilet‐Sublet cities waxing'),
-                # List containing exactly one integer. Since list items are only
-                # randomly type-checked, only a list of exactly one item enables us
-                # to match the explicit index at fault below.
+                # List containing exactly one integer. Since list items are
+                # only randomly type-checked, only a list of exactly one item
+                # enables us to match the explicit index at fault below.
                 HintPithUnsatisfiedMetadata(
                     pith=[73,],
-                    # Match that the exception message raised for this object...
+                    # Match that the exception message raised for this
+                    # object...
                     exception_str_match_regexes=(
                         # Declares the index of a random list item *NOT*
                         # satisfying this hint.
-                        r'\s[Ll]ist item \d+\s',
-                        # Double-quotes the value of this item.
-                        r'\s"73"\s',
+                        r'\b[Ll]ist index \d+ item\b',
+                        # Preserves the value of this item unquoted.
+                        r'\s73\s',
                     ),
                 ),
             ),
         ),
 
         # Generic list.
         HintPepMetadata(
@@ -831,15 +832,15 @@
             piths_unsatisfied_meta=(
                 # Tuple containing fewer items than required.
                 HintPithUnsatisfiedMetadata(
                     pith=('Obeisance',),
                     # Match that the raised exception message...
                     exception_str_match_regexes=(
                         # Compares this tuple's length to the expected length.
-                        r'\b1 not 2\b',
+                        r'\b1 != 2\b',
                     ),
                 ),
             ),
         ),
 
         # Fixed-length tuple of at least one ignorable child hint.
         HintPepMetadata(
@@ -865,30 +866,30 @@
                     pith=(
                         999.888,
                         'Obese, slipshodly muslin‐shod priests had maudlin solo',
                     ),
                     # Match that the raised exception message...
                     exception_str_match_regexes=(
                         # Compares this tuple's length to the expected length.
-                        r'\b2 not 3\b',
+                        r'\b2 != 3\b',
                     ),
                 ),
                 # Tuple containing a floating-point number, a string, and a
                 # boolean (in that exact order).
                 HintPithUnsatisfiedMetadata(
                     pith=(
                         75.83,
                         'Unwholesome gentry ventings',
                         False,
                     ),
                     # Match that the raised exception message...
                     exception_str_match_regexes=(
                         # Declares the index and expected type of a fixed tuple
                         # item *NOT* satisfying this hint.
-                        r'\s[Tt]uple item 2\s',
+                        r'\b[Tt]uple index 2 item\b',
                         r'\bstr\b',
                     ),
                 ),
             ),
         ),
 
         # Nested fixed-length tuple of at least one ignorable child hint.
@@ -932,15 +933,15 @@
                         ),
                     ),
                     # Match that the raised exception message...
                     exception_str_match_regexes=(
                         # Declares the index and expected type of a random
                         # tuple item of a fixed tuple item *NOT* satisfying
                         # this hint.
-                        r'\s[Tt]uple item \d+ tuple item 2\s',
+                        r'\b[Tt]uple index \d+ item tuple index 2 item\b',
                         r'\bstr\b',
                     ),
                 ),
             ),
         ),
 
         # Generic fixed-length tuple.
@@ -991,15 +992,15 @@
                 # enables us to match the explicit index at fault below.
                 HintPithUnsatisfiedMetadata(
                     pith=((53,)),
                     # Match that the raised exception message...
                     exception_str_match_regexes=(
                         # Declares the index and expected type of this tuple's
                         # problematic item.
-                        r'\s[Tt]uple item 0\s',
+                        r'\b[Tt]uple index 0 item\b',
                         r'\bstr\b',
                     ),
                 ),
             ),
         ),
 
         # Generic variadic tuple.
@@ -1060,23 +1061,24 @@
 
                 # List of bytestring items.
                 HintPithUnsatisfiedMetadata(
                     pith=[
                         b'Blamelessly Slur-chastened rights forthwith, affrighting',
                         b"Beauty's lurid, beleaguered knolls, eland-leagued and",
                     ],
-                    # Match that the exception message raised for this object...
+                    # Match that the exception message raised for this
+                    # object...
                     exception_str_match_regexes=(
                         # Declares all non-"typing" types *NOT* satisfied by a
                         # random list item *NOT* satisfying this hint.
                         r'\bint\b',
                         r'\bstr\b',
                         # Declares the index of the random list item *NOT*
                         # satisfying this hint.
-                        r'\b[Ll]ist item \d+\b',
+                        r'\b[Ll]ist index \d+ item\b',
                     ),
                 ),
             ),
         ),
 
         # Nested union of one non-"typing" type and one "typing" type.
         HintPepMetadata(
@@ -1109,23 +1111,24 @@
                         r'\*',
                     ),
                 ),
 
                 # Sequence of integer items.
                 HintPithUnsatisfiedMetadata(
                     pith=((144, 233, 377, 610, 987, 1598, 2585, 4183, 6768,)),
-                    # Match that the exception message raised for this object...
+                    # Match that the exception message raised for this
+                    # object...
                     exception_str_match_regexes=(
                         # Declares all non-"typing" types *NOT* satisfied by a
                         # random tuple item *NOT* satisfying this hint.
                         r'\bByteString\b',
                         r'\bstr\b',
                         # Declares the index of the random tuple item *NOT*
                         # satisfying this hint.
-                        r'\b[Tt]uple item \d+\b',
+                        r'\b[Tt]uple index \d+ item\b',
                     ),
                 ),
             ),
         ),
 
         # Nested union of no non-"typing" type and multiple "typing" types.
         HintPepMetadata(
@@ -1160,21 +1163,22 @@
 
                 # Mutable sequence of string constants.
                 HintPithUnsatisfiedMetadata(
                     pith=[
                         'Of genteel gentle‐folk — that that Ƹsper',
                         'At my brand‐defaced, landless side',
                     ],
-                    # Match that the exception message raised for this object...
+                    # Match that the exception message raised for this
+                    # object...
                     exception_str_match_regexes=(
                         # Declares all non-"typing" types *NOT* satisfied by a
                         # random list item *NOT* satisfying this hint.
                         r'\bByteString\b',
                         r'\bCallable\b',
                         # Declares the index of the random list item *NOT*
                         # satisfying this hint.
-                        r'\b[Ll]ist item \d+\b',
+                        r'\b[Ll]ist index \d+ item\b',
                     ),
                 ),
             ),
         ),
     ))
```

### Comparing `beartype-0.9.0/beartype_test/a00_unit/data/hint/pep/proposal/_data_pep586.py` & `beartype-0.9.1/beartype_test/a00_unit/data/hint/pep/proposal/_data_pep586.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/data/hint/pep/proposal/_data_pep589.py` & `beartype-0.9.1/beartype_test/a00_unit/data/hint/pep/proposal/_data_pep589.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/data/hint/pep/proposal/_data_pep593.py` & `beartype-0.9.1/beartype_test/a00_unit/data/hint/pep/proposal/_data_pep593.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/data/hint/pep/proposal/data_pep484.py` & `beartype-0.9.1/beartype_test/a00_unit/data/hint/pep/proposal/data_pep484.py`

 * *Files 1% similar despite different names*

```diff
@@ -914,22 +914,23 @@
             piths_unsatisfied_meta=(
                 # String constant.
                 HintPithUnsatisfiedMetadata('Devilet‐Sublet cities waxing'),
                 # List containing exactly one integer. Since list items are
                 # only randomly type-checked, only a list of exactly one item
                 # enables us to match the explicit index at fault below.
                 HintPithUnsatisfiedMetadata(
-                    pith=[73,],
-                    # Match that the exception message raised for this object...
+                    pith=[1010011010,],  # <-- oh, we've done it now
+                    # Match that the exception message raised for this
+                    # object...
                     exception_str_match_regexes=(
                         # Declares the index of the random list item *NOT*
                         # satisfying this hint.
-                        r'\s[Ll]ist item \d+\s',
-                        # Double-quotes the value of this item.
-                        r'\s"73"\s',
+                        r'\b[Ll]ist index \d+ item\b',
+                        # Preserves the value of this item as is.
+                        r'\s1010011010\s',
                     ),
                 ),
             ),
         ),
 
         # Generic list.
         HintPepMetadata(
@@ -1250,15 +1251,15 @@
             piths_unsatisfied_meta=(
                 # Tuple containing fewer items than required.
                 HintPithUnsatisfiedMetadata(
                     pith=('Obeisance',),
                     # Match that the exception message raised for this object...
                     exception_str_match_regexes=(
                         # Compare this tuple's length to the expected length.
-                        r'\b1 not 2\b',
+                        r'\b1 != 2\b',
                     ),
                 ),
             ),
         ),
 
         # Fixed-length tuple of at least one ignorable child hint.
         HintPepMetadata(
@@ -1283,30 +1284,30 @@
                     pith=(
                         999.888,
                         'Obese, slipshodly muslin‐shod priests had maudlin solo',
                     ),
                     # Match that the exception message raised for this object...
                     exception_str_match_regexes=(
                         # Compare this tuple's length to the expected length.
-                        r'\b2 not 3\b',
+                        r'\b2 != 3\b',
                     ),
                 ),
                 # Tuple containing a floating-point number, a string, and a
                 # boolean (in that exact order).
                 HintPithUnsatisfiedMetadata(
                     pith=(
                         75.83,
                         'Unwholesome gentry ventings',
                         False,
                     ),
                     # Match that the exception message raised for this object...
                     exception_str_match_regexes=(
                         # Declares the index and expected type of this fixed
                         # tuple item *NOT* satisfying this hint.
-                        r'\s[Tt]uple item 2\s',
+                        r'\b[Tt]uple index 2 item\b',
                         r'\bstr\b',
                     ),
                 ),
             ),
         ),
 
         # Nested fixed-length tuple of at least one ignorable child hint.
@@ -1345,20 +1346,21 @@
                     pith=(
                         (
                             75.83,
                             'Vespers’ hymnal seance, invoking',
                             True,
                         ),
                     ),
-                    # Match that the exception message raised for this object...
+                    # Match that the exception message raised for this
+                    # object...
                     exception_str_match_regexes=(
                         # Declares the index and expected type of a rondom
                         # tuple item of a fixed tuple item *NOT* satisfying
                         # this hint.
-                        r'\s[Tt]uple item \d+ tuple item 2\s',
+                        r'\b[Tt]uple index \d+ item tuple index 2 item\b',
                         r'\bstr\b',
                     ),
                 ),
             ),
         ),
 
         # Generic fixed-length tuple.
@@ -1408,15 +1410,15 @@
                 HintPithUnsatisfiedMetadata(
                     pith=((53,)),
                     # Match that the exception message raised for this
                     # object...
                     exception_str_match_regexes=(
                         # Declares the index and expected type of a random
                         # tuple item *NOT* satisfying this hint.
-                        r'\s[Tt]uple item \d+\s',
+                        r'\b[Tt]uple index \d+ item\b',
                         r'\bstr\b',
                     ),
                 ),
             ),
         ),
 
         # Generic variadic tuple.
@@ -1503,22 +1505,23 @@
                         r'\*',
                     ),
                 ),
 
                 # Tuple of integers.
                 HintPithUnsatisfiedMetadata(
                     pith=(1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89,),
-                    # Match that the exception message raised for this object...
+                    # Match that the exception message raised for this
+                    # object...
                     exception_str_match_regexes=(
                         # Contains a bullet point declaring the non-"typing"
                         # type *NOT* satisfied by this object.
                         r'\n\*\s.*\bint\b',
                         # Contains a bullet point declaring the index of the
-                        # random list item *NOT* satisfying this hint.
-                        r'\n\*\s.*\b[Tt]uple item \d+\b',
+                        # random tuple item *NOT* satisfying this hint.
+                        r'\n\*\s.*\b[Tt]uple index \d+ item\b',
                     ),
                 ),
             ),
         ),
 
         # Union of three non-"typing" types and an originative "typing" type of
         # a union of three non-"typing" types and an originative "typing" type,
@@ -1574,43 +1577,45 @@
                         r'\*',
                     ),
                 ),
 
                 # Sequence of bytestring items.
                 HintPithUnsatisfiedMetadata(
                     pith=(b"May they rest their certainties' Solicitousness to",),
-                    # Match that the exception message raised for this object...
+                    # Match that the exception message raised for this
+                    # object...
                     exception_str_match_regexes=(
                         # Contains a bullet point declaring one of the
                         # non-"typing" types *NOT* satisfied by this object.
                         r'\n\*\s.*\bint\b',
                         # Contains a bullet point declaring the index of the
-                        # random list item *NOT* satisfying this hint.
-                        r'\n\*\s.*\b[Tt]uple item \d+\b',
+                        # random tuple item *NOT* satisfying this hint.
+                        r'\n\*\s.*\b[Tt]uple index \d+ item\b',
                     ),
                 ),
 
                 # Sequence of mutable sequences of bytestring items.
                 HintPithUnsatisfiedMetadata(
                     pith=([b'Untaint these ties',],),
-                    # Match that the exception message raised for this object...
+                    # Match that the exception message raised for this
+                    # object...
                     exception_str_match_regexes=(
                         # Contains an unindented bullet point declaring one of
                         # the non-"typing" types unsatisfied by this object.
                         r'\n\*\s.*\bfloat\b',
                         # Contains an indented bullet point declaring one of
                         # the non-"typing" types unsatisfied by this object.
                         r'\n\s+\*\s.*\bint\b',
                         # Contains an unindented bullet point declaring the
                         # index of the random tuple item *NOT* satisfying
                         # this hint.
-                        r'\n\*\s.*\b[Tt]uple item \d+\b',
+                        r'\n\*\s.*\b[Tt]uple index \d+ item\b',
                         # Contains an indented bullet point declaring the index
                         # of the random list item *NOT* satisfying this hint.
-                        r'\n\s+\*\s.*\b[L]ist item \d+\b',
+                        r'\n\s+\*\s.*\b[L]ist index \d+ item\b',
                     ),
                 ),
             ),
         ),
 
         # Union of one non-"typing" type and one concrete generic.
         HintPepMetadata(
@@ -1655,23 +1660,24 @@
 
                 # List of bytestring items.
                 HintPithUnsatisfiedMetadata(
                     pith=[
                         b'Blamelessly Slur-chastened rights forthwith, affrighting',
                         b"Beauty's lurid, beleaguered knolls, eland-leagued and",
                     ],
-                    # Match that the exception message raised for this object...
+                    # Match that the exception message raised for this
+                    # object...
                     exception_str_match_regexes=(
                         # Declares all non-"typing" types *NOT* satisfied by a
                         # random list item *NOT* satisfying this hint.
                         r'\bint\b',
                         r'\bstr\b',
                         # Declares the index of the random list item *NOT*
                         # satisfying this hint.
-                        r'\b[Ll]ist item \d+\b',
+                        r'\b[Ll]ist index \d+ item\b',
                     ),
                 ),
             ),
         ),
 
         # Nested union of one non-"typing" type and one "typing" type.
         HintPepMetadata(
@@ -1711,15 +1717,15 @@
                     exception_str_match_regexes=(
                         # Declares all non-"typing" types *NOT* satisfied by a
                         # random tuple item *NOT* satisfying this hint.
                         r'\bByteString\b',
                         r'\bstr\b',
                         # Declares the index of the random tuple item *NOT*
                         # satisfying this hint.
-                        r'\b[Tt]uple item \d+\b',
+                        r'\b[Tt]uple index \d+ item\b',
                     ),
                 ),
             ),
         ),
 
         # Nested union of *NO* isinstanceable type and multiple "typing" types.
         HintPepMetadata(
@@ -1753,23 +1759,24 @@
 
                 # Mutable sequence of string constants.
                 HintPithUnsatisfiedMetadata(
                     pith=[
                         'Of genteel gentle‐folk — that that Ƹsper',
                         'At my brand‐defaced, landless side',
                     ],
-                    # Match that the exception message raised for this object...
+                    # Match that the exception message raised for this
+                    # object...
                     exception_str_match_regexes=(
                         # Declares all non-"typing" types *NOT* satisfied by a
                         # random list item *NOT* satisfying this hint.
                         r'\bByteString\b',
                         r'\bCallable\b',
                         # Declares the index of the random list item *NOT*
                         # satisfying this hint.
-                        r'\b[Ll]ist item \d+\b',
+                        r'\b[Ll]ist index \d+ item\b',
                     ),
                 ),
             ),
         ),
 
         # ................{ UNION ~ optional                  }................
         # Ignorable unsubscripted "Optional" attribute.
```

### Comparing `beartype-0.9.0/beartype_test/a00_unit/data/hint/util/data_hintmetacls.py` & `beartype-0.9.1/beartype_test/a00_unit/data/hint/util/data_hintmetacls.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,22 +7,169 @@
 Project-wide **type hint metadata class hierarchy** (i.e., hierarchy of
 classes encapsulating sample type hints instantiated by the
 :mod:`beartype_test.a00_unit.data.hint` submodules).
 '''
 
 # ....................{ IMPORTS                           }....................
 from beartype._data.hint.pep.sign.datapepsigncls import HintSign
-from typing import Optional
+from typing import Optional, Tuple
 
-# ....................{ HINTS                             }....................
+# ....................{ PRIVATE                           }....................
 _NoneTypeOrType = (type, type(None))
 '''
 2-tuple matching both classes and the ``None`` singleton.
 '''
 
+
+_EXCEPTION_STR_MATCH_REGEXES_MANDATORY = (
+    # Ensure *ALL* exception messages contain the substring "type hint".
+    # Exception messages *NOT* containing this substring are overly ambiguous
+    # and thus effectively erroneous.
+    r'\btype hint\b',
+)
+'''
+Tuple of all **mandatory exception matching regexes** (i.e., r''-style
+uncompiled regular expression strings, each unconditionally matching a
+substring of the exception message expected to be raised by wrapper functions
+when either passed or returning *any* possible pith).
+'''
+
+# ....................{ CLASSES ~ hint : [un]satisfied    }....................
+class HintPithSatisfiedMetadata(object):
+    '''
+    **Type hint-satisfying pith metadata** (i.e., dataclass whose instance
+    variables describe an object satisfying a type hint when either passed as a
+    parameter *or* returned as a value annotated by that hint).
+
+    Attributes
+    ----------
+    pith : object
+        Arbitrary object *not* satisfying this hint when either passed as a
+        parameter *or* returned as a value annotated by this hint.
+    is_context_manager : bool
+        If this pith is a **context manager** (i.e., object defining both the
+        ``__exit__`` and ``__enter__`` dunder methods required to satisfy the
+        context manager protocol), this boolean is either:
+
+        * ``True`` if callers should preserve this context manager as is (e.g.,
+          by passing this context manager to the decorated callable).
+        * ``False`` if callers should safely open and close this context
+          manager to its context *and* replace this context manager with that
+          context (e.g., by passing this context to the decorated callable).
+
+        If this pith is *not* a context manager, this boolean is ignored.
+        Defaults to ``False``.
+    is_pith_factory : bool
+        ``True`` only if this pith is actually a **pith factory** (i.e.,
+        callable accepting *no* parameters and dynamically creating and
+        returning the value to be used as the desired pith, presumably by
+        passing this value to the decorated callable). Defaults to ``False``.
+    '''
+
+    # ..................{ INITIALIZERS                      }..................
+    def __init__(
+        self,
+
+        # Mandatory parameters.
+        pith: object,
+
+        # Optional parameters.
+        is_context_manager: bool = False,
+        is_pith_factory: bool = False,
+    ) -> None:
+        assert isinstance(is_context_manager, bool), (
+            f'{repr(is_context_manager)} not boolean.')
+        assert isinstance(is_pith_factory, bool), (
+            f'{repr(is_pith_factory)} not boolean.')
+
+        # Classify all passed parameters.
+        self.pith = pith
+        self.is_context_manager = is_context_manager
+        self.is_pith_factory = is_pith_factory
+
+    # ..................{ STRINGIFIERS                      }..................
+    def __repr__(self) -> str:
+        return '\n'.join((
+            f'{self.__class__.__name__}(',
+            f'    pith={repr(self.pith)},',
+            f'    is_context_manager={repr(self.is_context_manager)},',
+            f'    is_pith_factory={repr(self.is_pith_factory)},',
+            f')',
+        ))
+
+
+class HintPithUnsatisfiedMetadata(object):
+    '''
+    **Type hint-unsatisfying pith metadata** (i.e., dataclass whose instance
+    variables describe an object *not* satisfying a type hint when either
+    passed as a parameter *or* returned as a value annotated by that hint).
+
+    Attributes
+    ----------
+    pith : object
+        Arbitrary object *not* satisfying this hint when either passed as a
+        parameter *or* returned as a value annotated by this hint.
+    exception_str_match_regexes : Tuple[str]
+        Tuple of zero or more r''-style uncompiled regular expression strings,
+        each matching a substring of the exception message expected to be
+        raised by wrapper functions when either passed or returning this
+        ``pith``. Defaults to the empty tuple.
+    exception_str_not_match_regexes : Tuple[str]
+        Tuple of zero or more r''-style uncompiled regular expression strings,
+        each *not* matching a substring of the exception message expected to be
+        raised by wrapper functions when either passed or returning this
+        ``pith``. Defaults to the empty tuple.
+    '''
+
+    # ..................{ INITIALIZERS                      }..................
+    def __init__(
+        self,
+
+        # Mandatory parameters.
+        pith: object,
+
+        # Optional parameters.
+        exception_str_match_regexes: Tuple[str] = (),
+        exception_str_not_match_regexes: Tuple[str] = (),
+    ) -> None:
+        assert isinstance(exception_str_match_regexes, tuple), (
+            f'{repr(exception_str_match_regexes)} not tuple.')
+        assert isinstance(exception_str_not_match_regexes, tuple), (
+            f'{repr(exception_str_not_match_regexes)} not tuple.')
+        assert all(
+            isinstance(exception_str_match_regex, str)
+            for exception_str_match_regex in exception_str_match_regexes
+        ), f'{repr(exception_str_match_regexes)} not tuple of regexes.'
+        assert all(
+            isinstance(exception_str_not_match_regex, str)
+            for exception_str_not_match_regex in (
+                exception_str_not_match_regexes)
+        ), f'{repr(exception_str_not_match_regexes)} not tuple of regexes.'
+
+        # Classify all remaining passed parameters.
+        self.pith = pith
+        self.exception_str_not_match_regexes = exception_str_not_match_regexes
+
+        # Classify the tuple of all r''-style uncompiled regular expression
+        # strings appended by the tuple of all mandatory such strings.
+        self.exception_str_match_regexes = (
+            exception_str_match_regexes +
+            _EXCEPTION_STR_MATCH_REGEXES_MANDATORY
+        )
+
+    # ..................{ STRINGIFIERS                      }..................
+    def __repr__(self) -> str:
+        return '\n'.join((
+            f'{self.__class__.__name__}(',
+            f'    pith={repr(self.pith)},',
+            f'    exception_str_match_regexes={repr(self.exception_str_match_regexes)},',
+            f'    exception_str_not_match_regexes={repr(self.exception_str_not_match_regexes)},',
+            f')',
+        ))
+
 # ....................{ CLASSES ~ hint : superclass       }....................
 class HintNonpepMetadata(object):
     '''
     **PEP-noncompliant type hint metadata** (i.e., dataclass whose instance
     variables describe a type hint that is either PEP-noncompliant or *mostly*
     indistinguishable from a PEP-noncompliant type hint with metadata
     applicable to various testing scenarios).
@@ -64,16 +211,16 @@
 
         # Mandatory parameters.
         hint: object,
 
         # Optional parameters.
         is_ignorable: bool = False,
         is_supported: bool = True,
-        piths_satisfied_meta: 'Tuple[HintPithSatisfiedMetadata]' = (),
-        piths_unsatisfied_meta: 'Tuple[HintPithUnsatisfiedMetadata]' = (),
+        piths_satisfied_meta: Tuple[HintPithSatisfiedMetadata] = (),
+        piths_unsatisfied_meta: Tuple[HintPithUnsatisfiedMetadata] = (),
     ) -> None:
         assert isinstance(is_ignorable, bool), (
             f'{repr(is_ignorable)} not bool.')
         assert isinstance(is_supported, bool), (
             f'{repr(is_supported)} not bool.')
         assert isinstance(piths_unsatisfied_meta, tuple), (
             f'{repr(piths_unsatisfied_meta)} not tuple.')
@@ -294,134 +441,7 @@
             f'    is_typevars={repr(self.is_typevars)},',
             f'    is_type_typing={repr(self.is_type_typing)},',
             f'    is_typing={repr(self.is_typing)},',
             f'    piths_satisfied_meta={repr(self.piths_satisfied_meta)},',
             f'    piths_unsatisfied_meta={repr(self.piths_unsatisfied_meta)},',
             f')',
         ))
-
-# ....................{ CLASSES ~ hint : [un]satisfied    }....................
-class HintPithSatisfiedMetadata(object):
-    '''
-    **Type hint-satisfying pith metadata** (i.e., dataclass whose instance
-    variables describe an object satisfying a type hint when either passed as a
-    parameter *or* returned as a value annotated by that hint).
-
-    Attributes
-    ----------
-    pith : object
-        Arbitrary object *not* satisfying this hint when either passed as a
-        parameter *or* returned as a value annotated by this hint.
-    is_context_manager : bool
-        If this pith is a **context manager** (i.e., object defining both the
-        ``__exit__`` and ``__enter__`` dunder methods required to satisfy the
-        context manager protocol), this boolean is either:
-
-        * ``True`` if callers should preserve this context manager as is (e.g.,
-          by passing this context manager to the decorated callable).
-        * ``False`` if callers should safely open and close this context
-          manager to its context *and* replace this context manager with that
-          context (e.g., by passing this context to the decorated callable).
-
-        If this pith is *not* a context manager, this boolean is ignored.
-        Defaults to ``False``.
-    is_pith_factory : bool
-        ``True`` only if this pith is actually a **pith factory** (i.e.,
-        callable accepting *no* parameters and dynamically creating and
-        returning the value to be used as the desired pith, presumably by
-        passing this value to the decorated callable). Defaults to ``False``.
-    '''
-
-    # ..................{ INITIALIZERS                      }..................
-    def __init__(
-        self,
-
-        # Mandatory parameters.
-        pith: object,
-
-        # Optional parameters.
-        is_context_manager: bool = False,
-        is_pith_factory: bool = False,
-    ) -> None:
-        assert isinstance(is_context_manager, bool), (
-            f'{repr(is_context_manager)} not boolean.')
-        assert isinstance(is_pith_factory, bool), (
-            f'{repr(is_pith_factory)} not boolean.')
-
-        # Classify all passed parameters.
-        self.pith = pith
-        self.is_context_manager = is_context_manager
-        self.is_pith_factory = is_pith_factory
-
-    # ..................{ STRINGIFIERS                      }..................
-    def __repr__(self) -> str:
-        return '\n'.join((
-            f'{self.__class__.__name__}(',
-            f'    pith={repr(self.pith)},',
-            f'    is_context_manager={repr(self.is_context_manager)},',
-            f'    is_pith_factory={repr(self.is_pith_factory)},',
-            f')',
-        ))
-
-
-class HintPithUnsatisfiedMetadata(object):
-    '''
-    **Type hint-unsatisfying pith metadata** (i.e., dataclass whose instance
-    variables describe an object *not* satisfying a type hint when either
-    passed as a parameter *or* returned as a value annotated by that hint).
-
-    Attributes
-    ----------
-    pith : object
-        Arbitrary object *not* satisfying this hint when either passed as a
-        parameter *or* returned as a value annotated by this hint.
-    exception_str_match_regexes : Tuple[str]
-        Tuple of zero or more r''-style uncompiled regular expression strings,
-        each matching a substring of the exception message expected to be
-        raised by wrapper functions when either passed or returning this
-        ``pith``. Defaults to the empty tuple.
-    exception_str_not_match_regexes : Tuple[str]
-        Tuple of zero or more r''-style uncompiled regular expression strings,
-        each *not* matching a substring of the exception message expected to be
-        raised by wrapper functions when either passed or returning this
-        ``pith``. Defaults to the empty tuple.
-    '''
-
-    # ..................{ INITIALIZERS                      }..................
-    def __init__(
-        self,
-
-        # Mandatory parameters.
-        pith: object,
-
-        # Optional parameters.
-        exception_str_match_regexes: 'Tuple[str]' = (),
-        exception_str_not_match_regexes: 'Tuple[str]' = (),
-    ) -> None:
-        assert isinstance(exception_str_match_regexes, tuple), (
-            f'{repr(exception_str_match_regexes)} not tuple.')
-        assert isinstance(exception_str_not_match_regexes, tuple), (
-            f'{repr(exception_str_not_match_regexes)} not tuple.')
-        assert all(
-            isinstance(exception_str_match_regex, str)
-            for exception_str_match_regex in exception_str_match_regexes
-        ), f'{repr(exception_str_match_regexes)} not tuple of regexes.'
-        assert all(
-            isinstance(exception_str_not_match_regex, str)
-            for exception_str_not_match_regex in (
-                exception_str_not_match_regexes)
-        ), f'{repr(exception_str_not_match_regexes)} not tuple of regexes.'
-
-        # Classify all passed parameters.
-        self.pith = pith
-        self.exception_str_match_regexes = exception_str_match_regexes
-        self.exception_str_not_match_regexes = exception_str_not_match_regexes
-
-    # ..................{ STRINGIFIERS                      }..................
-    def __repr__(self) -> str:
-        return '\n'.join((
-            f'{self.__class__.__name__}(',
-            f'    pith={repr(self.pith)},',
-            f'    exception_str_match_regexes={repr(self.exception_str_match_regexes)},',
-            f'    exception_str_not_match_regexes={repr(self.exception_str_not_match_regexes)},',
-            f')',
-        ))
```

### Comparing `beartype-0.9.0/beartype_test/a00_unit/data/hint/util/data_hintmetatyping.py` & `beartype-0.9.1/beartype_test/a00_unit/data/hint/util/data_hintmetatyping.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/data/pep/pep563/data_pep563_club.py` & `beartype-0.9.1/beartype_test/a00_unit/data/pep/pep563/data_pep563_club.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/data/pep/pep563/data_pep563_poem.py` & `beartype-0.9.1/beartype_test/a00_unit/data/pep/pep563/data_pep563_poem.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/data/util/func/data_utilfunccode.py` & `beartype-0.9.1/beartype_test/a00_unit/data/util/func/data_utilfunccode.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/data/util/mod/data_utilmodule_bad.py` & `beartype-0.9.1/beartype_test/a00_unit/data/util/mod/data_utilmodule_bad.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a00_unit/data/util/mod/data_utilmodule_good.py` & `beartype-0.9.1/beartype_test/a00_unit/data/util/mod/data_utilmodule_good.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/a90_func/doc/test_docreadme.py` & `beartype-0.9.1/beartype_test/a90_func/doc/test_docreadme.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,25 +41,25 @@
         Builtin fixture object permitting object attributes to be safely
         modified for the duration of this unit test.
     '''
 
     # Defer heavyweight imports.
     from docutils.core import publish_parts
     from docutils.utils import Reporter
-    from beartype_test.util.path.pytpathproject import get_project_readme_file
+    from beartype_test.util.path.pytpathmain import get_main_readme_file
 
     # Decoded plaintext contents of this project's readme file as a string.
     #
     # Note this encoding *MUST* explicitly be passed here. Although macOS and
     # Linux both default to this encoding, Windows defaults to the single-byte
     # encoding "cp1252" for backward compatibility. Failing to pass this
     # encoding here results in a non-human-readable test failure under Windows:
     #     UnicodeDecodeError: 'charmap' codec can't decode byte 0x9d in
     #     position 1495: character maps to <undefined>
-    README_CONTENTS = get_project_readme_file().read_text(encoding='utf-8')
+    README_CONTENTS = get_main_readme_file().read_text(encoding='utf-8')
 
     # List of all warning and error messages emitted by "docutils" during
     # parsing of this project's top-level "README.rst" file.
     system_messages = []
 
     # Original non-monkey-patched method of the public :mod:`docutils`
     # singleton emitting warnings and errors *BEFORE* patching this method.
```

### Comparing `beartype-0.9.0/beartype_test/a90_func/pep/test_pep561_static.py` & `beartype-0.9.1/beartype_test/a90_func/pep/test_pep561_static.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,40 +57,40 @@
     '''
     Functional test testing this project's compliance with :pep:`561` by
     externally running :mod:`mypy`, the most popular third-party static type
     checker as of this test, against this project's top-level package.
     '''
 
     # Defer heavyweight imports.
-    from beartype_test.util.path.pytpathproject import (
-        get_project_mypy_config_file,
-        get_project_package_dir,
+    from beartype_test.util.path.pytpathmain import (
+        get_main_mypy_config_file,
+        get_main_package_dir,
     )
     from mypy import api
 
     # List of all command-line options (i.e., "-"-prefixed strings) to be
     # effectively passed to the external "mypy" command.
     #
     # Note this iterable *MUST* be defined as a list rather than tuple. If a
     # tuple, the function called below raises an exception. Hot garbage!
     MYPY_OPTIONS = [
         # Absolute dirname of this project's top-level mypy configuration.
         # Since our "tox" configuration isolates testing to a temporary
         # directory, mypy is unable to find its configuration without help.
-        '--config-file', str(get_project_mypy_config_file()),
+        '--config-file', str(get_main_mypy_config_file()),
     ]
 
     # List of all command-line arguments (i.e., non-options) to be effectively
     # passed to the external "mypy" command.
     #
     # Note this iterable *MUST* be defined as a list rather than tuple. If a
     # tuple, the function called below raises an exception. Steaming trash!
     MYPY_ARGUMENTS = [
         # Absolute dirname of this project's top-level package.
-        str(get_project_package_dir()),
+        str(get_main_package_dir()),
     ]
 
     # Tuple of all command-line options to be effectively passed to the
     # external "mypy" command.
     #
     # Note that we intentionally do *NOT* assert that call to have exited with
     # a successful exit code. Although mypy does exit with success on local
```

### Comparing `beartype-0.9.0/beartype_test/conftest.py` & `beartype-0.9.1/beartype_test/conftest.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/util/mark/pytmark.py` & `beartype-0.9.1/beartype_test/util/mark/pytmark.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/util/mark/pytskip.py` & `beartype-0.9.1/beartype_test/util/mark/pytskip.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/util/mod/pytmodimport.py` & `beartype-0.9.1/beartype_test/util/mod/pytmodimport.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/util/mod/pytmodtest.py` & `beartype-0.9.1/beartype_test/util/mod/pytmodtest.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,51 @@
     # Defer heavyweight imports.
     from beartype._util.mod.utilmodtest import is_module_typing_any_attr
 
     # Return true only if the "Annotated" type hint is importable from either
     # the official "typing" or third-party "typing_extensions" modules.
     return is_module_typing_any_attr('Annotated')
 
-# ....................{ TESTERS ~ numpy                   }....................
+# ....................{ TESTERS ~ lib                     }....................
+@callable_cached
+def is_package_sphinx() -> bool:
+    '''
+    ``True`` only if a reasonably recent version of Sphinx is importable under
+    the active Python interpreter.
+    '''
+
+    # Defer heavyweight imports.
+    from beartype.meta import _LIB_DOCTIME_MANDATORY_VERSION_MINIMUM_SPHINX
+    from beartype._util.mod.utilmodtest import is_module_version_at_least
+
+    # Return true only if this version of this package is importable.
+    return is_module_version_at_least(
+        'sphinx', _LIB_DOCTIME_MANDATORY_VERSION_MINIMUM_SPHINX)
+
+
+@callable_cached
+def is_package_typing_extensions() -> bool:
+    '''
+    ``True`` only if a reasonably recent version of the third-party
+    :mod:`typing_extensions` package is importable under the active Python
+    interpreter.
+    '''
+
+    # Defer heavyweight imports.
+    from beartype.meta import (
+        _LIB_RUNTIME_OPTIONAL_VERSION_MINIMUM_TYPING_EXTENSIONS)
+    from beartype._util.mod.utilmodtest import is_module_version_at_least
+
+    # Return true only if this version of this package is importable.
+    return is_module_version_at_least(
+        'typing_extensions',
+        _LIB_RUNTIME_OPTIONAL_VERSION_MINIMUM_TYPING_EXTENSIONS,
+    )
+
+# ....................{ TESTERS ~ lib : numpy             }....................
 @callable_cached
 def is_package_numpy() -> bool:
     '''
     ``True`` only if a reasonably recent version of NumPy is importable under
     the active Python interpreter.
     '''
 
@@ -52,15 +88,15 @@
     from beartype.meta import _LIB_RUNTIME_OPTIONAL_VERSION_MINIMUM_NUMPY
     from beartype._util.mod.utilmodtest import is_module_version_at_least
 
     # Return true only if this version of this package is importable.
     return is_module_version_at_least(
         'numpy', _LIB_RUNTIME_OPTIONAL_VERSION_MINIMUM_NUMPY)
 
-# ....................{ TESTERS ~ numpy : ndarray         }....................
+
 @callable_cached
 def is_package_numpy_typing_ndarray_deep() -> bool:
     '''
     ``True`` only if :attr:`numpy.typing.NDArray` type hints are deeply
     supported by the :func:`beartype.beartype` decorator under the active
     Python interpreter.
 
@@ -76,27 +112,7 @@
     # Return true only if...
     return (
         # A recent version of NumPy is importable *AND*...
         is_package_numpy() and
         # Beartype validators are usable under the active Python interpreter.
         is_package_beartype_vale_usable()
     )
-
-# ....................{ TESTERS ~ typing                  }....................
-@callable_cached
-def is_package_typing_extensions() -> bool:
-    '''
-    ``True`` only if a reasonably recent version of the third-party
-    :mod:`typing_extensions` package is importable under the active Python
-    interpreter.
-    '''
-
-    # Defer heavyweight imports.
-    from beartype.meta import (
-        _LIB_RUNTIME_OPTIONAL_VERSION_MINIMUM_TYPING_EXTENSIONS)
-    from beartype._util.mod.utilmodtest import is_module_version_at_least
-
-    # Return true only if this version of this package is importable.
-    return is_module_version_at_least(
-        'typing_extensions',
-        _LIB_RUNTIME_OPTIONAL_VERSION_MINIMUM_TYPING_EXTENSIONS,
-    )
```

### Comparing `beartype-0.9.0/beartype_test/util/os/command/pytcmdexit.py` & `beartype-0.9.1/beartype_test/util/os/command/pytcmdexit.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/util/pytcontext.py` & `beartype-0.9.1/beartype_test/util/pytcontext.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/beartype_test/util/pytroar.py` & `beartype-0.9.1/beartype_test/util/pytroar.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/conftest.py` & `beartype-0.9.1/conftest.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/doc/Makefile` & `beartype-0.9.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/doc/RELEASE.rst` & `beartype-0.9.1/doc/RELEASE.rst`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/doc/make.bat` & `beartype-0.9.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/doc/source/conf.py` & `beartype-0.9.1/doc/source/conf.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,36 +20,35 @@
 #At the least, we probably need to add the following line to our top-level
 #"conftest.py" file:
 #    pytest_plugins = 'sphinx.testing.fixtures'
 #FIXME: Additionally, we should similarly add a single pytest-based functional
 #test exercising the correctness of our top-level "README.rst" file -- ideally
 #by invoking "checkdocs" somehow if conditionally available.
 
-# ....................{ IMPORTS                           }....................
-# Sphinx defaults to hardcoding version specifiers. Since this is insane, we
-# import our package-specific version specifier for reuse below. See also:
-# * https://protips.readthedocs.io/git-tag-version.html
-#   "Inferring Release Number from Git Tags", detailing a clever one-liner
-#   harvesting this specifier from the most recent git tag.
-from beartype.meta import AUTHORS, COPYRIGHT, NAME, VERSION
-from beartype.roar import BeartypeDependencyOptionalMissingWarning
-from warnings import warn
-
 # ....................{ IMPORTS ~ kludge                  }....................
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 # See also:
 # * https://samnicholls.net/2016/06/15/how-to-sphinx-readthedocs
 #   The "Make autodoc actually work" is the canonical writeup on this kludge.
+import os, sys
+sys.path.insert(0, os.path.abspath('../../'))
 
-#FIXME: Uncomment if actually necessary.
-# import os, sys
-# sys.path.insert(0, os.path.abspath('..'))
+# ....................{ IMPORTS                           }....................
+# Sphinx defaults to hardcoding version specifiers. Since this is insane, we
+# import our package-specific version specifier for reuse below. See also:
+# * https://protips.readthedocs.io/git-tag-version.html
+#   "Inferring Release Number from Git Tags", detailing a clever one-liner
+#   harvesting this specifier from the most recent git tag.
+from beartype.meta import AUTHORS, COPYRIGHT, NAME, VERSION
+from beartype.roar import BeartypeDependencyOptionalMissingWarning
+from beartype._util.mod.utilmodtest import is_module
+from warnings import warn
 
 # ....................{ METADATA                          }....................
 # Metadata programmatically defined by this package.
 project = NAME
 author = AUTHORS
 copyright = COPYRIGHT
 release = VERSION
@@ -67,19 +66,47 @@
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = [
     # ..................{ BUILTIN                           }..................
     # Builtin extensions unconditionally available under *ALL* reasonably
     # modern versions of Sphinx uniquely prefixed by "sphinx.ext.".
 
+    #FIXME: Actually, we probably just want to use the third-party Sphinx
+    #AutoAPI extension instead at:
+    #    https://github.com/readthedocs/sphinx-autoapi
+    #...is what we'd be saying if AutoAPI was still actively maintained. *sigh*
+    #FIXME: Almost certainly insufficient. Since this is Sphinx, the
+    #"autodoc" extension requires additional non-trivial configuration. Note,
+    #however, that the "autosummary" extension enabled below *SHOULD* automate
+    #most of that configuration once its fully working. Ergo, avoid investing a
+    #considerable amount of effort in "autodoc" itself. Try "autosummary"!
+
     # Builtin extension autogenerating reStructuredText documentation from
     # class, callable, and variable docstrings embedded in Python modules,
     # documenting this project's public (and optionally also private) API.
     'sphinx.ext.autodoc',
 
+    #FIXME: How does this compare with "viewcode"? Are the two at all
+    #comparable? Does merely one suffice? Research us up, please.
+    #FIXME: Almost certainly insufficient. Since this is Sphinx, the
+    #"autosummary" extension requires additional non-trivial configuration that
+    #absolutely *SHOULD* come bundled with Sphinx but currently isn't for
+    #nebulous reasons. See this StackOverflow answer for an exhaustive solution
+    #requiring copying of third-party templates into our configuration:
+    #    https://stackoverflow.com/a/62613202/2809027
+    #Lastly, note that this issue may have been resolved by a bleeding-edge
+    #Sphinx version by the time we finally resolve this. See also the end of:
+    #    https://github.com/sphinx-doc/sphinx/issues/7912
+
+    # Builtin extension autosummarizing reStructuredText documentation
+    # autogenerated by the "autodoc" extension (listed above). By default,
+    # the "autodoc" extension fails to automatically structure (i.e., summarize
+    # with a single compact HTML markup tag) the documentation it generates.
+    'sphinx.ext.autosummary',
+
     # Builtin extension autogenerating reStructuredText documentation from
     # class, callable, and variable docstrings embedded in Python modules
     # formatted according to either NumPy or Google style.
     #
     # Note this effectively requires 'sphinx.ext.autodoc' to be listed as well.
     'sphinx.ext.napoleon',
 
@@ -97,30 +124,28 @@
     # usability, this block should typically be empty. Third-party Sphinx
     # extensions should ideally be optionally enabled. See below.
 ]
 
 # ....................{ EXTENSIONS ~ optional             }....................
 # Third-party Sphinx extensions conditionally used if externally installed.
 
-# Attempt to optionally...
-try:
-    # Import "sphinx_rtd_theme", a third-party Sphinx extension providing the
-    # official Read The Docs (RTD) HTML theme. This theme is preferable where
-    # available for improved mobile-friendly rendering.
-    import sphinx_rtd_theme
-
+# If "sphinx_rtd_theme" (i.e., the third-party Sphinx extension providing the
+# official Read The Docs (RTD) HTML theme) is importable under the active
+# Python interpreter, prefer this theme to Sphinx's default HTML theme for
+# substantially more mobile-friendly rendering.
+if is_module('sphinx_rtd_theme'):
     # Register the fully-qualified name of this extension.
     extensions.append('sphinx_rtd_theme')
 
     # Set the HTML theme to this theme.
     html_theme = 'sphinx_rtd_theme'
-# If this theme extension is unavailable:
-# * Fallback to the default Sphinx HTML theme.
-# * Emit a non-fatal warning informing end users of this fallback.
-except ImportError:
+# Else, this theme extension is unavailable. In this case, fallback to the
+# Sphinx's default HTML theme *AND*...
+else:
+    # Emit a non-fatal warning informing end users of this fallback.
     warn(
         (
             'Optional Sphinx extension "sphinx_rtd_theme" not found; '
             'falling back to default Sphinx HTML theme.'
         ),
         BeartypeDependencyOptionalMissingWarning
     )
```

### Comparing `beartype-0.9.0/doc/source/index.rst` & `beartype-0.9.1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/pytest.ini` & `beartype-0.9.1/pytest.ini`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/setup.py` & `beartype-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `beartype-0.9.0/tox.ini` & `beartype-0.9.1/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -24,14 +24,46 @@
 # *THIS CONFIGURATION IS INTENDED TO BE RUN FROM CONTINUOUS INTEGRATION (CI).*
 # This configuration is *not* intended to be run directly from the command line
 # (e.g., by running "tox" without arguments), as doing so will implicitly
 # create duplicate testing environments and thus rerun testing environments.
 # That's bad. Instead, run the top-level "tox" shell script in this repository:
 #     $ ./tox
 #
+# *THIS CONFIGURATION IS INTOLERANT OF UNICODE CHARACTERS.* Note that setting
+# "PYIOENCODING = UTF-8" under the "setenv" section below has no meaningful
+# effect. For unknown reasons, "tox" is incapable of processing UTF-8 here.
+# This is why nobody gets good things. If this file contains one or more
+# UTF-8-encoded characters here, "tox" fails with a non-human-readable
+# exception traceback resembling:
+#     Traceback (most recent call last):
+#       File "/opt/hostedtoolcache/Python/3.8.12/x64/lib/python3.8/runpy.py", line 194, in _run_module_as_main
+#         return _run_code(code, main_globals, None,
+#       File "/opt/hostedtoolcache/Python/3.8.12/x64/lib/python3.8/runpy.py", line 87, in _run_code
+#         exec(code, run_globals)
+#       File "/opt/hostedtoolcache/Python/3.8.12/x64/lib/python3.8/site-packages/tox/__main__.py", line 4, in <module>
+#         tox.cmdline()
+#       File "/opt/hostedtoolcache/Python/3.8.12/x64/lib/python3.8/site-packages/tox/session/__init__.py", line 44, in cmdline
+#         main(args)
+#       File "/opt/hostedtoolcache/Python/3.8.12/x64/lib/python3.8/site-packages/tox/session/__init__.py", line 65, in main
+#         config = load_config(args)
+#       File "/opt/hostedtoolcache/Python/3.8.12/x64/lib/python3.8/site-packages/tox/session/__init__.py", line 81, in load_config
+#         config = parseconfig(args)
+#       File "/opt/hostedtoolcache/Python/3.8.12/x64/lib/python3.8/site-packages/tox/config/__init__.py", line 282, in parseconfig
+#         ParseIni(config, config_file, content)
+#       File "/opt/hostedtoolcache/Python/3.8.12/x64/lib/python3.8/site-packages/tox/config/__init__.py", line 1145, in __init__
+#         self._cfg = py.iniconfig.IniConfig(config.toxinipath, ini_data)
+#       File "/opt/hostedtoolcache/Python/3.8.12/x64/lib/python3.8/site-packages/py/_vendored_packages/iniconfig/__init__.py", line 54, in __init__
+#         tokens = self._parse(iter(f))
+#       File "/opt/hostedtoolcache/Python/3.8.12/x64/lib/python3.8/site-packages/py/_vendored_packages/iniconfig/__init__.py", line 82, in _parse
+#         for lineno, line in enumerate(line_iter):
+#       File "/opt/hostedtoolcache/Python/3.8.12/x64/lib/python3.8/codecs.py", line 322, in decode
+#         (result, consumed) = self._buffer_decode(data, self.errors, final)
+#     UnicodeDecodeError: 'utf-8' codec can't decode byte 0xd7 in position 3335: invalid continuation byte
+#     Error: Process completed with exit code 1.
+#
 # --------------------( VARIABLES                         )--------------------
 # tox dynamically substitutes "{"- and "}"-delimited variable names with the
 # strings to which those variables expand. Supported variable names include:
 #
 # * "{envtmpdir}", the absolute dirname of a temporary directory specific to
 #   the current virtual environment to which this project has been installed.
 # * "{posargs}", the whitespace-delimited list of all command-line arguments
@@ -57,27 +89,23 @@
 # * The "tox-env" setting in ".github/workflows/python_test.yml".
 #!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 # Test matrix defined as a bash-interpolated string, where tox implicitly:
 # * Expands "py" to "python".
 # * Delimits the subsequent two digits with a dot to associate each resulting
 #   test configuration with the basename of an external command running an
 #   externally installed Python interpreter.
-# * Expands "-"-delimited lists via the Cartesian set product A × B,
+# * Expands "-"-delimited lists via the Cartesian set product A x B,
 #   effectively "multiplying" each environment on the left of each "-" against
 #   each environment on the right of that "-". Moreover, each such environment
 #   remains preserved and thus distinctly testable as that environment.
 #
 # For example, setting "envlist = py27,py38" produces a test matrix exercising
 # the externally installed "python2.7" and "python3.8" commands. See also:
 #     https://tox.readthedocs.io/en/latest/config.html#generating-environments-conditional-settings
-
-#FIXME: Add "310" back to this list *AFTER* the radioactive fallout from the
-#recent PEP 563 reversion finally settles. This is why the bleeding edge cuts.
-envlist = py{36,37,38,39,py36,py37}-coverage
-#envlist = py3{6,7,8,9}-{linux,windows},pypy3{6,7}-{linux,windows}
+envlist = py{36,37,38,39,310,py36,py37}-coverage
 
 #FIXME: Override this from within CI configurations by passing the
 #"--skip-missing-interpreters=false" when running the "tox" command,
 #preventing CI runs from erroneously returning success on missing interpreters.
 
 # Ignore Python environments unavailable on the current system. By default,
 # "tox" fails on the first unavailable Python environment. While sensible for
@@ -163,36 +191,27 @@
     PIP_CACHE_DIR
 
 # ....................{ ENV ~ dependencies                }....................
 # Comma- and newline-delimited string listing the names of all "setup.py"-based
 # "extras" required as mandatory or optional dependencies when testing this
 # project.
 extras =
-    #FIXME: Actually, let's *NOT* do this. Ideally, we would enable this when
-    #manually testing locally and disable this when automatically testing
-    #remotely under CI to reduce consumption of scarce CI minutes. Sadly, there
-    #appears to be no sane means of achieving this without defining a
-    #completely separate "tox.ini" file for remote testing -- which we are
-    #currently *NOT* prepared to do, because violating DRY brings pain.
-    # Install all optional runtime dependencies to maximize test coverage.
-    #all
-
     # Install all mandatory test-specific dependencies. This is the official
     # solution supported by "tox" developers for eliminating redundancy between
     # testing dependencies listed within this file and the top-level "setup.py"
     # script. While non-intuitive, we have little recourse. See also:
     #     https://stackoverflow.com/questions/29870629/pip-install-test-dependencies-for-tox-from-setup-py
     #     https://stackoverflow.com/questions/39922650/tox-tests-use-setup-py-extra-require-as-tox-deps-source
     #     https://github.com/tox-dev/tox/issues/13#issuecomment-247788280
     # Note that this also requires ".[test-tox]" to be listed as a dependency.
     test-tox
 
     # If the caller explicitly concatenated the current environment name by
     # "-coverage" (e.g., "py310-coverage"), install all mandatory
-    # coverage-specific dependencies.
+    # coverage-specific dependencies as well.
     coverage: test-tox-coverage
 
 # Comma- and newline-delimited string listing the names of all mandatory
 # dependencies (i.e., third-party packages) required to test this project.
 #
 # Note that this also requires "test-tox" to be listed as an extra above.
 deps = .[test-tox]
@@ -226,15 +245,17 @@
 
     # Run our entire pytest-based test suite. Dismantled, this is:
     # * "{env:_COVERAGE_COMMAND:}", expanding to either:
     #   * If measuring coverage, the value of the "${_COVERAGE_COMMAND}"
     #     environment variable defined above.
     #   * Else, the empty string.
     # * "--maxfail={n}", halting testing on the {n}th failure.
-    {envpython} -m {env:_COVERAGE_COMMAND:} pytest --maxfail=1 {posargs} "{toxinidir}"
+    {envpython} \
+        -m {env:_COVERAGE_COMMAND:} \
+        pytest --maxfail=1 {posargs} "{toxinidir}"
     # {envpython} -m {env:_COVERAGE_COMMAND:} pytest --maxfail=1 -vvvv {posargs} "{toxinidir}"
     # {envpython} -m {env:_COVERAGE_COMMAND:} pytest --maxfail=1 -k test_pep563_closure_nested {posargs} "{toxinidir}"
 
     # If measuring coverage, additionally generate a coverage report in the
     # specific format expected by Codecov *AFTER* running our test suite and
     # thus collecting coverage statistics.
     coverage: {envpython} -m coverage xml -o "{toxinidir}/coverage.xml"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

