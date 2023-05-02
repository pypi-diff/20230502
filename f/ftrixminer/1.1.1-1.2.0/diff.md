# Comparing `tmp/ftrixminer-1.1.1.tar.gz` & `tmp/ftrixminer-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftrixminer-1.1.1.tar", last modified: Wed Apr 26 07:48:42 2023, max compression
+gzip compressed data, was "ftrixminer-1.2.0.tar", last modified: Tue May  2 11:56:30 2023, max compression
```

## Comparing `ftrixminer-1.1.1.tar` & `ftrixminer-1.2.0.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:42.731673 ftrixminer-1.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:42.715673 ftrixminer-1.1.1/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:42.715673 ftrixminer-1.1.1/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:42.715673 ftrixminer-1.1.1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:42.715673 ftrixminer-1.1.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:42.711673 ftrixminer-1.1.1/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:42.715673 ftrixminer-1.1.1/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:42.719673 ftrixminer-1.1.1/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:42.719673 ftrixminer-1.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:42.719673 ftrixminer-1.1.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16137 2023-04-26 07:48:42.731673 ftrixminer-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:42.719673 ftrixminer-1.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:42.711673 ftrixminer-1.1.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:42.719673 ftrixminer-1.1.1/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:42.719673 ftrixminer-1.1.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:42.719673 ftrixminer-1.1.1/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:42.719673 ftrixminer-1.1.1/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/docs/user/explanations/22-developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/docs/user/explanations/23-testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/docs/user/explanations/24-devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/docs/user/explanations/25-docs-structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/docs/user/explanations/51-todo.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:42.719673 ftrixminer-1.1.1/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/docs/user/how-to/01-installing_development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:42.719673 ftrixminer-1.1.1/docs/user/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:42.723673 ftrixminer-1.1.1/docs/user/reference/api/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/docs/user/reference/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/docs/user/reference/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/docs/user/reference/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:42.723673 ftrixminer-1.1.1/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/docs/user/tutorials/tbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 07:48:42.731673 ftrixminer-1.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:42.711673 ftrixminer-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:42.723673 ftrixminer-1.1.1/src/ftrixminer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16137 2023-04-26 07:48:42.000000 ftrixminer-1.1.1/src/ftrixminer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-26 07:48:42.000000 ftrixminer-1.1.1/src/ftrixminer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 07:48:42.000000 ftrixminer-1.1.1/src/ftrixminer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-26 07:48:42.000000 ftrixminer-1.1.1/src/ftrixminer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-26 07:48:42.000000 ftrixminer-1.1.1/src/ftrixminer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-26 07:48:42.000000 ftrixminer-1.1.1/src/ftrixminer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:42.723673 ftrixminer-1.1.1/src/ftrixminer_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/src/ftrixminer_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/src/ftrixminer_api/aiohttp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/src/ftrixminer_api/context_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/src/ftrixminer_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:42.723673 ftrixminer-1.1.1/src/ftrixminer_api/miners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/src/ftrixminer_api/miners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/src/ftrixminer_api/miners/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/src/ftrixminer_api/miners/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/src/ftrixminer_api/miners/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/src/ftrixminer_api/miners/miners.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/src/ftrixminer_api/thing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/src/ftrixminer_api/things.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:42.723673 ftrixminer-1.1.1/src/ftrixminer_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/src/ftrixminer_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/src/ftrixminer_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:42.727673 ftrixminer-1.1.1/src/ftrixminer_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/src/ftrixminer_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/src/ftrixminer_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/src/ftrixminer_cli/subcommands/explore1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/src/ftrixminer_cli/subcommands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/src/ftrixminer_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:42.727673 ftrixminer-1.1.1/src/ftrixminer_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/src/ftrixminer_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/src/ftrixminer_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 07:48:42.000000 ftrixminer-1.1.1/src/ftrixminer_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/src/ftrixminer_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:42.727673 ftrixminer-1.1.1/src/ftrixminer_lib/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/src/ftrixminer_lib/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/src/ftrixminer_lib/contexts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/src/ftrixminer_lib/envvar.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/src/ftrixminer_lib/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:42.727673 ftrixminer-1.1.1/src/ftrixminer_lib/miners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/src/ftrixminer_lib/miners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/src/ftrixminer_lib/miners/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/src/ftrixminer_lib/miners/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/src/ftrixminer_lib/miners/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/src/ftrixminer_lib/miners/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/src/ftrixminer_lib/miners/direct_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/src/ftrixminer_lib/miners/miners.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/src/ftrixminer_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:42.727673 ftrixminer-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:48:42.727673 ftrixminer-1.1.1/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/tests/configurations/direct_poll.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/tests/configurations/service.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-04-26 07:48:32.000000 ftrixminer-1.1.1/tests/test_miner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:30.064362 ftrixminer-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:30.056362 ftrixminer-1.2.0/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:30.056362 ftrixminer-1.2.0/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:30.056362 ftrixminer-1.2.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:30.056362 ftrixminer-1.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:30.052362 ftrixminer-1.2.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:30.056362 ftrixminer-1.2.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:30.056362 ftrixminer-1.2.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:30.060362 ftrixminer-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:30.060362 ftrixminer-1.2.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16137 2023-05-02 11:56:30.064362 ftrixminer-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:30.060362 ftrixminer-1.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:30.052362 ftrixminer-1.2.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:30.060362 ftrixminer-1.2.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:30.060362 ftrixminer-1.2.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:30.060362 ftrixminer-1.2.0/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:30.060362 ftrixminer-1.2.0/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/docs/user/explanations/22-developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/docs/user/explanations/23-testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/docs/user/explanations/24-devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/docs/user/explanations/25-docs-structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/docs/user/explanations/51-todo.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:30.060362 ftrixminer-1.2.0/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/docs/user/how-to/01-installing_development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:30.060362 ftrixminer-1.2.0/docs/user/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:30.060362 ftrixminer-1.2.0/docs/user/reference/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/docs/user/reference/api/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/docs/user/reference/api/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/docs/user/reference/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:30.060362 ftrixminer-1.2.0/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/docs/user/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 11:56:30.064362 ftrixminer-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:30.056362 ftrixminer-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:30.060362 ftrixminer-1.2.0/src/ftrixminer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16137 2023-05-02 11:56:30.000000 ftrixminer-1.2.0/src/ftrixminer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-02 11:56:30.000000 ftrixminer-1.2.0/src/ftrixminer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 11:56:30.000000 ftrixminer-1.2.0/src/ftrixminer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-02 11:56:30.000000 ftrixminer-1.2.0/src/ftrixminer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-02 11:56:30.000000 ftrixminer-1.2.0/src/ftrixminer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-02 11:56:30.000000 ftrixminer-1.2.0/src/ftrixminer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:30.064362 ftrixminer-1.2.0/src/ftrixminer_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/src/ftrixminer_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/src/ftrixminer_api/aiohttp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/src/ftrixminer_api/context_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/src/ftrixminer_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:30.064362 ftrixminer-1.2.0/src/ftrixminer_api/miners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/src/ftrixminer_api/miners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/src/ftrixminer_api/miners/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/src/ftrixminer_api/miners/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/src/ftrixminer_api/miners/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/src/ftrixminer_api/miners/miners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/src/ftrixminer_api/thing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/src/ftrixminer_api/things.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:30.064362 ftrixminer-1.2.0/src/ftrixminer_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/src/ftrixminer_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/src/ftrixminer_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:30.064362 ftrixminer-1.2.0/src/ftrixminer_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/src/ftrixminer_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/src/ftrixminer_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/src/ftrixminer_cli/subcommands/explore1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/src/ftrixminer_cli/subcommands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/src/ftrixminer_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:30.064362 ftrixminer-1.2.0/src/ftrixminer_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/src/ftrixminer_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/src/ftrixminer_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-02 11:56:29.000000 ftrixminer-1.2.0/src/ftrixminer_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/src/ftrixminer_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:30.064362 ftrixminer-1.2.0/src/ftrixminer_lib/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/src/ftrixminer_lib/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/src/ftrixminer_lib/contexts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/src/ftrixminer_lib/envvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/src/ftrixminer_lib/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:30.064362 ftrixminer-1.2.0/src/ftrixminer_lib/miners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/src/ftrixminer_lib/miners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/src/ftrixminer_lib/miners/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/src/ftrixminer_lib/miners/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/src/ftrixminer_lib/miners/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/src/ftrixminer_lib/miners/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/src/ftrixminer_lib/miners/direct_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/src/ftrixminer_lib/miners/miners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/src/ftrixminer_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:30.064362 ftrixminer-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:56:30.064362 ftrixminer-1.2.0/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/tests/configurations/direct_poll.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/tests/configurations/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-05-02 11:56:19.000000 ftrixminer-1.2.0/tests/test_miner.py
```

### Comparing `ftrixminer-1.1.1/.dae-devops/Makefile` & `ftrixminer-1.2.0/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/.dae-devops/docs/conventions.rst` & `ftrixminer-1.2.0/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/.dae-devops/docs/developing.rst` & `ftrixminer-1.2.0/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/.dae-devops/docs/devops.rst` & `ftrixminer-1.2.0/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/.dae-devops/docs/docs_structure.rst` & `ftrixminer-1.2.0/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/.dae-devops/docs/installing.rst` & `ftrixminer-1.2.0/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/.dae-devops/docs/testing.rst` & `ftrixminer-1.2.0/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/.dae-devops/project.yaml` & `ftrixminer-1.2.0/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/.devcontainer/Dockerfile` & `ftrixminer-1.2.0/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/.devcontainer/devcontainer.json` & `ftrixminer-1.2.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/.github/CONTRIBUTING.rst` & `ftrixminer-1.2.0/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/.github/actions/install_requirements/action.yml` & `ftrixminer-1.2.0/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/.github/dependabot.yml` & `ftrixminer-1.2.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/.github/pages/make_switcher.py` & `ftrixminer-1.2.0/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/.github/workflows/code.yml` & `ftrixminer-1.2.0/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/.github/workflows/docs.yml` & `ftrixminer-1.2.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/.github/workflows/docs_clean.yml` & `ftrixminer-1.2.0/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/.github/workflows/linkcheck.yml` & `ftrixminer-1.2.0/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/.gitignore` & `ftrixminer-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/.gitlab-ci.yml` & `ftrixminer-1.2.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/.vscode/launch.json` & `ftrixminer-1.2.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/LICENSE` & `ftrixminer-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/PKG-INFO` & `ftrixminer-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftrixminer
-Version: 1.1.1
+Version: 1.2.0
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `ftrixminer-1.1.1/README.rst` & `ftrixminer-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/docs/conf.py` & `ftrixminer-1.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/docs/images/dls-favicon.ico` & `ftrixminer-1.2.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/docs/images/dls-logo.svg` & `ftrixminer-1.2.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/docs/index.rst` & `ftrixminer-1.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/docs/user/explanations/25-docs-structure.rst` & `ftrixminer-1.2.0/docs/user/explanations/25-docs-structure.rst`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/docs/user/index.rst` & `ftrixminer-1.2.0/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/pyproject.toml` & `ftrixminer-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/src/ftrixminer.egg-info/PKG-INFO` & `ftrixminer-1.2.0/src/ftrixminer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftrixminer
-Version: 1.1.1
+Version: 1.2.0
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `ftrixminer-1.1.1/src/ftrixminer.egg-info/SOURCES.txt` & `ftrixminer-1.2.0/src/ftrixminer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/src/ftrixminer_api/context_base.py` & `ftrixminer-1.2.0/src/ftrixminer_api/context_base.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/src/ftrixminer_api/exceptions.py` & `ftrixminer-1.2.0/src/ftrixminer_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/src/ftrixminer_api/miners/aiohttp.py` & `ftrixminer-1.2.0/src/ftrixminer_api/miners/aiohttp.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/src/ftrixminer_api/miners/context.py` & `ftrixminer-1.2.0/src/ftrixminer_api/miners/context.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/src/ftrixminer_api/miners/miners.py` & `ftrixminer-1.2.0/src/ftrixminer_api/miners/miners.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/src/ftrixminer_api/thing.py` & `ftrixminer-1.2.0/src/ftrixminer_api/thing.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/src/ftrixminer_api/things.py` & `ftrixminer-1.2.0/src/ftrixminer_api/things.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/src/ftrixminer_cli/main.py` & `ftrixminer-1.2.0/src/ftrixminer_cli/main.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/src/ftrixminer_cli/subcommands/base.py` & `ftrixminer-1.2.0/src/ftrixminer_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/src/ftrixminer_cli/subcommands/explore1.py` & `ftrixminer-1.2.0/src/ftrixminer_cli/subcommands/explore1.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/src/ftrixminer_cli/subcommands/service.py` & `ftrixminer-1.2.0/src/ftrixminer_cli/subcommands/service.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/src/ftrixminer_cli/version.py` & `ftrixminer-1.2.0/src/ftrixminer_cli/version.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/src/ftrixminer_lib/__main__.py` & `ftrixminer-1.2.0/src/ftrixminer_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/src/ftrixminer_lib/contexts/base.py` & `ftrixminer-1.2.0/src/ftrixminer_lib/contexts/base.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/src/ftrixminer_lib/exceptions.py` & `ftrixminer-1.2.0/src/ftrixminer_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/src/ftrixminer_lib/miners/aiohttp.py` & `ftrixminer-1.2.0/src/ftrixminer_lib/miners/aiohttp.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,29 +92,28 @@
     # ----------------------------------------------------------------------------------------
     async def activate_coro(self) -> None:
         """
         Activate the direct miner and web server in a two asyncio tasks.
         """
 
         try:
+            # Don't show pytds (mssql server) debug.
+            logging.getLogger("pytds").setLevel("WARNING")
+
             # Build a local miner for our back-end.
             self.__direct_miner = Miners().build_object(
                 self.specification()["type_specific_tbd"]["direct_miner_specification"]
             )
 
-            logger.info("[COLSHUT] calling self.__direct_miner.activate()")
             # Get the local implementation started.
             await self.__direct_miner.activate()
 
             # ----------------------------------------------
-            logger.info("[COLSHUT] calling BaseAiohttp.activate_coro_base(self)")
             await BaseAiohttp.activate_coro_base(self)
 
-            logger.info("[COLSHUT] returning")
-
         except Exception as exception:
             raise RuntimeError("exception while starting miner server") from exception
 
     # ----------------------------------------------------------------------------------------
     async def direct_shutdown(self) -> None:
         """
         Shut down any started sub-process or coro tasks.
```

