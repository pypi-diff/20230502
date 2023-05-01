# Comparing `tmp/augmenty-1.3.5.tar.gz` & `tmp/augmenty-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "augmenty-1.3.5.tar", last modified: Mon May  1 20:20:19 2023, max compression
+gzip compressed data, was "augmenty-1.3.6.tar", last modified: Mon May  1 22:29:38 2023, max compression
```

## Comparing `augmenty-1.3.5.tar` & `augmenty-1.3.6.tar`

### file list

```diff
@@ -1,158 +1,158 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.755472 augmenty-1.3.5/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.735472 augmenty-1.3.5/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.735472 augmenty-1.3.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      729 2023-05-01 20:20:08.000000 augmenty-1.3.5/.github/ISSUE_TEMPLATE/01_bugs.md
--rw-r--r--   0 root         (0) root         (0)      418 2023-05-01 20:20:08.000000 augmenty-1.3.5/.github/ISSUE_TEMPLATE/02_docs.md
--rw-r--r--   0 root         (0) root         (0)      291 2023-05-01 20:20:08.000000 augmenty-1.3.5/.github/ISSUE_TEMPLATE/03_feature-request.md
--rw-r--r--   0 root         (0) root         (0)      283 2023-05-01 20:20:08.000000 augmenty-1.3.5/.github/ISSUE_TEMPLATE/04_augmenter-request.md
--rw-r--r--   0 root         (0) root         (0)      625 2023-05-01 20:20:08.000000 augmenty-1.3.5/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 root         (0) root         (0)      776 2023-05-01 20:20:08.000000 augmenty-1.3.5/.github/dependabot.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.735472 augmenty-1.3.5/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1013 2023-05-01 20:20:08.000000 augmenty-1.3.5/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 root         (0) root         (0)     1280 2023-05-01 20:20:08.000000 augmenty-1.3.5/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)     1673 2023-05-01 20:20:08.000000 augmenty-1.3.5/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)     2697 2023-05-01 20:20:08.000000 augmenty-1.3.5/.github/workflows/tests.yml
--rw-r--r--   0 root         (0) root         (0)      186 2023-05-01 20:20:08.000000 augmenty-1.3.5/.gitignore
--rw-r--r--   0 root         (0) root         (0)      797 2023-05-01 20:20:08.000000 augmenty-1.3.5/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)     2716 2023-05-01 20:20:09.000000 augmenty-1.3.5/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1075 2023-05-01 20:20:08.000000 augmenty-1.3.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7212 2023-05-01 20:20:19.755472 augmenty-1.3.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      372 2023-05-01 20:20:08.000000 augmenty-1.3.5/citation.cff
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.739472 augmenty-1.3.5/docs/
--rw-r--r--   0 root         (0) root         (0)      634 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.739472 augmenty-1.3.5/docs/_static/
--rw-r--r--   0 root         (0) root         (0)     1150 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/_static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)   385037 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/_static/icon.png
--rw-r--r--   0 root         (0) root         (0)   395381 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/_static/icon_dark.png
--rw-r--r--   0 root         (0) root         (0)     2308 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/adding_an_augmenter.rst
--rw-r--r--   0 root         (0) root         (0)     6366 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/augmenters_overview.md
--rw-r--r--   0 root         (0) root         (0)      392 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/augmenty.augment_utilities.rst
--rw-r--r--   0 root         (0) root         (0)     1009 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/augmenty.character.rst
--rw-r--r--   0 root         (0) root         (0)      733 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/augmenty.doc.rst
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/augmenty.keyboard.rst
--rw-r--r--   0 root         (0) root         (0)      500 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/augmenty.lang.rst
--rw-r--r--   0 root         (0) root         (0)      334 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/augmenty.span.rst
--rw-r--r--   0 root         (0) root         (0)     1089 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/augmenty.token.rst
--rw-r--r--   0 root         (0) root         (0)      330 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/augmenty.util.rst
--rw-r--r--   0 root         (0) root         (0)     4190 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     2561 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/create_augmenters_table.py
--rw-r--r--   0 root         (0) root         (0)     3444 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/faq.rst
--rw-r--r--   0 root         (0) root         (0)     2578 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     1055 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/installation.rst
--rw-r--r--   0 root         (0) root         (0)      795 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)     1149 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/news.rst
--rw-r--r--   0 root         (0) root         (0)       61 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.739472 augmenty-1.3.5/docs/tutorials/
--rw-r--r--   0 root         (0) root         (0)    15539 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/tutorials/introduction.ipynb
--rw-r--r--   0 root         (0) root         (0)      210 2023-05-01 20:20:08.000000 augmenty-1.3.5/docs/tutorials/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.743472 augmenty-1.3.5/img/
--rw-r--r--   0 root         (0) root         (0)   385037 2023-05-01 20:20:08.000000 augmenty-1.3.5/img/icon.png
--rw-r--r--   0 root         (0) root         (0)     3243 2023-05-01 20:20:09.000000 augmenty-1.3.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     4521 2023-05-01 20:20:08.000000 augmenty-1.3.5/readme.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-01 20:20:19.755472 augmenty-1.3.5/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.735472 augmenty-1.3.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.743472 augmenty-1.3.5/src/augmenty/
--rw-r--r--   0 root         (0) root         (0)     2053 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/__init__.py
--rw-r--r--   0 root         (0) root         (0)      164 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/about.py
--rw-r--r--   0 root         (0) root         (0)     3336 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/augment_utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.743472 augmenty-1.3.5/src/augmenty/character/
--rw-r--r--   0 root         (0) root         (0)      355 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/character/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1564 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/character/casing.py
--rw-r--r--   0 root         (0) root         (0)     4613 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/character/replace.py
--rw-r--r--   0 root         (0) root         (0)     1566 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/character/spacing.py
--rw-r--r--   0 root         (0) root         (0)     1606 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/character/swap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.743472 augmenty-1.3.5/src/augmenty/doc/
--rw-r--r--   0 root         (0) root         (0)      184 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/doc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2666 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/doc/casing.py
--rw-r--r--   0 root         (0) root         (0)     3887 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/doc/subset.py
--rw-r--r--   0 root         (0) root         (0)     3509 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.743472 augmenty-1.3.5/src/augmenty/lang/
--rw-r--r--   0 root         (0) root         (0)      784 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.743472 augmenty-1.3.5/src/augmenty/lang/da/
--rw-r--r--   0 root         (0) root         (0)      195 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/da/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1878 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/da/augmenters.py
--rw-r--r--   0 root         (0) root         (0)      790 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/da/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.747472 augmenty-1.3.5/src/augmenty/lang/de/
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/de/__init__.py
--rw-r--r--   0 root         (0) root         (0)      783 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/de/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.747472 augmenty-1.3.5/src/augmenty/lang/el/
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/el/__init__.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/el/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.747472 augmenty-1.3.5/src/augmenty/lang/en/
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/en/__init__.py
--rw-r--r--   0 root         (0) root         (0)      776 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/en/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.747472 augmenty-1.3.5/src/augmenty/lang/es/
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/es/__init__.py
--rw-r--r--   0 root         (0) root         (0)      783 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/es/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.747472 augmenty-1.3.5/src/augmenty/lang/fr/
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/fr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      783 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/fr/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.747472 augmenty-1.3.5/src/augmenty/lang/hu/
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/hu/__init__.py
--rw-r--r--   0 root         (0) root         (0)      803 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/hu/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.747472 augmenty-1.3.5/src/augmenty/lang/it/
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/it/__init__.py
--rw-r--r--   0 root         (0) root         (0)      784 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/it/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.747472 augmenty-1.3.5/src/augmenty/lang/lt/
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/lt/__init__.py
--rw-r--r--   0 root         (0) root         (0)      794 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/lt/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.747472 augmenty-1.3.5/src/augmenty/lang/mk/
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/mk/__init__.py
--rw-r--r--   0 root         (0) root         (0)      823 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/mk/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.747472 augmenty-1.3.5/src/augmenty/lang/nb/
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/nb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      784 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/nb/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.747472 augmenty-1.3.5/src/augmenty/lang/nl/
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/nl/__init__.py
--rw-r--r--   0 root         (0) root         (0)      775 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/nl/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.747472 augmenty-1.3.5/src/augmenty/lang/pl/
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/pl/__init__.py
--rw-r--r--   0 root         (0) root         (0)      775 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/pl/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.751472 augmenty-1.3.5/src/augmenty/lang/pt/
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/pt/__init__.py
--rw-r--r--   0 root         (0) root         (0)      780 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/pt/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.751472 augmenty-1.3.5/src/augmenty/lang/ro/
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/ro/__init__.py
--rw-r--r--   0 root         (0) root         (0)      780 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/ro/keyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.751472 augmenty-1.3.5/src/augmenty/lang/ru/
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/ru/__init__.py
--rw-r--r--   0 root         (0) root         (0)      828 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/lang/ru/keyboard.py
--rw-r--r--   0 root         (0) root         (0)     8801 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/meta.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.751472 augmenty-1.3.5/src/augmenty/span/
--rw-r--r--   0 root         (0) root         (0)      177 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/span/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11745 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/span/entities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.751472 augmenty-1.3.5/src/augmenty/token/
--rw-r--r--   0 root         (0) root         (0)      680 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/token/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3967 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/token/casing.py
--rw-r--r--   0 root         (0) root         (0)    12158 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/token/insert.py
--rw-r--r--   0 root         (0) root         (0)    11343 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/token/replace.py
--rw-r--r--   0 root         (0) root         (0)     2951 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/token/spacing.py
--rw-r--r--   0 root         (0) root         (0)     2325 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/token/static_embedding_util.py
--rw-r--r--   0 root         (0) root         (0)     4915 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/token/swap.py
--rw-r--r--   0 root         (0) root         (0)      814 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/token/wordnet_util.py
--rw-r--r--   0 root         (0) root         (0)     3798 2023-05-01 20:20:08.000000 augmenty-1.3.5/src/augmenty/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.743472 augmenty-1.3.5/src/augmenty.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7212 2023-05-01 20:20:19.000000 augmenty-1.3.5/src/augmenty.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3423 2023-05-01 20:20:19.000000 augmenty-1.3.5/src/augmenty.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 20:20:19.000000 augmenty-1.3.5/src/augmenty.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      438 2023-05-01 20:20:19.000000 augmenty-1.3.5/src/augmenty.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-01 20:20:19.000000 augmenty-1.3.5/src/augmenty.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.755472 augmenty-1.3.5/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 20:20:08.000000 augmenty-1.3.5/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20399 2023-05-01 20:20:08.000000 augmenty-1.3.5/tests/books.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-05-01 20:20:08.000000 augmenty-1.3.5/tests/fixtures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 20:20:19.755472 augmenty-1.3.5/tests/lang/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 20:20:08.000000 augmenty-1.3.5/tests/lang/__init__.py
--rw-r--r--   0 root         (0) root         (0)      999 2023-05-01 20:20:08.000000 augmenty-1.3.5/tests/lang/test_da.py
--rw-r--r--   0 root         (0) root         (0)      147 2023-05-01 20:20:08.000000 augmenty-1.3.5/tests/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     2960 2023-05-01 20:20:08.000000 augmenty-1.3.5/tests/test_all_augmenters.py
--rw-r--r--   0 root         (0) root         (0)     1779 2023-05-01 20:20:08.000000 augmenty-1.3.5/tests/test_augmentation_utilities.py
--rw-r--r--   0 root         (0) root         (0)     2280 2023-05-01 20:20:08.000000 augmenty-1.3.5/tests/test_character.py
--rw-r--r--   0 root         (0) root         (0)     2105 2023-05-01 20:20:08.000000 augmenty-1.3.5/tests/test_doc.py
--rw-r--r--   0 root         (0) root         (0)      185 2023-05-01 20:20:08.000000 augmenty-1.3.5/tests/test_general.py
--rw-r--r--   0 root         (0) root         (0)     1717 2023-05-01 20:20:08.000000 augmenty-1.3.5/tests/test_issue_170.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-05-01 20:20:08.000000 augmenty-1.3.5/tests/test_keyboard.py
--rw-r--r--   0 root         (0) root         (0)     3144 2023-05-01 20:20:08.000000 augmenty-1.3.5/tests/test_spans.py
--rw-r--r--   0 root         (0) root         (0)      490 2023-05-01 20:20:08.000000 augmenty-1.3.5/tests/test_static_embedding.py
--rw-r--r--   0 root         (0) root         (0)     7445 2023-05-01 20:20:08.000000 augmenty-1.3.5/tests/test_token.py
--rw-r--r--   0 root         (0) root         (0)      397 2023-05-01 20:20:08.000000 augmenty-1.3.5/tests/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:29:38.303380 augmenty-1.3.6/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:29:38.287380 augmenty-1.3.6/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:29:38.287380 augmenty-1.3.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      729 2023-05-01 22:29:27.000000 augmenty-1.3.6/.github/ISSUE_TEMPLATE/01_bugs.md
+-rw-r--r--   0 root         (0) root         (0)      418 2023-05-01 22:29:27.000000 augmenty-1.3.6/.github/ISSUE_TEMPLATE/02_docs.md
+-rw-r--r--   0 root         (0) root         (0)      291 2023-05-01 22:29:27.000000 augmenty-1.3.6/.github/ISSUE_TEMPLATE/03_feature-request.md
+-rw-r--r--   0 root         (0) root         (0)      283 2023-05-01 22:29:27.000000 augmenty-1.3.6/.github/ISSUE_TEMPLATE/04_augmenter-request.md
+-rw-r--r--   0 root         (0) root         (0)      625 2023-05-01 22:29:27.000000 augmenty-1.3.6/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 root         (0) root         (0)      776 2023-05-01 22:29:27.000000 augmenty-1.3.6/.github/dependabot.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:29:38.287380 augmenty-1.3.6/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1013 2023-05-01 22:29:27.000000 augmenty-1.3.6/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 root         (0) root         (0)     1280 2023-05-01 22:29:27.000000 augmenty-1.3.6/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)     1673 2023-05-01 22:29:27.000000 augmenty-1.3.6/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)     2697 2023-05-01 22:29:27.000000 augmenty-1.3.6/.github/workflows/tests.yml
+-rw-r--r--   0 root         (0) root         (0)      186 2023-05-01 22:29:27.000000 augmenty-1.3.6/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      797 2023-05-01 22:29:27.000000 augmenty-1.3.6/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)     2918 2023-05-01 22:29:28.000000 augmenty-1.3.6/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-05-01 22:29:27.000000 augmenty-1.3.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7212 2023-05-01 22:29:38.303380 augmenty-1.3.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      372 2023-05-01 22:29:27.000000 augmenty-1.3.6/citation.cff
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:29:38.291380 augmenty-1.3.6/docs/
+-rw-r--r--   0 root         (0) root         (0)      634 2023-05-01 22:29:27.000000 augmenty-1.3.6/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:29:38.291380 augmenty-1.3.6/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)     1150 2023-05-01 22:29:27.000000 augmenty-1.3.6/docs/_static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)   385037 2023-05-01 22:29:27.000000 augmenty-1.3.6/docs/_static/icon.png
+-rw-r--r--   0 root         (0) root         (0)   395381 2023-05-01 22:29:27.000000 augmenty-1.3.6/docs/_static/icon_dark.png
+-rw-r--r--   0 root         (0) root         (0)     2308 2023-05-01 22:29:27.000000 augmenty-1.3.6/docs/adding_an_augmenter.rst
+-rw-r--r--   0 root         (0) root         (0)     6366 2023-05-01 22:29:27.000000 augmenty-1.3.6/docs/augmenters_overview.md
+-rw-r--r--   0 root         (0) root         (0)      392 2023-05-01 22:29:27.000000 augmenty-1.3.6/docs/augmenty.augment_utilities.rst
+-rw-r--r--   0 root         (0) root         (0)     1009 2023-05-01 22:29:27.000000 augmenty-1.3.6/docs/augmenty.character.rst
+-rw-r--r--   0 root         (0) root         (0)      733 2023-05-01 22:29:27.000000 augmenty-1.3.6/docs/augmenty.doc.rst
+-rw-r--r--   0 root         (0) root         (0)      409 2023-05-01 22:29:27.000000 augmenty-1.3.6/docs/augmenty.keyboard.rst
+-rw-r--r--   0 root         (0) root         (0)      500 2023-05-01 22:29:27.000000 augmenty-1.3.6/docs/augmenty.lang.rst
+-rw-r--r--   0 root         (0) root         (0)      334 2023-05-01 22:29:27.000000 augmenty-1.3.6/docs/augmenty.span.rst
+-rw-r--r--   0 root         (0) root         (0)     1089 2023-05-01 22:29:27.000000 augmenty-1.3.6/docs/augmenty.token.rst
+-rw-r--r--   0 root         (0) root         (0)      330 2023-05-01 22:29:27.000000 augmenty-1.3.6/docs/augmenty.util.rst
+-rw-r--r--   0 root         (0) root         (0)     4190 2023-05-01 22:29:27.000000 augmenty-1.3.6/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     2561 2023-05-01 22:29:27.000000 augmenty-1.3.6/docs/create_augmenters_table.py
+-rw-r--r--   0 root         (0) root         (0)     3444 2023-05-01 22:29:27.000000 augmenty-1.3.6/docs/faq.rst
+-rw-r--r--   0 root         (0) root         (0)     2578 2023-05-01 22:29:27.000000 augmenty-1.3.6/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     1055 2023-05-01 22:29:27.000000 augmenty-1.3.6/docs/installation.rst
+-rw-r--r--   0 root         (0) root         (0)      795 2023-05-01 22:29:27.000000 augmenty-1.3.6/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)     1149 2023-05-01 22:29:27.000000 augmenty-1.3.6/docs/news.rst
+-rw-r--r--   0 root         (0) root         (0)       61 2023-05-01 22:29:27.000000 augmenty-1.3.6/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:29:38.291380 augmenty-1.3.6/docs/tutorials/
+-rw-r--r--   0 root         (0) root         (0)    15539 2023-05-01 22:29:27.000000 augmenty-1.3.6/docs/tutorials/introduction.ipynb
+-rw-r--r--   0 root         (0) root         (0)      210 2023-05-01 22:29:27.000000 augmenty-1.3.6/docs/tutorials/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:29:38.291380 augmenty-1.3.6/img/
+-rw-r--r--   0 root         (0) root         (0)   385037 2023-05-01 22:29:27.000000 augmenty-1.3.6/img/icon.png
+-rw-r--r--   0 root         (0) root         (0)     3243 2023-05-01 22:29:28.000000 augmenty-1.3.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     4521 2023-05-01 22:29:27.000000 augmenty-1.3.6/readme.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-01 22:29:38.303380 augmenty-1.3.6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:29:38.283380 augmenty-1.3.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:29:38.291380 augmenty-1.3.6/src/augmenty/
+-rw-r--r--   0 root         (0) root         (0)     2053 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      164 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/about.py
+-rw-r--r--   0 root         (0) root         (0)     3336 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/augment_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:29:38.295380 augmenty-1.3.6/src/augmenty/character/
+-rw-r--r--   0 root         (0) root         (0)      355 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/character/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1564 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/character/casing.py
+-rw-r--r--   0 root         (0) root         (0)     4613 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/character/replace.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/character/spacing.py
+-rw-r--r--   0 root         (0) root         (0)     1606 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/character/swap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:29:38.295380 augmenty-1.3.6/src/augmenty/doc/
+-rw-r--r--   0 root         (0) root         (0)      184 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/doc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2666 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/doc/casing.py
+-rw-r--r--   0 root         (0) root         (0)     3887 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/doc/subset.py
+-rw-r--r--   0 root         (0) root         (0)     3509 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:29:38.295380 augmenty-1.3.6/src/augmenty/lang/
+-rw-r--r--   0 root         (0) root         (0)      784 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/lang/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:29:38.295380 augmenty-1.3.6/src/augmenty/lang/da/
+-rw-r--r--   0 root         (0) root         (0)      195 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/lang/da/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1878 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/lang/da/augmenters.py
+-rw-r--r--   0 root         (0) root         (0)      790 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/lang/da/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:29:38.295380 augmenty-1.3.6/src/augmenty/lang/de/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/lang/de/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      783 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/lang/de/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:29:38.295380 augmenty-1.3.6/src/augmenty/lang/el/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/lang/el/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/lang/el/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:29:38.295380 augmenty-1.3.6/src/augmenty/lang/en/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/lang/en/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      776 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/lang/en/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:29:38.295380 augmenty-1.3.6/src/augmenty/lang/es/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/lang/es/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      783 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/lang/es/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:29:38.295380 augmenty-1.3.6/src/augmenty/lang/fr/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/lang/fr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      783 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/lang/fr/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:29:38.295380 augmenty-1.3.6/src/augmenty/lang/hu/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/lang/hu/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      803 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/lang/hu/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:29:38.295380 augmenty-1.3.6/src/augmenty/lang/it/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/lang/it/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      784 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/lang/it/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:29:38.295380 augmenty-1.3.6/src/augmenty/lang/lt/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/lang/lt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      794 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/lang/lt/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:29:38.295380 augmenty-1.3.6/src/augmenty/lang/mk/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/lang/mk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      823 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/lang/mk/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:29:38.299380 augmenty-1.3.6/src/augmenty/lang/nb/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/lang/nb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      784 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/lang/nb/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:29:38.299380 augmenty-1.3.6/src/augmenty/lang/nl/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/lang/nl/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      775 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/lang/nl/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:29:38.299380 augmenty-1.3.6/src/augmenty/lang/pl/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/lang/pl/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      775 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/lang/pl/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:29:38.299380 augmenty-1.3.6/src/augmenty/lang/pt/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/lang/pt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      780 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/lang/pt/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:29:38.299380 augmenty-1.3.6/src/augmenty/lang/ro/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/lang/ro/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      780 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/lang/ro/keyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:29:38.299380 augmenty-1.3.6/src/augmenty/lang/ru/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/lang/ru/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      828 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/lang/ru/keyboard.py
+-rw-r--r--   0 root         (0) root         (0)     8801 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/meta.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:29:38.299380 augmenty-1.3.6/src/augmenty/span/
+-rw-r--r--   0 root         (0) root         (0)      177 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/span/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13569 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/span/entities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:29:38.299380 augmenty-1.3.6/src/augmenty/token/
+-rw-r--r--   0 root         (0) root         (0)      680 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/token/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3967 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/token/casing.py
+-rw-r--r--   0 root         (0) root         (0)    12158 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/token/insert.py
+-rw-r--r--   0 root         (0) root         (0)    11343 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/token/replace.py
+-rw-r--r--   0 root         (0) root         (0)     2951 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/token/spacing.py
+-rw-r--r--   0 root         (0) root         (0)     2325 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/token/static_embedding_util.py
+-rw-r--r--   0 root         (0) root         (0)     4915 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/token/swap.py
+-rw-r--r--   0 root         (0) root         (0)      814 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/token/wordnet_util.py
+-rw-r--r--   0 root         (0) root         (0)     3798 2023-05-01 22:29:27.000000 augmenty-1.3.6/src/augmenty/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:29:38.295380 augmenty-1.3.6/src/augmenty.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7212 2023-05-01 22:29:38.000000 augmenty-1.3.6/src/augmenty.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3423 2023-05-01 22:29:38.000000 augmenty-1.3.6/src/augmenty.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 22:29:38.000000 augmenty-1.3.6/src/augmenty.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      438 2023-05-01 22:29:38.000000 augmenty-1.3.6/src/augmenty.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-01 22:29:38.000000 augmenty-1.3.6/src/augmenty.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:29:38.303380 augmenty-1.3.6/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 22:29:27.000000 augmenty-1.3.6/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20399 2023-05-01 22:29:27.000000 augmenty-1.3.6/tests/books.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-05-01 22:29:27.000000 augmenty-1.3.6/tests/fixtures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 22:29:38.303380 augmenty-1.3.6/tests/lang/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 22:29:27.000000 augmenty-1.3.6/tests/lang/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      999 2023-05-01 22:29:27.000000 augmenty-1.3.6/tests/lang/test_da.py
+-rw-r--r--   0 root         (0) root         (0)      147 2023-05-01 22:29:27.000000 augmenty-1.3.6/tests/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     2960 2023-05-01 22:29:27.000000 augmenty-1.3.6/tests/test_all_augmenters.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2023-05-01 22:29:27.000000 augmenty-1.3.6/tests/test_augmentation_utilities.py
+-rw-r--r--   0 root         (0) root         (0)     2280 2023-05-01 22:29:27.000000 augmenty-1.3.6/tests/test_character.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-05-01 22:29:27.000000 augmenty-1.3.6/tests/test_doc.py
+-rw-r--r--   0 root         (0) root         (0)      185 2023-05-01 22:29:27.000000 augmenty-1.3.6/tests/test_general.py
+-rw-r--r--   0 root         (0) root         (0)     1711 2023-05-01 22:29:27.000000 augmenty-1.3.6/tests/test_issue_170.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-05-01 22:29:27.000000 augmenty-1.3.6/tests/test_keyboard.py
+-rw-r--r--   0 root         (0) root         (0)     3144 2023-05-01 22:29:27.000000 augmenty-1.3.6/tests/test_spans.py
+-rw-r--r--   0 root         (0) root         (0)      490 2023-05-01 22:29:27.000000 augmenty-1.3.6/tests/test_static_embedding.py
+-rw-r--r--   0 root         (0) root         (0)     7445 2023-05-01 22:29:27.000000 augmenty-1.3.6/tests/test_token.py
+-rw-r--r--   0 root         (0) root         (0)      397 2023-05-01 22:29:27.000000 augmenty-1.3.6/tests/test_util.py
```

### Comparing `augmenty-1.3.5/.github/ISSUE_TEMPLATE/01_bugs.md` & `augmenty-1.3.6/.github/ISSUE_TEMPLATE/01_bugs.md`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/.github/ISSUE_TEMPLATE/config.yml` & `augmenty-1.3.6/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/.github/dependabot.yml` & `augmenty-1.3.6/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/.github/workflows/dependabot_automerge.yml` & `augmenty-1.3.6/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/.github/workflows/documentation.yml` & `augmenty-1.3.6/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/.github/workflows/release.yml` & `augmenty-1.3.6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/.github/workflows/tests.yml` & `augmenty-1.3.6/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/.pre-commit-config.yaml` & `augmenty-1.3.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/CHANGELOG.md` & `augmenty-1.3.6/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.3.6 (2023-05-01)
+### Fix
+* Entity augmenter now allows for passing in spans or string ([`faf2abc`](https://github.com/KennethEnevoldsen/augmenty/commit/faf2abcfd05b3efe1a954a4d5e1b09b7c65ae50b))
+
 ## v1.3.5 (2023-05-01)
 ### Fix
 * Removed upper bounds on all dependencies ([`78b6a1d`](https://github.com/KennethEnevoldsen/augmenty/commit/78b6a1dd109e5946b8ba69b3e1215cc6aff328c6))
 
 ## v1.3.4 (2023-05-01)
 ### Fix
 * Handle offset outside "head" annotation scope ([`c02f076`](https://github.com/KennethEnevoldsen/augmenty/commit/c02f076d64ff7e18b5d6a239d2f02a7be966326d))
```

