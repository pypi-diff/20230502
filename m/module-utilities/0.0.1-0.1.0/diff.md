# Comparing `tmp/module-utilities-0.0.1.tar.gz` & `tmp/module-utilities-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "module-utilities-0.0.1.tar", last modified: Thu Apr 27 20:45:00 2023, max compression
+gzip compressed data, was "module-utilities-0.1.0.tar", last modified: Tue May  2 03:10:13 2023, max compression
```

## Comparing `module-utilities-0.0.1.tar` & `module-utilities-0.1.0.tar`

### file list

```diff
@@ -1,114 +1,118 @@
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 20:45:00.819540 module-utilities-0.0.1/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1361 2023-04-25 12:34:23.000000 module-utilities-0.0.1/.cruft.json
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      513 2023-04-25 12:34:23.000000 module-utilities-0.0.1/.editorconfig
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 20:45:00.775315 module-utilities-0.0.1/.github/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      374 2023-04-25 12:34:23.000000 module-utilities-0.0.1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1319 2023-04-25 19:34:57.000000 module-utilities-0.0.1/.gitignore
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      161 2023-04-25 12:34:23.000000 module-utilities-0.0.1/.markdownlint.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3581 2023-04-25 12:34:23.000000 module-utilities-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       20 2023-04-25 12:34:23.000000 module-utilities-0.0.1/.prettierrc.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      122 2023-04-25 12:34:23.000000 module-utilities-0.0.1/AUTHORS.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      180 2023-04-25 12:46:31.000000 module-utilities-0.0.1/CHANGELOG.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9217 2023-04-25 14:02:24.000000 module-utilities-0.0.1/CONTRIBUTING.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1645 2023-04-25 12:34:23.000000 module-utilities-0.0.1/LICENSE
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      258 2023-04-25 12:34:23.000000 module-utilities-0.0.1/MANIFEST.in
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    10572 2023-04-25 12:46:19.000000 module-utilities-0.0.1/Makefile
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5805 2023-04-27 20:45:00.819771 module-utilities-0.0.1/PKG-INFO
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2898 2023-04-27 20:43:16.000000 module-utilities-0.0.1/README.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 20:45:00.776124 module-utilities-0.0.1/changelog.d/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       64 2023-04-25 12:34:23.000000 module-utilities-0.0.1/changelog.d/README.txt
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 20:45:00.776819 module-utilities-0.0.1/changelog.d/templates/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 20:45:00.778290 module-utilities-0.0.1/changelog.d/templates/auto-changelog/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      213 2023-04-25 12:25:54.000000 module-utilities-0.0.1/changelog.d/templates/auto-changelog/macros.jinja2
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      774 2023-04-25 12:25:54.000000 module-utilities-0.0.1/changelog.d/templates/auto-changelog/template.jinja2
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      269 2023-04-25 12:34:23.000000 module-utilities-0.0.1/changelog.d/templates/new_fragment.md.j2
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      204 2023-04-27 20:43:16.000000 module-utilities-0.0.1/conftest.py
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 20:45:00.787817 module-utilities-0.0.1/docs/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1201 2023-04-25 12:34:23.000000 module-utilities-0.0.1/docs/Makefile
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 20:45:00.760962 module-utilities-0.0.1/docs/_static/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 20:45:00.788630 module-utilities-0.0.1/docs/_static/css/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2937 2023-04-25 12:34:23.000000 module-utilities-0.0.1/docs/_static/css/nist-combined.css
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 20:45:00.790544 module-utilities-0.0.1/docs/_static/js/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      767 2023-04-25 12:34:23.000000 module-utilities-0.0.1/docs/_static/js/leave_notice.js
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      706 2023-04-25 12:34:23.000000 module-utilities-0.0.1/docs/_static/js/nist-header-footer.js
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 20:45:00.795960 module-utilities-0.0.1/docs/_templates/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 20:45:00.800654 module-utilities-0.0.1/docs/_templates/autodocsumm/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      289 2023-04-25 12:34:23.000000 module-utilities-0.0.1/docs/_templates/autodocsumm/class-noindex.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      249 2023-04-25 12:34:23.000000 module-utilities-0.0.1/docs/_templates/autodocsumm/class.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      405 2023-04-25 12:34:23.000000 module-utilities-0.0.1/docs/_templates/autodocsumm/module-inherit.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      424 2023-04-25 12:34:23.000000 module-utilities-0.0.1/docs/_templates/autodocsumm/module-noindex.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      374 2023-04-25 12:34:23.000000 module-utilities-0.0.1/docs/_templates/autodocsumm/module.rst
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 20:45:00.802198 module-utilities-0.0.1/docs/_templates/autosummary/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      106 2023-04-25 12:34:23.000000 module-utilities-0.0.1/docs/_templates/autosummary/base.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1255 2023-04-25 12:34:23.000000 module-utilities-0.0.1/docs/_templates/autosummary/class.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1119 2023-04-25 12:34:23.000000 module-utilities-0.0.1/docs/_templates/autosummary/module.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1418 2023-04-25 12:34:23.000000 module-utilities-0.0.1/docs/_templates/class-individual-pages.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1255 2023-04-25 12:34:23.000000 module-utilities-0.0.1/docs/_templates/class-single-page.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1186 2023-04-25 12:34:23.000000 module-utilities-0.0.1/docs/_templates/custom-module-template.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1212 2023-04-25 12:34:23.000000 module-utilities-0.0.1/docs/_templates/module-custom-imported.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1177 2023-04-25 12:34:23.000000 module-utilities-0.0.1/docs/_templates/module-custom.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1071 2023-04-25 12:34:23.000000 module-utilities-0.0.1/docs/_templates/module-single.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1179 2023-04-25 12:34:23.000000 module-utilities-0.0.1/docs/_templates/module-template.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       69 2023-04-25 12:34:23.000000 module-utilities-0.0.1/docs/authors.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       71 2023-04-25 12:34:23.000000 module-utilities-0.0.1/docs/changelog.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    14799 2023-04-25 12:47:34.000000 module-utilities-0.0.1/docs/conf.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       74 2023-04-25 12:34:23.000000 module-utilities-0.0.1/docs/contributing.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 20:45:00.803993 module-utilities-0.0.1/docs/examples/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      887 2023-04-25 12:34:23.000000 module-utilities-0.0.1/docs/examples/create-symlinks.sh
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      550 2023-04-25 12:34:23.000000 module-utilities-0.0.1/docs/examples/example-usage.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       71 2023-04-25 12:34:23.000000 module-utilities-0.0.1/docs/examples/index.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 20:45:00.804563 module-utilities-0.0.1/docs/examples/usage/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1787 2023-04-25 12:34:23.000000 module-utilities-0.0.1/docs/examples/usage/demo.ipynb
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      241 2023-04-25 12:34:23.000000 module-utilities-0.0.1/docs/index.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      943 2023-04-25 12:34:23.000000 module-utilities-0.0.1/docs/installation.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       40 2023-04-25 12:34:23.000000 module-utilities-0.0.1/docs/license.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      767 2023-04-25 12:34:23.000000 module-utilities-0.0.1/docs/make.bat
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      169 2023-04-25 12:34:23.000000 module-utilities-0.0.1/docs/navigation.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 20:45:00.805094 module-utilities-0.0.1/docs/reference/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      144 2023-04-25 12:34:23.000000 module-utilities-0.0.1/docs/reference/index.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-25 12:34:23.000000 module-utilities-0.0.1/docs/spelling_wordlist.txt
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 20:45:00.810236 module-utilities-0.0.1/environment/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      943 2023-04-27 20:43:16.000000 module-utilities-0.0.1/environment/dev-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      220 2023-04-27 20:43:16.000000 module-utilities-0.0.1/environment/dev.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      108 2023-04-25 12:34:23.000000 module-utilities-0.0.1/environment/dist-conda.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       79 2023-04-25 12:34:23.000000 module-utilities-0.0.1/environment/dist-pypi.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      574 2023-04-25 12:34:23.000000 module-utilities-0.0.1/environment/docs-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      337 2023-04-27 20:43:16.000000 module-utilities-0.0.1/environment/docs.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       53 2023-04-25 12:34:23.000000 module-utilities-0.0.1/environment/lint-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      113 2023-04-27 20:43:16.000000 module-utilities-0.0.1/environment/lint.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       25 2023-04-25 12:34:23.000000 module-utilities-0.0.1/environment/test-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      104 2023-04-27 20:43:16.000000 module-utilities-0.0.1/environment/test.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      299 2023-04-25 12:34:23.000000 module-utilities-0.0.1/environment/tools.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      101 2023-04-27 20:42:59.000000 module-utilities-0.0.1/environment.yaml
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 20:45:00.810713 module-utilities-0.0.1/examples/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      222 2023-04-25 12:34:23.000000 module-utilities-0.0.1/examples/README.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 20:45:00.811200 module-utilities-0.0.1/examples/usage/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1787 2023-04-25 12:34:23.000000 module-utilities-0.0.1/examples/usage/demo.ipynb
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5421 2023-04-27 20:43:16.000000 module-utilities-0.0.1/pyproject.toml
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 20:45:00.812168 module-utilities-0.0.1/scripts/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1099 2023-04-25 12:34:23.000000 module-utilities-0.0.1/scripts/docs-examples-symlinks.sh
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      489 2023-04-25 12:34:23.000000 module-utilities-0.0.1/scripts/tox-ipykernel-display-name.sh
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      300 2023-04-27 20:45:00.820507 module-utilities-0.0.1/setup.cfg
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      323 2023-04-25 12:34:23.000000 module-utilities-0.0.1/setup.py
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 20:45:00.764943 module-utilities-0.0.1/src/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 20:45:00.813643 module-utilities-0.0.1/src/module_utilities/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      709 2023-04-27 20:43:16.000000 module-utilities-0.0.1/src/module_utilities/__init__.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     8354 2023-04-27 20:43:16.000000 module-utilities-0.0.1/src/module_utilities/cached.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    21684 2023-04-27 20:43:16.000000 module-utilities-0.0.1/src/module_utilities/docfiller.py
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 20:45:00.817111 module-utilities-0.0.1/src/module_utilities/external/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       26 2023-04-27 20:43:16.000000 module-utilities-0.0.1/src/module_utilities/external/__init__.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    23552 2023-04-27 20:43:16.000000 module-utilities-0.0.1/src/module_utilities/external/docscrape.py
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 20:45:00.816225 module-utilities-0.0.1/src/module_utilities.egg-info/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5805 2023-04-27 20:45:00.000000 module-utilities-0.0.1/src/module_utilities.egg-info/PKG-INFO
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2436 2023-04-27 20:45:00.000000 module-utilities-0.0.1/src/module_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-04-27 20:45:00.000000 module-utilities-0.0.1/src/module_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-04-25 12:55:39.000000 module-utilities-0.0.1/src/module_utilities.egg-info/not-zip-safe
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       30 2023-04-27 20:45:00.000000 module-utilities-0.0.1/src/module_utilities.egg-info/requires.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       17 2023-04-27 20:45:00.000000 module-utilities-0.0.1/src/module_utilities.egg-info/top_level.txt
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 20:45:00.819178 module-utilities-0.0.1/tests/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       46 2023-04-25 12:34:23.000000 module-utilities-0.0.1/tests/__init__.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 20:43:16.000000 module-utilities-0.0.1/tests/conftest.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9519 2023-04-27 20:43:16.000000 module-utilities-0.0.1/tests/test_cached.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     6359 2023-04-27 20:43:16.000000 module-utilities-0.0.1/tests/test_docfiller.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       92 2023-04-25 13:36:05.000000 module-utilities-0.0.1/tests/test_module_utilities.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4767 2023-04-27 20:43:16.000000 module-utilities-0.0.1/tox.ini
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.105541 module-utilities-0.1.0/
+-rw-r--r--   0 wpk      (42033)    36681     1361 2023-05-02 03:09:02.000000 module-utilities-0.1.0/.cruft.json
+-rw-r--r--   0 wpk      (42033)    36681      540 2023-05-02 03:09:02.000000 module-utilities-0.1.0/.editorconfig
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.011827 module-utilities-0.1.0/.github/
+-rw-r--r--   0 wpk      (42033)    36681      368 2023-05-02 03:09:02.000000 module-utilities-0.1.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 wpk      (42033)    36681     1307 2023-05-02 03:09:02.000000 module-utilities-0.1.0/.gitignore
+-rw-r--r--   0 wpk      (42033)    36681      161 2023-04-27 23:45:36.000000 module-utilities-0.1.0/.markdownlint.yaml
+-rw-r--r--   0 wpk      (42033)    36681     3581 2023-04-27 23:45:36.000000 module-utilities-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 wpk      (42033)    36681       20 2023-04-27 23:45:36.000000 module-utilities-0.1.0/.prettierrc.yaml
+-rw-r--r--   0 wpk      (42033)    36681      122 2023-04-27 23:45:36.000000 module-utilities-0.1.0/AUTHORS.md
+-rw-r--r--   0 wpk      (42033)    36681      271 2023-05-02 03:09:02.000000 module-utilities-0.1.0/CHANGELOG.md
+-rw-r--r--   0 wpk      (42033)    36681     9273 2023-05-02 03:09:02.000000 module-utilities-0.1.0/CONTRIBUTING.md
+-rw-r--r--   0 wpk      (42033)    36681     1645 2023-04-27 23:45:36.000000 module-utilities-0.1.0/LICENSE
+-rw-r--r--   0 wpk      (42033)    36681      258 2023-04-27 23:45:36.000000 module-utilities-0.1.0/MANIFEST.in
+-rw-r--r--   0 wpk      (42033)    36681    11231 2023-05-02 03:09:02.000000 module-utilities-0.1.0/Makefile
+-rw-r--r--   0 wpk      (42033)    36681     5914 2023-05-02 03:10:13.106029 module-utilities-0.1.0/PKG-INFO
+-rw-r--r--   0 wpk      (42033)    36681     2916 2023-04-27 23:45:36.000000 module-utilities-0.1.0/README.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.012488 module-utilities-0.1.0/changelog.d/
+-rw-r--r--   0 wpk      (42033)    36681       64 2023-04-27 23:45:36.000000 module-utilities-0.1.0/changelog.d/README.txt
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.013278 module-utilities-0.1.0/changelog.d/templates/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.014974 module-utilities-0.1.0/changelog.d/templates/auto-changelog/
+-rw-r--r--   0 wpk      (42033)    36681      213 2023-04-27 23:45:36.000000 module-utilities-0.1.0/changelog.d/templates/auto-changelog/macros.jinja2
+-rw-r--r--   0 wpk      (42033)    36681      774 2023-04-27 23:45:36.000000 module-utilities-0.1.0/changelog.d/templates/auto-changelog/template.jinja2
+-rw-r--r--   0 wpk      (42033)    36681      269 2023-04-27 23:45:36.000000 module-utilities-0.1.0/changelog.d/templates/new_fragment.md.j2
+-rw-r--r--   0 wpk      (42033)    36681      204 2023-04-27 23:45:36.000000 module-utilities-0.1.0/conftest.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.022045 module-utilities-0.1.0/docs/
+-rw-r--r--   0 wpk      (42033)    36681     1406 2023-05-02 03:09:02.000000 module-utilities-0.1.0/docs/Makefile
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:12.996629 module-utilities-0.1.0/docs/_static/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.022550 module-utilities-0.1.0/docs/_static/css/
+-rw-r--r--   0 wpk      (42033)    36681     2937 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/_static/css/nist-combined.css
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.024544 module-utilities-0.1.0/docs/_static/js/
+-rw-r--r--   0 wpk      (42033)    36681      767 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/_static/js/leave_notice.js
+-rw-r--r--   0 wpk      (42033)    36681      706 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/_static/js/nist-header-footer.js
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.034680 module-utilities-0.1.0/docs/_templates/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.041479 module-utilities-0.1.0/docs/_templates/autodocsumm/
+-rw-r--r--   0 wpk      (42033)    36681      289 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/_templates/autodocsumm/class-noindex.rst
+-rw-r--r--   0 wpk      (42033)    36681      249 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/_templates/autodocsumm/class.rst
+-rw-r--r--   0 wpk      (42033)    36681      405 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/_templates/autodocsumm/module-inherit.rst
+-rw-r--r--   0 wpk      (42033)    36681      424 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/_templates/autodocsumm/module-noindex.rst
+-rw-r--r--   0 wpk      (42033)    36681      374 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/_templates/autodocsumm/module.rst
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.044400 module-utilities-0.1.0/docs/_templates/autosummary/
+-rw-r--r--   0 wpk      (42033)    36681      106 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 wpk      (42033)    36681     1255 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 wpk      (42033)    36681     1119 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 wpk      (42033)    36681     1418 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/_templates/class-individual-pages.rst
+-rw-r--r--   0 wpk      (42033)    36681     1255 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/_templates/class-single-page.rst
+-rw-r--r--   0 wpk      (42033)    36681     1186 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/_templates/custom-module-template.rst
+-rw-r--r--   0 wpk      (42033)    36681     1212 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/_templates/module-custom-imported.rst
+-rw-r--r--   0 wpk      (42033)    36681     1177 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/_templates/module-custom.rst
+-rw-r--r--   0 wpk      (42033)    36681     1071 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/_templates/module-single.rst
+-rw-r--r--   0 wpk      (42033)    36681     1179 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/_templates/module-template.rst
+-rw-r--r--   0 wpk      (42033)    36681       69 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/authors.md
+-rw-r--r--   0 wpk      (42033)    36681       71 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/changelog.md
+-rw-r--r--   0 wpk      (42033)    36681    14799 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/conf.py
+-rw-r--r--   0 wpk      (42033)    36681       74 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/contributing.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.048983 module-utilities-0.1.0/docs/examples/
+-rw-r--r--   0 wpk      (42033)    36681      887 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/examples/create-symlinks.sh
+-rw-r--r--   0 wpk      (42033)    36681      540 2023-05-02 03:09:02.000000 module-utilities-0.1.0/docs/examples/example-usage.md
+-rw-r--r--   0 wpk      (42033)    36681       71 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/examples/index.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.050652 module-utilities-0.1.0/docs/examples/usage/
+-rw-r--r--   0 wpk      (42033)    36681     1787 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/examples/usage/demo.ipynb
+-rw-r--r--   0 wpk      (42033)    36681      241 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/index.md
+-rw-r--r--   0 wpk      (42033)    36681      943 2023-05-02 03:09:02.000000 module-utilities-0.1.0/docs/installation.md
+-rw-r--r--   0 wpk      (42033)    36681       40 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/license.md
+-rw-r--r--   0 wpk      (42033)    36681      767 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/make.bat
+-rw-r--r--   0 wpk      (42033)    36681      169 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/navigation.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.053297 module-utilities-0.1.0/docs/reference/
+-rw-r--r--   0 wpk      (42033)    36681      144 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/reference/index.md
+-rw-r--r--   0 wpk      (42033)    36681        0 2023-04-27 23:45:36.000000 module-utilities-0.1.0/docs/spelling_wordlist.txt
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.067973 module-utilities-0.1.0/environment/
+-rw-r--r--   0 wpk      (42033)    36681      943 2023-04-27 23:45:36.000000 module-utilities-0.1.0/environment/dev-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      232 2023-05-02 03:09:02.000000 module-utilities-0.1.0/environment/dev.yaml
+-rw-r--r--   0 wpk      (42033)    36681      108 2023-04-27 23:45:36.000000 module-utilities-0.1.0/environment/dist-conda.yaml
+-rw-r--r--   0 wpk      (42033)    36681       79 2023-04-27 23:45:36.000000 module-utilities-0.1.0/environment/dist-pypi.yaml
+-rw-r--r--   0 wpk      (42033)    36681      574 2023-04-27 23:45:36.000000 module-utilities-0.1.0/environment/docs-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      349 2023-05-02 03:09:02.000000 module-utilities-0.1.0/environment/docs.yaml
+-rw-r--r--   0 wpk      (42033)    36681       64 2023-05-02 03:09:02.000000 module-utilities-0.1.0/environment/lint-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      136 2023-05-02 03:09:02.000000 module-utilities-0.1.0/environment/lint.yaml
+-rw-r--r--   0 wpk      (42033)    36681       25 2023-04-27 23:45:36.000000 module-utilities-0.1.0/environment/test-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      116 2023-05-02 03:09:02.000000 module-utilities-0.1.0/environment/test.yaml
+-rw-r--r--   0 wpk      (42033)    36681      299 2023-04-27 23:45:36.000000 module-utilities-0.1.0/environment/tools.yaml
+-rw-r--r--   0 wpk      (42033)    36681      113 2023-05-02 03:09:02.000000 module-utilities-0.1.0/environment.yaml
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.069105 module-utilities-0.1.0/examples/
+-rw-r--r--   0 wpk      (42033)    36681      222 2023-04-27 23:45:36.000000 module-utilities-0.1.0/examples/README.md
+-rw-r--r--   0 wpk      (42033)    36681     6200 2023-05-02 03:09:02.000000 module-utilities-0.1.0/pyproject.toml
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.074828 module-utilities-0.1.0/scripts/
+-rw-r--r--   0 wpk      (42033)    36681      403 2023-05-02 03:09:02.000000 module-utilities-0.1.0/scripts/dist-conda.mk
+-rw-r--r--   0 wpk      (42033)    36681      312 2023-05-02 03:09:02.000000 module-utilities-0.1.0/scripts/dist-pypi.mk
+-rw-r--r--   0 wpk      (42033)    36681     1099 2023-04-27 23:45:36.000000 module-utilities-0.1.0/scripts/docs-examples-symlinks.sh
+-rw-r--r--   0 wpk      (42033)    36681      266 2023-05-02 03:09:02.000000 module-utilities-0.1.0/scripts/lint.mk
+-rw-r--r--   0 wpk      (42033)    36681       91 2023-05-02 03:09:02.000000 module-utilities-0.1.0/scripts/run-prettier.sh
+-rw-r--r--   0 wpk      (42033)    36681      489 2023-04-27 23:45:36.000000 module-utilities-0.1.0/scripts/tox-ipykernel-display-name.sh
+-rw-r--r--   0 wpk      (42033)    36681      300 2023-05-02 03:10:13.108394 module-utilities-0.1.0/setup.cfg
+-rw-r--r--   0 wpk      (42033)    36681      323 2023-04-27 23:45:36.000000 module-utilities-0.1.0/setup.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:12.999548 module-utilities-0.1.0/src/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.088628 module-utilities-0.1.0/src/module_utilities/
+-rw-r--r--   0 wpk      (42033)    36681      683 2023-05-02 03:09:02.000000 module-utilities-0.1.0/src/module_utilities/__init__.py
+-rw-r--r--   0 wpk      (42033)    36681     2646 2023-05-02 03:09:02.000000 module-utilities-0.1.0/src/module_utilities/_doc.py
+-rw-r--r--   0 wpk      (42033)    36681    23552 2023-05-02 03:09:02.000000 module-utilities-0.1.0/src/module_utilities/_docscrape.py
+-rw-r--r--   0 wpk      (42033)    36681      382 2023-05-02 03:09:02.000000 module-utilities-0.1.0/src/module_utilities/_typing.py
+-rw-r--r--   0 wpk      (42033)    36681     5824 2023-05-02 03:09:02.000000 module-utilities-0.1.0/src/module_utilities/attributedict.py
+-rw-r--r--   0 wpk      (42033)    36681     9856 2023-05-02 03:09:02.000000 module-utilities-0.1.0/src/module_utilities/cached.py
+-rw-r--r--   0 wpk      (42033)    36681    18093 2023-05-02 03:09:02.000000 module-utilities-0.1.0/src/module_utilities/docfiller.py
+-rw-r--r--   0 wpk      (42033)    36681        0 2023-05-02 03:09:02.000000 module-utilities-0.1.0/src/module_utilities/py.typed
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.099900 module-utilities-0.1.0/src/module_utilities.egg-info/
+-rw-r--r--   0 wpk      (42033)    36681     5914 2023-05-02 03:10:12.000000 module-utilities-0.1.0/src/module_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 wpk      (42033)    36681     2572 2023-05-02 03:10:12.000000 module-utilities-0.1.0/src/module_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 wpk      (42033)    36681        1 2023-05-02 03:10:12.000000 module-utilities-0.1.0/src/module_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 wpk      (42033)    36681        1 2023-04-25 12:55:39.000000 module-utilities-0.1.0/src/module_utilities.egg-info/not-zip-safe
+-rw-r--r--   0 wpk      (42033)    36681       48 2023-05-02 03:10:12.000000 module-utilities-0.1.0/src/module_utilities.egg-info/requires.txt
+-rw-r--r--   0 wpk      (42033)    36681       17 2023-05-02 03:10:12.000000 module-utilities-0.1.0/src/module_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 03:10:13.104771 module-utilities-0.1.0/tests/
+-rw-r--r--   0 wpk      (42033)    36681       46 2023-04-27 23:45:36.000000 module-utilities-0.1.0/tests/__init__.py
+-rw-r--r--   0 wpk      (42033)    36681        0 2023-04-27 23:45:36.000000 module-utilities-0.1.0/tests/conftest.py
+-rw-r--r--   0 wpk      (42033)    36681    10864 2023-05-02 03:09:02.000000 module-utilities-0.1.0/tests/test_cached.py
+-rw-r--r--   0 wpk      (42033)    36681     6176 2023-05-02 03:09:02.000000 module-utilities-0.1.0/tests/test_docfiller.py
+-rw-r--r--   0 wpk      (42033)    36681      169 2023-05-02 03:09:02.000000 module-utilities-0.1.0/tests/test_module_utilities.py
+-rw-r--r--   0 wpk      (42033)    36681     3950 2023-05-02 03:09:02.000000 module-utilities-0.1.0/tox.ini
```

### Comparing `module-utilities-0.0.1/.cruft.json` & `module-utilities-0.1.0/.cruft.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'commit'": "'38e14cd6d21fdc444081dcb1e34c15d0ebdc3683'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": "feature/markdown",
-    "commit": "0d65a8e29d3eb4691349e2dce13e9740a0cf7185",
+    "commit": "38e14cd6d21fdc444081dcb1e34c15d0ebdc3683",
     "context": {
         "cookiecutter": {
             "_copy_without_render": [
                 "*.html",
                 "docs/_templates/*.rst",
                 "docs/_templates/autosummary/*.rst",
                 "docs/_templates/autodocsumm/*.rst",
```

### Comparing `module-utilities-0.0.1/.editorconfig` & `module-utilities-0.1.0/.editorconfig`

 * *Files 13% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 
 [LICENSE]
 insert_final_newline = false
 
 [Makefile]
 indent_style = tab
 
+[*.mk]
+indent_style = tab
+
 [*.{yaml,yml}]
 indent_size = 2
 
 [*.ini]
 indent_size = 4
 
 [*.json]
```

### Comparing `module-utilities-0.0.1/.gitignore` & `module-utilities-0.1.0/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 # Distribution / packaging
 .Python
 env/
 build/
 develop-eggs/
 dist/
-dist-conda/
 downloads/
 eggs/
 .eggs/
 lib/
 lib64/
 parts/
 sdist/
```

### Comparing `module-utilities-0.0.1/.pre-commit-config.yaml` & `module-utilities-0.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `module-utilities-0.0.1/CONTRIBUTING.md` & `module-utilities-0.1.0/CONTRIBUTING.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,21 +25,22 @@
 ### Implement Features
 
 Look through the GitHub issues for features. Anything tagged with "enhancement"
 and "help wanted" is open to whoever wants to implement it.
 
 ### Write Documentation
 
-`module-utilities` could always use more documentation, whether
-as part of the official `module-utilities` docs, in docstrings,
-or even on the web in blog posts, articles, and such.
+`module-utilities` could always use more documentation, whether as part of the
+official `module-utilities` docs, in docstrings, or even on the web in blog
+posts, articles, and such.
 
 ### Submit Feedback
 
-The best way to send feedback is to file an issue at <https://github.com/wpk-nist-gov/module-utilities/issues>.
+The best way to send feedback is to file an issue at
+<https://github.com/wpk-nist-gov/module-utilities/issues>.
 
 If you are proposing a feature:
 
 - Explain in detail how it would work.
 - Keep the scope as narrow as possible, to make it easier to implement.
 - Remember that this is a volunteer-driven project, and that contributions are
   welcome :)
@@ -95,16 +96,16 @@
 
 ```console
 conda env update -n {env-name} environment/tools.yaml
 ```
 
 ### Getting the repo
 
-Ready to contribute? Here's how to set up `module_utilities` for
-local development.
+Ready to contribute? Here's how to set up `module_utilities` for local
+development.
 
 - Fork the `module_utilities` repo on GitHub.
 
 - Clone your fork locally:
 
   ```bash
   git clone git@github.com:your_name_here/module-utilities.git
@@ -151,15 +152,16 @@
   - Alternativley, you can create centrally located conda environmentment using
     the command:
 
     ```bash
     make mamba-dev
     ```
 
-    This will create a conda environment 'module-utilities-env' in the default location.
+    This will create a conda environment 'module-utilities-env' in the default
+    location.
 
     To install (an editable version) of the current package:
 
     ```bash
     pip install -e . --no-deps
     ```
 
@@ -288,41 +290,45 @@
 ## Building the docs
 
 We use [tox] to isolate the documentation build. Useful commands are as follows.
 
 - Build the docs:
 
   ```bash
-  tox -e docs-build
+  tox -e docs -- build
   ```
 
 - Spellcheck the docs:
 
   ```bash
-  tox -e docs-spelling
+  tox -e docs -- spelling
   ```
 
 - Create a release of the docs:
 
   ```bash
-  tox -e docs-release
+  tox -e docs -- release
   ```
 
   If you make any changes to `docs/examples`, you should run:
 
   ```bash
   make docs-examples-symlink
   ```
 
   to update symlinks from `docs/examples` to `examples`.
 
   After this, the docs can be pushed to the correct branch for distribution.
 
 - Live documentation updates using
 
+  ```bash
+  make docs-livehtml
+  ```
+
 ## Using tox
 
 The package is setup to use tox to test, build and release pip and conda
 distributions, and release the docs. Most of these tasks have a command in the
 `Makefile`. To test against multiple versions, use:
 
 ```bash
@@ -334,15 +340,15 @@
 ```bash
 make docs-build
 ```
 
 To release the documentation use:
 
 ```bash
-make docs-release posargs='-m "commit message" -r origin -p'
+make docs-release release_args='-m "commit message" -r origin -p'
 ```
 
 Where posargs is are passed to ghp-import. Note that the branch created is
 called `nist-pages`. This can be changed in `tox.ini`.
 
 To build the distribution, use:
```

### Comparing `module-utilities-0.0.1/LICENSE` & `module-utilities-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `module-utilities-0.0.1/Makefile` & `module-utilities-0.1.0/Makefile`

 * *Files 10% similar despite different names*

```diff
@@ -138,30 +138,30 @@
 
 version: version-scm version-import
 
 ################################################################################
 # Environment files
 ################################################################################
 ENVIRONMENTS = $(addsuffix .yaml,$(addprefix environment/, dev docs test))
-PRETTIER = pre-commit run prettier --files
+PRETTIER = bash scripts/run-prettier.sh
 
 environment/%.yaml: environment.yaml environment/%-extras.yaml ## create combined environment/{dev,docs,test}.yaml
 	conda-merge $^ > $@
-	-$(PRETTIER) $@ &> /dev/null || true
+	$(PRETTIER) $@
 
 environment/dev.yaml: ## development environment yaml file
 environment/test.yaml: ## testing environment yaml file
 enviornment/docs.yaml: ## docs environment yaml file
 
 
 # special for linters
 environment/lint.yaml: environment.yaml $(addsuffix .yaml, $(addprefix environment/, test-extras lint-extras)) ## mypy environment
 	echo $^
 	conda-merge $^ > $@
-	-$(PRETTIER) $@ &> /dev/null || true
+	$(PRETTIER) $@
 
 ENVIRONMENTS += environment/lint.yaml
 
 .PHONY: environment-files-clean
 environment-files-clean: ## clean all created environment/{dev,docs,test}.yaml
 	-rm $(ENVIRONMENTS) 2> /dev/null || true
 
@@ -184,106 +184,118 @@
 
 mamba-dev-update: environment/dev.yaml ## update development environment
 	mamba env update -f $<
 
 ################################################################################
 # TOX
 ###############################################################################
-tox_posargs?=-v
+tox_args?=-v
 version?=
-TOX=CONDA_EXE=mamba SETUPTOOLS_SCM_PRETEND_VERSION=$(version) tox $(tox_posargs)
+TOX=CONDA_EXE=mamba SETUPTOOLS_SCM_PRETEND_VERSION=$(version) tox $(tox_args)
 
 .PHONY: tox-ipykernel-display-name
 tox-ipykernel-display-name: ## Update display-name for any tox env with ipykernel
 	bash ./scripts/tox-ipykernel-display-name.sh module-utilities
 
 ## dev env
 .PHONY: dev-env
 dev-env: environment/dev.yaml ## create development environment using tox
 	tox -e dev
 
 ## testing
 .PHONY: test-all
-test-all: environment/test.yaml ## run tests on every Python version with tox
+test-all: environment/test.yaml ## run tests on every Python version with tox.  can pass posargs=...
 	$(TOX) -- $(posargs)
 
-
 ## docs
 .PHONY: docs-examples-symlink
 docs-examples-symlink: ## create symlinks to notebooks from /examples/ to /docs/examples.
 	bash ./scripts/docs-examples-symlinks.sh
 
 
-.PHONY: docs-build docs-release docs-clean docs-spelling docs-nist-pages docs-open docs-live docs-clean-build docs-linkcheck
-posargs=
+.PHONY: docs-build docs-release docs-clean docs-command
 docs-build: ## build docs in isolation
-	$(TOX) -e $@ -- $(posargs)
+	$(TOX) -e docs -- build
 docs-clean: ## clean docs
 	rm -rf docs/_build/*
 	rm -rf docs/generated/*
 	rm -rf docs/reference/generated/*
 docs-clean-build: docs-clean docs-build ## clean and build
-docs-release: ## release docs.  use posargs=... to override stuff
-	$(TOX) -e $@ -- $(posargs)
+docs-release: ## release docs.  use release_args=... to override stuff
+	$(TOX) -e docs -- release
+docs-command: ## run command with command=...
+	$(TOX) -e docs -- command
+
+.PHONY: .docs-spelling docs-nist-pages docs-open docs-livehtml docs-clean-build docs-linkcheck
 docs-spelling: ## run spell check with sphinx
-	$(TOX) -e $@ -- $(posargs)
-docs-nist-pages: ## do both build and releas
-	$(TOX) -e $@ -- $(posargs)
-docs-live: ## use autobuild for docs
-	$(TOX) -e $@ -- $(posargs)
+	$(TOX) -e docs -- spelling
+docs-livehtml: ## use autobuild for docs
+	$(TOX) -e docs -- livehtml
 docs-open: ## open the build
 	$(BROWSER) docs/_build/html/index.html
 docs-linkcheck: ## check links
-	$(TOX) -e docs-build -- linkcheck
+	$(TOX) -e docs -- linkcheck
+
+docs-build docs-release docs-command docs-clean docs-livehtml docs-linkcheck: environment/docs.yaml
 
-docs-build docs-release docs-clean docs-spelling docs-nist-pages docs-live: environment/docs.yaml
+## linting
+.PHONY: lint-mypy lint-pyright lint-pytype lint-all lint-command
+lint-mypy: ## run mypy mypy_args=...
+	$(TOX) -e lint -- mypy
+lint-pyright: ## run pyright pyright_args=...
+	$(TOX) -e lint -- pyright
+lint-pytype: ## run pytype pytype_args=...
+	$(TOX) -e lint -- pytype
+lint-all:
+	$(TOX) -e lint -- all
+lint-command:
+	$(TOX) -e lint -- command
 
+lint-mypy lint-pyright lint-pytype lint-all lint-command: environment/lint.yaml
 
 ## distribution
-.PHONY: dist-pypi-build dist-pypi-testrelease dist-pypi-release dist-conda-recipe dist-conda-build
+.PHONY: dist-pypi-build dist-pypi-testrelease dist-pypi-release dist-pypi-command
 
-posargs=
-dist-pypi-build: ## build dist, can pass posargs=... and tox_posargs=...
-	$(TOX) -e $@ -- $(posargs)
-dist-pypi-testrelease: ## test release on testpypi. can pass posargs=... and tox_posargs=...
-	$(TOX) -e $@ -- $(posargs)
+dist-pypi-build: ## build dist
+	$(TOX) -e dist-pypi -- build
+dist-pypi-testrelease: ## test release on testpypi
+	$(TOX) -e dist-pypi -- testrelease
 dist-pypi-release: ## release to pypi, can pass posargs=...
-	$(TOX) -e $@ -- $(posargs)
-dist-pypi-build dist-pypi-testrelease dist-pypi-release: environment/dist-pypi.yaml
+	$(TOX) -e dist-pypi -- release
+dist-pypi-command: ## run command with command=...
+	$(TOX) -e dist-pypi -- command
+dist-pypi-build dist-pypi-testrelease dist-pypi-release dist-pypi-command: environment/dist-pypi.yaml
 
+.PHONY: dist-conda-recipe dist-conda-build dist-conda-command
 dist-conda-recipe: ## build conda recipe can pass posargs=...
-	$(TOX) -e $@ -- $(posargs)
+	$(TOX) -e dist-conda -- recipe
 dist-conda-build: ## build conda recipe can pass posargs=...
-	$(TOX) -e $@ -- $(pasargs)
-dist-conda-build dist-conda-recipe: environment/dist-conda.yaml
+	$(TOX) -e dist-conda -- build
+dist-conda-command: ## run command with command=...
+	$(TOX) -e dist-conda -- command
+dist-conda-build dist-conda-recipe dist-conda-command: environment/dist-conda.yaml
 
 
 ## test distribution
-.PHONY: test-dist-pypi-remote test-dist-conda-remote test-dist-pypi-local test-dist-conda-local
+.PHONY: testdist-pypi-remote testdist-conda-remote testdist-pypi-local testdist-conda-local
 
 py?=310
-test-dist-pypi-remote: ## test pypi install, can run as `make test-dist-pypi-remote py=39` to run test-dist-pypi-local-py39
+testdist-pypi-remote: ## test pypi install, can run as `make test-dist-pypi-remote py=39` to run test-dist-pypi-local-py39
 	$(TOX) -e $@-py$(py) -- $(posargs)
-
-test-dist-conda-remote: ## test conda install, can run as `make test-dist-conda-remote py=39` to run test-dist-conda-local-py39
+testdist-conda-remote: ## test conda install, can run as `make test-dist-conda-remote py=39` to run test-dist-conda-local-py39
 	$(TOX) -e $@-py$(py) -- $(poasargs)
-
-test-dist-pypi-local: ## test pypi install, can run as `make test-dist-pypi-local py=39` to run test-dist-pypi-local-py39
+testdist-pypi-local: ## test pypi install, can run as `make test-dist-pypi-local py=39` to run test-dist-pypi-local-py39
 	$(TOX) -e $@-py$(py) -- $(posargs)
-
-test-dist-conda-local: ## test conda install, can run as `make test-dist-conda-local py=39` to run test-dist-conda-local-py39
+testdist-conda-local: ## test conda install, can run as `make test-dist-conda-local py=39` to run test-dist-conda-local-py39
 	$(TOX) -e $@-py$(py) -- $(poasargs)
 
-
-test-dist-pypi: environment/test.
-
+testdist-pypi-remote testdist-conda-remote testdist-pypi-local testdist-conda-local: environment/test.yaml
 
 ## list all options
 .PHONY: tox-list
-
 tox-list:
 	$(TOX) -a
 
 
 ################################################################################
 # installation
 ################################################################################
```

### Comparing `module-utilities-0.0.1/PKG-INFO` & `module-utilities-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: module-utilities
-Version: 0.0.1
+Version: 0.1.0
 Summary: Collection of utilities to aid working with python modules.
 Home-page: https://github.com/wpk-nist-gov/module-utilities
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
 License: NIST license
 Project-URL: homepage, https://github.com/wpk-nist-gov/module-utilities
 Project-URL: documentation, https://pages.nist.gov/module-utilities/
 Keywords: module-utilities
@@ -101,17 +101,19 @@
 ```python
 import module_utilities
 
 ```
 
 <!-- end-docs -->
 
-## Documentation
+<!-- ## Documentation -->
 
+<!--
 See the [documentation][docs-link] for a look at `module-utilities` in action.
+-->
 
 ## License
 
 This is free software. See [LICENSE][license-link].
 
 ## Related work
 
@@ -131,18 +133,25 @@
 
 # Changelog
 
 Changelog for `module-utilities`
 
 ## Unreleased
 
-See the fragment files in [changelog.d](https://github.com/wpk-nist-gov/module-utilities)
+See the fragment files in
+[changelog.d](https://github.com/wpk-nist-gov/module-utilities)
 
 <!-- scriv-insert-here -->
 
+## v0.1.0 — 2023-05-01
+
+### Added
+
+- Add typing support. Passing mypy, pyright, pytype.
+
 This software was developed by employees of the National Institute of Standards
 and Technology (NIST), an agency of the Federal Government. Pursuant to title 17
 United States Code Section 105, works of NIST employees are not subject to
 copyright protection in the United States and are considered to be in the public
 domain. Permission to freely use, copy, modify, and distribute this software and
 its documentation without fee is hereby granted, provided that this notice and
 disclaimer of warranty appears in all copies.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `module-utilities-0.0.1/README.md` & `module-utilities-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -74,17 +74,19 @@
 ```python
 import module_utilities
 
 ```
 
 <!-- end-docs -->
 
-## Documentation
+<!-- ## Documentation -->
 
+<!--
 See the [documentation][docs-link] for a look at `module-utilities` in action.
+-->
 
 ## License
 
 This is free software. See [LICENSE][license-link].
 
 ## Related work
```

### Comparing `module-utilities-0.0.1/changelog.d/templates/auto-changelog/template.jinja2` & `module-utilities-0.1.0/changelog.d/templates/auto-changelog/template.jinja2`

 * *Files identical despite different names*

### Comparing `module-utilities-0.0.1/docs/Makefile` & `module-utilities-0.1.0/docs/Makefile`

 * *Files 20% similar despite different names*

```diff
@@ -14,33 +14,39 @@
 ALLSPHINXAUTOOPTS = $(ALLSPHINXOPTS) \
 	--ignore "*/$(BUILDDIR)/*" \
 	--ignore "*/generated/*" \
 	--ignore "*/jupyter_execute/*" \
 	--ignore "*/.ipynb_checkpoints/*"
 
 
+
+.PHONY: help Makefile clean-all build livehtml showlinks release command
 # Put it first so that "make" without argument is like "make help".
 help:
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(ALLSPHINXOPTS) $(O)
 
-
-allclean: clean
-	rm -rf $(BUILDDIR)/*
-	rm -rf generated/*
-	rm -rf reference/generated/*
-
-.PHONY: help Makefile allclean
-
 # Catch-all target: route all unknown targets to Sphinx using the new
 # "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
 %: Makefile
 	$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(ALLSPHINXOPTS) $(O)
 
+clean-all: clean
+	rm -rf $(BUILDDIR)/*
+	rm -rf generated/*
+	rm -rf reference/generated/*
+
+# Alias to html
+build: html
 
-.PHONY: livehtml
 livehtml:
 	$(SPHINXAUTOBUILD) "$(SOURCEDIR)" "$(BUILDDIR)/html" $(ALLSPHINXAUTOOPTS) $(O)
 
-
-.PHONY: showlinks
 showlinks:
 	python -m sphinx.ext.intersphinx $(BUILDDIR)/html/objects.inv
+
+release_args ?= '-m "update docs" -b nist-pages'
+release:
+	ghp-import -o -n -m $(release_args) $(BUILDDIR)/html
+
+command ?= @echo pass "command=..."
+command:
+	$(command)
```

### Comparing `module-utilities-0.0.1/docs/_static/css/nist-combined.css` & `module-utilities-0.1.0/docs/_static/css/nist-combined.css`

 * *Files identical despite different names*

### Comparing `module-utilities-0.0.1/docs/_static/js/leave_notice.js` & `module-utilities-0.1.0/docs/_static/js/leave_notice.js`

 * *Files identical despite different names*

### Comparing `module-utilities-0.0.1/docs/_static/js/nist-header-footer.js` & `module-utilities-0.1.0/docs/_static/js/nist-header-footer.js`

 * *Files identical despite different names*

### Comparing `module-utilities-0.0.1/docs/_templates/autosummary/class.rst` & `module-utilities-0.1.0/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.0.1/docs/_templates/autosummary/module.rst` & `module-utilities-0.1.0/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.0.1/docs/_templates/class-individual-pages.rst` & `module-utilities-0.1.0/docs/_templates/class-individual-pages.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.0.1/docs/_templates/class-single-page.rst` & `module-utilities-0.1.0/docs/_templates/class-single-page.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.0.1/docs/_templates/custom-module-template.rst` & `module-utilities-0.1.0/docs/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.0.1/docs/_templates/module-custom-imported.rst` & `module-utilities-0.1.0/docs/_templates/module-custom-imported.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.0.1/docs/_templates/module-custom.rst` & `module-utilities-0.1.0/docs/_templates/module-custom.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.0.1/docs/_templates/module-single.rst` & `module-utilities-0.1.0/docs/_templates/module-single.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.0.1/docs/_templates/module-template.rst` & `module-utilities-0.1.0/docs/_templates/module-template.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.0.1/docs/conf.py` & `module-utilities-0.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `module-utilities-0.0.1/docs/examples/create-symlinks.sh` & `module-utilities-0.1.0/docs/examples/create-symlinks.sh`

 * *Files identical despite different names*

### Comparing `module-utilities-0.0.1/docs/examples/example-usage.md` & `module-utilities-0.1.0/docs/examples/example-usage.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ---
 jupytext:
-    text_representation:
-        format_name: myst
+  text_representation:
+    format_name: myst
 kernelspec:
-    display_name: Python 3
-    name: python3
+  display_name: Python 3
+  name: python3
 ---
 
 # Usage
 
 An example for using ipython directives or jupytext
 
 ## jupytext
```

### Comparing `module-utilities-0.0.1/docs/examples/usage/demo.ipynb` & `module-utilities-0.1.0/docs/examples/usage/demo.ipynb`

 * *Files identical despite different names*

### Comparing `module-utilities-0.0.1/docs/installation.md` & `module-utilities-0.1.0/docs/installation.md`

 * *Files 12% similar despite different names*

```diff
@@ -10,21 +10,20 @@
 
 or
 
 ```bash
 conda install -c wpk-nist module_utilities
 ```
 
-This is the preferred method to install module-utilities, as it
-will always install the most recent stable release.
+This is the preferred method to install module-utilities, as it will always
+install the most recent stable release.
 
 ## From sources
 
-The sources for module-utilities can be downloaded from the
-[Github repo].
+The sources for module-utilities can be downloaded from the [Github repo].
 
 You can either clone the public repository:
 
 ```bash
 git clone git://github.com/wpk-nist-gov/module-utilities.git
 ```
 
@@ -38,10 +37,11 @@
 
 ```bash
 conda env create [-n {name}] -f environment.yaml
 conda activate {name}
 pip install [-e] --no-deps .
 ```
 
-where options in brackets are options (for environment name, and editable install, repectively).
+where options in brackets are options (for environment name, and editable
+install, repectively).
 
 [github repo]: https://github.com/wpk-nist-gov/module-utilities
```

### Comparing `module-utilities-0.0.1/docs/make.bat` & `module-utilities-0.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `module-utilities-0.0.1/environment/dev-extras.yaml` & `module-utilities-0.1.0/environment/dev-extras.yaml`

 * *Files identical despite different names*

### Comparing `module-utilities-0.0.1/environment/docs-extras.yaml` & `module-utilities-0.1.0/environment/docs-extras.yaml`

 * *Files identical despite different names*

### Comparing `module-utilities-0.0.1/pyproject.toml` & `module-utilities-0.1.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
 ]
 dynamic = ["readme", "version"]
 requires-python = ">=3.8"
-dependencies = []
+dependencies = ["typing-extensions"]
 
 [project.urls]
 homepage = "https://github.com/wpk-nist-gov/module-utilities"
 documentation = "https://pages.nist.gov/module-utilities/"
 
 [project.optional-dependencies]
 test = ["pytest"]
@@ -60,16 +60,17 @@
 [tool.setuptools_scm]
 fallback_version = "999"
 
 [tool.aliases]
 test = "pytest"
 
 [tool.pytest.ini_options]
-addopts = "--verbose --doctest-modules --ignore-glob=**/docfiller.py"
-testpaths = ["tests", "src"]
+addopts = "--doctest-modules"
+# testpaths = ["src/module_utilities", "tests"]
+testpaths = ["src", "tests"]
 
 [tool.isort]
 profile = "black"
 skip_gitignore = true
 known_first_party = ["module_utilities"]
 
 [tool.ruff]
@@ -218,25 +219,51 @@
 
 [tool.commitizen]
 use_shortcuts = true
 
 [tool.cruft]
 
 [tool.mypy]
-files = ["src/module_utilities"]
+files = ["src/**/*.py", "tests/**/*.py"]
+# files = ["src", "tests"]
 show_error_codes = true
 warn_unused_ignores = true
 warn_return_any = true
 warn_unused_configs = true
 exclude = [".eggs", ".tox", "doc", "docs"]
+check_untyped_defs = true
 
 [[tool.mypy.overrides]]
 ignore_missing_imports = true
 module = []
 
 [[tool.mypy.overrides]]
 ignore_errors = true
 module = []
 
 [tool.pyright]
 include = ["src", "tests"]
 exclude = ["**/__pycache__", ".tox/**", "**/.mypy_cache"]
+pythonVersion = "3.10"
+typeCheckingMode = "basic"
+# enable subset of "strict"
+reportDuplicateImport = true
+reportInvalidStubStatement = true
+reportOverlappingOverload = true
+reportPropertyTypeMismatch = true
+reportUntypedClassDecorator = true
+reportUntypedFunctionDecorator = true
+reportUntypedNamedTuple = true
+reportUnusedImport = true
+# disable subset of "basic"
+reportGeneralTypeIssues = false
+reportMissingModuleSource = false
+reportOptionalCall = false
+reportOptionalIterable = false
+reportOptionalMemberAccess = false
+reportOptionalOperand = false
+reportOptionalSubscript = false
+reportPrivateImportUsage = false
+reportUnboundVariable = false
+
+[tool.pytype]
+inputs = ["src", "tests"]
```

### Comparing `module-utilities-0.0.1/scripts/docs-examples-symlinks.sh` & `module-utilities-0.1.0/scripts/docs-examples-symlinks.sh`

 * *Files identical despite different names*

### Comparing `module-utilities-0.0.1/src/module_utilities/__init__.py` & `module-utilities-0.1.0/src/module_utilities/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from . import cached, docfiller
 
 # updated versioning scheme
 try:
     from importlib.metadata import version as _version
 except ImportError:
     # if the fallback library is missing, we are doomed.
-    from importlib_metadata import version as _version  # type: ignore[no-redef]
+    from importlib_metadata import version as _version
 
 try:
     __version__ = _version("module_utilities")
 except Exception:
     # Local copy or not installed with setuptools.
     # Disable minimum version checks on downstream libraries.
     __version__ = "999"
```

### Comparing `module-utilities-0.0.1/src/module_utilities/cached.py` & `module-utilities-0.1.0/src/module_utilities/cached.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,75 @@
 """Routines to define cached properties/methods in a class."""
+from __future__ import annotations
 
 from functools import wraps
 from inspect import signature
+from typing import Any, Callable, TypeVar, cast, overload
+
+from typing_extensions import ParamSpec
 
 __all__ = ["decorate", "prop", "meth", "clear"]
 
+# from ._typing import F
+
+P = ParamSpec("P")
+R = TypeVar("R")
+
+
+# @overload
+# def decorate(
+#     *, key=..., as_property: Literal[True] = ..., check_use_cache=...
+# ) -> Callable[[Callable[[Any], R]], R]:
+#     ...
+
+# @overload
+# def decorate(
+#     *, key=..., as_property: Literal[False] = ..., check_use_cache=...
+# ) -> Callable[[Callable[P, R]], Callable[P, R]]:
+#     ...
 
-def decorate(*funcs, key=None, as_property=True, check_use_cache=False):
-    """General purpose cached decorator."""
+
+def decorate(
+    *, key: str | None = None, as_property: bool = True, check_use_cache: bool = False
+):  # -> Callable[[Callable[[Any], R]], R] | Callable[[Callable[P, R]], Callable[P, R]]:
+    """
+    General purpose cached decorator.
+
+    Must always be called.
+    """
     if as_property:
-        return prop(*funcs, key=key, check_use_cache=check_use_cache)
+        return prop(key=key, check_use_cache=check_use_cache)
     else:
-        return meth(*funcs, key=key, check_use_cache=check_use_cache)
+        return meth(key=key, check_use_cache=check_use_cache)
 
 
-def prop(*funcs, key=None, check_use_cache=False):
+@overload
+def prop(func: Callable[[Any], R]) -> R:
+    ...
+
+
+@overload
+def prop(
+    *, key: str | None = None, check_use_cache: bool = False
+) -> Callable[[Callable[[Any], R]], R]:
+    ...
+
+
+def prop(
+    func: Callable[[Any], R] | None = None,
+    *,
+    key: str | None = None,
+    check_use_cache: bool = False,
+) -> R | Callable[[Callable[[Any], R]], R]:
     """
     Decorator to cache a property within a class.
 
     Parameters
     ----------
-    *funcs : callable
+    _func: callable
         This parameter is used in the case that you decorate without ().
         That is, you can decorate with ``@prop`` or ``@prop()``.
     key : string, optional
         Optional key for storage in `_cache`.
         Default to attribute/method ``__name__``.
     check_use_cache : bool, default=False
         If `True`, then only apply caching if
@@ -97,49 +142,61 @@
 
     See Also
     --------
     clear : corresponding decorator to clear cache
     meth : decorator for cache creation of function
     """
 
-    def cached_lookup(func):
+    def cached_lookup(_func: Callable[[Any], R]) -> R:
         if key is None:
-            key_inner = func.__name__
+            key_inner = _func.__name__
         else:
             key_inner = key
 
-        @property
-        @wraps(func)
-        def wrapper(self, *args, **kwargs):
+        @wraps(_func)
+        def wrapper(self) -> R:
             if (not check_use_cache) or (getattr(self, "_use_cache", False)):
                 try:
-                    return self._cache[key_inner]
+                    return cast(R, self._cache[key_inner])
                 except AttributeError:
                     self._cache = dict()
                 except KeyError:
                     pass
 
-                self._cache[key_inner] = ret = func(self, *args, **kwargs)
+                self._cache[key_inner] = ret = _func(self)
                 return ret
             else:
-                return func(self, *args, **kwargs)
+                return _func(self)
 
-        return wrapper
+        return property(wrapper)  # type: ignore
 
-    if len(funcs) == 0:
-        return cached_lookup
-    elif len(funcs) == 1 and callable(funcs[0]):
-        return cached_lookup(funcs[0])
+    if func:
+        return cached_lookup(func)
     else:
-        raise ValueError(
-            "Must call either single callable func or no func. If setting `key`, pass `key=value`."
-        )
+        return cached_lookup
+
 
+@overload
+def meth(func: Callable[P, R]) -> Callable[P, R]:
+    ...
 
-def meth(*funcs, key=None, check_use_cache=False):
+
+@overload
+def meth(
+    *, key: str | None = None, check_use_cache: bool = False
+) -> Callable[[Callable[P, R]], Callable[P, R]]:
+    ...
+
+
+def meth(
+    func: Callable[P, R] | None = None,
+    *,
+    key: str | None = None,
+    check_use_cache: bool = False,
+) -> Callable[P, R] | Callable[[Callable[P, R]], Callable[P, R]]:
     """
     Decorator to cache a function within a class
 
     Requires the Class to have a cache dict called ``_cache``.
 
     Examples
     --------
@@ -173,62 +230,71 @@
 
     See Also
     --------
     clear : corresponding decorator to remove cache
     prop : decorator for properties
     """
 
-    def cached_lookup(func):
+    def cached_lookup(_func: Callable[P, R]) -> Callable[P, R]:
         if key is None:
-            key_inner = func.__name__
+            key_inner = _func.__name__
         else:
             key_inner = key
 
         # use signature
-        bind = signature(func).bind
+        bind = signature(_func).bind
 
-        @wraps(func)
-        def wrapper(self, *args, **kwargs):
+        @wraps(_func)
+        def wrapper(*args: P.args, **kwargs: P.kwargs) -> R:
+            self = args[0]
             if (not check_use_cache) or (getattr(self, "_use_cache", False)):
-                params = bind(self, *args, **kwargs)
+                params = bind(*args, **kwargs)
                 params.apply_defaults()
                 key_func = (
                     key_inner,
                     params.args[1:],
                     frozenset(params.kwargs.items()),
                 )
                 try:
-                    return self._cache[key_func]
+                    return cast(R, self._cache[key_func])  # type: ignore
                 except TypeError:
                     # this means that key_func is bad hash
-                    return func(self, *args, **kwargs)
+                    return _func(*args, **kwargs)
                 except AttributeError:
-                    self._cache = dict()
+                    self._cache = dict()  # type: ignore
                 except KeyError:
                     pass
 
-                self._cache[key_func] = ret = func(self, *args, **kwargs)
+                self._cache[key_func] = ret = _func(*args, **kwargs)  # type: ignore
                 return ret
 
             else:
-                return func(self, *args, **kwargs)
+                return _func(*args, **kwargs)
 
         return wrapper
 
-    if len(funcs) == 0:
-        return cached_lookup
-    elif len(funcs) == 1 and callable(funcs[0]):
-        return cached_lookup(funcs[0])
+    if func:
+        return cached_lookup(func)
     else:
-        raise ValueError(
-            "Must call either single callable func or no func. If setting `key`, pass `key=value`."
-        )
+        return cached_lookup
+
+
+@overload
+def clear(key_or_func: Callable[P, R]) -> Callable[P, R]:
+    ...
+
+
+@overload
+def clear(key_or_func: str, *keys: str) -> Callable[[Callable[P, R]], Callable[P, R]]:
+    ...
 
 
-def clear(*keys):
+def clear(
+    key_or_func: str | Callable[P, R], *keys: str
+) -> Callable[P, R] | Callable[[Callable[P, R]], Callable[P, R]]:
     """
     Decorator to clear self._cache of specified properties
 
     Parameters
     ----------
     *keys :
         Remove these keys from cache.  if len(keys)==0, remove all keys.
@@ -277,42 +343,46 @@
 
     See Also
     --------
     prop : corresponding decorator for cache creation of property
     meth : decorator for cache creation of function
     """
 
-    if len(keys) == 1 and callable(keys[0]):
-        function = keys[0]
-        keys = ()
+    if callable(key_or_func):
+        function = key_or_func
+        keys_inner = keys
     else:
         function = None
+        keys_inner = (key_or_func,) + keys
 
-    def decorator(func):
+    def decorator(func: Callable[P, R]) -> Callable[P, R]:
         @wraps(func)
-        def wrapper(self, *args, **kwargs):
-            # self._clear_caches(*keys)
-            # clear out keys
+        def wrapper(*args: P.args, **kwargs: P.kwargs) -> R:
+            # self._clear_caches(*keys_inner)
+            # clear out keys_inner
+            self = args[0]
             if hasattr(self, "_cache"):
-                if len(keys) == 0:
+                if len(keys_inner) == 0:
                     self._cache = dict()
                 else:
-                    for name in keys:
+                    for name in keys_inner:
                         try:
                             del self._cache[name]
                         except KeyError:
                             pass
 
                     # functions
                     keys_tuples = [
-                        k for k in self._cache if isinstance(k, tuple) and k[0] in keys
+                        k
+                        for k in self._cache
+                        if isinstance(k, tuple) and k[0] in keys_inner
                     ]
-                    for name in keys_tuples:
-                        del self._cache[name]
-            return func(self, *args, **kwargs)
+                    for k in keys_tuples:
+                        del self._cache[k]
+            return func(*args, **kwargs)
 
         return wrapper
 
     if function:
         return decorator(function)
     else:
         return decorator
```

### Comparing `module-utilities-0.0.1/src/module_utilities/docfiller.py` & `module-utilities-0.1.0/src/module_utilities/docfiller.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,41 @@
 """
-Fill and share documentation (:mod:`module_utilities.docfiller`)
+Fill and share documentation (:mod:`module_utilities.doc_decorate`)
 ================================================================
 """
-# type: ignore
 from __future__ import annotations
 
 import inspect
 import os
-from collections.abc import Mapping
 from textwrap import dedent
-from typing import Any, Callable, TypeVar
+from typing import TYPE_CHECKING, Any, Callable
 
 from . import cached
-from .external.docscrape import NumpyDocString, Parameter
+from ._doc import doc as _pd_doc
+from ._docscrape import NumpyDocString, Parameter  # type: ignore
+from .attributedict import AttributeDict
+
+if TYPE_CHECKING:
+    from collections.abc import Mapping, Sequence
+
+    from ._typing import F
 
 try:
     # Default is DOC_SUB is True
     DOC_SUB = os.getenv("DOCFILLER_SUB", "True").lower() not in (
         "0",
         "f",
         "false",
     )
 except KeyError:
     DOC_SUB = True
 
 
-# Taken directly from pandas.utils._decorators.doc
-# See https://github.com/pandas-dev/pandas/blob/main/pandas/util/_decorators.py
-# would just use the pandas version, but since it's a private
-# module, feel it's better to have static version here.
-
-
-# to maintain type information across generic functions and parametrization
-T = TypeVar("T")
-# used in decorators to preserve the signature of the function it decorates
-# see https://mypy.readthedocs.io/en/stable/generics.html#declaring-decorators
-FuncType = Callable[..., Any]
-F = TypeVar("F", bound=FuncType)
-
-
-def doc(*docstrings: str | Callable, **params) -> Callable[[F], F]:
+# Factory method to create doc_decorate
+def doc_decorate(*docstrings: str | Callable, **params) -> Callable[[F], F]:
     """
     A decorator take docstring templates, concatenate them and perform string
     substitution on it.
 
     This decorator will add a variable "_docstring_components" to the wrapped
     callable to keep track the original docstring template for potential usage.
     If it should be consider as a template, it will be saved as a string.
@@ -53,249 +45,32 @@
     Parameters
     ----------
     *docstrings : str or callable
         The string / docstring / docstring template to be appended in order
         after default docstring under callable.
     **params
         The string which would be used to format docstring template.
-    """
-
-    def decorator(decorated: F) -> F:
-        # collecting docstring and docstring templates
-        docstring_components: list[str | Callable] = []
-        if decorated.__doc__:
-            docstring_components.append(dedent(decorated.__doc__))
-
-        for docstring in docstrings:
-            if hasattr(docstring, "_docstring_components"):
-                # error: Item "str" of "Union[str, Callable[..., Any]]" has no attribute
-                # "_docstring_components"
-                # error: Item "function" of "Union[str, Callable[..., Any]]" has no
-                # attribute "_docstring_components"
-                docstring_components.extend(docstring._docstring_components)
-            elif isinstance(docstring, str) or docstring.__doc__:
-                docstring_components.append(docstring)
-
-        # formatting templates and concatenating docstring
-        decorated.__doc__ = "".join(
-            [
-                # change to format_map to avoid converting to a dict.
-                # component.format(**params)
-                component.format_map(params)
-                if isinstance(component, str)
-                else dedent(component.__doc__ or "")
-                for component in docstring_components
-            ]
-        )
-
-        # error: "F" has no attribute "_docstring_components"
-        decorated._docstring_components = docstring_components
-        return decorated
-
-    return decorator
-
-
-# Factory method to create docfiller
-def docfiller(*templates, **params):
-    """
-    To fill common docs.
 
-    Taken from pandas.utils._decorators
+    Notes
+    -----
+    Doc filling can be turned off by setting the environment variable
+    ``DOCFILLER_SUB`` to one of ``0, f, false``.
     """
 
     if DOC_SUB:
-        return doc(*templates, **params)
+        return _pd_doc(*docstrings, **params)
     else:
 
         def decorated(func):
             return func
 
         return decorated
 
 
-def _get_nested_values(d, join_string="\n"):
-    out = []
-    for k in d:
-        v = d[k]
-        if isinstance(v, str):
-            out.append(v)
-        else:
-            out.extend(_get_nested_values(v, join_string=None))
-
-    if join_string is not None:
-        out = join_string.join(out)
-
-    return out
-
-
-class AttributeDict(Mapping):
-    """
-    Dictionary with recursive attribute like access.
-
-    To be used in str.format calls, so can expand on fields like
-    `{name.property}` in a nested manner.
-
-    Parameters
-    ----------
-    entries : dict
-    recursive : bool, default=True
-        If True, recursively return ``AttributeDict`` for nested dicts.
-
-    Example
-    -------
-    >>> d = AttributeDict({"a": 1, "b": {"c": 2}})
-    >>> d.a
-    1
-    >>> d.b
-    AttributeDict({'c': 2})
-    >>> d.b.c
-    2
-    """
-
-    __slots__ = ("_entries", "_recursive", "_allow_missing")
-
-    def __init__(self, entries=None, recursive=True, allow_missing=True):
-        if entries is None:
-            entries = {}
-        self._entries = entries
-        self._recursive = recursive
-        self._allow_missing = allow_missing
-
-    def __getitem__(self, key):
-        if isinstance(key, slice):
-            return _get_nested_values(self._getslice(key), join_string="\n")
-
-        if key == ":":
-            return _get_nested_values(self._entries, join_string="\n")
-
-        elif "," in key:
-            return "\n".join(self[x] for x in (x.strip() for x in key.split(",")))
-
-        if self._allow_missing and key not in self._entries:
-            return f"{{{key}}}"
-        else:
-            return self._entries[key]
-
-    def _getslice(self, s):
-        start = s.start
-        stop = s.stop
-
-        keys = list(self._entries.keys())
-
-        if isinstance(s.start, int) or s.start is None and isinstance(s.stop, int):
-            slc = s
-
-        else:
-            if s.start is None:
-                start = 0
-            else:
-                start = keys.index(s.start)
-
-            if s.stop is None:
-                stop = len(self) + 1
-            else:
-                stop = keys.index(s.stop) + 1
-
-            slc = slice(start, stop, s.step)
-
-        subset = {k: self._entries[k] for k in keys[slc]}
-        return subset
-
-    def __setitem__(self, key, value):
-        self._entries[key] = value
-
-    def __iter__(self):
-        return iter(self._entries)
-
-    def __len__(self):
-        return len(self._entries)
-
-    def _items(self):
-        yield from self._entries.items()
-
-    def __dir__(self):
-        return list(self.keys()) + super().__dir__()
-
-    def _update(self, *args, **kwargs):
-        self._entries.update(*args, **kwargs)
-
-    def __getattr__(self, attr):
-        if attr in self._entries:
-            out = self._entries[attr]
-            if self._recursive and isinstance(out, dict):
-                out = type(self)(out)
-            return out
-        else:
-            try:
-                return self.__getattribute__(attr)
-            except AttributeError as err:
-                # If Python is run with -OO, it will strip docstrings and our lookup
-                # from self._entries will fail. We check for __debug__, which is actually
-                # set to False by -O (it is True for normal execution).
-                # But we only want to see an error when building the docs;
-                # not something users should see, so this slight inconsistency is fine.
-                if __debug__:
-                    raise err
-                else:
-                    pass
-
-    def __repr__(self):
-        return f"{self.__class__.__name__}({repr(self._entries)})"
-
-    @classmethod
-    def _from_dict(cls, params, max_level=1, level=0, recursive=True):
-        # to hide level parameter
-        out = cls(recursive=recursive)
-        for k in params:
-            v = params[k]
-            if isinstance(v, dict) and level < max_level:
-                v = cls._from_dict(
-                    v, max_level=max_level, level=level + 1, recursive=recursive
-                )
-            out[k] = v
-        return out
-
-    @classmethod
-    def from_dict(cls, params, max_level=1, recursive=True):
-        """
-        Create AttributeDict recursively for nested dictionaries.
-
-        To be used in cases where need to apply AttibuteDict to parameters
-        passed with ``func(**params)``.
-
-
-        Parameters
-        ----------
-        params : mapping
-            Mapping to apply cls to.
-        max_level : int, default=1
-            How deep to apply cls to.
-        recursive : bool, default=True
-            ``recursive`` parameter of resulting object.
-
-        Returns
-        -------
-        AttributeDict
-
-        Examples
-        --------
-        >>> d = {"a": "p0", "b": {"c": {"d": "d0"}}}
-        >>> AttributeDict.from_dict(d, max_level=1)
-        AttributeDict({'a': 'p0', 'b': AttributeDict({'c': {'d': 'd0'}})})
-
-        >>> AttributeDict.from_dict(d, max_level=2)
-        AttributeDict({'a': 'p0', 'b': AttributeDict({'c': AttributeDict({'d': 'd0'})})})
-
-        """
-        return cls._from_dict(
-            params=params, max_level=max_level, level=0, recursive=recursive
-        )
-
-
-def _build_param_docstring(name, ptype, desc):
+def _build_param_docstring(name: str, ptype: str, desc: str | Sequence[str]) -> str:
     """
     Create multiline documentation of single name, type, desc.
 
     Parameters
     ----------
     ==========
     name : str
@@ -332,27 +107,26 @@
 
     if len(desc) > 0:
         desc = "\n    ".join(desc)
         s += f"\n    {desc}"
     return s
 
 
-def _params_to_string(params, key_char="|"):
+def _params_to_string(params, key_char: str = "|") -> str | dict[str, Any]:
     """
     Parse list of Parameters objects to string
 
     Examples
     --------
-    >>> from module_utilities.docscrape import Parameter
+    >>> from module_utilities.docfiller import Parameter
     >>> p = Parameter(name="a", type="int", desc=["A parameter"])
-    >>> out = _parse_params_to_string(p)
+    >>> out = _params_to_string(p)
     >>> print(out["a"])
     a : int
         A parameter
-
     """
 
     if len(params) == 0:
         return ""
 
     if isinstance(params, Parameter):
         params = [params]
@@ -372,15 +146,17 @@
             key = name
 
         out[key] = _build_param_docstring(name=name, ptype=p.type, desc=p.desc)
 
     return out
 
 
-def parse_docstring(func_or_doc, key_char="|", expand=True):
+def _parse_docstring(
+    func_or_doc: Callable | str, key_char: str = "|", expand: bool = True
+):
     """
     Parse numpy style docstring from function or string to dictionary.
 
     Parameters
     ----------
     func_or_doc : callable or str
         If function, extract docstring from function.
@@ -412,15 +188,15 @@
     ...
     ... Returns
     ... -------
     ... output : float
     ...     an output
     ... '''
 
-    >>> p = parse_docstring(doc_string)
+    >>> p = _parse_docstring(doc_string)
     >>> print(p["parameters"]["x"])
     x : int
         x parameter
     >>> print(p["parameters"]["y_alt"])
     y : float
         y parameter
     >>> print(p["returns"]["output"])
@@ -454,28 +230,56 @@
                 "References",
                 "Examples",
             ]
         }
     return parsed
 
 
-def dedent_recursive(data):
-    """Dedent nested mapping of strings."""
-    out = type(data)()
+def dedent_recursive(data: Mapping[str, Any]) -> dict[str, Any]:
+    """
+    Dedent nested mapping of strings.
+
+    Parameters
+    ----------
+    data : dict
+
+    Returns
+    -------
+    output : object
+        Same type of ``data``, with dedented values
+
+    Examples
+    --------
+    >>> data = {
+    ...     'a': {'value' : '''
+    ...      a : int
+    ...          A thing
+    ...      '''}}
+    >>> print(data['a']['value'])
+    <BLANKLINE>
+         a : int
+             A thing
+    <BLANKLINE>
+    >>> data = dedent_recursive(data)
+    >>> print(data['a']['value'])
+    a : int
+        A thing
+    """
+    out = {}
     for k in data:
         v = data[k]
         if isinstance(v, str):
             v = dedent(v).strip()
         else:
             v = dedent_recursive(v)
         out[k] = v
     return out
 
 
-def _recursive_keys(data):
+def _recursive_keys(data) -> list[str]:
     keys = []
     for k, v in data.items():
         if isinstance(v, dict):
             key_list = [f"{k}.{x}" for x in _recursive_keys(v)]
         elif isinstance(v, str):
             key_list = [k]
         else:
@@ -484,77 +288,86 @@
         keys.extend(key_list)
 
     return keys
 
 
 class DocFiller:
     """
+    Class to handle doc filling.
 
     Parameters
     ----------
     func_or_doc : callable or str
         Docstring to parse.  If callable, extract from function signature.
     key_char : str, default='|'
         Optional string to split name into key/name pair.
     """
 
-    def __init__(self, params=None):
+    def __init__(self, params: Mapping[str, Any] | None = None) -> None:
         if params is None:
-            params = {}
-        self.data = params
+            self.data = {}
+        elif isinstance(params, dict):
+            self.data = params
+        else:
+            self.data = dict(params)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"{self.__class__.__name__}({repr(self.data)})"
 
-    def __getitem__(self, key):
+    def __getitem__(self, key: str):
         val = self.data[key]
         if isinstance(val, dict):
             return type(self)(val)
         else:
             return val
 
-    def dedent(self):
+    def dedent(self) -> DocFiller:
+        """Recursively dedent params"""
         return type(self)(dedent_recursive(self.data))
 
     @cached.meth
-    def keys(self):
+    def keys(self) -> list[str]:
+        """List of keys"""
         return _recursive_keys(self.data)
 
-    def assign_combined_key(self, new_key, keys):
+    def assign_combined_key(self, new_key: str, keys: Sequence[str]):
         """Combine multiple keys into single key"""
-
         data = self.data.copy()
-
         data[new_key] = "\n".join([self.data[k] for k in keys])
         return type(self)(data)
 
     @classmethod
-    def concat(cls, *args, **kwargs):
+    def concat(
+        cls,
+        *args: Mapping[str, Any] | DocFiller,
+        **kwargs: Mapping[str, Any] | DocFiller,
+    ) -> DocFiller:
         """
         Create new object from multiple DocFiller or dict objects.
 
         Parameters
         ----------
         *args : dict or Docfiller objects
-        **kwargs : named dict or Docfiller objects
+        **kwargs : dict or Docfiller objects
+            The passed name will be used as the top level.
 
         Returns
         -------
         DocFiller
             combined DocFiller object.
 
         Notes
         -----
         Use unnamed `args` to pass in underlying data.
         Use names ``kwargs`` to add namespace.
         """
 
         # create
 
-        data = {}
+        data: dict[str, Any] = {}
 
         def _update_data(x):
             if isinstance(x, DocFiller):
                 # x = x.params
                 x = x.data
             data.update(**x)
 
@@ -564,77 +377,99 @@
         for k, v in kwargs.items():
             if isinstance(v, cls):
                 kwargs[k] = v.data
 
         _update_data(kwargs)
         return cls(data)
 
-    def append(self, *args, **kwargs):
+    def append(
+        self,
+        *args: Mapping[str, Any] | DocFiller,
+        **kwargs: Mapping[str, Any] | DocFiller,
+    ) -> DocFiller:
         """Calls ``concat`` method with ``self`` as first argument."""
-
         return type(self).concat(self, *args, **kwargs)
 
-    def insert_level(self, name):
+    def insert_level(self, name: str) -> DocFiller:
         """Insert a level/namespace."""
         return type(self)({name: self.data})
 
-    def levels_to_top(self, *names):
+    def levels_to_top(self, *names: str) -> DocFiller:
         """Make a level top level accessible"""
 
         params = dict(self.data)
         for name in names:
-            for k, v in self.data[name].items():
-                params[k] = v
+            d = self.data[name]
+            if isinstance(d, str):
+                raise ValueError(f"level {name} is not a dict")
+            else:
+                for k, v in self.data[name].items():
+                    params[k] = v
         return type(self)(params)
 
-    def rename_levels(self, **kws):
+    def rename_levels(self, **kws: str) -> DocFiller:
+        """Rename a keys at top level."""
         params = {}
         for k, v in self.data.items():
             key = kws.get(k, k)
             params[key] = v
         return type(self)(params)
 
     @cached.prop
-    def params(self):
+    def params(self) -> AttributeDict:
+        """An AttributeDict view of parameters."""
         return AttributeDict.from_dict(self.data, max_level=1)
 
     @cached.prop
-    def default_decorator(self) -> Callable[[F], F]:
-        return docfiller(**self.params)
+    def _default_decorator(self) -> Callable[[F], F]:
+        return doc_decorate(**self.params)
 
-    def update(self, *args, **kwargs):
+    def update(self, *args, **kwargs) -> DocFiller:
+        """Update parameters"""
         data = self.data.copy()
         data.update(*args, **kwargs)
         return type(self)(params=data)
 
-    def __call__(self, *templates, **params) -> Callable[[F], F]:
+    def decorate(self, func: F) -> F:
+        """
+        Default decorator.
+
+        This uses `self.params` and the decorated funciton docstring as a template.
+        """
+        return self._default_decorator(func)  # type: ignore
+
+    def __call__(self, *templates: Callable | str, **params) -> Callable[[F], F]:
         """
         General decorator.
 
         This should always be used in a callable manner.
 
         If want to call without any parameter use decorate()
+
+        Parameters
+        ----------
+        *templates : callable
+            docstrings to be used as templates.
+        **params
+            Extra parameters to be substituted.
         """
         ntemplates, nparams = len(templates), len(params)
 
         if ntemplates == nparams == 0:
-            return self.default_decorator
-        if nparams > 0:
-            params = AttributeDict.from_dict({**self.data, **params}, max_level=1)
-        else:
-            params = self.params
-        return docfiller(*templates, **params)
-
-    def dec(self, _target=None, **params) -> Callable[[F], F]:
-        """Special case of no templates."""
-
-        dec = self(**params)
-        if _target is not None:
-            dec = dec(_target)
-        return dec
+            return self.decorate
+        elif nparams == 0:
+            return doc_decorate(*templates, **self.params)
+        else:
+            return self.update(params)(*templates)
+
+        # if nparams > 0:
+        #     params = AttributeDict.from_dict({**self.data, **params}, max_level=1)
+        # else:
+        #     params = self.params
+        # return doc_decorate(*templates, **params)
 
     # NOTE: This is dangerous.
     # if you pass a function as a template, but forget to explicitly pass it,
     # you overwrite the docstring for that function.  Just really confusing
     # def dec(self, *funcs, docstrings=None, **params) -> Callable[[F], F]:
     #     """
     #     General decorator.
@@ -651,16 +486,15 @@
     #     nfuncs = len(funcs)
 
     #     if nfuncs == 0:
     #         func = None
     #     elif nfuncs == 1 and callable(funcs[0]):
     #         func = funcs[0]
     #     else:
-    #         func = None
-    #         raise ValueError("Must call with zero or one functions.  If trying to set docstrings, be explicit")
+    #         func = None    #         raise ValueError("Must call with zero or one functions.  If trying to set docstrings, be explicit")
 
     #     if docstrings is None:
     #         docstrings = ()
     #     elif callable(docstrings) or isinstance(docstrings, str):
     #         docstrings = (docstrings,)
 
     #     ndocstrings, nparams = (len(x) for x in (docstrings, params))
@@ -668,15 +502,15 @@
     #     if ndocstrings == nparams == 0:
     #         dec = self.default_decorator
     #     else:
     #         if nparams > 0:
     #             params = AttributeDict.from_dict({**self.data, **params}, max_level=1)
     #         else:
     #             params = self.params
-    #         dec = docfiller(*docstrings, **params)
+    #         dec = doc_decorate(*docstrings, **params)
 
     #     if func:
     #         dec = dec(func)
     #     return dec
 
     # def __call__(self, *funcs, docstrings=None, **params) -> Callable[[F], F]:
     #     """
@@ -685,26 +519,26 @@
     #     Does not handle templates.
     #     """
     #     return self.dec(*funcs, docstrings=docstrings, **params)
 
     @classmethod
     def from_dict(
         cls,
-        params,
-        namespace=None,
-        combine_keys=None,
-        keep_keys=True,
-        key_map=None,
-    ):
+        params: Mapping[str, Any],
+        namespace: str | None = None,
+        combine_keys: str | Sequence[str] | None = None,
+        keep_keys: bool | str | Sequence[str] = True,
+        key_map: Mapping[str, str] | Callable | None = None,
+    ) -> DocFiller:
         """
         Create a Docfiller instance from a dictionary.
 
         Parameters
         ----------
-        params : mapkping
+        params : mapping
         namespace : str, optional
             Top level namespace for DocFiller.
         combine_keys : str, sequence of str, mapping, optional.
             If str or sequence of str, Keys of ``params`` to at the top level.
             If mapping, should be of form {namespace: key(s)}
 
         keep_keys : str, sequence of str, bool
@@ -717,15 +551,15 @@
         Returns
         -------
         DocFiller
         """
         if not keep_keys:
             keep_keys = []
         elif keep_keys is True:
-            keep_keys = params.keys()
+            keep_keys = [k for k in params]
         elif isinstance(keep_keys, str):
             keep_keys = [keep_keys]
 
         if combine_keys:
             if isinstance(combine_keys, str):
                 combine_keys = [combine_keys]
 
@@ -741,43 +575,67 @@
 
             for k in combine_keys:
                 updated_params.update(**params[k])
 
         else:
             updated_params = {k: params[k] for k in keep_keys}
 
-        if key_map:
-            if not callable(key_map):
-                key_map = lambda x: key_map[x]
+        if key_map is not None:
+            if callable(key_map):
+                mapper = key_map
+            else:
+                mapper = lambda x: key_map[x]  # type: ignore
 
-            updated_params = {key_map(k): updated_params[k] for k in updated_params}
+            updated_params = {mapper(k): updated_params[k] for k in updated_params}
 
         if namespace:
             updated_params = {namespace: updated_params}
 
         return cls(params=updated_params)
 
     @classmethod
     def from_docstring(
         cls,
-        func_or_doc,
-        namespace=None,
-        combine_keys=None,
-        key_char="|",
-        keep_keys=True,
-        key_map=None,
-    ):
+        func_or_doc: Callable | str,
+        namespace: str | None = None,
+        combine_keys: str | Sequence[str] | None = None,
+        key_char: str = "|",
+        keep_keys: bool = True,
+        key_map: Mapping | Callable | None = None,
+    ) -> DocFiller:
         """
         Create a Docfiller instance from a function or docstring.
 
         Parameters
         ----------
-        func_or_doc
+        func_or_doc : str or callable
+            Docstring to parse to get parameters.
+        namespace : str, optional
+            Top level namespace for DocFiller.
+        combine_keys : str, sequence of str, mapping, optional.
+            If str or sequence of str, Keys of ``params`` to at the top level.
+            If mapping, should be of form {namespace: key(s)}
+        key_char : str, default="|"
+            Character to split names.  By default, for parameters, the key will be parsed from
+            The docstring. If you want to override this, you can use
+            `key | name : ....` in the definition (where `'|'` is the value of `key_char`).
+        keep_keys : str, sequence of str, bool
+            If False, then don't keep any keys at top level.  This is useful with the
+            ``combine_keys`` parameter.
+            If True, keep all keys, regardless of combine_keys.
+            If str or sequence of str, keep these keys in output.
+        key_map : mapping or callable
+            Function or mapping to new keys in resulting dict.
+
+        Returns
+        -------
+        DocFiller
+
         """
-        params = parse_docstring(
+        params = _parse_docstring(
             func_or_doc=func_or_doc, key_char=key_char, expand=True
         )
         return cls.from_dict(
             params=params,
             namespace=namespace,
             combine_keys=combine_keys,
             keep_keys=keep_keys,
```

### Comparing `module-utilities-0.0.1/src/module_utilities/external/docscrape.py` & `module-utilities-0.1.0/src/module_utilities/_docscrape.py`

 * *Files identical despite different names*

### Comparing `module-utilities-0.0.1/src/module_utilities.egg-info/PKG-INFO` & `module-utilities-0.1.0/src/module_utilities.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: module-utilities
-Version: 0.0.1
+Version: 0.1.0
 Summary: Collection of utilities to aid working with python modules.
 Home-page: https://github.com/wpk-nist-gov/module-utilities
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
 License: NIST license
 Project-URL: homepage, https://github.com/wpk-nist-gov/module-utilities
 Project-URL: documentation, https://pages.nist.gov/module-utilities/
 Keywords: module-utilities
@@ -101,17 +101,19 @@
 ```python
 import module_utilities
 
 ```
 
 <!-- end-docs -->
 
-## Documentation
+<!-- ## Documentation -->
 
+<!--
 See the [documentation][docs-link] for a look at `module-utilities` in action.
+-->
 
 ## License
 
 This is free software. See [LICENSE][license-link].
 
 ## Related work
 
@@ -131,18 +133,25 @@
 
 # Changelog
 
 Changelog for `module-utilities`
 
 ## Unreleased
 
-See the fragment files in [changelog.d](https://github.com/wpk-nist-gov/module-utilities)
+See the fragment files in
+[changelog.d](https://github.com/wpk-nist-gov/module-utilities)
 
 <!-- scriv-insert-here -->
 
+## v0.1.0 — 2023-05-01
+
+### Added
+
+- Add typing support. Passing mypy, pyright, pytype.
+
 This software was developed by employees of the National Institute of Standards
 and Technology (NIST), an agency of the Federal Government. Pursuant to title 17
 United States Code Section 105, works of NIST employees are not subject to
 copyright protection in the United States and are considered to be in the public
 domain. Permission to freely use, copy, modify, and distribute this software and
 its documentation without fee is hereby granted, provided that this notice and
 disclaimer of warranty appears in all copies.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `module-utilities-0.0.1/src/module_utilities.egg-info/SOURCES.txt` & `module-utilities-0.1.0/src/module_utilities.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -64,26 +64,32 @@
 environment/docs.yaml
 environment/lint-extras.yaml
 environment/lint.yaml
 environment/test-extras.yaml
 environment/test.yaml
 environment/tools.yaml
 examples/README.md
-examples/usage/demo.ipynb
+scripts/dist-conda.mk
+scripts/dist-pypi.mk
 scripts/docs-examples-symlinks.sh
+scripts/lint.mk
+scripts/run-prettier.sh
 scripts/tox-ipykernel-display-name.sh
 src/module_utilities/__init__.py
+src/module_utilities/_doc.py
+src/module_utilities/_docscrape.py
+src/module_utilities/_typing.py
+src/module_utilities/attributedict.py
 src/module_utilities/cached.py
 src/module_utilities/docfiller.py
+src/module_utilities/py.typed
 src/module_utilities.egg-info/PKG-INFO
 src/module_utilities.egg-info/SOURCES.txt
 src/module_utilities.egg-info/dependency_links.txt
 src/module_utilities.egg-info/not-zip-safe
 src/module_utilities.egg-info/requires.txt
 src/module_utilities.egg-info/top_level.txt
-src/module_utilities/external/__init__.py
-src/module_utilities/external/docscrape.py
 tests/__init__.py
 tests/conftest.py
 tests/test_cached.py
 tests/test_docfiller.py
 tests/test_module_utilities.py
```

### Comparing `module-utilities-0.0.1/tests/test_cached.py` & `module-utilities-0.1.0/tests/test_cached.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-import pytest
+from __future__ import annotations
+from typing import Any
 
+import pytest
 
 from module_utilities import cached
 
 
 class Baseclass:
-    def __init__(self, a, b):
+    def __init__(self, a, b) -> None:
         self.a = a
         self.b = b
 
-    def get_value(self):
+    def get_value(self) -> tuple[Any, ...]:
         return self.a, self.b
 
-    def get_xy(self, x, y):
+    def get_xy(self, x, y) -> tuple[Any, ...]:
         return self.get_value() + (x, y)
 
 
 def prop_test(obj, prop, value, key=None, docstring=None):
     """test a single property"""
     if key is None:
         key = prop
@@ -48,146 +50,177 @@
     # test is same
     assert getattr(obj, meth)(*args, **kws) is getattr(obj, meth)(*args, **kws)
 
     if docstring is not None:
         assert getattr(type(obj), meth).__doc__ == docstring
 
 
-def do_prop_test(x, key=None, docstring="a doc string", check_empty=True):
+def do_prop_test(x, key=None, docstring="a doc string", check_empty=True) -> None:
     if key is None:
         key = "prop"
 
     # nothing here
     if check_empty:
         assert not hasattr(x, "_cache") or len(x._cache) == 0
     prop_test(x, prop="prop", value=(1, 2), key=key, docstring=docstring)
 
-    assert tuple(x._cache.keys()) == (key,)
+    assert tuple(x._cache.keys()) == (key,)  # pytype: disable=attribute-error
 
     # change value
     x.a, x.b = 2, 4
 
     prop_test(x, prop="prop", value=(1, 2), key=key, docstring=docstring)
 
     # remove cache:
     del x._cache
     prop_test(x, prop="prop", value=(2, 4), key=key, docstring=docstring)
 
 
 def test_prop():
-    for dec in [cached.decorate, cached.prop]:
+    class test(Baseclass):
+        @cached.prop
+        def prop(self):
+            "a doc string"
+            return self.get_value()
 
-        class test(Baseclass):
-            @dec
-            def prop(self):
-                "a doc string"
-                return self.get_value()
+    do_prop_test(test(1, 2))
 
-        do_prop_test(test(1, 2))
 
-        class test(Baseclass):
-            @dec()
-            def prop(self):
-                "a doc string"
-                self._hello = 1
-                return self.get_value()
+def test_prop2():
+    class test(Baseclass):
+        @cached.prop()
+        def prop(self):
+            "a doc string"
+            self._hello = 1
+            return self.get_value()
 
-        do_prop_test(test(1, 2))
+    do_prop_test(test(1, 2))
 
-        class test(Baseclass):
-            @dec(key="there")
-            def prop(self):
-                "a doc string"
-                return self.get_value()
 
-        do_prop_test(test(1, 2), key="there")
+def test_prop3() -> None:
+    class test(Baseclass):
+        @cached.prop(key="there")
+        def prop(self):
+            "a doc string"
+            return self.get_value()
+
+    do_prop_test(test(1, 2), key="there")
+
+
+def test_prop4():
+    class test(Baseclass):
+        @cached.decorate()
+        def prop(self):
+            "a doc string"
+            self._hello = 1
+            return self.get_value()
 
+    do_prop_test(test(1, 2))
 
-def do_meth_test(x, key=None, docstring="a doc string", check_empty=True):
+
+def test_prop5():
+    class test(Baseclass):
+        @cached.decorate(key="there")
+        def prop(self):
+            "a doc string"
+            return self.get_value()
+
+    do_prop_test(test(1, 2), key="there")
+
+
+def do_meth_test(x, key=None, docstring="a doc string", check_empty=True) -> None:
     if key is None:
         key = "meth"
 
-    key_tot = (key, (3, 4), frozenset())
+    key_tot: tuple[str, tuple[Any, ...], frozenset[Any]] = (key, (3, 4), frozenset())
 
     target = (1, 2, 3, 4)
     if check_empty:
         assert not hasattr(x, "_cache") or len(x._cache) == 0
     meth_test(x, "meth", target, args=(3, 4), key=key_tot, docstring=docstring)
 
-    assert tuple(x._cache.keys()) == (key_tot,)
+    assert tuple(x._cache.keys()) == (key_tot,)  # pytype: disable=attribute-error
 
     # change value
     x.a = 2
     x.b = 4
 
     meth_test(x, "meth", target, args=(3, 4), key=key_tot, docstring=docstring)
-    assert tuple(x._cache.keys()) == (key_tot,)
+    assert tuple(x._cache.keys()) == (key_tot,)  # pytype: disable=attribute-error
 
     # remove cache:
     del x._cache
     target = (2, 4, 3, 4)
     meth_test(x, "meth", target, args=(3, 4), key=key_tot, docstring=docstring)
-    assert tuple(x._cache.keys()) == (key_tot,)
+    assert tuple(x._cache.keys()) == (key_tot,)  # pytype: disable=attribute-error
 
     # getting write signature
     del x._cache
     meth_test(x, "meth", target, kws=dict(x=3, y=4), key=key_tot, docstring=docstring)
-    assert tuple(x._cache.keys()) == (key_tot,)
+    assert tuple(x._cache.keys()) == (key_tot,)  # pytype: disable=attribute-error
 
     del x._cache
     meth_test(x, "meth", target, kws=dict(y=4, x=3), key=key_tot, docstring=docstring)
-    assert tuple(x._cache.keys()) == (key_tot,)
+    assert tuple(x._cache.keys()) == (key_tot,)  # pytype: disable=attribute-error
 
     del x._cache
     meth_test(
         x, "meth", target, args=(3,), kws=dict(y=4), key=key_tot, docstring=docstring
     )
-    assert tuple(x._cache.keys()) == (key_tot,)
+    assert tuple(x._cache.keys()) == (key_tot,)  # pytype: disable=attribute-error
 
 
-def test_meth():
+def test_meth() -> None:
     class test(Baseclass):
         @cached.decorate(as_property=False)
         def meth(self, x, y):
             "a doc string"
             return self.get_xy(x, y)
 
     do_meth_test(test(1, 2))
 
+
+def test_meth2() -> None:
     class test(Baseclass):
         @cached.meth
         def meth(self, x, y):
             "a doc string"
             return self.get_xy(x, y)
 
     do_meth_test(test(1, 2))
 
+
+def test_meth3() -> None:
     class test(Baseclass):
         @cached.meth()
         def meth(self, x, y):
             "a doc string"
             return self.get_xy(x, y)
 
     do_meth_test(test(1, 2))
 
+
+def test_meth4() -> None:
     class test(Baseclass):
         @cached.meth(key="there")
         def meth(self, x, y):
             "a doc string"
             return self.get_xy(x, y)
 
     do_meth_test(test(1, 2), key="there")
 
 
-def test_clear():
+def test_clear() -> None:
     class test(Baseclass):
         def __init__(self, a, b):
             self._a = a
             self._b = b
 
+            self._cache = {}
+
         @property
         def a(self):
             return self._a
 
         @a.setter
         @cached.clear
         def a(self, val):
@@ -205,26 +238,29 @@
         @cached.clear
         def clear_all(self):
             "a clear string"
             pass
 
         @property
         def aprop(self):
-            return self._aprop
-
-        @cached.prop
-        def test_prop(self):
-            return [2.0]
+            if hasattr(self, "_aprop"):
+                return self._aprop
+            else:
+                raise ValueError("must set aprop")
 
         @aprop.setter
         @cached.clear("prop", "test_prop")
         def aprop(self, val):
             self._aprop = val
 
         @cached.prop
+        def test_prop(self):
+            return [2.0]
+
+        @cached.prop
         def prop(self):
             "a doc string"
             return self.get_value()
 
         @cached.clear("meth")
         def clear_meth(self):
             pass
@@ -232,15 +268,15 @@
         @cached.meth
         def meth(self, x, y):
             "a doc string"
             return self.get_xy(x, y)
 
     x = test(1, 2)
     key_prop = "prop"
-    key_meth = ("meth", (3, 4), frozenset())
+    key_meth = ("meth", (3, 4), frozenset())  # type: ignore
     docstring = "a doc string"
     prop_test(x, prop="prop", value=(1, 2), key=key_prop, docstring=docstring)
     meth_test(
         x,
         meth="meth",
         value=(1, 2, 3, 4),
         args=(3, 4),
@@ -279,96 +315,109 @@
     assert key_prop not in x._cache
     assert "test_prop" not in x._cache
     assert key_meth in x._cache
 
     x.prop
     x.meth(3, 4)
     x.meth(5, 6)
-    key_meth2 = ("meth", (5, 6), frozenset())
+    key_meth2 = ("meth", (5, 6), frozenset())  # type: ignore
 
     assert key_prop in x._cache
     assert key_meth in x._cache
     assert key_meth2 in x._cache
 
     x.clear_meth()
     assert key_meth not in x._cache
     assert key_meth2 not in x._cache
     assert key_prop in x._cache
 
 
-def test_use_cache():
+def test_use_cache() -> None:
     class tmp:
         _use_cache = False
 
+        def __init__(self):
+            self._cache = {}
+
         @cached.prop(check_use_cache=True)
         def prop0(self):
             return [1, 2]
 
         @cached.prop
         def prop1(self):
             return [2, 3]
 
         @cached.decorate(check_use_cache=True)
         def prop2(self):
             return [1, 2]
 
-        @cached.decorate
+        @cached.decorate()
         def prop3(self):
             return [1, 2]
 
     x = tmp()
 
     for p in ["prop0", "prop2"]:
         assert getattr(x, p) is not getattr(x, p)
         assert not hasattr(x, "_cache") or p not in x._cache
 
     for p in ["prop1", "prop3"]:
         assert getattr(x, p) is getattr(x, p)
         assert p in x._cache
 
+
+def test_use_cache2() -> None:
     class tmp:
         _use_cache = True
 
+        def __init__(self):
+            self._cache = {}
+
         @cached.prop(check_use_cache=True)
         def prop0(self):
             return [1, 2]
 
         @cached.prop
         def prop1(self):
             return [2, 3]
 
         @cached.decorate(check_use_cache=True)
         def prop2(self):
             return [1, 2]
 
-        @cached.decorate
+        @cached.decorate()
         def prop3(self):
             return [1, 2]
 
     x = tmp()
 
     for p in ["prop0", "prop1", "prop2", "prop3"]:
         assert getattr(x, p) is getattr(x, p)
         assert p in x._cache
 
+
+def test_use_cache3() -> None:
     # if not have _use_cache parameter
     class tmp:
+        def __init__(self):
+            self._cache = {}
+
         @cached.prop(check_use_cache=True)
         def prop0(self):
             return [1, 2]
 
         @cached.prop
         def prop1(self):
             return [2, 3]
 
         @cached.decorate(check_use_cache=True)
         def prop2(self):
             return [1, 2]
 
-        @cached.decorate
+        @cached.decorate()
         def prop3(self):
             return [1, 2]
 
     x = tmp()
 
     for p in ["prop0", "prop2"]:
         assert getattr(x, p) is not getattr(x, p)
@@ -392,14 +441,16 @@
             return self.a, self.b
 
     x = test(1, 2)
 
     with pytest.raises(AttributeError):
         x.prop
 
+
+def test_error_with_slots2():
     class test:
         __slots__ = ["a", "b", "_cache"]
 
         def __init__(self, a, b):
             self.a = a
             self.b = b
```

### Comparing `module-utilities-0.0.1/tests/test_docfiller.py` & `module-utilities-0.1.0/tests/test_docfiller.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,13 @@
+from __future__ import annotations
 from textwrap import dedent
 
+# from typing import TYPE_CHECKING
+# from typing_extensions import reveal_type
+
 import pytest
 
 from module_utilities import docfiller
 from module_utilities.docfiller import DocFiller, dedent_recursive
 
 # just testing on doc routine:
 
@@ -46,15 +50,15 @@
     output : float
     """
     )
 
 
 @pytest.fixture
 def template(params):
-    @docfiller.doc(**params)
+    @docfiller.doc_decorate(**params)
     def func(*args, **kwargs):
         """
         {summary}
 
         Parameters
         ----------
         {a}
@@ -74,23 +78,23 @@
 
 
 def test_doc(template, expected):
     assert template.__doc__ == expected
 
 
 def test_doc_from_template(template, params, expected):
-    @docfiller.doc(template, **params)
+    @docfiller.doc_decorate(template, **params)
     def func():
         pass
 
     assert func.__doc__ == expected
 
 
 def test_doc_from_docstring(template, params, expected):
-    @docfiller.doc(template.__doc__, **params)
+    @docfiller.doc_decorate(template.__doc__, **params)
     def func():
         pass
 
     assert func.__doc__ == expected
 
 
 def test_DocFiller(template, params, expected):
@@ -103,35 +107,35 @@
     assert func.__doc__ == expected
 
     # @d.update(**params).dec(template)
     # NOTE: can't do above in python 3.8
     dd = d.update(**params)
 
     @dd(template)
-    def func():
+    def func2():
         pass
 
-    assert func.__doc__ == expected
+    assert func2.__doc__ == expected
 
     # @d.update(params).dec(template)
     dd = d.update(params)
 
     @dd(template)
-    def func():
+    def func3():
         pass
 
-    assert func.__doc__ == expected
+    assert func3.__doc__ == expected
 
     d = docfiller.DocFiller.from_dict(params)
 
     @d(template)
-    def func():
+    def func4():
         pass
 
-    assert func.__doc__ == expected
+    assert func4.__doc__ == expected
 
 
 def test_DocFiller_docstring():
     docstring = """
     A summary line
 
     An extended summary
@@ -151,58 +155,36 @@
         A floating return
     """
 
     d = DocFiller.from_docstring(docstring, combine_keys="parameters")
 
     docstring = dedent(docstring)
 
-    for dec in [d, d.dec]:
-
-        @dec()
-        def function():
-            """
-            {summary}
-
-            {extended_summary}
-
-            Parameters
-            ----------
-            {a}
-            {b}
-            {c}
-
-            Returns
-            -------
-            {returns[:]}
-            """
-
-        assert docstring == function.__doc__
-
-        # @dec
-        # def function():
-        #     """
-        #     {summary}
+    @d()
+    def function():
+        """
+        {summary}
 
-        #     {extended_summary}
+        {extended_summary}
 
-        #     Parameters
-        #     ----------
-        #     {a}
-        #     {b}
-        #     {c}
+        Parameters
+        ----------
+        {a}
+        {b}
+        {c}
 
-        #     Returns
-        #     -------
-        #     {returns[:]}
-        #     """
+        Returns
+        -------
+        {returns[:]}
+        """
 
-        # assert docstring == function.__doc__
+    assert docstring == function.__doc__
 
-    @d.dec
-    def function():
+    @d.decorate
+    def function2():
         """
         {summary}
 
         {extended_summary}
 
         Parameters
         ----------
@@ -211,30 +193,29 @@
         {c}
 
         Returns
         -------
         {returns[:]}
         """
 
-    assert docstring == function.__doc__
-
+    assert docstring == function2.__doc__
     # update
     dd = d.update(
         hello="""
         hello : int
             Hello param
         """,
         there="""
         there : float
             There param
         """,
     ).dedent()
 
-    @dd()
-    def function():
+    @dd.decorate
+    def function3():
         """
         {summary}
 
         Parameters
         ----------
         {a}
         {b}
@@ -254,15 +235,15 @@
         B parameter
     hello : int
         Hello param
     there : float
         There param
     """
     )
-    assert function.__doc__ == expected
+    assert function3.__doc__ == expected
 
     d2 = docfiller.DocFiller.from_docstring(
         """
         Parameters
         ----------
         hello : int
             Hello param
@@ -271,22 +252,22 @@
         """,
         combine_keys="parameters",
         keep_keys=False,
     )
 
     dd = d.append(d2)
 
-    @dd(function)
-    def func2():
+    @dd(function3)
+    def function4():
         pass
 
-    assert func2.__doc__ == expected
+    assert function4.__doc__ == expected
 
 
-def test_DocFiller_namespace():
+def test_DocFiller_namespace() -> None:
     s0 = """
     Parameters
     ----------
     a : int
         A param
     b : int
         B param
@@ -334,15 +315,15 @@
         out : float
             OO param
         """
     )
 
     for dd in [dd0, dd1]:
 
-        @dd.dec
+        @dd.decorate
         def func():
             """
             Parameters
             ----------
             {a.parameters.a}
             {b.parameters.b_alt}
 
@@ -364,23 +345,25 @@
         d1.rename_levels(parameters="p", returns="r")
         .levels_to_top("p", "r")
         .insert_level("b")
     )
 
     dd = dd0.append(dd1)
 
-    @dd()
-    def func():
+    @dd.decorate
+    def func2(a: int, b: int) -> tuple[int, int]:
         """
         Parameters
         ----------
         {a.p.a}
         {b.p.b_alt}
 
         Returns
         -------
         {b.r.out}
         """
 
-        pass
+        return a, b
 
-    assert func.__doc__ == expected
+    assert func2.__doc__ == expected
+
+    assert func2(1, 1) == (1, 1)
```

