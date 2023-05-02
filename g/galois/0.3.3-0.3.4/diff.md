# Comparing `tmp/galois-0.3.3.tar.gz` & `tmp/galois-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galois/galois/dist/.tmp-x229jcv2/galois-0.3.3.tar", last modified: Wed Feb  1 15:45:23 2023, max compression
+gzip compressed data, was "/home/runner/work/galois/galois/dist/.tmp-8tqaql7k/galois-0.3.4.tar", last modified: Tue May  2 20:40:23 2023, max compression
```

## Comparing `galois-0.3.3.tar` & `galois-0.3.4.tar`

### file list

```diff
@@ -1,1386 +1,1387 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-02-01 15:44:59.000000 galois-0.3.3/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-02-01 15:44:59.000000 galois-0.3.3/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-02-01 15:44:59.000000 galois-0.3.3/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-02-01 15:44:59.000000 galois-0.3.3/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-02-01 15:44:59.000000 galois-0.3.3/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-02-01 15:44:59.000000 galois-0.3.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-02-01 15:44:59.000000 galois-0.3.3/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-02-01 15:44:59.000000 galois-0.3.3/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-02-01 15:44:59.000000 galois-0.3.3/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-02-01 15:44:59.000000 galois-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-01 15:44:59.000000 galois-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-02-01 15:45:23.000000 galois-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-02-01 15:44:59.000000 galois-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-02-01 15:44:59.000000 galois-0.3.3/benchmarks/test_fec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-02-01 15:44:59.000000 galois-0.3.3/benchmarks/test_field_arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-01 15:44:59.000000 galois-0.3.3/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-01 15:44:59.000000 galois-0.3.3/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-02-01 15:44:59.000000 galois-0.3.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-02-01 15:44:59.000000 galois-0.3.3/docs/_static/extra.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-02-01 15:44:59.000000 galois-0.3.3/docs/_templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-02-01 15:44:59.000000 galois-0.3.3/docs/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/docs/basic-usage/
--rw-r--r--   0 runner    (1001) docker     (123)    11301 2023-02-01 15:44:59.000000 galois-0.3.3/docs/basic-usage/array-arithmetic.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-02-01 15:44:59.000000 galois-0.3.3/docs/basic-usage/array-classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-02-01 15:44:59.000000 galois-0.3.3/docs/basic-usage/array-creation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-02-01 15:44:59.000000 galois-0.3.3/docs/basic-usage/compilation-modes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-02-01 15:44:59.000000 galois-0.3.3/docs/basic-usage/element-representation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-02-01 15:44:59.000000 galois-0.3.3/docs/basic-usage/poly-arithmetic.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-02-01 15:44:59.000000 galois-0.3.3/docs/basic-usage/poly.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14987 2023-02-01 15:44:59.000000 galois-0.3.3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/docs/development/
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-02-01 15:44:59.000000 galois-0.3.3/docs/development/documentation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-02-01 15:44:59.000000 galois-0.3.3/docs/development/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-02-01 15:44:59.000000 galois-0.3.3/docs/development/linter.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-02-01 15:44:59.000000 galois-0.3.3/docs/development/unit-tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-01 15:44:59.000000 galois-0.3.3/docs/genindex.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-02-01 15:44:59.000000 galois-0.3.3/docs/getting-started.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-02-01 15:44:59.000000 galois-0.3.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-02-01 15:44:59.000000 galois-0.3.3/docs/ipython_with_reprs.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-02-01 15:44:59.000000 galois-0.3.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/docs/performance/
--rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-02-01 15:44:59.000000 galois-0.3.3/docs/performance/benchmarks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-02-01 15:44:59.000000 galois-0.3.3/docs/performance/binary-extension-fields.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-02-01 15:44:59.000000 galois-0.3.3/docs/performance/prime-fields.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/docs/release-notes/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-02-01 15:44:59.000000 galois-0.3.3/docs/release-notes/v0.0.14.md
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-02-01 15:44:59.000000 galois-0.3.3/docs/release-notes/v0.0.15.md
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-02-01 15:44:59.000000 galois-0.3.3/docs/release-notes/v0.0.16.md
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-02-01 15:44:59.000000 galois-0.3.3/docs/release-notes/v0.0.17.md
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-02-01 15:44:59.000000 galois-0.3.3/docs/release-notes/v0.0.18.md
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-02-01 15:44:59.000000 galois-0.3.3/docs/release-notes/v0.0.19.md
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-02-01 15:44:59.000000 galois-0.3.3/docs/release-notes/v0.0.20.md
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-02-01 15:44:59.000000 galois-0.3.3/docs/release-notes/v0.0.21.md
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-02-01 15:44:59.000000 galois-0.3.3/docs/release-notes/v0.0.22.md
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-02-01 15:44:59.000000 galois-0.3.3/docs/release-notes/v0.0.23.md
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-02-01 15:44:59.000000 galois-0.3.3/docs/release-notes/v0.0.24.md
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-02-01 15:44:59.000000 galois-0.3.3/docs/release-notes/v0.0.25.md
--rw-r--r--   0 runner    (1001) docker     (123)     7148 2023-02-01 15:44:59.000000 galois-0.3.3/docs/release-notes/v0.0.26.md
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-02-01 15:44:59.000000 galois-0.3.3/docs/release-notes/v0.0.27.md
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-02-01 15:44:59.000000 galois-0.3.3/docs/release-notes/v0.0.28.md
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-02-01 15:44:59.000000 galois-0.3.3/docs/release-notes/v0.0.29.md
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-02-01 15:44:59.000000 galois-0.3.3/docs/release-notes/v0.0.30.md
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-02-01 15:44:59.000000 galois-0.3.3/docs/release-notes/v0.0.31.md
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-02-01 15:44:59.000000 galois-0.3.3/docs/release-notes/v0.0.32.md
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-02-01 15:44:59.000000 galois-0.3.3/docs/release-notes/v0.0.33.md
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-02-01 15:44:59.000000 galois-0.3.3/docs/release-notes/v0.1.0.md
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-02-01 15:44:59.000000 galois-0.3.3/docs/release-notes/v0.1.1.md
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-02-01 15:44:59.000000 galois-0.3.3/docs/release-notes/v0.1.2.md
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-02-01 15:44:59.000000 galois-0.3.3/docs/release-notes/v0.2.0.md
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-02-01 15:44:59.000000 galois-0.3.3/docs/release-notes/v0.3.0.md
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-02-01 15:44:59.000000 galois-0.3.3/docs/release-notes/v0.3.1.md
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-02-01 15:44:59.000000 galois-0.3.3/docs/release-notes/v0.3.2.md
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-02-01 15:44:59.000000 galois-0.3.3/docs/release-notes/v0.3.3.md
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-02-01 15:44:59.000000 galois-0.3.3/docs/release-notes/versioning.rst
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-01 15:44:59.000000 galois-0.3.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-02-01 15:44:59.000000 galois-0.3.3/docs/tutorials/intro-to-extension-fields.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10120 2023-02-01 15:44:59.000000 galois-0.3.3/docs/tutorials/intro-to-prime-fields.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/logo/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-02-01 15:44:59.000000 galois-0.3.3/logo/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    24465 2023-02-01 15:44:59.000000 galois-0.3.3/logo/galois-favicon-color.png
--rw-r--r--   0 runner    (1001) docker     (123)    20786 2023-02-01 15:44:59.000000 galois-0.3.3/logo/galois-favicon-white.png
--rw-r--r--   0 runner    (1001) docker     (123)    81221 2023-02-01 15:44:59.000000 galois-0.3.3/logo/galois-github-social.png
--rw-r--r--   0 runner    (1001) docker     (123)    16252 2023-02-01 15:44:59.000000 galois-0.3.3/logo/galois-github-social.svg
--rw-r--r--   0 runner    (1001) docker     (123)   105002 2023-02-01 15:44:59.000000 galois-0.3.3/logo/galois-heading.png
--rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-02-01 15:44:59.000000 galois-0.3.3/logo/galois-logo-small.png
--rw-r--r--   0 runner    (1001) docker     (123)    54587 2023-02-01 15:44:59.000000 galois-0.3.3/logo/galois-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    15396 2023-02-01 15:44:59.000000 galois-0.3.3/logo/galois-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-02-01 15:44:59.000000 galois-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-02-01 15:44:59.000000 galois-0.3.3/requirements-min.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-02-01 15:44:59.000000 galois-0.3.3/scripts/create_conway_polys_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-02-01 15:44:59.000000 galois-0.3.3/scripts/create_irreducible_polys_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    22092 2023-02-01 15:44:59.000000 galois-0.3.3/scripts/create_prime_factors_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    12618 2023-02-01 15:44:59.000000 galois-0.3.3/scripts/generate_fec_test_vectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    38108 2023-02-01 15:44:59.000000 galois-0.3.3/scripts/generate_field_test_vectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-02-01 15:44:59.000000 galois-0.3.3/scripts/generate_int_test_vectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-02-01 15:44:59.000000 galois-0.3.3/scripts/sparse_poly_performance_test.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-01 15:45:23.000000 galois-0.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/src/galois/
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/src/galois/_codes/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_codes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44262 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_codes/_bch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7953 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_codes/_cyclic.py
--rw-r--r--   0 runner    (1001) docker     (123)    15946 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_codes/_linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    33742 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_codes/_reed_solomon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/src/galois/_databases/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_databases/_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)  1552384 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_databases/conway_polys.db
--rw-r--r--   0 runner    (1001) docker     (123)   466944 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_databases/irreducible_polys.db
--rw-r--r--   0 runner    (1001) docker     (123)  8187904 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_databases/prime_factors.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/src/galois/_domains/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_domains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18547 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_domains/_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    26170 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_domains/_calculate.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_domains/_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    12633 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_domains/_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_domains/_linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_domains/_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_domains/_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    26519 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_domains/_ufunc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/src/galois/_fields/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71788 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_fields/_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    19170 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_fields/_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_fields/_gf2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19641 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_fields/_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_fields/_primitive_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_fields/_ufunc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    53456 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_lfsr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_math.py
--rw-r--r--   0 runner    (1001) docker     (123)    26121 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_modular.py
--rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_ntt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    22544 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_polymorphic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/src/galois/_polys/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_polys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_polys/_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_polys/_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13776 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_polys/_conway.py
--rw-r--r--   0 runner    (1001) docker     (123)    16083 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_polys/_dense.py
--rw-r--r--   0 runner    (1001) docker     (123)    15179 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_polys/_factor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_polys/_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14389 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_polys/_irreducible.py
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_polys/_lagrange.py
--rw-r--r--   0 runner    (1001) docker     (123)    66636 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_polys/_poly.py
--rw-r--r--   0 runner    (1001) docker     (123)    16356 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_polys/_primitive.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_polys/_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_polys/_sparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    51256 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/_prime.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-01 15:45:22.000000 galois-0.3.3/src/galois/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-02-01 15:44:59.000000 galois-0.3.3/src/galois/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/src/galois.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-02-01 15:45:23.000000 galois-0.3.3/src/galois.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    57311 2023-02-01 15:45:23.000000 galois-0.3.3/src/galois.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 15:45:23.000000 galois-0.3.3/src/galois.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-02-01 15:45:23.000000 galois-0.3.3/src/galois.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-01 15:45:23.000000 galois-0.3.3/src/galois.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 15:44:59.000000 galois-0.3.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/codes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/codes/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/codes/data/bch/
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k10_d2_alpha6_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k10_d2_alpha6_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k10_d2_alpha9_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k10_d2_alpha9_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k10_d2_alpha9_c3_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k10_d2_alpha9_c3_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k13_d1_alpha6_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k13_d1_alpha6_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k13_d1_alpha9_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k13_d1_alpha9_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k13_d1_alpha9_c3_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k13_d1_alpha9_c3_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k1_d6_alpha9_c3_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k1_d6_alpha9_c3_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k1_d7_alpha9_c3_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k1_d7_alpha9_c3_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k1_d8_alpha6_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k1_d8_alpha6_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k1_d8_alpha9_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k1_d8_alpha9_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k1_d8_alpha9_c3_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k1_d8_alpha9_c3_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k4_d4_alpha9_c3_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k4_d4_alpha9_c3_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k4_d5_alpha6_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k4_d5_alpha6_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k4_d5_alpha9_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k4_d5_alpha9_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k4_d5_alpha9_c3_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k4_d5_alpha9_c3_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k4_d6_alpha6_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k4_d6_alpha6_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k4_d6_alpha9_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k4_d6_alpha9_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k4_d7_alpha6_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k4_d7_alpha6_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k4_d7_alpha9_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k4_d7_alpha9_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k7_d3_alpha6_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k7_d3_alpha6_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k7_d3_alpha9_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k7_d3_alpha9_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k7_d3_alpha9_c3_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k7_d3_alpha9_c3_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k7_d4_alpha6_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k7_d4_alpha6_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k7_d4_alpha9_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n13_k7_d4_alpha9_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k11_d2_alpha2_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k11_d2_alpha2_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k11_d2_alpha2_c3_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k11_d2_alpha2_c3_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k11_d2_alpha9_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k11_d2_alpha9_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k11_d3_alpha2_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k11_d3_alpha2_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k11_d3_alpha9_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k11_d3_alpha9_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k15_d1_alpha2_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k15_d1_alpha2_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k15_d1_alpha2_c3_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k15_d1_alpha2_c3_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k15_d1_alpha9_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k15_d1_alpha9_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k1_d6_alpha2_c3_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k1_d6_alpha2_c3_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k1_d7_alpha2_c3_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k1_d7_alpha2_c3_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k1_d8_alpha2_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k1_d8_alpha2_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k1_d8_alpha2_c3_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k1_d8_alpha2_c3_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k1_d8_alpha9_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k1_d8_alpha9_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k5_d4_alpha2_c3_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k5_d4_alpha2_c3_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k5_d5_alpha2_c3_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k5_d5_alpha2_c3_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k5_d6_alpha2_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k5_d6_alpha2_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k5_d6_alpha9_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k5_d6_alpha9_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k5_d7_alpha2_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k5_d7_alpha2_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k5_d7_alpha9_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k5_d7_alpha9_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k7_d3_alpha2_c3_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k7_d3_alpha2_c3_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k7_d4_alpha2_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k7_d4_alpha2_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k7_d4_alpha9_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k7_d4_alpha9_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k7_d5_alpha2_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k7_d5_alpha2_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k7_d5_alpha9_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n15_k7_d5_alpha9_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8962 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k11_d6_alpha3_c3_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k11_d6_alpha3_c3_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k11_d8_alpha17_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10439 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k11_d8_alpha17_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8962 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k11_d8_alpha3_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10878 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k11_d8_alpha3_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k14_d5_alpha3_c3_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    11684 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k14_d5_alpha3_c3_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k14_d6_alpha17_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    12498 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k14_d6_alpha17_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k14_d6_alpha3_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k14_d6_alpha3_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k14_d7_alpha17_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10415 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k14_d7_alpha17_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k14_d7_alpha3_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10401 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k14_d7_alpha3_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k17_d4_alpha3_c3_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10399 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k17_d4_alpha3_c3_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k17_d5_alpha17_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    12990 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k17_d5_alpha17_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k17_d5_alpha3_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k17_d5_alpha3_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k1_d16_alpha3_c3_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k1_d16_alpha3_c3_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k1_d17_alpha3_c3_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k1_d17_alpha3_c3_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k1_d18_alpha17_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k1_d18_alpha17_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k1_d18_alpha3_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k1_d18_alpha3_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k1_d18_alpha3_c3_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k1_d18_alpha3_c3_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k20_d3_alpha17_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    11218 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k20_d3_alpha17_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k20_d3_alpha3_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    12970 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k20_d3_alpha3_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k20_d3_alpha3_c3_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k20_d3_alpha3_c3_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k20_d4_alpha17_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    11218 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k20_d4_alpha17_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k20_d4_alpha3_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    13290 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k20_d4_alpha3_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k23_d2_alpha17_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    13147 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k23_d2_alpha17_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k23_d2_alpha3_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    12021 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k23_d2_alpha3_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k23_d2_alpha3_c3_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k23_d2_alpha3_c3_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k26_d1_alpha17_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k26_d1_alpha17_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k26_d1_alpha3_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k26_d1_alpha3_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k26_d1_alpha3_c3_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k26_d1_alpha3_c3_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k4_d13_alpha3_c3_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10743 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k4_d13_alpha3_c3_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k4_d14_alpha3_c3_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10423 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k4_d14_alpha3_c3_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k4_d15_alpha17_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10904 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k4_d15_alpha17_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k4_d15_alpha3_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10423 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k4_d15_alpha3_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k4_d15_alpha3_c3_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10583 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k4_d15_alpha3_c3_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k4_d16_alpha17_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10741 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k4_d16_alpha17_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k4_d16_alpha3_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10583 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k4_d16_alpha3_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k4_d17_alpha17_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10904 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k4_d17_alpha17_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k4_d17_alpha3_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10743 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k4_d17_alpha3_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k7_d12_alpha3_c3_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k7_d12_alpha3_c3_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k7_d14_alpha17_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    11047 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k7_d14_alpha17_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k7_d14_alpha3_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k7_d14_alpha3_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k8_d10_alpha17_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k8_d10_alpha17_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k8_d10_alpha3_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k8_d10_alpha3_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k8_d10_alpha3_c3_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k8_d10_alpha3_c3_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k8_d11_alpha17_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10566 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k8_d11_alpha17_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k8_d11_alpha3_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10420 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k8_d11_alpha3_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k8_d11_alpha3_c3_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k8_d11_alpha3_c3_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k8_d12_alpha17_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10566 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k8_d12_alpha17_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k8_d12_alpha3_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k8_d12_alpha3_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k8_d13_alpha17_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k8_d13_alpha17_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k8_d13_alpha3_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10740 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k8_d13_alpha3_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k8_d7_alpha3_c3_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10740 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k8_d7_alpha3_c3_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k8_d8_alpha3_c3_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10580 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k8_d8_alpha3_c3_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k8_d9_alpha17_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    11369 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k8_d9_alpha17_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k8_d9_alpha3_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10580 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k8_d9_alpha3_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k8_d9_alpha3_c3_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/bch/n26_k8_d9_alpha3_c3_sys.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/codes/data/reed_solomon/
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n15_k10_d6_alpha2_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n15_k10_d6_alpha2_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n15_k10_d6_alpha9_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n15_k10_d6_alpha9_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n15_k11_d5_alpha2_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n15_k11_d5_alpha2_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n15_k11_d5_alpha9_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n15_k11_d5_alpha9_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n15_k12_d4_alpha2_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n15_k12_d4_alpha2_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n15_k12_d4_alpha9_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n15_k12_d4_alpha9_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n15_k13_d3_alpha2_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n15_k13_d3_alpha2_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n15_k13_d3_alpha9_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n15_k13_d3_alpha9_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n15_k14_d2_alpha2_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n15_k14_d2_alpha2_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n15_k14_d2_alpha9_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n15_k14_d2_alpha9_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n15_k8_d8_alpha2_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n15_k8_d8_alpha2_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n15_k8_d8_alpha9_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n15_k8_d8_alpha9_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n15_k9_d7_alpha2_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n15_k9_d7_alpha2_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n15_k9_d7_alpha9_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n15_k9_d7_alpha9_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n16_k10_d7_alpha11_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n16_k10_d7_alpha11_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n16_k10_d7_alpha31_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6613 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n16_k10_d7_alpha31_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n16_k11_d6_alpha11_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n16_k11_d6_alpha11_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n16_k11_d6_alpha31_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n16_k11_d6_alpha31_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n16_k12_d5_alpha11_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n16_k12_d5_alpha11_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n16_k12_d5_alpha31_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n16_k12_d5_alpha31_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n16_k13_d4_alpha11_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n16_k13_d4_alpha11_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n16_k13_d4_alpha31_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n16_k13_d4_alpha31_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n16_k14_d3_alpha11_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n16_k14_d3_alpha11_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n16_k14_d3_alpha31_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n16_k14_d3_alpha31_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n16_k15_d2_alpha11_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n16_k15_d2_alpha11_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n16_k15_d2_alpha31_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n16_k15_d2_alpha31_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n16_k9_d8_alpha11_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n16_k9_d8_alpha11_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n16_k9_d8_alpha31_c1_nonsys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/data/reed_solomon/n16_k9_d8_alpha31_c1_sys.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     9887 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/test_bch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-02-01 15:44:59.000000 galois-0.3.3/tests/codes/test_reed_solomon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-02-01 15:44:59.000000 galois-0.3.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-02-01 15:44:59.000000 galois-0.3.3/tests/data/carmichael_lambda.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-02-01 15:44:59.000000 galois-0.3.3/tests/data/crt.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-02-01 15:44:59.000000 galois-0.3.3/tests/data/egcd.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-02-01 15:44:59.000000 galois-0.3.3/tests/data/euler_phi.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-02-01 15:44:59.000000 galois-0.3.3/tests/data/ilog.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-02-01 15:44:59.000000 galois-0.3.3/tests/data/iroot.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-02-01 15:44:59.000000 galois-0.3.3/tests/data/is_cyclic.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-02-01 15:44:59.000000 galois-0.3.3/tests/data/is_perfect_power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-02-01 15:44:59.000000 galois-0.3.3/tests/data/is_powersmooth.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-02-01 15:44:59.000000 galois-0.3.3/tests/data/is_prime.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-02-01 15:44:59.000000 galois-0.3.3/tests/data/is_prime_power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-02-01 15:44:59.000000 galois-0.3.3/tests/data/is_smooth.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-02-01 15:44:59.000000 galois-0.3.3/tests/data/is_square_free.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-02-01 15:44:59.000000 galois-0.3.3/tests/data/isqrt.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-02-01 15:44:59.000000 galois-0.3.3/tests/data/kth_prime.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-02-01 15:44:59.000000 galois-0.3.3/tests/data/lcm.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-02-01 15:44:59.000000 galois-0.3.3/tests/data/next_prime.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-02-01 15:44:59.000000 galois-0.3.3/tests/data/prev_prime.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-02-01 15:44:59.000000 galois-0.3.3/tests/data/primes.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-02-01 15:44:59.000000 galois-0.3.3/tests/data/prod.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14351 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/fields/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/fields/data/GF(109987^4)/
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(109987^4)/add.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(109987^4)/additive_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(109987^4)/additive_order.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(109987^4)/characteristic_poly_element.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(109987^4)/characteristic_poly_matrix.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(109987^4)/column_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(109987^4)/convolve.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(109987^4)/divide.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(109987^4)/field_norm.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(109987^4)/field_trace.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(109987^4)/left_null_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(109987^4)/log.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(109987^4)/lu_decompose.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(109987^4)/matrix_determinant.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(109987^4)/matrix_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(109987^4)/matrix_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(109987^4)/matrix_solve.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(109987^4)/minimal_poly_element.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(109987^4)/multiplicative_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(109987^4)/multiplicative_order.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(109987^4)/multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(109987^4)/null_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(109987^4)/plu_decompose.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(109987^4)/power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(109987^4)/properties.json
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(109987^4)/row_reduce.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(109987^4)/row_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(109987^4)/scalar_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(109987^4)/subtract.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/fields/data/GF(2)/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2)/add.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2)/additive_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2)/additive_order.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2)/characteristic_poly_element.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2)/characteristic_poly_matrix.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2)/column_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2)/convolve.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2)/divide.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2)/field_norm.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2)/field_trace.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2)/left_null_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2)/log.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2)/lu_decompose.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2)/matrix_determinant.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2)/matrix_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2)/matrix_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2)/matrix_solve.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2)/minimal_poly_element.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2)/multiplicative_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2)/multiplicative_order.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2)/multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2)/null_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2)/plu_decompose.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2)/power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2)/properties.json
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2)/row_reduce.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2)/row_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2)/scalar_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2)/subtract.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/fields/data/GF(2147483647)/
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2147483647)/add.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2147483647)/additive_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2147483647)/additive_order.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2147483647)/characteristic_poly_element.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2147483647)/characteristic_poly_matrix.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2147483647)/column_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2147483647)/convolve.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2147483647)/divide.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2147483647)/field_norm.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2147483647)/field_trace.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2147483647)/left_null_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2147483647)/log.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2147483647)/lu_decompose.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2147483647)/matrix_determinant.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2147483647)/matrix_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2147483647)/matrix_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2147483647)/matrix_solve.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2147483647)/minimal_poly_element.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2147483647)/multiplicative_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2147483647)/multiplicative_order.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2147483647)/multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2147483647)/null_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2147483647)/plu_decompose.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2147483647)/power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2147483647)/properties.json
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2147483647)/row_reduce.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2147483647)/row_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2147483647)/scalar_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2147483647)/subtract.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/fields/data/GF(2^100)/
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^100)/add.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^100)/additive_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^100)/additive_order.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^100)/characteristic_poly_element.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^100)/characteristic_poly_matrix.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^100)/column_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^100)/convolve.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^100)/divide.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^100)/field_norm.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^100)/field_trace.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^100)/left_null_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^100)/log.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^100)/lu_decompose.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^100)/matrix_determinant.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^100)/matrix_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^100)/matrix_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^100)/matrix_solve.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^100)/minimal_poly_element.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^100)/multiplicative_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^100)/multiplicative_order.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^100)/multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^100)/null_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     9559 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^100)/plu_decompose.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^100)/power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^100)/properties.json
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^100)/row_reduce.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^100)/row_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^100)/scalar_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^100)/subtract.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/fields/data/GF(2^2)/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^2)/add.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^2)/additive_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^2)/additive_order.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^2)/characteristic_poly_element.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^2)/characteristic_poly_matrix.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^2)/column_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^2)/convolve.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^2)/divide.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^2)/field_norm.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^2)/field_trace.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^2)/left_null_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^2)/log.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^2)/lu_decompose.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^2)/matrix_determinant.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^2)/matrix_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^2)/matrix_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^2)/matrix_solve.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^2)/minimal_poly_element.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^2)/multiplicative_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^2)/multiplicative_order.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^2)/multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^2)/null_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^2)/plu_decompose.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^2)/power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^2)/properties.json
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^2)/row_reduce.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^2)/row_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^2)/scalar_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^2)/subtract.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/fields/data/GF(2^3)/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^3)/add.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^3)/additive_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^3)/additive_order.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^3)/characteristic_poly_element.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^3)/characteristic_poly_matrix.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^3)/column_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^3)/convolve.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^3)/divide.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^3)/field_norm.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^3)/field_trace.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^3)/left_null_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^3)/log.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^3)/lu_decompose.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^3)/matrix_determinant.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^3)/matrix_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^3)/matrix_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^3)/matrix_solve.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^3)/minimal_poly_element.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^3)/multiplicative_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^3)/multiplicative_order.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^3)/multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^3)/null_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^3)/plu_decompose.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^3)/power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^3)/properties.json
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^3)/row_reduce.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^3)/row_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^3)/scalar_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^3)/subtract.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/fields/data/GF(2^32)/
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^32)/add.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^32)/additive_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^32)/additive_order.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^32)/characteristic_poly_element.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^32)/characteristic_poly_matrix.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^32)/column_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^32)/convolve.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^32)/divide.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^32)/field_norm.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^32)/field_trace.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^32)/left_null_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^32)/log.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^32)/lu_decompose.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^32)/matrix_determinant.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^32)/matrix_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^32)/matrix_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^32)/matrix_solve.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^32)/minimal_poly_element.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^32)/multiplicative_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^32)/multiplicative_order.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^32)/multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^32)/null_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^32)/plu_decompose.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^32)/power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^32)/properties.json
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^32)/row_reduce.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^32)/row_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^32)/scalar_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^32)/subtract.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/fields/data/GF(2^8)/
--rw-r--r--   0 runner    (1001) docker     (123)   528631 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8)/add.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8)/additive_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8)/additive_order.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8)/characteristic_poly_element.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8)/characteristic_poly_matrix.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8)/column_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8)/convolve.pkl
--rw-r--r--   0 runner    (1001) docker     (123)   526573 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8)/divide.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8)/field_norm.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8)/field_trace.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8)/left_null_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8)/log.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8)/lu_decompose.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8)/matrix_determinant.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8)/matrix_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8)/matrix_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8)/matrix_solve.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8)/minimal_poly_element.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8)/multiplicative_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8)/multiplicative_order.pkl
--rw-r--r--   0 runner    (1001) docker     (123)   528631 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8)/multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8)/null_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8)/plu_decompose.pkl
--rw-r--r--   0 runner    (1001) docker     (123)  1061101 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8)/power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8)/properties.json
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8)/row_reduce.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8)/row_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)  1065247 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8)/scalar_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)   528631 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8)/subtract.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/
--rw-r--r--   0 runner    (1001) docker     (123)   528631 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/add.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/additive_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/additive_order.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/characteristic_poly_element.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/characteristic_poly_matrix.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/column_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/convolve.pkl
--rw-r--r--   0 runner    (1001) docker     (123)   526573 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/divide.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/field_norm.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/field_trace.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/left_null_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/log.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/lu_decompose.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/matrix_determinant.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/matrix_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/matrix_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/matrix_solve.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/minimal_poly_element.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/multiplicative_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/multiplicative_order.pkl
--rw-r--r--   0 runner    (1001) docker     (123)   528631 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/null_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/plu_decompose.pkl
--rw-r--r--   0 runner    (1001) docker     (123)  1061101 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/properties.json
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/row_reduce.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/row_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)  1065247 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/scalar_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)   528631 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/subtract.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/fields/data/GF(31)/
--rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(31)/add.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(31)/additive_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(31)/additive_order.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(31)/characteristic_poly_element.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(31)/characteristic_poly_matrix.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(31)/column_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(31)/convolve.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(31)/divide.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(31)/field_norm.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(31)/field_trace.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(31)/left_null_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(31)/log.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(31)/lu_decompose.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(31)/matrix_determinant.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(31)/matrix_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(31)/matrix_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(31)/matrix_solve.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(31)/minimal_poly_element.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(31)/multiplicative_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(31)/multiplicative_order.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(31)/multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(31)/null_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(31)/plu_decompose.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    17087 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(31)/power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(31)/properties.json
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(31)/row_reduce.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(31)/row_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    17631 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(31)/scalar_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(31)/subtract.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/fields/data/GF(3191)/
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(3191)/add.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(3191)/additive_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(3191)/additive_order.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(3191)/characteristic_poly_element.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(3191)/characteristic_poly_matrix.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(3191)/column_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(3191)/convolve.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(3191)/divide.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(3191)/field_norm.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(3191)/field_trace.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(3191)/left_null_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(3191)/log.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(3191)/lu_decompose.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(3191)/matrix_determinant.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(3191)/matrix_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(3191)/matrix_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(3191)/matrix_solve.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(3191)/minimal_poly_element.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(3191)/multiplicative_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(3191)/multiplicative_order.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(3191)/multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(3191)/null_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(3191)/plu_decompose.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(3191)/power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(3191)/properties.json
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(3191)/row_reduce.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(3191)/row_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(3191)/scalar_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(3191)/subtract.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/fields/data/GF(36893488147419103183)/
--rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(36893488147419103183)/add.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(36893488147419103183)/additive_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(36893488147419103183)/additive_order.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(36893488147419103183)/characteristic_poly_element.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(36893488147419103183)/characteristic_poly_matrix.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(36893488147419103183)/column_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(36893488147419103183)/convolve.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(36893488147419103183)/divide.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(36893488147419103183)/field_norm.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(36893488147419103183)/field_trace.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(36893488147419103183)/left_null_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(36893488147419103183)/log.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(36893488147419103183)/lu_decompose.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(36893488147419103183)/matrix_determinant.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(36893488147419103183)/matrix_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(36893488147419103183)/matrix_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(36893488147419103183)/matrix_solve.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(36893488147419103183)/minimal_poly_element.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(36893488147419103183)/multiplicative_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(36893488147419103183)/multiplicative_order.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(36893488147419103183)/multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(36893488147419103183)/null_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(36893488147419103183)/plu_decompose.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(36893488147419103183)/power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(36893488147419103183)/properties.json
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(36893488147419103183)/row_reduce.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(36893488147419103183)/row_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(36893488147419103183)/scalar_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(36893488147419103183)/subtract.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/fields/data/GF(5)/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(5)/add.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(5)/additive_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(5)/additive_order.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(5)/characteristic_poly_element.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(5)/characteristic_poly_matrix.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(5)/column_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(5)/convolve.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(5)/divide.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(5)/field_norm.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(5)/field_trace.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(5)/left_null_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(5)/log.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(5)/lu_decompose.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(5)/matrix_determinant.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(5)/matrix_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(5)/matrix_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(5)/matrix_solve.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(5)/minimal_poly_element.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(5)/multiplicative_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(5)/multiplicative_order.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(5)/multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(5)/null_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(5)/plu_decompose.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(5)/power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(5)/properties.json
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(5)/row_reduce.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(5)/row_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(5)/scalar_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(5)/subtract.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/fields/data/GF(7)/
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7)/add.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7)/additive_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7)/additive_order.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7)/characteristic_poly_element.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7)/characteristic_poly_matrix.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7)/column_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7)/convolve.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7)/divide.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7)/field_norm.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7)/field_trace.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7)/left_null_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7)/log.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7)/lu_decompose.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7)/matrix_determinant.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7)/matrix_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7)/matrix_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7)/matrix_solve.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7)/minimal_poly_element.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7)/multiplicative_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7)/multiplicative_order.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7)/multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7)/null_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7)/plu_decompose.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7)/power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7)/properties.json
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7)/row_reduce.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7)/row_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7)/scalar_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7)/subtract.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/fields/data/GF(7^3)/
--rw-r--r--   0 runner    (1001) docker     (123)   946927 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3)/add.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3)/additive_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3)/additive_order.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3)/characteristic_poly_element.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3)/characteristic_poly_matrix.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3)/column_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3)/convolve.pkl
--rw-r--r--   0 runner    (1001) docker     (123)   944175 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3)/divide.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3)/field_norm.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3)/field_trace.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3)/left_null_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3)/log.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3)/lu_decompose.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3)/matrix_determinant.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3)/matrix_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3)/matrix_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3)/matrix_solve.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3)/minimal_poly_element.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3)/multiplicative_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3)/multiplicative_order.pkl
--rw-r--r--   0 runner    (1001) docker     (123)   946927 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3)/multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3)/null_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3)/plu_decompose.pkl
--rw-r--r--   0 runner    (1001) docker     (123)  1899087 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3)/power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3)/properties.json
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3)/row_reduce.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3)/row_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)  1904623 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3)/scalar_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)   946927 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3)/subtract.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/
--rw-r--r--   0 runner    (1001) docker     (123)   946927 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/add.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/additive_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/additive_order.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/characteristic_poly_element.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/characteristic_poly_matrix.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/column_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/convolve.pkl
--rw-r--r--   0 runner    (1001) docker     (123)   944175 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/divide.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/field_norm.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/field_trace.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/left_null_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/log.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/lu_decompose.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/matrix_determinant.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/matrix_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/matrix_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/matrix_solve.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/minimal_poly_element.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/multiplicative_inverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/multiplicative_order.pkl
--rw-r--r--   0 runner    (1001) docker     (123)   946927 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/null_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/plu_decompose.pkl
--rw-r--r--   0 runner    (1001) docker     (123)  1899087 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/properties.json
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/row_reduce.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/row_space.pkl
--rw-r--r--   0 runner    (1001) docker     (123)  1904623 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/scalar_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)   946927 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/subtract.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/test_advanced_arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/test_arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/test_arithmetic_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/test_arithmetic_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/test_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/test_broadcasting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/test_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    10121 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/test_constructors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/test_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/test_fft.py
--rw-r--r--   0 runner    (1001) docker     (123)    13472 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/test_instantiation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14912 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/test_linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)    15876 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/test_ntt.py
--rw-r--r--   0 runner    (1001) docker     (123)    12872 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/test_numpy_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13067 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/test_numpy_ufuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/test_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/test_sqrt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8381 2023-02-01 15:44:59.000000 galois-0.3.3/tests/fields/test_squares.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/polys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/polys/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/polys/data/GF(109987^4)/
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(109987^4)/add.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(109987^4)/crt.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(109987^4)/derivative.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(109987^4)/divmod.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(109987^4)/egcd.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(109987^4)/evaluate.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(109987^4)/evaluate_matrix.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(109987^4)/evaluate_poly.pkl
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(109987^4)/is_irreducible.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(109987^4)/is_monic.pkl
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(109987^4)/is_primitive.pkl
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(109987^4)/is_square_free.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(109987^4)/lagrange_poly.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(109987^4)/lcm.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(109987^4)/modular_power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(109987^4)/multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(109987^4)/power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(109987^4)/prod.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(109987^4)/reverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(109987^4)/roots.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(109987^4)/scalar_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(109987^4)/subtract.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/polys/data/GF(2)/
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2)/add.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2)/crt.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2)/derivative.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2)/divmod.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2)/egcd.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2)/evaluate.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2)/evaluate_matrix.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2)/evaluate_poly.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2)/is_irreducible.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2)/is_monic.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2)/is_primitive.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2)/is_square_free.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2)/lagrange_poly.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2)/lcm.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2)/modular_power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2)/multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2)/power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2)/prod.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2)/reverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2)/roots.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2)/scalar_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2)/subtract.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/polys/data/GF(2147483647)/
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2147483647)/add.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2147483647)/crt.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2147483647)/derivative.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2147483647)/divmod.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2147483647)/egcd.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2147483647)/evaluate.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2147483647)/evaluate_matrix.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2147483647)/evaluate_poly.pkl
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2147483647)/is_irreducible.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2147483647)/is_monic.pkl
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2147483647)/is_primitive.pkl
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2147483647)/is_square_free.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2147483647)/lagrange_poly.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2147483647)/lcm.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2147483647)/modular_power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2147483647)/multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2147483647)/power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2147483647)/prod.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2147483647)/reverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2147483647)/roots.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2147483647)/scalar_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2147483647)/subtract.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/polys/data/GF(2^100)/
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^100)/add.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    11490 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^100)/crt.pkl
--rw-r--r--   0 runner    (1001) docker     (123)   163205 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^100)/derivative.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^100)/divmod.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^100)/egcd.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^100)/evaluate.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^100)/evaluate_matrix.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^100)/evaluate_poly.pkl
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^100)/is_irreducible.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^100)/is_monic.pkl
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^100)/is_primitive.pkl
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^100)/is_square_free.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^100)/lagrange_poly.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10395 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^100)/lcm.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^100)/modular_power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^100)/multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^100)/power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    13095 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^100)/prod.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^100)/reverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^100)/roots.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^100)/scalar_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^100)/subtract.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/polys/data/GF(2^2)/
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^2)/add.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^2)/crt.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^2)/derivative.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^2)/divmod.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^2)/egcd.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^2)/evaluate.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^2)/evaluate_matrix.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^2)/evaluate_poly.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^2)/is_irreducible.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^2)/is_monic.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^2)/is_primitive.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^2)/is_square_free.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^2)/lagrange_poly.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^2)/lcm.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^2)/modular_power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^2)/multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^2)/power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^2)/prod.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^2)/reverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^2)/roots.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^2)/scalar_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^2)/subtract.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/polys/data/GF(2^3)/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^3)/add.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^3)/crt.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^3)/derivative.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^3)/divmod.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^3)/egcd.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^3)/evaluate.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^3)/evaluate_matrix.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^3)/evaluate_poly.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^3)/is_irreducible.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^3)/is_monic.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^3)/is_primitive.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^3)/is_square_free.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^3)/lagrange_poly.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^3)/lcm.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^3)/modular_power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^3)/multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^3)/power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^3)/prod.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^3)/reverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^3)/roots.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^3)/scalar_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^3)/subtract.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/polys/data/GF(2^32)/
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^32)/add.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^32)/crt.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    22229 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^32)/derivative.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^32)/divmod.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^32)/egcd.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^32)/evaluate.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^32)/evaluate_matrix.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^32)/evaluate_poly.pkl
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^32)/is_irreducible.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^32)/is_monic.pkl
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^32)/is_primitive.pkl
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^32)/is_square_free.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^32)/lagrange_poly.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^32)/lcm.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^32)/modular_power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^32)/multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^32)/power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^32)/prod.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^32)/reverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^32)/roots.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^32)/scalar_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^32)/subtract.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/polys/data/GF(2^8)/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8)/add.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8)/crt.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8)/derivative.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8)/divmod.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8)/egcd.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    43528 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8)/evaluate.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8)/evaluate_matrix.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8)/evaluate_poly.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8)/is_irreducible.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8)/is_monic.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8)/is_primitive.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8)/is_square_free.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8)/lagrange_poly.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8)/lcm.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8)/modular_power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8)/multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8)/power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8)/prod.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8)/reverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8)/roots.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8)/scalar_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8)/subtract.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/add.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/crt.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/derivative.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/divmod.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/egcd.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    43541 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/evaluate.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/evaluate_matrix.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/evaluate_poly.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/is_irreducible.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/is_monic.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/is_primitive.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/is_square_free.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/lagrange_poly.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/lcm.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/modular_power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/prod.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/reverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/roots.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/scalar_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/subtract.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/polys/data/GF(31)/
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(31)/add.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(31)/crt.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(31)/derivative.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(31)/divmod.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(31)/egcd.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(31)/evaluate.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(31)/evaluate_matrix.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(31)/evaluate_poly.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(31)/is_irreducible.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(31)/is_monic.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(31)/is_primitive.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(31)/is_square_free.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(31)/lagrange_poly.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(31)/lcm.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(31)/modular_power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(31)/multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(31)/power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(31)/prod.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(31)/reverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(31)/roots.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(31)/scalar_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(31)/subtract.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/polys/data/GF(3191)/
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(3191)/add.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(3191)/crt.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(3191)/derivative.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(3191)/divmod.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(3191)/egcd.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(3191)/evaluate.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(3191)/evaluate_matrix.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(3191)/evaluate_poly.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(3191)/is_irreducible.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(3191)/is_monic.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(3191)/is_primitive.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(3191)/is_square_free.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(3191)/lagrange_poly.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(3191)/lcm.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(3191)/modular_power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(3191)/multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(3191)/power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(3191)/prod.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(3191)/reverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(3191)/roots.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(3191)/scalar_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(3191)/subtract.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/polys/data/GF(36893488147419103183)/
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(36893488147419103183)/add.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(36893488147419103183)/crt.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(36893488147419103183)/derivative.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(36893488147419103183)/divmod.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(36893488147419103183)/egcd.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(36893488147419103183)/evaluate.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(36893488147419103183)/evaluate_matrix.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(36893488147419103183)/evaluate_poly.pkl
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(36893488147419103183)/is_irreducible.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(36893488147419103183)/is_monic.pkl
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(36893488147419103183)/is_primitive.pkl
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(36893488147419103183)/is_square_free.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(36893488147419103183)/lagrange_poly.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(36893488147419103183)/lcm.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(36893488147419103183)/modular_power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(36893488147419103183)/multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(36893488147419103183)/power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(36893488147419103183)/prod.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(36893488147419103183)/reverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(36893488147419103183)/roots.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(36893488147419103183)/scalar_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(36893488147419103183)/subtract.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/polys/data/GF(5)/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(5)/add.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(5)/crt.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(5)/derivative.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(5)/divmod.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(5)/egcd.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(5)/evaluate.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(5)/evaluate_matrix.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(5)/evaluate_poly.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(5)/is_irreducible.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(5)/is_monic.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(5)/is_primitive.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(5)/is_square_free.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(5)/lagrange_poly.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(5)/lcm.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(5)/modular_power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(5)/multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(5)/power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(5)/prod.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(5)/reverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(5)/roots.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(5)/scalar_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(5)/subtract.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/polys/data/GF(7)/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7)/add.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7)/crt.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7)/derivative.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7)/divmod.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7)/egcd.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7)/evaluate.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7)/evaluate_matrix.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7)/evaluate_poly.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7)/is_irreducible.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7)/is_monic.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7)/is_primitive.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7)/is_square_free.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7)/lagrange_poly.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7)/lcm.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7)/modular_power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7)/multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7)/power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7)/prod.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7)/reverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7)/roots.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7)/scalar_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7)/subtract.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/polys/data/GF(7^3)/
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3)/add.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3)/crt.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3)/derivative.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3)/divmod.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3)/egcd.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    58150 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3)/evaluate.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3)/evaluate_matrix.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3)/evaluate_poly.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3)/is_irreducible.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3)/is_monic.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3)/is_primitive.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3)/is_square_free.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3)/lagrange_poly.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3)/lcm.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3)/modular_power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3)/multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3)/power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3)/prod.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3)/reverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3)/roots.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3)/scalar_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3)/subtract.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/add.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/crt.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/derivative.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/divmod.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/egcd.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    58174 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/evaluate.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/evaluate_matrix.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/evaluate_poly.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/is_irreducible.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/is_monic.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/is_primitive.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/is_square_free.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/lagrange_poly.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/lcm.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/modular_power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/power.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/prod.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/reverse.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/roots.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/scalar_multiply.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/subtract.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 15:45:23.000000 galois-0.3.3/tests/polys/luts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/luts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/luts/irreducible_polys.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/luts/irreducible_polys_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/luts/irreducible_polys_25.py
--rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/luts/irreducible_polys_3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/luts/irreducible_polys_4.py
--rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/luts/irreducible_polys_5.py
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/luts/irreducible_polys_9.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/luts/irreducible_polys_min.py
--rw-r--r--   0 runner    (1001) docker     (123)    20590 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/luts/poly_factors.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/luts/primitive_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/luts/primitive_elements_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/luts/primitive_elements_3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/luts/primitive_elements_5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/luts/primitive_polys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/luts/primitive_polys_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/luts/primitive_polys_25.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/luts/primitive_polys_3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/luts/primitive_polys_4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/luts/primitive_polys_5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/luts/primitive_polys_9.py
--rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/test_arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/test_arithmetic_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/test_arithmetic_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/test_arithmetic_implementations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/test_arithmetic_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/test_constructors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/test_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/test_conway_polys.py
--rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/test_factors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/test_instantiation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/test_irreducible_polys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/test_lagrange_poly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/test_non_poly_arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/test_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/test_poly_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/test_primitive_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-02-01 15:44:59.000000 galois-0.3.3/tests/polys/test_primitive_polys.py
--rw-r--r--   0 runner    (1001) docker     (123)     9573 2023-02-01 15:44:59.000000 galois-0.3.3/tests/test_berlekamp_massey.py
--rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-02-01 15:44:59.000000 galois-0.3.3/tests/test_factor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-02-01 15:44:59.000000 galois-0.3.3/tests/test_fibonacci_lfsr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-02-01 15:44:59.000000 galois-0.3.3/tests/test_galois_lfsr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-02-01 15:44:59.000000 galois-0.3.3/tests/test_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     9970 2023-02-01 15:44:59.000000 galois-0.3.3/tests/test_modular.py
--rw-r--r--   0 runner    (1001) docker     (123)    15142 2023-02-01 15:44:59.000000 galois-0.3.3/tests/test_number_theory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-02-01 15:44:59.000000 galois-0.3.3/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-02-01 15:44:59.000000 galois-0.3.3/tests/test_primes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-02 20:39:55.000000 galois-0.3.4/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-02 20:39:55.000000 galois-0.3.4/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-02 20:39:55.000000 galois-0.3.4/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-02 20:39:55.000000 galois-0.3.4/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-05-02 20:39:55.000000 galois-0.3.4/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-02 20:39:55.000000 galois-0.3.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-02 20:39:55.000000 galois-0.3.4/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-02 20:39:55.000000 galois-0.3.4/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-02 20:39:55.000000 galois-0.3.4/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-02 20:39:55.000000 galois-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-02 20:39:55.000000 galois-0.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14702 2023-05-02 20:40:23.000000 galois-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-05-02 20:39:55.000000 galois-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-02 20:39:55.000000 galois-0.3.4/benchmarks/test_fec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-02 20:39:55.000000 galois-0.3.4/benchmarks/test_field_arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-02 20:39:55.000000 galois-0.3.4/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 20:39:55.000000 galois-0.3.4/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-02 20:39:55.000000 galois-0.3.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-02 20:39:55.000000 galois-0.3.4/docs/_static/extra.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-02 20:39:55.000000 galois-0.3.4/docs/_templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-02 20:39:55.000000 galois-0.3.4/docs/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/docs/basic-usage/
+-rw-r--r--   0 runner    (1001) docker     (123)    11301 2023-05-02 20:39:55.000000 galois-0.3.4/docs/basic-usage/array-arithmetic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-05-02 20:39:55.000000 galois-0.3.4/docs/basic-usage/array-classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-05-02 20:39:55.000000 galois-0.3.4/docs/basic-usage/array-creation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-05-02 20:39:55.000000 galois-0.3.4/docs/basic-usage/compilation-modes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-05-02 20:39:55.000000 galois-0.3.4/docs/basic-usage/element-representation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-05-02 20:39:55.000000 galois-0.3.4/docs/basic-usage/poly-arithmetic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-05-02 20:39:55.000000 galois-0.3.4/docs/basic-usage/poly.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14987 2023-05-02 20:39:55.000000 galois-0.3.4/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/docs/development/
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-02 20:39:55.000000 galois-0.3.4/docs/development/documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-02 20:39:55.000000 galois-0.3.4/docs/development/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-02 20:39:55.000000 galois-0.3.4/docs/development/linter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-02 20:39:55.000000 galois-0.3.4/docs/development/unit-tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 20:39:55.000000 galois-0.3.4/docs/genindex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-05-02 20:39:55.000000 galois-0.3.4/docs/getting-started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-05-02 20:39:55.000000 galois-0.3.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-05-02 20:39:55.000000 galois-0.3.4/docs/ipython_with_reprs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-02 20:39:55.000000 galois-0.3.4/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/docs/performance/
+-rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-05-02 20:39:55.000000 galois-0.3.4/docs/performance/benchmarks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-05-02 20:39:55.000000 galois-0.3.4/docs/performance/binary-extension-fields.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-05-02 20:39:55.000000 galois-0.3.4/docs/performance/prime-fields.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/docs/release-notes/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-02 20:39:55.000000 galois-0.3.4/docs/release-notes/v0.0.14.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-02 20:39:55.000000 galois-0.3.4/docs/release-notes/v0.0.15.md
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-02 20:39:55.000000 galois-0.3.4/docs/release-notes/v0.0.16.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-02 20:39:55.000000 galois-0.3.4/docs/release-notes/v0.0.17.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-02 20:39:55.000000 galois-0.3.4/docs/release-notes/v0.0.18.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-02 20:39:55.000000 galois-0.3.4/docs/release-notes/v0.0.19.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-02 20:39:55.000000 galois-0.3.4/docs/release-notes/v0.0.20.md
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-02 20:39:55.000000 galois-0.3.4/docs/release-notes/v0.0.21.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-02 20:39:55.000000 galois-0.3.4/docs/release-notes/v0.0.22.md
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-02 20:39:55.000000 galois-0.3.4/docs/release-notes/v0.0.23.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-05-02 20:39:55.000000 galois-0.3.4/docs/release-notes/v0.0.24.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-02 20:39:55.000000 galois-0.3.4/docs/release-notes/v0.0.25.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7148 2023-05-02 20:39:55.000000 galois-0.3.4/docs/release-notes/v0.0.26.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-05-02 20:39:55.000000 galois-0.3.4/docs/release-notes/v0.0.27.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-02 20:39:55.000000 galois-0.3.4/docs/release-notes/v0.0.28.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-05-02 20:39:55.000000 galois-0.3.4/docs/release-notes/v0.0.29.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-05-02 20:39:55.000000 galois-0.3.4/docs/release-notes/v0.0.30.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-02 20:39:55.000000 galois-0.3.4/docs/release-notes/v0.0.31.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-02 20:39:55.000000 galois-0.3.4/docs/release-notes/v0.0.32.md
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-02 20:39:55.000000 galois-0.3.4/docs/release-notes/v0.0.33.md
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-02 20:39:55.000000 galois-0.3.4/docs/release-notes/v0.1.0.md
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-02 20:39:55.000000 galois-0.3.4/docs/release-notes/v0.1.1.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-02 20:39:55.000000 galois-0.3.4/docs/release-notes/v0.1.2.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-02 20:39:55.000000 galois-0.3.4/docs/release-notes/v0.2.0.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-02 20:39:55.000000 galois-0.3.4/docs/release-notes/v0.3.0.md
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-02 20:39:55.000000 galois-0.3.4/docs/release-notes/v0.3.1.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-02 20:39:55.000000 galois-0.3.4/docs/release-notes/v0.3.2.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-02 20:39:55.000000 galois-0.3.4/docs/release-notes/v0.3.3.md
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-02 20:39:55.000000 galois-0.3.4/docs/release-notes/v0.3.4.md
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-02 20:39:55.000000 galois-0.3.4/docs/release-notes/versioning.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-02 20:39:55.000000 galois-0.3.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-05-02 20:39:55.000000 galois-0.3.4/docs/tutorials/intro-to-extension-fields.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10120 2023-05-02 20:39:55.000000 galois-0.3.4/docs/tutorials/intro-to-prime-fields.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-02 20:39:55.000000 galois-0.3.4/logo/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    24465 2023-05-02 20:39:55.000000 galois-0.3.4/logo/galois-favicon-color.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20786 2023-05-02 20:39:55.000000 galois-0.3.4/logo/galois-favicon-white.png
+-rw-r--r--   0 runner    (1001) docker     (123)    81221 2023-05-02 20:39:55.000000 galois-0.3.4/logo/galois-github-social.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16252 2023-05-02 20:39:55.000000 galois-0.3.4/logo/galois-github-social.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   105002 2023-05-02 20:39:55.000000 galois-0.3.4/logo/galois-heading.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-05-02 20:39:55.000000 galois-0.3.4/logo/galois-logo-small.png
+-rw-r--r--   0 runner    (1001) docker     (123)    54587 2023-05-02 20:39:55.000000 galois-0.3.4/logo/galois-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15396 2023-05-02 20:39:55.000000 galois-0.3.4/logo/galois-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-02 20:39:55.000000 galois-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-02 20:39:55.000000 galois-0.3.4/requirements-min.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-02 20:39:55.000000 galois-0.3.4/scripts/create_conway_polys_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-05-02 20:39:55.000000 galois-0.3.4/scripts/create_irreducible_polys_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22092 2023-05-02 20:39:55.000000 galois-0.3.4/scripts/create_prime_factors_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12618 2023-05-02 20:39:55.000000 galois-0.3.4/scripts/generate_fec_test_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38108 2023-05-02 20:39:55.000000 galois-0.3.4/scripts/generate_field_test_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-05-02 20:39:55.000000 galois-0.3.4/scripts/generate_int_test_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-02 20:39:55.000000 galois-0.3.4/scripts/sparse_poly_performance_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 20:40:23.000000 galois-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/src/galois/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/src/galois/_codes/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_codes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44262 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_codes/_bch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7953 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_codes/_cyclic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15946 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_codes/_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33742 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_codes/_reed_solomon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/src/galois/_databases/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_databases/_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1552384 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_databases/conway_polys.db
+-rw-r--r--   0 runner    (1001) docker     (123)   466944 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_databases/irreducible_polys.db
+-rw-r--r--   0 runner    (1001) docker     (123)  8187904 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_databases/prime_factors.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/src/galois/_domains/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_domains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18547 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_domains/_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26170 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_domains/_calculate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_domains/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12633 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_domains/_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17826 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_domains/_linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_domains/_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_domains/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26519 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_domains/_ufunc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/src/galois/_fields/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71788 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_fields/_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19170 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_fields/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_fields/_gf2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19641 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_fields/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_fields/_primitive_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_fields/_ufunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53456 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_lfsr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26121 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_modular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_ntt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22544 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_polymorphic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/src/galois/_polys/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_polys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_polys/_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_polys/_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13776 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_polys/_conway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16083 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_polys/_dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15179 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_polys/_factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_polys/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14389 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_polys/_irreducible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_polys/_lagrange.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66636 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_polys/_poly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16356 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_polys/_primitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_polys/_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_polys/_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51256 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/_prime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-02 20:40:22.000000 galois-0.3.4/src/galois/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-05-02 20:39:55.000000 galois-0.3.4/src/galois/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/src/galois.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14702 2023-05-02 20:40:22.000000 galois-0.3.4/src/galois.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    57340 2023-05-02 20:40:23.000000 galois-0.3.4/src/galois.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:40:22.000000 galois-0.3.4/src/galois.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-02 20:40:22.000000 galois-0.3.4/src/galois.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 20:40:22.000000 galois-0.3.4/src/galois.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:39:55.000000 galois-0.3.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/codes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/codes/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/codes/data/bch/
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k10_d2_alpha6_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k10_d2_alpha6_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k10_d2_alpha9_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k10_d2_alpha9_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k10_d2_alpha9_c3_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k10_d2_alpha9_c3_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k13_d1_alpha6_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k13_d1_alpha6_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k13_d1_alpha9_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k13_d1_alpha9_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k13_d1_alpha9_c3_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k13_d1_alpha9_c3_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k1_d6_alpha9_c3_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k1_d6_alpha9_c3_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k1_d7_alpha9_c3_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k1_d7_alpha9_c3_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k1_d8_alpha6_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k1_d8_alpha6_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k1_d8_alpha9_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k1_d8_alpha9_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k1_d8_alpha9_c3_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k1_d8_alpha9_c3_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k4_d4_alpha9_c3_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k4_d4_alpha9_c3_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k4_d5_alpha6_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k4_d5_alpha6_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k4_d5_alpha9_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k4_d5_alpha9_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k4_d5_alpha9_c3_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k4_d5_alpha9_c3_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k4_d6_alpha6_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k4_d6_alpha6_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k4_d6_alpha9_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k4_d6_alpha9_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k4_d7_alpha6_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k4_d7_alpha6_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k4_d7_alpha9_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k4_d7_alpha9_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k7_d3_alpha6_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k7_d3_alpha6_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k7_d3_alpha9_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k7_d3_alpha9_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k7_d3_alpha9_c3_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k7_d3_alpha9_c3_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k7_d4_alpha6_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k7_d4_alpha6_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k7_d4_alpha9_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n13_k7_d4_alpha9_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k11_d2_alpha2_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k11_d2_alpha2_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k11_d2_alpha2_c3_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k11_d2_alpha2_c3_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k11_d2_alpha9_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k11_d2_alpha9_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k11_d3_alpha2_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k11_d3_alpha2_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k11_d3_alpha9_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k11_d3_alpha9_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k15_d1_alpha2_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k15_d1_alpha2_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k15_d1_alpha2_c3_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k15_d1_alpha2_c3_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k15_d1_alpha9_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k15_d1_alpha9_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k1_d6_alpha2_c3_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k1_d6_alpha2_c3_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k1_d7_alpha2_c3_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k1_d7_alpha2_c3_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k1_d8_alpha2_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k1_d8_alpha2_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k1_d8_alpha2_c3_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k1_d8_alpha2_c3_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k1_d8_alpha9_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k1_d8_alpha9_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k5_d4_alpha2_c3_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k5_d4_alpha2_c3_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k5_d5_alpha2_c3_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k5_d5_alpha2_c3_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k5_d6_alpha2_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k5_d6_alpha2_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k5_d6_alpha9_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k5_d6_alpha9_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k5_d7_alpha2_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k5_d7_alpha2_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k5_d7_alpha9_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k5_d7_alpha9_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k7_d3_alpha2_c3_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k7_d3_alpha2_c3_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k7_d4_alpha2_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k7_d4_alpha2_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k7_d4_alpha9_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k7_d4_alpha9_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k7_d5_alpha2_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k7_d5_alpha2_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k7_d5_alpha9_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n15_k7_d5_alpha9_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8962 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k11_d6_alpha3_c3_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k11_d6_alpha3_c3_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k11_d8_alpha17_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10439 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k11_d8_alpha17_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8962 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k11_d8_alpha3_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10878 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k11_d8_alpha3_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k14_d5_alpha3_c3_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    11684 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k14_d5_alpha3_c3_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k14_d6_alpha17_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    12498 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k14_d6_alpha17_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k14_d6_alpha3_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k14_d6_alpha3_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k14_d7_alpha17_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10415 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k14_d7_alpha17_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k14_d7_alpha3_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10401 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k14_d7_alpha3_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k17_d4_alpha3_c3_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10399 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k17_d4_alpha3_c3_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k17_d5_alpha17_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    12990 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k17_d5_alpha17_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k17_d5_alpha3_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k17_d5_alpha3_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k1_d16_alpha3_c3_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k1_d16_alpha3_c3_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k1_d17_alpha3_c3_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k1_d17_alpha3_c3_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k1_d18_alpha17_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k1_d18_alpha17_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k1_d18_alpha3_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k1_d18_alpha3_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k1_d18_alpha3_c3_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k1_d18_alpha3_c3_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k20_d3_alpha17_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    11218 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k20_d3_alpha17_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k20_d3_alpha3_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    12970 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k20_d3_alpha3_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k20_d3_alpha3_c3_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k20_d3_alpha3_c3_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k20_d4_alpha17_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    11218 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k20_d4_alpha17_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k20_d4_alpha3_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    13290 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k20_d4_alpha3_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k23_d2_alpha17_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    13147 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k23_d2_alpha17_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k23_d2_alpha3_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    12021 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k23_d2_alpha3_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k23_d2_alpha3_c3_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k23_d2_alpha3_c3_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k26_d1_alpha17_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k26_d1_alpha17_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k26_d1_alpha3_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k26_d1_alpha3_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k26_d1_alpha3_c3_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k26_d1_alpha3_c3_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k4_d13_alpha3_c3_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10743 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k4_d13_alpha3_c3_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k4_d14_alpha3_c3_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10423 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k4_d14_alpha3_c3_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k4_d15_alpha17_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10904 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k4_d15_alpha17_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k4_d15_alpha3_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10423 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k4_d15_alpha3_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k4_d15_alpha3_c3_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10583 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k4_d15_alpha3_c3_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k4_d16_alpha17_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10741 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k4_d16_alpha17_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k4_d16_alpha3_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10583 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k4_d16_alpha3_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k4_d17_alpha17_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10904 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k4_d17_alpha17_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k4_d17_alpha3_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10743 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k4_d17_alpha3_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k7_d12_alpha3_c3_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k7_d12_alpha3_c3_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k7_d14_alpha17_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    11047 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k7_d14_alpha17_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k7_d14_alpha3_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k7_d14_alpha3_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k8_d10_alpha17_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k8_d10_alpha17_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k8_d10_alpha3_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k8_d10_alpha3_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k8_d10_alpha3_c3_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k8_d10_alpha3_c3_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k8_d11_alpha17_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10566 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k8_d11_alpha17_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k8_d11_alpha3_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10420 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k8_d11_alpha3_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k8_d11_alpha3_c3_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k8_d11_alpha3_c3_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k8_d12_alpha17_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10566 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k8_d12_alpha17_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k8_d12_alpha3_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k8_d12_alpha3_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k8_d13_alpha17_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k8_d13_alpha17_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k8_d13_alpha3_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10740 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k8_d13_alpha3_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k8_d7_alpha3_c3_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10740 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k8_d7_alpha3_c3_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k8_d8_alpha3_c3_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10580 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k8_d8_alpha3_c3_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k8_d9_alpha17_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    11369 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k8_d9_alpha17_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k8_d9_alpha3_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10580 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k8_d9_alpha3_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k8_d9_alpha3_c3_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/bch/n26_k8_d9_alpha3_c3_sys.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/codes/data/reed_solomon/
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n15_k10_d6_alpha2_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n15_k10_d6_alpha2_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n15_k10_d6_alpha9_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n15_k10_d6_alpha9_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n15_k11_d5_alpha2_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n15_k11_d5_alpha2_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n15_k11_d5_alpha9_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n15_k11_d5_alpha9_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n15_k12_d4_alpha2_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n15_k12_d4_alpha2_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n15_k12_d4_alpha9_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n15_k12_d4_alpha9_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n15_k13_d3_alpha2_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n15_k13_d3_alpha2_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n15_k13_d3_alpha9_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n15_k13_d3_alpha9_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n15_k14_d2_alpha2_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n15_k14_d2_alpha2_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n15_k14_d2_alpha9_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n15_k14_d2_alpha9_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n15_k8_d8_alpha2_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n15_k8_d8_alpha2_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n15_k8_d8_alpha9_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n15_k8_d8_alpha9_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n15_k9_d7_alpha2_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n15_k9_d7_alpha2_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n15_k9_d7_alpha9_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n15_k9_d7_alpha9_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n16_k10_d7_alpha11_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n16_k10_d7_alpha11_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n16_k10_d7_alpha31_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6613 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n16_k10_d7_alpha31_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n16_k11_d6_alpha11_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n16_k11_d6_alpha11_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n16_k11_d6_alpha31_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n16_k11_d6_alpha31_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n16_k12_d5_alpha11_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n16_k12_d5_alpha11_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n16_k12_d5_alpha31_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n16_k12_d5_alpha31_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n16_k13_d4_alpha11_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n16_k13_d4_alpha11_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n16_k13_d4_alpha31_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n16_k13_d4_alpha31_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n16_k14_d3_alpha11_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n16_k14_d3_alpha11_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n16_k14_d3_alpha31_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n16_k14_d3_alpha31_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n16_k15_d2_alpha11_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n16_k15_d2_alpha11_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n16_k15_d2_alpha31_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n16_k15_d2_alpha31_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n16_k9_d8_alpha11_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n16_k9_d8_alpha11_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n16_k9_d8_alpha31_c1_nonsys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/data/reed_solomon/n16_k9_d8_alpha31_c1_sys.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     9887 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/test_bch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-05-02 20:39:55.000000 galois-0.3.4/tests/codes/test_reed_solomon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-02 20:39:55.000000 galois-0.3.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-02 20:39:55.000000 galois-0.3.4/tests/data/carmichael_lambda.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-02 20:39:55.000000 galois-0.3.4/tests/data/crt.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-02 20:39:55.000000 galois-0.3.4/tests/data/egcd.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-02 20:39:55.000000 galois-0.3.4/tests/data/euler_phi.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-02 20:39:55.000000 galois-0.3.4/tests/data/ilog.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-02 20:39:55.000000 galois-0.3.4/tests/data/iroot.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-02 20:39:55.000000 galois-0.3.4/tests/data/is_cyclic.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-02 20:39:55.000000 galois-0.3.4/tests/data/is_perfect_power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-05-02 20:39:55.000000 galois-0.3.4/tests/data/is_powersmooth.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-02 20:39:55.000000 galois-0.3.4/tests/data/is_prime.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-02 20:39:55.000000 galois-0.3.4/tests/data/is_prime_power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-05-02 20:39:55.000000 galois-0.3.4/tests/data/is_smooth.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-02 20:39:55.000000 galois-0.3.4/tests/data/is_square_free.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-02 20:39:55.000000 galois-0.3.4/tests/data/isqrt.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-02 20:39:55.000000 galois-0.3.4/tests/data/kth_prime.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-02 20:39:55.000000 galois-0.3.4/tests/data/lcm.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-02 20:39:55.000000 galois-0.3.4/tests/data/next_prime.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-02 20:39:55.000000 galois-0.3.4/tests/data/prev_prime.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-02 20:39:55.000000 galois-0.3.4/tests/data/primes.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-02 20:39:55.000000 galois-0.3.4/tests/data/prod.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14351 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/fields/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/fields/data/GF(109987^4)/
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(109987^4)/add.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(109987^4)/additive_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(109987^4)/additive_order.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(109987^4)/characteristic_poly_element.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(109987^4)/characteristic_poly_matrix.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(109987^4)/column_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(109987^4)/convolve.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(109987^4)/divide.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(109987^4)/field_norm.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(109987^4)/field_trace.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(109987^4)/left_null_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(109987^4)/log.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(109987^4)/lu_decompose.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(109987^4)/matrix_determinant.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(109987^4)/matrix_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(109987^4)/matrix_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(109987^4)/matrix_solve.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(109987^4)/minimal_poly_element.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(109987^4)/multiplicative_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(109987^4)/multiplicative_order.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(109987^4)/multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(109987^4)/null_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(109987^4)/plu_decompose.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(109987^4)/power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(109987^4)/properties.json
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(109987^4)/row_reduce.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(109987^4)/row_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(109987^4)/scalar_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(109987^4)/subtract.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/fields/data/GF(2)/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2)/add.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2)/additive_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2)/additive_order.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2)/characteristic_poly_element.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2)/characteristic_poly_matrix.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2)/column_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2)/convolve.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2)/divide.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2)/field_norm.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2)/field_trace.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2)/left_null_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2)/log.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2)/lu_decompose.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2)/matrix_determinant.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2)/matrix_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2)/matrix_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2)/matrix_solve.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2)/minimal_poly_element.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2)/multiplicative_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2)/multiplicative_order.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2)/multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2)/null_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2)/plu_decompose.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2)/power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2)/properties.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2)/row_reduce.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2)/row_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2)/scalar_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2)/subtract.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/fields/data/GF(2147483647)/
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2147483647)/add.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2147483647)/additive_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2147483647)/additive_order.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2147483647)/characteristic_poly_element.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2147483647)/characteristic_poly_matrix.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2147483647)/column_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2147483647)/convolve.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2147483647)/divide.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2147483647)/field_norm.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2147483647)/field_trace.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2147483647)/left_null_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2147483647)/log.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2147483647)/lu_decompose.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2147483647)/matrix_determinant.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2147483647)/matrix_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2147483647)/matrix_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2147483647)/matrix_solve.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2147483647)/minimal_poly_element.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2147483647)/multiplicative_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2147483647)/multiplicative_order.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2147483647)/multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2147483647)/null_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2147483647)/plu_decompose.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2147483647)/power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2147483647)/properties.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2147483647)/row_reduce.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2147483647)/row_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2147483647)/scalar_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2147483647)/subtract.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/fields/data/GF(2^100)/
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^100)/add.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^100)/additive_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^100)/additive_order.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^100)/characteristic_poly_element.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^100)/characteristic_poly_matrix.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^100)/column_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^100)/convolve.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^100)/divide.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^100)/field_norm.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^100)/field_trace.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^100)/left_null_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^100)/log.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^100)/lu_decompose.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^100)/matrix_determinant.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^100)/matrix_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^100)/matrix_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^100)/matrix_solve.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^100)/minimal_poly_element.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^100)/multiplicative_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^100)/multiplicative_order.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^100)/multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^100)/null_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     9559 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^100)/plu_decompose.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^100)/power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^100)/properties.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^100)/row_reduce.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^100)/row_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^100)/scalar_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^100)/subtract.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/fields/data/GF(2^2)/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^2)/add.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^2)/additive_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^2)/additive_order.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^2)/characteristic_poly_element.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^2)/characteristic_poly_matrix.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^2)/column_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^2)/convolve.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^2)/divide.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^2)/field_norm.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^2)/field_trace.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^2)/left_null_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^2)/log.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^2)/lu_decompose.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^2)/matrix_determinant.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^2)/matrix_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^2)/matrix_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^2)/matrix_solve.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^2)/minimal_poly_element.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^2)/multiplicative_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^2)/multiplicative_order.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^2)/multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^2)/null_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^2)/plu_decompose.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^2)/power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^2)/properties.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^2)/row_reduce.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^2)/row_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^2)/scalar_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^2)/subtract.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/fields/data/GF(2^3)/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^3)/add.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^3)/additive_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^3)/additive_order.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^3)/characteristic_poly_element.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^3)/characteristic_poly_matrix.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^3)/column_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^3)/convolve.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^3)/divide.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^3)/field_norm.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^3)/field_trace.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^3)/left_null_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^3)/log.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^3)/lu_decompose.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^3)/matrix_determinant.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^3)/matrix_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^3)/matrix_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^3)/matrix_solve.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^3)/minimal_poly_element.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^3)/multiplicative_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^3)/multiplicative_order.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^3)/multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^3)/null_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^3)/plu_decompose.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^3)/power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^3)/properties.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^3)/row_reduce.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^3)/row_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^3)/scalar_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^3)/subtract.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/fields/data/GF(2^32)/
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^32)/add.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^32)/additive_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^32)/additive_order.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^32)/characteristic_poly_element.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^32)/characteristic_poly_matrix.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^32)/column_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^32)/convolve.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^32)/divide.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^32)/field_norm.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^32)/field_trace.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^32)/left_null_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^32)/log.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^32)/lu_decompose.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^32)/matrix_determinant.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^32)/matrix_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^32)/matrix_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^32)/matrix_solve.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^32)/minimal_poly_element.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^32)/multiplicative_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^32)/multiplicative_order.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^32)/multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^32)/null_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^32)/plu_decompose.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^32)/power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^32)/properties.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^32)/row_reduce.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^32)/row_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^32)/scalar_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^32)/subtract.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/fields/data/GF(2^8)/
+-rw-r--r--   0 runner    (1001) docker     (123)   528631 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8)/add.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8)/additive_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8)/additive_order.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8)/characteristic_poly_element.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8)/characteristic_poly_matrix.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8)/column_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8)/convolve.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)   526573 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8)/divide.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8)/field_norm.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8)/field_trace.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8)/left_null_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8)/log.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8)/lu_decompose.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8)/matrix_determinant.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8)/matrix_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8)/matrix_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8)/matrix_solve.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8)/minimal_poly_element.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8)/multiplicative_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8)/multiplicative_order.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)   528631 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8)/multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8)/null_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8)/plu_decompose.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)  1061101 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8)/power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8)/properties.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8)/row_reduce.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8)/row_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)  1065247 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8)/scalar_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)   528631 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8)/subtract.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/
+-rw-r--r--   0 runner    (1001) docker     (123)   528631 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/add.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/additive_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/additive_order.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/characteristic_poly_element.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/characteristic_poly_matrix.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/column_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/convolve.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)   526573 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/divide.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/field_norm.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/field_trace.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/left_null_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/log.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/lu_decompose.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/matrix_determinant.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/matrix_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/matrix_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/matrix_solve.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/minimal_poly_element.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/multiplicative_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/multiplicative_order.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)   528631 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/null_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/plu_decompose.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)  1061101 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/properties.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/row_reduce.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/row_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)  1065247 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/scalar_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)   528631 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/subtract.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/fields/data/GF(31)/
+-rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(31)/add.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(31)/additive_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(31)/additive_order.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(31)/characteristic_poly_element.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(31)/characteristic_poly_matrix.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(31)/column_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(31)/convolve.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(31)/divide.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(31)/field_norm.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(31)/field_trace.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(31)/left_null_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(31)/log.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(31)/lu_decompose.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(31)/matrix_determinant.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(31)/matrix_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(31)/matrix_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(31)/matrix_solve.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(31)/minimal_poly_element.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(31)/multiplicative_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(31)/multiplicative_order.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(31)/multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(31)/null_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(31)/plu_decompose.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    17087 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(31)/power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(31)/properties.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(31)/row_reduce.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(31)/row_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    17631 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(31)/scalar_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(31)/subtract.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/fields/data/GF(3191)/
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(3191)/add.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(3191)/additive_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(3191)/additive_order.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(3191)/characteristic_poly_element.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(3191)/characteristic_poly_matrix.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(3191)/column_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(3191)/convolve.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(3191)/divide.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(3191)/field_norm.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(3191)/field_trace.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(3191)/left_null_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(3191)/log.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(3191)/lu_decompose.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(3191)/matrix_determinant.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(3191)/matrix_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(3191)/matrix_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(3191)/matrix_solve.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(3191)/minimal_poly_element.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(3191)/multiplicative_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(3191)/multiplicative_order.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(3191)/multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(3191)/null_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(3191)/plu_decompose.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(3191)/power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(3191)/properties.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(3191)/row_reduce.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(3191)/row_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(3191)/scalar_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(3191)/subtract.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/fields/data/GF(36893488147419103183)/
+-rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(36893488147419103183)/add.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(36893488147419103183)/additive_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(36893488147419103183)/additive_order.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(36893488147419103183)/characteristic_poly_element.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(36893488147419103183)/characteristic_poly_matrix.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(36893488147419103183)/column_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(36893488147419103183)/convolve.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(36893488147419103183)/divide.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(36893488147419103183)/field_norm.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(36893488147419103183)/field_trace.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(36893488147419103183)/left_null_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(36893488147419103183)/log.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(36893488147419103183)/lu_decompose.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(36893488147419103183)/matrix_determinant.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(36893488147419103183)/matrix_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(36893488147419103183)/matrix_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(36893488147419103183)/matrix_solve.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(36893488147419103183)/minimal_poly_element.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(36893488147419103183)/multiplicative_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(36893488147419103183)/multiplicative_order.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(36893488147419103183)/multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(36893488147419103183)/null_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(36893488147419103183)/plu_decompose.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(36893488147419103183)/power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(36893488147419103183)/properties.json
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(36893488147419103183)/row_reduce.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(36893488147419103183)/row_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(36893488147419103183)/scalar_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(36893488147419103183)/subtract.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/fields/data/GF(5)/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(5)/add.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(5)/additive_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(5)/additive_order.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(5)/characteristic_poly_element.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(5)/characteristic_poly_matrix.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(5)/column_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(5)/convolve.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(5)/divide.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(5)/field_norm.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(5)/field_trace.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(5)/left_null_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(5)/log.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(5)/lu_decompose.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(5)/matrix_determinant.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(5)/matrix_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(5)/matrix_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(5)/matrix_solve.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(5)/minimal_poly_element.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(5)/multiplicative_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(5)/multiplicative_order.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(5)/multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(5)/null_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(5)/plu_decompose.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(5)/power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(5)/properties.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(5)/row_reduce.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(5)/row_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(5)/scalar_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(5)/subtract.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/fields/data/GF(7)/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7)/add.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7)/additive_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7)/additive_order.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7)/characteristic_poly_element.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7)/characteristic_poly_matrix.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7)/column_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7)/convolve.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7)/divide.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7)/field_norm.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7)/field_trace.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7)/left_null_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7)/log.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7)/lu_decompose.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7)/matrix_determinant.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7)/matrix_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7)/matrix_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7)/matrix_solve.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7)/minimal_poly_element.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7)/multiplicative_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7)/multiplicative_order.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7)/multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7)/null_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7)/plu_decompose.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7)/power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7)/properties.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7)/row_reduce.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7)/row_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7)/scalar_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7)/subtract.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/fields/data/GF(7^3)/
+-rw-r--r--   0 runner    (1001) docker     (123)   946927 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3)/add.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3)/additive_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3)/additive_order.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3)/characteristic_poly_element.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3)/characteristic_poly_matrix.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3)/column_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3)/convolve.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)   944175 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3)/divide.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3)/field_norm.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3)/field_trace.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3)/left_null_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3)/log.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3)/lu_decompose.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3)/matrix_determinant.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3)/matrix_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3)/matrix_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3)/matrix_solve.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3)/minimal_poly_element.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3)/multiplicative_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3)/multiplicative_order.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)   946927 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3)/multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3)/null_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3)/plu_decompose.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)  1899087 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3)/power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3)/properties.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3)/row_reduce.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3)/row_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)  1904623 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3)/scalar_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)   946927 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3)/subtract.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/
+-rw-r--r--   0 runner    (1001) docker     (123)   946927 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/add.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/additive_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/additive_order.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/characteristic_poly_element.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/characteristic_poly_matrix.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/column_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/convolve.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)   944175 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/divide.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/field_norm.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/field_trace.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/left_null_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/log.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/lu_decompose.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/matrix_determinant.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/matrix_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/matrix_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/matrix_solve.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/minimal_poly_element.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/multiplicative_inverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/multiplicative_order.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)   946927 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/null_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/plu_decompose.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)  1899087 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/properties.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/row_reduce.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/row_space.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)  1904623 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/scalar_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)   946927 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/subtract.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/test_advanced_arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/test_arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/test_arithmetic_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/test_arithmetic_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/test_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/test_broadcasting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/test_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10121 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/test_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/test_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/test_fft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13472 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/test_instantiation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15409 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/test_linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15876 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/test_ntt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12872 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/test_numpy_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13067 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/test_numpy_ufuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/test_sqrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8381 2023-05-02 20:39:55.000000 galois-0.3.4/tests/fields/test_squares.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/polys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/polys/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/polys/data/GF(109987^4)/
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(109987^4)/add.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(109987^4)/crt.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(109987^4)/derivative.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(109987^4)/divmod.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(109987^4)/egcd.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(109987^4)/evaluate.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(109987^4)/evaluate_matrix.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(109987^4)/evaluate_poly.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(109987^4)/is_irreducible.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(109987^4)/is_monic.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(109987^4)/is_primitive.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(109987^4)/is_square_free.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(109987^4)/lagrange_poly.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(109987^4)/lcm.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(109987^4)/modular_power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(109987^4)/multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(109987^4)/power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(109987^4)/prod.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(109987^4)/reverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(109987^4)/roots.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(109987^4)/scalar_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(109987^4)/subtract.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/polys/data/GF(2)/
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2)/add.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2)/crt.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2)/derivative.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2)/divmod.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2)/egcd.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2)/evaluate.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2)/evaluate_matrix.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2)/evaluate_poly.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2)/is_irreducible.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2)/is_monic.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2)/is_primitive.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2)/is_square_free.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2)/lagrange_poly.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2)/lcm.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2)/modular_power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2)/multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2)/power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2)/prod.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2)/reverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2)/roots.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2)/scalar_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2)/subtract.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/polys/data/GF(2147483647)/
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2147483647)/add.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2147483647)/crt.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2147483647)/derivative.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2147483647)/divmod.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2147483647)/egcd.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2147483647)/evaluate.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2147483647)/evaluate_matrix.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2147483647)/evaluate_poly.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2147483647)/is_irreducible.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2147483647)/is_monic.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2147483647)/is_primitive.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2147483647)/is_square_free.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2147483647)/lagrange_poly.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2147483647)/lcm.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2147483647)/modular_power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2147483647)/multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2147483647)/power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2147483647)/prod.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2147483647)/reverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2147483647)/roots.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2147483647)/scalar_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2147483647)/subtract.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/polys/data/GF(2^100)/
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^100)/add.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    11490 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^100)/crt.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)   163205 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^100)/derivative.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^100)/divmod.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^100)/egcd.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^100)/evaluate.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^100)/evaluate_matrix.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^100)/evaluate_poly.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^100)/is_irreducible.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^100)/is_monic.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^100)/is_primitive.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^100)/is_square_free.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^100)/lagrange_poly.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10395 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^100)/lcm.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^100)/modular_power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^100)/multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^100)/power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    13095 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^100)/prod.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^100)/reverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^100)/roots.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^100)/scalar_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^100)/subtract.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/polys/data/GF(2^2)/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^2)/add.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^2)/crt.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^2)/derivative.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^2)/divmod.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^2)/egcd.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^2)/evaluate.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^2)/evaluate_matrix.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^2)/evaluate_poly.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^2)/is_irreducible.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^2)/is_monic.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^2)/is_primitive.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^2)/is_square_free.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^2)/lagrange_poly.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^2)/lcm.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^2)/modular_power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^2)/multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^2)/power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^2)/prod.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^2)/reverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^2)/roots.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^2)/scalar_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^2)/subtract.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/polys/data/GF(2^3)/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^3)/add.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^3)/crt.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^3)/derivative.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^3)/divmod.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^3)/egcd.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^3)/evaluate.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^3)/evaluate_matrix.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^3)/evaluate_poly.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^3)/is_irreducible.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^3)/is_monic.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^3)/is_primitive.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^3)/is_square_free.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^3)/lagrange_poly.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^3)/lcm.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^3)/modular_power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^3)/multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^3)/power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^3)/prod.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^3)/reverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^3)/roots.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^3)/scalar_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^3)/subtract.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/polys/data/GF(2^32)/
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^32)/add.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^32)/crt.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    22229 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^32)/derivative.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^32)/divmod.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^32)/egcd.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^32)/evaluate.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^32)/evaluate_matrix.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^32)/evaluate_poly.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^32)/is_irreducible.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^32)/is_monic.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^32)/is_primitive.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^32)/is_square_free.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^32)/lagrange_poly.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^32)/lcm.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^32)/modular_power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^32)/multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^32)/power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^32)/prod.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^32)/reverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^32)/roots.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^32)/scalar_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^32)/subtract.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/polys/data/GF(2^8)/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8)/add.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8)/crt.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8)/derivative.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8)/divmod.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8)/egcd.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    43528 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8)/evaluate.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8)/evaluate_matrix.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8)/evaluate_poly.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8)/is_irreducible.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8)/is_monic.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8)/is_primitive.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8)/is_square_free.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8)/lagrange_poly.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8)/lcm.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8)/modular_power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8)/multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8)/power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8)/prod.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8)/reverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8)/roots.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8)/scalar_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8)/subtract.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/add.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/crt.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/derivative.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/divmod.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/egcd.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    43541 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/evaluate.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/evaluate_matrix.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/evaluate_poly.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/is_irreducible.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/is_monic.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/is_primitive.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/is_square_free.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/lagrange_poly.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/lcm.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/modular_power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/prod.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/reverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/roots.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/scalar_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/subtract.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/polys/data/GF(31)/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(31)/add.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(31)/crt.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(31)/derivative.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(31)/divmod.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(31)/egcd.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(31)/evaluate.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(31)/evaluate_matrix.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(31)/evaluate_poly.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(31)/is_irreducible.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(31)/is_monic.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(31)/is_primitive.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(31)/is_square_free.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(31)/lagrange_poly.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(31)/lcm.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(31)/modular_power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(31)/multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(31)/power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(31)/prod.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(31)/reverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(31)/roots.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(31)/scalar_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(31)/subtract.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/polys/data/GF(3191)/
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(3191)/add.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(3191)/crt.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(3191)/derivative.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(3191)/divmod.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(3191)/egcd.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(3191)/evaluate.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(3191)/evaluate_matrix.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(3191)/evaluate_poly.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(3191)/is_irreducible.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(3191)/is_monic.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(3191)/is_primitive.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(3191)/is_square_free.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(3191)/lagrange_poly.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(3191)/lcm.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(3191)/modular_power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(3191)/multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(3191)/power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(3191)/prod.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(3191)/reverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(3191)/roots.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(3191)/scalar_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(3191)/subtract.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/polys/data/GF(36893488147419103183)/
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(36893488147419103183)/add.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(36893488147419103183)/crt.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(36893488147419103183)/derivative.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(36893488147419103183)/divmod.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(36893488147419103183)/egcd.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(36893488147419103183)/evaluate.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(36893488147419103183)/evaluate_matrix.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(36893488147419103183)/evaluate_poly.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(36893488147419103183)/is_irreducible.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(36893488147419103183)/is_monic.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(36893488147419103183)/is_primitive.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(36893488147419103183)/is_square_free.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(36893488147419103183)/lagrange_poly.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(36893488147419103183)/lcm.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(36893488147419103183)/modular_power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(36893488147419103183)/multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(36893488147419103183)/power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(36893488147419103183)/prod.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(36893488147419103183)/reverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(36893488147419103183)/roots.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(36893488147419103183)/scalar_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(36893488147419103183)/subtract.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/polys/data/GF(5)/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(5)/add.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(5)/crt.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(5)/derivative.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(5)/divmod.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(5)/egcd.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(5)/evaluate.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(5)/evaluate_matrix.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(5)/evaluate_poly.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(5)/is_irreducible.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(5)/is_monic.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(5)/is_primitive.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(5)/is_square_free.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(5)/lagrange_poly.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(5)/lcm.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(5)/modular_power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(5)/multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(5)/power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(5)/prod.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(5)/reverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(5)/roots.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(5)/scalar_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(5)/subtract.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/polys/data/GF(7)/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7)/add.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7)/crt.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7)/derivative.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7)/divmod.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7)/egcd.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7)/evaluate.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7)/evaluate_matrix.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7)/evaluate_poly.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7)/is_irreducible.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7)/is_monic.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7)/is_primitive.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7)/is_square_free.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7)/lagrange_poly.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7)/lcm.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7)/modular_power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7)/multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7)/power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7)/prod.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7)/reverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7)/roots.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7)/scalar_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7)/subtract.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/polys/data/GF(7^3)/
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3)/add.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3)/crt.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3)/derivative.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3)/divmod.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3)/egcd.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    58150 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3)/evaluate.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3)/evaluate_matrix.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3)/evaluate_poly.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3)/is_irreducible.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3)/is_monic.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3)/is_primitive.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3)/is_square_free.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3)/lagrange_poly.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3)/lcm.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3)/modular_power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3)/multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3)/power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3)/prod.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3)/reverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3)/roots.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3)/scalar_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3)/subtract.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/add.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/crt.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/derivative.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/divmod.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/egcd.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    58174 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/evaluate.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/evaluate_matrix.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/evaluate_poly.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/is_irreducible.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/is_monic.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/is_primitive.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/is_square_free.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/lagrange_poly.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/lcm.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/modular_power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/power.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/prod.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/reverse.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/roots.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/scalar_multiply.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/subtract.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:40:23.000000 galois-0.3.4/tests/polys/luts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/luts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/luts/irreducible_polys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/luts/irreducible_polys_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/luts/irreducible_polys_25.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/luts/irreducible_polys_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/luts/irreducible_polys_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/luts/irreducible_polys_5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/luts/irreducible_polys_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/luts/irreducible_polys_min.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20590 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/luts/poly_factors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/luts/primitive_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/luts/primitive_elements_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/luts/primitive_elements_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/luts/primitive_elements_5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/luts/primitive_polys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/luts/primitive_polys_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/luts/primitive_polys_25.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/luts/primitive_polys_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/luts/primitive_polys_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/luts/primitive_polys_5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/luts/primitive_polys_9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/test_arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/test_arithmetic_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/test_arithmetic_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/test_arithmetic_implementations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/test_arithmetic_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/test_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/test_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/test_conway_polys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/test_factors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/test_instantiation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/test_irreducible_polys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/test_lagrange_poly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/test_non_poly_arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/test_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/test_poly_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/test_primitive_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-05-02 20:39:55.000000 galois-0.3.4/tests/polys/test_primitive_polys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9573 2023-05-02 20:39:55.000000 galois-0.3.4/tests/test_berlekamp_massey.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-05-02 20:39:55.000000 galois-0.3.4/tests/test_factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-05-02 20:39:55.000000 galois-0.3.4/tests/test_fibonacci_lfsr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-05-02 20:39:55.000000 galois-0.3.4/tests/test_galois_lfsr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-05-02 20:39:55.000000 galois-0.3.4/tests/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9970 2023-05-02 20:39:55.000000 galois-0.3.4/tests/test_modular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15142 2023-05-02 20:39:55.000000 galois-0.3.4/tests/test_number_theory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-02 20:39:55.000000 galois-0.3.4/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-05-02 20:39:55.000000 galois-0.3.4/tests/test_primes.py
```

### Comparing `galois-0.3.3/.github/workflows/build.yaml` & `galois-0.3.4/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/.github/workflows/docs.yaml` & `galois-0.3.4/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/.github/workflows/lint.yaml` & `galois-0.3.4/.github/workflows/lint.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 jobs:
   run-linter:
     name: Lint
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.7, 3.8, 3.9, '3.10']
+        python-version: [3.7, 3.8, 3.9, '3.10', 3.11]
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `galois-0.3.3/.github/workflows/release.yaml` & `galois-0.3.4/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/.github/workflows/test.yaml` & `galois-0.3.4/.github/workflows/test.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
   test-min:
     name: Min
     needs: wait-on-wheel
     if: ${{ github.event_name == 'pull_request' }}
     strategy:
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
-        python-version: [3.7, 3.8, 3.9, '3.10']
+        python-version: [3.7, 3.8, 3.9, '3.10', 3.11]
     runs-on: ${{ matrix.os }}
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
@@ -124,15 +124,15 @@
   test-latest:
     name: Latest
     needs: wait-on-wheel
     if: ${{ github.event_name == 'pull_request' }}
     strategy:
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
-        python-version: [3.7, 3.8, 3.9, '3.10']
+        python-version: [3.7, 3.8, 3.9, '3.10', 3.11]
     runs-on: ${{ matrix.os }}
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
```

