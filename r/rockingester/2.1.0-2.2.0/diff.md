# Comparing `tmp/rockingester-2.1.0.tar.gz` & `tmp/rockingester-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rockingester-2.1.0.tar", last modified: Mon May  1 07:14:23 2023, max compression
+gzip compressed data, was "rockingester-2.2.0.tar", last modified: Tue May  2 08:58:16 2023, max compression
```

## Comparing `rockingester-2.1.0.tar` & `rockingester-2.2.0.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.541447 rockingester-2.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.533447 rockingester-2.1.0/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-01 07:14:12.000000 rockingester-2.1.0/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.533447 rockingester-2.1.0/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-01 07:14:12.000000 rockingester-2.1.0/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-01 07:14:12.000000 rockingester-2.1.0/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-01 07:14:12.000000 rockingester-2.1.0/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-01 07:14:12.000000 rockingester-2.1.0/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-01 07:14:12.000000 rockingester-2.1.0/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-01 07:14:12.000000 rockingester-2.1.0/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-01 07:14:12.000000 rockingester-2.1.0/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-01 07:14:12.000000 rockingester-2.1.0/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.533447 rockingester-2.1.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-01 07:14:12.000000 rockingester-2.1.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-01 07:14:12.000000 rockingester-2.1.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.533447 rockingester-2.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-01 07:14:12.000000 rockingester-2.1.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.529447 rockingester-2.1.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.533447 rockingester-2.1.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-01 07:14:12.000000 rockingester-2.1.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-01 07:14:12.000000 rockingester-2.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.533447 rockingester-2.1.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-01 07:14:12.000000 rockingester-2.1.0/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-01 07:14:12.000000 rockingester-2.1.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.533447 rockingester-2.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-05-01 07:14:12.000000 rockingester-2.1.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-01 07:14:12.000000 rockingester-2.1.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-01 07:14:12.000000 rockingester-2.1.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-01 07:14:12.000000 rockingester-2.1.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-01 07:14:12.000000 rockingester-2.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-01 07:14:12.000000 rockingester-2.1.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-01 07:14:12.000000 rockingester-2.1.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.533447 rockingester-2.1.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-01 07:14:12.000000 rockingester-2.1.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-01 07:14:12.000000 rockingester-2.1.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-01 07:14:12.000000 rockingester-2.1.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-01 07:14:12.000000 rockingester-2.1.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-01 07:14:12.000000 rockingester-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16864 2023-05-01 07:14:23.541447 rockingester-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-01 07:14:12.000000 rockingester-2.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.533447 rockingester-2.1.0/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-01 07:14:12.000000 rockingester-2.1.0/configurations/development.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.533447 rockingester-2.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.529447 rockingester-2.1.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.537447 rockingester-2.1.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-01 07:14:12.000000 rockingester-2.1.0/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-05-01 07:14:12.000000 rockingester-2.1.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.537447 rockingester-2.1.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-01 07:14:12.000000 rockingester-2.1.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-01 07:14:12.000000 rockingester-2.1.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-01 07:14:12.000000 rockingester-2.1.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.537447 rockingester-2.1.0/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.537447 rockingester-2.1.0/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-01 07:14:12.000000 rockingester-2.1.0/docs/user/explanations/22-developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-01 07:14:12.000000 rockingester-2.1.0/docs/user/explanations/23-testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-01 07:14:12.000000 rockingester-2.1.0/docs/user/explanations/24-devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-01 07:14:12.000000 rockingester-2.1.0/docs/user/explanations/25-docs-structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-01 07:14:12.000000 rockingester-2.1.0/docs/user/explanations/51-todo.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.537447 rockingester-2.1.0/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-01 07:14:12.000000 rockingester-2.1.0/docs/user/how-to/01-installing_development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-01 07:14:12.000000 rockingester-2.1.0/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.537447 rockingester-2.1.0/docs/user/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.537447 rockingester-2.1.0/docs/user/reference/api/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-01 07:14:12.000000 rockingester-2.1.0/docs/user/reference/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-01 07:14:12.000000 rockingester-2.1.0/docs/user/reference/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-01 07:14:12.000000 rockingester-2.1.0/docs/user/reference/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-01 07:14:12.000000 rockingester-2.1.0/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.537447 rockingester-2.1.0/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-01 07:14:12.000000 rockingester-2.1.0/docs/user/tutorials/tbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-01 07:14:12.000000 rockingester-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 07:14:23.541447 rockingester-2.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.529447 rockingester-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.537447 rockingester-2.1.0/src/rockingester.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16864 2023-05-01 07:14:23.000000 rockingester-2.1.0/src/rockingester.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-01 07:14:23.000000 rockingester-2.1.0/src/rockingester.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 07:14:23.000000 rockingester-2.1.0/src/rockingester.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-01 07:14:23.000000 rockingester-2.1.0/src/rockingester.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-01 07:14:23.000000 rockingester-2.1.0/src/rockingester.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-01 07:14:23.000000 rockingester-2.1.0/src/rockingester.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.537447 rockingester-2.1.0/src/rockingester_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_api/aiohttp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.537447 rockingester-2.1.0/src/rockingester_api/collectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_api/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_api/collectors/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_api/collectors/collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_api/collectors/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_api/collectors/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_api/context_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_api/thing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_api/things.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.537447 rockingester-2.1.0/src/rockingester_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.541447 rockingester-2.1.0/src/rockingester_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_cli/subcommands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.541447 rockingester-2.1.0/src/rockingester_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-01 07:14:23.000000 rockingester-2.1.0/src/rockingester_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.541447 rockingester-2.1.0/src/rockingester_lib/collectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_lib/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_lib/collectors/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_lib/collectors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_lib/collectors/collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_lib/collectors/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_lib/collectors/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    14651 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_lib/collectors/direct_poll.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.541447 rockingester-2.1.0/src/rockingester_lib/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_lib/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_lib/contexts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_lib/envvar.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_lib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-01 07:14:12.000000 rockingester-2.1.0/src/rockingester_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.541447 rockingester-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:12.000000 rockingester-2.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-01 07:14:12.000000 rockingester-2.1.0/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:14:23.541447 rockingester-2.1.0/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-01 07:14:12.000000 rockingester-2.1.0/tests/configurations/direct_poll.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-01 07:14:12.000000 rockingester-2.1.0/tests/configurations/service.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-01 07:14:12.000000 rockingester-2.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12961 2023-05-01 07:14:12.000000 rockingester-2.1.0/tests/test_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.792846 rockingester-2.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.776846 rockingester-2.2.0/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-02 08:58:04.000000 rockingester-2.2.0/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.776846 rockingester-2.2.0/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-02 08:58:04.000000 rockingester-2.2.0/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-02 08:58:04.000000 rockingester-2.2.0/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-02 08:58:04.000000 rockingester-2.2.0/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-02 08:58:04.000000 rockingester-2.2.0/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-02 08:58:04.000000 rockingester-2.2.0/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-02 08:58:04.000000 rockingester-2.2.0/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-02 08:58:04.000000 rockingester-2.2.0/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-02 08:58:04.000000 rockingester-2.2.0/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.776846 rockingester-2.2.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-02 08:58:04.000000 rockingester-2.2.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-02 08:58:04.000000 rockingester-2.2.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.776846 rockingester-2.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-02 08:58:04.000000 rockingester-2.2.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.772846 rockingester-2.2.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.776846 rockingester-2.2.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-02 08:58:04.000000 rockingester-2.2.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-02 08:58:04.000000 rockingester-2.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.776846 rockingester-2.2.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-02 08:58:04.000000 rockingester-2.2.0/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-02 08:58:04.000000 rockingester-2.2.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.780846 rockingester-2.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-05-02 08:58:04.000000 rockingester-2.2.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-02 08:58:04.000000 rockingester-2.2.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-02 08:58:04.000000 rockingester-2.2.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-02 08:58:04.000000 rockingester-2.2.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-02 08:58:04.000000 rockingester-2.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-02 08:58:04.000000 rockingester-2.2.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-02 08:58:04.000000 rockingester-2.2.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.780846 rockingester-2.2.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-02 08:58:04.000000 rockingester-2.2.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-02 08:58:04.000000 rockingester-2.2.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-02 08:58:04.000000 rockingester-2.2.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-02 08:58:04.000000 rockingester-2.2.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-02 08:58:04.000000 rockingester-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16864 2023-05-02 08:58:16.792846 rockingester-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-02 08:58:04.000000 rockingester-2.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.780846 rockingester-2.2.0/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-02 08:58:04.000000 rockingester-2.2.0/configurations/development.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.780846 rockingester-2.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.772846 rockingester-2.2.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.780846 rockingester-2.2.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-02 08:58:04.000000 rockingester-2.2.0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-05-02 08:58:04.000000 rockingester-2.2.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.780846 rockingester-2.2.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-02 08:58:04.000000 rockingester-2.2.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-02 08:58:04.000000 rockingester-2.2.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-02 08:58:04.000000 rockingester-2.2.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.780846 rockingester-2.2.0/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.780846 rockingester-2.2.0/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-02 08:58:04.000000 rockingester-2.2.0/docs/user/explanations/22-developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-02 08:58:04.000000 rockingester-2.2.0/docs/user/explanations/23-testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-02 08:58:04.000000 rockingester-2.2.0/docs/user/explanations/24-devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-02 08:58:04.000000 rockingester-2.2.0/docs/user/explanations/25-docs-structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-02 08:58:04.000000 rockingester-2.2.0/docs/user/explanations/51-todo.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.784846 rockingester-2.2.0/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-02 08:58:04.000000 rockingester-2.2.0/docs/user/how-to/01-installing_development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-02 08:58:04.000000 rockingester-2.2.0/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.784846 rockingester-2.2.0/docs/user/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.784846 rockingester-2.2.0/docs/user/reference/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-02 08:58:04.000000 rockingester-2.2.0/docs/user/reference/api/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-02 08:58:04.000000 rockingester-2.2.0/docs/user/reference/api/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-02 08:58:04.000000 rockingester-2.2.0/docs/user/reference/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-02 08:58:04.000000 rockingester-2.2.0/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.784846 rockingester-2.2.0/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-02 08:58:04.000000 rockingester-2.2.0/docs/user/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-02 08:58:04.000000 rockingester-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 08:58:16.792846 rockingester-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.772846 rockingester-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.784846 rockingester-2.2.0/src/rockingester.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16864 2023-05-02 08:58:16.000000 rockingester-2.2.0/src/rockingester.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-02 08:58:16.000000 rockingester-2.2.0/src/rockingester.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 08:58:16.000000 rockingester-2.2.0/src/rockingester.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-02 08:58:16.000000 rockingester-2.2.0/src/rockingester.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-02 08:58:16.000000 rockingester-2.2.0/src/rockingester.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-02 08:58:16.000000 rockingester-2.2.0/src/rockingester.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.788846 rockingester-2.2.0/src/rockingester_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_api/aiohttp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.788846 rockingester-2.2.0/src/rockingester_api/collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_api/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_api/collectors/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_api/collectors/collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_api/collectors/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_api/collectors/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_api/context_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_api/thing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_api/things.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.788846 rockingester-2.2.0/src/rockingester_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.788846 rockingester-2.2.0/src/rockingester_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_cli/subcommands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.788846 rockingester-2.2.0/src/rockingester_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-02 08:58:16.000000 rockingester-2.2.0/src/rockingester_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.792846 rockingester-2.2.0/src/rockingester_lib/collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_lib/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_lib/collectors/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_lib/collectors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_lib/collectors/collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_lib/collectors/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_lib/collectors/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14728 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_lib/collectors/direct_poll.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.792846 rockingester-2.2.0/src/rockingester_lib/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_lib/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_lib/contexts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_lib/envvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-02 08:58:04.000000 rockingester-2.2.0/src/rockingester_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.792846 rockingester-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:04.000000 rockingester-2.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-02 08:58:04.000000 rockingester-2.2.0/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 08:58:16.792846 rockingester-2.2.0/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-02 08:58:04.000000 rockingester-2.2.0/tests/configurations/direct_poll.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-02 08:58:04.000000 rockingester-2.2.0/tests/configurations/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-02 08:58:04.000000 rockingester-2.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-05-02 08:58:04.000000 rockingester-2.2.0/tests/test_collector.py
```

### Comparing `rockingester-2.1.0/.dae-devops/Makefile` & `rockingester-2.2.0/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/.dae-devops/docs/conventions.rst` & `rockingester-2.2.0/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/.dae-devops/docs/developing.rst` & `rockingester-2.2.0/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/.dae-devops/docs/devops.rst` & `rockingester-2.2.0/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/.dae-devops/docs/docs_structure.rst` & `rockingester-2.2.0/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/.dae-devops/docs/installing.rst` & `rockingester-2.2.0/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/.dae-devops/docs/testing.rst` & `rockingester-2.2.0/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/.dae-devops/project.yaml` & `rockingester-2.2.0/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/.devcontainer/Dockerfile` & `rockingester-2.2.0/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/.devcontainer/devcontainer.json` & `rockingester-2.2.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/.github/CONTRIBUTING.rst` & `rockingester-2.2.0/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/.github/actions/install_requirements/action.yml` & `rockingester-2.2.0/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/.github/dependabot.yml` & `rockingester-2.2.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/.github/pages/make_switcher.py` & `rockingester-2.2.0/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/.github/workflows/code.yml` & `rockingester-2.2.0/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/.github/workflows/docs.yml` & `rockingester-2.2.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/.github/workflows/docs_clean.yml` & `rockingester-2.2.0/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/.github/workflows/linkcheck.yml` & `rockingester-2.2.0/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/.gitignore` & `rockingester-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/.gitlab-ci.yml` & `rockingester-2.2.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/.vscode/launch.json` & `rockingester-2.2.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/LICENSE` & `rockingester-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/PKG-INFO` & `rockingester-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rockingester
-Version: 2.1.0
+Version: 2.2.0
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `rockingester-2.1.0/README.rst` & `rockingester-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/configurations/development.yaml` & `rockingester-2.2.0/configurations/development.yaml`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/docs/conf.py` & `rockingester-2.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/docs/images/dls-favicon.ico` & `rockingester-2.2.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/docs/images/dls-logo.svg` & `rockingester-2.2.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/docs/index.rst` & `rockingester-2.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/docs/user/explanations/25-docs-structure.rst` & `rockingester-2.2.0/docs/user/explanations/25-docs-structure.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/docs/user/index.rst` & `rockingester-2.2.0/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/pyproject.toml` & `rockingester-2.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/src/rockingester.egg-info/PKG-INFO` & `rockingester-2.2.0/src/rockingester.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rockingester
-Version: 2.1.0
+Version: 2.2.0
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `rockingester-2.1.0/src/rockingester.egg-info/SOURCES.txt` & `rockingester-2.2.0/src/rockingester.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/src/rockingester_api/collectors/aiohttp.py` & `rockingester-2.2.0/src/rockingester_api/collectors/aiohttp.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/src/rockingester_api/collectors/collectors.py` & `rockingester-2.2.0/src/rockingester_api/collectors/collectors.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/src/rockingester_api/collectors/context.py` & `rockingester-2.2.0/src/rockingester_api/collectors/context.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/src/rockingester_api/context_base.py` & `rockingester-2.2.0/src/rockingester_api/context_base.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/src/rockingester_api/exceptions.py` & `rockingester-2.2.0/src/rockingester_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/src/rockingester_api/thing.py` & `rockingester-2.2.0/src/rockingester_api/thing.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/src/rockingester_api/things.py` & `rockingester-2.2.0/src/rockingester_api/things.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/src/rockingester_cli/main.py` & `rockingester-2.2.0/src/rockingester_cli/main.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/src/rockingester_cli/subcommands/base.py` & `rockingester-2.2.0/src/rockingester_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/src/rockingester_cli/subcommands/service.py` & `rockingester-2.2.0/src/rockingester_cli/subcommands/service.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/src/rockingester_cli/version.py` & `rockingester-2.2.0/src/rockingester_cli/version.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/src/rockingester_lib/__main__.py` & `rockingester-2.2.0/src/rockingester_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/src/rockingester_lib/collectors/aiohttp.py` & `rockingester-2.2.0/src/rockingester_lib/collectors/aiohttp.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/src/rockingester_lib/collectors/base.py` & `rockingester-2.2.0/src/rockingester_lib/collectors/base.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/src/rockingester_lib/collectors/collectors.py` & `rockingester-2.2.0/src/rockingester_lib/collectors/collectors.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/src/rockingester_lib/collectors/context.py` & `rockingester-2.2.0/src/rockingester_lib/collectors/context.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/src/rockingester_lib/collectors/direct_poll.py` & `rockingester-2.2.0/src/rockingester_lib/collectors/direct_poll.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 
 from dls_utilpack.callsign import callsign
 from dls_utilpack.explain import explain2
 from dls_utilpack.require import require
 from dls_utilpack.visit import VisitNotFound, get_xchem_directory
 from PIL import Image
 
+# Crystal plate object interface.
+from xchembku_api.crystal_plate_objects.interface import (
+    Interface as CrystalPlateInterface,
+)
+
 # Dataface client context.
 from xchembku_api.datafaces.context import Context as XchembkuDatafaceClientContext
 from xchembku_api.models.crystal_plate_filter_model import CrystalPlateFilterModel
 
 # Crystal plate pydantic model.
 from xchembku_api.models.crystal_plate_model import CrystalPlateModel
 
@@ -286,38 +291,39 @@
             # TODO: Consider if important to report/record same barcodes on different rockmaker directories.
             crystal_plate_model.rockminer_collected_stem = plate_directory.stem
             await self.__xchembku.upsert_crystal_plates(
                 [crystal_plate_model], "update rockminer_collected_stem"
             )
 
         # Get all the well images in the plate directory.
-        well_names = [
+        subwell_names = [
             entry.name for entry in os.scandir(plate_directory) if entry.is_file()
         ]
 
         # Make an object corresponding to the crystal plate model's type.
         crystal_plate_object = CrystalPlateObjects().build_object(
             {"type": crystal_plate_model.thing_type}
         )
 
         # Don't handle the plate directory until all images have arrived.
         # TODO: Put in some kind of failsafe in direct_poll.py to handle case where all the well images never arrive.
-        if len(well_names) < crystal_plate_object.get_well_count():
+        if len(subwell_names) < crystal_plate_object.get_well_count():
             return
 
         # Sort wells by name so that tests are deterministic.
-        well_names.sort()
+        subwell_names.sort()
 
         crystal_well_models: List[CrystalWellModel] = []
-        for well_name in well_names:
+        for subwell_name in subwell_names:
             # Make the well model, including image width/height.
             crystal_well_model = await self.ingest_well(
                 plate_directory,
-                well_name,
+                subwell_name,
                 crystal_plate_model,
+                crystal_plate_object,
                 target,
             )
 
             # Append well model to the list of all wells on the plate.
             crystal_well_models.append(crystal_well_model)
 
         # Here we create or update the crystal well records into xchembku.
@@ -327,45 +333,41 @@
         # TODO: Handle case where we upsert the crystal_well record but then unable to copy image file.
         shutil.copytree(
             plate_directory,
             target,
         )
 
         logger.info(
-            f"copied {len(well_names)} well images from plate {plate_directory.name} to {target}"
+            f"copied {len(subwell_names)} well images from plate {plate_directory.name} to {target}"
         )
 
         # Remember we "handled" this one.
         self.__handled_plate_names.append(plate_directory.stem)
 
     # ----------------------------------------------------------------------------------------
     async def ingest_well(
         self,
         plate_directory: Path,
-        well_name: str,
+        subwell_name: str,
         crystal_plate_model: CrystalPlateModel,
+        crystal_plate_object: CrystalPlateInterface,
         target: Path,
     ) -> CrystalWellModel:
         """
         Ingest the well into the database.
 
         Move the well image file to the ingested area.
         """
 
-        input_well_filename = plate_directory / well_name
-        ingested_well_filename = target / well_name
+        input_well_filename = plate_directory / subwell_name
+        ingested_well_filename = target / subwell_name
 
         # Stems are like "9acx_01A_1".
-        # TODO: Improve safety by ignoring wrongly formatted and non-jpg well filenames.
-        parts = Path(well_name).stem.split("_")
-        if len(parts) > 1:
-            # Strip off the leading 4-letter barcode and underscore.
-            position = "".join(parts[1:])
-        else:
-            position = parts[0]
+        # Convert the stem into a position as shown in soakdb3.
+        position = crystal_plate_object.normalize_subwell_name(subwell_name)
 
         error = None
         try:
             image = Image.open(input_well_filename)
             width, height = image.size
         except Exception as exception:
             error = str(exception)
```

