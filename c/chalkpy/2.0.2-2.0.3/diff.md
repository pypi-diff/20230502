# Comparing `tmp/chalkpy-2.0.2.tar.gz` & `tmp/chalkpy-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chalkpy-2.0.2.tar", last modified: Mon May  1 23:18:42 2023, max compression
+gzip compressed data, was "chalkpy-2.0.3.tar", last modified: Tue May  2 01:30:32 2023, max compression
```

## Comparing `chalkpy-2.0.2.tar` & `chalkpy-2.0.3.tar`

### file list

```diff
@@ -1,925 +1,926 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.087720 chalkpy-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-01 23:18:25.000000 chalkpy-2.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-05-01 23:18:42.087720 chalkpy-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-05-01 23:18:25.000000 chalkpy-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.019724 chalkpy-2.0.2/chalk/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.019724 chalkpy-2.0.2/chalk/_autosql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/_autosql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/_autosql/autosql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.019724 chalkpy-2.0.2/chalk/_monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)    16799 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/_monitoring/Chart.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/_monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64519 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/_monitoring/charts_codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/_monitoring/charts_enums_codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)    13537 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/_monitoring/charts_series_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/_monitoring/gql_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.019724 chalkpy-2.0.2/chalk/_reporting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/_reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/_reporting/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/_reporting/progress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.019724 chalkpy-2.0.2/chalk/_validation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/_validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/_validation/feature_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/_validation/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.019724 chalkpy-2.0.2/chalk/client/
--rw-r--r--   0 runner    (1001) docker     (123)    38477 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42271 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/client/client_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)    31681 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/client/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/client/exc.py
--rw-r--r--   0 runner    (1001) docker     (123)    24515 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/client/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.019724 chalkpy-2.0.2/chalk/clogging/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/clogging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/clogging/chalk_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.019724 chalkpy-2.0.2/chalk/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/config/auth_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/config/project_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.019724 chalkpy-2.0.2/chalk/df/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/df/ChalkDataFrameImpl.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/df/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/df/ast_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.023724 chalkpy-2.0.2/chalk/feature_n/
--rw-r--r--   0 runner    (1001) docker     (123)    14204 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/codegen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.023724 chalkpy-2.0.2/chalk/feature_n/feature_1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_1/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.023724 chalkpy-2.0.2/chalk/feature_n/feature_10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_10/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.023724 chalkpy-2.0.2/chalk/feature_n/feature_100/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_100/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_100/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.023724 chalkpy-2.0.2/chalk/feature_n/feature_101/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_101/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_101/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.023724 chalkpy-2.0.2/chalk/feature_n/feature_102/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_102/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_102/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.023724 chalkpy-2.0.2/chalk/feature_n/feature_103/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_103/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_103/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.023724 chalkpy-2.0.2/chalk/feature_n/feature_104/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_104/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_104/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.023724 chalkpy-2.0.2/chalk/feature_n/feature_105/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_105/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_105/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.023724 chalkpy-2.0.2/chalk/feature_n/feature_106/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_106/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_106/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.023724 chalkpy-2.0.2/chalk/feature_n/feature_107/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_107/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_107/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.023724 chalkpy-2.0.2/chalk/feature_n/feature_108/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_108/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_108/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.023724 chalkpy-2.0.2/chalk/feature_n/feature_109/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_109/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_109/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.023724 chalkpy-2.0.2/chalk/feature_n/feature_11/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_11/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.023724 chalkpy-2.0.2/chalk/feature_n/feature_110/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_110/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_110/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.023724 chalkpy-2.0.2/chalk/feature_n/feature_111/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_111/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_111/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.023724 chalkpy-2.0.2/chalk/feature_n/feature_112/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_112/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_112/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.023724 chalkpy-2.0.2/chalk/feature_n/feature_113/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_113/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_113/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.023724 chalkpy-2.0.2/chalk/feature_n/feature_114/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_114/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_114/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.027724 chalkpy-2.0.2/chalk/feature_n/feature_115/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_115/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_115/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.027724 chalkpy-2.0.2/chalk/feature_n/feature_116/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_116/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_116/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.027724 chalkpy-2.0.2/chalk/feature_n/feature_117/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_117/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_117/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.027724 chalkpy-2.0.2/chalk/feature_n/feature_118/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_118/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_118/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.027724 chalkpy-2.0.2/chalk/feature_n/feature_119/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_119/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_119/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.027724 chalkpy-2.0.2/chalk/feature_n/feature_12/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_12/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_12/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.027724 chalkpy-2.0.2/chalk/feature_n/feature_120/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_120/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_120/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.027724 chalkpy-2.0.2/chalk/feature_n/feature_121/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_121/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_121/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.027724 chalkpy-2.0.2/chalk/feature_n/feature_122/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_122/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_122/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.027724 chalkpy-2.0.2/chalk/feature_n/feature_123/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_123/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_123/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.027724 chalkpy-2.0.2/chalk/feature_n/feature_124/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_124/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_124/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.027724 chalkpy-2.0.2/chalk/feature_n/feature_125/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_125/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_125/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.027724 chalkpy-2.0.2/chalk/feature_n/feature_126/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_126/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_126/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.027724 chalkpy-2.0.2/chalk/feature_n/feature_127/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_127/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_127/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.027724 chalkpy-2.0.2/chalk/feature_n/feature_128/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_128/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_128/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.027724 chalkpy-2.0.2/chalk/feature_n/feature_129/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_129/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_129/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.027724 chalkpy-2.0.2/chalk/feature_n/feature_13/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_13/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_13/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.027724 chalkpy-2.0.2/chalk/feature_n/feature_130/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_130/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_130/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.027724 chalkpy-2.0.2/chalk/feature_n/feature_131/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_131/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_131/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.031723 chalkpy-2.0.2/chalk/feature_n/feature_132/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_132/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_132/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.031723 chalkpy-2.0.2/chalk/feature_n/feature_133/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_133/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_133/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.031723 chalkpy-2.0.2/chalk/feature_n/feature_134/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_134/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_134/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.031723 chalkpy-2.0.2/chalk/feature_n/feature_135/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_135/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_135/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.031723 chalkpy-2.0.2/chalk/feature_n/feature_136/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_136/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_136/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.031723 chalkpy-2.0.2/chalk/feature_n/feature_137/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_137/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_137/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.031723 chalkpy-2.0.2/chalk/feature_n/feature_138/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_138/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_138/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.031723 chalkpy-2.0.2/chalk/feature_n/feature_139/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_139/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_139/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.031723 chalkpy-2.0.2/chalk/feature_n/feature_14/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_14/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_14/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.031723 chalkpy-2.0.2/chalk/feature_n/feature_140/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_140/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_140/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.031723 chalkpy-2.0.2/chalk/feature_n/feature_141/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_141/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_141/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.031723 chalkpy-2.0.2/chalk/feature_n/feature_142/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_142/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_142/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.031723 chalkpy-2.0.2/chalk/feature_n/feature_143/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_143/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_143/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.031723 chalkpy-2.0.2/chalk/feature_n/feature_144/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_144/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_144/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.031723 chalkpy-2.0.2/chalk/feature_n/feature_145/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_145/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_145/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.031723 chalkpy-2.0.2/chalk/feature_n/feature_146/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_146/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_146/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.031723 chalkpy-2.0.2/chalk/feature_n/feature_147/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_147/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_147/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.031723 chalkpy-2.0.2/chalk/feature_n/feature_148/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_148/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_148/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.031723 chalkpy-2.0.2/chalk/feature_n/feature_149/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_149/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_149/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.035723 chalkpy-2.0.2/chalk/feature_n/feature_15/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_15/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_15/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.035723 chalkpy-2.0.2/chalk/feature_n/feature_150/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_150/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_150/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.035723 chalkpy-2.0.2/chalk/feature_n/feature_151/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_151/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_151/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.035723 chalkpy-2.0.2/chalk/feature_n/feature_152/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_152/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_152/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.035723 chalkpy-2.0.2/chalk/feature_n/feature_153/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_153/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_153/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.035723 chalkpy-2.0.2/chalk/feature_n/feature_154/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_154/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_154/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.035723 chalkpy-2.0.2/chalk/feature_n/feature_155/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_155/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_155/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.035723 chalkpy-2.0.2/chalk/feature_n/feature_156/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_156/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_156/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.035723 chalkpy-2.0.2/chalk/feature_n/feature_157/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_157/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_157/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.035723 chalkpy-2.0.2/chalk/feature_n/feature_158/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_158/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_158/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.035723 chalkpy-2.0.2/chalk/feature_n/feature_159/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_159/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_159/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.035723 chalkpy-2.0.2/chalk/feature_n/feature_16/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_16/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_16/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.035723 chalkpy-2.0.2/chalk/feature_n/feature_160/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_160/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_160/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.035723 chalkpy-2.0.2/chalk/feature_n/feature_161/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_161/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_161/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.035723 chalkpy-2.0.2/chalk/feature_n/feature_162/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_162/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_162/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.035723 chalkpy-2.0.2/chalk/feature_n/feature_163/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_163/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_163/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.035723 chalkpy-2.0.2/chalk/feature_n/feature_164/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_164/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_164/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.035723 chalkpy-2.0.2/chalk/feature_n/feature_165/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_165/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_165/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.035723 chalkpy-2.0.2/chalk/feature_n/feature_166/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_166/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8389 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_166/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.039723 chalkpy-2.0.2/chalk/feature_n/feature_167/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_167/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_167/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.039723 chalkpy-2.0.2/chalk/feature_n/feature_168/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_168/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_168/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.039723 chalkpy-2.0.2/chalk/feature_n/feature_169/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_169/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_169/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.039723 chalkpy-2.0.2/chalk/feature_n/feature_17/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_17/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_17/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.039723 chalkpy-2.0.2/chalk/feature_n/feature_170/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_170/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_170/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.039723 chalkpy-2.0.2/chalk/feature_n/feature_171/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_171/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_171/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.039723 chalkpy-2.0.2/chalk/feature_n/feature_172/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_172/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_172/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.039723 chalkpy-2.0.2/chalk/feature_n/feature_173/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_173/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_173/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.039723 chalkpy-2.0.2/chalk/feature_n/feature_174/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_174/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_174/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.039723 chalkpy-2.0.2/chalk/feature_n/feature_175/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_175/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8848 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_175/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.039723 chalkpy-2.0.2/chalk/feature_n/feature_176/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_176/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_176/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.039723 chalkpy-2.0.2/chalk/feature_n/feature_177/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_177/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_177/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.039723 chalkpy-2.0.2/chalk/feature_n/feature_178/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_178/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_178/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.039723 chalkpy-2.0.2/chalk/feature_n/feature_179/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_179/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_179/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.039723 chalkpy-2.0.2/chalk/feature_n/feature_18/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_18/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_18/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.039723 chalkpy-2.0.2/chalk/feature_n/feature_180/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_180/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_180/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.039723 chalkpy-2.0.2/chalk/feature_n/feature_181/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_181/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_181/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.039723 chalkpy-2.0.2/chalk/feature_n/feature_182/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_182/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_182/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.043722 chalkpy-2.0.2/chalk/feature_n/feature_183/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_183/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_183/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.043722 chalkpy-2.0.2/chalk/feature_n/feature_184/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_184/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_184/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.043722 chalkpy-2.0.2/chalk/feature_n/feature_185/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_185/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_185/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.043722 chalkpy-2.0.2/chalk/feature_n/feature_186/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_186/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_186/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.043722 chalkpy-2.0.2/chalk/feature_n/feature_187/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_187/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_187/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.043722 chalkpy-2.0.2/chalk/feature_n/feature_188/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_188/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_188/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.043722 chalkpy-2.0.2/chalk/feature_n/feature_189/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_189/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9562 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_189/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.043722 chalkpy-2.0.2/chalk/feature_n/feature_19/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_19/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_19/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.043722 chalkpy-2.0.2/chalk/feature_n/feature_190/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_190/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_190/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.043722 chalkpy-2.0.2/chalk/feature_n/feature_191/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_191/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_191/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.043722 chalkpy-2.0.2/chalk/feature_n/feature_192/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_192/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_192/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.043722 chalkpy-2.0.2/chalk/feature_n/feature_193/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_193/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_193/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.043722 chalkpy-2.0.2/chalk/feature_n/feature_194/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_194/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9817 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_194/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.043722 chalkpy-2.0.2/chalk/feature_n/feature_195/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_195/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_195/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.043722 chalkpy-2.0.2/chalk/feature_n/feature_196/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_196/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9919 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_196/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.043722 chalkpy-2.0.2/chalk/feature_n/feature_197/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_197/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9970 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_197/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.043722 chalkpy-2.0.2/chalk/feature_n/feature_198/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_198/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_198/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.047722 chalkpy-2.0.2/chalk/feature_n/feature_199/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_199/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10072 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_199/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.047722 chalkpy-2.0.2/chalk/feature_n/feature_2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_2/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.047722 chalkpy-2.0.2/chalk/feature_n/feature_20/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_20/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_20/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.047722 chalkpy-2.0.2/chalk/feature_n/feature_200/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_200/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10123 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_200/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.047722 chalkpy-2.0.2/chalk/feature_n/feature_201/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_201/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_201/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.047722 chalkpy-2.0.2/chalk/feature_n/feature_202/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_202/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_202/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.047722 chalkpy-2.0.2/chalk/feature_n/feature_203/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_203/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_203/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.047722 chalkpy-2.0.2/chalk/feature_n/feature_204/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_204/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_204/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.047722 chalkpy-2.0.2/chalk/feature_n/feature_205/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_205/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_205/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.047722 chalkpy-2.0.2/chalk/feature_n/feature_206/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_206/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_206/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.047722 chalkpy-2.0.2/chalk/feature_n/feature_207/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_207/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_207/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.047722 chalkpy-2.0.2/chalk/feature_n/feature_208/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_208/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10531 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_208/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.047722 chalkpy-2.0.2/chalk/feature_n/feature_209/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_209/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_209/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.047722 chalkpy-2.0.2/chalk/feature_n/feature_21/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_21/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_21/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.047722 chalkpy-2.0.2/chalk/feature_n/feature_210/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_210/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_210/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.047722 chalkpy-2.0.2/chalk/feature_n/feature_211/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_211/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_211/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.047722 chalkpy-2.0.2/chalk/feature_n/feature_212/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_212/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_212/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.047722 chalkpy-2.0.2/chalk/feature_n/feature_213/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_213/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_213/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.051722 chalkpy-2.0.2/chalk/feature_n/feature_214/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_214/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_214/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.051722 chalkpy-2.0.2/chalk/feature_n/feature_215/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_215/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_215/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.051722 chalkpy-2.0.2/chalk/feature_n/feature_216/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_216/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_216/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.051722 chalkpy-2.0.2/chalk/feature_n/feature_217/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_217/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10990 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_217/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.051722 chalkpy-2.0.2/chalk/feature_n/feature_218/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_218/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_218/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.051722 chalkpy-2.0.2/chalk/feature_n/feature_219/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_219/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_219/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.051722 chalkpy-2.0.2/chalk/feature_n/feature_22/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_22/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_22/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.051722 chalkpy-2.0.2/chalk/feature_n/feature_220/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_220/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_220/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.051722 chalkpy-2.0.2/chalk/feature_n/feature_221/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_221/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_221/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.051722 chalkpy-2.0.2/chalk/feature_n/feature_222/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_222/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11245 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_222/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.051722 chalkpy-2.0.2/chalk/feature_n/feature_223/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_223/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11296 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_223/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.051722 chalkpy-2.0.2/chalk/feature_n/feature_224/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_224/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_224/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.051722 chalkpy-2.0.2/chalk/feature_n/feature_225/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_225/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_225/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.051722 chalkpy-2.0.2/chalk/feature_n/feature_226/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_226/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_226/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.051722 chalkpy-2.0.2/chalk/feature_n/feature_227/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_227/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_227/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.051722 chalkpy-2.0.2/chalk/feature_n/feature_228/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_228/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_228/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.051722 chalkpy-2.0.2/chalk/feature_n/feature_229/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_229/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11602 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_229/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.055722 chalkpy-2.0.2/chalk/feature_n/feature_23/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_23/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_23/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.055722 chalkpy-2.0.2/chalk/feature_n/feature_230/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_230/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11653 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_230/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.055722 chalkpy-2.0.2/chalk/feature_n/feature_231/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_231/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11704 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_231/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.055722 chalkpy-2.0.2/chalk/feature_n/feature_232/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_232/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11755 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_232/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.055722 chalkpy-2.0.2/chalk/feature_n/feature_233/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_233/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_233/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.055722 chalkpy-2.0.2/chalk/feature_n/feature_234/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_234/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_234/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.055722 chalkpy-2.0.2/chalk/feature_n/feature_235/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_235/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11908 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_235/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.055722 chalkpy-2.0.2/chalk/feature_n/feature_236/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_236/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_236/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.055722 chalkpy-2.0.2/chalk/feature_n/feature_237/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_237/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_237/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.055722 chalkpy-2.0.2/chalk/feature_n/feature_238/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_238/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_238/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.055722 chalkpy-2.0.2/chalk/feature_n/feature_239/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_239/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_239/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.055722 chalkpy-2.0.2/chalk/feature_n/feature_24/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_24/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_24/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.055722 chalkpy-2.0.2/chalk/feature_n/feature_240/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_240/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_240/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.055722 chalkpy-2.0.2/chalk/feature_n/feature_241/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_241/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_241/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.055722 chalkpy-2.0.2/chalk/feature_n/feature_242/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_242/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12265 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_242/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.055722 chalkpy-2.0.2/chalk/feature_n/feature_243/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_243/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_243/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.055722 chalkpy-2.0.2/chalk/feature_n/feature_244/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_244/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_244/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.055722 chalkpy-2.0.2/chalk/feature_n/feature_245/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_245/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_245/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.059721 chalkpy-2.0.2/chalk/feature_n/feature_246/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_246/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_246/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.059721 chalkpy-2.0.2/chalk/feature_n/feature_247/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_247/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12520 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_247/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.059721 chalkpy-2.0.2/chalk/feature_n/feature_248/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_248/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12571 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_248/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.059721 chalkpy-2.0.2/chalk/feature_n/feature_249/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_249/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_249/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.059721 chalkpy-2.0.2/chalk/feature_n/feature_25/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_25/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_25/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.059721 chalkpy-2.0.2/chalk/feature_n/feature_250/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_250/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12673 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_250/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.059721 chalkpy-2.0.2/chalk/feature_n/feature_251/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_251/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_251/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.059721 chalkpy-2.0.2/chalk/feature_n/feature_252/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_252/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12775 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_252/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.059721 chalkpy-2.0.2/chalk/feature_n/feature_253/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_253/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_253/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.059721 chalkpy-2.0.2/chalk/feature_n/feature_254/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_254/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12877 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_254/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.059721 chalkpy-2.0.2/chalk/feature_n/feature_255/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_255/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12928 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_255/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.059721 chalkpy-2.0.2/chalk/feature_n/feature_256/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_256/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12979 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_256/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.059721 chalkpy-2.0.2/chalk/feature_n/feature_26/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_26/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_26/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.059721 chalkpy-2.0.2/chalk/feature_n/feature_27/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_27/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_27/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.059721 chalkpy-2.0.2/chalk/feature_n/feature_28/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_28/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_28/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.059721 chalkpy-2.0.2/chalk/feature_n/feature_29/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_29/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_29/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.059721 chalkpy-2.0.2/chalk/feature_n/feature_3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_3/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.059721 chalkpy-2.0.2/chalk/feature_n/feature_30/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_30/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_30/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.063721 chalkpy-2.0.2/chalk/feature_n/feature_31/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_31/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_31/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.063721 chalkpy-2.0.2/chalk/feature_n/feature_32/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_32/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_32/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.063721 chalkpy-2.0.2/chalk/feature_n/feature_33/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_33/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_33/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.063721 chalkpy-2.0.2/chalk/feature_n/feature_34/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_34/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_34/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.063721 chalkpy-2.0.2/chalk/feature_n/feature_35/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_35/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_35/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.063721 chalkpy-2.0.2/chalk/feature_n/feature_36/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_36/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_36/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.063721 chalkpy-2.0.2/chalk/feature_n/feature_37/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_37/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_37/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.063721 chalkpy-2.0.2/chalk/feature_n/feature_38/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_38/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_38/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.063721 chalkpy-2.0.2/chalk/feature_n/feature_39/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_39/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_39/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.063721 chalkpy-2.0.2/chalk/feature_n/feature_4/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_4/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.063721 chalkpy-2.0.2/chalk/feature_n/feature_40/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_40/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_40/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.063721 chalkpy-2.0.2/chalk/feature_n/feature_41/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_41/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_41/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.063721 chalkpy-2.0.2/chalk/feature_n/feature_42/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_42/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_42/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.063721 chalkpy-2.0.2/chalk/feature_n/feature_43/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_43/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_43/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.063721 chalkpy-2.0.2/chalk/feature_n/feature_44/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_44/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_44/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.063721 chalkpy-2.0.2/chalk/feature_n/feature_45/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_45/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_45/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.063721 chalkpy-2.0.2/chalk/feature_n/feature_46/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_46/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_46/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.063721 chalkpy-2.0.2/chalk/feature_n/feature_47/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_47/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_47/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.067721 chalkpy-2.0.2/chalk/feature_n/feature_48/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_48/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_48/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.067721 chalkpy-2.0.2/chalk/feature_n/feature_49/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_49/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_49/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.067721 chalkpy-2.0.2/chalk/feature_n/feature_5/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_5/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.067721 chalkpy-2.0.2/chalk/feature_n/feature_50/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_50/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_50/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.067721 chalkpy-2.0.2/chalk/feature_n/feature_51/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_51/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_51/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.067721 chalkpy-2.0.2/chalk/feature_n/feature_52/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_52/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_52/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.067721 chalkpy-2.0.2/chalk/feature_n/feature_53/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_53/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_53/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.067721 chalkpy-2.0.2/chalk/feature_n/feature_54/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_54/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_54/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.067721 chalkpy-2.0.2/chalk/feature_n/feature_55/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_55/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_55/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.067721 chalkpy-2.0.2/chalk/feature_n/feature_56/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_56/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_56/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.067721 chalkpy-2.0.2/chalk/feature_n/feature_57/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_57/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_57/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.067721 chalkpy-2.0.2/chalk/feature_n/feature_58/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_58/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_58/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.067721 chalkpy-2.0.2/chalk/feature_n/feature_59/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_59/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_59/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.067721 chalkpy-2.0.2/chalk/feature_n/feature_6/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_6/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.067721 chalkpy-2.0.2/chalk/feature_n/feature_60/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_60/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_60/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.067721 chalkpy-2.0.2/chalk/feature_n/feature_61/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_61/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_61/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.067721 chalkpy-2.0.2/chalk/feature_n/feature_62/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_62/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_62/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.067721 chalkpy-2.0.2/chalk/feature_n/feature_63/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_63/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_63/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.071721 chalkpy-2.0.2/chalk/feature_n/feature_64/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_64/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_64/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.071721 chalkpy-2.0.2/chalk/feature_n/feature_65/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_65/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_65/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.071721 chalkpy-2.0.2/chalk/feature_n/feature_66/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_66/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_66/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.071721 chalkpy-2.0.2/chalk/feature_n/feature_67/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_67/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_67/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.071721 chalkpy-2.0.2/chalk/feature_n/feature_68/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_68/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_68/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.071721 chalkpy-2.0.2/chalk/feature_n/feature_69/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_69/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_69/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.071721 chalkpy-2.0.2/chalk/feature_n/feature_7/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_7/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_7/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.071721 chalkpy-2.0.2/chalk/feature_n/feature_70/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_70/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_70/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.071721 chalkpy-2.0.2/chalk/feature_n/feature_71/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_71/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_71/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.071721 chalkpy-2.0.2/chalk/feature_n/feature_72/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_72/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_72/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.071721 chalkpy-2.0.2/chalk/feature_n/feature_73/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_73/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_73/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.071721 chalkpy-2.0.2/chalk/feature_n/feature_74/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_74/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_74/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.071721 chalkpy-2.0.2/chalk/feature_n/feature_75/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_75/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_75/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.071721 chalkpy-2.0.2/chalk/feature_n/feature_76/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_76/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_76/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.071721 chalkpy-2.0.2/chalk/feature_n/feature_77/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_77/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_77/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.071721 chalkpy-2.0.2/chalk/feature_n/feature_78/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_78/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_78/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.071721 chalkpy-2.0.2/chalk/feature_n/feature_79/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_79/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_79/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.071721 chalkpy-2.0.2/chalk/feature_n/feature_8/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_8/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_8/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.075720 chalkpy-2.0.2/chalk/feature_n/feature_80/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_80/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_80/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.075720 chalkpy-2.0.2/chalk/feature_n/feature_81/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_81/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_81/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.075720 chalkpy-2.0.2/chalk/feature_n/feature_82/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_82/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_82/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.075720 chalkpy-2.0.2/chalk/feature_n/feature_83/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_83/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_83/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.075720 chalkpy-2.0.2/chalk/feature_n/feature_84/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_84/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_84/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.075720 chalkpy-2.0.2/chalk/feature_n/feature_85/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_85/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_85/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.075720 chalkpy-2.0.2/chalk/feature_n/feature_86/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_86/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_86/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.075720 chalkpy-2.0.2/chalk/feature_n/feature_87/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_87/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_87/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.075720 chalkpy-2.0.2/chalk/feature_n/feature_88/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_88/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_88/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.075720 chalkpy-2.0.2/chalk/feature_n/feature_89/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_89/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_89/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.075720 chalkpy-2.0.2/chalk/feature_n/feature_9/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_9/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_9/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.075720 chalkpy-2.0.2/chalk/feature_n/feature_90/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_90/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_90/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.075720 chalkpy-2.0.2/chalk/feature_n/feature_91/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_91/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_91/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.075720 chalkpy-2.0.2/chalk/feature_n/feature_92/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_92/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_92/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.075720 chalkpy-2.0.2/chalk/feature_n/feature_93/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_93/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_93/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.075720 chalkpy-2.0.2/chalk/feature_n/feature_94/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_94/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_94/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.075720 chalkpy-2.0.2/chalk/feature_n/feature_95/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_95/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_95/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.075720 chalkpy-2.0.2/chalk/feature_n/feature_96/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_96/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_96/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.079720 chalkpy-2.0.2/chalk/feature_n/feature_97/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_97/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_97/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.079720 chalkpy-2.0.2/chalk/feature_n/feature_98/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_98/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_98/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.079720 chalkpy-2.0.2/chalk/feature_n/feature_99/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_99/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/feature_n/feature_99/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.079720 chalkpy-2.0.2/chalk/features/
--rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16549 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/features/_chalkop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/features/_class_property.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/features/_document.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.079720 chalkpy-2.0.2/chalk/features/_encoding/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/features/_encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13750 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/features/_encoding/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/features/_encoding/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/features/_encoding/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/features/_encoding/missing_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/features/_encoding/primitive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/features/_encoding/pyarrow.py
--rw-r--r--   0 runner    (1001) docker     (123)    11211 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/features/_encoding/rich.py
--rw-r--r--   0 runner    (1001) docker     (123)     8835 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/features/_encoding/serialized_dtype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.083720 chalkpy-2.0.2/chalk/features/dataframe/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/features/dataframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/features/dataframe/_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    51213 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/features/dataframe/_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/features/dataframe/_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    30875 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/features/feature_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/features/feature_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    29431 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/features/feature_set_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/features/feature_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/features/feature_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/features/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/features/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/features/live_updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/features/primary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/features/pseudofeatures.py
--rw-r--r--   0 runner    (1001) docker     (123)    62960 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/features/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/features/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.083720 chalkpy-2.0.2/chalk/gitignore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/gitignore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/gitignore/gitignore_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/gitignore/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.083720 chalkpy-2.0.2/chalk/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/integrations/named.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.083720 chalkpy-2.0.2/chalk/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.083720 chalkpy-2.0.2/chalk/monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/mypy_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.083720 chalkpy-2.0.2/chalk/parsed/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/parsed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20749 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/parsed/_graph_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10943 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/parsed/duplicate_input_gql.py
--rw-r--r--   0 runner    (1001) docker     (123)    13763 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/parsed/json_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/parsed/user_types_to_json.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.083720 chalkpy-2.0.2/chalk/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12079 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/serialization/parsed_annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.083720 chalkpy-2.0.2/chalk/sink/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/sink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/sink/_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.083720 chalkpy-2.0.2/chalk/sql/
--rw-r--r--   0 runner    (1001) docker     (123)    25011 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.083720 chalkpy-2.0.2/chalk/sql/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/sql/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/sql/_internal/chalk_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/sql/_internal/incremental.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.083720 chalkpy-2.0.2/chalk/sql/_internal/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/sql/_internal/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/sql/_internal/integrations/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/sql/_internal/integrations/cloudsql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/sql/_internal/integrations/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/sql/_internal/integrations/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/sql/_internal/integrations/redshift.py
--rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/sql/_internal/integrations/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/sql/_internal/integrations/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)    24525 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/sql/_internal/sql_file_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    17471 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/sql/_internal/sql_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/sql/_internal/string_chalk_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    13609 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/sql/finalized_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    19504 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/sql/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.087720 chalkpy-2.0.2/chalk/streams/
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/streams/_file_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/streams/_kafka_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    11994 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/streams/_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/streams/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/streams/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.087720 chalkpy-2.0.2/chalk/testing/
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.087720 chalkpy-2.0.2/chalk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/utils/annotation_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/utils/cached_type_hints.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/utils/collection_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/utils/duration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/utils/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/utils/environment_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/utils/log_with_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/utils/metaprogramming.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/utils/missing_dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/utils/notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/utils/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/utils/string.py
--rw-r--r--   0 runner    (1001) docker     (123)    19446 2023-05-01 23:18:25.000000 chalkpy-2.0.2/chalk/utils/stubgen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:18:42.087720 chalkpy-2.0.2/chalkpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23748 2023-05-01 23:18:41.000000 chalkpy-2.0.2/chalkpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-05-01 23:18:25.000000 chalkpy-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 23:18:42.087720 chalkpy-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-01 23:18:25.000000 chalkpy-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.573920 chalkpy-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-02 01:30:13.000000 chalkpy-2.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-05-02 01:30:32.573920 chalkpy-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-05-02 01:30:13.000000 chalkpy-2.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.485919 chalkpy-2.0.3/chalk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.485919 chalkpy-2.0.3/chalk/_autosql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/_autosql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/_autosql/autosql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.485919 chalkpy-2.0.3/chalk/_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)    16799 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/_monitoring/Chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/_monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64519 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/_monitoring/charts_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/_monitoring/charts_enums_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13537 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/_monitoring/charts_series_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/_monitoring/gql_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.485919 chalkpy-2.0.3/chalk/_reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/_reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/_reporting/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/_reporting/progress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.489919 chalkpy-2.0.3/chalk/_validation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/_validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/_validation/feature_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/_validation/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.489919 chalkpy-2.0.3/chalk/client/
+-rw-r--r--   0 runner    (1001) docker     (123)    39241 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42359 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/client/client_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31914 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/client/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/client/exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24515 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/client/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.489919 chalkpy-2.0.3/chalk/clogging/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/clogging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/clogging/chalk_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.489919 chalkpy-2.0.3/chalk/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/config/auth_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/config/project_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.489919 chalkpy-2.0.3/chalk/df/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/df/ChalkDataFrameImpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/df/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/df/ast_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.489919 chalkpy-2.0.3/chalk/feature_n/
+-rw-r--r--   0 runner    (1001) docker     (123)    14204 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/codegen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.489919 chalkpy-2.0.3/chalk/feature_n/feature_1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_1/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.489919 chalkpy-2.0.3/chalk/feature_n/feature_10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_10/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.489919 chalkpy-2.0.3/chalk/feature_n/feature_100/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_100/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_100/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.489919 chalkpy-2.0.3/chalk/feature_n/feature_101/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_101/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_101/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.489919 chalkpy-2.0.3/chalk/feature_n/feature_102/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_102/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_102/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.493919 chalkpy-2.0.3/chalk/feature_n/feature_103/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_103/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_103/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.493919 chalkpy-2.0.3/chalk/feature_n/feature_104/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_104/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_104/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.493919 chalkpy-2.0.3/chalk/feature_n/feature_105/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_105/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_105/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.493919 chalkpy-2.0.3/chalk/feature_n/feature_106/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_106/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_106/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.493919 chalkpy-2.0.3/chalk/feature_n/feature_107/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_107/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_107/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.493919 chalkpy-2.0.3/chalk/feature_n/feature_108/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_108/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_108/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.493919 chalkpy-2.0.3/chalk/feature_n/feature_109/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_109/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_109/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.493919 chalkpy-2.0.3/chalk/feature_n/feature_11/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_11/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.493919 chalkpy-2.0.3/chalk/feature_n/feature_110/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_110/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_110/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.493919 chalkpy-2.0.3/chalk/feature_n/feature_111/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_111/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_111/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.493919 chalkpy-2.0.3/chalk/feature_n/feature_112/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_112/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_112/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.493919 chalkpy-2.0.3/chalk/feature_n/feature_113/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_113/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_113/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.493919 chalkpy-2.0.3/chalk/feature_n/feature_114/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_114/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_114/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.497919 chalkpy-2.0.3/chalk/feature_n/feature_115/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_115/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_115/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.497919 chalkpy-2.0.3/chalk/feature_n/feature_116/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_116/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_116/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.497919 chalkpy-2.0.3/chalk/feature_n/feature_117/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_117/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_117/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.497919 chalkpy-2.0.3/chalk/feature_n/feature_118/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_118/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_118/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.497919 chalkpy-2.0.3/chalk/feature_n/feature_119/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_119/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_119/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.497919 chalkpy-2.0.3/chalk/feature_n/feature_12/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_12/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_12/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.497919 chalkpy-2.0.3/chalk/feature_n/feature_120/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_120/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_120/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.497919 chalkpy-2.0.3/chalk/feature_n/feature_121/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_121/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_121/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.497919 chalkpy-2.0.3/chalk/feature_n/feature_122/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_122/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_122/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.497919 chalkpy-2.0.3/chalk/feature_n/feature_123/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_123/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_123/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.497919 chalkpy-2.0.3/chalk/feature_n/feature_124/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_124/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_124/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.497919 chalkpy-2.0.3/chalk/feature_n/feature_125/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_125/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_125/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.497919 chalkpy-2.0.3/chalk/feature_n/feature_126/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_126/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_126/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.501919 chalkpy-2.0.3/chalk/feature_n/feature_127/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_127/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_127/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.501919 chalkpy-2.0.3/chalk/feature_n/feature_128/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_128/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_128/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.501919 chalkpy-2.0.3/chalk/feature_n/feature_129/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_129/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_129/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.501919 chalkpy-2.0.3/chalk/feature_n/feature_13/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_13/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_13/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.501919 chalkpy-2.0.3/chalk/feature_n/feature_130/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_130/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_130/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.501919 chalkpy-2.0.3/chalk/feature_n/feature_131/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_131/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_131/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.501919 chalkpy-2.0.3/chalk/feature_n/feature_132/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_132/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_132/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.501919 chalkpy-2.0.3/chalk/feature_n/feature_133/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_133/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_133/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.501919 chalkpy-2.0.3/chalk/feature_n/feature_134/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_134/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_134/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.501919 chalkpy-2.0.3/chalk/feature_n/feature_135/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_135/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_135/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.501919 chalkpy-2.0.3/chalk/feature_n/feature_136/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_136/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_136/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.501919 chalkpy-2.0.3/chalk/feature_n/feature_137/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_137/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_137/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.501919 chalkpy-2.0.3/chalk/feature_n/feature_138/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_138/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_138/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.505919 chalkpy-2.0.3/chalk/feature_n/feature_139/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_139/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_139/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.505919 chalkpy-2.0.3/chalk/feature_n/feature_14/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_14/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_14/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.505919 chalkpy-2.0.3/chalk/feature_n/feature_140/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_140/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_140/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.505919 chalkpy-2.0.3/chalk/feature_n/feature_141/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_141/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_141/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.505919 chalkpy-2.0.3/chalk/feature_n/feature_142/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_142/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_142/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.505919 chalkpy-2.0.3/chalk/feature_n/feature_143/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_143/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_143/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.505919 chalkpy-2.0.3/chalk/feature_n/feature_144/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_144/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_144/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.505919 chalkpy-2.0.3/chalk/feature_n/feature_145/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_145/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_145/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.505919 chalkpy-2.0.3/chalk/feature_n/feature_146/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_146/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_146/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.505919 chalkpy-2.0.3/chalk/feature_n/feature_147/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_147/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_147/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.505919 chalkpy-2.0.3/chalk/feature_n/feature_148/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_148/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_148/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.505919 chalkpy-2.0.3/chalk/feature_n/feature_149/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_149/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_149/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.505919 chalkpy-2.0.3/chalk/feature_n/feature_15/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_15/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_15/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.509919 chalkpy-2.0.3/chalk/feature_n/feature_150/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_150/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_150/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.509919 chalkpy-2.0.3/chalk/feature_n/feature_151/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_151/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_151/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.509919 chalkpy-2.0.3/chalk/feature_n/feature_152/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_152/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_152/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.509919 chalkpy-2.0.3/chalk/feature_n/feature_153/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_153/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_153/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.509919 chalkpy-2.0.3/chalk/feature_n/feature_154/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_154/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_154/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.509919 chalkpy-2.0.3/chalk/feature_n/feature_155/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_155/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_155/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.509919 chalkpy-2.0.3/chalk/feature_n/feature_156/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_156/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_156/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.509919 chalkpy-2.0.3/chalk/feature_n/feature_157/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_157/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_157/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.509919 chalkpy-2.0.3/chalk/feature_n/feature_158/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_158/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_158/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.509919 chalkpy-2.0.3/chalk/feature_n/feature_159/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_159/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_159/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.509919 chalkpy-2.0.3/chalk/feature_n/feature_16/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_16/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_16/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.509919 chalkpy-2.0.3/chalk/feature_n/feature_160/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_160/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_160/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.509919 chalkpy-2.0.3/chalk/feature_n/feature_161/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_161/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_161/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.513919 chalkpy-2.0.3/chalk/feature_n/feature_162/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_162/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_162/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.513919 chalkpy-2.0.3/chalk/feature_n/feature_163/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_163/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_163/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.513919 chalkpy-2.0.3/chalk/feature_n/feature_164/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_164/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_164/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.513919 chalkpy-2.0.3/chalk/feature_n/feature_165/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_165/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_165/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.513919 chalkpy-2.0.3/chalk/feature_n/feature_166/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_166/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8389 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_166/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.513919 chalkpy-2.0.3/chalk/feature_n/feature_167/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_167/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_167/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.513919 chalkpy-2.0.3/chalk/feature_n/feature_168/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_168/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_168/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.513919 chalkpy-2.0.3/chalk/feature_n/feature_169/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_169/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_169/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.513919 chalkpy-2.0.3/chalk/feature_n/feature_17/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_17/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_17/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.513919 chalkpy-2.0.3/chalk/feature_n/feature_170/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_170/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_170/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.513919 chalkpy-2.0.3/chalk/feature_n/feature_171/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_171/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_171/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.513919 chalkpy-2.0.3/chalk/feature_n/feature_172/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_172/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_172/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.513919 chalkpy-2.0.3/chalk/feature_n/feature_173/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_173/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_173/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.517919 chalkpy-2.0.3/chalk/feature_n/feature_174/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_174/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_174/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.517919 chalkpy-2.0.3/chalk/feature_n/feature_175/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_175/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8848 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_175/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.517919 chalkpy-2.0.3/chalk/feature_n/feature_176/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_176/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_176/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.517919 chalkpy-2.0.3/chalk/feature_n/feature_177/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_177/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_177/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.517919 chalkpy-2.0.3/chalk/feature_n/feature_178/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_178/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_178/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.517919 chalkpy-2.0.3/chalk/feature_n/feature_179/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_179/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_179/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.517919 chalkpy-2.0.3/chalk/feature_n/feature_18/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_18/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_18/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.517919 chalkpy-2.0.3/chalk/feature_n/feature_180/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_180/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_180/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.517919 chalkpy-2.0.3/chalk/feature_n/feature_181/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_181/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_181/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.517919 chalkpy-2.0.3/chalk/feature_n/feature_182/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_182/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_182/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.517919 chalkpy-2.0.3/chalk/feature_n/feature_183/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_183/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_183/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.517919 chalkpy-2.0.3/chalk/feature_n/feature_184/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_184/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_184/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.517919 chalkpy-2.0.3/chalk/feature_n/feature_185/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_185/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_185/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.521919 chalkpy-2.0.3/chalk/feature_n/feature_186/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_186/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_186/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.521919 chalkpy-2.0.3/chalk/feature_n/feature_187/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_187/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_187/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.521919 chalkpy-2.0.3/chalk/feature_n/feature_188/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_188/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_188/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.521919 chalkpy-2.0.3/chalk/feature_n/feature_189/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_189/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9562 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_189/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.521919 chalkpy-2.0.3/chalk/feature_n/feature_19/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_19/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_19/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.521919 chalkpy-2.0.3/chalk/feature_n/feature_190/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_190/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_190/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.521919 chalkpy-2.0.3/chalk/feature_n/feature_191/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_191/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_191/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.521919 chalkpy-2.0.3/chalk/feature_n/feature_192/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_192/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_192/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.521919 chalkpy-2.0.3/chalk/feature_n/feature_193/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_193/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_193/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.521919 chalkpy-2.0.3/chalk/feature_n/feature_194/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_194/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9817 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_194/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.521919 chalkpy-2.0.3/chalk/feature_n/feature_195/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_195/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_195/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.521919 chalkpy-2.0.3/chalk/feature_n/feature_196/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_196/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9919 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_196/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.521919 chalkpy-2.0.3/chalk/feature_n/feature_197/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_197/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9970 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_197/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.525919 chalkpy-2.0.3/chalk/feature_n/feature_198/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_198/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_198/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.525919 chalkpy-2.0.3/chalk/feature_n/feature_199/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_199/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10072 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_199/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.525919 chalkpy-2.0.3/chalk/feature_n/feature_2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_2/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.525919 chalkpy-2.0.3/chalk/feature_n/feature_20/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_20/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_20/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.525919 chalkpy-2.0.3/chalk/feature_n/feature_200/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_200/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10123 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_200/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.525919 chalkpy-2.0.3/chalk/feature_n/feature_201/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_201/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_201/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.525919 chalkpy-2.0.3/chalk/feature_n/feature_202/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_202/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_202/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.525919 chalkpy-2.0.3/chalk/feature_n/feature_203/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_203/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_203/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.525919 chalkpy-2.0.3/chalk/feature_n/feature_204/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_204/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_204/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.525919 chalkpy-2.0.3/chalk/feature_n/feature_205/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_205/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_205/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.525919 chalkpy-2.0.3/chalk/feature_n/feature_206/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_206/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_206/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.525919 chalkpy-2.0.3/chalk/feature_n/feature_207/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_207/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_207/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.525919 chalkpy-2.0.3/chalk/feature_n/feature_208/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_208/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10531 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_208/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.525919 chalkpy-2.0.3/chalk/feature_n/feature_209/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_209/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_209/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.525919 chalkpy-2.0.3/chalk/feature_n/feature_21/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_21/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_21/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.525919 chalkpy-2.0.3/chalk/feature_n/feature_210/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_210/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_210/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.525919 chalkpy-2.0.3/chalk/feature_n/feature_211/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_211/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_211/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.529919 chalkpy-2.0.3/chalk/feature_n/feature_212/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_212/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_212/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.529919 chalkpy-2.0.3/chalk/feature_n/feature_213/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_213/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_213/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.529919 chalkpy-2.0.3/chalk/feature_n/feature_214/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_214/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_214/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.529919 chalkpy-2.0.3/chalk/feature_n/feature_215/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_215/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_215/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.529919 chalkpy-2.0.3/chalk/feature_n/feature_216/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_216/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_216/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.529919 chalkpy-2.0.3/chalk/feature_n/feature_217/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_217/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10990 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_217/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.529919 chalkpy-2.0.3/chalk/feature_n/feature_218/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_218/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_218/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.529919 chalkpy-2.0.3/chalk/feature_n/feature_219/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_219/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_219/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.529919 chalkpy-2.0.3/chalk/feature_n/feature_22/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_22/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_22/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.529919 chalkpy-2.0.3/chalk/feature_n/feature_220/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_220/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_220/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.529919 chalkpy-2.0.3/chalk/feature_n/feature_221/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_221/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_221/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.529919 chalkpy-2.0.3/chalk/feature_n/feature_222/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_222/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11245 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_222/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.529919 chalkpy-2.0.3/chalk/feature_n/feature_223/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_223/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11296 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_223/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.529919 chalkpy-2.0.3/chalk/feature_n/feature_224/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_224/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_224/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.529919 chalkpy-2.0.3/chalk/feature_n/feature_225/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_225/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_225/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.529919 chalkpy-2.0.3/chalk/feature_n/feature_226/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_226/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11449 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_226/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.529919 chalkpy-2.0.3/chalk/feature_n/feature_227/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_227/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_227/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.529919 chalkpy-2.0.3/chalk/feature_n/feature_228/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_228/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_228/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.533919 chalkpy-2.0.3/chalk/feature_n/feature_229/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_229/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11602 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_229/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.533919 chalkpy-2.0.3/chalk/feature_n/feature_23/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_23/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_23/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.533919 chalkpy-2.0.3/chalk/feature_n/feature_230/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_230/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11653 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_230/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.533919 chalkpy-2.0.3/chalk/feature_n/feature_231/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_231/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11704 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_231/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.533919 chalkpy-2.0.3/chalk/feature_n/feature_232/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_232/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11755 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_232/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.533919 chalkpy-2.0.3/chalk/feature_n/feature_233/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_233/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_233/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.533919 chalkpy-2.0.3/chalk/feature_n/feature_234/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_234/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_234/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.533919 chalkpy-2.0.3/chalk/feature_n/feature_235/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_235/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11908 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_235/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.533919 chalkpy-2.0.3/chalk/feature_n/feature_236/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_236/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_236/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.533919 chalkpy-2.0.3/chalk/feature_n/feature_237/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_237/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_237/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.533919 chalkpy-2.0.3/chalk/feature_n/feature_238/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_238/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_238/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.533919 chalkpy-2.0.3/chalk/feature_n/feature_239/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_239/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_239/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.533919 chalkpy-2.0.3/chalk/feature_n/feature_24/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_24/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_24/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.533919 chalkpy-2.0.3/chalk/feature_n/feature_240/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_240/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_240/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.533919 chalkpy-2.0.3/chalk/feature_n/feature_241/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_241/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_241/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.533919 chalkpy-2.0.3/chalk/feature_n/feature_242/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_242/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12265 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_242/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.533919 chalkpy-2.0.3/chalk/feature_n/feature_243/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_243/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_243/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.537920 chalkpy-2.0.3/chalk/feature_n/feature_244/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_244/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_244/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.537920 chalkpy-2.0.3/chalk/feature_n/feature_245/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_245/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_245/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.537920 chalkpy-2.0.3/chalk/feature_n/feature_246/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_246/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_246/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.537920 chalkpy-2.0.3/chalk/feature_n/feature_247/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_247/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12520 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_247/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.537920 chalkpy-2.0.3/chalk/feature_n/feature_248/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_248/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12571 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_248/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.537920 chalkpy-2.0.3/chalk/feature_n/feature_249/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_249/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_249/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.537920 chalkpy-2.0.3/chalk/feature_n/feature_25/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_25/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_25/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.537920 chalkpy-2.0.3/chalk/feature_n/feature_250/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_250/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12673 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_250/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.537920 chalkpy-2.0.3/chalk/feature_n/feature_251/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_251/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_251/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.537920 chalkpy-2.0.3/chalk/feature_n/feature_252/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_252/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12775 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_252/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.537920 chalkpy-2.0.3/chalk/feature_n/feature_253/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_253/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_253/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.537920 chalkpy-2.0.3/chalk/feature_n/feature_254/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_254/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12877 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_254/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.537920 chalkpy-2.0.3/chalk/feature_n/feature_255/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_255/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12928 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_255/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.537920 chalkpy-2.0.3/chalk/feature_n/feature_256/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_256/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12979 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_256/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.537920 chalkpy-2.0.3/chalk/feature_n/feature_26/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_26/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_26/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.537920 chalkpy-2.0.3/chalk/feature_n/feature_27/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_27/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_27/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.537920 chalkpy-2.0.3/chalk/feature_n/feature_28/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_28/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_28/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.541920 chalkpy-2.0.3/chalk/feature_n/feature_29/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_29/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_29/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.541920 chalkpy-2.0.3/chalk/feature_n/feature_3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_3/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.541920 chalkpy-2.0.3/chalk/feature_n/feature_30/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_30/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_30/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.541920 chalkpy-2.0.3/chalk/feature_n/feature_31/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_31/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_31/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.541920 chalkpy-2.0.3/chalk/feature_n/feature_32/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_32/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_32/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.541920 chalkpy-2.0.3/chalk/feature_n/feature_33/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_33/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_33/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.541920 chalkpy-2.0.3/chalk/feature_n/feature_34/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_34/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_34/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.541920 chalkpy-2.0.3/chalk/feature_n/feature_35/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_35/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_35/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.541920 chalkpy-2.0.3/chalk/feature_n/feature_36/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_36/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_36/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.541920 chalkpy-2.0.3/chalk/feature_n/feature_37/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_37/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_37/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.541920 chalkpy-2.0.3/chalk/feature_n/feature_38/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_38/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_38/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.541920 chalkpy-2.0.3/chalk/feature_n/feature_39/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_39/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_39/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.541920 chalkpy-2.0.3/chalk/feature_n/feature_4/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_4/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.541920 chalkpy-2.0.3/chalk/feature_n/feature_40/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_40/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_40/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.541920 chalkpy-2.0.3/chalk/feature_n/feature_41/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_41/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_41/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.541920 chalkpy-2.0.3/chalk/feature_n/feature_42/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_42/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_42/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.541920 chalkpy-2.0.3/chalk/feature_n/feature_43/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_43/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_43/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.541920 chalkpy-2.0.3/chalk/feature_n/feature_44/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_44/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_44/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.545920 chalkpy-2.0.3/chalk/feature_n/feature_45/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_45/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_45/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.545920 chalkpy-2.0.3/chalk/feature_n/feature_46/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_46/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_46/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.545920 chalkpy-2.0.3/chalk/feature_n/feature_47/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_47/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_47/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.545920 chalkpy-2.0.3/chalk/feature_n/feature_48/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_48/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_48/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.545920 chalkpy-2.0.3/chalk/feature_n/feature_49/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_49/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_49/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.545920 chalkpy-2.0.3/chalk/feature_n/feature_5/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_5/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.545920 chalkpy-2.0.3/chalk/feature_n/feature_50/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_50/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_50/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.545920 chalkpy-2.0.3/chalk/feature_n/feature_51/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_51/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_51/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.545920 chalkpy-2.0.3/chalk/feature_n/feature_52/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_52/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_52/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.545920 chalkpy-2.0.3/chalk/feature_n/feature_53/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_53/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_53/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.545920 chalkpy-2.0.3/chalk/feature_n/feature_54/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_54/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_54/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.545920 chalkpy-2.0.3/chalk/feature_n/feature_55/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_55/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_55/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.545920 chalkpy-2.0.3/chalk/feature_n/feature_56/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_56/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_56/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.545920 chalkpy-2.0.3/chalk/feature_n/feature_57/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_57/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_57/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.549920 chalkpy-2.0.3/chalk/feature_n/feature_58/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_58/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_58/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.549920 chalkpy-2.0.3/chalk/feature_n/feature_59/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_59/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_59/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.549920 chalkpy-2.0.3/chalk/feature_n/feature_6/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_6/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.549920 chalkpy-2.0.3/chalk/feature_n/feature_60/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_60/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_60/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.549920 chalkpy-2.0.3/chalk/feature_n/feature_61/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_61/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_61/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.549920 chalkpy-2.0.3/chalk/feature_n/feature_62/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_62/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_62/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.549920 chalkpy-2.0.3/chalk/feature_n/feature_63/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_63/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_63/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.549920 chalkpy-2.0.3/chalk/feature_n/feature_64/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_64/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_64/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.549920 chalkpy-2.0.3/chalk/feature_n/feature_65/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_65/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_65/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.549920 chalkpy-2.0.3/chalk/feature_n/feature_66/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_66/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_66/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.549920 chalkpy-2.0.3/chalk/feature_n/feature_67/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_67/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_67/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.549920 chalkpy-2.0.3/chalk/feature_n/feature_68/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_68/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_68/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.549920 chalkpy-2.0.3/chalk/feature_n/feature_69/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_69/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_69/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.549920 chalkpy-2.0.3/chalk/feature_n/feature_7/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_7/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_7/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.553920 chalkpy-2.0.3/chalk/feature_n/feature_70/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_70/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_70/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.553920 chalkpy-2.0.3/chalk/feature_n/feature_71/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_71/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_71/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.553920 chalkpy-2.0.3/chalk/feature_n/feature_72/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_72/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_72/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.553920 chalkpy-2.0.3/chalk/feature_n/feature_73/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_73/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_73/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.553920 chalkpy-2.0.3/chalk/feature_n/feature_74/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_74/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_74/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.553920 chalkpy-2.0.3/chalk/feature_n/feature_75/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_75/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_75/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.553920 chalkpy-2.0.3/chalk/feature_n/feature_76/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_76/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_76/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.553920 chalkpy-2.0.3/chalk/feature_n/feature_77/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_77/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_77/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.553920 chalkpy-2.0.3/chalk/feature_n/feature_78/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_78/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_78/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.553920 chalkpy-2.0.3/chalk/feature_n/feature_79/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_79/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_79/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.553920 chalkpy-2.0.3/chalk/feature_n/feature_8/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_8/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_8/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.553920 chalkpy-2.0.3/chalk/feature_n/feature_80/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_80/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_80/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.553920 chalkpy-2.0.3/chalk/feature_n/feature_81/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_81/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_81/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.557920 chalkpy-2.0.3/chalk/feature_n/feature_82/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_82/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_82/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.557920 chalkpy-2.0.3/chalk/feature_n/feature_83/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_83/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_83/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.557920 chalkpy-2.0.3/chalk/feature_n/feature_84/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_84/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_84/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.557920 chalkpy-2.0.3/chalk/feature_n/feature_85/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_85/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_85/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.557920 chalkpy-2.0.3/chalk/feature_n/feature_86/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_86/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_86/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.557920 chalkpy-2.0.3/chalk/feature_n/feature_87/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_87/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_87/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.557920 chalkpy-2.0.3/chalk/feature_n/feature_88/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_88/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_88/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.557920 chalkpy-2.0.3/chalk/feature_n/feature_89/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_89/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_89/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.557920 chalkpy-2.0.3/chalk/feature_n/feature_9/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_9/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_9/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.557920 chalkpy-2.0.3/chalk/feature_n/feature_90/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_90/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_90/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.557920 chalkpy-2.0.3/chalk/feature_n/feature_91/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_91/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_91/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.557920 chalkpy-2.0.3/chalk/feature_n/feature_92/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_92/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_92/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.557920 chalkpy-2.0.3/chalk/feature_n/feature_93/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_93/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_93/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.557920 chalkpy-2.0.3/chalk/feature_n/feature_94/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_94/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_94/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.561920 chalkpy-2.0.3/chalk/feature_n/feature_95/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_95/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_95/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.561920 chalkpy-2.0.3/chalk/feature_n/feature_96/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_96/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_96/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.561920 chalkpy-2.0.3/chalk/feature_n/feature_97/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_97/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_97/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.561920 chalkpy-2.0.3/chalk/feature_n/feature_98/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_98/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_98/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.561920 chalkpy-2.0.3/chalk/feature_n/feature_99/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_99/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/feature_n/feature_99/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.561920 chalkpy-2.0.3/chalk/features/
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16549 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/features/_chalkop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/features/_class_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/features/_document.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.565920 chalkpy-2.0.3/chalk/features/_encoding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/features/_encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13750 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/features/_encoding/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/features/_encoding/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/features/_encoding/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/features/_encoding/missing_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/features/_encoding/primitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/features/_encoding/pyarrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11211 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/features/_encoding/rich.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8835 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/features/_encoding/serialized_dtype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.565920 chalkpy-2.0.3/chalk/features/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/features/dataframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/features/dataframe/_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51213 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/features/dataframe/_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/features/dataframe/_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30875 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/features/feature_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/features/feature_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29431 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/features/feature_set_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/features/feature_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/features/feature_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/features/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/features/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/features/live_updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/features/primary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/features/pseudofeatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64172 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/features/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/features/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.565920 chalkpy-2.0.3/chalk/gitignore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/gitignore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/gitignore/gitignore_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/gitignore/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.565920 chalkpy-2.0.3/chalk/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/integrations/named.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.565920 chalkpy-2.0.3/chalk/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.565920 chalkpy-2.0.3/chalk/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/mypy_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.565920 chalkpy-2.0.3/chalk/parsed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/parsed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20749 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/parsed/_graph_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10943 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/parsed/duplicate_input_gql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13763 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/parsed/json_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/parsed/user_types_to_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.565920 chalkpy-2.0.3/chalk/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12079 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/serialization/parsed_annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.565920 chalkpy-2.0.3/chalk/sink/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/sink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/sink/_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.569920 chalkpy-2.0.3/chalk/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)    26581 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.569920 chalkpy-2.0.3/chalk/sql/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/sql/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/sql/_internal/chalk_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/sql/_internal/incremental.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.569920 chalkpy-2.0.3/chalk/sql/_internal/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/sql/_internal/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/sql/_internal/integrations/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/sql/_internal/integrations/cloudsql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/sql/_internal/integrations/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8105 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/sql/_internal/integrations/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/sql/_internal/integrations/redshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/sql/_internal/integrations/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/sql/_internal/integrations/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24525 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/sql/_internal/sql_file_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20277 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/sql/_internal/sql_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/sql/_internal/string_chalk_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17338 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/sql/finalized_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20430 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/sql/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.569920 chalkpy-2.0.3/chalk/streams/
+-rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/streams/_file_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/streams/_kafka_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11994 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/streams/_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/streams/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/streams/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.569920 chalkpy-2.0.3/chalk/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.573920 chalkpy-2.0.3/chalk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/utils/annotation_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/utils/async_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/utils/cached_type_hints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/utils/collection_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/utils/duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/utils/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/utils/environment_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/utils/log_with_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/utils/metaprogramming.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/utils/missing_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/utils/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/utils/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/utils/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19446 2023-05-02 01:30:13.000000 chalkpy-2.0.3/chalk/utils/stubgen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:30:32.573920 chalkpy-2.0.3/chalkpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23777 2023-05-02 01:30:32.000000 chalkpy-2.0.3/chalkpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-05-02 01:30:13.000000 chalkpy-2.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 01:30:32.573920 chalkpy-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-02 01:30:13.000000 chalkpy-2.0.3/setup.py
```

### Comparing `chalkpy-2.0.2/PKG-INFO` & `chalkpy-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chalkpy
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python SDK for Chalk
 Author: Chalk AI, Inc.
 Project-URL: homepage, https://chalk.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `chalkpy-2.0.2/README.md` & `chalkpy-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/__init__.py` & `chalkpy-2.0.3/chalk/__init__.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/_autosql/autosql.py` & `chalkpy-2.0.3/chalk/_autosql/autosql.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/_monitoring/Chart.py` & `chalkpy-2.0.3/chalk/_monitoring/Chart.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/_monitoring/charts_codegen.py` & `chalkpy-2.0.3/chalk/_monitoring/charts_codegen.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/_monitoring/charts_enums_codegen.py` & `chalkpy-2.0.3/chalk/_monitoring/charts_enums_codegen.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/_monitoring/charts_series_base.py` & `chalkpy-2.0.3/chalk/_monitoring/charts_series_base.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/_monitoring/gql_conversion.py` & `chalkpy-2.0.3/chalk/_monitoring/gql_conversion.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/_reporting/models.py` & `chalkpy-2.0.3/chalk/_reporting/models.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/_reporting/progress.py` & `chalkpy-2.0.3/chalk/_reporting/progress.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/_validation/validation.py` & `chalkpy-2.0.3/chalk/_validation/validation.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/cli.py` & `chalkpy-2.0.3/chalk/cli.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/client/__init__.py` & `chalkpy-2.0.3/chalk/client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,24 +362,40 @@
         ...     ],
         ...     dataset_name='my_dataset'
         ... )
         >>> dataset.download_data('my_directory')
         """
         ...
 
-    def recompute(self, features: Optional[List[Union[Feature, Any]]] = None, branch: Optional[str] = None):
+    def recompute(
+        self,
+        features: Optional[List[Union[Feature, Any]]] = None,
+        branch: Optional[str] = None,
+        wait: bool = False,
+        show_progress: bool = False,
+    ):
         """Creates a new revision of this dataset by recomputing the specified features.
 
         Carries out the new computation on the branch specified when constructing the client.
 
         Parameters
         ------
         features
             A list of specific features to recompute. Features that don't exist in the dataset will be added.
             If not provided, all the existing features in the dataset will be recomputed.
