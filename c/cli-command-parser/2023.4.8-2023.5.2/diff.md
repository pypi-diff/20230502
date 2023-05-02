# Comparing `tmp/cli_command_parser-2023.4.8.tar.gz` & `tmp/cli_command_parser-2023.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli_command_parser-2023.4.8.tar", last modified: Sat Apr  8 14:59:10 2023, max compression
+gzip compressed data, was "cli_command_parser-2023.5.2.tar", last modified: Tue May  2 11:35:50 2023, max compression
```

## Comparing `cli_command_parser-2023.4.8.tar` & `cli_command_parser-2023.5.2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 14:59:10.626959 cli_command_parser-2023.4.8/
--rw-rw-rw-   0        0        0    11341 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.8/LICENSE
--rw-rw-rw-   0        0        0       64 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.8/MANIFEST.in
--rw-rw-rw-   0        0        0     4713 2023-04-08 14:59:10.626959 cli_command_parser-2023.4.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-08 14:59:10.476958 cli_command_parser-2023.4.8/lib/
-drwxrwxrwx   0        0        0        0 2023-04-08 14:59:10.550958 cli_command_parser-2023.4.8/lib/cli_command_parser/
--rw-rw-rw-   0        0        0     1016 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/__init__.py
--rw-rw-rw-   0        0        0      114 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/__main__.py
--rw-rw-rw-   0        0        0      295 2023-04-08 14:59:00.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/__version__.py
--rw-rw-rw-   0        0        0      463 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/actions.py
--rw-rw-rw-   0        0        0     3017 2022-10-15 14:00:15.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/annotations.py
--rw-rw-rw-   0        0        0    19746 2023-03-30 11:44:47.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/command_parameters.py
--rw-rw-rw-   0        0        0    12491 2023-03-31 11:57:05.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/commands.py
--rw-rw-rw-   0        0        0     9032 2023-04-08 14:58:49.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/compat.py
--rw-rw-rw-   0        0        0    15521 2023-04-07 12:09:39.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/config.py
--rw-rw-rw-   0        0        0    16854 2023-03-30 11:44:47.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/context.py
-drwxrwxrwx   0        0        0        0 2023-04-08 14:59:10.583958 cli_command_parser-2023.4.8/lib/cli_command_parser/conversion/
--rw-rw-rw-   0        0        0      234 2023-04-06 21:32:03.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/conversion/__init__.py
--rw-rw-rw-   0        0        0       54 2023-04-06 21:32:03.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/conversion/__main__.py
--rw-rw-rw-   0        0        0    12802 2023-04-06 21:32:03.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/conversion/argparse_ast.py
--rw-rw-rw-   0        0        0     1356 2023-04-06 21:32:03.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/conversion/argparse_utils.py
--rw-rw-rw-   0        0        0    21945 2023-04-08 14:58:49.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/conversion/command_builder.py
--rw-rw-rw-   0        0        0     1660 2023-04-06 21:32:03.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/conversion/utils.py
--rw-rw-rw-   0        0        0     7403 2023-04-07 12:09:39.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/conversion/visitor.py
--rw-rw-rw-   0        0        0     9792 2022-09-24 13:23:00.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/core.py
--rw-rw-rw-   0        0        0    13416 2023-03-29 11:48:12.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/documentation.py
--rw-rw-rw-   0        0        0     4800 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/error_handling.py
--rw-rw-rw-   0        0        0     7775 2022-11-12 17:12:38.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-08 14:59:10.597958 cli_command_parser-2023.4.8/lib/cli_command_parser/formatting/
--rw-rw-rw-   0        0        0        0 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/formatting/__init__.py
--rw-rw-rw-   0        0        0     6557 2022-09-24 13:23:00.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/formatting/commands.py
--rw-rw-rw-   0        0        0    20639 2023-04-08 14:58:49.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/formatting/params.py
--rw-rw-rw-   0        0        0     8572 2022-09-18 21:50:31.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/formatting/restructured_text.py
--rw-rw-rw-   0        0        0     5440 2023-04-06 21:32:03.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/formatting/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-08 14:59:10.606958 cli_command_parser-2023.4.8/lib/cli_command_parser/inputs/
--rw-rw-rw-   0        0        0     2125 2023-04-08 14:58:49.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/inputs/__init__.py
--rw-rw-rw-   0        0        0     1438 2023-04-08 14:58:49.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/inputs/base.py
--rw-rw-rw-   0        0        0     6313 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/inputs/choices.py
--rw-rw-rw-   0        0        0     1113 2023-04-08 14:58:49.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/inputs/exceptions.py
--rw-rw-rw-   0        0        0     8563 2023-04-08 14:58:49.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/inputs/files.py
--rw-rw-rw-   0        0        0     7318 2023-04-08 14:58:49.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/inputs/numeric.py
--rw-rw-rw-   0        0        0    21286 2023-04-08 14:58:49.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/inputs/time.py
--rw-rw-rw-   0        0        0     6490 2023-01-14 20:20:57.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/inputs/utils.py
--rw-rw-rw-   0        0        0     8145 2023-01-15 15:08:06.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/metadata.py
--rw-rw-rw-   0        0        0     6538 2022-09-19 11:52:48.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/nargs.py
-drwxrwxrwx   0        0        0        0 2023-04-08 14:59:10.626959 cli_command_parser-2023.4.8/lib/cli_command_parser/parameters/
--rw-rw-rw-   0        0        0      300 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/parameters/__init__.py
--rw-rw-rw-   0        0        0    25629 2023-04-08 14:58:49.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/parameters/base.py
--rw-rw-rw-   0        0        0    17128 2022-09-18 21:50:31.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/parameters/choice_map.py
--rw-rw-rw-   0        0        0    10236 2023-03-31 11:57:05.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/parameters/groups.py
--rw-rw-rw-   0        0        0     6452 2023-03-30 11:44:47.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/parameters/option_strings.py
--rw-rw-rw-   0        0        0    19899 2023-03-30 11:44:47.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/parameters/options.py
--rw-rw-rw-   0        0        0     2039 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/parameters/pass_thru.py
--rw-rw-rw-   0        0        0     3566 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/parameters/positionals.py
--rw-rw-rw-   0        0        0    11704 2022-09-19 11:52:48.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/parse_tree.py
--rw-rw-rw-   0        0        0    14238 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/parser.py
--rw-rw-rw-   0        0        0     9623 2023-04-01 22:51:43.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/testing.py
--rw-rw-rw-   0        0        0     1795 2023-01-14 18:15:47.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/typing.py
--rw-rw-rw-   0        0        0     4548 2023-01-14 20:20:57.000000 cli_command_parser-2023.4.8/lib/cli_command_parser/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-08 14:59:10.559958 cli_command_parser-2023.4.8/lib/cli_command_parser.egg-info/
--rw-rw-rw-   0        0        0     4713 2023-04-08 14:59:10.000000 cli_command_parser-2023.4.8/lib/cli_command_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2314 2023-04-08 14:59:10.000000 cli_command_parser-2023.4.8/lib/cli_command_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 14:59:10.000000 cli_command_parser-2023.4.8/lib/cli_command_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2023-04-08 14:59:10.000000 cli_command_parser-2023.4.8/lib/cli_command_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-08 14:59:10.000000 cli_command_parser-2023.4.8/lib/cli_command_parser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      324 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.8/pyproject.toml
--rw-rw-rw-   0        0        0     3483 2023-04-07 12:09:39.000000 cli_command_parser-2023.4.8/readme.rst
--rw-rw-rw-   0        0        0       99 2022-09-17 20:57:36.000000 cli_command_parser-2023.4.8/requirements-dev.txt
--rw-rw-rw-   0        0        0     1333 2023-04-08 14:59:10.628958 cli_command_parser-2023.4.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-02 11:35:50.513208 cli_command_parser-2023.5.2/
+-rw-rw-rw-   0        0        0    11341 2022-09-17 20:57:36.000000 cli_command_parser-2023.5.2/LICENSE
+-rw-rw-rw-   0        0        0       64 2022-09-17 20:57:36.000000 cli_command_parser-2023.5.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     5610 2023-05-02 11:35:50.514207 cli_command_parser-2023.5.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-02 11:35:50.361159 cli_command_parser-2023.5.2/lib/
+drwxrwxrwx   0        0        0        0 2023-05-02 11:35:50.428205 cli_command_parser-2023.5.2/lib/cli_command_parser/
+-rw-rw-rw-   0        0        0     1136 2023-04-29 17:20:11.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/__init__.py
+-rw-rw-rw-   0        0        0      114 2022-09-17 20:57:36.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/__main__.py
+-rw-rw-rw-   0        0        0      295 2023-05-02 11:35:39.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/__version__.py
+-rw-rw-rw-   0        0        0      463 2022-09-17 20:57:36.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/actions.py
+-rw-rw-rw-   0        0        0     2868 2023-05-02 11:35:36.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/annotations.py
+-rw-rw-rw-   0        0        0    22573 2023-05-02 11:35:36.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/command_parameters.py
+-rw-rw-rw-   0        0        0    12737 2023-04-30 17:54:18.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/commands.py
+-rw-rw-rw-   0        0        0     5150 2023-05-02 11:35:36.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/compat.py
+-rw-rw-rw-   0        0        0    16435 2023-04-29 17:20:11.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/config.py
+-rw-rw-rw-   0        0        0    16608 2023-05-02 11:35:36.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/context.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:35:50.459208 cli_command_parser-2023.5.2/lib/cli_command_parser/conversion/
+-rw-rw-rw-   0        0        0      234 2023-04-06 21:32:03.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/conversion/__init__.py
+-rw-rw-rw-   0        0        0       54 2023-04-06 21:32:03.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/conversion/__main__.py
+-rw-rw-rw-   0        0        0    12765 2023-05-02 11:35:36.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/conversion/argparse_ast.py
+-rw-rw-rw-   0        0        0     1356 2023-04-06 21:32:03.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/conversion/argparse_utils.py
+-rw-rw-rw-   0        0        0    24495 2023-05-02 11:35:36.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/conversion/command_builder.py
+-rw-rw-rw-   0        0        0     1660 2023-04-06 21:32:03.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/conversion/utils.py
+-rw-rw-rw-   0        0        0     7560 2023-04-15 20:51:25.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/conversion/visitor.py
+-rw-rw-rw-   0        0        0    10136 2023-04-23 16:53:29.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/core.py
+-rw-rw-rw-   0        0        0    13416 2023-03-29 11:48:12.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/documentation.py
+-rw-rw-rw-   0        0        0     6787 2023-04-29 17:20:11.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/error_handling.py
+-rw-rw-rw-   0        0        0     8093 2023-05-02 11:35:36.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:35:50.473206 cli_command_parser-2023.5.2/lib/cli_command_parser/formatting/
+-rw-rw-rw-   0        0        0        0 2022-09-17 20:57:36.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/formatting/__init__.py
+-rw-rw-rw-   0        0        0     6568 2023-04-15 20:51:25.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/formatting/commands.py
+-rw-rw-rw-   0        0        0    20558 2023-05-02 11:35:36.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/formatting/params.py
+-rw-rw-rw-   0        0        0     8572 2022-09-18 21:50:31.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/formatting/restructured_text.py
+-rw-rw-rw-   0        0        0     5440 2023-04-06 21:32:03.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/formatting/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:35:50.495207 cli_command_parser-2023.5.2/lib/cli_command_parser/inputs/
+-rw-rw-rw-   0        0        0     2125 2023-04-08 14:58:49.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/inputs/__init__.py
+-rw-rw-rw-   0        0        0     1438 2023-04-08 14:58:49.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/inputs/base.py
+-rw-rw-rw-   0        0        0     6313 2022-09-17 20:57:36.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/inputs/choices.py
+-rw-rw-rw-   0        0        0     1113 2023-04-08 14:58:49.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/inputs/exceptions.py
+-rw-rw-rw-   0        0        0     8563 2023-04-08 14:58:49.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/inputs/files.py
+-rw-rw-rw-   0        0        0     7772 2023-04-29 17:20:11.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/inputs/numeric.py
+-rw-rw-rw-   0        0        0    21205 2023-05-02 11:35:36.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/inputs/time.py
+-rw-rw-rw-   0        0        0     6490 2023-01-14 20:20:57.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/inputs/utils.py
+-rw-rw-rw-   0        0        0    10756 2023-05-02 11:35:36.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/metadata.py
+-rw-rw-rw-   0        0        0     7476 2023-04-15 20:51:25.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/nargs.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:35:50.513208 cli_command_parser-2023.5.2/lib/cli_command_parser/parameters/
+-rw-rw-rw-   0        0        0      300 2022-09-17 20:57:36.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/parameters/__init__.py
+-rw-rw-rw-   0        0        0    27625 2023-05-02 11:35:36.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/parameters/base.py
+-rw-rw-rw-   0        0        0    17312 2023-04-19 21:58:59.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/parameters/choice_map.py
+-rw-rw-rw-   0        0        0    10686 2023-04-23 16:53:29.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/parameters/groups.py
+-rw-rw-rw-   0        0        0     6913 2023-04-29 17:20:11.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/parameters/option_strings.py
+-rw-rw-rw-   0        0        0    25990 2023-05-02 11:35:36.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/parameters/options.py
+-rw-rw-rw-   0        0        0     2115 2023-04-30 17:54:18.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/parameters/pass_thru.py
+-rw-rw-rw-   0        0        0     4201 2023-04-15 20:51:25.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/parameters/positionals.py
+-rw-rw-rw-   0        0        0    11384 2023-04-15 20:51:25.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/parse_tree.py
+-rw-rw-rw-   0        0        0    15172 2023-04-30 17:54:18.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/parser.py
+-rw-rw-rw-   0        0        0    10811 2023-04-30 17:54:18.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/testing.py
+-rw-rw-rw-   0        0        0     1956 2023-04-30 17:54:18.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/typing.py
+-rw-rw-rw-   0        0        0     4968 2023-04-30 17:54:18.000000 cli_command_parser-2023.5.2/lib/cli_command_parser/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:35:50.438207 cli_command_parser-2023.5.2/lib/cli_command_parser.egg-info/
+-rw-rw-rw-   0        0        0     5610 2023-05-02 11:35:50.000000 cli_command_parser-2023.5.2/lib/cli_command_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2314 2023-05-02 11:35:50.000000 cli_command_parser-2023.5.2/lib/cli_command_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 11:35:50.000000 cli_command_parser-2023.5.2/lib/cli_command_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2023-05-02 11:35:50.000000 cli_command_parser-2023.5.2/lib/cli_command_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-02 11:35:50.000000 cli_command_parser-2023.5.2/lib/cli_command_parser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      316 2023-05-02 11:35:36.000000 cli_command_parser-2023.5.2/pyproject.toml
+-rw-rw-rw-   0        0        0     4414 2023-05-02 11:35:36.000000 cli_command_parser-2023.5.2/readme.rst
+-rw-rw-rw-   0        0        0      111 2023-04-10 12:30:46.000000 cli_command_parser-2023.5.2/requirements-dev.txt
+-rw-rw-rw-   0        0        0     1293 2023-05-02 11:35:50.515208 cli_command_parser-2023.5.2/setup.cfg
```

### Comparing `cli_command_parser-2023.4.8/LICENSE` & `cli_command_parser-2023.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.8/PKG-INFO` & `cli_command_parser-2023.5.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 Metadata-Version: 2.1
 Name: cli_command_parser
-Version: 2023.4.8
+Version: 2023.5.2
 Summary: CLI Command Parser
 Home-page: https://github.com/dskrypa/cli_command_parser
 Author: Doug Skrypa
 Author-email: dskrypa@gmail.com
 License: Apache 2.0
 Project-URL: Source, https://github.com/dskrypa/cli_command_parser
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Text Processing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: wcwidth
 Provides-Extra: conversion
 License-File: LICENSE
 
 CLI Command Parser
 ##################
 
 |downloads| |py_version| |coverage_badge| |build_status| |Blue|
 
-.. |py_version| image:: https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20-blue
+.. |py_version| image:: https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20-blue
     :target: https://pypi.org/project/cli-command-parser/
 
 .. |coverage_badge| image:: https://codecov.io/gh/dskrypa/cli_command_parser/branch/main/graph/badge.svg
     :target: https://codecov.io/gh/dskrypa/cli_command_parser
 
 .. |build_status| image:: https://github.com/dskrypa/cli_command_parser/actions/workflows/run-tests.yml/badge.svg
     :target: https://github.com/dskrypa/cli_command_parser/actions/workflows/run-tests.yml
@@ -107,14 +106,31 @@
 There are no required dependencies.  Support for formatting wide characters correctly in help text descriptions can
 be included by adding `wcwidth <https://wcwidth.readthedocs.io>`__ to your project's requirements, and/or by installing
 with optional dependencies::
 
     $ pip install -U cli-command-parser[wcwidth]
 
 
+Python Version Compatibility
+============================
+
+Python versions 3.8 and above are currently supported.  The last release of CLI Command Parser that supported 3.7 was
+2023-04-30.  Support for Python 3.7 `officially ends on 2023-06-27 <https://devguide.python.org/versions/>`__.
+
+When using Python 3.8, some additional packages that backport functionality that was added in later Python versions
+are required for compatibility.
+
+To use the argparse to cli-command-parser conversion script with Python 3.8, there is a dependency on
+`astunparse <https://astunparse.readthedocs.io>`__.  If you are using Python 3.9 or above, then ``astunparse`` is not
+necessary because the relevant code was added to the stdlib ``ast`` module.  If you're unsure, you can install
+cli-command-parser with the following command to automatically handle whether that extra dependency is needed or not::
+
+    $ pip install -U cli-command-parser[conversion]
+
+
 Links
 *****
 
 - Documentation: https://dskrypa.github.io/cli_command_parser/
 - Example Scripts: https://github.com/dskrypa/cli_command_parser/tree/main/examples
 - PyPI Releases: https://pypi.org/project/cli-command-parser/
 - Source Code: https://github.com/dskrypa/cli_command_parser
```

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/__init__.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 """
 Command Parser
 
 :author: Doug Skrypa
 """
 
-from .config import CommandConfig, ShowDefaults, OptionNameMode, SubcommandAliasHelpMode
+from .config import (
+    CommandConfig,
+    ShowDefaults,
+    OptionNameMode,
+    SubcommandAliasHelpMode,
+    AmbiguousComboMode,
+    AllowLeadingDash,
+)
 from .commands import Command, main
 from .context import Context, get_current_context, ctx, get_parsed, get_context, get_raw_arg
 from .exceptions import (
     CommandParserException,
     CommandDefinitionError,
     ParameterDefinitionError,
     UsageError,
@@ -19,16 +26,17 @@
     NoSuchOption,
     ParserExit,
     ParamConflict,
     ParamsMissing,
     NoActiveContext,
     AmbiguousParseTree,
 )
-from .error_handling import ErrorHandler, error_handler, no_exit_handler
+from .error_handling import ErrorHandler, error_handler, no_exit_handler, extended_error_handler
 from .formatting.commands import get_formatter
+from .nargs import REMAINDER
 from .parameters import (
     Parameter,
     PassThru,
     BasePositional,
     Positional,
     SubCommand,
     Action,
```

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/annotations.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/annotations.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,20 +4,15 @@
 :author: Doug Skrypa
 """
 
 from __future__ import annotations
 
 from collections.abc import Collection, Iterable
 from inspect import isclass
-from typing import Union, Optional, get_type_hints
-
-try:
-    from typing import get_origin, get_args as _get_args  # pylint: disable=C0412
-except ImportError:  # Added in 3.8; the versions from 3.8 are copied here
-    from .compat import get_origin, _get_args
+from typing import Union, Optional, get_type_hints, get_origin, get_args as _get_args  # pylint: disable=C0412
 
 try:
     from types import NoneType
 except ImportError:  # Added in 3.10
     NoneType = type(None)
 
 __all__ = ['get_descriptor_value_type']
```

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/command_parameters.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/command_parameters.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,17 @@
 
 :author: Doug Skrypa
 """
 
 from __future__ import annotations
 
 from collections import defaultdict
+from functools import cached_property
 from typing import TYPE_CHECKING, Optional, Collection, Iterator, List, Dict, Set, Tuple
 
-try:
-    from functools import cached_property
-except ImportError:
-    from .compat import cached_property
-
 from .actions import help_action
 from .config import CommandConfig, AmbiguousComboMode
 from .exceptions import CommandDefinitionError, ParameterDefinitionError, ParamsMissing
 from .exceptions import AmbiguousShortForm, AmbiguousCombo
 from .parameters.base import ParamBase, Parameter, BaseOption, BasePositional
 from .parameters import SubCommand, PassThru, ActionFlag, ParamGroup, Action, Option
 
@@ -35,33 +31,38 @@
 OptionMap = Dict[str, BaseOption]
 ActionFlags = List[ActionFlag]
 
 
 class CommandParameters:
     command: CommandCls                                  #: The Command associated with this CommandParameters object
     formatter: CommandHelpFormatter                      #: The formatter used for this Command's help text
-    command_parent: Optional[CommandCls] = None          #: The parent Command, if any
-    parent: Optional[CommandParameters] = None           #: The parent Command's CommandParameters
+    command_parent: Optional[CommandCls]                 #: The parent Command, if any
+    parent: Optional[CommandParameters]                  #: The parent Command's CommandParameters
     action: Optional[Action] = None                      #: An Action Parameter, if specified
     _pass_thru: Optional[PassThru] = None                #: A PassThru Parameter, if specified
     sub_command: Optional[SubCommand] = None             #: A SubCommand Parameter, if specified
     action_flags: ActionFlags                            #: List of action flags
     split_action_flags: Tuple[ActionFlags, ActionFlags]  #: Action flags split by before/after main
     options: List[BaseOption]                            #: List of optional Parameters
     combo_option_map: OptionMap                          #: Mapping of {short opt: Parameter} (no dash characters)
     groups: List[ParamGroup]                             #: List of ParamGroup objects
     positionals: List[BasePositional]                    #: List of positional Parameters
+    _deferred_positionals: List[BasePositional] = ()     #: Positional Parameters that are deferred to sub commands
     option_map: OptionMap                                #: Mapping of {--opt / -opt: Parameter}
 
-    def __init__(self, command: CommandCls, command_parent: Optional[CommandCls], config: CommandConfig):
+    def __init__(
+        self,
+        command: CommandCls,
+        command_parent: Optional[CommandCls],
+        parent_params: Optional[CommandParameters],
+        config: CommandConfig,
+    ):
         self.command = command
-        if command_parent is not None:
-            self.command_parent = command_parent
-            self.parent = command_parent.__class__.params(command_parent)
-
+        self.command_parent = command_parent
+        self.parent = parent_params
         self.config = config
         self._process_parameters()
 
     def __repr__(self) -> str:
         positionals = len(self.positionals)
         options = len(self.options)
         cls_name = self.__class__.__name__
@@ -72,97 +73,89 @@
         if self._pass_thru:
             return self._pass_thru
         elif self.parent:
             return self.parent.pass_thru
         return None
 
     @cached_property
+    def all_positionals(self) -> List[BasePositional]:
+        try:
+            if not self.parent.sub_command:
+                return self.parent.all_positionals + self.positionals
+        except AttributeError:
+            pass
+        return self.positionals
+
+    def get_positionals_to_parse(self, ctx: Context) -> List[BasePositional]:
+        positionals = self.all_positionals
+        if not positionals:
+            return []
+        for i, param in enumerate(positionals):
+            if not ctx.num_provided(param):
+                return [p for p in positionals[i:]]
+        return []
+
+    @cached_property
     def always_available_action_flags(self) -> Tuple[ActionFlag, ...]:
         """
         The :paramref:`.ActionFlag.before_main` :class:`.ActionFlag` actions that are always available, even if parsing
         failed (such as the one for ``--help``).
         """
         return tuple(af for af in self.action_flags if af.always_available)
 
     @cached_property
     def formatter(self) -> CommandHelpFormatter:
         from .formatting.commands import CommandHelpFormatter
 
-        if self.config is None:
-            formatter_factory = CommandHelpFormatter
-        else:
-            formatter_factory = self.config.command_formatter or CommandHelpFormatter
+        formatter_factory = self.config.command_formatter or CommandHelpFormatter
         formatter = formatter_factory(self.command, self)
+        formatter.maybe_add_positionals(self.all_positionals)
         formatter.maybe_add_option(self._pass_thru)
-        formatter.maybe_add_positionals(self.positionals)
         formatter.maybe_add_options(self.options)
         formatter.maybe_add_groups(self.groups)
         return formatter
 
-    @cached_property
-    def _classified_combo_options(self) -> Tuple[Dict[str, BaseOption], Dict[str, BaseOption]]:
-        multi_char_combos = {}
-        single_char_combos = {}
-        for combo, param in self.combo_option_map.items():
-            if len(combo) == 1:
-                single_char_combos[combo] = param
-            else:
-                multi_char_combos[combo] = param
-        return single_char_combos, multi_char_combos
-
-    @cached_property
-    def _potentially_ambiguous_combo_options(self) -> Dict[str, Tuple[BaseOption, Dict[str, BaseOption]]]:
-        single_char_combos, multi_char_combos = self._classified_combo_options
-        if not multi_char_combos:
-            return {}
-
-        ambiguous_combo_options = {}
-        for combo, param in multi_char_combos.items():
-            singles = {c: single_char_combos[c] for c in combo if c in single_char_combos}
-            if singles:
-                ambiguous_combo_options[combo] = (param, singles)
-
-        return ambiguous_combo_options
-
     @property
     def _has_help(self) -> bool:
         return help_action in self.always_available_action_flags or (self.parent and self.parent._has_help)
 
     # region Initialization
 
-    def _process_parameters(self):
-        """
-        Process all of the :class:`.Parameter` / :class:`.ParamGroup` members in the associated :class:`.Command` class.
-        """
+    def _iter_parameters(self) -> Iterator[ParamBase]:
         name_param_map = {}  # Allow subclasses to override names, but not within a given command
-        positionals = []
-        options = []
-        groups = set()
-
         for attr, param in self.command.__dict__.items():
             if attr.startswith('__') or not isinstance(param, ParamBase):  # Name mangled Parameters are still processed
                 continue