### Comparing `galois-0.3.3/.readthedocs.yml` & `galois-0.3.4/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/LICENSE` & `galois-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/PKG-INFO` & `galois-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galois
-Version: 0.3.3
+Version: 0.3.4
 Summary: A performant NumPy extension for Galois fields and their applications
 Author-email: Matt Hostetter <matthostetter@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/mhostetter/galois
 Project-URL: Source, https://github.com/mhostetter/galois
 Project-URL: Issues, https://github.com/mhostetter/galois/issues
 Project-URL: Documentation, https://mhostetter.github.io/galois/latest/
@@ -23,14 +23,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -40,15 +41,15 @@
 
 <div align=center>
   <a href="https://pypi.org/project/galois"><img src="https://img.shields.io/pypi/v/galois"></a>
   <a href="https://pypi.org/project/galois"><img src="https://img.shields.io/pypi/pyversions/galois"></a>
   <a href="https://pypi.org/project/galois"><img src="https://img.shields.io/pypi/wheel/galois"></a>
   <a href="https://pypistats.org/packages/galois"><img src="https://img.shields.io/pypi/dm/galois"></a>
   <a href="https://pypi.org/project/galois"><img src="https://img.shields.io/pypi/l/galois"></a>
-  <a href="https://twitter.com/galois_py"><img src="https://img.shields.io/twitter/follow/galois_py?label=galois_py&style=flat&logo=twitter"></a>
+  <a href="https://twitter.com/galois_py"><img src="https://img.shields.io/static/v1?label=follow&message=@galois_py&color=blue&logo=twitter"></a>
 </div>
 
 <div align=center>
   <a href="https://github.com/mhostetter/galois/actions/workflows/docs.yaml"><img src="https://github.com/mhostetter/galois/actions/workflows/docs.yaml/badge.svg"></a>
   <a href="https://github.com/mhostetter/galois/actions/workflows/lint.yaml"><img src="https://github.com/mhostetter/galois/actions/workflows/lint.yaml/badge.svg"></a>
   <a href="https://github.com/mhostetter/galois/actions/workflows/build.yaml"><img src="https://github.com/mhostetter/galois/actions/workflows/build.yaml/badge.svg"></a>
   <a href="https://github.com/mhostetter/galois/actions/workflows/test.yaml"><img src="https://github.com/mhostetter/galois/actions/workflows/test.yaml/badge.svg"></a>
