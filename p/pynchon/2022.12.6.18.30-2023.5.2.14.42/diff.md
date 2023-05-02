# Comparing `tmp/pynchon-2022.12.6.18.30.tar.gz` & `tmp/pynchon-2023.5.2.14.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynchon-2022.12.6.18.30.tar", last modified: Tue Dec  6 23:30:00 2022, max compression
+gzip compressed data, was "pynchon-2023.5.2.14.42.tar", last modified: Tue May  2 18:42:12 2023, max compression
```

## Comparing `pynchon-2022.12.6.18.30.tar` & `pynchon-2023.5.2.14.42.tar`

### file list

```diff
@@ -1,41 +1,169 @@
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2022-12-06 23:30:00.332284 pynchon-2022.12.6.18.30/
--rw-rw-r--   0 matt      (1000) matt      (1000)       50 2022-10-31 17:10:29.000000 pynchon-2022.12.6.18.30/MANIFEST.in
--rw-rw-r--   0 matt      (1000) matt      (1000)      737 2022-12-06 23:30:00.332284 pynchon-2022.12.6.18.30/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)     3973 2022-11-14 18:55:02.000000 pynchon-2022.12.6.18.30/README.md
--rw-rw-r--   0 matt      (1000) matt      (1000)     1387 2022-12-06 23:30:00.336284 pynchon-2022.12.6.18.30/setup.cfg
--rw-rw-r--   0 matt      (1000) matt      (1000)      730 2022-10-31 16:56:45.000000 pynchon-2022.12.6.18.30/setup.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2022-12-06 23:30:00.332284 pynchon-2022.12.6.18.30/src/
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2022-12-06 23:30:00.332284 pynchon-2022.12.6.18.30/src/pynchon/
--rw-rw-r--   0 matt      (1000) matt      (1000)     1692 2022-10-31 19:56:37.000000 pynchon-2022.12.6.18.30/src/pynchon/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)       78 2022-12-06 23:29:57.000000 pynchon-2022.12.6.18.30/src/pynchon/_version.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3438 2022-10-31 19:53:26.000000 pynchon-2022.12.6.18.30/src/pynchon/annotate.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2022-12-06 23:30:00.332284 pynchon-2022.12.6.18.30/src/pynchon/bin/
--rw-rw-r--   0 matt      (1000) matt      (1000)       98 2022-12-06 23:29:33.000000 pynchon-2022.12.6.18.30/src/pynchon/bin/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1191 2022-12-06 23:23:23.000000 pynchon-2022.12.6.18.30/src/pynchon/bin/api.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3078 2022-12-06 23:29:33.000000 pynchon-2022.12.6.18.30/src/pynchon/bin/cli.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     4164 2022-12-06 23:29:33.000000 pynchon-2022.12.6.18.30/src/pynchon/bin/common.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1208 2022-12-06 23:29:42.000000 pynchon-2022.12.6.18.30/src/pynchon/bin/groups.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1547 2022-12-06 23:29:33.000000 pynchon-2022.12.6.18.30/src/pynchon/bin/options.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1126 2022-11-01 16:35:39.000000 pynchon-2022.12.6.18.30/src/pynchon/bin/project.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     5125 2022-12-06 23:24:03.000000 pynchon-2022.12.6.18.30/src/pynchon/bin/render.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2022-12-06 23:30:00.332284 pynchon-2022.12.6.18.30/src/pynchon/templates/
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2022-12-06 23:30:00.332284 pynchon-2022.12.6.18.30/src/pynchon/templates/api/
--rw-rw-r--   0 matt      (1000) matt      (1000)       34 2022-10-31 23:55:47.000000 pynchon-2022.12.6.18.30/src/pynchon/templates/api/TOC.md.j2
--rw-rw-r--   0 matt      (1000) matt      (1000)     1190 2022-10-31 23:51:43.000000 pynchon-2022.12.6.18.30/src/pynchon/templates/api/classes.md.j2
--rw-rw-r--   0 matt      (1000) matt      (1000)      891 2022-10-31 23:52:22.000000 pynchon-2022.12.6.18.30/src/pynchon/templates/api/functions.md.j2
--rw-rw-r--   0 matt      (1000) matt      (1000)      322 2022-10-31 23:53:44.000000 pynchon-2022.12.6.18.30/src/pynchon/templates/api/modules.md.j2
--rw-rw-r--   0 matt      (1000) matt      (1000)      686 2022-10-31 23:55:45.000000 pynchon-2022.12.6.18.30/src/pynchon/templates/api/package.md.j2
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2022-12-06 23:30:00.332284 pynchon-2022.12.6.18.30/src/pynchon/templates/cli/
--rw-rw-r--   0 matt      (1000) matt      (1000)      403 2022-10-31 21:18:03.000000 pynchon-2022.12.6.18.30/src/pynchon/templates/cli/TOC.md.j2
--rw-rw-r--   0 matt      (1000) matt      (1000)      198 2022-10-31 20:54:31.000000 pynchon-2022.12.6.18.30/src/pynchon/templates/cli/detail.md.j2
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2022-10-31 20:40:42.000000 pynchon-2022.12.6.18.30/src/pynchon/templates/cli-toc.md.j2
--rw-rw-r--   0 matt      (1000) matt      (1000)     2985 2022-10-29 22:24:16.000000 pynchon-2022.12.6.18.30/src/pynchon/templates/toc.md.j2
--rw-rw-r--   0 matt      (1000) matt      (1000)     6267 2022-12-06 23:23:23.000000 pynchon-2022.12.6.18.30/src/pynchon/util.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2022-12-06 23:30:00.332284 pynchon-2022.12.6.18.30/src/pynchon.egg-info/
--rw-rw-r--   0 matt      (1000) matt      (1000)      737 2022-12-06 23:30:00.000000 pynchon-2022.12.6.18.30/src/pynchon.egg-info/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)      925 2022-12-06 23:30:00.000000 pynchon-2022.12.6.18.30/src/pynchon.egg-info/SOURCES.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2022-12-06 23:30:00.000000 pynchon-2022.12.6.18.30/src/pynchon.egg-info/dependency_links.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       46 2022-12-06 23:30:00.000000 pynchon-2022.12.6.18.30/src/pynchon.egg-info/entry_points.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2022-12-06 23:30:00.000000 pynchon-2022.12.6.18.30/src/pynchon.egg-info/not-zip-safe
--rw-rw-r--   0 matt      (1000) matt      (1000)      244 2022-12-06 23:30:00.000000 pynchon-2022.12.6.18.30/src/pynchon.egg-info/requires.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        8 2022-12-06 23:30:00.000000 pynchon-2022.12.6.18.30/src/pynchon.egg-info/top_level.txt
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.912925 pynchon-2023.5.2.14.42/
+-rw-rw-r--   0 matt      (1000) matt      (1000)       50 2022-10-31 17:10:29.000000 pynchon-2023.5.2.14.42/MANIFEST.in
+-rw-rw-r--   0 matt      (1000) matt      (1000)      736 2023-05-02 18:42:12.912925 pynchon-2023.5.2.14.42/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)     6135 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/README.md
+-rw-rw-r--   0 matt      (1000) matt      (1000)      979 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/pyproject.toml
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1601 2023-05-02 18:42:12.916925 pynchon-2023.5.2.14.42/setup.cfg
+-rw-rw-r--   0 matt      (1000) matt      (1000)      730 2022-10-31 16:56:45.000000 pynchon-2023.5.2.14.42/setup.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.896925 pynchon-2023.5.2.14.42/src/
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.900925 pynchon-2023.5.2.14.42/src/pynchon/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      251 2023-04-30 02:08:52.000000 pynchon-2023.5.2.14.42/src/pynchon/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      100 2023-05-02 02:18:56.000000 pynchon-2023.5.2.14.42/src/pynchon/__main__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       77 2023-05-02 18:42:10.000000 pynchon-2023.5.2.14.42/src/pynchon/_version.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.904925 pynchon-2023.5.2.14.42/src/pynchon/abcs/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      262 2023-04-30 02:08:52.000000 pynchon-2023.5.2.14.42/src/pynchon/abcs/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1244 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/abcs/attrdict.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2431 2023-05-02 01:26:44.000000 pynchon-2023.5.2.14.42/src/pynchon/abcs/config.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2909 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/abcs/meta.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1254 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/src/pynchon/abcs/path.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      686 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/abcs/plugin.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4788 2023-05-02 02:11:29.000000 pynchon-2023.5.2.14.42/src/pynchon/abcs/visitor.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4336 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/annotate.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.904925 pynchon-2023.5.2.14.42/src/pynchon/api/
+-rw-rw-r--   0 matt      (1000) matt      (1000)       20 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.42/src/pynchon/api/__init__.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.904925 pynchon-2023.5.2.14.42/src/pynchon/api/git/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      109 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.42/src/pynchon/api/git/__init__.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.904925 pynchon-2023.5.2.14.42/src/pynchon/api/project/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1146 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/api/project/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       28 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.42/src/pynchon/api/pynchon.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2215 2023-05-02 02:11:29.000000 pynchon-2023.5.2.14.42/src/pynchon/api/render.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5154 2023-05-02 02:11:29.000000 pynchon-2023.5.2.14.42/src/pynchon/app.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.904925 pynchon-2023.5.2.14.42/src/pynchon/bin/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      972 2023-05-02 03:00:09.000000 pynchon-2023.5.2.14.42/src/pynchon/bin/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.42/src/pynchon/bin/cli.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.42/src/pynchon/bin/dot.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3318 2023-04-30 22:57:08.000000 pynchon-2023.5.2.14.42/src/pynchon/bin/entry.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.42/src/pynchon/bin/groups.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-28 03:58:20.000000 pynchon-2023.5.2.14.42/src/pynchon/bin/options.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.42/src/pynchon/bin/parse.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.42/src/pynchon/bin/render.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.904925 pynchon-2023.5.2.14.42/src/pynchon/cli/
+-rw-rw-r--   0 matt      (1000) matt      (1000)       54 2023-04-30 18:28:18.000000 pynchon-2023.5.2.14.42/src/pynchon/cli/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     6992 2023-05-02 02:54:32.000000 pynchon-2023.5.2.14.42/src/pynchon/cli/common.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2423 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.42/src/pynchon/cli/options.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2439 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.42/src/pynchon/click.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.904925 pynchon-2023.5.2.14.42/src/pynchon/config/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1824 2023-05-02 02:11:29.000000 pynchon-2023.5.2.14.42/src/pynchon/config/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4672 2023-04-30 17:56:47.000000 pynchon-2023.5.2.14.42/src/pynchon/config/util.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1059 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.42/src/pynchon/constants.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2856 2023-05-02 01:23:34.000000 pynchon-2023.5.2.14.42/src/pynchon/core.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      115 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/src/pynchon/events.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       27 2023-04-29 21:27:56.000000 pynchon-2023.5.2.14.42/src/pynchon/exceptions.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.904925 pynchon-2023.5.2.14.42/src/pynchon/fleks/
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-30 02:43:01.000000 pynchon-2023.5.2.14.42/src/pynchon/fleks/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     8460 2023-05-02 03:00:09.000000 pynchon-2023.5.2.14.42/src/pynchon/models.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.908925 pynchon-2023.5.2.14.42/src/pynchon/plugins/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1006 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/api.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       95 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/ast.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      473 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/cicd.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1593 2023-05-02 03:03:42.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/core.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-29 22:36:50.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/cut.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.908925 pynchon-2023.5.2.14.42/src/pynchon/plugins/doctor/
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/doctor/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5684 2023-05-02 05:37:02.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/dot.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      374 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/files.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2797 2023-05-02 05:30:45.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/fixme.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      351 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/gen.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.908925 pynchon-2023.5.2.14.42/src/pynchon/plugins/git/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      373 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/git/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2448 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/git/config.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      305 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/globals.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-28 01:24:33.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/hooks.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     6075 2023-05-02 05:08:45.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/jinja.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3527 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/json.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      722 2023-04-29 19:14:56.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/load.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.908925 pynchon-2023.5.2.14.42/src/pynchon/plugins/makefile/
+-rw-rw-r--   0 matt      (1000) matt      (1000)       52 2023-04-28 18:54:48.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/makefile/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      840 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/parse.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1149 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/plugins.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4548 2023-04-30 18:42:04.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/project.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.908925 pynchon-2023.5.2.14.42/src/pynchon/plugins/python/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      112 2023-04-28 01:24:33.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/python/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2709 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/python/api.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/python/ast.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     7490 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/python/cli.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-28 01:24:33.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/python/config.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      236 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/python/models.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1525 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/python/platform.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      456 2023-04-30 02:08:52.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/python/pypi.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      723 2023-04-29 19:14:56.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/release.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4781 2023-04-30 17:58:57.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/render.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       60 2023-04-28 22:07:13.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/rtd.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.908925 pynchon-2023.5.2.14.42/src/pynchon/plugins/scaffolding/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3434 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/scaffolding/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1156 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/scaffolding/config.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1266 2023-04-30 17:56:47.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/util.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.908925 pynchon-2023.5.2.14.42/src/pynchon/shimport/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      209 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/src/pynchon/shimport/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      562 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/src/pynchon/shimport/abcs.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-30 01:24:51.000000 pynchon-2023.5.2.14.42/src/pynchon/shimport/hooks.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-30 17:41:25.000000 pynchon-2023.5.2.14.42/src/pynchon/shimport/importing.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    12287 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/src/pynchon/shimport/models.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2390 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/src/pynchon/shimport/module.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-30 18:08:09.000000 pynchon-2023.5.2.14.42/src/pynchon/shimport/registry.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-30 01:29:20.000000 pynchon-2023.5.2.14.42/src/pynchon/shimport/types.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      538 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/src/pynchon/shimport/util.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       73 2023-04-30 02:08:52.000000 pynchon-2023.5.2.14.42/src/pynchon/tagging.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.900925 pynchon-2023.5.2.14.42/src/pynchon/templates/
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.908925 pynchon-2023.5.2.14.42/src/pynchon/templates/cookie_cutter/
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.42/src/pynchon/templates/cookie_cutter/.gitkeep
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.900925 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.900925 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.908925 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/github/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      295 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/github/header.md.j2
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.908925 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/Makefile.md.j2
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.912925 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/core/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      392 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/core/VERSIONS.md.j2
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.912925 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/fixme/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      164 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/fixme/FIXME.md.j2
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.900925 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/python/
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.912925 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/python/api/
+-rw-rw-r--   0 matt      (1000) matt      (1000)       34 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/python/api/TOC.md.j2
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1190 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/python/api/classes.md.j2
+-rw-rw-r--   0 matt      (1000) matt      (1000)      891 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/python/api/functions.md.j2
+-rw-rw-r--   0 matt      (1000) matt      (1000)      322 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/python/api/modules.md.j2
+-rw-rw-r--   0 matt      (1000) matt      (1000)      686 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/python/api/package.md.j2
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2985 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/python/api/toc2.md.j2
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.912925 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/python/cli/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      623 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/python/cli/TOC.md.j2
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/python/cli/cli-toc.md.j2
+-rw-rw-r--   0 matt      (1000) matt      (1000)      198 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/python/cli/detail.md.j2
+-rw-rw-r--   0 matt      (1000) matt      (1000)      253 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/python/cli/main.module.md.j2
+-rw-rw-r--   0 matt      (1000) matt      (1000)      284 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.42/src/pynchon/testing.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.912925 pynchon-2023.5.2.14.42/src/pynchon/util/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2084 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/util/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1016 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/util/click.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4750 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/util/complexity.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      871 2023-04-30 02:08:52.000000 pynchon-2023.5.2.14.42/src/pynchon/util/config.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      577 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/util/events.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4348 2023-05-02 05:31:21.000000 pynchon-2023.5.2.14.42/src/pynchon/util/files.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1944 2023-05-02 02:11:29.000000 pynchon-2023.5.2.14.42/src/pynchon/util/lme.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      954 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/util/oop.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2423 2023-05-02 05:37:15.000000 pynchon-2023.5.2.14.42/src/pynchon/util/os.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2279 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/util/python.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2972 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/util/tagging.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      411 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/util/testing.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.912925 pynchon-2023.5.2.14.42/src/pynchon/util/text/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      837 2023-05-02 00:54:17.000000 pynchon-2023.5.2.14.42/src/pynchon/util/text/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      365 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/src/pynchon/util/text/__main__.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.912925 pynchon-2023.5.2.14.42/src/pynchon/util/text/loadf/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5301 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/src/pynchon/util/text/loadf/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1033 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/src/pynchon/util/text/loadf/__main__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1652 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/src/pynchon/util/text/loads.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.912925 pynchon-2023.5.2.14.42/src/pynchon/util/text/normalize/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      740 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/util/text/normalize/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       40 2023-04-29 02:48:43.000000 pynchon-2023.5.2.14.42/src/pynchon/util/text/normalize/__main__.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.912925 pynchon-2023.5.2.14.42/src/pynchon/util/text/render/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5245 2023-05-01 23:54:56.000000 pynchon-2023.5.2.14.42/src/pynchon/util/text/render/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      963 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/src/pynchon/util/text/render/__main__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1171 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/src/pynchon/util/typing.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.904925 pynchon-2023.5.2.14.42/src/pynchon.egg-info/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      736 2023-05-02 18:42:12.000000 pynchon-2023.5.2.14.42/src/pynchon.egg-info/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4455 2023-05-02 18:42:12.000000 pynchon-2023.5.2.14.42/src/pynchon.egg-info/SOURCES.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        1 2023-05-02 18:42:12.000000 pynchon-2023.5.2.14.42/src/pynchon.egg-info/dependency_links.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)       46 2023-05-02 18:42:12.000000 pynchon-2023.5.2.14.42/src/pynchon.egg-info/entry_points.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        1 2023-05-02 18:42:12.000000 pynchon-2023.5.2.14.42/src/pynchon.egg-info/not-zip-safe
+-rw-rw-r--   0 matt      (1000) matt      (1000)      398 2023-05-02 18:42:12.000000 pynchon-2023.5.2.14.42/src/pynchon.egg-info/requires.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        8 2023-05-02 18:42:12.000000 pynchon-2023.5.2.14.42/src/pynchon.egg-info/top_level.txt
```

### Comparing `pynchon-2022.12.6.18.30/PKG-INFO` & `pynchon-2023.5.2.14.42/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynchon
-Version: 2022.12.6.18.30
+Version: 2023.5.2.14.42
 Summary: Autodocs for python projects
 Home-page: https://github.com/elo-enterprises/pynchon/
 Author: elo
 Author-email: engineering@elo.enterprises
 License: MIT
 Project-URL: Documentation, https://github.com/elo-enterprises/pynchon/
 Project-URL: Source, https://github.com/elo-enterprises/pynchon/
