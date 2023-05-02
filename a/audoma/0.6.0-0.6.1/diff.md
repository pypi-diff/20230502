# Comparing `tmp/audoma-0.6.0.tar.gz` & `tmp/audoma-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audoma-0.6.0.tar", last modified: Thu Jan  5 07:06:28 2023, max compression
+gzip compressed data, was "audoma-0.6.1.tar", last modified: Tue May  2 06:50:57 2023, max compression
```

## Comparing `audoma-0.6.0.tar` & `audoma-0.6.1.tar`

### file list

```diff
@@ -1,110 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 07:06:28.981431 audoma-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-01-05 07:06:07.000000 audoma-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-01-05 07:06:07.000000 audoma-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-01-05 07:06:28.981431 audoma-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-01-05 07:06:07.000000 audoma-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 07:06:28.973431 audoma-0.6.0/audoma/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/choices.py
--rw-r--r--   0 runner    (1001) docker     (123)    13957 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 07:06:28.973431 audoma-0.6.0/audoma/django/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/django/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 07:06:28.973431 audoma-0.6.0/audoma/django/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/django/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/django/db/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/django/db/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 07:06:28.973431 audoma-0.6.0/audoma/django/forms/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/django/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/django/forms/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 07:06:28.977431 audoma-0.6.0/audoma/drf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/drf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/drf/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/drf/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/drf/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7846 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/drf/generics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/drf/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/drf/routers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/drf/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/drf/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/drf/viewsets.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/example_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/links.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    17835 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/openapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/plumbing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 07:06:28.977431 audoma-0.6.0/audoma/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 07:06:28.977431 audoma-0.6.0/audoma/tests/drf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/tests/drf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/tests/drf/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    17493 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/tests/drf/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/tests/drf/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/tests/drf/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/tests/test_audoma_django_db_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    12180 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    11412 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/tests/test_generics.py
--rw-r--r--   0 runner    (1001) docker     (123)    22513 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/tests/test_openapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/tests/test_plumbing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6725 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma/tests/testtools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 07:06:28.973431 audoma-0.6.0/audoma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-01-05 07:06:28.000000 audoma-0.6.0/audoma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-01-05 07:06:28.000000 audoma-0.6.0/audoma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 07:06:28.000000 audoma-0.6.0/audoma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-01-05 07:06:28.000000 audoma-0.6.0/audoma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-05 07:06:28.000000 audoma-0.6.0/audoma.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 07:06:28.969431 audoma-0.6.0/audoma_examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 07:06:28.977431 audoma-0.6.0/audoma_examples/drf_example/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 07:06:28.977431 audoma-0.6.0/audoma_examples/drf_example/audoma_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/audoma_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/audoma_api/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/audoma_api/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/audoma_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/audoma_api/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 07:06:28.977431 audoma-0.6.0/audoma_examples/drf_example/audoma_api/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/audoma_api/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/audoma_api/migrations/0002_alter_examplemodel_json_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/audoma_api/migrations/0002_examplesimplemodel_alter_examplemodel_json_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/audoma_api/migrations/0003_car_manufacturer.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/audoma_api/migrations/0003_merge_20220526_1439.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/audoma_api/migrations/0004_merge_20220620_1037.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/audoma_api/migrations/0005_auto_20220706_1013.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/audoma_api/migrations/0006_cartag.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/audoma_api/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/audoma_api/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/audoma_api/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/audoma_api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)    33415 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/audoma_api/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/audoma_api/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 07:06:28.977431 audoma-0.6.0/audoma_examples/drf_example/drf_example/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/drf_example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/drf_example/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/drf_example/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/drf_example/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/drf_example/v1_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/drf_example/v2_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/drf_example/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 07:06:28.981431 audoma-0.6.0/audoma_examples/drf_example/healthcare_api/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/healthcare_api/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 07:06:28.981431 audoma-0.6.0/audoma_examples/drf_example/healthcare_api/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/healthcare_api/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/healthcare_api/migrations/0002_prescription.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/healthcare_api/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/healthcare_api/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/healthcare_api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)    52703 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/healthcare_api/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/healthcare_api/views.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      667 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 07:06:28.981431 audoma-0.6.0/audoma_examples/drf_example/routers/
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/routers/db_routers.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-01-05 07:06:07.000000 audoma-0.6.0/audoma_examples/drf_example/runtests.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-01-05 07:06:07.000000 audoma-0.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-01-05 07:06:07.000000 audoma-0.6.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-01-05 07:06:28.981431 audoma-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-01-05 07:06:07.000000 audoma-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:50:57.526081 audoma-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-02 06:50:25.000000 audoma-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-02 06:50:25.000000 audoma-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-05-02 06:50:57.526081 audoma-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-02 06:50:25.000000 audoma-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:50:57.518081 audoma-0.6.1/audoma/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13957 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:50:57.518081 audoma-0.6.1/audoma/django/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/django/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:50:57.518081 audoma-0.6.1/audoma/django/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/django/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/django/db/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/django/db/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:50:57.522081 audoma-0.6.1/audoma/django/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/django/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/django/forms/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:50:57.522081 audoma-0.6.1/audoma/drf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/drf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/drf/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/drf/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/drf/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7846 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/drf/generics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/drf/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/drf/routers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/drf/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/drf/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/drf/viewsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/example_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17835 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/plumbing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:50:57.522081 audoma-0.6.1/audoma/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:50:57.522081 audoma-0.6.1/audoma/tests/drf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/tests/drf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/tests/drf/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17493 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/tests/drf/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/tests/drf/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/tests/drf/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/tests/test_audoma_django_db_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12180 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11412 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/tests/test_generics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22513 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/tests/test_openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/tests/test_plumbing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6725 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma/tests/testtools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:50:57.518081 audoma-0.6.1/audoma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-05-02 06:50:57.000000 audoma-0.6.1/audoma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-02 06:50:57.000000 audoma-0.6.1/audoma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 06:50:57.000000 audoma-0.6.1/audoma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-02 06:50:57.000000 audoma-0.6.1/audoma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 06:50:57.000000 audoma-0.6.1/audoma.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:50:57.518081 audoma-0.6.1/audoma_examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:50:57.522081 audoma-0.6.1/audoma_examples/drf_example/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:50:57.522081 audoma-0.6.1/audoma_examples/drf_example/audoma_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/audoma_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/audoma_api/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/audoma_api/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/audoma_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/audoma_api/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:50:57.526081 audoma-0.6.1/audoma_examples/drf_example/audoma_api/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/audoma_api/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/audoma_api/migrations/0002_alter_examplemodel_json_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/audoma_api/migrations/0002_examplesimplemodel_alter_examplemodel_json_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/audoma_api/migrations/0003_car_manufacturer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/audoma_api/migrations/0003_merge_20220526_1439.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/audoma_api/migrations/0004_merge_20220620_1037.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/audoma_api/migrations/0005_auto_20220706_1013.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/audoma_api/migrations/0006_cartag.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      638 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/audoma_api/migrations/0007_alter_examplemodel_decimal.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/audoma_api/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/audoma_api/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/audoma_api/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/audoma_api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33415 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/audoma_api/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/audoma_api/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:50:57.526081 audoma-0.6.1/audoma_examples/drf_example/drf_example/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/drf_example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/drf_example/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/drf_example/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/drf_example/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/drf_example/v1_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/drf_example/v2_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/drf_example/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:50:57.526081 audoma-0.6.1/audoma_examples/drf_example/healthcare_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/healthcare_api/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:50:57.526081 audoma-0.6.1/audoma_examples/drf_example/healthcare_api/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/healthcare_api/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/healthcare_api/migrations/0002_prescription.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/healthcare_api/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/healthcare_api/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/healthcare_api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52703 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/healthcare_api/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/healthcare_api/views.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      667 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 06:50:57.526081 audoma-0.6.1/audoma_examples/drf_example/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/routers/db_routers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-02 06:50:25.000000 audoma-0.6.1/audoma_examples/drf_example/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-02 06:50:25.000000 audoma-0.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-02 06:50:25.000000 audoma-0.6.1/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-02 06:50:57.526081 audoma-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-02 06:50:25.000000 audoma-0.6.1/setup.py
```

### Comparing `audoma-0.6.0/LICENSE` & `audoma-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/PKG-INFO` & `audoma-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audoma
-Version: 0.6.0
+Version: 0.6.1
 Summary: API Automatic Documentation Maker - DRF-SPECTACULAR wrapper
 Home-page: UNKNOWN
 Author: ITEO
 License: UNKNOWN
 Description: # audoma - API Automatic Documentation Maker
