# Comparing `tmp/ruamel.yaml-0.9.7.tar.gz` & `tmp/ruamel.yaml-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ruamel.yaml-0.9.7.tar", last modified: Sat Jun 13 08:00:36 2015, max compression
+gzip compressed data, was "dist/ruamel.yaml-0.9.8.tar", last modified: Thu Jun 18 13:31:38 2015, max compression
```

## Comparing `ruamel.yaml-0.9.7.tar` & `ruamel.yaml-0.9.8.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 anthon    (1001) users      (100)        0 2015-06-13 08:00:36.000000 ruamel.yaml-0.9.7/
--rw-rw-r--   0 anthon    (1001) users      (100)    11257 2015-06-13 08:00:36.000000 ruamel.yaml-0.9.7/PKG-INFO
--rw-rw-r--   0 anthon    (1001) users      (100)     3360 2015-04-18 18:21:04.000000 ruamel.yaml-0.9.7/CHANGES
--rw-rw-r--   0 anthon    (1001) users      (100)     7156 2015-06-05 07:34:08.000000 ruamel.yaml-0.9.7/setup.py
--rw-r--r--   0 anthon    (1001) users      (100)     1072 2014-11-23 15:33:58.000000 ruamel.yaml-0.9.7/LICENSE
--rw-rw-r--   0 anthon    (1001) users      (100)     8110 2015-06-13 07:38:45.000000 ruamel.yaml-0.9.7/README.rst
-drwxrwxr-x   0 anthon    (1001) users      (100)        0 2015-06-13 08:00:36.000000 ruamel.yaml-0.9.7/ext/
--rw-rw-r--   0 anthon    (1001) users      (100)  1012394 2014-11-17 10:05:04.000000 ruamel.yaml-0.9.7/ext/_yaml.c
--rw-rw-r--   0 anthon    (1001) users      (100)     9121 2014-11-17 09:38:59.000000 ruamel.yaml-0.9.7/ext/_yaml.pxd
--rw-rw-r--   0 anthon    (1001) users      (100)      476 2014-11-17 09:38:59.000000 ruamel.yaml-0.9.7/ext/_yaml.h
--rw-rw-r--   0 anthon    (1001) users      (100)    64737 2014-11-17 09:38:59.000000 ruamel.yaml-0.9.7/ext/_yaml.pyx
-drwxrwxr-x   0 anthon    (1001) users      (100)        0 2015-06-13 08:00:36.000000 ruamel.yaml-0.9.7/ruamel.yaml.egg-info/
--rw-r--r--   0 anthon    (1001) users      (100)        7 2015-06-13 08:00:36.000000 ruamel.yaml-0.9.7/ruamel.yaml.egg-info/namespace_packages.txt
--rw-r--r--   0 anthon    (1001) users      (100)     1051 2015-06-13 08:00:36.000000 ruamel.yaml-0.9.7/ruamel.yaml.egg-info/SOURCES.txt
--rw-r--r--   0 anthon    (1001) users      (100)    11257 2015-06-13 08:00:36.000000 ruamel.yaml-0.9.7/ruamel.yaml.egg-info/PKG-INFO
--rw-r--r--   0 anthon    (1001) users      (100)       13 2015-06-13 08:00:36.000000 ruamel.yaml-0.9.7/ruamel.yaml.egg-info/top_level.txt
--rw-r--r--   0 anthon    (1001) users      (100)       58 2015-06-13 08:00:36.000000 ruamel.yaml-0.9.7/ruamel.yaml.egg-info/requires.txt
--rw-r--r--   0 anthon    (1001) users      (100)       43 2015-06-13 08:00:36.000000 ruamel.yaml-0.9.7/ruamel.yaml.egg-info/entry_points.txt
--rw-r--r--   0 anthon    (1001) users      (100)        1 2015-06-13 08:00:36.000000 ruamel.yaml-0.9.7/ruamel.yaml.egg-info/dependency_links.txt
-drwxrwxr-x   0 anthon    (1001) users      (100)        0 2015-06-13 08:00:36.000000 ruamel.yaml-0.9.7/py/
--rw-rw-r--   0 anthon    (1001) users      (100)      402 2015-03-11 07:49:59.000000 ruamel.yaml-0.9.7/py/scalarstring.py
--rw-rw-r--   0 anthon    (1001) users      (100)    37947 2015-06-05 19:25:49.000000 ruamel.yaml-0.9.7/py/constructor.py
--rw-rw-r--   0 anthon    (1001) users      (100)     1969 2015-03-10 10:38:46.000000 ruamel.yaml-0.9.7/py/compat.py
--rw-rw-r--   0 anthon    (1001) users      (100)    47326 2015-05-29 07:37:56.000000 ruamel.yaml-0.9.7/py/emitter.py
--rw-rw-r--   0 anthon    (1001) users      (100)     6311 2015-04-18 18:09:09.000000 ruamel.yaml-0.9.7/py/composer.py
--rw-rw-r--   0 anthon    (1001) users      (100)     2893 2015-03-26 09:19:38.000000 ruamel.yaml-0.9.7/py/events.py
--rw-rw-r--   0 anthon    (1001) users      (100)    29949 2015-06-08 10:26:52.000000 ruamel.yaml-0.9.7/py/representer.py
--rw-rw-r--   0 anthon    (1001) users      (100)     1247 2015-06-13 07:29:36.000000 ruamel.yaml-0.9.7/py/__init__.py
--rw-rw-r--   0 anthon    (1001) users      (100)    28165 2015-04-18 18:09:09.000000 ruamel.yaml-0.9.7/py/parser.py
--rw-r--r--   0 anthon    (1001) users      (100)     3651 2014-11-22 17:11:54.000000 ruamel.yaml-0.9.7/py/cyaml.py
--rw-r--r--   0 anthon    (1001) users      (100)     7357 2014-11-22 17:11:54.000000 ruamel.yaml-0.9.7/py/reader.py
--rw-r--r--   0 anthon    (1001) users      (100)     2638 2014-11-22 17:11:54.000000 ruamel.yaml-0.9.7/py/error.py
--rw-rw-r--   0 anthon    (1001) users      (100)     1162 2015-03-10 10:38:31.000000 ruamel.yaml-0.9.7/py/configobjwalker.py
--rw-r--r--   0 anthon    (1001) users      (100)     4101 2014-11-22 17:11:54.000000 ruamel.yaml-0.9.7/py/dumper.py
--rw-r--r--   0 anthon    (1001) users      (100)     2525 2015-03-10 22:07:35.000000 ruamel.yaml-0.9.7/py/nodes.py
--rw-r--r--   0 anthon    (1001) users      (100)     8860 2015-05-27 10:15:33.000000 ruamel.yaml-0.9.7/py/resolver.py
--rw-r--r--   0 anthon    (1001) users      (100)     5772 2015-03-29 10:16:01.000000 ruamel.yaml-0.9.7/py/serializer.py
--rw-rw-r--   0 anthon    (1001) users      (100)    16879 2015-06-08 11:17:00.000000 ruamel.yaml-0.9.7/py/yaml.py
--rw-r--r--   0 anthon    (1001) users      (100)     1584 2014-11-22 17:34:36.000000 ruamel.yaml-0.9.7/py/loader.py
--rw-rw-r--   0 anthon    (1001) users      (100)     9397 2015-06-13 07:28:21.000000 ruamel.yaml-0.9.7/py/comments.py
--rw-r--r--   0 anthon    (1001) users      (100)    58633 2015-03-29 08:16:39.000000 ruamel.yaml-0.9.7/py/scanner.py
--rw-r--r--   0 anthon    (1001) users      (100)     4519 2015-03-29 11:16:54.000000 ruamel.yaml-0.9.7/py/tokens.py
-drwxrwxr-x   0 anthon    (1001) users      (100)        0 2015-06-13 08:00:36.000000 ruamel.yaml-0.9.7/py/convert/
--rw-rw-r--   0 anthon    (1001) users      (100)     3638 2015-06-02 09:51:05.000000 ruamel.yaml-0.9.7/py/convert/html.py
--rw-rw-r--   0 anthon    (1001) users      (100)        0 2015-06-02 07:07:09.000000 ruamel.yaml-0.9.7/py/convert/__init__.py
--rw-rw-r--   0 anthon    (1001) users      (100)     1291 2015-06-04 11:44:24.000000 ruamel.yaml-0.9.7/py/convert/from_csv.py
--rw-rw-r--   0 anthon    (1001) users      (100)    10638 2015-06-02 09:18:28.000000 ruamel.yaml-0.9.7/py/main.py
--rw-rw-r--   0 anthon    (1001) users      (100)       59 2015-06-13 08:00:36.000000 ruamel.yaml-0.9.7/setup.cfg
-drwxrwxr-x   0 anthon    (1001) users      (100)        0 2015-06-13 08:00:36.000000 ruamel.yaml-0.9.7/test/
--rw-rw-r--   0 anthon    (1001) users      (100)     6178 2015-06-05 06:46:39.000000 ruamel.yaml-0.9.7/test/test_util.py
--rw-rw-r--   0 anthon    (1001) users      (100)     2163 2015-03-29 12:06:45.000000 ruamel.yaml-0.9.7/test/test_indentation.py
--rw-rw-r--   0 anthon    (1001) users      (100)     2432 2015-03-11 08:48:33.000000 ruamel.yaml-0.9.7/test/test_string.py
--rw-rw-r--   0 anthon    (1001) users      (100)      618 2014-11-24 09:06:12.000000 ruamel.yaml-0.9.7/test/test_z_data.py
--rw-rw-r--   0 anthon    (1001) users      (100)     1543 2015-04-18 17:48:19.000000 ruamel.yaml-0.9.7/test/test_line_col.py
--rw-rw-r--   0 anthon    (1001) users      (100)     5435 2015-06-13 07:56:53.000000 ruamel.yaml-0.9.7/test/test_comments.py
--rw-rw-r--   0 anthon    (1001) users      (100)     1336 2015-05-27 10:17:02.000000 ruamel.yaml-0.9.7/test/test_json_numbers.py
--rw-rw-r--   0 anthon    (1001) users      (100)     1745 2014-11-25 13:38:50.000000 ruamel.yaml-0.9.7/test/test_yaml.py
--rw-rw-r--   0 anthon    (1001) users      (100)     2347 2015-06-02 06:43:24.000000 ruamel.yaml-0.9.7/test/test_utiltohtml.py
--rw-rw-r--   0 anthon    (1001) users      (100)      932 2014-11-22 17:27:08.000000 ruamel.yaml-0.9.7/test/test_a_dedent.py
--rw-rw-r--   0 anthon    (1001) users      (100)     1667 2015-06-02 10:12:04.000000 ruamel.yaml-0.9.7/test/test_convert.py
--rw-rw-r--   0 anthon    (1001) users      (100)     5496 2015-04-15 08:21:11.000000 ruamel.yaml-0.9.7/test/test_comment_manipulation.py
--rw-rw-r--   0 anthon    (1001) users      (100)     1795 2014-11-24 08:00:21.000000 ruamel.yaml-0.9.7/test/test_program_config.py
--rw-rw-r--   0 anthon    (1001) users      (100)       68 2014-11-23 15:09:32.000000 ruamel.yaml-0.9.7/MANIFEST.in
+drwxrwxr-x   0 anthon    (1001) users      (100)        0 2015-06-18 13:31:38.000000 ruamel.yaml-0.9.8/
+-rw-rw-r--   0 anthon    (1001) users      (100)    11257 2015-06-18 13:31:38.000000 ruamel.yaml-0.9.8/PKG-INFO
+-rw-rw-r--   0 anthon    (1001) users      (100)     3360 2015-04-18 18:21:04.000000 ruamel.yaml-0.9.8/CHANGES
+-rw-rw-r--   0 anthon    (1001) users      (100)     7156 2015-06-05 07:34:08.000000 ruamel.yaml-0.9.8/setup.py
+-rw-r--r--   0 anthon    (1001) users      (100)     1072 2014-11-23 15:33:58.000000 ruamel.yaml-0.9.8/LICENSE
+-rw-rw-r--   0 anthon    (1001) users      (100)     8110 2015-06-13 07:38:45.000000 ruamel.yaml-0.9.8/README.rst
+drwxrwxr-x   0 anthon    (1001) users      (100)        0 2015-06-18 13:31:38.000000 ruamel.yaml-0.9.8/ext/
+-rw-rw-r--   0 anthon    (1001) users      (100)  1012394 2014-11-17 10:05:04.000000 ruamel.yaml-0.9.8/ext/_yaml.c
+-rw-rw-r--   0 anthon    (1001) users      (100)     9121 2014-11-17 09:38:59.000000 ruamel.yaml-0.9.8/ext/_yaml.pxd
+-rw-rw-r--   0 anthon    (1001) users      (100)      476 2014-11-17 09:38:59.000000 ruamel.yaml-0.9.8/ext/_yaml.h
+-rw-rw-r--   0 anthon    (1001) users      (100)    64737 2014-11-17 09:38:59.000000 ruamel.yaml-0.9.8/ext/_yaml.pyx
+drwxrwxr-x   0 anthon    (1001) users      (100)        0 2015-06-18 13:31:38.000000 ruamel.yaml-0.9.8/ruamel.yaml.egg-info/
+-rw-r--r--   0 anthon    (1001) users      (100)        7 2015-06-18 13:31:38.000000 ruamel.yaml-0.9.8/ruamel.yaml.egg-info/namespace_packages.txt
+-rw-r--r--   0 anthon    (1001) users      (100)     1051 2015-06-18 13:31:38.000000 ruamel.yaml-0.9.8/ruamel.yaml.egg-info/SOURCES.txt
+-rw-r--r--   0 anthon    (1001) users      (100)    11257 2015-06-18 13:31:38.000000 ruamel.yaml-0.9.8/ruamel.yaml.egg-info/PKG-INFO
+-rw-r--r--   0 anthon    (1001) users      (100)       13 2015-06-18 13:31:38.000000 ruamel.yaml-0.9.8/ruamel.yaml.egg-info/top_level.txt
+-rw-r--r--   0 anthon    (1001) users      (100)       58 2015-06-18 13:31:38.000000 ruamel.yaml-0.9.8/ruamel.yaml.egg-info/requires.txt
+-rw-r--r--   0 anthon    (1001) users      (100)       43 2015-06-18 13:31:38.000000 ruamel.yaml-0.9.8/ruamel.yaml.egg-info/entry_points.txt
+-rw-r--r--   0 anthon    (1001) users      (100)        1 2015-06-18 13:31:38.000000 ruamel.yaml-0.9.8/ruamel.yaml.egg-info/dependency_links.txt
+drwxrwxr-x   0 anthon    (1001) users      (100)        0 2015-06-18 13:31:38.000000 ruamel.yaml-0.9.8/py/
+-rw-rw-r--   0 anthon    (1001) users      (100)      402 2015-03-11 07:49:59.000000 ruamel.yaml-0.9.8/py/scalarstring.py
+-rw-rw-r--   0 anthon    (1001) users      (100)    37947 2015-06-05 19:25:49.000000 ruamel.yaml-0.9.8/py/constructor.py
+-rw-rw-r--   0 anthon    (1001) users      (100)     1969 2015-03-10 10:38:46.000000 ruamel.yaml-0.9.8/py/compat.py
+-rw-rw-r--   0 anthon    (1001) users      (100)    47326 2015-05-29 07:37:56.000000 ruamel.yaml-0.9.8/py/emitter.py
+-rw-rw-r--   0 anthon    (1001) users      (100)     6311 2015-04-18 18:09:09.000000 ruamel.yaml-0.9.8/py/composer.py
+-rw-rw-r--   0 anthon    (1001) users      (100)     2893 2015-03-26 09:19:38.000000 ruamel.yaml-0.9.8/py/events.py
+-rw-rw-r--   0 anthon    (1001) users      (100)    29949 2015-06-08 10:26:52.000000 ruamel.yaml-0.9.8/py/representer.py
+-rw-rw-r--   0 anthon    (1001) users      (100)     1247 2015-06-18 13:27:00.000000 ruamel.yaml-0.9.8/py/__init__.py
+-rw-rw-r--   0 anthon    (1001) users      (100)    28165 2015-04-18 18:09:09.000000 ruamel.yaml-0.9.8/py/parser.py
+-rw-r--r--   0 anthon    (1001) users      (100)     3651 2014-11-22 17:11:54.000000 ruamel.yaml-0.9.8/py/cyaml.py
+-rw-r--r--   0 anthon    (1001) users      (100)     7357 2014-11-22 17:11:54.000000 ruamel.yaml-0.9.8/py/reader.py
+-rw-r--r--   0 anthon    (1001) users      (100)     2638 2014-11-22 17:11:54.000000 ruamel.yaml-0.9.8/py/error.py
+-rw-rw-r--   0 anthon    (1001) users      (100)     1162 2015-03-10 10:38:31.000000 ruamel.yaml-0.9.8/py/configobjwalker.py
+-rw-r--r--   0 anthon    (1001) users      (100)     4101 2014-11-22 17:11:54.000000 ruamel.yaml-0.9.8/py/dumper.py
+-rw-r--r--   0 anthon    (1001) users      (100)     2525 2015-03-10 22:07:35.000000 ruamel.yaml-0.9.8/py/nodes.py
+-rw-r--r--   0 anthon    (1001) users      (100)     8860 2015-05-27 10:15:33.000000 ruamel.yaml-0.9.8/py/resolver.py
+-rw-r--r--   0 anthon    (1001) users      (100)     5772 2015-03-29 10:16:01.000000 ruamel.yaml-0.9.8/py/serializer.py
+-rw-rw-r--   0 anthon    (1001) users      (100)    17104 2015-06-18 13:24:06.000000 ruamel.yaml-0.9.8/py/yaml.py
+-rw-r--r--   0 anthon    (1001) users      (100)     1584 2014-11-22 17:34:36.000000 ruamel.yaml-0.9.8/py/loader.py
+-rw-rw-r--   0 anthon    (1001) users      (100)     9397 2015-06-13 07:28:21.000000 ruamel.yaml-0.9.8/py/comments.py
+-rw-r--r--   0 anthon    (1001) users      (100)    58633 2015-03-29 08:16:39.000000 ruamel.yaml-0.9.8/py/scanner.py
+-rw-r--r--   0 anthon    (1001) users      (100)     4519 2015-03-29 11:16:54.000000 ruamel.yaml-0.9.8/py/tokens.py
+drwxrwxr-x   0 anthon    (1001) users      (100)        0 2015-06-18 13:31:38.000000 ruamel.yaml-0.9.8/py/convert/
+-rw-rw-r--   0 anthon    (1001) users      (100)     3638 2015-06-02 09:51:05.000000 ruamel.yaml-0.9.8/py/convert/html.py
+-rw-rw-r--   0 anthon    (1001) users      (100)        0 2015-06-02 07:07:09.000000 ruamel.yaml-0.9.8/py/convert/__init__.py
+-rw-rw-r--   0 anthon    (1001) users      (100)     1291 2015-06-04 11:44:24.000000 ruamel.yaml-0.9.8/py/convert/from_csv.py
+-rw-rw-r--   0 anthon    (1001) users      (100)    10638 2015-06-02 09:18:28.000000 ruamel.yaml-0.9.8/py/main.py
+-rw-rw-r--   0 anthon    (1001) users      (100)       59 2015-06-18 13:31:38.000000 ruamel.yaml-0.9.8/setup.cfg
+drwxrwxr-x   0 anthon    (1001) users      (100)        0 2015-06-18 13:31:38.000000 ruamel.yaml-0.9.8/test/
+-rw-rw-r--   0 anthon    (1001) users      (100)     6178 2015-06-05 06:46:39.000000 ruamel.yaml-0.9.8/test/test_util.py
+-rw-rw-r--   0 anthon    (1001) users      (100)     2163 2015-03-29 12:06:45.000000 ruamel.yaml-0.9.8/test/test_indentation.py
+-rw-rw-r--   0 anthon    (1001) users      (100)     2432 2015-03-11 08:48:33.000000 ruamel.yaml-0.9.8/test/test_string.py
+-rw-rw-r--   0 anthon    (1001) users      (100)      618 2014-11-24 09:06:12.000000 ruamel.yaml-0.9.8/test/test_z_data.py
+-rw-rw-r--   0 anthon    (1001) users      (100)     1543 2015-04-18 17:48:19.000000 ruamel.yaml-0.9.8/test/test_line_col.py
+-rw-rw-r--   0 anthon    (1001) users      (100)     5435 2015-06-13 07:56:53.000000 ruamel.yaml-0.9.8/test/test_comments.py
+-rw-rw-r--   0 anthon    (1001) users      (100)     1336 2015-05-27 10:17:02.000000 ruamel.yaml-0.9.8/test/test_json_numbers.py
+-rw-rw-r--   0 anthon    (1001) users      (100)     1745 2014-11-25 13:38:50.000000 ruamel.yaml-0.9.8/test/test_yaml.py
+-rw-rw-r--   0 anthon    (1001) users      (100)     2347 2015-06-02 06:43:24.000000 ruamel.yaml-0.9.8/test/test_utiltohtml.py
+-rw-rw-r--   0 anthon    (1001) users      (100)      932 2014-11-22 17:27:08.000000 ruamel.yaml-0.9.8/test/test_a_dedent.py
+-rw-rw-r--   0 anthon    (1001) users      (100)     1667 2015-06-02 10:12:04.000000 ruamel.yaml-0.9.8/test/test_convert.py
+-rw-rw-r--   0 anthon    (1001) users      (100)     5496 2015-04-15 08:21:11.000000 ruamel.yaml-0.9.8/test/test_comment_manipulation.py
+-rw-rw-r--   0 anthon    (1001) users      (100)     1795 2014-11-24 08:00:21.000000 ruamel.yaml-0.9.8/test/test_program_config.py
+-rw-rw-r--   0 anthon    (1001) users      (100)       68 2014-11-23 15:09:32.000000 ruamel.yaml-0.9.8/MANIFEST.in
```

### Comparing `ruamel.yaml-0.9.7/PKG-INFO` & `ruamel.yaml-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ruamel.yaml
-Version: 0.9.7
+Version: 0.9.8
 Summary: ruamel.yaml is a YAML parser/emitter that supports roundtrip preservation of comments, seq/map flow style, and map key order
 Home-page: https://bitbucket.org/ruamel/yaml
 Author: Anthon van der Neut
 Author-email: a.van.der.neut@ruamel.eu
 License: MIT license
 Description: 
         ruamel.yaml