```

### Comparing `pynchon-2022.12.6.18.30/setup.cfg` & `pynchon-2023.5.2.14.42/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -26,30 +26,43 @@
 	=src
 python_requires = >3.6
 install_requires = 
 	click
 	coloredlogs==15.0.1
 	memoized-property==1.0.3
 	memoization==0.4.0
-	pyjson5==1.6.1
+	json5==0.9.10
+	pygments
 	Jinja2==3.1.2
 	griffe==0.23.0
 	mccabe==0.7.0
+	pyyaml
+	termcolor
+	tomli # as tomllib; tomllib only available in py3.11
+	tomli_w==1.0.0
+	pydash==7.0.1
+	enlighten==1.11.2
+	rich==13.3.4
+	multipledispatch==0.6.0
+	blinker==1.6.2
+	pydantic
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
 j2 = 
 	j2cli==0.3.10
+	Jinja2
 dev = 
 	IPython
 testing = 
+	IPython
 	tox
 	pytest
 	pytest-cov
 	mock
 	flake8==5.0.4
 lint = 
 	tox
```

### Comparing `pynchon-2022.12.6.18.30/setup.py` & `pynchon-2023.5.2.14.42/setup.py`

 * *Files identical despite different names*

### Comparing `pynchon-2022.12.6.18.30/src/pynchon/annotate.py` & `pynchon-2023.5.2.14.42/src/pynchon/annotate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,99 +1,143 @@
 """ """
 import os
