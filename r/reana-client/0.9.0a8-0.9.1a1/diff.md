# Comparing `tmp/reana-client-0.9.0a8.tar.gz` & `tmp/reana-client-0.9.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reana-client-0.9.0a8.tar", last modified: Wed Dec  7 12:03:14 2022, max compression
+gzip compressed data, was "reana-client-0.9.1a1.tar", last modified: Tue May  2 08:53:31 2023, max compression
```

## Comparing `reana-client-0.9.0a8.tar` & `reana-client-0.9.1a1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 madonado   (501) staff       (20)        0 2022-12-07 12:03:14.321668 reana-client-0.9.0a8/
--rw-r--r--   0 madonado   (501) staff       (20)      272 2022-03-25 14:09:55.000000 reana-client-0.9.0a8/.flake8
--rw-r--r--   0 madonado   (501) staff       (20)     1099 2022-06-14 12:37:33.000000 reana-client-0.9.0a8/AUTHORS.rst
--rw-r--r--   0 madonado   (501) staff       (20)    11196 2022-11-25 13:27:21.000000 reana-client-0.9.0a8/CHANGES.rst
--rw-r--r--   0 madonado   (501) staff       (20)      675 2022-03-25 14:09:55.000000 reana-client-0.9.0a8/CONTRIBUTING.rst
--rw-r--r--   0 madonado   (501) staff       (20)     1092 2022-03-25 14:09:55.000000 reana-client-0.9.0a8/LICENSE
--rw-r--r--   0 madonado   (501) staff       (20)      692 2022-03-25 14:09:55.000000 reana-client-0.9.0a8/MANIFEST.in
--rw-r--r--   0 madonado   (501) staff       (20)    14651 2022-12-07 12:03:14.321957 reana-client-0.9.0a8/PKG-INFO
--rw-r--r--   0 madonado   (501) staff       (20)     2318 2022-03-25 14:09:55.000000 reana-client-0.9.0a8/README.rst
-drwxr-xr-x   0 madonado   (501) staff       (20)        0 2022-12-07 12:03:14.303821 reana-client-0.9.0a8/docs/
--rw-r--r--   0 madonado   (501) staff       (20)     1658 2022-11-25 13:27:21.000000 reana-client-0.9.0a8/docs/cmd_list.txt
--rw-r--r--   0 madonado   (501) staff       (20)     6316 2022-06-08 07:48:30.000000 reana-client-0.9.0a8/docs/conf.py
--rw-r--r--   0 madonado   (501) staff       (20)      797 2022-03-25 14:09:55.000000 reana-client-0.9.0a8/docs/index.rst
--rw-r--r--   0 madonado   (501) staff       (20)      210 2022-03-25 14:09:55.000000 reana-client-0.9.0a8/docs/requirements.txt
--rw-r--r--   0 madonado   (501) staff       (20)      313 2022-03-25 14:09:55.000000 reana-client-0.9.0a8/pytest.ini
-drwxr-xr-x   0 madonado   (501) staff       (20)        0 2022-12-07 12:03:14.305890 reana-client-0.9.0a8/reana_client/
--rw-r--r--   0 madonado   (501) staff       (20)      382 2022-03-25 14:09:55.000000 reana-client-0.9.0a8/reana_client/__init__.py
-drwxr-xr-x   0 madonado   (501) staff       (20)        0 2022-12-07 12:03:14.308988 reana-client-0.9.0a8/reana_client/api/
--rw-r--r--   0 madonado   (501) staff       (20)      337 2022-03-25 14:09:55.000000 reana-client-0.9.0a8/reana_client/api/__init__.py
--rw-r--r--   0 madonado   (501) staff       (20)    39001 2022-11-25 13:27:21.000000 reana-client-0.9.0a8/reana_client/api/client.py
--rw-r--r--   0 madonado   (501) staff       (20)      616 2022-03-25 14:09:55.000000 reana-client-0.9.0a8/reana_client/api/utils.py
-drwxr-xr-x   0 madonado   (501) staff       (20)        0 2022-12-07 12:03:14.312007 reana-client-0.9.0a8/reana_client/cli/
--rw-r--r--   0 madonado   (501) staff       (20)     3061 2022-11-25 13:27:21.000000 reana-client-0.9.0a8/reana_client/cli/__init__.py
--rw-r--r--   0 madonado   (501) staff       (20)     9029 2022-03-31 11:45:21.000000 reana-client-0.9.0a8/reana_client/cli/cwl_runner.py
--rw-r--r--   0 madonado   (501) staff       (20)    21486 2022-11-17 09:21:05.000000 reana-client-0.9.0a8/reana_client/cli/files.py
--rw-r--r--   0 madonado   (501) staff       (20)     3768 2022-10-03 11:38:26.000000 reana-client-0.9.0a8/reana_client/cli/ping.py
--rw-r--r--   0 madonado   (501) staff       (20)     3328 2022-10-03 11:38:26.000000 reana-client-0.9.0a8/reana_client/cli/quotas.py
--rw-r--r--   0 madonado   (501) staff       (20)     2114 2022-11-25 13:27:21.000000 reana-client-0.9.0a8/reana_client/cli/retention_rules.py
--rw-r--r--   0 madonado   (501) staff       (20)     4789 2022-11-15 09:36:26.000000 reana-client-0.9.0a8/reana_client/cli/secrets.py
--rw-r--r--   0 madonado   (501) staff       (20)    13480 2022-11-17 09:21:05.000000 reana-client-0.9.0a8/reana_client/cli/utils.py
--rw-r--r--   0 madonado   (501) staff       (20)    48270 2022-11-17 09:21:05.000000 reana-client-0.9.0a8/reana_client/cli/workflow.py
--rw-r--r--   0 madonado   (501) staff       (20)     2084 2022-05-18 15:02:53.000000 reana-client-0.9.0a8/reana_client/config.py
--rw-r--r--   0 madonado   (501) staff       (20)      528 2022-03-25 14:09:55.000000 reana-client-0.9.0a8/reana_client/errors.py
--rw-r--r--   0 madonado   (501) staff       (20)     1833 2022-06-17 12:43:36.000000 reana-client-0.9.0a8/reana_client/printer.py
--rw-r--r--   0 madonado   (501) staff       (20)     9106 2022-11-15 09:36:26.000000 reana-client-0.9.0a8/reana_client/utils.py
-drwxr-xr-x   0 madonado   (501) staff       (20)        0 2022-12-07 12:03:14.315222 reana-client-0.9.0a8/reana_client/validation/
--rw-r--r--   0 madonado   (501) staff       (20)      257 2022-03-25 14:09:55.000000 reana-client-0.9.0a8/reana_client/validation/__init__.py
--rw-r--r--   0 madonado   (501) staff       (20)     1296 2022-03-31 11:45:21.000000 reana-client-0.9.0a8/reana_client/validation/compute_backends.py
--rw-r--r--   0 madonado   (501) staff       (20)    19337 2022-05-18 15:02:53.000000 reana-client-0.9.0a8/reana_client/validation/environments.py
--rw-r--r--   0 madonado   (501) staff       (20)     2590 2022-03-31 11:45:21.000000 reana-client-0.9.0a8/reana_client/validation/parameters.py
--rw-r--r--   0 madonado   (501) staff       (20)     4009 2022-03-31 11:45:21.000000 reana-client-0.9.0a8/reana_client/validation/utils.py
--rw-r--r--   0 madonado   (501) staff       (20)     1402 2022-03-31 11:45:21.000000 reana-client-0.9.0a8/reana_client/validation/workspace.py
--rw-r--r--   0 madonado   (501) staff       (20)      462 2022-12-07 12:02:22.000000 reana-client-0.9.0a8/reana_client/version.py
-drwxr-xr-x   0 madonado   (501) staff       (20)        0 2022-12-07 12:03:14.308054 reana-client-0.9.0a8/reana_client.egg-info/
--rw-r--r--   0 madonado   (501) staff       (20)    14651 2022-12-07 12:03:14.000000 reana-client-0.9.0a8/reana_client.egg-info/PKG-INFO
--rw-r--r--   0 madonado   (501) staff       (20)     1583 2022-12-07 12:03:14.000000 reana-client-0.9.0a8/reana_client.egg-info/SOURCES.txt
--rw-r--r--   0 madonado   (501) staff       (20)        1 2022-12-07 12:03:14.000000 reana-client-0.9.0a8/reana_client.egg-info/dependency_links.txt
--rw-r--r--   0 madonado   (501) staff       (20)      112 2022-12-07 12:03:14.000000 reana-client-0.9.0a8/reana_client.egg-info/entry_points.txt
--rw-r--r--   0 madonado   (501) staff       (20)        1 2022-12-07 12:03:14.000000 reana-client-0.9.0a8/reana_client.egg-info/not-zip-safe
--rw-r--r--   0 madonado   (501) staff       (20)      472 2022-12-07 12:03:14.000000 reana-client-0.9.0a8/reana_client.egg-info/requires.txt
--rw-r--r--   0 madonado   (501) staff       (20)       13 2022-12-07 12:03:14.000000 reana-client-0.9.0a8/reana_client.egg-info/top_level.txt
--rw-r--r--   0 madonado   (501) staff       (20)       85 2022-03-25 14:09:55.000000 reana-client-0.9.0a8/requirements-dev.txt
--rwxr-xr-x   0 madonado   (501) staff       (20)     1959 2022-11-25 13:27:17.000000 reana-client-0.9.0a8/run-tests.sh
-drwxr-xr-x   0 madonado   (501) staff       (20)        0 2022-12-07 12:03:14.316350 reana-client-0.9.0a8/scripts/
--rwxr-xr-x   0 madonado   (501) staff       (20)     3285 2022-03-25 14:09:55.000000 reana-client-0.9.0a8/scripts/create-appimage.sh
--rw-r--r--   0 madonado   (501) staff       (20)     1173 2022-03-31 11:45:21.000000 reana-client-0.9.0a8/scripts/generate_cli_api.py
--rw-r--r--   0 madonado   (501) staff       (20)      174 2022-12-07 12:03:14.322898 reana-client-0.9.0a8/setup.cfg
--rw-r--r--   0 madonado   (501) staff       (20)     3009 2022-12-07 12:02:22.000000 reana-client-0.9.0a8/setup.py
-drwxr-xr-x   0 madonado   (501) staff       (20)        0 2022-12-07 12:03:14.321263 reana-client-0.9.0a8/tests/
--rw-r--r--   0 madonado   (501) staff       (20)     6685 2022-05-17 13:13:09.000000 reana-client-0.9.0a8/tests/conftest.py
--rw-r--r--   0 madonado   (501) staff       (20)    22941 2022-10-03 11:38:26.000000 reana-client-0.9.0a8/tests/test_cli_files.py
--rw-r--r--   0 madonado   (501) staff       (20)     2349 2022-03-25 14:09:55.000000 reana-client-0.9.0a8/tests/test_cli_ping.py
--rw-r--r--   0 madonado   (501) staff       (20)     1396 2022-11-25 13:27:21.000000 reana-client-0.9.0a8/tests/test_cli_retention_rules.py
--rw-r--r--   0 madonado   (501) staff       (20)     5519 2022-03-25 14:09:55.000000 reana-client-0.9.0a8/tests/test_cli_secrets.py
--rw-r--r--   0 madonado   (501) staff       (20)    33003 2022-10-04 08:35:49.000000 reana-client-0.9.0a8/tests/test_cli_workflows.py
--rw-r--r--   0 madonado   (501) staff       (20)     1354 2022-06-30 13:51:00.000000 reana-client-0.9.0a8/tests/test_utils.py
--rw-r--r--   0 madonado   (501) staff       (20)     5756 2022-03-31 11:45:21.000000 reana-client-0.9.0a8/tests/test_validate_compute_backends.py
--rw-r--r--   0 madonado   (501) staff       (20)     1820 2022-05-18 15:02:53.000000 reana-client-0.9.0a8/tests/test_validate_environments.py
--rw-r--r--   0 madonado   (501) staff       (20)     9450 2022-03-31 11:45:21.000000 reana-client-0.9.0a8/tests/test_validate_parameters.py
--rw-r--r--   0 madonado   (501) staff       (20)     2982 2022-03-25 14:09:55.000000 reana-client-0.9.0a8/tests/test_validate_server_capabilities.py
--rw-r--r--   0 madonado   (501) staff       (20)      444 2022-03-25 14:09:55.000000 reana-client-0.9.0a8/tests/test_version.py
--rw-r--r--   0 madonado   (501) staff       (20)      333 2022-11-10 13:25:47.000000 reana-client-0.9.0a8/tox.ini
+drwxr-xr-x   0 madonado   (501) staff       (20)        0 2023-05-02 08:53:31.414265 reana-client-0.9.1a1/
+-rw-r--r--   0 madonado   (501) staff       (20)      272 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/.flake8
+-rw-r--r--   0 madonado   (501) staff       (20)     1161 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/AUTHORS.rst
+-rw-r--r--   0 madonado   (501) staff       (20)    11704 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/CHANGES.rst
+-rw-r--r--   0 madonado   (501) staff       (20)      675 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/CONTRIBUTING.rst
+-rw-r--r--   0 madonado   (501) staff       (20)     1098 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/LICENSE
+-rw-r--r--   0 madonado   (501) staff       (20)      692 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/MANIFEST.in
+-rw-r--r--   0 madonado   (501) staff       (20)    15159 2023-05-02 08:53:31.414485 reana-client-0.9.1a1/PKG-INFO
+-rw-r--r--   0 madonado   (501) staff       (20)     2318 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/README.rst
+drwxr-xr-x   0 madonado   (501) staff       (20)        0 2023-05-02 08:53:31.397958 reana-client-0.9.1a1/docs/
+-rw-r--r--   0 madonado   (501) staff       (20)     1693 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/docs/cmd_list.txt
+-rw-r--r--   0 madonado   (501) staff       (20)     6316 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/docs/conf.py
+-rw-r--r--   0 madonado   (501) staff       (20)      797 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/docs/index.rst
+-rw-r--r--   0 madonado   (501) staff       (20)      210 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/docs/requirements.txt
+-rw-r--r--   0 madonado   (501) staff       (20)      313 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/pytest.ini
+drwxr-xr-x   0 madonado   (501) staff       (20)        0 2023-05-02 08:53:31.399581 reana-client-0.9.1a1/reana_client/
+-rw-r--r--   0 madonado   (501) staff       (20)      382 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/reana_client/__init__.py
+drwxr-xr-x   0 madonado   (501) staff       (20)        0 2023-05-02 08:53:31.402206 reana-client-0.9.1a1/reana_client/api/
+-rw-r--r--   0 madonado   (501) staff       (20)      337 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/reana_client/api/__init__.py
+-rw-r--r--   0 madonado   (501) staff       (20)    39998 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/reana_client/api/client.py
+-rw-r--r--   0 madonado   (501) staff       (20)      616 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/reana_client/api/utils.py
+drwxr-xr-x   0 madonado   (501) staff       (20)        0 2023-05-02 08:53:31.405057 reana-client-0.9.1a1/reana_client/cli/
+-rw-r--r--   0 madonado   (501) staff       (20)     3061 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/reana_client/cli/__init__.py
+-rw-r--r--   0 madonado   (501) staff       (20)     9028 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/reana_client/cli/cwl_runner.py
+-rw-r--r--   0 madonado   (501) staff       (20)    23046 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/reana_client/cli/files.py
+-rw-r--r--   0 madonado   (501) staff       (20)     3768 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/reana_client/cli/ping.py
+-rw-r--r--   0 madonado   (501) staff       (20)     3328 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/reana_client/cli/quotas.py
+-rw-r--r--   0 madonado   (501) staff       (20)     2114 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/reana_client/cli/retention_rules.py
+-rw-r--r--   0 madonado   (501) staff       (20)     4789 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/reana_client/cli/secrets.py
+-rw-r--r--   0 madonado   (501) staff       (20)    13480 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/reana_client/cli/utils.py
+-rw-r--r--   0 madonado   (501) staff       (20)    49124 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/reana_client/cli/workflow.py
+-rw-r--r--   0 madonado   (501) staff       (20)     2084 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/reana_client/config.py
+-rw-r--r--   0 madonado   (501) staff       (20)      528 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/reana_client/errors.py
+-rw-r--r--   0 madonado   (501) staff       (20)     1833 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/reana_client/printer.py
+-rw-r--r--   0 madonado   (501) staff       (20)     9107 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/reana_client/utils.py
+drwxr-xr-x   0 madonado   (501) staff       (20)        0 2023-05-02 08:53:31.407646 reana-client-0.9.1a1/reana_client/validation/
+-rw-r--r--   0 madonado   (501) staff       (20)      257 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/reana_client/validation/__init__.py
+-rw-r--r--   0 madonado   (501) staff       (20)     1296 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/reana_client/validation/compute_backends.py
+-rw-r--r--   0 madonado   (501) staff       (20)    19337 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/reana_client/validation/environments.py
+-rw-r--r--   0 madonado   (501) staff       (20)     2590 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/reana_client/validation/parameters.py
+-rw-r--r--   0 madonado   (501) staff       (20)     4009 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/reana_client/validation/utils.py
+-rw-r--r--   0 madonado   (501) staff       (20)     1402 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/reana_client/validation/workspace.py
+-rw-r--r--   0 madonado   (501) staff       (20)      462 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/reana_client/version.py
+drwxr-xr-x   0 madonado   (501) staff       (20)        0 2023-05-02 08:53:31.401373 reana-client-0.9.1a1/reana_client.egg-info/
+-rw-r--r--   0 madonado   (501) staff       (20)    15159 2023-05-02 08:53:31.000000 reana-client-0.9.1a1/reana_client.egg-info/PKG-INFO
+-rw-r--r--   0 madonado   (501) staff       (20)     1583 2023-05-02 08:53:31.000000 reana-client-0.9.1a1/reana_client.egg-info/SOURCES.txt
+-rw-r--r--   0 madonado   (501) staff       (20)        1 2023-05-02 08:53:31.000000 reana-client-0.9.1a1/reana_client.egg-info/dependency_links.txt
+-rw-r--r--   0 madonado   (501) staff       (20)      112 2023-05-02 08:53:31.000000 reana-client-0.9.1a1/reana_client.egg-info/entry_points.txt
+-rw-r--r--   0 madonado   (501) staff       (20)        1 2023-05-02 08:53:31.000000 reana-client-0.9.1a1/reana_client.egg-info/not-zip-safe
+-rw-r--r--   0 madonado   (501) staff       (20)      467 2023-05-02 08:53:31.000000 reana-client-0.9.1a1/reana_client.egg-info/requires.txt
+-rw-r--r--   0 madonado   (501) staff       (20)       13 2023-05-02 08:53:31.000000 reana-client-0.9.1a1/reana_client.egg-info/top_level.txt
+-rw-r--r--   0 madonado   (501) staff       (20)       85 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/requirements-dev.txt
+-rwxr-xr-x   0 madonado   (501) staff       (20)     1959 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/run-tests.sh
+drwxr-xr-x   0 madonado   (501) staff       (20)        0 2023-05-02 08:53:31.408496 reana-client-0.9.1a1/scripts/
+-rwxr-xr-x   0 madonado   (501) staff       (20)     3285 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/scripts/create-appimage.sh
+-rw-r--r--   0 madonado   (501) staff       (20)     1173 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/scripts/generate_cli_api.py
+-rw-r--r--   0 madonado   (501) staff       (20)      174 2023-05-02 08:53:31.415188 reana-client-0.9.1a1/setup.cfg
+-rw-r--r--   0 madonado   (501) staff       (20)     3012 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/setup.py
+drwxr-xr-x   0 madonado   (501) staff       (20)        0 2023-05-02 08:53:31.413963 reana-client-0.9.1a1/tests/
+-rw-r--r--   0 madonado   (501) staff       (20)     6685 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/tests/conftest.py
+-rw-r--r--   0 madonado   (501) staff       (20)    24033 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/tests/test_cli_files.py
+-rw-r--r--   0 madonado   (501) staff       (20)     2348 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/tests/test_cli_ping.py
+-rw-r--r--   0 madonado   (501) staff       (20)     1396 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/tests/test_cli_retention_rules.py
+-rw-r--r--   0 madonado   (501) staff       (20)     5519 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/tests/test_cli_secrets.py
+-rw-r--r--   0 madonado   (501) staff       (20)    34437 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/tests/test_cli_workflows.py
+-rw-r--r--   0 madonado   (501) staff       (20)     1354 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/tests/test_utils.py
+-rw-r--r--   0 madonado   (501) staff       (20)     5756 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/tests/test_validate_compute_backends.py
+-rw-r--r--   0 madonado   (501) staff       (20)     1820 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/tests/test_validate_environments.py
+-rw-r--r--   0 madonado   (501) staff       (20)     9450 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/tests/test_validate_parameters.py
+-rw-r--r--   0 madonado   (501) staff       (20)     2982 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/tests/test_validate_server_capabilities.py
+-rw-r--r--   0 madonado   (501) staff       (20)      444 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/tests/test_version.py
+-rw-r--r--   0 madonado   (501) staff       (20)      333 2023-05-02 08:41:32.000000 reana-client-0.9.1a1/tox.ini
```

### Comparing `reana-client-0.9.0a8/AUTHORS.rst` & `reana-client-0.9.1a1/AUTHORS.rst`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 - `Adelina Lintuluoto <https://orcid.org/0000-0002-0726-1452>`_
 - `Audrius Mecionis <https://orcid.org/0000-0002-3759-1663>`_
 - `Anton Khodak <https://orcid.org/0000-0003-3263-4553>`_
 - `Camila Diaz <https://orcid.org/0000-0001-5543-797X>`_
 - `Daniel Prelipcean <https://orcid.org/0000-0002-4855-194X>`_
 - `Diego Rodriguez <https://orcid.org/0000-0003-0649-2002>`_
 - `Dinos Kousidis <https://orcid.org/0000-0002-4914-4289>`_