```

### Comparing `ruamel.yaml-0.9.7/CHANGES` & `ruamel.yaml-0.9.8/CHANGES`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/setup.py` & `ruamel.yaml-0.9.8/setup.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/LICENSE` & `ruamel.yaml-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/README.rst` & `ruamel.yaml-0.9.8/README.rst`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/ext/_yaml.c` & `ruamel.yaml-0.9.8/ext/_yaml.c`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/ext/_yaml.pxd` & `ruamel.yaml-0.9.8/ext/_yaml.pxd`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/ext/_yaml.pyx` & `ruamel.yaml-0.9.8/ext/_yaml.pyx`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/ruamel.yaml.egg-info/SOURCES.txt` & `ruamel.yaml-0.9.8/ruamel.yaml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/ruamel.yaml.egg-info/PKG-INFO` & `ruamel.yaml-0.9.8/ruamel.yaml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ruamel.yaml
-Version: 0.9.7
+Version: 0.9.8
 Summary: ruamel.yaml is a YAML parser/emitter that supports roundtrip preservation of comments, seq/map flow style, and map key order
 Home-page: https://bitbucket.org/ruamel/yaml
 Author: Anthon van der Neut
 Author-email: a.van.der.neut@ruamel.eu
 License: MIT license
 Description: 
         ruamel.yaml
```