-import sys
 import inspect
 import importlib
+
 import pynchon
 from pynchon import util
-LOGGER = pynchon.get_logger(__name__)
+from pynchon.util import lme
+
+LOGGER = lme.get_logger(__name__)
+
 
 def klass(name, kls) -> None:
-    """ annotates a class """
+    """annotates a class"""
     LOGGER.debug(f"annotating class: {name}")
     mod = importlib.import_module(kls.parent.canonical_path)
     kls._handle = getattr(mod, name)
 
     properties = []
     for x in dir(kls._handle):
-        if x.startswith('_'):
+        if x.startswith("_"):
             continue
-        prop = getattr(kls._handle,x)
-        is_property = type(prop).__name__=='property'
+        prop = getattr(kls._handle, x)
+        is_property = type(prop).__name__ == "property"
         if not is_property:
             continue
         fxn = prop.fget
-        fxn_sig, fxn_doc = inspect.signature(fxn), fxn.__doc__ or ''
+        fxn_doc = fxn.__doc__ or ""
+        try:
+            fxn_sig = inspect.signature(fxn)
+        except (ValueError,) as exc:
+            LOGGER.warning(f"Could not retrieve function signature for {fxn}!")
+            fxn_sig = None
         try:
             fxn_code = fxn.__code__
-        except AttributeError: # C extensions..
+        except AttributeError:  # C extensions..
             fxn_code = None
         start = fxn_code.co_firstlineno if fxn_code else kls.lineno