+- `Giuseppe Steduto <https://orcid.org/0009-0002-1258-8553>`_
 - `Harri Hirvonsalo <https://orcid.org/0000-0002-5503-510X>`_
 - `Jan Okraska <https://orcid.org/0000-0002-1416-3244>`_
 - `Leticia Wanderley <https://orcid.org/0000-0003-4649-6630>`_
 - `Marco Donadoni <https://orcid.org/0000-0003-2922-5505>`_
 - `Marco Vidal <https://orcid.org/0000-0002-9363-4971>`_
 - `Matthew Feickert <https://orcid.org/0000-0003-4124-7862>`_
 - `Rokas Maciulaitis <https://orcid.org/0000-0003-1064-6967>`_
```

### Comparing `reana-client-0.9.0a8/CHANGES.rst` & `reana-client-0.9.1a1/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 Changes
 =======
 
-Version 0.9.0 (UNRELEASED)
+Version 0.9.1 (UNRELEASED)
+--------------------------
+
+- Adds ``prune`` command to delete all intermediate files of a given workflow.
+- Fixes ``list`` command to correctly list workflows when sorting them by their run number or by the size of their workspace.
+- Fixes ``du`` command help message typo.
+
+Version 0.9.0 (2023-01-26)
 --------------------------
 
 - Adds support for Python 3.11.