### Comparing `ftrixminer-1.1.1/src/ftrixminer_lib/miners/base.py` & `ftrixminer-1.2.0/src/ftrixminer_lib/miners/base.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/src/ftrixminer_lib/miners/context.py` & `ftrixminer-1.2.0/src/ftrixminer_lib/miners/context.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/src/ftrixminer_lib/miners/direct_poll.py` & `ftrixminer-1.2.0/src/ftrixminer_lib/miners/direct_poll.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 from typing import List
 
 import pytds
 from dls_utilpack.callsign import callsign
 from dls_utilpack.explain import explain2
 from dls_utilpack.require import require
 
+# Crystal plate constants.
+from xchembku_api.crystal_plate_objects.constants import TREENODE_NAMES_TO_THING_TYPES
+
 # Dataface client context.
 from xchembku_api.datafaces.context import Context as XchembkuDatafaceClientContext
 from xchembku_api.models.crystal_plate_filter_model import CrystalPlateFilterModel
 
 # Crystal well pydantic model.
 from xchembku_api.models.crystal_plate_model import CrystalPlateModel
 
@@ -81,17 +84,14 @@
             why="latest plate we already have in the database",
         )
         if len(crystal_plate_models) > 0:
             self.__latest_formulatrix__plate__id = crystal_plate_models[
                 0
             ].formulatrix__plate__id
 
