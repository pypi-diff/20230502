# Comparing `tmp/json-schema-for-humans-0.9.0.tar.gz` & `tmp/json-schema-for-humans-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/json-schema-for-humans-0.9.0.tar", last modified: Fri May 15 19:35:57 2020, max compression
+gzip compressed data, was "dist/json-schema-for-humans-0.9.1.tar", last modified: Sat May 16 17:08:58 2020, max compression
```

## Comparing `json-schema-for-humans-0.9.0.tar` & `json-schema-for-humans-0.9.1.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-15 19:35:57.000000 json-schema-for-humans-0.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-15 19:35:57.000000 json-schema-for-humans-0.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-15 19:35:57.000000 json-schema-for-humans-0.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)      469 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (116)      471 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/.github/workflows/pythonpackage.yml
--rw-r--r--   0 runner    (1001) docker     (116)      319 2020-05-15 19:35:56.000000 json-schema-for-humans-0.9.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (116)      563 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     4956 2020-05-15 19:35:57.000000 json-schema-for-humans-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3372 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-15 19:35:57.000000 json-schema-for-humans-0.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (116)       72 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/docs/Gemfile
--rw-r--r--   0 runner    (1001) docker     (116)       28 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/docs/_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-15 19:35:57.000000 json-schema-for-humans-0.9.0/docs/_data/
--rw-r--r--   0 runner    (1001) docker     (116)     1487 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/docs/_data/examples.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-15 19:35:57.000000 json-schema-for-humans-0.9.0/docs/_includes/
--rw-r--r--   0 runner    (1001) docker     (116)     3372 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/docs/_includes/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-15 19:35:57.000000 json-schema-for-humans-0.9.0/docs/_includes/examples/
--rw-r--r--   0 runner    (1001) docker     (116)      812 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/docs/_includes/examples/array.json
--rw-r--r--   0 runner    (1001) docker     (116)      516 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/docs/_includes/examples/array_advanced.json
--rw-r--r--   0 runner    (1001) docker     (116)      587 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/docs/_includes/examples/basic.json
--rw-r--r--   0 runner    (1001) docker     (116)      285 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/docs/_includes/examples/combining_not.json
--rw-r--r--   0 runner    (1001) docker     (116)      571 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/docs/_includes/examples/combining_oneOf.json
--rw-r--r--   0 runner    (1001) docker     (116)      439 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/docs/_includes/examples/deprecated.json
--rw-r--r--   0 runner    (1001) docker     (116)      485 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/docs/_includes/examples/geo.json
--rw-r--r--   0 runner    (1001) docker     (116)      684 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/docs/_includes/examples/multiple_types.json
--rw-r--r--   0 runner    (1001) docker     (116)      943 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/docs/_includes/examples/pattern_properties.json
--rw-r--r--   0 runner    (1001) docker     (116)     1861 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/docs/_includes/examples/references.json
--rw-r--r--   0 runner    (1001) docker     (116)      570 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/docs/_includes/examples/with_default.json
--rw-r--r--   0 runner    (1001) docker     (116)      523 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/docs/_includes/examples/with_definitions.json
--rw-r--r--   0 runner    (1001) docker     (116)     1322 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/docs/_includes/examples/with_descriptions.json
--rw-r--r--   0 runner    (1001) docker     (116)     1802 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/docs/_includes/examples/with_examples.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-15 19:35:57.000000 json-schema-for-humans-0.9.0/docs/assets/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-15 19:35:57.000000 json-schema-for-humans-0.9.0/docs/assets/examples/
--rw-r--r--   0 runner    (1001) docker     (116)     4387 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/docs/assets/examples/array.html
--rw-r--r--   0 runner    (1001) docker     (116)     3063 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/docs/assets/examples/array_advanced.html
--rw-r--r--   0 runner    (1001) docker     (116)     3062 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/docs/assets/examples/basic.html
--rw-r--r--   0 runner    (1001) docker     (116)     1831 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/docs/assets/examples/combining_not.html
--rw-r--r--   0 runner    (1001) docker     (116)     3562 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/docs/assets/examples/combining_oneOf.html
--rw-r--r--   0 runner    (1001) docker     (116)     3214 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/docs/assets/examples/deprecated.html
--rw-r--r--   0 runner    (1001) docker     (116)     2746 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/docs/assets/examples/geo.html
--rw-r--r--   0 runner    (1001) docker     (116)     3636 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/docs/assets/examples/multiple_types.html
--rw-r--r--   0 runner    (1001) docker     (116)     4602 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/docs/assets/examples/pattern_properties.html
--rw-r--r--   0 runner    (1001) docker     (116)    15495 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/docs/assets/examples/references.html
--rw-r--r--   0 runner    (1001) docker     (116)     1270 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/docs/assets/examples/schema_doc.css
--rw-r--r--   0 runner    (1001) docker     (116)      734 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/docs/assets/examples/schema_doc.min.js
--rw-r--r--   0 runner    (1001) docker     (116)     4097 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/docs/assets/examples/with_default.html
--rw-r--r--   0 runner    (1001) docker     (116)     7091 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/docs/assets/examples/with_definitions.html
--rw-r--r--   0 runner    (1001) docker     (116)    10657 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/docs/assets/examples/with_descriptions.html
--rw-r--r--   0 runner    (1001) docker     (116)     5425 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/docs/assets/examples/with_examples.html
--rw-r--r--   0 runner    (1001) docker     (116)     1292 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/docs/generate_examples.py
--rw-r--r--   0 runner    (1001) docker     (116)      694 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-15 19:35:57.000000 json-schema-for-humans-0.9.0/json_schema_for_humans/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/json_schema_for_humans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    16626 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/json_schema_for_humans/generate.py
--rw-r--r--   0 runner    (1001) docker     (116)     1270 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/json_schema_for_humans/schema_doc.css
--rw-r--r--   0 runner    (1001) docker     (116)     1955 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/json_schema_for_humans/schema_doc.js
--rw-r--r--   0 runner    (1001) docker     (116)      734 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/json_schema_for_humans/schema_doc.min.js
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-15 19:35:57.000000 json-schema-for-humans-0.9.0/json_schema_for_humans/templates/
--rw-r--r--   0 runner    (1001) docker     (116)    14995 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/json_schema_for_humans/templates/schema_doc.template.html
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-15 19:35:57.000000 json-schema-for-humans-0.9.0/json_schema_for_humans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4956 2020-05-15 19:35:56.000000 json-schema-for-humans-0.9.0/json_schema_for_humans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2780 2020-05-15 19:35:57.000000 json-schema-for-humans-0.9.0/json_schema_for_humans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-05-15 19:35:56.000000 json-schema-for-humans-0.9.0/json_schema_for_humans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       78 2020-05-15 19:35:56.000000 json-schema-for-humans-0.9.0/json_schema_for_humans.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-05-15 19:35:56.000000 json-schema-for-humans-0.9.0/json_schema_for_humans.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       47 2020-05-15 19:35:56.000000 json-schema-for-humans-0.9.0/json_schema_for_humans.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (116)       40 2020-05-15 19:35:56.000000 json-schema-for-humans-0.9.0/json_schema_for_humans.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       23 2020-05-15 19:35:56.000000 json-schema-for-humans-0.9.0/json_schema_for_humans.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      394 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)       39 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)      845 2020-05-15 19:35:57.000000 json-schema-for-humans-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)       70 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-15 19:35:57.000000 json-schema-for-humans-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-15 19:35:57.000000 json-schema-for-humans-0.9.0/tests/cases/
--rw-r--r--   0 runner    (1001) docker     (116)      812 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/tests/cases/array.json
--rw-r--r--   0 runner    (1001) docker     (116)      516 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/tests/cases/array_advanced.json
--rw-r--r--   0 runner    (1001) docker     (116)      587 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/tests/cases/basic.json
--rw-r--r--   0 runner    (1001) docker     (116)      285 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/tests/cases/combining_not.json
--rw-r--r--   0 runner    (1001) docker     (116)      571 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/tests/cases/combining_oneOf.json
--rw-r--r--   0 runner    (1001) docker     (116)      439 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/tests/cases/deprecated.json
--rw-r--r--   0 runner    (1001) docker     (116)      742 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/tests/cases/description_with_ref.json
--rw-r--r--   0 runner    (1001) docker     (116)      485 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/tests/cases/geo.json
--rw-r--r--   0 runner    (1001) docker     (116)      684 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/tests/cases/multiple_types.json
--rw-r--r--   0 runner    (1001) docker     (116)      943 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/tests/cases/pattern_properties.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-15 19:35:57.000000 json-schema-for-humans-0.9.0/tests/cases/reference_schemas/
--rw-r--r--   0 runner    (1001) docker     (116)      471 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/tests/cases/reference_schemas/final.json
--rw-r--r--   0 runner    (1001) docker     (116)      325 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/tests/cases/reference_schemas/intermediate.json
--rw-r--r--   0 runner    (1001) docker     (116)     1861 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/tests/cases/references.json
--rw-r--r--   0 runner    (1001) docker     (116)     1481 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/tests/cases/top_level_array.json
--rw-r--r--   0 runner    (1001) docker     (116)      427 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/tests/cases/top_level_combining.json
--rw-r--r--   0 runner    (1001) docker     (116)      570 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/tests/cases/with_default.json
--rw-r--r--   0 runner    (1001) docker     (116)      523 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/tests/cases/with_definitions.json
--rw-r--r--   0 runner    (1001) docker     (116)     1322 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/tests/cases/with_descriptions.json
--rw-r--r--   0 runner    (1001) docker     (116)     1802 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/tests/cases/with_examples.json
--rw-r--r--   0 runner    (1001) docker     (116)      648 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/tests/cases/with_special_chars.json
--rw-r--r--   0 runner    (1001) docker     (116)    13527 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/tests/generate_test.py
--rw-r--r--   0 runner    (1001) docker     (116)      145 2020-05-15 19:35:38.000000 json-schema-for-humans-0.9.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (116)      469 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      471 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/.github/workflows/pythonpackage.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      319 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (116)      563 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)     4956 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     3372 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (116)       72 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/Gemfile
+-rw-r--r--   0 runner    (1001) docker     (116)       28 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/docs/_data/
+-rw-r--r--   0 runner    (1001) docker     (116)     1487 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/_data/examples.yaml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/docs/_includes/
+-rw-r--r--   0 runner    (1001) docker     (116)     3372 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/_includes/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/docs/_includes/examples/
+-rw-r--r--   0 runner    (1001) docker     (116)      812 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/_includes/examples/array.json
+-rw-r--r--   0 runner    (1001) docker     (116)      516 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/_includes/examples/array_advanced.json
+-rw-r--r--   0 runner    (1001) docker     (116)      587 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/_includes/examples/basic.json
+-rw-r--r--   0 runner    (1001) docker     (116)      285 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/_includes/examples/combining_not.json
+-rw-r--r--   0 runner    (1001) docker     (116)      571 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/_includes/examples/combining_oneOf.json
+-rw-r--r--   0 runner    (1001) docker     (116)      439 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/_includes/examples/deprecated.json
+-rw-r--r--   0 runner    (1001) docker     (116)      485 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/_includes/examples/geo.json
+-rw-r--r--   0 runner    (1001) docker     (116)      684 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/_includes/examples/multiple_types.json
+-rw-r--r--   0 runner    (1001) docker     (116)      943 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/_includes/examples/pattern_properties.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1861 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/_includes/examples/references.json
+-rw-r--r--   0 runner    (1001) docker     (116)      570 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/_includes/examples/with_default.json
+-rw-r--r--   0 runner    (1001) docker     (116)      523 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/_includes/examples/with_definitions.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1322 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/_includes/examples/with_descriptions.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1802 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/_includes/examples/with_examples.json
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/docs/assets/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/docs/assets/examples/
+-rw-r--r--   0 runner    (1001) docker     (116)     4387 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/assets/examples/array.html
+-rw-r--r--   0 runner    (1001) docker     (116)     3063 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/assets/examples/array_advanced.html
+-rw-r--r--   0 runner    (1001) docker     (116)     3062 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/assets/examples/basic.html
+-rw-r--r--   0 runner    (1001) docker     (116)     1831 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/assets/examples/combining_not.html
+-rw-r--r--   0 runner    (1001) docker     (116)     3562 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/assets/examples/combining_oneOf.html
+-rw-r--r--   0 runner    (1001) docker     (116)     3214 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/assets/examples/deprecated.html
+-rw-r--r--   0 runner    (1001) docker     (116)     2746 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/assets/examples/geo.html
+-rw-r--r--   0 runner    (1001) docker     (116)     3636 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/assets/examples/multiple_types.html
+-rw-r--r--   0 runner    (1001) docker     (116)     4602 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/assets/examples/pattern_properties.html
+-rw-r--r--   0 runner    (1001) docker     (116)    15495 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/assets/examples/references.html
+-rw-r--r--   0 runner    (1001) docker     (116)     1270 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/assets/examples/schema_doc.css
+-rw-r--r--   0 runner    (1001) docker     (116)      734 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/assets/examples/schema_doc.min.js
+-rw-r--r--   0 runner    (1001) docker     (116)     4097 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/assets/examples/with_default.html
+-rw-r--r--   0 runner    (1001) docker     (116)     7091 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/assets/examples/with_definitions.html
+-rw-r--r--   0 runner    (1001) docker     (116)    10657 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/assets/examples/with_descriptions.html
+-rw-r--r--   0 runner    (1001) docker     (116)     5425 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/assets/examples/with_examples.html
+-rw-r--r--   0 runner    (1001) docker     (116)     1292 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/generate_examples.py
+-rw-r--r--   0 runner    (1001) docker     (116)      694 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/json_schema_for_humans/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/json_schema_for_humans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16626 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/json_schema_for_humans/generate.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1270 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/json_schema_for_humans/schema_doc.css
+-rw-r--r--   0 runner    (1001) docker     (116)     1955 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/json_schema_for_humans/schema_doc.js
+-rw-r--r--   0 runner    (1001) docker     (116)      734 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/json_schema_for_humans/schema_doc.min.js
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/json_schema_for_humans/templates/
+-rw-r--r--   0 runner    (1001) docker     (116)    14994 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/json_schema_for_humans/templates/schema_doc.template.html
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/json_schema_for_humans.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     4956 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/json_schema_for_humans.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2780 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/json_schema_for_humans.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/json_schema_for_humans.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       78 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/json_schema_for_humans.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/json_schema_for_humans.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)       47 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/json_schema_for_humans.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (116)       40 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/json_schema_for_humans.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       23 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/json_schema_for_humans.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      394 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (116)       39 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      845 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)       70 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/tests/cases/
+-rw-r--r--   0 runner    (1001) docker     (116)      812 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/array.json
+-rw-r--r--   0 runner    (1001) docker     (116)      516 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/array_advanced.json
+-rw-r--r--   0 runner    (1001) docker     (116)      587 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/basic.json
+-rw-r--r--   0 runner    (1001) docker     (116)      285 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/combining_not.json
+-rw-r--r--   0 runner    (1001) docker     (116)      571 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/combining_oneOf.json
+-rw-r--r--   0 runner    (1001) docker     (116)      439 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/deprecated.json
+-rw-r--r--   0 runner    (1001) docker     (116)      742 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/description_with_ref.json
+-rw-r--r--   0 runner    (1001) docker     (116)      485 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/geo.json
+-rw-r--r--   0 runner    (1001) docker     (116)      684 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/multiple_types.json
+-rw-r--r--   0 runner    (1001) docker     (116)      943 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/pattern_properties.json
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-16 17:08:58.000000 json-schema-for-humans-0.9.1/tests/cases/reference_schemas/
+-rw-r--r--   0 runner    (1001) docker     (116)      471 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/reference_schemas/final.json
+-rw-r--r--   0 runner    (1001) docker     (116)      325 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/reference_schemas/intermediate.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1861 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/references.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1481 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/top_level_array.json
+-rw-r--r--   0 runner    (1001) docker     (116)      427 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/top_level_combining.json
+-rw-r--r--   0 runner    (1001) docker     (116)      570 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/with_default.json
+-rw-r--r--   0 runner    (1001) docker     (116)      523 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/with_definitions.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1322 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/with_descriptions.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1802 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/with_examples.json
+-rw-r--r--   0 runner    (1001) docker     (116)      648 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/cases/with_special_chars.json
+-rw-r--r--   0 runner    (1001) docker     (116)    13527 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tests/generate_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)      145 2020-05-16 17:08:44.000000 json-schema-for-humans-0.9.1/tox.ini
```

### Comparing `json-schema-for-humans-0.9.0/LICENSE` & `json-schema-for-humans-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/PKG-INFO` & `json-schema-for-humans-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-schema-for-humans
-Version: 0.9.0
+Version: 0.9.1
 Summary: Generate static HTML documentation from JSON schemas
 Home-page: https://github.com/coveooss/json-schema-for-humans
 Author: Denis Blanchette, AbdulRahman Al Hamali
 Author-email: tools@coveo.com
 License: Apache Software License
 Description: # JSON Schema for Humans
         
