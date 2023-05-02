# Comparing `tmp/pynchon-2023.5.2.14.42.tar.gz` & `tmp/pynchon-2023.5.2.14.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynchon-2023.5.2.14.42.tar", last modified: Tue May  2 18:42:12 2023, max compression
+gzip compressed data, was "pynchon-2023.5.2.14.50.tar", last modified: Tue May  2 18:50:00 2023, max compression
```

## Comparing `pynchon-2023.5.2.14.42.tar` & `pynchon-2023.5.2.14.50.tar`

### file list

```diff
@@ -1,169 +1,169 @@
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.912925 pynchon-2023.5.2.14.42/
--rw-rw-r--   0 matt      (1000) matt      (1000)       50 2022-10-31 17:10:29.000000 pynchon-2023.5.2.14.42/MANIFEST.in
--rw-rw-r--   0 matt      (1000) matt      (1000)      736 2023-05-02 18:42:12.912925 pynchon-2023.5.2.14.42/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)     6135 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/README.md
--rw-rw-r--   0 matt      (1000) matt      (1000)      979 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/pyproject.toml
--rw-rw-r--   0 matt      (1000) matt      (1000)     1601 2023-05-02 18:42:12.916925 pynchon-2023.5.2.14.42/setup.cfg
--rw-rw-r--   0 matt      (1000) matt      (1000)      730 2022-10-31 16:56:45.000000 pynchon-2023.5.2.14.42/setup.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.896925 pynchon-2023.5.2.14.42/src/
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.900925 pynchon-2023.5.2.14.42/src/pynchon/
--rw-rw-r--   0 matt      (1000) matt      (1000)      251 2023-04-30 02:08:52.000000 pynchon-2023.5.2.14.42/src/pynchon/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      100 2023-05-02 02:18:56.000000 pynchon-2023.5.2.14.42/src/pynchon/__main__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)       77 2023-05-02 18:42:10.000000 pynchon-2023.5.2.14.42/src/pynchon/_version.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.904925 pynchon-2023.5.2.14.42/src/pynchon/abcs/
--rw-rw-r--   0 matt      (1000) matt      (1000)      262 2023-04-30 02:08:52.000000 pynchon-2023.5.2.14.42/src/pynchon/abcs/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1244 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/abcs/attrdict.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2431 2023-05-02 01:26:44.000000 pynchon-2023.5.2.14.42/src/pynchon/abcs/config.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2909 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/abcs/meta.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1254 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/src/pynchon/abcs/path.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      686 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/abcs/plugin.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     4788 2023-05-02 02:11:29.000000 pynchon-2023.5.2.14.42/src/pynchon/abcs/visitor.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     4336 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/annotate.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.904925 pynchon-2023.5.2.14.42/src/pynchon/api/
--rw-rw-r--   0 matt      (1000) matt      (1000)       20 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.42/src/pynchon/api/__init__.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.904925 pynchon-2023.5.2.14.42/src/pynchon/api/git/
--rw-rw-r--   0 matt      (1000) matt      (1000)      109 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.42/src/pynchon/api/git/__init__.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.904925 pynchon-2023.5.2.14.42/src/pynchon/api/project/
--rw-rw-r--   0 matt      (1000) matt      (1000)     1146 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/api/project/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)       28 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.42/src/pynchon/api/pynchon.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2215 2023-05-02 02:11:29.000000 pynchon-2023.5.2.14.42/src/pynchon/api/render.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     5154 2023-05-02 02:11:29.000000 pynchon-2023.5.2.14.42/src/pynchon/app.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.904925 pynchon-2023.5.2.14.42/src/pynchon/bin/
--rw-rw-r--   0 matt      (1000) matt      (1000)      972 2023-05-02 03:00:09.000000 pynchon-2023.5.2.14.42/src/pynchon/bin/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.42/src/pynchon/bin/cli.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.42/src/pynchon/bin/dot.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3318 2023-04-30 22:57:08.000000 pynchon-2023.5.2.14.42/src/pynchon/bin/entry.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.42/src/pynchon/bin/groups.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-28 03:58:20.000000 pynchon-2023.5.2.14.42/src/pynchon/bin/options.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.42/src/pynchon/bin/parse.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.42/src/pynchon/bin/render.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.904925 pynchon-2023.5.2.14.42/src/pynchon/cli/
--rw-rw-r--   0 matt      (1000) matt      (1000)       54 2023-04-30 18:28:18.000000 pynchon-2023.5.2.14.42/src/pynchon/cli/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     6992 2023-05-02 02:54:32.000000 pynchon-2023.5.2.14.42/src/pynchon/cli/common.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2423 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.42/src/pynchon/cli/options.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2439 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.42/src/pynchon/click.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.904925 pynchon-2023.5.2.14.42/src/pynchon/config/
--rw-rw-r--   0 matt      (1000) matt      (1000)     1824 2023-05-02 02:11:29.000000 pynchon-2023.5.2.14.42/src/pynchon/config/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     4672 2023-04-30 17:56:47.000000 pynchon-2023.5.2.14.42/src/pynchon/config/util.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1059 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.42/src/pynchon/constants.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2856 2023-05-02 01:23:34.000000 pynchon-2023.5.2.14.42/src/pynchon/core.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      115 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/src/pynchon/events.py
--rw-rw-r--   0 matt      (1000) matt      (1000)       27 2023-04-29 21:27:56.000000 pynchon-2023.5.2.14.42/src/pynchon/exceptions.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.904925 pynchon-2023.5.2.14.42/src/pynchon/fleks/
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-30 02:43:01.000000 pynchon-2023.5.2.14.42/src/pynchon/fleks/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     8460 2023-05-02 03:00:09.000000 pynchon-2023.5.2.14.42/src/pynchon/models.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.908925 pynchon-2023.5.2.14.42/src/pynchon/plugins/
--rw-rw-r--   0 matt      (1000) matt      (1000)     1006 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/api.py
--rw-rw-r--   0 matt      (1000) matt      (1000)       95 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/ast.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      473 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/cicd.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1593 2023-05-02 03:03:42.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/core.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-29 22:36:50.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/cut.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.908925 pynchon-2023.5.2.14.42/src/pynchon/plugins/doctor/
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/doctor/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     5684 2023-05-02 05:37:02.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/dot.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      374 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/files.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2797 2023-05-02 05:30:45.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/fixme.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      351 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/gen.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.908925 pynchon-2023.5.2.14.42/src/pynchon/plugins/git/
--rw-rw-r--   0 matt      (1000) matt      (1000)      373 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/git/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2448 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/git/config.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      305 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/globals.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-28 01:24:33.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/hooks.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     6075 2023-05-02 05:08:45.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/jinja.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3527 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/json.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      722 2023-04-29 19:14:56.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/load.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.908925 pynchon-2023.5.2.14.42/src/pynchon/plugins/makefile/
--rw-rw-r--   0 matt      (1000) matt      (1000)       52 2023-04-28 18:54:48.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/makefile/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      840 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/parse.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1149 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/plugins.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     4548 2023-04-30 18:42:04.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/project.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.908925 pynchon-2023.5.2.14.42/src/pynchon/plugins/python/
--rw-rw-r--   0 matt      (1000) matt      (1000)      112 2023-04-28 01:24:33.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/python/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2709 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/python/api.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/python/ast.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     7490 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/python/cli.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-28 01:24:33.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/python/config.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      236 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/python/models.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1525 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/python/platform.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      456 2023-04-30 02:08:52.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/python/pypi.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      723 2023-04-29 19:14:56.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/release.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     4781 2023-04-30 17:58:57.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/render.py
--rw-rw-r--   0 matt      (1000) matt      (1000)       60 2023-04-28 22:07:13.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/rtd.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.908925 pynchon-2023.5.2.14.42/src/pynchon/plugins/scaffolding/
--rw-rw-r--   0 matt      (1000) matt      (1000)     3434 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/scaffolding/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1156 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/scaffolding/config.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1266 2023-04-30 17:56:47.000000 pynchon-2023.5.2.14.42/src/pynchon/plugins/util.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.908925 pynchon-2023.5.2.14.42/src/pynchon/shimport/
--rw-rw-r--   0 matt      (1000) matt      (1000)      209 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/src/pynchon/shimport/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      562 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/src/pynchon/shimport/abcs.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-30 01:24:51.000000 pynchon-2023.5.2.14.42/src/pynchon/shimport/hooks.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-30 17:41:25.000000 pynchon-2023.5.2.14.42/src/pynchon/shimport/importing.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    12287 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/src/pynchon/shimport/models.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2390 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/src/pynchon/shimport/module.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-30 18:08:09.000000 pynchon-2023.5.2.14.42/src/pynchon/shimport/registry.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-30 01:29:20.000000 pynchon-2023.5.2.14.42/src/pynchon/shimport/types.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      538 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/src/pynchon/shimport/util.py
--rw-rw-r--   0 matt      (1000) matt      (1000)       73 2023-04-30 02:08:52.000000 pynchon-2023.5.2.14.42/src/pynchon/tagging.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.900925 pynchon-2023.5.2.14.42/src/pynchon/templates/
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.908925 pynchon-2023.5.2.14.42/src/pynchon/templates/cookie_cutter/
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.42/src/pynchon/templates/cookie_cutter/.gitkeep
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.900925 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.900925 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.908925 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/github/
--rw-rw-r--   0 matt      (1000) matt      (1000)      295 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/github/header.md.j2
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.908925 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/Makefile.md.j2
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.912925 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/core/
--rw-rw-r--   0 matt      (1000) matt      (1000)      392 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/core/VERSIONS.md.j2
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.912925 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/fixme/
--rw-rw-r--   0 matt      (1000) matt      (1000)      164 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/fixme/FIXME.md.j2
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.900925 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/python/
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.912925 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/python/api/
--rw-rw-r--   0 matt      (1000) matt      (1000)       34 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/python/api/TOC.md.j2
--rw-rw-r--   0 matt      (1000) matt      (1000)     1190 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/python/api/classes.md.j2
--rw-rw-r--   0 matt      (1000) matt      (1000)      891 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/python/api/functions.md.j2
--rw-rw-r--   0 matt      (1000) matt      (1000)      322 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/python/api/modules.md.j2
--rw-rw-r--   0 matt      (1000) matt      (1000)      686 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/python/api/package.md.j2
--rw-rw-r--   0 matt      (1000) matt      (1000)     2985 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/python/api/toc2.md.j2
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.912925 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/python/cli/
--rw-rw-r--   0 matt      (1000) matt      (1000)      623 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/python/cli/TOC.md.j2
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/python/cli/cli-toc.md.j2
--rw-rw-r--   0 matt      (1000) matt      (1000)      198 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/python/cli/detail.md.j2
--rw-rw-r--   0 matt      (1000) matt      (1000)      253 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/python/cli/main.module.md.j2
--rw-rw-r--   0 matt      (1000) matt      (1000)      284 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.42/src/pynchon/testing.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.912925 pynchon-2023.5.2.14.42/src/pynchon/util/
--rw-rw-r--   0 matt      (1000) matt      (1000)     2084 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/util/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1016 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/util/click.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     4750 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/util/complexity.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      871 2023-04-30 02:08:52.000000 pynchon-2023.5.2.14.42/src/pynchon/util/config.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      577 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/util/events.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     4348 2023-05-02 05:31:21.000000 pynchon-2023.5.2.14.42/src/pynchon/util/files.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1944 2023-05-02 02:11:29.000000 pynchon-2023.5.2.14.42/src/pynchon/util/lme.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      954 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/util/oop.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2423 2023-05-02 05:37:15.000000 pynchon-2023.5.2.14.42/src/pynchon/util/os.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2279 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/util/python.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2972 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/util/tagging.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      411 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/util/testing.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.912925 pynchon-2023.5.2.14.42/src/pynchon/util/text/
--rw-rw-r--   0 matt      (1000) matt      (1000)      837 2023-05-02 00:54:17.000000 pynchon-2023.5.2.14.42/src/pynchon/util/text/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      365 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/src/pynchon/util/text/__main__.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.912925 pynchon-2023.5.2.14.42/src/pynchon/util/text/loadf/
--rw-rw-r--   0 matt      (1000) matt      (1000)     5301 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/src/pynchon/util/text/loadf/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1033 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/src/pynchon/util/text/loadf/__main__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1652 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/src/pynchon/util/text/loads.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.912925 pynchon-2023.5.2.14.42/src/pynchon/util/text/normalize/
--rw-rw-r--   0 matt      (1000) matt      (1000)      740 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.42/src/pynchon/util/text/normalize/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)       40 2023-04-29 02:48:43.000000 pynchon-2023.5.2.14.42/src/pynchon/util/text/normalize/__main__.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.912925 pynchon-2023.5.2.14.42/src/pynchon/util/text/render/
--rw-rw-r--   0 matt      (1000) matt      (1000)     5245 2023-05-01 23:54:56.000000 pynchon-2023.5.2.14.42/src/pynchon/util/text/render/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      963 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/src/pynchon/util/text/render/__main__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1171 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.42/src/pynchon/util/typing.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:42:12.904925 pynchon-2023.5.2.14.42/src/pynchon.egg-info/
--rw-rw-r--   0 matt      (1000) matt      (1000)      736 2023-05-02 18:42:12.000000 pynchon-2023.5.2.14.42/src/pynchon.egg-info/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)     4455 2023-05-02 18:42:12.000000 pynchon-2023.5.2.14.42/src/pynchon.egg-info/SOURCES.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2023-05-02 18:42:12.000000 pynchon-2023.5.2.14.42/src/pynchon.egg-info/dependency_links.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       46 2023-05-02 18:42:12.000000 pynchon-2023.5.2.14.42/src/pynchon.egg-info/entry_points.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2023-05-02 18:42:12.000000 pynchon-2023.5.2.14.42/src/pynchon.egg-info/not-zip-safe
--rw-rw-r--   0 matt      (1000) matt      (1000)      398 2023-05-02 18:42:12.000000 pynchon-2023.5.2.14.42/src/pynchon.egg-info/requires.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        8 2023-05-02 18:42:12.000000 pynchon-2023.5.2.14.42/src/pynchon.egg-info/top_level.txt
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.408813 pynchon-2023.5.2.14.50/
+-rw-rw-r--   0 matt      (1000) matt      (1000)       50 2022-10-31 17:10:29.000000 pynchon-2023.5.2.14.50/MANIFEST.in
+-rw-rw-r--   0 matt      (1000) matt      (1000)      736 2023-05-02 18:50:00.408813 pynchon-2023.5.2.14.50/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)     6135 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.50/README.md
+-rw-rw-r--   0 matt      (1000) matt      (1000)      979 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/pyproject.toml
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1602 2023-05-02 18:50:00.408813 pynchon-2023.5.2.14.50/setup.cfg
+-rw-rw-r--   0 matt      (1000) matt      (1000)      730 2022-10-31 16:56:45.000000 pynchon-2023.5.2.14.50/setup.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.392812 pynchon-2023.5.2.14.50/src/
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.396813 pynchon-2023.5.2.14.50/src/pynchon/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      251 2023-04-30 02:08:52.000000 pynchon-2023.5.2.14.50/src/pynchon/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      100 2023-05-02 02:18:56.000000 pynchon-2023.5.2.14.50/src/pynchon/__main__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       77 2023-05-02 18:49:57.000000 pynchon-2023.5.2.14.50/src/pynchon/_version.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.396813 pynchon-2023.5.2.14.50/src/pynchon/abcs/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      262 2023-04-30 02:08:52.000000 pynchon-2023.5.2.14.50/src/pynchon/abcs/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1244 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/abcs/attrdict.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2431 2023-05-02 01:26:44.000000 pynchon-2023.5.2.14.50/src/pynchon/abcs/config.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2909 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/abcs/meta.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1254 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.50/src/pynchon/abcs/path.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      686 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/abcs/plugin.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4788 2023-05-02 02:11:29.000000 pynchon-2023.5.2.14.50/src/pynchon/abcs/visitor.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4336 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/annotate.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.396813 pynchon-2023.5.2.14.50/src/pynchon/api/
+-rw-rw-r--   0 matt      (1000) matt      (1000)       20 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.50/src/pynchon/api/__init__.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.396813 pynchon-2023.5.2.14.50/src/pynchon/api/git/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      109 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.50/src/pynchon/api/git/__init__.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.396813 pynchon-2023.5.2.14.50/src/pynchon/api/project/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1146 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/api/project/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       28 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.50/src/pynchon/api/pynchon.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2215 2023-05-02 02:11:29.000000 pynchon-2023.5.2.14.50/src/pynchon/api/render.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5154 2023-05-02 02:11:29.000000 pynchon-2023.5.2.14.50/src/pynchon/app.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.396813 pynchon-2023.5.2.14.50/src/pynchon/bin/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      972 2023-05-02 03:00:09.000000 pynchon-2023.5.2.14.50/src/pynchon/bin/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.50/src/pynchon/bin/cli.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.50/src/pynchon/bin/dot.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3318 2023-04-30 22:57:08.000000 pynchon-2023.5.2.14.50/src/pynchon/bin/entry.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.50/src/pynchon/bin/groups.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-28 03:58:20.000000 pynchon-2023.5.2.14.50/src/pynchon/bin/options.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.50/src/pynchon/bin/parse.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.50/src/pynchon/bin/render.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.396813 pynchon-2023.5.2.14.50/src/pynchon/cli/
+-rw-rw-r--   0 matt      (1000) matt      (1000)       54 2023-04-30 18:28:18.000000 pynchon-2023.5.2.14.50/src/pynchon/cli/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     6992 2023-05-02 02:54:32.000000 pynchon-2023.5.2.14.50/src/pynchon/cli/common.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2423 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.50/src/pynchon/cli/options.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2439 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.50/src/pynchon/click.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.396813 pynchon-2023.5.2.14.50/src/pynchon/config/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1824 2023-05-02 02:11:29.000000 pynchon-2023.5.2.14.50/src/pynchon/config/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4672 2023-04-30 17:56:47.000000 pynchon-2023.5.2.14.50/src/pynchon/config/util.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1059 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.50/src/pynchon/constants.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2856 2023-05-02 01:23:34.000000 pynchon-2023.5.2.14.50/src/pynchon/core.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      115 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.50/src/pynchon/events.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       27 2023-04-29 21:27:56.000000 pynchon-2023.5.2.14.50/src/pynchon/exceptions.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.400812 pynchon-2023.5.2.14.50/src/pynchon/fleks/
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-30 02:43:01.000000 pynchon-2023.5.2.14.50/src/pynchon/fleks/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     8460 2023-05-02 03:00:09.000000 pynchon-2023.5.2.14.50/src/pynchon/models.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.400812 pynchon-2023.5.2.14.50/src/pynchon/plugins/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1006 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/api.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       95 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/ast.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      473 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/cicd.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1593 2023-05-02 03:03:42.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/core.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-29 22:36:50.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/cut.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.400812 pynchon-2023.5.2.14.50/src/pynchon/plugins/doctor/
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/doctor/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5684 2023-05-02 05:37:02.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/dot.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      374 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/files.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2797 2023-05-02 05:30:45.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/fixme.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      351 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/gen.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.400812 pynchon-2023.5.2.14.50/src/pynchon/plugins/git/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      373 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/git/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2448 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/git/config.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      305 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/globals.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-28 01:24:33.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/hooks.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     6082 2023-05-02 18:49:46.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/jinja.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3527 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/json.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      722 2023-04-29 19:14:56.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/load.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.400812 pynchon-2023.5.2.14.50/src/pynchon/plugins/makefile/
+-rw-rw-r--   0 matt      (1000) matt      (1000)       52 2023-04-28 18:54:48.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/makefile/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      840 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/parse.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1149 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/plugins.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4548 2023-04-30 18:42:04.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/project.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.400812 pynchon-2023.5.2.14.50/src/pynchon/plugins/python/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      112 2023-04-28 01:24:33.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/python/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2709 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/python/api.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/python/ast.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     7490 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/python/cli.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-28 01:24:33.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/python/config.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      236 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/python/models.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1525 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/python/platform.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      456 2023-04-30 02:08:52.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/python/pypi.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      723 2023-04-29 19:14:56.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/release.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4781 2023-04-30 17:58:57.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/render.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       60 2023-04-28 22:07:13.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/rtd.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.400812 pynchon-2023.5.2.14.50/src/pynchon/plugins/scaffolding/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3434 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/scaffolding/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1156 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/scaffolding/config.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1266 2023-04-30 17:56:47.000000 pynchon-2023.5.2.14.50/src/pynchon/plugins/util.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.404813 pynchon-2023.5.2.14.50/src/pynchon/shimport/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      209 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.50/src/pynchon/shimport/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      562 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.50/src/pynchon/shimport/abcs.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-30 01:24:51.000000 pynchon-2023.5.2.14.50/src/pynchon/shimport/hooks.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-30 17:41:25.000000 pynchon-2023.5.2.14.50/src/pynchon/shimport/importing.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    12287 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.50/src/pynchon/shimport/models.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2390 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.50/src/pynchon/shimport/module.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-30 18:08:09.000000 pynchon-2023.5.2.14.50/src/pynchon/shimport/registry.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-30 01:29:20.000000 pynchon-2023.5.2.14.50/src/pynchon/shimport/types.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      538 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.50/src/pynchon/shimport/util.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       73 2023-04-30 02:08:52.000000 pynchon-2023.5.2.14.50/src/pynchon/tagging.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.392812 pynchon-2023.5.2.14.50/src/pynchon/templates/
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.404813 pynchon-2023.5.2.14.50/src/pynchon/templates/cookie_cutter/
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.50/src/pynchon/templates/cookie_cutter/.gitkeep
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.392812 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.392812 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.404813 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/github/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      295 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/github/header.md.j2
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.404813 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/Makefile.md.j2
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.404813 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/core/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      392 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/core/VERSIONS.md.j2
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.404813 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/fixme/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      164 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/fixme/FIXME.md.j2
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.392812 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/python/
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.404813 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/python/api/
+-rw-rw-r--   0 matt      (1000) matt      (1000)       34 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/python/api/TOC.md.j2
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1190 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/python/api/classes.md.j2
+-rw-rw-r--   0 matt      (1000) matt      (1000)      891 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/python/api/functions.md.j2
+-rw-rw-r--   0 matt      (1000) matt      (1000)      322 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/python/api/modules.md.j2
+-rw-rw-r--   0 matt      (1000) matt      (1000)      686 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/python/api/package.md.j2
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2985 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/python/api/toc2.md.j2
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.404813 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/python/cli/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      623 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/python/cli/TOC.md.j2
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/python/cli/cli-toc.md.j2
+-rw-rw-r--   0 matt      (1000) matt      (1000)      198 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/python/cli/detail.md.j2
+-rw-rw-r--   0 matt      (1000) matt      (1000)      253 2023-05-01 23:44:40.000000 pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/python/cli/main.module.md.j2
+-rw-rw-r--   0 matt      (1000) matt      (1000)      284 2023-04-27 22:45:44.000000 pynchon-2023.5.2.14.50/src/pynchon/testing.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.404813 pynchon-2023.5.2.14.50/src/pynchon/util/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2084 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/util/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1016 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/util/click.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4750 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/util/complexity.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      871 2023-04-30 02:08:52.000000 pynchon-2023.5.2.14.50/src/pynchon/util/config.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      577 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/util/events.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4348 2023-05-02 05:31:21.000000 pynchon-2023.5.2.14.50/src/pynchon/util/files.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1944 2023-05-02 02:11:29.000000 pynchon-2023.5.2.14.50/src/pynchon/util/lme.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      954 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/util/oop.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2423 2023-05-02 05:37:15.000000 pynchon-2023.5.2.14.50/src/pynchon/util/os.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2279 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/util/python.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2972 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/util/tagging.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      411 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/util/testing.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.404813 pynchon-2023.5.2.14.50/src/pynchon/util/text/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      837 2023-05-02 00:54:17.000000 pynchon-2023.5.2.14.50/src/pynchon/util/text/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      365 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.50/src/pynchon/util/text/__main__.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.404813 pynchon-2023.5.2.14.50/src/pynchon/util/text/loadf/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5301 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.50/src/pynchon/util/text/loadf/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1033 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.50/src/pynchon/util/text/loadf/__main__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1654 2023-05-02 18:49:46.000000 pynchon-2023.5.2.14.50/src/pynchon/util/text/loads.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.408813 pynchon-2023.5.2.14.50/src/pynchon/util/text/normalize/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      740 2023-04-30 03:53:04.000000 pynchon-2023.5.2.14.50/src/pynchon/util/text/normalize/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       40 2023-04-29 02:48:43.000000 pynchon-2023.5.2.14.50/src/pynchon/util/text/normalize/__main__.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.408813 pynchon-2023.5.2.14.50/src/pynchon/util/text/render/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5245 2023-05-01 23:54:56.000000 pynchon-2023.5.2.14.50/src/pynchon/util/text/render/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      963 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.50/src/pynchon/util/text/render/__main__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1171 2023-05-01 23:36:05.000000 pynchon-2023.5.2.14.50/src/pynchon/util/typing.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-05-02 18:50:00.396813 pynchon-2023.5.2.14.50/src/pynchon.egg-info/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      736 2023-05-02 18:50:00.000000 pynchon-2023.5.2.14.50/src/pynchon.egg-info/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4455 2023-05-02 18:50:00.000000 pynchon-2023.5.2.14.50/src/pynchon.egg-info/SOURCES.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        1 2023-05-02 18:50:00.000000 pynchon-2023.5.2.14.50/src/pynchon.egg-info/dependency_links.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)       46 2023-05-02 18:50:00.000000 pynchon-2023.5.2.14.50/src/pynchon.egg-info/entry_points.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        1 2023-05-02 18:50:00.000000 pynchon-2023.5.2.14.50/src/pynchon.egg-info/not-zip-safe
+-rw-rw-r--   0 matt      (1000) matt      (1000)      399 2023-05-02 18:50:00.000000 pynchon-2023.5.2.14.50/src/pynchon.egg-info/requires.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        8 2023-05-02 18:50:00.000000 pynchon-2023.5.2.14.50/src/pynchon.egg-info/top_level.txt
```

### Comparing `pynchon-2023.5.2.14.42/PKG-INFO` & `pynchon-2023.5.2.14.50/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynchon
-Version: 2023.5.2.14.42
+Version: 2023.5.2.14.50
 Summary: Autodocs for python projects
 Home-page: https://github.com/elo-enterprises/pynchon/
 Author: elo
 Author-email: engineering@elo.enterprises
 License: MIT
 Project-URL: Documentation, https://github.com/elo-enterprises/pynchon/
 Project-URL: Source, https://github.com/elo-enterprises/pynchon/
