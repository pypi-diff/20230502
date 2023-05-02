# Comparing `tmp/invoke-2.1.0.tar.gz` & `tmp/invoke-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmpgntf1yl8/dist/invoke-2.1.0.tar", last modified: Fri Apr 28 20:11:51 2023, max compression
+gzip compressed data, was "/tmp/tmpj0msl5e0/dist/invoke-2.1.1.tar", last modified: Tue May  2 02:11:06 2023, max compression
```

## Comparing `invoke-2.1.0.tar` & `invoke-2.1.1.tar`

### file list

```diff
@@ -1,214 +1,217 @@
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/invoke/
--rw-r--r--   0 jforcier  (1000) users      (100)     5229 2023-04-28 20:11:24.000000 invoke-2.1.0/invoke/loader.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/invoke/parser/
--rw-r--r--   0 jforcier  (1000) users      (100)    19809 2023-04-28 19:57:26.000000 invoke-2.1.0/invoke/parser/parser.py
--rw-r--r--   0 jforcier  (1000) users      (100)      181 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/parser/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)     9815 2023-04-28 19:57:26.000000 invoke-2.1.0/invoke/parser/context.py
--rw-r--r--   0 jforcier  (1000) users      (100)     6045 2023-04-28 19:57:26.000000 invoke-2.1.0/invoke/parser/argument.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4394 2023-04-28 19:57:26.000000 invoke-2.1.0/invoke/env.py
--rw-r--r--   0 jforcier  (1000) users      (100)    10018 2023-04-28 19:57:26.000000 invoke-2.1.0/invoke/util.py
--rw-r--r--   0 jforcier  (1000) users      (100)      235 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/main.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/invoke/vendor/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/invoke/vendor/lexicon/
--rw-r--r--   0 jforcier  (1000) users      (100)      407 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/lexicon/attribute_dict.py
--rw-r--r--   0 jforcier  (1000) users      (100)       80 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/lexicon/_version.py
--rw-r--r--   0 jforcier  (1000) users      (100)     3223 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/lexicon/alias_dict.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1133 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/lexicon/__init__.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/invoke/vendor/yaml/
--rw-r--r--   0 jforcier  (1000) users      (100)     4883 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/yaml/composer.py
--rw-r--r--   0 jforcier  (1000) users      (100)    43006 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/yaml/emitter.py
--rw-r--r--   0 jforcier  (1000) users      (100)    25495 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/yaml/parser.py
--rw-r--r--   0 jforcier  (1000) users      (100)    13170 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/yaml/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2533 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/yaml/error.py
--rw-r--r--   0 jforcier  (1000) users      (100)    14184 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/yaml/representer.py
--rw-r--r--   0 jforcier  (1000) users      (100)     3851 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/yaml/cyaml.py
--rw-r--r--   0 jforcier  (1000) users      (100)     8999 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/yaml/resolver.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4165 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/yaml/serializer.py
--rw-r--r--   0 jforcier  (1000) users      (100)     6794 2023-02-16 19:54:22.000000 invoke-2.1.0/invoke/vendor/yaml/reader.py
--rw-r--r--   0 jforcier  (1000) users      (100)    51277 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/yaml/scanner.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2837 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/yaml/dumper.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1440 2023-02-16 19:54:22.000000 invoke-2.1.0/invoke/vendor/yaml/nodes.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2445 2023-02-16 19:54:22.000000 invoke-2.1.0/invoke/vendor/yaml/events.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2573 2023-02-16 19:54:22.000000 invoke-2.1.0/invoke/vendor/yaml/tokens.py
--rw-r--r--   0 jforcier  (1000) users      (100)    28639 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/yaml/constructor.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2061 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/yaml/loader.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/invoke/vendor/fluidity/
--rw-r--r--   0 jforcier  (1000) users      (100)      135 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/fluidity/backwardscompat.py
--rw-r--r--   0 jforcier  (1000) users      (100)      196 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/fluidity/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)     8686 2023-02-16 19:54:22.000000 invoke-2.1.0/invoke/vendor/fluidity/machine.py
--rw-r--r--   0 jforcier  (1000) users      (100)        0 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/vendor/__init__.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/invoke/completion/
--rw-r--r--   0 jforcier  (1000) users      (100)        0 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/completion/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5222 2023-04-28 19:57:26.000000 invoke-2.1.0/invoke/completion/complete.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1356 2021-12-23 21:30:34.000000 invoke-2.1.0/invoke/completion/bash.completion
--rw-r--r--   0 jforcier  (1000) users      (100)     1429 2021-12-23 21:30:34.000000 invoke-2.1.0/invoke/completion/zsh.completion
--rw-r--r--   0 jforcier  (1000) users      (100)      382 2021-12-23 21:30:34.000000 invoke-2.1.0/invoke/completion/fish.completion
--rw-r--r--   0 jforcier  (1000) users      (100)       47 2023-02-16 19:54:15.000000 invoke-2.1.0/invoke/__main__.py
--rw-r--r--   0 jforcier  (1000) users      (100)    23060 2023-04-28 19:57:26.000000 invoke-2.1.0/invoke/collection.py
--rw-r--r--   0 jforcier  (1000) users      (100)    50005 2023-04-28 20:11:24.000000 invoke-2.1.0/invoke/config.py
--rw-r--r--   0 jforcier  (1000) users      (100)       80 2023-04-28 20:11:50.000000 invoke-2.1.0/invoke/_version.py
--rw-r--r--   0 jforcier  (1000) users      (100)    12227 2023-04-28 19:57:26.000000 invoke-2.1.0/invoke/exceptions.py
--rw-r--r--   0 jforcier  (1000) users      (100)    25486 2023-04-28 19:57:26.000000 invoke-2.1.0/invoke/context.py
--rw-r--r--   0 jforcier  (1000) users      (100)     8065 2023-04-28 19:57:26.000000 invoke-2.1.0/invoke/terminals.py
--rw-r--r--   0 jforcier  (1000) users      (100)    38177 2023-04-28 19:58:26.000000 invoke-2.1.0/invoke/program.py
--rw-r--r--   0 jforcier  (1000) users      (100)    65307 2023-04-28 19:57:26.000000 invoke-2.1.0/invoke/runners.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5097 2023-04-28 19:57:26.000000 invoke-2.1.0/invoke/watchers.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2229 2023-04-28 19:57:26.000000 invoke-2.1.0/invoke/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)    19946 2023-04-28 19:57:26.000000 invoke-2.1.0/invoke/tasks.py
--rw-r--r--   0 jforcier  (1000) users      (100)     8855 2023-04-28 19:57:26.000000 invoke-2.1.0/invoke/executor.py
--rw-r--r--   0 jforcier  (1000) users      (100)     3290 2023-04-28 20:11:51.000000 invoke-2.1.0/PKG-INFO
--rw-r--r--   0 jforcier  (1000) users      (100)     1314 2021-12-23 21:30:34.000000 invoke-2.1.0/LICENSE
--rw-r--r--   0 jforcier  (1000) users      (100)     4061 2023-04-28 19:57:26.000000 invoke-2.1.0/tasks.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1250 2023-04-28 19:57:26.000000 invoke-2.1.0/pyproject.toml
--rw-r--r--   0 jforcier  (1000) users      (100)     2711 2023-02-17 20:13:42.000000 invoke-2.1.0/setup.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/invoke.egg-info/
--rw-r--r--   0 jforcier  (1000) users      (100)        7 2023-04-28 20:11:50.000000 invoke-2.1.0/invoke.egg-info/top_level.txt
--rw-r--r--   0 jforcier  (1000) users      (100)     3290 2023-04-28 20:11:50.000000 invoke-2.1.0/invoke.egg-info/PKG-INFO
--rw-r--r--   0 jforcier  (1000) users      (100)       82 2023-04-28 20:11:50.000000 invoke-2.1.0/invoke.egg-info/entry_points.txt
--rw-r--r--   0 jforcier  (1000) users      (100)        1 2023-04-28 20:11:50.000000 invoke-2.1.0/invoke.egg-info/dependency_links.txt
--rw-r--r--   0 jforcier  (1000) users      (100)     5066 2023-04-28 20:11:50.000000 invoke-2.1.0/invoke.egg-info/SOURCES.txt
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/tests/
--rw-r--r--   0 jforcier  (1000) users      (100)    17268 2023-02-17 20:13:42.000000 invoke-2.1.0/tests/task.py
--rw-r--r--   0 jforcier  (1000) users      (100)    33509 2023-02-17 20:13:42.000000 invoke-2.1.0/tests/collection.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4100 2023-04-28 20:11:24.000000 invoke-2.1.0/tests/loader.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1661 2023-02-17 20:13:42.000000 invoke-2.1.0/tests/util.py
--rw-r--r--   0 jforcier  (1000) users      (100)     9820 2023-02-17 20:13:42.000000 invoke-2.1.0/tests/_util.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/tests/_support/
--rw-r--r--   0 jforcier  (1000) users      (100)        7 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/empty.py
--rw-r--r--   0 jforcier  (1000) users      (100)      264 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/explicit_root.py
--rw-r--r--   0 jforcier  (1000) users      (100)      178 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/simple_ns_list.py
--rw-r--r--   0 jforcier  (1000) users      (100)       44 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/oops.py
--rw-r--r--   0 jforcier  (1000) users      (100)      226 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/foo.py
--rw-r--r--   0 jforcier  (1000) users      (100)       99 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/debugging.py
--rw-r--r--   0 jforcier  (1000) users      (100)       57 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/custom_executor.py
--rw-r--r--   0 jforcier  (1000) users      (100)      157 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/sudo_prompt.py
--rw-r--r--   0 jforcier  (1000) users      (100)      194 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/deeper_ns_list.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/tests/_support/ignoreme/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/tests/_support/ignoreme/ignoremetoo/
--rw-r--r--   0 jforcier  (1000) users      (100)        0 2021-12-23 21:30:34.000000 invoke-2.1.0/tests/_support/ignoreme/ignoremetoo/.no
--rw-r--r--   0 jforcier  (1000) users      (100)      116 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/decorator_multi_default.py
--rw-r--r--   0 jforcier  (1000) users      (100)      365 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/autoprint.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/tests/_support/configs/
--rw-r--r--   0 jforcier  (1000) users      (100)       18 2021-12-23 21:30:34.000000 invoke-2.1.0/tests/_support/configs/echo.yaml
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/tests/_support/configs/underscores/
--rw-r--r--   0 jforcier  (1000) users      (100)       68 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/configs/underscores/tasks.py
--rw-r--r--   0 jforcier  (1000) users      (100)       32 2021-12-23 21:30:34.000000 invoke-2.1.0/tests/_support/configs/underscores/invoke.yaml
--rw-r--r--   0 jforcier  (1000) users      (100)       19 2021-12-23 21:30:34.000000 invoke-2.1.0/tests/_support/configs/no-echo.yaml
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/tests/_support/configs/json/
--rw-r--r--   0 jforcier  (1000) users      (100)       41 2021-12-23 21:30:34.000000 invoke-2.1.0/tests/_support/configs/json/invoke.json
--rw-r--r--   0 jforcier  (1000) users      (100)       23 2021-12-23 21:30:34.000000 invoke-2.1.0/tests/_support/configs/no-dedupe.yaml
--rw-r--r--   0 jforcier  (1000) users      (100)       89 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/configs/runtime.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/tests/_support/configs/three-of-em/
--rw-r--r--   0 jforcier  (1000) users      (100)       44 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/configs/three-of-em/invoke.py
--rw-r--r--   0 jforcier  (1000) users      (100)       46 2021-12-23 21:30:34.000000 invoke-2.1.0/tests/_support/configs/three-of-em/invoke.json
--rw-r--r--   0 jforcier  (1000) users      (100)       38 2021-12-23 21:30:34.000000 invoke-2.1.0/tests/_support/configs/three-of-em/invoke.yml
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/tests/_support/configs/json-and-python/
--rw-r--r--   0 jforcier  (1000) users      (100)       46 2021-12-23 21:30:34.000000 invoke-2.1.0/tests/_support/configs/json-and-python/invoke.json
--rw-r--r--   0 jforcier  (1000) users      (100)       44 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/configs/json-and-python/invoke.py
--rw-r--r--   0 jforcier  (1000) users      (100)      173 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/configs/collection.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/tests/_support/configs/yaml/
--rw-r--r--   0 jforcier  (1000) users      (100)       89 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/configs/yaml/tasks.py
--rw-r--r--   0 jforcier  (1000) users      (100)      127 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/configs/yaml/explicit.py
--rw-r--r--   0 jforcier  (1000) users      (100)       35 2021-12-23 21:30:34.000000 invoke-2.1.0/tests/_support/configs/yaml/invoke.yaml
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/tests/_support/configs/yml/
--rw-r--r--   0 jforcier  (1000) users      (100)       88 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/configs/yml/tasks.py
--rw-r--r--   0 jforcier  (1000) users      (100)      126 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/configs/yml/explicit.py
--rw-r--r--   0 jforcier  (1000) users      (100)       34 2021-12-23 21:30:34.000000 invoke-2.1.0/tests/_support/configs/yml/invoke.yml
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/tests/_support/configs/nested/
--rw-r--r--   0 jforcier  (1000) users      (100)       35 2021-12-23 21:30:34.000000 invoke-2.1.0/tests/_support/configs/nested/invoke.yaml
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/tests/_support/configs/all-four/
--rw-r--r--   0 jforcier  (1000) users      (100)       40 2021-12-23 21:30:34.000000 invoke-2.1.0/tests/_support/configs/all-four/invoke.yaml
--rw-r--r--   0 jforcier  (1000) users      (100)       38 2021-12-23 21:30:34.000000 invoke-2.1.0/tests/_support/configs/all-four/invoke.yml
--rw-r--r--   0 jforcier  (1000) users      (100)       46 2021-12-23 21:30:34.000000 invoke-2.1.0/tests/_support/configs/all-four/invoke.json
--rw-r--r--   0 jforcier  (1000) users      (100)       44 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/configs/all-four/invoke.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/tests/_support/configs/python/
--rw-r--r--   0 jforcier  (1000) users      (100)       40 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/configs/python/invoke.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/tests/_support/package/
--rw-r--r--   0 jforcier  (1000) users      (100)        0 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/package/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)       56 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/package/module.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4146 2021-12-23 21:30:34.000000 invoke-2.1.0/tests/_support/tree.json
--rw-r--r--   0 jforcier  (1000) users      (100)       78 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/alias_sorting.py
--rw-r--r--   0 jforcier  (1000) users      (100)      395 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/contextualized.py
--rw-r--r--   0 jforcier  (1000) users      (100)       35 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/has_modules.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/tests/_support/branch/
--rw-r--r--   0 jforcier  (1000) users      (100)       73 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/branch/explicit.py
--rw-r--r--   0 jforcier  (1000) users      (100)       86 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/branch/tasks.py
--rw-r--r--   0 jforcier  (1000) users      (100)      919 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/decorators.py
--rw-r--r--   0 jforcier  (1000) users      (100)      276 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/docstrings.py
--rw-r--r--   0 jforcier  (1000) users      (100)      511 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/depth_first.py
--rw-r--r--   0 jforcier  (1000) users      (100)      425 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/nontrivial_docstrings.py
--rw-r--r--   0 jforcier  (1000) users      (100)      188 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/namespacing.py
--rw-r--r--   0 jforcier  (1000) users      (100)      666 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/integration.py
--rw-r--r--   0 jforcier  (1000) users      (100)      121 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/empty_subcollection.py
--rw-r--r--   0 jforcier  (1000) users      (100)       85 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/subcollection_task_name.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/tests/_support/tree/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/tests/_support/tree/build/
--rw-r--r--   0 jforcier  (1000) users      (100)      274 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/tree/build/docs.py
--rw-r--r--   0 jforcier  (1000) users      (100)      278 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/tree/build/python.py
--rw-r--r--   0 jforcier  (1000) users      (100)      421 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/tree/build/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)      301 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/tree/deploy.py
--rw-r--r--   0 jforcier  (1000) users      (100)      171 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/tree/provision.py
--rw-r--r--   0 jforcier  (1000) users      (100)      653 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/tree/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)       96 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/_support/tasks.py
--rw-r--r--   0 jforcier  (1000) users      (100)    12415 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/executor.py
--rw-r--r--   0 jforcier  (1000) users      (100)    12116 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/parser_context.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4239 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/watchers.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2895 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/conftest.py
--rw-r--r--   0 jforcier  (1000) users      (100)     3261 2023-02-17 20:13:42.000000 invoke-2.1.0/tests/concurrency.py
--rw-r--r--   0 jforcier  (1000) users      (100)    44633 2023-02-17 20:13:42.000000 invoke-2.1.0/tests/config.py
--rw-r--r--   0 jforcier  (1000) users      (100)    70272 2023-02-17 20:13:42.000000 invoke-2.1.0/tests/runners.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4053 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/init.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4550 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/merge_dicts.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5361 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/cli.py
--rw-r--r--   0 jforcier  (1000) users      (100)    29680 2023-02-17 20:13:42.000000 invoke-2.1.0/tests/context.py
--rw-r--r--   0 jforcier  (1000) users      (100)     7687 2023-02-17 20:13:42.000000 invoke-2.1.0/tests/completion.py
--rw-r--r--   0 jforcier  (1000) users      (100)    56042 2023-04-28 19:58:26.000000 invoke-2.1.0/tests/program.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2945 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/terminals.py
--rw-r--r--   0 jforcier  (1000) users      (100)    22668 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/parser_parser.py
--rw-r--r--   0 jforcier  (1000) users      (100)     7179 2023-02-16 19:54:15.000000 invoke-2.1.0/tests/parser_argument.py
--rw-r--r--   0 jforcier  (1000) users      (100)      437 2023-04-28 19:58:12.000000 invoke-2.1.0/dev-requirements.txt
--rw-r--r--   0 jforcier  (1000) users      (100)     1328 2022-05-11 15:59:13.000000 invoke-2.1.0/README.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       38 2023-04-28 20:11:51.000000 invoke-2.1.0/setup.cfg
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/sites/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/sites/www/
--rw-r--r--   0 jforcier  (1000) users      (100)     2537 2022-03-25 22:40:47.000000 invoke-2.1.0/sites/www/prior-art.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      753 2023-01-07 00:40:50.000000 invoke-2.1.0/sites/www/installing.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     1791 2022-05-11 15:59:13.000000 invoke-2.1.0/sites/www/development.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     1218 2022-05-11 15:59:13.000000 invoke-2.1.0/sites/www/contact.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     8153 2023-01-07 00:40:50.000000 invoke-2.1.0/sites/www/faq.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      703 2023-02-16 19:54:15.000000 invoke-2.1.0/sites/www/conf.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2801 2022-05-11 15:59:13.000000 invoke-2.1.0/sites/www/index.rst
--rw-r--r--   0 jforcier  (1000) users      (100)    76512 2023-04-28 20:11:47.000000 invoke-2.1.0/sites/www/changelog.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     1367 2023-02-16 19:54:15.000000 invoke-2.1.0/sites/shared_conf.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/sites/docs/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/sites/docs/concepts/
--rw-r--r--   0 jforcier  (1000) users      (100)    16705 2023-01-07 00:40:53.000000 invoke-2.1.0/sites/docs/concepts/invoking-tasks.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     9234 2023-02-17 20:13:42.000000 invoke-2.1.0/sites/docs/concepts/library.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     2424 2022-03-25 22:40:47.000000 invoke-2.1.0/sites/docs/concepts/watchers.rst
--rw-r--r--   0 jforcier  (1000) users      (100)    17701 2023-01-07 00:40:50.000000 invoke-2.1.0/sites/docs/concepts/configuration.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     2917 2022-05-11 15:59:13.000000 invoke-2.1.0/sites/docs/concepts/loading.rst
--rw-r--r--   0 jforcier  (1000) users      (100)    10180 2023-01-07 00:40:50.000000 invoke-2.1.0/sites/docs/concepts/testing.rst
--rw-r--r--   0 jforcier  (1000) users      (100)    11750 2022-03-25 22:40:47.000000 invoke-2.1.0/sites/docs/concepts/namespaces.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     7640 2022-05-11 15:59:13.000000 invoke-2.1.0/sites/docs/getting-started.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      445 2023-02-16 19:54:15.000000 invoke-2.1.0/sites/docs/conf.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/sites/docs/_static/
--rw-r--r--   0 jforcier  (1000) users      (100)    15260 2021-12-23 21:30:34.000000 invoke-2.1.0/sites/docs/_static/rtd.css
--rw-r--r--   0 jforcier  (1000) users      (100)      943 2022-05-11 15:59:13.000000 invoke-2.1.0/sites/docs/index.rst
--rw-r--r--   0 jforcier  (1000) users      (100)    12466 2022-05-11 15:59:13.000000 invoke-2.1.0/sites/docs/invoke.rst
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-28 20:11:51.000000 invoke-2.1.0/sites/docs/api/
--rw-r--r--   0 jforcier  (1000) users      (100)       96 2022-03-25 22:40:47.000000 invoke-2.1.0/sites/docs/api/runners.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       68 2022-03-25 22:40:47.000000 invoke-2.1.0/sites/docs/api/program.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       60 2022-03-25 22:40:47.000000 invoke-2.1.0/sites/docs/api/tasks.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       80 2022-03-25 22:40:47.000000 invoke-2.1.0/sites/docs/api/executor.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      157 2022-03-25 22:40:47.000000 invoke-2.1.0/sites/docs/api/util.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       72 2022-03-25 22:40:47.000000 invoke-2.1.0/sites/docs/api/watchers.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       80 2022-03-25 22:40:47.000000 invoke-2.1.0/sites/docs/api/exceptions.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       63 2022-03-25 22:40:47.000000 invoke-2.1.0/sites/docs/api/__init__.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       68 2022-03-25 22:40:47.000000 invoke-2.1.0/sites/docs/api/context.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      229 2022-03-25 22:40:47.000000 invoke-2.1.0/sites/docs/api/loader.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      156 2022-03-25 22:40:47.000000 invoke-2.1.0/sites/docs/api/collection.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      401 2023-01-12 23:12:21.000000 invoke-2.1.0/sites/docs/api/parser.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       76 2022-03-25 22:40:47.000000 invoke-2.1.0/sites/docs/api/terminals.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       64 2022-03-25 22:40:47.000000 invoke-2.1.0/sites/docs/api/config.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      273 2022-03-18 21:53:07.000000 invoke-2.1.0/MANIFEST.in
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 02:11:06.000000 invoke-2.1.1/
+-rw-r--r--   0 jforcier  (1000) users      (100)     1314 2021-12-23 21:30:34.000000 invoke-2.1.1/LICENSE
+-rw-r--r--   0 jforcier  (1000) users      (100)     1328 2022-05-11 15:59:13.000000 invoke-2.1.1/README.rst
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 02:11:06.000000 invoke-2.1.1/sites/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 02:11:06.000000 invoke-2.1.1/sites/www/
+-rw-r--r--   0 jforcier  (1000) users      (100)     2537 2022-03-25 22:40:47.000000 invoke-2.1.1/sites/www/prior-art.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     8153 2023-01-07 00:40:50.000000 invoke-2.1.1/sites/www/faq.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      703 2023-02-16 19:54:15.000000 invoke-2.1.1/sites/www/conf.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2801 2022-05-11 15:59:13.000000 invoke-2.1.1/sites/www/index.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     1791 2022-05-11 15:59:13.000000 invoke-2.1.1/sites/www/development.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)    77066 2023-05-02 02:11:03.000000 invoke-2.1.1/sites/www/changelog.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     1218 2022-05-11 15:59:13.000000 invoke-2.1.1/sites/www/contact.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      753 2023-01-07 00:40:50.000000 invoke-2.1.1/sites/www/installing.rst
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 02:11:06.000000 invoke-2.1.1/sites/docs/
+-rw-r--r--   0 jforcier  (1000) users      (100)    12466 2022-05-11 15:59:13.000000 invoke-2.1.1/sites/docs/invoke.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      943 2022-05-11 15:59:13.000000 invoke-2.1.1/sites/docs/index.rst
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 02:11:06.000000 invoke-2.1.1/sites/docs/concepts/
+-rw-r--r--   0 jforcier  (1000) users      (100)    10180 2023-01-07 00:40:50.000000 invoke-2.1.1/sites/docs/concepts/testing.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     2424 2022-03-25 22:40:47.000000 invoke-2.1.1/sites/docs/concepts/watchers.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     2917 2022-05-11 15:59:13.000000 invoke-2.1.1/sites/docs/concepts/loading.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)    11750 2022-03-25 22:40:47.000000 invoke-2.1.1/sites/docs/concepts/namespaces.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)    16705 2023-01-07 00:40:53.000000 invoke-2.1.1/sites/docs/concepts/invoking-tasks.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     9234 2023-02-17 20:13:42.000000 invoke-2.1.1/sites/docs/concepts/library.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)    17701 2023-01-07 00:40:50.000000 invoke-2.1.1/sites/docs/concepts/configuration.rst
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 02:11:06.000000 invoke-2.1.1/sites/docs/api/
+-rw-r--r--   0 jforcier  (1000) users      (100)       68 2022-03-25 22:40:47.000000 invoke-2.1.1/sites/docs/api/context.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      157 2022-03-25 22:40:47.000000 invoke-2.1.1/sites/docs/api/util.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      401 2023-01-12 23:12:21.000000 invoke-2.1.1/sites/docs/api/parser.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       64 2022-03-25 22:40:47.000000 invoke-2.1.1/sites/docs/api/config.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       76 2022-03-25 22:40:47.000000 invoke-2.1.1/sites/docs/api/terminals.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       80 2022-03-25 22:40:47.000000 invoke-2.1.1/sites/docs/api/executor.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       72 2022-03-25 22:40:47.000000 invoke-2.1.1/sites/docs/api/watchers.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      229 2022-03-25 22:40:47.000000 invoke-2.1.1/sites/docs/api/loader.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       80 2022-03-25 22:40:47.000000 invoke-2.1.1/sites/docs/api/exceptions.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       68 2022-03-25 22:40:47.000000 invoke-2.1.1/sites/docs/api/program.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       96 2022-03-25 22:40:47.000000 invoke-2.1.1/sites/docs/api/runners.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       63 2022-03-25 22:40:47.000000 invoke-2.1.1/sites/docs/api/__init__.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       60 2022-03-25 22:40:47.000000 invoke-2.1.1/sites/docs/api/tasks.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      156 2022-03-25 22:40:47.000000 invoke-2.1.1/sites/docs/api/collection.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      445 2023-02-16 19:54:15.000000 invoke-2.1.1/sites/docs/conf.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 02:11:06.000000 invoke-2.1.1/sites/docs/_static/
+-rw-r--r--   0 jforcier  (1000) users      (100)    15260 2021-12-23 21:30:34.000000 invoke-2.1.1/sites/docs/_static/rtd.css
+-rw-r--r--   0 jforcier  (1000) users      (100)     7640 2022-05-11 15:59:13.000000 invoke-2.1.1/sites/docs/getting-started.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     1367 2023-02-16 19:54:15.000000 invoke-2.1.1/sites/shared_conf.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     3290 2023-05-02 02:11:06.000000 invoke-2.1.1/PKG-INFO
+-rw-r--r--   0 jforcier  (1000) users      (100)      273 2022-03-18 21:53:07.000000 invoke-2.1.1/MANIFEST.in
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 02:11:06.000000 invoke-2.1.1/invoke.egg-info/
+-rw-r--r--   0 jforcier  (1000) users      (100)     3290 2023-05-02 02:11:06.000000 invoke-2.1.1/invoke.egg-info/PKG-INFO
+-rw-r--r--   0 jforcier  (1000) users      (100)        1 2023-05-02 02:11:06.000000 invoke-2.1.1/invoke.egg-info/dependency_links.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)     5136 2023-05-02 02:11:06.000000 invoke-2.1.1/invoke.egg-info/SOURCES.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)       82 2023-05-02 02:11:06.000000 invoke-2.1.1/invoke.egg-info/entry_points.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)        7 2023-05-02 02:11:06.000000 invoke-2.1.1/invoke.egg-info/top_level.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)     2711 2023-02-17 20:13:42.000000 invoke-2.1.1/setup.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4061 2023-05-02 02:04:35.000000 invoke-2.1.1/tasks.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      437 2023-05-02 02:04:35.000000 invoke-2.1.1/dev-requirements.txt
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 02:11:06.000000 invoke-2.1.1/tests/
+-rw-r--r--   0 jforcier  (1000) users      (100)     7179 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/parser_argument.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4053 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/init.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 02:11:06.000000 invoke-2.1.1/tests/_support/
+-rw-r--r--   0 jforcier  (1000) users      (100)       85 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/subcollection_task_name.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       35 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/has_modules.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       96 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/tasks.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      425 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/nontrivial_docstrings.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      395 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/contextualized.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      121 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/empty_subcollection.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      666 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/integration.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      189 2023-05-02 02:04:46.000000 invoke-2.1.1/tests/_support/namespacing.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 02:11:06.000000 invoke-2.1.1/tests/_support/package/
+-rw-r--r--   0 jforcier  (1000) users      (100)       77 2023-05-02 02:04:46.000000 invoke-2.1.1/tests/_support/package/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       56 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/package/module.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      511 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/depth_first.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 02:11:06.000000 invoke-2.1.1/tests/_support/branch/
+-rw-r--r--   0 jforcier  (1000) users      (100)       73 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/branch/explicit.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       86 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/branch/tasks.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      264 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/explicit_root.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      116 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/decorator_multi_default.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      178 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/simple_ns_list.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 02:11:06.000000 invoke-2.1.1/tests/_support/ignoreme/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 02:11:06.000000 invoke-2.1.1/tests/_support/ignoreme/ignoremetoo/
+-rw-r--r--   0 jforcier  (1000) users      (100)        0 2021-12-23 21:30:34.000000 invoke-2.1.1/tests/_support/ignoreme/ignoremetoo/.no
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 02:11:06.000000 invoke-2.1.1/tests/_support/configs/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 02:11:06.000000 invoke-2.1.1/tests/_support/configs/yml/
+-rw-r--r--   0 jforcier  (1000) users      (100)       88 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/configs/yml/tasks.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      126 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/configs/yml/explicit.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       34 2021-12-23 21:30:34.000000 invoke-2.1.1/tests/_support/configs/yml/invoke.yml
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 02:11:06.000000 invoke-2.1.1/tests/_support/configs/three-of-em/
+-rw-r--r--   0 jforcier  (1000) users      (100)       46 2021-12-23 21:30:34.000000 invoke-2.1.1/tests/_support/configs/three-of-em/invoke.json
+-rw-r--r--   0 jforcier  (1000) users      (100)       44 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/configs/three-of-em/invoke.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       38 2021-12-23 21:30:34.000000 invoke-2.1.1/tests/_support/configs/three-of-em/invoke.yml
+-rw-r--r--   0 jforcier  (1000) users      (100)      173 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/configs/collection.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 02:11:06.000000 invoke-2.1.1/tests/_support/configs/all-four/
+-rw-r--r--   0 jforcier  (1000) users      (100)       44 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/configs/all-four/invoke.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       38 2021-12-23 21:30:34.000000 invoke-2.1.1/tests/_support/configs/all-four/invoke.yml
+-rw-r--r--   0 jforcier  (1000) users      (100)       40 2021-12-23 21:30:34.000000 invoke-2.1.1/tests/_support/configs/all-four/invoke.yaml
+-rw-r--r--   0 jforcier  (1000) users      (100)       46 2021-12-23 21:30:34.000000 invoke-2.1.1/tests/_support/configs/all-four/invoke.json
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 02:11:06.000000 invoke-2.1.1/tests/_support/configs/json/
+-rw-r--r--   0 jforcier  (1000) users      (100)       41 2021-12-23 21:30:34.000000 invoke-2.1.1/tests/_support/configs/json/invoke.json
+-rw-r--r--   0 jforcier  (1000) users      (100)       23 2021-12-23 21:30:34.000000 invoke-2.1.1/tests/_support/configs/no-dedupe.yaml
+-rw-r--r--   0 jforcier  (1000) users      (100)       89 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/configs/runtime.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 02:11:06.000000 invoke-2.1.1/tests/_support/configs/underscores/
+-rw-r--r--   0 jforcier  (1000) users      (100)       32 2021-12-23 21:30:34.000000 invoke-2.1.1/tests/_support/configs/underscores/invoke.yaml
+-rw-r--r--   0 jforcier  (1000) users      (100)       68 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/configs/underscores/tasks.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 02:11:06.000000 invoke-2.1.1/tests/_support/configs/python/
+-rw-r--r--   0 jforcier  (1000) users      (100)       40 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/configs/python/invoke.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       19 2021-12-23 21:30:34.000000 invoke-2.1.1/tests/_support/configs/no-echo.yaml
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 02:11:06.000000 invoke-2.1.1/tests/_support/configs/yaml/
+-rw-r--r--   0 jforcier  (1000) users      (100)      127 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/configs/yaml/explicit.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       89 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/configs/yaml/tasks.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       35 2021-12-23 21:30:34.000000 invoke-2.1.1/tests/_support/configs/yaml/invoke.yaml
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 02:11:06.000000 invoke-2.1.1/tests/_support/configs/nested/
+-rw-r--r--   0 jforcier  (1000) users      (100)       35 2021-12-23 21:30:34.000000 invoke-2.1.1/tests/_support/configs/nested/invoke.yaml
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 02:11:06.000000 invoke-2.1.1/tests/_support/configs/json-and-python/
+-rw-r--r--   0 jforcier  (1000) users      (100)       44 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/configs/json-and-python/invoke.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       46 2021-12-23 21:30:34.000000 invoke-2.1.1/tests/_support/configs/json-and-python/invoke.json
+-rw-r--r--   0 jforcier  (1000) users      (100)       18 2021-12-23 21:30:34.000000 invoke-2.1.1/tests/_support/configs/echo.yaml
+-rw-r--r--   0 jforcier  (1000) users      (100)      157 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/sudo_prompt.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4146 2021-12-23 21:30:34.000000 invoke-2.1.1/tests/_support/tree.json
+-rw-r--r--   0 jforcier  (1000) users      (100)      194 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/deeper_ns_list.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       57 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/custom_executor.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      365 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/autoprint.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       44 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/oops.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      276 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/docstrings.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      919 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/decorators.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       78 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/alias_sorting.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 02:11:06.000000 invoke-2.1.1/tests/_support/tree/
+-rw-r--r--   0 jforcier  (1000) users      (100)      653 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/tree/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      171 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/tree/provision.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 02:11:06.000000 invoke-2.1.1/tests/_support/tree/build/
+-rw-r--r--   0 jforcier  (1000) users      (100)      274 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/tree/build/docs.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      278 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/tree/build/python.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      421 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/tree/build/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      301 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/tree/deploy.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 02:11:06.000000 invoke-2.1.1/tests/_support/subspace/
+-rw-r--r--   0 jforcier  (1000) users      (100)       56 2023-05-02 02:04:46.000000 invoke-2.1.1/tests/_support/subspace/module.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       77 2023-05-02 02:04:46.000000 invoke-2.1.1/tests/_support/subspace/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)        7 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/empty.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       99 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/debugging.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      226 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/_support/foo.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    33509 2023-02-17 20:13:42.000000 invoke-2.1.1/tests/collection.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     9820 2023-02-17 20:13:42.000000 invoke-2.1.1/tests/_util.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    56042 2023-04-28 19:58:26.000000 invoke-2.1.1/tests/program.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4550 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/merge_dicts.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4239 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/watchers.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2945 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/terminals.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    29680 2023-02-17 20:13:42.000000 invoke-2.1.1/tests/context.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    12415 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/executor.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2895 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/conftest.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    70584 2023-04-29 19:30:04.000000 invoke-2.1.1/tests/runners.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    44633 2023-02-17 20:13:42.000000 invoke-2.1.1/tests/config.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     7687 2023-02-17 20:13:42.000000 invoke-2.1.1/tests/completion.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    17268 2023-02-17 20:13:42.000000 invoke-2.1.1/tests/task.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    12116 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/parser_context.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1661 2023-02-17 20:13:42.000000 invoke-2.1.1/tests/util.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    22668 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/parser_parser.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     3261 2023-02-17 20:13:42.000000 invoke-2.1.1/tests/concurrency.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     5361 2023-02-16 19:54:15.000000 invoke-2.1.1/tests/cli.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4371 2023-05-02 02:07:48.000000 invoke-2.1.1/tests/loader.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       38 2023-05-02 02:11:06.000000 invoke-2.1.1/setup.cfg
+-rw-r--r--   0 jforcier  (1000) users      (100)     1250 2023-05-02 02:04:35.000000 invoke-2.1.1/pyproject.toml
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 02:11:06.000000 invoke-2.1.1/invoke/
+-rw-r--r--   0 jforcier  (1000) users      (100)    38177 2023-05-02 02:04:35.000000 invoke-2.1.1/invoke/program.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    12227 2023-05-02 02:04:35.000000 invoke-2.1.1/invoke/exceptions.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       47 2023-02-16 19:54:15.000000 invoke-2.1.1/invoke/__main__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    25486 2023-05-02 02:04:35.000000 invoke-2.1.1/invoke/context.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    23060 2023-05-02 02:04:35.000000 invoke-2.1.1/invoke/collection.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    65509 2023-05-02 02:04:35.000000 invoke-2.1.1/invoke/runners.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     5305 2023-05-02 02:04:35.000000 invoke-2.1.1/invoke/loader.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     5097 2023-05-02 02:04:35.000000 invoke-2.1.1/invoke/watchers.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4394 2023-05-02 02:04:35.000000 invoke-2.1.1/invoke/env.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 02:11:06.000000 invoke-2.1.1/invoke/parser/
+-rw-r--r--   0 jforcier  (1000) users      (100)     6045 2023-05-02 02:04:35.000000 invoke-2.1.1/invoke/parser/argument.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     9815 2023-05-02 02:04:35.000000 invoke-2.1.1/invoke/parser/context.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      181 2023-02-16 19:54:15.000000 invoke-2.1.1/invoke/parser/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    19809 2023-05-02 02:04:35.000000 invoke-2.1.1/invoke/parser/parser.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     8855 2023-05-02 02:04:35.000000 invoke-2.1.1/invoke/executor.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2229 2023-05-02 02:04:35.000000 invoke-2.1.1/invoke/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     8065 2023-05-02 02:04:35.000000 invoke-2.1.1/invoke/terminals.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 02:11:06.000000 invoke-2.1.1/invoke/vendor/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 02:11:06.000000 invoke-2.1.1/invoke/vendor/yaml/
+-rw-r--r--   0 jforcier  (1000) users      (100)    51277 2023-02-16 19:54:15.000000 invoke-2.1.1/invoke/vendor/yaml/scanner.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     6794 2023-02-16 19:54:22.000000 invoke-2.1.1/invoke/vendor/yaml/reader.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2837 2023-02-16 19:54:15.000000 invoke-2.1.1/invoke/vendor/yaml/dumper.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1440 2023-02-16 19:54:22.000000 invoke-2.1.1/invoke/vendor/yaml/nodes.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    28639 2023-02-16 19:54:15.000000 invoke-2.1.1/invoke/vendor/yaml/constructor.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2061 2023-02-16 19:54:15.000000 invoke-2.1.1/invoke/vendor/yaml/loader.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2573 2023-02-16 19:54:22.000000 invoke-2.1.1/invoke/vendor/yaml/tokens.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2445 2023-02-16 19:54:22.000000 invoke-2.1.1/invoke/vendor/yaml/events.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    13170 2023-02-16 19:54:15.000000 invoke-2.1.1/invoke/vendor/yaml/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    43006 2023-02-16 19:54:15.000000 invoke-2.1.1/invoke/vendor/yaml/emitter.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4883 2023-02-16 19:54:15.000000 invoke-2.1.1/invoke/vendor/yaml/composer.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    25495 2023-02-16 19:54:15.000000 invoke-2.1.1/invoke/vendor/yaml/parser.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    14184 2023-02-16 19:54:15.000000 invoke-2.1.1/invoke/vendor/yaml/representer.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4165 2023-02-16 19:54:15.000000 invoke-2.1.1/invoke/vendor/yaml/serializer.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     3851 2023-02-16 19:54:15.000000 invoke-2.1.1/invoke/vendor/yaml/cyaml.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     8999 2023-02-16 19:54:15.000000 invoke-2.1.1/invoke/vendor/yaml/resolver.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2533 2023-02-16 19:54:15.000000 invoke-2.1.1/invoke/vendor/yaml/error.py
+-rw-r--r--   0 jforcier  (1000) users      (100)        0 2023-02-16 19:54:15.000000 invoke-2.1.1/invoke/vendor/__init__.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 02:11:06.000000 invoke-2.1.1/invoke/vendor/fluidity/
+-rw-r--r--   0 jforcier  (1000) users      (100)     8686 2023-02-16 19:54:22.000000 invoke-2.1.1/invoke/vendor/fluidity/machine.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      196 2023-02-16 19:54:15.000000 invoke-2.1.1/invoke/vendor/fluidity/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      135 2023-02-16 19:54:15.000000 invoke-2.1.1/invoke/vendor/fluidity/backwardscompat.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 02:11:06.000000 invoke-2.1.1/invoke/vendor/lexicon/
+-rw-r--r--   0 jforcier  (1000) users      (100)       80 2023-02-16 19:54:15.000000 invoke-2.1.1/invoke/vendor/lexicon/_version.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      407 2023-02-16 19:54:15.000000 invoke-2.1.1/invoke/vendor/lexicon/attribute_dict.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     3223 2023-02-16 19:54:15.000000 invoke-2.1.1/invoke/vendor/lexicon/alias_dict.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1133 2023-02-16 19:54:15.000000 invoke-2.1.1/invoke/vendor/lexicon/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    50005 2023-05-02 02:04:35.000000 invoke-2.1.1/invoke/config.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       80 2023-05-02 02:11:05.000000 invoke-2.1.1/invoke/_version.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    10018 2023-05-02 02:04:35.000000 invoke-2.1.1/invoke/util.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      235 2023-02-16 19:54:15.000000 invoke-2.1.1/invoke/main.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-02 02:11:06.000000 invoke-2.1.1/invoke/completion/
+-rw-r--r--   0 jforcier  (1000) users      (100)     1356 2021-12-23 21:30:34.000000 invoke-2.1.1/invoke/completion/bash.completion
+-rw-r--r--   0 jforcier  (1000) users      (100)        0 2023-02-16 19:54:15.000000 invoke-2.1.1/invoke/completion/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1429 2021-12-23 21:30:34.000000 invoke-2.1.1/invoke/completion/zsh.completion
+-rw-r--r--   0 jforcier  (1000) users      (100)     5222 2023-05-02 02:04:35.000000 invoke-2.1.1/invoke/completion/complete.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      382 2021-12-23 21:30:34.000000 invoke-2.1.1/invoke/completion/fish.completion
+-rw-r--r--   0 jforcier  (1000) users      (100)    19946 2023-05-02 02:04:35.000000 invoke-2.1.1/invoke/tasks.py
```

### Comparing `invoke-2.1.0/invoke/loader.py` & `invoke-2.1.1/invoke/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,15 @@
             # being imported is trying to load local-to-it names.
             if os.path.isfile(spec.origin):
                 path = os.path.dirname(spec.origin)
             if path not in sys.path:
                 sys.path.insert(0, path)
             # Actual import
             module = module_from_spec(spec)