@@ -73,21 +73,21 @@
         - Numeric types multiples and range
         - Constant and enumerated values
         - Required properties
         - Pattern properties
         - Default values
         - Array `minItems`, `maxItems`, `uniqueItems`, `items` (schema that must apply to all of the array items), and `contains`
         - Combining schema with `oneOf`, `allOf`, `anyOf`, and `not`
+        - Examples
         
         These are **not** supported at the moment (PRs welcome!):
         - String length and format
         - Property names and size
         - Array items at specific index (for example, first item must be a string and second must be an integer)
         - Property dependencies
-        - Examples
         - Media
         - Conditional subschemas
         
         References from inside a schema and to schemas in other files are supported (for example `{ $ref: "#/definitions/something" }` will be replaced by the 
         content of `schema["definitions"]["something"]`).
         
         ## Anchor links
```

### Comparing `json-schema-for-humans-0.9.0/README.md` & `json-schema-for-humans-0.9.1/README.md`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -65,21 +65,21 @@
 - Numeric types multiples and range
 - Constant and enumerated values
 - Required properties
 - Pattern properties
 - Default values
 - Array `minItems`, `maxItems`, `uniqueItems`, `items` (schema that must apply to all of the array items), and `contains`
 - Combining schema with `oneOf`, `allOf`, `anyOf`, and `not`
+- Examples
 
 These are **not** supported at the moment (PRs welcome!):
 - String length and format
 - Property names and size
 - Array items at specific index (for example, first item must be a string and second must be an integer)
 - Property dependencies
-- Examples
 - Media
 - Conditional subschemas
 
 References from inside a schema and to schemas in other files are supported (for example `{ $ref: "#/definitions/something" }` will be replaced by the 
 content of `schema["definitions"]["something"]`).
 
 ## Anchor links
```