```

### Comparing `pynchon-2023.5.2.14.42/README.md` & `pynchon-2023.5.2.14.50/README.md`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/pyproject.toml` & `pynchon-2023.5.2.14.50/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/setup.cfg` & `pynchon-2023.5.2.14.50/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 	=src
 python_requires = >3.6
 install_requires = 
 	click
 	coloredlogs==15.0.1
 	memoized-property==1.0.3
 	memoization==0.4.0
-	json5==0.9.10
+	pyjson5==1.6.1
 	pygments
 	Jinja2==3.1.2
 	griffe==0.23.0
 	mccabe==0.7.0
 	pyyaml
 	termcolor
 	tomli # as tomllib; tomllib only available in py3.11
```

### Comparing `pynchon-2023.5.2.14.42/setup.py` & `pynchon-2023.5.2.14.50/setup.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/abcs/attrdict.py` & `pynchon-2023.5.2.14.50/src/pynchon/abcs/attrdict.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/abcs/config.py` & `pynchon-2023.5.2.14.50/src/pynchon/abcs/config.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/abcs/meta.py` & `pynchon-2023.5.2.14.50/src/pynchon/abcs/meta.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/abcs/path.py` & `pynchon-2023.5.2.14.50/src/pynchon/abcs/path.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/abcs/plugin.py` & `pynchon-2023.5.2.14.50/src/pynchon/abcs/plugin.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/abcs/visitor.py` & `pynchon-2023.5.2.14.50/src/pynchon/abcs/visitor.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/annotate.py` & `pynchon-2023.5.2.14.50/src/pynchon/annotate.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/api/project/__init__.py` & `pynchon-2023.5.2.14.50/src/pynchon/api/project/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/api/render.py` & `pynchon-2023.5.2.14.50/src/pynchon/api/render.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/app.py` & `pynchon-2023.5.2.14.50/src/pynchon/app.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/bin/__init__.py` & `pynchon-2023.5.2.14.50/src/pynchon/bin/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/bin/entry.py` & `pynchon-2023.5.2.14.50/src/pynchon/bin/entry.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/cli/common.py` & `pynchon-2023.5.2.14.50/src/pynchon/cli/common.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/cli/options.py` & `pynchon-2023.5.2.14.50/src/pynchon/cli/options.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/click.py` & `pynchon-2023.5.2.14.50/src/pynchon/click.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/config/__init__.py` & `pynchon-2023.5.2.14.50/src/pynchon/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/config/util.py` & `pynchon-2023.5.2.14.50/src/pynchon/config/util.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/constants.py` & `pynchon-2023.5.2.14.50/src/pynchon/constants.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/core.py` & `pynchon-2023.5.2.14.50/src/pynchon/core.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/models.py` & `pynchon-2023.5.2.14.50/src/pynchon/models.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/plugins/__init__.py` & `pynchon-2023.5.2.14.50/src/pynchon/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/plugins/core.py` & `pynchon-2023.5.2.14.50/src/pynchon/plugins/core.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/plugins/dot.py` & `pynchon-2023.5.2.14.50/src/pynchon/plugins/dot.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/plugins/fixme.py` & `pynchon-2023.5.2.14.50/src/pynchon/plugins/fixme.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/plugins/git/config.py` & `pynchon-2023.5.2.14.50/src/pynchon/plugins/git/config.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/plugins/jinja.py` & `pynchon-2023.5.2.14.50/src/pynchon/plugins/jinja.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         defaults = dict(
             # exclude_patterns=src/pynchon/templates/
         )
 
     def _get_exclude_patterns(self, config):
         """ """
         return list(
-            set(config.jinja['exclude_patterns'] + config.globals['exclude_patterns'])
+            set(config.jinja.get('exclude_patterns',[]) + config.globals['exclude_patterns'])
         )
 
     def _get_templates(self, config):
         """ """
         templates = config.jinja['template_includes']
         templates = [t for t in templates]
         templates = [f"--include {t}" for t in templates]
