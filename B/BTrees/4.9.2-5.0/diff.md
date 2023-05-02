# Comparing `tmp/BTrees-4.9.2.tar.gz` & `tmp/BTrees-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BTrees-4.9.2.tar", last modified: Wed Jun  9 10:40:19 2021, max compression
+gzip compressed data, was "BTrees-5.0.tar", last modified: Fri Feb 10 15:12:07 2023, max compression
```

## Comparing `BTrees-4.9.2.tar` & `BTrees-5.0.tar`

### file list

```diff
@@ -1,106 +1,105 @@
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2021-06-09 10:40:19.168584 BTrees-4.9.2/
--rw-r--r--   0 jmadden    (501) staff       (20)      207 2021-06-09 10:40:18.000000 BTrees-4.9.2/.coveragerc
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2021-06-09 10:40:19.137364 BTrees-4.9.2/.github/
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2021-06-09 10:40:19.142892 BTrees-4.9.2/.github/workflows/
--rw-r--r--   0 jmadden    (501) staff       (20)    16288 2021-06-09 10:40:18.000000 BTrees-4.9.2/.github/workflows/tests.yml
--rw-r--r--   0 jmadden    (501) staff       (20)    16665 2021-06-09 10:40:18.000000 BTrees-4.9.2/CHANGES.rst
--rw-r--r--   0 jmadden    (501) staff       (20)       32 2021-06-09 10:40:18.000000 BTrees-4.9.2/COPYRIGHT.txt
--rw-r--r--   0 jmadden    (501) staff       (20)     2070 2021-06-09 10:40:18.000000 BTrees-4.9.2/LICENSE.txt
--rw-r--r--   0 jmadden    (501) staff       (20)      368 2021-06-09 10:40:18.000000 BTrees-4.9.2/MANIFEST.in
--rw-r--r--   0 jmadden    (501) staff       (20)    23199 2021-06-09 10:40:19.168885 BTrees-4.9.2/PKG-INFO
--rw-r--r--   0 jmadden    (501) staff       (20)     1288 2021-06-09 10:40:18.000000 BTrees-4.9.2/README.rst
--rw-r--r--   0 jmadden    (501) staff       (20)     7458 2021-06-09 10:40:18.000000 BTrees-4.9.2/bootstrap.py
--rw-r--r--   0 jmadden    (501) staff       (20)      833 2021-06-09 10:40:18.000000 BTrees-4.9.2/buildout.cfg
--rw-r--r--   0 jmadden    (501) staff       (20)       89 2021-06-09 10:40:18.000000 BTrees-4.9.2/doc-requirements.txt
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2021-06-09 10:40:19.145026 BTrees-4.9.2/docs/
--rw-r--r--   0 jmadden    (501) staff       (20)     5564 2021-06-09 10:40:18.000000 BTrees-4.9.2/docs/Makefile
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2021-06-09 10:40:19.145616 BTrees-4.9.2/docs/_static/
--rw-r--r--   0 jmadden    (501) staff       (20)      363 2021-06-09 10:40:18.000000 BTrees-4.9.2/docs/_static/custom.css
--rw-r--r--   0 jmadden    (501) staff       (20)        0 2021-06-09 10:40:18.000000 BTrees-4.9.2/docs/_static/placeholder.txt
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2021-06-09 10:40:19.145796 BTrees-4.9.2/docs/_templates/
--rw-r--r--   0 jmadden    (501) staff       (20)        0 2021-06-09 10:40:18.000000 BTrees-4.9.2/docs/_templates/placeholder.txt
--rw-r--r--   0 jmadden    (501) staff       (20)     3599 2021-06-09 10:40:18.000000 BTrees-4.9.2/docs/api.rst
--rw-r--r--   0 jmadden    (501) staff       (20)       28 2021-06-09 10:40:18.000000 BTrees-4.9.2/docs/changes.rst
--rw-r--r--   0 jmadden    (501) staff       (20)     9001 2021-06-09 10:40:18.000000 BTrees-4.9.2/docs/conf.py
--rw-r--r--   0 jmadden    (501) staff       (20)    17124 2021-06-09 10:40:18.000000 BTrees-4.9.2/docs/development.rst
--rw-r--r--   0 jmadden    (501) staff       (20)      533 2021-06-09 10:40:18.000000 BTrees-4.9.2/docs/index.rst
--rw-r--r--   0 jmadden    (501) staff       (20)     5096 2021-06-09 10:40:18.000000 BTrees-4.9.2/docs/make.bat
--rw-r--r--   0 jmadden    (501) staff       (20)    21735 2021-06-09 10:40:18.000000 BTrees-4.9.2/docs/overview.rst
--rw-r--r--   0 jmadden    (501) staff       (20)       88 2021-06-09 10:40:18.000000 BTrees-4.9.2/pyproject.toml
--rw-r--r--   0 jmadden    (501) staff       (20)      421 2021-06-09 10:40:19.169644 BTrees-4.9.2/setup.cfg
--rw-r--r--   0 jmadden    (501) staff       (20)     7541 2021-06-09 10:40:18.000000 BTrees-4.9.2/setup.py
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2021-06-09 10:40:19.138149 BTrees-4.9.2/src/
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2021-06-09 10:40:19.160229 BTrees-4.9.2/src/BTrees/
--rw-r--r--   0 jmadden    (501) staff       (20)    24825 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/BTreeItemsTemplate.c
--rw-r--r--   0 jmadden    (501) staff       (20)    25482 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/BTreeModuleTemplate.c
--rw-r--r--   0 jmadden    (501) staff       (20)    75653 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/BTreeTemplate.c
--rw-r--r--   0 jmadden    (501) staff       (20)    56136 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/BucketTemplate.c
--rw-r--r--   0 jmadden    (501) staff       (20)    23750 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/Interfaces.py
--rw-r--r--   0 jmadden    (501) staff       (20)     1937 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/Length.py
--rw-r--r--   0 jmadden    (501) staff       (20)    12070 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/MergeTemplate.c
--rw-r--r--   0 jmadden    (501) staff       (20)    17264 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/SetOpTemplate.c
--rw-r--r--   0 jmadden    (501) staff       (20)      281 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/SetOpTemplate.h
--rw-r--r--   0 jmadden    (501) staff       (20)    20507 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/SetTemplate.c
--rw-r--r--   0 jmadden    (501) staff       (20)    18335 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/TreeSetTemplate.c
--rw-r--r--   0 jmadden    (501) staff       (20)     1067 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/_IFBTree.c
--rw-r--r--   0 jmadden    (501) staff       (20)     1061 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/_IIBTree.c
--rw-r--r--   0 jmadden    (501) staff       (20)     1073 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/_IOBTree.c
--rw-r--r--   0 jmadden    (501) staff       (20)     1104 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/_IUBTree.c
--rw-r--r--   0 jmadden    (501) staff       (20)     1139 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/_LFBTree.c
--rw-r--r--   0 jmadden    (501) staff       (20)     1130 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/_LLBTree.c
--rw-r--r--   0 jmadden    (501) staff       (20)     1110 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/_LOBTree.c
--rw-r--r--   0 jmadden    (501) staff       (20)     1172 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/_LQBTree.c
--rw-r--r--   0 jmadden    (501) staff       (20)     1073 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/_OIBTree.c
--rw-r--r--   0 jmadden    (501) staff       (20)     1110 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/_OLBTree.c
--rw-r--r--   0 jmadden    (501) staff       (20)     1082 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/_OOBTree.c
--rw-r--r--   0 jmadden    (501) staff       (20)     1148 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/_OQBTree.c
--rw-r--r--   0 jmadden    (501) staff       (20)     1080 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/_OUBTree.c
--rw-r--r--   0 jmadden    (501) staff       (20)     1175 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/_QFBTree.c
--rw-r--r--   0 jmadden    (501) staff       (20)     1170 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/_QLBTree.c
--rw-r--r--   0 jmadden    (501) staff       (20)     1146 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/_QOBTree.c
--rw-r--r--   0 jmadden    (501) staff       (20)     1204 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/_QQBTree.c
--rw-r--r--   0 jmadden    (501) staff       (20)     1107 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/_UFBTree.c
--rw-r--r--   0 jmadden    (501) staff       (20)     1101 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/_UIBTree.c
--rw-r--r--   0 jmadden    (501) staff       (20)     1089 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/_UOBTree.c
--rw-r--r--   0 jmadden    (501) staff       (20)     1143 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/_UUBTree.c
--rw-r--r--   0 jmadden    (501) staff       (20)     4177 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/__init__.py
--rw-r--r--   0 jmadden    (501) staff       (20)    52889 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/_base.py
--rw-r--r--   0 jmadden    (501) staff       (20)     1726 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/_compat.h
--rw-r--r--   0 jmadden    (501) staff       (20)     4790 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/_compat.py
--rw-r--r--   0 jmadden    (501) staff       (20)    15693 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/_datatypes.py
--rw-r--r--   0 jmadden    (501) staff       (20)     4736 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/_fsBTree.c
--rw-r--r--   0 jmadden    (501) staff       (20)     7801 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/_module_builder.py
--rw-r--r--   0 jmadden    (501) staff       (20)    17406 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/check.py
--rw-r--r--   0 jmadden    (501) staff       (20)      899 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/floatvaluemacros.h
--rw-r--r--   0 jmadden    (501) staff       (20)     4072 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/intkeymacros.h
--rw-r--r--   0 jmadden    (501) staff       (20)     4574 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/intvaluemacros.h
--rw-r--r--   0 jmadden    (501) staff       (20)     1657 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/objectkeymacros.h
--rw-r--r--   0 jmadden    (501) staff       (20)      460 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/objectvaluemacros.h
--rw-r--r--   0 jmadden    (501) staff       (20)    15218 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/sorters.c
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2021-06-09 10:40:19.168358 BTrees-4.9.2/src/BTrees/tests/
--rw-r--r--   0 jmadden    (501) staff       (20)       23 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/tests/__init__.py
--rw-r--r--   0 jmadden    (501) staff       (20)    11342 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/tests/_test_builder.py
--rw-r--r--   0 jmadden    (501) staff       (20)   123801 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/tests/common.py
--rw-r--r--   0 jmadden    (501) staff       (20)    17877 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/tests/testBTrees.py
--rw-r--r--   0 jmadden    (501) staff       (20)     2939 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/tests/testBTreesUnicode.py
--rw-r--r--   0 jmadden    (501) staff       (20)    21207 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/tests/testConflict.py
--rw-r--r--   0 jmadden    (501) staff       (20)     1635 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/tests/testPersistency.py
--rw-r--r--   0 jmadden    (501) staff       (20)     3440 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/tests/test_Length.py
--rw-r--r--   0 jmadden    (501) staff       (20)     5828 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/tests/test_OOBTree.py
--rw-r--r--   0 jmadden    (501) staff       (20)   111017 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/tests/test__base.py
--rw-r--r--   0 jmadden    (501) staff       (20)     3126 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/tests/test__datatypes.py
--rw-r--r--   0 jmadden    (501) staff       (20)     2557 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/tests/test_btreesubclass.py
--rw-r--r--   0 jmadden    (501) staff       (20)    12591 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/tests/test_check.py
--rw-r--r--   0 jmadden    (501) staff       (20)     1791 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/tests/test_dynamic_btrees.py
--rw-r--r--   0 jmadden    (501) staff       (20)     2372 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/tests/test_fsBTree.py
--rw-r--r--   0 jmadden    (501) staff       (20)     2556 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/tests/test_utils.py
--rw-r--r--   0 jmadden    (501) staff       (20)     1835 2021-06-09 10:40:18.000000 BTrees-4.9.2/src/BTrees/utils.py
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2021-06-09 10:40:19.162244 BTrees-4.9.2/src/BTrees.egg-info/
--rw-r--r--   0 jmadden    (501) staff       (20)    23199 2021-06-09 10:40:19.000000 BTrees-4.9.2/src/BTrees.egg-info/PKG-INFO
--rw-r--r--   0 jmadden    (501) staff       (20)     2303 2021-06-09 10:40:19.000000 BTrees-4.9.2/src/BTrees.egg-info/SOURCES.txt
--rw-r--r--   0 jmadden    (501) staff       (20)        1 2021-06-09 10:40:19.000000 BTrees-4.9.2/src/BTrees.egg-info/dependency_links.txt
--rw-r--r--   0 jmadden    (501) staff       (20)        6 2021-06-09 10:40:19.000000 BTrees-4.9.2/src/BTrees.egg-info/entry_points.txt
--rw-r--r--   0 jmadden    (501) staff       (20)        1 2021-06-09 10:40:19.000000 BTrees-4.9.2/src/BTrees.egg-info/not-zip-safe
--rw-r--r--   0 jmadden    (501) staff       (20)      169 2021-06-09 10:40:19.000000 BTrees-4.9.2/src/BTrees.egg-info/requires.txt
--rw-r--r--   0 jmadden    (501) staff       (20)        7 2021-06-09 10:40:19.000000 BTrees-4.9.2/src/BTrees.egg-info/top_level.txt
--rw-r--r--   0 jmadden    (501) staff       (20)     1308 2021-06-09 10:40:18.000000 BTrees-4.9.2/tox.ini
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-02-10 15:12:07.936051 BTrees-5.0/
+-rw-r--r--   0 mac        (513) staff       (20)      580 2023-02-10 15:12:00.000000 BTrees-5.0/.coveragerc
+-rwxr-xr-x   0 mac        (513) staff       (20)     3008 2023-02-10 15:12:00.000000 BTrees-5.0/.manylinux-install.sh
+-rwxr-xr-x   0 mac        (513) staff       (20)      509 2023-02-10 15:12:00.000000 BTrees-5.0/.manylinux.sh
+-rw-r--r--   0 mac        (513) staff       (20)    17441 2023-02-10 15:12:00.000000 BTrees-5.0/CHANGES.rst
+-rw-r--r--   0 mac        (513) staff       (20)      799 2023-02-10 15:12:00.000000 BTrees-5.0/CONTRIBUTING.md
+-rw-r--r--   0 mac        (513) staff       (20)       32 2023-02-10 15:12:00.000000 BTrees-5.0/COPYRIGHT.txt
+-rw-r--r--   0 mac        (513) staff       (20)     2070 2023-02-10 15:12:00.000000 BTrees-5.0/LICENSE.txt
+-rw-r--r--   0 mac        (513) staff       (20)      474 2023-02-10 15:12:00.000000 BTrees-5.0/MANIFEST.in
+-rw-r--r--   0 mac        (513) staff       (20)    20266 2023-02-10 15:12:07.936264 BTrees-5.0/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)     1468 2023-02-10 15:12:00.000000 BTrees-5.0/README.rst
+-rw-r--r--   0 mac        (513) staff       (20)     1777 2023-02-10 15:12:00.000000 BTrees-5.0/appveyor.yml
+-rw-r--r--   0 mac        (513) staff       (20)      833 2023-02-10 15:12:00.000000 BTrees-5.0/buildout.cfg
+-rw-r--r--   0 mac        (513) staff       (20)       89 2023-02-10 15:12:00.000000 BTrees-5.0/doc-requirements.txt
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-02-10 15:12:07.910760 BTrees-5.0/docs/
+-rw-r--r--   0 mac        (513) staff       (20)     5564 2023-02-10 15:12:00.000000 BTrees-5.0/docs/Makefile
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-02-10 15:12:07.911387 BTrees-5.0/docs/_static/
+-rw-r--r--   0 mac        (513) staff       (20)      363 2023-02-10 15:12:00.000000 BTrees-5.0/docs/_static/custom.css
+-rw-r--r--   0 mac        (513) staff       (20)        0 2023-02-10 15:12:00.000000 BTrees-5.0/docs/_static/placeholder.txt
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-02-10 15:12:07.911585 BTrees-5.0/docs/_templates/
+-rw-r--r--   0 mac        (513) staff       (20)        0 2023-02-10 15:12:00.000000 BTrees-5.0/docs/_templates/placeholder.txt
+-rw-r--r--   0 mac        (513) staff       (20)     3599 2023-02-10 15:12:00.000000 BTrees-5.0/docs/api.rst
+-rw-r--r--   0 mac        (513) staff       (20)       28 2023-02-10 15:12:00.000000 BTrees-5.0/docs/changes.rst
+-rw-r--r--   0 mac        (513) staff       (20)     8990 2023-02-10 15:12:00.000000 BTrees-5.0/docs/conf.py
+-rw-r--r--   0 mac        (513) staff       (20)    17124 2023-02-10 15:12:00.000000 BTrees-5.0/docs/development.rst
+-rw-r--r--   0 mac        (513) staff       (20)      533 2023-02-10 15:12:00.000000 BTrees-5.0/docs/index.rst
+-rw-r--r--   0 mac        (513) staff       (20)     5096 2023-02-10 15:12:00.000000 BTrees-5.0/docs/make.bat
+-rw-r--r--   0 mac        (513) staff       (20)    21780 2023-02-10 15:12:00.000000 BTrees-5.0/docs/overview.rst
+-rw-r--r--   0 mac        (513) staff       (20)       88 2023-02-10 15:12:00.000000 BTrees-5.0/pyproject.toml
+-rw-r--r--   0 mac        (513) staff       (20)      562 2023-02-10 15:12:07.937209 BTrees-5.0/setup.cfg
+-rw-r--r--   0 mac        (513) staff       (20)     7580 2023-02-10 15:12:00.000000 BTrees-5.0/setup.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-02-10 15:12:07.902955 BTrees-5.0/src/
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-02-10 15:12:07.927977 BTrees-5.0/src/BTrees/
+-rw-r--r--   0 mac        (513) staff       (20)    24543 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/BTreeItemsTemplate.c
+-rw-r--r--   0 mac        (513) staff       (20)    24056 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/BTreeModuleTemplate.c
+-rw-r--r--   0 mac        (513) staff       (20)    75422 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/BTreeTemplate.c
+-rw-r--r--   0 mac        (513) staff       (20)    54931 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/BucketTemplate.c
+-rw-r--r--   0 mac        (513) staff       (20)    23750 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/Interfaces.py
+-rw-r--r--   0 mac        (513) staff       (20)     1937 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/Length.py
+-rw-r--r--   0 mac        (513) staff       (20)    12070 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/MergeTemplate.c
+-rw-r--r--   0 mac        (513) staff       (20)    17264 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/SetOpTemplate.c
+-rw-r--r--   0 mac        (513) staff       (20)      281 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/SetOpTemplate.h
+-rw-r--r--   0 mac        (513) staff       (20)    19964 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/SetTemplate.c
+-rw-r--r--   0 mac        (513) staff       (20)    17788 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/TreeSetTemplate.c
+-rw-r--r--   0 mac        (513) staff       (20)     1010 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/_IFBTree.c
+-rw-r--r--   0 mac        (513) staff       (20)     1004 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/_IIBTree.c
+-rw-r--r--   0 mac        (513) staff       (20)      984 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/_IOBTree.c
+-rw-r--r--   0 mac        (513) staff       (20)     1047 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/_IUBTree.c
+-rw-r--r--   0 mac        (513) staff       (20)     1082 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/_LFBTree.c
+-rw-r--r--   0 mac        (513) staff       (20)     1073 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/_LLBTree.c
+-rw-r--r--   0 mac        (513) staff       (20)     1053 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/_LOBTree.c
+-rw-r--r--   0 mac        (513) staff       (20)     1115 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/_LQBTree.c
+-rw-r--r--   0 mac        (513) staff       (20)      984 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/_OIBTree.c
+-rw-r--r--   0 mac        (513) staff       (20)     1053 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/_OLBTree.c
+-rw-r--r--   0 mac        (513) staff       (20)      993 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/_OOBTree.c
+-rw-r--r--   0 mac        (513) staff       (20)     1091 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/_OQBTree.c
+-rw-r--r--   0 mac        (513) staff       (20)     1023 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/_OUBTree.c
+-rw-r--r--   0 mac        (513) staff       (20)     1118 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/_QFBTree.c
+-rw-r--r--   0 mac        (513) staff       (20)     1113 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/_QLBTree.c
+-rw-r--r--   0 mac        (513) staff       (20)     1089 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/_QOBTree.c
+-rw-r--r--   0 mac        (513) staff       (20)     1147 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/_QQBTree.c
+-rw-r--r--   0 mac        (513) staff       (20)     1050 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/_UFBTree.c
+-rw-r--r--   0 mac        (513) staff       (20)     1044 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/_UIBTree.c
+-rw-r--r--   0 mac        (513) staff       (20)     1032 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/_UOBTree.c
+-rw-r--r--   0 mac        (513) staff       (20)     1086 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/_UUBTree.c
+-rw-r--r--   0 mac        (513) staff       (20)     4169 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)    52664 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/_base.py
+-rw-r--r--   0 mac        (513) staff       (20)     1163 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/_compat.h
+-rw-r--r--   0 mac        (513) staff       (20)     4072 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/_compat.py
+-rw-r--r--   0 mac        (513) staff       (20)    13555 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/_datatypes.py
+-rw-r--r--   0 mac        (513) staff       (20)     4673 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/_fsBTree.c
+-rw-r--r--   0 mac        (513) staff       (20)     7787 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/_module_builder.py
+-rw-r--r--   0 mac        (513) staff       (20)    17421 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/check.py
+-rw-r--r--   0 mac        (513) staff       (20)      899 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/floatvaluemacros.h
+-rw-r--r--   0 mac        (513) staff       (20)     4072 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/intkeymacros.h
+-rw-r--r--   0 mac        (513) staff       (20)     4574 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/intvaluemacros.h
+-rw-r--r--   0 mac        (513) staff       (20)     1193 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/objectkeymacros.h
+-rw-r--r--   0 mac        (513) staff       (20)      460 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/objectvaluemacros.h
+-rw-r--r--   0 mac        (513) staff       (20)    15218 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/sorters.c
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-02-10 15:12:07.935850 BTrees-5.0/src/BTrees/tests/
+-rw-r--r--   0 mac        (513) staff       (20)       23 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/tests/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)    11291 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/tests/_test_builder.py
+-rw-r--r--   0 mac        (513) staff       (20)   122582 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/tests/common.py
+-rw-r--r--   0 mac        (513) staff       (20)    17867 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/tests/testBTrees.py
+-rw-r--r--   0 mac        (513) staff       (20)    21207 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/tests/testConflict.py
+-rw-r--r--   0 mac        (513) staff       (20)     1629 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/tests/testPersistency.py
+-rw-r--r--   0 mac        (513) staff       (20)     2462 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/tests/test_Length.py
+-rw-r--r--   0 mac        (513) staff       (20)     5514 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/tests/test_OOBTree.py
+-rw-r--r--   0 mac        (513) staff       (20)   110865 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/tests/test__base.py
+-rw-r--r--   0 mac        (513) staff       (20)     3126 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/tests/test__datatypes.py
+-rw-r--r--   0 mac        (513) staff       (20)     2557 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/tests/test_btreesubclass.py
+-rw-r--r--   0 mac        (513) staff       (20)    12511 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/tests/test_check.py
+-rw-r--r--   0 mac        (513) staff       (20)     1295 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/tests/test_compile_flags.py
+-rw-r--r--   0 mac        (513) staff       (20)     1791 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/tests/test_dynamic_btrees.py
+-rw-r--r--   0 mac        (513) staff       (20)     2372 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/tests/test_fsBTree.py
+-rw-r--r--   0 mac        (513) staff       (20)     2348 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/tests/test_utils.py
+-rw-r--r--   0 mac        (513) staff       (20)     1798 2023-02-10 15:12:00.000000 BTrees-5.0/src/BTrees/utils.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-02-10 15:12:07.929639 BTrees-5.0/src/BTrees.egg-info/
+-rw-r--r--   0 mac        (513) staff       (20)    20266 2023-02-10 15:12:07.000000 BTrees-5.0/src/BTrees.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)     2291 2023-02-10 15:12:07.000000 BTrees-5.0/src/BTrees.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-02-10 15:12:07.000000 BTrees-5.0/src/BTrees.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-02-10 15:12:07.000000 BTrees-5.0/src/BTrees.egg-info/not-zip-safe
+-rw-r--r--   0 mac        (513) staff       (20)      167 2023-02-10 15:12:07.000000 BTrees-5.0/src/BTrees.egg-info/requires.txt
+-rw-r--r--   0 mac        (513) staff       (20)        7 2023-02-10 15:12:07.000000 BTrees-5.0/src/BTrees.egg-info/top_level.txt
+-rw-r--r--   0 mac        (513) staff       (20)     1503 2023-02-10 15:12:00.000000 BTrees-5.0/tox.ini
```

### Comparing `BTrees-4.9.2/CHANGES.rst` & `BTrees-5.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,58 @@
 ==================
  BTrees Changelog
 ==================
 
