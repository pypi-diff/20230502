# Comparing `tmp/cortex_cli-1.13.0.tar.gz` & `tmp/cortex_cli-1.13.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cortex_cli-1.13.0.tar", last modified: Mon May  1 20:31:39 2023, max compression
+gzip compressed data, was "cortex_cli-1.13.1.post1.tar", last modified: Tue May  2 20:19:39 2023, max compression
```

## Comparing `cortex_cli-1.13.0.tar` & `cortex_cli-1.13.1.post1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 20:31:39.275137 cortex_cli-1.13.0/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      260 2023-05-01 20:31:39.275137 cortex_cli-1.13.0/PKG-INFO
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     5211 2023-04-28 14:58:42.000000 cortex_cli-1.13.0/README.md
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 20:31:39.275137 cortex_cli-1.13.0/cortex_cli/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       22 2023-05-01 20:31:08.000000 cortex_cli-1.13.0/cortex_cli/__init__.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 20:31:39.275137 cortex_cli-1.13.0/cortex_cli/cli/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 23:15:18.000000 cortex_cli-1.13.0/cortex_cli/cli/__init__.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 20:31:39.275137 cortex_cli-1.13.0/cortex_cli/cli/api/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.13.0/cortex_cli/cli/api/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3992 2023-04-27 21:54:12.000000 cortex_cli-1.13.0/cortex_cli/cli/api/github_api.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      575 2023-03-09 15:57:05.000000 cortex_cli-1.13.0/cortex_cli/cli/api/http_api.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2789 2023-03-16 20:39:49.000000 cortex_cli-1.13.0/cortex_cli/cli/cli_api_base.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2792 2023-03-16 20:39:49.000000 cortex_cli-1.13.0/cortex_cli/cli/cli_api_base_config.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       90 2023-03-09 15:57:05.000000 cortex_cli-1.13.0/cortex_cli/cli/clients.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2027 2023-04-28 14:57:33.000000 cortex_cli-1.13.0/cortex_cli/cli/configure.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      971 2023-03-16 20:39:49.000000 cortex_cli-1.13.0/cortex_cli/cli/cortex_cli.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      994 2023-03-16 20:39:49.000000 cortex_cli-1.13.0/cortex_cli/cli/generic_get.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1005 2023-03-09 15:57:05.000000 cortex_cli-1.13.0/cortex_cli/cli/inferences.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    24829 2023-05-01 19:43:06.000000 cortex_cli-1.13.0/cortex_cli/cli/models.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3248 2023-04-07 17:56:26.000000 cortex_cli-1.13.0/cortex_cli/cli/pipelines.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 20:31:39.275137 cortex_cli-1.13.0/cortex_cli/core/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.13.0/cortex_cli/core/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     4182 2023-04-17 18:14:34.000000 cortex_cli-1.13.0/cortex_cli/core/cortex_data.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3648 2023-03-09 15:57:05.000000 cortex_cli-1.13.0/cortex_cli/core/drift_checks.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    11022 2023-04-17 18:14:34.000000 cortex_cli-1.13.0/cortex_cli/core/ethics_checks.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 20:31:39.275137 cortex_cli-1.13.0/cortex_cli/core/mlflow/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.13.0/cortex_cli/core/mlflow/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    13976 2023-03-09 15:57:05.000000 cortex_cli-1.13.0/cortex_cli/core/mlflow/mlflow_cortex.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 20:31:39.275137 cortex_cli-1.13.0/cortex_cli/core/models/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.13.0/cortex_cli/core/models/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     8121 2023-04-20 17:50:53.000000 cortex_cli-1.13.0/cortex_cli/core/models/cortex_model.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2828 2023-04-25 18:48:24.000000 cortex_cli-1.13.0/cortex_cli/core/secrets_manager.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 20:31:39.275137 cortex_cli-1.13.0/cortex_cli/model_templates/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.0/cortex_cli/model_templates/__init__.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 20:31:39.275137 cortex_cli-1.13.0/cortex_cli/model_templates/chatgpt_model/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-04-25 18:48:24.000000 cortex_cli-1.13.0/cortex_cli/model_templates/chatgpt_model/.gitignore
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-04-25 18:48:24.000000 cortex_cli-1.13.0/cortex_cli/model_templates/chatgpt_model/README.md
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.0/cortex_cli/model_templates/chatgpt_model/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      301 2023-04-25 18:48:24.000000 cortex_cli-1.13.0/cortex_cli/model_templates/chatgpt_model/cookiecutter.json
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-04-25 18:48:24.000000 cortex_cli-1.13.0/cortex_cli/model_templates/chatgpt_model/requirements.txt
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 20:31:39.275137 cortex_cli-1.13.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-04-25 18:48:24.000000 cortex_cli-1.13.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/.gitignore
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1645 2023-04-27 21:53:57.000000 cortex_cli-1.13.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/README.md
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      162 2023-04-25 18:48:24.000000 cortex_cli-1.13.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/conda.yml
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      322 2023-04-25 18:48:24.000000 cortex_cli-1.13.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/cortex.yml
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 20:31:39.275137 cortex_cli-1.13.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/data/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/data/.gitkeep
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 20:31:39.275137 cortex_cli-1.13.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/notebooks/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/notebooks/.gitkeep
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 20:31:39.275137 cortex_cli-1.13.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 20:31:39.275137 cortex_cli-1.13.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1654 2023-04-25 18:48:24.000000 cortex_cli-1.13.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 20:31:39.275137 cortex_cli-1.13.0/cortex_cli/model_templates/digits_model/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-04-25 18:48:24.000000 cortex_cli-1.13.0/cortex_cli/model_templates/digits_model/.gitignore
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-04-25 18:48:24.000000 cortex_cli-1.13.0/cortex_cli/model_templates/digits_model/README.md
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.0/cortex_cli/model_templates/digits_model/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      301 2023-04-25 18:48:24.000000 cortex_cli-1.13.0/cortex_cli/model_templates/digits_model/cookiecutter.json
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-04-25 18:48:24.000000 cortex_cli-1.13.0/cortex_cli/model_templates/digits_model/requirements.txt
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 20:31:39.275137 cortex_cli-1.13.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-04-25 18:48:24.000000 cortex_cli-1.13.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/.gitignore
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1645 2023-04-27 21:54:07.000000 cortex_cli-1.13.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/README.md
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      162 2023-04-25 18:48:24.000000 cortex_cli-1.13.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/conda.yml
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      455 2023-04-25 18:48:24.000000 cortex_cli-1.13.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/cortex.yml
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 20:31:39.275137 cortex_cli-1.13.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/data/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/data/.gitkeep
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 20:31:39.275137 cortex_cli-1.13.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/notebooks/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/notebooks/.gitkeep
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 20:31:39.275137 cortex_cli-1.13.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 20:31:39.275137 cortex_cli-1.13.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2377 2023-04-25 18:48:24.000000 cortex_cli-1.13.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 20:31:39.275137 cortex_cli-1.13.0/cortex_cli/tests/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.13.0/cortex_cli/tests/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1801 2023-03-09 15:57:05.000000 cortex_cli-1.13.0/cortex_cli/tests/test_cortex_data.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1825 2023-03-09 15:57:05.000000 cortex_cli-1.13.0/cortex_cli/tests/test_ethics_checks.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-01 20:31:39.275137 cortex_cli-1.13.0/cortex_cli.egg-info/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      260 2023-05-01 20:31:39.000000 cortex_cli-1.13.0/cortex_cli.egg-info/PKG-INFO
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3123 2023-05-01 20:31:39.000000 cortex_cli-1.13.0/cortex_cli.egg-info/SOURCES.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        1 2023-05-01 20:31:39.000000 cortex_cli-1.13.0/cortex_cli.egg-info/dependency_links.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       62 2023-05-01 20:31:39.000000 cortex_cli-1.13.0/cortex_cli.egg-info/entry_points.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      110 2023-05-01 20:31:39.000000 cortex_cli-1.13.0/cortex_cli.egg-info/requires.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       11 2023-05-01 20:31:39.000000 cortex_cli-1.13.0/cortex_cli.egg-info/top_level.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       89 2023-03-01 03:50:43.000000 cortex_cli-1.13.0/pyproject.toml
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      228 2023-05-01 20:31:39.275137 cortex_cli-1.13.0/setup.cfg
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1076 2023-04-25 18:48:24.000000 cortex_cli-1.13.0/setup.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-02 20:19:39.552653 cortex_cli-1.13.1.post1/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      266 2023-05-02 20:19:39.552653 cortex_cli-1.13.1.post1/PKG-INFO
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     5211 2023-05-02 16:03:43.000000 cortex_cli-1.13.1.post1/README.md
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-02 20:19:39.542653 cortex_cli-1.13.1.post1/cortex_cli/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       25 2023-05-02 20:17:33.000000 cortex_cli-1.13.1.post1/cortex_cli/__init__.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-02 20:19:39.552653 cortex_cli-1.13.1.post1/cortex_cli/cli/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 23:15:18.000000 cortex_cli-1.13.1.post1/cortex_cli/cli/__init__.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-02 20:19:39.552653 cortex_cli-1.13.1.post1/cortex_cli/cli/api/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.13.1.post1/cortex_cli/cli/api/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3992 2023-05-02 16:03:43.000000 cortex_cli-1.13.1.post1/cortex_cli/cli/api/github_api.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      575 2023-03-09 15:57:05.000000 cortex_cli-1.13.1.post1/cortex_cli/cli/api/http_api.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2789 2023-03-16 20:39:49.000000 cortex_cli-1.13.1.post1/cortex_cli/cli/cli_api_base.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2792 2023-03-16 20:39:49.000000 cortex_cli-1.13.1.post1/cortex_cli/cli/cli_api_base_config.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       90 2023-03-09 15:57:05.000000 cortex_cli-1.13.1.post1/cortex_cli/cli/clients.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2027 2023-05-02 16:03:43.000000 cortex_cli-1.13.1.post1/cortex_cli/cli/configure.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      971 2023-03-16 20:39:49.000000 cortex_cli-1.13.1.post1/cortex_cli/cli/cortex_cli.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      994 2023-03-16 20:39:49.000000 cortex_cli-1.13.1.post1/cortex_cli/cli/generic_get.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1005 2023-03-09 15:57:05.000000 cortex_cli-1.13.1.post1/cortex_cli/cli/inferences.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    24846 2023-05-02 20:19:24.000000 cortex_cli-1.13.1.post1/cortex_cli/cli/models.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3248 2023-04-07 17:56:26.000000 cortex_cli-1.13.1.post1/cortex_cli/cli/pipelines.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-02 20:19:39.552653 cortex_cli-1.13.1.post1/cortex_cli/core/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.13.1.post1/cortex_cli/core/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     4182 2023-04-17 18:14:34.000000 cortex_cli-1.13.1.post1/cortex_cli/core/cortex_data.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3648 2023-03-09 15:57:05.000000 cortex_cli-1.13.1.post1/cortex_cli/core/drift_checks.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    11022 2023-04-17 18:14:34.000000 cortex_cli-1.13.1.post1/cortex_cli/core/ethics_checks.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-02 20:19:39.552653 cortex_cli-1.13.1.post1/cortex_cli/core/mlflow/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.13.1.post1/cortex_cli/core/mlflow/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    13976 2023-03-09 15:57:05.000000 cortex_cli-1.13.1.post1/cortex_cli/core/mlflow/mlflow_cortex.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-02 20:19:39.552653 cortex_cli-1.13.1.post1/cortex_cli/core/models/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.13.1.post1/cortex_cli/core/models/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     8121 2023-04-20 17:50:53.000000 cortex_cli-1.13.1.post1/cortex_cli/core/models/cortex_model.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2828 2023-04-25 18:48:24.000000 cortex_cli-1.13.1.post1/cortex_cli/core/secrets_manager.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-02 20:19:39.552653 cortex_cli-1.13.1.post1/cortex_cli/model_templates/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.1.post1/cortex_cli/model_templates/__init__.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-02 20:19:39.552653 cortex_cli-1.13.1.post1/cortex_cli/model_templates/chatgpt_model/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-04-25 18:48:24.000000 cortex_cli-1.13.1.post1/cortex_cli/model_templates/chatgpt_model/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-04-25 18:48:24.000000 cortex_cli-1.13.1.post1/cortex_cli/model_templates/chatgpt_model/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.1.post1/cortex_cli/model_templates/chatgpt_model/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      301 2023-04-25 18:48:24.000000 cortex_cli-1.13.1.post1/cortex_cli/model_templates/chatgpt_model/cookiecutter.json
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-04-25 18:48:24.000000 cortex_cli-1.13.1.post1/cortex_cli/model_templates/chatgpt_model/requirements.txt
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-02 20:19:39.552653 cortex_cli-1.13.1.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-04-25 18:48:24.000000 cortex_cli-1.13.1.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1645 2023-05-02 16:03:43.000000 cortex_cli-1.13.1.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      162 2023-04-25 18:48:24.000000 cortex_cli-1.13.1.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/conda.yml
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      322 2023-04-25 18:48:24.000000 cortex_cli-1.13.1.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/cortex.yml
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-02 20:19:39.552653 cortex_cli-1.13.1.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/data/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.1.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/data/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-02 20:19:39.552653 cortex_cli-1.13.1.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/notebooks/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.1.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/notebooks/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-02 20:19:39.542653 cortex_cli-1.13.1.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-02 20:19:39.552653 cortex_cli-1.13.1.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.1.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1654 2023-04-25 18:48:24.000000 cortex_cli-1.13.1.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-02 20:19:39.552653 cortex_cli-1.13.1.post1/cortex_cli/model_templates/digits_model/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-04-25 18:48:24.000000 cortex_cli-1.13.1.post1/cortex_cli/model_templates/digits_model/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-04-25 18:48:24.000000 cortex_cli-1.13.1.post1/cortex_cli/model_templates/digits_model/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.1.post1/cortex_cli/model_templates/digits_model/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      301 2023-04-25 18:48:24.000000 cortex_cli-1.13.1.post1/cortex_cli/model_templates/digits_model/cookiecutter.json
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-04-25 18:48:24.000000 cortex_cli-1.13.1.post1/cortex_cli/model_templates/digits_model/requirements.txt
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-02 20:19:39.552653 cortex_cli-1.13.1.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-04-25 18:48:24.000000 cortex_cli-1.13.1.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1645 2023-05-02 16:03:43.000000 cortex_cli-1.13.1.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      162 2023-04-25 18:48:24.000000 cortex_cli-1.13.1.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/conda.yml
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      455 2023-04-25 18:48:24.000000 cortex_cli-1.13.1.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/cortex.yml
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-02 20:19:39.552653 cortex_cli-1.13.1.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/data/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.1.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/data/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-02 20:19:39.552653 cortex_cli-1.13.1.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/notebooks/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.1.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/notebooks/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-02 20:19:39.542653 cortex_cli-1.13.1.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-02 20:19:39.552653 cortex_cli-1.13.1.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.13.1.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2377 2023-04-25 18:48:24.000000 cortex_cli-1.13.1.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-02 20:19:39.552653 cortex_cli-1.13.1.post1/cortex_cli/tests/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.13.1.post1/cortex_cli/tests/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1801 2023-03-09 15:57:05.000000 cortex_cli-1.13.1.post1/cortex_cli/tests/test_cortex_data.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1825 2023-03-09 15:57:05.000000 cortex_cli-1.13.1.post1/cortex_cli/tests/test_ethics_checks.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-02 20:19:39.552653 cortex_cli-1.13.1.post1/cortex_cli.egg-info/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      266 2023-05-02 20:19:39.000000 cortex_cli-1.13.1.post1/cortex_cli.egg-info/PKG-INFO
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3123 2023-05-02 20:19:39.000000 cortex_cli-1.13.1.post1/cortex_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        1 2023-05-02 20:19:39.000000 cortex_cli-1.13.1.post1/cortex_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       62 2023-05-02 20:19:39.000000 cortex_cli-1.13.1.post1/cortex_cli.egg-info/entry_points.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      110 2023-05-02 20:19:39.000000 cortex_cli-1.13.1.post1/cortex_cli.egg-info/requires.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       11 2023-05-02 20:19:39.000000 cortex_cli-1.13.1.post1/cortex_cli.egg-info/top_level.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       89 2023-03-01 03:50:43.000000 cortex_cli-1.13.1.post1/pyproject.toml
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      228 2023-05-02 20:19:39.552653 cortex_cli-1.13.1.post1/setup.cfg
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1076 2023-04-25 18:48:24.000000 cortex_cli-1.13.1.post1/setup.py
```

### Comparing `cortex_cli-1.13.0/README.md` & `cortex_cli-1.13.1.post1/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0/cortex_cli/cli/api/github_api.py` & `cortex_cli-1.13.1.post1/cortex_cli/cli/api/github_api.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0/cortex_cli/cli/api/http_api.py` & `cortex_cli-1.13.1.post1/cortex_cli/cli/api/http_api.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0/cortex_cli/cli/cli_api_base.py` & `cortex_cli-1.13.1.post1/cortex_cli/cli/cli_api_base.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0/cortex_cli/cli/cli_api_base_config.py` & `cortex_cli-1.13.1.post1/cortex_cli/cli/cli_api_base_config.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0/cortex_cli/cli/configure.py` & `cortex_cli-1.13.1.post1/cortex_cli/cli/configure.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0/cortex_cli/cli/cortex_cli.py` & `cortex_cli-1.13.1.post1/cortex_cli/cli/cortex_cli.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0/cortex_cli/cli/generic_get.py` & `cortex_cli-1.13.1.post1/cortex_cli/cli/generic_get.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0/cortex_cli/cli/inferences.py` & `cortex_cli-1.13.1.post1/cortex_cli/cli/inferences.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0/cortex_cli/cli/models.py` & `cortex_cli-1.13.1.post1/cortex_cli/cli/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         default=True
     )
 
     # Properties
 
     @property
     def _template_location(self):
