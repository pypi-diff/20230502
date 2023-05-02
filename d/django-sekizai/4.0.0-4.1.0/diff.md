# Comparing `tmp/django-sekizai-4.0.0.tar.gz` & `tmp/django-sekizai-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sekizai-4.0.0.tar", last modified: Tue Jul 26 11:51:05 2022, max compression
+gzip compressed data, was "django-sekizai-4.1.0.tar", last modified: Tue May  2 15:39:11 2023, max compression
```

## Comparing `django-sekizai-4.0.0.tar` & `django-sekizai-4.1.0.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 11:51:05.551805 django-sekizai-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1486 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4484 2022-07-26 11:51:05.551805 django-sekizai-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3256 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 11:51:05.547805 django-sekizai-4.0.0/django_sekizai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4484 2022-07-26 11:51:05.000000 django-sekizai-4.0.0/django_sekizai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1651 2022-07-26 11:51:05.000000 django-sekizai-4.0.0/django_sekizai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-26 11:51:05.000000 django-sekizai-4.0.0/django_sekizai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-26 11:51:05.000000 django-sekizai-4.0.0/django_sekizai.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-07-26 11:51:05.000000 django-sekizai-4.0.0/django_sekizai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-07-26 11:51:05.000000 django-sekizai-4.0.0/django_sekizai.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 11:51:05.547805 django-sekizai-4.0.0/sekizai/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/sekizai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      356 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/sekizai/context.py
--rw-r--r--   0 runner    (1001) docker     (121)      326 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/sekizai/context_processors.py
--rw-r--r--   0 runner    (1001) docker     (121)      616 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/sekizai/data.py
--rw-r--r--   0 runner    (1001) docker     (121)     5375 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/sekizai/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/sekizai/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 11:51:05.547805 django-sekizai-4.0.0/sekizai/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/sekizai/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4518 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/sekizai/templatetags/sekizai_tags.py
--rw-r--r--   0 runner    (1001) docker     (121)      978 2022-07-26 11:51:05.551805 django-sekizai-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1696 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 11:51:05.547805 django-sekizai-4.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 11:51:05.547805 django-sekizai-4.0.0/tests/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/tests/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1280 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/tests/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 11:51:05.547805 django-sekizai-4.0.0/tests/templates/
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/tests/templates/basic.html
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/tests/templates/css.html
--rw-r--r--   0 runner    (1001) docker     (121)      260 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/tests/templates/css2.html
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/tests/templates/easy_base.html
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/tests/templates/easy_inherit.html
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/tests/templates/eat.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 11:51:05.547805 django-sekizai-4.0.0/tests/templates/errors/
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/tests/templates/errors/failadd.html
--rw-r--r--   0 runner    (1001) docker     (121)      137 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/tests/templates/errors/failbase.html
--rw-r--r--   0 runner    (1001) docker     (121)      137 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/tests/templates/errors/failbase2.html
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/tests/templates/errors/failinc.html
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/tests/templates/errors/failrender.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 11:51:05.551805 django-sekizai-4.0.0/tests/templates/inherit/
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/tests/templates/inherit/base.html
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/tests/templates/inherit/baseinc.html
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/tests/templates/inherit/chain.html
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/tests/templates/inherit/extend.html
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/tests/templates/inherit/extinc.html
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/tests/templates/inherit/nullbase.html
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/tests/templates/inherit/nullext.html
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/tests/templates/inherit/spacechain.html
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/tests/templates/inherit/subvarchain.html
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/tests/templates/inherit/super_blocks.html
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/tests/templates/inherit/varchain.html
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/tests/templates/named_end.html
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/tests/templates/namespaces.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 11:51:05.551805 django-sekizai-4.0.0/tests/templates/processors/
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/tests/templates/processors/addtoblock_namespace.html
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/tests/templates/processors/addtoblock_null.html
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/tests/templates/processors/namespace.html
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/tests/templates/processors/null.html
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/tests/templates/unique.html
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/tests/templates/variables.html
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/tests/templates/with_data.html
--rw-r--r--   0 runner    (1001) docker     (121)    14015 2022-07-26 11:50:53.000000 django-sekizai-4.0.0/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:39:11.112875 django-sekizai-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-05-02 15:39:11.112875 django-sekizai-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:39:11.104874 django-sekizai-4.1.0/django_sekizai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-05-02 15:39:11.000000 django-sekizai-4.1.0/django_sekizai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-02 15:39:11.000000 django-sekizai-4.1.0/django_sekizai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:39:11.000000 django-sekizai-4.1.0/django_sekizai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:39:10.000000 django-sekizai-4.1.0/django_sekizai.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-02 15:39:11.000000 django-sekizai-4.1.0/django_sekizai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 15:39:11.000000 django-sekizai-4.1.0/django_sekizai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:39:11.108875 django-sekizai-4.1.0/sekizai/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/sekizai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/sekizai/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/sekizai/context_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/sekizai/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/sekizai/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/sekizai/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:39:11.108875 django-sekizai-4.1.0/sekizai/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/sekizai/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/sekizai/templatetags/sekizai_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-02 15:39:11.112875 django-sekizai-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:39:11.108875 django-sekizai-4.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:39:11.108875 django-sekizai-4.1.0/tests/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/tests/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/tests/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:39:11.108875 django-sekizai-4.1.0/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/tests/templates/basic.html
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/tests/templates/css.html
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/tests/templates/css2.html
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/tests/templates/easy_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/tests/templates/easy_inherit.html
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/tests/templates/eat.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:39:11.108875 django-sekizai-4.1.0/tests/templates/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/tests/templates/errors/failadd.html
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/tests/templates/errors/failbase.html
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/tests/templates/errors/failbase2.html
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/tests/templates/errors/failinc.html
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/tests/templates/errors/failrender.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:39:11.112875 django-sekizai-4.1.0/tests/templates/inherit/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/tests/templates/inherit/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/tests/templates/inherit/baseinc.html
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/tests/templates/inherit/chain.html
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/tests/templates/inherit/extend.html
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/tests/templates/inherit/extinc.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/tests/templates/inherit/nullbase.html
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/tests/templates/inherit/nullext.html
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/tests/templates/inherit/spacechain.html
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/tests/templates/inherit/subvarchain.html
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/tests/templates/inherit/super_blocks.html
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/tests/templates/inherit/varchain.html
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/tests/templates/named_end.html
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/tests/templates/namespaces.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:39:11.112875 django-sekizai-4.1.0/tests/templates/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/tests/templates/processors/addtoblock_namespace.html
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/tests/templates/processors/addtoblock_null.html
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/tests/templates/processors/namespace.html
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/tests/templates/processors/null.html
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/tests/templates/unique.html
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/tests/templates/variables.html
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/tests/templates/with_data.html
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/tests/templates/with_data_basic.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14146 2023-05-02 15:39:00.000000 django-sekizai-4.1.0/tests/test_core.py
```

### Comparing `django-sekizai-4.0.0/LICENSE` & `django-sekizai-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-sekizai-4.0.0/PKG-INFO` & `django-sekizai-4.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sekizai
-Version: 4.0.0
+Version: 4.1.0
 Summary: Django Sekizai
 Home-page: https://github.com/django-cms/django-sekizai
 Author: Jonas Obrist
 Author-email: ojiidotch@gmail.com
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
@@ -14,18 +14,20 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `django-sekizai-4.0.0/README.rst` & `django-sekizai-4.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-sekizai-4.0.0/django_sekizai.egg-info/PKG-INFO` & `django-sekizai-4.1.0/django_sekizai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sekizai
-Version: 4.0.0
+Version: 4.1.0
 Summary: Django Sekizai
 Home-page: https://github.com/django-cms/django-sekizai
 Author: Jonas Obrist
 Author-email: ojiidotch@gmail.com
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
@@ -14,18 +14,20 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `django-sekizai-4.0.0/django_sekizai.egg-info/SOURCES.txt` & `django-sekizai-4.1.0/django_sekizai.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 tests/templates/easy_inherit.html
 tests/templates/eat.html
 tests/templates/named_end.html
 tests/templates/namespaces.html
 tests/templates/unique.html
 tests/templates/variables.html
 tests/templates/with_data.html