+            sys.modules[spec.name] = module  # so 'from . import xxx' works
             spec.loader.exec_module(module)
             return module, os.path.dirname(spec.origin)
         msg = "ImportError loading {!r}, raising ImportError"
         debug(msg.format(name))
         raise ImportError
```

### Comparing `invoke-2.1.0/invoke/parser/parser.py` & `invoke-2.1.1/invoke/parser/parser.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/parser/context.py` & `invoke-2.1.1/invoke/parser/context.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/parser/argument.py` & `invoke-2.1.1/invoke/parser/argument.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/env.py` & `invoke-2.1.1/invoke/env.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/util.py` & `invoke-2.1.1/invoke/util.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/vendor/lexicon/alias_dict.py` & `invoke-2.1.1/invoke/vendor/lexicon/alias_dict.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/vendor/lexicon/__init__.py` & `invoke-2.1.1/invoke/vendor/lexicon/__init__.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/vendor/yaml/composer.py` & `invoke-2.1.1/invoke/vendor/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/vendor/yaml/emitter.py` & `invoke-2.1.1/invoke/vendor/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/vendor/yaml/parser.py` & `invoke-2.1.1/invoke/vendor/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/vendor/yaml/__init__.py` & `invoke-2.1.1/invoke/vendor/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/vendor/yaml/error.py` & `invoke-2.1.1/invoke/vendor/yaml/error.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/vendor/yaml/representer.py` & `invoke-2.1.1/invoke/vendor/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/vendor/yaml/cyaml.py` & `invoke-2.1.1/invoke/vendor/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/vendor/yaml/resolver.py` & `invoke-2.1.1/invoke/vendor/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/vendor/yaml/serializer.py` & `invoke-2.1.1/invoke/vendor/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/vendor/yaml/reader.py` & `invoke-2.1.1/invoke/vendor/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/vendor/yaml/scanner.py` & `invoke-2.1.1/invoke/vendor/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/vendor/yaml/dumper.py` & `invoke-2.1.1/invoke/vendor/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/vendor/yaml/nodes.py` & `invoke-2.1.1/invoke/vendor/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/vendor/yaml/events.py` & `invoke-2.1.1/invoke/vendor/yaml/events.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/vendor/yaml/tokens.py` & `invoke-2.1.1/invoke/vendor/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/vendor/yaml/constructor.py` & `invoke-2.1.1/invoke/vendor/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/vendor/yaml/loader.py` & `invoke-2.1.1/invoke/vendor/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/vendor/fluidity/machine.py` & `invoke-2.1.1/invoke/vendor/fluidity/machine.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/completion/complete.py` & `invoke-2.1.1/invoke/completion/complete.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/completion/bash.completion` & `invoke-2.1.1/invoke/completion/bash.completion`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/completion/zsh.completion` & `invoke-2.1.1/invoke/completion/zsh.completion`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/collection.py` & `invoke-2.1.1/invoke/collection.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/config.py` & `invoke-2.1.1/invoke/config.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/exceptions.py` & `invoke-2.1.1/invoke/exceptions.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/context.py` & `invoke-2.1.1/invoke/context.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/terminals.py` & `invoke-2.1.1/invoke/terminals.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/program.py` & `invoke-2.1.1/invoke/program.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/runners.py` & `invoke-2.1.1/invoke/runners.py`

 * *Files 0% similar despite different names*

```diff
@@ -1342,15 +1342,20 @@
                 stdout=PIPE,
                 stderr=PIPE,
                 stdin=PIPE,
             )
 
     def kill(self) -> None:
         pid = self.pid if self.using_pty else self.process.pid
