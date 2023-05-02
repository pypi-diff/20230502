# Comparing `tmp/DeTrusty-0.9.0.tar.gz` & `tmp/DeTrusty-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeTrusty-0.9.0.tar", last modified: Thu Nov 24 13:27:59 2022, max compression
+gzip compressed data, was "DeTrusty-0.9.1.tar", last modified: Tue Dec  6 16:49:06 2022, max compression
```

## Comparing `DeTrusty-0.9.0.tar` & `DeTrusty-0.9.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-24 13:27:59.030717 DeTrusty-0.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-24 13:27:59.018716 DeTrusty-0.9.0/DeTrusty/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-24 13:27:59.022716 DeTrusty-0.9.0/DeTrusty/Decomposer/
--rw-r--r--   0 runner    (1001) docker     (123)    34051 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Decomposer/Decomposer.py
--rw-r--r--   0 runner    (1001) docker     (123)    42962 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Decomposer/Planner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12781 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Decomposer/Tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Decomposer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Decomposer/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-24 13:27:59.022716 DeTrusty-0.9.0/DeTrusty/Molecule/
--rw-r--r--   0 runner    (1001) docker     (123)    16000 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Molecule/MTCreation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8431 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Molecule/MTManager.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Molecule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-24 13:27:59.022716 DeTrusty-0.9.0/DeTrusty/Operators/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-24 13:27:59.026717 DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/OperatorStructures.py
--rw-r--r--   0 runner    (1001) docker     (123)    23044 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/Xaggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)    15974 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/Xbind.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/Xdistinct.py
--rw-r--r--   0 runner    (1001) docker     (123)     5799 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/Xexpression.py
--rw-r--r--   0 runner    (1001) docker     (123)    13497 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/Xfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16049 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/Xgjoin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7006 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/Xgoptional.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/Xgroupby.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/Xhaving.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/Xlimit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5252 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/Xnjoin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5672 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/Xnoptional.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/Xoffset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/Xorderby.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/Xproject.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/Xunion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/Xvalues.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-24 13:27:59.026717 DeTrusty-0.9.0/DeTrusty/Operators/BlockingOperators/
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/BlockingOperators/HashJoin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5031 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/BlockingOperators/HashOptional.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/BlockingOperators/NestedLoopJoin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/BlockingOperators/NestedLoopOptional.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/BlockingOperators/OperatorStructures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/BlockingOperators/Union.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/BlockingOperators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/Join.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-24 13:27:59.026717 DeTrusty-0.9.0/DeTrusty/Operators/NonBlockingOperators/
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/NonBlockingOperators/NestedHashJoin.py
--rw-r--r--   0 runner    (1001) docker     (123)    19378 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/NonBlockingOperators/NestedHashJoinFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/NonBlockingOperators/NestedHashOptional.py
--rw-r--r--   0 runner    (1001) docker     (123)     8796 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/NonBlockingOperators/NestedHashOptionalFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/NonBlockingOperators/OperatorStructures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4285 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/NonBlockingOperators/SymmetricHashJoin.py
--rw-r--r--   0 runner    (1001) docker     (123)    15216 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/NonBlockingOperators/Xjoin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/NonBlockingOperators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/Optional.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/Union.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Operators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-24 13:27:59.026717 DeTrusty-0.9.0/DeTrusty/Sparql/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-24 13:27:59.030717 DeTrusty-0.9.0/DeTrusty/Sparql/Parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Sparql/Parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34425 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Sparql/Parser/queryParser.py
--rw-r--r--   0 runner    (1001) docker     (123)    18174 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Sparql/Parser/queryParser1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)    41705 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Sparql/Parser/services.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Sparql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-24 13:27:59.030717 DeTrusty-0.9.0/DeTrusty/Wrapper/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-24 13:27:59.030717 DeTrusty-0.9.0/DeTrusty/Wrapper/RDFWrapper/
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Wrapper/RDFWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/Wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/DeTrusty/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-24 13:27:59.022716 DeTrusty-0.9.0/DeTrusty.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15695 2022-11-24 13:27:59.000000 DeTrusty-0.9.0/DeTrusty.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2022-11-24 13:27:59.000000 DeTrusty-0.9.0/DeTrusty.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-24 13:27:59.000000 DeTrusty-0.9.0/DeTrusty.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2022-11-24 13:27:59.000000 DeTrusty-0.9.0/DeTrusty.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2022-11-24 13:27:59.000000 DeTrusty-0.9.0/DeTrusty.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35150 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15695 2022-11-24 13:27:59.030717 DeTrusty-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14723 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-24 13:27:59.018716 DeTrusty-0.9.0/Scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1779 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/Scripts/create_rdfmts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       69 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/Scripts/restart_workers.sh
--rw-r--r--   0 runner    (1001) docker     (123)        5 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-11-24 13:27:59.030717 DeTrusty-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2022-11-24 13:27:44.000000 DeTrusty-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:49:06.750659 DeTrusty-0.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:49:06.738659 DeTrusty-0.9.1/DeTrusty/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:49:06.742659 DeTrusty-0.9.1/DeTrusty/Decomposer/
+-rw-r--r--   0 runner    (1001) docker     (123)    34080 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Decomposer/Decomposer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42962 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Decomposer/Planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12781 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Decomposer/Tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Decomposer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Decomposer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:49:06.742659 DeTrusty-0.9.1/DeTrusty/Molecule/
+-rw-r--r--   0 runner    (1001) docker     (123)    16000 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Molecule/MTCreation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8431 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Molecule/MTManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Molecule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:49:06.742659 DeTrusty-0.9.1/DeTrusty/Operators/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:49:06.746659 DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/OperatorStructures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23044 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/Xaggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15974 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/Xbind.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/Xdistinct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/Xexpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13497 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/Xfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16049 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/Xgjoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7006 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/Xgoptional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/Xgroupby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/Xhaving.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/Xlimit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/Xnjoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5672 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/Xnoptional.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/Xoffset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/Xorderby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/Xproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/Xunion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/Xvalues.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:49:06.746659 DeTrusty-0.9.1/DeTrusty/Operators/BlockingOperators/
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/BlockingOperators/HashJoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5031 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/BlockingOperators/HashOptional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/BlockingOperators/NestedLoopJoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/BlockingOperators/NestedLoopOptional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/BlockingOperators/OperatorStructures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/BlockingOperators/Union.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/BlockingOperators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/Join.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:49:06.750659 DeTrusty-0.9.1/DeTrusty/Operators/NonBlockingOperators/
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/NonBlockingOperators/NestedHashJoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19378 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/NonBlockingOperators/NestedHashJoinFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/NonBlockingOperators/NestedHashOptional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8796 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/NonBlockingOperators/NestedHashOptionalFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/NonBlockingOperators/OperatorStructures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4285 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/NonBlockingOperators/SymmetricHashJoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15216 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/NonBlockingOperators/Xjoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/NonBlockingOperators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/Optional.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/Union.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Operators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:49:06.750659 DeTrusty-0.9.1/DeTrusty/Sparql/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:49:06.750659 DeTrusty-0.9.1/DeTrusty/Sparql/Parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Sparql/Parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34760 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Sparql/Parser/queryParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18174 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Sparql/Parser/queryParser1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41662 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Sparql/Parser/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Sparql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:49:06.750659 DeTrusty-0.9.1/DeTrusty/Wrapper/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:49:06.750659 DeTrusty-0.9.1/DeTrusty/Wrapper/RDFWrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Wrapper/RDFWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/Wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/DeTrusty/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:49:06.738659 DeTrusty-0.9.1/DeTrusty.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15746 2022-12-06 16:49:06.000000 DeTrusty-0.9.1/DeTrusty.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2022-12-06 16:49:06.000000 DeTrusty-0.9.1/DeTrusty.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 16:49:06.000000 DeTrusty-0.9.1/DeTrusty.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2022-12-06 16:49:06.000000 DeTrusty-0.9.1/DeTrusty.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-06 16:49:06.000000 DeTrusty-0.9.1/DeTrusty.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35150 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15746 2022-12-06 16:49:06.750659 DeTrusty-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14723 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:49:06.738659 DeTrusty-0.9.1/Scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1933 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/Scripts/create_rdfmts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       69 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/Scripts/restart_workers.sh
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-06 16:49:06.750659 DeTrusty-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2022-12-06 16:48:54.000000 DeTrusty-0.9.1/setup.py
```

### Comparing `DeTrusty-0.9.0/DeTrusty/Decomposer/Decomposer.py` & `DeTrusty-0.9.1/DeTrusty/Decomposer/Decomposer.py`

 * *Files 1% similar despite different names*

```diff
@@ -697,14 +697,15 @@
                         fl2 = self.includeFilterAuxSK(f, jb.triples, jb, True)
                     fl1 = fl1 + fl2
         return fl1
 
     def includeFilterAux(self, f, sl):
         fl1 = []
         for s in sl:
+            # print(type(s))
             vars_s = set()
             for t in s.triples:
                 vars_s.update(set(utils.getVars(t)))
             vars_f = f.getVars()
             if set(vars_s) & set(vars_f) == set(vars_f):
                 s.include_filter(f)
                 fl1 = fl1 + [f]
```

### Comparing `DeTrusty-0.9.0/DeTrusty/Decomposer/Planner.py` & `DeTrusty-0.9.1/DeTrusty/Decomposer/Planner.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Decomposer/Tree.py` & `DeTrusty-0.9.1/DeTrusty/Decomposer/Tree.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Decomposer/utils.py` & `DeTrusty-0.9.1/DeTrusty/Decomposer/utils.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Logger.py` & `DeTrusty-0.9.1/DeTrusty/Logger.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Molecule/MTCreation.py` & `DeTrusty-0.9.1/DeTrusty/Molecule/MTCreation.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Molecule/MTManager.py` & `DeTrusty-0.9.1/DeTrusty/Molecule/MTManager.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/OperatorStructures.py` & `DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/OperatorStructures.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/Xaggregate.py` & `DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/Xaggregate.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/Xbind.py` & `DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/Xbind.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/Xdistinct.py` & `DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/Xdistinct.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/Xexpression.py` & `DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/Xexpression.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/Xfilter.py` & `DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/Xfilter.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/Xgjoin.py` & `DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/Xgjoin.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/Xgoptional.py` & `DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/Xgoptional.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/Xgroupby.py` & `DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/Xgroupby.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,15 @@
         self.qresults = out
         arg_list = list()
         tmp = list()                                                       # [tup1,tup2,...]
 
         for arg in self.args:
             arg_list.append(arg.name[1:])
 