+tests/templates/with_data_basic.html
 tests/templates/errors/failadd.html
 tests/templates/errors/failbase.html
 tests/templates/errors/failbase2.html
 tests/templates/errors/failinc.html
 tests/templates/errors/failrender.html
 tests/templates/inherit/base.html
 tests/templates/inherit/baseinc.html
```

### Comparing `django-sekizai-4.0.0/sekizai/data.py` & `django-sekizai-4.1.0/sekizai/data.py`

 * *Files identical despite different names*

### Comparing `django-sekizai-4.0.0/sekizai/helpers.py` & `django-sekizai-4.1.0/sekizai/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,20 +83,20 @@
             _get_nodelist(parent_template),
             extend_node
         )
     return found
 
 
 def _scan_namespaces(nodelist, current_block=None):
-    from sekizai.templatetags.sekizai_tags import RenderBlock
+    from sekizai.templatetags.sekizai_tags import RenderBlock, WithData
     found = []
 
     for node in nodelist:
         # check if this is RenderBlock node
-        if isinstance(node, RenderBlock):
+        if isinstance(node, (RenderBlock, WithData)):
             # resolve it's name against a dummy context
             found.append(node.kwargs['name'].resolve({}))
             found += _scan_namespaces(node.blocks['nodelist'], node)
         # handle {% extends ... %} tags if check_inheritance is True
         elif isinstance(node, ExtendsNode):
             found += _extend_nodelist(node)
         # in block nodes we have to scan for super blocks
