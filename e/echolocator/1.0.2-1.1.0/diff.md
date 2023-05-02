# Comparing `tmp/echolocator-1.0.2.tar.gz` & `tmp/echolocator-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echolocator-1.0.2.tar", last modified: Wed Apr 26 08:01:54 2023, max compression
+gzip compressed data, was "echolocator-1.1.0.tar", last modified: Tue May  2 11:09:31 2023, max compression
```

## Comparing `echolocator-1.0.2.tar` & `echolocator-1.1.0.tar`

### file list

```diff
@@ -1,225 +1,228 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.968341 echolocator-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.932341 echolocator-1.0.2/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-04-26 08:01:44.000000 echolocator-1.0.2/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.936341 echolocator-1.0.2/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-26 08:01:44.000000 echolocator-1.0.2/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-26 08:01:44.000000 echolocator-1.0.2/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-26 08:01:44.000000 echolocator-1.0.2/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-26 08:01:44.000000 echolocator-1.0.2/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-26 08:01:44.000000 echolocator-1.0.2/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-26 08:01:44.000000 echolocator-1.0.2/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-26 08:01:44.000000 echolocator-1.0.2/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-26 08:01:44.000000 echolocator-1.0.2/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.936341 echolocator-1.0.2/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-26 08:01:44.000000 echolocator-1.0.2/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-04-26 08:01:44.000000 echolocator-1.0.2/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.936341 echolocator-1.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-26 08:01:44.000000 echolocator-1.0.2/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.924341 echolocator-1.0.2/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.936341 echolocator-1.0.2/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-26 08:01:44.000000 echolocator-1.0.2/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-26 08:01:44.000000 echolocator-1.0.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.936341 echolocator-1.0.2/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-26 08:01:44.000000 echolocator-1.0.2/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-26 08:01:44.000000 echolocator-1.0.2/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.936341 echolocator-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-04-26 08:01:44.000000 echolocator-1.0.2/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-26 08:01:44.000000 echolocator-1.0.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-26 08:01:44.000000 echolocator-1.0.2/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-26 08:01:44.000000 echolocator-1.0.2/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-26 08:01:44.000000 echolocator-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-26 08:01:44.000000 echolocator-1.0.2/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-26 08:01:44.000000 echolocator-1.0.2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.936341 echolocator-1.0.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-26 08:01:44.000000 echolocator-1.0.2/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-26 08:01:44.000000 echolocator-1.0.2/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-26 08:01:44.000000 echolocator-1.0.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-26 08:01:44.000000 echolocator-1.0.2/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 08:01:44.000000 echolocator-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-04-26 08:01:44.000000 echolocator-1.0.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    14215 2023-04-26 08:01:54.968341 echolocator-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-26 08:01:44.000000 echolocator-1.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.936341 echolocator-1.0.2/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-04-26 08:01:44.000000 echolocator-1.0.2/configurations/development.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.940341 echolocator-1.0.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.940341 echolocator-1.0.2/docs/1_tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/1_tutorials/101_run_conda.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/1_tutorials/102_update_image.rst
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/1_tutorials.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.940341 echolocator-1.0.2/docs/2_how-to/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/2_how-to/201_add_fields.rst
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/2_how-to.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.940341 echolocator-1.0.2/docs/3_explanations/
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/3_explanations/301_naming_conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/3_explanations/302_process.rst
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/3_explanations.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.940341 echolocator-1.0.2/docs/4_reference/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/4_reference/402_building_conda.rst
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/4_reference.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.940341 echolocator-1.0.2/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.940341 echolocator-1.0.2/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/_static/theme_overrides.css
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.944341 echolocator-1.0.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12006 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/images/excalidraw-example.svg
--rw-r--r--   0 runner    (1001) docker     (123)    21331 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/images/git_merge.png
--rw-r--r--   0 runner    (1001) docker     (123)   703604 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/images/image_details.png
--rw-r--r--   0 runner    (1001) docker     (123)   135258 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/images/image_list.png
--rw-r--r--   0 runner    (1001) docker     (123)   142461 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/images/swiss3.png
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-26 08:01:44.000000 echolocator-1.0.2/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.944341 echolocator-1.0.2/modulefiles/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-26 08:01:44.000000 echolocator-1.0.2/modulefiles/conda
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-26 08:01:44.000000 echolocator-1.0.2/modulefiles/paths
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-04-26 08:01:44.000000 echolocator-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 08:01:54.968341 echolocator-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.928341 echolocator-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.944341 echolocator-1.0.2/src/echolocator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14215 2023-04-26 08:01:54.000000 echolocator-1.0.2/src/echolocator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-04-26 08:01:54.000000 echolocator-1.0.2/src/echolocator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 08:01:54.000000 echolocator-1.0.2/src/echolocator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-26 08:01:54.000000 echolocator-1.0.2/src/echolocator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-26 08:01:54.000000 echolocator-1.0.2/src/echolocator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-26 08:01:54.000000 echolocator-1.0.2/src/echolocator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.944341 echolocator-1.0.2/src/echolocator_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_api/aiohttp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_api/context_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.944341 echolocator-1.0.2/src/echolocator_api/databases/
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_api/databases/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.948341 echolocator-1.0.2/src/echolocator_api/guis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_api/guis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_api/guis/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_api/guis/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_api/guis/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_api/guis/guis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.948341 echolocator-1.0.2/src/echolocator_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.948341 echolocator-1.0.2/src/echolocator_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_cli/subcommands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.948341 echolocator-1.0.2/src/echolocator_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 08:01:54.000000 echolocator-1.0.2/src/echolocator_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.948341 echolocator-1.0.2/src/echolocator_lib/composers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/composers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/composers/composers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/composers/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/composers/prettyhelper.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/composers/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.952341 echolocator-1.0.2/src/echolocator_lib/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/contexts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/envvar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.952341 echolocator-1.0.2/src/echolocator_lib/guis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19340 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/guis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.952341 echolocator-1.0.2/src/echolocator_lib/guis/html/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.952341 echolocator-1.0.2/src/echolocator_lib/guis/html/css/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/css/image_edit_ux.css
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/css/image_list_ux.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.952341 echolocator-1.0.2/src/echolocator_lib/guis/html/css/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/css/images/dls_logo_50x50.png
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/css/pixel_ux.css
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/css/styles.css
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/css/system_health_ux.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.952341 echolocator-1.0.2/src/echolocator_lib/guis/html/images/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/images/green_dot_crosshair.png
--rw-r--r--   0 runner    (1001) docker     (123)   105264 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/images/radial1.666.png
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.956341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.956341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/common/base.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.956341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/echolocator/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/echolocator/events.js
--rw-r--r--   0 runner    (1001) docker     (123)    17332 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/echolocator/image_edit_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/echolocator/image_list_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/echolocator/page.js
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/echolocator/pixel_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/echolocator/system_health_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/echolocator/tabs_manager.js
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/echolocator/ux_auto_update.js
--rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/echolocator/ux_base.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.928341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jquery/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.956341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/jquery.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.928341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.960341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/
--rw-r--r--   0 runner    (1001) docker     (123)    30801 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   255077 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.928341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.960341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.964341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_dadada_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)    18024 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.928341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/raphael/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.964341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    92764 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/raphael.min.js
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/runtime.js
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/version.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.964341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.964341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/box/
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/box/two_corners.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.964341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/chart_area/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/chart_area/chart_area.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.964341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/hair/
--rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/hair/guide2.js
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/hair/guide4.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.964341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/histogram/
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/histogram/histogram.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.964341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/image_area/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/image_area/image_area.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.964341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/justgage/
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/justgage/gauge.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.964341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    38111 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/justgage.js
--rw-r--r--   0 runner    (1001) docker     (123)    92764 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/raphael-2.1.4.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/spreader.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.964341 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/sprite/
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/sprite/shape.js
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/transformer.js
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/targeting.html
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/guis/html/targeting.js
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-26 08:01:44.000000 echolocator-1.0.2/src/echolocator_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.968341 echolocator-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:44.000000 echolocator-1.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-04-26 08:01:44.000000 echolocator-1.0.2/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.968341 echolocator-1.0.2/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-26 08:01:44.000000 echolocator-1.0.2/tests/configurations/service.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-04-26 08:01:44.000000 echolocator-1.0.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.968341 echolocator-1.0.2/tests/example_images/
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-04-26 08:01:44.000000 echolocator-1.0.2/tests/example_images/1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-04-26 08:01:44.000000 echolocator-1.0.2/tests/example_images/2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    19595 2023-04-26 08:01:44.000000 echolocator-1.0.2/tests/example_images/3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-04-26 08:01:44.000000 echolocator-1.0.2/tests/example_images/4.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 08:01:54.968341 echolocator-1.0.2/tests/images/
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-04-26 08:01:44.000000 echolocator-1.0.2/tests/images/1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-04-26 08:01:44.000000 echolocator-1.0.2/tests/images/2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    19595 2023-04-26 08:01:44.000000 echolocator-1.0.2/tests/images/3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-04-26 08:01:44.000000 echolocator-1.0.2/tests/test_droplocation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10089 2023-04-26 08:01:44.000000 echolocator-1.0.2/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     9169 2023-04-26 08:01:44.000000 echolocator-1.0.2/tests/test_fetch_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     8565 2023-04-26 08:01:44.000000 echolocator-1.0.2/tests/test_fetch_images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.688869 echolocator-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.672869 echolocator-1.1.0/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-02 11:09:23.000000 echolocator-1.1.0/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.672869 echolocator-1.1.0/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-02 11:09:23.000000 echolocator-1.1.0/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-02 11:09:23.000000 echolocator-1.1.0/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-02 11:09:23.000000 echolocator-1.1.0/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-02 11:09:23.000000 echolocator-1.1.0/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-02 11:09:23.000000 echolocator-1.1.0/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-02 11:09:23.000000 echolocator-1.1.0/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-02 11:09:23.000000 echolocator-1.1.0/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-02 11:09:23.000000 echolocator-1.1.0/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.672869 echolocator-1.1.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-02 11:09:23.000000 echolocator-1.1.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-02 11:09:23.000000 echolocator-1.1.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.672869 echolocator-1.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-02 11:09:23.000000 echolocator-1.1.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.668869 echolocator-1.1.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.672869 echolocator-1.1.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-02 11:09:23.000000 echolocator-1.1.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-02 11:09:23.000000 echolocator-1.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.672869 echolocator-1.1.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-02 11:09:23.000000 echolocator-1.1.0/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-02 11:09:23.000000 echolocator-1.1.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.672869 echolocator-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-05-02 11:09:23.000000 echolocator-1.1.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-02 11:09:23.000000 echolocator-1.1.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-02 11:09:23.000000 echolocator-1.1.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-02 11:09:23.000000 echolocator-1.1.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-02 11:09:23.000000 echolocator-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-02 11:09:23.000000 echolocator-1.1.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-02 11:09:23.000000 echolocator-1.1.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.672869 echolocator-1.1.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-02 11:09:23.000000 echolocator-1.1.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-02 11:09:23.000000 echolocator-1.1.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-02 11:09:23.000000 echolocator-1.1.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-02 11:09:23.000000 echolocator-1.1.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-02 11:09:23.000000 echolocator-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-05-02 11:09:23.000000 echolocator-1.1.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    14215 2023-05-02 11:09:31.688869 echolocator-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-02 11:09:23.000000 echolocator-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.672869 echolocator-1.1.0/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-02 11:09:23.000000 echolocator-1.1.0/configurations/development.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.676869 echolocator-1.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.676869 echolocator-1.1.0/docs/1_tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/1_tutorials/101_run_conda.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/1_tutorials/102_update_image.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/1_tutorials.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.676869 echolocator-1.1.0/docs/2_how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/2_how-to/201_add_fields.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/2_how-to.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.676869 echolocator-1.1.0/docs/3_explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/3_explanations/301_naming_conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/3_explanations/302_process.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/3_explanations.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.676869 echolocator-1.1.0/docs/4_reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/4_reference/402_building_conda.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/4_reference.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.676869 echolocator-1.1.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.676869 echolocator-1.1.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/_static/theme_overrides.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.676869 echolocator-1.1.0/docs/diagrams/
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/diagrams/3drop_texrank_coordinates.drawio
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.676869 echolocator-1.1.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12006 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/images/excalidraw-example.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    21331 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/images/git_merge.png
+-rw-r--r--   0 runner    (1001) docker     (123)   703604 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/images/image_details.png
+-rw-r--r--   0 runner    (1001) docker     (123)   135258 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/images/image_list.png
+-rw-r--r--   0 runner    (1001) docker     (123)   142461 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/images/swiss3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-02 11:09:23.000000 echolocator-1.1.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.676869 echolocator-1.1.0/modulefiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-02 11:09:23.000000 echolocator-1.1.0/modulefiles/conda
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-02 11:09:23.000000 echolocator-1.1.0/modulefiles/paths
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-05-02 11:09:23.000000 echolocator-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 11:09:31.688869 echolocator-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.668869 echolocator-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.680869 echolocator-1.1.0/src/echolocator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14215 2023-05-02 11:09:31.000000 echolocator-1.1.0/src/echolocator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-05-02 11:09:31.000000 echolocator-1.1.0/src/echolocator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 11:09:31.000000 echolocator-1.1.0/src/echolocator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-02 11:09:31.000000 echolocator-1.1.0/src/echolocator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-02 11:09:31.000000 echolocator-1.1.0/src/echolocator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-02 11:09:31.000000 echolocator-1.1.0/src/echolocator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.680869 echolocator-1.1.0/src/echolocator_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_api/aiohttp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_api/context_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.680869 echolocator-1.1.0/src/echolocator_api/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_api/databases/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.680869 echolocator-1.1.0/src/echolocator_api/guis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_api/guis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_api/guis/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_api/guis/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_api/guis/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_api/guis/guis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.680869 echolocator-1.1.0/src/echolocator_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.680869 echolocator-1.1.0/src/echolocator_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_cli/subcommands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.680869 echolocator-1.1.0/src/echolocator_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-02 11:09:31.000000 echolocator-1.1.0/src/echolocator_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.680869 echolocator-1.1.0/src/echolocator_lib/composers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/composers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/composers/composers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/composers/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/composers/prettyhelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/composers/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.680869 echolocator-1.1.0/src/echolocator_lib/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/contexts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/envvar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.680869 echolocator-1.1.0/src/echolocator_lib/guis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19411 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/guis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.684869 echolocator-1.1.0/src/echolocator_lib/guis/html/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.684869 echolocator-1.1.0/src/echolocator_lib/guis/html/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/css/image_edit_ux.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/css/image_list_ux.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.684869 echolocator-1.1.0/src/echolocator_lib/guis/html/css/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/css/images/dls_logo_50x50.png
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/css/pixel_ux.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/css/styles.css
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/css/system_health_ux.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.684869 echolocator-1.1.0/src/echolocator_lib/guis/html/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/images/green_dot_crosshair.png
+-rw-r--r--   0 runner    (1001) docker     (123)   105264 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/images/radial1.666.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.684869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.684869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/common/base.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.684869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/centroid_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/events.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19245 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/image_edit_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/image_list_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/page.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/pixel_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/system_health_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/tabs_manager.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/ux_auto_update.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/ux_base.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.668869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jquery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.684869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/jquery.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.668869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.684869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    30801 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   255077 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.668869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.684869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.688869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_dadada_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18024 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.668869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/raphael/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.688869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    92764 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/raphael.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/runtime.js
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/version.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.688869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.688869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/box/
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/box/two_corners.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.688869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/chart_area/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/chart_area/chart_area.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.688869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/hair/
+-rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/hair/guide2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/hair/guide4.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.688869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/histogram/
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/histogram/histogram.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.688869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/image_area/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/image_area/image_area.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.688869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/justgage/
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/justgage/gauge.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.688869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    38111 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/justgage.js
+-rw-r--r--   0 runner    (1001) docker     (123)    92764 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/raphael-2.1.4.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/spreader.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.688869 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/sprite/
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/sprite/shape.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/transformer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/targeting.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/guis/html/targeting.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-02 11:09:23.000000 echolocator-1.1.0/src/echolocator_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.688869 echolocator-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:23.000000 echolocator-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-05-02 11:09:23.000000 echolocator-1.1.0/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.688869 echolocator-1.1.0/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-02 11:09:23.000000 echolocator-1.1.0/tests/configurations/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-05-02 11:09:23.000000 echolocator-1.1.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.688869 echolocator-1.1.0/tests/example_images/
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-05-02 11:09:23.000000 echolocator-1.1.0/tests/example_images/1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-05-02 11:09:23.000000 echolocator-1.1.0/tests/example_images/2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    19595 2023-05-02 11:09:23.000000 echolocator-1.1.0/tests/example_images/3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-05-02 11:09:23.000000 echolocator-1.1.0/tests/example_images/4.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 11:09:31.688869 echolocator-1.1.0/tests/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-05-02 11:09:23.000000 echolocator-1.1.0/tests/images/1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-05-02 11:09:23.000000 echolocator-1.1.0/tests/images/2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    19595 2023-05-02 11:09:23.000000 echolocator-1.1.0/tests/images/3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-05-02 11:09:23.000000 echolocator-1.1.0/tests/test_droplocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10167 2023-05-02 11:09:23.000000 echolocator-1.1.0/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9169 2023-05-02 11:09:23.000000 echolocator-1.1.0/tests/test_fetch_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-05-02 11:09:23.000000 echolocator-1.1.0/tests/test_fetch_images.py
```

### Comparing `echolocator-1.0.2/.dae-devops/Makefile` & `echolocator-1.1.0/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/.dae-devops/docs/conventions.rst` & `echolocator-1.1.0/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/.dae-devops/docs/developing.rst` & `echolocator-1.1.0/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/.dae-devops/docs/devops.rst` & `echolocator-1.1.0/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/.dae-devops/docs/docs_structure.rst` & `echolocator-1.1.0/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/.dae-devops/docs/installing.rst` & `echolocator-1.1.0/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/.dae-devops/docs/testing.rst` & `echolocator-1.1.0/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/.dae-devops/project.yaml` & `echolocator-1.1.0/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/.devcontainer/Dockerfile` & `echolocator-1.1.0/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/.devcontainer/devcontainer.json` & `echolocator-1.1.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/.github/CONTRIBUTING.rst` & `echolocator-1.1.0/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/.github/actions/install_requirements/action.yml` & `echolocator-1.1.0/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/.github/dependabot.yml` & `echolocator-1.1.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/.github/pages/make_switcher.py` & `echolocator-1.1.0/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/.github/workflows/code.yml` & `echolocator-1.1.0/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/.github/workflows/docs.yml` & `echolocator-1.1.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/.github/workflows/docs_clean.yml` & `echolocator-1.1.0/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/.github/workflows/linkcheck.yml` & `echolocator-1.1.0/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/.gitignore` & `echolocator-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/.gitlab-ci.yml` & `echolocator-1.1.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/.vscode/launch.json` & `echolocator-1.1.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/LICENSE` & `echolocator-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/Makefile` & `echolocator-1.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/PKG-INFO` & `echolocator-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echolocator
-Version: 1.0.2
+Version: 1.1.0
 Summary: XChem GUI for manually targeting drop points for the Echo dispenser.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `echolocator-1.0.2/README.rst` & `echolocator-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/configurations/development.yaml` & `echolocator-1.1.0/configurations/development.yaml`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/docs/1_tutorials/101_run_conda.rst` & `echolocator-1.1.0/docs/1_tutorials/101_run_conda.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/docs/1_tutorials/102_update_image.rst` & `echolocator-1.1.0/docs/1_tutorials/102_update_image.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/docs/2_how-to/201_add_fields.rst` & `echolocator-1.1.0/docs/2_how-to/201_add_fields.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/docs/3_explanations/301_naming_conventions.rst` & `echolocator-1.1.0/docs/3_explanations/301_naming_conventions.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/docs/3_explanations/302_process.rst` & `echolocator-1.1.0/docs/3_explanations/302_process.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/docs/4_reference/402_building_conda.rst` & `echolocator-1.1.0/docs/4_reference/402_building_conda.rst`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/docs/_static/theme_overrides.css` & `echolocator-1.1.0/docs/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/docs/conf.py` & `echolocator-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/docs/images/dls-favicon.ico` & `echolocator-1.1.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/docs/images/dls-logo.svg` & `echolocator-1.1.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/docs/images/excalidraw-example.svg` & `echolocator-1.1.0/docs/images/excalidraw-example.svg`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/docs/images/git_merge.png` & `echolocator-1.1.0/docs/images/git_merge.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/docs/images/image_details.png` & `echolocator-1.1.0/docs/images/image_details.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/docs/images/image_list.png` & `echolocator-1.1.0/docs/images/image_list.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/docs/images/swiss3.png` & `echolocator-1.1.0/docs/images/swiss3.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/modulefiles/conda` & `echolocator-1.1.0/modulefiles/conda`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/pyproject.toml` & `echolocator-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator.egg-info/PKG-INFO` & `echolocator-1.1.0/src/echolocator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echolocator
-Version: 1.0.2
+Version: 1.1.0
 Summary: XChem GUI for manually targeting drop points for the Echo dispenser.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `echolocator-1.0.2/src/echolocator.egg-info/SOURCES.txt` & `echolocator-1.1.0/src/echolocator.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 docs/1_tutorials/102_update_image.rst
 docs/2_how-to/201_add_fields.rst
 docs/3_explanations/301_naming_conventions.rst
 docs/3_explanations/302_process.rst
 docs/4_reference/402_building_conda.rst
 docs/_static/theme_overrides.css
 docs/_static/css/custom.css