+        branch
+            If specified, Chalk will route your request to the relevant branch.
+            If None, Chalk will route your request to a non-branch deployment.
+            If not specified, Chalk will use the current client's branch info.
+        wait
+            If True, this method will block until recomputation is finished.
+        show_progress
+            [BETA] If True, progress bars will be shown while recomputation is running.
+            This flag will also be propogated to the methods of the resulting
+            `Dataset`.
 
         Raises
         ------
         ValueError
             If no branch was provided to the Chalk Client.
 
         Examples
@@ -637,14 +653,15 @@
         input_times: Union[Sequence[datetime], datetime, None] = None,
         output: Sequence[Union[str, Feature, Any]] = (),
         required_output: Sequence[FeatureReference] = (),
         environment: Optional[EnvironmentId] = None,
         dataset_name: Optional[str] = None,
         branch: Optional[BranchId] = ...,
         max_samples: Optional[int] = None,
+        wait: bool = False,
         show_progress: bool = False,
     ) -> Dataset:
         """Compute feature values from the offline store.
         See `Dataset` for more information.
 
         Parameters
         ----------
@@ -674,14 +691,16 @@
         max_samples
             The maximum number of samples to include in the `DataFrame`.
             If not specified, all samples will be returned.
         branch
             If specified, Chalk will route your request to the relevant branch.
             If None, Chalk will route your request to a non-branch deployment.
             If not specified, Chalk will use the current client's branch info.
+        wait
+            If True, this method will block until the query is finished.
         show_progress
             [BETA] If True, progress bars will be shown while the query is running.
             This flag will also be propogated to the methods of the resulting
             `Dataset`.
 
         Other Parameters
         ----------------
```

### Comparing `chalkpy-2.0.2/chalk/client/client_impl.py` & `chalkpy-2.0.3/chalk/client/client_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     ChalkGetDatasetException,
     ChalkOfflineQueryException,
     ChalkOnlineQueryException,
     ChalkRecomputeDatasetException,
     ChalkResolverRunException,
     ChalkUpdateGraphEntityException,
     ChalkWhoAmIException,
+    _generic_chalk_exception,
 )
 from chalk.client.models import (
     ChalkError,
     ComputeResolverOutputRequest,
     ComputeResolverOutputResponse,
     CreateOfflineQueryJobRequest,
     CreateOfflineQueryJobResponse,
@@ -455,15 +456,15 @@
             branch = self._config.branch
             result = self._request(
                 method="GET",
                 uri=f"/v1/branches",
                 response=_BranchMetadataResponse,
                 json=None,
                 environment_override=None,
-                exception_cls=ChalkBaseException,
+                exception_cls=_generic_chalk_exception("error getting branches"),
                 preview_deployment_id=None,
                 branch=branch,
                 api_server_override=self._get_local_server_override(None),
             )
 
         except ChalkBaseException as e:
             # If we can't get branches, we can't do anything else
@@ -607,16 +608,16 @@
         input_times: Union[Sequence[datetime], datetime, None] = None,
         output: Sequence[FeatureReference] = (),
         required_output: Sequence[FeatureReference] = (),
         environment: Optional[EnvironmentId] = None,
         dataset_name: Optional[str] = None,
         branch: Optional[BranchId] = ...,  # distinguished from user explicitly specifying branch=None
         max_samples: Optional[int] = None,
-        show_progress: bool = False,
         wait: bool = False,
+        show_progress: bool = False,
     ) -> DatasetImpl:
         if branch is Ellipsis:
             branch = self._config.branch
         unbranched = branch is None
         if wait and unbranched:
             raise ChalkOfflineQueryException(
                 errors=[
@@ -653,17 +654,15 @@
             max_samples=max_samples,
         )
 
         initialized_dataset = dataset_from_response(response, self)
         revision = initialized_dataset.revisions[-1]
         revision._show_progress = show_progress
         # Set as hydrated so that we never call hydration on datasets from unbranched queries.
-        revision._hydrated = (
-            unbranched or revision.status == QueryStatus.SUCCESSFUL or (isinstance(wait, float) and wait == 0.0)
-        )
+        revision._hydrated = revision._hydrated or unbranched or (isinstance(wait, float) and wait == 0.0)
 
         if not wait:
             return initialized_dataset
 
         revision.wait_for_completion()
         initialized_dataset.is_finished = True
         return initialized_dataset
@@ -919,22 +918,23 @@
             revision_id=str(revision_id) if revision_id is not None else None,
             features=[str(f) for f in features],
             branch=branch,
         )
         exception_name = str(dataset_name) if dataset_name else str(dataset_id) if dataset_id else None
         return self._request(
             method="POST",
-            uri="/v1/dataset/recompute",
+            uri="/v4/dataset/recompute",
             json=request,
             response=DatasetRevisionResponse,
             environment_override=environment,
             exception_cls=ChalkRecomputeDatasetException,
             preview_deployment_id=None,
             branch=branch,
             dataset_name=exception_name,
+            api_server_override=self._get_local_server_override(branch),
         )
 
     def _create_dataset_job(
         self,
         optional_output: List[str],
         required_output: List[str],
         query_input: Optional[OfflineQueryInput],
```

### Comparing `chalkpy-2.0.2/chalk/client/dataset.py` & `chalkpy-2.0.3/chalk/client/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -464,15 +464,15 @@
         num_bytes: Optional[int] = None,
         created_at: Optional[datetime] = None,
         started_at: Optional[datetime] = None,
         terminated_at: Optional[datetime] = None,
         dataset_name: Optional[str] = None,
         dataset_id: Optional[uuid.UUID] = None,
         branch: Optional[str] = None,
-        show_progress: bool = True,
+        show_progress: bool = False,
     ):
         self.revision_id = revision_id
         self.environment = environment
         self.creator_id = creator_id
         self.outputs = outputs
         self.givens_uri = givens_uri
         self.status = status
@@ -485,15 +485,15 @@
         self.started_at = started_at
         self.terminated_at = terminated_at
         self.dataset_name = dataset_name
         self.dataset_id = dataset_id
         self._client = client
         self._branch: BranchId = branch
         self._show_progress = show_progress
-        self._hydrated = False
+        self._hydrated = self.status == QueryStatus.SUCCESSFUL
 
     @property
     def data_as_polars(self) -> pl.LazyFrame:
         warnings.warn(
             DeprecationWarning(
                 "The property `DatasetRevision.data_as_polars` is deprecated. Please use the method `DatasetRevision.get_data_as_polars()` instead."
             )
@@ -744,31 +744,42 @@
         num_executors: Optional[int] = 16,
     ) -> None:
         return self.revisions[-1].download_data(
             path=path,
             num_executors=num_executors,
         )
 
-    def recompute(self, features: Optional[List[Union[Feature, Any]]] = None, branch: Optional[str] = None):
+    def recompute(
+        self,
+        features: Optional[List[Union[Feature, Any]]] = None,
+        branch: Optional[str] = None,
+        wait: bool = False,
+        show_progress: bool = False,
+    ):
         if len(self.revisions) == 0:
             raise IndexError("No revisions exist for dataset")
         if self._client._config.branch is None and branch is None:
             raise ValueError("A branch was not provided to the chalk client or as an argument to recompute.")
 
         new_revision_response = self._client._recompute_dataset(
             dataset_name=self.dataset_name,
             dataset_id=self.dataset_id,
             revision_id=self.revisions[-1].revision_id,
             features=features or [],
             branch=branch or self._client._config.branch,
             environment=self.environment,
         )
         new_revision = dataset_revision_from_response(new_revision_response, self._client)
-        new_revision._hydrated = True
+        new_revision._show_progress = show_progress
         self.revisions.append(new_revision)
+
+        if not wait:
+            return self
+
+        new_revision.wait_for_completion()
         return self
 
     def __repr__(self) -> str:
         if self.errors:
             return f"Dataset(name='{self.dataset_name}', version='{self.version}', errors='{self.errors}')"
         if self.dataset_name:
             return f"Dataset(name='{self.dataset_name}', version='{self.version}')"
```

### Comparing `chalkpy-2.0.2/chalk/client/exc.py` & `chalkpy-2.0.3/chalk/client/exc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import abc
-from typing import List, Optional
+from typing import List, Optional, Type, cast
 
 from chalk.client.models import ChalkError
 
 
 class ChalkBaseException(Exception, abc.ABC):
     """The base type for Chalk exceptions.
 