-        properties.append(dict(
-            name=x,
-            doc=fxn_doc,
-            signature=fxn_sig,
-            start=str(start),
-            end='', # FIXME
-            annotation=str(fxn_sig.return_annotation).replace("<class '","").replace("'>",""),
-            fixme='FIXME' in fxn_doc))
+        properties.append(
+            dict(
+                name=x,
+                doc=fxn_doc,
+                signature=fxn_sig,
+                start=str(start),
+                end="",  # FIXME
+                annotation=fxn_sig
+                and str(fxn_sig.return_annotation)
+                .replace("<class '", "")
+                .replace("'>", ""),
+                fixme="FIXME" in fxn_doc,
+            )
+        )
 
     bases = []
     for x in kls._handle.__bases__:
         tmp = "[{name}]({link})"
-        qname = x.__module__.replace('.', '')
+        qname = x.__module__.replace(".", "")
         bname = x.__name__
-        if 'builtin' in qname:
+        if "builtin" in qname:
             tmp = tmp.format(
                 name=f"`__builtin__.{bname}`",
-                link=f"{pynchon.URL_BUILTINS}#func-{bname}")
+                link=f"{pynchon.URL_BUILTINS}#func-{bname}",
+            )
         else:
             tmp = tmp.format(name=bname, link=f"#{qname}")
         bases.append(tmp)
 