-
-            name = param.name
             try:
-                other_attr, other_param = name_param_map[name]
+                other_attr, other_param = name_param_map[param.name]
             except KeyError:
-                name_param_map[name] = (attr, param)
+                name_param_map[param.name] = (attr, param)
+                yield param
             else:
                 raise CommandDefinitionError(
                     'Name conflict - multiple parameters within a Command cannot have the same name - conflicting'
                     f' params: {other_attr}={other_param}, {attr}={param}'
                 )
 
+    def _process_parameters(self):
+        """
+        Process all of the :class:`.Parameter` / :class:`.ParamGroup` members in the associated :class:`.Command` class.
+        """
+        positionals = []
+        options = []
+        groups = set()
+
+        for param in self._iter_parameters():
             if isinstance(param, BasePositional):
                 positionals.append(param)
             elif isinstance(param, BaseOption):
                 options.append(param)
             elif isinstance(param, ParamGroup):
                 # Groups will only be discovered here when defined with `as` - ex: `with ParamGroup(...) as foo:`
+                # Group members will always be discovered at the top level since context managers share the outer scope
                 groups.add(param)
             elif isinstance(param, PassThru):
                 if self.pass_thru:
                     raise CommandDefinitionError(
                         f'Invalid PassThru param={param!r} - it cannot follow another PassThru param'
                     )
                 self._pass_thru = param
@@ -171,57 +164,66 @@
                     f'Unexpected type={param.__class__} for param={param!r} - custom parameters must extend'
                     ' BasePositional, BaseOption, or ParamGroup'
                 )
 
             if param.group:
                 _find_groups(groups, param)
 
-        if self.config and self.config.add_help and (not self.parent or not self.parent._has_help):
+        if self.config.add_help and self.command_parent is not None and (not self.parent or not self.parent._has_help):
             options.append(help_action)
 
         self._process_positionals(positionals)
         self._process_options(options)
         self._process_groups(groups)
 
     def _process_groups(self, groups: Set[ParamGroup]):
         if self.parent:
             _groups, groups = groups, self.parent.groups.copy()
             groups.extend(_groups)
 
         self.groups = sorted(groups)
 
     def _process_positionals(self, params: List[BasePositional]):
-        var_nargs_param = None
-        for param in params:
-            if self.sub_command:
-                raise CommandDefinitionError(
-                    f'Positional param={param!r} may not follow the sub command {self.sub_command} - re-order the'
-                    ' positionals, move it into the sub command(s), or convert it to an optional parameter'
-                )
-            elif var_nargs_param:
+        unfollowable = action_or_sub_cmd = split_index = None
+        parent = self.parent
+        if parent and parent._deferred_positionals:
+            params = parent._deferred_positionals + params
+
+        for i, param in enumerate(params):
+            if unfollowable:
+                if 0 in unfollowable.nargs:
+                    why = 'because it is a positional that is not required'
+                else:
+                    why = 'because it accepts a variable number of arguments with no specific choices defined'
                 raise CommandDefinitionError(
-                    f'Additional Positional parameters cannot follow {var_nargs_param} because it accepts'
-                    f' a variable number of arguments with no specific choices defined - param={param!r} is invalid'
+                    f'Additional Positional parameters cannot follow {unfollowable} {why} - param={param!r} is invalid'
                 )
-
-            if isinstance(param, (SubCommand, Action)):
-                if self.action:  # self.sub_command being already defined is handled above
+            elif isinstance(param, (SubCommand, Action)):
+                if action_or_sub_cmd:
                     raise CommandDefinitionError(
                         f'Only 1 Action xor SubCommand is allowed in a given Command - {self.command.__name__} cannot'
-                        f' contain both {self.action} and {param}'
+                        f' contain both {action_or_sub_cmd} and {param}'
                     )
                 elif isinstance(param, SubCommand):
-                    self.sub_command = param
-                else:
-                    self.action = param
+                    self.sub_command = action_or_sub_cmd = param
+                    split_index = i + 1
+                    if param.has_choices and 0 in param.nargs:  # It has local choices or is not required
+                        unfollowable = param
+                else:  # It's an Action
+                    self.action = action_or_sub_cmd = param
                     if not param.has_choices:
                         raise CommandDefinitionError(f'No choices were registered for {self.action}')
+            elif 0 in param.nargs or (param.nargs.variable and not param.has_choices):
+                unfollowable = param
 
-            if param.nargs.variable and not param.has_choices:
-                var_nargs_param = param
+        if split_index:
+            if self.sub_command.has_local_choices:
+                self._deferred_positionals = params[split_index:]
+            else:
+                params, self._deferred_positionals = params[:split_index], params[split_index:]
 
         self.positionals = params
 
     def _process_options(self, params: Collection[BaseOption]):
         parent = self.parent
         if parent:
             option_map = parent.option_map.copy()
@@ -231,35 +233,27 @@
             option_map = {}
             combo_option_map = {}
             options = []
 
         for param in params:
             options.append(param)
             opts = param.option_strs
+            if not opts.has_min_opts():
+                raise ParameterDefinitionError(f'No option strings were registered for param={param!r}')
             self._process_option_strs(param, 'long', opts.long, option_map, combo_option_map)
             self._process_option_strs(param, 'short', opts.short, option_map, combo_option_map)
 
         self.options = options
         self.option_map = option_map
         self._process_action_flags(options)
         self.combo_option_map = dict(sorted(combo_option_map.items(), key=lambda kv: (-len(kv[0]), kv[0])))  # noqa
 
-        if self.config and self.config.ambiguous_short_combos == AmbiguousComboMode.STRICT:
+        if self.config.ambiguous_short_combos == AmbiguousComboMode.STRICT:
             self._strict_ambiguous_short_combo_check()
 
-    def _strict_ambiguous_short_combo_check(self):
-        potentially_ambiguous_combo_options = self._potentially_ambiguous_combo_options
-        if not potentially_ambiguous_combo_options:
-            return
-
-        param_conflicts_map = {
-            param: singles.values() for param, singles in potentially_ambiguous_combo_options.values()
-        }
-        raise AmbiguousShortForm(param_conflicts_map)
-
     def _process_option_strs(
         self, param: BaseOption, opt_type: str, opt_strs: List[str], option_map: OptionMap, combo_option_map: OptionMap
     ):
         for opt in opt_strs:
             try:
                 existing = option_map[opt]
             except KeyError:
@@ -273,15 +267,15 @@
 
     def _process_action_flags(self, options: List[BaseOption]):
         action_flags = sorted((p for p in options if isinstance(p, ActionFlag)))
         grouped_ordered_flags = {True: defaultdict(list), False: defaultdict(list)}
         for param in action_flags:
             if param.func is None:
                 raise ParameterDefinitionError(f'No function was registered for param={param!r}')
-            grouped_ordered_flags[param.before_main][param.order].append(param)
+            grouped_ordered_flags[param.before_main][param.order].append(param)  # noqa  # PyCharm infers the wrong type
 
         found_non_always = False
         invalid = {}
         for before_main, prio_params in grouped_ordered_flags.items():
             for prio, params in prio_params.items():
                 param: ActionFlag = params[0]  # Don't pop and check `if params` - all are needed for the group check
                 if found_non_always and param.always_available:
@@ -306,16 +300,93 @@
 
         n_before = len(grouped_ordered_flags[True])
         self.action_flags = action_flags
         self.split_action_flags = action_flags[:n_before], action_flags[n_before:]
 
     # endregion
 
+    # region Ambiguous Short Combo Handling
+
+    def _strict_ambiguous_short_combo_check(self):
+        # Called during initial Option processing when using AmbiguousComboMode.STRICT
+        potentially_ambiguous_combo_options = self._potentially_ambiguous_combo_options
+        if not potentially_ambiguous_combo_options:
+            return
+
+        param_conflicts_map = {
+            param: singles.values() for param, singles in potentially_ambiguous_combo_options.values()
+        }
+        raise AmbiguousShortForm(param_conflicts_map)
+
+    @cached_property
+    def _classified_combo_options(self) -> Tuple[OptionMap, OptionMap]:
+        multi_char_combos = {}
+        single_char_combos = {}
+        for combo, param in self.combo_option_map.items():
+            if len(combo) == 1:
+                single_char_combos[combo] = param
+            else:
+                multi_char_combos[combo] = param
+        return single_char_combos, multi_char_combos
+
+    @cached_property
+    def _potentially_ambiguous_combo_options(self) -> Dict[str, Tuple[BaseOption, OptionMap]]:
+        single_char_combos, multi_char_combos = self._classified_combo_options
+        if not multi_char_combos:
+            return {}
+        return _find_ambiguous_combos(single_char_combos, multi_char_combos)
+
+    @cached_property
+    def _nested_potentially_ambiguous_combo_options(self):
+        single_char_combos, multi_char_combos = self._classified_combo_options
+        for params in self._iter_nested_params():
+            nested_single_char_combos, nested_multi_char_combos = params._classified_combo_options
+            single_char_combos.update(nested_single_char_combos)
+            multi_char_combos.update(nested_multi_char_combos)
+
+        if not multi_char_combos:
+            return {}
+        return _find_ambiguous_combos(single_char_combos, multi_char_combos)
+
+    def _is_combo_potentially_ambiguous(self, option: str) -> Optional[bool]:
+        # Called by short_option_to_param_value_pairs after ensuring the length is > 1
+        to_check = option[1:]  # Strip leading '-'
+        # Note: len(to_check) will never be 2 here - this is only called if len(option) > 2
+        potentially_ambiguous_combo_options = self._nested_potentially_ambiguous_combo_options
+        acm = self.config.ambiguous_short_combos
+        if acm == AmbiguousComboMode.PERMISSIVE and to_check in potentially_ambiguous_combo_options:
+            return True  # Permissive mode allows exact matches of multi-char short forms
+        elif acm == AmbiguousComboMode.IGNORE:
+            return None
+
+        ambiguous = set()
+        for multi, (param, singles) in potentially_ambiguous_combo_options.items():
+            if multi in to_check:
+                ambiguous.add(param)
+                ambiguous.update(p for c, p in singles.items() if c in to_check)
+
+        if ambiguous:
+            raise AmbiguousCombo(ambiguous, option)
+
+        return False
+
+    # endregion
+
     # region Option Processing
 
+    def _iter_nested_params(self) -> Iterator[CommandParameters]:
+        if not self.sub_command:
+            return
+        for choice in self.sub_command.choices.values():
+            command = choice.target
+            try:
+                yield command.__class__.params(command)
+            except AttributeError:  # The target was None (it's a subcommand's local choice)
+                pass
+
     def get_option_param_value_pairs(self, option: str) -> Optional[Tuple[BaseOption, ...]]:
         if option.startswith('---'):
             return None
         elif option.startswith('--'):
             try:
                 opt, param, value = self.long_option_to_param_value_pair(option)
             except KeyError:
@@ -343,75 +414,52 @@
                 raise
 
     def short_option_to_param_value_pairs(self, option: str) -> List[Tuple[str, BaseOption, Optional[str]]]:
         try:
             option, value = option.split('=', 1)
         except ValueError:
             value = None
-
-        if len(option) > 2:  # 2 due to '-' prefix
-            self._ensure_combo_is_unambiguous(option)
+        else:
+            # Note: if the option is not in this Command's option_map, the KeyError is handled by CommandParser
+            return [(option, self.option_map[option], value)]
 
         try:
             param = self.option_map[option]
         except KeyError:
-            if value is not None:
+            opt_len = len(option)
+            if opt_len < 2 or (opt_len > 2 and self._is_combo_potentially_ambiguous(option)):
                 raise
         else:
             return [(option, param, value)]
 
         key, value = option[1], option[2:]
         # value will never be empty if key is a valid option because by this point, option is not a short option
         combo_option_map = self.combo_option_map
         param = combo_option_map[key]
         if param.would_accept(value, short_combo=True):
             return [(key, param, value)]
         else:
+            # Multi-char short options can never be combined with each other, but single-char ones can
             return [(c, combo_option_map[c], None) for c in option[1:]]
 
-    def _ensure_combo_is_unambiguous(self, option: str):
-        # Called by short_option_to_param_value_pairs after ensuring the length is > 1
-        acm = AmbiguousComboMode.PERMISSIVE if not self.config else self.config.ambiguous_short_combos
-        if acm == AmbiguousComboMode.IGNORE:
-            return
-
-        to_check = option[1:]  # Strip leading '-'
-        potentially_ambiguous_combo_options = self._potentially_ambiguous_combo_options
-        if acm == AmbiguousComboMode.PERMISSIVE and to_check in potentially_ambiguous_combo_options:
-            return  # Permissive mode allows exact matches of multi-char short forms
-
-        ambiguous = set()
-        for multi, (param, singles) in potentially_ambiguous_combo_options.items():
-            if multi in to_check:
-                ambiguous.add(param)
-                ambiguous.update(p for c, p in singles.items() if c in to_check)
-
-        if ambiguous:
-            raise AmbiguousCombo(ambiguous, option)
-
     def find_option_that_accepts_values(self, option: str) -> Optional[BaseOption]:
         if option.startswith('--'):
             param = self.long_option_to_param_value_pair(option)[1]
             if param.accepts_values:
                 return param
         elif option.startswith('-'):
             for _, param, _ in self.short_option_to_param_value_pairs(option):
                 if param.accepts_values:
                     return param
         else:
             raise ValueError(f'Invalid option={option!r}')
         return None
 
     def find_nested_option_that_accepts_values(self, option: str) -> Optional[BaseOption]:
-        if not self.sub_command:
-            return None
-
-        for choice in self.sub_command.choices.values():
-            command = choice.target
-            params = command.__class__.params(command)
+        for params in self._iter_nested_params():
             try:
                 param = params.find_option_that_accepts_values(option)
             except KeyError:
                 pass
             else:
                 if param is not None:
                     return param
@@ -419,20 +467,15 @@
             param = params.find_nested_option_that_accepts_values(option)
             if param is not None:
                 return param
 
         return None
 
     def find_nested_pass_thru(self) -> Optional[PassThru]:
-        if not self.sub_command:
-            return None
-
-        for choice in self.sub_command.choices.values():
-            command = choice.target
-            params = command.__class__.params(command)
+        for params in self._iter_nested_params():
             if params._pass_thru:
                 return params._pass_thru
 
         return None
 
     # endregion
 
@@ -445,30 +488,38 @@
                 if exc is None:
                     exc = e
 
         if exc is not None:
             raise exc
 
     def try_env_params(self, ctx: Context) -> Iterator[Option]:
+        """Yields Option parameters that have an environment variable configured, and did not have any CLI values."""
         for param in self.options:
-            try:
-                param.env_var  # noqa
-            except AttributeError:
-                pass
-            else:
-                if ctx.num_provided(param) == 0:
-                    yield param
+            if param.env_var and ctx.num_provided(param) == 0:
+                yield param
 
     def required_check_params(self) -> Iterator[Parameter]:
         ignore = SubCommand
-        yield from (p for p in self.positionals if p.required and not p.group and not isinstance(p, ignore))
+        yield from (p for p in self.all_positionals if p.required and not p.group and not isinstance(p, ignore))
         yield from (p for p in self.options if p.required and not p.group)
         pass_thru = self._pass_thru
         if pass_thru and pass_thru.required and not pass_thru.group:
             yield pass_thru
 
 
 def _find_groups(groups: Set[ParamGroup], param: ParamBase):
     group = param.group
     while group:
         groups.add(group)
         group = group.group
+
+
+def _find_ambiguous_combos(
+    single_char_combos: OptionMap, multi_char_combos: OptionMap
+) -> Dict[str, Tuple[BaseOption, OptionMap]]:
+    ambiguous_combo_options = {}
+    for combo, param in multi_char_combos.items():
+        singles = {c: single_char_combos[c] for c in combo if c in single_char_combos}
+        if singles:
+            ambiguous_combo_options[combo] = (param, singles)
+
+    return ambiguous_combo_options
```

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/commands.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,17 +35,21 @@
     def __new__(cls):
         ctx = get_or_create_context(cls)
         # By storing the Context here instead of __init__, every single subclass won't need to
         # call super().__init__(...) from their own __init__ for this step
         self = super().__new__(cls)
         self.__ctx = ctx
         if not hasattr(self, 'ctx'):
-            self.ctx = ctx
+            self.ctx: Context = ctx  # noqa  # PyCharm complains this is invalid, but doesn't understand it without it
         return self
 
+    def __repr__(self) -> str:
+        cls = self.__class__
+        return f'<{cls.__name__} in prog={cls.__class__.meta(cls).prog!r}>'
+
     # region Parse & Run
 
     @classmethod
     @overload
     def parse_and_run(cls: Type[CommandObj], argv: Argv = None, **kwargs) -> Optional[CommandObj]:
         ...  # These overloads indicate that an instance of the same type or another may be returned
 
@@ -104,30 +108,30 @@
         :param argv: The arguments to parse (defaults to :data:`sys.argv`)
         :return: A Command instance with parsed arguments that is ready for :meth:`.__call__` or :meth:`.main`
         """
         ctx = get_or_create_context(cls, argv)
         cmd_cls = cls
         with ExitStack() as stack:
             stack.enter_context(ctx)
-            sub_cmd = CommandParser.parse_args(ctx)
+            sub_cmd = CommandParser.parse_args_and_get_next_cmd(ctx)
             while sub_cmd:
                 cmd_cls = sub_cmd
                 ctx = stack.enter_context(ctx._sub_context(cmd_cls))
-                sub_cmd = CommandParser.parse_args(ctx)
+                sub_cmd = CommandParser.parse_args_and_get_next_cmd(ctx)
 
             return cmd_cls()
 
     # endregion
 
     def __call__(self, *args, **kwargs) -> int:
         """
         Primary entry point for running a command.  Subclasses generally should not override this method.
 
         Handles exceptions using the configured :class:`.ErrorHandler`.  Alternate error handlers can be specified
-        via the :paramref:`~.core.CommandMeta.__new__.error_handler` parameter during Command class initialization.
+        via the :paramref:`~.core.CommandMeta.error_handler` parameter during Command class initialization.
         To skip error handling, define the class with ``error_handler=None``.
 
         Calls the following methods in order:
 
             #. :meth:`._pre_init_actions_`
             #. :meth:`._init_command_`
             #. :meth:`._before_main_`
@@ -155,19 +159,19 @@
         return ctx.actions_taken
 
     def _pre_init_actions_(self, *args, **kwargs):
         """
         The first method called by :meth:`.__call__` (before :meth:`.main` and others).
 
         Validates the number of ActionFlags that were specified, and calls all of the specified
-        :obj:`~.parameters.before_main` / :obj:`~.parameters.action_flag` actions such as ``--help`` that were
+        :func:`~.options.before_main` / :obj:`~.options.action_flag` actions such as ``--help`` that were
         defined with ``before_main=True`` and ``always_available=True`` in their configured order.
 
-        :param args: Positional arguments to pass to the :obj:`~.parameters.action_flag` methods
-        :param kwargs: Keyword arguments to pass to the :obj:`~.parameters.action_flag` methods
+        :param args: Positional arguments to pass to the :obj:`~.options.action_flag` methods
+        :param kwargs: Keyword arguments to pass to the :obj:`~.options.action_flag` methods
         """
         ctx = self.__ctx
         n_flags = ctx.action_flag_count
         if n_flags and not ctx.config.multiple_action_flags and n_flags > 1:
             raise ParamConflict(ctx.all_action_flags, 'combining multiple action flags is disabled')
 
         before = ctx.categorized_action_flags[ActionPhase.BEFORE_MAIN]
@@ -196,31 +200,31 @@
         """
         pass
 
     def _before_main_(self, *args, **kwargs):
         """
         Called by :meth:`.__call__` after :meth:`._init_command_` and before :meth:`.main` is called.
 
-        Calls all of the specified :obj:`~.parameters.before_main` / :obj:`~.parameters.action_flag` actions that were
-        defined with ``before_main=True`` and ``always_available=False`` in their configured order.
+        Calls all of the specified :func:`~.options.before_main` / :obj:`~.options.action_flag` actions that
+        were defined with ``before_main=True`` and ``always_available=False`` in their configured order.
 
-        :param args: Positional arguments to pass to the :obj:`~.parameters.action_flag` methods
-        :param kwargs: Keyword arguments to pass to the :obj:`~.parameters.action_flag` methods
+        :param args: Positional arguments to pass to the :obj:`~.options.action_flag` methods
+        :param kwargs: Keyword arguments to pass to the :obj:`~.options.action_flag` methods
         """
         for param in self.__ctx.iter_action_flags(ActionPhase.BEFORE_MAIN):
             param.func(self, *args, **kwargs)
 
     def main(self, *args, **kwargs) -> Optional[int]:
         """
         Primary method that is called when running a Command.
 
         If any arguments were specified that are associated with triggering a method that was decorated / registered as
-        a positional :class:`~.parameters.Action`'s target method, then that method is called here.
+        a positional :class:`~.choice_map.Action`'s target method, then that method is called here.
 
-        Commands that do not have any positional :class:`Actions<.parameters.Action>` can override this method, and do
+        Commands that do not have any positional :class:`Actions<.choice_map.Action>` can override this method, and do
         **not** need to call ``super().main(*args, **kwargs)``.
 
         Initialization code that is common for all actions, or that should be run before :meth:`._before_main_` should
         be placed in ``__init__``.
 
         :param args: Positional arguments to pass to the action method
         :param kwargs: Keyword arguments to pass to the action method
@@ -233,25 +237,25 @@
                 action.target()(self, *args, **kwargs)
 
         return ctx.actions_taken
 
     def _after_main_(self, *args, **kwargs):
         """
         Called by :meth:`.__call__` after :meth:`.main` is called.  Calls all of the specified
-        :obj:`~.parameters.after_main` / :obj:`~.parameters.action_flag` actions that were defined with
+        :func:`~.options.after_main` / :obj:`~.options.action_flag` actions that were defined with
         ``before_main=False`` in their configured order.
 
-        :param args: Positional arguments to pass to the :obj:`~.parameters.action_flag` methods
-        :param kwargs: Keyword arguments to pass to the :obj:`~.parameters.action_flag` methods
+        :param args: Positional arguments to pass to the :obj:`~.options.action_flag` methods
+        :param kwargs: Keyword arguments to pass to the :obj:`~.options.action_flag` methods
         """
         for param in self.__ctx.iter_action_flags(ActionPhase.AFTER_MAIN):
             param.func(self, *args, **kwargs)
 
 
-def main(argv: Argv = None, return_command: Bool = False, **kwargs):
+def main(argv: Argv = None, return_command: Bool = False, **kwargs) -> Optional[CommandObj]:
     """
     Convenience function that can be used as the main entry point for a program.
 
     As long as only one :class:`Command` subclass is present, this function will detect it and call its
     :meth:`~Command.parse_and_run` method.  Subcommands do not count as direct subclasses of Command, so this function
     will continue to work even if subcommands are present (as long as they extend their parent command).
```

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/config.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 Configuration options for Command behavior.
 
 :author: Doug Skrypa
 """
 
 from __future__ import annotations
 
+from collections import ChainMap
 from enum import Enum
-from typing import TYPE_CHECKING, Optional, Any, Union, Callable, Type, TypeVar, Generic, Sequence, overload, Dict
+from typing import TYPE_CHECKING, Optional, Any, Union, Callable, Type, TypeVar, Generic, overload, Dict
 
 from .utils import FixedFlag, MissingMixin, _NotSet
 
 if TYPE_CHECKING:
     from .command_parameters import CommandParameters
     from .error_handling import ErrorHandler
     from .formatting.commands import CommandHelpFormatter
@@ -20,14 +21,15 @@
 
 __all__ = [
     'CommandConfig',
     'ShowDefaults',
     'OptionNameMode',
     'SubcommandAliasHelpMode',
     'AmbiguousComboMode',
+    'AllowLeadingDash',
     'DEFAULT_CONFIG',
 ]
 
 CV = TypeVar('CV')
 DV = TypeVar('DV')
 ConfigValue = Union[CV, DV]
 
@@ -79,14 +81,17 @@
     :UNDERSCORE: ``--foo_bar``
     :DASH: ``--foo-bar``
     :BOTH: Both ``--foo-bar`` and ``--foo_bar`` will be accepted
     :BOTH_UNDERSCORE: Both ``--foo-bar`` and ``--foo_bar`` will be accepted, but only ``--foo_bar`` with be displayed
       in help text
     :BOTH_DASH: Both ``--foo-bar`` and ``--foo_bar`` will be accepted, but only ``--foo-bar`` with be displayed
       in help text
+    :NONE: No long form option string will be added.  At least one short form option string must be defined.  Note that
+      it is NOT necessary to use ``name_mode=None`` to prevent the automatic creation of long form option strings - if
+      any long form option strings are explicitly provided for a given Parameter, then no automatic ones will be added.
 
     If a long form is provided explicitly for a given optional Parameter, then this setting will be ignored.
 
     The value may be specified to Commands as ``option_name_mode=<mode>`` or to Parameters as ``name_mode=<mode>``,
     where ``<mode>`` is one of:
 
         - ``OptionNameMode.UNDERSCORE`` or ``OptionNameMode.DASH`` or ``OptionNameMode.BOTH``
@@ -97,22 +102,23 @@
 
     UNDERSCORE = 1
     DASH = 2
     BOTH = 3                # = 1|2
     #                         & 4  -> display options set
     BOTH_UNDERSCORE = 15    # & 8  -> show only underscore version
     BOTH_DASH = 23          # & 16 -> show only dash version
+    NONE = 32
 
     @classmethod
-    def _missing_(cls, value: Union[str, int]) -> OptionNameMode:
+    def _missing_(cls, value: Union[str, int, None]) -> OptionNameMode:
         try:
             return OPT_NAME_MODE_ALIASES[value]
         except KeyError:
             pass
-        return super()._missing_(value)
+        return cls.NONE if value is None else super()._missing_(value)
 
 
 OPT_NAME_MODE_ALIASES = {
     '-': OptionNameMode.DASH,
     '_': OptionNameMode.UNDERSCORE,
     '*': OptionNameMode.BOTH,
     '-_': OptionNameMode.BOTH,
@@ -174,80 +180,98 @@
     """
 
     IGNORE = 'ignore'           # Ignore potentially ambiguous combinations of short options entirely
     PERMISSIVE = 'permissive'   # Allow multi-char short options that overlap with a single char one for exact matches
     STRICT = 'strict'           # Reject multi-char short options that overlap with a single char one before parsing
 
 