```

### Comparing `audoma-0.6.0/README.md` & `audoma-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma/choices.py` & `audoma-0.6.1/audoma/choices.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma/decorators.py` & `audoma-0.6.1/audoma/decorators.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma/django/db/fields.py` & `audoma-0.6.1/audoma/django/db/fields.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma/drf/decorators.py` & `audoma-0.6.1/audoma/drf/decorators.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma/drf/fields.py` & `audoma-0.6.1/audoma/drf/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,17 +203,17 @@
     def bind(self, field_name, parent):
         # The method name defaults to `get_{field_name}`.
         if self.method_name is None:
             self.method_name = "get_{field_name}".format(field_name=field_name)
         super().bind(field_name, parent)
         if self.field is not None:
             set_override(self, "field", self.field)
-        # set params for child field
-        self.field.parent = self.parent
-        self.field.field_name = self.field_name
+            # set params for child field
+            self.field.parent = self.parent
+            self.field.field_name = self.field_name
 
     def to_representation(self, obj):
         method = getattr(self.parent, self.method_name)
         value = method(obj)
         if not self.field or value is None:
             return value
         else:
```

### Comparing `audoma-0.6.0/audoma/drf/filters.py` & `audoma-0.6.1/audoma/drf/filters.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma/drf/generics.py` & `audoma-0.6.1/audoma/drf/generics.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma/drf/mixins.py` & `audoma-0.6.1/audoma/drf/mixins.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma/drf/routers.py` & `audoma-0.6.1/audoma/drf/routers.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma/drf/serializers.py` & `audoma-0.6.1/audoma/drf/serializers.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma/drf/validators.py` & `audoma-0.6.1/audoma/drf/validators.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma/drf/viewsets.py` & `audoma-0.6.1/audoma/drf/viewsets.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma/example_generators.py` & `audoma-0.6.1/audoma/example_generators.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma/examples.py` & `audoma-0.6.1/audoma/examples.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma/hooks.py` & `audoma-0.6.1/audoma/hooks.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma/links.py` & `audoma-0.6.1/audoma/links.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma/mixins.py` & `audoma-0.6.1/audoma/mixins.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma/openapi.py` & `audoma-0.6.1/audoma/openapi.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma/operations.py` & `audoma-0.6.1/audoma/operations.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma/plumbing.py` & `audoma-0.6.1/audoma/plumbing.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma/schema.py` & `audoma-0.6.1/audoma/schema.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma/settings.py` & `audoma-0.6.1/audoma/settings.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma/tests/drf/test_fields.py` & `audoma-0.6.1/audoma/tests/drf/test_fields.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma/tests/drf/test_mixins.py` & `audoma-0.6.1/audoma/tests/drf/test_mixins.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma/tests/drf/test_serializers.py` & `audoma-0.6.1/audoma/tests/drf/test_serializers.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma/tests/drf/test_validators.py` & `audoma-0.6.1/audoma/tests/drf/test_validators.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma/tests/test_audoma_django_db_fields.py` & `audoma-0.6.1/audoma/tests/test_audoma_django_db_fields.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma/tests/test_decorators.py` & `audoma-0.6.1/audoma/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma/tests/test_generics.py` & `audoma-0.6.1/audoma/tests/test_generics.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma/tests/test_openapi.py` & `audoma-0.6.1/audoma/tests/test_openapi.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma/tests/test_plumbing.py` & `audoma-0.6.1/audoma/tests/test_plumbing.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma/tests/test_schema.py` & `audoma-0.6.1/audoma/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma/tests/testtools.py` & `audoma-0.6.1/audoma/tests/testtools.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma.egg-info/PKG-INFO` & `audoma-0.6.1/audoma.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audoma
-Version: 0.6.0
+Version: 0.6.1
 Summary: API Automatic Documentation Maker - DRF-SPECTACULAR wrapper
 Home-page: UNKNOWN
 Author: ITEO
 License: UNKNOWN
 Description: # audoma - API Automatic Documentation Maker