### Comparing `json-schema-for-humans-0.9.0/docs/_data/examples.yaml` & `json-schema-for-humans-0.9.1/docs/_data/examples.yaml`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/docs/_includes/README.md` & `json-schema-for-humans-0.9.1/docs/_includes/README.md`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -65,21 +65,21 @@
 - Numeric types multiples and range
 - Constant and enumerated values
 - Required properties
 - Pattern properties
 - Default values
 - Array `minItems`, `maxItems`, `uniqueItems`, `items` (schema that must apply to all of the array items), and `contains`
 - Combining schema with `oneOf`, `allOf`, `anyOf`, and `not`
+- Examples
 
 These are **not** supported at the moment (PRs welcome!):
 - String length and format
 - Property names and size
 - Array items at specific index (for example, first item must be a string and second must be an integer)
 - Property dependencies
-- Examples
 - Media
 - Conditional subschemas
 
 References from inside a schema and to schemas in other files are supported (for example `{ $ref: "#/definitions/something" }` will be replaced by the 
 content of `schema["definitions"]["something"]`).
 
 ## Anchor links
```

### Comparing `json-schema-for-humans-0.9.0/docs/_includes/examples/array.json` & `json-schema-for-humans-0.9.1/docs/_includes/examples/array.json`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/docs/_includes/examples/array_advanced.json` & `json-schema-for-humans-0.9.1/docs/_includes/examples/array_advanced.json`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/docs/_includes/examples/basic.json` & `json-schema-for-humans-0.9.1/docs/_includes/examples/basic.json`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/docs/_includes/examples/combining_oneOf.json` & `json-schema-for-humans-0.9.1/docs/_includes/examples/combining_oneOf.json`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/docs/_includes/examples/multiple_types.json` & `json-schema-for-humans-0.9.1/docs/_includes/examples/multiple_types.json`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/docs/_includes/examples/pattern_properties.json` & `json-schema-for-humans-0.9.1/docs/_includes/examples/pattern_properties.json`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/docs/_includes/examples/references.json` & `json-schema-for-humans-0.9.1/docs/_includes/examples/references.json`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/docs/_includes/examples/with_default.json` & `json-schema-for-humans-0.9.1/docs/_includes/examples/with_default.json`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/docs/_includes/examples/with_definitions.json` & `json-schema-for-humans-0.9.1/docs/_includes/examples/with_definitions.json`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/docs/_includes/examples/with_descriptions.json` & `json-schema-for-humans-0.9.1/docs/_includes/examples/with_descriptions.json`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/docs/_includes/examples/with_examples.json` & `json-schema-for-humans-0.9.1/docs/_includes/examples/with_examples.json`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/docs/assets/examples/array.html` & `json-schema-for-humans-0.9.1/docs/assets/examples/array.html`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/docs/assets/examples/array_advanced.html` & `json-schema-for-humans-0.9.1/docs/assets/examples/array_advanced.html`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/docs/assets/examples/basic.html` & `json-schema-for-humans-0.9.1/docs/assets/examples/basic.html`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/docs/assets/examples/combining_not.html` & `json-schema-for-humans-0.9.1/docs/assets/examples/combining_not.html`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/docs/assets/examples/combining_oneOf.html` & `json-schema-for-humans-0.9.1/docs/assets/examples/combining_oneOf.html`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/docs/assets/examples/deprecated.html` & `json-schema-for-humans-0.9.1/docs/assets/examples/deprecated.html`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/docs/assets/examples/geo.html` & `json-schema-for-humans-0.9.1/docs/assets/examples/geo.html`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/docs/assets/examples/multiple_types.html` & `json-schema-for-humans-0.9.1/docs/assets/examples/multiple_types.html`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/docs/assets/examples/pattern_properties.html` & `json-schema-for-humans-0.9.1/docs/assets/examples/pattern_properties.html`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/docs/assets/examples/references.html` & `json-schema-for-humans-0.9.1/docs/assets/examples/references.html`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/docs/assets/examples/schema_doc.css` & `json-schema-for-humans-0.9.1/docs/assets/examples/schema_doc.css`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/docs/assets/examples/schema_doc.min.js` & `json-schema-for-humans-0.9.1/docs/assets/examples/schema_doc.min.js`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/docs/assets/examples/with_default.html` & `json-schema-for-humans-0.9.1/docs/assets/examples/with_default.html`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/docs/assets/examples/with_definitions.html` & `json-schema-for-humans-0.9.1/docs/assets/examples/with_definitions.html`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/docs/assets/examples/with_descriptions.html` & `json-schema-for-humans-0.9.1/docs/assets/examples/with_descriptions.html`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/docs/assets/examples/with_examples.html` & `json-schema-for-humans-0.9.1/docs/assets/examples/with_examples.html`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/docs/generate_examples.py` & `json-schema-for-humans-0.9.1/docs/generate_examples.py`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/docs/index.md` & `json-schema-for-humans-0.9.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/json_schema_for_humans/generate.py` & `json-schema-for-humans-0.9.1/json_schema_for_humans/generate.py`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/json_schema_for_humans/schema_doc.css` & `json-schema-for-humans-0.9.1/json_schema_for_humans/schema_doc.css`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/json_schema_for_humans/schema_doc.js` & `json-schema-for-humans-0.9.1/json_schema_for_humans/schema_doc.js`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/json_schema_for_humans/schema_doc.min.js` & `json-schema-for-humans-0.9.1/json_schema_for_humans/schema_doc.min.js`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/json_schema_for_humans/templates/schema_doc.template.html` & `json-schema-for-humans-0.9.1/json_schema_for_humans/templates/schema_doc.template.html`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         {%- endfor -%}
     </ul>
     <div class="tab-content card">
         {%- for element in property[operator] -%}
             {%- set tab_id = index ~ "__option" ~ loop.index -%}
             <div class="tab-pane fade card-body {% if loop.index == 1 -%}active show{% endif -%}"
                  id="tab-pane_{{ tab_id }}" role="tabpanel">
-                {{ content(tab_id, tab_label ~ " " ~ loop.index, element, property_path, False) }}
+                {{ content(tab_id, tab_label ~ " " ~ loop.index, element, property_path, True) }}
             </div>
         {%- endfor -%}
     </div>
 {%- endmacro -%}
 
 {%- macro add_description(property) -%}
     {%- set description = property.get("description") | get_description -%}
```