+class AllowLeadingDash(Enum):
+    """
+    How a given Parameter should handle values with a leading dash (``-``).  Only configurable at the Parameter level,
+    not the Command level.
+
+    The behavior based on each supported option:
+
+    :NUMERIC: Allow numeric values like ``-5`` and ``-1.3``, but reject values like ``-d``.
+    :ALWAYS: Always allow values with a leading dash.
+    :NEVER: Never allow values with a leading dash.
+    """
+
+    NUMERIC = 'numeric'     # Allow a leading dash when the value is numeric
+    ALWAYS = 'always'       # Always allow a leading dash
+    NEVER = 'never'         # Never allow a leading dash
+
+    @classmethod
+    def _missing_(cls, value):
+        if isinstance(value, str):
+            try:
+                return cls._member_map_[value.upper()]  # noqa
+            except KeyError:
+                pass
+        elif value is True:
+            return cls.ALWAYS
+        elif value is False:
+            return cls.NEVER
+        return super()._missing_(value)  # noqa
+
+
 # endregion
 
 
 class ConfigItem(Generic[CV, DV]):
     __slots__ = ('default', 'type', 'name')
 
     def __init__(self, default: DV, type: Callable[[Any], CV] = None):  # noqa
         self.default = default
         self.type = type
 
     def __set_name__(self, owner: Type[CommandConfig], name: str):
         self.name = name
         owner.FIELDS.add(name)
 
-    def get_value(self, instance: CommandConfig) -> ConfigValue:
-        try:
-            return instance.__dict__[self.name]
-        except KeyError:
-            pass
-
-        for parent in instance.parents:
-            try:
-                return self.get_value(parent)
-            except KeyError:
-                pass
-
-        raise KeyError
-
     @overload
     def __get__(self, instance: None, owner: Type[CommandConfig]) -> ConfigItem[CV, DV]:
         ...
 
     @overload
     def __get__(self, instance: CommandConfig, owner: Type[CommandConfig]) -> ConfigValue:
         ...
 
     def __get__(self, instance, owner):
         if instance is None:
             return self
-        try:
-            return self.get_value(instance)
-        except KeyError:
-            return self.default
+        return instance._data.get(self.name, self.default)
 
     def __set__(self, instance: CommandConfig, value: ConfigValue):
         if instance._read_only:
             raise AttributeError(f'Unable to set attribute {self.name}={value!r} because {instance} is read-only')
         elif self.type is not None:
             value = self.type(value)
-        instance.__dict__[self.name] = value
+        instance._data[self.name] = value
 
     def __delete__(self, instance: CommandConfig):
         if instance._read_only:
             raise AttributeError(f'Unable to delete attribute {self.name} because {instance} is read-only')
         try:
-            del instance.__dict__[self.name]
+            del instance._data[self.name]
         except KeyError as e:
             raise AttributeError(f'No {self.name!r} config was stored for {instance}') from e
 
     def __repr__(self) -> str:
         return f'<{self.__class__.__name__}({self.default!r}, type={self.type!r})>'
 
 
 class CommandConfig:
     """Configuration options for Commands."""
 
+    # Note: PyCharm may incorrectly think ConfigItem attrs are read only: https://youtrack.jetbrains.com/issue/PY-29770
+
+    __slots__ = ('_data', '_read_only')
+    _data: ChainMap
+    _read_only: bool
     FIELDS = set()
 
     # region Error Handling Options
 
     #: The :class:`.ErrorHandler` to be used by :meth:`.Command.__call__`
     error_handler: Optional[ErrorHandler] = ConfigItem(_NotSet)
 
@@ -341,34 +365,30 @@
     usage_column_width: int = ConfigItem(30, int)
 
     #: Min width (in chars) for the usage column in help text after adjusting for group indentation / terminal width
     min_usage_column_width: int = ConfigItem(20, int)
 
     # endregion
 
-    def __init__(self, parents: Optional[Sequence[CommandConfig]] = None, read_only: bool = False, **kwargs):
-        self.parents = parents or ()
+    def __init__(self, parent: Optional[CommandConfig] = None, read_only: bool = False, **kwargs):
+        self._data = parent._data.new_child() if parent else ChainMap()
         self._read_only = read_only
-        fields = self.FIELDS
-        for key, val in kwargs.items():
-            if key in fields:
-                setattr(self, key, val)
-            else:
-                # The number of times one or more invalid options will be provided is extremely low compared to how
-                # often this exception will not need to be raised, so the re-iteration over kwargs is acceptable.
-                # This also avoids creating the `bad` dict that would otherwise be thrown away on 99.9% of init calls.
-                bad = ', '.join(sorted(key for key in kwargs if key not in fields))
-                raise TypeError(f'Invalid configuration - unsupported options: {bad}')
+        if kwargs:
+            try:
+                for key, val in kwargs.items():
+                    setattr(self, key, val)
+            except AttributeError:
+                bad = set(kwargs).difference(self.FIELDS)
+                raise TypeError(f'Invalid configuration - unsupported options: {", ".join(sorted(bad))}') from None
 
     def __repr__(self) -> str:
         settings = ', '.join(f'{k}={v!r}' for k, v in self.as_dict(False).items())
-        cfg_str = f', {settings}' if settings else ''
-        return f'<{self.__class__.__name__}(parents={self.parents!r}{cfg_str})>'
+        return f'<{self.__class__.__name__}[depth={len(self._data.maps)}]({settings})>'
 
     def as_dict(self, full: Bool = True) -> Dict[str, Any]:
         """Return a dict representing the configured options."""
         if full:
             return {key: getattr(self, key) for key in self.FIELDS}
-        return {key: val for key, val in self.__dict__.items() if key in self.FIELDS}
+        return {key: val for key, val in self._data.items() if key in self.FIELDS}
 
 
-DEFAULT_CONFIG = CommandConfig(read_only=True)
+DEFAULT_CONFIG: CommandConfig = CommandConfig(read_only=True)
```

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/context.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/context.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,87 +8,64 @@
 from __future__ import annotations
 
 import sys
 from collections import defaultdict
 from contextlib import AbstractContextManager
 from contextvars import ContextVar
 from enum import Enum
+from functools import cached_property
 from inspect import Signature, Parameter as _Parameter
 from typing import TYPE_CHECKING, Any, Callable, Union, Sequence, Optional, Iterator, Collection, cast
 from typing import Dict, Tuple, List
 
-try:
-    from functools import cached_property
-except ImportError:
-    from .compat import cached_property
-
 from .config import CommandConfig, DEFAULT_CONFIG
 from .error_handling import ErrorHandler, NullErrorHandler, extended_error_handler
 from .exceptions import NoActiveContext, MissingArgument
 from .utils import _NotSet, Terminal
 
 if TYPE_CHECKING:
     from .command_parameters import CommandParameters
     from .commands import Command
     from .parameters import Parameter, ActionFlag
     from .typing import Bool, ParamOrGroup, CommandType, AnyConfig, OptStr, PathLike
 
-__all__ = [
-    'Context',
-    'ctx',
-    'get_current_context',
-    'get_or_create_context',
-    'get_context',
-    'get_parsed',
-    'get_raw_arg',
-    'ParseState',
-]
+__all__ = ['Context', 'ctx', 'get_current_context', 'get_or_create_context', 'get_context', 'get_parsed', 'get_raw_arg']
 
 _context_stack = ContextVar('cli_command_parser.context.stack', default=[])
 _TERMINAL = Terminal()
 
 
-class ParseState(Enum):
-    INITIAL = 1
-    COMPLETE = 2
-    FAILED = 3
-
-    @property
-    def done(self) -> bool:
-        return self._value_ > 1
-
-
 class Context(AbstractContextManager):  # Extending AbstractContextManager to make PyCharm's type checker happy
     """
     The parsing context.
 
     Holds user input while parsing, and holds the parsed values.  Handles config overrides / hierarchy for settings that
     affect parser behavior.
     """
 
     config: CommandConfig
     prog: OptStr = None
     _terminal_width: Optional[int]
     allow_argv_prog: Bool = True
+    _provided: Dict[ParamOrGroup, int]
 
     def __init__(
         self,
         argv: Optional[Sequence[str]] = None,
         command: Optional[CommandType] = None,
         parent: Optional[Context] = None,
         config: AnyConfig = None,
         terminal_width: int = None,
         allow_argv_prog: Bool = None,
         **kwargs,
     ):
         self.command = command
         self.parent = parent
-        self.state = ParseState.INITIAL
         self.config = _normalize_config(config, kwargs, parent, command)
-        if parent is not None:
+        if parent:
             self._set_argv(parent.prog, argv)
             self._parsed = parent._parsed.copy()
             self.unknown = parent.unknown.copy()
             self._provided = parent._provided.copy()
             if terminal_width is None:
                 terminal_width = parent._terminal_width
             if allow_argv_prog is None:
@@ -124,16 +101,15 @@
 
     def _sub_context(self, command: CommandType, argv: Optional[Sequence[str]] = None, **kwargs) -> Context:
         if argv is None:
             argv = self.remaining
         return self.__class__(argv, command, parent=self, **kwargs)
 
     def __repr__(self) -> str:
-        cmd_name = getattr(self.command, '__name__', None)
-        return f'<{self.__class__.__name__}[state={self.state}, command={cmd_name}]>'
+        return f'<{self.__class__.__name__}[command={getattr(self.command, "__name__", None)}]>'
 
     def __enter__(self) -> Context:
         _context_stack.get().append(self)
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         _context_stack.get().pop()
@@ -178,15 +154,15 @@
             if recursive and self.parent:
                 parsed = self.parent.get_parsed(exclude, recursive)
             else:
                 parsed = {}
 
             params = self.params
             if params:
-                for group in (params.positionals, params.options, (params.pass_thru,)):
+                for group in (params.all_positionals, params.options, (params.pass_thru,)):
                     for param in group:
                         if param and param not in exclude:
                             try:
                                 parsed[param.name] = param.result_value()
                             except MissingArgument:
                                 parsed[param.name] = None
 
@@ -216,15 +192,15 @@
     # region Parsing
 
     def get_parsed_value(self, param: Parameter):
         """Not intended to be called by users.  Used by Parameters to access their parsed values."""
         try:
             return self._parsed[param]
         except KeyError:
-            self._parsed[param] = value = param._init_value_factory(self.state)
+            self._parsed[param] = value = param._init_value_factory()
             return value
 
     def set_parsed_value(self, param: Parameter, value: Any):
         """Not intended to be called by users.  Used by Parameters during parsing to store parsed values."""
         self._parsed[param] = value
 
     def record_action(self, param: ParamOrGroup, val_count: int = 1):
@@ -233,14 +209,17 @@
         """
         self._provided[param] += val_count
 
     def num_provided(self, param: ParamOrGroup) -> int:
         """Not intended to be called by users.  Used by Parameters during parsing to handle nargs."""
         return self._provided[param]
 
+    def get_missing(self) -> List[Parameter]:
+        return [p for p in self.params.required_check_params() if self._provided[p] == 0]
+
     # endregion
 
     # region Actions
 
     @cached_property
     def _parsed_action_flags(self) -> Tuple[int, List[ActionFlag], List[ActionFlag]]:
         """
@@ -303,28 +282,24 @@
 
 
 def _normalize_config(
     config: AnyConfig, kwargs: Dict[str, Any], parent: Optional[Context], command: Optional[CommandType]
 ) -> CommandConfig:
     if config is not None:
         if kwargs:
-            raise ValueError(f'Cannot combine config={config!r} with keyword config arguments={kwargs}')
+            raise TypeError(f'Cannot combine config={config!r} with keyword config arguments={kwargs}')
         elif isinstance(config, CommandConfig):
             return config
         kwargs = config
 
-    parents = []
-    if parent and parent.config:
-        parents.append(parent.config)
-    if command is not None:
-        cmd_cfg = command.__class__.config(command)
-        if cmd_cfg:
-            parents.append(cmd_cfg)
+    if parent:
+        for key, val in parent.config._data.items():
+            kwargs.setdefault(key, val)
 
-    return CommandConfig(parents=parents, **kwargs)
+    return CommandConfig(parent=command.__class__.config(command) if command is not None else None, **kwargs)
 
 
 class ActionPhase(Enum):
     PRE_INIT = 0
     BEFORE_MAIN = 1
     AFTER_MAIN = 2
 
@@ -352,15 +327,15 @@
 
     def __eq__(self, other) -> bool:
         return get_current_context() == other
 
     def __contains__(self, item) -> bool:
         return item in get_current_context()
 
-    def __enter__(self):
+    def __enter__(self) -> Context:
         return get_current_context().__enter__()
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         return get_current_context().__exit__(exc_type, exc_val, exc_tb)
 
     @property
     def terminal_width(self) -> int:
```

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/conversion/argparse_ast.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/conversion/argparse_ast.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from __future__ import annotations
 
 import ast
 import logging
 import sys
 from argparse import ArgumentParser
 from ast import AST, Assign, Call, withitem
-from functools import partial
+from functools import partial, cached_property
 from inspect import Signature, BoundArguments
 from pathlib import Path
 from typing import TYPE_CHECKING, Union, Optional, Callable, Collection, TypeVar, Generic, Type, Iterator
 from typing import List, Tuple, Dict, Set
 
-from cli_command_parser.compat import cached_property
 from .argparse_utils import ArgumentParser as _ArgumentParser, SubParsersAction as _SubParsersAction
 from .utils import get_name_repr, iter_module_parents, unparse
 
 if TYPE_CHECKING:
     from cli_command_parser.typing import PathLike
     from .visitor import TrackedRefMap, TrackedRef
```

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/conversion/argparse_utils.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/conversion/argparse_utils.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/conversion/command_builder.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/conversion/command_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,66 +1,74 @@
 from __future__ import annotations
 
 import keyword
 import logging
 from abc import ABC, abstractmethod
-from ast import literal_eval, Attribute, Name, GeneratorExp, Subscript, DictComp, ListComp, SetComp
+from ast import literal_eval, Attribute, Name, GeneratorExp, Subscript, DictComp, ListComp, SetComp, Constant, Str
 from dataclasses import dataclass, fields
+from functools import cached_property
 from itertools import count
 from typing import TYPE_CHECKING, Union, Optional, Iterator, Iterable, Type, TypeVar, Generic, List, Tuple
 
-from cli_command_parser.compat import cached_property
 from cli_command_parser.nargs import Nargs
 from .argparse_ast import AC, ParserArg, ArgGroup, MutuallyExclusiveGroup, AstArgumentParser, Script
 from .utils import collection_contents, unparse
 
 if TYPE_CHECKING:
     from cli_command_parser.typing import OptStr
     from .argparse_ast import ArgCollection
 
 __all__ = ['convert_script']
 log = logging.getLogger(__name__)
 
 C = TypeVar('C', bound='Converter')
 
 RESERVED = set(keyword.kwlist) | set(getattr(keyword, 'softkwlist', ('_', 'case', 'match')))  # soft was added in 3.9
+# TODO: Handle argparse.SUPPRESS ('==SUPPRESS==')
 
 
-def convert_script(script: Script) -> str:
-    return ScriptConverter(script).convert()
+def convert_script(script: Script, add_methods: bool = False) -> str:
+    return ScriptConverter(script, add_methods=add_methods).convert()
 
 
-class Converter(ABC):
+class Converter(Generic[AC], ABC):
     converts: Type[AC] = None
+    newline_between_members: bool = False
     _ac_converter_map = {}
 
-    def __init_subclass__(cls, converts: Type[AC] = None, **kwargs):
+    def __init_subclass__(cls, converts: Type[AC] = None, newline_between_members: bool = None, **kwargs):
         super().__init_subclass__(**kwargs)
         if converts:
             cls.converts = converts
             cls._ac_converter_map[converts] = cls
+        if newline_between_members is not None:
+            cls.newline_between_members = newline_between_members
 
     def __init__(self, ast_obj: Union[AC, Script], parent: Optional[Converter] = None):
         self.ast_obj = ast_obj
         self.parent = parent
 
     @classmethod
-    def for_ast_callable(cls, ast_obj: Union[AC, Type[AC]]) -> Type[Converter]:
+    def for_ast_callable(cls, ast_obj: Union[AC, Type[AC]]) -> Type[Converter[AC]]:
         if not isinstance(ast_obj, type):
             ast_obj = ast_obj.__class__
         try:
             return cls._ac_converter_map[ast_obj]
         except KeyError:
             pass
         for converts_cls, converter_cls in cls._ac_converter_map.items():
             if issubclass(ast_obj, converts_cls):
                 return converter_cls
         raise TypeError(f'No Converter is registered for {ast_obj.__class__.__name__} objects')
 
     @classmethod
+    def init_for_ast_callable(cls, ast_obj: AC, *args, **kwargs) -> Converter[AC]:
+        return cls.for_ast_callable(ast_obj)(ast_obj, *args, **kwargs)
+
+    @classmethod
     def init_group(cls: Type[C], parent: CollectionConverter, ast_objs: List[AC]) -> ConverterGroup[C]:
         return ConverterGroup(parent, cls, [cls(ast_obj, parent) for ast_obj in ast_objs])
 
     def convert(self, indent: int = 0) -> str:
         return '\n'.join(self.format_lines(indent))
 
     @abstractmethod
@@ -82,31 +90,38 @@
     def __getitem__(self, index: int) -> C:
         return self.members[index]
 
     def __iter__(self) -> Iterator[C]:
         yield from self.members
 
     def format_all(self, indent: int = 0) -> Iterator[str]:
-        for member in self.members:
+        newline_between_members = self.member_type.newline_between_members
+        for i, member in enumerate(self.members):
+            if i and newline_between_members:
+                yield ''
             yield from member.format_lines(indent)
 
 
 class ScriptConverter(Converter, converts=Script):
+    def __init__(self, *args, add_methods: bool = False, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.add_methods = add_methods
+
     def format_lines(self, indent: int = 0) -> Iterator[str]:
         # TODO: Filter to what is actually used
         yield (
             'from cli_command_parser import'
             ' Command, SubCommand, ParamGroup, Positional, Option, Flag, Counter, PassThru, main'
         )
         counter = count()
         for parser in self.ast_obj.parsers:
-            yield from ParserConverter(parser, counter=counter).format_lines()
+            yield from ParserConverter(parser, counter=counter, add_methods=self.add_methods).format_lines()
 
 
-class CollectionConverter(Converter, ABC):
+class CollectionConverter(Converter[AC], ABC):
     ast_obj: ArgCollection
     parent: CollectionConverter | None
     _name_mode = None
 
     @cached_property
     def name_mode(self) -> str | None:
         return self._name_mode or (self.parent.name_mode if self.parent else None)
@@ -129,46 +144,82 @@
         last = False
         for child_group in self.grouped_children:
             if last and child_group and issubclass(child_group.member_type, GroupConverter):
                 yield ''
             yield from child_group.format_all(indent)
             last = bool(child_group)
 
-        if not any(cg for cg in self.grouped_children):
-            yield f'{prefix}    pass'
+        yield from self.finalize(any(cg for cg in self.grouped_children), prefix, indent)
 
+    def finalize(self, had_members: bool, prefix: str, indent: int = 4):
+        if not had_members:
+            yield f'{prefix}{" " * indent}pass'
 
-class ParserConverter(CollectionConverter, converts=AstArgumentParser):
+
+class ParserConverter(CollectionConverter[AstArgumentParser], converts=AstArgumentParser):
     _auto_gen_disclaimer = '# This is an automatically generated name that should probably be updated'
     ast_obj: AstArgumentParser
     parent: ParserConverter | None
 
-    def __init__(self, parser: AstArgumentParser, parent: ParserConverter = None, counter: count = None):
+    def __init__(
+        self,
+        parser: AstArgumentParser,
+        parent: ParserConverter = None,
+        counter: count = None,
+        *,
+        add_methods: bool = False,
+    ):
         super().__init__(parser, parent)
         self.counter = count() if counter is None else counter
+        self.add_methods = add_methods
 
     @cached_property
     def sub_parser_converters(self) -> List[ParserConverter]:
-        return [self.__class__(sub_parser, self, self.counter) for sub_parser in self.ast_obj.sub_parsers]
+        cls, add_methods = self.__class__, self.add_methods
+        return [cls(sub_parser, self, self.counter, add_methods=add_methods) for sub_parser in self.ast_obj.sub_parsers]
 
     def descendant_args(self) -> Iterator[ParamConverter]:
         yield from super().descendant_args()
         for sp_converter in self.sub_parser_converters:
             yield from sp_converter.descendant_args()
 
     def format_lines(self, indent: int = 0) -> Iterator[str]:
         suffix = f'  {self._auto_gen_disclaimer}' if self.parent is None else ''
-        # TODO: Add _init_command_ and/or main methods
         # TODO: If subparsers have no unique args, use action methods instead?
         yield '\n'
         yield f'class {self.name}({self._get_args()}):{suffix}'
         yield from self.format_members('')
         for sp_converter in self.sub_parser_converters:
             yield from sp_converter.format_lines()
 
+    def finalize(self, had_members: bool, prefix: str, indent: int = 4):
+        if not self.add_methods:
+            yield from super().finalize(had_members, prefix, indent)
+            return
+
+        if had_members:
+            yield ''
+
+        had_last = False
+        prefix += ' ' * indent
+        if not self.is_sub_parser:
+            had_members = had_last = True
+            yield f'{prefix}def _init_command_(self):'
+            yield f'{prefix}    pass'
+
+        if not self.sub_parser_converters:
+            had_members = True
+            if had_last:
+                yield ''
+            yield f'{prefix}def main(self):'
+            yield f'{prefix}    pass'
+
+        if not had_members:  # This case is unlikely, but here just in case
+            yield f'{prefix}pass'
+
     def _get_args(self) -> str:
         kwargs = self.ast_obj.init_func_kwargs.copy()
         # log.debug(f'Processing args for {kwargs}')
         kwargs['option_name_mode'] = self._name_mode
         if self.is_sub_parser:
             key, value = self._choices
             if key:
@@ -236,25 +287,26 @@
             return None
         name_modes = {pc._name_mode for pc in self.descendant_args() if pc.is_option and '_' in pc.attr_name}
         return next(iter(name_modes)) if len(name_modes) == 1 else None
 
     # endregion
 
 
-class GroupConverter(CollectionConverter, converts=ArgGroup):
+class GroupConverter(CollectionConverter[ArgGroup], converts=ArgGroup, newline_between_members=True):
     ast_obj: ArgGroup
 
     def format_lines(self, indent: int = 4) -> Iterator[str]:
         prefix = ' ' * indent
         yield f'{prefix}with ParamGroup({self._get_args()}):'
         yield from self.format_members(prefix, indent + 4)
 
     def _get_args(self) -> str:
         # log.debug(f'Processing args for {self.ast_obj._init_func_bound}')
         description = self.ast_obj.init_func_kwargs.get('description')
+        # TODO: Missing required=True
         title = self.ast_obj.init_func_kwargs.get('title')
         if title:
             title_str = literal_eval(title)
             if title_str.lower().endswith(' options'):
                 if description:
                     title = repr(title_str[:-7].rstrip())
                 else:
@@ -264,15 +316,15 @@
         if description:
             args.append(f'description={description}')
         if isinstance(self.ast_obj, MutuallyExclusiveGroup):
             args.append('mutually_exclusive=True')
         return ', '.join(args)
 
 
-class ParamConverter(Converter, converts=ParserArg):
+class ParamConverter(Converter[ParserArg], converts=ParserArg):
     ast_obj: ParserArg
     parent: CollectionConverter | None
     _counter = count()
 
     def __init__(self, arg: ParserArg, parent: CollectionConverter, num: int):
         super().__init__(arg, parent)
         self.num = num
@@ -316,14 +368,18 @@
         return "'_'" if '_' in self._attr_name else None
 
     @cached_property
     def _attr_name(self) -> str:
         return next(name for name in self._attr_name_candidates() if name not in RESERVED)
 
     def _attr_name_candidates(self) -> Iterator[str]:
+        dest = self.ast_obj.init_func_raw_kwargs.get('dest')
+        if dest is not None and isinstance(dest, (Constant, Str)):  # Str is for 3.7 compatibility
+            yield getattr(dest, dest._fields[0])  # .value for Constant, .s for Str
+
         long, short, plain = self._grouped_opt_strs
         if self.is_positional or self.is_pass_thru:
             yield from plain
         if self.is_option or self.is_pass_thru:
             for group in (long, short):
                 for opt in group:
                     opt = opt.lstrip('-')
@@ -391,14 +447,15 @@
     # region High Level Param Type
 
     @cached_property
     def is_pass_thru(self) -> bool:
         nargs = self.ast_obj.init_func_kwargs.get('nargs')
         if not nargs:
             return False
+        # TODO: Refactor to take advantage of new nargs=REMAINDER support
         return nargs in self.ast_obj.get_tracked_refs('argparse', 'REMAINDER', ())
 
     @cached_property
     def is_positional(self) -> bool:
         long, short, plain = self._grouped_opt_strs
         return plain and not long and not short
 
@@ -589,17 +646,24 @@
         try:
             value, opposite = values[action]
         except KeyError:
             if action == 'store_const':
                 action = None
         else:
             if default == opposite:
-                default = None
+                const = None
+                if action == 'store_true':
+                    default = None
+            elif not default and action == 'store_false':
+                default = 'True'
+                const = None
+            else:
+                const = value if default else None
+
             action = None
-            const = value if default else None
 
         kwargs['type'] = kwargs['nargs'] = None
         if action:
             action = repr(action)
         return cls.from_kwargs(action=action, const=const, default=default, **kwargs)
 
     @classmethod
```

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/conversion/utils.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/conversion/utils.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/conversion/visitor.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/conversion/visitor.py`

 * *Files 3% similar despite different names*

```diff
@@ -133,28 +133,30 @@
 
         if not visited_any:
             self.generic_visit(node)
 
     # endregion
 
     def resolve_ref(self, name: Union[str, AST, Attribute, Name, expr]):