### Comparing `augmenty-1.3.5/LICENSE` & `augmenty-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/PKG-INFO` & `augmenty-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: augmenty
-Version: 1.3.5
+Version: 1.3.6
 Summary: An augmentation library based on SpaCy for joint augmentation of text and labels.
 Author-email: Kenneth Enevoldsen <kennethcenevoldsen@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Kenneth Enevoldsen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: augmenty Version: 1.3.5 Summary: An augmentation
+Metadata-Version: 2.1 Name: augmenty Version: 1.3.6 Summary: An augmentation
 library based on SpaCy for joint augmentation of text and labels. Author-email:
 Kenneth Enevoldsen
 gmail.com> License: MIT License Copyright (c) 2021 Kenneth Enevoldsen
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

### Comparing `augmenty-1.3.5/docs/Makefile` & `augmenty-1.3.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/docs/_static/favicon.ico` & `augmenty-1.3.6/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/docs/_static/icon.png` & `augmenty-1.3.6/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/docs/_static/icon_dark.png` & `augmenty-1.3.6/docs/_static/icon_dark.png`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/docs/adding_an_augmenter.rst` & `augmenty-1.3.6/docs/adding_an_augmenter.rst`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/docs/augmenters_overview.md` & `augmenty-1.3.6/docs/augmenters_overview.md`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/docs/augmenty.character.rst` & `augmenty-1.3.6/docs/augmenty.character.rst`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/docs/augmenty.doc.rst` & `augmenty-1.3.6/docs/augmenty.doc.rst`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/docs/augmenty.token.rst` & `augmenty-1.3.6/docs/augmenty.token.rst`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/docs/conf.py` & `augmenty-1.3.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/docs/create_augmenters_table.py` & `augmenty-1.3.6/docs/create_augmenters_table.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/docs/faq.rst` & `augmenty-1.3.6/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/docs/index.rst` & `augmenty-1.3.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/docs/installation.rst` & `augmenty-1.3.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/docs/make.bat` & `augmenty-1.3.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/docs/news.rst` & `augmenty-1.3.6/docs/news.rst`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/docs/tutorials/introduction.ipynb` & `augmenty-1.3.6/docs/tutorials/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/img/icon.png` & `augmenty-1.3.6/img/icon.png`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/pyproject.toml` & `augmenty-1.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "augmenty"
-version = "1.3.5"
+version = "1.3.6"
 description = "An augmentation library based on SpaCy for joint augmentation of text and labels."
 authors = [{name = "Kenneth Enevoldsen", email = "kennethcenevoldsen@gmail.com"}]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