-- Adds support for ``.reanaignore`` during file upload. Files that match ``.reanaignore`` will not be uploaded.
-- Adds support for ``.gitignore`` during file upload. Files that match ``.gitignore`` will not be uploaded.
+- Adds support for ``.gitignore`` and ``.reanaignore`` to specify files that should not be uploaded to REANA.
 - Adds ``retention-rules-list`` command to list the retention rules of a workflow.
-- Changes ``delete`` CLI command to always delete workspace.
-- Changes ``delete_workflow`` API method to always delete workspace.
-- Changes ``list`` to hide deleted workflows by default.
+- Changes REANA specification loading and validation functionalities by porting some of the logic to ``reana-commons``.
+- Changes ``create`` and ``restart`` commands to always upload the REANA specification file.
+- Changes ``delete`` command to always delete the workflow's workspace.
+- Changes ``delete_workflow`` Python API function to always delete the workflow's workspace.
+- Changes ``download`` command to add the possibility to write files to the standard output via ``-o -`` option.
+- Changes ``list`` command to hide deleted workflows by default.
 - Changes ``list`` command to allow displaying deleted workflows via ``--all`` and ``--show-deleted-runs`` options.
-- Changes ``list`` command to allow displaying the duration of workflows with the ``--include-duration`` option.
-- Changes ``status`` command to allow displaying the duration of workflows with the ``--include-duration`` option.
-- Changes REANA specification loading and validation functionality by porting some of the logic to ``reana-commons``.
+- Changes ``list`` and ``status`` commands to allow displaying the duration of workflows with the ``--include-duration`` option.
 - Changes ``mv`` command to allow moving files while a workflow is running.
 - Changes ``upload`` command to prevent uploading symlinks.