-        if not isinstance(name, str):
-            name = get_name_repr(name)
-        try:
-            return self.scopes[name]
-        except KeyError:
-            pass
-        try:
-            obj_name, attr = name.rsplit('.', 1)
-        except ValueError:
-            return None
-        try:
-            obj = self.scopes[obj_name]
-        except KeyError:
-            return None
+        if isinstance(name, Attribute) and isinstance(name.value, Call):
+            obj = self.visit_Call(name.value)
+            attr = name.attr
+        else:
+            if not isinstance(name, str):
+                name = get_name_repr(name)
+            try:
+                return self.scopes[name]
+            except KeyError:
+                pass
+            try:
+                obj_name, attr = name.rsplit('.', 1)
+                obj = self.scopes[obj_name]
+            except (ValueError, KeyError):
+                return None
+
         try:
             can_call = attr in obj.visit_funcs
         except (AttributeError, TypeError):
             return None
         return getattr(obj, attr) if can_call else None
 
     def visit_withitem(self, item):
```

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/core.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,33 +4,35 @@
 
 :author: Doug Skrypa
 """
 
 from __future__ import annotations
 
 from abc import ABC, ABCMeta
-from typing import TYPE_CHECKING, Optional, Union, TypeVar, Callable, Iterable, Collection, Any, Mapping, Sequence
+from typing import TYPE_CHECKING, Optional, Union, TypeVar, Callable, Iterable, Collection, Any, Mapping, Iterator
 from typing import Dict, Tuple, List
 from warnings import warn
 from weakref import WeakSet
 
 from .command_parameters import CommandParameters
-from .config import CommandConfig
+from .config import CommandConfig, DEFAULT_CONFIG
 from .exceptions import CommandDefinitionError
 from .metadata import ProgramMetadata
 
 if TYPE_CHECKING:
     from .typing import Config, AnyConfig, CommandCls, CommandAny, OptStr, Bool
 
 __all__ = ['CommandMeta', 'get_parent', 'get_config', 'get_params', 'get_metadata', 'get_top_level_commands']
 
 Bases = Union[Tuple[type, ...], Iterable[type]]
 Choices = Union[Mapping[str, Optional[str]], Collection[str]]
 T = TypeVar('T')
 
+META_KEYS = {'prog', 'usage', 'description', 'epilog', 'doc_name'}
+
 
 class CommandMeta(ABCMeta, type):
     # noinspection PyUnresolvedReferences
     """
     :param choice: SubCommand value to map to this command.
     :param choices: SubCommand values to map to this command.  Optionally, a mapping of ``{choice: help text}`` may be
       provided to customize the help text displayed for each choice.
@@ -68,16 +70,15 @@
         *,
         choice: str = None,
         choices: Choices = None,
         help: str = None,  # noqa
         config: AnyConfig = None,
         **kwargs,
     ) -> CommandCls:
-        meta_iter = ((k, kwargs.pop(k, None)) for k in ('prog', 'usage', 'description', 'epilog', 'doc_name'))
-        metadata = {k: v for k, v in meta_iter if v}
+        metadata = {k: v for k, v in ((k, kwargs.pop(k)) for k in META_KEYS.intersection(kwargs)) if v}
         namespace['_CommandMeta__params'] = None  # Prevent commands from inheriting parent params
         namespace['_CommandMeta__metadata'] = None  # Prevent commands from inheriting parent metadata directly
         namespace['_CommandMeta__parents'] = None  # Prevent commands from inheriting parents directly
 
         config = mcs._prepare_config(bases, config, kwargs)
         if config:
             namespace['_CommandMeta__config'] = config
@@ -125,27 +126,27 @@
         if config is not None:
             if kwargs:
                 raise CommandDefinitionError(f'Cannot combine config={config!r} with keyword config arguments={kwargs}')
             elif isinstance(config, CommandConfig):
                 return config
             kwargs = config  # It was a dict
 
-        parent = mcs._from_parent(mcs.config, bases)
-        if kwargs or (not parent and ABC not in bases):
+        parent_config = mcs._from_parent(mcs.config, bases)
+        if kwargs or (not parent_config and ABC not in bases):
             cfg_kwargs = {k: kwargs.pop(k) for k in CommandConfig.FIELDS.intersection(kwargs)}
-            return CommandConfig(parents=(parent,) if parent else (), **cfg_kwargs)
+            return CommandConfig(parent=parent_config, **cfg_kwargs)
 
         return None
 
     @classmethod
-    def config(mcs, cls: CommandAny) -> Config:
+    def config(mcs, cls: CommandAny, default: T = None) -> Union[CommandConfig, T]:
         try:
             return cls.__config     # This attr is not overwritten for every subclass
         except AttributeError:      # This means that the Command and all of its parents have no custom config
-            return None
+            return default
 
     # endregion
 
     @classmethod
     def parent(mcs, cls: CommandAny, include_abc: bool = True) -> Optional[CommandCls]:
         """
         :param cls: A Command class or object
@@ -158,20 +159,15 @@
         try:
             first, parent = cls.__parents  # Works for both Command objects and classes
         except TypeError:
             pass
         else:
             return first if include_abc else parent
 
-        try:
-            mro = type.mro(cls)[1:]
-        except TypeError:  # a Command object was provided instead of a Command class
-            cls = cls.__class__
-            mro = type.mro(cls)[1:]
-
+        cls, mro = _mro(cls)
         first = parent = None
         for parent_cls in mro:
             if isinstance(parent_cls, mcs):
                 if first is None:
                     first = parent_cls
                 if ABC not in parent_cls.__bases__:
                     parent = parent_cls
@@ -184,39 +180,48 @@
     def params(mcs, cls: CommandCls) -> CommandParameters:
         # Late initialization is necessary to allow late assignment of Parameters for now
         try:
             params = cls.__params
         except AttributeError:
             raise TypeError('CommandParameters are only available for Command subclasses') from None
         if not params:
-            cls.__params = params = CommandParameters(cls, mcs.parent(cls, True), mcs.config(cls))
+            parent = mcs.parent(cls, True)
+            parent_params = mcs.params(parent) if parent is not None else None
+            cls.__params = params = CommandParameters(cls, parent, parent_params, mcs.config(cls, DEFAULT_CONFIG))
         return params
 
     @classmethod
-    def meta(mcs, cls: CommandCls, no_sys_argv: Bool = False) -> Optional[ProgramMetadata]:
+    def meta(mcs, cls: CommandCls, no_sys_argv: Bool = False) -> ProgramMetadata:
         meta = cls.__metadata
         if not meta:
             parent_meta = mcs._from_parent(mcs.meta, type.mro(cls)[1:])
             cls.__metadata = meta = ProgramMetadata.for_command(cls, parent=parent_meta, no_sys_argv=no_sys_argv)
         return meta
 
 
-def _choice_items(choice: OptStr, choices: Optional[Choices]) -> Sequence[Tuple[OptStr, OptStr]]:
-    if not choices:
-        return ((choice, None),)  # noqa
-
+def _mro(cmd_cls):
     try:
-        items = {kv: None for kv in choices.items()}
-    except AttributeError:
-        items = {(c, None): None for c in choices}
+        return cmd_cls, type.mro(cmd_cls)[1:-1]  # 0 is always the class itself, -1 is always object
+    except TypeError:  # a Command object was provided instead of a Command class
+        cmd_cls = cmd_cls.__class__
+        return cmd_cls, type.mro(cmd_cls)[1:-1]
+
 
-    if choice:
-        return {(choice, None): None, **items}
+def _choice_items(choice: OptStr, choices: Optional[Choices]) -> Iterator[Tuple[OptStr, OptStr]]:
+    if not choices:
+        yield choice, None
     else:
-        return items
+        try:
+            items = choices.items()
+        except AttributeError:  # Choices is not a dict of choice:help
+            items = ((c, None) for c in choices)
+
+        if choice and choice not in choices:
+            yield choice, None
+        yield from items
 
 
 get_parent = CommandMeta.parent
 get_config = CommandMeta.config
 get_metadata = CommandMeta.meta
```

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/documentation.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/documentation.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/exceptions.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,34 +37,35 @@
     'NoActiveContext',
 ]
 
 
 class CommandParserException(Exception):
     """Base class for all other Command Parser exceptions"""
 
-    code: int = 2
+    code: int = 3
 
-    def show(self):
+    def show(self) -> bool:
         message = str(self)
         if message:
             print(message, file=sys.stderr)
+        return True
 
     def exit(self):
         self.show()
         sys.exit(self.code)
 
 
 class ParserExit(CommandParserException):
     """Exception used to exit with the given message and status code"""
 
-    def __init__(self, message: str = None, code: int = None):
+    def __init__(self, message: str = None, code: int = 0):
         self.code = code
         self.message = message
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.message or ''
 
 
 # region Developer Errors
 
 
 class CommandDefinitionError(CommandParserException):
@@ -179,42 +180,44 @@
     def __str__(self) -> str:
         return f'argument conflict - the following arguments cannot be combined: {self._usage_msg()}'
 
 
 class ParamsMissing(UsageError):
     """Error raised when one or more required Parameters were not provided"""
 
-    def __init__(self, params: Collection[ParamOrGroup], message: str = None):
+    def __init__(self, params: Collection[ParamOrGroup], message: str = None, partial: bool = False):
         self.params = params
         self.usage_str = ', '.join(param.format_usage(full=True, delim=' / ') for param in params)
+        self.partial = partial
         if message:
             self.message = message
 
     def __str__(self) -> str:
         message = f' ({self.message})' if self.message else ''
         if not message:
             message = '; '.join(p.missing_hint for p in self.params if p.missing_hint)
 
         if len(self.params) > 1:
-            prefix = 'arguments missing - the following arguments are required'
+            mid = '- at least one of' if self.partial else '-'
+            prefix = f'arguments missing {mid} the following arguments are required'
         else:
             prefix = 'argument missing - the following argument is required'
         return f'{prefix}: {self.usage_str}{message}'
 
 
 class BadArgument(ParamUsageError):
     """Error raised when an invalid value is provided for a Parameter"""
 
 
 class InvalidChoice(BadArgument):
     """Error raised when a value that does not match one of the pre-defined choices was provided for a Parameter"""
 
     def __init__(self, param: Optional[Parameter], invalid: Any, choices: Collection[Any]):
         if isinstance(invalid, Collection) and not isinstance(invalid, str):
-            bad_str = 'choices: {}'.format(', '.join(map(repr, invalid)))
+            bad_str = f'choices: {", ".join(map(repr, invalid))}'
         else:
             bad_str = f'choice: {invalid!r}'
         choices_str = ', '.join(map(repr, choices))
         super().__init__(param, f'invalid {bad_str} (choose from: {choices_str})')
 
 
 class MissingArgument(BadArgument):
@@ -237,11 +240,15 @@
 
 
 class UnsupportedAction(CommandParserException):
     """Indicates that an attempted action cannot be completed.  Only used internally."""
 
 
 class Backtrack(CommandParserException):
-    """Raised when backtracking took place"""
+    """Raised when backtracking took place.  Only used internally."""
+
+
+class NextCommand(CommandParserException):
+    """Raised by the parser to advance to the next Command in certain cases.  Only used internally."""
 
 
 # endregion
```

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/formatting/commands.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/formatting/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         self.opt_group.extend(param for param in params if not param.group)
 
     def format_usage(self, delim: str = ' ', sub_cmd_choice: str = None) -> str:
         meta = get_metadata(self.command)
         if meta.usage:
             return meta.usage
 
-        params = self.params.positionals + self.params.options  # noqa
+        params = self.params.all_positionals + self.params.options  # noqa
         pass_thru = self.params.pass_thru
         if pass_thru is not None:
             params.append(pass_thru)
 
         parts = ['usage:', meta.prog]
         if sub_cmd_choice:
             parts.append(sub_cmd_choice)
@@ -151,15 +151,15 @@
 def get_formatter(command: CommandAny) -> CommandHelpFormatter:
     """Get the :class:`CommandHelpFormatter` for the given Command"""
     return get_params(command).formatter
 
 
 def get_usage_sub_cmds(command: CommandCls):
     cmd_mcs: Type[CommandMeta] = command.__class__  # Using metaclass to avoid potentially overwritten attrs
-    parent: CommandType = cmd_mcs.parent(command)
+    parent: CommandType = cmd_mcs.parent(command, False)
     if not parent:
         return []
 
     cmd_chain = get_usage_sub_cmds(parent)
 
     sub_cmd_param: SubCommand = cmd_mcs.params(parent).sub_command
     if not sub_cmd_param:
```

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/formatting/params.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/formatting/params.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,31 +3,28 @@
 
 :author: Doug Skrypa
 """
 # pylint: disable=W0613
 
 from __future__ import annotations
 
+from functools import cached_property
 from typing import TYPE_CHECKING, Type, Callable, Iterator, Iterable, Tuple, Dict
 
-try:
-    from functools import cached_property
-except ImportError:
-    from ..compat import cached_property
-
 from ..config import SubcommandAliasHelpMode
 from ..context import ctx
 from ..core import get_config
 from ..parameters.base import BasePositional, BaseOption
 from ..parameters.choice_map import ChoiceMap, Choice
 from ..parameters import ParamGroup, PassThru, TriFlag
 from .restructured_text import RstTable
 from .utils import format_help_entry, _should_add_default
 
 if TYPE_CHECKING:
+    from ..parameters.option_strings import TriFlagOptionStrings
     from ..typing import Bool, ParamOrGroup, OptStr
 
 BoolFormatterMap = Dict[bool, Callable[[str], str]]
 
 
 class ParamHelpFormatter:
     __slots__ = ('param',)
@@ -161,32 +158,32 @@
             yield from (f'{opt} {metavar}' for opt in opts.option_strs())
 
     def format_usage(self, include_meta: Bool = False, full: Bool = False, delim: str = ', ') -> str:
         if full:
             return delim.join(self.iter_usage_parts())
 
         param: BaseOption = self.param
-        opt = param.option_strs.display_long[0]
+        opt = param.option_strs.get_usage_opt()
         if not include_meta or param.nargs == 0:
             return opt
         return f'{opt} {self._format_usage_metavar()}'
 
     def rst_usage(self) -> str:
         return ', '.join(f'``{part}``' for part in self.iter_usage_parts())
 
 
 class TriFlagHelpFormatter(OptionHelpFormatter, param_cls=TriFlag):
     def format_usage(self, include_meta: Bool = False, full: Bool = False, delim: str = ', ') -> str:
-        opts = self.param.option_strs
+        opts: TriFlagOptionStrings = self.param.option_strs
         if full:
             primary = delim.join(opts.primary_option_strs())
             alts = delim.join(opts.alt_option_strs())
             return f'{primary} | {alts}'
         else:
-            return f'{opts.display_long_primary[0]} | {opts.display_long_alt[0]}'
+            return f'{opts.get_usage_opt(False)} | {opts.get_usage_opt(True)}'
 
     def format_description(self, rst: Bool = False, alt: bool = False) -> str:
         if not alt:
             return super().format_description(rst=rst)
         alt_help = self.param.alt_help
         if alt_help:
             return super().format_description(rst=rst, description=alt_help)
@@ -215,15 +212,15 @@
     def format_metavar(self) -> str:
         param: ChoiceMap = self.param
         if param.choices:
             config = ctx.config
             choices = (str(c) for c in (c.choice for cg in self.choice_groups for c in cg.choices) if c is not None)
             if config.sort_choices:
                 choices = sorted(choices)
-            return '{{{}}}'.format(config.choice_delim.join(choices))
+            return f'{{{config.choice_delim.join(choices)}}}'
         else:
             return param.metavar or param.name.upper()
 
     def format_usage(self, include_meta: Bool = False, full: Bool = False, delim: str = ', ') -> str:
         return self.format_metavar()
 
     def format_help(self, prefix: str = '', tw_offset: int = 0) -> str:
@@ -350,15 +347,15 @@
         first, choice_strs = self.choices[0], self.choice_strs
         try:
             usage, *additional = choice_strs
         except ValueError:  # choice_strs is empty
             return first, first.format_usage(), first.help
 
         if additional:
-            usage = '{{{}}}'.format('|'.join(choice_strs))
+            usage = f'{{{"|".join(choice_strs)}}}'
 
         return first, usage, first.help
 
     def prepare_aliases(self, format_str: str = 'Alias of: {choice}') -> Iterator[Tuple[Choice, OptStr, OptStr]]:
         """
         Prepare this group's Choices for inclusion in help text / documentation using an alternate description for
         aliases.
@@ -401,15 +398,14 @@
 
 class PassThruHelpFormatter(ParamHelpFormatter, param_cls=PassThru):
     required_formatter_map = {True: '-- {}'.format, False: '[-- {}]'.format}
 
 
 class GroupHelpFormatter(ParamHelpFormatter, param_cls=ParamGroup):  # noqa  # pylint: disable=W0223
     required_formatter_map: BoolFormatterMap = {True: '{{{}}}'.format, False: '[{}]'.format}
-    # TODO: #18 Group order changes between invocations - should be sorted as declared or alphanumerically (config?)
 
     def _get_choice_delim(self) -> str:
         param: ParamGroup = self.param
         if param.mutually_dependent:
             return ' + '
         elif param.mutually_exclusive:
             return ' | '
@@ -421,24 +417,24 @@
         members = choice_delim.join(mem.formatter.format_usage(include_meta, full, delim) for mem in self.param.members)
         return self.maybe_wrap_usage(choice_delim.join(members))
 
     def format_description(self, rst: Bool = False, description: str = None) -> str:
         if description:
             return description
         group = self.param
-        if not group.description and not group._name:
-            if ctx.config.show_group_type and (group.mutually_exclusive or group.mutually_dependent):
-                return 'Mutually {} options'.format('exclusive' if group.mutually_exclusive else 'dependent')
-            else:
-                return 'Optional arguments'
-        else:
+        if group.description or group._name:
             description = group.description or f'{group.name} options'
             if ctx.config.show_group_type and (group.mutually_exclusive or group.mutually_dependent):
-                description += ' (mutually {})'.format('exclusive' if group.mutually_exclusive else 'dependent')
+                description += f' (mutually {"exclusive" if group.mutually_exclusive else "dependent"})'
             return description
+        elif ctx.config.show_group_type and (group.mutually_exclusive or group.mutually_dependent):
+            return f'Mutually {"exclusive" if group.mutually_exclusive else "dependent"} options'
+
+        adjective = 'Required' if group.required else 'Other' if group.contains_required else 'Optional'
+        return f'{adjective} arguments'
 
     def _get_spacer(self) -> str:
         group = self.param
         if group.mutually_exclusive:
             return '\u00A6 '  # BROKEN BAR
         elif group.mutually_dependent:
             return '\u2551 '  # BOX DRAWINGS DOUBLE VERTICAL
```

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/formatting/restructured_text.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/formatting/restructured_text.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/formatting/utils.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/formatting/utils.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/inputs/__init__.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/inputs/__init__.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/inputs/base.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/inputs/base.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/inputs/choices.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/inputs/choices.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/inputs/exceptions.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/inputs/exceptions.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/inputs/files.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/inputs/files.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/inputs/numeric.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/inputs/numeric.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,22 @@
 
 
 class NumericInput(InputType[NT], ABC):
     __slots__ = ()
     type: NumType
 
     def is_valid_type(self, value: str) -> bool:
+        """
+        Called during parsing when :meth:`.Parameter.would_accept` is called to determine if the value would be
+        accepted later for processing / conversion when called.
+
+        :param value: The parsed argument to validate
+        :return: True if this input would accept it for processing later (where it may still be rejected), False if
+          it should be rejected before attempting to process / convert / store it.
+        """
         try:
             self.type(value)
         except (ValueError, TypeError):
             return False
         return True
 
     @abstractmethod
```

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/inputs/time.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/inputs/time.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,22 +18,17 @@
 
 from abc import ABC, abstractmethod
 from calendar import day_name, day_abbr, month_name, month_abbr
 from datetime import datetime, date, time, timedelta
 from enum import Enum
 from locale import LC_ALL, setlocale
 from threading import RLock
-from typing import Union, Iterator, Collection, Sequence, Optional, TypeVar, Type, overload
+from typing import Union, Iterator, Collection, Sequence, Optional, TypeVar, Type, Literal, overload
 from typing import Tuple, Dict
 
-try:
-    from typing import Literal
-except ImportError:
-    from ..compat import Literal
-
 from ..typing import T, Bool, Locale, TimeBound
 from ..utils import MissingMixin
 from .base import InputType
 from .exceptions import InputValidationError, InvalidChoiceError
 
 __all__ = ['DTFormatMode', 'Day', 'Month', 'TimeDelta', 'DateTime', 'Date', 'Time']
```

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/inputs/utils.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/inputs/utils.py`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/metadata.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/metadata.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,29 +3,36 @@
 
 :author: Doug Skrypa
 """
 # pylint: disable=R0801
 
 from __future__ import annotations
 
+from collections import defaultdict
+from functools import cached_property
+from importlib.metadata import entry_points, EntryPoint
 from inspect import getmodule
 from pathlib import Path
+from sys import modules
 from textwrap import dedent
 from typing import TYPE_CHECKING, Any, Type, Optional, Union, Tuple, Dict
 from urllib.parse import urlparse
 
 from .context import ctx, NoActiveContext
 
 if TYPE_CHECKING:
     from .typing import Bool, CommandType, OptStr
 
 __all__ = ['ProgramMetadata']
 
 DEFAULT_FILE_NAME: str = 'UNKNOWN'
 
+# TODO: Make it possible to auto-detect author email/url more centrally without needing to import version vars in every
+#  CLI module
+
 
 class Metadata:
     __slots__ = ('default', 'name')
 
     def __init__(self, default):
         self.default = default
 
@@ -57,15 +64,15 @@
     _fields = {'parent'}
     parent: Optional[ProgramMetadata] = None
     path: Path = Metadata(None)
     package: str = Metadata(None)
     module: str = Metadata(None)
     command: str = Metadata(None)
     prog: str = Metadata(None)
-    prog_from_sys_argv: bool = Metadata(None)
+    prog_src: str = Metadata(None)
     url: str = Metadata(None)
     docs_url: str = Metadata(None)
     email: str = Metadata(None)
     version: str = Metadata('')
     usage: str = Metadata(None)
     description: str = Metadata(None)
     epilog: str = Metadata(None)
@@ -107,23 +114,23 @@
         if command.__module__ != 'cli_command_parser.commands':
             # Prevent inheritors from getting docstrings from the base Command
             doc_str = g.get('__doc__')
             doc = command.__doc__
         else:
             doc = doc_str = None
 
-        prog, prog_from_sys_argv = _prog(prog, path, parent, no_sys_argv)
+        prog, prog_src = _prog_finder.normalize(prog, path, parent, no_sys_argv, command)
         return cls(
             parent=parent,
             path=path,
             package=g.get('__package__'),
             module=g.get('__module__'),
             command=command.__qualname__,
             prog=prog,
-            prog_from_sys_argv=prog_from_sys_argv,
+            prog_src=prog_src,
             url=url or g.get('__url__'),
             docs_url=docs_url or _docs_url_from_repo_url(url) or _docs_url_from_repo_url(g.get('__url__')),
             email=email or g.get('__author_email__'),
             version=version or g.get('__version__'),
             usage=usage,
             description=_description(description, doc),
             epilog=epilog,
@@ -160,48 +167,114 @@
         return doc_str
 
 
 def _repr(obj, indent=0) -> str:
     if not isinstance(obj, ProgramMetadata):
         return repr(obj)
 
-    field_dict = {field: getattr(obj, field) for field in obj._fields}
+    field_dict = {field: getattr(obj, field) for field in sorted(obj._fields)}
     prev_str = ' ' * indent
     indent += 4
     indent_str = ' ' * indent
     fields_str = '\n'.join(f'{indent_str}{k}={_repr(v, indent)},' for k, v in field_dict.items())
     return f'<{obj.__class__.__name__}(\n{fields_str}\n{prev_str})>'
 
 
-def _prog(prog: OptStr, cmd_path: Path, parent: Optional[ProgramMetadata], no_sys_argv: Bool) -> Tuple[OptStr, bool]:
-    # TODO: Attempt to detect the name to use via importlib.metadata.entry_points?  3.8+, with return value changes
-    #  after 3.9
-    if prog:
-        return prog, False
-    if no_sys_argv is None:
+class ProgFinder:
+    @cached_property
+    def mod_obj_prog_map(self) -> Dict[str, Dict[str, str]]:
+        mod_obj_prog_map = defaultdict(dict)
+        for entry_point in self._get_console_scripts():
+            module, obj = map(str.strip, entry_point.value.split(':', 1))
+            obj = obj.split('[', 1)[0].strip()  # Strip extras, if any
+            mod_obj_prog_map[module][obj] = entry_point.name
+
+        mod_obj_prog_map.default_factory = None  # Disable automatic defaults
+        return mod_obj_prog_map
+
+    @classmethod
+    def _get_console_scripts(cls) -> Tuple[EntryPoint, ...]:
         try:
-            no_sys_argv = not ctx.allow_argv_prog
-        except NoActiveContext:
-            no_sys_argv = False
+            return entry_points(group='console_scripts')
+        except TypeError:  # Python 3.8 or 3.9
+            return entry_points()['console_scripts']
+
+    def normalize(
+        self,
+        prog: OptStr,
+        cmd_path: Path,
+        parent: Optional[ProgramMetadata],
+        no_sys_argv: Bool,
+        command: CommandType,
+    ) -> Tuple[OptStr, str]:
+        if prog:
+            return prog, 'class kwargs'
+
+        ep_name = self._from_entry_point(command)
+        # TODO: This isn't working for documentation generation...
+        if ep_name:
+            return ep_name, 'entry_points'
+
+        if no_sys_argv is None:
+            try:
+                no_sys_argv = not ctx.allow_argv_prog
+            except NoActiveContext:
+                no_sys_argv = False
+
+        if parent and parent.prog != parent.path.name and (not no_sys_argv or parent.prog_src != 'sys.argv'):
+            return parent.prog, parent.prog_src
+        elif not no_sys_argv:
+            argv_name = self._from_sys_argv()
+            if argv_name:
+                return argv_name, 'sys.argv'
+
+        return cmd_path.name, 'path'
+
+    def _from_entry_point(self, command: CommandType) -> OptStr:
+        main_mod = 'cli_command_parser.commands'
+        for prog, obj, obj_mod, obj_name in self._iter_entry_point_candidates(command):
+            if obj is command or (obj_mod == main_mod and obj_name == 'main'):
+                return prog
+
+        return None
 
-    if parent and parent.prog != parent.path.name and (not no_sys_argv or not parent.prog_from_sys_argv):
-        return parent.prog, parent.prog_from_sys_argv
-    elif not no_sys_argv:
+    def _iter_entry_point_candidates(self, command: CommandType):
+        try:
+            # TODO: This likely won't work for a base command in one module, sub commands defined in separate modules,
+            #  and main imported from cli_command_parser in the package's __init__/__main__ module...
+            obj_prog_map = self.mod_obj_prog_map[command.__module__]
+            module = modules[command.__module__]
+        except KeyError as e:
+            pass
+        else:
+            for obj_name, prog in obj_prog_map.items():
+                base_name = obj_name.split('.', 1)[0]
+                try:
+                    obj = getattr(module, base_name)
+                except AttributeError:
+                    pass
+                else:
+                    yield prog, obj, getattr(obj, '__module__', ''), getattr(obj, '__name__', '')
+
+    def _from_sys_argv(self) -> OptStr:
         try:
             ctx_prog = ctx.prog
         except NoActiveContext:
-            ctx_prog = None
+            return None
 
         if ctx_prog:
             path = Path(ctx_prog)
             # Windows allows invocation without .exe - assume a file with an extension is a match
             if path.exists() or next(path.parent.glob(f'{path.name}.???'), None) is not None:
-                return path.name, True
+                return path.name
+
+        return None
+
 
-    return cmd_path.name, False
+_prog_finder = ProgFinder()
 
 
 def _path_and_globals(command: CommandType, path: Path = None) -> Tuple[Path, Dict[str, Any]]:
     module = getmodule(command)
     if path is None:
         try:
             path = Path(module.__file__).resolve()
```

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/nargs.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/nargs.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,33 +2,37 @@
 Helpers for handling ``nargs=...`` for Parameters.
 
 :author: Doug Skrypa
 """
 
 from __future__ import annotations
 