@@ -39,14 +39,29 @@
         """
         if self.errors:
             return self.message + "\n" + "\n".join(["\t" + e.message for e in self.errors])
 
         return self.message
 
 
+def _generate_chalk_exception_class(name: str, message: str) -> Type[ChalkBaseException]:
+    new_exception_cls = type(
+        name,
+        (ChalkBaseException,),
+        {
+            "message": message,
+        },
+    )
+    return cast(Type[ChalkBaseException], new_exception_cls)
+
+
+def _generic_chalk_exception(message: str) -> Type[ChalkBaseException]:
+    return _generate_chalk_exception_class("ChalkException", message)
+
+
 class ChalkCustomException(ChalkBaseException):
     def __init__(self, message: str, errors: Optional[List[ChalkError]] = None):
         self._message = message
         super().__init__(errors=errors)
 
     @property
     def message(self) -> str:
```

### Comparing `chalkpy-2.0.2/chalk/client/models.py` & `chalkpy-2.0.3/chalk/client/models.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/config/auth_config.py` & `chalkpy-2.0.3/chalk/config/auth_config.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/config/project_config.py` & `chalkpy-2.0.3/chalk/config/project_config.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/df/ast_parser.py` & `chalkpy-2.0.3/chalk/df/ast_parser.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/__init__.py` & `chalkpy-2.0.3/chalk/feature_n/__init__.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/codegen.py` & `chalkpy-2.0.3/chalk/feature_n/codegen.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_10/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_10/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_100/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_100/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_101/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_101/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_102/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_102/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_103/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_103/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_104/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_104/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_105/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_105/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_106/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_106/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_107/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_107/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_108/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_108/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_109/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_109/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_11/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_11/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_110/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_110/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_111/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_111/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_112/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_112/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_113/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_113/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_114/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_114/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_115/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_115/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_116/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_116/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_117/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_117/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_118/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_118/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_119/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_119/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_12/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_12/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_120/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_120/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_121/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_121/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_122/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_122/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_123/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_123/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_124/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_124/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_125/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_125/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_126/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_126/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_127/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_127/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_128/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_128/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_129/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_129/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_13/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_13/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_130/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_130/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_131/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_131/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_132/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_132/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_133/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_133/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_134/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_134/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_135/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_135/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_136/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_136/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_137/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_137/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_138/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_138/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_139/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_139/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_14/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_14/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_140/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_140/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_141/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_141/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_142/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_142/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_143/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_143/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_144/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_144/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_145/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_145/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_146/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_146/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_147/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_147/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_148/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_148/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_149/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_149/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_15/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_15/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_150/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_150/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_151/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_151/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_152/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_152/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_153/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_153/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_154/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_154/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_155/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_155/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_156/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_156/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_157/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_157/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_158/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_158/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_159/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_159/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_16/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_16/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_160/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_160/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_161/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_161/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_162/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_162/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_163/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_163/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_164/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_164/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_165/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_165/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_166/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_166/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_167/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_167/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_168/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_168/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_169/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_169/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_17/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_17/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_170/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_170/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_171/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_171/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_172/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_172/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_173/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_173/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_174/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_174/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_175/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_175/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_176/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_176/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_177/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_177/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_178/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_178/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_179/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_179/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_18/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_18/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_180/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_180/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_181/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_181/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_182/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_182/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_183/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_183/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_184/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_184/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_185/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_185/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_186/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_186/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_187/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_187/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_188/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_188/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_189/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_189/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_19/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_19/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_190/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_190/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_191/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_191/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_192/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_192/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_193/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_193/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_194/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_194/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_195/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_195/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_196/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_196/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_197/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_197/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_198/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_198/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_199/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_199/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_20/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_20/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_200/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_200/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_201/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_201/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_202/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_202/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_203/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_203/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_204/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_204/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_205/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_205/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_206/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_206/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_207/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_207/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_208/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_208/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_209/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_209/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_21/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_21/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_210/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_210/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_211/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_211/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_212/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_212/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_213/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_213/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_214/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_214/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_215/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_215/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_216/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_216/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_217/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_217/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_218/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_218/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_219/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_219/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_22/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_22/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_220/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_220/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_221/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_221/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_222/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_222/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_223/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_223/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_224/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_224/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_225/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_225/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_226/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_226/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_227/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_227/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_228/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_228/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_229/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_229/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_23/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_23/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_230/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_230/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_231/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_231/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_232/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_232/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_233/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_233/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_234/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_234/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_235/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_235/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_236/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_236/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_237/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_237/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_238/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_238/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_239/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_239/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_24/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_24/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_240/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_240/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_241/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_241/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_242/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_242/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_243/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_243/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_244/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_244/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_245/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_245/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_246/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_246/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_247/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_247/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_248/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_248/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_249/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_249/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_25/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_25/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_250/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_250/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_251/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_251/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_252/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_252/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_253/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_253/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_254/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_254/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_255/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_255/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_256/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_256/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_26/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_26/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_27/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_27/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_28/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_28/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_29/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_29/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_30/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_30/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_31/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_31/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_32/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_32/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_33/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_33/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_34/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_34/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_35/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_35/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_36/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_36/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_37/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_37/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_38/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_38/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_39/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_39/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_40/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_40/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_41/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_41/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_42/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_42/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_43/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_43/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_44/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_44/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_45/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_45/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_46/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_46/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_47/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_47/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_48/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_48/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_49/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_49/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_50/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_50/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_51/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_51/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_52/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_52/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_53/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_53/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_54/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_54/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_55/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_55/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_56/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_56/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_57/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_57/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_58/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_58/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_59/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_59/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_60/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_60/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_61/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_61/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_62/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_62/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_63/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_63/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_64/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_64/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_65/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_65/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_66/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_66/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_67/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_67/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_68/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_68/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_69/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_69/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_7/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_7/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_70/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_70/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_71/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_71/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_72/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_72/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_73/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_73/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_74/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_74/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_75/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_75/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_76/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_76/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_77/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_77/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_78/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_78/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_79/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_79/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_8/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_8/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_80/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_80/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_81/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_81/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_82/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_82/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_83/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_83/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_84/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_84/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_85/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_85/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_86/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_86/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_87/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_87/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_88/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_88/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_89/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_89/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_9/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_9/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_90/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_90/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_91/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_91/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_92/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_92/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_93/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_93/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_94/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_94/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_95/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_95/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_96/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_96/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_97/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_97/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_98/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_98/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/feature_n/feature_99/feature.py` & `chalkpy-2.0.3/chalk/feature_n/feature_99/feature.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/features/__init__.py` & `chalkpy-2.0.3/chalk/features/__init__.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/features/_chalkop.py` & `chalkpy-2.0.3/chalk/features/_chalkop.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/features/_class_property.py` & `chalkpy-2.0.3/chalk/features/_class_property.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/features/_encoding/converter.py` & `chalkpy-2.0.3/chalk/features/_encoding/converter.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/features/_encoding/inputs.py` & `chalkpy-2.0.3/chalk/features/_encoding/inputs.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/features/_encoding/json.py` & `chalkpy-2.0.3/chalk/features/_encoding/json.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/features/_encoding/pyarrow.py` & `chalkpy-2.0.3/chalk/features/_encoding/pyarrow.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/features/_encoding/rich.py` & `chalkpy-2.0.3/chalk/features/_encoding/rich.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/features/_encoding/serialized_dtype.py` & `chalkpy-2.0.3/chalk/features/_encoding/serialized_dtype.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/features/dataframe/_filters.py` & `chalkpy-2.0.3/chalk/features/dataframe/_filters.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/features/dataframe/_impl.py` & `chalkpy-2.0.3/chalk/features/dataframe/_impl.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/features/dataframe/_validation.py` & `chalkpy-2.0.3/chalk/features/dataframe/_validation.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/features/feature_field.py` & `chalkpy-2.0.3/chalk/features/feature_field.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/features/feature_set.py` & `chalkpy-2.0.3/chalk/features/feature_set.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/features/feature_set_decorator.py` & `chalkpy-2.0.3/chalk/features/feature_set_decorator.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/features/feature_time.py` & `chalkpy-2.0.3/chalk/features/feature_time.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/features/feature_wrapper.py` & `chalkpy-2.0.3/chalk/features/feature_wrapper.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/features/filter.py` & `chalkpy-2.0.3/chalk/features/filter.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/features/hooks.py` & `chalkpy-2.0.3/chalk/features/hooks.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/features/live_updates.py` & `chalkpy-2.0.3/chalk/features/live_updates.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/features/primary.py` & `chalkpy-2.0.3/chalk/features/primary.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/features/pseudofeatures.py` & `chalkpy-2.0.3/chalk/features/pseudofeatures.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/features/resolver.py` & `chalkpy-2.0.3/chalk/features/resolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import abc
+import asyncio
 import dataclasses
 import functools
 import inspect
 from dataclasses import dataclass
 from datetime import datetime
 from inspect import Parameter, isclass
 from typing import (
@@ -64,15 +65,15 @@
     from chalk.sql import BaseSQLSourceProtocol
 
 T = TypeVar("T")
 T_co = TypeVar("T_co", covariant=True)
 P = ParamSpec("P")
 V = TypeVar("V")
 
-ResolverHook: TypeAlias = "ClassVar[Optional[Callable[[Resolver], None]]]"
+ResolverHook: TypeAlias = "Optional[Callable[[Resolver], None]]"
 
 _logger = get_logger(__name__)
 
 
 @dataclasses.dataclass(frozen=True)
 class ResolverArgErrorHandler:
     default_value: Any
@@ -215,17 +216,55 @@
     def __hash__(self):
         return hash(self.fqn)
 
     @property
     def __name__(self):
         return self.fn.__name__
 
-    @abc.abstractmethod
+    def _process_call(self, *args: P.args, **kwargs: P.kwargs) -> T:
+        # __call__ is defined to support userland code that invokes a resolver
+        # as if it is a normal python function
+        # If the user returns a ChalkQuery, then we'll want to automatically execute it
+        from chalk.sql import FinalizedChalkQuery
+        from chalk.sql._internal.chalk_query import ChalkQuery
+        from chalk.sql._internal.string_chalk_query import StringChalkQuery
+
+        result = self.fn(*args, **kwargs)
+
+        if isinstance(result, (ChalkQuery, StringChalkQuery)):
+            result = result.all()
+        if isinstance(result, FinalizedChalkQuery):
+            result = result.execute(_flatten_features(self.output))
+        return result
+
+    async def _process_async_call(self, *args: P.args, **kwargs: P.kwargs):
+        # __call__ is defined to support userland code that invokes a resolver
+        # as if it is a normal python function
+        # If the user returns a ChalkQuery, then we'll want to automatically execute it
+        from chalk.sql import FinalizedChalkQuery
+        from chalk.sql._internal.chalk_query import ChalkQuery
+        from chalk.sql._internal.string_chalk_query import StringChalkQuery
+
+        assert asyncio.iscoroutinefunction(self.fn)
+
+        result = await self.fn(*args, **kwargs)
+
+        if isinstance(result, (ChalkQuery, StringChalkQuery)):
+            result = result.all()
+        if isinstance(result, FinalizedChalkQuery):
+            result = await result.async_execute(_flatten_features(self.output))
+        return result
+
     def __call__(self, *args: P.args, **kwargs: P.kwargs) -> T:
-        raise NotImplementedError
+        if asyncio.iscoroutinefunction(self.fn):
+            # Not awaiting this coroutine here -- when the caller awaits it,
+            # it will run
+            return cast(T, self._process_async_call(*args, **kwargs))
+        else:
+            return self._process_call(*args, **kwargs)
 
     @classmethod
     def add_to_registry(cls, r: Resolver):
         """
         Adds the given resolver to the registry, but first removes any existing resolvers with the same FQN.
         """
         new_resolvers = [r2 for r2 in cls.registry if r2.name != r.name]
@@ -236,35 +275,17 @@
     def name(self) -> str:
         return self.fqn.split(".")[-1]
 
 
 register_live_updates_if_in_notebook(Resolver)
 
 
-def _process_call(result: T, *, declared_output: Optional[Type[Features]]) -> T:
-    # __call__ is defined to support userland code that invokes a resolver
-    # as if it is a normal python function
-    # If the user returns a ChalkQuery, then we'll want to automatically execute it
-    from chalk.sql import FinalizedChalkQuery
-    from chalk.sql._internal.chalk_query import ChalkQuery
-    from chalk.sql._internal.string_chalk_query import StringChalkQuery
-
-    if isinstance(result, (ChalkQuery, StringChalkQuery)):
-        result = result.all()
-    if isinstance(result, FinalizedChalkQuery):
-        result = result.execute(_flatten_features(declared_output))
-    return result
-
-
 class SinkResolver(Resolver[P, T]):
     registry: "List[SinkResolver]" = []
 
-    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> T:
-        return _process_call(self.fn(*args, **kwargs), declared_output=None)
-
     def __init__(
         self,
         function_definition: str,
         fqn: str,
         filename: str,
         doc: Optional[str],
         inputs: List[Feature],
@@ -302,25 +323,22 @@
             max_delay = parse_chalk_duration(max_delay)
         self.max_delay = max_delay
         self.upsert = upsert
         self.integration = integration
         self.default_args = default_args
         self.max_staleness = None
         self.state = None
-        self.output = []
+        self.output = None
         self.input_is_df = input_is_df
 
     def __repr__(self):
         return f"SinkResolver(name={self.fqn})"
 
 
 class OnlineResolver(Resolver[P, T]):
-    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> T:
-        return _process_call(self.fn(*args, **kwargs), declared_output=self.output)
-
     def __init__(
         self,
         function_definition: str,
         fqn: str,
         filename: str,
         doc: Optional[str],
         inputs: List[Feature],
@@ -361,17 +379,14 @@
         self.timeout = timeout
 
     def __repr__(self):
         return f"OnlineResolver(name={self.fqn})"
 
 
 class OfflineResolver(Resolver[P, T]):
-    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> T:
-        return _process_call(self.fn(*args, **kwargs), declared_output=self.output)
-
     def __init__(
         self,
         function_definition: str,
         fqn: str,
         filename: str,
         doc: Optional[str],
         inputs: List[Feature],
@@ -1467,41 +1482,47 @@
     if not return_annotation:
         raise TypeError(f"Parse function '{parse_fqn}' must have a return annotation.")
     if get_origin(return_annotation) in (UnionType, Union):
         return_args = get_args(return_annotation)
         parse_output = next((a for a in return_args if a is not type(None)), None)
         if len(return_args) != 2 or type(None) not in return_args or parse_output is None:
             raise TypeError(
-                f"Parse function '{parse_fqn}' return annotation of length '{len(return_args)}' must be of length one "
-                f"(Optional is supported) "
+                (
+                    f"Parse function '{parse_fqn}' return annotation of length '{len(return_args)}' must be of length one "
+                    f"(Optional is supported) "
+                )
             )
         output_optional = True
     elif get_origin(return_annotation):
         raise TypeError(
             f"Parse function '{parse_fqn}' return annotation {return_annotation} must be either Optional or a singleton."
         )
     else:
         parse_output = return_annotation
     if not issubclass(parse_output, BaseModel):
         raise TypeError(f"Parse function '{parse_fqn}' return annotation must be of type pydantic.BaseModel")
     stream_fn_inputs = inspect.signature(stream_fn).parameters
     stream_input_annotations = [param.annotation for param in stream_fn_inputs.values()]
     if len(stream_input_annotations) != 1:
         raise TypeError(
-            f"Streaming resolver '{stream_fqn}' of length '{len(stream_input_annotations)}' must have "
-            f"one input argument"
+            (
+                f"Streaming resolver '{stream_fqn}' of length '{len(stream_input_annotations)}' must have "
+                f"one input argument"
+            )
         )
     stream_input_annotation = stream_input_annotations[0]
     if get_origin(stream_input_annotation) in (List, list):
         stream_input_args = get_args(stream_input_annotation)
         stream_input_arg = next((a for a in stream_input_args if a is not type(None)), None)
         if len(stream_input_args) != 1 or stream_input_arg is None:
             raise TypeError(
-                f"Streaming resolver '{stream_fqn}' input annotation of length '{len(stream_input_args)}' must be of "
-                f"length one (List or DataFrame supported) "
+                (
+                    f"Streaming resolver '{stream_fqn}' input annotation of length '{len(stream_input_args)}' must be of "
+                    f"length one (List or DataFrame supported) "
+                )
             )
     elif isinstance(stream_input_annotation, DataFrameMeta):
         stream_input_annotation = cast(Type[DataFrame], stream_input_annotation)
         stream_input_arg = stream_input_annotation.__pydantic_model__
     else:
         stream_input_arg = stream_input_annotation
     if parse_output != stream_input_arg:
@@ -1561,53 +1582,65 @@
         raise TypeError(f"Stream resolver '{stream_fqn}' outputs must be Features or DataFrame")
 
     for key, value in keys.items():
         if not isinstance(key, str):
             raise TypeError(f"Stream resolver '{stream_fqn}' key '{key}' should be type string")
         if key not in input_model_type.__fields__.keys():
             raise ValueError(
-                f"Stream resolver '{stream_fqn}' specifies an invalid ‘key’ mapping. "
-                f"Key ‘{key}’ is not an attribute in input model class '{input_model_type}'"
+                (
+                    f"Stream resolver '{stream_fqn}' specifies an invalid 'key' mapping. "
+                    f"Key '{key}' is not an attribute in input model class '{input_model_type}'"
+                )
             )
         if not isinstance(value, FeatureWrapper):
             raise TypeError(
-                f"Stream resolver '{stream_fqn}' maps key '{key}' to value '{value}', "
-                f"but '{value}' is not of type Feature"
+                (
+                    f"Stream resolver '{stream_fqn}' maps key '{key}' to value '{value}', "
+                    f"but '{value}' is not of type Feature"
+                )
             )
         value = unwrap_feature(value)
         if not value.is_scalar:
             raise TypeError(
-                f"Stream resolver '{stream_fqn}' maps key '{key}' to value '{value}', "
-                f"but '{value}' is not a scalar feature"
+                (
+                    f"Stream resolver '{stream_fqn}' maps key '{key}' to value '{value}', "
+                    f"but '{value}' is not a scalar feature"
+                )
             )
         if value not in output_features:
             output_fqns = [f.fqn for f in output_features]
             raise ValueError(
-                f"Stream resolver '{stream_fqn}' specifies an invalid ‘key’ mapping: "
-                f"Key ‘{key}’ is mapped to ‘{value}‘, but value '{value}' is not present"
-                f" in output features {output_fqns}"
+                (
+                    f"Stream resolver '{stream_fqn}' specifies an invalid 'key' mapping: "
+                    f"Key '{key}' is mapped to '{value}', but value '{value}' is not present"
+                    f" in output features {output_fqns}"
+                )
             )
     return {key: keys[key] for key in sorted(keys.keys())}
 
 
 def _validate_timestamp(stream_fn: Callable[P, T], timestamp: str, source: StreamSource):
     stream_fqn = get_resolver_fqn(function=stream_fn)
     input_model_type = _get_windowed_stream_resolver_input_type(stream_fn)
 
     if timestamp not in input_model_type.__fields__.keys():
         raise ValueError(
-            f"Stream resolver '{stream_fqn}' specifies an invalid ‘timestamp’ attribute. "
-            f"‘{timestamp}’ is not an attribute in input model class '{input_model_type}'"
+            (
+                f"Stream resolver '{stream_fqn}' specifies an invalid 'timestamp' attribute. "
+                f"'{timestamp}' is not an attribute in input model class '{input_model_type}'"
+            )
         )
     model_field = input_model_type.__fields__[timestamp]
     if model_field.type_ != datetime:
         raise TypeError(
-            f"Stream resolver '{stream_fqn}' specifies an invalid ‘timestamp’ attribute. "
-            f"‘{timestamp}’ field must be of type datetime.datetime. "
-            f"Use the parse function to convert your timestamp to a timezoned (not naive!) datetime."
+            (
+                f"Stream resolver '{stream_fqn}' specifies an invalid 'timestamp' attribute. "
+                f"'{timestamp}' field must be of type datetime.datetime. "
+                f"Use the parse function to convert your timestamp to a timezoned (not naive!) datetime."
+            )
         )
 
 
 def parse_and_register_stream_resolver(
     *,
     caller_globals: Optional[Dict[str, Any]],
     caller_locals: Optional[Dict[str, Any]],
@@ -1649,22 +1682,26 @@
         parse_info = _validate_parse_function(
             stream_fn=fn, parse_fn=parse, globals=caller_globals, locals=caller_locals
         )
     if keys is not None and mode == "continuous":
         keys = _validate_keys(stream_fn=fn, keys=keys)
     elif keys is None and mode == "continuous":
         raise ValueError(
-            f"Stream resolver '{fqn}' must take a 'keys' argument in the decorator "
-            f"if mode is continuous. The 'keys' argument should be dict mapping from "
-            f"the attribute of the incoming message to the Chalk feature"
+            (
+                f"Stream resolver '{fqn}' must take a 'keys' argument in the decorator "
+                f"if mode is continuous. The 'keys' argument should be dict mapping from "
+                f"the attribute of the incoming message to the Chalk feature"
+            )
         )
     elif keys and not is_windowed_resolver:
         raise ValueError(
-            f"Stream resolver '{fqn}' takes in a 'keys' argument in the decorator "
-            f"but is not a windowed resolver. Only windowed resolvers take in 'keys'."
+            (
+                f"Stream resolver '{fqn}' takes in a 'keys' argument in the decorator "
+                f"but is not a windowed resolver. Only windowed resolvers take in 'keys'."
+            )
         )
 
     if isinstance(output_features.features[0], type) and issubclass(output_features.features[0], DataFrame):
         output_feature_fqns = set(f.fqn for f in cast(Type[DataFrame], output_features.features[0]).columns)
     else:
         output_feature_fqns = set(f.fqn for f in output_features.features)
 
@@ -1674,24 +1711,28 @@
     )
     parsed = parse_function(fn, caller_globals, caller_locals, allow_custom_args=True, is_streaming_resolver=True)
 
     if timestamp and is_windowed_resolver:
         _validate_timestamp(stream_fn=fn, timestamp=timestamp, source=StreamSource)
     elif timestamp and not is_windowed_resolver:
         raise ValueError(
-            f"Stream resolver '{fqn}' takes in a 'timestamp' argument in the decorator "
-            f"but is not a windowed resolver. Only windowed resolvers take in 'timestamp'."
+            (
+                f"Stream resolver '{fqn}' takes in a 'timestamp' argument in the decorator "
+                f"but is not a windowed resolver. Only windowed resolvers take in 'timestamp'."
+            )
         )
     for resolver in StreamResolver.registry:
         if resolver.source == source:
             if resolver.timestamp != timestamp:
                 raise ValueError(
-                    f"Stream resolver '{fqn}' specifies ‘timestamp’ attribute, "
-                    f"but stream resolver '{resolver.fqn}' does not or specifies a different attribute. "
-                    f"Stream resolvers with the same source must all have the same timestamp value"
+                    (
+                        f"Stream resolver '{fqn}' specifies 'timestamp' attribute, "
+                        f"but stream resolver '{resolver.fqn}' does not or specifies a different attribute. "
+                        f"Stream resolvers with the same source must all have the same timestamp value"
+                    )
                 )
 
     resolver = StreamResolver(
         function_definition=parsed.function_definition,
         fqn=parsed.fqn,
         filename=caller_filename,
         source=source,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `chalkpy-2.0.2/chalk/features/tag.py` & `chalkpy-2.0.3/chalk/features/tag.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/gitignore/gitignore_parser.py` & `chalkpy-2.0.3/chalk/gitignore/gitignore_parser.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/gitignore/helper.py` & `chalkpy-2.0.3/chalk/gitignore/helper.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/importer.py` & `chalkpy-2.0.3/chalk/importer.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/integrations/named.py` & `chalkpy-2.0.3/chalk/integrations/named.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/logging/__init__.py` & `chalkpy-2.0.3/chalk/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/mypy_plugin.py` & `chalkpy-2.0.3/chalk/mypy_plugin.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/parsed/_graph_validation.py` & `chalkpy-2.0.3/chalk/parsed/_graph_validation.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/parsed/duplicate_input_gql.py` & `chalkpy-2.0.3/chalk/parsed/duplicate_input_gql.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/parsed/json_conversions.py` & `chalkpy-2.0.3/chalk/parsed/json_conversions.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/parsed/user_types_to_json.py` & `chalkpy-2.0.3/chalk/parsed/user_types_to_json.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/serialization/parsed_annotation.py` & `chalkpy-2.0.3/chalk/serialization/parsed_annotation.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/sql/__init__.py` & `chalkpy-2.0.3/chalk/sql/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -178,14 +178,15 @@
 
 
 @overload
 def PostgreSQLSource(
     *,
     name: str,
     engine_args: Optional[Dict[str, Any]] = ...,
+    async_engine_args: Optional[Dict[str, Any]] = ...,
 ) -> SQLSourceWithTableIngestProtocol:
     """If you have only one PostgreSQL integration, there's no need to provide
     a distinguishing name.
 
     But what happens when you have two data sources of the same kind?
     When you create a new data source from your dashboard,
     you have an option to provide a name for the integration.