+5.0 (2023-02-10)
+================
+
+- Build Linux binary wheels for Python 3.11.
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+
+4.11.3 (2022-11-17)
+===================
+
+- point release to rebuild full set of wheels
+
+
+4.11.2 (2022-11-16)
+===================
+
+- Add support for building arm64 wheels on macOS.
+
+
+4.11.1 (2022-11-09)
+===================
+
+- Fix macOS wheel build issues on GitHub Actions
+
+- We no longer provide 32bit wheels for the Windows platform, only x86_64.
+
+
+4.11.0 (2022-11-03)
+===================
+
+- Add support for Python 3.11.
+
+
+4.10.1 (2022-09-12)
+===================
+
+- Disable unsafe math optimizations in C code.
+  (`#184 <https://github.com/zopefoundation/BTrees/pull/184>`_)
+
+
+4.10.0 (2022-03-09)
+===================
+
+- Add support for Python 3.10.
+
+
 4.9.2 (2021-06-09)
 ==================
 
 - Fix ``fsBTree.TreeSet`` and ``fsBTree.BTree`` raising
   ``SystemError``. See `issue 170 <https://github.com/zopefoundation/BTrees/issues/170>`_.
 
 - Fix all the ``fsBTree`` objects to provide the correct interfaces
```

### Comparing `BTrees-4.9.2/LICENSE.txt` & `BTrees-5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `BTrees-4.9.2/README.rst` & `BTrees-5.0/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,33 @@
-=========================================
- BTrees:  scalable persistent components
-=========================================
+=============================================
+ ``BTrees``:  scalable persistent components
+=============================================
 
 .. image:: https://github.com/zopefoundation/BTrees/actions/workflows/tests.yml/badge.svg
     :target: https://github.com/zopefoundation/BTrees/actions/workflows/tests.yml
 
 .. image:: https://ci.appveyor.com/api/projects/status/github/zopefoundation/BTrees?branch=master&svg=true
     :target: https://ci.appveyor.com/project/mgedmin/BTrees
 
 .. image:: https://coveralls.io/repos/github/zopefoundation/BTrees/badge.svg?branch=master
     :target: https://coveralls.io/github/zopefoundation/BTrees?branch=master
 
+.. image:: https://readthedocs.org/projects/btrees/badge/?version=latest
+        :target: https://btrees.readthedocs.io/en/latest/
+        :alt: Documentation Status
+
 .. image:: https://img.shields.io/pypi/v/BTrees.svg
         :target: https://pypi.org/project/BTrees/
         :alt: Current version on PyPI
 
 .. image:: https://img.shields.io/pypi/pyversions/BTrees.svg
         :target: https://pypi.org/project/BTrees/
         :alt: Supported Python versions
 
 
 This package contains a set of persistent object containers built around
 a modified BTree data structure.  The trees are optimized for use inside
 ZODB's "optimistic concurrency" paradigm, and include explicit resolution
 of conflicts detected by that mechanism.
 
-Please see `the Sphinx documentation <http://btrees.readthedocs.io/>`_ for further
-information.
+Please see `the Sphinx documentation <https://btrees.readthedocs.io/>`_ for
+further information.
```

### Comparing `BTrees-4.9.2/buildout.cfg` & `BTrees-5.0/buildout.cfg`

 * *Files identical despite different names*

### Comparing `BTrees-4.9.2/docs/Makefile` & `BTrees-5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `BTrees-4.9.2/docs/api.rst` & `BTrees-5.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `BTrees-4.9.2/docs/conf.py` & `BTrees-5.0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,10 +272,10 @@
 #texinfo_show_urls = 'footnote'
 
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
     'https://docs.python.org/3/': None,
     'https://persistent.readthedocs.io/en/latest/': None,
-    "https://zodb.readthedocs.io/en/latest/": None,
+    "https://zodb.org/en/latest/": None,
     "https://zopeinterface.readthedocs.io/en/latest/": None,
 }
```

### Comparing `BTrees-4.9.2/docs/development.rst` & `BTrees-5.0/docs/development.rst`

 * *Files identical despite different names*

### Comparing `BTrees-4.9.2/docs/index.rst` & `BTrees-5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `BTrees-4.9.2/docs/make.bat` & `BTrees-5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `BTrees-4.9.2/docs/overview.rst` & `BTrees-5.0/docs/overview.rst`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
    >>> t.update({1: "red", 2: "green", 3: "blue", 4: "spades"})
    >>> len(t)
    4
    >>> t[2]
    'green'
    >>> s = t.keys() # this is a "lazy" sequence object
    >>> s
-   <OOBTreeItems object at ...>
+   <...TreeItems object at ...>
    >>> len(s)  # it acts like a Python list
    4
    >>> s[-2]
    3
    >>> list(s) # materialize the full list
    [1, 2, 3, 4]
    >>> list(t.values())
@@ -256,17 +256,18 @@
    >>> list(s.keys())           # note that the lists are in sorted order
    [[1], [2], [3]]
    >>> s.has_key([3])           # and [3] is in the set
    True
    >>> L2[0] = 5                # horrible -- the set is insane now
    >>> s.has_key([3])           # for example, it's insane this way
    False
-   >>> s
-   OOSet([[1], [5], [3]])
-   >>>
+   >>> s.__class__
+   <class 'BTrees.OOBTree.OOSet'>
+   >>> list(s)
+   [[1], [5], [3]]
 
 Key lookup relies on that the keys remain in sorted order (an efficient form of
 binary search is used).  By mutating key L2 after inserting it, we destroyed the
 invariant that the OOSet is sorted.  As a result, all future operations on this
 set are unpredictable.
 
 A subtler variant of this problem arises due to persistence:  by default, Python
```

### Comparing `BTrees-4.9.2/setup.py` & `BTrees-5.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,29 +7,28 @@
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
-from __future__ import print_function
 
 import os
 import sys
 
 from distutils.errors import CCompilerError
 from distutils.errors import DistutilsExecError
 from distutils.errors import DistutilsPlatformError
 
 from setuptools import Extension
 from setuptools import find_packages
 from setuptools import setup
 from setuptools.command.build_ext import build_ext
 
-version = '4.9.2'
+version = '5.0'
 
 def _read(fname):
     here = os.path.abspath(os.path.dirname(__file__))
     with open(os.path.join(here, fname)) as f:
         return f.read()
 
 
@@ -67,15 +66,15 @@
             raise
 
 # Include directories for C extensions
 # Sniff the location of the headers in 'persistent' or fall back
 # to local headers in the include sub-directory
 
 
-class ModuleHeaderDir(object):
+class ModuleHeaderDir:
 
     def __init__(self, require_spec, where='..'):
         # By default, assume top-level pkg has the same name as the dist.
         # Also assume that headers are located in the package dir, and
         # are meant to be included as follows:
         #    #include "module/header_name.h"
         self._require_spec = require_spec
@@ -185,55 +184,58 @@
       version=version,
       description='Scalable persistent object containers',
       long_description=README,
       classifiers=[
           "Development Status :: 6 - Mature",
           "License :: OSI Approved :: Zope Public License",
           "Programming Language :: Python",
-          "Programming Language :: Python :: 2",
-          "Programming Language :: Python :: 2.7",
           "Programming Language :: Python :: 3",
-          "Programming Language :: Python :: 3.5",
-          "Programming Language :: Python :: 3.6",
           "Programming Language :: Python :: 3.7",
           "Programming Language :: Python :: 3.8",
           "Programming Language :: Python :: 3.9",
+          "Programming Language :: Python :: 3.10",
+          "Programming Language :: Python :: 3.11",
           "Programming Language :: Python :: Implementation :: CPython",
           "Programming Language :: Python :: Implementation :: PyPy",
           "Framework :: ZODB",
           "Topic :: Database",
           "Topic :: Software Development :: Libraries :: Python Modules",
           "Operating System :: Microsoft :: Windows",
           "Operating System :: Unix",
       ],
       author="Zope Foundation",
       author_email="zodb-dev@zope.org",
       url="https://github.com/zopefoundation/BTrees",
+      project_urls={
+        'Documentation': 'https://btrees.readthedocs.io',
+        'Issue Tracker': 'https://github.com/zopefoundation/BTrees/issues',
+        'Sources': 'https://github.com/zopefoundation/BTrees',
+      },
       license="ZPL 2.1",
       platforms=["any"],
       packages=find_packages('src'),
       package_dir={'': 'src'},
       include_package_data=True,
       zip_safe=False,
       ext_modules=ext_modules,
       setup_requires=['persistent'],
       extras_require={
           'test': TESTS_REQUIRE,
           'ZODB': [
               'ZODB',
           ],
           'docs': [
-              # Sphinx 4 and r.s.autointerface 0.8 are incompatible.
-              'Sphinx < 4',
+              'Sphinx',
               'repoze.sphinx.autointerface',
               'sphinx_rtd_theme',
           ],
       },
       test_suite="BTrees.tests",
       tests_require=TESTS_REQUIRE,
+      python_requires='>=3.7',
       install_requires=REQUIRES,
       cmdclass={
           'build_ext': optional_build_ext,
       },
       entry_points="""\
       """
 )
```

### Comparing `BTrees-4.9.2/src/BTrees/BTreeItemsTemplate.c` & `BTrees-5.0/src/BTrees/BTreeItemsTemplate.c`

 * *Files 1% similar despite different names*

```diff
@@ -422,19 +422,15 @@
             i += len;
         return BTreeItems_item(self, i);
     }
     if (PySlice_Check(subscript))
     {
         Py_ssize_t start, stop, step, slicelength;
 
-#ifdef PY3K
 #define SLICEOBJ(x) (x)
-#else
-#define SLICEOBJ(x) (PySliceObject*)(x)
-#endif
 
         if (PySlice_GetIndicesEx(SLICEOBJ(subscript), len,
                                  &start, &stop, &step, &slicelength) < 0)
         {
             return NULL;
         }
 
@@ -459,35 +455,28 @@
 
 static PySequenceMethods BTreeItems_as_sequence =
 {
     (lenfunc) BTreeItems_length,            /* sq_length */
     (binaryfunc)0,                          /* sq_concat */
     (ssizeargfunc)0,                        /* sq_repeat */
     (ssizeargfunc) BTreeItems_item,         /* sq_item */
-#ifndef PY3K
-    /* Py3K doesn't honor this slot */
-    (ssizessizeargfunc) BTreeItems_slice,   /* sq_slice */
-#endif
 };
 
 /* Number Method items (just for nb_nonzero!) */
 
 static int
 BTreeItems_nonzero(BTreeItems *self)
 {
     return BTreeItems_length_or_nonzero(self, 1);
 }
 
 static PyNumberMethods BTreeItems_as_number_for_nonzero = {
     0,                                      /* nb_add */
     0,                                      /* nb_subtract */
     0,                                      /* nb_multiply */
-#ifndef PY3K
-    0,                                      /* nb_divide */
-#endif
     0,                                      /* nb_remainder */
     0,                                      /* nb_divmod */
     0,                                      /* nb_power */
     0,                                      /* nb_negative */
     0,                                      /* nb_positive */
     0,                                      /* nb_absolute */
    (inquiry)BTreeItems_nonzero              /* nb_nonzero */
@@ -642,15 +631,15 @@
             i->position = -1;
             PyErr_Clear();
         }
     }
     return 0;
 }
 
