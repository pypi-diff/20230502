# Comparing `tmp/dbt_dry_run-0.6.6.tar.gz` & `tmp/dbt_dry_run-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_dry_run-0.6.6.tar", max compression
+gzip compressed data, was "dbt_dry_run-0.6.7.tar", max compression
```

## Comparing `dbt_dry_run-0.6.6.tar` & `dbt_dry_run-0.6.7.tar`

### file list

```diff
@@ -1,53 +1,54 @@
--rw-r--r--   0        0        0    11356 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/LICENSE
--rw-r--r--   0        0        0    12394 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/README.md
--rw-r--r--   0        0        0        0 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/__init__.py
--rw-r--r--   0        0        0      110 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/__main__.py
--rw-r--r--   0        0        0        0 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/adapter/__init__.py
--rw-r--r--   0        0        0     1597 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/adapter/service.py
--rw-r--r--   0        0        0     3626 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/cli.py
--rw-r--r--   0        0        0     3691 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/columns_metadata.py
--rw-r--r--   0        0        0     1327 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/exception.py
--rw-r--r--   0        0        0     5035 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/execution.py
--rw-r--r--   0        0        0      595 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/flags.py
--rw-r--r--   0        0        0        0 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/linting/__init__.py
--rw-r--r--   0        0        0     1783 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/linting/column_linting.py
--rw-r--r--   0        0        0     4967 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/literals.py
--rw-r--r--   0        0        0      264 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/models/__init__.py
--rw-r--r--   0        0        0     4471 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/models/manifest.py
--rw-r--r--   0        0        0     2491 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/models/profile.py
--rw-r--r--   0        0        0      692 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/models/report.py
--rw-r--r--   0        0        0     2176 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/models/table.py
--rw-r--r--   0        0        0     1757 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/node_runner/__init__.py
--rw-r--r--   0        0        0     4671 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/node_runner/model_runner.py
--rw-r--r--   0        0        0      759 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/node_runner/node_test_runner.py
--rw-r--r--   0        0        0     1564 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/node_runner/seed_runner.py
--rw-r--r--   0        0        0     3861 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/node_runner/snapshot_runner.py
--rw-r--r--   0        0        0     1521 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/node_runner/source_runner.py
--rw-r--r--   0        0        0     4679 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/result_reporter.py
--rw-r--r--   0        0        0     2468 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/results.py
--rw-r--r--   0        0        0     4899 2023-04-13 10:33:14.668043 dbt_dry_run-0.6.6/dbt_dry_run/scheduler.py
--rw-r--r--   0        0        0      620 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/sql_runner/__init__.py
--rw-r--r--   0        0        0     3487 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/sql_runner/big_query_sql_runner.py
--rw-r--r--   0        0        0        0 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/__init__.py
--rw-r--r--   0        0        0      231 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/conftest.py
--rw-r--r--   0        0        0        0 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/linting/__init__.py
--rw-r--r--   0        0        0     1846 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/linting/test_column_linting.py
--rw-r--r--   0        0        0     1691 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/models/test_manifest.py
--rw-r--r--   0        0        0     2761 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/models/test_profile.py
--rw-r--r--   0        0        0        0 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/node_runner/__init__.py
--rw-r--r--   0        0        0    15828 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/node_runner/test_model_runner.py
--rw-r--r--   0        0        0     1019 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/node_runner/test_node_runner.py
--rw-r--r--   0        0        0     2482 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/node_runner/test_seed_runner.py
--rw-r--r--   0        0        0     9693 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/node_runner/test_snapshot_runner.py
--rw-r--r--   0        0        0     2938 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/node_runner/test_test_runner.py
--rw-r--r--   0        0        0        0 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/sql_runner/__init__.py
--rw-r--r--   0        0        0     4436 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/sql_runner/test_big_query_sql_runner.py
--rw-r--r--   0        0        0     5503 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/test_columns_metadata.py
--rw-r--r--   0        0        0     2678 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/test_execution.py
--rw-r--r--   0        0        0     8855 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/test_literals.py
--rw-r--r--   0        0        0     2337 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/test_result_reporter.py
--rw-r--r--   0        0        0     3831 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/test_scheduler.py
--rw-r--r--   0        0        0     1879 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/test/utils.py
--rw-r--r--   0        0        0      184 2023-04-13 10:33:14.672043 dbt_dry_run-0.6.6/dbt_dry_run/version.py
--rw-r--r--   0        0        0     2057 2023-04-13 10:33:14.676043 dbt_dry_run-0.6.6/pyproject.toml
--rw-r--r--   0        0        0    13340 1970-01-01 00:00:00.000000 dbt_dry_run-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/LICENSE
+-rw-r--r--   0        0        0    12394 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/README.md
+-rw-r--r--   0        0        0        0 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/__init__.py
+-rw-r--r--   0        0        0      110 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/adapter/__init__.py
+-rw-r--r--   0        0        0     1994 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/adapter/service.py
+-rw-r--r--   0        0        0      122 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/adapter/utils.py
+-rw-r--r--   0        0        0     4072 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/cli.py
+-rw-r--r--   0        0        0     3691 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/columns_metadata.py
+-rw-r--r--   0        0        0     1327 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/exception.py
+-rw-r--r--   0        0        0     5018 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/execution.py
+-rw-r--r--   0        0        0      595 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/flags.py
+-rw-r--r--   0        0        0        0 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/linting/__init__.py
+-rw-r--r--   0        0        0     1783 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/linting/column_linting.py
+-rw-r--r--   0        0        0     4967 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/literals.py
+-rw-r--r--   0        0        0      264 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/models/__init__.py
+-rw-r--r--   0        0        0     4471 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/models/manifest.py
+-rw-r--r--   0        0        0     2491 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/models/profile.py
+-rw-r--r--   0        0        0      692 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/models/report.py
+-rw-r--r--   0        0        0     2176 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/models/table.py
+-rw-r--r--   0        0        0     1757 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/node_runner/__init__.py
+-rw-r--r--   0        0        0     4671 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/node_runner/model_runner.py
+-rw-r--r--   0        0        0      759 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/node_runner/node_test_runner.py
+-rw-r--r--   0        0        0     1564 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/node_runner/seed_runner.py
+-rw-r--r--   0        0        0     3861 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/node_runner/snapshot_runner.py
+-rw-r--r--   0        0        0     1521 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/node_runner/source_runner.py
+-rw-r--r--   0        0        0     4679 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/result_reporter.py
+-rw-r--r--   0        0        0     2468 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/results.py
+-rw-r--r--   0        0        0     4899 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/scheduler.py
+-rw-r--r--   0        0        0      620 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/sql_runner/__init__.py
+-rw-r--r--   0        0        0     3487 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/sql_runner/big_query_sql_runner.py
+-rw-r--r--   0        0        0        0 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/test/__init__.py
+-rw-r--r--   0        0        0      231 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/test/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/test/linting/__init__.py
+-rw-r--r--   0        0        0     1846 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/test/linting/test_column_linting.py
+-rw-r--r--   0        0        0     1691 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/test/models/test_manifest.py
+-rw-r--r--   0        0        0     2761 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/test/models/test_profile.py
+-rw-r--r--   0        0        0        0 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/test/node_runner/__init__.py
+-rw-r--r--   0        0        0    15828 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/test/node_runner/test_model_runner.py
+-rw-r--r--   0        0        0     1019 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/test/node_runner/test_node_runner.py
+-rw-r--r--   0        0        0     2482 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/test/node_runner/test_seed_runner.py
+-rw-r--r--   0        0        0     9693 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/test/node_runner/test_snapshot_runner.py
+-rw-r--r--   0        0        0     2938 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/test/node_runner/test_test_runner.py
+-rw-r--r--   0        0        0        0 2023-05-02 09:26:54.665686 dbt_dry_run-0.6.7/dbt_dry_run/test/sql_runner/__init__.py
+-rw-r--r--   0        0        0     4436 2023-05-02 09:26:54.669686 dbt_dry_run-0.6.7/dbt_dry_run/test/sql_runner/test_big_query_sql_runner.py
+-rw-r--r--   0        0        0     5503 2023-05-02 09:26:54.669686 dbt_dry_run-0.6.7/dbt_dry_run/test/test_columns_metadata.py
+-rw-r--r--   0        0        0     2678 2023-05-02 09:26:54.669686 dbt_dry_run-0.6.7/dbt_dry_run/test/test_execution.py
+-rw-r--r--   0        0        0     8855 2023-05-02 09:26:54.669686 dbt_dry_run-0.6.7/dbt_dry_run/test/test_literals.py
+-rw-r--r--   0        0        0     2337 2023-05-02 09:26:54.669686 dbt_dry_run-0.6.7/dbt_dry_run/test/test_result_reporter.py
+-rw-r--r--   0        0        0     3831 2023-05-02 09:26:54.669686 dbt_dry_run-0.6.7/dbt_dry_run/test/test_scheduler.py
+-rw-r--r--   0        0        0     1879 2023-05-02 09:26:54.669686 dbt_dry_run-0.6.7/dbt_dry_run/test/utils.py
+-rw-r--r--   0        0        0      167 2023-05-02 09:26:54.669686 dbt_dry_run-0.6.7/dbt_dry_run/version.py
+-rw-r--r--   0        0        0     2057 2023-05-02 09:26:54.673686 dbt_dry_run-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0    13340 1970-01-01 00:00:00.000000 dbt_dry_run-0.6.7/PKG-INFO
```

### Comparing `dbt_dry_run-0.6.6/LICENSE` & `dbt_dry_run-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/README.md` & `dbt_dry_run-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/cli.py` & `dbt_dry_run-0.6.7/dbt_dry_run/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+import json
 import os
 from typing import Optional
 
 import typer