### Comparing `ruamel.yaml-0.9.7/py/constructor.py` & `ruamel.yaml-0.9.8/py/constructor.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/py/compat.py` & `ruamel.yaml-0.9.8/py/compat.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/py/emitter.py` & `ruamel.yaml-0.9.8/py/emitter.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/py/composer.py` & `ruamel.yaml-0.9.8/py/composer.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/py/events.py` & `ruamel.yaml-0.9.8/py/events.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/py/representer.py` & `ruamel.yaml-0.9.8/py/representer.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/py/__init__.py` & `ruamel.yaml-0.9.8/py/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         if first_letter in 'abcr':
             ret_val += 'rc' if first_letter == 'r' else first_letter
         elif first_letter in 'pd':
             ret_val += '.post' if first_letter == 'p' else '.dev'
     return ret_val
 
 
-version_info = (0, 9, 7)
+version_info = (0, 9, 8)
 __version__ = _convert_version(version_info)
 
 del _convert_version
 
 try:
     from .cyaml import *
     __with_libyaml__ = True
```

### Comparing `ruamel.yaml-0.9.7/py/parser.py` & `ruamel.yaml-0.9.8/py/parser.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/py/cyaml.py` & `ruamel.yaml-0.9.8/py/cyaml.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/py/reader.py` & `ruamel.yaml-0.9.8/py/reader.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/py/error.py` & `ruamel.yaml-0.9.8/py/error.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/py/configobjwalker.py` & `ruamel.yaml-0.9.8/py/configobjwalker.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/py/dumper.py` & `ruamel.yaml-0.9.8/py/dumper.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/py/nodes.py` & `ruamel.yaml-0.9.8/py/nodes.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/py/resolver.py` & `ruamel.yaml-0.9.8/py/resolver.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/py/serializer.py` & `ruamel.yaml-0.9.8/py/serializer.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/py/yaml.py` & `ruamel.yaml-0.9.8/py/yaml.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,17 @@
         except ImportError:
             print("to convert from .ini you need to install configobj:")
             print("  pip install configobj:")
             sys.exit(1)
         errors = 0
         doc = []
         cfg = ConfigObj(open(self._args.file))
