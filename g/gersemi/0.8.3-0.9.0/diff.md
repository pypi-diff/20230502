# Comparing `tmp/gersemi-0.8.3.tar.gz` & `tmp/gersemi-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gersemi-0.8.3.tar", last modified: Sat Mar  4 16:22:35 2023, max compression
+gzip compressed data, was "gersemi-0.9.0.tar", last modified: Tue May  2 16:46:29 2023, max compression
```

## Comparing `gersemi-0.8.3.tar` & `gersemi-0.9.0.tar`

### file list

```diff
@@ -1,74 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:22:35.981796 gersemi-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-03-04 16:22:26.000000 gersemi-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11670 2023-03-04 16:22:35.981796 gersemi-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10648 2023-03-04 16:22:26.000000 gersemi-0.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:22:35.977796 gersemi-0.8.3/gersemi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/ast_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/base_command_invocation_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/base_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10691 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/builtin_commands
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/cmake.lark
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/command_invocation_dumper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:22:35.981796 gersemi-0.8.3/gersemi/command_invocation_dumpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/command_invocation_dumpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/command_invocation_dumpers/argument_aware_command_invocation_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/command_invocation_dumpers/condition_syntax_command_invocation_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/command_invocation_dumpers/ctest_command_dumpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/command_invocation_dumpers/install_command_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)    24292 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/command_invocation_dumpers/module_command_dumpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/command_invocation_dumpers/multiple_signature_command_invocation_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/command_invocation_dumpers/preserving_command_invocation_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9731 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/command_invocation_dumpers/project_command_dumpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17340 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/command_invocation_dumpers/scripting_command_dumpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/command_invocation_dumpers/section_aware_command_invocation_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/command_invocation_dumpers/set_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/command_invocation_dumpers/specialized_dumpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/command_invocation_dumpers/target_link_libraries_command_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/command_line_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/custom_command_definition_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/formatted_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/keyword_with_pairs_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/parsing_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/postprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/result.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/return_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/sanity_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/task_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:22:35.981796 gersemi-0.8.3/gersemi/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/tasks/check_formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/tasks/format_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/tasks/forward_to_stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/tasks/rewrite_in_place.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/tasks/show_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-03-04 16:22:26.000000 gersemi-0.8.3/gersemi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:22:35.977796 gersemi-0.8.3/gersemi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11670 2023-03-04 16:22:35.000000 gersemi-0.8.3/gersemi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-03-04 16:22:35.000000 gersemi-0.8.3/gersemi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-04 16:22:35.000000 gersemi-0.8.3/gersemi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-04 16:22:35.000000 gersemi-0.8.3/gersemi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-04 16:22:35.000000 gersemi-0.8.3/gersemi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-04 16:22:35.000000 gersemi-0.8.3/gersemi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-04 16:22:35.981796 gersemi-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-03-04 16:22:26.000000 gersemi-0.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 16:22:35.981796 gersemi-0.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-03-04 16:22:26.000000 gersemi-0.8.3/tests/test_custom_command_dumper_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-03-04 16:22:26.000000 gersemi-0.8.3/tests/test_custom_command_formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)    28313 2023-03-04 16:22:26.000000 gersemi-0.8.3/tests/test_executable.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-03-04 16:22:26.000000 gersemi-0.8.3/tests/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-03-04 16:22:26.000000 gersemi-0.8.3/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-03-04 16:22:26.000000 gersemi-0.8.3/tests/test_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-03-04 16:22:26.000000 gersemi-0.8.3/tests/tests_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:46:29.064202 gersemi-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-05-02 16:46:17.000000 gersemi-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-05-02 16:46:29.064202 gersemi-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15532 2023-05-02 16:46:17.000000 gersemi-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:46:29.048202 gersemi-0.9.0/gersemi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/ast_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/base_command_invocation_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/base_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/builtin_commands
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/cmake.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/command_invocation_dumper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:46:29.056202 gersemi-0.9.0/gersemi/command_invocation_dumpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/command_invocation_dumpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/command_invocation_dumpers/argument_aware_command_invocation_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/command_invocation_dumpers/condition_syntax_command_invocation_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/command_invocation_dumpers/ctest_command_dumpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24395 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/command_invocation_dumpers/module_command_dumpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/command_invocation_dumpers/multiple_signature_command_invocation_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/command_invocation_dumpers/preserving_command_invocation_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17819 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/command_invocation_dumpers/project_command_dumpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33017 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/command_invocation_dumpers/scripting_command_dumpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/command_invocation_dumpers/section_aware_command_invocation_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/command_invocation_dumpers/specialized_dumpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/command_invocation_dumpers/target_link_libraries_command_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/command_invocation_dumpers/two_word_keyword_isolator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/command_line_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/custom_command_definition_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/formatted_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/keyword_with_pairs_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/parsing_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/postprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/return_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/sanity_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/task_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:46:29.060202 gersemi-0.9.0/gersemi/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/tasks/check_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/tasks/format_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/tasks/forward_to_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/tasks/rewrite_in_place.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/tasks/show_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-02 16:46:17.000000 gersemi-0.9.0/gersemi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:46:29.048202 gersemi-0.9.0/gersemi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-05-02 16:46:29.000000 gersemi-0.9.0/gersemi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-05-02 16:46:29.000000 gersemi-0.9.0/gersemi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 16:46:29.000000 gersemi-0.9.0/gersemi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-02 16:46:29.000000 gersemi-0.9.0/gersemi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-02 16:46:29.000000 gersemi-0.9.0/gersemi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 16:46:29.000000 gersemi-0.9.0/gersemi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 16:46:29.064202 gersemi-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-02 16:46:17.000000 gersemi-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:46:29.064202 gersemi-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-02 16:46:17.000000 gersemi-0.9.0/tests/test_custom_command_dumper_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-05-02 16:46:17.000000 gersemi-0.9.0/tests/test_custom_command_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28369 2023-05-02 16:46:17.000000 gersemi-0.9.0/tests/test_executable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-02 16:46:17.000000 gersemi-0.9.0/tests/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-02 16:46:17.000000 gersemi-0.9.0/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-02 16:46:17.000000 gersemi-0.9.0/tests/test_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-02 16:46:17.000000 gersemi-0.9.0/tests/tests_generator.py
```

### Comparing `gersemi-0.8.3/LICENSE` & `gersemi-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gersemi-0.8.3/PKG-INFO` & `gersemi-0.9.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gersemi
-Version: 0.8.3
+Version: 0.9.0
 Summary: A formatter to make your CMake code the real treasure
 Home-page: https://github.com/BlankSpruce/gersemi
 Author: Blank Spruce
 Author-email: blankspruce@protonmail.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -37,14 +37,15 @@
 ```
 
 ## Usage
 
 ```
 usage: gersemi [-c] [-i] [--diff] [--default-config] [--version] [-h] [-l INTEGER]
                [--unsafe] [-q] [--color] [--definitions src [src ...]]
+               [--list-expansion {favour-inlining,favour-expansion}]
                [src ...]
 
 A formatter to make your CMake code the real treasure.
 
 positional arguments:
   src                   File or directory to format. If only - is provided input is taken
                         from stdin instead
@@ -71,14 +72,23 @@
   --color               If --diff is selected showed diff is colorized
   --definitions src [src ...]
                         Files or directories containing custom command definitions
                         (functions or macros). If only - is provided custom definitions, if
                         there are any, are taken from stdin instead. Commands from not
                         deprecated CMake native modules don't have to be provided (check
                         https://cmake.org/cmake/help/latest/manual/cmake-modules.7.html)
+  --list-expansion {favour-inlining,favour-expansion}
+                        Switch controls how code is expanded into multiple lines when it's
+                        not possible to keep it formatted in one line. With 'favour-
+                        inlining' (default) the list of entities will be formatted in such
+                        way that sublists might still be formatted into single line as long
+                        as it's possible. With 'favour-expansion' the list of entities will
+                        be formatted in such way that sublists will be completely expanded
+                        once expansion becomes necessary at all.
+
 ```
 
 ### [pre-commit](https://pre-commit.com/) hook
 
 You can use gersemi with a pre-commit hook by adding the following to `.pre-commit-config.yaml` of your repository:
 ```yaml
 repos:
@@ -92,16 +102,19 @@
 
 ## Formatting
 
 The key goal is for the tool to "just work" and to have as little configuration as possible so that you don't have to worry about fine-tuning formatter to your needs - as long as you embrace the `gersemi` style of formatting, similarly as `black` or `gofmt` do their job. Currently only line length can be changed with `80` as default value. Currently the basic assumption is that code to format is valid CMake language code - `gersemi` might be able to format some particular cases of invalid code but it's not guaranteed and it shouldn't be relied upon. Moreover only commands from CMake 3.0 onwards are supported and will be formatted properly - for instance [`exec_program` has been deprecated since CMake 3.0](https://cmake.org/cmake/help/latest/command/exec_program.html) so it won't be formatted. Be warned though it's not production ready so the changes to code might be destructive and you should always have a backup (version control helps a lot).
 
 ### Style
 
-Here's an example of `gersemi` style of formatting:
+#### Default style `favour-inlining`
+
+`gersemi` will try to format the code in a way that respects set character limit for single line and only break line whenever necessary.
 
+Example:
 ```cmake
 cmake_minimum_required(VERSION 3.18 FATAL_ERROR)
 project(example CXX)
 
 message(STATUS "This is example project")
 message(
     STATUS
@@ -213,14 +226,162 @@
     COMMAND
         cmake -E echo "something quite a bit                           longer"
     WORKING_DIRECTORY ${CMAKE_CURRENT_BINARY_DIR}/something
     DEPENDS
         ${CMAKE_CURRENT_SOURCE_DIR}/something
         ${CMAKE_CURRENT_SOURCE_DIR}/something_else
     COMMENT "example custom command"
+)
+```
+
+#### Alternative style `favour-expansion`
+
+In this style lines are broken in one of these cases:
+- there is at least one multi-value argument present a single command invocation, either keyworded one like `PUBLIC` in `target_link_libraries` or standalone one like list of files in `add_library`, which has more than one value
+- there are more than one multi-value arguments present in the command invocation like `target_link_libraries` with `PUBLIC` and `PRIVATE` arguments.
+- character limit for single line is reached
+
+One-value arguments (like `NAME` in `add_test`) will be inlined unless that'd violate character limit. Structure or control flow commands (`if`, `while`, `function`, `foreach` etc.) are exempted from these special rules and follow the same formatting as `favour-inlining`. This style is more merge or `git blame` friendly because usually multi-value arguments are changed one element at a time and with this style such change will be visible as one line of code per element.
+
+Example:
+```cmake
+cmake_minimum_required(VERSION 3.18 FATAL_ERROR)
+project(example CXX)
+
+message(STATUS "This is example project")
+message(
+    STATUS
+    "Here is yet another but much much longer message that should be displayed"
+)
+
+# project version
+set(VERSION_MAJOR 0)
+set(VERSION_MINOR 1)
+set(VERSION_PATCH 0)
+
+add_compile_options(
+    -Wall
+    -Wpedantic
+    -fsanitize=address
+    -fconcepts
+    -fsomething-else
+)
+
+if(NOT ${SOME_OPTION})
+    add_compile_options(-Werror)
+endif()
+
+# foobar library
+add_library(foobar)
+add_library(example::foobar ALIAS foobar)
+
+target_sources(
+    foobar
+    PUBLIC
+        include/some_subdirectory/header.hpp
+        include/another_subdirectory/header.hpp
+    PRIVATE
+        src/some_subdirectory/src1.cpp
+        src/some_subdirectory/src1.cpp
+        src/another_subdirectory/src1.cpp
+        src/another_subdirectory/src2.cpp
+        src/another_subdirectory/src3.cpp
+)
+
+target_include_directories(
+    foobar
+    INTERFACE
+        $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/include>
+        $<INSTALL_INTERFACE:include>
+)
+
+target_link_libraries(
+    foobar
+    PUBLIC
+        example::dependency_one
+        example::dependency_two
+    PRIVATE
+        example::some_util
+        external::some_lib
+        external::another_lib
+        Boost::Boost
+)
+
+include(GNUInstallDirs)
+set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/${CMAKE_INSTALL_LIBDIR})
+set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/${CMAKE_INSTALL_LIBDIR})
+set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/${CMAKE_INSTALL_BINDIR})
+
+# example executable
+add_executable(app main.cpp)
+target_link_libraries(
+    app
+    PRIVATE
+        example::foobar
+        Boost::Boost
+)
+
+# tests
+include(CTest)
+include(GTest)
+enable_testing()
+add_subdirectory(tests)
+
+# some helper function - see more details in "Let's make a deal" section
+function(add_test_executable)
+    set(OPTIONS
+        QUIET
+        VERBOSE
+        SOME_PARTICULARLY_LONG_KEYWORD_THAT_ENABLES_SOMETHING
+    )
+    set(ONE_VALUE_ARGS
+        NAME
+        TESTED_TARGET
+    )
+    set(MULTI_VALUE_ARGS
+        SOURCES
+        DEPENDENCIES
+    )
+
+    cmake_parse_arguments(
+        THIS_FUNCTION_PREFIX
+        ${OPTIONS}
+        ${ONE_VALUE_ARGS}
+        ${MULTI_VALUE_ARGS}
+    )
+    # rest of the function
+endfunction()
+
+add_test_executable(
+    NAME foobar_tests
+    TESTED_TARGET foobar
+    SOURCES
+        some_test1.cpp
+        some_test2.cpp
+        some_test3.cpp
+        some_test4.cpp
+        some_test5.cpp
+    QUIET
+    DEPENDENCIES googletest::googletest
+)
+
+add_custom_command(
+    OUTPUT
+        ${SOMETHING_TO_OUTPUT}
+    COMMAND
+        ${CMAKE_COMMAND} -E cat foobar
+    COMMAND
+        cmake -E echo foobar
+    COMMAND
+        cmake -E echo "something quite a bit                           longer"
+    WORKING_DIRECTORY ${CMAKE_CURRENT_BINARY_DIR}/something
+    DEPENDS
+        ${CMAKE_CURRENT_SOURCE_DIR}/something
+        ${CMAKE_CURRENT_SOURCE_DIR}/something_else
+    COMMENT "example custom command"
 )
 ```
 
 ### Let's make a deal
 
 It's possible to provide reasonable formatting for custom commands. However on language level there are no hints available about supported keywords for given command so `gersemi` has to generate specialized formatter. To do that custom command definition is necessary which should be provided with `--definitions`. There are limitations though since it'd probably require full-blown CMake language interpreter to do it in every case so let's make a deal: if your custom command definition (function or macro) uses `cmake_parse_arguments` and does it in obvious manner such specialized formatter will be generated. For instance this definition is okay (you can find other examples in `tests/custom_command_formatting/`):
 ```cmake
```