```

### Comparing `augmenty-1.3.5/readme.md` & `augmenty-1.3.6/readme.md`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/__init__.py` & `augmenty-1.3.6/src/augmenty/__init__.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/augment_utilities.py` & `augmenty-1.3.6/src/augmenty/augment_utilities.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/character/casing.py` & `augmenty-1.3.6/src/augmenty/character/casing.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/character/replace.py` & `augmenty-1.3.6/src/augmenty/character/replace.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/character/spacing.py` & `augmenty-1.3.6/src/augmenty/character/spacing.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/character/swap.py` & `augmenty-1.3.6/src/augmenty/character/swap.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/doc/casing.py` & `augmenty-1.3.6/src/augmenty/doc/casing.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/doc/subset.py` & `augmenty-1.3.6/src/augmenty/doc/subset.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/keyboard.py` & `augmenty-1.3.6/src/augmenty/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/lang/__init__.py` & `augmenty-1.3.6/src/augmenty/lang/__init__.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/lang/da/augmenters.py` & `augmenty-1.3.6/src/augmenty/lang/da/augmenters.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/lang/da/keyboard.py` & `augmenty-1.3.6/src/augmenty/lang/da/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/lang/de/keyboard.py` & `augmenty-1.3.6/src/augmenty/lang/de/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/lang/el/keyboard.py` & `augmenty-1.3.6/src/augmenty/lang/el/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/lang/en/keyboard.py` & `augmenty-1.3.6/src/augmenty/lang/en/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/lang/es/keyboard.py` & `augmenty-1.3.6/src/augmenty/lang/es/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/lang/fr/keyboard.py` & `augmenty-1.3.6/src/augmenty/lang/fr/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/lang/hu/keyboard.py` & `augmenty-1.3.6/src/augmenty/lang/hu/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/lang/it/keyboard.py` & `augmenty-1.3.6/src/augmenty/lang/it/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/lang/lt/keyboard.py` & `augmenty-1.3.6/src/augmenty/lang/lt/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/lang/mk/keyboard.py` & `augmenty-1.3.6/src/augmenty/lang/mk/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/lang/nb/keyboard.py` & `augmenty-1.3.6/src/augmenty/lang/nb/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/lang/nl/keyboard.py` & `augmenty-1.3.6/src/augmenty/lang/nl/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/lang/pl/keyboard.py` & `augmenty-1.3.6/src/augmenty/lang/pl/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/lang/pt/keyboard.py` & `augmenty-1.3.6/src/augmenty/lang/pt/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/lang/ro/keyboard.py` & `augmenty-1.3.6/src/augmenty/lang/ro/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/lang/ru/keyboard.py` & `augmenty-1.3.6/src/augmenty/lang/ru/keyboard.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/meta.json` & `augmenty-1.3.6/src/augmenty/meta.json`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/span/entities.py` & `augmenty-1.3.6/src/augmenty/span/entities.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,95 @@
 import random
 from functools import partial