-/* Support for the iteration protocol new in Python 2.2. */
+/* Support for the iteration protocol */
 
 static PyTypeObject BTreeIter_Type;
 
 /* The type of iterator objects, returned by e.g. iter(IIBTree()). */
 typedef struct
 {
     PyObject_HEAD
```

### Comparing `BTrees-4.9.2/src/BTrees/BTreeModuleTemplate.c` & `BTrees-5.0/src/BTrees/BTreeModuleTemplate.c`

 * *Files 6% similar despite different names*

```diff
@@ -80,16 +80,16 @@
 
 static int
 longlong_handle_overflow(PY_LONG_LONG result, int overflow)
 {
     if (overflow)
     {
         PyErr_Clear();
-        /* Python 3 tends to have an exception already set, Python 2 not so
-           much. We want to consistently raise a TypeError.
+        /* Python 3 tends to have an exception already set.
+           We want to consistently raise a TypeError.
         */
         PyErr_SetString(PyExc_TypeError, "couldn't convert integer to C long long");
         return 0;
     }
     else if (result == -1 && PyErr_Occurred())
         /* An exception has already been raised. */
         return 0;
@@ -99,27 +99,14 @@
 
 #ifdef NEED_LONG_LONG_KEYS
 
 #if defined(ZODB_UNSIGNED_VALUE_INTS) || defined(ZODB_UNSIGNED_KEY_INTS)
 static int
 ulonglong_check(PyObject *ob)
 {
-#ifndef PY3K
-    if (PyInt_Check(ob))
-    {
-        long tmp;
-        tmp = PyInt_AS_LONG(ob);
-        if (tmp < 0) {
-            PyErr_SetString(PyExc_TypeError, "unsigned value less than 0");
-            return 0;
-        }
-        return 1;
-    }
-#endif
-
     if (!PyLong_Check(ob))
     {
         return 0;
     }
 
     if (PyLong_AsUnsignedLongLong(ob) == (unsigned long long)-1 && PyErr_Occurred())
     {
@@ -128,20 +115,14 @@
     return 1;
 }
 #endif /* defined(ZODB_UNSIGNED_VALUE_INTS) || defined(ZODB_UNSIGNED_KEY_INTS) */
 
 static int
 longlong_check(PyObject *ob)
 {
-#ifndef PY3K
-    /* Python's small integers can always fit into a long long. */
-    if (PyInt_Check(ob))
-        return 1;
-#endif
-
     if (PyLong_Check(ob)) {
         int overflow;
         PY_LONG_LONG result;
         result = PyLong_AsLongLongAndOverflow(ob, &overflow);
         return longlong_handle_overflow(result, overflow);
     }
     return 0;
@@ -159,28 +140,14 @@
 }
 
 static int
 ulonglong_convert(PyObject *ob, unsigned PY_LONG_LONG *value)
 {
     unsigned PY_LONG_LONG val;
 
-#ifndef PY3K
-    if (PyInt_Check(ob))
-    {
-        long tmp;
-        tmp = PyInt_AS_LONG(ob);
-        if (tmp < 0) {
-            PyErr_SetString(PyExc_TypeError, "unsigned value less than 0");
-            return 0;
-        }
-        (*value) = (unsigned PY_LONG_LONG)tmp;
-        return 1;
-    }
-#endif
-
     if (!PyLong_Check(ob))
     {
         PyErr_SetString(PyExc_TypeError, "expected integer key");
         return 0;
     }
 
     val = PyLong_AsUnsignedLongLong(ob);
@@ -207,21 +174,14 @@
 }
 
 static int
 longlong_convert(PyObject *ob, PY_LONG_LONG *value)
 {
     PY_LONG_LONG val;
     int overflow;
-#ifndef PY3K
-    if (PyInt_Check(ob))
-    {
-        (*value) = (PY_LONG_LONG)PyInt_AS_LONG(ob);
-        return 1;
-    }
-#endif
 
     if (!PyLong_Check(ob))
     {
         PyErr_SetString(PyExc_TypeError, "expected integer key");
         return 0;
     }
     val = PyLong_AsLongLongAndOverflow(ob, &overflow);
@@ -586,19 +546,15 @@
 ;
 
 static int
 init_type_with_meta_base(PyTypeObject *type, PyTypeObject* meta, PyTypeObject* base)
 {
     int result;
     PyObject* slotnames;
-#ifdef PY3K
     ((PyObject*)type)->ob_type = meta;
-#else
-    type->ob_type = meta;
-#endif
     type->tp_base = base;
 
     if (PyType_Ready(type) < 0)
         return 0;
     /*
       persistent looks for __slotnames__ in the dict at deactivation time,
       and if it's not present, calls ``copyreg._slotnames``, which itself
@@ -628,29 +584,26 @@
     }
     if (PyDict_SetItem(type->tp_dict, _bucket_type_str, (PyObject*)bucket_type) < 0) {
         return 0;
     }
     return 1;
 }
 
-#ifdef PY3K
 static struct PyModuleDef moduledef = {
         PyModuleDef_HEAD_INIT,
         "_" MOD_NAME_PREFIX "BTree",    /* m_name */
         BTree_module_documentation,     /* m_doc */
         -1,                             /* m_size */
         module_methods,                 /* m_methods */
         NULL,                           /* m_reload */
         NULL,                           /* m_traverse */
         NULL,                           /* m_clear */
         NULL,                           /* m_free */
     };
 
-#endif
-
 static PyObject*
 module_init(void)
 {
     PyObject *module, *mod_dict, *interfaces, *conflicterr;
 
 #ifdef KEY_TYPE_IS_PYOBJECT
     object_ = PyTuple_GetItem(Py_TYPE(Py_None)->tp_bases, 0);
@@ -709,39 +662,30 @@
     if (ConflictError == NULL)
     {
         Py_INCREF(PyExc_ValueError);
         ConflictError=PyExc_ValueError;
     }
 
     /* Initialize the PyPersist_C_API and the type objects. */
-#ifdef PY3K
     cPersistenceCAPI = (cPersistenceCAPIstruct *)PyCapsule_Import(
                 "persistent.cPersistence.CAPI", 0);
-#else
-    cPersistenceCAPI = (cPersistenceCAPIstruct *)PyCObject_Import(
-                "persistent.cPersistence", "CAPI");
-#endif
     if (cPersistenceCAPI == NULL) {
        /* The Capsule API attempts to import 'persistent' and then
         * walk down to the specified attribute using getattr. If the C
         * extensions aren't available, this can result in an
         * AttributeError being raised. Let that percolate up as an
         * ImportError so it can be caught in the expected way.
         */
        if (PyErr_Occurred() && !PyErr_ExceptionMatches(PyExc_ImportError)) {
            PyErr_SetString(PyExc_ImportError, "persistent C extension unavailable");
        }
         return NULL;
    }
 
-#ifdef PY3K
 #define _SET_TYPE(typ) ((PyObject*)(&typ))->ob_type = &PyType_Type
-#else
-#define _SET_TYPE(typ) (typ).ob_type = &PyType_Type
-#endif
     _SET_TYPE(BTreeItemsType);
     _SET_TYPE(BTreeIter_Type);
     BTreeIter_Type.tp_getattro = PyObject_GenericGetAttr;
     BucketType.tp_new = PyType_GenericNew;
     SetType.tp_new = PyType_GenericNew;
     BTreeType.tp_new = PyType_GenericNew;
     TreeSetType.tp_new = PyType_GenericNew;
@@ -761,21 +705,15 @@
         return NULL;
 
     if (!init_tree_type(&TreeSetType, &SetType)) {
         return NULL;
     }
 
     /* Create the module and add the functions */
-#ifdef PY3K
     module = PyModule_Create(&moduledef);
-#else
-    module = Py_InitModule4("_" MOD_NAME_PREFIX "BTree",
-                       module_methods, BTree_module_documentation,
-                       (PyObject *)NULL, PYTHON_API_VERSION);
-#endif
 
     /* Add some symbolic constants to the module */
     mod_dict = PyModule_GetDict(module);
 
     if (PyDict_SetItemString(mod_dict, MOD_NAME_PREFIX "Bucket",
                              (PyObject *)&BucketType) < 0)
         return NULL;
@@ -817,18 +755,11 @@
 #else
     if (PyDict_SetItemString(mod_dict, "using64bits", Py_False) < 0)
         return NULL;
 #endif
     return module;
 }
 
-#ifdef PY3K
 PyMODINIT_FUNC INITMODULE(void)
 {
     return module_init();
 }
-#else
-PyMODINIT_FUNC INITMODULE(void)
-{
-    module_init();
-}
-#endif
```

### Comparing `BTrees-4.9.2/src/BTrees/BTreeTemplate.c` & `BTrees-5.0/src/BTrees/BTreeTemplate.c`

 * *Files 0% similar despite different names*

```diff
@@ -22,19 +22,15 @@
   long isize;
   size = PyObject_GetAttr(OBJECT(OBJECT(self)->ob_type), name);
   if (size == NULL) {
       PyErr_Clear();
       return default_max;
   }
 
-#ifdef PY3K
   isize = PyLong_AsLong(size);
-#else
-  isize = PyInt_AsLong(size);
-#endif
 
   Py_DECREF(size);
   if (isize <= 0 && ! PyErr_Occurred()) {
     PyErr_SetString(PyExc_ValueError,
                     "non-positive max size in BTree subclass");
     return -1;
   }
@@ -2482,17 +2478,14 @@
   return BTree_length_or_nonzero(self, 1);
 }
 
 static PyNumberMethods BTree_as_number_for_nonzero = {
     0,                                      /* nb_add */
     bucket_sub,                             /* nb_subtract */
     0,                                      /* nb_multiply */
-#ifndef PY3K
-    0,                                      /* nb_divide */
-#endif
     0,                                      /* nb_remainder */
     0,                                      /* nb_divmod */
     0,                                      /* nb_power */
     0,                                      /* nb_negative */
     0,                                      /* nb_positive */
     0,                                      /* nb_absolute */
     (inquiry)BTree_nonzero,                 /* nb_nonzero */
@@ -2551,17 +2544,14 @@
     0, /* tp_as_mapping */
     0, /* tp_hash */
     0, /* tp_call */
     0, /* tp_str */
     0, /* tp_getattro */
     (setattrofunc)BTreeType_setattro, /* tp_setattro */
     0, /* tp_as_buffer */
-#ifndef PY3K
-    Py_TPFLAGS_CHECKTYPES |
-#endif
     Py_TPFLAGS_DEFAULT |
     Py_TPFLAGS_BASETYPE, /* tp_flags */
     0, /* tp_doc */
     0, /* tp_traverse */
     0, /* tp_clear */
     0, /* tp_richcompare */
     0, /* tp_weaklistoffset */
@@ -2587,17 +2577,14 @@
     &BTree_as_mapping,                      /* tp_as_mapping */
     0,                                      /* tp_hash */
     0,                                      /* tp_call */
     0,                                      /* tp_str */
     0,                                      /* tp_getattro */
     0,                                      /* tp_setattro */
     0,                                      /* tp_as_buffer */
-#ifndef PY3K
-    Py_TPFLAGS_CHECKTYPES |
-#endif
     Py_TPFLAGS_DEFAULT |
     Py_TPFLAGS_HAVE_GC |
     Py_TPFLAGS_BASETYPE,                    /* tp_flags */
     0,                                      /* tp_doc */
     (traverseproc)BTree_traverse,           /* tp_traverse */
     (inquiry)BTree_tp_clear,                /* tp_clear */
     0,                                      /* tp_richcompare */
```

### Comparing `BTrees-4.9.2/src/BTrees/BucketTemplate.c` & `BTrees-5.0/src/BTrees/BucketTemplate.c`

 * *Files 1% similar despite different names*

```diff
@@ -507,22 +507,16 @@
         INCREF of the seq argument.  So seq must always be DECREFed on
         the way out.
     */
     /* Use items() if it's not a sequence.  Alas, PySequence_Check()
      * returns true for a PeristentMapping or PersistentDict, and we
      * want to use items() in those cases too.
      */
-#ifdef PY3K
-#define ITERITEMS "items"
-#else
-#define ITERITEMS "iteritems"
-#endif
     if (!PySequence_Check(seq) || /* or it "looks like a dict" */
-        PyObject_HasAttrString(seq, ITERITEMS))
-#undef ITERITEMS
+        PyObject_HasAttrString(seq, "items"))
     {
         PyObject *items;
         items = PyObject_GetAttrString(seq, "items");
         if (items == NULL)
             return -1;
         seq = PyObject_CallObject(items, NULL);
         Py_DECREF(items);
@@ -1906,17 +1900,14 @@
     0,                                  /* sq_inplace_repeat */
 };
 
 static PyNumberMethods Bucket_as_number = {
      (binaryfunc)0,                     /* nb_add */
      bucket_sub,                        /* nb_subtract */
      (binaryfunc)0,                     /* nb_multiply */
-#ifndef PY3K
-     0,                                 /* nb_divide */
-#endif
      (binaryfunc)0,                     /* nb_remainder */
      (binaryfunc)0,                     /* nb_divmod */
      (ternaryfunc)0,                    /* nb_power */
      (unaryfunc)0,                      /* nb_negative */
      (unaryfunc)0,                      /* nb_positive */
      (unaryfunc)0,                      /* nb_absolute */
      (inquiry)0,                        /* nb_bool */
@@ -1929,61 +1920,23 @@
 };
 
 
 static PyObject *
 bucket_repr(Bucket *self)
 {
     PyObject *i, *r;
-#ifndef PY3K
-    char repr[10000];
-    int rv;
-#endif
 
     i = bucket_items(self, NULL, NULL);
     if (!i)
     {
         return NULL;
     }
-#ifdef PY3K
     r = PyUnicode_FromFormat("%s(%R)", Py_TYPE(self)->tp_name, i);
     Py_DECREF(i);
     return r;
-#else
-    r = PyObject_Repr(i);
-    Py_DECREF(i);
-    if (!r)
-    {
-        return NULL;
-    }
-    rv = PyOS_snprintf(repr, sizeof(repr),
-                       "%s(%s)", Py_TYPE(self)->tp_name,
-                       PyBytes_AS_STRING(r));
-    if (rv > 0 && (size_t)rv < sizeof(repr))
-    {
-        Py_DECREF(r);
-        return PyBytes_FromStringAndSize(repr, strlen(repr));
-    }
-    else
-    {
-        /* The static buffer wasn't big enough */
-        int size;
-        PyObject *s;
-        /* 3 for the parens and the null byte */
-        size = strlen(Py_TYPE(self)->tp_name) + PyBytes_GET_SIZE(r) + 3;
-        s = PyBytes_FromStringAndSize(NULL, size);
-        if (!s) {
-            Py_DECREF(r);
-            return r;
-        }
-        PyOS_snprintf(PyBytes_AS_STRING(s), size,
-                    "%s(%s)", Py_TYPE(self)->tp_name, PyBytes_AS_STRING(r));
-        Py_DECREF(r);
-        return s;
-    }
-#endif
 }
 
 static PyTypeObject BucketType = {
     PyVarObject_HEAD_INIT(NULL, 0)
     MODULE_NAME MOD_NAME_PREFIX "Bucket",   /* tp_name */
     sizeof(Bucket),                         /* tp_basicsize */
     0,                                      /* tp_itemsize */
@@ -1998,17 +1951,14 @@
     &Bucket_as_mapping,                     /* tp_as_mapping */
     0,                                      /* tp_hash */
     0,                                      /* tp_call */
     0,                                      /* tp_str */
     0,                                      /* tp_getattro */
     0,                                      /* tp_setattro */
     0,                                      /* tp_as_buffer */
-#ifndef PY3K
-    Py_TPFLAGS_CHECKTYPES |
-#endif
     Py_TPFLAGS_DEFAULT |
     Py_TPFLAGS_HAVE_GC |
     Py_TPFLAGS_BASETYPE,                    /* tp_flags */
     0,                                      /* tp_doc */
     (traverseproc)bucket_traverse,          /* tp_traverse */
     (inquiry)bucket_tp_clear,               /* tp_clear */
     0,                                      /* tp_richcompare */
```

### Comparing `BTrees-4.9.2/src/BTrees/Interfaces.py` & `BTrees-5.0/src/BTrees/Interfaces.py`

 * *Files identical despite different names*

### Comparing `BTrees-4.9.2/src/BTrees/Length.py` & `BTrees-5.0/src/BTrees/Length.py`

 * *Files identical despite different names*

### Comparing `BTrees-4.9.2/src/BTrees/MergeTemplate.c` & `BTrees-5.0/src/BTrees/MergeTemplate.c`

 * *Files identical despite different names*

### Comparing `BTrees-4.9.2/src/BTrees/SetOpTemplate.c` & `BTrees-5.0/src/BTrees/SetOpTemplate.c`

 * *Files identical despite different names*

### Comparing `BTrees-4.9.2/src/BTrees/SetTemplate.c` & `BTrees-5.0/src/BTrees/SetTemplate.c`

 * *Files 2% similar despite different names*

```diff
@@ -666,48 +666,33 @@
     0,                                  /* sq_inplace_repeat */
 };
 
 static PyNumberMethods set_as_number = {
      (binaryfunc)0,                     /* nb_add */
      bucket_sub,                        /* nb_subtract */
      (binaryfunc)0,                     /* nb_multiply */
-#ifndef PY3K
-     0,                                 /* nb_divide */
-#endif
      (binaryfunc)0,                     /* nb_remainder */
      (binaryfunc)0,                     /* nb_divmod */
      (ternaryfunc)0,                    /* nb_power */
      (unaryfunc)0,                      /* nb_negative */
      (unaryfunc)0,                      /* nb_positive */
      (unaryfunc)0,                      /* nb_absolute */
      (inquiry)0,                        /* nb_bool */
      (unaryfunc)0,                      /* nb_invert */
      (binaryfunc)0,                     /* nb_lshift */
      (binaryfunc)0,                     /* nb_rshift */
      bucket_and,                        /* nb_and */
      (binaryfunc)Generic_set_xor,       /* nb_xor */
      bucket_or,                         /* nb_or */
-#ifdef PY3K
      0,                                 /*nb_int*/
      0,                                 /*nb_reserved*/
      0,                                 /*nb_float*/
-#else
-     0,                                 /*nb_coerce*/
-     0,                                 /*nb_int*/
-     0,                                 /*nb_long*/
-     0,                                 /*nb_float*/
-     0,                                 /*nb_oct*/
-     0,                                 /*nb_hex*/
-#endif
      0,                                 /*nb_inplace_add*/
      (binaryfunc)set_isub,              /*nb_inplace_subtract*/
      0,                                 /*nb_inplace_multiply*/
-#ifndef PY3K
-     0,                                 /*nb_inplace_divide*/
-#endif
      0,                                 /*nb_inplace_remainder*/
      0,                                 /*nb_inplace_power*/
      0,                                 /*nb_inplace_lshift*/
      0,                                 /*nb_inplace_rshift*/
      (binaryfunc)set_iand,              /*nb_inplace_and*/
      (binaryfunc)set_ixor,              /*nb_inplace_xor*/
      (binaryfunc)set_ior,               /*nb_inplace_or*/
@@ -729,17 +714,14 @@
     0,                                  /* tp_as_mapping */
     0,                                  /* tp_hash */
     0,                                  /* tp_call */
     0,                                  /* tp_str */
     0,                                  /* tp_getattro */
     0,                                  /* tp_setattro */
     0,                                  /* tp_as_buffer */
-#ifndef PY3K
-    Py_TPFLAGS_CHECKTYPES |
-#endif
     Py_TPFLAGS_DEFAULT |
     Py_TPFLAGS_HAVE_GC |
     Py_TPFLAGS_BASETYPE,                /* tp_flags */
     0,                                  /* tp_doc */
     (traverseproc)bucket_traverse,      /* tp_traverse */
     (inquiry)bucket_tp_clear,           /* tp_clear */
     0,                                  /* tp_richcompare */
```

### Comparing `BTrees-4.9.2/src/BTrees/TreeSetTemplate.c` & `BTrees-5.0/src/BTrees/TreeSetTemplate.c`

 * *Files 1% similar despite different names*

```diff
@@ -548,48 +548,33 @@
 }
 
 
 static PyNumberMethods TreeSet_as_number = {
     0,                                      /* nb_add */
     bucket_sub,                             /* nb_subtract */
     0,                                      /* nb_multiply */
-#ifndef PY3K
-    0,                                      /* nb_divide */
-#endif
     0,                                      /* nb_remainder */
     0,                                      /* nb_divmod */
     0,                                      /* nb_power */
     0,                                      /* nb_negative */
     0,                                      /* nb_positive */
     0,                                      /* nb_absolute */
     (inquiry)BTree_nonzero,                 /* nb_nonzero */
     (unaryfunc)0,                           /* nb_invert */
     (binaryfunc)0,                          /* nb_lshift */
     (binaryfunc)0,                          /* nb_rshift */
     bucket_and,                             /* nb_and */
     (binaryfunc)Generic_set_xor,            /* nb_xor */
     bucket_or,                              /* nb_or */
-#ifdef PY3K
      0,                                 /*nb_int*/
      0,                                 /*nb_reserved*/
      0,                                 /*nb_float*/
-#else
-     0,                                 /*nb_coerce*/
-     0,                                 /*nb_int*/
-     0,                                 /*nb_long*/
-     0,                                 /*nb_float*/
-     0,                                 /*nb_oct*/
-     0,                                 /*nb_hex*/
-#endif
      0,                                 /*nb_inplace_add*/
      (binaryfunc)TreeSet_isub,          /*nb_inplace_subtract*/
      0,                                 /*nb_inplace_multiply*/
-#ifndef PY3K
-     0,                                 /*nb_inplace_divide*/
-#endif
      0,                                 /*nb_inplace_remainder*/
      0,                                 /*nb_inplace_power*/
      0,                                 /*nb_inplace_lshift*/
      0,                                 /*nb_inplace_rshift*/
      (binaryfunc)TreeSet_iand,          /*nb_inplace_and*/
      (binaryfunc)TreeSet_ixor,          /*nb_inplace_xor*/
      (binaryfunc)TreeSet_ior,           /*nb_inplace_or*/
@@ -612,17 +597,14 @@
     &TreeSet_as_mapping,                        /* tp_as_mapping */
     0,                                          /* tp_hash */
     0,                                          /* tp_call */
     0,                                          /* tp_str */
     0,                                          /* tp_getattro */
     0,                                          /* tp_setattro */
     0,                                          /* tp_as_buffer */
-#ifndef PY3K
-    Py_TPFLAGS_CHECKTYPES |
-#endif
     Py_TPFLAGS_DEFAULT |
     Py_TPFLAGS_HAVE_GC |
     Py_TPFLAGS_BASETYPE,                        /* tp_flags */
     0,                                          /* tp_doc */
     (traverseproc)BTree_traverse,               /* tp_traverse */
     (inquiry)BTree_tp_clear,                    /* tp_clear */
     0,                                          /* tp_richcompare */
```

### Comparing `BTrees-4.9.2/src/BTrees/_IFBTree.c` & `BTrees-5.0/src/BTrees/_IUBTree.c`

 * *Files 8% similar despite different names*

```diff
@@ -10,32 +10,30 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ############################################################################*/
 
 #define MASTER_ID "$Id$\n"
 
-/* IFBTree - int key, float value BTree
+/* IIBTree - int32_t key, uint32_t value BTree
 
    Implements a collection using int type keys
-   and float type values
+   and int type values
 */
 
 /* Setup template macros */
 
 #define PERSISTENT
 
-#define MOD_NAME_PREFIX "IF"
+#define MOD_NAME_PREFIX "IU"
 
 
 
 
+#define ZODB_UNSIGNED_VALUE_INTS
+
 #include "_compat.h"
 #include "intkeymacros.h"
-#include "floatvaluemacros.h"
+#include "intvaluemacros.h"
 
-#ifdef PY3K
-#define INITMODULE PyInit__IFBTree
-#else
-#define INITMODULE init_IFBTree
-#endif
+#define INITMODULE PyInit__IUBTree
 #include "BTreeModuleTemplate.c"
```

### Comparing `BTrees-4.9.2/src/BTrees/_IIBTree.c` & `BTrees-5.0/src/BTrees/_UUBTree.c`

 * *Files 9% similar despite different names*

```diff
@@ -10,32 +10,30 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ############################################################################*/
 
 #define MASTER_ID "$Id$\n"
 
-/* IIBTree - int key, int value BTree
+/* IIBTree - unsigned int key, unsigned int value BTree
 
    Implements a collection using int type keys
    and int type values
 */
 
 /* Setup template macros */
 
 #define PERSISTENT
 
-#define MOD_NAME_PREFIX "II"
+#define MOD_NAME_PREFIX "UU"
 
 
 
+#define ZODB_UNSIGNED_KEY_INTS
+#define ZODB_UNSIGNED_VALUE_INTS
 
 #include "_compat.h"
 #include "intkeymacros.h"
 #include "intvaluemacros.h"
 
-#ifdef PY3K
-#define INITMODULE PyInit__IIBTree
-#else
-#define INITMODULE init_IIBTree
-#endif
+#define INITMODULE PyInit__UUBTree
 #include "BTreeModuleTemplate.c"
```

### Comparing `BTrees-4.9.2/src/BTrees/_IOBTree.c` & `BTrees-5.0/src/BTrees/_OUBTree.c`

 * *Files 12% similar despite different names*

```diff
@@ -10,30 +10,28 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ############################################################################*/
 
 #define MASTER_ID "$Id$\n"
 
-/* IOBTree - int key, object value BTree
+/* OUBTree - object key, uint32_t value BTree
 
-   Implements a collection using int type keys
-   and object type values
+   Implements a collection using object type keys
+   and int type values
 */
 
 #define PERSISTENT
 
-#define MOD_NAME_PREFIX "IO"
+#define MOD_NAME_PREFIX "OU"
 
 
 
-                                
+
+#define ZODB_UNSIGNED_VALUE_INTS
+
 #include "_compat.h"
-#include "intkeymacros.h"
-#include "objectvaluemacros.h"
+#include "objectkeymacros.h"
+#include "intvaluemacros.h"
 
-#ifdef PY3K
-#define INITMODULE PyInit__IOBTree
-#else
-#define INITMODULE init_IOBTree
-#endif
+#define INITMODULE PyInit__OUBTree
 #include "BTreeModuleTemplate.c"
```

### Comparing `BTrees-4.9.2/src/BTrees/_IUBTree.c` & `BTrees-5.0/src/BTrees/_OQBTree.c`

 * *Files 10% similar despite different names*

```diff
@@ -8,36 +8,31 @@
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ############################################################################*/
 
-#define MASTER_ID "$Id$\n"
+#define MASTER_ID "$Id: _OIBTree.c 25186 2004-06-02 15:07:33Z jim $\n"
 
-/* IIBTree - int32_t key, uint32_t value BTree
+/* OQBTree - object key, uint64_t value BTree
 
-   Implements a collection using int type keys
+   Implements a collection using object type keys
    and int type values
 */
 
-/* Setup template macros */
-
 #define PERSISTENT
 
-#define MOD_NAME_PREFIX "IU"
+#define MOD_NAME_PREFIX "OQ"
 
 
 
 
+#define ZODB_64BIT_INTS
 #define ZODB_UNSIGNED_VALUE_INTS
 
 #include "_compat.h"
-#include "intkeymacros.h"
+#include "objectkeymacros.h"
 #include "intvaluemacros.h"
 
-#ifdef PY3K
-#define INITMODULE PyInit__IUBTree
-#else
-#define INITMODULE init_IUBTree
-#endif
+#define INITMODULE PyInit__OQBTree
 #include "BTreeModuleTemplate.c"
```

### Comparing `BTrees-4.9.2/src/BTrees/_LFBTree.c` & `BTrees-5.0/src/BTrees/_QFBTree.c`

 * *Files 9% similar despite different names*

```diff
@@ -10,34 +10,31 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ############################################################################*/
 
 #define MASTER_ID "$Id: _IFBTree.c 67074 2006-04-17 19:13:39Z fdrake $\n"
 
-/* IFBTree - int key, float value BTree
+/* QFBTree - uint64_t key, float value BTree
 
    Implements a collection using int type keys
    and float type values
 */
 
 /* Setup template macros */
 
 #define PERSISTENT
 
-#define MOD_NAME_PREFIX "LF"
+#define MOD_NAME_PREFIX "QF"
 
 
 
 
 #define ZODB_64BIT_INTS
+#define ZODB_UNSIGNED_KEY_INTS
 
 #include "_compat.h"
 #include "intkeymacros.h"
 #include "floatvaluemacros.h"
 
-#ifdef PY3K
-#define INITMODULE PyInit__LFBTree
-#else
-#define INITMODULE init_LFBTree
-#endif
+#define INITMODULE PyInit__QFBTree
 #include "BTreeModuleTemplate.c"
```

### Comparing `BTrees-4.9.2/src/BTrees/_LLBTree.c` & `BTrees-5.0/src/BTrees/_LLBTree.c`

 * *Files 11% similar despite different names*

```diff
@@ -31,13 +31,9 @@
 
 #define ZODB_64BIT_INTS
 
 #include "_compat.h"
 #include "intkeymacros.h"
 #include "intvaluemacros.h"
 
-#ifdef PY3K
 #define INITMODULE PyInit__LLBTree
-#else
-#define INITMODULE init_LLBTree
-#endif
 #include "BTreeModuleTemplate.c"
```

### Comparing `BTrees-4.9.2/src/BTrees/_LOBTree.c` & `BTrees-5.0/src/BTrees/_LOBTree.c`

 * *Files 9% similar despite different names*

```diff
@@ -29,13 +29,9 @@
 
 #define ZODB_64BIT_INTS
 
 #include "_compat.h"
 #include "intkeymacros.h"
 #include "objectvaluemacros.h"
 
-#ifdef PY3K
 #define INITMODULE PyInit__LOBTree
-#else
-#define INITMODULE init_LOBTree
-#endif
 #include "BTreeModuleTemplate.c"
```

### Comparing `BTrees-4.9.2/src/BTrees/_LQBTree.c` & `BTrees-5.0/src/BTrees/_LQBTree.c`

 * *Files 6% similar despite different names*

```diff
@@ -32,13 +32,9 @@
 #define ZODB_64BIT_INTS
 #define ZODB_UNSIGNED_VALUE_INTS
 
 #include "_compat.h"
 #include "intkeymacros.h"
 #include "intvaluemacros.h"
 
-#ifdef PY3K
 #define INITMODULE PyInit__LQBTree
-#else
-#define INITMODULE init_LQBTree
-#endif
 #include "BTreeModuleTemplate.c"
```

### Comparing `BTrees-4.9.2/src/BTrees/_OIBTree.c` & `BTrees-5.0/src/BTrees/_OIBTree.c`

 * *Files 14% similar despite different names*

```diff
@@ -22,18 +22,14 @@
 
 #define PERSISTENT
 
 #define MOD_NAME_PREFIX "OI"
 
 
 
-                                
+
 #include "_compat.h"
 #include "objectkeymacros.h"
 #include "intvaluemacros.h"
 
-#ifdef PY3K
 #define INITMODULE PyInit__OIBTree
-#else
-#define INITMODULE init_OIBTree
-#endif
 #include "BTreeModuleTemplate.c"
```

### Comparing `BTrees-4.9.2/src/BTrees/_OLBTree.c` & `BTrees-5.0/src/BTrees/_QQBTree.c`

 * *Files 16% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ############################################################################*/
 
-#define MASTER_ID "$Id: _OIBTree.c 25186 2004-06-02 15:07:33Z jim $\n"
+#define MASTER_ID "$Id: _IIBTree.c 25186 2004-06-02 15:07:33Z jim $\n"
 
-/* OIBTree - object key, int value BTree
+/* QQBTree - uint64_t key, uint64_t value BTree
 
-   Implements a collection using object type keys
+   Implements a collection using int type keys
    and int type values
 */
 
+/* Setup template macros */
+
 #define PERSISTENT
 
-#define MOD_NAME_PREFIX "OL"
+#define MOD_NAME_PREFIX "QQ"
 
 
 
 
 #define ZODB_64BIT_INTS
+#define ZODB_UNSIGNED_KEY_INTS
+#define ZODB_UNSIGNED_VALUE_INTS
 
 #include "_compat.h"
-#include "objectkeymacros.h"
+#include "intkeymacros.h"
 #include "intvaluemacros.h"
 
-#ifdef PY3K
-#define INITMODULE PyInit__OLBTree
-#else
-#define INITMODULE init_OLBTree
-#endif
+#define INITMODULE PyInit__QQBTree
 #include "BTreeModuleTemplate.c"
```

### Comparing `BTrees-4.9.2/src/BTrees/_OOBTree.c` & `BTrees-5.0/src/BTrees/_IOBTree.c`

 * *Files 15% similar despite different names*

```diff
@@ -10,30 +10,26 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ############################################################################*/
 
 #define MASTER_ID "$Id$\n"
 
-/* OOBTree - object key, object value BTree
+/* IOBTree - int key, object value BTree
 
-   Implements a collection using object type keys
+   Implements a collection using int type keys
    and object type values
 */
 
 #define PERSISTENT
 
-#define MOD_NAME_PREFIX "OO"
+#define MOD_NAME_PREFIX "IO"
+
 
 
 
-                                
 #include "_compat.h"
-#include "objectkeymacros.h"
+#include "intkeymacros.h"
 #include "objectvaluemacros.h"
 
-#ifdef PY3K
-#define INITMODULE PyInit__OOBTree
-#else
-#define INITMODULE init_OOBTree
-#endif
+#define INITMODULE PyInit__IOBTree
 #include "BTreeModuleTemplate.c"
```

### Comparing `BTrees-4.9.2/src/BTrees/_OQBTree.c` & `BTrees-5.0/src/BTrees/_OLBTree.c`

 * *Files 13% similar despite different names*

```diff
@@ -10,33 +10,28 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ############################################################################*/
 
 #define MASTER_ID "$Id: _OIBTree.c 25186 2004-06-02 15:07:33Z jim $\n"
 
-/* OQBTree - object key, uint64_t value BTree
+/* OIBTree - object key, int value BTree
 
    Implements a collection using object type keys
    and int type values
 */
 
 #define PERSISTENT
 
-#define MOD_NAME_PREFIX "OQ"
+#define MOD_NAME_PREFIX "OL"
 
 
 
 
 #define ZODB_64BIT_INTS
-#define ZODB_UNSIGNED_VALUE_INTS
 
 #include "_compat.h"
 #include "objectkeymacros.h"
 #include "intvaluemacros.h"
 
-#ifdef PY3K
-#define INITMODULE PyInit__OQBTree
-#else
-#define INITMODULE init_OQBTree
-#endif
+#define INITMODULE PyInit__OLBTree
 #include "BTreeModuleTemplate.c"
```

### Comparing `BTrees-4.9.2/src/BTrees/_OUBTree.c` & `BTrees-5.0/src/BTrees/_QOBTree.c`

 * *Files 11% similar despite different names*

```diff
@@ -8,34 +8,31 @@
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ############################################################################*/
 
-#define MASTER_ID "$Id$\n"
+#define MASTER_ID "$Id: _IOBTree.c 25186 2004-06-02 15:07:33Z jim $\n"
 
-/* OUBTree - object key, uint32_t value BTree
+/* QOBTree - uint64_t key, object value BTree
 
-   Implements a collection using object type keys
-   and int type values
+   Implements a collection using int type keys
+   and object type values
 */
 
 #define PERSISTENT
 
-#define MOD_NAME_PREFIX "OU"
+#define MOD_NAME_PREFIX "QO"
 
 
 
 
-#define ZODB_UNSIGNED_VALUE_INTS
+#define ZODB_64BIT_INTS
+#define ZODB_UNSIGNED_KEY_INTS
 
 #include "_compat.h"
-#include "objectkeymacros.h"
-#include "intvaluemacros.h"
+#include "intkeymacros.h"
+#include "objectvaluemacros.h"
 
-#ifdef PY3K
-#define INITMODULE PyInit__OUBTree
-#else
-#define INITMODULE init_OUBTree
-#endif
+#define INITMODULE PyInit__QOBTree
 #include "BTreeModuleTemplate.c"
```

### Comparing `BTrees-4.9.2/src/BTrees/_QFBTree.c` & `BTrees-5.0/src/BTrees/_LFBTree.c`

 * *Files 12% similar despite different names*

```diff
@@ -10,35 +10,30 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ############################################################################*/
 
 #define MASTER_ID "$Id: _IFBTree.c 67074 2006-04-17 19:13:39Z fdrake $\n"
 
-/* QFBTree - uint64_t key, float value BTree
+/* IFBTree - int key, float value BTree
 
    Implements a collection using int type keys
    and float type values
 */
 
 /* Setup template macros */
 
 #define PERSISTENT
 
-#define MOD_NAME_PREFIX "QF"
+#define MOD_NAME_PREFIX "LF"
 
 
 
 
 #define ZODB_64BIT_INTS
-#define ZODB_UNSIGNED_KEY_INTS
 
 #include "_compat.h"
 #include "intkeymacros.h"
 #include "floatvaluemacros.h"
 
-#ifdef PY3K
-#define INITMODULE PyInit__QFBTree
-#else
-#define INITMODULE init_QFBTree
-#endif
+#define INITMODULE PyInit__LFBTree
 #include "BTreeModuleTemplate.c"
```

### Comparing `BTrees-4.9.2/src/BTrees/_QLBTree.c` & `BTrees-5.0/src/BTrees/_UFBTree.c`

 * *Files 12% similar despite different names*

```diff
@@ -8,37 +8,31 @@
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ############################################################################*/
 
-#define MASTER_ID "$Id: _IIBTree.c 25186 2004-06-02 15:07:33Z jim $\n"
+#define MASTER_ID "$Id$\n"
 
-/* QLBTree - uint64_t key, int64_t value BTree
+/* IFBTree - unsigned int key, float value BTree
 
    Implements a collection using int type keys
-   and int type values
+   and float type values
 */
 
 /* Setup template macros */
 
 #define PERSISTENT
 
-#define MOD_NAME_PREFIX "QL"
+#define MOD_NAME_PREFIX "UF"
 
 
 
-
-#define ZODB_64BIT_INTS
 #define ZODB_UNSIGNED_KEY_INTS
 
 #include "_compat.h"
 #include "intkeymacros.h"
-#include "intvaluemacros.h"
+#include "floatvaluemacros.h"
 
-#ifdef PY3K
-#define INITMODULE PyInit__QLBTree
-#else
-#define INITMODULE init_QLBTree
-#endif
+#define INITMODULE PyInit__UFBTree
 #include "BTreeModuleTemplate.c"
```

### Comparing `BTrees-4.9.2/src/BTrees/_QOBTree.c` & `BTrees-5.0/src/BTrees/_IIBTree.c`

 * *Files 19% similar despite different names*

```diff
@@ -8,35 +8,30 @@
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ############################################################################*/
 
-#define MASTER_ID "$Id: _IOBTree.c 25186 2004-06-02 15:07:33Z jim $\n"
+#define MASTER_ID "$Id$\n"
 
-/* QOBTree - uint64_t key, object value BTree
+/* IIBTree - int key, int value BTree
 
    Implements a collection using int type keys
-   and object type values
+   and int type values
 */
 
-#define PERSISTENT
+/* Setup template macros */
 
-#define MOD_NAME_PREFIX "QO"
+#define PERSISTENT
 
+#define MOD_NAME_PREFIX "II"
 
 
 
-#define ZODB_64BIT_INTS
-#define ZODB_UNSIGNED_KEY_INTS
 
 #include "_compat.h"
 #include "intkeymacros.h"
-#include "objectvaluemacros.h"
+#include "intvaluemacros.h"
 
-#ifdef PY3K
-#define INITMODULE PyInit__QOBTree
-#else
-#define INITMODULE init_QOBTree
-#endif
+#define INITMODULE PyInit__IIBTree
 #include "BTreeModuleTemplate.c"
```

### Comparing `BTrees-4.9.2/src/BTrees/_QQBTree.c` & `BTrees-5.0/src/BTrees/_QLBTree.c`

 * *Files 10% similar despite different names*

```diff
@@ -10,36 +10,31 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ############################################################################*/
 
 #define MASTER_ID "$Id: _IIBTree.c 25186 2004-06-02 15:07:33Z jim $\n"
 
-/* QQBTree - uint64_t key, uint64_t value BTree
+/* QLBTree - uint64_t key, int64_t value BTree
 
    Implements a collection using int type keys
    and int type values
 */
 
 /* Setup template macros */
 
 #define PERSISTENT
 
-#define MOD_NAME_PREFIX "QQ"
+#define MOD_NAME_PREFIX "QL"
 
 
 
 
 #define ZODB_64BIT_INTS
 #define ZODB_UNSIGNED_KEY_INTS
-#define ZODB_UNSIGNED_VALUE_INTS
 
 #include "_compat.h"
 #include "intkeymacros.h"
 #include "intvaluemacros.h"
 
-#ifdef PY3K
-#define INITMODULE PyInit__QQBTree
-#else
-#define INITMODULE init_QQBTree
-#endif
+#define INITMODULE PyInit__QLBTree
 #include "BTreeModuleTemplate.c"
```

### Comparing `BTrees-4.9.2/src/BTrees/_UFBTree.c` & `BTrees-5.0/src/BTrees/_IFBTree.c`

 * *Files 12% similar despite different names*

```diff
@@ -10,33 +10,28 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ############################################################################*/
 
 #define MASTER_ID "$Id$\n"
 
-/* IFBTree - unsigned int key, float value BTree
+/* IFBTree - int key, float value BTree
 
    Implements a collection using int type keys
    and float type values
 */
 
 /* Setup template macros */
 
 #define PERSISTENT
 
-#define MOD_NAME_PREFIX "UF"
+#define MOD_NAME_PREFIX "IF"
 
 
 
-#define ZODB_UNSIGNED_KEY_INTS
 
 #include "_compat.h"
 #include "intkeymacros.h"
 #include "floatvaluemacros.h"
 
-#ifdef PY3K
-#define INITMODULE PyInit__UFBTree
-#else
-#define INITMODULE init_UFBTree
-#endif
+#define INITMODULE PyInit__IFBTree
 #include "BTreeModuleTemplate.c"
```

### Comparing `BTrees-4.9.2/src/BTrees/_UIBTree.c` & `BTrees-5.0/src/BTrees/_UIBTree.c`

 * *Files 16% similar despite different names*

```diff
@@ -30,13 +30,9 @@
 
 #define ZODB_UNSIGNED_KEY_INTS
 
 #include "_compat.h"
 #include "intkeymacros.h"
 #include "intvaluemacros.h"
 
-#ifdef PY3K
 #define INITMODULE PyInit__UIBTree
-#else
-#define INITMODULE init_UIBTree
-#endif
 #include "BTreeModuleTemplate.c"
```

### Comparing `BTrees-4.9.2/src/BTrees/_UOBTree.c` & `BTrees-5.0/src/BTrees/_UOBTree.c`

 * *Files 18% similar despite different names*

```diff
@@ -27,13 +27,9 @@
 
 
 #define ZODB_UNSIGNED_KEY_INTS
 #include "_compat.h"
 #include "intkeymacros.h"
 #include "objectvaluemacros.h"
 
-#ifdef PY3K
 #define INITMODULE PyInit__UOBTree
-#else
-#define INITMODULE init_UOBTree
-#endif
 #include "BTreeModuleTemplate.c"
```

### Comparing `BTrees-4.9.2/src/BTrees/__init__.py` & `BTrees-5.0/src/BTrees/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     name = vars(mod)['__name__']
     sys.modules[name] = mod
     globals()[name.split('.', 1)[1]] = mod
     __all__.append(name)
 
 
 @zope.interface.implementer(BTrees.Interfaces.IBTreeFamily)
-class _Family(object):
+class _Family:
     from BTrees import OOBTree as OO
     _BITSIZE = 0
     minint = maxint = maxuint = None
 
     def __init__(self):
         self.maxint = int(2 ** (self._BITSIZE - 1) - 1)
         self.minint = int(-self.maxint - 1)
```

### Comparing `BTrees-4.9.2/src/BTrees/_base.py` & `BTrees-5.0/src/BTrees/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,22 +10,18 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Python BTree implementation
 """
 
-
-
 from persistent import Persistent
 
 from .Interfaces import BTreesConflictError
-from ._compat import PY3
 from ._compat import compare
-from ._compat import xrange
 
 # XXX: Fix these. These ignores are temporary to
 # reduce the noise and help find specific issues during
 # refactoring
 # pylint:disable=too-many-lines,fixme,protected-access
 # pylint:disable=attribute-defined-outside-init,redefined-builtin,no-else-return
 # pylint:disable=redefined-outer-name,bad-continuation,unused-variable
@@ -86,15 +82,15 @@
             # type of this object.
             # This implementation is replaced by _fix_pickle and exists for
             # testing purposes.
             return type(self)  # pragma: no cover
 
         _BTree_reduce_up_bound = _BTree_reduce_as
 
-class _ArithmeticMixin(object):
+class _ArithmeticMixin:
     def __sub__(self, other):
         return difference(self.__class__, self, other)
 
     def __rsub__(self, other):
         return difference(self._set_type, type(self)(other), self)
 
     def __or__(self, other):
@@ -214,15 +210,15 @@
         start, end = self._range(*args, **kw)
         return self._keys[start:end]
 
     def iterkeys(self, *args, **kw):
         if not (args or kw):
             return iter(self._keys)
         keys = self._keys
-        return (keys[i] for i in xrange(*self._range(*args, **kw)))
+        return (keys[i] for i in range(*self._range(*args, **kw)))
 
     def __iter__(self):
         return iter(self._keys)
 
     def __contains__(self, key):
         try:
             tree_key = self._to_key(key)
@@ -235,18 +231,18 @@
     has_key = __contains__
 
     def _repr_helper(self, items):
         type_self = type(self)
         mod = type_self.__module__
         name = type_self.__name__
         name = name[:-2] if name.endswith("Py") else name
-        return "%s.%s(%r)" % (mod, name, items)
+        return "{}.{}({!r})".format(mod, name, items)
 
 
-class _SetIteration(object):
+class _SetIteration:
 
     __slots__ = ('to_iterate',
                  'useValues',
                  '_iter',
                  'active',
                  'position',
                  'key',
@@ -267,15 +263,15 @@
                 # iterate in sorted order. Other than that, we have no guarantee.
                 self.to_iterate = to_iterate = sorted(self.to_iterate)
 
         if useValues:
             try:
                 itmeth = to_iterate.iteritems
             except AttributeError:
-                if PY3 and isinstance(to_iterate, dict): #pragma no cover Py3k
+                if isinstance(to_iterate, dict):
                     itmeth = to_iterate.items().__iter__
                 else:
                     itmeth = to_iterate.__iter__
                     useValues = False
             else:
                 self.value = None
         else:
@@ -298,15 +294,15 @@
             self.position += 1
         except StopIteration:
             self.active = False
             self.position = -1
 
         return self
 
-class _MutableMappingMixin(object):
+class _MutableMappingMixin:
     # Methods defined in collections.abc.MutableMapping that
     # Bucket and Tree should both implement and can implement
     # the same. We don't want to extend that class though,
     # as the C version cannot.
     def popitem(self):
         """
         D.popitem() -> (k, v), remove and return some (key, value) pair
@@ -436,27 +432,27 @@
 
     def values(self, *args, **kw):
         start, end = self._range(*args, **kw)
         return self._values[start:end]
 
     def itervalues(self, *args, **kw):
         values = self._values
-        return (values[i] for i in xrange(*self._range(*args, **kw)))
+        return (values[i] for i in range(*self._range(*args, **kw)))
 
     def items(self, *args, **kw):
         keys = self._keys
         values = self._values
         return [(keys[i], values[i])
-                    for i in xrange(*self._range(*args, **kw))]
+                    for i in range(*self._range(*args, **kw))]
 
     def iteritems(self, *args, **kw):
         keys = self._keys
         values = self._values
         return ((keys[i], values[i])
-                    for i in xrange(*self._range(*args, **kw)))
+                    for i in range(*self._range(*args, **kw)))
 
     def __getstate__(self):
         keys = self._keys
         values = self._values
         data = []
         for i in range(len(keys)):
             data.append(keys[i])
@@ -619,15 +615,15 @@
 
         result._next = b_old._next
         return result.__getstate__()
 
     def __repr__(self):
         return self._repr_helper(self.items())
 
-class _MutableSetMixin(object):
+class _MutableSetMixin:
     # Like _MutableMappingMixin, but for sets.
     def isdisjoint(self, other):
         """
         Return True if two sets have a null intersection.
         """
         for value in other:
             if value in self:
@@ -878,15 +874,15 @@
 
         result._next = b_old._next
         return result.__getstate__()
 
     def __repr__(self):
         return self._repr_helper(self._keys)
 
-class _TreeItem(object):
+class _TreeItem:
 
     __slots__ = ('key',
                  'child',
                 )
 
     def __init__(self, key, child):
         self.key = key
@@ -937,17 +933,16 @@
 
     def clear(self):
         if self._data:
             # In the case of __init__, this was already set by __new__
             self._data = []
         self._firstbucket = None
 
-    def __nonzero__(self):
+    def __bool__(self):
         return bool(self._data)
-    __bool__ = __nonzero__ #Py3k rename
 
     def __len__(self):
         l = 0
         bucket = self._firstbucket
         while bucket is not None:
             l += len(bucket._keys)
             bucket = bucket._next
@@ -991,16 +986,15 @@
             return False
         return key in (self._findbucket(tree_key) or ())
 
     def has_key(self, key):
         index = self._search(key)
         if index < 0:
             return False
-        r = self._data[index].child.has_key(key)
-        return r and r + 1
+        return self._data[index].child.has_key(key)
 
     def keys(self, min=_marker, max=_marker,
              excludemin=False, excludemax=False,
              itertype='iterkeys'):
         if not self._data:
             return ()
 
@@ -1260,15 +1254,15 @@
         s_old = _get_simple_btree_bucket_state(old)
         s_com = _get_simple_btree_bucket_state(com)
         s_new = _get_simple_btree_bucket_state(new)
         return ((
             self._bucket_type()._p_resolveConflict(s_old, s_com, s_new), ), )
 
     def __repr__(self):
-        r = super(_Tree, self).__repr__()
+        r = super().__repr__()
         r = r.replace('Py', '')
         return r
 
 
 def _get_simple_btree_bucket_state(state):
     if state is None:
         return state
@@ -1285,15 +1279,15 @@
                         "bucket state")
     state = state[0]
     if not isinstance(state, tuple):
         raise TypeError("_p_resolveConflict: expected tuple for bucket state")
     return state
 
 
-class _TreeItems(object):
+class _TreeItems:
 
     __slots__ = ('firstbucket',
                  'itertype',
                  'iterargs',
                  'index',
                  'it',
                  'v',
@@ -1351,15 +1345,15 @@
                 done = 0
             if done:
                 return
             bucket = bucket._next
             done = 1
 
 
-class _TreeIterator(object):
+class _TreeIterator:
     """ Faux implementation for BBB only.
     """
     def __init__(self, items): #pragma: no cover
         raise TypeError(
             "TreeIterators are private implementation details "
             "of the C-based BTrees.\n\n"
             "Please use 'iter(tree)', rather than instantiating "
@@ -1423,15 +1417,15 @@
         add = self.add
         for i in items:
             add(i)
 
     _p_resolveConflict = _Tree._p_resolveConflict
 
 
-class set_operation(object):
+class set_operation:
 
     __slots__ = (
         'func',
         'set_type',
         '__name__',
         '_module',
     )
```

### Comparing `BTrees-4.9.2/src/BTrees/_compat.h` & `BTrees-5.0/src/BTrees/_compat.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-/* Straddle Python 2 / 3 */
 #ifndef BTREES__COMPAT_H
 #define BTREES__COMPAT_H
 
 #include "Python.h"
 
 #ifdef INTERN
 #undef INTERN
@@ -17,18 +16,14 @@
 #endif
 
 #ifndef Py_RETURN_NOTIMPLEMENTED
 #define Py_RETURN_NOTIMPLEMENTED \
     return Py_INCREF(Py_NotImplemented), Py_NotImplemented
 #endif
 
-#if PY_MAJOR_VERSION >= 3
-
-#define PY3K
-
 #define INTERN PyUnicode_InternFromString
 #define INT_FROM_LONG(x) PyLong_FromLong(x)
 #define INT_CHECK(x) PyLong_Check(x)
 #define INT_AS_LONG(x) PyLong_AsLong(x)
 #define UINT_FROM_LONG(x) PyLong_FromUnsignedLong(x)
 #define UINT_AS_LONG(x) PyLong_AsUnsignedLong(x)
 #define TEXT_FROM_STRING PyUnicode_FromString
@@ -40,25 +35,8 @@
   -1 -> There was an error, which the caller will detect with PyError_Occurred.
  */
 #define COMPARE(lhs, rhs) \
   (lhs == Py_None ? (rhs == Py_None ? 0 : -1) : (rhs == Py_None ? 1 : \
      (PyObject_RichCompareBool((lhs), (rhs), Py_LT) != 0 ? -1 : \
       (PyObject_RichCompareBool((lhs), (rhs), Py_EQ) > 0 ? 0 : 1))))
 
-#else
-
-#define INTERN PyString_InternFromString
-#define INT_FROM_LONG(x) PyInt_FromLong(x)
-#define INT_CHECK(x) PyInt_Check(x)
-#define INT_AS_LONG(x) PyInt_AS_LONG(x)
-#define UINT_FROM_LONG(x) PyInt_FromSize_t(x)
-#define UINT_AS_LONG(x) PyInt_AsUnsignedLongMask(x)
-#define TEXT_FROM_STRING PyString_FromString
-#define TEXT_FORMAT PyString_Format
-
-#define COMPARE(lhs, rhs) \
-  (lhs == Py_None ? (rhs == Py_None ? 0 : -1) : (rhs == Py_None ? 1 : \
-     PyObject_Compare((lhs), (rhs))))
-
-#endif
-
 #endif /* BTREES__COMPAT_H */
```

### Comparing `BTrees-4.9.2/src/BTrees/_compat.py` & `BTrees-5.0/src/BTrees/_compat.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,67 +12,27 @@
 #
 ##############################################################################
 import os
 import sys
 
 PYPY = hasattr(sys, 'pypy_version_info')
 
-
-if sys.version_info[0] < 3: # pragma: no cover Python2
-
-    PY2 = True
-    PY3 = False
-
-    int_types = int, long
-    xrange = xrange
-    def compare(x, y):
-        if x is None:
-            if y is None:
-                return 0
-            else:
-                return -1
-        elif y is None:
-            return 1
+def compare(x, y):
+    if x is None:
+        if y is None:
+            return 0
         else:
-            return cmp(x, y)
-
-    _bytes = str
-    def _ascii(x):
-        return bytes(x)
-
-else: # pragma: no cover Python3
-
-    PY2 = False
-    PY3 = True
-
-    int_types = int,
-    xrange = range
-
-    def compare(x, y):
-        if x is None:
-            if y is None:
-                return 0
-            else:
-                return -1
-        elif y is None:
-            return 1
-        else:
-            return (x > y) - (y > x)
-
-    _bytes = bytes
-    def _ascii(x):
-        return bytes(x, 'ascii')
-
-try:
-    from collections import abc
-except ImportError:
-    import collections as abc
+            return -1
+    elif y is None:
+        return 1
+    else:
+        return (x > y) - (y > x)
 
-collections_abc = abc
-del abc
+def _ascii(x):
+    return bytes(x, 'ascii')
 
 def _c_optimizations_required():
     """
     Return a true value if the C optimizations are required.
 
     This uses the ``PURE_PYTHON`` variable as documented in `import_c_extension`.
     """
```

### Comparing `BTrees-4.9.2/src/BTrees/_datatypes.py` & `BTrees-5.0/src/BTrees/_datatypes.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,33 +10,26 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """
 Descriptions of the datatypes supported by this package.
 """
-from __future__ import absolute_import
 
 from operator import index as operator__index__
 from struct import Struct
 from struct import error as struct_error
 
-try:
-    from abc import ABC
-except ImportError:
-    # Python < 3.4 (specifically, Python 2)
-    from abc import ABCMeta
-    ABC = ABCMeta('ABC', (object,), {})
+from abc import ABC
 
-from ._compat import int_types
 from .utils import Lazy
 
 # pylint:disable=raise-missing-from
 
-class DataType(object):
+class DataType:
     """
     Describes a data type used as a value.
 
     Subclasses will be defined for each particular
     supported type.
     """
 
@@ -198,75 +191,40 @@
     getting the type from ``thing`` (including mostly dealing with
     old-style) classes on Python 2.
     """
 
     # Comparisons only use special methods defined on the
     # type, not instance variables.
 
-    # On CPython 2, every subclass of object inherits __lt__
-    # (unless it overrides), and it has ``__objclass__`` of ``type``
-    # (of course it is also the same object as ``_object_lt`` at
-    # that point). Also, interestingly, CPython 2 classes inherit
-    # ``__lt__`` from ``type``, but *instances* do not.
-    #
     # On CPython 3, classes inherit __lt__ with ``__objclass__`` of ``object``.
-    # On PyPy2, classes don't inherit any __lt__.
     # On PyPy3, they do.
     #
     # Test these conditions at runtime and define the method variant
     # appropriately.
     #
     # Remember the method is checking if the object has default comparison
     assert '__lt__' not in DataType.__dict__
-    if hasattr(DataType, '__lt__'):
-        # CPython 2 or CPython 3 or PyPy3
-        if getattr(DataType.__lt__, '__objclass__', None) is object:
-            # CPython 3
-            @classmethod
-            def __subclasshook__(cls, C, _NoneType=type(None)):
-                if C is _NoneType:
-                    return False
-                defining_class = getattr(C.__lt__, '__objclass__', None)
-                if defining_class is None:
-                    # Implemented in Python
-                    return False
-                return C.__lt__.__objclass__ is object
-        elif getattr(DataType.__lt__, '__objclass__', None) is type:
-            # CPython 2
-            @classmethod
-            def __subclasshook__(cls, C, _NoneType=type(None)):
-                if C is _NoneType:
-                    return False
-                # If C is an old-style class, it may not even have __lt__
-                if isinstance(C, type):
-                    lt = C.__lt__
-                else:
-                    lt = getattr(C, '__lt__', None)
-                if lt is not None:
-                    defining_class = getattr(lt, '__objclass__', None)
-                    if defining_class is None:
-                        # Implemented in Python
-                        return False
-                    if defining_class is not type:
-                        return False
-                return not hasattr(C, '__cmp__')
-        else:
-            # PyPy3
-            @classmethod
-            def __subclasshook__(cls, C, _object_lt=object.__lt__, _NoneType=type(None)):
-                if C is _NoneType:
-                    return False
-                return C.__lt__ is _object_lt
-    else:
-        # PyPy2
+    if getattr(DataType.__lt__, '__objclass__', None) is object:
+        # CPython 3
         @classmethod
         def __subclasshook__(cls, C, _NoneType=type(None)):
             if C is _NoneType:
                 return False
-            return not hasattr(C, '__lt__') and not hasattr(C, '__cmp__')
+            defining_class = getattr(C.__lt__, '__objclass__', None)
+            if defining_class is None:
+                # Implemented in Python
+                return False
+            return C.__lt__.__objclass__ is object
+    else:
+        # PyPy3
+        @classmethod
+        def __subclasshook__(cls, C, _object_lt=object.__lt__, _NoneType=type(None)):
+            if C is _NoneType:
+                return False
+            return C.__lt__ is _object_lt
 
 
 class O(KeyDataType):
     """
     Arbitrary (sortable) Python objects.
     """
     long_name = 'Object'
@@ -277,15 +235,15 @@
         return Any()
 
     def supports_value_union(self):
         return False
 
     def __call__(self, item):
         if isinstance(item, _HasDefaultComparison):
-            raise TypeError("Object of class %s has default comparison" % (type(item).__name__,))
+            raise TypeError("Object of class {} has default comparison".format(type(item).__name__))
         return item
 
 
 class _AbstractNativeDataType(KeyDataType):
     """
     Uses `struct.Struct` to verify that the data can fit into a native
     type.
@@ -303,40 +261,35 @@
 
     def __call__(self, item):
         try:
             self._check_native(self._as_packable(item)) # pylint:disable=too-many-function-args
         except (struct_error, TypeError, ValueError):
             # PyPy can raise ValueError converting a negative number to a
             # unsigned value.
-            if isinstance(item, int_types):
+            if isinstance(item, int):
                 raise TypeError("Value out of range", item)
             raise TypeError(self._error_description)
 
         return self._as_python_type(item)
 
     def apply_weight(self, item, weight):
         return item * weight
 
     def supports_value_union(self):
         return True
 
 class _AbstractIntDataType(_AbstractNativeDataType):
     _as_python_type = int
-    _required_python_type = int_types
+    _required_python_type = int
     multiplication_identity = 1
     long_name = "Integer"
 
     def getTwoExamples(self):
         return 1, 2
 
-    # On Python 2, it's important for these values to be actual `int`
-    # values, not `long` when they fit; passing a value that's too big
-    # to `int` will still result in it being a `long`. For some reason
-    # on Windows, even the 32-bit values somehow wind up as longs
-    # unless we do the conversion.
     def get_lower_bound(self):
         exp = 64 if self.using64bits else 32
         exp -= 1
         return int(-(2 ** exp))
 
     def get_upper_bound(self):
         exp = 64 if self.using64bits else 32
@@ -396,15 +349,15 @@
     """
     tree_size = 500
     default_bucket_size = 500
     _length = None
 
     def __call__(self, item):
         if not isinstance(item, bytes) or len(item) != self._length:
-            raise TypeError("%s-byte array expected, not %r" % (self._length, item))
+            raise TypeError("{}-byte array expected, not {!r}".format(self._length, item))
         return item
 
     def supports_value_union(self):
         # We don't implement 'multiunion' for fsBTree.
         return False
 
 
@@ -495,9 +448,9 @@
         except TypeError:
             try:
                 as_bytes = self._as_8_bytes(operator__index__(item))
             except struct_error as e:
                 raise TypeError(e)
 
             if as_bytes[:2] != b'\x00\x00':
-                raise TypeError("Cannot convert %r to 6 bytes (%r)" % (item, as_bytes))
+                raise TypeError("Cannot convert {!r} to 6 bytes ({!r})".format(item, as_bytes))
             return as_bytes[2:]
```

### Comparing `BTrees-4.9.2/src/BTrees/_fsBTree.c` & `BTrees-5.0/src/BTrees/_fsBTree.c`

 * *Files 5% similar despite different names*

```diff
@@ -81,19 +81,15 @@
     {"fromBytes", (PyCFunction) bucket_fromBytes,	METH_O, \
      "fromSBytes(s) -- Set the state of the object from a bytes array"}, \
     {"toString", (PyCFunction) bucket_toBytes,	METH_NOARGS, \
      "toString() -- Deprecated alias for 'toBytes'"}, \
     {"fromString", (PyCFunction) bucket_fromBytes,	METH_O, \
      "fromString(s) -- Deprecated alias for 'fromBytes'"}, \
 
-#ifdef PY3K
 #define INITMODULE PyInit__fsBTree
-#else
-#define INITMODULE init_fsBTree
-#endif
 #include "BTreeModuleTemplate.c"
 
 static PyObject *
 bucket_toBytes(PyObject *oself)
 {
   Bucket *self = (Bucket *)oself;
   PyObject *items = NULL;
@@ -104,18 +100,18 @@
   len = self->len;
 
   items = PyBytes_FromStringAndSize(NULL, len*8);
   if (items == NULL)
     goto err;
   memcpy(PyBytes_AS_STRING(items),       self->keys,   len*2);
   memcpy(PyBytes_AS_STRING(items)+len*2, self->values, len*6);
-  
+
   PER_UNUSE(self);
   return items;
-  
+
  err:
   PER_UNUSE(self);
   Py_XDECREF(items);
   return NULL;
 }
 
 static PyObject *
@@ -125,15 +121,15 @@
   int len;
   KEY_TYPE *keys;
   VALUE_TYPE *values;
 
   len = PyBytes_Size(state);
   if (len < 0)
     return NULL;
-  
+
   if (len%8)
     {
       PyErr_SetString(PyExc_ValueError, "state string of wrong size");
       return NULL;
     }
   len /= 8;
```

### Comparing `BTrees-4.9.2/src/BTrees/_module_builder.py` & `BTrees-5.0/src/BTrees/_module_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 
 
 def populate_module(mod_globals,
                     key_datatype, value_datatype,
                     interface, module=None):
     from . import Interfaces as interfaces
     from ._compat import import_c_extension
-    from ._compat import collections_abc
+    import collections.abc
     from ._base import _fix_pickle
 
     module_name = mod_globals['__name__']
     # Define the Python implementations
     mod_globals.update(_create_globals(module_name, key_datatype, value_datatype))
     # Import the C versions, if possible. Whether or not this is possible,
     # this currently makes the non-`Py' suffixed names available. This should change
@@ -171,18 +171,18 @@
             'TreeSet': interfaces.ITreeSet,
             'TreeItems': interfaces.IMinimalSequence,
     }.items():
         classImplements(mod_globals[cls_name], iface)
         classImplements(mod_globals[cls_name + 'Py'], iface)
 
     for cls_name, abc in {
-            'BTree': collections_abc.MutableMapping,
-            'Bucket': collections_abc.MutableMapping,
-            'Set': collections_abc.MutableSet,
-            'TreeSet': collections_abc.MutableSet,
+            'BTree': collections.abc.MutableMapping,
+            'Bucket': collections.abc.MutableMapping,
+            'Set': collections.abc.MutableSet,
+            'TreeSet': collections.abc.MutableSet,
     }.items():
         abc.register(mod_globals[cls_name])
         # Because of some quirks in the implementation of ABCMeta.__instancecheck__,
         # and the shenanigans we currently do to make Python classes pickle without the
         # 'Py' suffix, it's not actually necessary to register the Python version of the
         # class. Specifically, ABCMeta asks for the object's ``__class__`` instead of
         # using ``type()``, and our objects have a ``@property`` for ``__class__`` that returns
```

### Comparing `BTrees-4.9.2/src/BTrees/check.py` & `BTrees-5.0/src/BTrees/check.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,15 +248,15 @@
     return keys, values
 
 def type_and_adr(obj):
     if hasattr(obj, '_p_oid'):
         oid = oid_repr(obj._p_oid)
     else:
         oid = 'None'
-    return "%s (0x%x oid=%s)" % (type(obj).__name__, positive_id(obj), oid)
+    return "{} (0x{:x} oid={})".format(type(obj).__name__, positive_id(obj), oid)
 
 # Walker implements a depth-first search of a BTree (or TreeSet or Set or
 # Bucket).  Subclasses must implement the visit_btree() and visit_bucket()
 # methods, and arrange to call the walk() method.  walk() calls the
 # visit_XYZ() methods once for each node in the tree, in depth-first
 # left-to-right order.
 
@@ -397,15 +397,15 @@
             if i < n-1 and not compare(x, keys[i+1]) < 0:
                 s = "key %r at index %d >= key %r at index %d" % (
                     x, i, keys[i+1], i+1)
                 self.complain(s, obj, path)
             i += 1
 
     def complain(self, msg, obj, path):
-        s = "%s, in %s, path from root %s" % (
+        s = "{}, in {}, path from root {}".format(
                 msg,
                 type_and_adr(obj),
                 ".".join(map(str, path)))
         self.errors.append(s)
 
 class Printer(Walker): # pragma: no cover
     def __init__(self, obj):
@@ -436,15 +436,15 @@
                   type_and_adr(obj),
                   len(keys)))
         indent += "    "
         n = len(keys)
         for i in range(n):
             print("%skey %d: %r" % (indent, i, keys[i]),)
             if is_mapping:
-                print("value %r" % (values[i],))
+                print("value {!r}".format(values[i]))
 
 def check(btree):
     """Check internal value-based invariants in a BTree or TreeSet.
 
     The ``BTrees._base._Tree._check`` method checks internal C-level pointer consistency.
     The :func:`~BTrees.check.check` function here checks value-based invariants:  whether the
     keys in leaf bucket and internal nodes are in strictly increasing order,
```

### Comparing `BTrees-4.9.2/src/BTrees/floatvaluemacros.h` & `BTrees-5.0/src/BTrees/floatvaluemacros.h`

 * *Files identical despite different names*

### Comparing `BTrees-4.9.2/src/BTrees/intkeymacros.h` & `BTrees-5.0/src/BTrees/intkeymacros.h`

 * *Files identical despite different names*

### Comparing `BTrees-4.9.2/src/BTrees/intvaluemacros.h` & `BTrees-5.0/src/BTrees/intvaluemacros.h`

 * *Files identical despite different names*

### Comparing `BTrees-4.9.2/src/BTrees/objectkeymacros.h` & `BTrees-5.0/src/BTrees/objectkeymacros.h`

 * *Files 22% similar despite different names*

```diff
@@ -16,26 +16,15 @@
     /*        arg->ob_type->tp_compare, */
     /*        ((PyTypeObject *)object_)->ob_type->tp_compare); */
     if (arg == Py_None) {
       return 1;
     }
 
 
-#ifdef PY3K
     if (Py_TYPE(arg)->tp_richcompare == Py_TYPE(object_)->tp_richcompare)
-#else
-    if ((Py_TYPE(arg)->tp_richcompare == NULL
-	 && Py_TYPE(arg)->tp_compare == Py_TYPE(object_)->tp_compare)
-	/* Also exclude new-style classes. On Python 2, they can be compared,
-	   but order by address, making them not suitable for BTrees. */
-	|| PyType_CheckExact(arg)
-	/* But let classes with a meta class that implements comparison through. */
-	|| (PyType_Check(arg) && Py_TYPE(arg)->tp_richcompare == PyType_Type.tp_richcompare)
-	)
-#endif
     {
         PyErr_Format(PyExc_TypeError,
 		     "Object of class %s has default comparison",
 		     Py_TYPE(arg)->tp_name);
         return 0;
     }
     return 1;
```

### Comparing `BTrees-4.9.2/src/BTrees/sorters.c` & `BTrees-5.0/src/BTrees/sorters.c`

 * *Files identical despite different names*

### Comparing `BTrees-4.9.2/src/BTrees/tests/_test_builder.py` & `BTrees-5.0/src/BTrees/tests/_test_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from .common import itemsToSet
 from .common import makeMapBuilder
 from .common import makeSetBuilder
 from .common import TestLongIntKeys
 from .common import TestLongIntValues
 
 
-class _FilteredModuleProxy(object):
+class _FilteredModuleProxy:
     """
     Accesses either ``<name>`` or ``<name>Py`` from a module.
 
     This conveniently lets us avoid lots of 'getattr' calls.
 
     Accessing ``def_<name>`` returns a callable that
     returns ``<name>``. This is suitable for use as class attributes.
@@ -59,33 +59,32 @@
         return attr
 
 
 def _flattened(*args):
     def f(tuple_or_klass):
         if isinstance(tuple_or_klass, tuple):
             for x in tuple_or_klass:
-                for c in f(x):
-                    yield c
+                yield from f(x)
         else:
             yield tuple_or_klass
 
     return tuple(f(args))
 
-class ClassBuilder(object):
+class ClassBuilder:
 
     # Use TestAuto as a prefix to avoid clashing with manual tests
     TESTCASE_PREFIX = 'TestAuto'
 
     def __init__(self, btree_module, btree_tests_base=BTreeTests):
         self.btree_module = btree_module
         # These will be instances of _datatypes.DataType
         self.key_type = btree_module.BTreePy._to_key
         self.value_type = btree_module.BTreePy._to_value
 
-        class _BoundsMixin(object):
+        class _BoundsMixin:
             # For test purposes, we can only support negative keys if they are ordered like
             # integers. Our int -> 2 byte conversion for fsBTree doesn't do this.
             # -1 is \xff\xff which is the largest possible key.
             SUPPORTS_NEGATIVE_KEYS = (
                 self.key_type.get_lower_bound() != 0
                 and self.key_type.coerce(-1) < self.key_type.coerce(0)
             )
```

### Comparing `BTrees-4.9.2/src/BTrees/tests/common.py` & `BTrees-5.0/src/BTrees/tests/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,43 +7,35 @@
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE
 #
 ##############################################################################
-from __future__ import division
 
 import sys
 import functools
 import unittest
 import platform
 from unittest import skip
 
-
-from BTrees._compat import PY3
 from BTrees._compat import _c_optimizations_ignored
 from BTrees._compat import PYPY
 from BTrees._base   import _tp_name
 
 def _no_op(test_method):
     return test_method
 
 try:
     __import__('ZODB')
 except ImportError:
     _skip_wo_ZODB = skip('ZODB not available')
 else:
     _skip_wo_ZODB = _no_op
 
-if PY3:
-    _skip_under_Py3k = skip("Not on Python 3")
-else:
-    _skip_under_Py3k = _no_op
-
 if platform.architecture()[0] == '32bit':
     _skip_on_32_bits = skip("32-bit platform")
 else:
     _skip_on_32_bits = _no_op
 
 if _c_optimizations_ignored():
     skipOnPurePython = skip("Not on Pure Python")
@@ -79,23 +71,23 @@
         if not (self.SUPPORTS_NEGATIVE_KEYS and self.SUPPORTS_NEGATIVE_VALUES):
             with self.assertRaises(UnsignedError):
                 func(self)
         else:
             func(self)
     return test
 
-class SignedMixin(object):
+class SignedMixin:
     SUPPORTS_NEGATIVE_KEYS = True
     SUPPORTS_NEGATIVE_VALUES = True
     #: The values to pass to ``random.randrange()`` to generate
     #: valid keys.
     KEY_RANDRANGE_ARGS = (-2000, 2001)
 
 
-class ZODBAccess(object):
+class ZODBAccess:
 
     db = None
 
     def tearDown(self):
         if self.db is not None:
             self.db.close()
             del self.db
@@ -131,15 +123,15 @@
     def _getTargetInterface(self):
         raise NotImplementedError("subclass must return the expected interface ")
 
     def _makeOne(self):
         return self._getTargetClass()()
 
     def setUp(self):
-        super(Base, self).setUp()
+        super().setUp()
         _skip_if_pure_py_and_py_test(self)
 
     def coerce_to_key(self, item):
         return item
 
     def coerce_to_value(self, value):
         return value
@@ -196,35 +188,33 @@
         # Now make sure that it actually has the required methods.
         # First, get the required methods:
         abc_attrs = set(dir(abc))
         # If the method was None, that means it's not required;
         # if it's not callable, it's not a method (None is not callable)
         # If it's a private attribute (starting with only one _), it's
         # an implementation detail to ignore.
-        abc_attrs -= set(x for x in abc_attrs
+        abc_attrs -= {x for x in abc_attrs
                          if (x[0] == '_' and x[1] != '_')
-                         or not callable(getattr(abc, x, None)))
+                         or not callable(getattr(abc, x, None))}
         # Drop things from Python typing and zope.interface that may or may not
         # be present.
         abc_attrs -= {
             '__provides__',
             '__implemented__',
             '__providedBy__',
-            '__metaclass__', # Python 2.7
-            '__class_getitem__', # Python 3.9
+            '__class_getitem__', # Python 3.9+
             # Also the equality and comparison operators;
-            # we don't implement those methods, but the ABC does. On Python
-            # 3, we seem to inherit them from somewhere, but we don't on Python 3
+            # we don't implement those methods, but the ABC does.
             '__lt__', '__le__', '__eq__', '__gt__', '__ge__', '__ne__',
         }
         btr_attrs = set(dir(type(t)))
 
         missing_attrs = abc_attrs - btr_attrs
         self.assertFalse(sorted(missing_attrs),
-                         "Class %r is missing these methods: %s" % (type(t), missing_attrs))
+                         "Class {!r} is missing these methods: {}".format(type(t), missing_attrs))
 
     def testPersistentSubclass(self):
         # Can we subclass this and Persistent?
         # https://github.com/zopefoundation/BTrees/issues/78
         import persistent
 
         class PersistentSubclass(persistent.Persistent):
@@ -479,15 +469,15 @@
 
         if type(t) is not t.__class__:
             # We're fibbing; this breaks issubclass of itself,
             # contrary to the usual mechanism
             self.assertFalse(issubclass(t.__class__, type(t)))
 
 
-        class NonSub(object):
+        class NonSub:
             pass
 
         self.assertFalse(issubclass(NonSub, type(t)))
         self.assertFalse(isinstance(NonSub(), type(t)))
 
 class MappingBase(Base): # pylint:disable=too-many-public-methods
     # Tests common to mappings (buckets, btrees)
@@ -497,16 +487,16 @@
         # Make some data
         to_key = self.coerce_to_key
         to_value = self.coerce_to_value
         for i in range(l):
             t[to_key(i)] = to_value(i)
 
     def _getCollectionsABC(self):
-        from BTrees._compat import collections_abc
-        return collections_abc.MutableMapping
+        import collections.abc
+        return collections.abc.MutableMapping
 
     def test_popitem(self):
         t = self._makeOne()
         K = self.KEYS
         V = self.VALUES
         # Empty
         with self.assertRaises(KeyError):
@@ -896,15 +886,14 @@
 
     def testSlicing(self): # pylint:disable=too-many-locals
         # Test that slicing of .keys()/.values()/.items() works exactly the
         # same way as slicing a Python list with the same contents.
         # This tests fixes to several bugs in this area, starting with
         # http://collector.zope.org/Zope/419,
         # "BTreeItems slice contains 1 too many elements".
-        from .._compat import xrange
         t = self._makeOne()
         val_multiplier = -2 if self.SUPPORTS_NEGATIVE_VALUES else 2
         K = self.KEYS
         V = self.VALUES
         for n in range(10):
             t.clear()
             self.assertEqual(len(t), 0)
@@ -966,15 +955,15 @@
                     self.assertEqual(list(x), values[lo:hi])
 
                     x = islice[lo:hi]
                     self.assertEqual(list(x), items[lo:hi])
 
         # The specific test case from Zope collector 419.
         t.clear()
-        for i in xrange(100):
+        for i in range(100):
             t[K[i]] = self.VALUES[1]
         tslice = t.items()[20:80]
         self.assertEqual(len(tslice), 60)
         self.assertEqual(list(tslice), list(zip(
             [K[x] for x in range(20, 80)],
             [V[1]] * 60
         )))
@@ -1243,45 +1232,44 @@
         self.__test_value(2.5)
 
     def test_assign_value_type_None(self):
         self.__test_value(None)
 
     def testNewStyleClassAsKeyNotAllowed(self):
         m = self._makeOne()
-        class New(object):
+        class New:
             pass
 
         with self.assertRaises(TypeError):
             m[New] = self.getTwoValues()[0]
 
-    def testOldStyleClassAsKeyNotALlowed(self):
+    def testClassAsKeyNotAllowed(self):
         m = self._makeOne()
-        class Old: # Python 2: Old style class
+        class Cls:
             pass
 
         with self.assertRaises(TypeError):
-            m[Old] = self.getTwoValues()[0]
+            m[Cls] = self.getTwoValues()[0]
 
     def testNewStyleClassWithCustomMetaClassNotAllowed(self):
 
         class Meta(type):
             pass
 
         cls = Meta('Class', (object,), {})
         m = self._makeOne()
         with self.assertRaises(TypeError):
             m[cls] = self.getTwoValues()[0]
 
     def testEmptyFirstBucketReportedByGuido(self):
         # This was for Integer keys
-        from .._compat import xrange
         b = self._makeOne()
-        for i in xrange(29972): # reduce to 29971 and it works
+        for i in range(29972): # reduce to 29971 and it works
             b[self.coerce_to_key(i)] = self.coerce_to_value(i)
-        for i in xrange(30): # reduce to 29 and it works
+        for i in range(30): # reduce to 29 and it works
             del b[self.coerce_to_key(i)]
             try:
                 big_key = self.coerce_to_key(i + 40000)
             except TypeError:
                 # fsBtree only has a two-byte key
                 self.skipTest('Key to big')
             b[big_key] = self.coerce_to_value(i)
@@ -1850,15 +1838,15 @@
         # to set _p_changed (adding the first item sets it because
         # the _firstbucket gets set, but the second item only grew the
         # existing bucket)
         t = self._makeOne()
         # Note that for the property to actually hold, we have to fake a
         # _p_jar and _p_oid
         t._p_oid = b'\0\0\0\0\0'
-        class Jar(object):
+        class Jar:
             def __init__(self):
                 self._cache = self
                 self.registered = None
 
             def mru(self, arg):
                 pass
             def readCurrent(self, arg):
@@ -1904,15 +1892,15 @@
         # get set
         t = self._makeOne()
         K = self.KEYS
         V = self.VALUES
         # Note that for the property to actually hold, we have to fake a
         # _p_jar and _p_oid
         t._p_oid = b'\0\0\0\0\0'
-        class Jar(object):
+        class Jar:
             def __init__(self):
                 self._cache = self
                 self.registered = None
 
             def mru(self, arg):
                 pass
             def readCurrent(self, arg):
@@ -2001,16 +1989,16 @@
         self.assertEqual(str(exc.exception), typeErrOK)
 
 
 class NormalSetTests(Base):
     # Test common to all set types
 
     def _getCollectionsABC(self):
-        from BTrees._compat import collections_abc
-        return collections_abc.MutableSet
+        import collections.abc
+        return collections.abc.MutableSet
 
     def _populate(self, t, l):
         # Make some data
         t.update(self.coerce_to_key(k) for k in range(l))
 
     def test_isdisjoint(self):
         t = self._makeOne()
@@ -2020,32 +2008,32 @@
         # Empty sequences
         self.assertTrue(t.isdisjoint(()))
         self.assertTrue(t.isdisjoint([]))
         self.assertTrue(t.isdisjoint(set()))
         # non-empty sequences but empty set
         self.assertTrue(t.isdisjoint((K[1], K[2])))
         self.assertTrue(t.isdisjoint([K[1], K[2]]))
-        self.assertTrue(t.isdisjoint(set((K[1], K[2]))))
+        self.assertTrue(t.isdisjoint({K[1], K[2]}))
         self.assertTrue(t.isdisjoint(K[k] for k in range(10)))
 
         # non-empty sequences and non-empty set, null intersection
         self._populate(t, 2)
         self.assertEqual(set(t), {K[0], K[1]})
 
         self.assertTrue(t.isdisjoint((K[2], K[3])))
         self.assertTrue(t.isdisjoint([K[2], K[3]]))
-        self.assertTrue(t.isdisjoint(set((K[2], K[3]))))
+        self.assertTrue(t.isdisjoint({K[2], K[3]}))
         self.assertTrue(t.isdisjoint(K[k] for k in range(2, 10)))
 
         # non-null intersection
         self.assertFalse(t.isdisjoint(t))
         self.assertFalse(t.isdisjoint((K[0],)))
         self.assertFalse(t.isdisjoint((K[1],)))
         self.assertFalse(t.isdisjoint([K[2], K[3], K[0]]))
-        self.assertFalse(t.isdisjoint(set((K[2], K[3], K[1]))))
+        self.assertFalse(t.isdisjoint({K[2], K[3], K[1]}))
         self.assertFalse(t.isdisjoint(K[k] for k in range(1, 10)))
 
     def test_discard(self):
         t = self._makeOne()
         K = self.KEYS
         # empty set, raises no error, even if the key is
         # of the wrong type
@@ -2084,28 +2072,28 @@
         orig_t = t
         t |= (K[1],)
         t |= [K[2],]
         t |= {K[1], K[2], K[3]}
         t |= (K[k] for k in range(10))
         t |= t
         self.assertIs(t, orig_t)
-        self.assertEqual(set(t), set(K[k] for k in range(10)))
+        self.assertEqual(set(t), {K[k] for k in range(10)})
 
     def test___iand__(self):
         t = self._makeOne()
         K = self.KEYS
         orig_t = t
         t &= (K[1],)
         t &= [K[2],]
         t &= {K[3], K[4]}
         self.assertIs(t, orig_t)
         self.assertEqual(set(t), set())
 
         self._populate(t, 10)
-        self.assertEqual(set(t), set(K[k] for k in range(10)))
+        self.assertEqual(set(t), {K[k] for k in range(10)})
 
         t &= (K[1], K[2], K[3])
         self.assertIs(t, orig_t)
         self.assertEqual(set(t), {K[1], K[2], K[3]})
 
     def test___isub__(self):
         t = self._makeOne()
@@ -2114,15 +2102,15 @@
         t -= (K[1],)
         t -= [K[2],]
         t -= {K[3], K[4]}
         self.assertIs(t, orig_t)
         self.assertEqual(set(t), set())
 
         self._populate(t, 10)
-        self.assertEqual(set(t), set(K[k] for k in range(10)))
+        self.assertEqual(set(t), {K[k] for k in range(10)})
 
         t -= (K[1], K[2], K[3])
         self.assertIs(t, orig_t)
         self.assertEqual(set(t), {K[0], K[4], K[5], K[6], K[7], K[8], K[9]})
 
         t -= t
         self.assertIs(t, orig_t)
@@ -2190,76 +2178,63 @@
         t = self._makeOne()
         k = self.KEYS[5]
         t.insert(k)
         self.assertEqual(t.insert(k), 0)
         self.assertEqual(t.add(k), 0)
 
     def testInsert(self):
-        from .._compat import PY2
         t = self._makeOne()
         K = self.KEYS
         t.insert(K[1])
-        if PY2:
-            self.assertTrue(t.has_key(K[1]))
         self.assertTrue(K[1] in t)
         self.assertTrue(K[2] not in t)
 
     def testBigInsert(self):
-        from .._compat import PY2
-        from .._compat import xrange
         t = self._makeOne()
-        r = xrange(10000)
+        r = range(10000)
         to_key = self.coerce_to_key
         for x in r:
             t.insert(to_key(x))
         for x in r:
             x = to_key(x)
-            if PY2:
-                self.assertTrue(t.has_key(x))
             self.assertTrue(x in t)
 
     def testRemoveSucceeds(self):
-        from .._compat import xrange
         t = self._makeOne()
-        r = xrange(10000)
+        r = range(10000)
         to_key = self.coerce_to_key
         for x in r:
             t.insert(to_key(x))
         for x in r:
             t.remove(to_key(x))
 
     def testRemoveFails(self):
         self.assertRaises(KeyError, self._removenonexistent)
 
     def _removenonexistent(self):
         self._makeOne().remove(self.KEYS[1])
 
     def testHasKeyFails(self):
-        from .._compat import PY2
         t = self._makeOne()
-        if PY2:
-            self.assertTrue(not t.has_key(1))
         self.assertTrue(1 not in t)
 
     def testKeys(self):
-        from .._compat import xrange
         t = self._makeOne()
-        r = [self.KEYS[x] for x in xrange(1000)]
+        r = [self.KEYS[x] for x in range(1000)]
         for x in r:
             t.insert(x)
         diff = lsubtract(t.keys(), r)
         self.assertEqual(diff, [])
         diff = lsubtract(t.keys(None, None), r)
         self.assertEqual(diff, [])
 
 
     def testClear(self):
-        from .._compat import xrange
         t = self._makeOne()
-        r = xrange(1000)
+        r = range(1000)
         K = self.KEYS
         for x in r:
             t.insert(K[x])
         t.clear()
         diff = lsubtract(t.keys(), [])
         self.assertEqual(diff, [], diff)
 
@@ -2411,15 +2386,15 @@
         # deleting an item in a small set to fail to set _p_changed.
         # There must be at least two objects so that _firstbucket doesn't
         # get set
         t = self._makeOne()
         # Note that for the property to actually hold, we have to fake a
         # _p_jar and _p_oid
         t._p_oid = b'\0\0\0\0\0'
-        class Jar(object):
+        class Jar:
             def __init__(self):
                 self._cache = self
                 self.registered = None
 
             def mru(self, arg):
                 pass
             def readCurrent(self, arg):
@@ -2442,15 +2417,15 @@
     def testAddingOneSetsChanged(self):
         # A bug in the BTree Set Python implementation once caused
         # adding an object not to set _p_changed
         t = self._makeOne()
         # Note that for the property to actually hold, we have to fake a
         # _p_jar and _p_oid
         t._p_oid = b'\0\0\0\0\0'
-        class Jar(object):
+        class Jar:
             def __init__(self):
                 self._cache = self
                 self.registered = None
 
             def mru(self, arg):
                 pass
             def readCurrent(self, arg):
@@ -2466,36 +2441,34 @@
         # Whether or not doing `t.add(0)` again would result in
         # _p_changed being set depends on whether this is a TreeSet or a plain Set
 
 
 class ExtendedSetTests(NormalSetTests):
 
     def testLen(self):
-        from .._compat import xrange
         t = self._makeOne()
-        r = xrange(10000)
+        r = range(10000)
         to_key = self.coerce_to_key
         for x in r:
             t.insert(to_key(x))
         self.assertEqual(len(t), 10000, len(t))
 
     def testGetItem(self):
-        from .._compat import xrange
         t = self._makeOne()
-        r = xrange(10000)
+        r = range(10000)
         to_key = self.coerce_to_key
         for x in r:
             t.insert(to_key(x))
         for x in r:
             self.assertEqual(t[x], to_key(x))
 
 class KeyCoercionFailed(Exception):
     """Raised when we use a static key that we expect to be able to fit."""
 
-class InternalKeysMappingTest(object):
+class InternalKeysMappingTest:
     # There must not be any internal keys not in the BTree
 
     def _makeOne(self):
         return self._getTargetClass()()
 
     def add_key(self, tree, i):
         value = self.coerce_to_value(i)
@@ -2568,15 +2541,15 @@
         data = tree.__getstate__()[0]
         self.assertTrue(data[1] != key)
 
         transaction.abort()
         db.close()
 
 
-class ModuleTest(object):
+class ModuleTest:
     # test for presence of generic names in module
     prefix = ''
     key_type = None
     value_type = None
     def _getModule(self):
         raise NotImplementedError
 
@@ -2632,18 +2605,18 @@
         self._check_union_presence(self.value_type, 'weightedIntersection')
 
     # The multiunion function requires the key type to support unions
     def test_multiunion_presence(self):
         self._check_union_presence(self.key_type, 'multiunion')
 
 
-class I_SetsBase(object):
+class I_SetsBase:
 
     def setUp(self):
-        super(I_SetsBase, self).setUp()
+        super().setUp()
         _skip_if_pure_py_and_py_test(self)
 
     def _getTargetClass(self):
         raise NotImplementedError
 
     def _makeOne(self):
         return self._getTargetClass()()
@@ -2684,15 +2657,15 @@
 LARGEST_64_BITS = 0x7fffffffffffffff # Signed. 2**63 - 1
 SMALLEST_64_BITS = -LARGEST_64_BITS - 1
 
 SMALLEST_POSITIVE_65_BITS = LARGEST_64_BITS + 1
 LARGEST_NEGATIVE_65_BITS = SMALLEST_64_BITS - 1
 
 
-class TestLongIntSupport(object):
+class TestLongIntSupport:
 
     def getTwoValues(self):
         # Return two distinct values; these must compare as un-equal.
         #
         # These values must be usable as values.
         return object(), object()
 
@@ -2807,17 +2780,17 @@
         return setbuilder(self.KEYS[k] for k in keys)
     return result
 
 # Subclasses have to set up:
 #     builders() - function returning functions to build inputs,
 #     each returned callable takes an optional keys arg
 #     intersection, union, difference - set to the type-correct versions
-class SetResult(object):
+class SetResult:
     def setUp(self):
-        super(SetResult, self).setUp()
+        super().setUp()
         _skip_if_pure_py_and_py_test(self)
 
         rawAkeys = [1,    3,    5, 6] # pylint:disable=bad-whitespace
         rawBkeys = [   2, 3, 4,    6, 7] # pylint:disable=bad-whitespace
         self.Akeys = [self.KEYS[k] for k in rawAkeys]
         self.Bkeys = [self.KEYS[k] for k in rawBkeys]
         self.As = [makeset(rawAkeys) for makeset in self.builders()]
@@ -3131,15 +3104,15 @@
 # Subclasses must set up (as class variables):
 #     multiunion, union
 #     mkset, mktreeset
 #     mkbucket, mkbtree
 class MultiUnion(SignedMixin):
 
     def setUp(self):
-        super(MultiUnion, self).setUp()
+        super().setUp()
         _skip_if_pure_py_and_py_test(self)
 
     def testEmpty(self):
         self.assertEqual(len(self.multiunion([])), 0)
 
     def _testOne(self, builder):
         for sequence in (
@@ -3171,16 +3144,15 @@
         self._testOne(tuple)
 
     def testOneSet(self):
         self._testOne(set)
 
     def testOneGenerator(self):
         def generator(seq):
-            for i in seq:
-                yield i
+            yield from seq
 
         self._testOne(generator)
 
     def testValuesIgnored(self):
         for builder in self.mkbucket, self.mkbtree, dict:
             input = builder([(1, 2), (3, 4), (5, 6)])
             output = self.multiunion([input])
@@ -3220,16 +3192,15 @@
                 self.multiunion((kind(i1),))
 
     def testBadIterable(self):
         class MyException(Exception):
             pass
 
         def gen():
-            for i in range(3):
-                yield i
+            yield from range(3)
             raise MyException
 
         with self.assertRaises(MyException):
             self.multiunion((gen(),))
 
     def testBigInput(self):
         N = 100000
@@ -3275,22 +3246,22 @@
         fast = self.multiunion(list(range(N))) # like N distinct singleton sets
         self.assertEqual(len(slow), N)
         self.assertEqual(len(fast), N)
         self.assertEqual(list(slow), list(fast))
         self.assertEqual(list(fast), list(range(N)))
 
 
-class ConflictTestBase(SignedMixin, object):
+class ConflictTestBase(SignedMixin):
     # Tests common to all types: sets, buckets, and BTrees
 
     storage = None
     db = None
 
     def setUp(self):
-        super(ConflictTestBase, self).setUp()
+        super().setUp()
         _skip_if_pure_py_and_py_test(self)
         def identity(x):
             return x
 
         self.key_tx = abs if not self.SUPPORTS_NEGATIVE_KEYS else identity
         self.val_tx = abs if not self.SUPPORTS_NEGATIVE_VALUES else identity
```

### Comparing `BTrees-4.9.2/src/BTrees/tests/testBTrees.py` & `BTrees-5.0/src/BTrees/tests/testBTrees.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,15 @@
             # at some unrelated line.
             del t   # trigger destructor
 
 
 LP294788_ids = {}
 
 
-class ToBeDeleted(object):
+class ToBeDeleted:
     def __init__(self, id):
         assert isinstance(id, int) #we don't want to store any object ref here
         self.id = id
 
         global LP294788_ids
         LP294788_ids[id] = 1
 
@@ -305,15 +305,15 @@
             if trandom.random() > 0.1 or not ids:
                 #add
                 id = None
                 while id is None or id in ids:
                     id = trandom.randint(0, 1000000)
 
                 ids[id] = 1
-                t[id] = (id, ToBeDeleted(id), u'somename')
+                t[id] = (id, ToBeDeleted(id), 'somename')
             else:
                 #del
                 keys = list(ids.keys())
                 if keys:
                     id = trandom.choice(keys)
                     del t[id]
                     del ids[id]
@@ -374,15 +374,15 @@
         ids = {}
         for i in range(1024):
             if trandom.random() > 0.1 or not ids:
                 #add
                 id = None
                 while id is None or id in ids:
                     id = trandom.randint(0, 1000000)
-                    id = (id, ToBeDeleted(id), u'somename')
+                    id = (id, ToBeDeleted(id), 'somename')
 
                 ids[id] = 1
                 t[id] = 1
             else:
                 #del
                 id = trandom.choice(list(ids.keys()))
                 del ids[id]
```

### Comparing `BTrees-4.9.2/src/BTrees/tests/testBTreesUnicode.py` & `BTrees-5.0/src/BTrees/tests/test__datatypes.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,87 +1,94 @@
 ##############################################################################
 #
-# Copyright (c) 2001, 2002 Zope Foundation and Contributors.
+# Copyright 2012 Zope Foundation and Contributors.
 # All Rights Reserved.
 #
 # This software is subject to the provisions of the Zope Public License,
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
-# FOR A PARTICULAR PURPOSE
+# FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 
 import unittest
-from .common import _skip_under_Py3k
+from BTrees import _datatypes
 
-# When an OOBtree contains unicode strings as keys,
-# it is neccessary accessing non-unicode strings are
-# either ascii strings or encoded as unicoded using the
-# corresponding encoding
-
-encoding = 'ISO-8859-1'
-
-class TestBTreesUnicode(unittest.TestCase):
-    """ test unicode"""
-
-    def setUp(self):
-        #setup an OOBTree with some unicode strings
-        from BTrees.OOBTree import OOBTree
-
-
-        self.s = b'dreit\xe4gigen'.decode('latin1')
-
-        self.data = [(b'alien', 1),
-                     (b'k\xf6nnten', 2),
-                     (b'fox', 3),
-                     (b'future', 4),
-                     (b'quick', 5),
-                     (b'zerst\xf6rt', 6),
-                     (u'dreit\xe4gigen', 7),
-                    ]
-
-        self.tree = OOBTree()
-        for k, v in self.data:
-            if isinstance(k, bytes):
-                k = k.decode('latin1')
-            self.tree[k] = v
-
-    def testAllKeys(self):
-        # check every item of the tree
-        for k, v in self.data:
-            if isinstance(k, bytes):
-                k = k.decode(encoding)
-            self.assertIn(k, self.tree)
-            self.assertEqual(self.tree[k], v)
-
-    def testUnicodeKeys(self):
-        # try to access unicode keys in tree
-        k, v = self.data[-1]
-        self.assertEqual(k, self.s)
-        self.assertEqual(self.tree[k], v)
-        self.assertEqual(self.tree[self.s], v)
-
-
-    def testAsciiKeys(self):
-        # try to access some "plain ASCII" keys in the tree;
-        # they get upconverted to unicode for comparison on Python 2
-        for k, v in self.data[0], self.data[2]:
-            self.assertIsInstance(k, bytes)
-            if bytes is str:
-                self.assertEqual(self.tree[k], v)
-            else:
-                with self.assertRaises(TypeError):
-                    self.tree.__getitem__(k)
-
-
-class TestBTreeBucketUnicode(unittest.TestCase):
-
-    def testUnicodeRepr(self):
-        # Regression test for
-        # https://github.com/zopefoundation/BTrees/issues/106
-        items = [(1, u'\uaabb')]
-        from BTrees.OOBTree import OOBucket
-        bucket = OOBucket(items)
-        self.assertEqual(repr(bucket),
-                         'BTrees.OOBTree.OOBucket(%s)' % repr(items))
+to_ob = _datatypes.Any()
+to_int = _datatypes.I()
+to_float = _datatypes.F()
+to_long = _datatypes.L()
+to_2_bytes = _datatypes.f()
+to_6_bytes = _datatypes.s()
+
+class TestDatatypes(unittest.TestCase):
+    def test_to_ob(self):
+        for thing in "abc", 0, 1.3, (), frozenset((1, 2)), object():
+            self.assertTrue(to_ob(thing) is thing)
+
+    def test_to_int_w_int(self):
+        self.assertEqual(to_int(3), 3)
+
+    def test_to_int_w_long_in_range(self):
+        try:
+            self.assertEqual(to_int(long(3)), 3)
+        except NameError: #Python3
+            pass
+
+    def test_to_int_w_overflow(self):
+        self.assertRaises(TypeError, to_int, 2**64)
+
+    def test_to_int_w_invalid(self):
+        self.assertRaises(TypeError, to_int, ())
+
+    def test_to_float_w_float(self):
+        self.assertEqual(to_float(3.14159), 3.14159)
+
+    def test_to_float_w_int(self):
+        self.assertEqual(to_float(3), 3.0)
+
+    def test_to_float_w_invalid(self):
+        self.assertRaises(TypeError, to_float, ())
+
+    def test_to_long_w_int(self):
+        self.assertEqual(to_long(3), 3)
+
+    def test_to_long_w_long_in_range(self):
+        try:
+            self.assertEqual(to_long(long(3)), 3)
+        except NameError: #Python3
+            pass
+
+    def test_to_long_w_overflow(self):
+        self.assertRaises(TypeError, to_long, 2**64)
+
+    def test_to_long_w_invalid(self):
+        self.assertRaises(TypeError, to_long, ())
+
+    def test_to_2_bytes_w_ok(self):
+        self.assertEqual(to_2_bytes(b'ab'), b'ab')
+
+    def test_to_2_bytes_w_invalid_length(self):
+        self.assertRaises(TypeError, to_2_bytes, b'a')
+        self.assertRaises(TypeError, to_2_bytes, b'abcd')
+
+    def test_to_6_bytes_w_ok(self):
+        self.assertEqual(to_6_bytes(b'abcdef'), b'abcdef')
+
+    def test_to_6_bytes_w_invalid_length(self):
+        self.assertRaises(TypeError, to_6_bytes, b'a')
+        self.assertRaises(TypeError, to_6_bytes, b'abcd')
+
+    def test_coerce_to_6_bytes(self):
+        # correct input is passed through
+        self.assertEqual(to_6_bytes.coerce(b'abcdef'), b'abcdef')
+
+        # small positive integers are converted
+        self.assertEqual(to_6_bytes.coerce(1), b'\x00\x00\x00\x00\x00\x01')
+
+        # negative values are disallowed
+        self.assertRaises(TypeError, to_6_bytes.coerce, -1)
+
+        # values outside the bigger than 64-bits are disallowed
+        self.assertRaises(TypeError, to_6_bytes.coerce, 2 ** 64 + 1)
```

### Comparing `BTrees-4.9.2/src/BTrees/tests/testConflict.py` & `BTrees-5.0/src/BTrees/tests/testConflict.py`

 * *Files identical despite different names*

### Comparing `BTrees-4.9.2/src/BTrees/tests/testPersistency.py` & `BTrees-5.0/src/BTrees/tests/testPersistency.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     @_skip_wo_ZODB
     def test_empty_bucket_persistency(self):
         from transaction import commit
         root = self._getRoot()
         try:
             # tree with 3 buckets (internal implementation details)
             tree = OOBTree(
-                dict((i, i) for i in range(3 * BUCKET_SIZE // 2 + 2)))
+                {i: i for i in range(3 * BUCKET_SIZE // 2 + 2)})
             root["tree"] = tree
             commit()
             # almost clear the second bucket keeping the last element
             for i in range(BUCKET_SIZE // 2, BUCKET_SIZE - 1):
                 del tree[i]
             commit()
             del tree[BUCKET_SIZE - 1]  # remove the last element
```

### Comparing `BTrees-4.9.2/src/BTrees/tests/test_Length.py` & `BTrees-5.0/src/BTrees/tests/test_Length.py`

 * *Files 9% similar despite different names*

```diff
@@ -59,41 +59,14 @@
         self.assertEqual(length.value, 3)
 
     def test_change_w_negative_delta(self):
         length = self._makeOne()
         length.change(-3)
         self.assertEqual(length.value, -3)
 
-    def test_change_overflows_to_long(self):
-        import sys
-        try:
-            length = self._makeOne(sys.maxint)
-        except AttributeError: # pragma: no cover Py3k
-            return
-        else: # pragma: no cover Py2
-            self.assertEqual(length(), sys.maxint)
-            self.assertTrue(type(length()) is int)
-            length.change(+1)
-            self.assertEqual(length(), sys.maxint + 1)
-            self.assertTrue(type(length()) is long)
-
-    def test_change_underflows_to_long(self):
-        import sys
-        try:
-            minint = (-sys.maxint) - 1
-        except AttributeError: # pragma: no cover Py3k
-            return
-        else: # pragma: no cover Py2
-            length = self._makeOne(minint)
-            self.assertEqual(length(), minint)
-            self.assertTrue(type(length()) is int)
-            length.change(-1)
-            self.assertEqual(length(), minint - 1)
-            self.assertTrue(type(length()) is long)
-
     def test___call___no_args(self):
         length = self._makeOne(42)
         self.assertEqual(length(), 42)
 
     def test___call___w_args(self):
         length = self._makeOne(42)
         self.assertEqual(length(0, None, (), [], {}), 42)
```

### Comparing `BTrees-4.9.2/src/BTrees/tests/test_OOBTree.py` & `BTrees-5.0/src/BTrees/tests/test_OOBTree.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,45 +30,34 @@
         # extensions; old-style instances are too hard to introspect
         # in C.
 
         # This is white box because we know that the check is being
         # used in a function that's used in lots of places.
         # Otherwise, there are many permutations that would have to be
         # checked.
-        from .._compat import PY2
         t = self._makeOne()
 
         class OldStyle:
             pass
 
-        if self._getTargetClass() is OOBTree.OOBTreePy or not PY2:
+        if self._getTargetClass() is OOBTree.OOBTreePy:
             with self.assertRaises(TypeError):
                 t[OldStyle()] = 1
 
-        class C(object):
+        class C:
             pass
 
         with self.assertRaises(TypeError) as raising:
             t[C()] = 1
 
         self.assertEqual(
             raising.exception.args[0],
             "Object of class C has default comparison")
 
-        if PY2: # we only check for __cmp__ on Python2
-
-            class With___cmp__(object):
-                def __cmp__(*args):
-                    return 1
-            c = With___cmp__()
-            t[c] = 1
-
-            t.clear()
-
-        class With___lt__(object):
+        class With___lt__:
             def __lt__(*args):
                 return 1
 
         c = With___lt__()
         t[c] = 1
         t.clear()
 
@@ -80,15 +69,15 @@
         t[c] = 1
 
         t.clear()
 
     def testAcceptDefaultComparisonOnGet(self):
         # Issue #42
         t = self._makeOne()
-        class C(object):
+        class C:
             pass
 
         self.assertEqual(t.get(C(), 42), 42)
         self.assertRaises(KeyError, t.__getitem__, C())
         self.assertFalse(C() in t)
 
 
@@ -154,15 +143,15 @@
 
     def testIdentityTrumpsBrokenComparison(self):
         # Identical keys always match, even if their comparison is
         # broken. See https://github.com/zopefoundation/BTrees/issues/50
         from functools import total_ordering
 
         @total_ordering
-        class Bad(object):
+        class Bad:
             def __eq__(self, other):
                 return False
 
             __lt__ = __cmp__ = __eq__
 
         t = self._makeOne()
         bad_key = Bad()
```

### Comparing `BTrees-4.9.2/src/BTrees/tests/test__base.py` & `BTrees-5.0/src/BTrees/tests/test__base.py`

 * *Files 0% similar despite different names*

```diff
@@ -472,24 +472,24 @@
         bucket = self._makeOne()
         bucket.update({'a': 'b'})
         self.assertEqual(bucket._keys, ['a'])
         self.assertEqual(bucket._values, ['b'])
 
     def test_update_value_w_items(self):
         bucket = self._makeOne()
-        class Foo(object):
+        class Foo:
             def items(self):
                 return [('a', 'b')]
         bucket.update(Foo())
         self.assertEqual(bucket._keys, ['a'])
         self.assertEqual(bucket._values, ['b'])
 
     def test_update_value_w_invalid_items(self):
         bucket = self._makeOne()
-        class Foo(object):
+        class Foo:
             def items(self):
                 return ('a', 'b', 'c')
         self.assertRaises(TypeError, bucket.update, Foo())
 
     def test_update_sequence(self):
         bucket = self._makeOne()
         bucket.update([('a', 'b')])
@@ -1516,23 +1516,23 @@
     def test_update_value_w_iteritems(self):
         tree = self._makeOne()
         tree.update({'a': 'b'})
         self.assertEqual(tree._findbucket('a')['a'], 'b')
 
     def test_update_value_w_items(self):
         tree = self._makeOne()
-        class Foo(object):
+        class Foo:
             def items(self):
                 return [('a', 'b')]
         tree.update(Foo())
         self.assertEqual(tree._findbucket('a')['a'], 'b')
 
     def test_update_value_w_invalid_items(self):
         tree = self._makeOne()
-        class Foo(object):
+        class Foo:
             def items(self):
                 return ('a', 'b', 'c')
         self.assertRaises(TypeError, tree.update, Foo())
 
     def test_update_sequence(self):
         tree = self._makeOne()
         tree.update([('a', 'b')])
@@ -1922,42 +1922,42 @@
         self.assertTrue(tree in jar._current)
 
     def test__del_miss(self):
         tree = self._makeOne({'a': 'b'})
         self.assertRaises(KeyError, tree._del, 'nonesuch')
 
     def test__del_fixes_up_node_key(self):
-        SOURCE = dict([('%05d' % i, i) for i in range(1000)])
+        SOURCE = {'%05d' % i: i for i in range(1000)}
         tree = self._makeOne(SOURCE)
         before = tree._data[1].key
         del tree[before]
         after = tree._data[1].key
         self.assertTrue(after > before)
 
     def test__del_empties_first_bucket_not_zeroth_item(self):
-        SOURCE = dict([('%05d' % i, i) for i in range(1000)])
+        SOURCE = {'%05d' % i: i for i in range(1000)}
         tree = self._makeOne(SOURCE)
         bucket = tree._data[1].child._firstbucket
         next_b = bucket._next
         for key in list(bucket): # don't del while iterting
             del tree[key]
         self.assertTrue(tree._data[1].child._firstbucket is next_b)
 
     def test__del_empties_first_bucket_zeroth_item(self):
-        SOURCE = dict([('%05d' % i, i) for i in range(1000)])
+        SOURCE = {'%05d' % i: i for i in range(1000)}
         tree = self._makeOne(SOURCE)
         bucket = tree._data[0].child._firstbucket
         next_b = bucket._next
         for key in list(bucket): # don't del while iterting
             del tree[key]
         self.assertTrue(tree._data[0].child._firstbucket is next_b)
         self.assertTrue(tree._firstbucket is next_b)
 
     def test__del_empties_other_bucket_not_zeroth_item(self):
-        SOURCE = dict([('%05d' % i, i) for i in range(1000)])
+        SOURCE = {'%05d' % i: i for i in range(1000)}
         tree = self._makeOne(SOURCE)
         bucket = tree._data[1].child._firstbucket._next
         next_b = bucket._next
         for key in list(bucket): # don't del while iterting
             del tree[key]
         self.assertTrue(tree._data[1].child._firstbucket._next is next_b)
 
@@ -2044,15 +2044,15 @@
     def test__check_nonempty_w_null_child(self):
         tree = self._makeOne({'a': 'b'})
         tree._data.append(tree._data[0].__class__('c', None))
         e = self.assertRaises(AssertionError, tree._check)
         self.assertEqual(str(e), "BTree has NULL child")
 
     def test__check_nonempty_w_heterogenous_child(self):
-        class Other(object):
+        class Other:
             pass
         tree = self._makeOne({'a': 'b'})
         tree._data.append(tree._data[0].__class__('c', Other()))
         e = self.assertRaises(AssertionError, tree._check)
         self.assertEqual(str(e), "BTree children have different types")
 
     def test__check_nonempty_w_empty_child(self):
@@ -2069,15 +2069,15 @@
         tree._data.append(c_first.__class__('a', c_tree))
         tree._firstbucket = object()
         e = self.assertRaises(AssertionError, tree._check)
         self.assertEqual(str(e), "BTree has firstbucket different than "
                                  "its first child's firstbucket")
 
     def test__check_nonempty_w_invalid_child(self):
-        class Invalid(object):
+        class Invalid:
             size = 2
         tree = self._makeOne({'a': 'b'})
         tree._data[0].child = Invalid()
         e = self.assertRaises(AssertionError, tree._check)
         self.assertEqual(str(e), "Incorrect child type")
 
     def test__check_branch_traverse_bucket_pointers(self):
@@ -2475,15 +2475,15 @@
         self.assertEqual(len(_set), len(LETTERS))
         for letter in LETTERS:
             self.assertTrue(letter in _set)
 
     def test_update_mppaing(self):
         _set = self._makeOne()
         LETTERS = 'abcdefghijklmnopqrstuvwxyz'
-        a_dict = dict([(y, x) for x, y in enumerate(LETTERS)])
+        a_dict = {y: x for x, y in enumerate(LETTERS)}
         _set.update(a_dict)
         self.assertEqual(len(_set), len(LETTERS))
         for letter in LETTERS:
             self.assertTrue(letter in _set)
 
 
 class Test_set_operation(unittest.TestCase):
@@ -2494,25 +2494,25 @@
         from .._base import set_operation
         return set_operation
 
     def _makeOne(self, func, set_type):
         return self._getTargetClass()(func, set_type)
 
     def test_it(self):
-        class _SetType(object):
+        class _SetType:
             pass
         _called_with = []
         def _func(*args, **kw):
             _called_with.append((args, kw))
         set_op = self._makeOne(_func, _SetType)
         set_op('a', b=1)
         self.assertEqual(_called_with, [((_SetType, 'a',), {'b': 1})])
 
 
-class _SetObBase(object):
+class _SetObBase:
 
     def _makeSet(self, *args):
         return  _Set(*args)
 
     def _makeMapping(self, *args, **kw):
         return  _Mapping(*args, **kw)
 
@@ -2924,32 +2924,32 @@
     def test_MERGE_WEIGHT_numeric(self):
         from BTrees._base import MERGE_WEIGHT_numeric
         faux_self = object()
         self.assertEqual(MERGE_WEIGHT_numeric(faux_self, 1, 17), 17)
         self.assertEqual(MERGE_WEIGHT_numeric(faux_self, 7, 1), 7)
 
 
-class _Cache(object):
+class _Cache:
     def __init__(self):
         self._mru = []
     def mru(self, oid):
         self._mru.append(oid)
 
 
-class _Jar(object):
+class _Jar:
     def __init__(self):
         self._current = set()
         self._cache = _Cache()
     def readCurrent(self, obj):
         self._current.add(obj)
     def register(self, obj):
         pass
 
 
-class _Set(object):
+class _Set:
     def __init__(self, *args, **kw):
         if len(args) == 1 and isinstance(args[0], tuple):
             keys = args[0]
         else:
             keys = set(args)
         self._keys = sorted(keys)
     def keys(self):
@@ -2972,16 +2972,15 @@
             self._values.append(v)
     MERGE_DEFAULT = 42
     def MERGE_WEIGHT(self, v, w):
         return v
     def MERGE(self, v1, w1, v2, w2):
         return v1 * w1 + v2 * w2
     def iteritems(self):
-        for k, v in zip(self._keys, self._values):
-            yield k,v
+        yield from zip(self._keys, self._values)
     def __iter__(self):
         return iter(self._keys)
     def __getitem__(self, key):
         search = dict(zip(self._keys, self._values))
         return search[key]
     def __repr__(self):
         return repr(dict(zip(self._keys, self._values)))
```

### Comparing `BTrees-4.9.2/src/BTrees/tests/test_btreesubclass.py` & `BTrees-5.0/src/BTrees/tests/test_btreesubclass.py`

 * *Files identical despite different names*

### Comparing `BTrees-4.9.2/src/BTrees/tests/test_check.py` & `BTrees-5.0/src/BTrees/tests/test_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 class Test_classify(unittest.TestCase):
 
     def _callFUT(self, obj):
         from BTrees.check import classify
         return classify(obj)
 
     def test_classify_w_unknown(self):
-        class NotClassified(object):
+        class NotClassified:
             pass
         self.assertRaises(KeyError, self._callFUT, NotClassified())
 
     def test_classify_w_bucket(self):
         from BTrees.OOBTree import OOBucketPy
         from BTrees.check import TYPE_BUCKET
         kind, is_mapping = self._callFUT(OOBucketPy())
@@ -66,37 +66,37 @@
 
     def _callFUT(self, obj, is_mapping):
         from BTrees.check import crack_btree
         return crack_btree(obj, is_mapping)
 
     def test_w_empty_tree(self):
         from BTrees.check import BTREE_EMPTY
-        class Empty(object):
+        class Empty:
             def __getstate__(self):
                 return None
         kind, keys, kids = self._callFUT(Empty(), True)
         self.assertEqual(kind, BTREE_EMPTY)
         self.assertEqual(keys, [])
         self.assertEqual(kids, [])
 
     def test_w_degenerate_tree(self):
         from BTrees.check import BTREE_ONE
-        class Degenerate(object):
+        class Degenerate:
             def __getstate__(self):
                 return ((('a', 1, 'b', 2),),)
         kind, keys, kids = self._callFUT(Degenerate(), True)
         self.assertEqual(kind, BTREE_ONE)
         self.assertEqual(keys, ('a', 1, 'b', 2))
         self.assertEqual(kids, None)
 
     def test_w_normal_tree(self):
         from BTrees.check import BTREE_NORMAL
         first_bucket = [object()] * 8
         second_bucket = [object()] * 8
-        class Normal(object):
+        class Normal:
             def __getstate__(self):
                 return ((first_bucket, 'b', second_bucket), first_bucket)
         kind, keys, kids = self._callFUT(Normal(), True)
         self.assertEqual(kind, BTREE_NORMAL)
         self.assertEqual(keys, ['b'])
         self.assertEqual(kids, [first_bucket, second_bucket])
 
@@ -104,39 +104,39 @@
 class Test_crack_bucket(unittest.TestCase):
 
     def _callFUT(self, obj, is_mapping):
         from BTrees.check import crack_bucket
         return crack_bucket(obj, is_mapping)
 
     def test_w_empty_set(self):
-        class EmptySet(object):
+        class EmptySet:
             def __getstate__(self):
                 return ([],)
         keys, values = self._callFUT(EmptySet(), False)
         self.assertEqual(keys, [])
         self.assertEqual(values, [])
 
     def test_w_non_empty_set(self):
-        class NonEmptySet(object):
+        class NonEmptySet:
             def __getstate__(self):
                 return (['a', 'b', 'c'],)
         keys, values = self._callFUT(NonEmptySet(), False)
         self.assertEqual(keys, ['a', 'b', 'c'])
         self.assertEqual(values, [])
 
     def test_w_empty_mapping(self):
-        class EmptyMapping(object):
+        class EmptyMapping:
             def __getstate__(self):
                 return ([], object())
         keys, values = self._callFUT(EmptyMapping(), True)
         self.assertEqual(keys, [])
         self.assertEqual(values, [])
 
     def test_w_non_empty_mapping(self):
-        class NonEmptyMapping(object):
+        class NonEmptyMapping:
             def __getstate__(self):
                 return (['a', 1, 'b', 2, 'c', 3], object())
         keys, values = self._callFUT(NonEmptyMapping(), True)
         self.assertEqual(keys, ['a', 'b', 'c'])
         self.assertEqual(values, [1, 2, 3])
 
 
@@ -144,22 +144,22 @@
 
     def _callFUT(self, obj):
         from BTrees.check import type_and_adr
         return type_and_adr(obj)
 
     def test_type_and_adr_w_oid(self):
         from BTrees.utils import oid_repr
-        class WithOid(object):
+        class WithOid:
             _p_oid = b'DEADBEEF'
         t_and_a = self._callFUT(WithOid())
         self.assertTrue(t_and_a.startswith('WithOid (0x'))
         self.assertTrue(t_and_a.endswith('oid=%s)' % oid_repr(b'DEADBEEF')))
 
     def test_type_and_adr_wo_oid(self):
-        class WithoutOid(object):
+        class WithoutOid:
             pass
         t_and_a = self._callFUT(WithoutOid())
         self.assertTrue(t_and_a.startswith('WithoutOid (0x'))
         self.assertTrue(t_and_a.endswith('oid=None)'))
 
 
 class WalkerTests(unittest.TestCase):
```

### Comparing `BTrees-4.9.2/src/BTrees/tests/test_dynamic_btrees.py` & `BTrees-5.0/src/BTrees/tests/test_dynamic_btrees.py`

 * *Files identical despite different names*

### Comparing `BTrees-4.9.2/src/BTrees/tests/test_fsBTree.py` & `BTrees-5.0/src/BTrees/tests/test_fsBTree.py`

 * *Files identical despite different names*

### Comparing `BTrees-4.9.2/src/BTrees/tests/test_utils.py` & `BTrees-5.0/src/BTrees/tests/test_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,21 +28,14 @@
 
     def test_w_zero(self):
         self.assertEqual(self._callFUT(0), 0)
 
     def test_w_positive(self):
         self.assertEqual(self._callFUT(1), 1)
 
-    def test_w_big_positive(self):
-        import sys
-        try:
-            self.assertEqual(self._callFUT(sys.maxint), sys.maxint)
-        except AttributeError: # pragma: no cover Py3k
-            pass
-
 
 class Test_oid_repr(unittest.TestCase):
 
     def _callFUT(self, oid):
         from BTrees.utils import oid_repr
         return oid_repr(oid)
```

### Comparing `BTrees-4.9.2/src/BTrees/utils.py` & `BTrees-5.0/src/BTrees/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,45 +11,44 @@
 # FOR A PARTICULAR PURPOSE
 #
 ##############################################################################
 # Copied from ZODB/utils.py
 
 from binascii import hexlify
 
-from ._compat import _bytes
 
 def non_negative(int_val):
     if int_val < 0:
         # Coerce to non-negative.
         int_val &= 0x7FFFFFFFFFFFFFFF
     return int_val
 
 
 def positive_id(obj): # pragma: no cover
     """Return id(obj) as a non-negative integer."""
     return non_negative(id(obj))
 
 
 def oid_repr(oid):
-    if isinstance(oid, _bytes) and len(oid) == 8:
+    if isinstance(oid, bytes) and len(oid) == 8:
         # Convert to hex and strip leading zeroes.
         as_hex = hexlify(oid).lstrip(b'0')
         # Ensure two characters per input byte.
         chunks = [b'0x']
         if len(as_hex) & 1:
             chunks.append(b'0')
         elif as_hex == b'':
             as_hex = b'00'
         chunks.append(as_hex)
         return b''.join(chunks)
     else:
         return repr(oid)
 
 
-class Lazy(object):
+class Lazy:
     """
     A simple version of ``Lazy`` from ``zope.cachedescriptors``
     """
 
     __slots__ = ('func',)
 
     def __init__(self, func):
```

### Comparing `BTrees-4.9.2/src/BTrees.egg-info/SOURCES.txt` & `BTrees-5.0/src/BTrees.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 .coveragerc
+.manylinux-install.sh
+.manylinux.sh
 CHANGES.rst
+CONTRIBUTING.md
 COPYRIGHT.txt
 LICENSE.txt
 MANIFEST.in
 README.rst
-bootstrap.py
+appveyor.yml
 buildout.cfg
 doc-requirements.txt
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
-.github/workflows/tests.yml
 docs/Makefile
 docs/api.rst
 docs/changes.rst
 docs/conf.py
 docs/development.rst
 docs/index.rst
 docs/make.bat
@@ -69,27 +71,26 @@
 src/BTrees/objectkeymacros.h
 src/BTrees/objectvaluemacros.h
 src/BTrees/sorters.c
 src/BTrees/utils.py
 src/BTrees.egg-info/PKG-INFO
 src/BTrees.egg-info/SOURCES.txt
 src/BTrees.egg-info/dependency_links.txt
-src/BTrees.egg-info/entry_points.txt
 src/BTrees.egg-info/not-zip-safe
 src/BTrees.egg-info/requires.txt
 src/BTrees.egg-info/top_level.txt
 src/BTrees/tests/__init__.py
 src/BTrees/tests/_test_builder.py
 src/BTrees/tests/common.py
 src/BTrees/tests/testBTrees.py
-src/BTrees/tests/testBTreesUnicode.py
 src/BTrees/tests/testConflict.py
 src/BTrees/tests/testPersistency.py
 src/BTrees/tests/test_Length.py
 src/BTrees/tests/test_OOBTree.py
 src/BTrees/tests/test__base.py
 src/BTrees/tests/test__datatypes.py
 src/BTrees/tests/test_btreesubclass.py
 src/BTrees/tests/test_check.py
+src/BTrees/tests/test_compile_flags.py
 src/BTrees/tests/test_dynamic_btrees.py
 src/BTrees/tests/test_fsBTree.py
 src/BTrees/tests/test_utils.py
```

### Comparing `BTrees-4.9.2/tox.ini` & `BTrees-5.0/tox.ini`

 * *Files 23% similar despite different names*

```diff
@@ -1,59 +1,74 @@
+# Generated from:
+# https://github.com/zopefoundation/meta/tree/master/config/c-code
 [tox]
+minversion = 3.18
 envlist =
-# Jython support pending 2.7 support, due 2012-07-15 or so.  See:
-# http://fwierzbicki.blogspot.com/2012/03/adconion-to-fund-jython-27.html
-#   py27,jython,pypy,coverage,docs
-    py27,py27-pure,py35,py35-pure,py36,py37,py38,py39,pypy,pypy3,w_zodb,w_zodb-pure,coverage,docs
+    lint
+    py37,py37-pure
+    py38,py38-pure
+    py39,py39-pure
+    py310,py310-pure
+    py311,py311-pure
+    pypy3
+    docs
+    coverage
+    w_zodb
+    w_zodb-pure
 
 [testenv]
 usedevelop = true
-extras =
-    test
-commands =
-    python -m zope.testrunner --test-path=src --auto-color --auto-progress {posargs}
+deps =
 setenv =
+    pure: PURE_PYTHON=1
+    !pure-!pypy3: PURE_PYTHON=0
     PYTHONFAULTHANDLER=1
     PYTHONDEVMODE=1
     ZOPE_INTERFACE_STRICT_IRO=1
     ZOPE_INTERFACE_LOG_CHANGED_IRO=1
-    PURE_PYTHON=0
-    pure: PURE_PYTHON=1
-    pypy: PURE_PYTHON=1
-    pypy3: PURE_PYTHON=1
-
-#[testenv:jython]
-#commands =
-#   jython setup.py test -q
+commands =
+    zope-testrunner --test-path=src {posargs:-vc}
+    sphinx-build -b doctest -d {envdir}/.cache/doctrees docs {envdir}/.cache/doctest
+extras =
+    test
+    docs
 
 [testenv:w_zodb]
-basepython =
-    python2.7
-deps =
-    ZODB
+basepython = python3.11
+deps = ZODB
 
 [testenv:w_zodb-pure]
-basepython =
-    python2.7
-deps =
-    ZODB
+basepython = python3.11
+deps = ZODB
 
 [testenv:coverage]
-basepython =
-    python3
-commands =
-    coverage run -m zope.testrunner --test-path=src --auto-color --auto-progress {posargs}
-    coverage report --fail-under=92
+basepython = python3
+allowlist_externals =
+    mkdir
 deps =
     coverage
-    ZODB
+setenv =
+    PURE_PYTHON=1
+commands =
+    mkdir -p {toxinidir}/parts/htmlcov
+    coverage run -m zope.testrunner --test-path=src {posargs:-vc}
+    coverage html -i
+    coverage report -i -m --fail-under=93
+
+[testenv:lint]
+basepython = python3
+skip_install = true
+commands =
+    check-manifest
+    check-python-versions
+deps =
+    check-manifest
+    check-python-versions >= 0.19.1
+    wheel
 
 [testenv:docs]
-basepython =
-    python3
+basepython = python3
+skip_install = false
+commands_pre =
 commands =
     sphinx-build -b html -d docs/_build/doctrees docs docs/_build/html
     sphinx-build -b doctest -d docs/_build/doctrees docs docs/_build/doctest
-deps =
-    --requirement doc-requirements.txt
-extras =
-    docs
```