-        current = os.path.dirname(os.path.realpath(__file__))
+        current = os.path.dirname(os.path.dirname(os.path.realpath(__file__)))
         template_path = os.path.join(current, self.MODEL_TEMPLATES_PATH)
         return os.path.join(template_path, self._template)
 
     @property
     def _model_path(self):
         return os.path.join(self._path, self._repo)
```

### Comparing `cortex_cli-1.13.0/cortex_cli/cli/pipelines.py` & `cortex_cli-1.13.1.post1/cortex_cli/cli/pipelines.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0/cortex_cli/core/cortex_data.py` & `cortex_cli-1.13.1.post1/cortex_cli/core/cortex_data.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0/cortex_cli/core/drift_checks.py` & `cortex_cli-1.13.1.post1/cortex_cli/core/drift_checks.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0/cortex_cli/core/ethics_checks.py` & `cortex_cli-1.13.1.post1/cortex_cli/core/ethics_checks.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0/cortex_cli/core/mlflow/mlflow_cortex.py` & `cortex_cli-1.13.1.post1/cortex_cli/core/mlflow/mlflow_cortex.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0/cortex_cli/core/models/cortex_model.py` & `cortex_cli-1.13.1.post1/cortex_cli/core/models/cortex_model.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0/cortex_cli/core/secrets_manager.py` & `cortex_cli-1.13.1.post1/cortex_cli/core/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0/cortex_cli/model_templates/chatgpt_model/.gitignore` & `cortex_cli-1.13.1.post1/cortex_cli/model_templates/chatgpt_model/.gitignore`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0/cortex_cli/model_templates/chatgpt_model/README.md` & `cortex_cli-1.13.1.post1/cortex_cli/model_templates/chatgpt_model/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/.gitignore` & `cortex_cli-1.13.1.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/.gitignore`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/README.md` & `cortex_cli-1.13.1.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py` & `cortex_cli-1.13.1.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0/cortex_cli/model_templates/digits_model/.gitignore` & `cortex_cli-1.13.1.post1/cortex_cli/model_templates/digits_model/.gitignore`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0/cortex_cli/model_templates/digits_model/README.md` & `cortex_cli-1.13.1.post1/cortex_cli/model_templates/digits_model/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/.gitignore` & `cortex_cli-1.13.1.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/.gitignore`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/README.md` & `cortex_cli-1.13.1.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py` & `cortex_cli-1.13.1.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0/cortex_cli/tests/test_cortex_data.py` & `cortex_cli-1.13.1.post1/cortex_cli/tests/test_cortex_data.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0/cortex_cli/tests/test_ethics_checks.py` & `cortex_cli-1.13.1.post1/cortex_cli/tests/test_ethics_checks.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0/cortex_cli.egg-info/SOURCES.txt` & `cortex_cli-1.13.1.post1/cortex_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.13.0/setup.py` & `cortex_cli-1.13.1.post1/setup.py`

 * *Files identical despite different names*