@@ -194,14 +195,16 @@
     Parameters
     ----------
     name
         Name of the integration, as configured in your dashboard.
     engine_args
         Additional arguments to use when constructing the SQLAlchemy engine. These arguments will be
         merged with any default arguments from the named integration.
+    async_engine_args
+        Additional arguments to use when constructing an async SQLAlchemy engine.
 
     Returns
     -------
     SQLSourceWithTableIngestProtocol
         The SQL source for use in Chalk resolvers.
 
     Examples
@@ -216,14 +219,15 @@
     *,
     host: str = ...,
     port: Union[int, str] = ...,
     db: str = ...,
     user: str = ...,
     password: str = ...,
     engine_args: Optional[Dict[str, Any]] = ...,
+    async_engine_args: Optional[Dict[str, Any]] = ...,
 ) -> SQLSourceWithTableIngestProtocol:
     """You can also configure the integration directly using environment
     variables on your local machine or from those added through the
     generic environment variable support (https://docs.chalk.ai/docs/env-vars).
 
     Parameters
     ----------
@@ -235,14 +239,16 @@
         The database name.
     user
         PostgreSQL username to connect as.
     password
         The password to be used if the server demands password authentication.
     engine_args
         Additional arguments to use when constructing the SQLAlchemy engine.
+    async_engine_args
+        Additional arguments to use when constructing an async SQLAlchemy engine.
 
     Returns
     -------
     SQLSourceWithTableIngestProtocol
         The SQL source for use in Chalk resolvers.
 
     Examples
@@ -268,25 +274,28 @@
     host: Optional[str] = None,
     port: Optional[Union[int, str]] = None,
     db: Optional[str] = None,
     user: Optional[str] = None,
     password: Optional[str] = None,
     name: Optional[str] = None,
     engine_args: Optional[Dict[str, Any]] = None,
+    async_engine_args: Optional[Dict[str, Any]] = None,
 ) -> TableIngestProtocol:
     """Create a PostgreSQL data source. SQL-based data sources
     created without arguments assume a configuration in your
     Chalk Dashboard. Those created with the `name=` keyword
     argument will use the configuration for the integration
     with the given name. And finally, those created with
     explicit arguments will use those arguments to configure
     the data source. See the overloaded signatures for more
     details.
     """
-    return PostgreSQLSourceImpl(host, port, db, user, password, name, engine_args=engine_args)
+    return PostgreSQLSourceImpl(
+        host, port, db, user, password, name, engine_args=engine_args, async_engine_args=async_engine_args
+    )
 
 
 @overload
 def MySQLSource() -> SQLSourceWithTableIngestProtocol:
     """If you have only one MySQL connection that you'd like
     to add to Chalk, you do not need to specify any arguments
     to construct the source in your code.