```

### Comparing `django-sekizai-4.0.0/sekizai/templatetags/sekizai_tags.py` & `django-sekizai-4.1.0/sekizai/templatetags/sekizai_tags.py`

 * *Files identical despite different names*

### Comparing `django-sekizai-4.0.0/setup.cfg` & `django-sekizai-4.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 4.0.0
+current_version = 4.1.0
 commit = True
 tag = False
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

### Comparing `django-sekizai-4.0.0/setup.py` & `django-sekizai-4.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,30 +17,32 @@
     'License :: OSI Approved :: BSD License',
     'Operating System :: OS Independent',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3 :: Only',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Framework :: Django',
     'Framework :: Django :: 3.2',
     'Framework :: Django :: 4.0',
     'Framework :: Django :: 4.1',
+    'Framework :: Django :: 4.2',
     'Topic :: Internet :: WWW/HTTP',
     'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     'Topic :: Software Development',
     'Topic :: Software Development :: Libraries',
 ]
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.rst").read_text()
 
 setup(
     name='django-sekizai',
-    version='4.0.0',
+    version='4.1.0',
     author='Jonas Obrist',
     author_email='ojiidotch@gmail.com',
     maintainer='Django CMS Association and contributors',
     maintainer_email='info@django-cms.org',
     url='https://github.com/django-cms/django-sekizai',
     license='BSD-3-Clause',
     description='Django Sekizai',
```

### Comparing `django-sekizai-4.0.0/tests/settings.py` & `django-sekizai-4.1.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-sekizai-4.0.0/tests/test_core.py` & `django-sekizai-4.1.0/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -375,14 +375,17 @@
 
 
 class HelperTests(TestCase):
 
     def test_validate_template_js_css(self):
         self.assertTrue(validate_template('basic.html', ['js', 'css']))
 
+    def test_validate_template_with_data(self):
+        self.assertTrue(validate_template('with_data_basic.html', ['js', 'css']))
+
     def test_validate_template_js(self):
         self.assertTrue(validate_template('basic.html', ['js']))
 
     def test_validate_template_css(self):
         self.assertTrue(validate_template('basic.html', ['css']))
 
     def test_validate_template_empty(self):
```

