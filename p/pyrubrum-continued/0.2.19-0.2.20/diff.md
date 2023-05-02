# Comparing `tmp/pyrubrum-continued-0.2.19.tar.gz` & `tmp/pyrubrum-continued-0.2.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrubrum-continued-0.2.19.tar", last modified: Wed Apr 26 00:47:30 2023, max compression
+gzip compressed data, was "pyrubrum-continued-0.2.20.tar", last modified: Tue May  2 03:00:28 2023, max compression
```

## Comparing `pyrubrum-continued-0.2.19.tar` & `pyrubrum-continued-0.2.20.tar`

### file list

```diff
@@ -1,178 +1,178 @@
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-26 00:47:30.000000 pyrubrum-continued-0.2.19/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       28 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/.flake8
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-26 00:47:30.000000 pyrubrum-continued-0.2.19/.github/
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-26 00:47:30.000000 pyrubrum-continued-0.2.19/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      635 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      397 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/.github/ISSUE_TEMPLATE/documentation.md
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      625 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      334 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/.github/ISSUE_TEMPLATE/typo.md
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      270 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/.github/dependabot.yml
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     2475 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/.gitignore
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      125 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/.gitmodules
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      571 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/.pre-commit-config.yaml
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)    31212 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/CHANGELOG.md
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3355 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/CODE_OF_CONDUCT.md
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      710 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/CONTRIBUTING.md
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1984 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/FEATURES.md
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)    34878 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/LICENSE
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      282 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/MANIFEST.in
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      715 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/NOTICE
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     6226 2023-04-26 00:47:30.000000 pyrubrum-continued-0.2.19/PKG-INFO
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     4225 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/README.md
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1081 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/SECURITY.md
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     6810 2023-03-19 17:42:06.000000 pyrubrum-continued-0.2.19/changelog_generator.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       52 2023-03-19 17:52:13.000000 pyrubrum-continued-0.2.19/dev-requirements.txt
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-26 00:47:30.000000 pyrubrum-continued-0.2.19/docs/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      638 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/Makefile
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      764 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/make.bat
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-26 00:47:30.000000 pyrubrum-continued-0.2.19/docs/source/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      716 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/CONTRIBUTING.md
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-26 00:47:30.000000 pyrubrum-continued-0.2.19/docs/source/_static/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      710 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/_static/CONTRIBUTING.md
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-26 00:47:30.000000 pyrubrum-continued-0.2.19/docs/source/_static/flowcharts/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3689 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/_static/flowcharts/attributes.png
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)    56344 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/_static/flowcharts/cafe_bot.png
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)    34720 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/_static/flowcharts/calendar_bot.png
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      469 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/_static/flowcharts/deep_link.png
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)    25806 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/_static/flowcharts/hitchhiker_bot.png
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      299 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/_static/flowcharts/inheritance.png
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     5363 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/_static/flowcharts/link.png
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3783 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/_static/flowcharts/menu.png
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)    42294 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/_static/flowcharts/overview-1.png
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)    28709 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/_static/flowcharts/overview.png
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3887 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/_static/flowcharts/page_menu.png
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)    26253 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/_static/flowcharts/sample_bot.png
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-26 00:47:30.000000 pyrubrum-continued-0.2.19/docs/source/api/
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-26 00:47:30.000000 pyrubrum-continued-0.2.19/docs/source/api/database/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       77 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/database/base_database.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       77 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/database/dict_database.rst
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-26 00:47:30.000000 pyrubrum-continued-0.2.19/docs/source/api/database/errors/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       84 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/database/errors/database_error.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       78 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/database/errors/delete_error.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       78 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/database/errors/expire_error.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       69 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/database/errors/get_error.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      177 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/database/errors/index.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       84 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/database/errors/not_found_error.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       69 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/database/errors/set_error.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      117 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/database/index.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       80 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/database/redis_database.rst
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-26 00:47:30.000000 pyrubrum-continued-0.2.19/docs/source/api/handlers/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       74 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/handlers/base_handler.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       62 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/handlers/handler.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      197 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/handlers/index.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      113 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/handlers/parameterized_base_handler.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      101 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/handlers/parameterized_handler.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       66 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/handlers/pass_handler.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      109 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/handlers/pass_parameterized_handler.rst
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-26 00:47:30.000000 pyrubrum-continued-0.2.19/docs/source/api/keyboard/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       59 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/keyboard/button.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       62 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/keyboard/element.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       98 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/keyboard/index.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       65 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/keyboard/keyboard.rst
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-26 00:47:30.000000 pyrubrum-continued-0.2.19/docs/source/api/menus/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       65 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/menus/base_menu.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       78 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/menus/deep_link_menu.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      127 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/menus/index.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       66 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/menus/link_menu.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       53 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/menus/menu.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       65 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/menus/page_menu.rst
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-26 00:47:30.000000 pyrubrum-continued-0.2.19/docs/source/api/objects/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       70 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/objects/index.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       54 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/objects/user.rst
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-26 00:47:30.000000 pyrubrum-continued-0.2.19/docs/source/api/styles/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       69 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/styles/base_style.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      104 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/styles/index.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       69 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/styles/menu_style.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       69 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/styles/page_style.rst
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-26 00:47:30.000000 pyrubrum-continued-0.2.19/docs/source/api/tree/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       95 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/tree/index.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       53 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/tree/node.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       69 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/tree/recursive_add.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       57 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/tree/transform.rst
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-26 00:47:30.000000 pyrubrum-continued-0.2.19/docs/source/api/types/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       67 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/types/index.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       56 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/api/types/types.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     5306 2023-03-19 17:42:06.000000 pyrubrum-continued-0.2.19/docs/source/conf.py
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-26 00:47:30.000000 pyrubrum-continued-0.2.19/docs/source/examples/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      147 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/examples/sample.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1388 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/flowchart.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1458 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/glossary.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     2453 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/index.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      689 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/license.rst
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-26 00:47:30.000000 pyrubrum-continued-0.2.19/docs/source/quickstart/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      761 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/quickstart/installation.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     7519 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs/source/quickstart/overview.rst
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       67 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/docs-requirements.txt
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3825 2023-03-19 17:42:06.000000 pyrubrum-continued-0.2.19/docs_updater.py
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-26 00:47:30.000000 pyrubrum-continued-0.2.19/examples/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3255 2023-04-18 19:43:10.000000 pyrubrum-continued-0.2.19/examples/cafe_bot.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3578 2023-03-19 17:42:06.000000 pyrubrum-continued-0.2.19/examples/calendar_bot.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     2394 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.19/examples/hitchhiker_bot.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       24 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/examples/requirements.txt
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1471 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/examples/sample.env
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1678 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.19/examples/sample_bot.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       16 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/fast-requirements.txt
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       30 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/pyproject.toml
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-26 00:47:30.000000 pyrubrum-continued-0.2.19/pyrubrum/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     2404 2023-04-26 00:47:17.000000 pyrubrum-continued-0.2.19/pyrubrum/__init__.py
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-26 00:47:30.000000 pyrubrum-continued-0.2.19/pyrubrum/database/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      924 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/pyrubrum/database/__init__.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3615 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/pyrubrum/database/base_database.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3369 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/pyrubrum/database/dict_database.py
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-26 00:47:30.000000 pyrubrum-continued-0.2.19/pyrubrum/database/errors/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1042 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/pyrubrum/database/errors/__init__.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1072 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.19/pyrubrum/database/errors/delete_error.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      915 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/pyrubrum/database/errors/error.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1102 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.19/pyrubrum/database/errors/expire_error.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1069 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.19/pyrubrum/database/errors/get_error.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1049 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/pyrubrum/database/errors/not_found_error.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1097 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.19/pyrubrum/database/errors/set_error.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     4714 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.19/pyrubrum/database/redis_database.py
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-26 00:47:30.000000 pyrubrum-continued-0.2.19/pyrubrum/handlers/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1120 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/pyrubrum/handlers/__init__.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     5594 2023-04-18 19:43:10.000000 pyrubrum-continued-0.2.19/pyrubrum/handlers/base_handler.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     6280 2023-04-18 19:58:27.000000 pyrubrum-continued-0.2.19/pyrubrum/handlers/handler.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     9330 2023-04-18 19:58:44.000000 pyrubrum-continued-0.2.19/pyrubrum/handlers/parameterized_base_handler.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     4203 2023-04-18 19:58:52.000000 pyrubrum-continued-0.2.19/pyrubrum/handlers/parameterized_handler.py
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-26 00:47:30.000000 pyrubrum-continued-0.2.19/pyrubrum/keyboard/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      889 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/pyrubrum/keyboard/__init__.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3743 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/pyrubrum/keyboard/button.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1319 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/pyrubrum/keyboard/element.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     2042 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.19/pyrubrum/keyboard/keyboard.py
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-26 00:47:30.000000 pyrubrum-continued-0.2.19/pyrubrum/menus/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1071 2023-03-20 08:21:09.000000 pyrubrum-continued-0.2.19/pyrubrum/menus/__init__.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3695 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.19/pyrubrum/menus/base_menu.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3299 2023-04-25 22:08:03.000000 pyrubrum-continued-0.2.19/pyrubrum/menus/content_page_menu.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     4692 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.19/pyrubrum/menus/deep_link_menu.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3247 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/pyrubrum/menus/link_menu.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     9076 2023-04-25 09:10:06.000000 pyrubrum-continued-0.2.19/pyrubrum/menus/menu.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     4892 2023-03-20 11:18:25.000000 pyrubrum-continued-0.2.19/pyrubrum/menus/page_menu.py
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-26 00:47:30.000000 pyrubrum-continued-0.2.19/pyrubrum/menus/styles/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      904 2023-03-20 07:53:10.000000 pyrubrum-continued-0.2.19/pyrubrum/menus/styles/__init__.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     2033 2023-03-20 08:34:39.000000 pyrubrum-continued-0.2.19/pyrubrum/menus/styles/base_style.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3836 2023-04-26 00:47:04.000000 pyrubrum-continued-0.2.19/pyrubrum/menus/styles/menu_style.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)    11810 2023-04-26 00:47:10.000000 pyrubrum-continued-0.2.19/pyrubrum/menus/styles/page_style.py
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-26 00:47:30.000000 pyrubrum-continued-0.2.19/pyrubrum/objects/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      829 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/pyrubrum/objects/__init__.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     4469 2023-03-19 17:42:06.000000 pyrubrum-continued-0.2.19/pyrubrum/objects/user.py
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-26 00:47:30.000000 pyrubrum-continued-0.2.19/pyrubrum/tree/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      885 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/pyrubrum/tree/__init__.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     6184 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/pyrubrum/tree/node.py
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-26 00:47:30.000000 pyrubrum-continued-0.2.19/pyrubrum/types/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     4370 2023-03-19 17:42:06.000000 pyrubrum-continued-0.2.19/pyrubrum/types/__init__.py
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-26 00:47:30.000000 pyrubrum-continued-0.2.19/pyrubrum_continued.egg-info/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     6226 2023-04-26 00:47:29.000000 pyrubrum-continued-0.2.19/pyrubrum_continued.egg-info/PKG-INFO
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     4626 2023-04-26 00:47:29.000000 pyrubrum-continued-0.2.19/pyrubrum_continued.egg-info/SOURCES.txt
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)        1 2023-04-26 00:47:29.000000 pyrubrum-continued-0.2.19/pyrubrum_continued.egg-info/dependency_links.txt
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       38 2023-04-26 00:47:29.000000 pyrubrum-continued-0.2.19/pyrubrum_continued.egg-info/requires.txt
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)        9 2023-04-26 00:47:29.000000 pyrubrum-continued-0.2.19/pyrubrum_continued.egg-info/top_level.txt
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       14 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/requirements.txt
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       38 2023-04-26 00:47:30.000000 pyrubrum-continued-0.2.19/setup.cfg
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3131 2023-03-19 14:42:30.000000 pyrubrum-continued-0.2.19/setup.py
-drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-04-26 00:47:30.000000 pyrubrum-continued-0.2.19/tests/
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     2001 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/tests/test_deep_link_menu.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1280 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/tests/test_dict_database.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1406 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/tests/test_link_menu.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3119 2023-03-24 07:38:17.000000 pyrubrum-continued-0.2.19/tests/test_menu.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     2747 2023-03-19 17:42:06.000000 pyrubrum-continued-0.2.19/tests/test_node.py
--rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      957 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.19/tests/test_version.py
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-05-02 03:00:28.000000 pyrubrum-continued-0.2.20/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       28 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/.flake8
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-05-02 03:00:28.000000 pyrubrum-continued-0.2.20/.github/
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-05-02 03:00:28.000000 pyrubrum-continued-0.2.20/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      635 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      397 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/.github/ISSUE_TEMPLATE/documentation.md
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      625 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      334 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/.github/ISSUE_TEMPLATE/typo.md
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      270 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/.github/dependabot.yml
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     2475 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/.gitignore
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      125 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/.gitmodules
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      571 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/.pre-commit-config.yaml
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)    31212 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/CHANGELOG.md
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3355 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/CODE_OF_CONDUCT.md
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      710 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/CONTRIBUTING.md
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1984 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/FEATURES.md
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)    34878 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/LICENSE
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      282 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/MANIFEST.in
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      715 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/NOTICE
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     6226 2023-05-02 03:00:28.000000 pyrubrum-continued-0.2.20/PKG-INFO
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     4225 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/README.md
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1081 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/SECURITY.md
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     6810 2023-03-19 17:42:06.000000 pyrubrum-continued-0.2.20/changelog_generator.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       52 2023-03-19 17:52:13.000000 pyrubrum-continued-0.2.20/dev-requirements.txt
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-05-02 03:00:28.000000 pyrubrum-continued-0.2.20/docs/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      638 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/Makefile
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      764 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/make.bat
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-05-02 03:00:28.000000 pyrubrum-continued-0.2.20/docs/source/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      716 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/CONTRIBUTING.md
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-05-02 03:00:28.000000 pyrubrum-continued-0.2.20/docs/source/_static/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      710 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/_static/CONTRIBUTING.md
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-05-02 03:00:28.000000 pyrubrum-continued-0.2.20/docs/source/_static/flowcharts/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3689 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/_static/flowcharts/attributes.png
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)    56344 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/_static/flowcharts/cafe_bot.png
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)    34720 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/_static/flowcharts/calendar_bot.png
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      469 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/_static/flowcharts/deep_link.png
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)    25806 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/_static/flowcharts/hitchhiker_bot.png
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      299 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/_static/flowcharts/inheritance.png
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     5363 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/_static/flowcharts/link.png
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3783 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/_static/flowcharts/menu.png
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)    42294 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/_static/flowcharts/overview-1.png
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)    28709 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/_static/flowcharts/overview.png
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3887 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/_static/flowcharts/page_menu.png
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)    26253 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/_static/flowcharts/sample_bot.png
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-05-02 03:00:28.000000 pyrubrum-continued-0.2.20/docs/source/api/
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-05-02 03:00:28.000000 pyrubrum-continued-0.2.20/docs/source/api/database/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       77 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/database/base_database.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       77 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/database/dict_database.rst
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-05-02 03:00:28.000000 pyrubrum-continued-0.2.20/docs/source/api/database/errors/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       84 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/database/errors/database_error.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       78 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/database/errors/delete_error.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       78 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/database/errors/expire_error.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       69 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/database/errors/get_error.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      177 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/database/errors/index.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       84 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/database/errors/not_found_error.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       69 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/database/errors/set_error.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      117 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/database/index.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       80 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/database/redis_database.rst
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-05-02 03:00:28.000000 pyrubrum-continued-0.2.20/docs/source/api/handlers/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       74 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/handlers/base_handler.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       62 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/handlers/handler.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      197 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/handlers/index.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      113 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/handlers/parameterized_base_handler.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      101 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/handlers/parameterized_handler.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       66 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/handlers/pass_handler.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      109 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/handlers/pass_parameterized_handler.rst
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-05-02 03:00:28.000000 pyrubrum-continued-0.2.20/docs/source/api/keyboard/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       59 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/keyboard/button.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       62 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/keyboard/element.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       98 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/keyboard/index.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       65 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/keyboard/keyboard.rst
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-05-02 03:00:28.000000 pyrubrum-continued-0.2.20/docs/source/api/menus/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       65 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/menus/base_menu.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       78 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/menus/deep_link_menu.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      127 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/menus/index.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       66 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/menus/link_menu.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       53 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/menus/menu.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       65 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/menus/page_menu.rst
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-05-02 03:00:28.000000 pyrubrum-continued-0.2.20/docs/source/api/objects/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       70 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/objects/index.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       54 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/objects/user.rst
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-05-02 03:00:28.000000 pyrubrum-continued-0.2.20/docs/source/api/styles/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       69 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/styles/base_style.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      104 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/styles/index.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       69 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/styles/menu_style.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       69 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/styles/page_style.rst
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-05-02 03:00:28.000000 pyrubrum-continued-0.2.20/docs/source/api/tree/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       95 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/tree/index.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       53 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/tree/node.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       69 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/tree/recursive_add.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       57 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/tree/transform.rst
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-05-02 03:00:28.000000 pyrubrum-continued-0.2.20/docs/source/api/types/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       67 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/types/index.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       56 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/api/types/types.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     5306 2023-03-19 17:42:06.000000 pyrubrum-continued-0.2.20/docs/source/conf.py
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-05-02 03:00:28.000000 pyrubrum-continued-0.2.20/docs/source/examples/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      147 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/examples/sample.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1388 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/flowchart.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1458 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/glossary.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     2453 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/index.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      689 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/license.rst
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-05-02 03:00:28.000000 pyrubrum-continued-0.2.20/docs/source/quickstart/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      761 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/quickstart/installation.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     7519 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs/source/quickstart/overview.rst
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       67 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/docs-requirements.txt
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3825 2023-03-19 17:42:06.000000 pyrubrum-continued-0.2.20/docs_updater.py
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-05-02 03:00:28.000000 pyrubrum-continued-0.2.20/examples/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3313 2023-05-02 02:59:32.000000 pyrubrum-continued-0.2.20/examples/cafe_bot.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3578 2023-03-19 17:42:06.000000 pyrubrum-continued-0.2.20/examples/calendar_bot.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     2394 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.20/examples/hitchhiker_bot.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       24 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/examples/requirements.txt
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1471 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/examples/sample.env
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1678 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.20/examples/sample_bot.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       16 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/fast-requirements.txt
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       30 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/pyproject.toml
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-05-02 03:00:28.000000 pyrubrum-continued-0.2.20/pyrubrum/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     2404 2023-05-02 02:59:56.000000 pyrubrum-continued-0.2.20/pyrubrum/__init__.py
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-05-02 03:00:28.000000 pyrubrum-continued-0.2.20/pyrubrum/database/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      924 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/pyrubrum/database/__init__.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3615 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/pyrubrum/database/base_database.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3369 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/pyrubrum/database/dict_database.py
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-05-02 03:00:28.000000 pyrubrum-continued-0.2.20/pyrubrum/database/errors/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1042 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/pyrubrum/database/errors/__init__.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1072 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.20/pyrubrum/database/errors/delete_error.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      915 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/pyrubrum/database/errors/error.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1102 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.20/pyrubrum/database/errors/expire_error.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1069 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.20/pyrubrum/database/errors/get_error.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1049 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/pyrubrum/database/errors/not_found_error.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1097 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.20/pyrubrum/database/errors/set_error.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     4714 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.20/pyrubrum/database/redis_database.py
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-05-02 03:00:28.000000 pyrubrum-continued-0.2.20/pyrubrum/handlers/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1120 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/pyrubrum/handlers/__init__.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     5594 2023-04-18 19:43:10.000000 pyrubrum-continued-0.2.20/pyrubrum/handlers/base_handler.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     6280 2023-04-18 19:58:27.000000 pyrubrum-continued-0.2.20/pyrubrum/handlers/handler.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     9330 2023-04-18 19:58:44.000000 pyrubrum-continued-0.2.20/pyrubrum/handlers/parameterized_base_handler.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     4203 2023-04-18 19:58:52.000000 pyrubrum-continued-0.2.20/pyrubrum/handlers/parameterized_handler.py
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-05-02 03:00:28.000000 pyrubrum-continued-0.2.20/pyrubrum/keyboard/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      889 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/pyrubrum/keyboard/__init__.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3743 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/pyrubrum/keyboard/button.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1319 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/pyrubrum/keyboard/element.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     2042 2023-03-19 17:42:05.000000 pyrubrum-continued-0.2.20/pyrubrum/keyboard/keyboard.py
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-05-02 03:00:28.000000 pyrubrum-continued-0.2.20/pyrubrum/menus/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1071 2023-03-20 08:21:09.000000 pyrubrum-continued-0.2.20/pyrubrum/menus/__init__.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     4054 2023-05-02 02:59:32.000000 pyrubrum-continued-0.2.20/pyrubrum/menus/base_menu.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3299 2023-05-02 02:59:32.000000 pyrubrum-continued-0.2.20/pyrubrum/menus/content_page_menu.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     4378 2023-05-02 02:59:10.000000 pyrubrum-continued-0.2.20/pyrubrum/menus/deep_link_menu.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3131 2023-05-02 02:59:32.000000 pyrubrum-continued-0.2.20/pyrubrum/menus/link_menu.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     8763 2023-05-02 02:43:51.000000 pyrubrum-continued-0.2.20/pyrubrum/menus/menu.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     4892 2023-03-20 11:18:25.000000 pyrubrum-continued-0.2.20/pyrubrum/menus/page_menu.py
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-05-02 03:00:28.000000 pyrubrum-continued-0.2.20/pyrubrum/menus/styles/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      904 2023-03-20 07:53:10.000000 pyrubrum-continued-0.2.20/pyrubrum/menus/styles/__init__.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     2033 2023-03-20 08:34:39.000000 pyrubrum-continued-0.2.20/pyrubrum/menus/styles/base_style.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3752 2023-05-02 02:59:32.000000 pyrubrum-continued-0.2.20/pyrubrum/menus/styles/menu_style.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)    11621 2023-05-02 02:59:32.000000 pyrubrum-continued-0.2.20/pyrubrum/menus/styles/page_style.py
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-05-02 03:00:28.000000 pyrubrum-continued-0.2.20/pyrubrum/objects/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      829 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/pyrubrum/objects/__init__.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     4469 2023-03-19 17:42:06.000000 pyrubrum-continued-0.2.20/pyrubrum/objects/user.py
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-05-02 03:00:28.000000 pyrubrum-continued-0.2.20/pyrubrum/tree/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      885 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/pyrubrum/tree/__init__.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     6184 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/pyrubrum/tree/node.py
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-05-02 03:00:28.000000 pyrubrum-continued-0.2.20/pyrubrum/types/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     4370 2023-03-19 17:42:06.000000 pyrubrum-continued-0.2.20/pyrubrum/types/__init__.py
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-05-02 03:00:28.000000 pyrubrum-continued-0.2.20/pyrubrum_continued.egg-info/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     6226 2023-05-02 03:00:27.000000 pyrubrum-continued-0.2.20/pyrubrum_continued.egg-info/PKG-INFO
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     4626 2023-05-02 03:00:27.000000 pyrubrum-continued-0.2.20/pyrubrum_continued.egg-info/SOURCES.txt
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)        1 2023-05-02 03:00:27.000000 pyrubrum-continued-0.2.20/pyrubrum_continued.egg-info/dependency_links.txt
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       38 2023-05-02 03:00:27.000000 pyrubrum-continued-0.2.20/pyrubrum_continued.egg-info/requires.txt
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)        9 2023-05-02 03:00:27.000000 pyrubrum-continued-0.2.20/pyrubrum_continued.egg-info/top_level.txt
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       14 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/requirements.txt
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)       38 2023-05-02 03:00:28.000000 pyrubrum-continued-0.2.20/setup.cfg
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3131 2023-03-19 14:42:30.000000 pyrubrum-continued-0.2.20/setup.py
+drwxr-xr-x   0 zhesheng (40041) zhuchengliang (40006)        0 2023-05-02 03:00:28.000000 pyrubrum-continued-0.2.20/tests/
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     2100 2023-05-02 02:59:32.000000 pyrubrum-continued-0.2.20/tests/test_deep_link_menu.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1280 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/tests/test_dict_database.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     1487 2023-05-02 02:59:32.000000 pyrubrum-continued-0.2.20/tests/test_link_menu.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     3043 2023-05-02 02:48:07.000000 pyrubrum-continued-0.2.20/tests/test_menu.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)     2747 2023-03-19 17:42:06.000000 pyrubrum-continued-0.2.20/tests/test_node.py
+-rw-r--r--   0 zhesheng (40041) zhuchengliang (40006)      957 2023-03-19 14:36:38.000000 pyrubrum-continued-0.2.20/tests/test_version.py
```

### Comparing `pyrubrum-continued-0.2.19/.github/ISSUE_TEMPLATE/bug_report.md` & `pyrubrum-continued-0.2.20/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/.github/ISSUE_TEMPLATE/feature_request.md` & `pyrubrum-continued-0.2.20/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/.gitignore` & `pyrubrum-continued-0.2.20/.gitignore`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/.pre-commit-config.yaml` & `pyrubrum-continued-0.2.20/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/CHANGELOG.md` & `pyrubrum-continued-0.2.20/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/CODE_OF_CONDUCT.md` & `pyrubrum-continued-0.2.20/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/CONTRIBUTING.md` & `pyrubrum-continued-0.2.20/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/FEATURES.md` & `pyrubrum-continued-0.2.20/FEATURES.md`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/LICENSE` & `pyrubrum-continued-0.2.20/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/NOTICE` & `pyrubrum-continued-0.2.20/NOTICE`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/PKG-INFO` & `pyrubrum-continued-0.2.20/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrubrum-continued
-Version: 0.2.19
+Version: 0.2.20
 Summary: An intuitive framework for creating Telegram bots
 Home-page: https://github.com/hearot/pyrubrum
 Author: Hearot
 Author-email: gabriel@hearot.it
 License: GPLv3
 Project-URL: Tracker, https://github.com/hearot/pyrubrum/issues
 Project-URL: Source, https://github.com/hearot/pyrubrum
@@ -95,33 +95,33 @@
    - LRU caching with [functools.lru_cache](https://docs.python.org/3/library/functools.html#functools.lru_cache)
    - Native support for the *"Go back"* button
    - No limit for `callback_data` (see [Telegram Bot API](https://core.telegram.org/bots/api#inlinekeyboardbutton))
    - Paging integration with `PageMenu`
 
 ### Examples
 
-In order to make use of the proposed examples, you need to create your own environment file by renaming [sample.env](https://github.com/hearot/pyrubrum/blob/v0.2.19/examples/sample.env) into `.env` and editing all the necessary variables.
+In order to make use of the proposed examples, you need to create your own environment file by renaming [sample.env](https://github.com/hearot/pyrubrum/blob/v0.2.20/examples/sample.env) into `.env` and editing all the necessary variables.
 
-   - [Café](https://github.com/hearot/pyrubrum/blob/v0.2.19/examples/cafe_bot.py) - Get an overview of the design which lies inside Pyrubrum while interacting with multiple commands and pages.
-   - [Calendar](https://github.com/hearot/pyrubrum/blob/v0.2.19/examples/calendar_bot.py) - Get what day of the week a day is by simply choosing a year, a month and a day while discovering the potential of Pyrubrum page menus.
-   - [Hitchhiker](https://github.com/hearot/pyrubrum/blob/v0.2.19/examples/hitchhiker_bot.py) - Come to know how media are handled with Pyrubrum and...[get an existential question answered](https://en.wikipedia.org/wiki/Phrases_from_The_Hitchhiker%27s_Guide_to_the_Galaxy#The_Answer_to_the_Ultimate_Question_of_Life,_the_Universe,_and_Everything_is_42).
-   - [Sample](https://github.com/hearot/pyrubrum/blob/v0.2.19/examples/sample_bot.py) - Interact with inline menus while understanding how Pyrubrum works.
+   - [Café](https://github.com/hearot/pyrubrum/blob/v0.2.20/examples/cafe_bot.py) - Get an overview of the design which lies inside Pyrubrum while interacting with multiple commands and pages.
+   - [Calendar](https://github.com/hearot/pyrubrum/blob/v0.2.20/examples/calendar_bot.py) - Get what day of the week a day is by simply choosing a year, a month and a day while discovering the potential of Pyrubrum page menus.
+   - [Hitchhiker](https://github.com/hearot/pyrubrum/blob/v0.2.20/examples/hitchhiker_bot.py) - Come to know how media are handled with Pyrubrum and...[get an existential question answered](https://en.wikipedia.org/wiki/Phrases_from_The_Hitchhiker%27s_Guide_to_the_Galaxy#The_Answer_to_the_Ultimate_Question_of_Life,_the_Universe,_and_Everything_is_42).
+   - [Sample](https://github.com/hearot/pyrubrum/blob/v0.2.20/examples/sample_bot.py) - Interact with inline menus while understanding how Pyrubrum works.
 
 ### Changelog
 
-> See [CHANGELOG.md](https://github.com/hearot/pyrubrum/blob/v0.2.19/CHANGELOG.md).
-> Find new features in [FEATURES.md](https://github.com/hearot/pyrubrum/blob/v0.2.19/FEATURES.md).
+> See [CHANGELOG.md](https://github.com/hearot/pyrubrum/blob/v0.2.20/CHANGELOG.md).
+> Find new features in [FEATURES.md](https://github.com/hearot/pyrubrum/blob/v0.2.20/FEATURES.md).
 
 ### Commit messages
 
 > See [Conventional Commits](https://www.conventionalcommits.org).
 
 ### Contributing
 
-> See [CONTRIBUTING.md](https://github.com/hearot/pyrubrum/blob/v0.2.19/CONTRIBUTING.md).
+> See [CONTRIBUTING.md](https://github.com/hearot/pyrubrum/blob/v0.2.20/CONTRIBUTING.md).
 
 ### Versioning
 
 > See [PEP 440](https://www.python.org/dev/peps/pep-0440/).
 
 ### Thanks
 
@@ -131,8 +131,8 @@
 ### Branding
 
 > See [hearot/pyrubrum-assets](https://github.com/hearot/pyrubrum-assets).
 
 ### Copyright & License
 
 - Copyright (C) 2020 [Hearot](https://github.com/hearot).
-- Licensed under the terms of the [GNU General Public License v3 (GPLv3)](https://github.com/hearot/pyrubrum/blob/v0.2.19/LICENSE).
+- Licensed under the terms of the [GNU General Public License v3 (GPLv3)](https://github.com/hearot/pyrubrum/blob/v0.2.20/LICENSE).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyrubrum-continued Version: 0.2.19 Summary: An
+Metadata-Version: 2.1 Name: pyrubrum-continued Version: 0.2.20 Summary: An
 intuitive framework for creating Telegram bots Home-page: https://github.com/
 hearot/pyrubrum Author: Hearot Author-email: gabriel@hearot.it License: GPLv3
 Project-URL: Tracker, https://github.com/hearot/pyrubrum/issues Project-URL:
 Source, https://github.com/hearot/pyrubrum Keywords: bot bots chat messenger
 mtproto pyrogram python telegram Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v3 (GPLv3) Classifier: Natural Language ::
@@ -42,35 +42,35 @@
 encrypted parameters - Intuitive creation of inline keyboards - LRU caching
 with [functools.lru_cache](https://docs.python.org/3/library/
 functools.html#functools.lru_cache) - Native support for the *"Go back"* button
 - No limit for `callback_data` (see [Telegram Bot API](https://
 core.telegram.org/bots/api#inlinekeyboardbutton)) - Paging integration with
 `PageMenu` ### Examples In order to make use of the proposed examples, you need
 to create your own environment file by renaming [sample.env](https://
-github.com/hearot/pyrubrum/blob/v0.2.19/examples/sample.env) into `.env` and
+github.com/hearot/pyrubrum/blob/v0.2.20/examples/sample.env) into `.env` and
 editing all the necessary variables. - [CafÃ©](https://github.com/hearot/
-pyrubrum/blob/v0.2.19/examples/cafe_bot.py) - Get an overview of the design
+pyrubrum/blob/v0.2.20/examples/cafe_bot.py) - Get an overview of the design
 which lies inside Pyrubrum while interacting with multiple commands and pages.
-- [Calendar](https://github.com/hearot/pyrubrum/blob/v0.2.19/examples/
+- [Calendar](https://github.com/hearot/pyrubrum/blob/v0.2.20/examples/
 calendar_bot.py) - Get what day of the week a day is by simply choosing a year,
 a month and a day while discovering the potential of Pyrubrum page menus. -
-[Hitchhiker](https://github.com/hearot/pyrubrum/blob/v0.2.19/examples/
+[Hitchhiker](https://github.com/hearot/pyrubrum/blob/v0.2.20/examples/
 hitchhiker_bot.py) - Come to know how media are handled with Pyrubrum and...
 [get an existential question answered](https://en.wikipedia.org/wiki/
 Phrases_from_The_Hitchhiker%27s_Guide_to_the_Galaxy#The_Answer_to_the_Ultimate_Question_of_Life,_the_Universe,_and_Everything_is_42).
-- [Sample](https://github.com/hearot/pyrubrum/blob/v0.2.19/examples/
+- [Sample](https://github.com/hearot/pyrubrum/blob/v0.2.20/examples/
 sample_bot.py) - Interact with inline menus while understanding how Pyrubrum
 works. ### Changelog > See [CHANGELOG.md](https://github.com/hearot/pyrubrum/
-blob/v0.2.19/CHANGELOG.md). > Find new features in [FEATURES.md](https://
-github.com/hearot/pyrubrum/blob/v0.2.19/FEATURES.md). ### Commit messages > See
+blob/v0.2.20/CHANGELOG.md). > Find new features in [FEATURES.md](https://
+github.com/hearot/pyrubrum/blob/v0.2.20/FEATURES.md). ### Commit messages > See
 [Conventional Commits](https://www.conventionalcommits.org). ### Contributing >
-See [CONTRIBUTING.md](https://github.com/hearot/pyrubrum/blob/v0.2.19/
+See [CONTRIBUTING.md](https://github.com/hearot/pyrubrum/blob/v0.2.20/
 CONTRIBUTING.md). ### Versioning > See [PEP 440](https://www.python.org/dev/
 peps/pep-0440/). ### Thanks - [veggero/tytg](https://github.com/veggero/tytg)
 for giving me the idea of developing a simple framework with which you can code
 a folder-like bot. - [bakhoraliev](https://github.com/bakhoraliev) for letting
 me understand that an object-oriented library would make the difference in
 developing this project. ### Branding > See [hearot/pyrubrum-assets](https://
 github.com/hearot/pyrubrum-assets). ### Copyright & License - Copyright (C)
 2020 [Hearot](https://github.com/hearot). - Licensed under the terms of the
 [GNU General Public License v3 (GPLv3)](https://github.com/hearot/pyrubrum/
-blob/v0.2.19/LICENSE).
+blob/v0.2.20/LICENSE).
```