-from typing import Union, Optional, Sequence, Collection, Tuple, Set, FrozenSet
+from typing import Union, Optional, Sequence, Collection, Iterable, Tuple, Set, FrozenSet
 
-NargsValue = Union[str, int, Tuple[int, Optional[int]], Sequence[int], Set[int], FrozenSet[int], range]
+__all__ = ['Nargs', 'NargsValue', 'REMAINDER', 'nargs_max_sum', 'nargs_min_sum']
 
-NARGS_STR_RANGES = {'?': (0, 1), '*': (0, None), '+': (1, None)}
+REMAINDER = type('REMAINDER', (), {})()
+_UNBOUND = (None, REMAINDER)
+NARGS_STR_RANGES = {'?': (0, 1), '*': (0, None), '+': (1, None), 'REMAINDER': (0, REMAINDER)}
 SET_ERROR_FMT = 'Invalid nargs={!r} set - expected non-empty set where all values are integers >= 0'
 SEQ_ERROR_FMT = 'Invalid nargs={!r} sequence - expected 2 ints where 0 <= a <= b or b is None'
 
+NargsValue = Union[str, int, Tuple[int, Optional[int]], Sequence[int], Set[int], FrozenSet[int], range, type(REMAINDER)]
+
 
 class Nargs:
     """
     Helper class for validating the number of values provided for a given :class:`.Parameter`.  Unifies the
     handling of different ways of specifying the required number of values.
 
     Acceptable values include ``?``, ``*``, and ``+``, and they have the same meaning that they have in argparse.
     Additionally, integers, a range of integers, or a set/tuple of integers are accepted for more specific requirements.
     """
 
-    __slots__ = ('_orig', 'range', 'min', 'max', 'allowed', 'variable')
+    __slots__ = ('_orig', 'range', 'min', 'max', 'allowed', 'variable', '_has_upper_bound')
     _orig: NargsValue
     range: Optional[range]
     min: Optional[int]
     max: Optional[int]
     allowed: Collection[int]
     variable: bool
 
@@ -66,32 +70,35 @@
             self.max = max(nargs)
         elif isinstance(nargs, Sequence):
             try:
                 self.min, self.max = self.allowed = a, b = nargs
             except (ValueError, TypeError) as e:
                 raise e.__class__(SEQ_ERROR_FMT.format(nargs)) from e
 
-            if not (isinstance(a, int) and (b is None or isinstance(b, int))):
+            if not (isinstance(a, int) and (b in _UNBOUND or isinstance(b, int))):
                 raise TypeError(SEQ_ERROR_FMT.format(nargs))
-            elif 0 > a or (b is not None and a > b):
+            elif 0 > a or (b not in _UNBOUND and a > b):
                 raise ValueError(SEQ_ERROR_FMT.format(nargs))
+        elif nargs is REMAINDER:
+            self.min, self.max = self.allowed = (0, REMAINDER)
         else:
             raise TypeError(f'Unexpected type={nargs.__class__.__name__} for nargs={nargs!r}')
 
         self.variable = self.min != self.max
+        self._has_upper_bound = self.max not in _UNBOUND
 
     def __repr__(self) -> str:
         return f'{self.__class__.__name__}({self._orig!r})'
 
     def __str__(self) -> str:
         rng = self.range
         if rng is not None:
             return f'{rng.start} ~ {rng.stop}' if rng.step == 1 else f'{rng.start} ~ {rng.stop} (step={rng.step})'
-        elif self.max is None:
-            return f'{self.min} or more'
+        elif not self._has_upper_bound:
+            return f'{self.min} or more' if self.max is None else self.max.__class__.__name__
         elif self.min == self.max:
             return str(self.min)
         elif isinstance(self.allowed, frozenset):
             return '{{{}}}'.format(','.join(map(str, sorted(self.allowed))))  # pylint: disable=C0209
         else:
             return f'{self.min} ~ {self.max}'
 
@@ -104,17 +111,17 @@
             return self._eq_nargs(other)
         elif isinstance(other, int):
             return self.min == self.max == other
         else:
             return NotImplemented
 
     def _eq_nargs(self, other: Nargs) -> bool:
-        if self.max is None:
-            return other.max is None and self.min == other.min
-        elif other.max is None:
+        if not self._has_upper_bound:
+            return other.max is self.max and self.min == other.min
+        elif not other._has_upper_bound:
             return False
         elif isinstance(other._orig, type(self._orig)):
             return self.allowed == other.allowed
 
         # After this point, the allowed / range attribute types cannot match because the originals did not match
         if isinstance(self.allowed, frozenset):
             return self._compare_allowed_set(other)
@@ -144,11 +151,27 @@
         Returns True if the minimum number of values have been provided to satisfy the requirements, and if the number
         of values has not exceeded the maximum allowed.  Returns False if the count is below the minimum or above the
         maximum.
 
         For more advanced use cases, such as range or a set of counts, the count must also match one of the specific
         numbers provided for this to return True.
         """
-        if self.max is None:
-            return count >= self.min
-        else:
+        if self._has_upper_bound:
             return count in self.allowed
+        else:
+            return count >= self.min
+
+    @property
+    def has_upper_bound(self) -> bool:
+        return self._has_upper_bound
+
+    @property
+    def upper_bound(self) -> Union[int, float]:
+        return self.max if self._has_upper_bound else float('inf')
+
+
+def nargs_max_sum(nargs_objects: Iterable[Nargs]) -> Union[int, float]:
+    return sum(obj.upper_bound for obj in nargs_objects)
+
+
+def nargs_min_sum(nargs_objects: Iterable[Nargs]) -> int:
+    return sum(obj.min for obj in nargs_objects)
```

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/parameters/base.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/parameters/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,45 +6,41 @@
 # pylint: disable=R0801
 
 from __future__ import annotations
 
 import re
 from abc import ABC, abstractmethod
 from contextvars import ContextVar
-from functools import partial, update_wrapper
+from functools import partial, update_wrapper, cached_property
 from itertools import chain
-from typing import TYPE_CHECKING, Any, Type, Generic, Optional, Callable, Collection, Union, overload
-from typing import List, FrozenSet
-
-try:
-    from functools import cached_property  # pylint: disable=C0412
-except ImportError:
-    from ..compat import cached_property
+from typing import TYPE_CHECKING, Any, Type, Generic, Optional, Callable, Collection, Union, Iterator, overload
+from typing import List, Tuple, FrozenSet
 
 from ..annotations import get_descriptor_value_type
-from ..config import CommandConfig, OptionNameMode
-from ..context import Context, ctx, get_current_context, ParseState
+from ..config import CommandConfig, OptionNameMode, AllowLeadingDash
+from ..context import Context, ctx, get_current_context
 from ..exceptions import ParameterDefinitionError, BadArgument, MissingArgument, InvalidChoice
 from ..exceptions import ParamUsageError, NoActiveContext, UnsupportedAction
 from ..inputs import InputType, normalize_input_type
 from ..inputs.choices import _ChoicesBase, Choices, ChoiceMap as ChoiceMapInput
 from ..inputs.exceptions import InputValidationError, InvalidChoiceError
-from ..nargs import Nargs
-from ..typing import Bool, CommandCls, CommandObj, CommandAny, Param, T_co
-from ..utils import _NotSet
+from ..nargs import Nargs, REMAINDER
+from ..typing import Bool, ValSrc, OptStrs, CommandCls, CommandObj, CommandAny, Param, LeadingDash, T_co
+from ..utils import _NotSet, ValueSource
 from .option_strings import OptionStrings
 
 if TYPE_CHECKING:
     from types import MethodType
     from ..formatting.params import ParamHelpFormatter
     from .groups import ParamGroup
 
 __all__ = ['Parameter', 'BasePositional', 'BaseOption']
 
 _group_stack = ContextVar('cli_command_parser.parameters.base.group_stack', default=[])
+_is_numeric = re.compile(r'^-\d+$|^-\d*\.\d+?$').match
 
 
 class parameter_action:  # pylint: disable=C0103
     """
     Decorator that is used to register :paramref:`Parameter.__init__.action` handler methods to store values that are
     provided for that type of :class:`Parameter`.  The name of the decorated method is used as the ``action`` name.
 
@@ -61,19 +57,20 @@
         with the original method.
 
         Since `__set_name__` is called on descriptors before their containing class's parent's `__init_subclass__` is
         called, name action/method name conflicts are handled by imitating a name mangled dunder attribute that will be
         unique to each subclass.  The mangled name is replaced with the friendlier `_actions` in
         :meth:`Parameter.__init_subclass__`.
         """
+        attr = f'_{parameter_cls.__name__}__actions'
         try:
-            actions = getattr(parameter_cls, f'_{parameter_cls.__name__}__actions')
+            actions = getattr(parameter_cls, attr)
         except AttributeError:
             actions = set()
-            setattr(parameter_cls, f'_{parameter_cls.__name__}__actions', actions)
+            setattr(parameter_cls, attr, actions)
 
         actions.add(name)
 
     def __call__(self, *args, **kwargs) -> int:
         result = self.method(*args, **kwargs)
         return 1 if result is None else result
 
@@ -208,23 +205,23 @@
       never include the default value in usage / help messages.  Default: follow the ``show_defaults`` setting.
     """
 
     # region Attributes & Initialization
 
     # Class attributes
     _actions: FrozenSet[str] = frozenset()          #: The actions supported by this Parameter
-    _positional: bool = False                       #: Whether this Parameter is positional or not
     _repr_attrs: Optional[Collection[str]] = None   #: Attributes to include in ``repr()`` output
     accepts_none: bool = False                      #: Whether this Parameter can be provided without a value
     accepts_values: bool = True                     #: Whether this Parameter can be provided with at least 1 value
     # Instance attributes with class defaults
     metavar: str = None
     nargs: Nargs = Nargs(1)                         # Set in subclasses
     type: Optional[Callable[[str], T_co]] = None    # Only set here if not set by __init__ in Option/Positional
     show_default: bool = None
+    allow_leading_dash: AllowLeadingDash = AllowLeadingDash.NUMERIC  # Set in some subclasses
 
     def __init_subclass__(
         cls, accepts_values: bool = None, accepts_none: bool = None, repr_attrs: Collection[str] = None, **kwargs
     ):
         """
         :param accepts_values: Indicates whether a given subclass of Parameter accepts values, or not.  :class:`.Flag`
           is an example of a class that does not accept values.
@@ -272,23 +269,28 @@
         super().__init__(name=name, required=required, help=help, hide=hide)
         self.action = action
         self.default = None if default is _NotSet and not required and self.nargs.max == 1 else default
         self.metavar = metavar
         if show_default is not None:
             self.show_default = show_default
 
-    def _init_value_factory(self, state: ParseState):
+    def _init_value_factory(self):
         return _NotSet
 
     def __set_name__(self, command: CommandCls, name: str):
         super().__set_name__(command, name)
         type_attr = self.type
         choices = isinstance(type_attr, (ChoiceMapInput, Choices)) and type_attr.type is None
-        if not (choices or type_attr is None) or not self._config(command).allow_annotation_type:
+        if (
+            not (choices or type_attr is None)
+            or not self._config(command).allow_annotation_type
+            or self.nargs.max is REMAINDER
+        ):
             return
+
         annotated_type = get_descriptor_value_type(command, name)
         if annotated_type is None:
             return
         elif choices:
             type_attr.type = annotated_type
         else:  # self.type must be None
             # Choices present earlier would have already been converted
@@ -329,51 +331,42 @@
             value = self.result()
 
         name = self._name
         if name is not None:
             command.__dict__[name] = value  # Skip __get__ on subsequent accesses
         return value
 
-    def _nargs_max_reached(self) -> bool:
+    def _get_parsed_and_max_reached(self) -> Tuple[List[T_co], bool]:
+        parsed = ctx.get_parsed_value(self)
         try:
-            return len(ctx.get_parsed_value(self)) >= self.nargs.max
-        except TypeError:
-            return False
+            nargs_max_reached = len(parsed) >= self.nargs.max
+        except TypeError:  # None or REMAINDER
+            nargs_max_reached = False
+        return parsed, nargs_max_reached
 
-    def take_action(  # pylint: disable=W0613
-        self, value: Optional[str], short_combo: bool = False, opt_str: str = None
+    def take_action(
+        self, value: Optional[str], short_combo: bool = False, opt_str: str = None, src: ValSrc = ValueSource.CLI
     ):
-        action = self.action
-        if action == 'append' and self._nargs_max_reached():
-            val_count = len(ctx.get_parsed_value(self))
-            raise ParamUsageError(
-                self, f'cannot accept any additional args with nargs={self.nargs}: val_count={val_count!r}'
-            )
-        elif action == 'store':
-            val = ctx.get_parsed_value(self)
-            if val is not _NotSet:
-                raise ParamUsageError(self, f'received value={value!r} but a stored value={val!r} already exists')
-
         ctx.record_action(self)
-        action_method = getattr(self, action)
-        return action_method(self.prepare_and_validate(value, short_combo))
+        return getattr(self, self.action)(self.prepare_and_validate(value, short_combo))
 
     def would_accept(self, value: str, short_combo: bool = False) -> bool:
         action = self.action
         if action in {'store', 'store_all'} and ctx.get_parsed_value(self) is not _NotSet:
             return False
-        elif action == 'append' and self._nargs_max_reached():
+        elif action == 'append' and self._get_parsed_and_max_reached()[1]:
             return False
         try:
             normalized = self.prepare_value(value, short_combo, True)
         except BadArgument:
             return False
         return self.is_valid_arg(normalized)
 
     def prepare_and_validate(self, value: str, short_combo: bool = False) -> T_co:
+        """Called by :meth:`.take_action` to prepare/validate the value before it is passed to the action method."""
         if value is not None:
             value = self.prepare_value(value, short_combo)
         self.validate(value)
         return value
 
     def prepare_value(  # pylint: disable=W0613
         self, value: str, short_combo: bool = False, pre_action: bool = False
@@ -390,15 +383,18 @@
         except (TypeError, ValueError) as e:
             raise BadArgument(self, f'bad value={value!r} for type={type_func!r}: {e}') from e
         except Exception as e:
             raise BadArgument(self, f'unable to cast value={value!r} to type={type_func!r}') from e
 
     def validate(self, value: Optional[T_co]):
         if isinstance(value, str) and value.startswith('-'):
-            if len(value) > 1 and not _is_numeric(value):
+            if self.allow_leading_dash == AllowLeadingDash.NUMERIC:
+                if len(value) > 1 and not _is_numeric(value):
+                    raise BadArgument(self, f'invalid value={value!r}')
+            elif self.allow_leading_dash == AllowLeadingDash.NEVER:
                 raise BadArgument(self, f'invalid value={value!r}')
         elif value is None:
             if not self.accepts_none:
                 raise MissingArgument(self)
         elif not self.accepts_values:
             raise BadArgument(self, f'does not accept values, but value={value!r} was provided')
 
@@ -474,27 +470,36 @@
 
     # endregion
 
 
 class BasicActionMixin:
     action: str
     nargs: Nargs
+    type: Optional[Callable]
 
-    def _init_value_factory(self, state: ParseState):
+    def _init_value_factory(self):
         if self.action == 'append':
             return []
-        return super()._init_value_factory(state)  # noqa
+        return super()._init_value_factory()  # noqa
 
     @parameter_action
     def store(self: Parameter, value: T_co):
+        prev = ctx.get_parsed_value(self)
+        if prev is not _NotSet:
+            raise ParamUsageError(self, f'can only be specified once - found multiple values: {prev!r}, {value!r}')
         ctx.set_parsed_value(self, value)
 
     @parameter_action
     def append(self: Parameter, value: T_co):
-        ctx.get_parsed_value(self).append(value)
+        parsed, nargs_max_reached = self._get_parsed_and_max_reached()
+        if nargs_max_reached:
+            raise ParamUsageError(
+                self, f'cannot accept any additional args with nargs={self.nargs} - already found {len(parsed)} values'
+            )
+        parsed.append(value)
 
     def _pre_pop_values(self: Parameter):
         if self.action != 'append' or not self.nargs.variable or self.type not in (None, str):
             return []
 
         return ctx.get_parsed_value(self)
 
@@ -510,27 +515,44 @@
         if self.action != 'append' or self.type not in (None, str):
             raise UnsupportedAction
 
         values = ctx.get_parsed_value(self)
         if not values:
             return values
 
-        ctx.set_parsed_value(self, self._init_value_factory(ctx.state))
+        ctx.set_parsed_value(self, self._init_value_factory())
         ctx._provided[self] = 0
         return values
 
     def pop_last(self: Union[Parameter, BasicActionMixin], count: int = 1) -> List[str]:
         values = self._pre_pop_values()
         if not values or count >= len(values) or not self.nargs.satisfied(len(values) - count):
             raise UnsupportedAction
 
         ctx.set_parsed_value(self, values[:-count])
         ctx.record_action(self, -count)
         return values[-count:]
 
+    def _validate_nargs_and_allow_leading_dash(self, allow_leading_dash: LeadingDash):
+        if allow_leading_dash is not None:
+            allow_leading_dash = AllowLeadingDash(allow_leading_dash)
+
+        if self.nargs.max is REMAINDER:
+            if self.type is not None:
+                raise ParameterDefinitionError(f'Type casting and choices are not supported with nargs={self.nargs!r}')
+            elif allow_leading_dash not in (None, AllowLeadingDash.ALWAYS):
+                raise ParameterDefinitionError(
+                    f'With nargs={self.nargs!r}, only allow_leading_dash=AllowLeadingDash.ALWAYS is supported - found:'
+                    f' {allow_leading_dash!r}'
+                )
+            allow_leading_dash = AllowLeadingDash.ALWAYS
+
+        if allow_leading_dash is not None:
+            self.allow_leading_dash = allow_leading_dash
+
 
 class BasePositional(Parameter[T_co], ABC):
     """
     Base class for :class:`.Positional`, :class:`.SubCommand`, :class:`.Action`, and any other parameters that are
     provided positionally, without prefixes.  It is not meant to be used directly.
 
     All positional parameters are required by default.
@@ -539,15 +561,14 @@
     parser.
 
     :param action: The action to take on individual parsed values.  Actions must be defined as methods in classes
       that extend Parameter, and must be registered via :class:`parameter_action`.
     :param kwargs: Additional keyword arguments to pass to :class:`Parameter`.
     """
 
-    _positional: bool = True
     _default_ok: bool = False
 
     def __init_subclass__(cls, default_ok: bool = None, **kwargs):  # pylint: disable=W0222
         """
         :param default_ok: Whether default values are supported for this Parameter type
         :param kwargs: Additional keyword arguments to pass to :meth:`.Parameter.__init_subclass__`.
         """
@@ -580,45 +601,60 @@
 
     :param option_strs: The long and/or short option prefixes for this option.  If no long prefixes are specified,
       then one will automatically be added based on the name assigned to this parameter.
     :param action: The action to take on individual parsed values.  Actions must be defined as methods in classes
       that extend Parameter, and must be registered via :class:`parameter_action`.
     :param name_mode: Override the configured :ref:`configuration:Parsing Options:option_name_mode` for this
       Option/Flag/Counter/etc.
+    :param env_var: A string or sequence (tuple, list, etc) of strings representing environment variables that should
+      be searched for a value when no value was provided via CLI.  If a value was provided via CLI, then these variables
+      will not be checked.  If multiple env variable names/keys were provided, then they will be checked in the order
+      that they were provided.  When enabled, values from env variables take precedence over the default value.  When
+      enabled and the Parameter is required, then either a CLI value or an env var value must be provided.
     :param kwargs: Additional keyword arguments to pass to :class:`Parameter`.
     """
 
     _opt_str_cls: Type[OptionStrings] = OptionStrings
     option_strs: OptionStrings
+    env_var: OptStrs = None
 
-    def __init__(self, *option_strs: str, action: str, name_mode: Union[OptionNameMode, str] = None, **kwargs):
+    def __init__(
+        self,
+        *option_strs: str,
+        action: str,
+        name_mode: Union[OptionNameMode, str, None] = _NotSet,
+        env_var: OptStrs = None,
+        **kwargs,
+    ):
         _validate_opt_strs(option_strs)
         super().__init__(action, **kwargs)
         self.option_strs = self._opt_str_cls(option_strs, name_mode)
+        if env_var:
+            self.env_var = env_var
 
     def __set_name__(self, command: CommandCls, name: str):
         super().__set_name__(command, name)
         if not self.option_strs.name_mode:
             self.option_strs.name_mode = command.__class__.config(command).option_name_mode
         self.option_strs.update(name)
 
+    def env_vars(self) -> Iterator[str]:
+        env_var = self.env_var
+        if env_var:
+            if isinstance(env_var, str):
+                yield env_var
+            else:
+                yield from env_var
+
 
 def get_active_param_group() -> Optional[ParamGroup]:
     try:
         return _group_stack.get()[-1]
     except (AttributeError, IndexError):
         return None
 
 
 def _validate_opt_strs(opt_strs: Collection[str]):
     bad = ', '.join(opt for opt in opt_strs if not 0 < opt.count('-', 0, 3) < 3 or opt.endswith('-') or '=' in opt)
     if bad:
         msg = f"Bad option(s) - they must start with '--' or '-', may not end with '-', and may not contain '=': {bad}"
         raise ParameterDefinitionError(msg)
