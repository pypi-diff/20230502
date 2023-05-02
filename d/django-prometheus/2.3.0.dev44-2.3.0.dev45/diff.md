# Comparing `tmp/django-prometheus-2.3.0.dev44.tar.gz` & `tmp/django-prometheus-2.3.0.dev45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-prometheus-2.3.0.dev44.tar", last modified: Mon May  1 19:37:36 2023, max compression
+gzip compressed data, was "django-prometheus-2.3.0.dev45.tar", last modified: Mon May  1 19:53:27 2023, max compression
```

## Comparing `django-prometheus-2.3.0.dev44.tar` & `django-prometheus-2.3.0.dev45.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:36.629759 django-prometheus-2.3.0.dev44/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-05-01 19:37:36.633759 django-prometheus-2.3.0.dev44/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:36.625759 django-prometheus-2.3.0.dev44/django_prometheus/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-01 19:37:26.000000 django-prometheus-2.3.0.dev44/django_prometheus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:36.625759 django-prometheus-2.3.0.dev44/django_prometheus/cache/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/cache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:36.625759 django-prometheus-2.3.0.dev44/django_prometheus/cache/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/cache/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/cache/backends/django_memcached_consul.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/cache/backends/filebased.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/cache/backends/locmem.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/cache/backends/memcached.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/cache/backends/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/cache/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:36.629759 django-prometheus-2.3.0.dev44/django_prometheus/conf/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/conf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:36.629759 django-prometheus-2.3.0.dev44/django_prometheus/db/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:36.629759 django-prometheus-2.3.0.dev44/django_prometheus/db/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/db/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/db/backends/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:36.629759 django-prometheus-2.3.0.dev44/django_prometheus/db/backends/mysql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/db/backends/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/db/backends/mysql/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:36.629759 django-prometheus-2.3.0.dev44/django_prometheus/db/backends/postgis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/db/backends/postgis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/db/backends/postgis/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:36.629759 django-prometheus-2.3.0.dev44/django_prometheus/db/backends/postgresql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/db/backends/postgresql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/db/backends/postgresql/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:36.629759 django-prometheus-2.3.0.dev44/django_prometheus/db/backends/sqlite3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/db/backends/sqlite3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/db/backends/sqlite3/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/db/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/db/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/exports.py
--rw-r--r--   0 runner    (1001) docker     (123)    11981 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:36.629759 django-prometheus-2.3.0.dev44/django_prometheus/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/tests/test_django_prometheus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/tests/test_exports.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/tests/test_testutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/testutils.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/django_prometheus/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:37:36.625759 django-prometheus-2.3.0.dev44/django_prometheus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-05-01 19:37:36.000000 django-prometheus-2.3.0.dev44/django_prometheus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-01 19:37:36.000000 django-prometheus-2.3.0.dev44/django_prometheus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 19:37:36.000000 django-prometheus-2.3.0.dev44/django_prometheus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-01 19:37:36.000000 django-prometheus-2.3.0.dev44/django_prometheus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-01 19:37:36.000000 django-prometheus-2.3.0.dev44/django_prometheus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-01 19:37:36.633759 django-prometheus-2.3.0.dev44/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-01 19:37:13.000000 django-prometheus-2.3.0.dev44/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:53:27.294363 django-prometheus-2.3.0.dev45/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-05-01 19:53:27.294363 django-prometheus-2.3.0.dev45/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:53:27.286363 django-prometheus-2.3.0.dev45/django_prometheus/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-01 19:53:15.000000 django-prometheus-2.3.0.dev45/django_prometheus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/django_prometheus/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:53:27.290363 django-prometheus-2.3.0.dev45/django_prometheus/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/django_prometheus/cache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:53:27.290363 django-prometheus-2.3.0.dev45/django_prometheus/cache/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/django_prometheus/cache/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/django_prometheus/cache/backends/django_memcached_consul.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/django_prometheus/cache/backends/filebased.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/django_prometheus/cache/backends/locmem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/django_prometheus/cache/backends/memcached.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/django_prometheus/cache/backends/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/django_prometheus/cache/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:53:27.290363 django-prometheus-2.3.0.dev45/django_prometheus/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/django_prometheus/conf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:53:27.290363 django-prometheus-2.3.0.dev45/django_prometheus/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/django_prometheus/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:53:27.290363 django-prometheus-2.3.0.dev45/django_prometheus/db/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/django_prometheus/db/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/django_prometheus/db/backends/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:53:27.290363 django-prometheus-2.3.0.dev45/django_prometheus/db/backends/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/django_prometheus/db/backends/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/django_prometheus/db/backends/mysql/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:53:27.290363 django-prometheus-2.3.0.dev45/django_prometheus/db/backends/postgis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/django_prometheus/db/backends/postgis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/django_prometheus/db/backends/postgis/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:53:27.294363 django-prometheus-2.3.0.dev45/django_prometheus/db/backends/postgresql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/django_prometheus/db/backends/postgresql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/django_prometheus/db/backends/postgresql/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:53:27.294363 django-prometheus-2.3.0.dev45/django_prometheus/db/backends/sqlite3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/django_prometheus/db/backends/sqlite3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/django_prometheus/db/backends/sqlite3/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/django_prometheus/db/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/django_prometheus/db/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/django_prometheus/exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11981 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/django_prometheus/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/django_prometheus/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/django_prometheus/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:53:27.294363 django-prometheus-2.3.0.dev45/django_prometheus/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/django_prometheus/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/django_prometheus/tests/test_django_prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/django_prometheus/tests/test_exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/django_prometheus/tests/test_testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/django_prometheus/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/django_prometheus/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/django_prometheus/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:53:27.286363 django-prometheus-2.3.0.dev45/django_prometheus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-05-01 19:53:27.000000 django-prometheus-2.3.0.dev45/django_prometheus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-01 19:53:27.000000 django-prometheus-2.3.0.dev45/django_prometheus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 19:53:27.000000 django-prometheus-2.3.0.dev45/django_prometheus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-01 19:53:27.000000 django-prometheus-2.3.0.dev45/django_prometheus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-01 19:53:27.000000 django-prometheus-2.3.0.dev45/django_prometheus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-01 19:53:27.294363 django-prometheus-2.3.0.dev45/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-01 19:52:58.000000 django-prometheus-2.3.0.dev45/setup.py
```

### Comparing `django-prometheus-2.3.0.dev44/LICENSE` & `django-prometheus-2.3.0.dev45/LICENSE`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev44/PKG-INFO` & `django-prometheus-2.3.0.dev45/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-prometheus
-Version: 2.3.0.dev44
+Version: 2.3.0.dev45
 Summary: Django middlewares to monitor your application with Prometheus.io.
 Home-page: http://github.com/korfuri/django-prometheus
 Author: Uriel Corfa
 Author-email: uriel@corfa.fr
 License: Apache
 Project-URL: Changelog, https://github.com/korfuri/django-prometheus/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/korfuri/django-prometheus/blob/master/README.md
```