@@ -304,14 +313,15 @@
 
 
 @overload
 def MySQLSource(
     *,
     name: str,
     engine_args: Optional[Dict[str, Any]] = ...,
+    async_engine_args: Optional[Dict[str, Any]] = ...,
 ) -> SQLSourceWithTableIngestProtocol:
     """If you have only one MySQL integration, there's no need to provide
     a distinguishing name.
 
     But what happens when you have two data sources of the same kind?
     When you create a new data source from your dashboard,
     you have an option to provide a name for the integration.
@@ -336,20 +346,21 @@
     """
     ...
 
 
 @overload
 def MySQLSource(
     *,
-    host: str = ...,
+    host: str,
     port: Union[int, str] = ...,
     db: str = ...,
     user: str = ...,
     password: str = ...,
     engine_args: Optional[Dict[str, Any]] = ...,
+    async_engine_args: Optional[Dict[str, Any]] = ...,
 ) -> SQLSourceWithTableIngestProtocol:
     """
     You can also configure the integration directly using environment
     variables on your local machine or from those added through the
     generic environment variable support (https://docs.chalk.ai/docs/env-vars).
 
     Parameters
@@ -362,14 +373,16 @@
         The database name.
     user
         MySQL username to connect as.
     password
         The password to be used if the server demands password authentication.
     engine_args
         Additional arguments to use when constructing the SQLAlchemy engine.
+    async_engine_args:
+        Additional arguments to use when constructing an async SQLAlchemy engine.
 
     Returns
     -------
     SQLSourceWithTableIngestProtocol
         The SQL source for use in Chalk resolvers.
 
     Examples
@@ -395,74 +408,86 @@
     host: Optional[str] = None,
     port: Optional[Union[int, str]] = None,
     db: Optional[str] = None,
     user: Optional[str] = None,
     password: Optional[str] = None,
     name: Optional[str] = None,
     engine_args: Optional[Dict[str, Any]] = None,
+    async_engine_args: Optional[Dict[str, Any]] = None,
 ) -> SQLSourceWithTableIngestProtocol:
     """Create a MySQL data source. SQL-based data sources
     created without arguments assume a configuration in your
     Chalk Dashboard. Those created with the `name=` keyword
     argument will use the configuration for the integration
     with the given name. And finally, those created with
     explicit arguments will use those arguments to configure
     the data source. See the overloaded signatures for more
     details.
     """
-    return MySQLSourceImpl(host, port, db, user, password, name, engine_args=engine_args)
+    return MySQLSourceImpl(
+        host, port, db, user, password, name, engine_args=engine_args, async_engine_args=async_engine_args
+    )
 
 
 def SQLiteInMemorySource(
-    name: Optional[str] = None, engine_args: Optional[Dict[str, Any]] = None
+    name: Optional[str] = None,
+    engine_args: Optional[Dict[str, Any]] = None,
+    async_engine_args: Optional[Dict[str, Any]] = None,
 ) -> SQLSourceWithTableIngestProtocol:
     """Testing SQL source.
 
     If you have only one SQLiteInMemorySource integration, there's no need to provide
     a distinguishing name.
 
     Parameters
     ----------
     name
         The name of the integration.
     engine_args
         Additional arguments to use when constructing the SQLAlchemy engine.