```

### Comparing `audoma-0.6.0/audoma.egg-info/SOURCES.txt` & `audoma-0.6.1/audoma.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 audoma_examples/drf_example/audoma_api/migrations/0002_alter_examplemodel_json_and_more.py
 audoma_examples/drf_example/audoma_api/migrations/0002_examplesimplemodel_alter_examplemodel_json_and_more.py
 audoma_examples/drf_example/audoma_api/migrations/0003_car_manufacturer.py
 audoma_examples/drf_example/audoma_api/migrations/0003_merge_20220526_1439.py
 audoma_examples/drf_example/audoma_api/migrations/0004_merge_20220620_1037.py
 audoma_examples/drf_example/audoma_api/migrations/0005_auto_20220706_1013.py
 audoma_examples/drf_example/audoma_api/migrations/0006_cartag.py
+audoma_examples/drf_example/audoma_api/migrations/0007_alter_examplemodel_decimal.py
 audoma_examples/drf_example/audoma_api/migrations/__init__.py
 audoma_examples/drf_example/drf_example/__init__.py
 audoma_examples/drf_example/drf_example/asgi.py
 audoma_examples/drf_example/drf_example/settings.py
 audoma_examples/drf_example/drf_example/urls.py
 audoma_examples/drf_example/drf_example/v1_urls.py
 audoma_examples/drf_example/drf_example/v2_urls.py