+docs/diagrams/3drop_texrank_coordinates.drawio
 docs/images/dls-favicon.ico
 docs/images/dls-logo.svg
 docs/images/excalidraw-example.svg
 docs/images/git_merge.png
 docs/images/image_details.png
 docs/images/image_list.png
 docs/images/swiss3.png
@@ -105,14 +106,15 @@
 src/echolocator_lib/guis/html/css/system_health_ux.css
 src/echolocator_lib/guis/html/css/images/dls_logo_50x50.png
 src/echolocator_lib/guis/html/images/green_dot_crosshair.png
 src/echolocator_lib/guis/html/images/radial1.666.png
 src/echolocator_lib/guis/html/javascript/runtime.js
 src/echolocator_lib/guis/html/javascript/version.js
 src/echolocator_lib/guis/html/javascript/common/base.js
+src/echolocator_lib/guis/html/javascript/echolocator/centroid_ux.js
 src/echolocator_lib/guis/html/javascript/echolocator/events.js
 src/echolocator_lib/guis/html/javascript/echolocator/image_edit_ux.js
 src/echolocator_lib/guis/html/javascript/echolocator/image_list_ux.js
 src/echolocator_lib/guis/html/javascript/echolocator/page.js
 src/echolocator_lib/guis/html/javascript/echolocator/pixel_ux.js
 src/echolocator_lib/guis/html/javascript/echolocator/system_health_ux.js
 src/echolocator_lib/guis/html/javascript/echolocator/tabs_manager.js