```

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/plugins/json.py` & `pynchon-2023.5.2.14.50/src/pynchon/plugins/json.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/plugins/load.py` & `pynchon-2023.5.2.14.50/src/pynchon/plugins/load.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/plugins/parse.py` & `pynchon-2023.5.2.14.50/src/pynchon/plugins/parse.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/plugins/plugins.py` & `pynchon-2023.5.2.14.50/src/pynchon/plugins/plugins.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/plugins/project.py` & `pynchon-2023.5.2.14.50/src/pynchon/plugins/project.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/plugins/python/api.py` & `pynchon-2023.5.2.14.50/src/pynchon/plugins/python/api.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/plugins/python/cli.py` & `pynchon-2023.5.2.14.50/src/pynchon/plugins/python/cli.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/plugins/python/platform.py` & `pynchon-2023.5.2.14.50/src/pynchon/plugins/python/platform.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/plugins/release.py` & `pynchon-2023.5.2.14.50/src/pynchon/plugins/release.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/plugins/render.py` & `pynchon-2023.5.2.14.50/src/pynchon/plugins/render.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/plugins/scaffolding/__init__.py` & `pynchon-2023.5.2.14.50/src/pynchon/plugins/scaffolding/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/plugins/scaffolding/config.py` & `pynchon-2023.5.2.14.50/src/pynchon/plugins/scaffolding/config.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/plugins/util.py` & `pynchon-2023.5.2.14.50/src/pynchon/plugins/util.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/shimport/abcs.py` & `pynchon-2023.5.2.14.50/src/pynchon/shimport/abcs.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/shimport/models.py` & `pynchon-2023.5.2.14.50/src/pynchon/shimport/models.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/shimport/module.py` & `pynchon-2023.5.2.14.50/src/pynchon/shimport/module.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/shimport/util.py` & `pynchon-2023.5.2.14.50/src/pynchon/shimport/util.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/python/api/classes.md.j2` & `pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/python/api/classes.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/python/api/functions.md.j2` & `pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/python/api/functions.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/python/api/package.md.j2` & `pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/python/api/package.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/python/api/toc2.md.j2` & `pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/python/api/toc2.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/templates/includes/pynchon/plugins/python/cli/TOC.md.j2` & `pynchon-2023.5.2.14.50/src/pynchon/templates/includes/pynchon/plugins/python/cli/TOC.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/util/__init__.py` & `pynchon-2023.5.2.14.50/src/pynchon/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/util/click.py` & `pynchon-2023.5.2.14.50/src/pynchon/util/click.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/util/complexity.py` & `pynchon-2023.5.2.14.50/src/pynchon/util/complexity.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/util/config.py` & `pynchon-2023.5.2.14.50/src/pynchon/util/config.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/util/events.py` & `pynchon-2023.5.2.14.50/src/pynchon/util/events.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/util/files.py` & `pynchon-2023.5.2.14.50/src/pynchon/util/files.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/util/lme.py` & `pynchon-2023.5.2.14.50/src/pynchon/util/lme.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/util/oop.py` & `pynchon-2023.5.2.14.50/src/pynchon/util/oop.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/util/os.py` & `pynchon-2023.5.2.14.50/src/pynchon/util/os.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/util/python.py` & `pynchon-2023.5.2.14.50/src/pynchon/util/python.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/util/tagging.py` & `pynchon-2023.5.2.14.50/src/pynchon/util/tagging.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/util/text/__init__.py` & `pynchon-2023.5.2.14.50/src/pynchon/util/text/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/util/text/loadf/__init__.py` & `pynchon-2023.5.2.14.50/src/pynchon/util/text/loadf/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/util/text/loadf/__main__.py` & `pynchon-2023.5.2.14.50/src/pynchon/util/text/loadf/__main__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/util/text/loads.py` & `pynchon-2023.5.2.14.50/src/pynchon/util/text/loads.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ pynchon.util.text.loads
 
     Helpers for loading data structures from strings
 """
 import json as json_mod
 
-import json5 as json5_mod
+import pyjson5 as json5_mod
 
 from pynchon.util import typing, lme
 
 LOGGER = lme.get_logger(__name__)
 
 
 def ini(content: str) -> typing.StringMaybe:
```

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/util/text/normalize/__init__.py` & `pynchon-2023.5.2.14.50/src/pynchon/util/text/normalize/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/util/text/render/__init__.py` & `pynchon-2023.5.2.14.50/src/pynchon/util/text/render/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/util/text/render/__main__.py` & `pynchon-2023.5.2.14.50/src/pynchon/util/text/render/__main__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon/util/typing.py` & `pynchon-2023.5.2.14.50/src/pynchon/util/typing.py`

 * *Files identical despite different names*

### Comparing `pynchon-2023.5.2.14.42/src/pynchon.egg-info/PKG-INFO` & `pynchon-2023.5.2.14.50/src/pynchon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynchon
-Version: 2023.5.2.14.42
+Version: 2023.5.2.14.50
 Summary: Autodocs for python projects
 Home-page: https://github.com/elo-enterprises/pynchon/
 Author: elo
 Author-email: engineering@elo.enterprises
 License: MIT
 Project-URL: Documentation, https://github.com/elo-enterprises/pynchon/
 Project-URL: Source, https://github.com/elo-enterprises/pynchon/
```

### Comparing `pynchon-2023.5.2.14.42/src/pynchon.egg-info/SOURCES.txt` & `pynchon-2023.5.2.14.50/src/pynchon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