-- Fixes ``validate --environment`` command to detect illegal white space characters in image names.
+- Changes ``validation --environment`` command to use Docker registry v2 APIs to check that a Docker image exists in DockerHub.
 - Fixes ``list`` command to highlight the workflow specified in ``REANA_WORKON`` correctly.
 - Fixes ``secrets-delete`` command error message when deleting non existing secrets.
-- Fixes ``upload`` command to report in case input directories are listed under files and vice versa.
-
-Version 0.8.2 (UNRELEASED)
---------------------------
-
-- Changes ``download`` command to add the possibility to write files to the standard output via ``-o -`` option.
+- Fixes ``start`` command to report failed workflows as errors.
 - Fixes ``start`` and ``run`` commands to correctly follow the execution of the workflow until termination.
+- Fixes ``status`` command to respect output format provided by the ``--format`` option.
+- Fixes ``upload`` command to report when input directories are listed under the ``files`` section in the REANA specification file and vice versa.
+- Fixes ``validate --environment`` command to detect illegal whitespace characters in Docker image names.
 
 Version 0.8.1 (2022-02-15)
 --------------------------
 
 - Adds support for creating reana-client standalone AppImage executables.
 - Adds support for Python 3.10.
 - Adds workflow name validation for ``create_workflow_from_json()`` Python API function.
```

### Comparing `reana-client-0.9.0a8/CONTRIBUTING.rst` & `reana-client-0.9.1a1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `reana-client-0.9.0a8/LICENSE` & `reana-client-0.9.1a1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (C) 2017, 2018, 2019, 2020, 2021, 2022 CERN.
+Copyright (C) 2017, 2018, 2019, 2020, 2021, 2022, 2023 CERN.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 the Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions:
```

### Comparing `reana-client-0.9.0a8/MANIFEST.in` & `reana-client-0.9.1a1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `reana-client-0.9.0a8/PKG-INFO` & `reana-client-0.9.1a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reana-client
-Version: 0.9.0a8
+Version: 0.9.1a1
 Summary: REANA client
 Home-page: https://github.com/reanahub/reana-client
 Author: REANA
 Author-email: info@reana.io
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
@@ -97,40 +97,45 @@
 - `REANA-Client known issues <https://github.com/reanahub/reana-client/issues>`_
 - `REANA-Client source code <https://github.com/reanahub/reana-client>`_
 
 
 Changes
 =======
 
-Version 0.9.0 (UNRELEASED)
+Version 0.9.1 (UNRELEASED)
+--------------------------
+
+- Adds ``prune`` command to delete all intermediate files of a given workflow.
+- Fixes ``list`` command to correctly list workflows when sorting them by their run number or by the size of their workspace.
+- Fixes ``du`` command help message typo.
+
+Version 0.9.0 (2023-01-26)
 --------------------------
 
 - Adds support for Python 3.11.
-- Adds support for ``.reanaignore`` during file upload. Files that match ``.reanaignore`` will not be uploaded.
-- Adds support for ``.gitignore`` during file upload. Files that match ``.gitignore`` will not be uploaded.
+- Adds support for ``.gitignore`` and ``.reanaignore`` to specify files that should not be uploaded to REANA.
 - Adds ``retention-rules-list`` command to list the retention rules of a workflow.
-- Changes ``delete`` CLI command to always delete workspace.
-- Changes ``delete_workflow`` API method to always delete workspace.
-- Changes ``list`` to hide deleted workflows by default.
+- Changes REANA specification loading and validation functionalities by porting some of the logic to ``reana-commons``.
+- Changes ``create`` and ``restart`` commands to always upload the REANA specification file.
+- Changes ``delete`` command to always delete the workflow's workspace.
+- Changes ``delete_workflow`` Python API function to always delete the workflow's workspace.
+- Changes ``download`` command to add the possibility to write files to the standard output via ``-o -`` option.
+- Changes ``list`` command to hide deleted workflows by default.
 - Changes ``list`` command to allow displaying deleted workflows via ``--all`` and ``--show-deleted-runs`` options.
-- Changes ``list`` command to allow displaying the duration of workflows with the ``--include-duration`` option.
-- Changes ``status`` command to allow displaying the duration of workflows with the ``--include-duration`` option.
-- Changes REANA specification loading and validation functionality by porting some of the logic to ``reana-commons``.
+- Changes ``list`` and ``status`` commands to allow displaying the duration of workflows with the ``--include-duration`` option.
 - Changes ``mv`` command to allow moving files while a workflow is running.
 - Changes ``upload`` command to prevent uploading symlinks.
-- Fixes ``validate --environment`` command to detect illegal white space characters in image names.
+- Changes ``validation --environment`` command to use Docker registry v2 APIs to check that a Docker image exists in DockerHub.
 - Fixes ``list`` command to highlight the workflow specified in ``REANA_WORKON`` correctly.
 - Fixes ``secrets-delete`` command error message when deleting non existing secrets.
-- Fixes ``upload`` command to report in case input directories are listed under files and vice versa.
-
-Version 0.8.2 (UNRELEASED)
---------------------------
-
-- Changes ``download`` command to add the possibility to write files to the standard output via ``-o -`` option.
+- Fixes ``start`` command to report failed workflows as errors.
 - Fixes ``start`` and ``run`` commands to correctly follow the execution of the workflow until termination.
+- Fixes ``status`` command to respect output format provided by the ``--format`` option.
+- Fixes ``upload`` command to report when input directories are listed under the ``files`` section in the REANA specification file and vice versa.
+- Fixes ``validate --environment`` command to detect illegal whitespace characters in Docker image names.
 
 Version 0.8.1 (2022-02-15)
 --------------------------
 
 - Adds support for creating reana-client standalone AppImage executables.
 - Adds support for Python 3.10.
 - Adds workflow name validation for ``create_workflow_from_json()`` Python API function.
```

### Comparing `reana-client-0.9.0a8/README.rst` & `reana-client-0.9.1a1/README.rst`

 * *Files identical despite different names*

### Comparing `reana-client-0.9.0a8/docs/cmd_list.txt` & `reana-client-0.9.1a1/docs/cmd_list.txt`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,15 @@
   open   Open an interactive session inside the workspace.
 
 Workspace file management commands:
   download  Download workspace files.
   du        Get workspace disk usage.
   ls        List workspace files.
   mv        Move files within workspace.
+  prune     Prune workspace files.
   rm        Delete files from workspace.
   upload    Upload files and directories to workspace.
 
 Workspace file retention commands:
   retention-rules-list  List the retention rules for a workflow.
 
 Secret management commands:
```

### Comparing `reana-client-0.9.0a8/docs/conf.py` & `reana-client-0.9.1a1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "reana"
-copyright = "2017-2020 info@reana.io"
+copyright = "2017-2023 info@reana.io"
 author = "info@reana.io"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