### Comparing `rockingester-2.1.0/src/rockingester_lib/contexts/base.py` & `rockingester-2.2.0/src/rockingester_lib/contexts/base.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/src/rockingester_lib/exceptions.py` & `rockingester-2.2.0/src/rockingester_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/src/rockingester_lib/version.py` & `rockingester-2.2.0/src/rockingester_lib/version.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/tests/base.py` & `rockingester-2.2.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/tests/configurations/direct_poll.yaml` & `rockingester-2.2.0/tests/configurations/direct_poll.yaml`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/tests/configurations/service.yaml` & `rockingester-2.2.0/tests/configurations/service.yaml`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/tests/conftest.py` & `rockingester-2.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.1.0/tests/test_collector.py` & `rockingester-2.2.0/tests/test_collector.py`

 * *Files 4% similar despite different names*

```diff
@@ -137,18 +137,20 @@
         """ """
         # Reference the xchembku object which the context has set up as the default.
         xchembku = xchembku_datafaces_get_default()
 
         # Make the plate on which the wells reside.
         visit = "cm00001-1_otherstuff"
         created_crystal_plate_models = []
+
+        scrabable_barcode = "98ab"
         created_crystal_plate_models.append(
             CrystalPlateModel(
                 formulatrix__plate__id=10,
-                barcode="98ab",
+                barcode=scrabable_barcode,
                 visit=visit,
                 thing_type=CrystalPlateObjectThingTypes.SWISS3,
             )
         )
 
         nobarcode_barcode = "98ac"
 
@@ -179,52 +181,52 @@
 
         plates_directory = Path(output_directory) / "SubwellImages"
 
         # Make the scrapable directory with some files.
         # This one gets scraped as normal.
         plate_directory1 = plates_directory / "98ab_2023-04-06_RI1000-0276-3drop"
         plate_directory1.mkdir(parents=True)
-        for i in range(10, 10 + scrapable_image_count):
-            filename = plate_directory1 / ("98ab_%03dA_1.jpg" % (i))
+        for i in range(scrapable_image_count):
+            filename = plate_directory1 / self.__subwell_filename(scrabable_barcode, i)
             with open(filename, "w") as stream:
                 stream.write("")
 
         # Make another scrapable directory with a different barcode.
         # This one gets ignored since it doesn't match any plate's barcode.
         plate_directory2 = (
             plates_directory / f"{nobarcode_barcode}_2023-04-06_RI1000-0276-3drop"
         )
         plate_directory2.mkdir(parents=True)
         nobarcode_image_count = 3
-        for i in range(10, 10 + nobarcode_image_count):
-            filename = plate_directory2 / ("%s_%03dA_1.jpg" % (nobarcode_barcode, i))
+        for i in range(nobarcode_image_count):
+            filename = plate_directory2 / self.__subwell_filename(nobarcode_barcode, i)
             with open(filename, "w") as stream:
                 stream.write("")
 
         # Make yet another scrapable directory with a different barcode.
         # This one gets ignored since it matches a plate with a bad visit name.
         plate_directory3 = (
             plates_directory / f"{novisit_barcode}_2023-04-06_RI1000-0276-3drop"
         )
         plate_directory3.mkdir(parents=True)
         novisit_image_count = 6
-        for i in range(10, 10 + novisit_image_count):
-            filename = plate_directory3 / ("%s_%03dA_1.jpg" % (novisit_barcode, i))
+        for i in range(novisit_image_count):
+            filename = plate_directory3 / self.__subwell_filename(novisit_barcode, i)
             with open(filename, "w") as stream:
                 stream.write("")
 
         # Make yet another scrapable directory with a different barcode.
         # This one gets completely ignored because it's not in the explicit list.
         plate_directory4 = (
             plates_directory / f"{excluded_barcode}_2023-04-06_RI1000-0276-3drop"
         )
         plate_directory4.mkdir(parents=True)
         excluded_image_count = 2
-        for i in range(10, 10 + excluded_image_count):
-            filename = plate_directory4 / ("%s_%03dA_1.jpg" % (excluded_barcode, i))
+        for i in range(excluded_image_count):
+            filename = plate_directory4 / self.__subwell_filename(excluded_barcode, i)
             with open(filename, "w") as stream:
                 stream.write("")
 
         # Wait for all the images to appear.
         time0 = time.time()
         timeout = 5.0
         while True:
@@ -255,18 +257,16 @@
         # Get all images in the database.
         crystal_well_models = await xchembku.fetch_crystal_wells_filenames()
         assert (
             len(crystal_well_models) == scrapable_image_count
         ), "images after scraping"
 
         # Make sure the positions got recorded right in the wells.
-        i = 10
-        for crystal_well_model in crystal_well_models:
-            assert crystal_well_model.position == "%03dA1" % (i)
-            i += 1
+        assert crystal_well_models[0].position == "A01a"
+        assert crystal_well_models[-1].position == "H12d"
 
         # The first "scrapable" plate directory should still exist.
         count = sum(1 for _ in plate_directory1.glob("*") if _.is_file())
         assert count == scrapable_image_count, "first (scrapable) plate_directory"
 
         # The second "nobarcode" plate directory should still exist.
         count = sum(1 for _ in plate_directory2.glob("*") if _.is_file())
@@ -301,7 +301,25 @@
         xchembku = xchembku_datafaces_get_default()
 
         await asyncio.sleep(2.0)
         # Get all images after servers start up and run briefly.
         records = await xchembku.fetch_crystal_wells_filenames()
 
         assert len(records) == scrapable_image_count, "images after restarting scraper"
+
+    # ----------------------------------------------------------------------------------------
+
+    def __subwell_filename(self, barcode, index):
+        """
+        Make a subwell image name which can be parsed by swiss3.
+        """
+
+        well_letters = "ABCDEFGH"
+
+        well = int(index / 3)
+        subwell = index % 3 + 1
+        row = well_letters[int(well / 12)]
+        col = "%02d" % (well % 12 + 1)
+
+        subwell_filename = f"{barcode}_{col}{row}_{subwell}"
+
+        return subwell_filename
```

