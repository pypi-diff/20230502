# Comparing `tmp/cmomy-0.3.0.tar.gz` & `tmp/cmomy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmomy-0.3.0.tar", last modified: Mon Apr 24 20:51:25 2023, max compression
+gzip compressed data, was "cmomy-0.4.0.tar", last modified: Tue May  2 05:03:51 2023, max compression
```

## Comparing `cmomy-0.3.0.tar` & `cmomy-0.4.0.tar`

### file list

```diff
@@ -1,144 +1,141 @@
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.185413 cmomy-0.3.0/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1475 2023-04-24 20:47:28.000000 cmomy-0.3.0/.cruft.json
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      513 2023-04-24 20:47:28.000000 cmomy-0.3.0/.editorconfig
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       31 2023-01-25 16:37:02.000000 cmomy-0.3.0/.gitattributes
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1313 2023-04-24 20:47:28.000000 cmomy-0.3.0/.gitignore
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      161 2023-04-24 20:47:28.000000 cmomy-0.3.0/.markdownlint.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3421 2023-04-24 20:47:28.000000 cmomy-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       20 2023-04-24 20:47:28.000000 cmomy-0.3.0/.prettierrc.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      122 2023-04-24 20:47:28.000000 cmomy-0.3.0/AUTHORS.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2171 2023-04-24 20:47:28.000000 cmomy-0.3.0/CHANGELOG.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     8861 2023-04-24 20:47:28.000000 cmomy-0.3.0/CONTRIBUTING.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1645 2023-03-15 19:07:26.000000 cmomy-0.3.0/LICENSE
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      258 2023-04-24 20:47:28.000000 cmomy-0.3.0/MANIFEST.in
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    10386 2023-04-24 20:47:28.000000 cmomy-0.3.0/Makefile
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9353 2023-04-24 20:51:25.185770 cmomy-0.3.0/PKG-INFO
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4599 2023-04-24 20:47:28.000000 cmomy-0.3.0/README.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.133343 cmomy-0.3.0/changelog.d/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      584 2023-04-24 20:47:28.000000 cmomy-0.3.0/changelog.d/20230424_125230_william.krekelberg_update_cruft.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       64 2023-04-24 20:47:28.000000 cmomy-0.3.0/changelog.d/README.txt
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.134000 cmomy-0.3.0/changelog.d/templates/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.135152 cmomy-0.3.0/changelog.d/templates/auto-changelog/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      213 2023-04-24 20:47:28.000000 cmomy-0.3.0/changelog.d/templates/auto-changelog/macros.jinja2
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      774 2023-04-24 20:47:28.000000 cmomy-0.3.0/changelog.d/templates/auto-changelog/template.jinja2
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      269 2023-04-24 20:47:28.000000 cmomy-0.3.0/changelog.d/templates/new_fragment.md.j2
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      652 2023-01-25 16:37:02.000000 cmomy-0.3.0/commands.sh
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      366 2023-01-25 16:37:02.000000 cmomy-0.3.0/conftest.py
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.140030 cmomy-0.3.0/docs/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1201 2023-04-06 00:58:31.000000 cmomy-0.3.0/docs/Makefile
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.117786 cmomy-0.3.0/docs/_static/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.140432 cmomy-0.3.0/docs/_static/css/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2937 2023-04-24 20:47:28.000000 cmomy-0.3.0/docs/_static/css/nist-combined.css
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.141219 cmomy-0.3.0/docs/_static/js/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      767 2023-04-24 20:47:28.000000 cmomy-0.3.0/docs/_static/js/leave_notice.js
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      706 2023-04-24 20:47:28.000000 cmomy-0.3.0/docs/_static/js/nist-header-footer.js
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.142747 cmomy-0.3.0/docs/_templates/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.144824 cmomy-0.3.0/docs/_templates/autodocsumm/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      289 2023-03-22 20:26:04.000000 cmomy-0.3.0/docs/_templates/autodocsumm/class-noindex.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      249 2023-03-22 20:26:04.000000 cmomy-0.3.0/docs/_templates/autodocsumm/class.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      405 2023-03-22 20:26:04.000000 cmomy-0.3.0/docs/_templates/autodocsumm/module-inherit.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      424 2023-03-22 20:26:04.000000 cmomy-0.3.0/docs/_templates/autodocsumm/module-noindex.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      374 2023-03-22 20:26:04.000000 cmomy-0.3.0/docs/_templates/autodocsumm/module.rst
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.146053 cmomy-0.3.0/docs/_templates/autosummary/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      106 2023-03-22 20:26:04.000000 cmomy-0.3.0/docs/_templates/autosummary/base.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1255 2023-03-22 20:26:04.000000 cmomy-0.3.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1119 2023-03-22 20:26:04.000000 cmomy-0.3.0/docs/_templates/autosummary/module.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1418 2023-03-22 20:26:04.000000 cmomy-0.3.0/docs/_templates/class-individual-pages.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1177 2023-03-22 20:26:04.000000 cmomy-0.3.0/docs/_templates/module-custom.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1071 2023-03-22 20:26:04.000000 cmomy-0.3.0/docs/_templates/module-single.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1179 2023-03-22 20:26:04.000000 cmomy-0.3.0/docs/_templates/module-template.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       69 2023-04-24 20:47:28.000000 cmomy-0.3.0/docs/authors.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       71 2023-04-24 20:47:28.000000 cmomy-0.3.0/docs/changelog.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    14554 2023-04-24 20:47:28.000000 cmomy-0.3.0/docs/conf.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       74 2023-04-24 20:47:28.000000 cmomy-0.3.0/docs/contributing.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      891 2023-04-24 20:47:28.000000 cmomy-0.3.0/docs/example_for_readme.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.146870 cmomy-0.3.0/docs/examples/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      887 2023-04-24 20:47:28.000000 cmomy-0.3.0/docs/examples/create-symlinks.sh
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       84 2023-04-24 20:47:28.000000 cmomy-0.3.0/docs/examples/index.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.147996 cmomy-0.3.0/docs/examples/usage/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)   156774 2023-04-24 20:47:28.000000 cmomy-0.3.0/docs/examples/usage/motivation.ipynb
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)   295212 2023-04-24 20:47:28.000000 cmomy-0.3.0/docs/examples/usage/usage_notebook.ipynb
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      224 2023-04-24 20:47:28.000000 cmomy-0.3.0/docs/index.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      860 2023-04-24 20:47:28.000000 cmomy-0.3.0/docs/installation.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       40 2023-04-24 20:47:28.000000 cmomy-0.3.0/docs/license.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      767 2023-03-15 18:41:43.000000 cmomy-0.3.0/docs/make.bat
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      169 2023-04-24 20:47:28.000000 cmomy-0.3.0/docs/navigation.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.149995 cmomy-0.3.0/docs/reference/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      158 2023-04-06 00:58:31.000000 cmomy-0.3.0/docs/reference/api-baseclasses.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      122 2023-04-06 00:58:31.000000 cmomy-0.3.0/docs/reference/api-modules.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      398 2023-04-06 00:58:31.000000 cmomy-0.3.0/docs/reference/api-public.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      194 2023-04-24 20:47:28.000000 cmomy-0.3.0/docs/reference/index.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      491 2023-04-21 20:37:24.000000 cmomy-0.3.0/docs/spelling_wordlist.txt
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.154283 cmomy-0.3.0/environment/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      967 2023-04-24 20:47:28.000000 cmomy-0.3.0/environment/dev-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      282 2023-04-24 20:47:28.000000 cmomy-0.3.0/environment/dev.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      108 2023-04-24 20:47:28.000000 cmomy-0.3.0/environment/dist-conda.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       79 2023-04-24 20:47:28.000000 cmomy-0.3.0/environment/dist-pypi.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      640 2023-04-24 20:47:28.000000 cmomy-0.3.0/environment/docs-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      435 2023-04-24 20:47:28.000000 cmomy-0.3.0/environment/docs.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       53 2023-04-24 20:47:28.000000 cmomy-0.3.0/environment/lint-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      175 2023-04-24 20:47:28.000000 cmomy-0.3.0/environment/lint.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       25 2023-04-24 20:47:28.000000 cmomy-0.3.0/environment/test-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      166 2023-04-24 20:47:28.000000 cmomy-0.3.0/environment/test.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      299 2023-04-24 20:47:28.000000 cmomy-0.3.0/environment/tools.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      159 2023-04-24 20:47:28.000000 cmomy-0.3.0/environment.yaml
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.154676 cmomy-0.3.0/examples/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      222 2023-04-24 20:47:28.000000 cmomy-0.3.0/examples/README.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.157041 cmomy-0.3.0/examples/archived/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    70967 2023-04-24 20:47:28.000000 cmomy-0.3.0/examples/archived/bootstrap.ipynb
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)   136974 2023-04-24 20:47:28.000000 cmomy-0.3.0/examples/archived/central_moments.ipynb
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    44856 2023-04-24 20:47:28.000000 cmomy-0.3.0/examples/archived/example_usage.ipynb
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    12217 2023-04-24 20:47:28.000000 cmomy-0.3.0/examples/archived/parallel_test.ipynb
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    58117 2023-04-24 20:47:28.000000 cmomy-0.3.0/examples/archived/test_accumulator.ipynb
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.158099 cmomy-0.3.0/examples/usage/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)   156774 2023-04-24 20:47:28.000000 cmomy-0.3.0/examples/usage/motivation.ipynb
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)   295212 2023-04-24 20:47:28.000000 cmomy-0.3.0/examples/usage/usage_notebook.ipynb
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5218 2023-04-24 20:47:28.000000 cmomy-0.3.0/pyproject.toml
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.159245 cmomy-0.3.0/scripts/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1099 2023-04-24 20:47:28.000000 cmomy-0.3.0/scripts/docs-examples-symlinks.sh
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      489 2023-04-24 20:47:28.000000 cmomy-0.3.0/scripts/tox-ipykernel-display-name.sh
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      286 2023-04-24 20:51:25.186801 cmomy-0.3.0/setup.cfg
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      323 2023-04-24 20:47:28.000000 cmomy-0.3.0/setup.py
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.121475 cmomy-0.3.0/src/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.169553 cmomy-0.3.0/src/cmomy/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1045 2023-03-29 00:12:57.000000 cmomy-0.3.0/src/cmomy/__init__.py
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.177109 cmomy-0.3.0/src/cmomy/_docfiller/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       23 2023-04-06 00:58:31.000000 cmomy-0.3.0/src/cmomy/_docfiller/__init__.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    19686 2023-04-06 00:58:31.000000 cmomy-0.3.0/src/cmomy/_docfiller/docfiller.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    23537 2023-04-06 00:58:31.000000 cmomy-0.3.0/src/cmomy/_docfiller/docscrape.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3354 2023-04-24 20:47:28.000000 cmomy-0.3.0/src/cmomy/_docstrings.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2736 2023-04-24 20:47:28.000000 cmomy-0.3.0/src/cmomy/_formatting.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     6463 2023-03-22 20:26:04.000000 cmomy-0.3.0/src/cmomy/_resample.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2311 2023-01-25 16:37:02.000000 cmomy-0.3.0/src/cmomy/_testing.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      658 2023-03-22 20:26:04.000000 cmomy-0.3.0/src/cmomy/_typing.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    39709 2023-04-24 20:47:28.000000 cmomy-0.3.0/src/cmomy/abstract_central.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5598 2023-04-06 00:58:31.000000 cmomy-0.3.0/src/cmomy/cached_decorators.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    51565 2023-04-24 20:47:28.000000 cmomy-0.3.0/src/cmomy/central.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      967 2023-01-25 16:37:02.000000 cmomy-0.3.0/src/cmomy/compile.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    10911 2023-04-24 20:47:28.000000 cmomy-0.3.0/src/cmomy/convert.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1834 2023-04-06 00:58:31.000000 cmomy-0.3.0/src/cmomy/options.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3122 2023-04-06 00:58:31.000000 cmomy-0.3.0/src/cmomy/pusher_interface.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    14250 2023-01-25 16:37:02.000000 cmomy-0.3.0/src/cmomy/pushers.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-03-22 20:26:04.000000 cmomy-0.3.0/src/cmomy/py.typed
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    13795 2023-04-24 20:47:28.000000 cmomy-0.3.0/src/cmomy/resample.py
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.184783 cmomy-0.3.0/src/cmomy/tests/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-01-25 16:37:02.000000 cmomy-0.3.0/src/cmomy/tests/__init__.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    11871 2023-03-22 20:26:04.000000 cmomy-0.3.0/src/cmomy/tests/conftest.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5427 2023-03-22 20:26:04.000000 cmomy-0.3.0/src/cmomy/tests/test_central.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9554 2023-03-22 20:26:04.000000 cmomy-0.3.0/src/cmomy/tests/test_central_2.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1085 2023-01-25 16:37:02.000000 cmomy-0.3.0/src/cmomy/tests/test_convert.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4085 2023-03-22 20:26:04.000000 cmomy-0.3.0/src/cmomy/tests/test_resample.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2354 2023-03-22 20:26:04.000000 cmomy-0.3.0/src/cmomy/tests/test_stability.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2682 2023-03-22 20:26:04.000000 cmomy-0.3.0/src/cmomy/tests/test_verify.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     6183 2023-03-22 20:26:04.000000 cmomy-0.3.0/src/cmomy/tests/test_xcentral.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4879 2023-03-22 20:26:04.000000 cmomy-0.3.0/src/cmomy/tests/test_xcentral_constructors.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3249 2023-04-24 20:47:28.000000 cmomy-0.3.0/src/cmomy/utils.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    62270 2023-04-24 20:47:28.000000 cmomy-0.3.0/src/cmomy/xcentral.py
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-24 20:51:25.174623 cmomy-0.3.0/src/cmomy.egg-info/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9353 2023-04-24 20:51:25.000000 cmomy-0.3.0/src/cmomy.egg-info/PKG-INFO
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3235 2023-04-24 20:51:25.000000 cmomy-0.3.0/src/cmomy.egg-info/SOURCES.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-04-24 20:51:25.000000 cmomy-0.3.0/src/cmomy.egg-info/dependency_links.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-04-06 00:42:47.000000 cmomy-0.3.0/src/cmomy.egg-info/not-zip-safe
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       91 2023-04-24 20:51:25.000000 cmomy-0.3.0/src/cmomy.egg-info/requires.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        6 2023-04-24 20:51:25.000000 cmomy-0.3.0/src/cmomy.egg-info/top_level.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4507 2023-04-24 20:47:28.000000 cmomy-0.3.0/tox.ini
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.710538 cmomy-0.4.0/
+-rw-r--r--   0 wpk      (42033)    36681     1475 2023-05-02 05:01:33.000000 cmomy-0.4.0/.cruft.json
+-rw-r--r--   0 wpk      (42033)    36681      540 2023-05-02 04:51:37.000000 cmomy-0.4.0/.editorconfig
+-rw-r--r--   0 wpk      (42033)    36681       31 2023-01-25 16:37:02.000000 cmomy-0.4.0/.gitattributes
+-rw-r--r--   0 wpk      (42033)    36681     1324 2023-05-02 04:51:37.000000 cmomy-0.4.0/.gitignore
+-rw-r--r--   0 wpk      (42033)    36681      161 2023-04-24 20:47:28.000000 cmomy-0.4.0/.markdownlint.yaml
+-rw-r--r--   0 wpk      (42033)    36681     3651 2023-05-02 04:51:37.000000 cmomy-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 wpk      (42033)    36681       20 2023-04-24 20:47:28.000000 cmomy-0.4.0/.prettierrc.yaml
+-rw-r--r--   0 wpk      (42033)    36681      122 2023-04-24 20:47:28.000000 cmomy-0.4.0/AUTHORS.md
+-rw-r--r--   0 wpk      (42033)    36681     2667 2023-05-02 04:51:37.000000 cmomy-0.4.0/CHANGELOG.md
+-rw-r--r--   0 wpk      (42033)    36681     9153 2023-05-02 04:51:37.000000 cmomy-0.4.0/CONTRIBUTING.md
+-rw-r--r--   0 wpk      (42033)    36681     1645 2023-03-15 19:07:26.000000 cmomy-0.4.0/LICENSE
+-rw-r--r--   0 wpk      (42033)    36681      258 2023-04-24 20:47:28.000000 cmomy-0.4.0/MANIFEST.in
+-rw-r--r--   0 wpk      (42033)    36681    11187 2023-05-02 04:51:37.000000 cmomy-0.4.0/Makefile
+-rw-r--r--   0 wpk      (42033)    36681     9851 2023-05-02 05:03:51.711032 cmomy-0.4.0/PKG-INFO
+-rw-r--r--   0 wpk      (42033)    36681     4601 2023-05-02 04:51:37.000000 cmomy-0.4.0/README.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.613503 cmomy-0.4.0/changelog.d/
+-rw-r--r--   0 wpk      (42033)    36681       64 2023-04-24 20:47:28.000000 cmomy-0.4.0/changelog.d/README.txt
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.614426 cmomy-0.4.0/changelog.d/templates/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.616035 cmomy-0.4.0/changelog.d/templates/auto-changelog/
+-rw-r--r--   0 wpk      (42033)    36681      213 2023-04-24 20:47:28.000000 cmomy-0.4.0/changelog.d/templates/auto-changelog/macros.jinja2
+-rw-r--r--   0 wpk      (42033)    36681      774 2023-04-24 20:47:28.000000 cmomy-0.4.0/changelog.d/templates/auto-changelog/template.jinja2
+-rw-r--r--   0 wpk      (42033)    36681      269 2023-04-24 20:47:28.000000 cmomy-0.4.0/changelog.d/templates/new_fragment.md.j2
+-rw-r--r--   0 wpk      (42033)    36681      366 2023-01-25 16:37:02.000000 cmomy-0.4.0/conftest.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.625606 cmomy-0.4.0/docs/
+-rw-r--r--   0 wpk      (42033)    36681     1401 2023-05-02 05:02:56.000000 cmomy-0.4.0/docs/Makefile
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.597134 cmomy-0.4.0/docs/_static/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.627106 cmomy-0.4.0/docs/_static/css/
+-rw-r--r--   0 wpk      (42033)    36681     2937 2023-04-24 20:47:28.000000 cmomy-0.4.0/docs/_static/css/nist-combined.css
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.629581 cmomy-0.4.0/docs/_static/js/
+-rw-r--r--   0 wpk      (42033)    36681      767 2023-04-24 20:47:28.000000 cmomy-0.4.0/docs/_static/js/leave_notice.js
+-rw-r--r--   0 wpk      (42033)    36681      706 2023-04-24 20:47:28.000000 cmomy-0.4.0/docs/_static/js/nist-header-footer.js
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.633907 cmomy-0.4.0/docs/_templates/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.639177 cmomy-0.4.0/docs/_templates/autodocsumm/
+-rw-r--r--   0 wpk      (42033)    36681      289 2023-03-22 20:26:04.000000 cmomy-0.4.0/docs/_templates/autodocsumm/class-noindex.rst
+-rw-r--r--   0 wpk      (42033)    36681      249 2023-03-22 20:26:04.000000 cmomy-0.4.0/docs/_templates/autodocsumm/class.rst
+-rw-r--r--   0 wpk      (42033)    36681      405 2023-03-22 20:26:04.000000 cmomy-0.4.0/docs/_templates/autodocsumm/module-inherit.rst
+-rw-r--r--   0 wpk      (42033)    36681      424 2023-03-22 20:26:04.000000 cmomy-0.4.0/docs/_templates/autodocsumm/module-noindex.rst
+-rw-r--r--   0 wpk      (42033)    36681      374 2023-03-22 20:26:04.000000 cmomy-0.4.0/docs/_templates/autodocsumm/module.rst
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.641878 cmomy-0.4.0/docs/_templates/autosummary/
+-rw-r--r--   0 wpk      (42033)    36681      106 2023-03-22 20:26:04.000000 cmomy-0.4.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 wpk      (42033)    36681     1255 2023-03-22 20:26:04.000000 cmomy-0.4.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 wpk      (42033)    36681     1119 2023-03-22 20:26:04.000000 cmomy-0.4.0/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 wpk      (42033)    36681     1418 2023-03-22 20:26:04.000000 cmomy-0.4.0/docs/_templates/class-individual-pages.rst
+-rw-r--r--   0 wpk      (42033)    36681     1177 2023-03-22 20:26:04.000000 cmomy-0.4.0/docs/_templates/module-custom.rst
+-rw-r--r--   0 wpk      (42033)    36681     1071 2023-03-22 20:26:04.000000 cmomy-0.4.0/docs/_templates/module-single.rst
+-rw-r--r--   0 wpk      (42033)    36681     1179 2023-03-22 20:26:04.000000 cmomy-0.4.0/docs/_templates/module-template.rst
+-rw-r--r--   0 wpk      (42033)    36681       69 2023-04-24 20:47:28.000000 cmomy-0.4.0/docs/authors.md
+-rw-r--r--   0 wpk      (42033)    36681       71 2023-04-24 20:47:28.000000 cmomy-0.4.0/docs/changelog.md
+-rw-r--r--   0 wpk      (42033)    36681    14595 2023-05-02 04:51:37.000000 cmomy-0.4.0/docs/conf.py
+-rw-r--r--   0 wpk      (42033)    36681       74 2023-04-24 20:47:28.000000 cmomy-0.4.0/docs/contributing.md
+-rw-r--r--   0 wpk      (42033)    36681      891 2023-04-24 20:47:28.000000 cmomy-0.4.0/docs/example_for_readme.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.644531 cmomy-0.4.0/docs/examples/
+-rw-r--r--   0 wpk      (42033)    36681      887 2023-04-24 20:47:28.000000 cmomy-0.4.0/docs/examples/create-symlinks.sh
+-rw-r--r--   0 wpk      (42033)    36681       84 2023-04-24 20:47:28.000000 cmomy-0.4.0/docs/examples/index.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.647120 cmomy-0.4.0/docs/examples/usage/
+-rw-r--r--   0 wpk      (42033)    36681   156774 2023-04-24 20:47:28.000000 cmomy-0.4.0/docs/examples/usage/motivation.ipynb
+-rw-r--r--   0 wpk      (42033)    36681   295212 2023-04-24 20:47:28.000000 cmomy-0.4.0/docs/examples/usage/usage_notebook.ipynb
+-rw-r--r--   0 wpk      (42033)    36681      224 2023-04-24 20:47:28.000000 cmomy-0.4.0/docs/index.md
+-rw-r--r--   0 wpk      (42033)    36681      860 2023-04-24 20:47:28.000000 cmomy-0.4.0/docs/installation.md
+-rw-r--r--   0 wpk      (42033)    36681       40 2023-04-24 20:47:28.000000 cmomy-0.4.0/docs/license.md
+-rw-r--r--   0 wpk      (42033)    36681      767 2023-03-15 18:41:43.000000 cmomy-0.4.0/docs/make.bat
+-rw-r--r--   0 wpk      (42033)    36681      169 2023-04-24 20:47:28.000000 cmomy-0.4.0/docs/navigation.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.651859 cmomy-0.4.0/docs/reference/
+-rw-r--r--   0 wpk      (42033)    36681      158 2023-04-06 00:58:31.000000 cmomy-0.4.0/docs/reference/api-baseclasses.rst
+-rw-r--r--   0 wpk      (42033)    36681      122 2023-04-06 00:58:31.000000 cmomy-0.4.0/docs/reference/api-modules.rst
+-rw-r--r--   0 wpk      (42033)    36681      398 2023-04-06 00:58:31.000000 cmomy-0.4.0/docs/reference/api-public.rst
+-rw-r--r--   0 wpk      (42033)    36681      194 2023-04-24 20:47:28.000000 cmomy-0.4.0/docs/reference/index.md
+-rw-r--r--   0 wpk      (42033)    36681      491 2023-04-21 20:37:24.000000 cmomy-0.4.0/docs/spelling_wordlist.txt
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.663443 cmomy-0.4.0/environment/
+-rw-r--r--   0 wpk      (42033)    36681      967 2023-04-24 20:47:28.000000 cmomy-0.4.0/environment/dev-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      310 2023-05-02 04:51:37.000000 cmomy-0.4.0/environment/dev.yaml
+-rw-r--r--   0 wpk      (42033)    36681      108 2023-04-24 20:47:28.000000 cmomy-0.4.0/environment/dist-conda.yaml
+-rw-r--r--   0 wpk      (42033)    36681       79 2023-04-24 20:47:28.000000 cmomy-0.4.0/environment/dist-pypi.yaml
+-rw-r--r--   0 wpk      (42033)    36681      640 2023-04-24 20:47:28.000000 cmomy-0.4.0/environment/docs-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      463 2023-05-02 04:51:37.000000 cmomy-0.4.0/environment/docs.yaml
+-rw-r--r--   0 wpk      (42033)    36681       53 2023-04-24 20:47:28.000000 cmomy-0.4.0/environment/lint-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      203 2023-05-02 04:51:37.000000 cmomy-0.4.0/environment/lint.yaml
+-rw-r--r--   0 wpk      (42033)    36681       25 2023-04-24 20:47:28.000000 cmomy-0.4.0/environment/test-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      194 2023-05-02 04:51:37.000000 cmomy-0.4.0/environment/test.yaml
+-rw-r--r--   0 wpk      (42033)    36681      299 2023-04-24 20:47:28.000000 cmomy-0.4.0/environment/tools.yaml
+-rw-r--r--   0 wpk      (42033)    36681      187 2023-05-02 04:51:37.000000 cmomy-0.4.0/environment.yaml
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.664364 cmomy-0.4.0/examples/
+-rw-r--r--   0 wpk      (42033)    36681      222 2023-04-24 20:47:28.000000 cmomy-0.4.0/examples/README.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.670757 cmomy-0.4.0/examples/archived/
+-rw-r--r--   0 wpk      (42033)    36681    70967 2023-04-24 20:47:28.000000 cmomy-0.4.0/examples/archived/bootstrap.ipynb
+-rw-r--r--   0 wpk      (42033)    36681   136974 2023-04-24 20:47:28.000000 cmomy-0.4.0/examples/archived/central_moments.ipynb
+-rw-r--r--   0 wpk      (42033)    36681    44856 2023-04-24 20:47:28.000000 cmomy-0.4.0/examples/archived/example_usage.ipynb
+-rw-r--r--   0 wpk      (42033)    36681    12217 2023-04-24 20:47:28.000000 cmomy-0.4.0/examples/archived/parallel_test.ipynb
+-rw-r--r--   0 wpk      (42033)    36681    58117 2023-04-24 20:47:28.000000 cmomy-0.4.0/examples/archived/test_accumulator.ipynb
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.673055 cmomy-0.4.0/examples/usage/
+-rw-r--r--   0 wpk      (42033)    36681   156774 2023-04-24 20:47:28.000000 cmomy-0.4.0/examples/usage/motivation.ipynb
+-rw-r--r--   0 wpk      (42033)    36681   295212 2023-04-24 20:47:28.000000 cmomy-0.4.0/examples/usage/usage_notebook.ipynb
+-rw-r--r--   0 wpk      (42033)    36681     6118 2023-05-02 04:51:37.000000 cmomy-0.4.0/pyproject.toml
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.678736 cmomy-0.4.0/scripts/
+-rw-r--r--   0 wpk      (42033)    36681      392 2023-05-02 04:51:37.000000 cmomy-0.4.0/scripts/dist-conda.mk
+-rw-r--r--   0 wpk      (42033)    36681      312 2023-05-02 04:51:37.000000 cmomy-0.4.0/scripts/dist-pypi.mk
+-rw-r--r--   0 wpk      (42033)    36681     1099 2023-04-24 20:47:28.000000 cmomy-0.4.0/scripts/docs-examples-symlinks.sh
+-rw-r--r--   0 wpk      (42033)    36681      266 2023-05-02 04:51:37.000000 cmomy-0.4.0/scripts/lint.mk
+-rw-r--r--   0 wpk      (42033)    36681       91 2023-05-02 04:51:37.000000 cmomy-0.4.0/scripts/run-prettier.sh
+-rw-r--r--   0 wpk      (42033)    36681      489 2023-04-24 20:47:28.000000 cmomy-0.4.0/scripts/tox-ipykernel-display-name.sh
+-rw-r--r--   0 wpk      (42033)    36681      286 2023-05-02 05:03:51.712585 cmomy-0.4.0/setup.cfg
+-rw-r--r--   0 wpk      (42033)    36681      323 2023-04-24 20:47:28.000000 cmomy-0.4.0/setup.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.600818 cmomy-0.4.0/src/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.694921 cmomy-0.4.0/src/cmomy/
+-rw-r--r--   0 wpk      (42033)    36681     1045 2023-03-29 00:12:57.000000 cmomy-0.4.0/src/cmomy/__init__.py
+-rw-r--r--   0 wpk      (42033)    36681     2736 2023-04-24 20:47:28.000000 cmomy-0.4.0/src/cmomy/_formatting.py
+-rw-r--r--   0 wpk      (42033)    36681     6463 2023-03-22 20:26:04.000000 cmomy-0.4.0/src/cmomy/_resample.py
+-rw-r--r--   0 wpk      (42033)    36681     2311 2023-01-25 16:37:02.000000 cmomy-0.4.0/src/cmomy/_testing.py
+-rw-r--r--   0 wpk      (42033)    36681      658 2023-03-22 20:26:04.000000 cmomy-0.4.0/src/cmomy/_typing.py
+-rw-r--r--   0 wpk      (42033)    36681    39729 2023-05-02 04:51:37.000000 cmomy-0.4.0/src/cmomy/abstract_central.py
+-rw-r--r--   0 wpk      (42033)    36681    51582 2023-05-02 04:51:37.000000 cmomy-0.4.0/src/cmomy/central.py
+-rw-r--r--   0 wpk      (42033)    36681      967 2023-01-25 16:37:02.000000 cmomy-0.4.0/src/cmomy/compile.py
+-rw-r--r--   0 wpk      (42033)    36681    10920 2023-05-02 04:51:37.000000 cmomy-0.4.0/src/cmomy/convert.py
+-rw-r--r--   0 wpk      (42033)    36681     3338 2023-05-02 04:51:37.000000 cmomy-0.4.0/src/cmomy/docstrings.py
+-rw-r--r--   0 wpk      (42033)    36681     1834 2023-04-06 00:58:31.000000 cmomy-0.4.0/src/cmomy/options.py
+-rw-r--r--   0 wpk      (42033)    36681     3122 2023-04-06 00:58:31.000000 cmomy-0.4.0/src/cmomy/pusher_interface.py
+-rw-r--r--   0 wpk      (42033)    36681    14250 2023-01-25 16:37:02.000000 cmomy-0.4.0/src/cmomy/pushers.py
+-rw-r--r--   0 wpk      (42033)    36681        0 2023-03-22 20:26:04.000000 cmomy-0.4.0/src/cmomy/py.typed
+-rw-r--r--   0 wpk      (42033)    36681    13795 2023-04-24 20:47:28.000000 cmomy-0.4.0/src/cmomy/resample.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.709666 cmomy-0.4.0/src/cmomy/tests/
+-rw-r--r--   0 wpk      (42033)    36681        0 2023-01-25 16:37:02.000000 cmomy-0.4.0/src/cmomy/tests/__init__.py
+-rw-r--r--   0 wpk      (42033)    36681    11913 2023-05-02 04:51:37.000000 cmomy-0.4.0/src/cmomy/tests/conftest.py
+-rw-r--r--   0 wpk      (42033)    36681     5427 2023-03-22 20:26:04.000000 cmomy-0.4.0/src/cmomy/tests/test_central.py
+-rw-r--r--   0 wpk      (42033)    36681     9455 2023-05-02 04:51:37.000000 cmomy-0.4.0/src/cmomy/tests/test_central_2.py
+-rw-r--r--   0 wpk      (42033)    36681     1085 2023-01-25 16:37:02.000000 cmomy-0.4.0/src/cmomy/tests/test_convert.py
+-rw-r--r--   0 wpk      (42033)    36681     4085 2023-03-22 20:26:04.000000 cmomy-0.4.0/src/cmomy/tests/test_resample.py
+-rw-r--r--   0 wpk      (42033)    36681     2354 2023-03-22 20:26:04.000000 cmomy-0.4.0/src/cmomy/tests/test_stability.py
+-rw-r--r--   0 wpk      (42033)    36681     2682 2023-03-22 20:26:04.000000 cmomy-0.4.0/src/cmomy/tests/test_verify.py
+-rw-r--r--   0 wpk      (42033)    36681     6183 2023-03-22 20:26:04.000000 cmomy-0.4.0/src/cmomy/tests/test_xcentral.py
+-rw-r--r--   0 wpk      (42033)    36681     4879 2023-03-22 20:26:04.000000 cmomy-0.4.0/src/cmomy/tests/test_xcentral_constructors.py
+-rw-r--r--   0 wpk      (42033)    36681     3190 2023-05-02 04:51:37.000000 cmomy-0.4.0/src/cmomy/utils.py
+-rw-r--r--   0 wpk      (42033)    36681    62294 2023-05-02 04:51:37.000000 cmomy-0.4.0/src/cmomy/xcentral.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-05-02 05:03:51.700780 cmomy-0.4.0/src/cmomy.egg-info/
+-rw-r--r--   0 wpk      (42033)    36681     9851 2023-05-02 05:03:51.000000 cmomy-0.4.0/src/cmomy.egg-info/PKG-INFO
+-rw-r--r--   0 wpk      (42033)    36681     3110 2023-05-02 05:03:51.000000 cmomy-0.4.0/src/cmomy.egg-info/SOURCES.txt
+-rw-r--r--   0 wpk      (42033)    36681        1 2023-05-02 05:03:51.000000 cmomy-0.4.0/src/cmomy.egg-info/dependency_links.txt
+-rw-r--r--   0 wpk      (42033)    36681        1 2023-04-06 00:42:47.000000 cmomy-0.4.0/src/cmomy.egg-info/not-zip-safe
+-rw-r--r--   0 wpk      (42033)    36681      113 2023-05-02 05:03:51.000000 cmomy-0.4.0/src/cmomy.egg-info/requires.txt
+-rw-r--r--   0 wpk      (42033)    36681        6 2023-05-02 05:03:51.000000 cmomy-0.4.0/src/cmomy.egg-info/top_level.txt
+-rw-r--r--   0 wpk      (42033)    36681     3704 2023-05-02 04:51:37.000000 cmomy-0.4.0/tox.ini
```

### Comparing `cmomy-0.3.0/.cruft.json` & `cmomy-0.4.0/.cruft.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'commit'": "'38e14cd6d21fdc444081dcb1e34c15d0ebdc3683'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": "feature/markdown",
-    "commit": "cdd6b53c60c026675336bf1250935194b2610fb9",
+    "commit": "38e14cd6d21fdc444081dcb1e34c15d0ebdc3683",
     "context": {
         "cookiecutter": {
             "_copy_without_render": [
                 "*.html",
                 "docs/_templates/*.rst",
                 "docs/_templates/autosummary/*.rst",
                 "docs/_templates/autodocsumm/*.rst",
```

### Comparing `cmomy-0.3.0/.editorconfig` & `cmomy-0.4.0/.editorconfig`

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

### Comparing `cmomy-0.3.0/.gitignore` & `cmomy-0.4.0/.gitignore`

 * *Files 10% similar despite different names*

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
@@ -105,8 +104,9 @@
 # IDE settings
 .vscode/
 pyrightconfig.json
 .autoenv.zsh
 .autoenv_leave.zsh
 /docs/**/generated/
 /monkeytype.sqlite3
-/dist-conda/
+/dist-conda/*
+!/dist-conda/Makefile
```

### Comparing `cmomy-0.3.0/.pre-commit-config.yaml` & `cmomy-0.4.0/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,20 @@
     rev: "v3.0.0-alpha.6"
     hooks:
       - id: prettier
         stages: [commit]
         additional_dependencies:
           - prettier-plugin-toml
         exclude: ^docs/example_for_readme.md
+  #** markdown
+  - repo: https://github.com/DavidAnson/markdownlint-cli2
+    rev: v0.6.0
+    hooks:
+      - id: markdownlint-cli2
+        args: ["--style prettier"]
   #* Linting
   - repo: https://github.com/charliermarsh/ruff-pre-commit
     # Ruff version.
     rev: "v0.0.261"
     hooks:
       - id: ruff
   - repo: https://github.com/psf/black
@@ -72,14 +78,24 @@
         args: ["-e", "lint-mypy"]
         language: system
         pass_filenames: false
         # additional_dependencies: [tox]
         types: [python]
         require_serial: true
         stages: [manual]
+      - id: pyright
+        name: pyright
+        entry: pyright
+        args: []
+        language: system
+        pass_filenames: true
+        # additional_dependencies: [tox]
+        types: [python]
+        require_serial: true
+        stages: [manual]
   # isort, pyupgrade, flake8 defer to ruff
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
         stages: [manual]
   - repo: https://github.com/asottile/pyupgrade
@@ -114,14 +130,7 @@
     rev: v2.2.4
     hooks:
       - id: codespell
         types_or: [python, rst, markdown, cython, c]
         additional_dependencies: [tomli]
         args: [-I, docs/spelling_wordlist.txt]
         stages: [manual]
-  #** markdown
-  - repo: https://github.com/DavidAnson/markdownlint-cli2
-    rev: v0.6.0
-    hooks:
-      - id: markdownlint-cli2
-        stages: [manual]
-        args: ["--style prettier"]
```

### Comparing `cmomy-0.3.0/CONTRIBUTING.md` & `cmomy-0.4.0/CONTRIBUTING.md`

 * *Files 9% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 [tox-conda]: https://github.com/tox-dev/tox-conda
 [cruft]: https://github.com/cruft/cruft
 [conda-merge]: https://github.com/amitbeka/conda-merge
 [git-flow]: https://github.com/nvie/gitflow
 [scriv]: https://github.com/nedbat/scriv
 [conventional-style]: https://www.conventionalcommits.org/en/v1.0.0/
 [commitizen]: https://github.com/commitizen-tools/commitizen
-[nb-conda-kernels]: https://github.com/Anaconda-Platform/nb_conda_kernels
+[nb_conda_kernels]: https://github.com/Anaconda-Platform/nb_conda_kernels
 
 This project uses a host of tools to (hopefully) make development easier. We
 recommend installing some of these tools system wide. For this, we recommend
 using either [pipx] or [condax]. We mostly use conda/condax, but the choice is
 yours. For conda, we recommend actually using [mamba]. Alternatively, you can
 setup `conda` to use the faster `mamba` solver. See [here][conda-fast-setup] for
 details.
@@ -98,162 +98,163 @@
 conda env update -n {env-name} environment/tools.yaml
 ```
 
 ### Getting the repo
 
 Ready to contribute? Here's how to set up `cmomy` for local development.
 
-1.  Fork the `cmomy` repo on GitHub.
+- Fork the `cmomy` repo on GitHub.
 
-1.  Clone your fork locally:
+- Clone your fork locally:
 
-    ```bash
-    git clone git@github.com:your_name_here/cmomy.git
-    ```
-
-    If the repo includes submodules, you can add them either with the initial
-    close using:
-
-    ```bash
-    git clone --recursive-submodules git@github.com:your_name_here/cmomy.git
-    ```
-
-    or after the clone using
+  ```bash
+  git clone git@github.com:your_name_here/cmomy.git
+  ```
 
-    ```bash
-    cd cmomy
-    git submodule update --init --recursive
-    ```
+  If the repo includes submodules, you can add them either with the initial
+  close using:
 
-1.  Create development environment. There are two options to create the
-    development environment.
+  ```bash
+  git clone --recursive-submodules git@github.com:your_name_here/cmomy.git
+  ```
 
-    a. The recommended method is to use tox by using either:
+  or after the clone using
 
-        ```bash
-        tox -e dev
-        ```
+  ```bash
+  cd cmomy
+  git submodule update --init --recursive
+  ```
 
-        or
+- Create development environment. There are two options to create the
+  development environment.
 
-        ```bash
-        make dev-env
-        ```
-        These create a development environment located at `.tox/dev`.
+  - The recommended method is to use tox by using either:
 
-        ```bash
-        make tox-ipykernel-display-name
-        ```
+    ```bash
+    tox -e dev
+    ```
 
-        This will add a meaningful display name for the kernel (assuming you're using
-        [nb-conda-kernels])
+    or
 
-    b. Alternativley, you can create centrally located conda environmentment
-    using the command:
+    ```bash
+    make dev-env
+    ```
 
-        ```bash
-        make mamba-dev
-        ```
+    These create a development environment located at `.tox/dev`.
 
-        This will create a conda environment 'cmomy-env' in the default location.
+    ```bash
+    make tox-ipykernel-display-name
+    ```
 
-        To install (an editable version) of the current package:
+    This will add a meaningful display name for the kernel (assuming you're
+    using [nb_conda_kernels])
 
-        ```bash
-        pip install -e . --no-deps
-        ```
+  - Alternativley, you can create centrally located conda environmentment using
+    the command:
 
-        or
+    ```bash
+    make mamba-dev
+    ```
 
-        ```bash
-        make install-dev
-        ```
+    This will create a conda environment 'cmomy-env' in the default location.
 
-1.  Initiate [pre-commit] with:
+    To install (an editable version) of the current package:
 
     ```bash
-    pre-commit install
+    pip install -e . --no-deps
     ```
 
-    To update the recipe, periodically run:
+    or
 
     ```bash
-    pre-commit autoupdate
+    make install-dev
     ```
 
-    If recipes change over time, you can clean up old installs with:
+- Initiate [pre-commit] with:
 
-    ```bash
-    pre-commit gc
-    ```
+  ```bash
+  pre-commit install
+  ```
 
-1.  Create a branch for local development:
+  To update the recipe, periodically run:
 
-    ```bash
-    git checkout -b name-of-your-bugfix-or-feature
-    ```
+  ```bash
+  pre-commit autoupdate
+  ```
 
-    Now you can make your changes locally. Alternatively, we recommend using
-    [git-flow].
+  If recipes change over time, you can clean up old installs with:
 
-1.  When you're done making changes, check that your changes pass the pre-commit
-    checks: tests.
+  ```bash
+  pre-commit gc
+  ```
 
-    ```bash
-    pre-commit run [--all-files]
-    ```
+- Create a branch for local development:
 
-    To run tests, use:
+  ```bash
+  git checkout -b name-of-your-bugfix-or-feature
+  ```
 
-    ```bash
-    pytest
-    ```
+  Now you can make your changes locally. Alternatively, we recommend using
+  [git-flow].
 
-    To test against multiple python versions, use tox:
+- When you're done making changes, check that your changes pass the pre-commit
+  checks: tests.
 
-    ```bash
-    tox
-    ```
+  ```bash
+  pre-commit run [--all-files]
+  ```
 
-    or using the `make`:
+  To run tests, use:
 
-    ```bash
-    make test-all
-    ```
+  ```bash
+  pytest
+  ```
 
-    Additionally, you should run the following:
+  To test against multiple python versions, use tox:
 
-    ```bash
-    make pre-commit-lint-markdown
-    make pre-commit-codespell
-    ```
+  ```bash
+  tox
+  ```
 
-1.  Create changelog fragment. See [scriv] for more info.
+  or using the `make`:
 
-    ```bash
-    scriv create --edit
-    ```
+  ```bash
+  make test-all
+  ```
 
-1.  Commit your changes and push your branch to GitHub:
+  Additionally, you should run the following:
 
-    ```bash
-    git add .
-    git commit -m "Your detailed description of your changes."
-    git push origin name-of-your-bugfix-or-feature
-    ```
+  ```bash
+  make pre-commit-lint-markdown
+  make pre-commit-codespell
+  ```
 
-    Note that the pre-commit hooks will force the commit message to be in the
-    [conventional sytle][conventional-style]. To assist this, you may want to
-    commit using [commitizen].
+- Create changelog fragment. See [scriv] for more info.
 
-    ```bash
-    cz commit
-    ```
+  ```bash
+  scriv create --edit
+  ```
+
+- Commit your changes and push your branch to GitHub:
+
+  ```bash
+  git add .
+  git commit -m "Your detailed description of your changes."
+  git push origin name-of-your-bugfix-or-feature
+  ```
 
-1.  Submit a pull request through the GitHub website.
+  Note that the pre-commit hooks will force the commit message to be in the
+  [conventional sytle][conventional-style]. To assist this, you may want to
+  commit using [commitizen].
+
+  ```bash
+  cz commit
+  ```
+
+- Submit a pull request through the GitHub website.
 
 ### Dependency management
 
 Dependencies need to be placed in a few locations, which depend on the nature of
 the dependency.
 
 - Package dependency: `environment.yaml` and `dependencies` section of
@@ -274,54 +275,58 @@
 
 which will rebuild all the needed yaml files.
 
 ## Pull Request Guidelines
 
 Before you submit a pull request, check that it meets these guidelines:
 
-1. The pull request should include tests.
-2. If the pull request adds functionality, the docs should be updated. Put your
-   new functionality into a function with a docstring, and add the feature to
-   the list in README.rst.
-3. The pull request should work for Python 3.8, 3.9, 3.10.
+- The pull request should include tests.
+- If the pull request adds functionality, the docs should be updated. Put your
+  new functionality into a function with a docstring, and add the feature to the
+  list in CHANGELOG.md. You should use [scriv] for this.
+- The pull request should work for Python 3.8, 3.9, 3.10.
 
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
@@ -333,15 +338,15 @@
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
 
@@ -360,9 +365,26 @@
 
 where `recipe` makes the conda recipe (using grayskull), and `build` makes the
 distro. This can be manually added to a channel.
 
 To test the created distributions, you can use one of:
 
 ```bash
+tox -e test-dist-[pypi, conda]-[local,remote]-py[38,39,...]
+```
+
+or
+
+```bash
 make test-dist-[pypi, conda]-[local,remote] py=[38, 39, 310]
 ```
+
+where one options in the brackets should be choosen.
+
+## Package version
+
+[setuptools_scm]: https://github.com/pypa/setuptools_scm
+
+Versioning is handled with [setuptools_scm].The pacakge version is set by the
+git tag. For convenience, you can override the version in the makefile (calling
+tox) by setting `version=v{major}.{minor}.{micro}`. This is useful for updating
+the docs, etc.
```

### Comparing `cmomy-0.3.0/LICENSE` & `cmomy-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/Makefile` & `cmomy-0.4.0/Makefile`

 * *Files 15% similar despite different names*

```diff
@@ -87,14 +87,17 @@
 	pre-commit run --all-files --hook-stage manual pyupgrade
 	pre-commit run --all-files --hook-stage manual nbqa-pyupgrade
 	pre-commit run --all-files --hook-stage manual nbqa-isort
 
 pre-commit-mypy: ## run mypy
 	pre-commit run --all-files --hook-stage manual mypy
 
+pre-commit-pyright: ## run pyright
+	pre-commit run --all-files --hook-stage manual pyright
+
 pre-commit-codespell: ## run codespell. Note that this imports allowed words from docs/spelling_wordlist.txt
 	pre-commit run --all-files --hook-stage manual codespell
 
 
 ################################################################################
 # my convenience functions
 ################################################################################
@@ -134,32 +137,31 @@
 	python -c 'import cmomy; print(cmomy.__version__)'
 
 version: version-scm version-import
 
 ################################################################################
 # Environment files
 ################################################################################
-
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
 
@@ -182,106 +184,118 @@
 
 mamba-dev-update: environment/dev.yaml ## update development environment
 	mamba env update -f $<
 
 ################################################################################
 # TOX
 ###############################################################################
-tox_posargs?=-v
-TOX=CONDA_EXE=mamba tox $(tox_posargs)
-
+tox_args?=-v
+version?=
+TOX=CONDA_EXE=mamba SETUPTOOLS_SCM_PRETEND_VERSION=$(version) tox $(tox_args)
 
 .PHONY: tox-ipykernel-display-name
 tox-ipykernel-display-name: ## Update display-name for any tox env with ipykernel
 	bash ./scripts/tox-ipykernel-display-name.sh cmomy
 
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

### Comparing `cmomy-0.3.0/PKG-INFO` & `cmomy-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmomy
-Version: 0.3.0
+Version: 0.4.0
 Summary: Central (co)moment calculation/manipulation
 Home-page: https://github.com/usnistgov/cmomy
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
 License: NIST license
 Project-URL: homepage, https://github.com/usnistgov/cmomy
 Project-URL: documentation, https://pages.nist.gov/cmomy/
 Keywords: cmomy
@@ -19,57 +19,58 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-# cmomy
-
-A Python package to calculate and manipulate Central (co)moments. The main
-features of `cmomy` are as follows:
-
-- [Numba][Numba] accelerated computation of central moments and co-moments
-- Routines to combine, and resample central moments.
-- Both [numpy][numpy] array-like and [xarray][xarray] DataArray interfaces to
-  Data.
-- Routines to convert between central and raw moments.
+<!-- markdownlint-disable MD041 -->
 
 [![Repo][repo-badge]][repo-link] [![Docs][docs-badge]][docs-link]
 [![PyPI license][license-badge]][license-link]
 [![PyPI version][pypi-badge]][pypi-link]
 [![Conda (channel only)][conda-badge]][conda-link]
 [![Code style: black][black-badge]][black-link]
 
+<!--
+  For more badges, see
+  https://shields.io/category/other
+  https://naereen.github.io/badges/
+  [pypi-badge]: https://badge.fury.io/py/cmomy
+-->
+
 [black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
-[black-link]: https://github.com/ambv/black
+[black-link]: https://github.com/psf/black
 [pypi-badge]: https://img.shields.io/pypi/v/cmomy
-
-<!-- [pypi-badge]: https://badge.fury.io/py/cmomy.svg -->
-
 [pypi-link]: https://pypi.org/project/cmomy
 [docs-badge]: https://img.shields.io/badge/docs-sphinx-informational
 [docs-link]: https://pages.nist.gov/cmomy/
 [repo-badge]: https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff
 [repo-link]: https://github.com/usnistgov/cmomy
 [conda-badge]: https://img.shields.io/conda/v/wpk-nist/cmomy
 [conda-link]: https://anaconda.org/wpk-nist/cmomy
+[license-badge]: https://img.shields.io/pypi/l/cmomy?color=informational
+[license-link]: https://github.com/usnistgov/cmomy/blob/main/LICENSE
+
+<!-- other links -->
+
 [numpy]: https://numpy.org
 [Numba]: https://numba.pydata.org/
 [xarray]: https://docs.xarray.dev/en/stable/
 
-<!-- Use total link so works from anywhere -->
+# cmomy
 
-[license-badge]: https://img.shields.io/pypi/l/cmomy?color=informational
-[license-link]: https://github.com/usnistgov/cmomy/blob/master/LICENSE
+A Python package to calculate and manipulate Central (co)moments. The main
+features of `cmomy` are as follows:
 
-<!-- For more badges see
-https://shields.io/category/other
-https://naereen.github.io/badges/
--->
+- [Numba][Numba] accelerated computation of central moments and co-moments
+- Routines to combine, and resample central moments.
+- Both [numpy][numpy] array-like and [xarray][xarray] DataArray interfaces to
+  Data.
+- Routines to convert between central and raw moments.
 
 ## Overview
 
 `cmomy` is an open source package to calculate central moments and co-moments in
 a numerical stable and direct way. Behind the scenes, `cmomy` makes use of
 [Numba][Numba] to rapidly calculate moments. A good introduction to the type of
 formulas used can be found
@@ -196,14 +197,36 @@
 
 ## Unreleased
 
 See the fragment files in [changelog.d](https://github.com/usnistgov/cmomy)
 
 <!-- scriv-insert-here -->
 
+## v0.4.0 — 2023-05-02
+
+### Added
+
+- Moved module `_docstrings_` to `docstrings`. This can be used by other
+  modules.
+
+### Changed
+
+- Update package layout
+- New linters via pre-commit
+- Development env now handled by tox
+
+- Now use `module-utilities` to handle caching and docfiller.
+
+[`v0.3.0...v0.4.0`](https://github.com/usnistgov/cmomy/compare/v0.3.0...v0.4.0)
+
+## v0.3.0 - 2023-04-24
+
+Full set of changes:
+[`v0.2.2...v0.3.0`](https://github.com/usnistgov/cmomy/compare/v0.2.2...v0.3.0)
+
 ## v0.2.2 - 2023-04-05
 
 Full set of changes:
 [`v0.2.1...v0.2.2`](https://github.com/usnistgov/cmomy/compare/v0.2.1...v0.2.2)
 
 ## v0.2.1 - 2023-04-05
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cmomy-0.3.0/README.md` & `cmomy-0.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,50 +1,51 @@
-# cmomy
-
-A Python package to calculate and manipulate Central (co)moments. The main
-features of `cmomy` are as follows:
-
-- [Numba][Numba] accelerated computation of central moments and co-moments
-- Routines to combine, and resample central moments.
-- Both [numpy][numpy] array-like and [xarray][xarray] DataArray interfaces to
-  Data.
-- Routines to convert between central and raw moments.
+<!-- markdownlint-disable MD041 -->
 
 [![Repo][repo-badge]][repo-link] [![Docs][docs-badge]][docs-link]
 [![PyPI license][license-badge]][license-link]
 [![PyPI version][pypi-badge]][pypi-link]
 [![Conda (channel only)][conda-badge]][conda-link]
 [![Code style: black][black-badge]][black-link]
 
+<!--
+  For more badges, see
+  https://shields.io/category/other
+  https://naereen.github.io/badges/
+  [pypi-badge]: https://badge.fury.io/py/cmomy
+-->
+
 [black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
-[black-link]: https://github.com/ambv/black
+[black-link]: https://github.com/psf/black
 [pypi-badge]: https://img.shields.io/pypi/v/cmomy
-
-<!-- [pypi-badge]: https://badge.fury.io/py/cmomy.svg -->
-
 [pypi-link]: https://pypi.org/project/cmomy
 [docs-badge]: https://img.shields.io/badge/docs-sphinx-informational
 [docs-link]: https://pages.nist.gov/cmomy/
 [repo-badge]: https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff
 [repo-link]: https://github.com/usnistgov/cmomy
 [conda-badge]: https://img.shields.io/conda/v/wpk-nist/cmomy
 [conda-link]: https://anaconda.org/wpk-nist/cmomy
+[license-badge]: https://img.shields.io/pypi/l/cmomy?color=informational
+[license-link]: https://github.com/usnistgov/cmomy/blob/main/LICENSE
+
+<!-- other links -->
+
 [numpy]: https://numpy.org
 [Numba]: https://numba.pydata.org/
 [xarray]: https://docs.xarray.dev/en/stable/
 
-<!-- Use total link so works from anywhere -->
+# cmomy
 
-[license-badge]: https://img.shields.io/pypi/l/cmomy?color=informational
-[license-link]: https://github.com/usnistgov/cmomy/blob/master/LICENSE
+A Python package to calculate and manipulate Central (co)moments. The main
+features of `cmomy` are as follows:
 
-<!-- For more badges see
-https://shields.io/category/other
-https://naereen.github.io/badges/
--->
+- [Numba][Numba] accelerated computation of central moments and co-moments
+- Routines to combine, and resample central moments.
+- Both [numpy][numpy] array-like and [xarray][xarray] DataArray interfaces to
+  Data.
+- Routines to convert between central and raw moments.
 
 ## Overview
 
 `cmomy` is an open source package to calculate central moments and co-moments in
 a numerical stable and direct way. Behind the scenes, `cmomy` makes use of
 [Numba][Numba] to rapidly calculate moments. A good introduction to the type of
 formulas used can be found
```

### Comparing `cmomy-0.3.0/changelog.d/templates/auto-changelog/template.jinja2` & `cmomy-0.4.0/changelog.d/templates/auto-changelog/template.jinja2`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/docs/Makefile` & `cmomy-0.4.0/docs/Makefile`

 * *Files 16% similar despite different names*

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
+release_args ?= -m "update docs" -b nist-pages
+release:
+	ghp-import -o -n $(release_args) $(BUILDDIR)/html
+
+command ?= @echo pass "command=..."
+command:
+	$(command)
```

### Comparing `cmomy-0.3.0/docs/_static/css/nist-combined.css` & `cmomy-0.4.0/docs/_static/css/nist-combined.css`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/docs/_static/js/leave_notice.js` & `cmomy-0.4.0/docs/_static/js/leave_notice.js`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/docs/_static/js/nist-header-footer.js` & `cmomy-0.4.0/docs/_static/js/nist-header-footer.js`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/docs/_templates/autosummary/class.rst` & `cmomy-0.4.0/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/docs/_templates/autosummary/module.rst` & `cmomy-0.4.0/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/docs/_templates/class-individual-pages.rst` & `cmomy-0.4.0/docs/_templates/class-individual-pages.rst`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/docs/_templates/module-custom.rst` & `cmomy-0.4.0/docs/_templates/module-custom.rst`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/docs/_templates/module-single.rst` & `cmomy-0.4.0/docs/_templates/module-single.rst`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/docs/_templates/module-template.rst` & `cmomy-0.4.0/docs/_templates/module-template.rst`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/docs/conf.py` & `cmomy-0.4.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -414,14 +414,16 @@
     "matplotlib": ("https://matplotlib.org/stable/", None),
     "dask": ("https://docs.dask.org/en/latest", None),
     "cftime": ("https://unidata.github.io/cftime", None),
     "sparse": ("https://sparse.pydata.org/en/latest/", None),
     "xarray": ("https://docs.xarray.dev/en/stable/", None),
 }
 
+linkcheck_ignore = ["https://doi.org/"]
+
 
 # based on numpy doc/source/conf.py
 def linkcode_resolve(domain, info):
     """Determine the URL corresponding to Python object"""
     import inspect
     from operator import attrgetter
```

### Comparing `cmomy-0.3.0/docs/example_for_readme.md` & `cmomy-0.4.0/docs/example_for_readme.md`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/docs/examples/create-symlinks.sh` & `cmomy-0.4.0/docs/examples/create-symlinks.sh`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/docs/examples/usage/motivation.ipynb` & `cmomy-0.4.0/docs/examples/usage/motivation.ipynb`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/docs/examples/usage/usage_notebook.ipynb` & `cmomy-0.4.0/docs/examples/usage/usage_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/docs/installation.md` & `cmomy-0.4.0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/docs/make.bat` & `cmomy-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/environment/dev-extras.yaml` & `cmomy-0.4.0/environment/dev-extras.yaml`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/environment/docs-extras.yaml` & `cmomy-0.4.0/environment/docs-extras.yaml`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/examples/archived/bootstrap.ipynb` & `cmomy-0.4.0/examples/archived/bootstrap.ipynb`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/examples/archived/central_moments.ipynb` & `cmomy-0.4.0/examples/archived/central_moments.ipynb`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/examples/archived/example_usage.ipynb` & `cmomy-0.4.0/examples/archived/example_usage.ipynb`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/examples/archived/parallel_test.ipynb` & `cmomy-0.4.0/examples/archived/parallel_test.ipynb`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/examples/archived/test_accumulator.ipynb` & `cmomy-0.4.0/examples/archived/test_accumulator.ipynb`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/examples/usage/motivation.ipynb` & `cmomy-0.4.0/examples/usage/motivation.ipynb`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/examples/usage/usage_notebook.ipynb` & `cmomy-0.4.0/examples/usage/usage_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/pyproject.toml` & `cmomy-0.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 requires-python = ">=3.8,<3.11"
 dependencies = [
     "numpy >= 1.20,<1.24",
     "numba >= 0.50",
     "xarray >= 0.16",
     "typing-extensions",
     "custom-inherit",
+    "module-utilities >= 0.1",
 ]
 
 [project.urls]
 homepage = "https://github.com/usnistgov/cmomy"
 documentation = "https://pages.nist.gov/cmomy/"
 
 [project.optional-dependencies]
@@ -64,15 +65,15 @@
 [tool.setuptools_scm]
 fallback_version = "999"
 
 [tool.aliases]
 test = "pytest"
 
 [tool.pytest.ini_options]
-addopts = "--verbose"
+addopts = "--verbose --doctest-modules --ignore-glob=**/_docfiller/*.py"
 testpaths = ["tests"]
 
 [tool.isort]
 profile = "black"
 skip_gitignore = true
 known_first_party = ["cmomy"]
 
@@ -228,15 +229,44 @@
 [tool.mypy]
 files = ["src/cmomy"]
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
+
+[tool.pyright]
+include = ["src", "tests"]
+exclude = ["**/__pycache__", ".tox/**", "**/.mypy_cache"]
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

### Comparing `cmomy-0.3.0/scripts/docs-examples-symlinks.sh` & `cmomy-0.4.0/scripts/docs-examples-symlinks.sh`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/src/cmomy/__init__.py` & `cmomy-0.4.0/src/cmomy/__init__.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/src/cmomy/_docstrings.py` & `cmomy-0.4.0/src/cmomy/docstrings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Common docstrings."""
-
 from __future__ import annotations
 
-from ._docfiller.docfiller import DocFiller
+from module_utilities.docfiller import DocFiller
 
-_docstring_cmomy = """\
+_docstrings = """\
 Parameters
 ----------
 copy : bool, optional
     If True, copy the data.  If False, attempt to use view.
 copy_kws : mapping, optional
     extra arguments to copy
 verify : bool, optional
@@ -76,15 +75,15 @@
     Dimension to reduce along.
 rep_dim : hashable, optional
     Name of new 'replicated' dimension:
 rec_dim : hashable, optional
     Name of dimension for 'records', i.e., multiple observations.
 """
 
-DOCFILLER_CMOMY = DocFiller.from_docstring(
-    _docstring_cmomy, combine_keys="parameters"
+docfiller = DocFiller.from_docstring(
+    _docstrings, combine_keys="parameters"
 ).assign_combined_key(
     "xr_params", ["dims", "attrs", "coords", "name", "indexes", "template"]
 )
 
 
-docfiller_shared = DOCFILLER_CMOMY()
+docfiller_decorate = docfiller()
```

### Comparing `cmomy-0.3.0/src/cmomy/_formatting.py` & `cmomy-0.4.0/src/cmomy/_formatting.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/src/cmomy/_resample.py` & `cmomy-0.4.0/src/cmomy/_resample.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/src/cmomy/_testing.py` & `cmomy-0.4.0/src/cmomy/_testing.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/src/cmomy/_typing.py` & `cmomy-0.4.0/src/cmomy/_typing.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/src/cmomy/abstract_central.py` & `cmomy-0.4.0/src/cmomy/abstract_central.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,21 +16,21 @@
     Union,
     cast,
     no_type_check,
 )
 
 import numpy as np
 from custom_inherit import DocInheritMeta
+from module_utilities import cached
 from numpy.core.numeric import normalize_axis_index  # type: ignore
 
 from . import convert
-from ._docstrings import docfiller_shared
 from ._formatting import repr_html
 from ._typing import Moments, T_Array, T_CentralMoments
-from .cached_decorators import gcached
+from .docstrings import docfiller_decorate
 from .options import DOC_SUB
 from .pushers import factory_pushers
 
 if TYPE_CHECKING:
     import xarray as xr
     from numpy.typing import ArrayLike, DTypeLike
 
@@ -188,15 +188,15 @@
         return self.val_shape + self.mom_shape_var
 
     @property
     def shape_flat_var(self) -> tuple[int, ...]:
         """Shape of flat variance."""
         return self.val_shape_flat + self.mom_shape_var
 
-    @gcached()
+    @cached.prop
     def _push(self):
         vec = len(self.val_shape) > 0
         cov = self.mom_ndim == 2
         return factory_pushers(cov=cov, vec=vec)
 
     def __repr__(self):
         """Repr for class."""
@@ -211,15 +211,15 @@
         """Used by np.array(self)."""  # noqa D401
         return np.asarray(self.data, dtype=dtype)
 
     ###########################################################################
     # ** top level creation/copy/new
     ###########################################################################
     @abstractmethod
-    @docfiller_shared
+    @docfiller_decorate
     def new_like(
         self: T_CentralMoments,
         *,
         data: ArrayLike | xr.DataArray | None = None,
         copy: bool = False,
         copy_kws: Mapping | None = None,
         verify: bool = True,
@@ -296,23 +296,23 @@
             copy_kws=copy_kws,
         )
 
     ###########################################################################
     # ** Access to underlying statistics
     ###########################################################################
 
-    @gcached()
+    @cached.prop
     def _weight_index(self):
         index = (0,) * len(self.mom)
         if self.val_ndim > 0:
             return (...,) + index
         else:
             return index
 
-    @gcached(prop=False)
+    @cached.meth
     def _single_index(self, val) -> tuple[list[int], ...]:
         # index with things like data[..., 1,0] data[..., 0,1]
         # index = (...,[1,0],[0,1])
         dims = len(self.mom)
         if dims == 1:
             index = [val]
         else:
@@ -552,15 +552,15 @@
             datas,
             target="datas",
             axis=axis,
             shape_flat=self.shape_flat,
             **kwargs,
         )[0]
 
-    @docfiller_shared
+    @docfiller_decorate
     def push_data(self: T_CentralMoments, data: Any) -> T_CentralMoments:
         """
         Push data object to moments.
 
         Parameters
         ----------
         data : array-like
@@ -570,15 +570,15 @@
         -------
         {pushed}
         """
         data = self._check_data(data)
         self._push.data(self._data_flat, data)
         return self
 
-    @docfiller_shared
+    @docfiller_decorate
     def push_datas(
         self: T_CentralMoments,
         datas,
         axis: int | None = None,
         **kwargs,
     ) -> T_CentralMoments:
         """
@@ -597,15 +597,15 @@
         {pushed}
         """
 
         datas = self._check_datas(datas=datas, axis=axis, **kwargs)
         self._push.datas(self._data_flat, datas)
         return self
 
-    @docfiller_shared
+    @docfiller_decorate
     def push_val(
         self: T_CentralMoments, x, w=None, broadcast: bool = False, **kwargs
     ) -> T_CentralMoments:
         """
         Push single sample to central moments.
 
         Parameters
@@ -636,15 +636,15 @@
 
         xr, target = self._check_val(x, "val", **kwargs)  # type: ignore
         yr = tuple(self._check_val(y, target=target, broadcast=broadcast) for y in ys)  # type: ignore
         wr = self._check_weight(w, target)  # type: ignore
         self._push.val(self._data_flat, *((wr, xr) + yr))
         return self
 
-    @docfiller_shared
+    @docfiller_decorate
     def push_vals(
         self: T_CentralMoments,
         x,
         w=None,
         axis: int | None = None,
         broadcast: bool = False,
         **kwargs,
@@ -776,15 +776,15 @@
         if not self._is_vector:
             if message is None:
                 message = "not implemented for scalar"
             raise ValueError(message)
 
     # * Universal reducers
 
-    @docfiller_shared
+    @docfiller_decorate
     def resample(
         self: T_CentralMoments,
         indices: np.ndarray,
         axis: int = 0,
         first: bool = True,
         **kws,
     ) -> T_CentralMoments:
@@ -990,15 +990,15 @@
             raise ValueError("must specify mom_ndim or mom")
 
         return mom_ndim
 
     # *** Core
     @classmethod
     @abstractmethod
-    @docfiller_shared
+    @docfiller_decorate
     def zeros(
         cls: type[T_CentralMoments],
         mom: Moments | None = None,
         val_shape: tuple[int, ...] | None = None,
         shape: tuple[int, ...] | None = None,
         mom_ndim: int | None = None,
         dtype: DTypeLike | None = None,
@@ -1031,15 +1031,15 @@
         from_data : General constructor
         numpy.zeros
 
         """
 
     @classmethod
     @abstractmethod
-    @docfiller_shared
+    @docfiller_decorate
     def from_data(
         cls: type[T_CentralMoments],
         data: Any,
         mom_ndim: int | None = None,
         mom: Moments | None = None,
         val_shape: tuple[int, ...] | None = None,
         copy: bool = True,
@@ -1069,15 +1069,15 @@
         out : object
             Same type as calling class.
 
         """
 
     @classmethod
     @abstractmethod
-    @docfiller_shared
+    @docfiller_decorate
     def from_datas(
         cls: type[T_CentralMoments],
         datas: Any,
         mom_ndim: int | None = None,
         axis: int | None = 0,
         mom: Moments | None = None,
         val_shape: tuple[int, ...] | None = None,
@@ -1108,15 +1108,15 @@
         See Also
         --------
         cmomy.CentralMoments.from_data
         """
 
     @classmethod
     @abstractmethod
-    @docfiller_shared
+    @docfiller_decorate
     def from_vals(
         cls: type[T_CentralMoments],
         x,
         w=None,
         axis: int | None = 0,
         mom: Moments = 2,
         val_shape: tuple[int, ...] | None = None,
@@ -1145,15 +1145,15 @@
         See Also
         --------
         push_vals
         """
 
     @classmethod
     @abstractmethod
-    @docfiller_shared
+    @docfiller_decorate
     def from_resample_vals(
         cls: type[T_CentralMoments],
         x,
         freq: np.ndarray | None = None,
         indices: np.ndarray | None = None,
         nrep: int | None = None,
         w: np.ndarray | None = None,
@@ -1207,15 +1207,15 @@
         cmomy.resample.randsamp_freq
         cmomy.resample.freq_to_indices
         cmomy.resample.indices_to_freq
         """
 
     @classmethod
     @abstractmethod
-    @docfiller_shared
+    @docfiller_decorate
     def from_raw(
         cls: type[T_CentralMoments],
         raw,
         mom_ndim: int | None = None,
         mom: Moments | None = None,
         val_shape: tuple[int, ...] | None = None,
         dtype: DTypeLike | None = None,
@@ -1253,15 +1253,15 @@
         Weights are taken from ``raw[...,0, 0]``.
         Using raw moments can result in numerical issues, especially for higher moments.  Use with care.
 
         """
 
     @classmethod
     @abstractmethod
-    @docfiller_shared
+    @docfiller_decorate
     def from_raws(
         cls: type[T_CentralMoments],
         raws,
         mom_ndim: int | None = None,
         mom: Moments | None = None,
         axis: int = 0,
         val_shape: tuple[int, ...] | None = None,
```

### Comparing `cmomy-0.3.0/src/cmomy/central.py` & `cmomy-0.4.0/src/cmomy/central.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import TYPE_CHECKING, Any, Hashable, Literal, Mapping, Sequence, cast
 
 import numpy as np
 import xarray as xr
 from numpy.core.numeric import normalize_axis_index  # type: ignore
 
 from . import convert
-from ._docstrings import docfiller_shared
+from .docstrings import docfiller_decorate
 from .resample import randsamp_freq, resample_data, resample_vals
 from .utils import _axis_expand_broadcast, _shape_insert_axis, _shape_reduce
 
 if TYPE_CHECKING:
     from numpy.typing import ArrayLike, DTypeLike
 
     from ._typing import ArrayOrder, Moments, T_CentralMoments
@@ -168,15 +168,15 @@
     out[0, 1, ...] = yave
 
     if last:
         out = np.moveaxis(out, [0, 1], [-2, -1])
     return out
 
 
-@docfiller_shared
+@docfiller_decorate
 def central_moments(
     x: np.ndarray | tuple[np.ndarray, np.ndarray],
     mom: Moments,
     w: np.ndarray | None = None,
     axis: int = 0,
     last: bool = True,
     dtype: DTypeLike | None = None,
@@ -371,15 +371,15 @@
             check_shape=check_shape,
             **kws,
         )
 
     ###########################################################################
     # SECTION: To/from xarray
     ###########################################################################
-    @docfiller_shared
+    @docfiller_decorate
     def to_xarray(
         self,
         dims: Hashable | Sequence[Hashable] | None = None,
         attrs: Mapping | None = None,
         coords: Mapping | None = None,
         name: Hashable | None = None,
         indexes: Any = None,
@@ -469,15 +469,15 @@
             )
 
         if copy:
             out = out.copy()
 
         return out
 
-    @docfiller_shared
+    @docfiller_decorate
     def to_xcentralmoments(
         self,
         dims: Hashable | Sequence[Hashable] | None = None,
         attrs: Mapping | None = None,
         coords: Mapping | None = None,
         name: Hashable | None = None,
         indexes: Any = None,
@@ -834,15 +834,15 @@
         wr = self._check_weights(w, target=target, axis=axis, **kwargs)
         self._push.vals(self._data_flat, *((wr, xr) + yr))
         return self
 
     ###########################################################################
     # SECTION: Manipulation
     ###########################################################################
-    @docfiller_shared
+    @docfiller_decorate
     def resample_and_reduce(
         self: T_CentralMoments,
         freq: np.ndarray | None = None,
         indices: np.ndarray | None = None,
         nrep: None = None,
         axis: int | None = None,
         parallel: bool = True,
@@ -896,15 +896,15 @@
         out = type(self).from_data(data, mom_ndim=self.mom_ndim, copy=False, **kws)
 
         if full_output:
             return out, freq
         else:
             return out
 
-    @docfiller_shared
+    @docfiller_decorate
     def reduce(
         self: T_CentralMoments, axis: int | None = None, **kws
     ) -> T_CentralMoments:
         """
         Create new object reduce along axis.
 
         Parameters
@@ -916,15 +916,15 @@
         """
         self._raise_if_scalar()
         axis = self._wrap_axis(axis, **kws)
         return type(self).from_datas(
             self.values, mom_ndim=self.mom_ndim, axis=axis, **kws
         )
 
-    @docfiller_shared
+    @docfiller_decorate
     def block(
         self: T_CentralMoments,
         block_size: int | None = None,
         axis: int | None = None,
         **kws,
     ) -> T_CentralMoments:
         """
@@ -975,15 +975,15 @@
             nblock = n // block_size
 
         datas = data[: (nblock * block_size), ...].reshape(
             (nblock, block_size) + data.shape[1:]
         )
         return type(self).from_datas(datas=datas, mom_ndim=self.mom_ndim, axis=1, **kws)
 
-    @docfiller_shared
+    @docfiller_decorate
     def reshape(
         self: T_CentralMoments,
         shape: tuple[int, ...],
         copy: bool = True,
         copy_kws: Mapping | None = None,
         **kws,
     ) -> T_CentralMoments:
@@ -1052,15 +1052,15 @@
             copy_kws=copy_kws,
             verify=True,
             check_shape=True,
             dtype=self.dtype,
             **kws,
         )
 
-    @docfiller_shared
+    @docfiller_decorate
     def moveaxis(
         self: T_CentralMoments,
         source: int | tuple[int, ...],
         destination: int | tuple[int, ...],
         copy: bool = True,
         copy_kws: Mapping | None = None,
         **kws,
```

### Comparing `cmomy-0.3.0/src/cmomy/compile.py` & `cmomy-0.4.0/src/cmomy/compile.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/src/cmomy/convert.py` & `cmomy-0.4.0/src/cmomy/convert.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Callable, Sequence, no_type_check
 
 import numpy as np
 from numpy import ndarray
 
-from ._docstrings import DocFiller
+from .docstrings import DocFiller
 from .options import OPTIONS
 from .utils import factory_binomial, myjit
 
 _bfac = factory_binomial(OPTIONS["nmax"])
 
 if TYPE_CHECKING:
     from numpy.typing import ArrayLike, DTypeLike
@@ -92,15 +92,15 @@
 dtype : str, optional
     Optional :mod:`numpy` data type to apply to output.
 out : ndarray, optional
     Optional numpy output array.  Should have same shape as ``x``.
 
 """
 
-docfiller_shared = DocFiller.from_docstring(_shared_docs, combine_keys="parameters")()
+docfiller_decorate = DocFiller.from_docstring(_shared_docs, combine_keys="parameters")()
 
 
 @myjit
 def _central_to_raw_moments(central, raw):
     nv = central.shape[0]
     order = central.shape[1] - 1
 
@@ -281,15 +281,15 @@
     data_r = data_r.reshape(reshape)
     out_r = out_r.reshape(reshape)
 
     func(data_r, out_r)
     return out_r.reshape(shape)
 
 
-@docfiller_shared
+@docfiller_decorate
 def to_raw_moments(
     x: ndarray,
     axis: int = -1,
     dtype: DTypeLike | None = None,
     order: ArrayOrder | None = None,
     out: np.ndarray | None = None,
 ) -> ndarray:
@@ -318,15 +318,15 @@
         func=_central_to_raw_moments,
         dtype=dtype,
         order=order,
         out=out,
     )
 
 
-@docfiller_shared
+@docfiller_decorate
 def to_raw_comoments(
     x: ndarray,
     axis: tuple[int, int] = (-2, -1),
     dtype: DTypeLike | None = None,
     order: ArrayOrder | None = None,
     out: np.ndarray | None = None,
 ) -> ndarray:
@@ -356,15 +356,15 @@
         func=_central_to_raw_comoments,
         dtype=dtype,
         order=order,
         out=out,
     )
 
 
-@docfiller_shared
+@docfiller_decorate
 def to_central_moments(
     x: ndarray,
     axis: int = -1,
     dtype: DTypeLike | None = None,
     order: ArrayOrder | None = None,
     out: np.ndarray | None = None,
 ) -> ndarray:
@@ -394,15 +394,15 @@
         func=_raw_to_central_moments,
         dtype=dtype,
         order=order,
         out=out,
     )
 
 
-@docfiller_shared
+@docfiller_decorate
 def to_central_comoments(
     x: ndarray,
     axis: tuple[int, int] = (-2, -1),
     dtype: DTypeLike | None = None,
     order: ArrayOrder | None = None,
     out: np.ndarray | None = None,
 ) -> ndarray:
```

### Comparing `cmomy-0.3.0/src/cmomy/options.py` & `cmomy-0.4.0/src/cmomy/options.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/src/cmomy/pusher_interface.py` & `cmomy-0.4.0/src/cmomy/pusher_interface.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/src/cmomy/pushers.py` & `cmomy-0.4.0/src/cmomy/pushers.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/src/cmomy/resample.py` & `cmomy-0.4.0/src/cmomy/resample.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/src/cmomy/tests/conftest.py` & `cmomy-0.4.0/src/cmomy/tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import pytest
 import xarray as xr
+from module_utilities import cached
 
 import cmomy.central as central
 import cmomy.xcentral as xcentral
-from cmomy.cached_decorators import gcached
 
 
 def _get_cmom(w, x, moments, axis=0, last=True):
     if w is None:
         w = np.array(1.0)
 
     if w.ndim == 1 and w.ndim != x.ndim and len(w) == x.shape[axis]:
@@ -113,15 +113,15 @@
             shape = (shape,)
         self.shape = shape
         self.axis = axis
         self.style = style
         self.mom = mom
         self.nsplit = nsplit
 
-    @gcached()
+    @cached.prop
     def cov(self):
         if isinstance(self.mom, int):
             return False
         if isinstance(self.mom, tuple) and len(self.mom) == 2:
             return True
 
     @property
@@ -135,53 +135,53 @@
     def broadcast(self):
         return self.style == "broadcast"
 
     @property
     def cls(self):
         return central.CentralMoments
 
-    @gcached()
+    @cached.prop
     def val_shape(self):
         val_shape = list(self.shape)
         val_shape.pop(self.axis)
         return tuple(val_shape)
 
     def _get_data(self, style=None):
         if style is None or style == "total":
             return np.random.rand(*self.shape)
         elif style == "broadcast":
             return np.random.rand(self.shape[self.axis])
         else:
             raise ValueError("bad style")
 
-    @gcached()
+    @cached.prop
     def xdata(self):
         return self._get_data()
 
-    @gcached()
+    @cached.prop
     def ydata(self):
         return self._get_data(style=self.style)
 
-    @gcached()
+    @cached.prop
     def w(self):
         if self.style is None:
             return None
         #            return np.array(1.0)
         else:
             return self._get_data(style=self.style)
         return self._get_weight()
 
-    @gcached()
+    @cached.prop
     def x(self):
         if self.cov:
             return (self.xdata, self.ydata)
         else:
             return self.xdata
 
-    @gcached()
+    @cached.prop
     def split_data(self):
         v = self.xdata.shape[self.axis] // self.nsplit
         splits = [v * i for i in range(1, self.nsplit)]
         X = np.split(self.xdata, splits, axis=self.axis)
 
         if self.style == "total":
             W = np.split(self.w, splits, axis=self.axis)
@@ -205,15 +205,15 @@
     def W(self):
         return self.split_data[0]
 
     @property
     def X(self):
         return self.split_data[1]
 
-    @gcached()
+    @cached.prop
     def data_fix(self):
         if self.cov:
             return _get_comom(
                 w=self.w,
                 x=self.x[0],
                 y=self.x[1],
                 moments=self.mom,
@@ -221,32 +221,32 @@
                 broadcast=self.broadcast,
             )
         else:
             return _get_cmom(
                 w=self.w, x=self.x, moments=self.mom, axis=self.axis, last=True
             )
 
-    @gcached()
+    @cached.prop
     def data_test(self):
         return central.central_moments(
             x=self.x,
             mom=self.mom,
             w=self.w,
             axis=self.axis,
             last=True,
             broadcast=self.broadcast,
         )
 
-    @gcached()
+    @cached.prop
     def s(self):
         s = self.cls.zeros(val_shape=self.val_shape, mom=self.mom)
         s.push_vals(x=self.x, w=self.w, axis=self.axis, broadcast=self.broadcast)
         return s
 
-    @gcached()
+    @cached.prop
     def S(self):
         return [
             self.cls.from_vals(
                 x=xx, w=ww, axis=self.axis, mom=self.mom, broadcast=self.broadcast
             )
             for ww, xx in zip(self.W, self.X)
         ]
@@ -290,34 +290,34 @@
 
                 raw[..., 0, 0] = self.w.sum(self.axis)
 
         else:
             raw = None
         return raw
 
-    @gcached()
+    @cached.prop
     def indices(self):
         ndat = self.xdata.shape[self.axis]
         nrep = 10
         return np.random.choice(ndat, (nrep, ndat), replace=True)
 
-    @gcached()
+    @cached.prop
     def freq(self):
         return central.randsamp_freq(indices=self.indices)
 
-    @gcached()
+    @cached.prop
     def xdata_resamp(self):
         xdata = self.xdata
 
         if self.axis != 0:
             xdata = np.moveaxis(xdata, self.axis, 0)
 
         return np.take(xdata, self.indices, axis=0)
 
-    @gcached()
+    @cached.prop
     def ydata_resamp(self):
         ydata = self.ydata
 
         if self.style == "broadcast":
             return np.take(ydata, self.indices, axis=0)
         else:
             if self.axis != 0:
@@ -327,64 +327,64 @@
     @property
     def x_resamp(self):
         if self.cov:
             return (self.xdata_resamp, self.ydata_resamp)
         else:
             return self.xdata_resamp
 
-    @gcached()
+    @cached.prop
     def w_resamp(self):
         w = self.w
 
         if self.style is None:
             return w
         elif self.style == "broadcast":
             return np.take(w, self.indices, axis=0)
         else:
             if self.axis != 0:
                 w = np.moveaxis(w, self.axis, 0)
             return np.take(w, self.indices, axis=0)
 
-    @gcached()
+    @cached.prop
     def data_test_resamp(self):
         return central.central_moments(
             x=self.x_resamp,
             mom=self.mom,
             w=self.w_resamp,
             axis=1,
             broadcast=self.broadcast,
         )
 
     # xcentral specific stuff
     @property
     def cls_xr(self):
         return xcentral.xCentralMoments
 
-    @gcached()
+    @cached.prop
     def s_xr(self):
         return self.cls_xr.from_vals(
             x=self.x, w=self.w, axis=self.axis, mom=self.mom, broadcast=self.broadcast
         )
 
-    @gcached()
+    @cached.prop
     def xdata_xr(self):
         dims = [f"dim_{i}" for i in range(len(self.shape) - 1)]
         dims.insert(self.axis, "rec")
         return xr.DataArray(self.xdata, dims=dims)
 
-    @gcached()
+    @cached.prop
     def ydata_xr(self):
         if self.style is None or self.style == "total":
             dims = self.xdata_xr.dims
         else:
             dims = "rec"
 
         return xr.DataArray(self.ydata, dims=dims)
 
-    @gcached()
+    @cached.prop
     def w_xr(self):
         if self.style is None:
             return None
         elif self.style == "broadcast":
             dims = "rec"
         else:
             dims = self.xdata_xr.dims
@@ -394,43 +394,43 @@
     @property
     def x_xr(self):
         if self.cov:
             return (self.xdata_xr, self.ydata_xr)
         else:
             return self.xdata_xr
 
-    @gcached()
+    @cached.prop
     def data_test_xr(self):
         return xcentral.xcentral_moments(
             x=self.x_xr, mom=self.mom, dim="rec", w=self.w_xr, broadcast=self.broadcast
         )
 
-    @gcached()
+    @cached.prop
     def W_xr(self):
         if isinstance(self.w_xr, xr.DataArray):
             dims = self.w_xr.dims
             return [xr.DataArray(_, dims=dims) for _ in self.W]
         else:
             return self.W
 
-    @gcached()
+    @cached.prop
     def X_xr(self):
         xdims = self.xdata_xr.dims
 
         if self.cov:
             ydims = self.ydata_xr.dims
 
             return [
                 (xr.DataArray(x, dims=xdims), xr.DataArray(y, dims=ydims))
                 for x, y in self.X
             ]
         else:
             return [xr.DataArray(x, dims=xdims) for x in self.X]
 
-    @gcached()
+    @cached.prop
     def S_xr(self):
         return [
             self.cls_xr.from_vals(
                 x=x, w=w, axis=self.axis, mom=self.mom, broadcast=self.broadcast
             )
             for w, x, in zip(self.W, self.X)
         ]
```

### Comparing `cmomy-0.3.0/src/cmomy/tests/test_central.py` & `cmomy-0.4.0/src/cmomy/tests/test_central.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/src/cmomy/tests/test_central_2.py` & `cmomy-0.4.0/src/cmomy/tests/test_central_2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import numpy as np
 import pytest
-from numpy.core.multiarray import normalize_axis_index
 
 from cmomy import CentralMoments, central_moments
 from cmomy._testing import _get_cmom, _get_comom
-from cmomy.cached_decorators import gcached
 from cmomy.tests.conftest import Data
 
 
 class DataContainer:
     def __init__(self, x, y, w):
         self.x = x
         self.y = y
```

### Comparing `cmomy-0.3.0/src/cmomy/tests/test_convert.py` & `cmomy-0.4.0/src/cmomy/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/src/cmomy/tests/test_resample.py` & `cmomy-0.4.0/src/cmomy/tests/test_resample.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/src/cmomy/tests/test_stability.py` & `cmomy-0.4.0/src/cmomy/tests/test_stability.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/src/cmomy/tests/test_verify.py` & `cmomy-0.4.0/src/cmomy/tests/test_verify.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/src/cmomy/tests/test_xcentral.py` & `cmomy-0.4.0/src/cmomy/tests/test_xcentral.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/src/cmomy/tests/test_xcentral_constructors.py` & `cmomy-0.4.0/src/cmomy/tests/test_xcentral_constructors.py`

 * *Files identical despite different names*

### Comparing `cmomy-0.3.0/src/cmomy/utils.py` & `cmomy-0.4.0/src/cmomy/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from functools import lru_cache
 from typing import TYPE_CHECKING, Sequence
 
 import numpy as np
 from numba import njit
 
-# from .cached_decorators import gcached  # , cached_clear
 from .options import OPTIONS
 
 if TYPE_CHECKING:
     from numpy.typing import ArrayLike, DTypeLike
 
     from ._typing import ArrayOrder
```

### Comparing `cmomy-0.3.0/src/cmomy/xcentral.py` & `cmomy-0.4.0/src/cmomy/xcentral.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,20 +15,20 @@
     cast,
     no_type_check,
 )
 from warnings import warn
 
 import numpy as np
 import xarray as xr
+from module_utilities import cached
 
 from . import convert
-from ._docstrings import docfiller_shared
 from .abstract_central import CentralMomentsABC
-from .cached_decorators import gcached
 from .central import CentralMoments
+from .docstrings import docfiller_decorate
 from .utils import _shape_reduce
 
 if TYPE_CHECKING:
     from numpy.typing import DTypeLike
 
     from ._typing import Dims, MomDims, Moments, T_CentralMoments
 
@@ -208,15 +208,15 @@
     out.loc[{mom_dims[0]: 0, mom_dims[1]: 1}] = xave[1]
 
     if last:
         out = out.transpose(..., *mom_dims)
     return out
 
 
-@docfiller_shared
+@docfiller_decorate
 def xcentral_moments(
     x: xr.DataArray | tuple[xr.DataArray, xr.DataArray],
     mom: Moments,
     w: xr.DataArray | None = None,
     axis: int | None = None,
     dim: Hashable | None = None,
     last: bool = True,
@@ -358,15 +358,15 @@
 
     @property
     def mom_dims(self) -> tuple[Hashable, ...]:
         """Names of moment dimensions."""
         return self.dims[-self.mom_ndim :]
 
     # ** top level creation/copy/new
-    @gcached()
+    @cached.prop
     def _template_val(self) -> xr.DataArray:
         """Template for values part of data."""
         return self._xdata[self._weight_index]
 
     def _wrap_like(self, x) -> xr.DataArray:
         return self._xdata.copy(data=x)
 
@@ -763,30 +763,30 @@
         )
 
     # ** To/from CentralMoments
     def to_centralmoments(self):
         """Create a CentralMoments object from xCentralMoments."""
         return CentralMoments(data=self.data, mom_ndim=self.mom_ndim)
 
-    @gcached()
+    @cached.prop
     def centralmoments_view(self):
         """
         Create CentralMoments view.
 
         This object has the same underlying data as `self`, but no
         DataArray attributes.  Useful for some function calls.
 
         See Also
         --------
         CentralMoments.to_xcentralmoments
         """
         return self.to_centralmoments()
 
     @classmethod
-    @docfiller_shared
+    @docfiller_decorate
     def from_centralmoments(
         cls,
         obj: CentralMoments,
         dims: Hashable | Sequence[Hashable] | None = None,
         attrs: Mapping | None = None,
         coords: Mapping | None = None,
         name: Hashable | None = None,
@@ -991,15 +991,15 @@
                 axis=axis,
                 broadcast=broadcast,
                 expand=expand,
                 shape_flat=shape_flat,
             )
 
     # ** Manipulation
-    @docfiller_shared
+    @docfiller_decorate
     def resample_and_reduce(
         self,
         freq: np.ndarray | None = None,
         indices: np.ndarray | None = None,
         nrep: int | None = None,
         axis: int | str | None = None,
         dim: Hashable | None = None,
@@ -1121,15 +1121,15 @@
     ) -> int:
         if isinstance(axis, str):
             raise ValueError("shouldn't get string axis here")
         else:
             return super()._wrap_axis(axis=axis, default=default, ndim=ndim)
 
     @no_type_check
-    @docfiller_shared
+    @docfiller_decorate
     def reduce(
         self: T_CentralMoments,
         dim: Hashable | None = None,
         axis: int | str | None = None,
         **kws,
     ) -> T_CentralMoments:
         """
@@ -1160,15 +1160,15 @@
         axis, dim = _select_axis_dim(dims=self.dims, axis=axis, dim=dim)
         axis = self._wrap_axis(axis)
         return type(self).from_datas(
             self.values, mom_ndim=self.mom_ndim, axis=axis, **kws
         )
 
     @no_type_check
-    @docfiller_shared
+    @docfiller_decorate
     def block(
         self,
         block_size: int,
         dim: Hashable | None = None,
         axis: int | str | None = None,
         coords_policy: Literal["first", "last", None] = "first",
         **kws,
@@ -1262,15 +1262,15 @@
         return self.centralmoments_view.block(
             block_size=block_size, axis=axis, **kws
         ).to_xcentralmoments(template=template)
 
     # ** Constructors
     @no_type_check
     @classmethod
-    @docfiller_shared
+    @docfiller_decorate
     def zeros(
         cls: type[T_CentralMoments],
         mom: Moments | None = None,
         val_shape: tuple[int, ...] | None = None,
         mom_ndim: int | None = None,
         shape: tuple[int, ...] | None = None,
         dtype: DTypeLike | None = None,
@@ -1330,15 +1330,15 @@
                 name=name,
                 indexes=indexes,
                 mom_dims=mom_dims,
                 **{"copy": True, "check_shape": True, "verify": True, **kws},
             ).zero()
 
     @classmethod
-    @docfiller_shared
+    @docfiller_decorate
     def from_data(
         cls,
         data: np.ndarray | xr.DataArray,
         mom: Moments | None = None,
         mom_ndim: int | None = None,
         val_shape: tuple[int, ...] | None = None,
         dtype: DTypeLike | None = None,
@@ -1422,15 +1422,15 @@
                 name=name,
                 template=template,
                 mom_dims=mom_dims,
             )
 
     @classmethod
     @no_type_check
-    @docfiller_shared
+    @docfiller_decorate
     def from_datas(
         cls,
         datas: np.ndarray | xr.DataArray,
         mom: Moments | None = None,
         mom_ndim: int | None = None,
         axis: int | str | None = None,
         dim: Hashable | None = None,
@@ -1519,15 +1519,15 @@
                 **kws,
             )
 
         return new
 
     @no_type_check
     @classmethod
-    @docfiller_shared
+    @docfiller_decorate
     def from_raw(
         cls,
         raw: np.ndarray | xr.DataArray,
         mom: Moments | None = None,
         mom_ndim: int | None = None,
         val_shape: tuple[int, ...] | None = None,
         dtype: DTypeLike | None = None,
@@ -1673,15 +1673,15 @@
                 name=name,
                 mom_dims=mom_dims,
                 **kws,
             )
 
     @no_type_check
     @classmethod
-    @docfiller_shared
+    @docfiller_decorate
     def from_vals(
         cls,
         x: np.ndarray
         | tuple[np.ndarray, np.ndarray]
         | xr.DataArray
         | tuple[xr.DataArray, xr.DataArray]
         | tuple[xr.DataArray, np.ndarray],
@@ -1781,15 +1781,15 @@
                 **kws,
             )
 
         return new
 
     @no_type_check
     @classmethod
-    @docfiller_shared
+    @docfiller_decorate
     def from_resample_vals(
         cls,
         x: np.ndarray
         | tuple[np.ndarray, np.ndarray]
         | xr.DataArray
         | tuple[xr.DataArray, xr.DataArray],
         freq=None,
```

### Comparing `cmomy-0.3.0/src/cmomy.egg-info/PKG-INFO` & `cmomy-0.4.0/src/cmomy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmomy
-Version: 0.3.0
+Version: 0.4.0
 Summary: Central (co)moment calculation/manipulation
 Home-page: https://github.com/usnistgov/cmomy
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
 License: NIST license
 Project-URL: homepage, https://github.com/usnistgov/cmomy
 Project-URL: documentation, https://pages.nist.gov/cmomy/
 Keywords: cmomy
@@ -19,57 +19,58 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-# cmomy
-
-A Python package to calculate and manipulate Central (co)moments. The main
-features of `cmomy` are as follows:
-
-- [Numba][Numba] accelerated computation of central moments and co-moments
-- Routines to combine, and resample central moments.
-- Both [numpy][numpy] array-like and [xarray][xarray] DataArray interfaces to
-  Data.
-- Routines to convert between central and raw moments.
+<!-- markdownlint-disable MD041 -->
 
 [![Repo][repo-badge]][repo-link] [![Docs][docs-badge]][docs-link]
 [![PyPI license][license-badge]][license-link]
 [![PyPI version][pypi-badge]][pypi-link]
 [![Conda (channel only)][conda-badge]][conda-link]
 [![Code style: black][black-badge]][black-link]
 
+<!--
+  For more badges, see
+  https://shields.io/category/other
+  https://naereen.github.io/badges/
+  [pypi-badge]: https://badge.fury.io/py/cmomy
+-->
+
 [black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
-[black-link]: https://github.com/ambv/black
+[black-link]: https://github.com/psf/black
 [pypi-badge]: https://img.shields.io/pypi/v/cmomy
-
-<!-- [pypi-badge]: https://badge.fury.io/py/cmomy.svg -->
-
 [pypi-link]: https://pypi.org/project/cmomy
 [docs-badge]: https://img.shields.io/badge/docs-sphinx-informational
 [docs-link]: https://pages.nist.gov/cmomy/
 [repo-badge]: https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff
 [repo-link]: https://github.com/usnistgov/cmomy
 [conda-badge]: https://img.shields.io/conda/v/wpk-nist/cmomy
 [conda-link]: https://anaconda.org/wpk-nist/cmomy
+[license-badge]: https://img.shields.io/pypi/l/cmomy?color=informational
+[license-link]: https://github.com/usnistgov/cmomy/blob/main/LICENSE
+
+<!-- other links -->
+
 [numpy]: https://numpy.org
 [Numba]: https://numba.pydata.org/
 [xarray]: https://docs.xarray.dev/en/stable/
 
-<!-- Use total link so works from anywhere -->
+# cmomy
 
-[license-badge]: https://img.shields.io/pypi/l/cmomy?color=informational
-[license-link]: https://github.com/usnistgov/cmomy/blob/master/LICENSE
+A Python package to calculate and manipulate Central (co)moments. The main
+features of `cmomy` are as follows:
 
-<!-- For more badges see
-https://shields.io/category/other
-https://naereen.github.io/badges/
--->
+- [Numba][Numba] accelerated computation of central moments and co-moments
+- Routines to combine, and resample central moments.
+- Both [numpy][numpy] array-like and [xarray][xarray] DataArray interfaces to
+  Data.
+- Routines to convert between central and raw moments.
 
 ## Overview
 
 `cmomy` is an open source package to calculate central moments and co-moments in
 a numerical stable and direct way. Behind the scenes, `cmomy` makes use of
 [Numba][Numba] to rapidly calculate moments. A good introduction to the type of
 formulas used can be found
@@ -196,14 +197,36 @@
 
 ## Unreleased
 
 See the fragment files in [changelog.d](https://github.com/usnistgov/cmomy)
 
 <!-- scriv-insert-here -->
 
+## v0.4.0 — 2023-05-02
+
+### Added
+
+- Moved module `_docstrings_` to `docstrings`. This can be used by other
+  modules.
+
+### Changed
+
+- Update package layout
+- New linters via pre-commit
+- Development env now handled by tox
+
+- Now use `module-utilities` to handle caching and docfiller.
+
+[`v0.3.0...v0.4.0`](https://github.com/usnistgov/cmomy/compare/v0.3.0...v0.4.0)
+
+## v0.3.0 - 2023-04-24
+
+Full set of changes:
+[`v0.2.2...v0.3.0`](https://github.com/usnistgov/cmomy/compare/v0.2.2...v0.3.0)
+
 ## v0.2.2 - 2023-04-05
 
 Full set of changes:
 [`v0.2.1...v0.2.2`](https://github.com/usnistgov/cmomy/compare/v0.2.1...v0.2.2)
 
 ## v0.2.1 - 2023-04-05
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cmomy-0.3.0/src/cmomy.egg-info/SOURCES.txt` & `cmomy-0.4.0/src/cmomy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,22 +8,20 @@
 AUTHORS.md
 CHANGELOG.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 Makefile
 README.md
-commands.sh
 conftest.py
 environment.yaml
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
-changelog.d/20230424_125230_william.krekelberg_update_cruft.md
 changelog.d/README.txt
 changelog.d/templates/new_fragment.md.j2
 changelog.d/templates/auto-changelog/macros.jinja2
 changelog.d/templates/auto-changelog/template.jinja2
 docs/Makefile
 docs/authors.md
 docs/changelog.md
@@ -74,43 +72,43 @@
 examples/archived/bootstrap.ipynb
 examples/archived/central_moments.ipynb
 examples/archived/example_usage.ipynb
 examples/archived/parallel_test.ipynb
 examples/archived/test_accumulator.ipynb
 examples/usage/motivation.ipynb
 examples/usage/usage_notebook.ipynb
+scripts/dist-conda.mk
+scripts/dist-pypi.mk
 scripts/docs-examples-symlinks.sh
+scripts/lint.mk
+scripts/run-prettier.sh
 scripts/tox-ipykernel-display-name.sh
 src/cmomy/__init__.py
-src/cmomy/_docstrings.py
 src/cmomy/_formatting.py
 src/cmomy/_resample.py
 src/cmomy/_testing.py
 src/cmomy/_typing.py
 src/cmomy/abstract_central.py
-src/cmomy/cached_decorators.py
 src/cmomy/central.py
 src/cmomy/compile.py
 src/cmomy/convert.py
+src/cmomy/docstrings.py
 src/cmomy/options.py
 src/cmomy/pusher_interface.py
 src/cmomy/pushers.py
 src/cmomy/py.typed
 src/cmomy/resample.py
 src/cmomy/utils.py
 src/cmomy/xcentral.py
 src/cmomy.egg-info/PKG-INFO
 src/cmomy.egg-info/SOURCES.txt
 src/cmomy.egg-info/dependency_links.txt
 src/cmomy.egg-info/not-zip-safe
 src/cmomy.egg-info/requires.txt
 src/cmomy.egg-info/top_level.txt
-src/cmomy/_docfiller/__init__.py
-src/cmomy/_docfiller/docfiller.py
-src/cmomy/_docfiller/docscrape.py
 src/cmomy/tests/__init__.py
 src/cmomy/tests/conftest.py
 src/cmomy/tests/test_central.py
 src/cmomy/tests/test_central_2.py
 src/cmomy/tests/test_convert.py
 src/cmomy/tests/test_resample.py
 src/cmomy/tests/test_stability.py
```