```

### Comparing `audoma-0.6.0/audoma_examples/drf_example/audoma_api/migrations/0001_initial.py` & `audoma-0.6.1/audoma_examples/drf_example/audoma_api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma_examples/drf_example/audoma_api/migrations/0002_alter_examplemodel_json_and_more.py` & `audoma-0.6.1/audoma_examples/drf_example/audoma_api/migrations/0002_alter_examplemodel_json_and_more.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma_examples/drf_example/audoma_api/migrations/0002_examplesimplemodel_alter_examplemodel_json_and_more.py` & `audoma-0.6.1/audoma_examples/drf_example/audoma_api/migrations/0002_examplesimplemodel_alter_examplemodel_json_and_more.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma_examples/drf_example/audoma_api/migrations/0003_car_manufacturer.py` & `audoma-0.6.1/audoma_examples/drf_example/audoma_api/migrations/0003_car_manufacturer.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma_examples/drf_example/audoma_api/migrations/0005_auto_20220706_1013.py` & `audoma-0.6.1/audoma_examples/drf_example/audoma_api/migrations/0005_auto_20220706_1013.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma_examples/drf_example/audoma_api/migrations/0006_cartag.py` & `audoma-0.6.1/audoma_examples/drf_example/audoma_api/migrations/0006_cartag.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma_examples/drf_example/audoma_api/models.py` & `audoma-0.6.1/audoma_examples/drf_example/audoma_api/models.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma_examples/drf_example/audoma_api/permissions.py` & `audoma-0.6.1/audoma_examples/drf_example/audoma_api/permissions.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma_examples/drf_example/audoma_api/serializers.py` & `audoma-0.6.1/audoma_examples/drf_example/audoma_api/serializers.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma_examples/drf_example/audoma_api/tests.py` & `audoma-0.6.1/audoma_examples/drf_example/audoma_api/tests.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma_examples/drf_example/audoma_api/views.py` & `audoma-0.6.1/audoma_examples/drf_example/audoma_api/views.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma_examples/drf_example/drf_example/settings.py` & `audoma-0.6.1/audoma_examples/drf_example/drf_example/settings.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma_examples/drf_example/drf_example/urls.py` & `audoma-0.6.1/audoma_examples/drf_example/drf_example/urls.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma_examples/drf_example/drf_example/v1_urls.py` & `audoma-0.6.1/audoma_examples/drf_example/drf_example/v1_urls.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma_examples/drf_example/drf_example/v2_urls.py` & `audoma-0.6.1/audoma_examples/drf_example/drf_example/v2_urls.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma_examples/drf_example/healthcare_api/migrations/0001_initial.py` & `audoma-0.6.1/audoma_examples/drf_example/healthcare_api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma_examples/drf_example/healthcare_api/migrations/0002_prescription.py` & `audoma-0.6.1/audoma_examples/drf_example/healthcare_api/migrations/0002_prescription.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma_examples/drf_example/healthcare_api/models.py` & `audoma-0.6.1/audoma_examples/drf_example/healthcare_api/models.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma_examples/drf_example/healthcare_api/serializers.py` & `audoma-0.6.1/audoma_examples/drf_example/healthcare_api/serializers.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma_examples/drf_example/healthcare_api/tests.py` & `audoma-0.6.1/audoma_examples/drf_example/healthcare_api/tests.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma_examples/drf_example/healthcare_api/views.py` & `audoma-0.6.1/audoma_examples/drf_example/healthcare_api/views.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma_examples/drf_example/manage.py` & `audoma-0.6.1/audoma_examples/drf_example/manage.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma_examples/drf_example/routers/db_routers.py` & `audoma-0.6.1/audoma_examples/drf_example/routers/db_routers.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/audoma_examples/drf_example/runtests.py` & `audoma-0.6.1/audoma_examples/drf_example/runtests.py`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/setup.cfg` & `audoma-0.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `audoma-0.6.0/setup.py` & `audoma-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 django_classifiers = [
     "Framework :: Django",
 ] + ["Framework :: Django :: {}".format(v) for v in django_versions]
 
 
 setup(
     name=name,
-    version="0.6.0",
+    version="0.6.1",
     packages=find_packages(),
     install_requires=get_reqiuired_packages(),
     description=description,
     long_description_content_type="text/markdown",
     long_description=long_description,
     author="ITEO",
     classifiers=[
```