### Comparing `django-prometheus-2.3.0.dev44/README.md` & `django-prometheus-2.3.0.dev45/README.md`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev44/django_prometheus/__init__.py` & `django-prometheus-2.3.0.dev45/django_prometheus/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Import all files that define metrics. This has the effect that
 # `import django_prometheus` will always instantiate all metric
 # objects right away.
 from django_prometheus import middleware, models
 
 __all__ = ["middleware", "models", "pip_prometheus"]
 
-__version__ = "2.3.0.dev44"
+__version__ = "2.3.0.dev45"
 
 
 # Import pip_prometheus to export the pip metrics automatically.
 try:
     import pip_prometheus
 except ImportError:
     # If people don't have pip, don't export anything.
```

### Comparing `django-prometheus-2.3.0.dev44/django_prometheus/apps.py` & `django-prometheus-2.3.0.dev45/django_prometheus/apps.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev44/django_prometheus/cache/backends/django_memcached_consul.py` & `django-prometheus-2.3.0.dev45/django_prometheus/cache/backends/django_memcached_consul.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev44/django_prometheus/cache/backends/filebased.py` & `django-prometheus-2.3.0.dev45/django_prometheus/cache/backends/filebased.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev44/django_prometheus/cache/backends/locmem.py` & `django-prometheus-2.3.0.dev45/django_prometheus/cache/backends/locmem.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev44/django_prometheus/cache/backends/memcached.py` & `django-prometheus-2.3.0.dev45/django_prometheus/cache/backends/memcached.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev44/django_prometheus/cache/backends/redis.py` & `django-prometheus-2.3.0.dev45/django_prometheus/cache/backends/redis.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev44/django_prometheus/cache/metrics.py` & `django-prometheus-2.3.0.dev45/django_prometheus/cache/metrics.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev44/django_prometheus/db/backends/mysql/base.py` & `django-prometheus-2.3.0.dev45/django_prometheus/db/backends/mysql/base.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev44/django_prometheus/db/backends/postgis/base.py` & `django-prometheus-2.3.0.dev45/django_prometheus/db/backends/postgis/base.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev44/django_prometheus/db/backends/postgresql/base.py` & `django-prometheus-2.3.0.dev45/django_prometheus/db/backends/postgresql/base.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev44/django_prometheus/db/common.py` & `django-prometheus-2.3.0.dev45/django_prometheus/db/common.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev44/django_prometheus/db/metrics.py` & `django-prometheus-2.3.0.dev45/django_prometheus/db/metrics.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev44/django_prometheus/exports.py` & `django-prometheus-2.3.0.dev45/django_prometheus/exports.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev44/django_prometheus/middleware.py` & `django-prometheus-2.3.0.dev45/django_prometheus/middleware.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev44/django_prometheus/migrations.py` & `django-prometheus-2.3.0.dev45/django_prometheus/migrations.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev44/django_prometheus/models.py` & `django-prometheus-2.3.0.dev45/django_prometheus/models.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev44/django_prometheus/tests/test_exports.py` & `django-prometheus-2.3.0.dev45/django_prometheus/tests/test_exports.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev44/django_prometheus/tests/test_testutils.py` & `django-prometheus-2.3.0.dev45/django_prometheus/tests/test_testutils.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev44/django_prometheus/testutils.py` & `django-prometheus-2.3.0.dev45/django_prometheus/testutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,8 +192,8 @@
     return "{%s}" % ",".join([f'{k}="{v}"' for k, v in labels.items()])
 
 
 def format_vector(vector):
     """Formats a list of (labels, value) where labels is a dict into a
     human-readable representation.
     """