-        os.kill(pid, signal.SIGKILL)
+        try:
+            os.kill(pid, signal.SIGKILL)
+        except ProcessLookupError:
+            # In odd situations where our subprocess is already dead, don't
+            # throw this upwards.
+            pass
 
     @property
     def process_is_finished(self) -> bool:
         if self.using_pty:
             # NOTE:
             # https://github.com/pexpect/ptyprocess/blob/4058faa05e2940662ab6da1330aa0586c6f9cd9c/ptyprocess/ptyprocess.py#L680-L687
             # implies that Linux "requires" use of the blocking, non-WNOHANG
@@ -1381,14 +1386,15 @@
                 code = -1 * code
             return code
             # TODO: do we care about WIFSTOPPED? Maybe someday?
         else:
             return self.process.returncode
 
     def stop(self) -> None:
+        super().stop()
         # If we opened a PTY for child communications, make sure to close() it,
         # otherwise long-running Invoke-using processes exhaust their file
         # descriptors eventually.
         if self.using_pty:
             try:
                 os.close(self.parent_fd)
             except Exception:
```

### Comparing `invoke-2.1.0/invoke/watchers.py` & `invoke-2.1.1/invoke/watchers.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/__init__.py` & `invoke-2.1.1/invoke/__init__.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/tasks.py` & `invoke-2.1.1/invoke/tasks.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke/executor.py` & `invoke-2.1.1/invoke/executor.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/PKG-INFO` & `invoke-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invoke
-Version: 2.1.0
+Version: 2.1.1
 Summary: Pythonic task execution
 Home-page: https://pyinvoke.org
 Author: Jeff Forcier
 Author-email: jeff@bitprophet.org
 License: BSD
 Project-URL: Docs, https://docs.pyinvoke.org
 Project-URL: Source, https://github.com/pyinvoke/invoke