```

### Comparing `reana-client-0.9.0a8/docs/index.rst` & `reana-client-0.9.1a1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `reana-client-0.9.0a8/reana_client/api/client.py` & `reana-client-0.9.1a1/reana_client/api/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1087,7 +1087,36 @@
             "Workflow retention rules could not be retrieved: "
             "\nStatus: {}\nReason: {}\n"
             "Message: {}".format(
                 e.response.status_code, e.response.reason, e.response.json()["message"]
             )
         )
         raise Exception(e.response.json()["message"])
+
+
+def prune_workspace(workflow, include_inputs, include_outputs, access_token):
+    """Prune workspace files."""
+    try:
+        (response, http_response) = current_rs_api_client.api.prune_workspace(
+            workflow_id_or_name=workflow,
+            include_inputs=include_inputs,
+            include_outputs=include_outputs,
+            access_token=access_token,
+        ).result()
+
+        if http_response.status_code == 200:
+            return response
+        else:
+            raise Exception(
+                "Expected status code 200 but replied with "
+                "{status_code}".format(status_code=http_response.status_code)
+            )
+
+    except HTTPError as e:
+        logging.debug(
+            "Workspace could not be pruned: "
+            "\nStatus: {}\nReason: {}\n"
+            "Message: {}".format(
+                e.response.status_code, e.response.reason, e.response.json()["message"]
+            )
+        )
+        raise Exception(e.response.json()["message"])
```

### Comparing `reana-client-0.9.0a8/reana_client/api/utils.py` & `reana-client-0.9.1a1/reana_client/api/utils.py`

 * *Files identical despite different names*

### Comparing `reana-client-0.9.0a8/reana_client/cli/__init__.py` & `reana-client-0.9.1a1/reana_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `reana-client-0.9.0a8/reana_client/cli/cwl_runner.py` & `reana-client-0.9.1a1/reana_client/cli/cwl_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,14 @@
         first_logs = ""
         while True:
             sleep(1)
             logging.error("Polling workflow logs")
             response = get_workflow_logs(workflow_id, access_token)
             logs = response["logs"]
             if logs != first_logs:
-
                 logging.error(logs[len(first_logs) :])
                 first_logs = logs
 
             if (
                 "Final process status" in logs
                 or "Traceback (most recent call last)" in logs
             ):
```

### Comparing `reana-client-0.9.0a8/reana_client/cli/files.py` & `reana-client-0.9.1a1/reana_client/cli/files.py`

 * *Files 3% similar despite different names*

```diff
@@ -530,14 +530,64 @@
     except Exception as e:
         logging.debug(traceback.format_exc())
         logging.debug(str(e))
         display_message("Something went wrong. {}".format(e), msg_type="error")
         sys.exit(1)
 
 