+    async_engine_args
+        Additional arguments to use when constructing an async SQLAlchemy engine.
 
     Returns
     -------
     SQLSourceWithTableIngestProtocol
         The SQL source for use in Chalk resolvers.
 
     Examples
     --------
     >>> source = SQLiteInMemorySource(name="RISK")
     """
-    return SQLiteSourceImpl(name=name, engine_args=engine_args)
+    return SQLiteSourceImpl(name=name, engine_args=engine_args, async_engine_args=async_engine_args)
 
 
 def SQLiteFileSource(
-    filename: Union[str, PathLike], name: Optional[str] = None, engine_args: Optional[Dict[str, Any]] = None
+    filename: Union[str, PathLike],
+    name: Optional[str] = None,
+    engine_args: Optional[Dict[str, Any]] = None,
+    async_engine_args: Optional[Dict[str, Any]] = None,
 ) -> SQLSourceWithTableIngestProtocol:
     """Create a SQLite source for a file.
 
     Parameters
     ----------
     filename
         The name of the file.
     name
         The name to use in testing
     engine_args
         Additional arguments to use when constructing the SQLAlchemy engine.
+    async_engine_args
+        Additional arguments to use when constructing an async SQLAlchemy engine.
 
     Returns
     -------
     SQLSourceWithTableIngestProtocol
         The SQL source for use in Chalk resolvers.
     """
-    return SQLiteSourceImpl(filename=filename, name=name, engine_args=engine_args)
+    return SQLiteSourceImpl(filename=filename, name=name, engine_args=engine_args, async_engine_args=async_engine_args)
 
 
 @overload
 def RedshiftSource() -> BaseSQLSourceProtocol:
     """If you have only one Redshift connection that you'd like
     to add to Chalk, you do not need to specify any arguments
     to construct the source in your code.