### Comparing `json-schema-for-humans-0.9.0/json_schema_for_humans.egg-info/PKG-INFO` & `json-schema-for-humans-0.9.1/json_schema_for_humans.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-schema-for-humans
-Version: 0.9.0
+Version: 0.9.1
 Summary: Generate static HTML documentation from JSON schemas
 Home-page: https://github.com/coveooss/json-schema-for-humans
 Author: Denis Blanchette, AbdulRahman Al Hamali
 Author-email: tools@coveo.com
 License: Apache Software License
 Description: # JSON Schema for Humans
         
@@ -73,21 +73,21 @@
         - Numeric types multiples and range
         - Constant and enumerated values
         - Required properties
         - Pattern properties
         - Default values
         - Array `minItems`, `maxItems`, `uniqueItems`, `items` (schema that must apply to all of the array items), and `contains`
         - Combining schema with `oneOf`, `allOf`, `anyOf`, and `not`
+        - Examples
         
         These are **not** supported at the moment (PRs welcome!):
         - String length and format
         - Property names and size
         - Array items at specific index (for example, first item must be a string and second must be an integer)
         - Property dependencies
-        - Examples
         - Media
         - Conditional subschemas
         
         References from inside a schema and to schemas in other files are supported (for example `{ $ref: "#/definitions/something" }` will be replaced by the 
         content of `schema["definitions"]["something"]`).
         
         ## Anchor links