-from typing import Callable, Dict, Generator, Iterable, Iterator, List, Optional, Union
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Generator,
+    Iterable,
+    Iterator,
+    List,
+    Optional,
+    Union,
+)
 
 import numpy as np
-import spacy
 from spacy.language import Language
-from spacy.tokens import Token
+from spacy.tokens import Span, Token
 from spacy.training import Example
+from spacy.util import registry
 
 from ..augment_utilities import make_text_from_orth
 
+# create entity type
+ENTITY = Union[str, List[str], Span]
+
+
+def __normalize_entity(entity: ENTITY, nlp: Language) -> Dict[str, List[Any]]:
+    spacy = None
+    pos = None
+    tag = None
+    morph = None
+    lemma = None
+
+    if isinstance(entity, str):
+        ent_doc = nlp(entity)
+        orth = [tok.text for tok in ent_doc]
+        spacy = [tok.whitespace_ for tok in ent_doc]
+    elif isinstance(entity, list):
+        orth = entity
+    elif isinstance(entity, Span):
+        orth = [tok.text for tok in entity]
+        spacy = [tok.whitespace_ for tok in entity]
+        pos = [tok.pos_ for tok in entity]
+        tag = [tok.tag_ for tok in entity]
+        morph = [tok.morph for tok in entity]
+        lemma = [tok.lemma_ for tok in entity]
+    else:
+        raise ValueError(
+            f"entity must be of type str, List[str] or Span, not {type(entity)}",
+        )
+    # if not specifed use default values
+    if spacy is None:
+        spacy = [True] * len(orth)
+    if pos is None:
+        pos = ["PROPN"] * len(orth)
+    if tag is None:
+        tag = ["PROPN"] * len(orth)
+    if morph is None:
+        morph = [""] * len(orth)
+    if lemma is None:
+        lemma = orth
+
+    return {
+        "ORTH": orth,
+        "SPACY": spacy,
+        "POS": pos,
+        "TAG": tag,
+        "MORPH": morph,
+        "LEMMA": lemma,
+    }
+
 
 def ent_augmenter_v1(
     nlp: Language,
     example: Example,
     level: float,
-    ent_dict: Dict[str, Iterable[List[str]]],
+    ent_dict: Dict[str, Iterable[ENTITY]],
     replace_consistency: bool,
     resolve_dependencies: bool,
 ) -> Iterator[Example]:
-    replaced_ents = {}  # type: Dict[str, List[str]]
+    replaced_ents: Dict[str, ENTITY] = {}
     example_dict = example.to_dict()
 
     offset = 0
 
     tok_anno = example_dict["token_annotation"]
     ents = example_dict["doc_annotation"]["entities"]
-    if example.y.has_annotation("HEAD"):
+    if example.y.has_annotation("HEAD") and resolve_dependencies:
         head = np.array(tok_anno["HEAD"])
 
     for ent in example.y.ents:
         if ent.label_ in ent_dict and random.random() < level:
             if replace_consistency and ent.text in replaced_ents:
                 new_ent = replaced_ents[ent.text]
             else:
@@ -39,32 +98,36 @@
                 else:
                     new_ent = random.sample(ent_dict[ent.label_], k=1)[  # type: ignore
                         0
                     ]
                 if replace_consistency:
                     replaced_ents[ent.text] = new_ent
 
+            normalized_ent = __normalize_entity(new_ent, nlp)
+            new_ent = normalized_ent["ORTH"]
+            spacing = normalized_ent["SPACY"]
+
             # Handle token annotations
             len_ent = len(new_ent)
             i = slice(ent.start + offset, ent.end + offset)
             tok_anno["ORTH"][i] = new_ent
-            tok_anno["LEMMA"][i] = new_ent
+            tok_anno["LEMMA"][i] = normalized_ent["LEMMA"]
 