```

### Comparing `echolocator-1.0.2/src/echolocator_api/context_base.py` & `echolocator-1.1.0/src/echolocator_api/context_base.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_api/databases/constants.py` & `echolocator-1.1.0/src/echolocator_api/databases/constants.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_api/exceptions.py` & `echolocator-1.1.0/src/echolocator_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_api/guis/aiohttp.py` & `echolocator-1.1.0/src/echolocator_api/guis/aiohttp.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_api/guis/context.py` & `echolocator-1.1.0/src/echolocator_api/guis/context.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_api/guis/guis.py` & `echolocator-1.1.0/src/echolocator_api/guis/guis.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_cli/main.py` & `echolocator-1.1.0/src/echolocator_cli/main.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_cli/subcommands/base.py` & `echolocator-1.1.0/src/echolocator_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_cli/subcommands/service.py` & `echolocator-1.1.0/src/echolocator_cli/subcommands/service.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_cli/version.py` & `echolocator-1.1.0/src/echolocator_cli/version.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/__main__.py` & `echolocator-1.1.0/src/echolocator_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/composers/composers.py` & `echolocator-1.1.0/src/echolocator_lib/composers/composers.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/composers/html.py` & `echolocator-1.1.0/src/echolocator_lib/composers/html.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             {"text": "#Crystals", "class": "T_number_of_crystals"},
             {"text": "Offset x (\u03BCm)", "class": "T_real_space_target_x"},
             {"text": "Offset y (\u03BCm)", "class": "T_real_space_target_y"},
             {"text": "drop", "class": "T_is_drop"},
             {"text": "well centroid x,y", "class": "T_well_centroid_x_y"},
             {"text": "auto x,y", "class": "T_auto_target_x_y"},
             {"text": "confirmed x,y", "class": "T_confirmed_target_x_y"},