-        tuple = self.left.get(True)                                     
-        # print(tuple)
+        tuple = self.left.get(True)
 
         while (tuple != "EOF"):
             match = [0] * len(tmp)
             append = True
 
             for i in range(len(tmp)):
                 tmp_dict = tmp[i]
```

### Comparing `DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/Xhaving.py` & `DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/Xhaving.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/Xlimit.py` & `DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/Xlimit.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/Xnjoin.py` & `DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/Xnjoin.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/Xnoptional.py` & `DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/Xnoptional.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/Xoffset.py` & `DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/Xoffset.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/Xorderby.py` & `DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/Xorderby.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/Xproject.py` & `DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/Xproject.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/Xunion.py` & `DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/Xunion.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Operators/AnapsidOperators/Xvalues.py` & `DeTrusty-0.9.1/DeTrusty/Operators/AnapsidOperators/Xvalues.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Operators/BlockingOperators/HashJoin.py` & `DeTrusty-0.9.1/DeTrusty/Operators/BlockingOperators/HashJoin.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Operators/BlockingOperators/HashOptional.py` & `DeTrusty-0.9.1/DeTrusty/Operators/BlockingOperators/HashOptional.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Operators/BlockingOperators/NestedLoopJoin.py` & `DeTrusty-0.9.1/DeTrusty/Operators/BlockingOperators/NestedLoopJoin.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Operators/BlockingOperators/NestedLoopOptional.py` & `DeTrusty-0.9.1/DeTrusty/Operators/BlockingOperators/NestedLoopOptional.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Operators/BlockingOperators/OperatorStructures.py` & `DeTrusty-0.9.1/DeTrusty/Operators/BlockingOperators/OperatorStructures.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Operators/BlockingOperators/Union.py` & `DeTrusty-0.9.1/DeTrusty/Operators/BlockingOperators/Union.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Operators/Join.py` & `DeTrusty-0.9.1/DeTrusty/Operators/Join.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Operators/NonBlockingOperators/NestedHashJoin.py` & `DeTrusty-0.9.1/DeTrusty/Operators/NonBlockingOperators/NestedHashJoin.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Operators/NonBlockingOperators/NestedHashJoinFilter.py` & `DeTrusty-0.9.1/DeTrusty/Operators/NonBlockingOperators/NestedHashJoinFilter.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Operators/NonBlockingOperators/NestedHashOptional.py` & `DeTrusty-0.9.1/DeTrusty/Operators/NonBlockingOperators/NestedHashOptional.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Operators/NonBlockingOperators/NestedHashOptionalFilter.py` & `DeTrusty-0.9.1/DeTrusty/Operators/NonBlockingOperators/NestedHashOptionalFilter.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Operators/NonBlockingOperators/OperatorStructures.py` & `DeTrusty-0.9.1/DeTrusty/Operators/NonBlockingOperators/OperatorStructures.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Operators/NonBlockingOperators/SymmetricHashJoin.py` & `DeTrusty-0.9.1/DeTrusty/Operators/NonBlockingOperators/SymmetricHashJoin.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Operators/NonBlockingOperators/Xjoin.py` & `DeTrusty-0.9.1/DeTrusty/Operators/NonBlockingOperators/Xjoin.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Operators/Optional.py` & `DeTrusty-0.9.1/DeTrusty/Operators/Optional.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Operators/Union.py` & `DeTrusty-0.9.1/DeTrusty/Operators/Union.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Sparql/Parser/queryParser.py` & `DeTrusty-0.9.1/DeTrusty/Sparql/Parser/queryParser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import urllib.parse
 from ply import lex, yacc