+        if self._args.test:
+            print(ruamel.yaml.dump(cfg))
+            return
         for line in configobj_walker(cfg):
             doc.append(line)
         joined = '\n'.join(doc)
         rto = self.round_trip_single(joined)
         if self._args.basename:
             out_fn = os.path.splitext(self._args.file)[0] + '.yaml'
             if self._args.verbose > 0:
@@ -213,15 +216,18 @@
         # test end
 
     def from_json(self):
         # use roundtrip to preserver order
         errors = 0
         docs = []
         for file_name in self._args.file:
-            inp = open(file_name).read()
+            if file_name == '-':
+                inp = sys.stdin.read()
+            else:
+                inp = open(file_name).read()
             loader = ruamel.yaml.Loader # RoundTripLoader
             docs.append(ruamel.yaml.load(inp, loader))
         dumper = ruamel.yaml.RoundTripDumper
         print(ruamel.yaml.dump_all(
             docs, Dumper=dumper,
             default_flow_style=self._args.flow))
         return 1 if errors else 0
@@ -445,14 +451,15 @@
         aliases=['from-ini'],
         help='convert .ini/config to block YAML',
         description='convert .ini/config to block YAML',
     )
     @option('--basename', '-b', action='store_true',
             help='re-use basename of file for .yaml file, instead of writing'
             ' to stdout')