-        logger.debug(
-            f"[CPMINP] initial self.__latest_formulatrix__plate__id is {self.__latest_formulatrix__plate__id}"
-        )
         # Poll periodically.
         self.__tick_future = asyncio.get_event_loop().create_task(self.tick())
 
     # ----------------------------------------------------------------------------------------
     async def deactivate(self) -> None:
         """
         Deactivate the object.
@@ -107,17 +107,15 @@
             # Wait for the ticking to stop.
             await self.__tick_future
 
         # Forget we have an xchembku client reference.
         self.__xchembku = None
 
         if self.__xchembku_client_context is not None:
-            logger.debug(f"[ECHDON] {callsign(self)} exiting __xchembku_client_context")
             await self.__xchembku_client_context.aexit()
-            logger.debug(f"[ECHDON] {callsign(self)} exited __xchembku_client_context")
             self.__xchembku_client_context = None
 
     # ----------------------------------------------------------------------------------------
     async def tick(self) -> None:
         """
         A coro task which does periodic checking for new files in the directories.
 
@@ -140,36 +138,36 @@
         """
         Scrape discover new plates in the Formulatrix database.
         """
 
         # Query mssql or dummy.
         rows = await self.query()
 
-        logger.debug(f"[FTRIXMINER POLL] discovered {len(rows)} plate rows")
+        logger.debug(f"[FTRIXMINER POLL] discovered {len(rows)} new plate rows")
 
         # Loop over the rows we got back from the query.
         for row in rows:
             formulatrix__plate__id = int(row[0])