-from dbt.flags import DEFAULT_PROFILES_DIR
 from typer import Option
 
 from dbt_dry_run.adapter.service import DbtArgs, ProjectService
+from dbt_dry_run.adapter.utils import default_profiles_dir
 from dbt_dry_run.exception import ManifestValidationError
 from dbt_dry_run.execution import dry_run_manifest
 from dbt_dry_run.flags import Flags, set_flags
 from dbt_dry_run.result_reporter import ResultReporter
 from dbt_dry_run.version import VERSION
 
 app = typer.Typer()
@@ -20,26 +21,29 @@
     profiles_dir: str,
     target: Optional[str],
     verbose: bool = False,
     report_path: Optional[str] = None,
     cli_vars: str = "{}",
     skip_not_compiled: bool = False,
     extra_check_columns_metadata_key: Optional[str] = None,
+    threads: Optional[int] = None,
 ) -> int:
+    cli_vars_parsed = json.loads(cli_vars)
     set_flags(
         Flags(
             skip_not_compiled=skip_not_compiled,
             extra_check_columns_metadata_key=extra_check_columns_metadata_key,
         )
     )
     args = DbtArgs(
         project_dir=project_dir,
         profiles_dir=os.path.abspath(profiles_dir),
         target=target,
-        vars=cli_vars,
+        vars=cli_vars_parsed,
+        threads=threads,
     )
     project = ProjectService(args)
     exit_code: int
     try:
         dry_run_results = dry_run_manifest(project)
         reporter = ResultReporter(dry_run_results, set(), verbose)
         exit_code = reporter.report_and_check_results()