### Comparing `pyrubrum-continued-0.2.19/README.md` & `pyrubrum-continued-0.2.20/README.md`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/SECURITY.md` & `pyrubrum-continued-0.2.20/SECURITY.md`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/changelog_generator.py` & `pyrubrum-continued-0.2.20/changelog_generator.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/docs/Makefile` & `pyrubrum-continued-0.2.20/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/docs/make.bat` & `pyrubrum-continued-0.2.20/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/docs/source/CONTRIBUTING.md` & `pyrubrum-continued-0.2.20/docs/source/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/docs/source/_static/CONTRIBUTING.md` & `pyrubrum-continued-0.2.20/docs/source/_static/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/docs/source/_static/flowcharts/attributes.png` & `pyrubrum-continued-0.2.20/docs/source/_static/flowcharts/attributes.png`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/docs/source/_static/flowcharts/cafe_bot.png` & `pyrubrum-continued-0.2.20/docs/source/_static/flowcharts/cafe_bot.png`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/docs/source/_static/flowcharts/calendar_bot.png` & `pyrubrum-continued-0.2.20/docs/source/_static/flowcharts/calendar_bot.png`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/docs/source/_static/flowcharts/hitchhiker_bot.png` & `pyrubrum-continued-0.2.20/docs/source/_static/flowcharts/hitchhiker_bot.png`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/docs/source/_static/flowcharts/link.png` & `pyrubrum-continued-0.2.20/docs/source/_static/flowcharts/link.png`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/docs/source/_static/flowcharts/menu.png` & `pyrubrum-continued-0.2.20/docs/source/_static/flowcharts/menu.png`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/docs/source/_static/flowcharts/overview-1.png` & `pyrubrum-continued-0.2.20/docs/source/_static/flowcharts/overview-1.png`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/docs/source/_static/flowcharts/overview.png` & `pyrubrum-continued-0.2.20/docs/source/_static/flowcharts/overview.png`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/docs/source/_static/flowcharts/page_menu.png` & `pyrubrum-continued-0.2.20/docs/source/_static/flowcharts/page_menu.png`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/docs/source/_static/flowcharts/sample_bot.png` & `pyrubrum-continued-0.2.20/docs/source/_static/flowcharts/sample_bot.png`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/docs/source/conf.py` & `pyrubrum-continued-0.2.20/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/docs/source/flowchart.rst` & `pyrubrum-continued-0.2.20/docs/source/flowchart.rst`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/docs/source/glossary.rst` & `pyrubrum-continued-0.2.20/docs/source/glossary.rst`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/docs/source/index.rst` & `pyrubrum-continued-0.2.20/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/docs/source/license.rst` & `pyrubrum-continued-0.2.20/docs/source/license.rst`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/docs/source/quickstart/installation.rst` & `pyrubrum-continued-0.2.20/docs/source/quickstart/installation.rst`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/docs/source/quickstart/overview.rst` & `pyrubrum-continued-0.2.20/docs/source/quickstart/overview.rst`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/docs_updater.py` & `pyrubrum-continued-0.2.20/docs_updater.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/examples/cafe_bot.py` & `pyrubrum-continued-0.2.20/examples/cafe_bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,20 @@
 
 def make_elements(elements: List[str]) -> List[Element]:
     return [Element(name, index) for index, name in enumerate(elements)]
 
 
 tree = transform(
     {
-        Menu("Start", "start", "ℹ️ Have a drink or a snack by saying /drink or /snack", default=True,): [
+        Menu(
+            "Start",
+            "start",
+            "ℹ️ Have a drink or a snack by saying /drink or /snack",
+            default=True,
+        ): [
             DeepLinkMenu("🍷 Drink", "link_drink", "drink"),
             DeepLinkMenu("🍬 Snack", "link_snack", "snack"),
         ],
         PageMenu(
             "Drink",
             "drink",
             "🍷 Choose the drink you want!",
```

### Comparing `pyrubrum-continued-0.2.19/examples/calendar_bot.py` & `pyrubrum-continued-0.2.20/examples/calendar_bot.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/examples/hitchhiker_bot.py` & `pyrubrum-continued-0.2.20/examples/hitchhiker_bot.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/examples/sample.env` & `pyrubrum-continued-0.2.20/examples/sample.env`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/examples/sample_bot.py` & `pyrubrum-continued-0.2.20/examples/sample_bot.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/__init__.py` & `pyrubrum-continued-0.2.20/pyrubrum/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 __author__ = "Hearot"
 __author_email__ = "gabriel@hearot.it"
 __copyright__ = "Copyright (C) 2020 Hearot <https://github.com/hearot>"
 __license__ = "GNU General Public License v3"
 __package__ = "pyrubrum"
 __url__ = "https://github.com/hearot/pyrubrum"
-__version__ = "0.2.19"
+__version__ = "0.2.20"
 
 from .database import BaseDatabase  # noqa
 from .database import DictDatabase  # noqa
 from .database import RedisDatabase  # noqa
 from .database.errors import DatabaseError  # noqa
 from .database.errors import DeleteError  # noqa
 from .database.errors import ExpireError  # noqa
```

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/database/__init__.py` & `pyrubrum-continued-0.2.20/pyrubrum/database/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/database/base_database.py` & `pyrubrum-continued-0.2.20/pyrubrum/database/base_database.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/database/dict_database.py` & `pyrubrum-continued-0.2.20/pyrubrum/database/dict_database.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/database/errors/__init__.py` & `pyrubrum-continued-0.2.20/pyrubrum/database/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/database/errors/delete_error.py` & `pyrubrum-continued-0.2.20/pyrubrum/database/errors/delete_error.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/database/errors/error.py` & `pyrubrum-continued-0.2.20/pyrubrum/database/errors/error.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/database/errors/expire_error.py` & `pyrubrum-continued-0.2.20/pyrubrum/database/errors/expire_error.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/database/errors/get_error.py` & `pyrubrum-continued-0.2.20/pyrubrum/database/errors/get_error.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/database/errors/not_found_error.py` & `pyrubrum-continued-0.2.20/pyrubrum/database/errors/not_found_error.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/database/errors/set_error.py` & `pyrubrum-continued-0.2.20/pyrubrum/database/errors/set_error.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/database/redis_database.py` & `pyrubrum-continued-0.2.20/pyrubrum/database/redis_database.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/handlers/__init__.py` & `pyrubrum-continued-0.2.20/pyrubrum/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/handlers/base_handler.py` & `pyrubrum-continued-0.2.20/pyrubrum/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/handlers/handler.py` & `pyrubrum-continued-0.2.20/pyrubrum/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/handlers/parameterized_base_handler.py` & `pyrubrum-continued-0.2.20/pyrubrum/handlers/parameterized_base_handler.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/handlers/parameterized_handler.py` & `pyrubrum-continued-0.2.20/pyrubrum/handlers/parameterized_handler.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/keyboard/__init__.py` & `pyrubrum-continued-0.2.20/pyrubrum/keyboard/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/keyboard/button.py` & `pyrubrum-continued-0.2.20/pyrubrum/keyboard/button.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/keyboard/element.py` & `pyrubrum-continued-0.2.20/pyrubrum/keyboard/element.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/keyboard/keyboard.py` & `pyrubrum-continued-0.2.20/pyrubrum/keyboard/keyboard.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/menus/__init__.py` & `pyrubrum-continued-0.2.20/pyrubrum/menus/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/menus/base_menu.py` & `pyrubrum-continued-0.2.20/pyrubrum/menus/base_menu.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Pyrubrum. If not, see <https://www.gnu.org/licenses/>.
 
 from abc import ABC
+from asyncio import iscoroutinefunction
 from typing import Any, Dict, Optional
 
 from pyrogram import Client
 
 from pyrubrum.handlers import BaseHandler
 from pyrubrum.keyboard import Button
 
@@ -70,15 +71,24 @@
         return hash(self.menu_id)
 
     def __init__(self, name: str, menu_id: str, is_link: Optional[bool] = False):
         self.is_link = is_link
         self.name = name
         self.menu_id = menu_id
 
-    def button(
+    @staticmethod
+    async def parse(var, handler, client, context, parameters):
+        if iscoroutinefunction(var):
+            return await var(handler, client, context, parameters)
+        elif callable(var):
+            return var(handler, client, context, parameters)
+        else:
+            return var
+
+    async def button(
         self,
         handler: BaseHandler,
         client: Client,
         context: Any,
         parameters: Optional[Dict[str, Any]] = None,
     ) -> Button:
         """Create an inline button which refers to this menu, using `name` as
```

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/menus/content_page_menu.py` & `pyrubrum-continued-0.2.20/pyrubrum/menus/content_page_menu.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         client: Client,
         context: Union[CallbackQuery, Message],
         parameters: Optional[Dict[str, Any]] = None,
     ):
         element_id = parameters.get("element_id", "")
         if element_id == "":
             page = int(parameters.get(f"page_{self.menu_id}", 0))
-        elif parameters.get('same_menu', False):
+        elif parameters.get("same_menu", False):
             page = int(element_id)
         else:
             page = 0
 
         content = await self.parse(self.content, handler, client, context, parameters)
         if content is None:
             return
@@ -78,15 +78,15 @@
                 )
             )
 
         if self.entries:
             for i, (c, t, x) in enumerate(self.entries[page]):
                 self.entries[page][i] = (await self.parse(c, handler, client, context, parameters), t, x)
 
-        text = "\n".join([c for c, t, x in self.entries[page]]) if self.entries else ''
+        text = "\n".join([c for c, t, x in self.entries[page]]) if self.entries else ""
         if self.header:
             text = await self.parse(self.header, handler, client, context, parameters) + "\n" + text
         if self.footer:
             text = text + "\n" + await self.parse(self.footer, handler, client, context, parameters)
         await self.call_preliminary(handler, client, context, parameters)
 
         self.items = [Element(t, x) for page in self.entries for c, t, x in page]
```

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/menus/deep_link_menu.py` & `pyrubrum-continued-0.2.20/pyrubrum/menus/deep_link_menu.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             raise ValueError("deep_link_type must be either " "'start' or 'startgroup'")
 
         BaseMenu.__init__(self, name, menu_id, is_link=True)
 
         self.payload = payload
         self.deep_link_type = deep_link_type
 
-    def button(
+    async def button(
         self,
         handler: "BaseHandler",  # noqa
         client: "Client",  # noqa
         context: Any,
         parameters: Optional[Dict[str, Any]] = None,
     ) -> Button:
         """Create an inline button which makes use of deep-linking, following
@@ -100,27 +100,16 @@
 
         if client_hash in USERNAMES:
             username = USERNAMES[client_hash]
         else:
             username = client.get_me().username
             USERNAMES[client_hash] = username
 
-        if callable(self.payload):
-            return Button(
-                self.name,
-                self.menu_id,
-                link=DEEP_LINK_TEMPLATE.format(
-                    deep_link_type=self.deep_link_type,
-                    payload=self.payload(handler, client, context, parameters),
-                    username=username,
-                ),
-            )
-
         return Button(
             self.name,
             self.menu_id,
             link=DEEP_LINK_TEMPLATE.format(
                 deep_link_type=self.deep_link_type,
-                payload=self.payload,
+                payload=await self.parse(self.payload, handler, client, context, parameters),
                 username=username,
             ),
         )
```

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/menus/link_menu.py` & `pyrubrum-continued-0.2.20/pyrubrum/menus/link_menu.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     """
 
     def __init__(self, name: str, menu_id: str, link: Types.Link):
         BaseMenu.__init__(self, name, menu_id, is_link=True)
 
         self.link = link
 
-    def button(
+    async def button(
         self,
         handler: "BaseHandler",  # noqa
         client: "Client",  # noqa
         context: Any,
         parameters: Optional[Dict[str, Any]] = None,
     ) -> Button:
         """Create an inline button which redirects to a website retrieved from
@@ -70,15 +70,11 @@
                 button is generated for.
             parameters (Optional[Dict[str, Any]]): The parameters which were
                 passed to the handler. Defaults to ``None``.
 
         Returns:
             Button: The generated button.
         """
-        if callable(self.link):
-            return Button(
-                self.name,
-                self.menu_id,
-                link=self.link(handler, client, context, parameters),
-            )
 
-        return Button(self.name, self.menu_id, link=self.link)
+        return Button(
+            self.name, self.menu_id, link=await self.parse(self.link, handler, client, context, parameters)
+        )
```

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/menus/menu.py` & `pyrubrum-continued-0.2.20/pyrubrum/menus/menu.py`

 * *Files 5% similar despite different names*

```diff
@@ -114,23 +114,14 @@
         self.deep_link = deep_link
         self.default = default
         self.message_filter = message_filter
         self.preliminary = preliminary
         self.style = style
         self.kwargs = kwargs
 
-    @staticmethod
-    async def parse(var, handler, client, context, parameters):
-        if iscoroutinefunction(var):
-            return await var(handler, client, context, parameters)
-        elif callable(var):
-            return var(handler, client, context, parameters)
-        else:
-            return var
-
     async def call_preliminary(
         self,
         handler: "Handler",  # noqa
         client: Client,
         context: Union[CallbackQuery, Message],
         parameters: Optional[Dict[str, Any]] = None,
     ):
```

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/menus/page_menu.py` & `pyrubrum-continued-0.2.20/pyrubrum/menus/page_menu.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/menus/styles/__init__.py` & `pyrubrum-continued-0.2.20/pyrubrum/menus/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/menus/styles/base_style.py` & `pyrubrum-continued-0.2.20/pyrubrum/menus/styles/base_style.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/menus/styles/menu_style.py` & `pyrubrum-continued-0.2.20/pyrubrum/menus/styles/menu_style.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,40 +71,37 @@
                 the handler.
             menu (Menu): The menu the keyboard is being built for.
 
         Returns:
             pyrogram.InlineKeyboardMarkup: The generated inline keyboard,
             which is then displayed to the user.
         """
+
+        async def get_button(menu):
+            return await menu.button(handler, client, context, parameters)
+
         parent, children = handler.get_family(menu.menu_id)
 
         keyboard = []
 
         if children:
             iterable = iter(children)
-            keyboard = list(
-                iter(
-                    lambda: list(
-                        map(
-                            lambda child: child.button(handler, client, context, parameters),
-                            islice(iterable, self.limit),
-                        )
-                    ),
-                    [],
-                )
-            )
+            keyboard = [
+                await child.button(handler, client, context, parameters)
+                for child in islice(iterable, self.limit)
+            ]
 
         extras = [handler[e] if isinstance(e, str) else e for e in self.extras]
-        buttons = [m.button(handler, client, context, parameters) for m in extras]
+        buttons = [await m.button(handler, client, context, parameters) for m in extras]
         if buttons:
             keyboard += [buttons]
 
         if self.back_to:
             parent = handler[self.back_to]
-        
+
         if parent and self.back_enable:
-            parent_button = parent.button(handler, client, context, parameters)
+            parent_button = await parent.button(handler, client, context, parameters)
             parent_button.name = self.back_text
             if parent_button:
                 keyboard += [[parent_button]]
 
         return keyboard
```

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/menus/styles/page_style.py` & `pyrubrum-continued-0.2.20/pyrubrum/menus/styles/page_style.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,25 +206,18 @@
                     )
                     for element in elements[i : i + self.limit]
                 ]
                 for i in range(0, len(elements), self.limit)
             ]
 
         if children:
-            keyboard += list(
-                iter(
-                    lambda: list(
-                        map(
-                            lambda child: child.button(handler, client, context, parameters),
-                            islice(iterable, self.limit),
-                        )
-                    ),
-                    [],
-                )
-            )
+            keyboard += [
+                await child.button(handler, client, context, parameters)
+                for child in islice(iterable, self.limit)
+            ]
 
         pages = ceil(len(items) / self.limit_items)
 
         if pages > 1:
             teleport_row = []
 
             if parameters[page_id] > 0:
@@ -285,21 +278,21 @@
 
                 teleport_row.append(next_page_button)
 
             if teleport_row:
                 keyboard += [teleport_row]
 
         extras = [handler[e] if isinstance(e, str) else e for e in self.extras]
-        buttons = [m.button(handler, client, context, parameters) for m in extras]
+        buttons = [await m.button(handler, client, context, parameters) for m in extras]
         if buttons:
             keyboard += [buttons]
 
         if self.back_to:
             parent = handler[self.back_to]
 
         if parent and self.back_enable:
-            parent_button = parent.button(handler, client, context, parameters)
+            parent_button = await parent.button(handler, client, context, parameters)
             parent_button.name = self.back_text
             if parent_button:
                 keyboard += [[parent_button]]
 
         return keyboard
```

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/objects/__init__.py` & `pyrubrum-continued-0.2.20/pyrubrum/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/objects/user.py` & `pyrubrum-continued-0.2.20/pyrubrum/objects/user.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/tree/__init__.py` & `pyrubrum-continued-0.2.20/pyrubrum/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/tree/node.py` & `pyrubrum-continued-0.2.20/pyrubrum/tree/node.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/pyrubrum/types/__init__.py` & `pyrubrum-continued-0.2.20/pyrubrum/types/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/pyrubrum_continued.egg-info/PKG-INFO` & `pyrubrum-continued-0.2.20/pyrubrum_continued.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrubrum-continued
-Version: 0.2.19
+Version: 0.2.20
 Summary: An intuitive framework for creating Telegram bots
 Home-page: https://github.com/hearot/pyrubrum
 Author: Hearot
 Author-email: gabriel@hearot.it
 License: GPLv3
 Project-URL: Tracker, https://github.com/hearot/pyrubrum/issues
 Project-URL: Source, https://github.com/hearot/pyrubrum
@@ -95,33 +95,33 @@
    - LRU caching with [functools.lru_cache](https://docs.python.org/3/library/functools.html#functools.lru_cache)
    - Native support for the *"Go back"* button
    - No limit for `callback_data` (see [Telegram Bot API](https://core.telegram.org/bots/api#inlinekeyboardbutton))
    - Paging integration with `PageMenu`
 
 ### Examples
 
-In order to make use of the proposed examples, you need to create your own environment file by renaming [sample.env](https://github.com/hearot/pyrubrum/blob/v0.2.19/examples/sample.env) into `.env` and editing all the necessary variables.
+In order to make use of the proposed examples, you need to create your own environment file by renaming [sample.env](https://github.com/hearot/pyrubrum/blob/v0.2.20/examples/sample.env) into `.env` and editing all the necessary variables.
 
-   - [Café](https://github.com/hearot/pyrubrum/blob/v0.2.19/examples/cafe_bot.py) - Get an overview of the design which lies inside Pyrubrum while interacting with multiple commands and pages.
-   - [Calendar](https://github.com/hearot/pyrubrum/blob/v0.2.19/examples/calendar_bot.py) - Get what day of the week a day is by simply choosing a year, a month and a day while discovering the potential of Pyrubrum page menus.
-   - [Hitchhiker](https://github.com/hearot/pyrubrum/blob/v0.2.19/examples/hitchhiker_bot.py) - Come to know how media are handled with Pyrubrum and...[get an existential question answered](https://en.wikipedia.org/wiki/Phrases_from_The_Hitchhiker%27s_Guide_to_the_Galaxy#The_Answer_to_the_Ultimate_Question_of_Life,_the_Universe,_and_Everything_is_42).
-   - [Sample](https://github.com/hearot/pyrubrum/blob/v0.2.19/examples/sample_bot.py) - Interact with inline menus while understanding how Pyrubrum works.
+   - [Café](https://github.com/hearot/pyrubrum/blob/v0.2.20/examples/cafe_bot.py) - Get an overview of the design which lies inside Pyrubrum while interacting with multiple commands and pages.
+   - [Calendar](https://github.com/hearot/pyrubrum/blob/v0.2.20/examples/calendar_bot.py) - Get what day of the week a day is by simply choosing a year, a month and a day while discovering the potential of Pyrubrum page menus.
+   - [Hitchhiker](https://github.com/hearot/pyrubrum/blob/v0.2.20/examples/hitchhiker_bot.py) - Come to know how media are handled with Pyrubrum and...[get an existential question answered](https://en.wikipedia.org/wiki/Phrases_from_The_Hitchhiker%27s_Guide_to_the_Galaxy#The_Answer_to_the_Ultimate_Question_of_Life,_the_Universe,_and_Everything_is_42).
+   - [Sample](https://github.com/hearot/pyrubrum/blob/v0.2.20/examples/sample_bot.py) - Interact with inline menus while understanding how Pyrubrum works.
 
 ### Changelog
 
-> See [CHANGELOG.md](https://github.com/hearot/pyrubrum/blob/v0.2.19/CHANGELOG.md).
-> Find new features in [FEATURES.md](https://github.com/hearot/pyrubrum/blob/v0.2.19/FEATURES.md).
+> See [CHANGELOG.md](https://github.com/hearot/pyrubrum/blob/v0.2.20/CHANGELOG.md).
+> Find new features in [FEATURES.md](https://github.com/hearot/pyrubrum/blob/v0.2.20/FEATURES.md).
 
 ### Commit messages
 
 > See [Conventional Commits](https://www.conventionalcommits.org).
 
 ### Contributing
 
-> See [CONTRIBUTING.md](https://github.com/hearot/pyrubrum/blob/v0.2.19/CONTRIBUTING.md).
+> See [CONTRIBUTING.md](https://github.com/hearot/pyrubrum/blob/v0.2.20/CONTRIBUTING.md).
 
 ### Versioning
 
 > See [PEP 440](https://www.python.org/dev/peps/pep-0440/).
 
 ### Thanks
 
@@ -131,8 +131,8 @@
 ### Branding
 
 > See [hearot/pyrubrum-assets](https://github.com/hearot/pyrubrum-assets).
 
 ### Copyright & License
 
 - Copyright (C) 2020 [Hearot](https://github.com/hearot).
-- Licensed under the terms of the [GNU General Public License v3 (GPLv3)](https://github.com/hearot/pyrubrum/blob/v0.2.19/LICENSE).
+- Licensed under the terms of the [GNU General Public License v3 (GPLv3)](https://github.com/hearot/pyrubrum/blob/v0.2.20/LICENSE).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyrubrum-continued Version: 0.2.19 Summary: An
+Metadata-Version: 2.1 Name: pyrubrum-continued Version: 0.2.20 Summary: An
 intuitive framework for creating Telegram bots Home-page: https://github.com/
 hearot/pyrubrum Author: Hearot Author-email: gabriel@hearot.it License: GPLv3
 Project-URL: Tracker, https://github.com/hearot/pyrubrum/issues Project-URL:
 Source, https://github.com/hearot/pyrubrum Keywords: bot bots chat messenger
 mtproto pyrogram python telegram Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v3 (GPLv3) Classifier: Natural Language ::
@@ -42,35 +42,35 @@
 encrypted parameters - Intuitive creation of inline keyboards - LRU caching
 with [functools.lru_cache](https://docs.python.org/3/library/
 functools.html#functools.lru_cache) - Native support for the *"Go back"* button
 - No limit for `callback_data` (see [Telegram Bot API](https://
 core.telegram.org/bots/api#inlinekeyboardbutton)) - Paging integration with
 `PageMenu` ### Examples In order to make use of the proposed examples, you need
 to create your own environment file by renaming [sample.env](https://
-github.com/hearot/pyrubrum/blob/v0.2.19/examples/sample.env) into `.env` and
+github.com/hearot/pyrubrum/blob/v0.2.20/examples/sample.env) into `.env` and
 editing all the necessary variables. - [CafÃ©](https://github.com/hearot/
-pyrubrum/blob/v0.2.19/examples/cafe_bot.py) - Get an overview of the design
+pyrubrum/blob/v0.2.20/examples/cafe_bot.py) - Get an overview of the design
 which lies inside Pyrubrum while interacting with multiple commands and pages.
-- [Calendar](https://github.com/hearot/pyrubrum/blob/v0.2.19/examples/
+- [Calendar](https://github.com/hearot/pyrubrum/blob/v0.2.20/examples/
 calendar_bot.py) - Get what day of the week a day is by simply choosing a year,
 a month and a day while discovering the potential of Pyrubrum page menus. -
-[Hitchhiker](https://github.com/hearot/pyrubrum/blob/v0.2.19/examples/
+[Hitchhiker](https://github.com/hearot/pyrubrum/blob/v0.2.20/examples/
 hitchhiker_bot.py) - Come to know how media are handled with Pyrubrum and...
 [get an existential question answered](https://en.wikipedia.org/wiki/
 Phrases_from_The_Hitchhiker%27s_Guide_to_the_Galaxy#The_Answer_to_the_Ultimate_Question_of_Life,_the_Universe,_and_Everything_is_42).
-- [Sample](https://github.com/hearot/pyrubrum/blob/v0.2.19/examples/
+- [Sample](https://github.com/hearot/pyrubrum/blob/v0.2.20/examples/
 sample_bot.py) - Interact with inline menus while understanding how Pyrubrum
 works. ### Changelog > See [CHANGELOG.md](https://github.com/hearot/pyrubrum/
-blob/v0.2.19/CHANGELOG.md). > Find new features in [FEATURES.md](https://
-github.com/hearot/pyrubrum/blob/v0.2.19/FEATURES.md). ### Commit messages > See
+blob/v0.2.20/CHANGELOG.md). > Find new features in [FEATURES.md](https://
+github.com/hearot/pyrubrum/blob/v0.2.20/FEATURES.md). ### Commit messages > See
 [Conventional Commits](https://www.conventionalcommits.org). ### Contributing >
-See [CONTRIBUTING.md](https://github.com/hearot/pyrubrum/blob/v0.2.19/
+See [CONTRIBUTING.md](https://github.com/hearot/pyrubrum/blob/v0.2.20/
 CONTRIBUTING.md). ### Versioning > See [PEP 440](https://www.python.org/dev/
 peps/pep-0440/). ### Thanks - [veggero/tytg](https://github.com/veggero/tytg)
 for giving me the idea of developing a simple framework with which you can code
 a folder-like bot. - [bakhoraliev](https://github.com/bakhoraliev) for letting
 me understand that an object-oriented library would make the difference in
 developing this project. ### Branding > See [hearot/pyrubrum-assets](https://
 github.com/hearot/pyrubrum-assets). ### Copyright & License - Copyright (C)
 2020 [Hearot](https://github.com/hearot). - Licensed under the terms of the
 [GNU General Public License v3 (GPLv3)](https://github.com/hearot/pyrubrum/
-blob/v0.2.19/LICENSE).
+blob/v0.2.20/LICENSE).
```

### Comparing `pyrubrum-continued-0.2.19/pyrubrum_continued.egg-info/SOURCES.txt` & `pyrubrum-continued-0.2.20/pyrubrum_continued.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/setup.py` & `pyrubrum-continued-0.2.20/setup.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/tests/test_deep_link_menu.py` & `pyrubrum-continued-0.2.20/tests/test_deep_link_menu.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,33 +27,36 @@
 USERNAMES[hash(client_test)] = username_test
 
 payload = "test_payload"
 
 expected_deep_link = "https://t.me/%s?start=%s" % (username_test, payload)
 
 
+@pytest.mark.asyncio
 @pytest.mark.parametrize("deep_type", PERMITTED_TYPES | {"fancytype"})
-def test_deep_link_menu(deep_type):
+async def test_deep_link_menu(deep_type):
     if deep_type in PERMITTED_TYPES:
         menu = DeepLinkMenu("Test", "test", payload, deep_type)
-        menu.button(None, client_test, None)
+        await menu.button(None, client_test, None)
     else:
         with pytest.raises(ValueError):
             DeepLinkMenu("Test", "test", payload, deep_type)
 
 
-def test_button():
+@pytest.mark.asyncio
+async def test_button():
     menu = DeepLinkMenu("Test", "test", payload)
-    button = menu.button(None, client_test, None)
+    button = await menu.button(None, client_test, None)
 
     assert button.link == expected_deep_link
     assert not hasattr(button, "menu_id")
     assert button.name == "Test"
 
 
-def test_button_with_function():
+@pytest.mark.asyncio
+async def test_button_with_function():
     menu = DeepLinkMenu("Test", "test", lambda a, b, c, d: payload)
-    button = menu.button(None, client_test, None)
+    button = await menu.button(None, client_test, None)
 
     assert button.link == expected_deep_link
     assert not hasattr(button, "menu_id")
     assert button.name == "Test"
```

### Comparing `pyrubrum-continued-0.2.19/tests/test_dict_database.py` & `pyrubrum-continued-0.2.20/tests/test_dict_database.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/tests/test_link_menu.py` & `pyrubrum-continued-0.2.20/tests/test_link_menu.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,29 +12,33 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with Pyrubrum. If not, see <http://www.gnu.org/licenses/>.
 
+import pytest
+
 from pyrubrum import LinkMenu
 
 example_link = "https://example.com"
 example_name = "Example"
 
 
-def test_button():
+@pytest.mark.asyncio
+async def test_button():
     link = LinkMenu(example_name, "test", example_link)
-    button = link.button(None, None, None)
+    button = await link.button(None, None, None)
 
     assert button.link == example_link
     assert not hasattr(button, "menu_id")
     assert button.name == example_name
 
 
-def test_button_with_function():
+@pytest.mark.asyncio
+async def test_button_with_function():
     link = LinkMenu(example_name, "test", lambda a, b, c, d: example_link)
-    button = link.button(None, None, None)
+    button = await link.button(None, None, None)
 
     assert button.link == example_link
     assert not hasattr(button, "menu_id")
     assert button.name == example_name
```

### Comparing `pyrubrum-continued-0.2.19/tests/test_menu.py` & `pyrubrum-continued-0.2.20/tests/test_menu.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,17 +82,14 @@
 
     def preliminary(a, b, c, d, e=None):
         worked.append(1)
 
     async def preliminary_async(a, b, c, d, e=None):
         worked.append(1)
 
-    async def preliminary_async(a, b, c, d=None):
-        worked.append(1)
-
     menu = Menu("Test", "test", "test_content", preliminary=preliminary)
     await menu.on_callback(handler, None, context)
     await menu.on_message(handler, None, context)
 
     menu = Menu("Test", "test", "test_content", preliminary=preliminary_async)
     await menu.on_callback(handler, None, context)
     await menu.on_message(handler, None, context)
```

### Comparing `pyrubrum-continued-0.2.19/tests/test_node.py` & `pyrubrum-continued-0.2.20/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `pyrubrum-continued-0.2.19/tests/test_version.py` & `pyrubrum-continued-0.2.20/tests/test_version.py`

 * *Files identical despite different names*