-    kls_code=inspect.getsource(kls._handle)
-    kls_fname=inspect.getfile(kls._handle)
-    kls._metadata=dict(
-        bases=bases, code=kls_code,
+    kls_code = inspect.getsource(kls._handle)
+    kls_fname = inspect.getfile(kls._handle)
+    kls._metadata = dict(
+        bases=bases,
+        code=kls_code,
         start=str(kls.lineno),
-        end=str(kls.endlineno or ''),
-        properties=properties)
+        end=str(kls.endlineno or ""),
+        properties=properties,
+    )
 
     kls._metadata.update(mccabe=util.complexity(kls_code, kls_fname))
 
+
 def module(name, module, working_dir=None) -> None:
-    """ annotates a module """
+    """annotates a module"""
     LOGGER.debug(f"annotating module: {name}")
-    module._metadata = dict(
-        base_url = str(module.filepath.relative_to(working_dir)))
+    module._metadata = dict(base_url=str(module.filepath.relative_to(working_dir)))
+
+
+def should_skip(name: str):
+    """ """
+    from pynchon.config import pynchon as pynchon_config
+
+    api_config = pynchon_config.get("api")
+    should_skip = api_config.get("skip_private_methods", False)
+    should_skip = should_skip and name.startswith("_")
+    LOGGER.warning(
+        f"annotation for `{name}` exits early; `pynchon.api.skip_private_methods` is set and this looks private"
+    )
+    return should_skip
+
 
 def function(name, fxn) -> None:
-    """ annotates a function """
+    """annotates a function"""
     LOGGER.debug(f"annotating fxn: {name}")
+    fxn._metadata = dict()
+    if should_skip(name):
+        return
     mod = importlib.import_module(fxn.parent.canonical_path)
     handle = getattr(mod, name)
-    fxn._handle = getattr(mod,name)
-    fxn_doc = fxn._handle.__doc__ or ''
+    fxn._handle = getattr(mod, name)
+    fxn_doc = fxn._handle.__doc__ or ""
     try:
         fxn_fname = inspect.getfile(fxn._handle)
     except (Exception,) as exc:
-        fxn_fname = '?'
+        fxn_fname = "?"
         fxn_code = None
     else:
         fxn_fname = os.path.relpath(fxn_fname)
         fxn_code = inspect.getsource(fxn._handle)
     try:
         fxn_sig = inspect.signature(fxn._handle)
     except (Exception,) as exc:
         fxn_sig = None
-    fixme_lines = [ i+fxn.lineno for i,l in enumerate(fxn_doc.split('\n')) if 'FIXME' in l]
+    fixme_lines = [
+        i + fxn.lineno for i, l in enumerate(fxn_doc.split("\n")) if "FIXME" in l
+    ]
     fxn._metadata = dict(
-            name=name,
-            doc=fxn_doc,
-            signature=fxn_sig,
-            # start=str(fxn._handle.__code__.co_firstlineno),
-            annotation=str(fxn_sig and fxn_sig.return_annotation or '').replace("<class '","").replace("'>",""),
-            fixme= [ dict(
-                glyph=' 🚩has FIXMEs ',
-                link=f'/{fxn_fname}#L{fixme_lines[0]}',
-                hover=f"on lines {fixme_lines}") ] if fixme_lines else [])
+        name=name,
+        doc=fxn_doc,
+        signature=fxn_sig,
+        # start=str(fxn._handle.__code__.co_firstlineno),
+        annotation=str(fxn_sig and fxn_sig.return_annotation or "")
+        .replace("<class '", "")
+        .replace("'>", ""),
+        fixme=[
+            dict(
+                glyph=" 🚩has FIXMEs ",
+                link=f"/{fxn_fname}#L{fixme_lines[0]}",
+                hover=f"on lines {fixme_lines}",
+            )
+        ]
+        if fixme_lines
+        else [],
+    )
     fxn_code and fxn._metadata.update(mccabe=util.complexity(fxn_code, fxn_fname))
```

### Comparing `pynchon-2022.12.6.18.30/src/pynchon/templates/api/classes.md.j2` & `pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/python/api/classes.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2022.12.6.18.30/src/pynchon/templates/api/functions.md.j2` & `pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/python/api/functions.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2022.12.6.18.30/src/pynchon/templates/api/package.md.j2` & `pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/python/api/package.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2022.12.6.18.30/src/pynchon/templates/toc.md.j2` & `pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/python/api/toc2.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2022.12.6.18.30/src/pynchon/util.py` & `pynchon-2023.5.2.14.42/src/pynchon/util/complexity.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,82 +1,34 @@
-""" pynchon.util
-"""
+GLYPH_COMPLEXITY = "🐉 Complex"
+
 import os