-            tok_anno["TAG"][i] = ["PROPN"] * len_ent
-            tok_anno["POS"][i] = ["PROPN"] * len_ent
+            tok_anno["POS"][i] = normalized_ent["POS"]
+            tok_anno["TAG"][i] = normalized_ent["TAG"]
 
-            tok_anno["MORPH"][i] = [""] * len_ent
+            tok_anno["MORPH"][i] = normalized_ent["MORPH"]
             tok_anno["DEP"][i] = [ent[0].dep_] + ["flat"] * (len_ent - 1)
 
             # Set sentence start based on first token in previous entity
             tok_anno["SENT_START"][i] = [ent[0].sent_start] + [0] * (len_ent - 1)
 
-            # set spacing to be whitespace for all tokens except the last one
-            # which is set based on the original entity
-            tok_anno["SPACY"][i] = [True] * (len_ent - 1) + [bool(ent[-1].whitespace_)]
+            # set the last spacing to be equal to the last token spacing in the previous entity
+            spacing[-1:] = [ent[-1].whitespace_]
+            tok_anno["SPACY"][i] = spacing
 
             offset_ = len_ent - (ent.end - ent.start)
             if example.y.has_annotation("HEAD") and resolve_dependencies:
                 # Handle HEAD
 
                 head[head > ent.start + offset] += offset_
                 # keep first head correcting for changing entity size, set rest to