@@ -112,15 +113,15 @@
 
 Import the `galois` package in Python.
 
 ```python
 In [1]: import galois
 
 In [2]: galois.__version__
-Out[2]: '0.3.3'
+Out[2]: '0.3.4'
 ```
 
 ### Create a [`FieldArray`](https://mhostetter.github.io/galois/latest/api/galois.FieldArray/) subclass
 
 Next, create a [`FieldArray`](https://mhostetter.github.io/galois/latest/api/galois.FieldArray/) subclass
 for the specific finite field you'd like to work in. This is created using the `galois.GF()` class factory. In this example, we are
 working in $\mathrm{GF}(3^5)$.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: galois Version: 0.3.3 Summary: A performant NumPy
+Metadata-Version: 2.1 Name: galois Version: 0.3.4 Summary: A performant NumPy
 extension for Galois fields and their applications Author-email: Matt Hostetter
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/mhostetter/
 galois Project-URL: Source, https://github.com/mhostetter/galois Project-URL:
 Issues, https://github.com/mhostetter/galois/issues Project-URL: Documentation,
 https://mhostetter.github.io/galois/latest/ Project-URL: Discuss, https://
 github.com/mhostetter/galois/discussions Project-URL: Changelog, https://
 mhostetter.github.io/galois/latest/release-notes/versioning/ Project-URL:
@@ -15,25 +15,26 @@
 Classifier: Intended Audience :: Telecommunications Industry Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: POSIX :: Linux Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Topic :: Scientific/
-Engineering :: Mathematics Classifier: Topic :: Security :: Cryptography
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Typing :: Typed Requires-Python: >=3.7 Description-Content-Type:
-text/markdown Provides-Extra: dev License-File: LICENSE # ![Galois: A
-performant NumPy extension for Galois fields and their applications](https://
-raw.githubusercontent.com/mhostetter/galois/master/logo/galois-heading.png)
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Security :: Cryptography Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Classifier: Typing :: Typed
+Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra:
+dev License-File: LICENSE # ![Galois: A performant NumPy extension for Galois
+fields and their applications](https://raw.githubusercontent.com/mhostetter/
+galois/master/logo/galois-heading.png)
 [https://img.shields.io/pypi/v/galois] [https://img.shields.io/pypi/pyversions/
   galois] [https://img.shields.io/pypi/wheel/galois] [https://img.shields.io/
 pypi/dm/galois] [https://img.shields.io/pypi/l/galois] [https://img.shields.io/
-       twitter/follow/galois_py?label=galois_py&style=flat&logo=twitter]
+      static/v1?label=follow&message=@galois_py&color=blue&logo=twitter]
  [https://github.com/mhostetter/galois/actions/workflows/docs.yaml/badge.svg]
  [https://github.com/mhostetter/galois/actions/workflows/lint.yaml/badge.svg]
 [https://github.com/mhostetter/galois/actions/workflows/build.yaml/badge.svg]
  [https://github.com/mhostetter/galois/actions/workflows/test.yaml/badge.svg]
          [https://codecov.io/gh/mhostetter/galois/branch/master/graph/
                           badge.svg?token=3FJML79ZUK]
 The `galois` library is a Python 3 package that extends NumPy arrays to operate
@@ -91,15 +92,15 @@
 ) guide is intended to assist the user with installing the library, creating
 two example arrays, and performing basic array arithmetic. See [Basic Usage]
 (https://mhostetter.github.io/galois/latest/basic-usage/array-classes/) for
 more detailed discussions and examples. ### Install the package The latest
 version of `galois` can be installed from [PyPI](https://pypi.org/project/
 galois/) using `pip`. ```console $ python3 -m pip install galois ``` Import the
 `galois` package in Python. ```python In [1]: import galois In [2]:
-galois.__version__ Out[2]: '0.3.3' ``` ### Create a [`FieldArray`](https://
+galois.__version__ Out[2]: '0.3.4' ``` ### Create a [`FieldArray`](https://
 mhostetter.github.io/galois/latest/api/galois.FieldArray/) subclass Next,
 create a [`FieldArray`](https://mhostetter.github.io/galois/latest/api/
 galois.FieldArray/) subclass for the specific finite field you'd like to work
 in. This is created using the `galois.GF()` class factory. In this example, we
 are working in $\mathrm{GF}(3^5)$. ```python In [3]: GF = galois.GF(3**5) In
 [4]: print(GF.properties) Galois Field: name: GF(3^5) characteristic: 3 degree:
 5 order: 243 irreducible_poly: x^5 + 2x + 1 is_primitive_poly: True
```

### Comparing `galois-0.3.3/README.md` & `galois-0.3.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 <div align=center>
   <a href="https://pypi.org/project/galois"><img src="https://img.shields.io/pypi/v/galois"></a>
   <a href="https://pypi.org/project/galois"><img src="https://img.shields.io/pypi/pyversions/galois"></a>
   <a href="https://pypi.org/project/galois"><img src="https://img.shields.io/pypi/wheel/galois"></a>
   <a href="https://pypistats.org/packages/galois"><img src="https://img.shields.io/pypi/dm/galois"></a>
   <a href="https://pypi.org/project/galois"><img src="https://img.shields.io/pypi/l/galois"></a>
-  <a href="https://twitter.com/galois_py"><img src="https://img.shields.io/twitter/follow/galois_py?label=galois_py&style=flat&logo=twitter"></a>
+  <a href="https://twitter.com/galois_py"><img src="https://img.shields.io/static/v1?label=follow&message=@galois_py&color=blue&logo=twitter"></a>
 </div>
 
 <div align=center>
   <a href="https://github.com/mhostetter/galois/actions/workflows/docs.yaml"><img src="https://github.com/mhostetter/galois/actions/workflows/docs.yaml/badge.svg"></a>
   <a href="https://github.com/mhostetter/galois/actions/workflows/lint.yaml"><img src="https://github.com/mhostetter/galois/actions/workflows/lint.yaml/badge.svg"></a>
   <a href="https://github.com/mhostetter/galois/actions/workflows/build.yaml"><img src="https://github.com/mhostetter/galois/actions/workflows/build.yaml/badge.svg"></a>
   <a href="https://github.com/mhostetter/galois/actions/workflows/test.yaml"><img src="https://github.com/mhostetter/galois/actions/workflows/test.yaml/badge.svg"></a>
@@ -74,15 +74,15 @@
 
 Import the `galois` package in Python.
 
 ```python
 In [1]: import galois
 
 In [2]: galois.__version__
-Out[2]: '0.3.3'
+Out[2]: '0.3.4'
 ```
 
 ### Create a [`FieldArray`](https://mhostetter.github.io/galois/latest/api/galois.FieldArray/) subclass
 
 Next, create a [`FieldArray`](https://mhostetter.github.io/galois/latest/api/galois.FieldArray/) subclass
 for the specific finite field you'd like to work in. This is created using the `galois.GF()` class factory. In this example, we are
 working in $\mathrm{GF}(3^5)$.
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # ![Galois: A performant NumPy extension for Galois fields and their
 applications](https://raw.githubusercontent.com/mhostetter/galois/master/logo/
 galois-heading.png)
 [https://img.shields.io/pypi/v/galois] [https://img.shields.io/pypi/pyversions/
   galois] [https://img.shields.io/pypi/wheel/galois] [https://img.shields.io/
 pypi/dm/galois] [https://img.shields.io/pypi/l/galois] [https://img.shields.io/
-       twitter/follow/galois_py?label=galois_py&style=flat&logo=twitter]
+      static/v1?label=follow&message=@galois_py&color=blue&logo=twitter]
  [https://github.com/mhostetter/galois/actions/workflows/docs.yaml/badge.svg]
  [https://github.com/mhostetter/galois/actions/workflows/lint.yaml/badge.svg]
 [https://github.com/mhostetter/galois/actions/workflows/build.yaml/badge.svg]
  [https://github.com/mhostetter/galois/actions/workflows/test.yaml/badge.svg]
          [https://codecov.io/gh/mhostetter/galois/branch/master/graph/
                           badge.svg?token=3FJML79ZUK]
 The `galois` library is a Python 3 package that extends NumPy arrays to operate
@@ -66,15 +66,15 @@
 ) guide is intended to assist the user with installing the library, creating
 two example arrays, and performing basic array arithmetic. See [Basic Usage]
 (https://mhostetter.github.io/galois/latest/basic-usage/array-classes/) for
 more detailed discussions and examples. ### Install the package The latest
 version of `galois` can be installed from [PyPI](https://pypi.org/project/
 galois/) using `pip`. ```console $ python3 -m pip install galois ``` Import the
 `galois` package in Python. ```python In [1]: import galois In [2]:
-galois.__version__ Out[2]: '0.3.3' ``` ### Create a [`FieldArray`](https://
+galois.__version__ Out[2]: '0.3.4' ``` ### Create a [`FieldArray`](https://
 mhostetter.github.io/galois/latest/api/galois.FieldArray/) subclass Next,
 create a [`FieldArray`](https://mhostetter.github.io/galois/latest/api/
 galois.FieldArray/) subclass for the specific finite field you'd like to work
 in. This is created using the `galois.GF()` class factory. In this example, we
 are working in $\mathrm{GF}(3^5)$. ```python In [3]: GF = galois.GF(3**5) In
 [4]: print(GF.properties) Galois Field: name: GF(3^5) characteristic: 3 degree:
 5 order: 243 irreducible_poly: x^5 + 2x + 1 is_primitive_poly: True
```

### Comparing `galois-0.3.3/benchmarks/test_fec.py` & `galois-0.3.4/benchmarks/test_fec.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/benchmarks/test_field_arithmetic.py` & `galois-0.3.4/benchmarks/test_field_arithmetic.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/Makefile` & `galois-0.3.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/_static/extra.css` & `galois-0.3.4/docs/_static/extra.css`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/api.rst` & `galois-0.3.4/docs/api.rst`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/basic-usage/array-arithmetic.rst` & `galois-0.3.4/docs/basic-usage/array-arithmetic.rst`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/basic-usage/array-classes.rst` & `galois-0.3.4/docs/basic-usage/array-classes.rst`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/basic-usage/array-creation.rst` & `galois-0.3.4/docs/basic-usage/array-creation.rst`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/basic-usage/compilation-modes.rst` & `galois-0.3.4/docs/basic-usage/compilation-modes.rst`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/basic-usage/element-representation.rst` & `galois-0.3.4/docs/basic-usage/element-representation.rst`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/basic-usage/poly-arithmetic.rst` & `galois-0.3.4/docs/basic-usage/poly-arithmetic.rst`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/basic-usage/poly.rst` & `galois-0.3.4/docs/basic-usage/poly.rst`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/conf.py` & `galois-0.3.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/development/documentation.rst` & `galois-0.3.4/docs/development/documentation.rst`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/development/installation.rst` & `galois-0.3.4/docs/development/installation.rst`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/development/linter.rst` & `galois-0.3.4/docs/development/linter.rst`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/development/unit-tests.rst` & `galois-0.3.4/docs/development/unit-tests.rst`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/getting-started.rst` & `galois-0.3.4/docs/getting-started.rst`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/index.rst` & `galois-0.3.4/docs/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -145,14 +145,15 @@
    api.rst
 
 .. toctree::
    :caption: Release Notes
    :hidden:
 
    release-notes/versioning.rst
+   release-notes/v0.3.4.md
    release-notes/v0.3.3.md
    release-notes/v0.3.2.md
    release-notes/v0.3.1.md
    release-notes/v0.3.0.md
    release-notes/v0.2.0.md
    release-notes/v0.1.2.md
    release-notes/v0.1.1.md
```

### Comparing `galois-0.3.3/docs/ipython_with_reprs.py` & `galois-0.3.4/docs/ipython_with_reprs.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/make.bat` & `galois-0.3.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/performance/benchmarks.rst` & `galois-0.3.4/docs/performance/benchmarks.rst`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/performance/binary-extension-fields.rst` & `galois-0.3.4/docs/performance/binary-extension-fields.rst`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/performance/prime-fields.rst` & `galois-0.3.4/docs/performance/prime-fields.rst`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/release-notes/v0.0.15.md` & `galois-0.3.4/docs/release-notes/v0.0.15.md`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/release-notes/v0.0.16.md` & `galois-0.3.4/docs/release-notes/v0.0.16.md`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/release-notes/v0.0.17.md` & `galois-0.3.4/docs/release-notes/v0.0.17.md`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/release-notes/v0.0.18.md` & `galois-0.3.4/docs/release-notes/v0.0.18.md`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/release-notes/v0.0.19.md` & `galois-0.3.4/docs/release-notes/v0.0.19.md`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/release-notes/v0.0.20.md` & `galois-0.3.4/docs/release-notes/v0.0.20.md`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/release-notes/v0.0.22.md` & `galois-0.3.4/docs/release-notes/v0.0.22.md`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/release-notes/v0.0.23.md` & `galois-0.3.4/docs/release-notes/v0.0.23.md`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/release-notes/v0.0.24.md` & `galois-0.3.4/docs/release-notes/v0.0.24.md`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/release-notes/v0.0.25.md` & `galois-0.3.4/docs/release-notes/v0.0.25.md`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/release-notes/v0.0.26.md` & `galois-0.3.4/docs/release-notes/v0.0.26.md`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/release-notes/v0.0.27.md` & `galois-0.3.4/docs/release-notes/v0.0.27.md`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/release-notes/v0.0.28.md` & `galois-0.3.4/docs/release-notes/v0.0.28.md`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/release-notes/v0.0.29.md` & `galois-0.3.4/docs/release-notes/v0.0.29.md`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/release-notes/v0.0.30.md` & `galois-0.3.4/docs/release-notes/v0.0.30.md`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/release-notes/v0.0.31.md` & `galois-0.3.4/docs/release-notes/v0.0.31.md`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/release-notes/v0.0.32.md` & `galois-0.3.4/docs/release-notes/v0.0.32.md`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/release-notes/v0.0.33.md` & `galois-0.3.4/docs/release-notes/v0.0.33.md`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/release-notes/v0.1.1.md` & `galois-0.3.4/docs/release-notes/v0.1.1.md`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/release-notes/v0.1.2.md` & `galois-0.3.4/docs/release-notes/v0.1.2.md`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/release-notes/v0.2.0.md` & `galois-0.3.4/docs/release-notes/v0.2.0.md`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/release-notes/v0.3.0.md` & `galois-0.3.4/docs/release-notes/v0.3.0.md`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/release-notes/v0.3.1.md` & `galois-0.3.4/docs/release-notes/v0.3.1.md`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/release-notes/v0.3.2.md` & `galois-0.3.4/docs/release-notes/v0.3.2.md`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/release-notes/v0.3.3.md` & `galois-0.3.4/docs/release-notes/v0.3.3.md`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/release-notes/versioning.rst` & `galois-0.3.4/docs/release-notes/versioning.rst`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/tutorials/intro-to-extension-fields.rst` & `galois-0.3.4/docs/tutorials/intro-to-extension-fields.rst`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/docs/tutorials/intro-to-prime-fields.rst` & `galois-0.3.4/docs/tutorials/intro-to-prime-fields.rst`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/logo/README.md` & `galois-0.3.4/logo/README.md`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/logo/galois-favicon-color.png` & `galois-0.3.4/logo/galois-favicon-color.png`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/logo/galois-favicon-white.png` & `galois-0.3.4/logo/galois-favicon-white.png`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/logo/galois-github-social.png` & `galois-0.3.4/logo/galois-github-social.png`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/logo/galois-github-social.svg` & `galois-0.3.4/logo/galois-github-social.svg`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/logo/galois-heading.png` & `galois-0.3.4/logo/galois-heading.png`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/logo/galois-logo-small.png` & `galois-0.3.4/logo/galois-logo-small.png`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/logo/galois-logo.png` & `galois-0.3.4/logo/galois-logo.png`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/logo/galois-logo.svg` & `galois-0.3.4/logo/galois-logo.svg`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/pyproject.toml` & `galois-0.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -43,23 +43,24 @@
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Topic :: Security :: Cryptography",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
 requires-python = ">=3.7"
 dependencies = [
-    "numpy >= 1.21.0, < 1.24",  # v1.21.0 is needed for dtype support of ufuncs, see https://numpy.org/devdocs/release/1.21.0-notes.html#ufunc-signature-and-dtype-generalization-and-casting
-    "numba >= 0.55, < 0.57",  # v0.55 is needed for support of NumPy 1.21
+    "numpy >= 1.21.0, < 1.25",  # v1.21.0 is needed for dtype support of ufuncs, see https://numpy.org/devdocs/release/1.21.0-notes.html#ufunc-signature-and-dtype-generalization-and-casting
+    "numba >= 0.55, < 0.58",  # v0.55 is needed for support of NumPy 1.21
     "typing_extensions >= 4.0.0",  # v4.0.0 is needed for use of Self (Python 3.11+) and Literal (Python 3.8+)
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
     "pylint >= 2.14",
```

### Comparing `galois-0.3.3/scripts/create_conway_polys_database.py` & `galois-0.3.4/scripts/create_conway_polys_database.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/scripts/create_irreducible_polys_database.py` & `galois-0.3.4/scripts/create_irreducible_polys_database.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/scripts/create_prime_factors_database.py` & `galois-0.3.4/scripts/create_prime_factors_database.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/scripts/generate_fec_test_vectors.py` & `galois-0.3.4/scripts/generate_fec_test_vectors.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/scripts/generate_field_test_vectors.py` & `galois-0.3.4/scripts/generate_field_test_vectors.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/scripts/generate_int_test_vectors.py` & `galois-0.3.4/scripts/generate_int_test_vectors.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/scripts/sparse_poly_performance_test.py` & `galois-0.3.4/scripts/sparse_poly_performance_test.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/__init__.py` & `galois-0.3.4/src/galois/__init__.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_codes/_bch.py` & `galois-0.3.4/src/galois/_codes/_bch.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_codes/_cyclic.py` & `galois-0.3.4/src/galois/_codes/_cyclic.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_codes/_linear.py` & `galois-0.3.4/src/galois/_codes/_linear.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_codes/_reed_solomon.py` & `galois-0.3.4/src/galois/_codes/_reed_solomon.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_databases/_interface.py` & `galois-0.3.4/src/galois/_databases/_interface.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_databases/conway_polys.db` & `galois-0.3.4/src/galois/_databases/conway_polys.db`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_databases/irreducible_polys.db` & `galois-0.3.4/src/galois/_databases/irreducible_polys.db`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_databases/prime_factors.db` & `galois-0.3.4/src/galois/_databases/prime_factors.db`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_domains/_array.py` & `galois-0.3.4/src/galois/_domains/_array.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_domains/_calculate.py` & `galois-0.3.4/src/galois/_domains/_calculate.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_domains/_factory.py` & `galois-0.3.4/src/galois/_domains/_factory.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_domains/_function.py` & `galois-0.3.4/src/galois/_domains/_function.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_domains/_linalg.py` & `galois-0.3.4/src/galois/_domains/_linalg.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,26 +307,26 @@
     """
 
     def __call__(self, A: Array) -> tuple[Array, Array]:
         verify_isinstance(A, self.field)
         if not A.ndim == 2:
             raise ValueError(f"Argument 'A' must be a 2-D matrix, not have shape {A.shape}.")
 
-        n = A.shape[0]
+        m = A.shape[0]
         Ai = A.copy()
-        L = self.field.Identity(n)
+        L = self.field.Identity(m)
 
-        for i in range(0, n - 1):
+        for i in range(0, m - 1):
             if Ai[i, i] == 0:
                 idxs = np.nonzero(Ai[i:, i])[0]  # The first non-zero entry in column `i` below row `i`
                 if idxs.size == 0:  # pylint: disable=no-else-continue
                     L[i, i] = 1
                     continue
                 else:
-                    raise ValueError("The LU decomposition of 'A' does not exist. Use the LUP decomposition instead.")
+                    raise ValueError("The LU decomposition of 'A' does not exist. Use the PLU decomposition instead.")
 
             l = Ai[i + 1 :, i] / Ai[i, i]
             Ai[i + 1 :, :] -= np.multiply.outer(l, Ai[i, :])
             L[i + 1 :, i] = l
 
         U = Ai
 
@@ -339,21 +339,21 @@
     """
 
     def __call__(self, A: Array) -> tuple[Array, Array, Array, int]:
         verify_isinstance(A, self.field)
         if not A.ndim == 2:
             raise ValueError(f"Argument 'A' must be a 2-D matrix, not have shape {A.shape}.")
 
-        n = A.shape[0]
+        m, n = A.shape
         Ai = A.copy()
-        L = self.field.Zeros((n, n))
-        P = self.field.Identity(n)  # Row permutation matrix
+        L = self.field.Zeros((m, m))
+        P = self.field.Identity(m)  # Row permutation matrix
         N_permutations = 0  # Number of permutations
 
-        for i in range(0, n - 1):
+        for i in range(0, min(m, n)):
             if Ai[i, i] == 0:
                 idxs = np.nonzero(Ai[i:, i])[0]  # The first non-zero entry in column `i` below row `i`
                 if idxs.size == 0:
                     L[i, i] = 1
                     continue
                 j = i + idxs[0]
```

### Comparing `galois-0.3.3/src/galois/_domains/_lookup.py` & `galois-0.3.4/src/galois/_domains/_lookup.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_domains/_meta.py` & `galois-0.3.4/src/galois/_domains/_meta.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_domains/_ufunc.py` & `galois-0.3.4/src/galois/_domains/_ufunc.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_fields/_array.py` & `galois-0.3.4/src/galois/_fields/_array.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_fields/_factory.py` & `galois-0.3.4/src/galois/_fields/_factory.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_fields/_gf2.py` & `galois-0.3.4/src/galois/_fields/_gf2.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_fields/_meta.py` & `galois-0.3.4/src/galois/_fields/_meta.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_fields/_primitive_element.py` & `galois-0.3.4/src/galois/_fields/_primitive_element.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_fields/_ufunc.py` & `galois-0.3.4/src/galois/_fields/_ufunc.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_helper.py` & `galois-0.3.4/src/galois/_helper.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_lfsr.py` & `galois-0.3.4/src/galois/_lfsr.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_math.py` & `galois-0.3.4/src/galois/_math.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_modular.py` & `galois-0.3.4/src/galois/_modular.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_ntt.py` & `galois-0.3.4/src/galois/_ntt.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_options.py` & `galois-0.3.4/src/galois/_options.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_polymorphic.py` & `galois-0.3.4/src/galois/_polymorphic.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_polys/_binary.py` & `galois-0.3.4/src/galois/_polys/_binary.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_polys/_conversions.py` & `galois-0.3.4/src/galois/_polys/_conversions.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_polys/_conway.py` & `galois-0.3.4/src/galois/_polys/_conway.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_polys/_dense.py` & `galois-0.3.4/src/galois/_polys/_dense.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_polys/_factor.py` & `galois-0.3.4/src/galois/_polys/_factor.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_polys/_functions.py` & `galois-0.3.4/src/galois/_polys/_functions.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_polys/_irreducible.py` & `galois-0.3.4/src/galois/_polys/_irreducible.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_polys/_lagrange.py` & `galois-0.3.4/src/galois/_polys/_lagrange.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_polys/_poly.py` & `galois-0.3.4/src/galois/_polys/_poly.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_polys/_primitive.py` & `galois-0.3.4/src/galois/_polys/_primitive.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_polys/_search.py` & `galois-0.3.4/src/galois/_polys/_search.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_polys/_sparse.py` & `galois-0.3.4/src/galois/_polys/_sparse.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/_prime.py` & `galois-0.3.4/src/galois/_prime.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois/typing.py` & `galois-0.3.4/src/galois/typing.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/src/galois.egg-info/PKG-INFO` & `galois-0.3.4/src/galois.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galois
-Version: 0.3.3
+Version: 0.3.4
 Summary: A performant NumPy extension for Galois fields and their applications
 Author-email: Matt Hostetter <matthostetter@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/mhostetter/galois
 Project-URL: Source, https://github.com/mhostetter/galois
 Project-URL: Issues, https://github.com/mhostetter/galois/issues
 Project-URL: Documentation, https://mhostetter.github.io/galois/latest/
@@ -23,14 +23,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -40,15 +41,15 @@
 
 <div align=center>
   <a href="https://pypi.org/project/galois"><img src="https://img.shields.io/pypi/v/galois"></a>
   <a href="https://pypi.org/project/galois"><img src="https://img.shields.io/pypi/pyversions/galois"></a>
   <a href="https://pypi.org/project/galois"><img src="https://img.shields.io/pypi/wheel/galois"></a>
   <a href="https://pypistats.org/packages/galois"><img src="https://img.shields.io/pypi/dm/galois"></a>
   <a href="https://pypi.org/project/galois"><img src="https://img.shields.io/pypi/l/galois"></a>
-  <a href="https://twitter.com/galois_py"><img src="https://img.shields.io/twitter/follow/galois_py?label=galois_py&style=flat&logo=twitter"></a>
+  <a href="https://twitter.com/galois_py"><img src="https://img.shields.io/static/v1?label=follow&message=@galois_py&color=blue&logo=twitter"></a>
 </div>
 
 <div align=center>
   <a href="https://github.com/mhostetter/galois/actions/workflows/docs.yaml"><img src="https://github.com/mhostetter/galois/actions/workflows/docs.yaml/badge.svg"></a>
   <a href="https://github.com/mhostetter/galois/actions/workflows/lint.yaml"><img src="https://github.com/mhostetter/galois/actions/workflows/lint.yaml/badge.svg"></a>
   <a href="https://github.com/mhostetter/galois/actions/workflows/build.yaml"><img src="https://github.com/mhostetter/galois/actions/workflows/build.yaml/badge.svg"></a>
   <a href="https://github.com/mhostetter/galois/actions/workflows/test.yaml"><img src="https://github.com/mhostetter/galois/actions/workflows/test.yaml/badge.svg"></a>
@@ -112,15 +113,15 @@
 
 Import the `galois` package in Python.
 
 ```python
 In [1]: import galois
 
 In [2]: galois.__version__
-Out[2]: '0.3.3'
+Out[2]: '0.3.4'
 ```
 
 ### Create a [`FieldArray`](https://mhostetter.github.io/galois/latest/api/galois.FieldArray/) subclass
 
 Next, create a [`FieldArray`](https://mhostetter.github.io/galois/latest/api/galois.FieldArray/) subclass
 for the specific finite field you'd like to work in. This is created using the `galois.GF()` class factory. In this example, we are
 working in $\mathrm{GF}(3^5)$.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: galois Version: 0.3.3 Summary: A performant NumPy
+Metadata-Version: 2.1 Name: galois Version: 0.3.4 Summary: A performant NumPy
 extension for Galois fields and their applications Author-email: Matt Hostetter
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/mhostetter/
 galois Project-URL: Source, https://github.com/mhostetter/galois Project-URL:
 Issues, https://github.com/mhostetter/galois/issues Project-URL: Documentation,
 https://mhostetter.github.io/galois/latest/ Project-URL: Discuss, https://
 github.com/mhostetter/galois/discussions Project-URL: Changelog, https://
 mhostetter.github.io/galois/latest/release-notes/versioning/ Project-URL:
@@ -15,25 +15,26 @@
 Classifier: Intended Audience :: Telecommunications Industry Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: POSIX :: Linux Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Topic :: Scientific/
-Engineering :: Mathematics Classifier: Topic :: Security :: Cryptography
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Typing :: Typed Requires-Python: >=3.7 Description-Content-Type:
-text/markdown Provides-Extra: dev License-File: LICENSE # ![Galois: A
-performant NumPy extension for Galois fields and their applications](https://
-raw.githubusercontent.com/mhostetter/galois/master/logo/galois-heading.png)
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Security :: Cryptography Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Classifier: Typing :: Typed
+Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra:
+dev License-File: LICENSE # ![Galois: A performant NumPy extension for Galois
+fields and their applications](https://raw.githubusercontent.com/mhostetter/
+galois/master/logo/galois-heading.png)
 [https://img.shields.io/pypi/v/galois] [https://img.shields.io/pypi/pyversions/
   galois] [https://img.shields.io/pypi/wheel/galois] [https://img.shields.io/
 pypi/dm/galois] [https://img.shields.io/pypi/l/galois] [https://img.shields.io/
-       twitter/follow/galois_py?label=galois_py&style=flat&logo=twitter]
+      static/v1?label=follow&message=@galois_py&color=blue&logo=twitter]
  [https://github.com/mhostetter/galois/actions/workflows/docs.yaml/badge.svg]
  [https://github.com/mhostetter/galois/actions/workflows/lint.yaml/badge.svg]
 [https://github.com/mhostetter/galois/actions/workflows/build.yaml/badge.svg]
  [https://github.com/mhostetter/galois/actions/workflows/test.yaml/badge.svg]
          [https://codecov.io/gh/mhostetter/galois/branch/master/graph/
                           badge.svg?token=3FJML79ZUK]
 The `galois` library is a Python 3 package that extends NumPy arrays to operate
@@ -91,15 +92,15 @@
 ) guide is intended to assist the user with installing the library, creating
 two example arrays, and performing basic array arithmetic. See [Basic Usage]
 (https://mhostetter.github.io/galois/latest/basic-usage/array-classes/) for
 more detailed discussions and examples. ### Install the package The latest
 version of `galois` can be installed from [PyPI](https://pypi.org/project/
 galois/) using `pip`. ```console $ python3 -m pip install galois ``` Import the
 `galois` package in Python. ```python In [1]: import galois In [2]:
-galois.__version__ Out[2]: '0.3.3' ``` ### Create a [`FieldArray`](https://
+galois.__version__ Out[2]: '0.3.4' ``` ### Create a [`FieldArray`](https://
 mhostetter.github.io/galois/latest/api/galois.FieldArray/) subclass Next,
 create a [`FieldArray`](https://mhostetter.github.io/galois/latest/api/
 galois.FieldArray/) subclass for the specific finite field you'd like to work
 in. This is created using the `galois.GF()` class factory. In this example, we
 are working in $\mathrm{GF}(3^5)$. ```python In [3]: GF = galois.GF(3**5) In
 [4]: print(GF.properties) Galois Field: name: GF(3^5) characteristic: 3 degree:
 5 order: 243 irreducible_poly: x^5 + 2x + 1 is_primitive_poly: True
```

### Comparing `galois-0.3.3/src/galois.egg-info/SOURCES.txt` & `galois-0.3.4/src/galois.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 docs/release-notes/v0.1.1.md
 docs/release-notes/v0.1.2.md
 docs/release-notes/v0.2.0.md
 docs/release-notes/v0.3.0.md
 docs/release-notes/v0.3.1.md
 docs/release-notes/v0.3.2.md
 docs/release-notes/v0.3.3.md
+docs/release-notes/v0.3.4.md
 docs/release-notes/versioning.rst
 docs/tutorials/intro-to-extension-fields.rst
 docs/tutorials/intro-to-prime-fields.rst
 logo/README.md
 logo/galois-favicon-color.png
 logo/galois-favicon-white.png
 logo/galois-github-social.png
```

### Comparing `galois-0.3.3/tests/codes/conftest.py` & `galois-0.3.4/tests/codes/conftest.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k10_d2_alpha6_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k10_d2_alpha6_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k10_d2_alpha6_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k10_d2_alpha6_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k10_d2_alpha9_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k10_d2_alpha9_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k10_d2_alpha9_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k10_d2_alpha9_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k10_d2_alpha9_c3_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k10_d2_alpha9_c3_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k10_d2_alpha9_c3_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k10_d2_alpha9_c3_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k13_d1_alpha6_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k13_d1_alpha6_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k13_d1_alpha6_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k13_d1_alpha6_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k13_d1_alpha9_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k13_d1_alpha9_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k13_d1_alpha9_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k13_d1_alpha9_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k13_d1_alpha9_c3_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k13_d1_alpha9_c3_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k13_d1_alpha9_c3_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k13_d1_alpha9_c3_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k1_d6_alpha9_c3_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k1_d6_alpha9_c3_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k1_d6_alpha9_c3_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k1_d6_alpha9_c3_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k1_d7_alpha9_c3_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k1_d7_alpha9_c3_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k1_d7_alpha9_c3_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k1_d7_alpha9_c3_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k1_d8_alpha6_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k1_d8_alpha6_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k1_d8_alpha6_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k1_d8_alpha6_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k1_d8_alpha9_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k1_d8_alpha9_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k1_d8_alpha9_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k1_d8_alpha9_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k1_d8_alpha9_c3_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k1_d8_alpha9_c3_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k1_d8_alpha9_c3_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k1_d8_alpha9_c3_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k4_d4_alpha9_c3_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k4_d4_alpha9_c3_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k4_d4_alpha9_c3_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k4_d4_alpha9_c3_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k4_d5_alpha6_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k4_d5_alpha6_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k4_d5_alpha6_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k4_d5_alpha6_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k4_d5_alpha9_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k4_d5_alpha9_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k4_d5_alpha9_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k4_d5_alpha9_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k4_d5_alpha9_c3_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k4_d5_alpha9_c3_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k4_d5_alpha9_c3_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k4_d5_alpha9_c3_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k4_d6_alpha6_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k4_d6_alpha6_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k4_d6_alpha6_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k4_d6_alpha6_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k4_d6_alpha9_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k4_d6_alpha9_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k4_d6_alpha9_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k4_d6_alpha9_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k4_d7_alpha6_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k4_d7_alpha6_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k4_d7_alpha6_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k4_d7_alpha6_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k4_d7_alpha9_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k4_d7_alpha9_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k4_d7_alpha9_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k4_d7_alpha9_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k7_d3_alpha6_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k7_d3_alpha6_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k7_d3_alpha6_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k7_d3_alpha6_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k7_d3_alpha9_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k7_d3_alpha9_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k7_d3_alpha9_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k7_d3_alpha9_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k7_d3_alpha9_c3_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k7_d3_alpha9_c3_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k7_d3_alpha9_c3_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k7_d3_alpha9_c3_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k7_d4_alpha6_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k7_d4_alpha6_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k7_d4_alpha6_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k7_d4_alpha6_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k7_d4_alpha9_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k7_d4_alpha9_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n13_k7_d4_alpha9_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n13_k7_d4_alpha9_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k11_d2_alpha2_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k11_d2_alpha2_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k11_d2_alpha2_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k11_d2_alpha2_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k11_d2_alpha2_c3_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k11_d2_alpha2_c3_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k11_d2_alpha2_c3_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k11_d2_alpha2_c3_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k11_d2_alpha9_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k11_d2_alpha9_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k11_d2_alpha9_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k11_d2_alpha9_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k11_d3_alpha2_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k11_d3_alpha2_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k11_d3_alpha2_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k11_d3_alpha2_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k11_d3_alpha9_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k11_d3_alpha9_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k11_d3_alpha9_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k11_d3_alpha9_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k15_d1_alpha2_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k15_d1_alpha2_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k15_d1_alpha2_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k15_d1_alpha2_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k15_d1_alpha2_c3_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k15_d1_alpha2_c3_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k15_d1_alpha2_c3_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k15_d1_alpha2_c3_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k15_d1_alpha9_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k15_d1_alpha9_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k15_d1_alpha9_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k15_d1_alpha9_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k1_d6_alpha2_c3_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k1_d6_alpha2_c3_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k1_d6_alpha2_c3_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k1_d6_alpha2_c3_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k1_d7_alpha2_c3_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k1_d7_alpha2_c3_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k1_d7_alpha2_c3_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k1_d7_alpha2_c3_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k1_d8_alpha2_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k1_d8_alpha2_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k1_d8_alpha2_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k1_d8_alpha2_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k1_d8_alpha2_c3_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k1_d8_alpha2_c3_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k1_d8_alpha2_c3_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k1_d8_alpha2_c3_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k1_d8_alpha9_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k1_d8_alpha9_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k1_d8_alpha9_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k1_d8_alpha9_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k5_d4_alpha2_c3_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k5_d4_alpha2_c3_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k5_d4_alpha2_c3_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k5_d4_alpha2_c3_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k5_d5_alpha2_c3_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k5_d5_alpha2_c3_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k5_d5_alpha2_c3_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k5_d5_alpha2_c3_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k5_d6_alpha2_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k5_d6_alpha2_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k5_d6_alpha2_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k5_d6_alpha2_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k5_d6_alpha9_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k5_d6_alpha9_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k5_d6_alpha9_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k5_d6_alpha9_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k5_d7_alpha2_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k5_d7_alpha2_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k5_d7_alpha2_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k5_d7_alpha2_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k5_d7_alpha9_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k5_d7_alpha9_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k5_d7_alpha9_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k5_d7_alpha9_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k7_d3_alpha2_c3_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k7_d3_alpha2_c3_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k7_d3_alpha2_c3_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k7_d3_alpha2_c3_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k7_d4_alpha2_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k7_d4_alpha2_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k7_d4_alpha2_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k7_d4_alpha2_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k7_d4_alpha9_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k7_d4_alpha9_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k7_d4_alpha9_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k7_d4_alpha9_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k7_d5_alpha2_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k7_d5_alpha2_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k7_d5_alpha2_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k7_d5_alpha2_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k7_d5_alpha9_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k7_d5_alpha9_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n15_k7_d5_alpha9_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n15_k7_d5_alpha9_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k11_d6_alpha3_c3_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k11_d6_alpha3_c3_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k11_d6_alpha3_c3_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k11_d6_alpha3_c3_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k11_d8_alpha17_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k11_d8_alpha17_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k11_d8_alpha17_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k11_d8_alpha17_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k11_d8_alpha3_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k11_d8_alpha3_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k11_d8_alpha3_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k11_d8_alpha3_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k14_d5_alpha3_c3_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k14_d5_alpha3_c3_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k14_d5_alpha3_c3_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k14_d5_alpha3_c3_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k14_d6_alpha17_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k14_d6_alpha17_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k14_d6_alpha17_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k14_d6_alpha17_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k14_d6_alpha3_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k14_d6_alpha3_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k14_d6_alpha3_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k14_d6_alpha3_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k14_d7_alpha17_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k14_d7_alpha17_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k14_d7_alpha17_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k14_d7_alpha17_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k14_d7_alpha3_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k14_d7_alpha3_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k14_d7_alpha3_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k14_d7_alpha3_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k17_d4_alpha3_c3_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k17_d4_alpha3_c3_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k17_d4_alpha3_c3_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k17_d4_alpha3_c3_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k17_d5_alpha17_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k17_d5_alpha17_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k17_d5_alpha17_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k17_d5_alpha17_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k17_d5_alpha3_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k17_d5_alpha3_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k17_d5_alpha3_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k17_d5_alpha3_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k1_d16_alpha3_c3_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k1_d16_alpha3_c3_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k1_d16_alpha3_c3_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k1_d16_alpha3_c3_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k1_d17_alpha3_c3_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k1_d17_alpha3_c3_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k1_d17_alpha3_c3_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k1_d17_alpha3_c3_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k1_d18_alpha17_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k1_d18_alpha17_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k1_d18_alpha17_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k1_d18_alpha17_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k1_d18_alpha3_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k1_d18_alpha3_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k1_d18_alpha3_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k1_d18_alpha3_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k1_d18_alpha3_c3_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k1_d18_alpha3_c3_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k1_d18_alpha3_c3_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k1_d18_alpha3_c3_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k20_d3_alpha17_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k20_d3_alpha17_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k20_d3_alpha17_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k20_d3_alpha17_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k20_d3_alpha3_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k20_d3_alpha3_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k20_d3_alpha3_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k20_d3_alpha3_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k20_d3_alpha3_c3_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k20_d3_alpha3_c3_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k20_d3_alpha3_c3_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k20_d3_alpha3_c3_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k20_d4_alpha17_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k20_d4_alpha17_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k20_d4_alpha17_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k20_d4_alpha17_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k20_d4_alpha3_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k20_d4_alpha3_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k20_d4_alpha3_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k20_d4_alpha3_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k23_d2_alpha17_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k23_d2_alpha17_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k23_d2_alpha17_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k23_d2_alpha17_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k23_d2_alpha3_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k23_d2_alpha3_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k23_d2_alpha3_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k23_d2_alpha3_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k23_d2_alpha3_c3_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k23_d2_alpha3_c3_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k23_d2_alpha3_c3_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k23_d2_alpha3_c3_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k26_d1_alpha17_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k26_d1_alpha17_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k26_d1_alpha17_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k26_d1_alpha17_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k26_d1_alpha3_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k26_d1_alpha3_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k26_d1_alpha3_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k26_d1_alpha3_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k26_d1_alpha3_c3_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k26_d1_alpha3_c3_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k26_d1_alpha3_c3_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k26_d1_alpha3_c3_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k4_d13_alpha3_c3_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k4_d13_alpha3_c3_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k4_d13_alpha3_c3_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k4_d13_alpha3_c3_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k4_d14_alpha3_c3_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k4_d14_alpha3_c3_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k4_d14_alpha3_c3_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k4_d14_alpha3_c3_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k4_d15_alpha17_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k4_d15_alpha17_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k4_d15_alpha17_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k4_d15_alpha17_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k4_d15_alpha3_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k4_d15_alpha3_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k4_d15_alpha3_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k4_d15_alpha3_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k4_d15_alpha3_c3_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k4_d15_alpha3_c3_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k4_d15_alpha3_c3_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k4_d15_alpha3_c3_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k4_d16_alpha17_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k4_d16_alpha17_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k4_d16_alpha17_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k4_d16_alpha17_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k4_d16_alpha3_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k4_d16_alpha3_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k4_d16_alpha3_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k4_d16_alpha3_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k4_d17_alpha17_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k4_d17_alpha17_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k4_d17_alpha17_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k4_d17_alpha17_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k4_d17_alpha3_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k4_d17_alpha3_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k4_d17_alpha3_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k4_d17_alpha3_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k7_d12_alpha3_c3_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k7_d12_alpha3_c3_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k7_d12_alpha3_c3_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k7_d12_alpha3_c3_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k7_d14_alpha17_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k7_d14_alpha17_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k7_d14_alpha17_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k7_d14_alpha17_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k7_d14_alpha3_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k7_d14_alpha3_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k7_d14_alpha3_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k7_d14_alpha3_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k8_d10_alpha17_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k8_d10_alpha17_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k8_d10_alpha17_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k8_d10_alpha17_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k8_d10_alpha3_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k8_d10_alpha3_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k8_d10_alpha3_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k8_d10_alpha3_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k8_d10_alpha3_c3_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k8_d10_alpha3_c3_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k8_d10_alpha3_c3_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k8_d10_alpha3_c3_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k8_d11_alpha17_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k8_d11_alpha17_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k8_d11_alpha17_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k8_d11_alpha17_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k8_d11_alpha3_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k8_d11_alpha3_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k8_d11_alpha3_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k8_d11_alpha3_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k8_d11_alpha3_c3_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k8_d11_alpha3_c3_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k8_d11_alpha3_c3_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k8_d11_alpha3_c3_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k8_d12_alpha17_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k8_d12_alpha17_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k8_d12_alpha17_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k8_d12_alpha17_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k8_d12_alpha3_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k8_d12_alpha3_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k8_d12_alpha3_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k8_d12_alpha3_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k8_d13_alpha17_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k8_d13_alpha17_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k8_d13_alpha17_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k8_d13_alpha17_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k8_d13_alpha3_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k8_d13_alpha3_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k8_d13_alpha3_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k8_d13_alpha3_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k8_d7_alpha3_c3_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k8_d7_alpha3_c3_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k8_d7_alpha3_c3_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k8_d7_alpha3_c3_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k8_d8_alpha3_c3_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k8_d8_alpha3_c3_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k8_d8_alpha3_c3_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k8_d8_alpha3_c3_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k8_d9_alpha17_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k8_d9_alpha17_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k8_d9_alpha17_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k8_d9_alpha17_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k8_d9_alpha3_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k8_d9_alpha3_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k8_d9_alpha3_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k8_d9_alpha3_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k8_d9_alpha3_c3_nonsys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k8_d9_alpha3_c3_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/bch/n26_k8_d9_alpha3_c3_sys.pkl` & `galois-0.3.4/tests/codes/data/bch/n26_k8_d9_alpha3_c3_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n15_k10_d6_alpha2_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n15_k10_d6_alpha2_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n15_k10_d6_alpha2_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n15_k10_d6_alpha2_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n15_k10_d6_alpha9_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n15_k10_d6_alpha9_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n15_k10_d6_alpha9_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n15_k10_d6_alpha9_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n15_k11_d5_alpha2_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n15_k11_d5_alpha2_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n15_k11_d5_alpha2_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n15_k11_d5_alpha2_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n15_k11_d5_alpha9_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n15_k11_d5_alpha9_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n15_k11_d5_alpha9_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n15_k11_d5_alpha9_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n15_k12_d4_alpha2_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n15_k12_d4_alpha2_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n15_k12_d4_alpha2_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n15_k12_d4_alpha2_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n15_k12_d4_alpha9_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n15_k12_d4_alpha9_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n15_k12_d4_alpha9_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n15_k12_d4_alpha9_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n15_k13_d3_alpha2_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n15_k13_d3_alpha2_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n15_k13_d3_alpha2_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n15_k13_d3_alpha2_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n15_k13_d3_alpha9_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n15_k13_d3_alpha9_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n15_k13_d3_alpha9_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n15_k13_d3_alpha9_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n15_k14_d2_alpha2_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n15_k14_d2_alpha2_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n15_k14_d2_alpha2_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n15_k14_d2_alpha2_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n15_k14_d2_alpha9_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n15_k14_d2_alpha9_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n15_k14_d2_alpha9_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n15_k14_d2_alpha9_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n15_k8_d8_alpha2_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n15_k8_d8_alpha2_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n15_k8_d8_alpha2_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n15_k8_d8_alpha2_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n15_k8_d8_alpha9_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n15_k8_d8_alpha9_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n15_k8_d8_alpha9_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n15_k8_d8_alpha9_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n15_k9_d7_alpha2_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n15_k9_d7_alpha2_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n15_k9_d7_alpha2_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n15_k9_d7_alpha2_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n15_k9_d7_alpha9_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n15_k9_d7_alpha9_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n15_k9_d7_alpha9_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n15_k9_d7_alpha9_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n16_k10_d7_alpha11_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n16_k10_d7_alpha11_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n16_k10_d7_alpha11_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n16_k10_d7_alpha11_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n16_k10_d7_alpha31_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n16_k10_d7_alpha31_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n16_k10_d7_alpha31_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n16_k10_d7_alpha31_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n16_k11_d6_alpha11_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n16_k11_d6_alpha11_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n16_k11_d6_alpha11_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n16_k11_d6_alpha11_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n16_k11_d6_alpha31_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n16_k11_d6_alpha31_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n16_k11_d6_alpha31_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n16_k11_d6_alpha31_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n16_k12_d5_alpha11_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n16_k12_d5_alpha11_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n16_k12_d5_alpha11_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n16_k12_d5_alpha11_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n16_k12_d5_alpha31_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n16_k12_d5_alpha31_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n16_k12_d5_alpha31_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n16_k12_d5_alpha31_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n16_k13_d4_alpha11_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n16_k13_d4_alpha11_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n16_k13_d4_alpha11_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n16_k13_d4_alpha11_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n16_k13_d4_alpha31_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n16_k13_d4_alpha31_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n16_k13_d4_alpha31_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n16_k13_d4_alpha31_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n16_k14_d3_alpha11_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n16_k14_d3_alpha11_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n16_k14_d3_alpha11_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n16_k14_d3_alpha11_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n16_k14_d3_alpha31_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n16_k14_d3_alpha31_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n16_k14_d3_alpha31_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n16_k14_d3_alpha31_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n16_k15_d2_alpha11_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n16_k15_d2_alpha11_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n16_k15_d2_alpha11_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n16_k15_d2_alpha11_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n16_k15_d2_alpha31_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n16_k15_d2_alpha31_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n16_k15_d2_alpha31_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n16_k15_d2_alpha31_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n16_k9_d8_alpha11_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n16_k9_d8_alpha11_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n16_k9_d8_alpha11_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n16_k9_d8_alpha11_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n16_k9_d8_alpha31_c1_nonsys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n16_k9_d8_alpha31_c1_nonsys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/data/reed_solomon/n16_k9_d8_alpha31_c1_sys.pkl` & `galois-0.3.4/tests/codes/data/reed_solomon/n16_k9_d8_alpha31_c1_sys.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/test_bch.py` & `galois-0.3.4/tests/codes/test_bch.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/codes/test_reed_solomon.py` & `galois-0.3.4/tests/codes/test_reed_solomon.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/conftest.py` & `galois-0.3.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/data/crt.pkl` & `galois-0.3.4/tests/data/crt.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/data/egcd.pkl` & `galois-0.3.4/tests/data/egcd.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/data/is_cyclic.pkl` & `galois-0.3.4/tests/data/is_cyclic.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/data/is_perfect_power.pkl` & `galois-0.3.4/tests/data/is_perfect_power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/data/is_powersmooth.pkl` & `galois-0.3.4/tests/data/is_powersmooth.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/data/is_smooth.pkl` & `galois-0.3.4/tests/data/is_smooth.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/data/is_square_free.pkl` & `galois-0.3.4/tests/data/is_square_free.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/data/lcm.pkl` & `galois-0.3.4/tests/data/lcm.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/data/primes.pkl` & `galois-0.3.4/tests/data/primes.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/data/prod.pkl` & `galois-0.3.4/tests/data/prod.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/conftest.py` & `galois-0.3.4/tests/fields/conftest.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(109987^4)/add.pkl` & `galois-0.3.4/tests/fields/data/GF(109987^4)/add.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(109987^4)/additive_inverse.pkl` & `galois-0.3.4/tests/fields/data/GF(109987^4)/additive_inverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(109987^4)/characteristic_poly_element.pkl` & `galois-0.3.4/tests/fields/data/GF(109987^4)/characteristic_poly_element.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(109987^4)/characteristic_poly_matrix.pkl` & `galois-0.3.4/tests/fields/data/GF(109987^4)/characteristic_poly_matrix.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(109987^4)/column_space.pkl` & `galois-0.3.4/tests/fields/data/GF(109987^4)/column_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(109987^4)/convolve.pkl` & `galois-0.3.4/tests/fields/data/GF(109987^4)/convolve.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(109987^4)/divide.pkl` & `galois-0.3.4/tests/fields/data/GF(109987^4)/divide.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(109987^4)/left_null_space.pkl` & `galois-0.3.4/tests/fields/data/GF(109987^4)/left_null_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(109987^4)/log.pkl` & `galois-0.3.4/tests/fields/data/GF(109987^4)/log.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(109987^4)/lu_decompose.pkl` & `galois-0.3.4/tests/fields/data/GF(109987^4)/lu_decompose.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(109987^4)/matrix_determinant.pkl` & `galois-0.3.4/tests/fields/data/GF(109987^4)/matrix_determinant.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(109987^4)/matrix_inverse.pkl` & `galois-0.3.4/tests/fields/data/GF(109987^4)/matrix_inverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(109987^4)/matrix_multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(109987^4)/matrix_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(109987^4)/matrix_solve.pkl` & `galois-0.3.4/tests/fields/data/GF(109987^4)/matrix_solve.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(109987^4)/minimal_poly_element.pkl` & `galois-0.3.4/tests/fields/data/GF(109987^4)/minimal_poly_element.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(109987^4)/multiplicative_inverse.pkl` & `galois-0.3.4/tests/fields/data/GF(109987^4)/multiplicative_inverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(109987^4)/multiplicative_order.pkl` & `galois-0.3.4/tests/fields/data/GF(109987^4)/multiplicative_order.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(109987^4)/multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(109987^4)/multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(109987^4)/null_space.pkl` & `galois-0.3.4/tests/fields/data/GF(109987^4)/null_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(109987^4)/plu_decompose.pkl` & `galois-0.3.4/tests/fields/data/GF(109987^4)/plu_decompose.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(109987^4)/power.pkl` & `galois-0.3.4/tests/fields/data/GF(109987^4)/power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(109987^4)/row_reduce.pkl` & `galois-0.3.4/tests/fields/data/GF(109987^4)/row_reduce.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(109987^4)/row_space.pkl` & `galois-0.3.4/tests/fields/data/GF(109987^4)/row_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(109987^4)/scalar_multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(109987^4)/scalar_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(109987^4)/subtract.pkl` & `galois-0.3.4/tests/fields/data/GF(109987^4)/subtract.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2)/characteristic_poly_matrix.pkl` & `galois-0.3.4/tests/fields/data/GF(2)/characteristic_poly_matrix.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2)/column_space.pkl` & `galois-0.3.4/tests/fields/data/GF(2)/column_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2)/convolve.pkl` & `galois-0.3.4/tests/fields/data/GF(2)/convolve.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2)/left_null_space.pkl` & `galois-0.3.4/tests/fields/data/GF(2)/left_null_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2)/lu_decompose.pkl` & `galois-0.3.4/tests/fields/data/GF(2)/lu_decompose.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2)/matrix_determinant.pkl` & `galois-0.3.4/tests/fields/data/GF(2)/matrix_determinant.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2)/matrix_inverse.pkl` & `galois-0.3.4/tests/fields/data/GF(2)/matrix_inverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2)/matrix_multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(2)/matrix_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2)/matrix_solve.pkl` & `galois-0.3.4/tests/fields/data/GF(2)/matrix_solve.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2)/null_space.pkl` & `galois-0.3.4/tests/fields/data/GF(2)/null_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2)/plu_decompose.pkl` & `galois-0.3.4/tests/fields/data/GF(2)/plu_decompose.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2)/row_reduce.pkl` & `galois-0.3.4/tests/fields/data/GF(2)/row_reduce.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2)/row_space.pkl` & `galois-0.3.4/tests/fields/data/GF(2)/row_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2147483647)/add.pkl` & `galois-0.3.4/tests/fields/data/GF(2147483647)/add.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2147483647)/characteristic_poly_element.pkl` & `galois-0.3.4/tests/fields/data/GF(2147483647)/characteristic_poly_element.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2147483647)/characteristic_poly_matrix.pkl` & `galois-0.3.4/tests/fields/data/GF(2147483647)/characteristic_poly_matrix.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2147483647)/column_space.pkl` & `galois-0.3.4/tests/fields/data/GF(2147483647)/column_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2147483647)/convolve.pkl` & `galois-0.3.4/tests/fields/data/GF(2147483647)/convolve.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2147483647)/divide.pkl` & `galois-0.3.4/tests/fields/data/GF(2147483647)/divide.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2147483647)/left_null_space.pkl` & `galois-0.3.4/tests/fields/data/GF(2147483647)/left_null_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2147483647)/lu_decompose.pkl` & `galois-0.3.4/tests/fields/data/GF(2147483647)/lu_decompose.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2147483647)/matrix_determinant.pkl` & `galois-0.3.4/tests/fields/data/GF(2147483647)/matrix_determinant.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2147483647)/matrix_inverse.pkl` & `galois-0.3.4/tests/fields/data/GF(2147483647)/matrix_inverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2147483647)/matrix_multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(2147483647)/matrix_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2147483647)/matrix_solve.pkl` & `galois-0.3.4/tests/fields/data/GF(2147483647)/matrix_solve.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2147483647)/minimal_poly_element.pkl` & `galois-0.3.4/tests/fields/data/GF(2147483647)/minimal_poly_element.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2147483647)/multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(2147483647)/multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2147483647)/null_space.pkl` & `galois-0.3.4/tests/fields/data/GF(2147483647)/null_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2147483647)/plu_decompose.pkl` & `galois-0.3.4/tests/fields/data/GF(2147483647)/plu_decompose.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2147483647)/power.pkl` & `galois-0.3.4/tests/fields/data/GF(2147483647)/power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2147483647)/row_reduce.pkl` & `galois-0.3.4/tests/fields/data/GF(2147483647)/row_reduce.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2147483647)/row_space.pkl` & `galois-0.3.4/tests/fields/data/GF(2147483647)/row_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2147483647)/scalar_multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(2147483647)/scalar_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2147483647)/subtract.pkl` & `galois-0.3.4/tests/fields/data/GF(2147483647)/subtract.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^100)/add.pkl` & `galois-0.3.4/tests/fields/data/GF(2^100)/add.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^100)/additive_inverse.pkl` & `galois-0.3.4/tests/fields/data/GF(2^100)/additive_inverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^100)/additive_order.pkl` & `galois-0.3.4/tests/fields/data/GF(2^100)/additive_order.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^100)/characteristic_poly_element.pkl` & `galois-0.3.4/tests/fields/data/GF(2^100)/characteristic_poly_element.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^100)/characteristic_poly_matrix.pkl` & `galois-0.3.4/tests/fields/data/GF(2^100)/characteristic_poly_matrix.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^100)/column_space.pkl` & `galois-0.3.4/tests/fields/data/GF(2^100)/column_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^100)/convolve.pkl` & `galois-0.3.4/tests/fields/data/GF(2^100)/convolve.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^100)/divide.pkl` & `galois-0.3.4/tests/fields/data/GF(2^100)/divide.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^100)/field_norm.pkl` & `galois-0.3.4/tests/fields/data/GF(2^100)/field_norm.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^100)/field_trace.pkl` & `galois-0.3.4/tests/fields/data/GF(2^100)/field_trace.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^100)/left_null_space.pkl` & `galois-0.3.4/tests/fields/data/GF(2^100)/left_null_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^100)/log.pkl` & `galois-0.3.4/tests/fields/data/GF(2^100)/log.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^100)/lu_decompose.pkl` & `galois-0.3.4/tests/fields/data/GF(2^100)/lu_decompose.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^100)/matrix_determinant.pkl` & `galois-0.3.4/tests/fields/data/GF(2^100)/matrix_determinant.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^100)/matrix_inverse.pkl` & `galois-0.3.4/tests/fields/data/GF(2^100)/matrix_inverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^100)/matrix_multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(2^100)/matrix_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^100)/matrix_solve.pkl` & `galois-0.3.4/tests/fields/data/GF(2^100)/matrix_solve.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^100)/minimal_poly_element.pkl` & `galois-0.3.4/tests/fields/data/GF(2^100)/minimal_poly_element.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^100)/multiplicative_inverse.pkl` & `galois-0.3.4/tests/fields/data/GF(2^100)/multiplicative_inverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^100)/multiplicative_order.pkl` & `galois-0.3.4/tests/fields/data/GF(2^100)/multiplicative_order.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^100)/multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(2^100)/multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^100)/null_space.pkl` & `galois-0.3.4/tests/fields/data/GF(2^100)/null_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^100)/plu_decompose.pkl` & `galois-0.3.4/tests/fields/data/GF(2^100)/plu_decompose.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^100)/power.pkl` & `galois-0.3.4/tests/fields/data/GF(2^100)/power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^100)/properties.json` & `galois-0.3.4/tests/fields/data/GF(2^100)/properties.json`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^100)/row_reduce.pkl` & `galois-0.3.4/tests/fields/data/GF(2^100)/row_reduce.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^100)/row_space.pkl` & `galois-0.3.4/tests/fields/data/GF(2^100)/row_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^100)/scalar_multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(2^100)/scalar_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^100)/subtract.pkl` & `galois-0.3.4/tests/fields/data/GF(2^100)/subtract.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^2)/characteristic_poly_matrix.pkl` & `galois-0.3.4/tests/fields/data/GF(2^2)/characteristic_poly_matrix.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^2)/column_space.pkl` & `galois-0.3.4/tests/fields/data/GF(2^2)/column_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^2)/convolve.pkl` & `galois-0.3.4/tests/fields/data/GF(2^2)/convolve.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^2)/left_null_space.pkl` & `galois-0.3.4/tests/fields/data/GF(2^2)/left_null_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^2)/lu_decompose.pkl` & `galois-0.3.4/tests/fields/data/GF(2^2)/lu_decompose.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^2)/matrix_determinant.pkl` & `galois-0.3.4/tests/fields/data/GF(2^2)/matrix_determinant.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^2)/matrix_inverse.pkl` & `galois-0.3.4/tests/fields/data/GF(2^2)/matrix_inverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^2)/matrix_multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(2^2)/matrix_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^2)/matrix_solve.pkl` & `galois-0.3.4/tests/fields/data/GF(2^2)/matrix_solve.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^2)/null_space.pkl` & `galois-0.3.4/tests/fields/data/GF(2^2)/null_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^2)/plu_decompose.pkl` & `galois-0.3.4/tests/fields/data/GF(2^2)/plu_decompose.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^2)/power.pkl` & `galois-0.3.4/tests/fields/data/GF(2^2)/power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^2)/row_reduce.pkl` & `galois-0.3.4/tests/fields/data/GF(2^2)/row_reduce.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^2)/row_space.pkl` & `galois-0.3.4/tests/fields/data/GF(2^2)/row_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^2)/scalar_multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(2^2)/scalar_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^3)/add.pkl` & `galois-0.3.4/tests/fields/data/GF(2^3)/add.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^3)/characteristic_poly_matrix.pkl` & `galois-0.3.4/tests/fields/data/GF(2^3)/characteristic_poly_matrix.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^3)/column_space.pkl` & `galois-0.3.4/tests/fields/data/GF(2^3)/column_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^3)/convolve.pkl` & `galois-0.3.4/tests/fields/data/GF(2^3)/convolve.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^3)/divide.pkl` & `galois-0.3.4/tests/fields/data/GF(2^3)/divide.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^3)/left_null_space.pkl` & `galois-0.3.4/tests/fields/data/GF(2^3)/left_null_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^3)/lu_decompose.pkl` & `galois-0.3.4/tests/fields/data/GF(2^3)/lu_decompose.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^3)/matrix_determinant.pkl` & `galois-0.3.4/tests/fields/data/GF(2^3)/matrix_determinant.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^3)/matrix_inverse.pkl` & `galois-0.3.4/tests/fields/data/GF(2^3)/matrix_inverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^3)/matrix_multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(2^3)/matrix_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^3)/matrix_solve.pkl` & `galois-0.3.4/tests/fields/data/GF(2^3)/matrix_solve.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^3)/multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(2^3)/multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^3)/null_space.pkl` & `galois-0.3.4/tests/fields/data/GF(2^3)/null_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^3)/plu_decompose.pkl` & `galois-0.3.4/tests/fields/data/GF(2^3)/plu_decompose.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^3)/power.pkl` & `galois-0.3.4/tests/fields/data/GF(2^3)/power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^3)/row_reduce.pkl` & `galois-0.3.4/tests/fields/data/GF(2^3)/row_reduce.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^3)/row_space.pkl` & `galois-0.3.4/tests/fields/data/GF(2^3)/row_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^3)/scalar_multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(2^3)/scalar_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^3)/subtract.pkl` & `galois-0.3.4/tests/fields/data/GF(2^3)/subtract.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^32)/add.pkl` & `galois-0.3.4/tests/fields/data/GF(2^32)/add.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^32)/characteristic_poly_element.pkl` & `galois-0.3.4/tests/fields/data/GF(2^32)/characteristic_poly_element.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^32)/characteristic_poly_matrix.pkl` & `galois-0.3.4/tests/fields/data/GF(2^32)/characteristic_poly_matrix.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^32)/column_space.pkl` & `galois-0.3.4/tests/fields/data/GF(2^32)/column_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^32)/convolve.pkl` & `galois-0.3.4/tests/fields/data/GF(2^32)/convolve.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^32)/divide.pkl` & `galois-0.3.4/tests/fields/data/GF(2^32)/divide.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^32)/left_null_space.pkl` & `galois-0.3.4/tests/fields/data/GF(2^32)/left_null_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^32)/lu_decompose.pkl` & `galois-0.3.4/tests/fields/data/GF(2^32)/lu_decompose.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^32)/matrix_determinant.pkl` & `galois-0.3.4/tests/fields/data/GF(2^32)/matrix_determinant.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^32)/matrix_inverse.pkl` & `galois-0.3.4/tests/fields/data/GF(2^32)/matrix_inverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^32)/matrix_multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(2^32)/matrix_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^32)/matrix_solve.pkl` & `galois-0.3.4/tests/fields/data/GF(2^32)/matrix_solve.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^32)/minimal_poly_element.pkl` & `galois-0.3.4/tests/fields/data/GF(2^32)/minimal_poly_element.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^32)/multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(2^32)/multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^32)/null_space.pkl` & `galois-0.3.4/tests/fields/data/GF(2^32)/null_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^32)/plu_decompose.pkl` & `galois-0.3.4/tests/fields/data/GF(2^32)/plu_decompose.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^32)/power.pkl` & `galois-0.3.4/tests/fields/data/GF(2^32)/power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^32)/row_reduce.pkl` & `galois-0.3.4/tests/fields/data/GF(2^32)/row_reduce.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^32)/row_space.pkl` & `galois-0.3.4/tests/fields/data/GF(2^32)/row_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^32)/scalar_multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(2^32)/scalar_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^32)/subtract.pkl` & `galois-0.3.4/tests/fields/data/GF(2^32)/subtract.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8)/add.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8)/add.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8)/additive_inverse.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8)/additive_inverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8)/additive_order.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8)/additive_order.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8)/characteristic_poly_element.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8)/characteristic_poly_element.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8)/characteristic_poly_matrix.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8)/characteristic_poly_matrix.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8)/column_space.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8)/column_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8)/convolve.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8)/convolve.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8)/divide.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8)/divide.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8)/field_norm.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8)/field_norm.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8)/field_trace.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8)/field_trace.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8)/left_null_space.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8)/left_null_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8)/log.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8)/log.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8)/lu_decompose.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8)/lu_decompose.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8)/matrix_determinant.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8)/matrix_determinant.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8)/matrix_inverse.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8)/matrix_inverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8)/matrix_multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8)/matrix_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8)/matrix_solve.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8)/matrix_solve.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8)/minimal_poly_element.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8)/minimal_poly_element.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8)/multiplicative_inverse.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8)/multiplicative_inverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8)/multiplicative_order.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8)/multiplicative_order.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8)/multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8)/multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8)/null_space.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8)/null_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8)/plu_decompose.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8)/plu_decompose.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8)/power.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8)/power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8)/row_reduce.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8)/row_reduce.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8)/row_space.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8)/row_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8)/scalar_multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8)/scalar_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8)/subtract.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8)/subtract.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/add.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/add.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/additive_inverse.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/additive_inverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/additive_order.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/additive_order.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/characteristic_poly_element.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/characteristic_poly_element.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/characteristic_poly_matrix.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/characteristic_poly_matrix.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/column_space.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/column_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/convolve.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/convolve.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/divide.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/divide.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/field_norm.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/field_norm.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/field_trace.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/field_trace.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/left_null_space.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/left_null_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/log.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/log.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/lu_decompose.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/lu_decompose.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/matrix_determinant.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/matrix_determinant.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/matrix_inverse.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/matrix_inverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/matrix_multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/matrix_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/matrix_solve.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/matrix_solve.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/minimal_poly_element.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/minimal_poly_element.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/multiplicative_inverse.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/multiplicative_inverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/multiplicative_order.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/multiplicative_order.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/null_space.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/null_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/plu_decompose.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/plu_decompose.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/power.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/row_reduce.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/row_reduce.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/row_space.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/row_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/scalar_multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/scalar_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(2^8, 283, 19)/subtract.pkl` & `galois-0.3.4/tests/fields/data/GF(2^8, 283, 19)/subtract.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(31)/add.pkl` & `galois-0.3.4/tests/fields/data/GF(31)/add.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(31)/additive_inverse.pkl` & `galois-0.3.4/tests/fields/data/GF(31)/additive_inverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(31)/additive_order.pkl` & `galois-0.3.4/tests/fields/data/GF(31)/additive_order.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(31)/characteristic_poly_element.pkl` & `galois-0.3.4/tests/fields/data/GF(31)/characteristic_poly_element.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(31)/characteristic_poly_matrix.pkl` & `galois-0.3.4/tests/fields/data/GF(31)/characteristic_poly_matrix.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(31)/column_space.pkl` & `galois-0.3.4/tests/fields/data/GF(31)/column_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(31)/convolve.pkl` & `galois-0.3.4/tests/fields/data/GF(31)/convolve.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(31)/divide.pkl` & `galois-0.3.4/tests/fields/data/GF(31)/divide.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(31)/field_norm.pkl` & `galois-0.3.4/tests/fields/data/GF(31)/field_norm.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(31)/field_trace.pkl` & `galois-0.3.4/tests/fields/data/GF(31)/field_trace.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(31)/left_null_space.pkl` & `galois-0.3.4/tests/fields/data/GF(31)/left_null_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(31)/log.pkl` & `galois-0.3.4/tests/fields/data/GF(31)/log.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(31)/lu_decompose.pkl` & `galois-0.3.4/tests/fields/data/GF(31)/lu_decompose.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(31)/matrix_determinant.pkl` & `galois-0.3.4/tests/fields/data/GF(31)/matrix_determinant.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(31)/matrix_inverse.pkl` & `galois-0.3.4/tests/fields/data/GF(31)/matrix_inverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(31)/matrix_multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(31)/matrix_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(31)/matrix_solve.pkl` & `galois-0.3.4/tests/fields/data/GF(31)/matrix_solve.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(31)/minimal_poly_element.pkl` & `galois-0.3.4/tests/fields/data/GF(31)/minimal_poly_element.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(31)/multiplicative_inverse.pkl` & `galois-0.3.4/tests/fields/data/GF(31)/multiplicative_inverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(31)/multiplicative_order.pkl` & `galois-0.3.4/tests/fields/data/GF(31)/multiplicative_order.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(31)/multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(31)/multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(31)/null_space.pkl` & `galois-0.3.4/tests/fields/data/GF(31)/null_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(31)/plu_decompose.pkl` & `galois-0.3.4/tests/fields/data/GF(31)/plu_decompose.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(31)/power.pkl` & `galois-0.3.4/tests/fields/data/GF(31)/power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(31)/row_reduce.pkl` & `galois-0.3.4/tests/fields/data/GF(31)/row_reduce.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(31)/row_space.pkl` & `galois-0.3.4/tests/fields/data/GF(31)/row_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(31)/scalar_multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(31)/scalar_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(31)/subtract.pkl` & `galois-0.3.4/tests/fields/data/GF(31)/subtract.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(3191)/add.pkl` & `galois-0.3.4/tests/fields/data/GF(3191)/add.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(3191)/characteristic_poly_matrix.pkl` & `galois-0.3.4/tests/fields/data/GF(3191)/characteristic_poly_matrix.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(3191)/column_space.pkl` & `galois-0.3.4/tests/fields/data/GF(3191)/column_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(3191)/convolve.pkl` & `galois-0.3.4/tests/fields/data/GF(3191)/convolve.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(3191)/divide.pkl` & `galois-0.3.4/tests/fields/data/GF(3191)/divide.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(3191)/left_null_space.pkl` & `galois-0.3.4/tests/fields/data/GF(3191)/left_null_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(3191)/lu_decompose.pkl` & `galois-0.3.4/tests/fields/data/GF(3191)/lu_decompose.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(3191)/matrix_determinant.pkl` & `galois-0.3.4/tests/fields/data/GF(3191)/matrix_determinant.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(3191)/matrix_inverse.pkl` & `galois-0.3.4/tests/fields/data/GF(3191)/matrix_inverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(3191)/matrix_multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(3191)/matrix_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(3191)/matrix_solve.pkl` & `galois-0.3.4/tests/fields/data/GF(3191)/matrix_solve.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(3191)/multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(3191)/multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(3191)/null_space.pkl` & `galois-0.3.4/tests/fields/data/GF(3191)/null_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(3191)/plu_decompose.pkl` & `galois-0.3.4/tests/fields/data/GF(3191)/plu_decompose.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(3191)/power.pkl` & `galois-0.3.4/tests/fields/data/GF(3191)/power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(3191)/row_reduce.pkl` & `galois-0.3.4/tests/fields/data/GF(3191)/row_reduce.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(3191)/row_space.pkl` & `galois-0.3.4/tests/fields/data/GF(3191)/row_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(3191)/scalar_multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(3191)/scalar_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(3191)/subtract.pkl` & `galois-0.3.4/tests/fields/data/GF(3191)/subtract.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(36893488147419103183)/add.pkl` & `galois-0.3.4/tests/fields/data/GF(36893488147419103183)/add.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(36893488147419103183)/additive_inverse.pkl` & `galois-0.3.4/tests/fields/data/GF(36893488147419103183)/additive_inverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(36893488147419103183)/additive_order.pkl` & `galois-0.3.4/tests/fields/data/GF(36893488147419103183)/additive_order.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(36893488147419103183)/characteristic_poly_element.pkl` & `galois-0.3.4/tests/fields/data/GF(36893488147419103183)/characteristic_poly_element.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(36893488147419103183)/characteristic_poly_matrix.pkl` & `galois-0.3.4/tests/fields/data/GF(36893488147419103183)/characteristic_poly_matrix.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(36893488147419103183)/column_space.pkl` & `galois-0.3.4/tests/fields/data/GF(36893488147419103183)/column_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(36893488147419103183)/convolve.pkl` & `galois-0.3.4/tests/fields/data/GF(36893488147419103183)/convolve.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(36893488147419103183)/divide.pkl` & `galois-0.3.4/tests/fields/data/GF(36893488147419103183)/divide.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(36893488147419103183)/field_norm.pkl` & `galois-0.3.4/tests/fields/data/GF(36893488147419103183)/field_norm.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(36893488147419103183)/field_trace.pkl` & `galois-0.3.4/tests/fields/data/GF(36893488147419103183)/field_trace.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(36893488147419103183)/left_null_space.pkl` & `galois-0.3.4/tests/fields/data/GF(36893488147419103183)/left_null_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(36893488147419103183)/log.pkl` & `galois-0.3.4/tests/fields/data/GF(36893488147419103183)/log.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(36893488147419103183)/lu_decompose.pkl` & `galois-0.3.4/tests/fields/data/GF(36893488147419103183)/lu_decompose.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(36893488147419103183)/matrix_determinant.pkl` & `galois-0.3.4/tests/fields/data/GF(36893488147419103183)/matrix_determinant.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(36893488147419103183)/matrix_inverse.pkl` & `galois-0.3.4/tests/fields/data/GF(36893488147419103183)/matrix_inverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(36893488147419103183)/matrix_multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(36893488147419103183)/matrix_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(36893488147419103183)/matrix_solve.pkl` & `galois-0.3.4/tests/fields/data/GF(36893488147419103183)/matrix_solve.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(36893488147419103183)/minimal_poly_element.pkl` & `galois-0.3.4/tests/fields/data/GF(36893488147419103183)/minimal_poly_element.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(36893488147419103183)/multiplicative_inverse.pkl` & `galois-0.3.4/tests/fields/data/GF(36893488147419103183)/multiplicative_inverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(36893488147419103183)/multiplicative_order.pkl` & `galois-0.3.4/tests/fields/data/GF(36893488147419103183)/multiplicative_order.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(36893488147419103183)/multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(36893488147419103183)/multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(36893488147419103183)/null_space.pkl` & `galois-0.3.4/tests/fields/data/GF(36893488147419103183)/null_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(36893488147419103183)/plu_decompose.pkl` & `galois-0.3.4/tests/fields/data/GF(36893488147419103183)/plu_decompose.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(36893488147419103183)/power.pkl` & `galois-0.3.4/tests/fields/data/GF(36893488147419103183)/power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(36893488147419103183)/row_reduce.pkl` & `galois-0.3.4/tests/fields/data/GF(36893488147419103183)/row_reduce.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(36893488147419103183)/row_space.pkl` & `galois-0.3.4/tests/fields/data/GF(36893488147419103183)/row_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(36893488147419103183)/scalar_multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(36893488147419103183)/scalar_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(36893488147419103183)/subtract.pkl` & `galois-0.3.4/tests/fields/data/GF(36893488147419103183)/subtract.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(5)/characteristic_poly_matrix.pkl` & `galois-0.3.4/tests/fields/data/GF(5)/characteristic_poly_matrix.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(5)/column_space.pkl` & `galois-0.3.4/tests/fields/data/GF(5)/column_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(5)/convolve.pkl` & `galois-0.3.4/tests/fields/data/GF(5)/convolve.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(5)/left_null_space.pkl` & `galois-0.3.4/tests/fields/data/GF(5)/left_null_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(5)/lu_decompose.pkl` & `galois-0.3.4/tests/fields/data/GF(5)/lu_decompose.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(5)/matrix_determinant.pkl` & `galois-0.3.4/tests/fields/data/GF(5)/matrix_determinant.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(5)/matrix_inverse.pkl` & `galois-0.3.4/tests/fields/data/GF(5)/matrix_inverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(5)/matrix_multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(5)/matrix_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(5)/matrix_solve.pkl` & `galois-0.3.4/tests/fields/data/GF(5)/matrix_solve.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(5)/null_space.pkl` & `galois-0.3.4/tests/fields/data/GF(5)/null_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(5)/plu_decompose.pkl` & `galois-0.3.4/tests/fields/data/GF(5)/plu_decompose.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(5)/power.pkl` & `galois-0.3.4/tests/fields/data/GF(5)/power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(5)/row_reduce.pkl` & `galois-0.3.4/tests/fields/data/GF(5)/row_reduce.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(5)/row_space.pkl` & `galois-0.3.4/tests/fields/data/GF(5)/row_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(5)/scalar_multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(5)/scalar_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7)/add.pkl` & `galois-0.3.4/tests/fields/data/GF(7)/add.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7)/characteristic_poly_matrix.pkl` & `galois-0.3.4/tests/fields/data/GF(7)/characteristic_poly_matrix.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7)/column_space.pkl` & `galois-0.3.4/tests/fields/data/GF(7)/column_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7)/convolve.pkl` & `galois-0.3.4/tests/fields/data/GF(7)/convolve.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7)/divide.pkl` & `galois-0.3.4/tests/fields/data/GF(7)/divide.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7)/left_null_space.pkl` & `galois-0.3.4/tests/fields/data/GF(7)/left_null_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7)/lu_decompose.pkl` & `galois-0.3.4/tests/fields/data/GF(7)/lu_decompose.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7)/matrix_determinant.pkl` & `galois-0.3.4/tests/fields/data/GF(7)/matrix_determinant.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7)/matrix_inverse.pkl` & `galois-0.3.4/tests/fields/data/GF(7)/matrix_inverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7)/matrix_multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(7)/matrix_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7)/matrix_solve.pkl` & `galois-0.3.4/tests/fields/data/GF(7)/matrix_solve.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7)/multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(7)/multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7)/null_space.pkl` & `galois-0.3.4/tests/fields/data/GF(7)/null_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7)/plu_decompose.pkl` & `galois-0.3.4/tests/fields/data/GF(7)/plu_decompose.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7)/power.pkl` & `galois-0.3.4/tests/fields/data/GF(7)/power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7)/row_reduce.pkl` & `galois-0.3.4/tests/fields/data/GF(7)/row_reduce.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7)/row_space.pkl` & `galois-0.3.4/tests/fields/data/GF(7)/row_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7)/scalar_multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(7)/scalar_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7)/subtract.pkl` & `galois-0.3.4/tests/fields/data/GF(7)/subtract.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3)/add.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3)/add.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3)/additive_inverse.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3)/additive_inverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3)/additive_order.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3)/additive_order.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3)/characteristic_poly_element.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3)/characteristic_poly_element.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3)/characteristic_poly_matrix.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3)/characteristic_poly_matrix.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3)/column_space.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3)/column_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3)/convolve.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3)/convolve.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3)/divide.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3)/divide.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3)/field_norm.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3)/field_norm.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3)/field_trace.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3)/field_trace.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3)/left_null_space.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3)/left_null_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3)/log.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3)/log.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3)/lu_decompose.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3)/lu_decompose.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3)/matrix_determinant.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3)/matrix_determinant.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3)/matrix_inverse.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3)/matrix_inverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3)/matrix_multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3)/matrix_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3)/matrix_solve.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3)/matrix_solve.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3)/minimal_poly_element.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3)/minimal_poly_element.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3)/multiplicative_inverse.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3)/multiplicative_inverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3)/multiplicative_order.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3)/multiplicative_order.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3)/multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3)/multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3)/null_space.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3)/null_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3)/plu_decompose.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3)/plu_decompose.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3)/power.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3)/power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3)/row_reduce.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3)/row_reduce.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3)/row_space.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3)/row_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3)/scalar_multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3)/scalar_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3)/subtract.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3)/subtract.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/add.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/add.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/additive_inverse.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/additive_inverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/additive_order.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/additive_order.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/characteristic_poly_element.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/characteristic_poly_element.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/characteristic_poly_matrix.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/characteristic_poly_matrix.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/column_space.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/column_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/convolve.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/convolve.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/divide.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/divide.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/field_norm.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/field_norm.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/field_trace.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/field_trace.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/left_null_space.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/left_null_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/log.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/log.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/lu_decompose.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/lu_decompose.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/matrix_determinant.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/matrix_determinant.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/matrix_inverse.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/matrix_inverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/matrix_multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/matrix_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/matrix_solve.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/matrix_solve.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/minimal_poly_element.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/minimal_poly_element.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/multiplicative_inverse.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/multiplicative_inverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/multiplicative_order.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/multiplicative_order.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/null_space.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/null_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/plu_decompose.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/plu_decompose.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/power.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/row_reduce.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/row_reduce.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/row_space.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/row_space.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/scalar_multiply.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/scalar_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/data/GF(7^3, 643, 244)/subtract.pkl` & `galois-0.3.4/tests/fields/data/GF(7^3, 643, 244)/subtract.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/test_advanced_arithmetic.py` & `galois-0.3.4/tests/fields/test_advanced_arithmetic.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/test_arithmetic.py` & `galois-0.3.4/tests/fields/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/test_arithmetic_exceptions.py` & `galois-0.3.4/tests/fields/test_arithmetic_exceptions.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/test_arithmetic_methods.py` & `galois-0.3.4/tests/fields/test_arithmetic_methods.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/test_assignment.py` & `galois-0.3.4/tests/fields/test_assignment.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/test_broadcasting.py` & `galois-0.3.4/tests/fields/test_broadcasting.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/test_classes.py` & `galois-0.3.4/tests/fields/test_classes.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/test_constructors.py` & `galois-0.3.4/tests/fields/test_constructors.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/test_conversion.py` & `galois-0.3.4/tests/fields/test_conversion.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/test_factory.py` & `galois-0.3.4/tests/fields/test_factory.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/test_fft.py` & `galois-0.3.4/tests/fields/test_fft.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/test_instantiation.py` & `galois-0.3.4/tests/fields/test_instantiation.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/test_linalg.py` & `galois-0.3.4/tests/fields/test_linalg.py`

 * *Files 2% similar despite different names*