-import sys
 import ast
+import sys
+from collections import OrderedDict
 
-import mccabe
 import griffe
+import mccabe
 
-import pynchon
-LOGGER = pynchon.get_logger(__name__)
-from pynchon import annotate
-
-LOGGER = pynchon.get_logger(__name__)
-WORKING_DIR = os.getcwd()
-GLYPH_COMPLEXITY = '🐉 Complex'
+from pynchon import annotate, constants
+from pynchon.abcs import Path
+from pynchon.util import lme
 
-def load_setupcfg(file:str='setup.cfg'):
-    """ """
-    if not os.path.exists(file):
-        err = f"Cannot load from nonexistent file @ `{file}`"
-        LOGGER.critical(err)
-        raise RuntimeError(err)
-    import configparser
-    config = configparser.ConfigParser()
-    config.read(file)
-    return config
+WORKING_DIR = Path(".")
+LOGGER = lme.get_logger(__name__)
 
-def load_entrypoints(config=None):
-    """ """
-    console_scripts = config['options.entry_points']['console_scripts']
-    console_scripts = [x for x in console_scripts.split('\n') if x ]
-    package = config['metadata']['name']
-    entrypoints = []
-    for c in console_scripts:
-        tmp = dict(
-            package=package,
-            bin_name=c.split('=')[0].strip(),
-            module=c.split('=')[1].strip().split(':')[0],
-            entrypoint=c.split('=')[1].strip().split(':')[1],
-        )
-        abs_entrypoint=tmp['module']+':'+tmp['entrypoint']
-        tmp['setuptools_entrypoint'] = abs_entrypoint
-        entrypoints.append(tmp)
-    return dict(package=package, entrypoints=entrypoints,)
 
-def click_recursive_help(cmd,
-    parent=None, out={}, file=sys.stdout):
+def clean_text(txt: str) -> str:
     """ """
-    # source: adapted from https://stackoverflow.com/questions/57810659/automatically-generate-all-help-documentation-for-click-commands
-    from click.core import Context as ClickContext
-    full_name = cmd.name
-    pname = getattr(cmd, 'parent', None)
-    pname = parent and getattr(parent, 'name', '') or ''
-    ctx = ClickContext(cmd, info_name=cmd.name, parent=parent)
-    help_txt = cmd.get_help(ctx)
-    invocation_sample = help_txt.split('\n')[0]
-    for x in 'Usage: [OPTIONS] COMMAND [COMMAND] [ARGS] ...'.split():
-        invocation_sample = invocation_sample.replace(x, '')
-    out = {
-        **out,
-        **{full_name: dict(
-            name=cmd.name,
-            invocation_sample=invocation_sample,
-            help=help_txt)}
-    }
-    commands = getattr(cmd, 'commands', {})
-    for sub in commands.values():
-        out ={**out, **click_recursive_help(sub, ctx)}
-    return out
+    return "\n".join([line for line in txt.split("\n") if line.strip()])
 
-def get_module(package:str='', file:str=''):
+
+def get_module(package: str = "", file: str = ""):
     """ """
     if not bool(package) ^ bool(file):
-        err = 'Expected --file or --package, but not both'
+        err = "Expected --file or --package, but not both"
         raise RuntimeError(err)
     if file:
         file = os.path.abspath(file)
         new_path = os.path.dirname(file)
         assert os.path.exists(file)
         LOGGER.warning(f"modifying sys.path to include {new_path}")
         sys.path.append(new_path)
@@ -85,94 +37,129 @@
     else:
         working_dir = WORKING_DIR
     loader = griffe.loader.GriffeLoader()
     module = loader.load_module(package)
     annotate.module(package, module, working_dir=working_dir)
     return module
 
+
 def get_refs(working_dir=None, module=None) -> dict:
     """ """
     refs = dict(
-        classes=dict([[k, v] for k, v in module.classes.items() if not module.classes[k].is_alias]),
-        modules=dict([[k, v] for k, v in module.modules.items() if not module.modules[k].is_alias]),
-        functions=dict([[k, v] for k, v in module.functions.items() if not module.functions[k].is_alias]),
+        classes=dict(
+            [
+                [k, v]
+                for k, v in module.classes.items()
+                if not module.classes[k].is_alias
+            ]
+        ),
+        modules=dict(
+            [
+                [k, v]
+                for k, v in module.modules.items()
+                if not module.modules[k].is_alias
+            ]
+        ),
+        functions=OrderedDict(
+            [
+                [k, v]
+                for k, v in sorted(module.functions.items())
+                if not module.functions[k].is_alias
+            ]
+        ),
     )
-    for name,kls in refs['classes'].items():
+    for name, kls in refs["classes"].items():
         annotate.klass(name, kls)