-            {"text": "echo coordinate x,y", "class": "T_echo_coordinate_x_y"},
+            {"text": "echo coordinate x,y", "class": "T_confirmed_microns_x_y"},
             {"text": "use", "class": "T_is_usable"},
             {"text": "error", "class": "T_error"},
         ]
 
         html_lines = []
 
         html_lines.append("<table>")
@@ -142,19 +142,19 @@
 
             if model.confirmed_target_x is None or model.confirmed_target_y is None:
                 t = "-"
             else:
                 t = f"{model.confirmed_target_x}, {model.confirmed_target_y}"
             html_lines.append("<td class='T_confirmed_target_x_y'>" + t + "</td>")
 
-            if model.echo_coordinate_x is None or model.echo_coordinate_y is None:
+            if model.confirmed_microns_x is None or model.confirmed_microns_y is None:
                 t = "-"
             else:
-                t = f"{model.echo_coordinate_x}, {model.echo_coordinate_y}"
-            html_lines.append("<td class='T_echo_coordinate_x_y'>" + t + "</td>")
+                t = f"{model.confirmed_microns_x}, {model.confirmed_microns_y}"
+            html_lines.append("<td class='T_confirmed_microns_x_y'>" + t + "</td>")
 
             t = model.is_usable
             if t is None:
                 t = "-"
             elif t:
                 t = "yes"
             else:
```

### Comparing `echolocator-1.0.2/src/echolocator_lib/composers/prettyhelper.py` & `echolocator-1.1.0/src/echolocator_lib/composers/prettyhelper.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/composers/text.py` & `echolocator-1.1.0/src/echolocator_lib/composers/text.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/contexts/base.py` & `echolocator-1.1.0/src/echolocator_lib/contexts/base.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/envvar.py` & `echolocator-1.1.0/src/echolocator_lib/envvar.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/aiohttp.py` & `echolocator-1.1.0/src/echolocator_lib/guis/aiohttp.py`

 * *Files 2% similar despite different names*

```diff
@@ -410,14 +410,15 @@
             raise RuntimeError("visit not submitted with request (programming error)")
 
         visit = visit.strip()
         if visit == "":
             response = {"error": "blank visit was given"}
             return response
 
+        # Get the barcode string submitted from the html form.
         barcode_filter = request_dict.get("barcode_filter")
 
         if barcode_filter is None:
             raise RuntimeError(
                 "barcode_filter not submitted with request (programming error)"
             )
 
@@ -475,31 +476,31 @@
 
         with open(filename, "w", newline="") as f:
             writer = csv.writer(f)
 
             for m in crystal_well_models:
                 row = []
                 row.append(m.position)
-                row.append(m.echo_coordinate_x or "")
-                row.append(m.echo_coordinate_y or "")
+                row.append(m.confirmed_microns_x or "")
+                row.append(m.confirmed_microns_y or "")
                 writer.writerow(row)
 
         response = {
             "confirmation": f"exported {len(crystal_well_models)} rows to {filename}"
         }
 
         soakdb3_crystal_well_models = []
         for m in crystal_well_models:
             soakdb3_crystal_well_models.append(
                 Soakdb3CrystalWellModel(
                     LabVisit=visit,
                     CrystalPlate=crystal_plate_model.rockminer_collected_stem,
                     CrystalWell=m.position,
-                    EchoX=m.echo_coordinate_x,
-                    EchoY=m.echo_coordinate_y,
+                    EchoX=m.confirmed_microns_x,
+                    EchoY=m.confirmed_microns_y,
                 )
             )
 
             # Append well records to soakdb3 database.
             # Soakdb3 wants the "/processing" to be on the end of the visitid.
             await self.__xchembku.inject_soakdb3_crystal_wells(
                 str(visit_directory / "processing"), soakdb3_crystal_well_models
```

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/constants.py` & `echolocator-1.1.0/src/echolocator_lib/guis/constants.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/context.py` & `echolocator-1.1.0/src/echolocator_lib/guis/context.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/guis.py` & `echolocator-1.1.0/src/echolocator_lib/guis/guis.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/css/image_list_ux.css` & `echolocator-1.1.0/src/echolocator_lib/guis/html/css/image_list_ux.css`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/css/images/dls_logo_50x50.png` & `echolocator-1.1.0/src/echolocator_lib/guis/html/css/images/dls_logo_50x50.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/css/styles.css` & `echolocator-1.1.0/src/echolocator_lib/guis/html/css/styles.css`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/images/green_dot_crosshair.png` & `echolocator-1.1.0/src/echolocator_lib/guis/html/images/green_dot_crosshair.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/images/radial1.666.png` & `echolocator-1.1.0/src/echolocator_lib/guis/html/images/radial1.666.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/index.html` & `echolocator-1.1.0/src/echolocator_lib/guis/html/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     <link rel="stylesheet" href="javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css">
 
     <!-- Common javascript classes. -->
     <script src="javascript/common/base.js"></script>
 
     <!-- Classes for screen interaction. -->
     <script src="javascript/raphael/raphael-2.1.4/raphael.min.js"></script>
+    <script src="javascript/webviz/sprite/shape.js"></script>
     <script src="javascript/webviz/hair/guide2.js"></script>
     <script src="javascript/webviz/spreader.js"></script>
     <script src="javascript/webviz/transformer.js"></script>
 
     <!-- Support for all echolocator pages. -->
     <script src="javascript/version.js"></script>
     <script src="javascript/runtime.js"></script>
@@ -30,14 +31,15 @@
     <!-- Logic for this page. -->
     <script src="javascript/echolocator/events.js"></script>
     <script src="javascript/echolocator/ux_base.js"></script>
     <script src="javascript/echolocator/ux_auto_update.js"></script>
     <script src="javascript/echolocator/tabs_manager.js"></script>
     <script src="javascript/echolocator/image_list_ux.js"></script>
     <script src="javascript/echolocator/image_edit_ux.js"></script>
+    <script src="javascript/echolocator/centroid_ux.js"></script>
     <script src="javascript/echolocator/pixel_ux.js"></script>
 
     <!-- javascript companion to html layout -->
     <script src="index.js"></script>
 
     <!-- Styles for this page. -->
     <link rel="stylesheet" href="css/styles.css">
@@ -87,21 +89,26 @@
                         <div class="T_title" title="image list">Image List</div>
                         <div class="T_composed T_image_list" style="overflow:scroll;height: 100%;">-</div>
                     </div>
                 </div>
             </div><!-- tab-image-list -->
 
             <div id="tab-image-edit">
-                <div id="image_edit_ux_interaction_parent">
+                <div id="image_edit_ux_interaction_parent" tabindex="0">
                     <div class="T_buttons T_hide_when_no_image" style="margin-top: 8px; margin-bottom: 8px;">
-                        <button class="T_previous_button" title="previous image">Previous</button>
-                        <button class="T_accept_button" title="accept image">Usable</button>
-                        <button class="T_reject_button" title="reject image">Not Usable</button>
-                        <button class="T_reset_button" title="reset image">Undecided</button>
-                        <button class="T_next_button" title="next image">Next</button>
+                        <button class="T_previous_button" title="previous image">Previous<span class="T_hint"> (left
+                                arrow)</span></button>
+                        <button class="T_accept_button" title="accept image">Usable<span class="T_hint"> (space
+                                bar)</span></space></button>
+                        <button class="T_reject_button" title="reject image">Not Usable<span class="T_hint"> (right
+                                click or X)</span></button>
+                        <button class="T_reset_button" title="reset image">Undecided<span class="T_hint"></span>
+                            (-)</span></button>
+                        <button class="T_next_button" title="next image">Next<span class="T_hint"> (right
+                                arrow)</span></button>
                     </div>
                     <div class="T_help T_hide_when_no_image">Right-click in the image to mark as not usable.</div>
 
                     <div class="T_image_info T_hide_when_no_image" style="margin-top: 8px; margin-bottom: 8px;">
                         <div class="T_field">
                             <div class="T_prompt">filename:</div>
                             <div class="T_input">
```

#### html2text {}

```diff
@@ -21,13 +21,14 @@
 Exports all images on the plate which have been decided.
 barcode
 [                    ]
 show only undecided
 ⁰
 Image List
 -
-Previous Usable Not Usable Undecided Next
+Previous (left arrow) Usable (space bar) Not Usable (right click or X)
+Undecided (-) Next (right arrow)
 Right-click in the image to mark as not usable.
 filename:
 Num crystals:
 is usable?
 [images/radial1.666.png]
```

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/index.js` & `echolocator-1.1.0/src/echolocator_lib/guis/html/index.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/common/base.js` & `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/common/base.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/echolocator/events.js` & `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/events.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/echolocator/image_edit_ux.js` & `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/image_edit_ux.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -76,23 +76,57 @@
 
         // Disable context menu for right-click on the image.
         this.#jquery_objects.$raphael1_paper.contextmenu(function(jquery_event_object) {
             that._handle_canvas_right_click(jquery_event_object);
             return false;
         });
 