```

### Comparing `invoke-2.1.0/LICENSE` & `invoke-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/tasks.py` & `invoke-2.1.1/tasks.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/pyproject.toml` & `invoke-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/setup.py` & `invoke-2.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/invoke.egg-info/PKG-INFO` & `invoke-2.1.1/invoke.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invoke
-Version: 2.1.0
+Version: 2.1.1
 Summary: Pythonic task execution
 Home-page: https://pyinvoke.org
 Author: Jeff Forcier
 Author-email: jeff@bitprophet.org
 License: BSD
 Project-URL: Docs, https://docs.pyinvoke.org
 Project-URL: Source, https://github.com/pyinvoke/invoke
```

### Comparing `invoke-2.1.0/invoke.egg-info/SOURCES.txt` & `invoke-2.1.1/invoke.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -167,13 +167,15 @@
 tests/_support/configs/yaml/tasks.py
 tests/_support/configs/yml/explicit.py
 tests/_support/configs/yml/invoke.yml
 tests/_support/configs/yml/tasks.py
 tests/_support/ignoreme/ignoremetoo/.no
 tests/_support/package/__init__.py
 tests/_support/package/module.py
+tests/_support/subspace/__init__.py
+tests/_support/subspace/module.py
 tests/_support/tree/__init__.py
 tests/_support/tree/deploy.py
 tests/_support/tree/provision.py
 tests/_support/tree/build/__init__.py
 tests/_support/tree/build/docs.py
 tests/_support/tree/build/python.py