+    @option('--test', action='store_true')
     @option('file')
     def ini(self):
         return self._yaml.from_ini()
 
     @sub_parser(
         #aliases=['to-html'],
         help='convert YAML to html tables',
```

### Comparing `ruamel.yaml-0.9.7/py/loader.py` & `ruamel.yaml-0.9.8/py/loader.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/py/comments.py` & `ruamel.yaml-0.9.8/py/comments.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/py/scanner.py` & `ruamel.yaml-0.9.8/py/scanner.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/py/tokens.py` & `ruamel.yaml-0.9.8/py/tokens.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/py/convert/html.py` & `ruamel.yaml-0.9.8/py/convert/html.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/py/convert/from_csv.py` & `ruamel.yaml-0.9.8/py/convert/from_csv.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/py/main.py` & `ruamel.yaml-0.9.8/py/main.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/test/test_util.py` & `ruamel.yaml-0.9.8/test/test_util.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/test/test_indentation.py` & `ruamel.yaml-0.9.8/test/test_indentation.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/test/test_string.py` & `ruamel.yaml-0.9.8/test/test_string.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/test/test_z_data.py` & `ruamel.yaml-0.9.8/test/test_z_data.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/test/test_line_col.py` & `ruamel.yaml-0.9.8/test/test_line_col.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/test/test_comments.py` & `ruamel.yaml-0.9.8/test/test_comments.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/test/test_json_numbers.py` & `ruamel.yaml-0.9.8/test/test_json_numbers.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/test/test_yaml.py` & `ruamel.yaml-0.9.8/test/test_yaml.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/test/test_utiltohtml.py` & `ruamel.yaml-0.9.8/test/test_utiltohtml.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/test/test_a_dedent.py` & `ruamel.yaml-0.9.8/test/test_a_dedent.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/test/test_convert.py` & `ruamel.yaml-0.9.8/test/test_convert.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/test/test_comment_manipulation.py` & `ruamel.yaml-0.9.8/test/test_comment_manipulation.py`

 * *Files identical despite different names*

### Comparing `ruamel.yaml-0.9.7/test/test_program_config.py` & `ruamel.yaml-0.9.8/test/test_program_config.py`

 * *Files identical despite different names*