### Comparing `gersemi-0.8.3/gersemi/__main__.py` & `gersemi-0.9.0/gersemi/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -118,14 +118,25 @@
         nargs="+",
         type=pathlib.Path,
         help="Files or directories containing custom command definitions (functions or macros). "
         "If only - is provided custom definitions, if there are any, are taken from stdin instead. "
         "Commands from not deprecated CMake native modules don't have to be provided "
         "(check https://cmake.org/cmake/help/latest/manual/cmake-modules.7.html)",
     )
+    configuration_group.add_argument(
+        "--list-expansion",
+        dest="list_expansion",
+        choices=["favour-inlining", "favour-expansion"],
+        help="Switch controls how code is expanded into multiple lines when it's not possible "
+        "to keep it formatted in one line. With 'favour-inlining' (default) the list of entities "
+        "will be formatted in such way that sublists might still be formatted into single line "
+        "as long as it's possible. With 'favour-expansion' the list of entities will be formatted "
+        "in such way that sublists will be completely expanded once expansion becomes necessary "
+        "at all.",
+    )
 
     parser.add_argument(
         dest="sources",
         metavar="src",
         nargs="*",
         type=pathlib.Path,
         help="File or directory to format. "
```

### Comparing `gersemi-0.8.3/gersemi/ast_helpers.py` & `gersemi-0.9.0/gersemi/ast_helpers.py`

 * *Files 20% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 
     def _visit(self, tree: Tree) -> bool:
         subtrees = filter(lambda node: isinstance(node, Tree), tree.children)
         return any(map(self.visit, subtrees))
 
     arguments = _visit
     commented_argument = _visit
+    unary_operation = _visit
+    binary_operation = _visit
 
 
 def contains_line_comment(nodes) -> bool:
     visit = ContainsLineComment().visit
     return any(map(lambda node: isinstance(node, Tree) and visit(node), nodes))
```

### Comparing `gersemi-0.8.3/gersemi/base_command_invocation_dumper.py` & `gersemi-0.9.0/gersemi/base_command_invocation_dumper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+from typing import List
 from gersemi.ast_helpers import contains_line_comment
 from gersemi.base_dumper import BaseDumper
+from gersemi.configuration import ListExpansion
+from gersemi.types import Nodes
 
 
 class BaseCommandInvocationDumper(BaseDumper):
     def format_command_with_short_name(self, begin, arguments, end):
         with self.indented():
             formatted_arguments = self.visit(arguments).lstrip()
         if (
@@ -15,46 +18,65 @@
         return f"{self._indent(begin)}{formatted_arguments}\n{self._indent(end)}"
 
     def _format_command_with_long_name(self, begin, arguments, end):
         with self.indented():
             formatted_arguments = self.visit(arguments)
         return "\n".join([self._indent(begin), formatted_arguments, self._indent(end)])
 
+    def _split_arguments(self, arguments: Nodes) -> List[Nodes]:
+        return [arguments]
+
+    def group_size(self, group):
+        return len(group)
+
+    def _inlining_condition(self, arguments):
+        groups = self._split_arguments(arguments.children)
+        group_sizes = list(map(self.group_size, groups))
+        if (
+            self.list_expansion == ListExpansion.FavourExpansion
+            and not self.inhibit_favour_expansion
+        ):
+            return all(size < 2 for size in group_sizes)
+        return all(size <= 4 for size in group_sizes)
+
     def format_command(self, tree):
         identifier, arguments = tree.children
+        arguments = self._preprocess_arguments(arguments)
         begin = f"{identifier}("
         end = ")"
-        if len(arguments.children) <= 4:
+        if self._inlining_condition(arguments):
             result = self._try_to_format_into_single_line(
-                arguments.children, separator=" ", prefix=begin, postfix=end
+                arguments.children, separator=" ", prefix=f"{identifier}(", postfix=")"
             )
             if result is not None:
                 return result
 
-        if len(begin) <= self.indent_size:
-            return self.format_command_with_short_name(begin, arguments, end)
-        return self._format_command_with_long_name(begin, arguments, end)
+        with self.select_expansion_strategy():
+            if len(begin) == self.indent_size:
+                return self.format_command_with_short_name(begin, arguments, end)
+            return self._format_command_with_long_name(begin, arguments, end)
 
     def arguments(self, tree):
         return "\n".join(self.visit_children(tree))
 
     def commented_argument(self, tree):
         argument, comment, *_ = tree.children
         formatted_argument = self.visit(argument)
         with self.not_indented():
             formatted_comment = self.visit(comment)
         return f"{formatted_argument} {formatted_comment}"
 
     def complex_argument(self, tree):
         arguments, *_ = tree.children
-        result = self._try_to_format_into_single_line(
-            arguments.children, separator=" ", prefix="(", postfix=")"
-        )
-        if result is not None:
-            return result
+        if len(arguments.children) <= 4:
+            result = self._try_to_format_into_single_line(
+                arguments.children, separator=" ", prefix="(", postfix=")"
+            )
+            if result is not None:
+                return result
 
         begin = self._indent("(\n")
         with self.indented():
             formatted_arguments = self.visit(arguments)
         end = self._indent(")")
         return f"{begin}{formatted_arguments}\n{end}"
 
@@ -65,7 +87,10 @@
         return " " * self.alignment + self.__default__(tree)
 
     def quoted_argument(self, tree):
         return " " * self.alignment + f'"{self.__default__(tree)}"'
 
     def unquoted_argument(self, tree):
         return self._indent(self.__default__(tree))
+
+    def _preprocess_arguments(self, arguments):
+        return arguments
```

### Comparing `gersemi-0.8.3/gersemi/base_dumper.py` & `gersemi-0.9.0/gersemi/base_dumper.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 from contextlib import contextmanager
 from textwrap import indent
 from typing import Optional
 from lark import Tree
 from lark.visitors import Interpreter
 from gersemi.ast_helpers import contains_line_comment
+from gersemi.configuration import ListExpansion
 from gersemi.types import Nodes
 
 
 class BaseDumper(Interpreter):
     def __init__(self, width, alignment=0):
         self.width = width
         self.indent_size = 4
         self.alignment = alignment
+        self.favour_expansion = False
 
     def __default__(self, tree: Tree):
         return "".join(self.visit_children(tree))
 
     def _indent(self, text: str):
         return indent(text, " " * self.alignment)
 
     def _try_to_format_into_single_line(
         self, children: Nodes, separator: str = "", prefix: str = "", postfix: str = ""
     ) -> Optional[str]:
+        if self.favour_expansion:
+            return None
+
         if not contains_line_comment(children):
             with self.not_indented():
                 formatted_children = separator.join(
                     self.visit(c) if isinstance(c, Tree) else c for c in children
                 )
             result = self._indent(f"{prefix}{formatted_children}{postfix}")
             if len(result) <= self.width and "\n" not in result:
@@ -42,7 +47,25 @@
             self.alignment = old_alignment
 
     def indented(self):
         return self.aligned_to(self.alignment + self.indent_size)
 
     def not_indented(self):
         return self.aligned_to(0)
+
+    @contextmanager
+    def select_expansion_strategy(self):
+        old = self.favour_expansion
+        try:
+            self.favour_expansion = self.list_expansion == ListExpansion.FavourExpansion
+            yield self
+        finally:
+            self.favour_expansion = old
+
+    @contextmanager
+    def select_inlining_strategy(self):
+        old = self.favour_expansion
+        try:
+            self.favour_expansion = False
+            yield self
+        finally:
+            self.favour_expansion = old
```

### Comparing `gersemi-0.8.3/gersemi/builtin_commands` & `gersemi-0.9.0/gersemi/builtin_commands`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 ## Scripting Commands
 block
 break
 cmake_host_system_information
 cmake_language
 cmake_minimum_required
 cmake_parse_arguments
+cmake_path
 cmake_policy
 configure_file
 continue
 else
 elseif
 endblock
 endforeach
```

### Comparing `gersemi-0.8.3/gersemi/cache.py` & `gersemi-0.9.0/gersemi/cache.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.8.3/gersemi/cmake.lark` & `gersemi-0.9.0/gersemi/cmake.lark`

 * *Files identical despite different names*

### Comparing `gersemi-0.8.3/gersemi/command_invocation_dumper.py` & `gersemi-0.9.0/gersemi/command_invocation_dumper.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,16 +50,16 @@
             self.__class__ = old_class  # pylint: disable=invalid-class-object
 
     def _get_patch(self, command_name):
         if command_name in BUILTIN_COMMAND_MAPPING:
             return BUILTIN_COMMAND_MAPPING[command_name]
 
         if command_name in self.custom_command_definitions:
-            keywords = self.custom_command_definitions[command_name]
-            return create_specialized_dumper(keywords)
+            arguments = self.custom_command_definitions[command_name]
+            return create_specialized_dumper(*arguments)
 
         return None
 
     def command_invocation(self, tree):
         command_name, _ = tree.children
         patch = self._get_patch(command_name)
         if patch is None:
```

### Comparing `gersemi-0.8.3/gersemi/command_invocation_dumpers/argument_aware_command_invocation_dumper.py` & `gersemi-0.9.0/gersemi/command_invocation_dumpers/condition_syntax_command_invocation_dumper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,139 +1,174 @@
-from typing import Dict, Iterator, Iterable, List, Optional, Sized, Tuple
-from gersemi.ast_helpers import is_one_of_keywords, is_comment
+from typing import List
+from lark import Tree
+from lark.visitors import Transformer, TransformerChain, Transformer_InPlace
+from gersemi.ast_helpers import contains_line_comment, is_one_of_keywords
 from gersemi.base_command_invocation_dumper import BaseCommandInvocationDumper
 from gersemi.types import Nodes
-from gersemi.utils import pop_all
+from gersemi.utils import advance
 
 
-def to_list_of_single_item_lists(sequence):
-    return [*map(lambda item: [item], sequence)]
+class IsolateUnaryOperators(Transformer_InPlace):
+    unary_operators: List[str] = []
 
+    def arguments(self, children: Nodes) -> Tree:
+        if len(children) < 2:
+            return Tree("arguments", children)
+
+        new_children: Nodes = []
+        iterator = zip(children, children[1:])
+        is_one_of_unary_operators = is_one_of_keywords(self.unary_operators)
+        for one_behind, current in iterator:
+            if is_one_of_unary_operators(one_behind):
+                new_children += [Tree("unary_operation", [one_behind, current])]
+                _, current = advance(iterator, times=1, default=(None, None))
+                if current is None:
+                    break
+            else:
+                new_children += [one_behind]
+        else:
+            new_children += [item for item in [current] if item is not None]
+        return Tree("arguments", new_children)
 
-def is_non_empty(sequence: Sized) -> bool:
-    return len(sequence) > 0
 
+class IsolateUnaryTests(IsolateUnaryOperators):
+    unary_operators: List[str] = [
+        "COMMAND",
+        "POLICY",
+        "TARGET",
+        "TEST",
+        "EXISTS",
+        "IS_DIRECTORY",
+        "IS_SYMLINK",
+        "IS_ABSOLUTE",
+        "DEFINED",
+    ]
+
+
+class IsolateBinaryTests(Transformer_InPlace):
+    binary_operators: List[str] = [
+        "IS_NEWER_THAN",
+        "MATCHES",
+        "LESS",
+        "GREATER",
+        "EQUAL",
+        "LESS_EQUAL",
+        "GREATER_EQUAL",
+        "STRLESS",
+        "STRGREATER",
+        "STREQUAL",
+        "STRLESS_EQUAL",
+        "STRGREATER_EQUAL",
+        "VERSION_LESS",
+        "VERSION_GREATER",
+        "VERSION_EQUAL",
+        "VERSION_LESS_EQUAL",
+        "VERSION_GREATER_EQUAL",
+        "IN_LIST",
+        "PATH_EQUAL",
+    ]
+
+    def arguments(self, children: Nodes) -> Tree:
+        if len(children) < 3:
+            return Tree("arguments", children)
+
+        new_children: Nodes = []
+        iterator = zip(children, children[1:], children[2:])
+        is_one_of_binary_operators = is_one_of_keywords(self.binary_operators)
+        for two_behind, one_behind, current in iterator:
+            if is_one_of_binary_operators(one_behind):
+                new_children += [
+                    Tree("binary_operation", [two_behind, one_behind, current])
+                ]
+                _, one_behind, current = advance(
+                    iterator, times=2, default=(None, None, None)
+                )
+                if current is None:
+                    break
+            else:
+                new_children += [two_behind]
+        else:
+            new_children += [item for item in [one_behind, current] if item is not None]
+        return Tree("arguments", new_children)
 
-def is_empty(sequence: Sized) -> bool:
-    return len(sequence) <= 0
 
+class IsolateNotExpressions(IsolateUnaryOperators):
+    unary_operators: List[str] = ["NOT"]
 
-class KeywordSplitter:
-    def __init__(self, options, one_value_keywords, multi_value_keywords):
-        self.is_one_of_options = is_one_of_keywords(options)
-        self.is_one_of_one_value_keywords = is_one_of_keywords(one_value_keywords)
-        self.is_one_of_multi_value_keywords = is_one_of_keywords(multi_value_keywords)
-        self.groups: List[Nodes] = []
-        self.accumulator: Nodes = []
-        self.comment_accumulator: Nodes = []
 
-    def _flush_accumulators(self):
-        each_comment_in_its_own_group = [[c] for c in pop_all(self.comment_accumulator)]
-        argument_group = pop_all(self.accumulator)
-        self.groups += [argument_group, *each_comment_in_its_own_group]
+class IsolateAndExpressions(IsolateUnaryOperators):
+    unary_operators: List[str] = ["AND"]
 
-    def _append_option_group(self, argument):
-        self._flush_accumulators()
-        self.groups += [[argument]]
 
-    def _append_one_value_group(self, argument, iterator):
-        self._flush_accumulators()
-        next_argument = next(iterator, None)
-        if next_argument is None:
-            self.groups += [[argument]]
-        else:
-            self.groups += [[argument, next_argument]]
+class IsolateOrExpressions(IsolateUnaryOperators):
+    unary_operators: List[str] = ["OR"]
 
-    def split(self, arguments: Nodes) -> Tuple[Iterator[Nodes], Nodes]:
-        iterator = iter(arguments)
-        tail: Optional[Nodes] = None
-        for argument in iterator:
-            if is_comment(argument):
-                self.comment_accumulator += [argument]
-            elif self.is_one_of_options(argument):
-                self._append_option_group(argument)
-            elif self.is_one_of_one_value_keywords(argument):
-                self._append_one_value_group(argument, iterator)
-            elif self.is_one_of_multi_value_keywords(argument):
-                self._flush_accumulators()
-                self.accumulator = [argument]
-            elif is_non_empty(self.accumulator):
-                self.accumulator += [*pop_all(self.comment_accumulator), argument]
-            else:
-                tail = [argument, *iterator]
-                break
 
-        self._flush_accumulators()
-        if tail is None:
-            tail = [*iterator]
-        return filter(is_non_empty, self.groups), tail
-
-
-class ArgumentAwareCommandInvocationDumper(BaseCommandInvocationDumper):
-    options: Iterable[str] = []
-    one_value_keywords: Iterable[str] = []
-    multi_value_keywords: Iterable[str] = []
-    keyword_formatters: Dict[str, str] = {}
+def IsolateConditions() -> Transformer:
+    return TransformerChain(
+        IsolateUnaryTests(),
+        IsolateBinaryTests(),
+        IsolateNotExpressions(),
+        IsolateAndExpressions(),
+        IsolateOrExpressions(),
+    )
 
-    def _default_format_values(self, values) -> str:
-        return "\n".join(map(self.visit, values))
 
-    def _format_group(self, group) -> str:
-        result = self._try_to_format_into_single_line(group, separator=" ")
+class ConditionSyntaxCommandInvocationDumper(BaseCommandInvocationDumper):
+    inhibit_favour_expansion = True
+
+    def unary_operation(self, tree):
+        result = self._try_to_format_into_single_line(tree.children, separator=" ")
         if result is not None:
             return result
 
-        keyword, *values = group
-        begin = self.visit(keyword)
-        if len(values) == 0:
-            return begin
+        operation, arg = tree.children
+        formatted_operation = self.visit(operation)
+
+        if (not contains_line_comment([operation])) and (
+            len(formatted_operation.strip()) < self.indent_size
+        ):
+            return f"{formatted_operation} {self.visit(arg).lstrip()}"
 
-        keyword_as_value = keyword.children[0]
         with self.indented():
-            formatter = getattr(
-                self,
-                self.keyword_formatters.get(keyword_as_value, "_default_format_values"),
-            )
-            formatted_values = formatter(values)
-        return f"{begin}\n{formatted_values}"
-
-    def _separate_front(self, arguments: Nodes) -> Tuple[List[Nodes], Nodes]:
-        is_one_of_keywords_with_values = is_one_of_keywords(
-            list(self.one_value_keywords) + list(self.multi_value_keywords)
-        )
-        for index, argument in enumerate(arguments):
-            if is_one_of_keywords_with_values(argument):
-                pivot = index
-                break
-        else:
-            return to_list_of_single_item_lists(arguments), []
-        return to_list_of_single_item_lists(arguments[:pivot]), arguments[pivot:]
+            formatted_arg = self.visit(arg)
+        return f"{formatted_operation}\n{formatted_arg}"
 
-    def _split_by_keywords(self, arguments: Nodes) -> Tuple[Iterator[Nodes], Nodes]:
-        splitter = KeywordSplitter(
-            self.options, self.one_value_keywords, self.multi_value_keywords
-        )
-        return splitter.split(arguments)
+    def binary_operation(self, tree):
+        result = self._try_to_format_into_single_line(tree.children, separator=" ")
+        if result is not None:
+            return result
+
+        lhs, operation, rhs = tree.children
+        formatted_lhs = self.visit(lhs)
+        with self.indented():
+            formatted_operation = self.visit(operation)
+            formatted_rhs = self.visit(rhs)
+        return f"{formatted_lhs}\n{formatted_operation}\n{formatted_rhs}"
+
+    def arguments(self, tree):
+        preprocessed = IsolateConditions().transform(tree)
+        return super().arguments(preprocessed)
+
+    def _preprocess_arguments(self, arguments):
+        return IsolateConditions().transform(arguments)
+
+    def _split_arguments(self, arguments):
+        if len(arguments) < 1:
+            return arguments
 
-    def _split_arguments(self, arguments: Nodes) -> List[Nodes]:
-        front, tail = self._separate_front(arguments)
-        keyworded_arguments, tail = self._split_by_keywords(tail)
-        back = to_list_of_single_item_lists(tail)
-        return [*front, *keyworded_arguments, *back]
+        head, *tail = arguments
+        return [[head], tail]
 
-    def format_command(self, tree):
-        identifier, arguments = tree.children
+    def complex_argument(self, tree):
+        arguments, *_ = tree.children
         result = self._try_to_format_into_single_line(
-            arguments.children, separator=" ", prefix=f"{identifier}(", postfix=")"
+            arguments.children, separator=" ", prefix="(", postfix=")"
         )
         if result is not None:
             return result
 
-        begin = self._indent(f"{identifier}(")
+        begin = self._indent("(\n")
         with self.indented():
             formatted_arguments = self.visit(arguments)
         end = self._indent(")")
-        return f"{begin}\n{formatted_arguments}\n{end}"
-
-    def arguments(self, tree):
-        groups = self._split_arguments(tree.children)
-        return "\n".join(map(self._format_group, groups))
+        return f"{begin}{formatted_arguments}\n{end}"
```

### Comparing `gersemi-0.8.3/gersemi/command_invocation_dumpers/ctest_command_dumpers.py` & `gersemi-0.9.0/gersemi/command_invocation_dumpers/ctest_command_dumpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 
 
 class CTestRunScript(ArgumentAwareCommandInvocationDumper):
     one_value_keywords = ["RETURN_VALUE"]
 
 
 class CTestStart(ArgumentAwareCommandInvocationDumper):
+    front_positional_arguments = ["<model>", "<source>", "<binary>"]
     options = ["APPEND", "QUIET"]
     one_value_keywords = ["GROUP"]
 
 
 class CTestSubmit(ArgumentAwareCommandInvocationDumper):
     options = ["QUIET"]
     one_value_keywords = [
```

### Comparing `gersemi-0.8.3/gersemi/command_invocation_dumpers/module_command_dumpers.py` & `gersemi-0.9.0/gersemi/command_invocation_dumpers/module_command_dumpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,15 @@
         "TESTS",
         "CACHE_ENTRIES",
         "PROPERTIES",
     ]
 
 
 class ConfigurePackageConfigFile(ArgumentAwareCommandInvocationDumper):
+    front_positional_arguments = ["<input>", "<output>"]
     options = ["NO_SET_AND_CHECK_MACRO", "NO_CHECK_REQUIRED_COMPONENTS_MACRO"]
     one_value_keywords = ["INSTALL_DESTINATION", "INSTALL_PREFIX"]
     multi_value_keywords = ["PATH_VARS"]
 
 
 class CPackAddComponent(ArgumentAwareCommandInvocationDumper):
     options = ["HIDDEN", "REQUIRED", "DISABLED", "DOWNLOADED"]
@@ -534,14 +535,15 @@
 
 
 class GTestDiscoverTests(
     CommandLineFormatter,
     KeywordWithPairsFormatter,
     ArgumentAwareCommandInvocationDumper,
 ):
+    front_positional_arguments = ["<target>"]
     options = ["NO_PRETTY_TYPES", "NO_PRETTY_VALUES"]
     one_value_keywords = [
         "WORKING_DIRECTORY",
         "TEST_PREFIX",
         "TEST_SUFFIX",
         "TEST_LIST",
         "DISCOVERY_TIMEOUT",
```

### Comparing `gersemi-0.8.3/gersemi/command_invocation_dumpers/preserving_command_invocation_dumper.py` & `gersemi-0.9.0/gersemi/command_invocation_dumpers/preserving_command_invocation_dumper.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.8.3/gersemi/command_invocation_dumpers/scripting_command_dumpers.py` & `gersemi-0.9.0/gersemi/command_invocation_dumpers/project_command_dumpers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,587 +1,542 @@
 from gersemi.command_line_formatter import CommandLineFormatter
 from gersemi.keyword_with_pairs_formatter import KeywordWithPairsFormatter
 from .argument_aware_command_invocation_dumper import (
     ArgumentAwareCommandInvocationDumper,
 )
-from .condition_syntax_command_invocation_dumper import (
-    ConditionSyntaxCommandInvocationDumper,
-)
 from .multiple_signature_command_invocation_dumper import (
     MultipleSignatureCommandInvocationDumper,
 )
-from .set_command import Set
+from .section_aware_command_invocation_dumper import SectionAwareCommandInvocationDumper
+from .target_link_libraries_command_dumper import TargetLinkLibraries
+from .two_word_keyword_isolator import TwoWordKeywordIsolator
+
+
+class AddCustomCommand(CommandLineFormatter, MultipleSignatureCommandInvocationDumper):
+    customized_signatures = {
+        "OUTPUT": dict(
+            options=["VERBATIM", "APPEND", "USES_TERMINAL", "COMMAND_EXPAND_LISTS"],
+            one_value_keywords=[
+                "MAIN_DEPENDENCY",
+                "WORKING_DIRECTORY",
+                "COMMENT",
+                "DEPFILE",
+                "JOB_POOL",
+            ],
+            multi_value_keywords=[
+                "OUTPUT",
+                "COMMAND",
+                "ARGS",
+                "DEPENDS",
+                "BYPRODUCTS",
+                "IMPLICIT_DEPENDS",
+                "OUTPUT",
+            ],
+        ),
+        "TARGET": dict(
+            options=[
+                "PRE_BUILD",
+                "PRE_LINK",
+                "POST_BUILD",
+                "VERBATIM",
+                "USES_TERMINAL",
+                "COMMAND_EXPAND_LISTS",
+            ],
+            one_value_keywords=["TARGET", "WORKING_DIRECTORY", "COMMENT", "TARGET"],
+            multi_value_keywords=["COMMAND", "ARGS", "BYPRODUCTS"],
+        ),
+    }
+    keyword_formatters = {
+        "COMMAND": "_format_command_line",
+        "ARGS": "_format_command_line",
+    }
 
 
-class Block(ArgumentAwareCommandInvocationDumper):
-    one_value_keywords = ["SCOPE_FOR"]
-    multi_value_keywords = ["PROPAGATE"]
+class AddCustomTarget(CommandLineFormatter, ArgumentAwareCommandInvocationDumper):
+    front_positional_arguments = ["Name", "ALL"]
+    options = ["VERBATIM", "USES_TERMINAL", "COMMAND_EXPAND_LISTS"]
+    one_value_keywords = ["WORKING_DIRECTORY", "COMMENT", "JOB_POOL"]
+    multi_value_keywords = ["COMMAND", "DEPENDS", "BYPRODUCTS", "SOURCES"]
+    keyword_formatters = {"COMMAND": "_format_command_line"}
 
+    def _format_positional_arguments_group(self, group):
+        if len(group) > 1:
+            if group[0].children[0] == "ALL":
+                first, *rest = group
+                return f"{self.visit(first)}\n{super()._format_command_line(rest)}"
+        return super()._format_command_line(group)
 
-class CMakeHostSysteInformation(ArgumentAwareCommandInvocationDumper):
-    one_value_keywords = ["RESULT"]
-    multi_value_keywords = ["QUERY"]
 
+class AddDependencies(ArgumentAwareCommandInvocationDumper):
+    front_positional_arguments = ["<target>"]
 
-class CMakeLanguage(ArgumentAwareCommandInvocationDumper):
-    options = ["DEFER", "EVAL"]
-    one_value_keywords = [
-        "DIRECTORY",
-        "ID",
-        "ID_VAR",
-        "GET_CALL_IDS",
-        "GET_CALL",
-        "SET_DEPENDENCY_PROVIDER",
-        "GET_MESSAGE_LOG_LEVEL",
-    ]
-    multi_value_keywords = ["CALL", "CANCEL_CALL", "SUPPORTED_METHODS"]
 
+class AddExecutable(ArgumentAwareCommandInvocationDumper):
+    two_words_keywords = [("IMPORTED", "GLOBAL")]
+    front_positional_arguments = ["<name>"]
+    options = [
+        "WIN32",
+        "MACOSX_BUNDLE",
+        "EXCLUDE_FROM_ALL",
+        "IMPORTED",
+        "IMPORTED GLOBAL",
+    ]
+    one_value_keywords = ["ALIAS"]
+
+
+class AddLibrary(TwoWordKeywordIsolator, ArgumentAwareCommandInvocationDumper):
+    two_words_keywords = [("IMPORTED", "GLOBAL")]
+    front_positional_arguments = ["<name>"]
+    options = [
+        "STATIC",
+        "SHARED",
+        "MODULE",
+        "EXCLUDE_FROM_ALL",
+        "OBJECT",
+        "IMPORTED",
+        "IMPORTED GLOBAL",
+        "UNKNOWN",
+    ]
+    one_value_keywords = ["ALIAS"]
+    multi_value_keywords = ["INTERFACE"]
+
+
+class AddSubdirectory(ArgumentAwareCommandInvocationDumper):
+    front_positional_arguments = ["source_dir", "binary_dir"]
+    options = ["EXCLUDE_FROM_ALL", "SYSTEM"]
+
+
+class AddTest(CommandLineFormatter, ArgumentAwareCommandInvocationDumper):
+    front_positional_arguments = ["<name>", "<command>"]
+    options = ["COMMAND_EXPAND_LISTS"]
+    one_value_keywords = ["NAME", "WORKING_DIRECTORY"]
+    multi_value_keywords = ["COMMAND", "CONFIGURATIONS"]
+    keyword_formatters = {"COMMAND": "_format_command_line"}
+
+
+class BuildCommand(ArgumentAwareCommandInvocationDumper):
+    front_positional_arguments = ["<variable>"]
+    one_value_keywords = ["CONFIGURATION", "TARGET", "PROJECT_NAME", "PARALLEL_LEVEL"]
 
-class CMakeParseArguments(ArgumentAwareCommandInvocationDumper):
-    one_value_keywords = ["PARSE_ARGV"]
 
+class CreateTestSourcelist(ArgumentAwareCommandInvocationDumper):
+    front_positional_arguments = ["sourceListName", "driverName"]
+    one_value_keywords = ["EXTRA_INCLUDE", "FUNCTION"]
 
-class ConfigureFile(ArgumentAwareCommandInvocationDumper):
+
+class DefineProperty(ArgumentAwareCommandInvocationDumper):
     options = [
-        "COPYONLY",
-        "ESCAPE_QUOTES",
-        "@ONLY",
-        "NO_SOURCE_PERMISSIONS",
-        "USE_SOURCE_PERMISSIONS",
+        "GLOBAL",
+        "DIRECTORY",
+        "TARGET",
+        "SOURCE",
+        "TEST",
+        "VARIABLE",
+        "CACHED_VARIABLE",
+        "INHERITED",
     ]
-    one_value_keywords = ["NEWLINE_STYLE"]
-    multi_value_keywords = ["FILE_PERMISSIONS"]
+    one_value_keywords = ["PROPERTY", "INITIALIZE_FROM_VARIABLE"]
+    multi_value_keywords = ["BRIEF_DOCS", "FULL_DOCS"]
 
 
-class EndBlock(ArgumentAwareCommandInvocationDumper):
-    pass
+class Export(MultipleSignatureCommandInvocationDumper):
+    customized_signatures = {
+        "EXPORT": dict(one_value_keywords=["EXPORT", "NAMESPACE", "FILE"]),
+        "TARGETS": dict(
+            options=["APPEND", "EXPORT_LINK_INTERFACE_LIBRARIES"],
+            one_value_keywords=["NAMESPACE", "FILE", "ANDROID_MK"],
+            multi_value_keywords=["TARGETS"],
+        ),
+        "PACKAGE": dict(one_value_keywords=["PACKAGE"]),
+    }
 
 
-class EndForeach(ArgumentAwareCommandInvocationDumper):
-    pass
+class FtlkWrapUi(ArgumentAwareCommandInvocationDumper):
+    front_positional_arguments = ["resultingLibraryName"]
 
 
-class EndFunction(ArgumentAwareCommandInvocationDumper):
-    pass
+class GetSourceFileProperty(ArgumentAwareCommandInvocationDumper):
+    front_positional_arguments = ["<variable>", "<file>"]
+    back_positional_arguments = ["<property>"]
+    one_value_keywords = ["DIRECTORY", "TARGET_DIRECTORY"]
 
 
-class EndMacro(ArgumentAwareCommandInvocationDumper):
-    pass
+class GetTargetProperty(ArgumentAwareCommandInvocationDumper):
+    front_positional_arguments = ["<VAR>", "target", "property"]
 
 
-class ExecuteProcess(CommandLineFormatter, ArgumentAwareCommandInvocationDumper):
-    options = [
-        "OUTPUT_QUIET",
-        "ERROR_QUIET",
-        "OUTPUT_STRIP_TRAILING_WHITESPACE",
-        "ERROR_STRIP_TRAILING_WHITESPACE",
-        "ECHO_OUTPUT_VARIABLE",
-        "ECHO_ERROR_VARIABLE",
-    ]
-    one_value_keywords = [
-        "WORKING_DIRECTORY",
-        "TIMEOUT",
-        "RESULT_VARIABLE",
-        "RESULTS_VARIABLE",
-        "OUTPUT_VARIABLE",
-        "ERROR_VARIABLE",
-        "INPUT_FILE",
-        "OUTPUT_FILE",
-        "ERROR_FILE",
-        "COMMAND_ECHO",
-        "ENCODING",
-        "COMMAND_ERROR_IS_FATAL",
-    ]
-    multi_value_keywords = ["COMMAND"]
-    keyword_formatters = {"COMMAND": "_format_command_line"}
+class GetTestProperty(ArgumentAwareCommandInvocationDumper):
+    front_positional_arguments = ["<VAR>", "target", "property"]
+
+
+class IncludeDirectories(ArgumentAwareCommandInvocationDumper):
+    options = ["AFTER", "BEFORE", "SYSTEM"]
 
 
-class File(MultipleSignatureCommandInvocationDumper):
+class IncludeExternalMsProject(ArgumentAwareCommandInvocationDumper):
+    front_positional_arguments = ["projectname", "location"]
+    one_value_keywords = ["TYPE", "GUID", "PLATFORM"]
+
+
+class Install(TwoWordKeywordIsolator, MultipleSignatureCommandInvocationDumper):
+    two_words_keywords = [("INCLUDES", "DESTINATION")]
+
     customized_signatures = {
-        # Reading
-        "READ": dict(
-            options=["HEX"],
-            one_value_keywords=["OFFSET", "LIMIT"],
-            multi_value_keywords=["READ"],
-        ),
-        "STRINGS": dict(
-            options=["NEWLINE_CONSUME", "NO_HEX_CONVERSION"],
-            one_value_keywords=[
-                "LENGTH_MAXIMUM",
-                "LENGTH_MINIMUM",
-                "LIMIT_COUNT",
-                "LIMIT_INPUT",
-                "LIMIT_OUTPUT",
-                "REGEX",
-                "ENCODING",
-            ],
-            multi_value_keywords=["STRINGS"],
-        ),
-        "GET_RUNTIME_DEPENDENCIES": dict(
-            one_value_keywords=[
-                "RESOLVED_DEPENDENCIES_VAR",
-                "UNRESOLVED_DEPENDENCIES_VAR",
-                "CONFLICTING_DEPENDENCIES_PREFIX",
-                "BUNDLE_EXECUTABLE",
-            ],
-            multi_value_keywords=[
-                "EXECUTABLES",
-                "LIBRARIES",
-                "MODULES",
-                "DIRECTORIES",
-                "PRE_INCLUDE_REGEXES",
-                "PRE_EXCLUDE_REGEXES",
-                "POST_INCLUDE_REGEXES",
-                "POST_EXCLUDE_REGEXES",
-                "POST_INCLUDE_FILES",
-                "POST_EXCLUDE_FILES",
+        "TARGETS": dict(
+            options=[
+                "ARCHIVE",
+                "LIBRARY",
+                "RUNTIME",
+                "OBJECTS",
+                "FRAMEWORK",
+                "BUNDLE",
+                "PRIVATE_HEADER",
+                "PUBLIC_HEADER",
+                "RESOURCE",
+                "OPTIONAL",
+                "EXCLUDE_FROM_ALL",
+                "NAMELINK_ONLY",
+                "NAMELINK_SKIP",
             ],
-        ),
-        # Writing
-        "GENERATE": dict(
-            options=["NO_SOURCE_PERMISSIONS", "USE_SOURCE_PERMISSIONS"],
             one_value_keywords=[
-                "INPUT",
-                "CONTENT",
-                "CONDITION",
-                "OUTPUT",
-                "TARGET",
-                "NEWLINE_STYLE",
-            ],
-            multi_value_keywords=["FILE_PERMISSIONS"],
-        ),
-        "CONFIGURE": dict(
-            options=["ESCAPE_QUOTES", "@ONLY"],
-            one_value_keywords=["OUTPUT", "CONTENT", "NEWLINE_STYLE"],
-        ),
-        # Filesystem
-        "GLOB": dict(
-            options=["CONFIGURE_DEPENDS"],
-            one_value_keywords=["GLOB", "LIST_DIRECTORIES", "RELATIVE"],
-        ),
-        "GLOB_RECURSE": dict(
-            options=["CONFIGURE_DEPENDS"],
-            one_value_keywords=["GLOB_RECURSE", "LIST_DIRECTORIES", "RELATIVE"],
-        ),
-        "COPY": dict(
-            options=[
-                "NO_SOURCE_PERMISSIONS",
-                "USE_SOURCE_PERMISSIONS",
-                "FOLLOW_SYMLINK_CHAIN",
-                "FILES_MATCHING",
-                "EXCLUDE",
+                "EXPORT",
+                "DESTINATION",
+                "COMPONENT",
+                "NAMELINK_COMPONENT",
+                "RUNTIME_DEPENDENCY_SET",
+                "FILE_SET",
             ],
-            one_value_keywords=["DESTINATION", "PATTERN", "REGEX"],
             multi_value_keywords=[
-                "COPY",
-                "FILE_PERMISSIONS",
-                "DIRECTORY_PERMISSIONS",
+                "TARGETS",
                 "PERMISSIONS",
-            ],
+                "CONFIGURATIONS",
+                "INCLUDES DESTINATION",
+                "RUNTIME_DEPENDENCIES",
+            ],
+        ),
+        "FILES": dict(
+            options=["OPTIONAL", "EXCLUDE_FROM_ALL"],
+            one_value_keywords=["TYPE", "DESTINATION", "COMPONENT", "RENAME"],
+            multi_value_keywords=["FILES", "PERMISSIONS", "CONFIGURATIONS"],
+        ),
+        "PROGRAMS": dict(
+            options=["OPTIONAL", "EXCLUDE_FROM_ALL"],
+            one_value_keywords=["TYPE", "DESTINATION", "COMPONENT", "RENAME"],
+            multi_value_keywords=["PROGRAMS", "PERMISSIONS", "CONFIGURATIONS"],
         ),
-        "COPY_FILE": dict(options=["ONLY_IF_DIFFERENT"], one_value_keywords=["RESULT"]),
-        "INSTALL": dict(
+        "DIRECTORY": dict(
             options=[
-                "NO_SOURCE_PERMISSIONS",
                 "USE_SOURCE_PERMISSIONS",
-                "FOLLOW_SYMLINK_CHAIN",
+                "OPTIONAL",
+                "MESSAGE_NEVER",
+                "EXCLUDE_FROM_ALL",
                 "FILES_MATCHING",
                 "EXCLUDE",
             ],
-            one_value_keywords=["DESTINATION", "PATTERN", "REGEX"],
+            one_value_keywords=["TYPE", "DESTINATION", "COMPONENT", "PATTERN", "REGEX"],
             multi_value_keywords=[
-                "INSTALL",
+                "DIRECTORY",
                 "FILE_PERMISSIONS",
                 "DIRECTORY_PERMISSIONS",
+                "CONFIGURATIONS",
                 "PERMISSIONS",
             ],
         ),
-        "CREATE_LINK": dict(
-            options=["COPY_ON_ERROR", "SYMBOLIC"],
-            one_value_keywords=["RESULT"],
-            multi_value_keywords=["CREATE_LINK"],
+        "SCRIPT": dict(
+            options=["EXCLUDE_FROM_ALL", "ALL_COMPONENTS"],
+            one_value_keywords=["SCRIPT", "COMPONENT"],
+        ),
+        "CODE": dict(
+            options=["EXCLUDE_FROM_ALL", "ALL_COMPONENTS"],
+            one_value_keywords=["CODE", "COMPONENT"],
         ),
-        "CHMOD": dict(
-            multi_value_keywords=[
-                "PERMISSIONS",
-                "FILE_PERMISSIONS",
-                "DIRECTORY_PERMISSIONS",
-            ]
-        ),
-        "CHMOD_RECURSE": dict(
-            multi_value_keywords=[
-                "PERMISSIONS",
-                "FILE_PERMISSIONS",
-                "DIRECTORY_PERMISSIONS",
-            ]
-        ),
-        "RENAME": dict(options=["NO_REPLACE"], one_value_keywords=["RESULT"]),
-        # Path Conversion
-        "REAL_PATH": dict(
-            options=["EXPAND_TILDE"], one_value_keywords=["BASE_DIRECTORY"]
-        ),
-        # Transfer
-        "DOWNLOAD": dict(
-            options=["SHOW_PROGRESS"],
+        "EXPORT": dict(
+            options=["EXPORT_LINK_INTERFACE_LIBRARIES", "EXCLUDE_FROM_ALL"],
             one_value_keywords=[
-                "INACTIVITY_TIMEOUT",
-                "LOG",
-                "STATUS",
-                "TIMEOUT",
-                "USERPWD",
-                "HTTPHEADER",
-                "NETRC",
-                "NETRC_FILE",
-                "EXPECTED_HASH",
-                "EXPECTED_MD5",
-                "TLS_VERIFY",
-                "TLS_CAINFO",
-                "RANGE_START",
-                "RANGE_END",
+                "EXPORT",
+                "DESTINATION",
+                "NAMESPACE",
+                "FILE",
+                "COMPONENT",
             ],
-            multi_value_keywords=["DOWNLOAD"],
+            multi_value_keywords=["PERMISSIONS", "CONFIGURATIONS"],
         ),
-        "UPLOAD": dict(
-            options=["SHOW_PROGRESS"],
-            one_value_keywords=[
-                "INACTIVITY_TIMEOUT",
-                "LOG",
-                "STATUS",
-                "TIMEOUT",
-                "USERPWD",
-                "HTTPHEADER",
-                "NETRC",
-                "NETRC_FILE",
-                "TLS_VERIFY",
-                "TLS_CAINFO",
-            ],
-            multi_value_keywords=["UPLOAD"],
-        ),
-        # Locking
-        "LOCK": dict(
-            options=["DIRECTORY", "RELEASE"],
-            one_value_keywords=["LOCK", "GUARD", "RESULT_VARIABLE", "TIMEOUT"],
-        ),
-        # Archiving
-        "ARCHIVE_CREATE": dict(
-            options=["VERBOSE"],
+        "EXPORT_ANDROID_MK": dict(
+            options=["EXPORT_LINK_INTERFACE_LIBRARIES", "EXCLUDE_FROM_ALL"],
             one_value_keywords=[
-                "OUTPUT",
-                "FORMAT",
-                "COMPRESSION",
-                "COMPRESSION_LEVEL",
-                "MTIME",
-            ],
-            multi_value_keywords=["PATHS"],
-        ),
-        "ARCHIVE_EXTRACT": dict(
-            options=["LIST_ONLY", "VERBOSE"],
-            one_value_keywords=["INPUT", "DESTINATION"],
-            multi_value_keywords=["PATTERNS"],
+                "EXPORT_ANDROID_MK",
+                "DESTINATION",
+                "NAMESPACE",
+                "FILE",
+                "COMPONENT",
+            ],
+            multi_value_keywords=["PERMISSIONS", "CONFIGURATIONS"],
+        ),
+        "IMPORTED_RUNTIME_ARTIFACTS": dict(
+            options=[
+                "LIBRARY",
+                "RUNTIME",
+                "FRAMEWORK",
+                "BUNDLE",
+                "OPTIONAL",
+                "EXCLUDE_FROM_ALL",
+            ],
+            one_value_keywords=["RUNTIME_DEPENDENCY_SET", "DESTINATION", "COMPONENT"],
+            multi_value_keywords=["PERMISSIONS", "CONFIGURATIONS"],
+        ),
+        "RUNTIME_DEPENDENCY_SET": dict(
+            options=["LIBRARY", "RUNTIME", "FRAMEWORK", "OPTIONAL", "EXCLUDE_FROM_ALL"],
+            one_value_keywords=["DESTINATION", "COMPONENT", "NAMELINK_COMPONENT"],
+            multi_value_keywords=[
+                "PERMISSIONS",
+                "CONFIGURATIONS",
+                "PRE_INCLUDE_REGEXES",
+                "PRE_EXCLUDE_REGEXES",
+                "POST_INCLUDE_REGEXES",
+                "POST_EXCLUDE_REGEXES",
+                "POST_INCLUDE_FILES",
+                "POST_EXCLUDE_FILES",
+                "DIRECTORIES",
+            ],
         ),
     }
 
 
-class FindFile(ArgumentAwareCommandInvocationDumper):
-    options = [
-        "NO_DEFAULT_PATH",
-        "NO_PACKAGE_ROOT_PATH",
-        "NO_CMAKE_PATH",
-        "NO_CMAKE_ENVIRONMENT_PATH",
-        "NO_SYSTEM_ENVIRONMENT_PATH",
-        "NO_CMAKE_SYSTEM_PATH",
-        "CMAKE_FIND_ROOT_PATH_BOTH",
-        "ONLY_CMAKE_FIND_ROOT_PATH",
-        "NO_CMAKE_FIND_ROOT_PATH",
-        "REQUIRED",
-        "NO_CMAKE_INSTALL_PREFIX",
-    ]
-    one_value_keywords = ["DOC", "ENV", "VALIDATOR"]
-    multi_value_keywords = ["NAMES", "HINTS", "PATHS", "PATH_SUFFIXES"]
+class LinkDirectories(ArgumentAwareCommandInvocationDumper):
+    options = ["AFTER", "BEFORE"]
 
 
-class FindLibrary(ArgumentAwareCommandInvocationDumper):
-    options = [
-        "NAMES_PER_DIR",
-        "NO_DEFAULT_PATH",
-        "NO_PACKAGE_ROOT_PATH",
-        "NO_CMAKE_PATH",
-        "NO_CMAKE_ENVIRONMENT_PATH",
-        "NO_SYSTEM_ENVIRONMENT_PATH",
-        "NO_CMAKE_SYSTEM_PATH",
-        "CMAKE_FIND_ROOT_PATH_BOTH",
-        "ONLY_CMAKE_FIND_ROOT_PATH",
-        "NO_CMAKE_FIND_ROOT_PATH",
-        "REQUIRED",
-        "NO_CMAKE_INSTALL_PREFIX",
-    ]
-    one_value_keywords = ["DOC", "ENV", "VALIDATOR"]
-    multi_value_keywords = ["NAMES", "HINTS", "PATHS", "PATH_SUFFIXES"]
+class LinkLibraries(ArgumentAwareCommandInvocationDumper):
+    one_value_keywords = ["debug", "optimized", "general"]
 
 
-class FindPackage(ArgumentAwareCommandInvocationDumper):
-    options = [
-        "EXACT",
-        "QUIET",
-        "MODULE",
-        "CONFIG",
-        "NO_MODULE",
-        "NO_POLICY_SCOPE",
-        "NO_DEFAULT_PATH",
-        "NO_PACKAGE_ROOT_PATH",
-        "NO_CMAKE_PATH",
-        "NO_CMAKE_ENVIRONMENT_PATH",
-        "NO_SYSTEM_ENVIRONMENT_PATH",
-        "NO_CMAKE_PACKAGE_REGISTRY",
-        "NO_CMAKE_BUILDS_PATH",
-        "NO_CMAKE_SYSTEM_PATH",
-        "NO_CMAKE_SYSTEM_PACKAGE_REGISTRY",
-        "CMAKE_FIND_ROOT_PATH_BOTH",
-        "ONLY_CMAKE_FIND_ROOT_PATH",
-        "NO_CMAKE_FIND_ROOT_PATH",
-        "NO_CMAKE_INSTALL_PREFIX",
-        "GLOBAL",
-    ]
-    multi_value_keywords = [
-        "REQUIRED",
-        "COMPONENTS",
-        "OPTIONAL_COMPONENTS",
-        "NAMES",
-        "CONFIGS",
-        "HINTS",
-        "PATHS",
-        "PATH_SUFFIXES",
-    ]
+class LoadCache(ArgumentAwareCommandInvocationDumper):
+    front_positional_arguments = ["pathToBuildDirectory"]
+    one_value_keywords = ["READ_WITH_PREFIX"]
+    multi_value_keywords = ["EXCLUDE", "INCLUDE_INTERNALS"]
 
 
-class FindPath(ArgumentAwareCommandInvocationDumper):
-    options = [
-        "NO_DEFAULT_PATH",
-        "NO_PACKAGE_ROOT_PATH",
-        "NO_CMAKE_PATH",
-        "NO_CMAKE_ENVIRONMENT_PATH",
-        "NO_SYSTEM_ENVIRONMENT_PATH",
-        "NO_CMAKE_SYSTEM_PATH",
-        "CMAKE_FIND_ROOT_PATH_BOTH",
-        "ONLY_CMAKE_FIND_ROOT_PATH",
-        "NO_CMAKE_FIND_ROOT_PATH",
-        "REQUIRED",
-        "NO_CMAKE_INSTALL_PREFIX",
-    ]
-    one_value_keywords = ["DOC", "ENV", "VALIDATOR"]
-    multi_value_keywords = ["NAMES", "HINTS", "PATHS", "PATH_SUFFIXES"]
+class Project(ArgumentAwareCommandInvocationDumper):
+    front_positional_arguments = ["<PROJECT-NAME>"]
+    one_value_keywords = ["VERSION", "DESCRIPTION", "HOMEPAGE_URL"]
+    multi_value_keywords = ["LANGUAGES"]
 
 
-class FindProgram(ArgumentAwareCommandInvocationDumper):
-    options = [
-        "NAMES_PER_DIR",
-        "NO_DEFAULT_PATH",
-        "NO_PACKAGE_ROOT_PATH",
-        "NO_CMAKE_PATH",
-        "NO_CMAKE_ENVIRONMENT_PATH",
-        "NO_SYSTEM_ENVIRONMENT_PATH",
-        "NO_CMAKE_SYSTEM_PATH",
-        "CMAKE_FIND_ROOT_PATH_BOTH",
-        "ONLY_CMAKE_FIND_ROOT_PATH",
-        "NO_CMAKE_FIND_ROOT_PATH",
-        "REQUIRED",
-        "NO_CMAKE_INSTALL_PREFIX",
-    ]
-    one_value_keywords = ["DOC", "ENV", "VALIDATOR"]
-    multi_value_keywords = ["NAMES", "HINTS", "PATHS", "PATH_SUFFIXES"]
+class SourceGroup(ArgumentAwareCommandInvocationDumper):
+    front_positional_arguments = ["<name>"]
+    one_value_keywords = ["REGULAR_EXPRESSION", "TREE", "PREFIX"]
+    multi_value_keywords = ["FILES"]
 
 
-class Foreach(ArgumentAwareCommandInvocationDumper):
-    options = ["IN"]
-    multi_value_keywords = ["RANGE", "LISTS", "ITEMS", "ZIP_LISTS"]
+class TargetCompileDefinitions(ArgumentAwareCommandInvocationDumper):
+    front_positional_arguments = ["<target>"]
+    multi_value_keywords = ["INTERFACE", "PUBLIC", "PRIVATE"]
 
 
-class Function(ArgumentAwareCommandInvocationDumper):
-    pass
+class TargetCompileFeatures(ArgumentAwareCommandInvocationDumper):
+    front_positional_arguments = ["<target>"]
+    multi_value_keywords = ["INTERFACE", "PUBLIC", "PRIVATE"]
 
 
-class GetDirectoryProperty(ArgumentAwareCommandInvocationDumper):
-    one_value_keywords = ["DIRECTORY", "DEFINITION"]
+class TargetCompileOptions(ArgumentAwareCommandInvocationDumper):
+    front_positional_arguments = ["<target>"]
+    options = ["BEFORE"]
+    multi_value_keywords = ["INTERFACE", "PUBLIC", "PRIVATE"]
 
 
-class GetFilenameComponent(ArgumentAwareCommandInvocationDumper):
-    options = [
-        "DIRECTORY",
-        "NAME",
-        "EXT",
-        "NAME_WE",
-        "LAST_EXT",
-        "NAME_WLE",
-        "PATH",
-        "PROGRAM",
-        "CACHE",
-    ]
-    one_value_keywords = ["BASE_DIR", "PROGRAM_ARGS"]
+class TargetIncludeDirectories(ArgumentAwareCommandInvocationDumper):
+    front_positional_arguments = ["<target>"]
+    options = ["BEFORE", "SYSTEM", "AFTER"]
+    multi_value_keywords = ["INTERFACE", "PUBLIC", "PRIVATE"]
 
 
-class GetProperty(ArgumentAwareCommandInvocationDumper):
-    options = ["GLOBAL", "VARIABLE", "SET", "DEFINED", "BRIEF_DOCS", "FULL_DOCS"]
-    one_value_keywords = ["TARGET", "INSTALL", "TEST", "CACHE", "PROPERTY"]
-    multi_value_keywords = ["DIRECTORY", "SOURCE"]
+class TargetLinkDirectories(ArgumentAwareCommandInvocationDumper):
+    front_positional_arguments = ["<target>"]
+    options = ["BEFORE"]
+    multi_value_keywords = ["INTERFACE", "PUBLIC", "PRIVATE"]
 
 
-class GetSourceFileProperty(ArgumentAwareCommandInvocationDumper):
-    one_value_keywords = ["DIRECTORY", "TARGET_DIRECTORY"]
+class TargetLinkOptions(ArgumentAwareCommandInvocationDumper):
+    front_positional_arguments = ["<target>"]
+    options = ["BEFORE"]
+    multi_value_keywords = ["INTERFACE", "PUBLIC", "PRIVATE"]
 
 
-class Include(ArgumentAwareCommandInvocationDumper):
-    options = ["OPTIONAL", "NO_POLICY_SCOPE"]
-    one_value_keywords = ["RESULT_VARIABLE"]
+class TargetPrecompileHeaders(ArgumentAwareCommandInvocationDumper):
+    front_positional_arguments = ["<target>"]
+    one_value_keywords = ["REUSE_FROM"]
+    multi_value_keywords = ["INTERFACE", "PUBLIC", "PRIVATE"]
 
 
-class List(MultipleSignatureCommandInvocationDumper):
-    customized_signatures = {
-        # Modification
-        "FILTER": dict(
-            options=["INCLUDE", "EXCLUDE"], one_value_keywords=["FILTER", "REGEX"]
-        ),
-        "REMOVE_DUPLICATES": dict(one_value_keywords=["REMOVE_DUPLICATES"]),
-        "TRANSFORM": dict(
-            one_value_keywords=["OUTPUT_VARIABLE"],
-            multi_value_keywords=[
-                "TRANSFORM",
-                "APPEND",
-                "PREPEND",
-                "TOLOWER",
-                "TOUPPER",
-                "STRIP",
-                "GENEX_STRIP",
-                "REPLACE",
-            ],
-        ),
-        # Ordering
-        "SORT": dict(one_value_keywords=["SORT", "COMPARE", "CASE", "ORDER"]),
+class TargetSources(SectionAwareCommandInvocationDumper):
+    front_positional_arguments = ["<target>"]
+    multi_value_keywords = ["INTERFACE", "PUBLIC", "PRIVATE"]
+    sections = {
+        "INTERFACE": {
+            "one_value_keywords": ["FILE_SET", "TYPE"],
+            "multi_value_keywords": ["BASE_DIRS", "FILES"],
+        },
+        "PUBLIC": {
+            "one_value_keywords": ["FILE_SET", "TYPE"],
+            "multi_value_keywords": ["BASE_DIRS", "FILES"],
+        },
+        "PRIVATE": {
+            "one_value_keywords": ["FILE_SET", "TYPE"],
+            "multi_value_keywords": ["BASE_DIRS", "FILES"],
+        },
     }
 
 
-class Macro(ArgumentAwareCommandInvocationDumper):
-    pass
-
-
-class MarkAsAdvanced(ArgumentAwareCommandInvocationDumper):
-    options = ["CLEAR", "FORCE"]
-
-
-class Math(ArgumentAwareCommandInvocationDumper):
-    one_value_keywords = ["OUTPUT_FORMAT"]
-    multi_value_keywords = ["EXPR"]
-
-
-class Message(ArgumentAwareCommandInvocationDumper):
-    options = [
-        "FATAL_ERROR",
-        "SEND_ERROR",
-        "WARNING",
-        "AUTHOR_WARNING",
-        "DEPRECATION",
-        "NOTICE",
-        "STATUS",
-        "VERBOSE",
-        "DEBUG",
-        "TRACE",
-        "CHECK_START",
-        "CHECK_PASS",
-        "CHECK_FAIL",
-        "CONFIGURE_LOG",
+class TryCompile(ArgumentAwareCommandInvocationDumper):
+    front_positional_arguments = [
+        "<compileResultVar>",
+        "<bindir>",
+        "<srcdir>",  # or "<srcfile>"
+        "<projectName>",
+        "<targetName>",
+    ]
+    option = ["NO_CACHE", "NO_LOG"]
+    one_value_keywords = [
+        "OUTPUT_VARIABLE",
+        "COPY_FILE",
+        "COPY_FILE_ERROR",
+        "C_STANDARD",
+        "C_STANDARD_REQUIRED",
+        "C_EXTENSIONS",
+        "CXX_STANDARD",
+        "CXX_STANDARD_REQUIRED",
+        "CXX_EXTENSIONS",
+        "OBJC_STANDARD",
+        "OBJC_STANDARD_REQUIRED",
+        "OBJC_EXTENSIONS",
+        "OBJCXX_STANDARD",
+        "OBJCXX_STANDARD_REQUIRED",
+        "OBJCXX_EXTENSIONS",
+        "CUDA_STANDARD",
+        "CUDA_STANDARD_REQUIRED",
+        "CUDA_EXTENSIONS",
+        "PROJECT",
+        "SOURCE_DIR",
+        "BINARY_DIR",
+        "TARGET",
+        "LOG_DESCRIPTION",
+    ]
+    multi_value_keywords = [
+        "SOURCES",
+        "CMAKE_FLAGS",
+        "COMPILE_DEFINITIONS",
+        "LINK_OPTIONS",
+        "LINK_LIBRARIES",
+        "SOURCE_FROM_CONTENT",
+        "SOURCE_FROM_VAR",
+        "SOURCE_FROM_FILE",
     ]
 
 
-class Return(ArgumentAwareCommandInvocationDumper):
-    multi_value_keywords = ["PROPAGATE"]
-
-
-class SeparateArguments(ArgumentAwareCommandInvocationDumper):
-    options = ["PROGRAM", "SEPARATE_ARGS"]
+class TryRun(ArgumentAwareCommandInvocationDumper):
+    front_positional_arguments = [
+        "<runResultVar>",
+        "<compileResultVar>",
+        "<bindir>",
+        "<srcfile>",
+    ]
+    options = ["NO_CACHE", "NO_LOG"]
+    one_value_keywords = [
+        "COMPILE_OUTPUT_VARIABLE",
+        "RUN_OUTPUT_VARIABLE",
+        "OUTPUT_VARIABLE",
+        "WORKING_DIRECTORY",
+        "COPY_FILE",
+        "COPY_FILE_ERROR",
+        "C_STANDARD",
+        "C_STANDARD_REQUIRED",
+        "C_EXTENSIONS",
+        "CXX_STANDARD",
+        "CXX_STANDARD_REQUIRED",
+        "CXX_EXTENSIONS",
+        "OBJC_STANDARD",
+        "OBJC_STANDARD_REQUIRED",
+        "OBJC_EXTENSIONS",
+        "OBJCXX_STANDARD",
+        "OBJCXX_STANDARD_REQUIRED",
+        "OBJCXX_EXTENSIONS",
+        "CUDA_STANDARD",
+        "CUDA_STANDARD_REQUIRED",
+        "CUDA_EXTENSIONS",
+        "RUN_OUTPUT_VARIABLE",
+        "RUN_OUTPUT_STDOUT_VARIABLE",
+        "RUN_OUTPUT_STDERR_VARIABLE",
+        "LOG_DESCRIPTION",
+    ]
+    multi_value_keywords = [
+        "CMAKE_FLAGS",
+        "COMPILE_DEFINITIONS",
+        "LINK_OPTIONS",
+        "LINK_LIBRARIES",
+        "ARGS",
+        "SOURCES",
+        "SOURCE_FROM_CONTENT",
+        "SOURCE_FROM_VAR",
+        "SOURCE_FROM_FILE",
+    ]
 
 
-class SetProperty(ArgumentAwareCommandInvocationDumper):
-    options = ["GLOBAL", "APPEND", "APPEND_STRING"]
-    one_value_keywords = ["DIRECTORY"]
-    multi_value_keywords = ["TARGET", "SOURCE", "INSTALL", "TEST", "CACHE", "PROPERTY"]
+class SetSourceFilesProperties(
+    KeywordWithPairsFormatter, ArgumentAwareCommandInvocationDumper
+):
+    multi_value_keywords = ["PROPERTIES", "DIRECTORY", "TARGET_DIRECTORY"]
+    keyword_formatters = {"PROPERTIES": "_format_keyword_with_pairs"}
 
 
-class String(MultipleSignatureCommandInvocationDumper):
-    customized_signatures = {
-        # Search and Replace
-        "FIND": dict(options=["REVERSE"], multi_value_keywords=["FIND"]),
-        # Regular Expressions
-        "REGEX": dict(one_value_keywords=["REGEX"]),
-        # Comparison
-        "COMPARE": dict(one_value_keywords=["COMPARE"]),
-        # Generation
-        "CONFIGURE": dict(
-            options=["@ONLY", "ESCAPE_QUOTES"], multi_value_keywords=["CONFIGURE"]
-        ),
-        "RANDOM": dict(one_value_keywords=["LENGTH", "ALPHABET", "RANDOM_SEED"]),
-        "UUID": dict(
-            options=["UPPER"], one_value_keywords=["UUID", "NAMESPACE", "NAME", "TYPE"]
-        ),
-        # JSON
-        "JSON": dict(
-            one_value_keywords=[
-                "ERROR_VARIABLE",
-                "GET",
-                "TYPE",
-                "MEMBER",
-                "LENGTH",
-                "REMOVE",
-                "SET",
-            ],
-            multi_value_keywords=["EQUAL"],
-        ),
-    }
+class SetTargetProperties(
+    KeywordWithPairsFormatter, ArgumentAwareCommandInvocationDumper
+):
+    multi_value_keywords = ["PROPERTIES"]
+    keyword_formatters = {"PROPERTIES": "_format_keyword_with_pairs"}
 
 
-class SetDirectoryProperties(
+class SetTestsProperties(
     KeywordWithPairsFormatter, ArgumentAwareCommandInvocationDumper
 ):
     multi_value_keywords = ["PROPERTIES"]
     keyword_formatters = {"PROPERTIES": "_format_keyword_with_pairs"}
 
 
-scripting_command_mapping = {
-    "block": Block,
-    "cmake_host_system_information": CMakeHostSysteInformation,
-    "cmake_language": CMakeLanguage,
-    "cmake_parse_arguments": CMakeParseArguments,
-    "configure_file": ConfigureFile,
-    "elseif": ConditionSyntaxCommandInvocationDumper,
-    "else": ConditionSyntaxCommandInvocationDumper,
-    "endif": ConditionSyntaxCommandInvocationDumper,
-    "endblock": EndBlock,
-    "endforeach": EndForeach,
-    "endfunction": EndFunction,
-    "endmacro": EndMacro,
-    "endwhile": ConditionSyntaxCommandInvocationDumper,
-    "execute_process": ExecuteProcess,
-    "file": File,
-    "find_file": FindFile,
-    "find_library": FindLibrary,
-    "find_package": FindPackage,
-    "find_path": FindPath,
-    "find_program": FindProgram,
-    "foreach": Foreach,
-    "function": Function,
-    "get_directory_property": GetDirectoryProperty,
-    "get_filename_component": GetFilenameComponent,
-    "get_property": GetProperty,
+project_command_mapping = {
+    "add_custom_command": AddCustomCommand,
+    "add_custom_target": AddCustomTarget,
+    "add_dependencies": AddDependencies,
+    "add_executable": AddExecutable,
+    "add_library": AddLibrary,
+    "add_subdirectory": AddSubdirectory,
+    "add_test": AddTest,
+    "build_command": BuildCommand,
+    "create_test_sourcelist": CreateTestSourcelist,
+    "define_property": DefineProperty,
+    "export": Export,
+    "fltk_wrap_ui": FtlkWrapUi,
     "get_source_file_property": GetSourceFileProperty,
-    "if": ConditionSyntaxCommandInvocationDumper,
-    "include": Include,
-    "list": List,
-    "macro": Macro,
-    "mark_as_advanced": MarkAsAdvanced,
-    "math": Math,
-    "message": Message,
-    "return": Return,
-    "separate_arguments": SeparateArguments,
-    "set_directory_properties": SetDirectoryProperties,
-    "set_property": SetProperty,
-    "set": Set,
-    "string": String,
-    "while": ConditionSyntaxCommandInvocationDumper,
+    "get_target_property": GetTargetProperty,
+    "get_test_property": GetTestProperty,
+    "include_directories": IncludeDirectories,
+    "include_external_msproject": IncludeExternalMsProject,
+    "install": Install,
+    "link_directories": LinkDirectories,
+    "link_libraries": LinkLibraries,
+    "load_cache": LoadCache,
+    "project": Project,
+    "source_group": SourceGroup,
+    "set_source_files_properties": SetSourceFilesProperties,
+    "set_target_properties": SetTargetProperties,
+    "set_tests_properties": SetTestsProperties,
+    "target_compile_definitions": TargetCompileDefinitions,
+    "target_compile_features": TargetCompileFeatures,
+    "target_compile_options": TargetCompileOptions,
+    "target_include_directories": TargetIncludeDirectories,
+    "target_link_directories": TargetLinkDirectories,
+    "target_link_libraries": TargetLinkLibraries,
+    "target_link_options": TargetLinkOptions,
+    "target_precompile_headers": TargetPrecompileHeaders,
+    "target_sources": TargetSources,
+    "try_compile": TryCompile,
+    "try_run": TryRun,
 }
```

### Comparing `gersemi-0.8.3/gersemi/command_invocation_dumpers/section_aware_command_invocation_dumper.py` & `gersemi-0.9.0/gersemi/command_invocation_dumpers/section_aware_command_invocation_dumper.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.8.3/gersemi/command_invocation_dumpers/target_link_libraries_command_dumper.py` & `gersemi-0.9.0/gersemi/command_invocation_dumpers/target_link_libraries_command_dumper.py`

 * *Files 19% similar despite different names*

```diff
@@ -24,14 +24,15 @@
                 new_children += [one_behind]
         else:
             new_children += [item for item in [current] if item is not None]
         return Tree("arguments", new_children)
 
 
 class TargetLinkLibraries(ArgumentAwareCommandInvocationDumper):
+    front_positional_arguments = ["<target>"]
     multi_value_keywords = [
         "INTERFACE",
         "PUBLIC",
         "PRIVATE",
         "LINK_PRIVATE",
         "LINK_PUBLIC",
         "LINK_INTERFACE_LIBRARIES",
@@ -40,10 +41,16 @@
     def specified_item(self, tree):
         specifier, item = tree.children
         formatted_specifier = self.visit(specifier)
         with self.not_indented():
             formatted_item = self.visit(item)
         return f"{formatted_specifier} {formatted_item}"
 
+    def _split_arguments(self, arguments):
+        preprocessed = IsolateConfigurationTypeAndItem().transform(
+            Tree("arguments", arguments)
+        )
+        return super()._split_arguments(preprocessed.children)
+
     def arguments(self, tree):
         preprocessed = IsolateConfigurationTypeAndItem().transform(tree)
         return super().arguments(preprocessed)
```

### Comparing `gersemi-0.8.3/gersemi/command_line_formatter.py` & `gersemi-0.9.0/gersemi/command_line_formatter.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.8.3/gersemi/configuration.py` & `gersemi-0.9.0/gersemi/configuration.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 from contextlib import contextmanager
 from dataclasses import asdict, dataclass, fields
+from enum import Enum
 from hashlib import sha1
 from itertools import chain
 import os
 from pathlib import Path
 from typing import Iterable, Optional
 import yaml
 
 
+class ListExpansion(Enum):
+    FavourInlining = "favour-inlining"
+    FavourExpansion = "favour-expansion"
+
+
 @dataclass
 class Configuration:
     line_length: int = 80
     unsafe: bool = False
     quiet: bool = False
     color: bool = False
     definitions: Iterable[Path] = tuple()
+    list_expansion: ListExpansion = ListExpansion.FavourInlining
 
     def summary(self):
         hasher = sha1()
         hasher.update(repr(self).encode("utf-8"))
         return hasher.hexdigest()
 
 
 def make_default_configuration_file():
     default_configuration = Configuration()
-    return yaml.safe_dump(asdict(default_configuration))
+    d = asdict(default_configuration)
+    d["list_expansion"] = d["list_expansion"].value
+    return yaml.safe_dump(d)
 
 
 def find_common_parent_path(paths: Iterable[Path]) -> Path:
     return Path(os.path.commonpath([path.absolute() for path in paths]))
 
 
 def find_dot_gersemirc(paths: Iterable[Path]) -> Optional[Path]:
@@ -53,31 +62,49 @@
         os.chdir(original)
 
 
 def normalize_definitions(definitions):
     return [Path(d).resolve() for d in definitions]
 
 
+def sanitize_list_expansion(list_expansion):
+    legal_values = [e.value for e in ListExpansion]
+    if list_expansion in legal_values:
+        return ListExpansion(list_expansion)
+    raise RuntimeError(
+        f"Unsupported list_expansion: '{list_expansion}'. Legal values: {', '.join(legal_values)}"
+    )
+
+
 def load_configuration_from_file(configuration_file_path: Path) -> Configuration:
     with enter_directory(configuration_file_path.parent):
         with open(configuration_file_path, "r", encoding="utf-8") as f:
             config = yaml.safe_load(f.read())
             if "definitions" in config:
                 config["definitions"] = normalize_definitions(config["definitions"])
+            if "list_expansion" in config:
+                config["list_expansion"] = sanitize_list_expansion(
+                    config["list_expansion"]
+                )
         return Configuration(**config)
 
 
 def override_configuration_with_args(
     configuration: Configuration, args
 ) -> Configuration:
     parameters = [field.name for field in fields(Configuration)]
     for param in parameters:
         value = getattr(args, param)
-        if value:
-            setattr(configuration, param, value)
+        if not value:
+            continue
+        if param == "definitions":
+            value = normalize_definitions(value)
+        if param == "list_expansion":
+            value = sanitize_list_expansion(value)
+        setattr(configuration, param, value)
     return configuration
 
 
 def make_configuration(args) -> Configuration:
     configuration_file_path = find_dot_gersemirc(args.sources)
     if configuration_file_path is not None:
         result = load_configuration_from_file(configuration_file_path)
```

### Comparing `gersemi-0.8.3/gersemi/custom_command_definition_finder.py` & `gersemi-0.9.0/gersemi/custom_command_definition_finder.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,18 @@
         self.stack[name] = [
             item for value in values for item in self._eval_variables(value)
         ]
 
     def _new_command(self, arguments):
         if len(arguments.children) > 0:
             name = arguments.children[0]
-            return self.visit(name)
+            positional_arguments = arguments.children[1:]
+            return self.visit(name), list(
+                map(str, map(self.visit, positional_arguments))
+            )
         raise RuntimeError
 
     def _cmake_parse_arguments(self, arguments):
         if is_parse_argv(arguments.children[0]):
             keywords = arguments.children[3:6]
         else:
             keywords = arguments.children[1:4]
@@ -84,23 +87,24 @@
 
     def block(self, tree):
         if self._should_definition_be_ignored(tree):
             return
 
         subinterpreter = self._inner_scope
         block_begin, *body, _ = subinterpreter.visit_children(tree)
-        name, *_ = block_begin
-        if name is None:
+        command_node, *_ = block_begin
+        if command_node is None:
             return
+        name, positional_arguments = command_node
 
         keywords, *_ = body
         if len(keywords) > 0:
-            self.found_commands[name.lower()] = keywords[0]
+            self.found_commands[name.lower()] = positional_arguments, keywords[0]
         else:
-            self.found_commands[name.lower()] = Keywords()
+            self.found_commands[name.lower()] = positional_arguments, Keywords()
 
     def block_body(self, tree):
         return [
             item for item in self.visit_children(tree) if isinstance(item, Keywords)
         ][:1]
 
     def command_invocation(self, tree):
```

### Comparing `gersemi-0.8.3/gersemi/exceptions.py` & `gersemi-0.9.0/gersemi/exceptions.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.8.3/gersemi/keyword_with_pairs_formatter.py` & `gersemi-0.9.0/gersemi/keyword_with_pairs_formatter.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.8.3/gersemi/parser.py` & `gersemi-0.9.0/gersemi/parser.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.8.3/gersemi/parsing_transformer.py` & `gersemi-0.9.0/gersemi/parsing_transformer.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.8.3/gersemi/postprocessor.py` & `gersemi-0.9.0/gersemi/postprocessor.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.8.3/gersemi/result.py` & `gersemi-0.9.0/gersemi/result.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.8.3/gersemi/runner.py` & `gersemi-0.9.0/gersemi/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,14 +158,15 @@
         custom_command_definitions = find_all_custom_command_definitions(
             set(configuration.definitions), pool
         )
         formatter = create_formatter(
             not configuration.unsafe,
             configuration.line_length,
             custom_command_definitions,
+            configuration.list_expansion,
         )
         execute = partial(run_task, formatter=formatter, task=task)
 
         results = [
             consume_task_result(result)
             for result in pool.imap_unordered(
                 execute, files_to_format, chunksize=CHUNKSIZE
```

### Comparing `gersemi-0.8.3/gersemi/sanity_checker.py` & `gersemi-0.9.0/gersemi/sanity_checker.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.8.3/gersemi/tasks/check_formatting.py` & `gersemi-0.9.0/gersemi/tasks/check_formatting.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.8.3/gersemi/tasks/format_file.py` & `gersemi-0.9.0/gersemi/tasks/format_file.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.8.3/gersemi/tasks/rewrite_in_place.py` & `gersemi-0.9.0/gersemi/tasks/rewrite_in_place.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.8.3/gersemi/tasks/show_diff.py` & `gersemi-0.9.0/gersemi/tasks/show_diff.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.8.3/gersemi/utils.py` & `gersemi-0.9.0/gersemi/utils.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.8.3/gersemi.egg-info/PKG-INFO` & `gersemi-0.9.0/gersemi.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gersemi
-Version: 0.8.3
+Version: 0.9.0
 Summary: A formatter to make your CMake code the real treasure
 Home-page: https://github.com/BlankSpruce/gersemi
 Author: Blank Spruce
 Author-email: blankspruce@protonmail.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -37,14 +37,15 @@
 ```
 
 ## Usage
 
 ```
 usage: gersemi [-c] [-i] [--diff] [--default-config] [--version] [-h] [-l INTEGER]
                [--unsafe] [-q] [--color] [--definitions src [src ...]]
+               [--list-expansion {favour-inlining,favour-expansion}]
                [src ...]
 
 A formatter to make your CMake code the real treasure.
 
 positional arguments:
   src                   File or directory to format. If only - is provided input is taken
                         from stdin instead
@@ -71,14 +72,23 @@
   --color               If --diff is selected showed diff is colorized
   --definitions src [src ...]
                         Files or directories containing custom command definitions
                         (functions or macros). If only - is provided custom definitions, if
                         there are any, are taken from stdin instead. Commands from not
                         deprecated CMake native modules don't have to be provided (check
                         https://cmake.org/cmake/help/latest/manual/cmake-modules.7.html)
+  --list-expansion {favour-inlining,favour-expansion}
+                        Switch controls how code is expanded into multiple lines when it's
+                        not possible to keep it formatted in one line. With 'favour-
+                        inlining' (default) the list of entities will be formatted in such
+                        way that sublists might still be formatted into single line as long
+                        as it's possible. With 'favour-expansion' the list of entities will
+                        be formatted in such way that sublists will be completely expanded
+                        once expansion becomes necessary at all.
+
 ```
 
 ### [pre-commit](https://pre-commit.com/) hook
 
 You can use gersemi with a pre-commit hook by adding the following to `.pre-commit-config.yaml` of your repository:
 ```yaml
 repos:
@@ -92,16 +102,19 @@
 
 ## Formatting
 
 The key goal is for the tool to "just work" and to have as little configuration as possible so that you don't have to worry about fine-tuning formatter to your needs - as long as you embrace the `gersemi` style of formatting, similarly as `black` or `gofmt` do their job. Currently only line length can be changed with `80` as default value. Currently the basic assumption is that code to format is valid CMake language code - `gersemi` might be able to format some particular cases of invalid code but it's not guaranteed and it shouldn't be relied upon. Moreover only commands from CMake 3.0 onwards are supported and will be formatted properly - for instance [`exec_program` has been deprecated since CMake 3.0](https://cmake.org/cmake/help/latest/command/exec_program.html) so it won't be formatted. Be warned though it's not production ready so the changes to code might be destructive and you should always have a backup (version control helps a lot).
 
 ### Style
 
-Here's an example of `gersemi` style of formatting:
+#### Default style `favour-inlining`
+
+`gersemi` will try to format the code in a way that respects set character limit for single line and only break line whenever necessary.
 
+Example:
 ```cmake
 cmake_minimum_required(VERSION 3.18 FATAL_ERROR)
 project(example CXX)
 
 message(STATUS "This is example project")
 message(
     STATUS
@@ -213,14 +226,162 @@
     COMMAND
         cmake -E echo "something quite a bit                           longer"
     WORKING_DIRECTORY ${CMAKE_CURRENT_BINARY_DIR}/something
     DEPENDS
         ${CMAKE_CURRENT_SOURCE_DIR}/something
         ${CMAKE_CURRENT_SOURCE_DIR}/something_else
     COMMENT "example custom command"
+)
+```
+
+#### Alternative style `favour-expansion`
+
+In this style lines are broken in one of these cases:
+- there is at least one multi-value argument present a single command invocation, either keyworded one like `PUBLIC` in `target_link_libraries` or standalone one like list of files in `add_library`, which has more than one value
+- there are more than one multi-value arguments present in the command invocation like `target_link_libraries` with `PUBLIC` and `PRIVATE` arguments.
+- character limit for single line is reached
+
+One-value arguments (like `NAME` in `add_test`) will be inlined unless that'd violate character limit. Structure or control flow commands (`if`, `while`, `function`, `foreach` etc.) are exempted from these special rules and follow the same formatting as `favour-inlining`. This style is more merge or `git blame` friendly because usually multi-value arguments are changed one element at a time and with this style such change will be visible as one line of code per element.
+
+Example:
+```cmake
+cmake_minimum_required(VERSION 3.18 FATAL_ERROR)
+project(example CXX)
+
+message(STATUS "This is example project")
+message(
+    STATUS
+    "Here is yet another but much much longer message that should be displayed"
+)
+
+# project version
+set(VERSION_MAJOR 0)
+set(VERSION_MINOR 1)
+set(VERSION_PATCH 0)
+
+add_compile_options(
+    -Wall
+    -Wpedantic
+    -fsanitize=address
+    -fconcepts
+    -fsomething-else
+)
+
+if(NOT ${SOME_OPTION})
+    add_compile_options(-Werror)
+endif()
+
+# foobar library
+add_library(foobar)
+add_library(example::foobar ALIAS foobar)
+
+target_sources(
+    foobar
+    PUBLIC
+        include/some_subdirectory/header.hpp
+        include/another_subdirectory/header.hpp
+    PRIVATE
+        src/some_subdirectory/src1.cpp
+        src/some_subdirectory/src1.cpp
+        src/another_subdirectory/src1.cpp
+        src/another_subdirectory/src2.cpp
+        src/another_subdirectory/src3.cpp
+)
+
+target_include_directories(
+    foobar
+    INTERFACE
+        $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/include>
+        $<INSTALL_INTERFACE:include>
+)
+
+target_link_libraries(
+    foobar
+    PUBLIC
+        example::dependency_one
+        example::dependency_two
+    PRIVATE
+        example::some_util
+        external::some_lib
+        external::another_lib
+        Boost::Boost
+)
+
+include(GNUInstallDirs)
+set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/${CMAKE_INSTALL_LIBDIR})
+set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/${CMAKE_INSTALL_LIBDIR})
+set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/${CMAKE_INSTALL_BINDIR})
+
+# example executable
+add_executable(app main.cpp)
+target_link_libraries(
+    app
+    PRIVATE
+        example::foobar
+        Boost::Boost
+)
+
+# tests
+include(CTest)
+include(GTest)
+enable_testing()
+add_subdirectory(tests)
+
+# some helper function - see more details in "Let's make a deal" section
+function(add_test_executable)
+    set(OPTIONS
+        QUIET
+        VERBOSE
+        SOME_PARTICULARLY_LONG_KEYWORD_THAT_ENABLES_SOMETHING
+    )
+    set(ONE_VALUE_ARGS
+        NAME
+        TESTED_TARGET
+    )
+    set(MULTI_VALUE_ARGS
+        SOURCES
+        DEPENDENCIES
+    )
+
+    cmake_parse_arguments(
+        THIS_FUNCTION_PREFIX
+        ${OPTIONS}
+        ${ONE_VALUE_ARGS}
+        ${MULTI_VALUE_ARGS}
+    )
+    # rest of the function
+endfunction()
+
+add_test_executable(
+    NAME foobar_tests
+    TESTED_TARGET foobar
+    SOURCES
+        some_test1.cpp
+        some_test2.cpp
+        some_test3.cpp
+        some_test4.cpp
+        some_test5.cpp
+    QUIET
+    DEPENDENCIES googletest::googletest
+)
+
+add_custom_command(
+    OUTPUT
+        ${SOMETHING_TO_OUTPUT}
+    COMMAND
+        ${CMAKE_COMMAND} -E cat foobar
+    COMMAND
+        cmake -E echo foobar
+    COMMAND
+        cmake -E echo "something quite a bit                           longer"
+    WORKING_DIRECTORY ${CMAKE_CURRENT_BINARY_DIR}/something
+    DEPENDS
+        ${CMAKE_CURRENT_SOURCE_DIR}/something
+        ${CMAKE_CURRENT_SOURCE_DIR}/something_else
+    COMMENT "example custom command"
 )
 ```
 
 ### Let's make a deal
 
 It's possible to provide reasonable formatting for custom commands. However on language level there are no hints available about supported keywords for given command so `gersemi` has to generate specialized formatter. To do that custom command definition is necessary which should be provided with `--definitions`. There are limitations though since it'd probably require full-blown CMake language interpreter to do it in every case so let's make a deal: if your custom command definition (function or macro) uses `cmake_parse_arguments` and does it in obvious manner such specialized formatter will be generated. For instance this definition is okay (you can find other examples in `tests/custom_command_formatting/`):
 ```cmake
```

### Comparing `gersemi-0.8.3/gersemi.egg-info/SOURCES.txt` & `gersemi-0.9.0/gersemi.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -37,24 +37,23 @@
 gersemi.egg-info/entry_points.txt
 gersemi.egg-info/requires.txt
 gersemi.egg-info/top_level.txt
 gersemi/command_invocation_dumpers/__init__.py
 gersemi/command_invocation_dumpers/argument_aware_command_invocation_dumper.py
 gersemi/command_invocation_dumpers/condition_syntax_command_invocation_dumper.py
 gersemi/command_invocation_dumpers/ctest_command_dumpers.py
-gersemi/command_invocation_dumpers/install_command_dumper.py
 gersemi/command_invocation_dumpers/module_command_dumpers.py
 gersemi/command_invocation_dumpers/multiple_signature_command_invocation_dumper.py
 gersemi/command_invocation_dumpers/preserving_command_invocation_dumper.py
 gersemi/command_invocation_dumpers/project_command_dumpers.py
 gersemi/command_invocation_dumpers/scripting_command_dumpers.py
 gersemi/command_invocation_dumpers/section_aware_command_invocation_dumper.py
-gersemi/command_invocation_dumpers/set_command.py
 gersemi/command_invocation_dumpers/specialized_dumpers.py
 gersemi/command_invocation_dumpers/target_link_libraries_command_dumper.py
+gersemi/command_invocation_dumpers/two_word_keyword_isolator.py
 gersemi/tasks/__init__.py
 gersemi/tasks/check_formatting.py
 gersemi/tasks/format_file.py
 gersemi/tasks/forward_to_stdout.py
 gersemi/tasks/rewrite_in_place.py
 gersemi/tasks/show_diff.py
 tests/test_custom_command_dumper_generation.py
```

### Comparing `gersemi-0.8.3/setup.py` & `gersemi-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.8.3/tests/test_custom_command_dumper_generation.py` & `gersemi-0.9.0/tests/test_custom_command_dumper_generation.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.8.3/tests/test_custom_command_formatting.py` & `gersemi-0.9.0/tests/test_custom_command_formatting.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.8.3/tests/test_executable.py` & `gersemi-0.9.0/tests/test_executable.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,16 @@
 def temporary_dir_copies(directory_paths):
     with ExitStack() as stack:
         copies = [stack.enter_context(temporary_dir_copy(p)) for p in directory_paths]
         yield copies
 
 
 def assert_success(*args, **kwargs):
-    assert gersemi(*args, **kwargs).returncode == 0
+    process = gersemi(*args, **kwargs)
+    assert process.returncode == 0, (process.stdout, process.stderr)
 
 
 def assert_fail(*args, **kwargs):
     assert gersemi(*args, **kwargs).returncode == 1
 
 
 def compare_directories(left, right):
```

### Comparing `gersemi-0.8.3/tests/test_formatter.py` & `gersemi-0.9.0/tests/test_formatter.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import pytest
 from gersemi.exceptions import ASTMismatch
 from gersemi.sanity_checker import check_code_equivalence
 from .tests_generator import generate_input_output_tests
 
 
-def test_formatter(formatter, case):
+def test_formatter(formatter_creator, case):
+    formatter = formatter_creator(case.config)
     assert formatter.format(case.given) == case.expected
 
 
-def test_formatter_idempotence(formatter, case):
+def test_formatter_idempotence(formatter_creator, case):
+    formatter = formatter_creator(case.config)
     formatted_once = formatter.format(case.given)
     formatted_twice = formatter.format(formatted_once)
     assert formatted_once == formatted_twice
 
 
 def test_abstract_syntax_tree_equivalence(parser, parser_with_simple_grammar, case):
     for p in [parser, parser_with_simple_grammar]:
```

### Comparing `gersemi-0.8.3/tests/test_parser.py` & `gersemi-0.9.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.8.3/tests/tests_generator.py` & `gersemi-0.9.0/tests/tests_generator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import collections
 import os
 import pathlib
+import yaml
 
 
 InputOnlyCase = collections.namedtuple("InputOnlyCase", ["name", "content"])
 InputOutputCase = collections.namedtuple(
-    "InputOutputCase", ["name", "given", "expected"]
+    "InputOutputCase", ["name", "given", "expected", "config"]
 )
 
 
 def has_extension(expected_extension):
     def verify(filename):
         extension = "".join(pathlib.Path(filename).suffixes)
         return extension == expected_extension
@@ -55,18 +56,28 @@
 
 def get_matching_output_filename(input_filename, output_extension):
     return f"{remove_extension(input_filename)}{output_extension}"
 
 
 def make_input_output_case(input_filename, output_extension, where):
     output_filename = get_matching_output_filename(input_filename, output_extension)
+    given = get_content(input_filename, directory=where)
+    if given.startswith("###"):
+        head, *rest = given.splitlines()
+        given = "\n".join(rest)
+
+        config = yaml.safe_load(head[3:])
+    else:
+        config = dict()
+
     return InputOutputCase(
         remove_extension(input_filename),
-        get_content(input_filename, directory=where),
+        given,
         get_content(output_filename, directory=where),
+        config,
     )
 
 
 def discover_input_output_cases(where, input_extension, output_extension):
     input_files = get_files_with_extension(where, input_extension)
     output_files = get_files_with_extension(where, output_extension)
     for inp in input_files:
```