```

### Comparing `invoke-2.1.0/tests/task.py` & `invoke-2.1.1/tests/task.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/tests/collection.py` & `invoke-2.1.1/tests/collection.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/tests/loader.py` & `invoke-2.1.1/tests/loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import sys
 from importlib.util import spec_from_file_location
 from types import ModuleType
+from pathlib import Path
 
 from pytest import raises
 
 from invoke import Config
 from invoke.loader import Loader, FilesystemLoader as FSLoader
 from invoke.exceptions import CollectionNotFound
 
@@ -46,25 +47,29 @@
         loader = _BasicLoader(config=config)
         assert loader.config.tasks.collection_name == "mytasks"
 
     def adds_module_parent_dir_to_sys_path(self):
         # Crummy doesn't-explode test.
         _BasicLoader().load("namespacing")
 
-    def doesnt_dupliate_parent_dir_addition(self):
+    def doesnt_duplicate_parent_dir_addition(self):
         _BasicLoader().load("namespacing")
         _BasicLoader().load("namespacing")
         # If the bug is present, this will be 2 at least (and often more, since
         # other tests will pollute it (!).
         assert sys.path.count(support) == 1
 
     def can_load_package(self):
         loader = _BasicLoader()
-        # make sure it doesn't explode
-        loader.load("package")
+        # Load itself doesn't explode (tests 'from . import xxx' internally)
+        mod, loc = loader.load("package")
+        # Properties of returned values look as expected
+        package = Path(support) / "package"
+        assert loc == str(package)
+        assert mod.__file__ == str(package / "__init__.py")
 
     def load_name_defaults_to_config_tasks_collection_name(self):
         "load() name defaults to config.tasks.collection_name"
 
         class MockLoader(_BasicLoader):
             def find(self, name):
                 # Sanity