@@ -98,30 +161,32 @@
 
     text = make_text_from_orth(example_dict)
 
     doc = nlp.make_doc(text)
     yield Example.from_dict(doc, example_dict)
 
 
-@spacy.registry.augmenters("ents_replace_v1")
+@registry.augmenters("ents_replace_v1")
 def create_ent_augmenter_v1(
     level: float,
-    ent_dict: Dict[str, Iterable[List[str]]],
+    ent_dict: Dict[str, Iterable[ENTITY]],
     replace_consistency: bool = True,
     resolve_dependencies: bool = True,
 ) -> Callable[[Language, Example], Iterator[Example]]:
     """Create an augmenter which replaces an entity based on a dictionary
     lookup.
 
     Args:
         level: the percentage of entities to be augmented.
         ent_dict: A dictionary with keys corresponding
             the the entity type you wish to replace (e.g. "PER") and a itarable of the
-            replacements. A replacement is a list of string of the desired entity
-            replacement ["Kenneth", "Enevoldsen"].
+            replacements entities. A replacement can be either 1) a list of string of the desired entity
+            i.e. ["Kenneth", "Enevoldsen"], 2) a string of the desired entity i.e. "Kenneth Enevoldsen", this
+            will be split using the tokenizer of the nlp pipeline, or 3) Span object with the desired entity, here all information will be passed
+            on except for the dependency tree.
         replace_consistency: Should an entity always be replaced with
             the same entity? Defaults to True.
         resolve_dependencies: Attempts to resolve the dependency tree
             by setting head of the original entitity aa the head of the
             first token in the new entity. The remainder is the passed as
     Returns:
         The augmenter
@@ -156,15 +221,15 @@
         i = np.random.choice(lp, size=1, replace=True, p=patterns_p)[0]
         yield [
             str(np.random.choice(names[p], size=1, replace=True, p=names_p.get(p))[0])
             for p in patterns[i]
         ]
 
 
-@spacy.registry.augmenters("per_replace_v1")
+@registry.augmenters("per_replace_v1")
 def create_per_replace_augmenter_v1(
     names: Dict[
         str,
         List[str],
     ],  # {"firstname": ["Kenneth", "Lasse"], "lastname": ["Enevoldsen", "Hansen"]}
     patterns: List[List[str]],  # ["firstname", "firstname", "lastname"]
     level: float,
@@ -252,15 +317,15 @@
 
     text = make_text_from_orth(example_dict)
 
     doc = nlp.make_doc(text)
     yield Example.from_dict(doc, example_dict)
 
 
-@spacy.registry.augmenters("ents_format_v1")
+@registry.augmenters("ents_format_v1")
 def create_ent_format_augmenter_v1(
     reordering: List[Union[int, None]],
     formatter: List[Union[Callable[[Token], str], None]],
     level: float,
     ent_types: Optional[List[str]] = None,
 ) -> Callable[[Language, Example], Iterator[Example]]:
     """Creates an augmenter which reorders and formats a entity according to