@@ -730,14 +755,15 @@
 
 
 @overload
 def CloudSQLSource(
     *,
     name: str,
     engine_args: Optional[Dict[str, Any]] = ...,
+    async_engine_args: Optional[Dict[str, Any]] = None,
 ) -> BaseSQLSourceProtocol:
     """If you have only one CloudSQL integration, there's no need to provide
     a distinguishing name.
 
     But what happens when you have two data sources of the same kind?
     When you create a new data source from your dashboard,
     you have an option to provide a name for the integration.
@@ -746,14 +772,16 @@
     Parameters
     ----------
     name
         Name of the integration, as configured in your dashboard.
     engine_args
         Additional arguments to use when constructing the SQLAlchemy engine. These arguments will be
         merged with any default arguments from the named integration.
+    async_engine_args
+        Additional arguments to use when constructing an async SQLAlchemy engine.
 
     Returns
     -------
     BaseSQLSourceProtocol
         The SQL source for use in Chalk resolvers.
 
     Examples
@@ -767,14 +795,15 @@
 def CloudSQLSource(
     *,
     instance_name: Optional[str] = ...,
     db: Optional[str] = ...,
     user: Optional[str] = ...,
     password: Optional[str] = ...,
     engine_args: Optional[Dict[str, Any]] = ...,
+    async_engine_args: Optional[Dict[str, Any]] = None,
 ) -> BaseSQLSourceProtocol:
     """You can also configure the integration directly using environment
     variables on your local machine or from those added through the
     generic environment variable support (https://docs.chalk.ai/docs/env-vars).
 
     Parameters
     ----------
@@ -784,14 +813,16 @@
         Database to use.
     user
         Username to use.
     password
         The password to use.
     engine_args
         Additional arguments to use when constructing the SQLAlchemy engine.
+    async_engine_args
+        Additional arguments to use when constructing an async SQLAlchemy engine.
 
     Returns
     -------
     BaseSQLSourceProtocol
         The SQL source for use in Chalk resolvers.
 
     Examples
@@ -810,14 +841,15 @@
     *,
     name: Optional[str] = None,
     instance_name: Optional[str] = None,
     db: Optional[str] = None,
     user: Optional[str] = None,
     password: Optional[str] = None,
     engine_args: Optional[Dict[str, Any]] = None,
+    async_engine_args: Optional[Dict[str, Any]] = None,
 ) -> BaseSQLSourceProtocol:
     """Create a CloudSQL data source. SQL-based data sources
     created without arguments assume a configuration in your
     Chalk Dashboard. Those created with the `name=` keyword
     argument will use the configuration for the integration
     with the given name. And finally, those created with
     explicit arguments will use those arguments to configure
@@ -827,14 +859,15 @@
     return CloudSQLSourceImpl(
         name=name,
         instance_name=instance_name,
         db=db,
         user=user,
         password=password,
         engine_args=engine_args,
+        async_engine_args=async_engine_args,
     )
 
 
 __all__ = [
     "BaseSQLSourceProtocol",
     "BigQuerySource",
     "CloudSQLSource",
```

### Comparing `chalkpy-2.0.2/chalk/sql/_internal/chalk_query.py` & `chalkpy-2.0.3/chalk/sql/_internal/chalk_query.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/sql/_internal/incremental.py` & `chalkpy-2.0.3/chalk/sql/_internal/incremental.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/sql/_internal/integrations/bigquery.py` & `chalkpy-2.0.3/chalk/sql/_internal/integrations/bigquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,15 @@
     validate_dtypes_for_efficient_execution,
 )
 from chalk.sql.finalized_query import FinalizedChalkQuery
 from chalk.utils.log_with_context import get_logger
 from chalk.utils.missing_dependency import missing_dependency_exception
 
 if TYPE_CHECKING:
-    from google.cloud import bigquery, bigquery_storage_v1
-    from google.cloud.bigquery import ScalarQueryParameter, ScalarQueryParameterType, dbapi
+    from google.cloud.bigquery import ScalarQueryParameterType
     from sqlalchemy.engine import Connection
     from sqlalchemy.engine.url import URL
 
 try:
     import sqlalchemy as sa
 except ImportError:
     sa = None
@@ -116,15 +115,15 @@
         self.project = project or load_integration_variable(integration_name=name, name="BQ_PROJECT")
         self.credentials_base64 = credentials_base64 or load_integration_variable(
             integration_name=name, name="BQ_CREDENTIALS_BASE64"
         )
         self.credentials_path = credentials_path or load_integration_variable(
             integration_name=name, name="BQ_CREDENTIALS_PATH"
         )
-        BaseSQLSource.__init__(self, name=name, engine_args=engine_args)
+        BaseSQLSource.__init__(self, name=name, engine_args=engine_args, async_engine_args={})
 
     def local_engine_url(self) -> URL:
         from sqlalchemy.engine.url import URL
 
         query = {
             k: v
             for k, v in {
@@ -136,14 +135,15 @@
         }
         return URL.create(drivername="bigquery", host=self.project, database=self.dataset, query=query)
 
     @contextlib.contextmanager
     def _get_bq_client(self):
         # gated already
         import google.cloud.bigquery
+        import google.cloud.bigquery.dbapi
 
         with self.get_engine().connect() as conn:
             dbapi = conn.connection.dbapi_connection
             assert isinstance(dbapi, google.cloud.bigquery.dbapi.Connection)
             client = dbapi._client
             assert isinstance(client, google.cloud.bigquery.Client)
             yield client
@@ -152,16 +152,15 @@
         self,
         finalized_query: FinalizedChalkQuery,
         columns_to_converters: Callable[[List[str]], Dict[str, FeatureConverter]],
         connection: Optional[Connection],
     ) -> pa.Table:
         try:
             try:
-                from google.cloud import bigquery, bigquery_storage_v1
-                from google.cloud.bigquery import ScalarQueryParameter, dbapi
+                from google.cloud import bigquery
                 from sqlalchemy.sql import Select
             except ModuleNotFoundError:
                 raise missing_dependency_exception("chalkpy[bigquery]")
 
             if isinstance(finalized_query.query, Select):
                 validate_dtypes_for_efficient_execution(
                     finalized_query.query, _supported_sqlalchemy_types_for_pa_querying
```

### Comparing `chalkpy-2.0.2/chalk/sql/_internal/integrations/cloudsql.py` & `chalkpy-2.0.3/chalk/sql/_internal/integrations/cloudsql.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,29 +16,34 @@
         *,
         instance_name: Optional[str] = None,
         db: Optional[str] = None,
         user: Optional[str] = None,
         password: Optional[str] = None,
         name: Optional[str] = None,
         engine_args: Optional[Dict[str, Any]] = None,
+        async_engine_args: Optional[Dict[str, Any]] = None,
     ):
         try:
             import psycopg2
         except ImportError:
             raise missing_dependency_exception("chalkpy[postgresql]")
         del psycopg2  # unused
         prefix = name + "_" if name else ""
         self.instance_name = instance_name or os.getenv(prefix + "CLOUDSQL_INSTANCE_NAME")
         self.db = db or os.getenv(prefix + "CLOUDSQL_DATABASE")
         self.user = user or os.getenv(prefix + "CLOUDSQL_USER")
         self.password = password or os.getenv(prefix + "CLOUDSQL_PASSWORD")
         if engine_args is None:
             engine_args = {}
+        if async_engine_args is None:
+            async_engine_args = {}
         engine_args.setdefault("pool_size", 20)
         engine_args.setdefault("max_overflow", 60)
+        async_engine_args.setdefault("pool_size", 20)
+        async_engine_args.setdefault("max_overflow", 60)
         engine_args.setdefault(
             "connect_args",
             {
                 "keepalives": 1,
                 "keepalives_idle": 30,
                 "keepalives_interval": 10,
                 "keepalives_count": 5,
@@ -46,20 +51,33 @@
         )
         # We set the default isolation level to autocommit since the SQL sources are read-only, and thus
         # transactions are not needed
         # Setting the isolation level on the engine, instead of the connection, avoids
         # a DBAPI statement to reset the transactional level back to the default before returning the
         # connection to the pool
         engine_args.setdefault("isolation_level", os.environ.get("CHALK_SQL_ISOLATION_LEVEL", "AUTOCOMMIT"))
-        BaseSQLSource.__init__(self, name=name, engine_args=engine_args)
+        async_engine_args.setdefault("isolation_level", os.environ.get("CHALK_SQL_ISOLATION_LEVEL", "AUTOCOMMIT"))
+        BaseSQLSource.__init__(self, name=name, engine_args=engine_args, async_engine_args=async_engine_args)
 
     def local_engine_url(self) -> URL:
         from sqlalchemy.engine.url import URL
 
         return URL.create(
-            drivername="postgresql",
+            drivername="postgresql+psycopg2",
+            username=self.user,
+            password=self.password,
+            host="",
+            query={"host": "{}/{}/.s.PGSQL.5432".format("/cloudsql", self.instance_name)},
+            database=self.db,
+        )
+
+    def async_local_engine_url(self) -> URL:
+        from sqlalchemy.engine.url import URL
+
+        return URL.create(
+            drivername="postgresql+asyncpg",
             username=self.user,
             password=self.password,
             host="",
             query={"host": "{}/{}/.s.PGSQL.5432".format("/cloudsql", self.instance_name)},
             database=self.db,
         )
```

### Comparing `chalkpy-2.0.2/chalk/sql/_internal/integrations/mysql.py` & `chalkpy-2.0.3/chalk/sql/_internal/integrations/mysql.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,15 @@
         host: Optional[str] = None,
         port: Optional[Union[int, str]] = None,
         db: Optional[str] = None,
         user: Optional[str] = None,
         password: Optional[str] = None,
         name: Optional[str] = None,
         engine_args: Optional[Dict[str, Any]] = None,
+        async_engine_args: Optional[Dict[str, Any]] = None,
     ):
         try:
             import pymysql
         except ModuleNotFoundError:
             raise missing_dependency_exception("chalkpy[mysql]")
         del pymysql
         self.name = name
@@ -37,28 +38,45 @@
         )
         self.db = db or load_integration_variable(name="MYSQL_DATABASE", integration_name=name)
         self.user = user or load_integration_variable(name="MYSQL_USER", integration_name=name)
         self.password = password or load_integration_variable(name="MYSQL_PWD", integration_name=name)
         self.ingested_tables: Dict[str, Any] = {}
         if engine_args is None:
             engine_args = {}
+        if async_engine_args is None:
+            async_engine_args = {}
         engine_args.setdefault("pool_size", 20)
         engine_args.setdefault("max_overflow", 60)
+        async_engine_args.setdefault("pool_size", 20)
+        async_engine_args.setdefault("max_overflow", 60)
         # We set the default isolation level to autocommit since the SQL sources are read-only, and thus
         # transactions are not needed
         # Setting the isolation level on the engine, instead of the connection, avoids
         # a DBAPI statement to reset the transactional level back to the default before returning the
         # connection to the pool
         engine_args.setdefault("isolation_level", os.environ.get("CHALK_SQL_ISOLATION_LEVEL", "AUTOCOMMIT"))
-        BaseSQLSource.__init__(self, name=name, engine_args=engine_args)
+        async_engine_args.setdefault("isolation_level", os.environ.get("CHALK_SQL_ISOLATION_LEVEL", "AUTOCOMMIT"))
+        BaseSQLSource.__init__(self, name=name, engine_args=engine_args, async_engine_args=async_engine_args)
 
     def local_engine_url(self) -> URL:
         from sqlalchemy.engine.url import URL
 
         return URL.create(
             drivername="mysql+pymysql",
             username=self.user,
             password=self.password,
             host=self.host,
             port=self.port,
             database=self.db,
         )
+
+    def async_local_engine_url(self) -> URL:
+        from sqlalchemy.engine.url import URL
+
+        return URL.create(
+            drivername="mysql+aiomysql",
+            username=self.user,
+            password=self.password,
+            host=self.host,
+            port=self.port,
+            database=self.db,
+        )
```

### Comparing `chalkpy-2.0.2/chalk/sql/_internal/integrations/postgres.py` & `chalkpy-2.0.3/chalk/sql/_internal/integrations/postgres.py`

 * *Files 7% similar despite different names*

```diff
@@ -66,14 +66,15 @@
         host: Optional[str] = None,
         port: Optional[Union[int, str]] = None,
         db: Optional[str] = None,
         user: Optional[str] = None,
         password: Optional[str] = None,
         name: Optional[str] = None,
         engine_args: Optional[Dict[str, Any]] = None,
+        async_engine_args: Optional[Dict[str, Any]] = None,
     ):
         try:
             import psycopg2
         except ImportError:
             raise missing_dependency_exception("chalkpy[postgresql]")
         del psycopg2  # unused
         self.name = name
@@ -85,16 +86,20 @@
         )
         self.db = db or load_integration_variable(integration_name=name, name="PGDATABASE")
         self.user = user or load_integration_variable(integration_name=name, name="PGUSER")
         self.password = password or load_integration_variable(integration_name=name, name="PGPASSWORD")
         self.ingested_tables: Dict[str, Any] = {}
         if engine_args is None:
             engine_args = {}
+        if async_engine_args is None:
+            async_engine_args = {}
         engine_args.setdefault("pool_size", 20)
         engine_args.setdefault("max_overflow", 60)
+        async_engine_args.setdefault("pool_size", 20)
+        async_engine_args.setdefault("max_overflow", 60)
         engine_args.setdefault(
             "connect_args",
             {
                 "keepalives": 1,
                 "keepalives_idle": 30,
                 "keepalives_interval": 10,
                 "keepalives_count": 5,
@@ -102,21 +107,34 @@
         )
         # We set the default isolation level to autocommit since the SQL sources are read-only, and thus
         # transactions are not needed
         # Setting the isolation level on the engine, instead of the connection, avoids
         # a DBAPI statement to reset the transactional level back to the default before returning the
         # connection to the pool
         engine_args.setdefault("isolation_level", os.environ.get("CHALK_SQL_ISOLATION_LEVEL", "AUTOCOMMIT"))
-        BaseSQLSource.__init__(self, name=name, engine_args=engine_args)
+        async_engine_args.setdefault("isolation_level", os.environ.get("CHALK_SQL_ISOLATION_LEVEL", "AUTOCOMMIT"))
+        BaseSQLSource.__init__(self, name=name, engine_args=engine_args, async_engine_args=async_engine_args)
 
     def local_engine_url(self) -> URL:
         from sqlalchemy.engine.url import URL
 
         return URL.create(
-            drivername="postgresql",
+            drivername="postgresql+psycopg2",
+            username=self.user,
+            password=self.password,
+            host=self.host,
+            port=self.port,
+            database=self.db,
+        )
+
+    def async_local_engine_url(self) -> URL:
+        from sqlalchemy.engine.url import URL
+
+        return URL.create(
+            drivername="postgresql+asyncpg",
             username=self.user,
             password=self.password,
             host=self.host,
             port=self.port,
             database=self.db,
         )
```

### Comparing `chalkpy-2.0.2/chalk/sql/_internal/integrations/redshift.py` & `chalkpy-2.0.3/chalk/sql/_internal/integrations/redshift.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         )
         # We set the default isolation level to autocommit since the SQL sources are read-only, and thus
         # transactions are not needed
         # Setting the isolation level on the engine, instead of the connection, avoids
         # a DBAPI statement to reset the transactional level back to the default before returning the
         # connection to the pool
         engine_args.setdefault("isolation_level", os.environ.get("CHALK_SQL_ISOLATION_LEVEL", "AUTOCOMMIT"))
-        BaseSQLSource.__init__(self, name=name, engine_args=engine_args)
+        BaseSQLSource.__init__(self, name=name, engine_args=engine_args, async_engine_args={})
 
     def local_engine_url(self) -> URL:
         from sqlalchemy.engine.url import URL
 
         return URL.create(
             drivername="redshift+psycopg2",
             username=self.user,
```

### Comparing `chalkpy-2.0.2/chalk/sql/_internal/integrations/snowflake.py` & `chalkpy-2.0.3/chalk/sql/_internal/integrations/snowflake.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         )
         self.warehouse = warehouse or load_integration_variable(integration_name=name, name="SNOWFLAKE_WAREHOUSE")
         self.user = user or load_integration_variable(integration_name=name, name="SNOWFLAKE_USER")
         self.password = password or load_integration_variable(integration_name=name, name="SNOWFLAKE_PASSWORD")
         self.db = db or load_integration_variable(integration_name=name, name="SNOWFLAKE_DATABASE")
         self.schema = schema or load_integration_variable(integration_name=name, name="SNOWFLAKE_SCHEMA")
         self.role = role or load_integration_variable(integration_name=name, name="SNOWFLAKE_ROLE")
-        BaseSQLSource.__init__(self, name=name, engine_args=engine_args)
+        BaseSQLSource.__init__(self, name=name, engine_args=engine_args, async_engine_args={})
 
     def local_engine_url(self) -> URL:
         from sqlalchemy.engine.url import URL
 
         query = {
             k: v
             for k, v in (
```

### Comparing `chalkpy-2.0.2/chalk/sql/_internal/integrations/sqlite.py` & `chalkpy-2.0.3/chalk/sql/_internal/integrations/sqlite.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,27 +17,39 @@
 
 class SQLiteSourceImpl(TableIngestMixIn, BaseSQLSource, SQLSourceWithTableIngestProtocol):
     def __init__(
         self,
         name: Optional[str] = None,
         filename: Optional[Union[PathLike, str]] = None,
         engine_args: Optional[Dict[str, Any]] = None,
+        async_engine_args: Optional[Dict[str, Any]] = None,
     ):
         self.ingested_tables: Dict[str, Any] = {}
         self.filename = filename
         if engine_args is None:
             engine_args = {}
+        if async_engine_args is None:
+            async_engine_args = {}
         # We set the default isolation level to autocommit since the SQL sources are read-only, and thus
         # transactions are not needed
         # Setting the isolation level on the engine, instead of the connection, avoids
         # a DBAPI statement to reset the transactional level back to the default before returning the
         # connection to the pool
         engine_args.setdefault("isolation_level", os.environ.get("CHALK_SQL_ISOLATION_LEVEL", "AUTOCOMMIT"))
-        BaseSQLSource.__init__(self, name=name, engine_args=engine_args)
+        async_engine_args.setdefault("isolation_level", os.environ.get("CHALK_SQL_ISOLATION_LEVEL", "AUTOCOMMIT"))
+        BaseSQLSource.__init__(self, name=name, engine_args=engine_args, async_engine_args=async_engine_args)
 
     def local_engine_url(self) -> URL:
         try:
             from sqlalchemy.engine.url import URL
         except ImportError:
             raise missing_dependency_exception("chalkpy[sqlite]")
         database = ":memory:" if self.filename is None else str(self.filename)
-        return URL.create(drivername="sqlite", database=database, query={"check_same_thread": "true"})
+        return URL.create(drivername="sqlite+pysqlite", database=database, query={"check_same_thread": "true"})
+
+    def async_local_engine_url(self) -> URL:
+        try:
+            from sqlalchemy.engine.url import URL
+        except ImportError:
+            raise missing_dependency_exception("chalkpy[sqlite]")
+        database = ":memory:" if self.filename is None else str(self.filename)
+        return URL.create(drivername="sqlite+aiosqlite", database=database, query={"check_same_thread": "true"})
```

### Comparing `chalkpy-2.0.2/chalk/sql/_internal/sql_file_resolver.py` & `chalkpy-2.0.3/chalk/sql/_internal/sql_file_resolver.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/sql/_internal/sql_source.py` & `chalkpy-2.0.3/chalk/sql/_internal/sql_source.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
+import asyncio
 import contextlib
-import functools
 import inspect
 import json
 import logging
 import os
 import os.path
 import warnings
 from dataclasses import dataclass
@@ -32,19 +32,21 @@
 from chalk.features import Feature, FeatureConverter, Features, FeatureWrapper, unwrap_feature
 from chalk.integrations.named import load_integration_variable
 from chalk.sql._internal.chalk_query import ChalkQuery
 from chalk.sql._internal.incremental import IncrementalSettings
 from chalk.sql._internal.string_chalk_query import StringChalkQuery
 from chalk.sql.finalized_query import FinalizedChalkQuery
 from chalk.sql.protocols import BaseSQLSourceProtocol, ChalkQueryProtocol, StringChalkQueryProtocol, TableIngestProtocol
+from chalk.utils.async_helpers import async_null_context
 from chalk.utils.environment_parsing import env_var_bool
 from chalk.utils.log_with_context import get_logger, get_logging_context
 from chalk.utils.missing_dependency import missing_dependency_exception
 
 if TYPE_CHECKING:
+    import sqlalchemy.ext.asyncio
     from sqlalchemy.engine import URL, Connection, Engine
     from sqlalchemy.orm import Session
     from sqlalchemy.sql import Select
     from sqlalchemy.sql.elements import Label
     from sqlalchemy.types import TypeEngine
 
 TTableIngestMixIn = TypeVar("TTableIngestMixIn", bound="TableIngestMixIn")
@@ -132,34 +134,46 @@
         )
         return self
 
 
 class BaseSQLSource(BaseSQLSourceProtocol):
     registry: ClassVar[List["BaseSQLSource"]] = []
 
-    def __init__(self, name: Optional[str], engine_args: Optional[Dict[str, Any]]):
+    def __init__(
+        self,
+        name: Optional[str],
+        engine_args: Optional[Dict[str, Any]],
+        async_engine_args: Optional[Dict[str, Any]],
+    ):
         try:
             import sqlalchemy
         except ImportError:
             raise missing_dependency_exception("chalkpy[sql]")
         del sqlalchemy  # unused
 
         self._incremental_settings = None
         self._resolver_and_sqlfile_to_sqlstring: Dict[Tuple[str, str], str] = {}
         self.registry.append(self)
         self.name = name
         if engine_args is None:
             engine_args = {}
+        if async_engine_args is None:
+            async_engine_args = {}
         if self.name is not None:
             for k, v in self._load_env_engine_args(name=self.name).items():
                 engine_args.setdefault(k, v)
+                async_engine_args.setdefault(k, v)
         engine_args.setdefault("pool_pre_ping", env_var_bool("USE_CLIENT_POOL_PRE_PING"))
-        engine_args.setdefault("url", self.local_engine_url())
         engine_args.setdefault("echo", CHALK_QUERY_LOGGING)
-        self.engine_args = engine_args
+        async_engine_args.setdefault("pool_pre_ping", env_var_bool("USE_CLIENT_POOL_PRE_PING"))
+        async_engine_args.setdefault("echo", CHALK_QUERY_LOGGING)
+        self._engine_args = engine_args
+        self._async_engine_args = async_engine_args
+        self._engine = None
+        self._async_engine = None
 
     def query_sql_file(
         self,
         path: Union[str, bytes, PathLike],
         fields: Optional[Mapping[str, Union[Feature, str, Any]]] = None,
         args: Optional[Mapping[str, object]] = None,
     ) -> StringChalkQueryProtocol:
@@ -232,14 +246,17 @@
             targets=targets,
             source=self,
         )
 
     def local_engine_url(self) -> URL:
         raise NotImplementedError
 
+    def async_local_engine_url(self) -> URL:
+        raise NotImplementedError
+
     def execute_query(
         self,
         finalized_query: FinalizedChalkQuery,
         columns_to_converters: Callable[[List[str]], Dict[str, FeatureConverter]],
         connection: Optional[Connection] = None,
     ) -> pa.Table:
         try:
@@ -254,14 +271,72 @@
             pass
         except UnsupportedEfficientExecutionError as e:
             log_level = e.log_level
             _logger.log(log_level, str(e))
 
         return self.execute_query_inefficient(finalized_query, columns_to_converters, connection)
 
+    async def async_execute_query(
+        self,
+        finalized_query: FinalizedChalkQuery,
+        columns_to_converters: Callable[[List[str]], Dict[str, FeatureConverter]],
+        connection: Optional[sqlalchemy.ext.asyncio.AsyncConnection] = None,
+    ):
+        try:
+            return await self.async_execute_query_efficient(finalized_query, columns_to_converters, connection)
+        except NotImplementedError:
+            _logger.info(
+                (
+                    "The SQL statement will be executed into SQLAlchemy objects, as the database backend does "
+                    "not support a more efficient execution mechanism."
+                )
+            )
+            pass
+        except UnsupportedEfficientExecutionError as e:
+            log_level = e.log_level
+            _logger.log(log_level, str(e))
+
+        return await self.async_execute_query_inefficient(finalized_query, columns_to_converters, connection)
+
+    async def async_execute_query_inefficient(
+        self,
+        finalized_query: FinalizedChalkQuery,
+        columns_to_converters: Callable[[List[str]], Dict[str, FeatureConverter]],
+        connection: Optional[sqlalchemy.ext.asyncio.AsyncConnection],
+    ):
+        if connection is None:
+            try:
+                eng = self.get_async_engine()
+            except NotImplementedError:
+                return await asyncio.get_running_loop().run_in_executor(
+                    None, self.execute_query_inefficient, finalized_query, columns_to_converters, connection
+                )
+            cnx_ctx = eng.connect()
+        else:
+            cnx_ctx = async_null_context(connection)
+        async with cnx_ctx as cnx:
+            res = await cnx.execute(finalized_query.query, finalized_query.params)
+            desc = res.cursor.description  # type: ignore
+            result_columns: list[str] = [col[0] for col in desc]
+            converters = columns_to_converters(result_columns)
+            data: Dict[str, List[Any]] = {}
+            for v in converters.keys():
+                # Create an entry for the columns, so the pyarrow table will have the correct columns even
+                # if there is no data
+                data[v] = []
+            for row in res.all():
+                for k, v in zip(result_columns, row):
+                    if k not in data:
+                        # We are not interested in this column
+                        continue
+                    data[k].append(converters[k].from_rich_to_primitive(v, missing_value_strategy="default_or_allow"))
+            # Only keep the columns provided by the schema
+            schema = pa.schema([pa.field(k, v.pyarrow_dtype) for (k, v) in converters.items()])
+            return pa.Table.from_pydict(data, schema=schema)
+
     def execute_query_inefficient(
         self,
         finalized_query: FinalizedChalkQuery,
         columns_to_converters: Callable[[List[str]], Dict[str, FeatureConverter]],
         connection: Optional[Connection],
     ):
         with self.get_engine().connect() if connection is None else contextlib.nullcontext(connection) as cnx:
@@ -288,14 +363,22 @@
         self,
         finalized_query: FinalizedChalkQuery,
         columns_to_converters: Callable[[List[str]], Dict[str, FeatureConverter]],
         connection: Optional[Connection],
     ) -> pa.Table:
         raise NotImplementedError()
 
+    async def async_execute_query_efficient(
+        self,
+        finalized_query: FinalizedChalkQuery,
+        columns_to_converters: Callable[[List[str]], Dict[str, FeatureConverter]],
+        connection: Optional[sqlalchemy.ext.asyncio.AsyncConnection],
+    ):
+        raise NotImplementedError()
+
     def compile_query(
         self,
         finalized_query: FinalizedChalkQuery,
         paramstyle: Optional[str] = None,
     ) -> Tuple[str, Sequence[Any], Dict[str, Any]]:
         """Compile a query into a string and the bindparams"""
         dialect = self.local_engine_url().get_dialect()(paramstyle=paramstyle)
@@ -313,63 +396,45 @@
         if extra_args is None:
             return {}
         else:
             extra_args = json.loads(extra_args)
             assert isinstance(extra_args, dict), "ENGINE_ARGUMENTS must be a JSON object"
             return extra_args
 
-    def get_engine(self, additional_engine_args: Optional[Dict[str, Any]] = None) -> Engine:
-        if additional_engine_args is not None:
-            # Deprecating the additional engine args, and instead requiring they are specified when creating the engine,
-            # since otherwise the engine won't be cached
-            # If we need different types of engines for a given SQL source, we should probably add explicit methods
-            # e.g. get_read_engine, get_write_engine, etc...
-            warnings.warn(
-                DeprecationWarning(
-                    (
-                        "The argument `additional_engine_args` is deprecated for the method `SQLSource.get_engine`. "
-                        "Instead, specify the arguments when constructing the SQL source -- "
-                        "e.g. `PostgresSQLSource(engine_args=...)`"
-                    )
-                )
-            )
-
-        if additional_engine_args is None:
-            return self._get_engine_default()
-        else:
-            return self._get_engine_with_args(additional_engine_args)
-
-    def _get_engine_with_args(self, additional_engine_args: Dict[str, Any]) -> Engine:
-        from sqlalchemy.engine import create_engine
-
-        args = dict(self.engine_args)
-        args.update(additional_engine_args)
-
-        return create_engine(**args)
-
-    @functools.lru_cache(None)
-    def _get_engine_default(self) -> Engine:
-        from sqlalchemy.engine import create_engine
-
-        isolation_level = self.engine_args.get("isolation_level")
+    def _check_engine_isolation_level(self):
+        isolation_level = self._engine_args.get("isolation_level")
         if isolation_level == "AUTOCOMMIT":
             warnings.warn(
                 UserWarning(
                     (
                         f"The SQL engine '{self.name}' is being created with the AUTOCOMMIT transaction isolation level, which helps improve "
                         "performance for SELECT statements by avoiding unnecessary transactions. If a different transaction level is needed for an "
                         "individual connection, use the `execution_options` method when retrieving a connection -- e.g. "
                         "`with get_engine().connect().execution_options(isolation_level='REPEATABLE READ') as cnx: ...`. "
                         "For more information, please see "
                         "https://docs.sqlalchemy.org/en/20/core/connections.html#setting-isolation-level-or-dbapi-autocommit-for-a-connection"
                     )
                 )
             )
 
-        return create_engine(**self.engine_args)
+    def get_engine(self) -> Engine:
+        from sqlalchemy.engine import create_engine
+
+        if self._engine is None:
+            self._check_engine_isolation_level()
+            self._engine = create_engine(url=self.local_engine_url(), **self._engine_args)
+        return self._engine
+
+    def get_async_engine(self):
+        from sqlalchemy.ext.asyncio import create_async_engine
+
+        if self._async_engine is None:
+            self._check_engine_isolation_level()
+            self._async_engine = create_async_engine(url=self.async_local_engine_url(), **self._async_engine_args)
+        return self._async_engine
 
     def raw_session(self) -> Session:
         from sqlalchemy.orm import Session
 
         warnings.warn(
             DeprecationWarning(
                 (
```

### Comparing `chalkpy-2.0.2/chalk/sql/_internal/string_chalk_query.py` & `chalkpy-2.0.3/chalk/sql/_internal/string_chalk_query.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/sql/finalized_query.py` & `chalkpy-2.0.3/chalk/sql/finalized_query.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from chalk.features import DataFrame, Feature, FeatureConverter, Features
 from chalk.sql._internal.incremental import IncrementalSettings
 from chalk.sql.protocols import BaseSQLSourceProtocol
 from chalk.utils.missing_dependency import missing_dependency_exception
 from chalk.utils.string import normalize_string_for_matching
 
 if TYPE_CHECKING:
+    import sqlalchemy.ext.asyncio
     from sqlalchemy.engine import Connection
     from sqlalchemy.sql import Select
     from sqlalchemy.sql.elements import TextClause
 
 
 class Finalizer(str, Enum):
     ONE_OR_NONE = "OneOrNone"
@@ -113,67 +114,155 @@
         Returns
         -------
         DataFrame
             A `DataFrame`, if the `.finalizer` is ALL; otherwise, `Features` set.
             If the finalizer is ONE_OR_NONE or FIRST, then the result may be
             `None` if no row was found
         """