```

### Comparing `invoke-2.1.0/tests/util.py` & `invoke-2.1.1/tests/util.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/tests/_util.py` & `invoke-2.1.1/tests/_util.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/tests/_support/tree.json` & `invoke-2.1.1/tests/_support/tree.json`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/tests/_support/decorators.py` & `invoke-2.1.1/tests/_support/decorators.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/tests/_support/integration.py` & `invoke-2.1.1/tests/_support/integration.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/tests/_support/tree/__init__.py` & `invoke-2.1.1/tests/_support/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/tests/executor.py` & `invoke-2.1.1/tests/executor.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/tests/parser_context.py` & `invoke-2.1.1/tests/parser_context.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/tests/watchers.py` & `invoke-2.1.1/tests/watchers.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/tests/conftest.py` & `invoke-2.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/tests/concurrency.py` & `invoke-2.1.1/tests/concurrency.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/tests/config.py` & `invoke-2.1.1/tests/config.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/tests/runners.py` & `invoke-2.1.1/tests/runners.py`

 * *Files 0% similar despite different names*

```diff
@@ -1398,19 +1398,14 @@
         def run_always_stops_timer(self):
             runner = _GenericExceptingRunner(Context())
             runner._timer = Mock()
             with raises(_GenericException):
                 runner.run(_)
             runner._timer.cancel.assert_called_once_with()
 
-        def stop_cancels_timer(self):
-            runner = self._mocked_timer()
-            runner.stop()
-            runner._timer.cancel.assert_called_once_with()
-
         def timer_aliveness_is_test_of_timing_out(self):
             # Might be redundant, but easy enough to unit test
             runner = Runner(Context())
             runner._timer = Mock()
             runner._timer.is_alive.return_value = False
             assert runner.timed_out
             runner._timer.is_alive.return_value = True
@@ -1426,14 +1421,20 @@
         def always_runs_no_matter_what(self):
             runner = _GenericExceptingRunner(context=Context())
             runner.stop = Mock()
             with raises(_GenericException):
                 runner.run(_)
             runner.stop.assert_called_once_with()
 
+        def cancels_timer(self):
+            runner = self._runner()
+            runner._timer = Mock()
+            runner.stop()
+            runner._timer.cancel.assert_called_once_with()
+
     class asynchronous:
         def returns_Promise_immediately_and_finishes_on_join(self):
             # Dummy subclass with controllable process_is_finished flag
             class _Finisher(_Dummy):
                 _finished = False
 
                 @property
@@ -1530,14 +1531,23 @@
 class Local_:
     def _run(self, *args, **kwargs):
         return _run(*args, **dict(kwargs, klass=_FastLocal))
 
     def _runner(self, *args, **kwargs):
         return _runner(*args, **dict(kwargs, klass=_FastLocal))
 
+    class stop:
+        @mock_subprocess()
+        def calls_super(self):
+            # Re #910
+            runner = self._runner()
+            runner._timer = Mock()  # twiddled by parent class stop()
+            runner.run(_)
+            runner._timer.cancel.assert_called_once_with()
+
     class pty:
         @mock_pty()
         def when_pty_True_we_use_pty_fork_and_os_exec(self):
             "when pty=True, we use pty.fork and os.exec*"
             self._run(_, pty=True)
             # @mock_pty's asserts check os/pty calls for us.
```