@@ -65,31 +69,37 @@
 
 _EXTRA_CHECK_COLUMNS_METADATA_KEY_HELP = """
     An extra metadata key that can be used in place of `dry_run.check_columns` for verifying column metadata has been
     specified correctly. `dry_run.check_columns` will always take precedence. The metadata key should be of boolean type
     or it will be cast to a boolean to be 'True/Falsey`
 """
 
+_THREADS_HELP = """
+"[dbt] Number of threads to execute DAG with. You can normally set this higher than the concurrency of your actual dbt
+runs because the dry run queries execute much faster and don't use any resources"
+"""
+
 
 def version_callback(value: bool) -> None:
     if value:
         print(f"dbt-dry-run v{VERSION}")
         raise typer.Exit()
 
 
 @app.command()
 def run(
     profiles_dir: str = Option(
-        DEFAULT_PROFILES_DIR, help="[dbt] Where to search for `profiles.yml`"
+        default_profiles_dir(), help="[dbt] Where to search for `profiles.yml`"
     ),
     project_dir: str = Option(
         os.getcwd(), help="[dbt] Where to search for `dbt_project.yml`"
     ),
     vars: str = Option("{}", help="[dbt] CLI Variables to pass to dbt"),
     target: Optional[str] = Option(None, help="[dbt] Target profile"),
+    threads: Optional[int] = Option(None, help=_THREADS_HELP),
     verbose: bool = Option(False, help="Output verbose error messages"),
     report_path: Optional[str] = Option(None, help="Json path to dump report to"),
     skip_not_compiled: bool = Option(
         False, "--skip-not-compiled", help=_SKIP_NOT_COMPILED_HELP
     ),
     extra_check_columns_metadata_key: Optional[str] = Option(
         None,
@@ -103,14 +113,15 @@
         profiles_dir,
         target,
         verbose,
         report_path,
         vars,
         skip_not_compiled,
         extra_check_columns_metadata_key,
+        threads,
     )
     if exit_code > 0:
         raise typer.Exit(exit_code)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/columns_metadata.py` & `dbt_dry_run-0.6.7/dbt_dry_run/columns_metadata.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/exception.py` & `dbt_dry_run-0.6.7/dbt_dry_run/exception.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/execution.py` & `dbt_dry_run-0.6.7/dbt_dry_run/execution.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,16 +21,14 @@
 from dbt_dry_run.node_runner.seed_runner import SeedRunner
 from dbt_dry_run.node_runner.snapshot_runner import SnapshotRunner
 from dbt_dry_run.node_runner.source_runner import SourceRunner
 from dbt_dry_run.results import DryRunResult, Results
 from dbt_dry_run.scheduler import ManifestScheduler
 from dbt_dry_run.sql_runner.big_query_sql_runner import BigQuerySQLRunner
 
-CONCURRENCY = 8
-
 _RUNNER_CLASSES: List[Any] = [
     ModelRunner,
     SeedRunner,
     SnapshotRunner,
     NodeTestRunner,
     SourceRunner,
 ]
```

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/flags.py` & `dbt_dry_run-0.6.7/dbt_dry_run/flags.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/linting/column_linting.py` & `dbt_dry_run-0.6.7/dbt_dry_run/linting/column_linting.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/literals.py` & `dbt_dry_run-0.6.7/dbt_dry_run/literals.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/models/manifest.py` & `dbt_dry_run-0.6.7/dbt_dry_run/models/manifest.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/models/profile.py` & `dbt_dry_run-0.6.7/dbt_dry_run/models/profile.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/models/report.py` & `dbt_dry_run-0.6.7/dbt_dry_run/models/report.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/models/table.py` & `dbt_dry_run-0.6.7/dbt_dry_run/models/table.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/node_runner/__init__.py` & `dbt_dry_run-0.6.7/dbt_dry_run/node_runner/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/node_runner/model_runner.py` & `dbt_dry_run-0.6.7/dbt_dry_run/node_runner/model_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/node_runner/node_test_runner.py` & `dbt_dry_run-0.6.7/dbt_dry_run/node_runner/node_test_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/node_runner/seed_runner.py` & `dbt_dry_run-0.6.7/dbt_dry_run/node_runner/seed_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/node_runner/snapshot_runner.py` & `dbt_dry_run-0.6.7/dbt_dry_run/node_runner/snapshot_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/node_runner/source_runner.py` & `dbt_dry_run-0.6.7/dbt_dry_run/node_runner/source_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/result_reporter.py` & `dbt_dry_run-0.6.7/dbt_dry_run/result_reporter.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/results.py` & `dbt_dry_run-0.6.7/dbt_dry_run/results.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/scheduler.py` & `dbt_dry_run-0.6.7/dbt_dry_run/scheduler.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/sql_runner/__init__.py` & `dbt_dry_run-0.6.7/dbt_dry_run/sql_runner/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/sql_runner/big_query_sql_runner.py` & `dbt_dry_run-0.6.7/dbt_dry_run/sql_runner/big_query_sql_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/test/linting/test_column_linting.py` & `dbt_dry_run-0.6.7/dbt_dry_run/test/linting/test_column_linting.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/test/models/test_manifest.py` & `dbt_dry_run-0.6.7/dbt_dry_run/test/models/test_manifest.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/test/models/test_profile.py` & `dbt_dry_run-0.6.7/dbt_dry_run/test/models/test_profile.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/test/node_runner/test_model_runner.py` & `dbt_dry_run-0.6.7/dbt_dry_run/test/node_runner/test_model_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/test/node_runner/test_node_runner.py` & `dbt_dry_run-0.6.7/dbt_dry_run/test/node_runner/test_node_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/test/node_runner/test_seed_runner.py` & `dbt_dry_run-0.6.7/dbt_dry_run/test/node_runner/test_seed_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/test/node_runner/test_snapshot_runner.py` & `dbt_dry_run-0.6.7/dbt_dry_run/test/node_runner/test_snapshot_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/test/node_runner/test_test_runner.py` & `dbt_dry_run-0.6.7/dbt_dry_run/test/node_runner/test_test_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/test/sql_runner/test_big_query_sql_runner.py` & `dbt_dry_run-0.6.7/dbt_dry_run/test/sql_runner/test_big_query_sql_runner.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/test/test_columns_metadata.py` & `dbt_dry_run-0.6.7/dbt_dry_run/test/test_columns_metadata.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/test/test_execution.py` & `dbt_dry_run-0.6.7/dbt_dry_run/test/test_execution.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/test/test_literals.py` & `dbt_dry_run-0.6.7/dbt_dry_run/test/test_literals.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/test/test_result_reporter.py` & `dbt_dry_run-0.6.7/dbt_dry_run/test/test_result_reporter.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/test/test_scheduler.py` & `dbt_dry_run-0.6.7/dbt_dry_run/test/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/dbt_dry_run/test/utils.py` & `dbt_dry_run-0.6.7/dbt_dry_run/test/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_dry_run-0.6.6/pyproject.toml` & `dbt_dry_run-0.6.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt-dry-run"
-version = "0.6.6"
+version = "0.6.7"
 description = "Dry run dbt projects"
 authors = ["Connor Charles <connor.charles@autotrader.co.uk>",
            "Phil hope <philip.hope@autotrader.co.uk>",
            "Angelos Georgiadis <angelos.georgiadis@autotrader.co.uk>",
            "Richard Wilmer <richard.wilmer@autotrader.co.uk>"]
 readme = "README.md"
 license = "Apache-2.0"
@@ -29,15 +29,15 @@
 pytest = "^7.2.0"
 mypy = "^0.931"
 types-PyYAML = "^6.0.4"
 pytest-cov = "^4.0.0"
 twine = "^3.8.0"
 types-setuptools = "^57.4.9"
 pytest-mock = "^3.7.0"
-dbt-bigquery = "^1.4.1"
+dbt-bigquery = "^1.5.0"
 
 [build-system]
 requires = ["poetry-core>=1.5.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 testpaths = "dbt_dry_run/test"
```

### Comparing `dbt_dry_run-0.6.6/PKG-INFO` & `dbt_dry_run-0.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-dry-run
-Version: 0.6.6
+Version: 0.6.7
 Summary: Dry run dbt projects
 Home-page: https://github.com/autotraderuk/dbt-dry-run
 License: Apache-2.0
 Author: Connor Charles
 Author-email: connor.charles@autotrader.co.uk
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
```