-    for name,mod in refs['modules'].items():
+    for name, mod in refs["modules"].items():
         annotate.module(name, mod, working_dir=working_dir)
-    for name,fxn in refs['functions'].items():
+    for name, fxn in refs["functions"].items():
         annotate.function(name, fxn)
     return refs
 
+
 def visit_module(
-        output=[], stats={}, module=None, template=pynchon.T_TOC_API,
-        visited=[], exclude:list=[], module_name=None, working_dir=WORKING_DIR):
-    """ recursive visitor for this package, submodules, classes, functions, etc """
+    output=[],
+    stats={},
+    module=None,
+    template=constants.T_TOC_API,
+    visited=[],
+    exclude: list = [],
+    module_name=None,
+    working_dir=WORKING_DIR,
+):
+    """recursive visitor for this package, submodules, classes, functions, etc"""
     if module_name in exclude:
         LOGGER.debug(f"skipping module: {module_name}")
         return output
     annotate.module(module_name, module, working_dir=working_dir)
     refs = get_refs(working_dir=working_dir, module=module)
     # LOGGER.debug(f"exclude: {exclude}")
     LOGGER.debug(f"rendering module: {module_name}")
     rendered = template.render(
-        griffe=griffe, stats=stats,
+        griffe=griffe,
+        stats=stats,
         working_dir=working_dir,
-        module_name=module_name, module=module,
-        **refs)
+        module_name=module_name,
+        module=module,
+        **refs,
+    )
     output.append(clean_text(rendered))
-    for name, sub in refs['modules'].items():
+    for name, sub in refs["modules"].items():
         if sub in visited:
             continue
         visit_module(
-            output=output, module=sub,
+            output=output,
+            module=sub,
             working_dir=working_dir,
             module_name=f"{module_name}.{name}",
-            visited=visited+[module],
+            visited=visited + [module],
             exclude=exclude,
-            template=template)
+            template=template,
+        )
     return output
 
 
-def clean_text(txt:str) -> str:
-    """ """
-    return '\n'.join([
-        line for line in txt.split('\n') if line.strip() ])
-
 class Checker(mccabe.McCabeChecker):
     """ """
 
     def run(self):
         if self.max_complexity < 0:
             return
         visitor = mccabe.PathGraphingAstVisitor()
         visitor.preorder(self.tree, visitor)
         for graph in visitor.graphs.values():
-            tmp=graph.complexity()
+            tmp = graph.complexity()
             if tmp > self.max_complexity:
                 text = self._error_tmpl % (graph.entity, tmp)
                 yield tmp, graph.lineno, graph.column, text, type(self)
 
-def complexity(code:str=None, fname:str=None, threshold:int=7):
+
+def complexity(code: str = None, fname: str = None, threshold: int = 7):
     """ """
-    threshold=7
+    threshold = 7
     try:
         tree = compile(code, fname, "exec", ast.PyCF_ONLY_AST)
     except SyntaxError:
         e = sys.exc_info()[1]
         sys.stderr.write("Unable to parse %s: %s\n" % (fname, e))
         return 0
     complex = []
     Checker.max_complexity = threshold
-    for complexity, lineno, offset, text, check in Checker(tree, fname).run():
-        complex.append(dict(
-            file=os.path.relpath(fname),lineno=lineno,
-            # text=text,
-            score=complexity))
+    for complexity, lineno, _offset, text, check in Checker(tree, fname).run():
+        complex.append(
+            dict(
+                file=os.path.relpath(fname),
+                lineno=lineno,
+                # text=text,
+                score=complexity,
+            )
+        )
     out = []
     for admonition in complex:
-        out.append(dict(
-            glyph=GLYPH_COMPLEXITY,
-            hover=f'score {admonition["score"]} / {threshold}',
-            link=f'/{admonition["file"]}#L{admonition["lineno"]}'))
+        out.append(
+            dict(
+                glyph=GLYPH_COMPLEXITY,
+                hover=f'score {admonition["score"]} / {threshold}',
+                link=f'/{admonition["file"]}#L{admonition["lineno"]}',
+            )
+        )
     return out
```

### Comparing `pynchon-2022.12.6.18.30/src/pynchon.egg-info/PKG-INFO` & `pynchon-2023.5.2.14.42/src/pynchon.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynchon
-Version: 2022.12.6.18.30
+Version: 2023.5.2.14.42
 Summary: Autodocs for python projects
 Home-page: https://github.com/elo-enterprises/pynchon/
 Author: elo
 Author-email: engineering@elo.enterprises
 License: MIT
 Project-URL: Documentation, https://github.com/elo-enterprises/pynchon/
 Project-URL: Source, https://github.com/elo-enterprises/pynchon/
```