### Comparing `invoke-2.1.0/tests/init.py` & `invoke-2.1.1/tests/init.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/tests/merge_dicts.py` & `invoke-2.1.1/tests/merge_dicts.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/tests/cli.py` & `invoke-2.1.1/tests/cli.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/tests/context.py` & `invoke-2.1.1/tests/context.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/tests/completion.py` & `invoke-2.1.1/tests/completion.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/tests/program.py` & `invoke-2.1.1/tests/program.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/tests/terminals.py` & `invoke-2.1.1/tests/terminals.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/tests/parser_parser.py` & `invoke-2.1.1/tests/parser_parser.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/tests/parser_argument.py` & `invoke-2.1.1/tests/parser_argument.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/README.rst` & `invoke-2.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/sites/www/prior-art.rst` & `invoke-2.1.1/sites/www/prior-art.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/sites/www/installing.rst` & `invoke-2.1.1/sites/www/installing.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/sites/www/development.rst` & `invoke-2.1.1/sites/www/development.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/sites/www/contact.rst` & `invoke-2.1.1/sites/www/contact.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/sites/www/faq.rst` & `invoke-2.1.1/sites/www/faq.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/sites/www/conf.py` & `invoke-2.1.1/sites/www/conf.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/sites/www/index.rst` & `invoke-2.1.1/sites/www/index.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/sites/www/changelog.rst` & `invoke-2.1.1/sites/www/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 =========
 Changelog
 =========
 