+        // Key down anywhere in the tab.
+        this.$interaction_parent.on("keydown", function(jquery_event_object) {
+            // Don't pass the event onward, such as allowing the Tab key to select an element in the tab.
+            if (jquery_event_object.keyCode === 9) {
+                jquery_event_object.preventDefault();
+            }
+
+            console.log(F + ": [KYDOEV]" +
+                " jquery_event_object.keyCode " + jquery_event_object.keyCode +
+                " jquery_event_object.target " + that.node_description(jquery_event_object.target));
+
+            // Left arrow?
+            if (jquery_event_object.keyCode === 37) {
+                that._handle_previous_or_next(-1);
+            }
+            // Space bar?
+            if (jquery_event_object.keyCode === 32) {
+                that._send_update(true);
+            }
+            // X key?
+            if (jquery_event_object.keyCode === 88) {
+                that._send_update(false);
+            }
+            // - key?
+            if (jquery_event_object.keyCode === 189) {
+                that._send_update(null);
+            }
+            // Right arrow?
+            if (jquery_event_object.keyCode === 39) {
+                that._handle_previous_or_next(1);
+            }
+        });
+
         // Set up jquery event handling for DOM elements.
         this.#jquery_objects.previous_button.click(
             function(jquery_event_object) {
                 console.log(F + ": clicked previous");
                 that._handle_previous_or_next(-1);
             });
 
         this.#jquery_objects.accept_button.click(
             function(jquery_event_object) {
+                console.log(F + ": clicked accept");
                 that._send_update(true);
             });
 
         this.#jquery_objects.reject_button.click(
             function(jquery_event_object) {
                 that._send_update(false);
             });
@@ -130,15 +164,15 @@
             echolocator__PixelUx__UserMotionEvent,
             function(event) {
                 that.#is_dragging = true;
             });
 
         // ----------------------------------------------------------
         // Make the crosshair for the well centroid, but it is not draggable.
-        this.#well_centroid_ux = new echolocator__PixelUx(
+        this.#well_centroid_ux = new echolocator__CentroidUx(
             self.runtime,
             "well_centroid",
             this.$interaction_parent,
             "lightblue",
             false);
 
         // ----------------------------------------------------------
@@ -194,15 +228,23 @@
                 "crystal_well_uuid": this.#crystal_well_uuid,
                 "is_usable": is_usable
             }
 
             if (confirmed_target !== undefined) {
                 model["confirmed_target_x"] = confirmed_target.x;
                 model["confirmed_target_y"] = confirmed_target.y;
-
+            }
+            // Caller is confirming the drop target?
+            else if (is_usable === true) {
+                // But no previous drop target has been set?
+                if (this.#record["confirmed_target_x"] === null) {
+                    // Take the confirmed drop target from the auto target.
+                    model["confirmed_target_x"] = this.#record["auto_target_x"];
+                    model["confirmed_target_y"] = this.#record["auto_target_y"];
+                }
             }
 
             json_object["crystal_well_droplocation_model"] = model;
 
             // Tell server to add response["html"] for next image in series.
             json_object[this.SHOULD_ADVANCE] = true;
 
@@ -376,30 +418,30 @@
         };
 
         this.#confirmed_target_ux.set_uuid(this.#crystal_well_uuid, confirmed_target);
 
         // The the pixel ux about the crystal_well_uuid so it can be included in sending changes.
         var x = record.well_centroid_x;
         if (x === null)
-            x = record.auto_target_x;
-        if (x === null)
-            x = 10;
+            x = 100;
 
         var y = record.well_centroid_y;
         if (y === null)
-            y = record.auto_target_y;
-        if (y === null)
-            y = 10;
+            y = 100;
 
         var well_centroid = {
             x: x,
             y: y
         };
+        var image_size = {
+            w: record.width ? record.width : 100,
+            h: record.height ? record.height : 100
+        };
 
-        this.#well_centroid_ux.set_uuid(this.#crystal_well_uuid, well_centroid);
+        this.#well_centroid_ux.set(well_centroid, image_size);
 
         // Let the spreader calculate the available space for the image.
         // This will trigger a call to this.handle_spread_event().
         // This only needs to be here for the very first opening of this tab.
         this.image1_spreader.spread();
 
         // Resize the image to fit on the screen.
@@ -442,14 +484,16 @@
         // Resize the displayed image according to the current screen size.
         this.resize_image()
 
         // Tell pixel_ux to render under the new transformer.
         this.#confirmed_target_ux.render()
         this.#well_centroid_ux.render()
 