-
-
-def _is_numeric(text: str) -> Bool:
-    try:
-        num_match = _is_numeric._num_match
-    except AttributeError:
-        _is_numeric._num_match = num_match = re.compile(r'^-\d+$|^-\d*\.\d+?$').match
-    return num_match(text)
```

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/parameters/choice_map.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/parameters/choice_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 :author: Doug Skrypa
 """
 
 from __future__ import annotations
 
 from functools import partial
 from string import whitespace, printable
-from typing import Type, TypeVar, Generic, Optional, Callable, Union, Collection, Mapping, Dict
+from typing import Type, TypeVar, Generic, Optional, Callable, Union, Collection, Mapping, NoReturn, Dict
 from types import MethodType
 
-from ..context import ctx, ParseState
+from ..context import ctx
 from ..exceptions import ParameterDefinitionError, BadArgument, MissingArgument, InvalidChoice, CommandDefinitionError
 from ..formatting.utils import format_help_entry
 from ..nargs import Nargs
 from ..typing import Bool, CommandCls
 from ..utils import _NotSet, camel_to_snake_case, short_repr
 from .base import BasePositional, parameter_action
 
@@ -96,15 +96,15 @@
 
     def __init__(self, *, action: str = 'append', title: str = None, description: str = None, **kwargs):
         super().__init__(action=action, **kwargs)
         self.title = title
         self.description = description
         self.choices = {}
 
-    def _init_value_factory(self, state: ParseState):
+    def _init_value_factory(self):
         return []
 
     # region Choice Registration
 
     @property
     def has_choices(self) -> bool:
         return bool(self.choices)
@@ -114,30 +114,44 @@
             lengths = set(map(len, map(str.split, self.choices)))
         except TypeError:
             lengths = set(map(len, map(str.split, filter(None, self.choices))))
             lengths.add(0)
 
         self.nargs = Nargs(lengths)
 
+    @classmethod
+    def _validate_positional(cls, value: str, prefix: str = 'choice'):
+        if not value or value.startswith('-'):
+            raise cls._choice_validation_exc(
+                f"Invalid {cls.__name__} {prefix}={value!r} - may not be empty or start with '-'"
+            )
+
+        bad = {c for c in value if (c in whitespace and c != ' ') or c not in printable}
+        if bad:
+            raise cls._choice_validation_exc(f'Invalid {cls.__name__} {prefix}={value!r} - invalid characters: {bad}')
+
     def register_choice(self, choice: str, target: T = _NotSet, help: str = None):  # noqa
-        _validate_positional(self.__class__.__name__, choice, exc=self._choice_validation_exc)
+        self._validate_positional(choice)
         self._register_choice(choice, target, help)
 
     def _register_choice(
         self, choice: OptStr, target: Optional[T] = _NotSet, help: str = None, local: bool = False  # noqa
     ):
         try:
             existing = self.choices[choice]
         except KeyError:
             self.choices[choice] = Choice(choice, target, help, local)
             self._update_nargs()
         else:
             prefix = 'Invalid default' if choice is None else f'Invalid choice={choice!r} for'
             raise CommandDefinitionError(f'{prefix} target={target!r} - already assigned to {existing}')
 
+    def _no_choices_error(self) -> NoReturn:
+        raise CommandDefinitionError(f'No choices were registered for {self}')
+
     # endregion
 
     # region Argument Handling
 
     @parameter_action
     def append(self, value: str):
         values = value.split()
@@ -146,42 +160,43 @@
 
         ctx.get_parsed_value(self).extend(values)
         n_values = len(values)
         ctx.record_action(self, n_values - 1)  # - 1 because it was already called before dispatching to this method
         return n_values
 
     def validate(self, value: str):
-        values = ctx.get_parsed_value(self).copy()
-        values.append(value)
         choices = self.choices
-        if choices:
-            choice = ' '.join(values)
-            if choice in choices:
-                return
-            elif len(values) > self.nargs.max:
-                raise BadArgument(self, 'too many values')
-            prefix = choice + ' '
-            if not any(c.startswith(prefix) for c in choices if c):
-                raise InvalidChoice(self, prefix[:-1], choices)
-        elif value.startswith('-'):
-            raise BadArgument(self, f'invalid value={value!r}')
+        if not choices:
+            self._no_choices_error()
+
+        values = (*ctx.get_parsed_value(self), value)
+        choice = ' '.join(values)
+        if choice in choices:
+            return
+        elif len(values) > self.nargs.max:
+            raise BadArgument(self, 'too many values')
+        prefix = choice + ' '
+        if not any(c.startswith(prefix) for c in choices if c):
+            raise InvalidChoice(self, prefix[:-1], choices)
 
     def result_value(self) -> OptStr:
         choices = self.choices
         if not choices:
-            raise CommandDefinitionError(f'No choices were registered for {self}')
+            self._no_choices_error()
 
         values = ctx.get_parsed_value(self)
         if not values:
             if None in choices:
                 return None
             raise MissingArgument(self)
+
         val_count = len(values)
         if val_count not in self.nargs:
             raise BadArgument(self, f'expected nargs={self.nargs} values but found {val_count}')
+
         choice = ' '.join(values)
         if choice not in choices:
             raise InvalidChoice(self, choice, choices)
         return choice
 
     result = result_value
 
@@ -233,28 +248,32 @@
         self.required = required
         if not required:
             # This results in next_cmd=None in parse_args, so the base cmd will run
             self._register_choice(None, None, default_help)
         if local_choices:
             self._register_local_choices(local_choices)
 
+    @property
+    def has_local_choices(self) -> bool:
+        return None in self.choices or any(c.target is None for c in self.choices.values())
+
     def _register_local_choices(self, local_choices: Union[Mapping[str, str], Collection[str]]):
         try:
             choice_help_iter = local_choices.items()
         except AttributeError:
             choice_help_iter = ((choice, None) for choice in local_choices)
 
         for choice, help_text in choice_help_iter:
             self._register_choice(choice, None, help_text, True)
 
     def register_command(self, choice: OptStr, command: CommandCls, help: OptStr) -> CommandCls:  # noqa
         if choice is None:
             choice = camel_to_snake_case(command.__name__)
         else:
-            _validate_positional(self.__class__.__name__, choice, exc=self._choice_validation_exc)
+            self._validate_positional(choice)
 
         try:
             self.register_choice(choice, command, help)
         except CommandDefinitionError:
             from ..core import get_parent
 
             parent = get_parent(command)
@@ -289,14 +308,17 @@
                 raise CommandDefinitionError(
                     f'Cannot combine a positional command_or_choice={command_or_choice!r} choice with choice={choice!r}'
                 )
             return partial(self.register_command, command_or_choice, help=help)
         else:
             return self.register_command(choice, command_or_choice, help=help)  # noqa
 
+    def _no_choices_error(self) -> NoReturn:
+        raise CommandDefinitionError(f'{ctx.command}.{self.name} = {self} has no sub Commands')
+
 
 class Action(ChoiceMap[MethodType], title='Actions'):
     """
     Actions are similar to :class:`.SubCommand` parameters, but allow methods in :class:`.Command` classes to
     be registered as a callable to be executed based on a user's choice instead of separate sub Commands.
 
     Actions are better suited for use cases where all of the target functions accept the same arguments.  If target
@@ -363,18 +385,7 @@
 
         if method_or_choice is None:
             return partial(self.register_action, choice, help=help, default=default)
         else:
             return self.register_action(choice, method_or_choice, help=help, default=default)
 
     __call__ = register
-
-
-def _validate_positional(
-    param_cls: str, value: str, prefix: str = 'choice', exc: Type[Exception] = ParameterDefinitionError
-):
-    if not value or value.startswith('-'):
-        raise exc(f"Invalid {param_cls} {prefix}={value!r} - may not be empty or start with '-'")
-
-    bad = {c for c in value if (c in whitespace and c != ' ') or c not in printable}
-    if bad:
-        raise exc(f'Invalid {param_cls} {prefix}={value!r} - invalid characters: {bad}')
```

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/parameters/groups.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/parameters/groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,29 +223,43 @@
         that nested groups are validated before any group that they are a member of.
         """
         provided, missing = self._categorize_params()
         ctx.record_action(self, len(provided))
         self._check_conflicts(provided, missing)
         if not missing:
             return
-        elif not provided and (self.required or (self.mutually_dependent and any(p.required for p in self.members))):
-            raise ParamsMissing(missing)
+        req_any, req_all = self._classify_required()
+        if not provided and req_any:
+            raise ParamsMissing(missing, partial=not req_all)
         elif provided or not self.in_mutually_exclusive_group:
             req_missing = [p for p in missing if p.required]
             if req_missing:
                 raise ParamsMissing(req_missing)
 
+    def _classify_required(self) -> Tuple[bool, bool]:
+        """Returns a tuple of (req_any, req_all)"""
+        if self.mutually_dependent and (self.required or any(p.required for p in self.members)):
+            return True, True
+        elif self.required:
+            return True, False
+        else:
+            return False, False
+
     # endregion
 
     # region Usage / Help Text
 
     @property
     def contains_positional(self) -> bool:
         # Used by the help text formatter when grouping parameters / groups
-        return any(isinstance(p, BasePositional) for p in self)
+        return any(isinstance(p, BasePositional) for p in self.members)
+
+    @property
+    def contains_required(self) -> bool:
+        return any(p.required for p in self.members)
 
     @property
     def show_in_help(self) -> bool:
         if self.hide or not self.members:
             return False
         elif self.group is not None:
             return self.group.show_in_help
```

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/parameters/option_strings.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/parameters/option_strings.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Optional, Collection, Union, Iterator, List, Set, Tuple
 
 from ..config import OptionNameMode, DEFAULT_CONFIG
 from ..exceptions import ParameterDefinitionError
+from ..utils import _NotSet
 
 if TYPE_CHECKING:
     from ..typing import Bool
 
 __all__ = ['OptionStrings', 'TriFlagOptionStrings']
 
 
@@ -21,68 +22,71 @@
     __slots__ = ('name_mode', '_long', '_short', 'combinable', '_display_long')
     name_mode: Optional[OptionNameMode]
     combinable: Set[str]
     _display_long: Set[str]
     _long: Set[str]
     _short: Set[str]
 
-    def __init__(self, option_strs: Collection[str], name_mode: Union[OptionNameMode, str] = None):
-        self.name_mode = OptionNameMode(name_mode) if name_mode is not None else None
+    def __init__(self, option_strs: Collection[str], name_mode: Union[OptionNameMode, str, None] = _NotSet):
+        self.name_mode = OptionNameMode(name_mode) if name_mode is not _NotSet else None
         self._display_long = self._long = {opt for opt in option_strs if opt.startswith('--')}
         self._short = short_opts = {opt for opt in option_strs if 1 == opt.count('-', 0, 2)}
         self.combinable = {opt[1:] for opt in short_opts if len(opt) == 2}
         bad_opts = ', '.join(opt for opt in short_opts if '-' in opt[1:])
         if bad_opts:
             raise ParameterDefinitionError(f"Bad short option(s) - may not contain '-': {bad_opts}")
 
     def __repr__(self) -> str:
         options = ', '.join(self.all_option_strs())
         return f'<{self.__class__.__name__}[name_mode={self.name_mode}][{options}]>'
 
-    @classmethod
-    def _sort_options(cls, options: Collection[str]):
-        return sorted(options, key=lambda opt: (-len(opt), opt))
-
     def has_long(self) -> Bool:
         """Whether any (primary / non-alternate, for TriFlag) long option strings were defined"""
         return self._long  # Explicit values were provided during param init
 
+    def has_min_opts(self) -> Bool:
+        """Returns a truthy value if the minimum required number of option strings have been registered"""
+        return self._long or self._short
+
     def update(self, name: str):
         """
         Called by :meth:`.BaseOption.__set_name__` to add the assigned name to the long option strings for this param.
         """
         if self.has_long():
             return
 
         mode = self.name_mode or DEFAULT_CONFIG.option_name_mode
         mode_val: int = mode._value_  # noqa # This Flag doesn't subclass int due to breakage in 3.11
         if mode_val & 4:  # any option was set
             self._display_long = self._display_long.copy()
         if mode & OptionNameMode.DASH:
-            option = '--{}'.format(name.replace('_', '-'))
+            option = f'--{name.replace("_", "-")}'
             self._long.add(option)
             if mode_val & 16:  # OptionNameMode.BOTH_DASH = OptionNameMode.DASH | 4 | 16
                 self._display_long.add(option)
         if mode & OptionNameMode.UNDERSCORE:
             option = f'--{name}'
             self._long.add(option)
             if mode_val & 8:  # OptionNameMode.BOTH_UNDERSCORE = OptionNameMode.DASH | 4 | 8
                 self._display_long.add(option)
 
     @property
     def long(self) -> List[str]:
-        return self._sort_options(self._long)
+        return _sort_options(self._long)
 
     @property
     def short(self) -> List[str]:
-        return self._sort_options(self._short)
+        return _sort_options(self._short)
 
     @property
     def display_long(self) -> List[str]:
-        return self._sort_options(self._display_long)
+        return _sort_options(self._display_long)
+
+    def get_usage_opt(self) -> str:
+        return next(self.option_strs())
 
     def option_strs(self) -> Iterator[str]:
         yield from self.display_long
         yield from self.short
 
     all_option_strs = option_strs
 
@@ -93,14 +97,17 @@
     _alt_short: Optional[str]
     _alt_long: Union[Set[str], Tuple[str]]
 
     def has_long(self) -> Bool:
         """Whether any primary / non-alternate long option strings were defined"""
         return self._long.difference(self._alt_long)
 
+    def has_min_opts(self) -> Bool:
+        return next(self.option_strs(False), None) and next(self.option_strs(True), None)
+
     def add_alts(self, prefix: Optional[str], long: Optional[str], short: Optional[str]):
         self._alt_prefix = prefix
         self._alt_long = (long,) if long else set()
         self._alt_short = short
 
     def update_alts(self, name: str):
         """
@@ -108,15 +115,15 @@
         """
         if self._alt_long:
             return
 
         mode = self.name_mode or DEFAULT_CONFIG.option_name_mode
         mode_val: int = mode._value_  # noqa # This Flag doesn't subclass int due to breakage in 3.11
         if mode & OptionNameMode.DASH:
-            option = '--{}-{}'.format(self._alt_prefix, name.replace('_', '-'))
+            option = f'--{self._alt_prefix}-{name.replace("_", "-")}'
             self._alt_long.add(option)
             self._long.add(option)
             if mode_val & 16:  # OptionNameMode.BOTH_DASH = OptionNameMode.DASH | 4 | 16
                 self._display_long.add(option)
         if mode & OptionNameMode.UNDERSCORE:
             option = f'--{self._alt_prefix}_{name}'
             self._alt_long.add(option)
@@ -143,15 +150,15 @@
 
     @property
     def short_primary(self) -> List[str]:
         return [opt for opt in self.short if opt != self._alt_short]
 
     # @property
     # def long_alt(self) -> List[str]:
-    #     return self._sort_options(self._alt_long)
+    #     return _sort_options(self._alt_long)
 
     @property
     def display_long_alt(self) -> List[str]:
         return [opt for opt in self.display_long if opt in self._alt_long]
 
     @property
     def short_alt(self) -> List[str]:
@@ -161,16 +168,23 @@
         yield from self.display_long_primary
         yield from self.short_primary
 
     def alt_option_strs(self) -> Iterator[str]:
         yield from self.display_long_alt
         yield from self.short_alt
 
+    def get_usage_opt(self, alt: bool = False) -> str:
+        return next(self.option_strs(alt))
+
     def option_strs(self, alt: bool = False) -> Iterator[str]:
         if alt:
             yield from self.alt_option_strs()
         else:
             yield from self.primary_option_strs()
 
     def all_option_strs(self) -> Iterator[str]:
         yield from self.option_strs(False)
         yield from self.option_strs(True)
+
+
+def _sort_options(options: Collection[str]):
+    return sorted(options, key=lambda opt: (-len(opt), opt))
```

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/parameters/options.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/parameters/options.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,28 +2,33 @@
 Optional Parameters
 
 :author: Doug Skrypa
 """
 
 from __future__ import annotations
 
-from abc import ABC
+import logging
+from abc import ABC, abstractmethod
 from functools import partial, update_wrapper
-from typing import Any, Optional, Callable, Sequence, Iterator, Union, TypeVar, Tuple
+from typing import TYPE_CHECKING, Any, Optional, Callable, Union, TypeVar, Tuple
 
-from ..context import ctx, ParseState
-from ..exceptions import ParameterDefinitionError, BadArgument, CommandDefinitionError, ParamUsageError
+from ..context import ctx
+from ..exceptions import ParameterDefinitionError, BadArgument, CommandDefinitionError, ParamUsageError, ParamConflict
 from ..inputs import normalize_input_type
 from ..nargs import Nargs, NargsValue
-from ..typing import Bool, T_co, ChoicesType, InputTypeFunc, CommandCls, CommandObj, OptStr
-from ..utils import _NotSet
+from ..typing import T_co, TypeFunc
+from ..utils import _NotSet, ValueSource, str_to_bool
 from .base import BasicActionMixin, BaseOption, parameter_action
 from .option_strings import TriFlagOptionStrings
 
+if TYPE_CHECKING:
+    from ..typing import Bool, ChoicesType, InputTypeFunc, CommandCls, CommandObj, OptStr, ValSrc, LeadingDash
+
 __all__ = ['Option', 'Flag', 'TriFlag', 'ActionFlag', 'Counter', 'action_flag', 'before_main', 'after_main']
+log = logging.getLogger(__name__)
 
 TD = TypeVar('TD')
 TC = TypeVar('TC')
 TA = TypeVar('TA')
 
 
 class Option(BasicActionMixin, BaseOption[T_co]):
@@ -44,89 +49,115 @@
       raised if the user did not provide a value for this parameter.  Defaults to ``False``.
     :param type: A callable (function, class, etc.) that accepts a single string argument, which should be called
       on every value for this parameter to transform the value.  By default, no transformation is performed, and
       values will be strings.  If not specified, but a type annotation is detected, then that annotation will be
       used as if it was provided here.  When both are present, this argument takes precedence.
     :param choices: A container that holds the specific values that users must pick from.  By default, any value is
       allowed.
-    :param env_var: A string or sequence (tuple, list, etc) of strings representing environment variables that should
-      be searched for a value when no value was provided via CLI.  If a value was provided via CLI, then these variables
-      will not be checked.  If multiple env variable names/keys were provided, then they will be checked in the order
-      that they were provided.  When enabled, values from env variables take precedence over the default value.  When
-      enabled and the Parameter is required, then either a CLI value or an env var value must be provided.
+    :param allow_leading_dash: Whether string values may begin with a dash (``-``).  By default, if a value begins with
+      a dash, it is only accepted if it appears to be a negative numeric value.  Use ``True`` / ``always`` /
+      ``AllowLeadingDash.ALWAYS`` to allow any value that begins with a dash (as long as it is not an option string for
+      an Option/Flag/etc).  To reject all values beginning with a dash, including numbers, use ``False`` / ``never`` /
+      ``AllowLeadingDash.NEVER``.
     :param kwargs: Additional keyword arguments to pass to :class:`.BaseOption`.
     """
 
-    env_var: Union[str, Sequence[str]] = None
-
     def __init__(
         self,
         *option_strs: str,
         nargs: NargsValue = None,
         action: str = _NotSet,
         default: Any = _NotSet,
         required: Bool = False,
         type: InputTypeFunc = None,  # noqa
         choices: ChoicesType = None,
-        env_var: Union[str, Sequence[str]] = None,
+        allow_leading_dash: LeadingDash = None,
         **kwargs,
     ):
         if nargs is not None:
             self.nargs = Nargs(nargs)
         if 0 in self.nargs:
-            raise ParameterDefinitionError(f'Invalid nargs={self.nargs} - use Flag or Counter for Options with 0 args')
+            details = 'use Flag or Counter for Options with 0 args'
+            if isinstance(nargs, range) and nargs.start == 0 and nargs.step != nargs.stop:
+                suffix = f', {nargs.step}' if nargs.step != 1 else ''
+                details = f'try using range({nargs.step}, {nargs.stop}{suffix}) instead, or {details}'
+            raise ParameterDefinitionError(f'Invalid nargs={nargs!r} - {details}')
         if action is _NotSet:
             action = 'store' if self.nargs == 1 else 'append'
         elif action == 'store' and self.nargs != 1:
             raise ParameterDefinitionError(f'Invalid nargs={self.nargs} for action={action!r}')
         super().__init__(*option_strs, action=action, default=default, required=required, **kwargs)
         self.type = normalize_input_type(type, choices)
-        if env_var:
-            self.env_var = env_var
-
-    def env_vars(self) -> Iterator[str]:
-        env_var = self.env_var
-        if env_var:
-            if isinstance(env_var, str):
-                yield env_var
-            else:
-                yield from env_var
-
-
-# TODO: 1/2 flag, 1/2 option, like Counter, but for any value
+        self._validate_nargs_and_allow_leading_dash(allow_leading_dash)
 
 
 class _Flag(BaseOption[T_co], ABC):
     nargs = Nargs(0)
+    type = staticmethod(str_to_bool)  # Without staticmethod, this would be interpreted as a normal method
+    strict_env: bool
+    use_env_value: bool = False
     _use_opt_str: bool = False
 
     def __init_subclass__(cls, use_opt_str: bool = False, **kwargs):  # pylint: disable=W0222
         super().__init_subclass__(**kwargs)
         cls._use_opt_str = use_opt_str
 
-    def __init__(self, *option_strs: str, **kwargs):
+    def __init__(
+        self,
+        *option_strs: str,
+        type: TypeFunc = None,  # noqa
+        strict_env: bool = True,
+        use_env_value: bool = False,
+        **kwargs,
+    ):
         if 'metavar' in kwargs:
             raise TypeError(f"{self.__class__.__name__}.__init__() got an unexpected keyword argument: 'metavar'")
         super().__init__(*option_strs, **kwargs)
+        self.strict_env = strict_env
+        if use_env_value:
+            self.use_env_value = use_env_value
+        if type is not None:
+            self.type = type
 
-    def _init_value_factory(self, state: ParseState):
+    def _init_value_factory(self):
         if self.action == 'store_const':
             return self.default
         else:
             return []
 
-    def take_action(self, value: Optional[str], short_combo: bool = False, opt_str: str = None):
+    def take_action(
+        self, value: Optional[str], short_combo: bool = False, opt_str: str = None, src: ValSrc = ValueSource.CLI
+    ):
         # log.debug(f'{self!r}.take_action({value!r})')
         ctx.record_action(self)
-        action_method = getattr(self, self.action)
         if value is None:
+            action_method = getattr(self, self.action)
             return action_method(opt_str) if self._use_opt_str else action_method()
+        elif src != ValueSource.CLI:
+            src, env_var = src
+            try:
+                return self.take_env_var_action(value, env_var)
+            except ParamUsageError as e:
+                if not self.strict_env:
+                    log.warning(e)
+                    return
+                raise
 
         raise ParamUsageError(self, f'received value={value!r} but no values are accepted for action={self.action!r}')
 
+    def prepare_env_var_value(self, value: str, env_var: str) -> T_co:
+        try:
+            return self.type(value)
+        except Exception as e:
+            raise ParamUsageError(self, f'unable to parse value={value!r} from env_var={env_var!r}: {e}') from e
+
+    @abstractmethod
+    def take_env_var_action(self, value: str, env_var: str):
+        raise NotImplementedError
+
     def would_accept(self, value: Optional[str], short_combo: bool = False) -> bool:  # noqa
         return value is None
 
     def result_value(self) -> Any:
         return ctx.get_parsed_value(self)
 
     result = result_value
@@ -141,14 +172,28 @@
     :param action: The action to take on individual parsed values.  Actions must be defined as methods in classes
       that extend Parameter, and must be registered via :class:`.parameter_action`.  Defaults to ``store_const``, but
       accepts ``append_const`` to build a list of the specified constant.
     :param default: The default value for this parameter if it is not specified.  Defaults to ``False`` when
       ``const=True`` (the default), and to ``True`` when ``const=False``.  Defaults to ``None`` for any other
       constant.
     :param const: The constant value to store/append when this parameter is specified.  Defaults to ``True``.
+    :param type: A callable (function, class, etc.) that accepts a single string argument and returns a boolean value,
+      which should be called on environment variable values, if any are configured for this Flag via
+      :paramref:`.BaseOption.env_var`.  It should return a truthy value if any action should be taken (i.e., if the
+      constant should be stored/appended), or a falsey value for no action to be taken.  The
+      :func:`default function<.str_to_bool>` handles parsing ``1`` / ``true`` / ``yes`` and similar as ``True``,
+      and ``0`` / ``false`` / ``no`` and similar as ``False``.  If :paramref:`use_env_value` is ``True``, then this
+      function should return either the default or constant value instead.
+    :param strict_env: When ``True`` (the default), if an :paramref:`.BaseOption.env_var` is used as the source of a
+      value for this parameter and that value is invalid, then parsing will fail.  When ``False``, invalid values from
+      environment variables will be ignored (and a warning message will be logged).
+    :param use_env_value: If ``True``, when an :paramref:`.BaseOption.env_var` is used as the source of a value for
+      this Flag, the parsed value will be stored as this Flag's value (it must match either the default or constant
+      value).  If ``False`` (the default), then the parsed value will be used to determine whether this Flag's normal
+      action should be taken as if it was specified via a CLI argument.
     :param kwargs: Additional keyword arguments to pass to :class:`.BaseOption`.
     """
 
     __default_const_map = {True: False, False: True, _NotSet: True}
     default: TD
     const: TC
 
@@ -164,14 +209,24 @@
         if default is _NotSet:
             default = self.__default_const_map.get(const)  # will be True, False, or None
         if default is False:  # Avoid surprises for custom non-truthy values
             kwargs.setdefault('show_default', False)
         super().__init__(*option_strs, action=action, default=default, **kwargs)
         self.const = const
 
+    def take_env_var_action(self, value: str, env_var: str):
+        parsed = self.prepare_env_var_value(value, env_var)
+        if self.use_env_value:
+            if parsed == self.const:
+                getattr(self, self.action)()
+            elif parsed != self.default:
+                raise BadArgument(self, f'invalid value={parsed!r} from env_var={env_var!r}')
+        elif parsed:
+            getattr(self, self.action)()
+
     @parameter_action
     def store_const(self):
         ctx.set_parsed_value(self, self.const)
 
     @parameter_action
     def append_const(self):
         ctx.get_parsed_value(self).append(self.const)
@@ -191,14 +246,28 @@
     :param alt_long: The alternate long form to use.
     :param alt_short: The alternate short form to use.
     :param alt_help: The help text to display with the alternate option strings.
     :param action: The action to take on individual parsed values.  Only ``store_const`` (the default) is supported.
     :param default: The default value to use if neither the primary or alternate options are provided.  Defaults
       to None.
     :param name_mode: Override the configured :ref:`configuration:Parsing Options:option_name_mode` for this TriFlag.