-    return "\n".join(["{} = {}".format(format_labels(labels), value) for labels, value in vector])
+    return "\n".join([f"{format_labels(labels)} = {value}" for labels, value in vector])
```

### Comparing `django-prometheus-2.3.0.dev44/django_prometheus/utils.py` & `django-prometheus-2.3.0.dev45/django_prometheus/utils.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev44/django_prometheus.egg-info/PKG-INFO` & `django-prometheus-2.3.0.dev45/django_prometheus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-prometheus
-Version: 2.3.0.dev44
+Version: 2.3.0.dev45
 Summary: Django middlewares to monitor your application with Prometheus.io.
 Home-page: http://github.com/korfuri/django-prometheus
 Author: Uriel Corfa
 Author-email: uriel@corfa.fr
 License: Apache
 Project-URL: Changelog, https://github.com/korfuri/django-prometheus/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/korfuri/django-prometheus/blob/master/README.md
```

### Comparing `django-prometheus-2.3.0.dev44/django_prometheus.egg-info/SOURCES.txt` & `django-prometheus-2.3.0.dev45/django_prometheus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev44/pyproject.toml` & `django-prometheus-2.3.0.dev45/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev44/setup.py` & `django-prometheus-2.3.0.dev45/setup.py`

 * *Files identical despite different names*