+        this.$interaction_parent.focus();
+
     } // end method
 
     // -----------------------------------------------------------------------
     // Resize the displayed image according to the current screen size.
 
     resize_image() {
         var F = "echolocator__ImageEditUx::resize_image";
```

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/echolocator/image_list_ux.js` & `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/image_list_ux.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/echolocator/pixel_ux.js` & `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/pixel_ux.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -81,21 +81,21 @@
     } // end method
 
     // -----------------------------------------------------------------------
     // Render the viewable things according to the current tranformer settings.
     render(event) {
         var F = "echolocator__PixelUx[" + this.plugin_link_name + "]::render"
 
-        console.log(F + ": rendering target [" + this.#target.x + ", " + this.#target.y + "]")
+        // console.log(F + ": [INTERPI] rendering target [" + this.#target.x + ", " + this.#target.y + "]")
 
         // Everything we send or receive from the outside is data coordinates.
         // Convert it to view coordinates which is are used by the guide.
         var view_position = this.#transformer.data_to_view(this.#target);
 
-        console.log(F + ": rendering to view position [" + view_position.x + ", " + view_position.y + "]")
+        // console.log(F + ": [INTERPI] rendering to view position [" + view_position.x + ", " + view_position.y + "]")
 
         // Move the guide to the canvas view location.
         this.#guide.set_box({
             position: view_position
         })
 
     } // end method
```

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/echolocator/system_health_ux.js` & `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/system_health_ux.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/echolocator/tabs_manager.js` & `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/tabs_manager.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/echolocator/ux_auto_update.js` & `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/ux_auto_update.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/echolocator/ux_base.js` & `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/echolocator/ux_base.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/jquery.min.js` & `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jquery/3.6.0/jquery.min.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css` & `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js` & `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png` & `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png` & `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png` & `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png` & `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png` & `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css` & `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/raphael.min.js` & `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/raphael/raphael-2.1.4/raphael.min.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/box/two_corners.js` & `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/box/two_corners.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/chart_area/chart_area.js` & `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/chart_area/chart_area.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/hair/guide2.js` & `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/hair/guide2.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/hair/guide4.js` & `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/hair/guide4.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -4,15 +4,15 @@
 // inherit the base methods and variables
 webviz__hair__Guide4.prototype = new maxiv__common__Base();
 
 // override the constructor
 webviz__hair__Guide4.prototype.constructor = webviz__hair__Guide4;
 
 // -------------------------------------------------------------------------------
-// constructor (functioning as a prototype, this constructor cannot take arguments)
+// Constructor.
 
 function webviz__hair__Guide4(page, name, classname) {
     // we are not doing a prototype construction?
     if (arguments.length > 0) {
         var F = "webviz__hair__Guide4";
 
         this.parent = maxiv__common__Base.prototype;
```

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/histogram/histogram.js` & `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/histogram/histogram.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/image_area/image_area.js` & `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/image_area/image_area.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/justgage/gauge.js` & `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/justgage/gauge.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/justgage.js` & `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/justgage.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/raphael-2.1.4.min.js` & `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/justgage/justgage-1.2.2/raphael-2.1.4.min.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/spreader.js` & `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/spreader.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/javascript/webviz/transformer.js` & `echolocator-1.1.0/src/echolocator_lib/guis/html/javascript/webviz/transformer.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/targeting.html` & `echolocator-1.1.0/src/echolocator_lib/guis/html/targeting.html`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/guis/html/targeting.js` & `echolocator-1.1.0/src/echolocator_lib/guis/html/targeting.js`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/src/echolocator_lib/version.py` & `echolocator-1.1.0/src/echolocator_lib/version.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/tests/base.py` & `echolocator-1.1.0/tests/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 import os
 
 import pytest
 from dls_multiconf_lib.constants import ThingTypes as MulticonfThingTypes
 
 # Configurator.
 from dls_multiconf_lib.multiconfs import Multiconfs, multiconfs_set_default
+
+# Types which the CrystalPlateObjects factory can use to build an instance.
+from xchembku_api.crystal_plate_objects.constants import (
+    ThingTypes as CrystalPlateObjectThingTypes,
+)
 from xchembku_api.models.crystal_plate_model import CrystalPlateModel
 from xchembku_api.models.crystal_well_autolocation_model import (
     CrystalWellAutolocationModel,
 )
 from xchembku_api.models.crystal_well_droplocation_model import (
     CrystalWellDroplocationModel,
 )
@@ -96,14 +101,15 @@
 
         # Make the plate on which the wells reside.
         crystal_plate_model = CrystalPlateModel(
             formulatrix__plate__id=10,
             barcode=self.barcode,
             rockminer_collected_stem=self.rockminer_collected_stem,
             visit=self.visit,
+            thing_type=CrystalPlateObjectThingTypes.SWISS3,
         )
 
         await xchembku.upsert_crystal_plates([crystal_plate_model])
         self.crystal_plate_uuid = crystal_plate_model.uuid
 
     # ----------------------------------------------------------------------------------------
 
@@ -144,10 +150,10 @@
             t = CrystalWellDroplocationModel(
                 crystal_well_uuid=m.uuid,
                 confirmed_target_x=self.injected_count * 100 + 2,
                 confirmed_target_y=self.injected_count * 100 + 3,
                 is_usable=True,
             )
 
-            await xchembku.originate_crystal_well_droplocations([t])
+            await xchembku.upsert_crystal_well_droplocations([t])
 
         return m
```

### Comparing `echolocator-1.0.2/tests/configurations/service.yaml` & `echolocator-1.1.0/tests/configurations/service.yaml`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/tests/conftest.py` & `echolocator-1.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/tests/example_images/1.jpg` & `echolocator-1.1.0/tests/example_images/1.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/tests/example_images/2.jpg` & `echolocator-1.1.0/tests/example_images/2.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/tests/example_images/3.jpg` & `echolocator-1.1.0/tests/example_images/3.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/tests/example_images/4.png` & `echolocator-1.1.0/tests/example_images/4.png`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/tests/images/1.jpg` & `echolocator-1.1.0/tests/images/1.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/tests/images/2.jpg` & `echolocator-1.1.0/tests/images/2.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/tests/images/3.jpg` & `echolocator-1.1.0/tests/images/3.jpg`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/tests/test_droplocation.py` & `echolocator-1.1.0/tests/test_droplocation.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/tests/test_export.py` & `echolocator-1.1.0/tests/test_export.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,31 +248,32 @@
         assert len(rows) == 3
 
         # Check each row has 3 parts.
         for row in rows:
             assert len(row) == 3
 
         # Check the well positions are those that are considered "confirmed".
+        # The position constants are fromt the Swiss3 microns computation.
         assert rows[0][0] == "02A_1"
-        assert int(rows[0][1]) == -198
-        assert int(rows[0][2]) == -297
+        assert int(rows[0][1]) == -561
+        assert int(rows[0][2]) == -842
         assert rows[1][0] == "04A_1"
-        assert int(rows[1][1]) == 2
-        assert int(rows[1][2]) == -97
+        assert int(rows[1][1]) == 6
+        assert int(rows[1][2]) == -274
         assert rows[2][0] == "05A_1"
-        assert int(rows[2][1]) == 102
-        assert int(rows[2][2]) == 3
+        assert int(rows[2][1]) == 289
+        assert int(rows[2][2]) == 9
 
         # Check the results stored in soakdbb3, there should be no change to the first ones.
         queried_models = await self.__xchembku.fetch_soakdb3_crystal_wells(
             str(self.__visit_directory / "processing")
         )
         assert len(queried_models) == 3
         assert queried_models[0].CrystalWell == "02A_1"
-        assert int(queried_models[0].EchoX) == -198
-        assert int(queried_models[0].EchoY) == -297
+        assert int(queried_models[0].EchoX) == -561
+        assert int(queried_models[0].EchoY) == -842
         assert queried_models[1].CrystalWell == "04A_1"
-        assert int(queried_models[1].EchoX) == 2
-        assert int(queried_models[1].EchoY) == -97
+        assert int(queried_models[1].EchoX) == 6
+        assert int(queried_models[1].EchoY) == -274
         assert queried_models[2].CrystalWell == "05A_1"
-        assert int(queried_models[2].EchoX) == 102
-        assert int(queried_models[2].EchoY) == 3
+        assert int(queried_models[2].EchoX) == 289
+        assert int(queried_models[2].EchoY) == 9
```

### Comparing `echolocator-1.0.2/tests/test_fetch_image.py` & `echolocator-1.1.0/tests/test_fetch_image.py`

 * *Files identical despite different names*

### Comparing `echolocator-1.0.2/tests/test_fetch_images.py` & `echolocator-1.1.0/tests/test_fetch_images.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,22 +9,14 @@
 
 # Utilities.
 from dls_utilpack.describe import describe
 
 # Things xchembku provides.
 from xchembku_api.datafaces.context import Context as XchembkuDatafaceClientContext
 from xchembku_api.datafaces.datafaces import xchembku_datafaces_get_default
-from xchembku_api.models.crystal_plate_model import CrystalPlateModel
-from xchembku_api.models.crystal_well_autolocation_model import (
-    CrystalWellAutolocationModel,
-)
-from xchembku_api.models.crystal_well_droplocation_model import (
-    CrystalWellDroplocationModel,
-)
-from xchembku_api.models.crystal_well_model import CrystalWellModel
 
 # Client context creator.
 from echolocator_api.guis.context import Context as GuiClientContext
 
 # GUI constants.
 from echolocator_lib.guis.constants import Commands, Cookies, Keywords
 
@@ -104,34 +96,23 @@
     async def __run_part1(self, constants, output_directory):
         """ """
         # Reference the xchembku object which the context has set up as the default.
         xchembku = xchembku_datafaces_get_default()
 
         await self.__request_initial()
 
-        # Make the plate on which the wells reside.
-        visit = "cm00001-1"
-        crystal_plate_model = CrystalPlateModel(
-            formulatrix__plate__id=10,
-            barcode="98ab",
-            visit=visit,
-        )
-
-        await xchembku.upsert_crystal_plates([crystal_plate_model])
-        self.__crystal_plate_uuid = crystal_plate_model.uuid
-
         crystal_wells = []
 
         # Inject some wells.
-        crystal_wells.append(await self.__inject(xchembku, False, False))
-        crystal_wells.append(await self.__inject(xchembku, True, True))
-        crystal_wells.append(await self.__inject(xchembku, True, False))
-        crystal_wells.append(await self.__inject(xchembku, True, True))
-        crystal_wells.append(await self.__inject(xchembku, True, True))
-        crystal_wells.append(await self.__inject(xchembku, True, False))
+        crystal_wells.append(await self.inject(xchembku, False, False))
+        crystal_wells.append(await self.inject(xchembku, True, True))
+        crystal_wells.append(await self.inject(xchembku, True, False))
+        crystal_wells.append(await self.inject(xchembku, True, True))
+        crystal_wells.append(await self.inject(xchembku, True, True))
+        crystal_wells.append(await self.inject(xchembku, True, False))
 
         await self.__request_all(crystal_wells)
 
     # ----------------------------------------------------------------------------------------
 
     async def __request_initial(self):
         """ """
@@ -196,50 +177,7 @@
         assert columns[0].get_text() == Path(crystal_wells[1].filename).stem
 
         # Check the last row's filename.
         row = rows[5]
         columns = row.find_all(class_="T_filename")
         assert len(columns) == 1
         assert columns[0].get_text() == Path(crystal_wells[5].filename).stem
-
-    # ----------------------------------------------------------------------------------------
-
-    async def __inject(self, xchembku, autolocation: bool, droplocation: bool):
-        """ """
-        if not hasattr(self, "injected_count"):
-            self.injected_count = 0
-
-        filename = "/tmp/aaaa_%03d_1.jpg" % (self.injected_count)
-
-        # Write well record.
-        m = CrystalWellModel(
-            position="01A_1",
-            filename=filename,
-            crystal_plate_uuid=self.__crystal_plate_uuid,
-        )
-
-        await xchembku.upsert_crystal_wells([m])
-
-        if autolocation:
-            # Add a crystal well autolocation.
-            t = CrystalWellAutolocationModel(
-                crystal_well_uuid=m.uuid,
-                number_of_crystals=self.injected_count,
-                auto_target_x=self.injected_count * 10 + 1,
-                auto_target_y=self.injected_count * 10 + 2,
-            )
-
-            await xchembku.originate_crystal_well_autolocations([t])
-
-        if droplocation:
-            # Add a crystal well droplocation.
-            t = CrystalWellDroplocationModel(
-                crystal_well_uuid=m.uuid,
-                confirmed_target_x=self.injected_count * 10 + 3,
-                confirmed_target_y=self.injected_count * 10 + 4,
-            )
-
-            await xchembku.originate_crystal_well_droplocations([t])
-
-        self.injected_count += 1
-
-        return m
```