+            thing_type = TREENODE_NAMES_TO_THING_TYPES.get(row[3])
+            if thing_type is None:
+                raise RuntimeError(f"programming error: plate type {row[3]} unexpected")
             crystal_plate_model = CrystalPlateModel(
                 barcode=str(row[1]),
                 visit=str(row[2]),
+                thing_type=thing_type,
                 formulatrix__plate__id=formulatrix__plate__id,
             )
 
             # Add plate to our database.
             # I don't worry about performance hit of adding plates one by one with upsert
             # since new plates don't get added very often.
             await self.__xchembku.upsert_crystal_plates([crystal_plate_model])
 
             self.__latest_formulatrix__plate__id = formulatrix__plate__id
 
-            logger.debug(
-                f"self.__latest_formulatrix__plate__id is now {self.__latest_formulatrix__plate__id}"
-            )
-
     # ----------------------------------------------------------------------------------------
     async def query(self) -> List[List]:
         """
         Read dummy data from configuration.
         """
 
         server = self.__mssql["server"]
@@ -190,32 +188,38 @@
         connection = pytds.connect(
             self.__mssql["server"],
             self.__mssql["database"],
             self.__mssql["username"],
             self.__mssql["password"],
         )
 
+        # Select only plate types we care about.
+        treenode_names = [
+            f"'{str(name)}'" for name in list(TREENODE_NAMES_TO_THING_TYPES.keys())
+        ]
+
         # Plate's treenode is "ExperimentPlate".
         # Parent of ExperimentPlate is "Experiment", aka visit
         # Parent of Experiment is "Project", aka plate type.
         # Parent of Project is "ProjectsFolder", we only care about "XChem"
         # Get all xchem barcodes and the associated experiment name.
         sql = (
             "SELECT"
             " Plate.ID AS id,"
             " Plate.Barcode AS barcode,"
-            " experiment_node.Name AS visit"
+            " experiment_node.Name AS visit,"
+            " plate_type_node.Name AS plate_type"
             " FROM Plate"
             " JOIN Experiment ON experiment.ID = plate.experimentID"
             " JOIN TreeNode AS experiment_node ON experiment_node.ID = Experiment.TreeNodeID"
             " JOIN TreeNode AS plate_type_node ON plate_type_node.ID = experiment_node.ParentID"
             " JOIN TreeNode AS projects_folder_node ON projects_folder_node.ID = plate_type_node.ParentID"
             f" WHERE Plate.ID > {self.__latest_formulatrix__plate__id}"
             " AND projects_folder_node.Name = 'xchem'"
-            " AND plate_type_node.NAME IN ('SWISSci_3drop')"
+            f" AND plate_type_node.Name IN ({',' .join(treenode_names)})"
         )
 
         cursor = connection.cursor()
         cursor.execute(sql)
         rows = cursor.fetchall()
 
         return rows