+@files_group.command("prune")
+@check_connection
+@add_workflow_option
+@add_access_token_options
+@click.option(
+    "--include-inputs",
+    "include_inputs",
+    is_flag=True,
+    help="Delete also the input files of the workflow. Note that this includes the workflow specification file.",
+)
+@click.option(
+    "--include-outputs",
+    "include_outputs",
+    is_flag=True,
+    help="Delete also the output files of the workflow.",
+)
+@click.pass_context
+def prune_files(
+    ctx, workflow, access_token, include_inputs, include_outputs
+):  # noqa: D301
+    """Prune workspace files.
+
+    The ``prune`` command deletes all the intermediate files of a given workflow that are not present
+    in the input or output section of the workflow specification.
+
+    Examples:\n
+    \t $ reana-client prune -w myanalysis.42\n
+    \t $ reana-client prune -w myanalysis.42 --include-inputs
+    """
+    from reana_client.api.client import prune_workspace
+
+    logging.debug("command: {}".format(ctx.command_path.replace(" ", ".")))
+    for p in ctx.params:
+        logging.debug("{param}: {value}".format(param=p, value=ctx.params[p]))
+
+    try:
+        response = prune_workspace(
+            workflow, include_inputs, include_outputs, access_token
+        )
+        display_message(response["message"], msg_type="success")
+    except Exception as e:
+        logging.debug(traceback.format_exc())
+        logging.debug(str(e))
+        display_message(
+            "Workspace could not be pruned: \n{}".format(e),
+            msg_type="error",
+        )
+        sys.exit(1)
+
+
 @files_group.command("du")
 @add_workflow_option
 @check_connection
 @add_access_token_options
 @click.option("-s", "--summarize", is_flag=True, help="Display total.")
 @click.option(
     "--filter",
@@ -551,15 +601,15 @@
 @human_readable_or_raw_option
 @click.pass_context
 def workflow_disk_usage(
     ctx, workflow, access_token, summarize, filters, human_readable_or_raw
 ):  # noqa: D301
     """Get workspace disk usage.
 
-    The ``du`` command allows to chech the disk usage of given workspace.
+    The ``du`` command allows to check the disk usage of given workspace.
 
     Examples:\n
     \t $ reana-client du -w myanalysis.42 -s\n
     \t $ reana-client du -w myanalysis.42 -s --human-readable\n
     \t $ reana-client du -w myanalysis.42 --filter name=data/
     """
     from reana_client.api.client import get_workflow_disk_usage
```

### Comparing `reana-client-0.9.0a8/reana_client/cli/ping.py` & `reana-client-0.9.1a1/reana_client/cli/ping.py`

 * *Files identical despite different names*

### Comparing `reana-client-0.9.0a8/reana_client/cli/quotas.py` & `reana-client-0.9.1a1/reana_client/cli/quotas.py`

 * *Files identical despite different names*

### Comparing `reana-client-0.9.0a8/reana_client/cli/retention_rules.py` & `reana-client-0.9.1a1/reana_client/cli/retention_rules.py`

 * *Files identical despite different names*

### Comparing `reana-client-0.9.0a8/reana_client/cli/secrets.py` & `reana-client-0.9.1a1/reana_client/cli/secrets.py`

 * *Files identical despite different names*

### Comparing `reana-client-0.9.0a8/reana_client/cli/utils.py` & `reana-client-0.9.1a1/reana_client/cli/utils.py`

 * *Files identical despite different names*

### Comparing `reana-client-0.9.0a8/reana_client/cli/workflow.py` & `reana-client-0.9.1a1/reana_client/cli/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of REANA.
-# Copyright (C) 2017, 2018, 2019, 2020, 2021, 2022 CERN.
+# Copyright (C) 2017, 2018, 2019, 2020, 2021, 2022, 2023 CERN.
 #
 # REANA is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 """REANA client workflow related commands."""
 
 import json
 import logging
@@ -240,15 +240,14 @@
         if verbose or include_progress:
             headers[type] += progress_header
         if verbose or include_duration:
             headers[type] += duration_header
 
         data = []
         for workflow in response:
-            workflow["size"] = workflow["size"][human_readable_or_raw]
             name, run_number = get_workflow_name_and_run_number(workflow["name"])
             workflow["name"] = name
             workflow["run_number"] = run_number
             workflow["duration"] = get_workflow_duration(workflow)
             if type == "interactive":
                 workflow["session_uri"] = format_session_uri(
                     reana_server_url=ctx.obj.reana_server_url,
@@ -267,27 +266,38 @@
                     value = workflow.get("progress", {}).get(_key) or "-"
                 if not value:
                     value = workflow.get(header)
                 row.append(value)
             data.append(row)
 
         # Sort by given column, making sure that `None` is at the bottom of the list.
+        def get_sort_key(x, column_id):
+            if sort_columm_name == "run_number":
+                return list(map(int, x[column_id].split(".")))
+            elif sort_columm_name in workspace_size_header:
+                return x[column_id]["raw"]
+            return x[column_id] is not None, x[column_id]
+
         sort_column_id = 2
         if sort_columm_name.lower() in headers[type]:
             sort_column_id = headers[type].index(sort_columm_name.lower())
         data = sorted(
             data,
-            key=lambda x: (x[sort_column_id] is not None, x[sort_column_id]),
+            key=lambda x: get_sort_key(x, sort_column_id),
             reverse=True,
         )
 
-        # Substitute `None` with "-"
         for row in data:
             for i, value in enumerate(row):
-                row[i] = value or "-"
+                # Substitute `None` with "-"
+                content = value or "-"
+                # Replace raw size with human-readable size if requested
+                if headers[type][i] in workspace_size_header:
+                    content = value.get(human_readable_or_raw)
+                row[i] = content
 
         workflow_ids = ["{0}.{1}".format(w[0], w[1]) for w in data]
         if os.getenv("REANA_WORKON", "") in workflow_ids:
             active_workflow_idx = workflow_ids.index(os.getenv("REANA_WORKON", ""))
             data[active_workflow_idx][headers[type].index("run_number")] += " *"
 
         display_formatted_output(data, headers[type], _format, output_format)
@@ -352,35 +362,47 @@
     # Check that name is not an UUIDv4.
     # Otherwise it would mess up `--workflow` flag usage because no distinction
     # could be made between the name and actual UUID of workflow.
     if is_uuid_v4(name):
         display_message("Workflow name cannot be a valid UUIDv4", msg_type="error")
         sys.exit(1)
 
+    specification_filename = click.format_filename(file)
+
     try:
         reana_specification = load_validate_reana_spec(
-            click.format_filename(file),
+            specification_filename,
             access_token=access_token,
             skip_validation=skip_validation,
             server_capabilities=True,
         )
         logging.info("Connecting to {0}".format(get_api_url()))
         response = create_workflow(reana_specification, name, access_token)
-        click.echo(click.style(response["workflow_name"], fg="green"))
+        workflow_name = response["workflow_name"]
+
+        click.echo(click.style(workflow_name, fg="green"))
         # check if command is called from wrapper command
         if "invoked_by_subcommand" in ctx.parent.__dict__:
-            ctx.parent.workflow_name = response["workflow_name"]
+            ctx.parent.workflow_name = workflow_name
     except Exception as e:
         logging.debug(traceback.format_exc())
         logging.debug(str(e))
         display_message(
             "Cannot create workflow {}: \n{}".format(name, str(e)), msg_type="error"
         )
         sys.exit(1)
 
+    # upload specification file by default
+    ctx.invoke(
+        upload_files,
+        workflow=workflow_name,
+        filenames=(specification_filename,),
+        access_token=access_token,
+    )
+
 
 @workflow_execution_group.command("start")
 @add_workflow_option
 @add_access_token_options
 @check_connection
 @click.option(
     "-p",
@@ -574,69 +596,78 @@
 
     parsed_parameters = {
         "input_parameters": parameters,
         "operational_options": options,
         "restart": True,
     }
     if file:
+        specification_filename = click.format_filename(file)
         parsed_parameters["reana_specification"] = load_validate_reana_spec(
             click.format_filename(file)
         )
-    if workflow:
-        if parameters or options:
-            try:
-                if "reana_specification" in parsed_parameters:
-                    workflow_type = parsed_parameters["reana_specification"][
-                        "workflow"
-                    ]["type"]
-                    original_parameters = (
-                        parsed_parameters["reana_specification"]
-                        .get("inputs", {})
-                        .get("parameters", {})
-                    )
-                else:
-                    response = get_workflow_parameters(workflow, access_token)
-                    workflow_type = response["type"]
-                    original_parameters = response["parameters"]
+        # upload new specification
+        ctx.invoke(
+            upload_files,
+            workflow=workflow,
+            filenames=(specification_filename,),
+            access_token=access_token,
+        )
 
-                parsed_parameters["operational_options"] = validate_operational_options(
-                    workflow_type, parsed_parameters["operational_options"]
-                )
-                parsed_parameters["input_parameters"] = validate_input_parameters(
-                    parsed_parameters["input_parameters"], original_parameters
+    if parameters or options:
+        try:
+            if "reana_specification" in parsed_parameters:
+                workflow_type = parsed_parameters["reana_specification"]["workflow"][
+                    "type"
+                ]
+                original_parameters = (
+                    parsed_parameters["reana_specification"]
+                    .get("inputs", {})
+                    .get("parameters", {})
                 )
+            else:
+                response = get_workflow_parameters(workflow, access_token)
+                workflow_type = response["type"]
+                original_parameters = response["parameters"]
 
-            except REANAValidationError as e:
-                display_message(e.message, msg_type="error")
-                sys.exit(1)
-            except Exception as e:
-                display_message(
-                    "Could not apply given input parameters: "
-                    "{0} \n{1}".format(parameters, str(e)),
-                    msg_type="error",
-                )
-                sys.exit(1)
-        try:
-            logging.info("Connecting to {0}".format(get_api_url()))
-            response = start_workflow(workflow, access_token, parsed_parameters)
-            workflow = response["workflow_name"] + "." + str(response["run_number"])
-            current_status = get_workflow_status(workflow, access_token).get("status")
-            display_message(
-                get_workflow_status_change_msg(workflow, current_status),
-                msg_type="success",
+            parsed_parameters["operational_options"] = validate_operational_options(
+                workflow_type, parsed_parameters["operational_options"]
             )
+            parsed_parameters["input_parameters"] = validate_input_parameters(
+                parsed_parameters["input_parameters"], original_parameters
+            )
+
+        except REANAValidationError as e:
+            display_message(e.message, msg_type="error")
+            sys.exit(1)
         except Exception as e:
-            logging.debug(traceback.format_exc())
-            logging.debug(str(e))
             display_message(
-                "Cannot start workflow {}: \n{}".format(workflow, str(e)),
+                "Could not apply given input parameters: "
+                "{0} \n{1}".format(parameters, str(e)),
                 msg_type="error",
             )
             sys.exit(1)
 
+    try:
+        logging.info("Connecting to {0}".format(get_api_url()))
+        response = start_workflow(workflow, access_token, parsed_parameters)
+        workflow = response["workflow_name"] + "." + str(response["run_number"])
+        current_status = get_workflow_status(workflow, access_token).get("status")
+        display_message(
+            get_workflow_status_change_msg(workflow, current_status),
+            msg_type="success",
+        )
+    except Exception as e:
+        logging.debug(traceback.format_exc())
+        logging.debug(str(e))
+        display_message(
+            "Cannot start workflow {}: \n{}".format(workflow, str(e)),
+            msg_type="error",
+        )
+        sys.exit(1)
+
 
 @workflow_execution_group.command("status")
 @add_workflow_option
 @click.option(
     "--format",
     "_format",
     multiple=True,
@@ -1150,15 +1181,16 @@
 @click.pass_context
 def workflow_delete(
     ctx, workflow: str, all_runs: bool, should_delete_workspace: bool, access_token: str
 ):  # noqa: D301
     """Delete a workflow.
 
     The ``delete`` command removes workflow run(s) from the database.
-    Note that the workspace will always be deleted, even when ``--include-workspace`` is not specified.
+    Note that the workspace and any open session attached to it will always be
+    deleted, even when ``--include-workspace`` is not specified.
     Note also that you can remove all past runs of a workflow by specifying ``--include-all-runs`` flag.
 
     Example:\n
     \t $ reana-client delete -w myanalysis.42\n
     \t $ reana-client delete -w myanalysis.42 --include-all-runs
     """
     from reana_client.api.client import delete_workflow
```

### Comparing `reana-client-0.9.0a8/reana_client/config.py` & `reana-client-0.9.1a1/reana_client/config.py`

 * *Files identical despite different names*

### Comparing `reana-client-0.9.0a8/reana_client/errors.py` & `reana-client-0.9.1a1/reana_client/errors.py`

 * *Files identical despite different names*

### Comparing `reana-client-0.9.0a8/reana_client/printer.py` & `reana-client-0.9.1a1/reana_client/printer.py`

 * *Files identical despite different names*

### Comparing `reana-client-0.9.0a8/reana_client/utils.py` & `reana-client-0.9.1a1/reana_client/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,14 +134,15 @@
 def get_workflow_duration(workflow: Dict) -> Optional[int]:
     """Calculate the duration of the workflow.
 
     :param workflow: Workflow details returned by the server.
     :return: The duration of the workflow in seconds or ``None`` if the starting
         time is not present.
     """
+
     # FIXME: Use datetime.fromisoformat when moving to Python 3.7 or higher
     def fromisoformat(date_string):
         return datetime.strptime(date_string, "%Y-%m-%dT%H:%M:%S")
 
     progress = workflow.get("progress", {})
     run_started_at = progress.get("run_started_at")
     run_finished_at = progress.get("run_finished_at")
```

### Comparing `reana-client-0.9.0a8/reana_client/validation/compute_backends.py` & `reana-client-0.9.1a1/reana_client/validation/compute_backends.py`

 * *Files identical despite different names*

### Comparing `reana-client-0.9.0a8/reana_client/validation/environments.py` & `reana-client-0.9.1a1/reana_client/validation/environments.py`

 * *Files identical despite different names*

### Comparing `reana-client-0.9.0a8/reana_client/validation/parameters.py` & `reana-client-0.9.1a1/reana_client/validation/parameters.py`

 * *Files identical despite different names*

### Comparing `reana-client-0.9.0a8/reana_client/validation/utils.py` & `reana-client-0.9.1a1/reana_client/validation/utils.py`

 * *Files identical despite different names*

### Comparing `reana-client-0.9.0a8/reana_client/validation/workspace.py` & `reana-client-0.9.1a1/reana_client/validation/workspace.py`

 * *Files identical despite different names*

### Comparing `reana-client-0.9.0a8/reana_client.egg-info/PKG-INFO` & `reana-client-0.9.1a1/reana_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reana-client
-Version: 0.9.0a8
+Version: 0.9.1a1
 Summary: REANA client
 Home-page: https://github.com/reanahub/reana-client
 Author: REANA
 Author-email: info@reana.io
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
@@ -97,40 +97,45 @@
 - `REANA-Client known issues <https://github.com/reanahub/reana-client/issues>`_
 - `REANA-Client source code <https://github.com/reanahub/reana-client>`_
 
 
 Changes
 =======
 
-Version 0.9.0 (UNRELEASED)
+Version 0.9.1 (UNRELEASED)
+--------------------------
+
+- Adds ``prune`` command to delete all intermediate files of a given workflow.
+- Fixes ``list`` command to correctly list workflows when sorting them by their run number or by the size of their workspace.
+- Fixes ``du`` command help message typo.
+
+Version 0.9.0 (2023-01-26)
 --------------------------
 
 - Adds support for Python 3.11.
-- Adds support for ``.reanaignore`` during file upload. Files that match ``.reanaignore`` will not be uploaded.
-- Adds support for ``.gitignore`` during file upload. Files that match ``.gitignore`` will not be uploaded.
+- Adds support for ``.gitignore`` and ``.reanaignore`` to specify files that should not be uploaded to REANA.
 - Adds ``retention-rules-list`` command to list the retention rules of a workflow.
-- Changes ``delete`` CLI command to always delete workspace.
-- Changes ``delete_workflow`` API method to always delete workspace.
-- Changes ``list`` to hide deleted workflows by default.
+- Changes REANA specification loading and validation functionalities by porting some of the logic to ``reana-commons``.
+- Changes ``create`` and ``restart`` commands to always upload the REANA specification file.
+- Changes ``delete`` command to always delete the workflow's workspace.
+- Changes ``delete_workflow`` Python API function to always delete the workflow's workspace.
+- Changes ``download`` command to add the possibility to write files to the standard output via ``-o -`` option.
+- Changes ``list`` command to hide deleted workflows by default.
 - Changes ``list`` command to allow displaying deleted workflows via ``--all`` and ``--show-deleted-runs`` options.
-- Changes ``list`` command to allow displaying the duration of workflows with the ``--include-duration`` option.
-- Changes ``status`` command to allow displaying the duration of workflows with the ``--include-duration`` option.
-- Changes REANA specification loading and validation functionality by porting some of the logic to ``reana-commons``.
+- Changes ``list`` and ``status`` commands to allow displaying the duration of workflows with the ``--include-duration`` option.
 - Changes ``mv`` command to allow moving files while a workflow is running.
 - Changes ``upload`` command to prevent uploading symlinks.
-- Fixes ``validate --environment`` command to detect illegal white space characters in image names.
+- Changes ``validation --environment`` command to use Docker registry v2 APIs to check that a Docker image exists in DockerHub.
 - Fixes ``list`` command to highlight the workflow specified in ``REANA_WORKON`` correctly.
 - Fixes ``secrets-delete`` command error message when deleting non existing secrets.
-- Fixes ``upload`` command to report in case input directories are listed under files and vice versa.
-
-Version 0.8.2 (UNRELEASED)
---------------------------
-
-- Changes ``download`` command to add the possibility to write files to the standard output via ``-o -`` option.
+- Fixes ``start`` command to report failed workflows as errors.
 - Fixes ``start`` and ``run`` commands to correctly follow the execution of the workflow until termination.
+- Fixes ``status`` command to respect output format provided by the ``--format`` option.
+- Fixes ``upload`` command to report when input directories are listed under the ``files`` section in the REANA specification file and vice versa.
+- Fixes ``validate --environment`` command to detect illegal whitespace characters in Docker image names.
 
 Version 0.8.1 (2022-02-15)
 --------------------------
 
 - Adds support for creating reana-client standalone AppImage executables.
 - Adds support for Python 3.10.
 - Adds workflow name validation for ``create_workflow_from_json()`` Python API function.
```

### Comparing `reana-client-0.9.0a8/reana_client.egg-info/SOURCES.txt` & `reana-client-0.9.1a1/reana_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reana-client-0.9.0a8/run-tests.sh` & `reana-client-0.9.1a1/run-tests.sh`

 * *Files identical despite different names*

### Comparing `reana-client-0.9.0a8/scripts/create-appimage.sh` & `reana-client-0.9.1a1/scripts/create-appimage.sh`

 * *Files identical despite different names*

### Comparing `reana-client-0.9.0a8/scripts/generate_cli_api.py` & `reana-client-0.9.1a1/scripts/generate_cli_api.py`

 * *Files identical despite different names*

### Comparing `reana-client-0.9.0a8/setup.py` & `reana-client-0.9.1a1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of REANA.
-# Copyright (C) 2017, 2018, 2019, 2020, 2021, 2022 CERN.
+# Copyright (C) 2017, 2018, 2019, 2020, 2021, 2022, 2023 CERN.
 #
 # REANA is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """REANA client"""
 
 from __future__ import absolute_import, print_function
@@ -15,15 +15,15 @@
 
 from setuptools import find_packages, setup
 
 readme = open("README.rst").read()
 history = open("CHANGES.rst").read()
 
 tests_require = [
-    "pytest-reana>=0.9.0a7,<0.10.0",
+    "pytest-reana>=0.9.0,<0.10.0",
 ]
 
 extras_require = {
     "docs": [
         "Sphinx>=1.5.1",
         "sphinx-rtd-theme>=0.1.9",
         "sphinx-click>=1.0.4",
@@ -41,15 +41,15 @@
     "pytest-runner>=2.7",
 ]
 
 install_requires = [
     "click>=7",
     "pathspec==0.9.0",
     "jsonpointer>=2.0",
-    "reana-commons[yadage,snakemake,cwl]>=0.9.0a16,<0.10.0",
+    "reana-commons[yadage,snakemake,cwl]>=0.9.3a2,<0.10.0",
     "tablib>=0.12.1,<0.13",
     "werkzeug>=0.14.1 ; python_version<'3.10'",
     "werkzeug>=0.15.0 ; python_version>='3.10'",
     "swagger_spec_validator>=2.4.0,<3.0.0; python_version<'3.7'",
 ]
 
 packages = find_packages()
```

### Comparing `reana-client-0.9.0a8/tests/conftest.py` & `reana-client-0.9.1a1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `reana-client-0.9.0a8/tests/test_cli_files.py` & `reana-client-0.9.1a1/tests/test_cli_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -630,7 +630,41 @@
             )
             json_response = json.loads(result.output)
             assert result.exit_code == 0
             assert isinstance(json_response, list)
             assert len(json_response) == 3
             assert json_response[0]["name"] in response["items"][0]["name"]
             assert "2021-06-14" in json_response[1]["last-modified"]
+
+
+def test_prune_workspace():
+    """Test prune workspace files."""
+    status_code = 200
+    response = {
+        "message": "The workspace has been correctly pruned.",
+        "workflow_id": "string",
+        "workflow_name": "string",
+    }
+    env = {"REANA_SERVER_URL": "localhost"}
+    mock_http_response, mock_response = Mock(), Mock()
+    mock_http_response.status_code = status_code
+    mock_response = response
+    reana_token = "000000"
+    runner = CliRunner(env=env)
+    with runner.isolation():
+        with patch(
+            "reana_client.api.client.current_rs_api_client",
+            make_mock_api_client("reana-server")(mock_response, mock_http_response),
+        ):
+            result = runner.invoke(
+                cli,
+                [
+                    "prune",
+                    "-t",
+                    reana_token,
+                    "--workflow",
+                    "test-worflow.1",
+                    "--include-outputs",
+                ],
+            )
+            assert result.exit_code == 0
+            assert response["message"] in result.output
```

### Comparing `reana-client-0.9.0a8/tests/test_cli_ping.py` & `reana-client-0.9.1a1/tests/test_cli_ping.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,13 +60,12 @@
     mock_response = response
     runner = CliRunner(env=env)
     with runner.isolation():
         with patch(
             "reana_client.api.client.current_rs_api_client",
             make_mock_api_client("reana-server")(mock_response, mock_http_response),
         ):
-
             result = runner.invoke(cli, ["ping", "-t", reana_token])
             message = "Authenticated as: John Doe <johndoe@example.org>"
             assert message in result.output
             message = "Connected"
             assert message in result.output
```

### Comparing `reana-client-0.9.0a8/tests/test_cli_retention_rules.py` & `reana-client-0.9.1a1/tests/test_cli_retention_rules.py`

 * *Files identical despite different names*

### Comparing `reana-client-0.9.0a8/tests/test_cli_secrets.py` & `reana-client-0.9.1a1/tests/test_cli_secrets.py`

 * *Files identical despite different names*

### Comparing `reana-client-0.9.0a8/tests/test_cli_workflows.py` & `reana-client-0.9.1a1/tests/test_cli_workflows.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,61 +110,91 @@
         with patch("reana_client.api.client.get_workflows") as mock_get_workflows:
             mock_get_workflows.return_value = response
             runner.invoke(cli, ["list", "-t", reana_token] + cli_options)
             kwargs = mock_get_workflows.call_args.kwargs
             assert kwargs["status"] == expected_status_filter
 
 
-def test_workflows_sorting():
+@pytest.mark.parametrize(
+    "cli_options, expected_output",
+    [
+        (
+            ["list", "-t", "000000", "--sort", "run_number"],
+            (
+                "mytest   15           2018-06-13T10:55:37   -                     -                     running\n"
+                "mytest   2            2018-06-13T09:55:35   -                     -                     running\n"
+                "mytest   1 *          2018-06-13T09:47:35   2018-06-13T09:47:40   2018-06-13T10:30:03   running"
+            ),
+        ),
+        (
+            [
+                "list",
+                "-t",
+                "000000",
+                "--include-workspace-size",
+                "-h",
+                "--sort",
+                "size",
+            ],
+            (
+                "mytest   1 *          2018-06-13T09:47:35   2018-06-13T09:47:40   2018-06-13T10:30:03   running   1.55 MiB\n"
+                "mytest   2            2018-06-13T09:55:35   -                     -                     running   540 KiB \n"
+                "mytest   15           2018-06-13T10:55:37   -                     -                     running   192 KiB "
+            ),
+        ),
+    ],
+)
+def test_workflows_sorting(cli_options: List[str], expected_output: str):
     """Test workflows sorting."""
     response = {
         "items": [
             {
                 "status": "running",
                 "created": "2018-06-13T09:47:35",
                 "user": "00000000-0000-0000-0000-000000000000",
                 "name": "mytest.1",
                 "id": "256b25f4-4cfb-4684-b7a8-73872ef455a1",
                 "progress": {
                     "run_started_at": "2018-06-13T09:47:40",
                     "run_finished_at": "2018-06-13T10:30:03",
                 },
-                "size": {"raw": 0, "human_readable": "0 Bytes"},
+                "size": {"raw": 1622016, "human_readable": "1.55 MiB"},
             },
             {
                 "status": "running",
                 "created": "2018-06-13T09:55:35",
                 "user": "00000000-0000-0000-0000-000000000000",
                 "name": "mytest.2",
                 "id": "256b25f4-4cfb-4684-b7a8-73872ef455a2",
-                "size": {"raw": 0, "human_readable": "0 Bytes"},
+                "size": {"raw": 552960, "human_readable": "540 KiB"},
+            },
+            {
+                "status": "running",
+                "created": "2018-06-13T10:55:37",
+                "user": "00000000-0000-0000-0000-000000000000",
+                "name": "mytest.15",
+                "id": "256b25f4-4cfb-4684-b7a8-73872ef455a3",
+                "size": {"raw": 196608, "human_readable": "192 KiB"},
             },
         ]
     }
     status_code = 200
     mock_http_response, mock_response = Mock(), Mock()
     mock_http_response.status_code = status_code
     mock_response = response
     env = {"REANA_SERVER_URL": "localhost", "REANA_WORKON": "mytest.1"}
-    reana_token = "000000"
     runner = CliRunner(env=env)
     with runner.isolation():
         with patch(
             "reana_client.api.client.current_rs_api_client",
             make_mock_api_client("reana-server")(mock_response, mock_http_response),
         ):
-            result = runner.invoke(
-                cli, ["list", "-t", reana_token, "--sort", "run_number"]
-            )
-            message = (
-                "mytest   2            2018-06-13T09:55:35   -                     -                     running\n"
-                "mytest   1 *          2018-06-13T09:47:35   2018-06-13T09:47:40   2018-06-13T10:30:03   running"
-            )
+            result = runner.invoke(cli, cli_options)
             assert result.exit_code == 0
-            assert message in result.output
+            assert expected_output in result.output
 
 
 def test_workflows_sessions():
     """Test list command for getting interactive sessions."""
     response = {
         "items": [
             {
@@ -481,24 +511,27 @@
     mock_http_response.status_code = status_code
     mock_response = response
     runner = CliRunner(env=env)
     with runner.isolation():
         with patch(
             "reana_client.api.client.current_rs_api_client",
             make_mock_api_client("reana-server")(mock_response, mock_http_response),
-        ):
+        ), patch("reana_client.api.client.requests.post") as upload_request:
             with runner.isolated_filesystem():
                 with open("reana.yaml", "w") as f:
                     f.write(create_yaml_workflow_schema)
                 result = runner.invoke(
                     cli, ["create", "-t", reana_token, "--skip-validation"]
                 )
                 assert result.exit_code == 0
                 assert response["workflow_name"] in result.output
 
+                upload_request.assert_called_once()
+                assert "File /reana.yaml was successfully uploaded." in result.output
+
 
 def test_workflow_create_not_valid_name(create_yaml_workflow_schema):
     """Test workflow create when creation is successfull."""
     env = {"REANA_SERVER_URL": "localhost"}
     illegal_workflow_name = "workflow.name"
     runner = CliRunner(env=env)
     result = runner.invoke(cli, ["create", "-n", illegal_workflow_name])
```

### Comparing `reana-client-0.9.0a8/tests/test_utils.py` & `reana-client-0.9.1a1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `reana-client-0.9.0a8/tests/test_validate_compute_backends.py` & `reana-client-0.9.1a1/tests/test_validate_compute_backends.py`

 * *Files identical despite different names*

### Comparing `reana-client-0.9.0a8/tests/test_validate_environments.py` & `reana-client-0.9.1a1/tests/test_validate_environments.py`

 * *Files identical despite different names*

### Comparing `reana-client-0.9.0a8/tests/test_validate_parameters.py` & `reana-client-0.9.1a1/tests/test_validate_parameters.py`

 * *Files identical despite different names*

### Comparing `reana-client-0.9.0a8/tests/test_validate_server_capabilities.py` & `reana-client-0.9.1a1/tests/test_validate_server_capabilities.py`

 * *Files identical despite different names*