+    :param type: A callable (function, class, etc.) that accepts a single string argument and returns a boolean value,
+      which should be called on environment variable values, if any are configured for this TriFlag via
+      :paramref:`.BaseOption.env_var`.  It should return a truthy value if the primary constant should be stored, or a
+      falsey value if the alternate constant should be stored.  The :func:`default function<.str_to_bool>` handles
+      parsing ``1`` / ``true`` / ``yes`` and similar as ``True``, and ``0`` / ``false`` / ``no`` and similar
+      as ``False``.  If :paramref:`use_env_value` is ``True``, then this function should return the primary or
+      alternate constant or the default value instead.
+    :param strict_env: When ``True`` (the default), if an :paramref:`.BaseOption.env_var` is used as the source of a
+      value for this parameter and that value is invalid, then parsing will fail.  When ``False``, invalid values from
+      environment variables will be ignored (and a warning message will be logged).
+    :param use_env_value: If ``True``, when an :paramref:`.BaseOption.env_var` is used as the source of a value for
+      this TriFlag, the parsed value will be stored as this TriFlag's value (it must match the primary or alternate
+      constant, or the default value).  If ``False`` (the default), then the parsed value will be used to determine
+      whether this TriFlag's normal action should be taken as if it was specified via a CLI argument.
     :param kwargs: Additional keyword arguments to pass to :class:`.BaseOption`.
     """
 
     _opt_str_cls = TriFlagOptionStrings
     option_strs: TriFlagOptionStrings
     alt_help: OptStr = None
     default: TD
@@ -209,15 +278,15 @@
         *option_strs: str,
         consts: Tuple[TC, TA] = (True, False),
         alt_prefix: str = None,
         alt_long: str = None,
         alt_short: str = None,
         alt_help: str = None,
         action: str = 'store_const',
-        default: TD = None,
+        default: TD = _NotSet,
         **kwargs,
     ):
         if alt_short and '-' in alt_short[1:]:
             raise ParameterDefinitionError(f"Bad alt_short option - may not contain '-': {alt_short}")
         elif alt_prefix and ('=' in alt_prefix or alt_prefix.startswith('-')):
             raise ParameterDefinitionError(f"Bad alt_prefix - may not contain '=' or start with '-': {alt_prefix}")
         elif not alt_prefix and not alt_long:
@@ -225,33 +294,68 @@
 
         try:
             _pos, _neg = consts
         except (ValueError, TypeError) as e:
             msg = f'Invalid consts={consts!r} - expected a 2-tuple of (positive, negative) constants to store'
             raise ParameterDefinitionError(msg) from e
 
+        if default is _NotSet and not kwargs.get('required', False):
+            default = None
+        if default in consts:
+            raise ParameterDefinitionError(
+                f'Invalid default={default!r} with consts={consts!r} - the default must not match either value'
+            )
+
         alt_opt_strs = filter(None, (alt_short, alt_long))
         super().__init__(*option_strs, *alt_opt_strs, action=action, default=default, **kwargs)
         self.consts = consts
         self.option_strs.add_alts(alt_prefix, alt_long, alt_short)
         if alt_help:
             self.alt_help = alt_help
 
     def __set_name__(self, command: CommandCls, name: str):
         super().__set_name__(command, name)
         self.option_strs.update_alts(name)
 
-    @parameter_action
-    def store_const(self, opt_str: str):
+    def _get_const(self, opt_str: str) -> Union[TC, TA]:
         if opt_str in self.option_strs.alt_allowed:
-            const = self.consts[1]
+            return self.consts[1]
         else:
-            const = self.consts[0]
+            return self.consts[0]
+
+    @parameter_action
+    def store_const(self, opt_str: str):
+        self._store_const(self._get_const(opt_str))
+
+    def _store_const(self, const: Union[TC, TA]):
         ctx.set_parsed_value(self, const)
 
+    def take_action(
+        self, value: Optional[str], short_combo: bool = False, opt_str: str = None, src: ValSrc = ValueSource.CLI
+    ):
+        if value is None:
+            prev_parsed = ctx.get_parsed_value(self)
+            const = self._get_const(opt_str)
+            if prev_parsed is not self.default and prev_parsed != const:
+                raise ParamConflict([self])
+        return super().take_action(value, short_combo, opt_str, src)
+
+    def take_env_var_action(self, value: str, env_var: str):
+        parsed = self.prepare_env_var_value(value, env_var)
+        if self.use_env_value:
+            if parsed in self.consts:
+                self._store_const(parsed)
+            elif parsed != self.default:
+                raise BadArgument(self, f'invalid value={parsed!r} from env_var={env_var!r}')
+        else:
+            self._store_const(self.consts[0] if parsed else self.consts[1])
+
+
+# region Action Flag
+
 
 class ActionFlag(Flag, repr_attrs=('order', 'before_main')):
     """
     A :class:`.Flag` that triggers the execution of a function / method / other callable when specified.
 
     :param option_strs: The long and/or short option prefixes for this option.  If no long prefixes are specified,
       then one will automatically be added based on the name assigned to this parameter.
@@ -314,14 +418,15 @@
         if not isinstance(other, ActionFlag):
             return NotImplemented
         return all(getattr(self, a) == getattr(other, a) for a in ('name', 'func', 'command', 'order', 'before_main'))
 
     def __lt__(self, other: ActionFlag) -> bool:
         if not isinstance(other, ActionFlag):
             return NotImplemented
+        # noinspection PyTypeChecker
         return (not self.before_main, self.order, self.name) < (not other.before_main, other.order, other.name)
 
     def __call__(self, func: Callable) -> ActionFlag:
         """
         Allows use as a decorator on the method to be called.  A given method can only be decorated with one ActionFlag.
 
         If stacking :class:`.Action` and :class:`.ActionFlag` decorators, the Action decorator must be first (i.e., the
@@ -356,14 +461,17 @@
 
 
 def after_main(*option_strs: str, order: Union[int, float] = 1, func: Callable = None, **kwargs) -> ActionFlag:
     """An ActionFlag that will be executed after :meth:`.Command.main`"""
     return ActionFlag(*option_strs, order=order, func=func, before_main=False, **kwargs)
 
 
+# endregion
+
+
 class Counter(BaseOption[int], accepts_values=True, accepts_none=True):
     """
     A :class:`.Flag`-like option that counts the number of times it was specified.  Supports an optional integer value
     to explicitly increase the stored value by that amount.
 
     :param option_strs: The long and/or short option prefixes for this option.  If no long prefixes are specified,
       then one will automatically be added based on the name assigned to this parameter.
@@ -384,15 +492,15 @@
         vals = {'const': const, 'default': default}
         bad_types = ', '.join(f'{k}={v!r}' for k, v in vals.items() if not isinstance(v, self.type))
         if bad_types:
             raise ParameterDefinitionError(f'Invalid type for parameters (expected int): {bad_types}')
         super().__init__(*option_strs, action=action, default=default, **kwargs)
         self.const = const
 
-    def _init_value_factory(self, state: ParseState):
+    def _init_value_factory(self):
         return self.default
 
     def prepare_value(self, value: Optional[str], short_combo: bool = False, pre_action: bool = False) -> int:
         if value is None:
             return self.const
         try:
             return self.type(value)
```

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/parameters/pass_thru.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/parameters/pass_thru.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,60 +2,62 @@
 PassThru Parameters
 
 :author: Doug Skrypa
 """
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Collection, Any
+from typing import TYPE_CHECKING, Any
 
 from ..context import ctx
 from ..exceptions import ParamUsageError, MissingArgument
 from ..nargs import Nargs
-from ..utils import _NotSet
+from ..utils import _NotSet, ValueSource
 from .base import Parameter, parameter_action
 
 if TYPE_CHECKING:
-    from ..typing import Bool
+    from ..typing import Bool, Strings, ValSrc
 
 __all__ = ['PassThru']
 
 
 class PassThru(Parameter):
     """
     Collects all remaining arguments, without processing them.  Must be preceded by ``--`` and a space.
 
     :param action: The action to take on individual parsed values.  Only ``store_all`` (the default) is supported
       for this parameter type.
     :param kwargs: Additional keyword arguments to pass to :class:`.Parameter`.
     """
 
-    nargs = Nargs('*')
+    nargs = Nargs('REMAINDER')
     missing_hint: str = "missing pass thru args separated from others with '--'"
 
     def __init__(self, action: str = 'store_all', default: Any = _NotSet, required: Bool = False, **kwargs):
         if not required and default is _NotSet:
             default = None
         super().__init__(action=action, required=required, default=default, **kwargs)
 
     @parameter_action
-    def store_all(self, values: Collection[str]):
+    def store_all(self, values: Strings):
         ctx.set_parsed_value(self, values)
 
     def take_action(  # pylint: disable=W0237
-        self, values: Collection[str], short_combo: bool = False, opt_str: str = None
+        self, values: Strings, short_combo: bool = False, opt_str: str = None, src: ValSrc = ValueSource.CLI
     ):
         value = ctx.get_parsed_value(self)
         if value is not _NotSet:
-            raise ParamUsageError(self, f'received values={values!r} but a stored value={value!r} already exists')
+            raise ParamUsageError(
+                self,
+                f'can only be specified once - found values={values!r} but a stored value={value!r} already exists',
+            )
 
         ctx.record_action(self)
         normalized = list(map(self.prepare_value, values))
-        action_method = getattr(self, self.action)
-        return action_method(normalized)
+        return getattr(self, self.action)(normalized)
 
     def result_value(self) -> Any:
         value = ctx.get_parsed_value(self)
         if value is _NotSet:
             if self.required:
                 raise MissingArgument(self)
             return self.default
```

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/parameters/positionals.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/parameters/positionals.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from ..exceptions import ParameterDefinitionError
 from ..inputs import normalize_input_type
 from ..nargs import Nargs, NargsValue
 from ..utils import _NotSet
 from .base import BasicActionMixin, BasePositional
 
 if TYPE_CHECKING:
-    from ..typing import InputTypeFunc, ChoicesType
+    from ..typing import InputTypeFunc, ChoicesType, LeadingDash
 
 __all__ = ['Positional']
 
 
 class Positional(BasicActionMixin, BasePositional, default_ok=True):
     """
     A parameter that must be provided positionally.
@@ -37,25 +37,31 @@
       values will be strings.  If not specified, but a type annotation is detected, then that annotation will be
       used as if it was provided here.  When both are present, this argument takes precedence.
     :param default: Only supported when 0 values are allowed by the specified ``nargs``.  If not specified and
       ``action='store'``, then this will default to ``None``; if ``action='append'``, and no values are provided, then
       an empty list will be returned for this Parameter.
     :param choices: A container that holds the specific values that users must pick from.  By default, any value is
       allowed.
+    :param allow_leading_dash: Whether string values may begin with a dash (``-``).  By default, if a value begins with
+      a dash, it is only accepted if it appears to be a negative numeric value.  Use ``True`` / ``always`` /
+      ``AllowLeadingDash.ALWAYS`` to allow any value that begins with a dash (as long as it is not an option string for
+      an Option/Flag/etc).  To reject all values beginning with a dash, including numbers, use ``False`` / ``never`` /
+      ``AllowLeadingDash.NEVER``.
     :param kwargs: Additional keyword arguments to pass to :class:`.BasePositional`.
     """
 
     def __init__(
         self,
         nargs: NargsValue = None,
         action: str = _NotSet,
         type: InputTypeFunc = None,  # noqa
         default: Any = _NotSet,
         *,
         choices: ChoicesType = None,
+        allow_leading_dash: LeadingDash = None,
         **kwargs,
     ):
         if nargs is not None:
             self.nargs = Nargs(nargs)
             if self.nargs == 0:
                 cls_name = self.__class__.__name__
                 raise ParameterDefinitionError(f'Invalid nargs={self.nargs} - {cls_name} must allow at least 1 value')
@@ -67,7 +73,8 @@
         if default is not _NotSet and required:
             raise ParameterDefinitionError(
                 f'Invalid default={default!r} - only allowed for Positional parameters when nargs=? or nargs=*'
             )
         kwargs.setdefault('required', required)
         super().__init__(action=action, default=default, **kwargs)
         self.type = normalize_input_type(type, choices)
+        self._validate_nargs_and_allow_leading_dash(allow_leading_dash)
```

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/parse_tree.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/parse_tree.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Union, Optional, Collection, Iterable, Iterator, MutableMapping, Dict, Set, Tuple
 
 from .exceptions import AmbiguousParseTree
+from .nargs import nargs_max_sum, nargs_min_sum
 from .utils import _parse_tree_target_repr
 
 if TYPE_CHECKING:
     from .nargs import Nargs
     from .parameters.base import BasePositional
     from .parameters.choice_map import Choice
     from .typing import OptStr, CommandCls
@@ -25,15 +26,15 @@
     n: int
     remaining: Union[int, float]
 
     def __init__(self, nargs: Nargs, remaining: Union[int, float, None] = None, n: int = 1):
         self.nargs = nargs
         self.n = n
         if remaining is None:
-            self.remaining = float('inf') if nargs.max is None else nargs.max - 1  # -1 since one would be consumed
+            self.remaining = nargs.upper_bound - 1  # -1 since one would be consumed
         else:
             self.remaining = remaining
 
     def __repr__(self) -> str:
         return f'AnyWord({self.nargs!r}, remaining={self.remaining}, n={self.n})'
 
     def __add__(self, other: int) -> AnyWord:
@@ -82,29 +83,21 @@
         return set(self._link_params(recursive))
 
     def _link_params(self, recursive: bool = False) -> Iterator[BasePositional]:
         for node in self.values():
             yield node.param
         if recursive:
             for node in self.values():
-                try:
-                    unbound = node.word.nargs.max is None
-                except AttributeError:  # node.word is not an AnyWord
-                    yield from node._link_params(True)
-                else:
-                    yield from node._link_params(not unbound)
+                yield from node._link_params(_has_upper_bound(node))
 
     def nargs_min(self) -> int:
-        return sum(p.nargs.min for p in self.link_params(True))
+        return nargs_min_sum(p.nargs for p in self.link_params(True))
 
     def nargs_max(self) -> Union[int, float]:
-        values = [p.nargs.max for p in self.link_params(True)]
-        if None in values:
-            return float('inf')
-        return sum(values)
+        return nargs_max_sum(p.nargs for p in self.link_params(True))
 
     # region AnyWord Methods
 
     @property
     def any_word(self) -> AnyWord:
         try:
             return self._any_word
@@ -256,15 +249,15 @@
     # endregion
 
     # region Build Tree
 
     @classmethod
     def build_tree(cls, command: CommandCls) -> PosNode:
         root = cls(None, None, target=command)
-        process_params(command, [root], command.__class__.params(command).positionals)
+        process_params(command, [root], command.__class__.params(command).all_positionals)
         return root
 
     def update_node(self, word: Word, param: BasePositional, target: Target) -> PosNode:
         try:
             *parts, last = word.split()
         except AttributeError:  # The choice is None or Any
             if word:
@@ -303,15 +296,15 @@
         except KeyError:
             pass
         else:
             raise AmbiguousParseTree(self, target, word)
 
         node = PosNode(word, param, target, self)
         # TODO: This needs to be converted to be lazy instead
-        if word.nargs.max is not None:
+        if word.nargs.has_upper_bound:
             while True:
                 try:
                     node = node._create_child()
                 except ValueError:
                     break
 
         return node
@@ -321,20 +314,22 @@
     def print_tree(self, indent: int = 0, recursive: bool = True):
         prefix = ' ' * indent
         print(f'{prefix}- <PosNode[{self.word!r}, links: {len(self)}, target={_parse_tree_target_repr(self.target)}]>')
         if not recursive:
             return
         indent += 2
         for node in self.values():
-            try:
-                unbound = node.word.nargs.max is None
-            except AttributeError:  # node.word is not an AnyWord
-                node.print_tree(indent, True)
-            else:
-                node.print_tree(indent, not unbound)
+            node.print_tree(indent, _has_upper_bound(node))
+
+
+def _has_upper_bound(node) -> bool:
+    try:
+        return node.word.nargs.has_upper_bound
+    except AttributeError:
+        return True
 
 
 def process_params(command: CommandCls, nodes: Iterable[PosNode], params: Iterable[BasePositional]) -> Set[PosNode]:
     for param in params:
         nodes = process_param(command, nodes, param)
 
     return nodes
@@ -354,15 +349,15 @@
             target = choice.target
             try:
                 params = get_params(target)
             except TypeError:
                 new_nodes.update(node.update_node(choice.choice, param, target) for node in nodes)
             else:
                 choice_nodes = {node.update_node(choice.choice, param, target) for node in nodes}
-                new_nodes.update(process_params(target, choice_nodes, params.positionals))
+                new_nodes.update(process_params(target, choice_nodes, params.all_positionals))
 
         return new_nodes
 
     try:
         choices: Collection[str] = param.type.choices  # noqa
     except AttributeError:  # It was not a _ChoicesBase input type
         pass
```

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/parser.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,140 +7,125 @@
 from __future__ import annotations
 
 # import logging
 from collections import deque
 from os import environ
 from typing import TYPE_CHECKING, Optional, Union, Any, Deque, List
 
-from .context import ActionPhase, Context, ParseState
+from .context import ActionPhase, Context
 from .exceptions import UsageError, ParamUsageError, NoSuchOption, MissingArgument, ParamsMissing
-from .exceptions import CommandDefinitionError, Backtrack, UnsupportedAction
+from .exceptions import Backtrack, NextCommand, UnsupportedAction
+from .nargs import REMAINDER, nargs_max_sum, nargs_min_sum
 from .parse_tree import PosNode
 from .parameters.base import BasicActionMixin, Parameter, BasePositional, BaseOption
+from .utils import ValueSource
 
 if TYPE_CHECKING:
     from .command_parameters import CommandParameters
+    from .config import CommandConfig
     from .typing import CommandType
 
 __all__ = ['CommandParser']
 # log = logging.getLogger(__name__)
 
 
 class CommandParser:
     """Stateful parser used for a single pass of argument parsing"""
 
-    __slots__ = ('_last', 'arg_deque', 'ctx', 'deferred', 'node', 'params', 'positionals')
+    __slots__ = ('_last', 'arg_deque', 'config', 'deferred', 'params', 'positionals')
 
     arg_deque: Optional[Deque[str]]
+    config: CommandConfig
     deferred: Optional[List[str]]
+    params: CommandParameters
+    positionals: List[BasePositional]
     _last: Optional[Parameter]
 
-    def __init__(self, ctx: Context):
+    def __init__(self, ctx: Context, params: CommandParameters, config: CommandConfig):
         self._last = None
-        self.ctx = ctx
-        self.params = ctx.params
-        self.positionals = ctx.params.positionals.copy()
-        if ctx.config.reject_ambiguous_pos_combos:
+        self.params = params
+        self.positionals = params.get_positionals_to_parse(ctx)
+        self.config = config
+        if config.reject_ambiguous_pos_combos:
             PosNode.build_tree(ctx.command)
 
     @classmethod
-    def parse_args(cls, ctx: Context) -> Optional[CommandType]:
+    def parse_args_and_get_next_cmd(cls, ctx: Context) -> Optional[CommandType]:
         try:
-            parsed = cls.__parse_args(ctx)
+            return cls(ctx, ctx.params, ctx.config).get_next_cmd(ctx)
         except UsageError:
-            ctx.state = ParseState.FAILED
             if not ctx.categorized_action_flags[ActionPhase.PRE_INIT]:
                 raise
             return None
-        except Exception:
-            ctx.state = ParseState.FAILED
-            raise
-        else:
-            if ctx.state == ParseState.INITIAL:
-                ctx.state = ParseState.COMPLETE
-            return parsed
-
-    @classmethod
-    def __parse_args(cls, ctx: Context) -> Optional[CommandType]:
-        params = ctx.params
-        sub_cmd_param = params.sub_command
-        if sub_cmd_param and not sub_cmd_param.choices:
-            raise CommandDefinitionError(f'{ctx.command}.{sub_cmd_param.name} = {sub_cmd_param} has no sub Commands')
 
-        cls(ctx)._parse_args(ctx)
+    def get_next_cmd(self, ctx: Context) -> Optional[CommandType]:
+        self._parse_args(ctx)
+        params = self.params
         params.validate_groups()
-
-        if sub_cmd_param:
-            next_cmd = sub_cmd_param.target()  # type: CommandType
-            missing = cls._missing(params, ctx)
-            if missing and next_cmd.__class__.parent(next_cmd) is not ctx.command:
-                ctx.state = ParseState.FAILED
-                if ctx.categorized_action_flags[ActionPhase.PRE_INIT]:
-                    return None
+        missing = ctx.get_missing()
+        no_pre_init_action = not ctx.categorized_action_flags[ActionPhase.PRE_INIT]
+        next_cmd = params.sub_command.target() if params.sub_command else None
+        if next_cmd is not None:
+            if missing and no_pre_init_action and next_cmd.__class__.parent(next_cmd) is not ctx.command:
                 raise ParamsMissing(missing)
-            return next_cmd
-
-        missing = cls._missing(params, ctx)
-        if missing and not ctx.config.allow_missing and (not params.action or params.action not in missing):
-            # Action is excluded because it provides a better error message
-            if not ctx.categorized_action_flags[ActionPhase.PRE_INIT]:
+        elif missing and not ctx.config.allow_missing and (not params.action or params.action not in missing):
+            if no_pre_init_action:
                 raise ParamsMissing(missing)
         elif ctx.remaining and not ctx.config.ignore_unknown:
-            raise NoSuchOption('unrecognized arguments: {}'.format(' '.join(ctx.remaining)))
-
-        return None
-
-    @classmethod
-    def _missing(cls, params: CommandParameters, ctx: Context) -> List[Parameter]:
-        return [p for p in params.required_check_params() if ctx.num_provided(p) == 0]
+            raise NoSuchOption(f'unrecognized arguments: {" ".join(ctx.remaining)}') from None
+        return next_cmd
 
     def _parse_args(self, ctx: Context):
         self.arg_deque = arg_deque = self.handle_pass_thru(ctx)
         self.deferred = ctx.remaining = []
         while arg_deque:
             arg = arg_deque.popleft()
-            if arg == '--':
-                if ctx.params.find_nested_pass_thru():  # pylint: disable=R1723
-                    self.deferred.append(arg)
-                    self.deferred.extend(arg_deque)
+            try:
+                if self._parse_arg(ctx, arg):
                     break
-                else:
-                    raise NoSuchOption(f'invalid argument: {arg}')
-            elif arg.startswith('---'):
-                raise NoSuchOption(f'invalid argument: {arg}')
-            elif arg.startswith('--'):
-                self.handle_long(arg)
-            elif arg.startswith('-') and arg != '-':
-                try:
-                    self.handle_short(arg)
-                except KeyError:
-                    self._check_sub_command_options(arg)
-                    if self.positionals:
-                        try:
-                            self.handle_positional(arg)
-                        except UsageError:
-                            self.deferred.append(arg)
-                    else:
-                        self.deferred.append(arg)
-            else:
-                self.handle_positional(arg)
+            except NextCommand:
+                self.deferred.append(arg)
+                self.deferred.extend(arg_deque)
+                break
 
         self._parse_env_vars(ctx)
 
+    def _parse_arg(self, ctx: Context, arg: str):
+        if arg == '--':
+            if self._maybe_consume_remainder(arg):
+                return True
+            elif ctx.params.find_nested_pass_thru():  # pylint: disable=R1723
+                # TODO: Make sure a test exists where parsing fails because required params were not provided yet
+                raise NextCommand
+            else:
+                raise NoSuchOption(f'invalid argument: {arg}')
+        elif arg.startswith('---'):
+            if not self._maybe_consume_remainder(arg):
+                raise NoSuchOption(f'invalid argument: {arg}')
+        elif arg.startswith('--'):
+            self.handle_long(arg)
+        elif arg.startswith('-') and arg != '-':
+            self.handle_short(arg)
+        else:
+            self.handle_positional(arg)
+
+        return False
+
     def _parse_env_vars(self, ctx: Context):
         # TODO: It would be helpful to store arg provenance for error messages, especially for a conflict between
         #  mutually exclusive params when they were provided via env
+        env = ValueSource.ENV
         for param in self.params.try_env_params(ctx):
             for env_var in param.env_vars():
                 try:
                     value = environ[env_var]
                 except KeyError:
                     pass
                 else:
-                    param.take_action(value)
+                    param.take_action(value, src=(env, env_var))
                     break
 
     def handle_pass_thru(self, ctx: Context) -> Deque[str]:
         remaining = ctx.remaining
         pass_thru = self.params.pass_thru
         if pass_thru is not None:
             try:
@@ -149,60 +134,92 @@
                 pass  # If required, it's handled by the normal missing param handler
             else:
                 remainder_start = separator_pos + 1
                 pass_thru.take_action(remaining[remainder_start:])
                 return deque(remaining[:separator_pos])
         return deque(remaining)
 
+    def _maybe_consume_remainder(self, arg: str) -> bool:
+        if len(self.positionals) == 1:
+            param = self.positionals[0]
+            if param.nargs.max is REMAINDER:
+                self.handle_remainder(param, arg)
+                return True
+        return False
+
+    def handle_remainder(self, param: Parameter, value: str) -> int:
+        found = param.take_action(value)
+        arg_deque = self.arg_deque
+        while arg_deque:
+            found += param.take_action(arg_deque.popleft())
+        return found
+
     def handle_positional(self, arg: str):
         # log.debug(f'handle_positional({arg=})')
         try:
-            param = self.positionals.pop(0)  # type: BasePositional
+            param: BasePositional = self.positionals.pop(0)
         except IndexError:
             self.deferred.append(arg)
         else:
-            try:
-                found = param.take_action(arg)
-            except UsageError:
-                self.positionals.insert(0, param)
-                raise
-            try:
-                self.consume_values(param, found=found)
-            except Backtrack:
-                self.positionals.insert(0, param)
+            if param.nargs.max is REMAINDER:
+                self.handle_remainder(param, arg)
             else:
-                self._last = param
+                try:
+                    found = param.take_action(arg)
+                except UsageError:
+                    self.positionals.insert(0, param)
+                    raise
+                try:
+                    self.consume_values(param, found=found)
+                except Backtrack:
+                    self.positionals.insert(0, param)
+                else:
+                    self._last = param
 
     def handle_long(self, arg: str):
         # log.debug(f'handle_long({arg=})')
         try:
             opt, param, value = self.params.long_option_to_param_value_pair(arg)
         except KeyError:
-            self._check_sub_command_options(arg)
-            self.deferred.append(arg)
+            if not self._maybe_consume_remainder(arg):
+                self._check_sub_command_options(arg)
+                self.deferred.append(arg)
         else:
             if value is not None or (param.accepts_none and not param.accepts_values):
                 param.take_action(value, opt_str=opt)
             elif not self.consume_values(param) and param.accepts_none:
                 param.take_action(None, opt_str=opt)
             self._last = param
 
     def handle_short(self, arg: str):
         # log.debug(f'handle_short({arg=})')
-        param_val_combos = self.params.short_option_to_param_value_pairs(arg)
-        # log.debug(f'Split {arg=} into {param_val_combos=}')
-        if len(param_val_combos) == 1:
-            opt, param, value = param_val_combos[0]
-            self._handle_short_value(opt, param, value)
+        try:
+            param_val_combos = self.params.short_option_to_param_value_pairs(arg)
+        except KeyError:  # Handles 3 potential KeyErrors for either the full short option or a single-char combo
+            self._handle_short_not_found(arg)
         else:
-            last_opt, last_param, _last_val = param_val_combos[-1]
-            for opt, param, _ in param_val_combos[:-1]:
-                param.take_action(None, short_combo=True, opt_str=opt)
+            # log.debug(f'Split {arg=} into {param_val_combos=}')
+            last = param_val_combos.pop()
+            if param_val_combos:
+                # Note: This loop is only executed for single char combined flags, where the values will always be None
+                for opt, param, value in param_val_combos:
+                    param.take_action(value, short_combo=True, opt_str=opt)
+            self._handle_short_value(*last)
 
-            self._handle_short_value(last_opt, last_param, None)
+    def _handle_short_not_found(self, arg: str):
+        if self._maybe_consume_remainder(arg):
+            return
+        self._check_sub_command_options(arg)
+        if self.positionals:
+            try:
+                self.handle_positional(arg)
+            except UsageError:
+                self.deferred.append(arg)
+        else:
+            self.deferred.append(arg)
 
     def _handle_short_value(self, opt: str, param: BaseOption, value: Any):
         # log.debug(f'Handling short {value=} for {param=}')
         if value is not None or (param.accepts_none and not param.accepts_values):
             param.take_action(value, short_combo=True, opt_str=opt)
         elif not self.consume_values(param) and param.accepts_none:
             param.take_action(None, short_combo=True, opt_str=opt)
@@ -211,43 +228,47 @@
 
     def _check_sub_command_options(self, arg: str):
         # log.debug(f'_check_sub_command_options({arg=})')
         # This check is only needed when subcommand option values may be misinterpreted as positional values
         if not self.positionals:
             return
         param = self.params.find_nested_option_that_accepts_values(arg)
-        if param is not None:
+        if param is None:
+            return
+        elif len(self.positionals) == 1 and 0 in self.positionals[0].nargs:
+            raise NextCommand
+        else:
             raise ParamUsageError(param, 'subcommand arguments must be provided after the subcommand')
 
     def _maybe_backtrack(self, param: Parameter, found: int) -> int:
         """
         If we hit the end of the list of provided argument values, unfulfilled Positional parameters remain, and the
         Parameter being processed accepts a variable number of arguments, then check to see if it's possible to
         backtrack to move some of those values to the remaining positionals.
 
         :param param: The :class:`.Parameter` that was consuming values when the arg_deque became empty
         :param found: The number of values that were consumed by the given Parameter
         :return: The updated found count, if backtracking was possible, otherwise the unmodified found count
         """
-        if not self.ctx.config.allow_backtrack or not self.positionals or found < 2:
+        if not self.config.allow_backtrack or not self.positionals or found < 2:
             return found
 
         can_pop = param.can_pop_counts()
         to_pop = _to_pop(self.positionals, can_pop, found - 1)
         if to_pop is None:
             return found
 
         self.arg_deque.extendleft(reversed(param.pop_last(to_pop)))
         return found - to_pop
 
     def _maybe_backtrack_last(self, param: Union[BasePositional, BasicActionMixin], found: int):
         """
         Similar to :meth:`._maybe_backtrack`, but allows backtracking even after starting to process a Positional.
         """
-        if not self.ctx.config.allow_backtrack:
+        if not self.config.allow_backtrack:
             return
 
         can_pop = self._last.can_pop_counts()
         to_pop = _to_pop([param, *self.positionals], can_pop, max(can_pop, default=0) + found, found)
         if to_pop is None:
             return
 
@@ -264,33 +285,36 @@
         """
         Consume values for the given Parameter.
 
         :param param: The active :class:`.Parameter` that should receive the discovered values
         :param found: The number of already discovered values for that Parameter (only specified for positional params)
         :return: The total number of values that were found for the given Parameter.
         """
+        remainder = param.nargs.max is REMAINDER
         while True:
             try:
                 value = self.arg_deque.popleft()
             except IndexError:
                 # log.debug(f'Ran out of values in deque while processing {param=}')
                 found = self._maybe_backtrack(param, found)
                 return self._finalize_consume(param, None, found)
             else:
                 # log.debug(f'Found {value=} in deque - may use it for {param=}')
-                if value.startswith('--'):
+                if remainder:
+                    return self.handle_remainder(param, value)
+                elif value.startswith('--'):
                     return self._finalize_consume(param, value, found)
                 elif value.startswith('-') and value != '-':
                     if self.params.get_option_param_value_pairs(value):
                         # log.debug(f'{value=} will not be used with {param=} - it is also a parameter')
                         return self._finalize_consume(param, value, found)
                     else:
                         try:
                             self._check_sub_command_options(value)
-                        except ParamUsageError as e:
+                        except (ParamUsageError, NextCommand) as e:
                             return self._finalize_consume(param, value, found, e)
 
                     if not param.would_accept(value):
                         # log.debug(f'{value=} will not be used with {param=} - it would not be accepted')
                         return self._finalize_consume(param, value, found, NoSuchOption(f'invalid argument: {value}'))
                     # log.debug(f'{value=} may be used with {param=} as a value')
 
@@ -320,19 +344,18 @@
         raise MissingArgument(param, f'expected {n} value{s}, but only found {found}')
 
 
 def _to_pop(positionals: List[BasePositional], can_pop: List[int], available: int, req_mod: int = 0) -> Optional[int]:
     if not can_pop:
         return None
 
-    required = sum(p.nargs.min for p in positionals)
+    required = nargs_min_sum(p.nargs for p in positionals)
     if available < required:
         return None
 
     required -= req_mod
-    nargs_max_vals = [p.nargs.max for p in positionals]
-    acceptable = float('inf') if None in nargs_max_vals else sum(nargs_max_vals)
+    acceptable = nargs_max_sum(p.nargs for p in positionals)
     for n in can_pop:
         if required <= n <= acceptable:
             return n
 
     return None
```

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/testing.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/testing.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import sys
 from contextlib import AbstractContextManager, contextmanager
 from difflib import unified_diff
 from io import StringIO, BytesIO
 from typing import TYPE_CHECKING, Any, Iterable, Type, Union, Callable, IO, ContextManager, Dict, List, Tuple
 from unittest import TestCase
-from unittest.mock import Mock, seal
+from unittest.mock import Mock, seal, patch
 
 from .actions import help_action
 from .commands import Command
 from .context import Context
 from .core import get_params
 from .documentation import load_commands
 from .exceptions import UsageError
@@ -36,18 +36,22 @@
     'sealed_mock',
     'load_command',
 ]
 
 Argv = List[str]
 Expected = Dict[str, Any]
 Kwargs = Dict[str, Any]
+Env = Dict[str, str]
 Case = Tuple[Argv, Expected]
+EnvCase = Tuple[Argv, Env, Expected]
 ExceptionCase = Union[Argv, Tuple[Argv, Type[Exception]], Tuple[Argv, Type[Exception], str]]
 CallExceptionCase = Union[Tuple[Kwargs, Type[Exception]], Tuple[Kwargs, Type[Exception], str]]
 
+OPT_ENV_MOD = 'cli_command_parser.parser.environ'
+
 
 class ParserTest(TestCase):
     # def setUp(self):
     #     print()
     #
     # def subTest(self, *args, **kwargs):
     #     print()
@@ -67,14 +71,25 @@
         return cmd
 
     def assert_parse_results_cases(self, cmd_cls: CommandCls, cases: Iterable[Case], message: str = None):
         for argv, expected in cases:
             with self.subTest(expected='results', argv=argv):
                 self.assert_parse_results(cmd_cls, argv, expected, message)
 
+    def assert_env_parse_results(
+        self, cmd_cls: CommandCls, argv: Argv, env: Env, expected: Expected, message: str = None
+    ) -> Command:
+        with patch(OPT_ENV_MOD, env):
+            return self.assert_parse_results(cmd_cls, argv, expected, message)
+
+    def assert_env_parse_results_cases(self, cmd_cls: CommandCls, cases: Iterable[EnvCase], message: str = None):
+        for argv, env, expected in cases:
+            with self.subTest(expected='results', argv=argv, env=env):
+                self.assert_env_parse_results(cmd_cls, argv, env, expected, message)
+
     def assert_parse_fails(
         self,
         cmd_cls: CommandCls,
         argv: Argv,
         expected_exc: Type[Exception] = UsageError,
         expected_pattern: str = None,
         message: str = None,
@@ -101,14 +116,20 @@
                     argv, exc, pat = case
                 else:
                     pat = None
 
                 with self.subTest(expected='exception', argv=argv):
                     self.assert_parse_fails(cmd_cls, argv, exc, pat, message=message)
 
+    def assert_argv_parse_fails_cases(
+        self, cmd_cls: CommandCls, cases: Iterable[Argv], exc: Type[Exception] = UsageError, message: str = None
+    ):
+        """Convenience method for calling :meth:`.assert_parse_fails_cases` with a default exception type."""
+        self.assert_parse_fails_cases(cmd_cls, cases, exc, message)
+
     def assert_call_fails(
         self,
         func: Callable,
         kwargs: Kwargs,
         exc: Type[Exception] = Exception,
         pattern: str = None,
         message: str = None,
@@ -152,14 +173,19 @@
         self.assertEqual(prefix, text[:new_line])
 
     def assert_str_contains(self, sub_text: str, text: str, diff_lines: int = 3):
         if sub_text not in text:
             diff = format_diff(sub_text, text, n=diff_lines)
             self.fail('String did not contain expected text:\n' + diff)
 
+    @contextmanager
+    def env_vars(self, case: str, **env_vars):
+        with self.subTest(case=case), patch(OPT_ENV_MOD, env_vars):
+            yield
+
 
 # region Formatting
 
 
 def _colored(text: str, color: int, end: str = '\n'):
     return f'\x1b[38;5;{color}m{text}\x1b[0m{end}'
```

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/typing.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/typing.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,30 +10,32 @@
 from typing import Tuple, List, Dict
 
 if TYPE_CHECKING:
     from datetime import datetime, date, time, timedelta
     from enum import Enum
     from pathlib import Path
     from .commands import Command
-    from .config import CommandConfig
+    from .config import CommandConfig, AllowLeadingDash
     from .core import CommandMeta
     from .inputs import InputType
     from .parameters import Parameter, ParamGroup
+    from .utils import ValueSource
 
 T = TypeVar('T')
 T_co = TypeVar('T_co', covariant=True)
 TypeFunc = Callable[[str], T_co]
 
 NT = TypeVar('NT', bound=float, covariant=True)
 Number = Union[NT, None]
 NumType = Callable[[Union[str, float, int]], NT]
 RngType = Union[range, int, Sequence[int]]
 
 InputTypeFunc = Union[None, TypeFunc, 'InputType', range, Type['Enum']]
 ChoicesType = Optional[Collection[Any]]
+ValSrc = Union['ValueSource', Tuple['ValueSource', str]]
 
 Bool = Union[bool, Any]
 Strs = Union[str, Sequence[str]]
 OptStr = Optional[str]
 OptStrs = Optional[Strs]
 Strings = Collection[str]
 PathLike = Union[str, 'Path']
@@ -44,14 +46,15 @@
 FP = Union[TextIO, BinaryIO]
 Deserializer = Callable[[Union[str, bytes, FP]], Any]
 Serializer = Callable[..., Union[str, bytes, None]]
 Converter = Union[Deserializer, Serializer]
 
 Config = Optional['CommandConfig']
 AnyConfig = Union[Config, Dict[str, Any]]
+LeadingDash = Union['AllowLeadingDash', str, bool]
 
 Param = TypeVar('Param', bound='Parameter')
 ParamList = List[Param]
 ParamOrGroup = Union[Param, 'ParamGroup']
 
 CommandObj = TypeVar('CommandObj', bound='Command')
 CommandType = TypeVar('CommandType', bound='CommandMeta')
```

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser/utils.py` & `cli_command_parser-2023.5.2/lib/cli_command_parser/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,40 +2,39 @@
 Utilities for working with terminals, strings, and Enums.
 
 :author: Doug Skrypa
 """
 
 from __future__ import annotations
 
-from enum import Flag, EnumMeta
+from enum import Flag, Enum, EnumMeta
 from shutil import get_terminal_size
 from time import monotonic
 from typing import Any, Callable, TypeVar, List
 
 try:
     from enum import CONFORM
 except ImportError:
     CONFORM = None
 
 FlagEnum = TypeVar('FlagEnum', bound='FixedFlag')
 _NotSet = object()
 
-
 # region Text Processing / Formatting
 
 
 def camel_to_snake_case(text: str, delim: str = '_') -> str:
     return ''.join(f'{delim}{c}' if i and c.isupper() else c for i, c in enumerate(text)).lower()
 
 
 def short_repr(obj: Any, max_len: int = 100, sep: str = '...', func: Callable[[Any], str] = repr) -> str:
     obj_repr = func(obj)
     if len(obj_repr) > max_len:
         part_len = (max_len - len(sep)) // 2
-        return '{}{}{}'.format(obj_repr[:part_len], sep, obj_repr[-part_len:])
+        return f'{obj_repr[:part_len]}{sep}{obj_repr[-part_len:]}'
     return obj_repr
 
 
 def _parse_tree_target_repr(target) -> str:
     try:
         return target.__name__
     except AttributeError:
@@ -119,15 +118,15 @@
 
         raise KeyError
 
     def _decompose(self) -> List[FlagEnum]:
         if self._name_ is None or '|' in self._name_:  # | check is for 3.11 where pseudo-members are assigned names
             val = self._value_
             members = ((mem, mem._value_) for mem in self.__class__)
-            return sorted(mem for mem, mem_val in members if mem_val & val == mem_val)
+            return sorted(mem for mem, mem_val in members if mem_val & val == mem_val)  # noqa
         return [self]
 
     def __lt__(self, other: FlagEnum) -> bool:
         return self._value_ < other._value_
 
 
 class Terminal:  # pylint: disable=R0903
@@ -140,7 +139,25 @@
 
     @property
     def width(self) -> int:
         if monotonic() - self._last_time > self._cache_time:
             self._width = get_terminal_size()[0]
             self._last_time = monotonic()
         return self._width
+
+
+class ValueSource(Enum):
+    CLI = 'cli'
+    ENV = 'env'
+
+
+def str_to_bool(value: str) -> bool:
+    try:
+        return bool(int(value))
+    except (TypeError, ValueError):
+        pass
+    lower = value.lower()
+    if lower in {'t', 'true', 'y', 'yes'}:
+        return True
+    elif lower in {'f', 'false', 'n', 'no'}:
+        return False
+    raise ValueError(f'Unable to parse boolean value from value={value!r}')
```

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser.egg-info/PKG-INFO` & `cli_command_parser-2023.5.2/lib/cli_command_parser.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 Metadata-Version: 2.1
 Name: cli-command-parser
-Version: 2023.4.8
+Version: 2023.5.2
 Summary: CLI Command Parser
 Home-page: https://github.com/dskrypa/cli_command_parser
 Author: Doug Skrypa
 Author-email: dskrypa@gmail.com
 License: Apache 2.0
 Project-URL: Source, https://github.com/dskrypa/cli_command_parser
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Text Processing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: wcwidth
 Provides-Extra: conversion
 License-File: LICENSE
 
 CLI Command Parser
 ##################
 
 |downloads| |py_version| |coverage_badge| |build_status| |Blue|
 
-.. |py_version| image:: https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20-blue
+.. |py_version| image:: https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20-blue
     :target: https://pypi.org/project/cli-command-parser/
 
 .. |coverage_badge| image:: https://codecov.io/gh/dskrypa/cli_command_parser/branch/main/graph/badge.svg
     :target: https://codecov.io/gh/dskrypa/cli_command_parser
 
 .. |build_status| image:: https://github.com/dskrypa/cli_command_parser/actions/workflows/run-tests.yml/badge.svg
     :target: https://github.com/dskrypa/cli_command_parser/actions/workflows/run-tests.yml
@@ -107,14 +106,31 @@
 There are no required dependencies.  Support for formatting wide characters correctly in help text descriptions can
 be included by adding `wcwidth <https://wcwidth.readthedocs.io>`__ to your project's requirements, and/or by installing
 with optional dependencies::
 
     $ pip install -U cli-command-parser[wcwidth]
 
 
+Python Version Compatibility
+============================
+
+Python versions 3.8 and above are currently supported.  The last release of CLI Command Parser that supported 3.7 was
+2023-04-30.  Support for Python 3.7 `officially ends on 2023-06-27 <https://devguide.python.org/versions/>`__.
+
+When using Python 3.8, some additional packages that backport functionality that was added in later Python versions
+are required for compatibility.
+
+To use the argparse to cli-command-parser conversion script with Python 3.8, there is a dependency on
+`astunparse <https://astunparse.readthedocs.io>`__.  If you are using Python 3.9 or above, then ``astunparse`` is not
+necessary because the relevant code was added to the stdlib ``ast`` module.  If you're unsure, you can install
+cli-command-parser with the following command to automatically handle whether that extra dependency is needed or not::
+
+    $ pip install -U cli-command-parser[conversion]
+
+
 Links
 *****
 
 - Documentation: https://dskrypa.github.io/cli_command_parser/
 - Example Scripts: https://github.com/dskrypa/cli_command_parser/tree/main/examples
 - PyPI Releases: https://pypi.org/project/cli-command-parser/
 - Source Code: https://github.com/dskrypa/cli_command_parser
```

### Comparing `cli_command_parser-2023.4.8/lib/cli_command_parser.egg-info/SOURCES.txt` & `cli_command_parser-2023.5.2/lib/cli_command_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cli_command_parser-2023.4.8/readme.rst` & `cli_command_parser-2023.5.2/readme.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 CLI Command Parser
 ##################
 
 |downloads| |py_version| |coverage_badge| |build_status| |Blue|
 
-.. |py_version| image:: https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20-blue
+.. |py_version| image:: https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20-blue
     :target: https://pypi.org/project/cli-command-parser/
 
 .. |coverage_badge| image:: https://codecov.io/gh/dskrypa/cli_command_parser/branch/main/graph/badge.svg
     :target: https://codecov.io/gh/dskrypa/cli_command_parser
 
 .. |build_status| image:: https://github.com/dskrypa/cli_command_parser/actions/workflows/run-tests.yml/badge.svg
     :target: https://github.com/dskrypa/cli_command_parser/actions/workflows/run-tests.yml
@@ -78,14 +78,31 @@
 There are no required dependencies.  Support for formatting wide characters correctly in help text descriptions can
 be included by adding `wcwidth <https://wcwidth.readthedocs.io>`__ to your project's requirements, and/or by installing
 with optional dependencies::
 
     $ pip install -U cli-command-parser[wcwidth]
 
 
+Python Version Compatibility
+============================
+
+Python versions 3.8 and above are currently supported.  The last release of CLI Command Parser that supported 3.7 was
+2023-04-30.  Support for Python 3.7 `officially ends on 2023-06-27 <https://devguide.python.org/versions/>`__.
+
+When using Python 3.8, some additional packages that backport functionality that was added in later Python versions
+are required for compatibility.
+
+To use the argparse to cli-command-parser conversion script with Python 3.8, there is a dependency on
+`astunparse <https://astunparse.readthedocs.io>`__.  If you are using Python 3.9 or above, then ``astunparse`` is not
+necessary because the relevant code was added to the stdlib ``ast`` module.  If you're unsure, you can install
+cli-command-parser with the following command to automatically handle whether that extra dependency is needed or not::
+
+    $ pip install -U cli-command-parser[conversion]
+
+
 Links
 *****
 
 - Documentation: https://dskrypa.github.io/cli_command_parser/
 - Example Scripts: https://github.com/dskrypa/cli_command_parser/tree/main/examples
 - PyPI Releases: https://pypi.org/project/cli-command-parser/
 - Source Code: https://github.com/dskrypa/cli_command_parser
```

### Comparing `cli_command_parser-2023.4.8/setup.cfg` & `cli_command_parser-2023.5.2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -41,44 +41,41 @@
 00000280: 5320 496e 6465 7065 6e64 656e 740d 0a09  S Independent...
 00000290: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
 000002a0: 7561 6765 203a 3a20 5079 7468 6f6e 0d0a  uage :: Python..
 000002b0: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
 000002c0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
 000002d0: 3a3a 2033 0d0a 0950 726f 6772 616d 6d69  :: 3...Programmi
 000002e0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000002f0: 7974 686f 6e20 3a3a 2033 2e37 0d0a 0950  ython :: 3.7...P
+000002f0: 7974 686f 6e20 3a3a 2033 2e38 0d0a 0950  ython :: 3.8...P
 00000300: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
 00000310: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000320: 2033 2e38 0d0a 0950 726f 6772 616d 6d69   3.8...Programmi
+00000320: 2033 2e39 0d0a 0950 726f 6772 616d 6d69   3.9...Programmi
 00000330: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000340: 7974 686f 6e20 3a3a 2033 2e39 0d0a 0950  ython :: 3.9...P
-00000350: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000360: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000370: 2033 2e31 300d 0a09 5072 6f67 7261 6d6d   3.10...Programm
-00000380: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000390: 5079 7468 6f6e 203a 3a20 332e 3131 0d0a  Python :: 3.11..
-000003a0: 0954 6f70 6963 203a 3a20 536f 6674 7761  .Topic :: Softwa
-000003b0: 7265 2044 6576 656c 6f70 6d65 6e74 203a  re Development :
-000003c0: 3a20 5573 6572 2049 6e74 6572 6661 6365  : User Interface
-000003d0: 730d 0a09 546f 7069 6320 3a3a 2054 6578  s...Topic :: Tex
-000003e0: 7420 5072 6f63 6573 7369 6e67 0d0a 0d0a  t Processing....
-000003f0: 5b6f 7074 696f 6e73 5d0d 0a69 6e63 6c75  [options]..inclu
-00000400: 6465 5f70 6163 6b61 6765 5f64 6174 6120  de_package_data 
-00000410: 3d20 5472 7565 0d0a 7061 636b 6167 6573  = True..packages
-00000420: 203d 2066 696e 643a 0d0a 7061 636b 6167   = find:..packag
-00000430: 655f 6469 7220 3d20 3d20 6c69 620d 0a70  e_dir = = lib..p
-00000440: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
-00000450: 203e 3d33 2e37 0d0a 7465 7374 735f 7265   >=3.7..tests_re
-00000460: 7175 6972 6520 3d20 7465 7374 746f 6f6c  quire = testtool
-00000470: 733b 2063 6f76 6572 6167 650d 0a0d 0a5b  s; coverage....[
-00000480: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
-00000490: 2e66 696e 645d 0d0a 7768 6572 6520 3d20  .find]..where = 
-000004a0: 6c69 620d 0a0d 0a5b 6f70 7469 6f6e 732e  lib....[options.
-000004b0: 6578 7472 6173 5f72 6571 7569 7265 5d0d  extras_require].
-000004c0: 0a77 6377 6964 7468 203d 200d 0a09 7763  .wcwidth = ...wc
-000004d0: 7769 6474 680d 0a63 6f6e 7665 7273 696f  width..conversio
-000004e0: 6e20 3d20 0d0a 0961 7374 756e 7061 7273  n = ...astunpars
-000004f0: 653b 2070 7974 686f 6e5f 7665 7273 696f  e; python_versio
-00000500: 6e3c 2233 2e39 220d 0a0d 0a5b 6567 675f  n<"3.9"....[egg_
-00000510: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
-00000520: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
-00000530: 300d 0a0d 0a                             0....
+00000340: 7974 686f 6e20 3a3a 2033 2e31 300d 0a09  ython :: 3.10...
+00000350: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000360: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000370: 3a20 332e 3131 0d0a 0954 6f70 6963 203a  : 3.11...Topic :
+00000380: 3a20 536f 6674 7761 7265 2044 6576 656c  : Software Devel
+00000390: 6f70 6d65 6e74 203a 3a20 5573 6572 2049  opment :: User I
+000003a0: 6e74 6572 6661 6365 730d 0a09 546f 7069  nterfaces...Topi
+000003b0: 6320 3a3a 2054 6578 7420 5072 6f63 6573  c :: Text Proces
+000003c0: 7369 6e67 0d0a 0d0a 5b6f 7074 696f 6e73  sing....[options
+000003d0: 5d0d 0a69 6e63 6c75 6465 5f70 6163 6b61  ]..include_packa
+000003e0: 6765 5f64 6174 6120 3d20 5472 7565 0d0a  ge_data = True..
+000003f0: 7061 636b 6167 6573 203d 2066 696e 643a  packages = find:
+00000400: 0d0a 7061 636b 6167 655f 6469 7220 3d20  ..package_dir = 
+00000410: 3d20 6c69 620d 0a70 7974 686f 6e5f 7265  = lib..python_re
+00000420: 7175 6972 6573 203d 203e 3d33 2e38 0d0a  quires = >=3.8..
+00000430: 7465 7374 735f 7265 7175 6972 6520 3d20  tests_require = 
+00000440: 7465 7374 746f 6f6c 733b 2063 6f76 6572  testtools; cover
+00000450: 6167 650d 0a0d 0a5b 6f70 7469 6f6e 732e  age....[options.
+00000460: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
+00000470: 7768 6572 6520 3d20 6c69 620d 0a0d 0a5b  where = lib....[
+00000480: 6f70 7469 6f6e 732e 6578 7472 6173 5f72  options.extras_r
+00000490: 6571 7569 7265 5d0d 0a77 6377 6964 7468  equire]..wcwidth
+000004a0: 203d 200d 0a09 7763 7769 6474 680d 0a63   = ...wcwidth..c
+000004b0: 6f6e 7665 7273 696f 6e20 3d20 0d0a 0961  onversion = ...a
+000004c0: 7374 756e 7061 7273 653b 2070 7974 686f  stunparse; pytho
+000004d0: 6e5f 7665 7273 696f 6e3c 2233 2e39 220d  n_version<"3.9".
+000004e0: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
+000004f0: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
+00000500: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
```