```

### Comparing `ftrixminer-1.1.1/src/ftrixminer_lib/miners/miners.py` & `ftrixminer-1.2.0/src/ftrixminer_lib/miners/miners.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/src/ftrixminer_lib/version.py` & `ftrixminer-1.2.0/src/ftrixminer_lib/version.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/tests/base.py` & `ftrixminer-1.2.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/tests/configurations/direct_poll.yaml` & `ftrixminer-1.2.0/tests/configurations/direct_poll.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -17,13 +17,15 @@
       database: records1
       username: na
       password: na
       records1:
         - - 1
           - 98ab
           - cm00001-1
+          - SWISSci_3Drop
         - - 2
           - 98ac
           - cm00001-1
+          - SWISSci_3drop
     xchembku_dataface_specification: *XCHEMBKU_DATAFACE_SPECIFICATION
   context:
     start_as: direct
```

### Comparing `ftrixminer-1.1.1/tests/configurations/service.yaml` & `ftrixminer-1.2.0/tests/configurations/service.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -35,17 +35,19 @@
             database: records1
             username: na
             password: na
             records1:
                 - - 1
                   - 98ab
                   - cm00001-1
+                  - SWISSci_3Drop
                 - - 2
                   - 98ac
                   - cm00001-1
+                  - SWISSci_3Drop
         xchembku_dataface_specification: *XCHEMBKU_DATAFACE_SPECIFICATION
 
 # The ftrixminer client/server composite.
 ftrixminer_miner_specification:
     type: "ftrixminer_lib.miners.aiohttp"
     type_specific_tbd:
         # The remote ftrixminer server access.