+- :release:`2.1.1 <2023-05-01>`
+- :bug:`934` The `importlib` upgrade in 2.1 had a corner case bug (regarding
+  ``from . import <submodule>`` functionality within package-like task trees)
+  which in turn exposed a false-pass in our test suite. Both have now been
+  fixed. Thanks to Greg Meyer and Robert J. Berger for the bug reports.
+- :release:`2.0.1 <2023-04-29>`
+- :bug:`910` Add more rigor around subprocess/runner shutdown to avoid spurious
+  exceptions & also fix downstream issues in libraries like Fabric. Reported by
+  Orlando Rodríguez.
 - :release:`2.1.0 <2023-04-28>`
 - :support:`675` Implement `importlib` and deprecate `imp` module. Patches
   provided by Jesse P. Johnson
-- :bug:`376` Resolve equality comparison bug for non-collections. Patch via
-  Jesse P. Johnson
+- :bug:`376 major` Resolve equality comparison bug for non-collections. Patch
+  via Jesse P. Johnson
 - :support:`906` Implement type hints and type checking tests with mypy to
   reduce errors and impove code documentation. Patches by Jesse P. Johnson and
   review by Sam Bull.
 - :support:`901 backported` (via :issue:`903`) Tweak test suite ``setup``
   methods to be named ``setup_method`` so pytest stops whining about it. Patch
   via Jesse P. Johnson.
 - :release:`2.0.0 <2023-01-16>`
```

### Comparing `invoke-2.1.0/sites/shared_conf.py` & `invoke-2.1.1/sites/shared_conf.py`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/sites/docs/concepts/invoking-tasks.rst` & `invoke-2.1.1/sites/docs/concepts/invoking-tasks.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/sites/docs/concepts/library.rst` & `invoke-2.1.1/sites/docs/concepts/library.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/sites/docs/concepts/watchers.rst` & `invoke-2.1.1/sites/docs/concepts/watchers.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/sites/docs/concepts/configuration.rst` & `invoke-2.1.1/sites/docs/concepts/configuration.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/sites/docs/concepts/loading.rst` & `invoke-2.1.1/sites/docs/concepts/loading.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/sites/docs/concepts/testing.rst` & `invoke-2.1.1/sites/docs/concepts/testing.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/sites/docs/concepts/namespaces.rst` & `invoke-2.1.1/sites/docs/concepts/namespaces.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/sites/docs/getting-started.rst` & `invoke-2.1.1/sites/docs/getting-started.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/sites/docs/_static/rtd.css` & `invoke-2.1.1/sites/docs/_static/rtd.css`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/sites/docs/index.rst` & `invoke-2.1.1/sites/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invoke-2.1.0/sites/docs/invoke.rst` & `invoke-2.1.1/sites/docs/invoke.rst`

 * *Files identical despite different names*