```diff
@@ -365,14 +365,36 @@
         assert np.array_equal(l, l_truth)
         assert np.array_equal(u, u_truth)
         assert type(p) is GF
         assert type(l) is GF
         assert type(u) is GF
 
 
+def test_bug_476():
+    """
+    See https://github.com/mhostetter/galois/issues/476.
+    """
+    GF = galois.GF(2)
+    A = GF(
+        [
+            [1, 0, 0, 0, 0, 1],
+            [1, 1, 1, 1, 0, 1],
+            [1, 0, 0, 0, 0, 0],
+            [0, 1, 0, 0, 0, 0],
+            [0, 0, 1, 0, 0, 0],
+            [0, 0, 0, 1, 0, 0],
+            [0, 0, 0, 0, 1, 0],
+            [0, 0, 0, 0, 0, 1],
+        ]
+    )
+    P, L, U = A.plu_decompose()
+    PLU = P @ L @ U
+    assert np.array_equal(A, PLU)
+
+
 def test_matrix_inverse_exceptions():
     GF = galois.GF(2**8)
     with pytest.raises(np.linalg.LinAlgError):
         A = GF.Random(5)
         np.linalg.inv(A)
     with pytest.raises(np.linalg.LinAlgError):
         A = GF.Random((2, 2, 2))
```