```

### Comparing `augmenty-1.3.5/src/augmenty/token/__init__.py` & `augmenty-1.3.6/src/augmenty/token/__init__.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/token/casing.py` & `augmenty-1.3.6/src/augmenty/token/casing.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/token/insert.py` & `augmenty-1.3.6/src/augmenty/token/insert.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/token/replace.py` & `augmenty-1.3.6/src/augmenty/token/replace.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/token/spacing.py` & `augmenty-1.3.6/src/augmenty/token/spacing.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/token/static_embedding_util.py` & `augmenty-1.3.6/src/augmenty/token/static_embedding_util.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/token/swap.py` & `augmenty-1.3.6/src/augmenty/token/swap.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/token/wordnet_util.py` & `augmenty-1.3.6/src/augmenty/token/wordnet_util.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty/util.py` & `augmenty-1.3.6/src/augmenty/util.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/src/augmenty.egg-info/PKG-INFO` & `augmenty-1.3.6/src/augmenty.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: augmenty
-Version: 1.3.5
+Version: 1.3.6
 Summary: An augmentation library based on SpaCy for joint augmentation of text and labels.
 Author-email: Kenneth Enevoldsen <kennethcenevoldsen@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Kenneth Enevoldsen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: augmenty Version: 1.3.5 Summary: An augmentation
+Metadata-Version: 2.1 Name: augmenty Version: 1.3.6 Summary: An augmentation
 library based on SpaCy for joint augmentation of text and labels. Author-email:
 Kenneth Enevoldsen
 gmail.com> License: MIT License Copyright (c) 2021 Kenneth Enevoldsen
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

### Comparing `augmenty-1.3.5/src/augmenty.egg-info/SOURCES.txt` & `augmenty-1.3.6/src/augmenty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/tests/books.py` & `augmenty-1.3.6/tests/books.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/tests/fixtures.py` & `augmenty-1.3.6/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/tests/lang/test_da.py` & `augmenty-1.3.6/tests/lang/test_da.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/tests/test_all_augmenters.py` & `augmenty-1.3.6/tests/test_all_augmenters.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/tests/test_augmentation_utilities.py` & `augmenty-1.3.6/tests/test_augmentation_utilities.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/tests/test_character.py` & `augmenty-1.3.6/tests/test_character.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/tests/test_doc.py` & `augmenty-1.3.6/tests/test_doc.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/tests/test_issue_170.py` & `augmenty-1.3.6/tests/test_issue_170.py`

 * *Files 12% similar despite different names*

```diff
@@ -54,21 +54,21 @@
     assert len(list(doc.sents)) == 2
     return doc
 
 
 def test_entity_with_no_dep(nlp, example_doc: Doc):
     level = 1.0
     docs = [example_doc]
-    ents_as_str = ["Melvin R. Brown"]
     augmenter = augmenty.load(
         "ents_replace_v1",
         level=level,
-        ent_dict={"pers": [[s] for s in ents_as_str]},
+        ent_dict={"pers": ["Melvin R. Brown"]},
         replace_consistency=True,
         resolve_dependencies=True,
     )
     aug_doc = list(augmenty.docs(docs, augmenter, nlp))[0]
     assert len(aug_doc.ents) == len(docs[0].ents)
     assert (
         aug_doc.text
         == "Melvin R. Brown and Melvin R. Brown (concussion protocol) are each progressing. SS Melvin R. Brown"
     )
+    assert aug_doc[0].text == "Melvin"
```

### Comparing `augmenty-1.3.5/tests/test_spans.py` & `augmenty-1.3.6/tests/test_spans.py`

 * *Files identical despite different names*

### Comparing `augmenty-1.3.5/tests/test_token.py` & `augmenty-1.3.6/tests/test_token.py`

 * *Files identical despite different names*