```

### Comparing `ftrixminer-1.1.1/tests/conftest.py` & `ftrixminer-1.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ftrixminer-1.1.1/tests/test_miner.py` & `ftrixminer-1.2.0/tests/test_miner.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 import time
 
 # Things xchembku provides.
 from xchembku_api.datafaces.context import Context as XchembkuDatafaceClientContext
 from xchembku_api.datafaces.datafaces import xchembku_datafaces_get_default
 from xchembku_api.models.crystal_plate_filter_model import CrystalPlateFilterModel
 
+# Crystal plate objects factory.
+from xchembku_lib.crystal_plate_objects.crystal_plate_objects import CrystalPlateObjects
+
 # Client context creator.
 from ftrixminer_api.miners.context import Context as MinerClientContext
 
 # Server context creator.
 from ftrixminer_lib.miners.context import Context as MinerServerContext
 
 # Base class for the tester.
@@ -102,40 +105,42 @@
     # ----------------------------------------------------------------------------------------
 
     async def __run_part1(self, plate_count, constants, output_directory):
         """ """
         # Reference the xchembku object which the context has set up as the default.
         xchembku = xchembku_datafaces_get_default()
 
-        # Get list of plates before we create any of the mock plates.
+        # Filter get all crystal plates.
         filter = CrystalPlateFilterModel()
-        records = await xchembku.fetch_crystal_plates(filter)
-
-        # assert len(records) == 0, "images before any mock plates"
 
         # Wait for all the plates to appear.
         time0 = time.time()
-        timeout = 2.0
+        timeout = 5.0
         while True:
 
             # Get all images.
-            records = await xchembku.fetch_crystal_plates(filter)
+            models = await xchembku.fetch_crystal_plates(filter)
 
             # Stop looping when we got the images we expect.
-            if len(records) >= plate_count:
+            if len(models) >= plate_count:
                 break
 
             if time.time() - time0 > timeout:
                 raise RuntimeError(
-                    f"only {len(records)} images out of {plate_count}"
+                    f"only {len(models)} images out of {plate_count}"
                     f" registered within {timeout} seconds"
                 )
             await asyncio.sleep(1.0)
 
-        assert len(records) == plate_count, "plates after mining"
+        assert len(models) == plate_count, "plates after mining"
+
+        # Make sure that the model which came out of the database can be instantiated.
+        specification = {"type": models[0].thing_type}
+        o = CrystalPlateObjects().build_object(specification)
+        assert o.get_well_count() == 288
 
     # ----------------------------------------------------------------------------------------
 
     async def __run_part2(self, plate_count, constants, output_directory):
         """ """
         # Reference the xchembku object which the context has set up as the default.
         xchembku = xchembku_datafaces_get_default()
```