```

### Comparing `json-schema-for-humans-0.9.0/json_schema_for_humans.egg-info/SOURCES.txt` & `json-schema-for-humans-0.9.1/json_schema_for_humans.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/setup.cfg` & `json-schema-for-humans-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/tests/cases/array.json` & `json-schema-for-humans-0.9.1/tests/cases/array.json`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/tests/cases/array_advanced.json` & `json-schema-for-humans-0.9.1/tests/cases/array_advanced.json`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/tests/cases/basic.json` & `json-schema-for-humans-0.9.1/tests/cases/basic.json`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/tests/cases/combining_oneOf.json` & `json-schema-for-humans-0.9.1/tests/cases/combining_oneOf.json`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/tests/cases/description_with_ref.json` & `json-schema-for-humans-0.9.1/tests/cases/description_with_ref.json`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/tests/cases/multiple_types.json` & `json-schema-for-humans-0.9.1/tests/cases/multiple_types.json`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/tests/cases/pattern_properties.json` & `json-schema-for-humans-0.9.1/tests/cases/pattern_properties.json`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/tests/cases/references.json` & `json-schema-for-humans-0.9.1/tests/cases/references.json`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/tests/cases/top_level_array.json` & `json-schema-for-humans-0.9.1/tests/cases/top_level_array.json`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/tests/cases/with_default.json` & `json-schema-for-humans-0.9.1/tests/cases/with_default.json`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/tests/cases/with_definitions.json` & `json-schema-for-humans-0.9.1/tests/cases/with_definitions.json`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/tests/cases/with_descriptions.json` & `json-schema-for-humans-0.9.1/tests/cases/with_descriptions.json`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/tests/cases/with_examples.json` & `json-schema-for-humans-0.9.1/tests/cases/with_examples.json`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/tests/cases/with_special_chars.json` & `json-schema-for-humans-0.9.1/tests/cases/with_special_chars.json`

 * *Files identical despite different names*

### Comparing `json-schema-for-humans-0.9.0/tests/generate_test.py` & `json-schema-for-humans-0.9.1/tests/generate_test.py`

 * *Files identical despite different names*