+import sys
 # not all module needed (TODO: check after integrating expression to Having, Aggregate)
 from .services import Query, Argument, Triple, UnionBlock, JoinBlock, Optional, Filter, Expression, Values, Bind, Aggregate, Having, HavingHelper, Service
 
+test = list()
 
 # Lexer
 reserved = {
     'PREFIX': 'PREFIX',
     'UNION': 'UNION',
     'FILTER': 'FILTER',
     'OPTIONAL': 'OPTIONAL',
@@ -335,14 +337,18 @@
     p[0] = False
 
 
 def p_single_var_list_0(p): 
     """
     var_list : VARIABLE
     """
+    # if p[1][1:] not in test:
+    #     p_error(p[1])
+        # print('grouping variable should be in aggregate')
+        # sys.exit()
     p[0] = [Argument(p[1], False)]
 
 
 def p_single_var_list_1(p): 
     """
     var_list : LPAR expression AS VARIABLE RPAR
     """
@@ -357,14 +363,18 @@
     # p[0] = [Argument(p[1], False, alias=p[3])]
 
 
 def p_var_list_0(p):
     """
     var_list : VARIABLE var_list 
     """
+    # if p[1][1:] not in test:
+    #     p_error(p[1])
+        # print('grouping variable should be in aggregate')
+        # sys.exit()
     p[0] = [Argument(p[1], False)] + p[2]
 
 
 def p_var_list_1(p):
     """
     var_list : LPAR expression AS VARIABLE RPAR var_list 
     """
@@ -384,14 +394,15 @@
 ################################################################
 
 
 def p_group_by_0(p):
    """
    group_by : GROUP BY group_var group_var_list
    """
+   test.append(p[3].name[1:])
    p[0] = [p[3]] + p[4]
 
 
 def p_group_by_1(p):
    """
    group_by : empty
    """
@@ -1648,15 +1659,15 @@
     if xsd in p[1]:
         p[0] = Argument(c[:c.find("^")], True, datatype=c[c.rfind("^")+1:])
     if "@" in p[1]:
         p[0] = Argument(c[:c.find("^")], True, datatype="<" + xsd + "string>", lang=c[c.rfind("@")+1:])
 
 
 def p_error(p):
-    print(p)
+    # print(type(p))
     if isinstance(p, str):
         value = p
     else:
         value = p.value
     raise TypeError("unknown text at %r" % (value,))
```

### Comparing `DeTrusty-0.9.0/DeTrusty/Sparql/Parser/queryParser1_1.py` & `DeTrusty-0.9.1/DeTrusty/Sparql/Parser/queryParser1_1.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/Sparql/Parser/services.py` & `DeTrusty-0.9.1/DeTrusty/Sparql/Parser/services.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,14 +97,16 @@
         vars_ = []
         if isinstance(self.triples, list):
             for t in self.triples:
                 vars_.extend(t.getVars())
         else:
             vars_.extend(self.triples.getVars())
         for filter_ in self.filters:
+            if isinstance(filter_, Bind):
+                vars_.append(filter_.alias)
             vars_.extend(filter_.getVars())
         return vars_
 
     def getConsts(self):
         if isinstance(self.triples, list):
             c = []
             for t in self.triples:
@@ -835,17 +837,14 @@
     def __repr__(self):
         return "\n" + "BIND (" + str(self.expr) + " AS " + self.alias + ")"
 
     def show(self, x):
         return "\n" + x + "BIND (" + str(self.expr) + " AS " + self.alias + ")"
 
     def getVars(self):
-        if self.alias:
-            # not sure if this correct, check later
-            return [self.alias] + self.expr.getVars()
         return self.expr.getVars()
 
     def getConsts(self):
         c = []
         for row in self.expr:
             for arg in row:
                 const = arg.getConsts()
```

### Comparing `DeTrusty-0.9.0/DeTrusty/Wrapper/RDFWrapper/__init__.py` & `DeTrusty-0.9.1/DeTrusty/Wrapper/RDFWrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty/__init__.py` & `DeTrusty-0.9.1/DeTrusty/__init__.py`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/DeTrusty.egg-info/PKG-INFO` & `DeTrusty-0.9.1/DeTrusty.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: DeTrusty
-Version: 0.9.0
+Version: 0.9.1
 Summary: DeTrusty - Decentralized and Trustable Query Engine
 Home-page: https://github.com/SDM-TIB/DeTrusty
-Download-URL: https://github.com/SDM-TIB/DeTrusty/archive/refs/tags/v0.9.0.tar.gz
+Download-URL: https://github.com/SDM-TIB/DeTrusty/archive/refs/tags/v0.9.1.tar.gz
 Author: Philipp D. Rohde
 Author-email: philipp.rohde@tib.eu
 License: GNU/GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `DeTrusty-0.9.0/DeTrusty.egg-info/SOURCES.txt` & `DeTrusty-0.9.1/DeTrusty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/LICENSE` & `DeTrusty-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/PKG-INFO` & `DeTrusty-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: DeTrusty
-Version: 0.9.0
+Version: 0.9.1
 Summary: DeTrusty - Decentralized and Trustable Query Engine
 Home-page: https://github.com/SDM-TIB/DeTrusty
-Download-URL: https://github.com/SDM-TIB/DeTrusty/archive/refs/tags/v0.9.0.tar.gz
+Download-URL: https://github.com/SDM-TIB/DeTrusty/archive/refs/tags/v0.9.1.tar.gz
 Author: Philipp D. Rohde
 Author-email: philipp.rohde@tib.eu
 License: GNU/GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `DeTrusty-0.9.0/README.md` & `DeTrusty-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `DeTrusty-0.9.0/Scripts/create_rdfmts.py` & `DeTrusty-0.9.1/Scripts/create_rdfmts.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 #!/usr/bin/env python3
 
 import getopt
 import json
+import pathlib
 import sys
 
+PACKAGE_DETRUSTY = str(pathlib.Path(__file__).parent.parent.resolve())
+sys.path.append(PACKAGE_DETRUSTY)
 from DeTrusty.Molecule.MTCreation import DEFAULT_OUTPUT_PATH, create_rdfmts, logger
+sys.path.remove(PACKAGE_DETRUSTY)
 
 
 def get_options(argv):
     try:
         opts, args = getopt.getopt(argv, 'h:s:o:j')
     except getopt.GetoptError:
         usage()
```

### Comparing `DeTrusty-0.9.0/setup.py` & `DeTrusty-0.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,12 +43,13 @@
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: OS Independent',
         'Intended Audience :: Science/Research'
     ]
 )
```