### Comparing `galois-0.3.3/tests/fields/test_methods.py` & `galois-0.3.4/tests/fields/test_methods.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/test_ntt.py` & `galois-0.3.4/tests/fields/test_ntt.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/test_numpy_functions.py` & `galois-0.3.4/tests/fields/test_numpy_functions.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/test_numpy_ufuncs.py` & `galois-0.3.4/tests/fields/test_numpy_ufuncs.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/test_properties.py` & `galois-0.3.4/tests/fields/test_properties.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/test_sqrt.py` & `galois-0.3.4/tests/fields/test_sqrt.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/fields/test_squares.py` & `galois-0.3.4/tests/fields/test_squares.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/conftest.py` & `galois-0.3.4/tests/polys/conftest.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(109987^4)/add.pkl` & `galois-0.3.4/tests/polys/data/GF(109987^4)/add.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(109987^4)/crt.pkl` & `galois-0.3.4/tests/polys/data/GF(109987^4)/crt.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(109987^4)/derivative.pkl` & `galois-0.3.4/tests/polys/data/GF(109987^4)/derivative.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(109987^4)/divmod.pkl` & `galois-0.3.4/tests/polys/data/GF(109987^4)/divmod.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(109987^4)/egcd.pkl` & `galois-0.3.4/tests/polys/data/GF(109987^4)/egcd.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(109987^4)/evaluate.pkl` & `galois-0.3.4/tests/polys/data/GF(109987^4)/evaluate.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(109987^4)/evaluate_matrix.pkl` & `galois-0.3.4/tests/polys/data/GF(109987^4)/evaluate_matrix.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(109987^4)/evaluate_poly.pkl` & `galois-0.3.4/tests/polys/data/GF(109987^4)/evaluate_poly.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(109987^4)/is_monic.pkl` & `galois-0.3.4/tests/polys/data/GF(109987^4)/is_monic.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(109987^4)/lagrange_poly.pkl` & `galois-0.3.4/tests/polys/data/GF(109987^4)/lagrange_poly.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(109987^4)/lcm.pkl` & `galois-0.3.4/tests/polys/data/GF(109987^4)/lcm.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(109987^4)/modular_power.pkl` & `galois-0.3.4/tests/polys/data/GF(109987^4)/modular_power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(109987^4)/multiply.pkl` & `galois-0.3.4/tests/polys/data/GF(109987^4)/multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(109987^4)/power.pkl` & `galois-0.3.4/tests/polys/data/GF(109987^4)/power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(109987^4)/prod.pkl` & `galois-0.3.4/tests/polys/data/GF(109987^4)/prod.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(109987^4)/reverse.pkl` & `galois-0.3.4/tests/polys/data/GF(109987^4)/reverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(109987^4)/roots.pkl` & `galois-0.3.4/tests/polys/data/GF(109987^4)/roots.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(109987^4)/scalar_multiply.pkl` & `galois-0.3.4/tests/polys/data/GF(109987^4)/scalar_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(109987^4)/subtract.pkl` & `galois-0.3.4/tests/polys/data/GF(109987^4)/subtract.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2)/add.pkl` & `galois-0.3.4/tests/polys/data/GF(2)/add.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2)/crt.pkl` & `galois-0.3.4/tests/polys/data/GF(2)/crt.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2)/divmod.pkl` & `galois-0.3.4/tests/polys/data/GF(2)/divmod.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2)/egcd.pkl` & `galois-0.3.4/tests/polys/data/GF(2)/egcd.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2)/evaluate.pkl` & `galois-0.3.4/tests/polys/data/GF(2)/evaluate.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2)/evaluate_matrix.pkl` & `galois-0.3.4/tests/polys/data/GF(2)/evaluate_matrix.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2)/evaluate_poly.pkl` & `galois-0.3.4/tests/polys/data/GF(2)/evaluate_poly.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2)/lcm.pkl` & `galois-0.3.4/tests/polys/data/GF(2)/lcm.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2)/modular_power.pkl` & `galois-0.3.4/tests/polys/data/GF(2)/modular_power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2)/multiply.pkl` & `galois-0.3.4/tests/polys/data/GF(2)/multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2)/prod.pkl` & `galois-0.3.4/tests/polys/data/GF(2)/prod.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2)/reverse.pkl` & `galois-0.3.4/tests/polys/data/GF(2)/reverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2)/roots.pkl` & `galois-0.3.4/tests/polys/data/GF(2)/roots.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2)/scalar_multiply.pkl` & `galois-0.3.4/tests/polys/data/GF(2)/scalar_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2)/subtract.pkl` & `galois-0.3.4/tests/polys/data/GF(2)/subtract.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2147483647)/add.pkl` & `galois-0.3.4/tests/polys/data/GF(2147483647)/add.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2147483647)/crt.pkl` & `galois-0.3.4/tests/polys/data/GF(2147483647)/crt.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2147483647)/derivative.pkl` & `galois-0.3.4/tests/polys/data/GF(2147483647)/derivative.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2147483647)/divmod.pkl` & `galois-0.3.4/tests/polys/data/GF(2147483647)/divmod.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2147483647)/egcd.pkl` & `galois-0.3.4/tests/polys/data/GF(2147483647)/egcd.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2147483647)/evaluate.pkl` & `galois-0.3.4/tests/polys/data/GF(2147483647)/evaluate.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2147483647)/evaluate_matrix.pkl` & `galois-0.3.4/tests/polys/data/GF(2147483647)/evaluate_matrix.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2147483647)/evaluate_poly.pkl` & `galois-0.3.4/tests/polys/data/GF(2147483647)/evaluate_poly.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2147483647)/lagrange_poly.pkl` & `galois-0.3.4/tests/polys/data/GF(2147483647)/lagrange_poly.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2147483647)/lcm.pkl` & `galois-0.3.4/tests/polys/data/GF(2147483647)/lcm.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2147483647)/modular_power.pkl` & `galois-0.3.4/tests/polys/data/GF(2147483647)/modular_power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2147483647)/multiply.pkl` & `galois-0.3.4/tests/polys/data/GF(2147483647)/multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2147483647)/power.pkl` & `galois-0.3.4/tests/polys/data/GF(2147483647)/power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2147483647)/prod.pkl` & `galois-0.3.4/tests/polys/data/GF(2147483647)/prod.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2147483647)/reverse.pkl` & `galois-0.3.4/tests/polys/data/GF(2147483647)/reverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2147483647)/roots.pkl` & `galois-0.3.4/tests/polys/data/GF(2147483647)/roots.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2147483647)/scalar_multiply.pkl` & `galois-0.3.4/tests/polys/data/GF(2147483647)/scalar_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2147483647)/subtract.pkl` & `galois-0.3.4/tests/polys/data/GF(2147483647)/subtract.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^100)/add.pkl` & `galois-0.3.4/tests/polys/data/GF(2^100)/add.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^100)/crt.pkl` & `galois-0.3.4/tests/polys/data/GF(2^100)/crt.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^100)/derivative.pkl` & `galois-0.3.4/tests/polys/data/GF(2^100)/derivative.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^100)/divmod.pkl` & `galois-0.3.4/tests/polys/data/GF(2^100)/divmod.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^100)/egcd.pkl` & `galois-0.3.4/tests/polys/data/GF(2^100)/egcd.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^100)/evaluate.pkl` & `galois-0.3.4/tests/polys/data/GF(2^100)/evaluate.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^100)/evaluate_matrix.pkl` & `galois-0.3.4/tests/polys/data/GF(2^100)/evaluate_matrix.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^100)/evaluate_poly.pkl` & `galois-0.3.4/tests/polys/data/GF(2^100)/evaluate_poly.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^100)/is_monic.pkl` & `galois-0.3.4/tests/polys/data/GF(2^100)/is_monic.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^100)/lagrange_poly.pkl` & `galois-0.3.4/tests/polys/data/GF(2^100)/lagrange_poly.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^100)/lcm.pkl` & `galois-0.3.4/tests/polys/data/GF(2^100)/lcm.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^100)/modular_power.pkl` & `galois-0.3.4/tests/polys/data/GF(2^100)/modular_power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^100)/multiply.pkl` & `galois-0.3.4/tests/polys/data/GF(2^100)/multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^100)/power.pkl` & `galois-0.3.4/tests/polys/data/GF(2^100)/power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^100)/prod.pkl` & `galois-0.3.4/tests/polys/data/GF(2^100)/prod.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^100)/reverse.pkl` & `galois-0.3.4/tests/polys/data/GF(2^100)/reverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^100)/roots.pkl` & `galois-0.3.4/tests/polys/data/GF(2^100)/roots.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^100)/scalar_multiply.pkl` & `galois-0.3.4/tests/polys/data/GF(2^100)/scalar_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^100)/subtract.pkl` & `galois-0.3.4/tests/polys/data/GF(2^100)/subtract.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^2)/add.pkl` & `galois-0.3.4/tests/polys/data/GF(2^2)/add.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^2)/crt.pkl` & `galois-0.3.4/tests/polys/data/GF(2^2)/crt.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^2)/derivative.pkl` & `galois-0.3.4/tests/polys/data/GF(2^2)/derivative.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^2)/divmod.pkl` & `galois-0.3.4/tests/polys/data/GF(2^2)/divmod.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^2)/egcd.pkl` & `galois-0.3.4/tests/polys/data/GF(2^2)/egcd.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^2)/evaluate.pkl` & `galois-0.3.4/tests/polys/data/GF(2^2)/evaluate.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^2)/evaluate_matrix.pkl` & `galois-0.3.4/tests/polys/data/GF(2^2)/evaluate_matrix.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^2)/evaluate_poly.pkl` & `galois-0.3.4/tests/polys/data/GF(2^2)/evaluate_poly.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^2)/lagrange_poly.pkl` & `galois-0.3.4/tests/polys/data/GF(2^2)/lagrange_poly.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^2)/lcm.pkl` & `galois-0.3.4/tests/polys/data/GF(2^2)/lcm.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^2)/modular_power.pkl` & `galois-0.3.4/tests/polys/data/GF(2^2)/modular_power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^2)/multiply.pkl` & `galois-0.3.4/tests/polys/data/GF(2^2)/multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^2)/prod.pkl` & `galois-0.3.4/tests/polys/data/GF(2^2)/prod.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^2)/reverse.pkl` & `galois-0.3.4/tests/polys/data/GF(2^2)/reverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^2)/roots.pkl` & `galois-0.3.4/tests/polys/data/GF(2^2)/roots.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^2)/scalar_multiply.pkl` & `galois-0.3.4/tests/polys/data/GF(2^2)/scalar_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^2)/subtract.pkl` & `galois-0.3.4/tests/polys/data/GF(2^2)/subtract.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^3)/add.pkl` & `galois-0.3.4/tests/polys/data/GF(2^3)/add.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^3)/crt.pkl` & `galois-0.3.4/tests/polys/data/GF(2^3)/crt.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^3)/derivative.pkl` & `galois-0.3.4/tests/polys/data/GF(2^3)/derivative.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^3)/divmod.pkl` & `galois-0.3.4/tests/polys/data/GF(2^3)/divmod.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^3)/egcd.pkl` & `galois-0.3.4/tests/polys/data/GF(2^3)/egcd.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^3)/evaluate.pkl` & `galois-0.3.4/tests/polys/data/GF(2^3)/evaluate.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^3)/evaluate_matrix.pkl` & `galois-0.3.4/tests/polys/data/GF(2^3)/evaluate_matrix.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^3)/evaluate_poly.pkl` & `galois-0.3.4/tests/polys/data/GF(2^3)/evaluate_poly.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^3)/lagrange_poly.pkl` & `galois-0.3.4/tests/polys/data/GF(2^3)/lagrange_poly.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^3)/lcm.pkl` & `galois-0.3.4/tests/polys/data/GF(2^3)/lcm.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^3)/modular_power.pkl` & `galois-0.3.4/tests/polys/data/GF(2^3)/modular_power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^3)/multiply.pkl` & `galois-0.3.4/tests/polys/data/GF(2^3)/multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^3)/prod.pkl` & `galois-0.3.4/tests/polys/data/GF(2^3)/prod.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^3)/reverse.pkl` & `galois-0.3.4/tests/polys/data/GF(2^3)/reverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^3)/roots.pkl` & `galois-0.3.4/tests/polys/data/GF(2^3)/roots.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^3)/scalar_multiply.pkl` & `galois-0.3.4/tests/polys/data/GF(2^3)/scalar_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^3)/subtract.pkl` & `galois-0.3.4/tests/polys/data/GF(2^3)/subtract.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^32)/add.pkl` & `galois-0.3.4/tests/polys/data/GF(2^32)/add.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^32)/crt.pkl` & `galois-0.3.4/tests/polys/data/GF(2^32)/crt.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^32)/derivative.pkl` & `galois-0.3.4/tests/polys/data/GF(2^32)/derivative.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^32)/divmod.pkl` & `galois-0.3.4/tests/polys/data/GF(2^32)/divmod.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^32)/egcd.pkl` & `galois-0.3.4/tests/polys/data/GF(2^32)/egcd.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^32)/evaluate.pkl` & `galois-0.3.4/tests/polys/data/GF(2^32)/evaluate.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^32)/evaluate_matrix.pkl` & `galois-0.3.4/tests/polys/data/GF(2^32)/evaluate_matrix.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^32)/evaluate_poly.pkl` & `galois-0.3.4/tests/polys/data/GF(2^32)/evaluate_poly.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^32)/lagrange_poly.pkl` & `galois-0.3.4/tests/polys/data/GF(2^32)/lagrange_poly.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^32)/lcm.pkl` & `galois-0.3.4/tests/polys/data/GF(2^32)/lcm.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^32)/modular_power.pkl` & `galois-0.3.4/tests/polys/data/GF(2^32)/modular_power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^32)/multiply.pkl` & `galois-0.3.4/tests/polys/data/GF(2^32)/multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^32)/power.pkl` & `galois-0.3.4/tests/polys/data/GF(2^32)/power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^32)/prod.pkl` & `galois-0.3.4/tests/polys/data/GF(2^32)/prod.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^32)/reverse.pkl` & `galois-0.3.4/tests/polys/data/GF(2^32)/reverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^32)/roots.pkl` & `galois-0.3.4/tests/polys/data/GF(2^32)/roots.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^32)/scalar_multiply.pkl` & `galois-0.3.4/tests/polys/data/GF(2^32)/scalar_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^32)/subtract.pkl` & `galois-0.3.4/tests/polys/data/GF(2^32)/subtract.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^8)/add.pkl` & `galois-0.3.4/tests/polys/data/GF(2^8)/add.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^8)/crt.pkl` & `galois-0.3.4/tests/polys/data/GF(2^8)/crt.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^8)/derivative.pkl` & `galois-0.3.4/tests/polys/data/GF(2^8)/derivative.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^8)/divmod.pkl` & `galois-0.3.4/tests/polys/data/GF(2^8)/divmod.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^8)/egcd.pkl` & `galois-0.3.4/tests/polys/data/GF(2^8)/egcd.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^8)/evaluate.pkl` & `galois-0.3.4/tests/polys/data/GF(2^8)/evaluate.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^8)/evaluate_matrix.pkl` & `galois-0.3.4/tests/polys/data/GF(2^8)/evaluate_matrix.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^8)/evaluate_poly.pkl` & `galois-0.3.4/tests/polys/data/GF(2^8)/evaluate_poly.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^8)/lagrange_poly.pkl` & `galois-0.3.4/tests/polys/data/GF(2^8)/lagrange_poly.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^8)/lcm.pkl` & `galois-0.3.4/tests/polys/data/GF(2^8)/lcm.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^8)/modular_power.pkl` & `galois-0.3.4/tests/polys/data/GF(2^8)/modular_power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^8)/multiply.pkl` & `galois-0.3.4/tests/polys/data/GF(2^8)/multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^8)/power.pkl` & `galois-0.3.4/tests/polys/data/GF(2^8)/power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^8)/prod.pkl` & `galois-0.3.4/tests/polys/data/GF(2^8)/prod.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^8)/reverse.pkl` & `galois-0.3.4/tests/polys/data/GF(2^8)/reverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^8)/roots.pkl` & `galois-0.3.4/tests/polys/data/GF(2^8)/roots.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^8)/scalar_multiply.pkl` & `galois-0.3.4/tests/polys/data/GF(2^8)/scalar_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^8)/subtract.pkl` & `galois-0.3.4/tests/polys/data/GF(2^8)/subtract.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/add.pkl` & `galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/add.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/crt.pkl` & `galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/crt.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/derivative.pkl` & `galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/derivative.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/divmod.pkl` & `galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/divmod.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/egcd.pkl` & `galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/egcd.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/evaluate.pkl` & `galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/evaluate.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/evaluate_matrix.pkl` & `galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/evaluate_matrix.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/evaluate_poly.pkl` & `galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/evaluate_poly.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/lagrange_poly.pkl` & `galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/lagrange_poly.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/lcm.pkl` & `galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/lcm.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/modular_power.pkl` & `galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/modular_power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/multiply.pkl` & `galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/prod.pkl` & `galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/prod.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/reverse.pkl` & `galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/reverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/roots.pkl` & `galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/roots.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/scalar_multiply.pkl` & `galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/scalar_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(2^8, 283, 19)/subtract.pkl` & `galois-0.3.4/tests/polys/data/GF(2^8, 283, 19)/subtract.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(31)/add.pkl` & `galois-0.3.4/tests/polys/data/GF(31)/add.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(31)/crt.pkl` & `galois-0.3.4/tests/polys/data/GF(31)/crt.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(31)/divmod.pkl` & `galois-0.3.4/tests/polys/data/GF(31)/divmod.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(31)/egcd.pkl` & `galois-0.3.4/tests/polys/data/GF(31)/egcd.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(31)/evaluate.pkl` & `galois-0.3.4/tests/polys/data/GF(31)/evaluate.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(31)/evaluate_matrix.pkl` & `galois-0.3.4/tests/polys/data/GF(31)/evaluate_matrix.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(31)/evaluate_poly.pkl` & `galois-0.3.4/tests/polys/data/GF(31)/evaluate_poly.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(31)/lagrange_poly.pkl` & `galois-0.3.4/tests/polys/data/GF(31)/lagrange_poly.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(31)/lcm.pkl` & `galois-0.3.4/tests/polys/data/GF(31)/lcm.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(31)/modular_power.pkl` & `galois-0.3.4/tests/polys/data/GF(31)/modular_power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(31)/multiply.pkl` & `galois-0.3.4/tests/polys/data/GF(31)/multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(31)/power.pkl` & `galois-0.3.4/tests/polys/data/GF(31)/power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(31)/prod.pkl` & `galois-0.3.4/tests/polys/data/GF(31)/prod.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(31)/reverse.pkl` & `galois-0.3.4/tests/polys/data/GF(31)/reverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(31)/roots.pkl` & `galois-0.3.4/tests/polys/data/GF(31)/roots.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(31)/scalar_multiply.pkl` & `galois-0.3.4/tests/polys/data/GF(31)/scalar_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(31)/subtract.pkl` & `galois-0.3.4/tests/polys/data/GF(31)/subtract.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(3191)/add.pkl` & `galois-0.3.4/tests/polys/data/GF(3191)/add.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(3191)/crt.pkl` & `galois-0.3.4/tests/polys/data/GF(3191)/crt.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(3191)/derivative.pkl` & `galois-0.3.4/tests/polys/data/GF(3191)/derivative.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(3191)/divmod.pkl` & `galois-0.3.4/tests/polys/data/GF(3191)/divmod.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(3191)/egcd.pkl` & `galois-0.3.4/tests/polys/data/GF(3191)/egcd.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(3191)/evaluate.pkl` & `galois-0.3.4/tests/polys/data/GF(3191)/evaluate.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(3191)/evaluate_matrix.pkl` & `galois-0.3.4/tests/polys/data/GF(3191)/evaluate_matrix.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(3191)/evaluate_poly.pkl` & `galois-0.3.4/tests/polys/data/GF(3191)/evaluate_poly.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(3191)/lagrange_poly.pkl` & `galois-0.3.4/tests/polys/data/GF(3191)/lagrange_poly.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(3191)/lcm.pkl` & `galois-0.3.4/tests/polys/data/GF(3191)/lcm.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(3191)/modular_power.pkl` & `galois-0.3.4/tests/polys/data/GF(3191)/modular_power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(3191)/multiply.pkl` & `galois-0.3.4/tests/polys/data/GF(3191)/multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(3191)/power.pkl` & `galois-0.3.4/tests/polys/data/GF(3191)/power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(3191)/prod.pkl` & `galois-0.3.4/tests/polys/data/GF(3191)/prod.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(3191)/reverse.pkl` & `galois-0.3.4/tests/polys/data/GF(3191)/reverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(3191)/roots.pkl` & `galois-0.3.4/tests/polys/data/GF(3191)/roots.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(3191)/scalar_multiply.pkl` & `galois-0.3.4/tests/polys/data/GF(3191)/scalar_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(3191)/subtract.pkl` & `galois-0.3.4/tests/polys/data/GF(3191)/subtract.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(36893488147419103183)/add.pkl` & `galois-0.3.4/tests/polys/data/GF(36893488147419103183)/add.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(36893488147419103183)/crt.pkl` & `galois-0.3.4/tests/polys/data/GF(36893488147419103183)/crt.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(36893488147419103183)/derivative.pkl` & `galois-0.3.4/tests/polys/data/GF(36893488147419103183)/derivative.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(36893488147419103183)/divmod.pkl` & `galois-0.3.4/tests/polys/data/GF(36893488147419103183)/divmod.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(36893488147419103183)/egcd.pkl` & `galois-0.3.4/tests/polys/data/GF(36893488147419103183)/egcd.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(36893488147419103183)/evaluate.pkl` & `galois-0.3.4/tests/polys/data/GF(36893488147419103183)/evaluate.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(36893488147419103183)/evaluate_matrix.pkl` & `galois-0.3.4/tests/polys/data/GF(36893488147419103183)/evaluate_matrix.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(36893488147419103183)/evaluate_poly.pkl` & `galois-0.3.4/tests/polys/data/GF(36893488147419103183)/evaluate_poly.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(36893488147419103183)/is_monic.pkl` & `galois-0.3.4/tests/polys/data/GF(36893488147419103183)/is_monic.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(36893488147419103183)/lagrange_poly.pkl` & `galois-0.3.4/tests/polys/data/GF(36893488147419103183)/lagrange_poly.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(36893488147419103183)/lcm.pkl` & `galois-0.3.4/tests/polys/data/GF(36893488147419103183)/lcm.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(36893488147419103183)/modular_power.pkl` & `galois-0.3.4/tests/polys/data/GF(36893488147419103183)/modular_power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(36893488147419103183)/multiply.pkl` & `galois-0.3.4/tests/polys/data/GF(36893488147419103183)/multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(36893488147419103183)/power.pkl` & `galois-0.3.4/tests/polys/data/GF(36893488147419103183)/power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(36893488147419103183)/prod.pkl` & `galois-0.3.4/tests/polys/data/GF(36893488147419103183)/prod.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(36893488147419103183)/reverse.pkl` & `galois-0.3.4/tests/polys/data/GF(36893488147419103183)/reverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(36893488147419103183)/roots.pkl` & `galois-0.3.4/tests/polys/data/GF(36893488147419103183)/roots.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(36893488147419103183)/scalar_multiply.pkl` & `galois-0.3.4/tests/polys/data/GF(36893488147419103183)/scalar_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(36893488147419103183)/subtract.pkl` & `galois-0.3.4/tests/polys/data/GF(36893488147419103183)/subtract.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(5)/add.pkl` & `galois-0.3.4/tests/polys/data/GF(5)/add.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(5)/crt.pkl` & `galois-0.3.4/tests/polys/data/GF(5)/crt.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(5)/divmod.pkl` & `galois-0.3.4/tests/polys/data/GF(5)/divmod.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(5)/egcd.pkl` & `galois-0.3.4/tests/polys/data/GF(5)/egcd.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(5)/evaluate.pkl` & `galois-0.3.4/tests/polys/data/GF(5)/evaluate.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(5)/evaluate_matrix.pkl` & `galois-0.3.4/tests/polys/data/GF(5)/evaluate_matrix.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(5)/evaluate_poly.pkl` & `galois-0.3.4/tests/polys/data/GF(5)/evaluate_poly.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(5)/lagrange_poly.pkl` & `galois-0.3.4/tests/polys/data/GF(5)/lagrange_poly.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(5)/lcm.pkl` & `galois-0.3.4/tests/polys/data/GF(5)/lcm.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(5)/modular_power.pkl` & `galois-0.3.4/tests/polys/data/GF(5)/modular_power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(5)/multiply.pkl` & `galois-0.3.4/tests/polys/data/GF(5)/multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(5)/power.pkl` & `galois-0.3.4/tests/polys/data/GF(5)/power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(5)/prod.pkl` & `galois-0.3.4/tests/polys/data/GF(5)/prod.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(5)/reverse.pkl` & `galois-0.3.4/tests/polys/data/GF(5)/reverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(5)/roots.pkl` & `galois-0.3.4/tests/polys/data/GF(5)/roots.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(5)/scalar_multiply.pkl` & `galois-0.3.4/tests/polys/data/GF(5)/scalar_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(5)/subtract.pkl` & `galois-0.3.4/tests/polys/data/GF(5)/subtract.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7)/add.pkl` & `galois-0.3.4/tests/polys/data/GF(7)/add.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7)/crt.pkl` & `galois-0.3.4/tests/polys/data/GF(7)/crt.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7)/divmod.pkl` & `galois-0.3.4/tests/polys/data/GF(7)/divmod.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7)/egcd.pkl` & `galois-0.3.4/tests/polys/data/GF(7)/egcd.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7)/evaluate.pkl` & `galois-0.3.4/tests/polys/data/GF(7)/evaluate.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7)/evaluate_matrix.pkl` & `galois-0.3.4/tests/polys/data/GF(7)/evaluate_matrix.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7)/evaluate_poly.pkl` & `galois-0.3.4/tests/polys/data/GF(7)/evaluate_poly.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7)/lagrange_poly.pkl` & `galois-0.3.4/tests/polys/data/GF(7)/lagrange_poly.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7)/lcm.pkl` & `galois-0.3.4/tests/polys/data/GF(7)/lcm.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7)/modular_power.pkl` & `galois-0.3.4/tests/polys/data/GF(7)/modular_power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7)/multiply.pkl` & `galois-0.3.4/tests/polys/data/GF(7)/multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7)/prod.pkl` & `galois-0.3.4/tests/polys/data/GF(7)/prod.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7)/reverse.pkl` & `galois-0.3.4/tests/polys/data/GF(7)/reverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7)/roots.pkl` & `galois-0.3.4/tests/polys/data/GF(7)/roots.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7)/scalar_multiply.pkl` & `galois-0.3.4/tests/polys/data/GF(7)/scalar_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7)/subtract.pkl` & `galois-0.3.4/tests/polys/data/GF(7)/subtract.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7^3)/add.pkl` & `galois-0.3.4/tests/polys/data/GF(7^3)/add.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7^3)/crt.pkl` & `galois-0.3.4/tests/polys/data/GF(7^3)/crt.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7^3)/derivative.pkl` & `galois-0.3.4/tests/polys/data/GF(7^3)/derivative.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7^3)/divmod.pkl` & `galois-0.3.4/tests/polys/data/GF(7^3)/divmod.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7^3)/egcd.pkl` & `galois-0.3.4/tests/polys/data/GF(7^3)/egcd.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7^3)/evaluate.pkl` & `galois-0.3.4/tests/polys/data/GF(7^3)/evaluate.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7^3)/evaluate_matrix.pkl` & `galois-0.3.4/tests/polys/data/GF(7^3)/evaluate_matrix.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7^3)/evaluate_poly.pkl` & `galois-0.3.4/tests/polys/data/GF(7^3)/evaluate_poly.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7^3)/lagrange_poly.pkl` & `galois-0.3.4/tests/polys/data/GF(7^3)/lagrange_poly.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7^3)/lcm.pkl` & `galois-0.3.4/tests/polys/data/GF(7^3)/lcm.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7^3)/modular_power.pkl` & `galois-0.3.4/tests/polys/data/GF(7^3)/modular_power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7^3)/multiply.pkl` & `galois-0.3.4/tests/polys/data/GF(7^3)/multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7^3)/prod.pkl` & `galois-0.3.4/tests/polys/data/GF(7^3)/prod.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7^3)/reverse.pkl` & `galois-0.3.4/tests/polys/data/GF(7^3)/reverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7^3)/roots.pkl` & `galois-0.3.4/tests/polys/data/GF(7^3)/roots.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7^3)/scalar_multiply.pkl` & `galois-0.3.4/tests/polys/data/GF(7^3)/scalar_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7^3)/subtract.pkl` & `galois-0.3.4/tests/polys/data/GF(7^3)/subtract.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/add.pkl` & `galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/add.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/crt.pkl` & `galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/crt.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/derivative.pkl` & `galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/derivative.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/divmod.pkl` & `galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/divmod.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/egcd.pkl` & `galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/egcd.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/evaluate.pkl` & `galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/evaluate.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/evaluate_matrix.pkl` & `galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/evaluate_matrix.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/evaluate_poly.pkl` & `galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/evaluate_poly.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/lagrange_poly.pkl` & `galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/lagrange_poly.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/lcm.pkl` & `galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/lcm.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/modular_power.pkl` & `galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/modular_power.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/multiply.pkl` & `galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/prod.pkl` & `galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/prod.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/reverse.pkl` & `galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/reverse.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/roots.pkl` & `galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/roots.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/scalar_multiply.pkl` & `galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/scalar_multiply.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/data/GF(7^3, 643, 244)/subtract.pkl` & `galois-0.3.4/tests/polys/data/GF(7^3, 643, 244)/subtract.pkl`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/luts/irreducible_polys.py` & `galois-0.3.4/tests/polys/luts/irreducible_polys.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/luts/irreducible_polys_2.py` & `galois-0.3.4/tests/polys/luts/irreducible_polys_2.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/luts/irreducible_polys_25.py` & `galois-0.3.4/tests/polys/luts/irreducible_polys_25.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/luts/irreducible_polys_3.py` & `galois-0.3.4/tests/polys/luts/irreducible_polys_3.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/luts/irreducible_polys_4.py` & `galois-0.3.4/tests/polys/luts/irreducible_polys_4.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/luts/irreducible_polys_5.py` & `galois-0.3.4/tests/polys/luts/irreducible_polys_5.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/luts/irreducible_polys_9.py` & `galois-0.3.4/tests/polys/luts/irreducible_polys_9.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/luts/irreducible_polys_min.py` & `galois-0.3.4/tests/polys/luts/irreducible_polys_min.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/luts/poly_factors.py` & `galois-0.3.4/tests/polys/luts/poly_factors.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/luts/primitive_elements.py` & `galois-0.3.4/tests/polys/luts/primitive_elements.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/luts/primitive_elements_2.py` & `galois-0.3.4/tests/polys/luts/primitive_elements_2.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/luts/primitive_elements_3.py` & `galois-0.3.4/tests/polys/luts/primitive_elements_3.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/luts/primitive_elements_5.py` & `galois-0.3.4/tests/polys/luts/primitive_elements_5.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/luts/primitive_polys.py` & `galois-0.3.4/tests/polys/luts/primitive_polys.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/luts/primitive_polys_2.py` & `galois-0.3.4/tests/polys/luts/primitive_polys_2.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/luts/primitive_polys_25.py` & `galois-0.3.4/tests/polys/luts/primitive_polys_25.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/luts/primitive_polys_3.py` & `galois-0.3.4/tests/polys/luts/primitive_polys_3.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/luts/primitive_polys_4.py` & `galois-0.3.4/tests/polys/luts/primitive_polys_4.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/luts/primitive_polys_5.py` & `galois-0.3.4/tests/polys/luts/primitive_polys_5.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/luts/primitive_polys_9.py` & `galois-0.3.4/tests/polys/luts/primitive_polys_9.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/test_arithmetic.py` & `galois-0.3.4/tests/polys/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/test_arithmetic_exceptions.py` & `galois-0.3.4/tests/polys/test_arithmetic_exceptions.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/test_arithmetic_functions.py` & `galois-0.3.4/tests/polys/test_arithmetic_functions.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/test_arithmetic_implementations.py` & `galois-0.3.4/tests/polys/test_arithmetic_implementations.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/test_arithmetic_methods.py` & `galois-0.3.4/tests/polys/test_arithmetic_methods.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/test_constructors.py` & `galois-0.3.4/tests/polys/test_constructors.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/test_conversions.py` & `galois-0.3.4/tests/polys/test_conversions.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/test_conway_polys.py` & `galois-0.3.4/tests/polys/test_conway_polys.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/test_factors.py` & `galois-0.3.4/tests/polys/test_factors.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/test_instantiation.py` & `galois-0.3.4/tests/polys/test_instantiation.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/test_irreducible_polys.py` & `galois-0.3.4/tests/polys/test_irreducible_polys.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/test_lagrange_poly.py` & `galois-0.3.4/tests/polys/test_lagrange_poly.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/test_non_poly_arithmetic.py` & `galois-0.3.4/tests/polys/test_non_poly_arithmetic.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/test_operations.py` & `galois-0.3.4/tests/polys/test_operations.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/test_poly_tests.py` & `galois-0.3.4/tests/polys/test_poly_tests.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/test_primitive_elements.py` & `galois-0.3.4/tests/polys/test_primitive_elements.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/polys/test_primitive_polys.py` & `galois-0.3.4/tests/polys/test_primitive_polys.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/test_berlekamp_massey.py` & `galois-0.3.4/tests/test_berlekamp_massey.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/test_factor.py` & `galois-0.3.4/tests/test_factor.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/test_fibonacci_lfsr.py` & `galois-0.3.4/tests/test_fibonacci_lfsr.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/test_galois_lfsr.py` & `galois-0.3.4/tests/test_galois_lfsr.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/test_math.py` & `galois-0.3.4/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/test_modular.py` & `galois-0.3.4/tests/test_modular.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/test_number_theory.py` & `galois-0.3.4/tests/test_number_theory.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/test_options.py` & `galois-0.3.4/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `galois-0.3.3/tests/test_primes.py` & `galois-0.3.4/tests/test_primes.py`

 * *Files identical despite different names*