-        res = self.execute_to_dataframe(expected_features, connection)
 
-        if self._finalizer in (Finalizer.ONE_OR_NONE, Finalizer.FIRST) and len(res) == 0:
-            return None
-        if self._finalizer in (Finalizer.ONE, Finalizer.ONE_OR_NONE, Finalizer.FIRST):
-            return res.slice(0, 1).to_features()[0]
-        return res
+        pa_table = self.execute_to_pyarrow(expected_features, connection)
+        return self._pa_table_to_res(pa_table)
 
-    def execute_to_pyarrow(
+    async def async_execute(
         self,
         expected_features: Optional[Sequence[Feature]] = None,
-        connection: Optional[Connection] = None,
-    ) -> pa.Table:
-        """Actually execute the query, and return a PyArrow table. Unlike :meth:`.execute`, this method will always keep the
-        results as a PyArrow table, even if the finalizer implies a singleton results (e.g. ONE, ONE_OR_NONE, or FIRST).
+        connection: Optional[Any] = None,
+    ) -> Union[Features, DataFrame, None]:
+        """Actually execute the query to a `DataFrame` or set of features.
+
+        If the finalizer was ONE, ONE_OR_NONE, or FIRST, then a `Features` instance
+        is returned. Otherwise, if the `finalizer` is ALL, then a `DataFrame` instance
+        is returned.
 
         Parameters
         ----------
         expected_features
             The list of expected features for the output, as provided by the resovler in which this query is executed.
             If not specified, the column names as returned by the query will be used to determine the output features.
         connection
-            Execute the query using the supplied connection. If None (the default), then a new connection will be acquired
+            Execute the query using the supplied connection. If `None` (default), a new connection will be acquired
             from the underlying source for the query
 
         Returns
         -------
-        Table
-            A `pa.Table`, even if the result contains 0 or 1 rows.
+        DataFrame
+            A `DataFrame`, if the `.finalizer` is ALL; otherwise, `Features` set.
+            If the finalizer is ONE_OR_NONE or FIRST, then the result may be
+            `None` if no row was found
         """
+
+        pa_table = await self.async_execute_to_pyarrow(expected_features, connection)
+        return self._pa_table_to_res(pa_table)
+
+    def _pa_table_to_res(self, pa_table: pa.Table):
+        try:
+            import polars as pl
+        except ImportError:
+            raise missing_dependency_exception("chalkpy[runtime]")
+        df = pl.from_arrow(pa_table)
+        assert isinstance(df, pl.DataFrame)
+        res = DataFrame(df)
+        if self._finalizer in (Finalizer.ONE_OR_NONE, Finalizer.FIRST) and len(res) == 0:
+            return None
+        if self._finalizer in (Finalizer.ONE, Finalizer.ONE_OR_NONE, Finalizer.FIRST):
+            return res.slice(0, 1).to_features()[0]
+        return res
+
+    def _get_col_to_converter(
+        self,
+        expected_features: Optional[Sequence[Feature]] = None,
+    ):
+        expected_feature_root_fqns = (
+            None if expected_features is None else frozenset(x.root_fqn for x in expected_features)
+        )
+
+        def col_to_converters(column_names: List[str]) -> Dict[str, FeatureConverter]:
+            # First map the column names to determine the feature fqns
+            col_name_mapping = self.get_col_name_mapping(tuple(column_names), expected_feature_root_fqns)
+            return {k: Feature.from_root_fqn(v).converter for (k, v) in col_name_mapping.items()}
+
+        return col_to_converters
+
+    def _check_incremental_settings(self):
         if self.incremental_settings is not None:
             # FIXME: Move the incrementalization logic here, so then the `execute` and `execute_to_dataframe`
             # methods can take the hwm timestamp as a paramater, to allow for direct execution
             warnings.warn(
                 (
                     "This query specified an incremental configuration, which has not been applied. "
                     "This is likely because the resolver is being executed directly. "
                     "The query will be attempted without any high-water-mark timestamp. "
                     "This will attempt to select all data, "
                     "or if the filters depend on the incremental timestamp, "
                     "will result in a query execution error. "
                 )
             )
+
+    def execute_to_pyarrow(
+        self,
+        expected_features: Optional[Sequence[Feature]] = None,
+        connection: Optional[Connection] = None,
+    ) -> pa.Table:
+        """Actually execute the query, and return a PyArrow table. Unlike :meth:`.execute`, this method will always keep the
+        results as a PyArrow table, even if the finalizer implies a singleton results (e.g. ONE, ONE_OR_NONE, or FIRST).
+
+        Parameters
+        ----------
+        expected_features
+            The list of expected features for the output, as provided by the resovler in which this query is executed.
+            If not specified, the column names as returned by the query will be used to determine the output features.
+        connection
+            Execute the query using the supplied connection. If None (the default), then a new connection will be acquired
+            from the underlying source for the query
+
+        Returns
+        -------
+        Table
+            A `pa.Table`, even if the result contains 0 or 1 rows.
+        """
+        self._check_incremental_settings()
+        col_to_converters = self._get_col_to_converter(expected_features)
+
+        pa_table = self.source.execute_query(self, col_to_converters, connection)
+
+        return self._postprocess_table(pa_table, expected_features)
+
+    async def async_execute_to_pyarrow(
+        self,
+        expected_features: Optional[Sequence[Feature]] = None,
+        connection: Optional[sqlalchemy.ext.asyncio.AsyncConnection] = None,
+    ) -> pa.Table:
+        """Actually execute the query, and return a PyArrow table. Unlike :meth:`.execute`, this method will always keep the
+        results as a PyArrow table, even if the finalizer implies a singleton results (e.g. ONE, ONE_OR_NONE, or FIRST).
+
+        Parameters
+        ----------
+        expected_features
+            The list of expected features for the output, as provided by the resovler in which this query is executed.
+            If not specified, the column names as returned by the query will be used to determine the output features.
+        connection
+            Execute the query using the supplied connection. If None (the default), then a new connection will be acquired
+            from the underlying source for the query
+
+        Returns
+        -------
+        Table
+            A `pa.Table`, even if the result contains 0 or 1 rows.
+        """
+        self._check_incremental_settings()
+        col_to_converters = self._get_col_to_converter(expected_features)
+
+        pa_table = await self.source.async_execute_query(self, col_to_converters, connection)
+
+        return self._postprocess_table(pa_table, expected_features)
+
+    def _postprocess_table(self, pa_table: pa.Table, expected_features: Optional[Sequence[Feature]]):
         expected_feature_root_fqns = (
             None if expected_features is None else frozenset(x.root_fqn for x in expected_features)
         )
-
-        def converter_getters(column_names: List[str]) -> Dict[str, FeatureConverter]:
-            # First map the column names to determine the feature fqns
-            col_name_mapping = self.get_col_name_mapping(tuple(column_names), expected_feature_root_fqns)
-            return {k: Feature.from_root_fqn(v).converter for (k, v) in col_name_mapping.items()}
-
-        pa_table = self.source.execute_query(self, converter_getters, connection)
         col_name_mapping = self.get_col_name_mapping(tuple(pa_table.column_names), expected_feature_root_fqns)
         pa_table = pa_table.select(list(col_name_mapping.keys()))
         pa_table = pa_table.rename_columns([col_name_mapping[x] for x in pa_table.column_names])
 
         if self._finalizer == Finalizer.ONE:
             if len(pa_table) != 1:
                 raise ValueError(f"Expected exactly one row; got {len(pa_table)} rows")
```

### Comparing `chalkpy-2.0.2/chalk/sql/protocols.py` & `chalkpy-2.0.3/chalk/sql/protocols.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 
 from chalk.features import DataFrame, Feature, FeatureConverter, Features
 from chalk.sql._internal.incremental import IncrementalSettings
 from chalk.utils.duration import Duration
 
 if TYPE_CHECKING:
     import sqlalchemy
-    from sqlalchemy.engine import URL, Connection
+    import sqlalchemy.ext.asyncio
+    from sqlalchemy.engine import Connection
     from sqlalchemy.orm import Session
 
     from chalk.sql.finalized_query import FinalizedChalkQuery
 
 TTableIngestProtocol = TypeVar("TTableIngestProtocol", bound="TableIngestProtocol")
 
 
@@ -504,14 +505,39 @@
     ) -> pa.Table:
         """Execute a query to a `pa.Table`.
 
         Parameters
         ----------
         finalized_query
             The query to execute
+        columns_to_converters
+            A function that, given the list of column names returned from the database,
+            produces a mapping of columns to converters. Columns not in the resulting dictionary should be ignored.
+        connection
+            A connection to execute the query under. If not specified, then a new connection is acquired.
+
+        Returns
+        -------
+        pa.Table
+            A `pa.Table` containing the results.
+        """
+        ...
+
+    async def async_execute_query(
+        self,
+        finalized_query: FinalizedChalkQuery,
+        columns_to_converters: Callable[[List[str]], Dict[str, FeatureConverter]],
+        connection: Optional[sqlalchemy.ext.asyncio.AsyncConnection] = None,
+    ) -> pa.Table:
+        """Execute a query to a `pa.Table`.
+
+        Parameters
+        ----------
+        finalized_query
+            The query to execute
         columns_to_converters
             A function that, given the list of column names returned from the database,
             produces a mapping of columns to converters. Columns not in the resulting dictionary should be ignored.
         connection
             A connection to execute the query under. If not specified, then a new connection is acquired.
 
         Returns
```

### Comparing `chalkpy-2.0.2/chalk/state.py` & `chalkpy-2.0.3/chalk/state.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/streams/__init__.py` & `chalkpy-2.0.3/chalk/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/streams/_kafka_source.py` & `chalkpy-2.0.3/chalk/streams/_kafka_source.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/streams/_windows.py` & `chalkpy-2.0.3/chalk/streams/_windows.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/streams/types.py` & `chalkpy-2.0.3/chalk/streams/types.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/testing/__init__.py` & `chalkpy-2.0.3/chalk/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/utils/annotation_parsing.py` & `chalkpy-2.0.3/chalk/utils/annotation_parsing.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/utils/collections.py` & `chalkpy-2.0.3/chalk/utils/collections.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/utils/duration.py` & `chalkpy-2.0.3/chalk/utils/duration.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/utils/enum.py` & `chalkpy-2.0.3/chalk/utils/enum.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/utils/log_with_context.py` & `chalkpy-2.0.3/chalk/utils/log_with_context.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/utils/metaprogramming.py` & `chalkpy-2.0.3/chalk/utils/metaprogramming.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/utils/notebook.py` & `chalkpy-2.0.3/chalk/utils/notebook.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/utils/paths.py` & `chalkpy-2.0.3/chalk/utils/paths.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/utils/string.py` & `chalkpy-2.0.3/chalk/utils/string.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalk/utils/stubgen.py` & `chalkpy-2.0.3/chalk/utils/stubgen.py`

 * *Files identical despite different names*

### Comparing `chalkpy-2.0.2/chalkpy.egg-info/SOURCES.txt` & `chalkpy-2.0.3/chalkpy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -617,14 +617,15 @@
 chalk/streams/_kafka_source.py
 chalk/streams/_windows.py
 chalk/streams/base.py
 chalk/streams/types.py
 chalk/testing/__init__.py
 chalk/utils/__init__.py
 chalk/utils/annotation_parsing.py
+chalk/utils/async_helpers.py
 chalk/utils/cached_type_hints.py
 chalk/utils/collection_type.py
 chalk/utils/collections.py
 chalk/utils/constants.py
 chalk/utils/duration.py
 chalk/utils/enum.py
 chalk/utils/environment_parsing.py
```

### Comparing `chalkpy-2.0.2/pyproject.toml` & `chalkpy-2.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     "pre-commit",
     "mypy",
     "pytest",
     "pytest-env",
     "pytest-timeout",
     "pytest-xdist",
     "python-dotenv",
+    "pytest-asyncio",
     "sqlalchemy2-stubs",
     "types-psycopg2",
     "types-pymysql",
     "types-pyyaml",
     "types-requests",
 ]
 
@@ -69,15 +70,15 @@
     "sqlglot>=11.3.2",
     "polars[timezone]==0.17.2",
 ]
 
 
 # SQL-specific
 sql=[
-    "sqlalchemy>=1.4.26,<2",
+    "sqlalchemy[asyncio]>=1.4.26,<2",
     # And the runtime dependencies
     # [[[cog
     # import pathlib, tomli
     # for dep in sorted(set(tomli.loads(pathlib.Path("pyproject.toml").read_text())["project"]["optional-dependencies"]["runtime"])):
     #     print(f'    "{dep}",')
     # ]]]
     "duckdb==0.6.0",
@@ -92,30 +93,31 @@
     # [[[cog
     # import pathlib, tomli
     # for dep in sorted(set(tomli.loads(pathlib.Path("pyproject.toml").read_text())["project"]["optional-dependencies"]["sql"])):
     #     print(f'    "{dep}",')
     # ]]]
     "duckdb==0.6.0",
     "polars[timezone]==0.17.2",
-    "sqlalchemy>=1.4.26,<2",
+    "sqlalchemy[asyncio]>=1.4.26,<2",
     "sqlglot>=11.3.2",
     # [[[end]]]
 ]
 
 postgresql=[
     "psycopg2>=2.9.4,<3",
+    "asyncpg>=0.27.0,<0.28",
     # And the sql dependencies
     # [[[cog
     # import pathlib, tomli
     # for dep in sorted(set(tomli.loads(pathlib.Path("pyproject.toml").read_text())["project"]["optional-dependencies"]["sql"])):
     #     print(f'    "{dep}",')
     # ]]]
     "duckdb==0.6.0",
     "polars[timezone]==0.17.2",
-    "sqlalchemy>=1.4.26,<2",
+    "sqlalchemy[asyncio]>=1.4.26,<2",
     "sqlglot>=11.3.2",
     # [[[end]]]
 ]
 
 snowflake=[
     "snowflake-connector-python>=3,<3.1",
     "snowflake-sqlalchemy>=1.4.2,<1.5",
@@ -123,61 +125,64 @@
     # [[[cog
     # import pathlib, tomli
     # for dep in sorted(set(tomli.loads(pathlib.Path("pyproject.toml").read_text())["project"]["optional-dependencies"]["sql"])):
     #     print(f'    "{dep}",')
     # ]]]
     "duckdb==0.6.0",
     "polars[timezone]==0.17.2",
-    "sqlalchemy>=1.4.26,<2",
+    "sqlalchemy[asyncio]>=1.4.26,<2",
     "sqlglot>=11.3.2",
     # [[[end]]]
 ]
 
 sqlite=[
+    "aiosqlite>=0.19.0,<0.20",
     # And the sql dependencies
     # [[[cog
     # import pathlib, tomli
     # for dep in sorted(set(tomli.loads(pathlib.Path("pyproject.toml").read_text())["project"]["optional-dependencies"]["sql"])):
     #     print(f'    "{dep}",')
     # ]]]
     "duckdb==0.6.0",
     "polars[timezone]==0.17.2",
-    "sqlalchemy>=1.4.26,<2",
+    "sqlalchemy[asyncio]>=1.4.26,<2",
     "sqlglot>=11.3.2",
     # [[[end]]]
 ]
 
 redshift=[
     "sqlalchemy-redshift>=0.8.11,<0.9",
     "redshift_connector>=2.0.909,<2.1",
     # And the postgresql dependencies
     # [[[cog
     # import pathlib, tomli
     # for dep in sorted(set(tomli.loads(pathlib.Path("pyproject.toml").read_text())["project"]["optional-dependencies"]["postgresql"])):
     #     print(f'    "{dep}",')
     # ]]]
+    "asyncpg>=0.27.0,<0.28",
     "duckdb==0.6.0",
     "polars[timezone]==0.17.2",
     "psycopg2>=2.9.4,<3",
-    "sqlalchemy>=1.4.26,<2",
+    "sqlalchemy[asyncio]>=1.4.26,<2",
     "sqlglot>=11.3.2",
     # [[[end]]]
 ]
 
 mysql=[
     "pymysql>=1.0.2,<2",
+    "aiomysql>=0.1.1,<0.2",
     # And the sql dependencies
     # [[[cog
     # import pathlib, tomli
     # for dep in sorted(set(tomli.loads(pathlib.Path("pyproject.toml").read_text())["project"]["optional-dependencies"]["sql"])):
     #     print(f'    "{dep}",')
     # ]]]
     "duckdb==0.6.0",
     "polars[timezone]==0.17.2",
-    "sqlalchemy>=1.4.26,<2",
+    "sqlalchemy[asyncio]>=1.4.26,<2",
     "sqlglot>=11.3.2",
     # [[[end]]]
 ]
 
 all=[
     # "All" includes everything except for dev dependencies
     # [[[cog
@@ -186,24 +191,27 @@
     # final_deps = set()
     # for grp, deps in grps.items():
     #    if grp in ("runtime", "sql", "bigquery", "postgresql", "snowflake", "sqlite", "redshift", "mysql"):
     #        final_deps.update(deps)
     # for dep in sorted(final_deps):
     #     print(f'    "{dep}",')
     # ]]]
+    "aiomysql>=0.1.1,<0.2",
+    "aiosqlite>=0.19.0,<0.20",
+    "asyncpg>=0.27.0,<0.28",
     "duckdb==0.6.0",
     "polars[timezone]==0.17.2",
     "psycopg2>=2.9.4,<3",
     "pymysql>=1.0.2,<2",
     "redshift_connector>=2.0.909,<2.1",
     "snowflake-connector-python>=3,<3.1",
     "snowflake-sqlalchemy>=1.4.2,<1.5",
     "sqlalchemy-bigquery>=1.5.0,<1.7",
     "sqlalchemy-redshift>=0.8.11,<0.9",
-    "sqlalchemy>=1.4.26,<2",
+    "sqlalchemy[asyncio]>=1.4.26,<2",
     "sqlglot>=11.3.2",
     # [[[end]]]
 ]
 
 # Deprecated groups
 polars=[
     # deprecated; should use chalkpy[runtime]
@@ -259,14 +267,15 @@
 env = [
     "CHALK_ALLOW_REGISTRY_UPDATES=1",
     "PYTHONASYNCIODEBUG=1",
     "SQLALCHEMY_WARN_20=1",
 ]
 log_cli = true
 addopts = ""
+asyncio_mode = "auto"
 
 [tool.pyright]
 typeCheckingMode = "basic"
 strictListInference = true
 strictDictionaryInference = true
 strictSetInference = true
 # strictParameterNoneValue
```

