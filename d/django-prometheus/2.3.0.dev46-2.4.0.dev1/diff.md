# Comparing `tmp/django-prometheus-2.3.0.dev46.tar.gz` & `tmp/django-prometheus-2.4.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-prometheus-2.3.0.dev46.tar", last modified: Tue May  2 15:25:31 2023, max compression
+gzip compressed data, was "django-prometheus-2.4.0.dev1.tar", last modified: Tue May  2 15:51:24 2023, max compression
```

## Comparing `django-prometheus-2.3.0.dev46.tar` & `django-prometheus-2.4.0.dev1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:25:31.122952 django-prometheus-2.3.0.dev46/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-05-02 15:25:31.122952 django-prometheus-2.3.0.dev46/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:25:31.110952 django-prometheus-2.3.0.dev46/django_prometheus/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-02 15:25:22.000000 django-prometheus-2.3.0.dev46/django_prometheus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/django_prometheus/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:25:31.114952 django-prometheus-2.3.0.dev46/django_prometheus/cache/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/django_prometheus/cache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:25:31.114952 django-prometheus-2.3.0.dev46/django_prometheus/cache/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/django_prometheus/cache/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/django_prometheus/cache/backends/django_memcached_consul.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/django_prometheus/cache/backends/filebased.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/django_prometheus/cache/backends/locmem.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/django_prometheus/cache/backends/memcached.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/django_prometheus/cache/backends/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/django_prometheus/cache/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:25:31.114952 django-prometheus-2.3.0.dev46/django_prometheus/conf/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/django_prometheus/conf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:25:31.118952 django-prometheus-2.3.0.dev46/django_prometheus/db/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/django_prometheus/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:25:31.118952 django-prometheus-2.3.0.dev46/django_prometheus/db/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/django_prometheus/db/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/django_prometheus/db/backends/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:25:31.118952 django-prometheus-2.3.0.dev46/django_prometheus/db/backends/mysql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/django_prometheus/db/backends/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/django_prometheus/db/backends/mysql/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:25:31.118952 django-prometheus-2.3.0.dev46/django_prometheus/db/backends/postgis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/django_prometheus/db/backends/postgis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/django_prometheus/db/backends/postgis/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:25:31.118952 django-prometheus-2.3.0.dev46/django_prometheus/db/backends/postgresql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/django_prometheus/db/backends/postgresql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/django_prometheus/db/backends/postgresql/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:25:31.118952 django-prometheus-2.3.0.dev46/django_prometheus/db/backends/sqlite3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/django_prometheus/db/backends/sqlite3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/django_prometheus/db/backends/sqlite3/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/django_prometheus/db/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/django_prometheus/db/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/django_prometheus/exports.py
--rw-r--r--   0 runner    (1001) docker     (123)    11981 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/django_prometheus/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/django_prometheus/migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/django_prometheus/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:25:31.122952 django-prometheus-2.3.0.dev46/django_prometheus/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/django_prometheus/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/django_prometheus/tests/test_django_prometheus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/django_prometheus/tests/test_exports.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/django_prometheus/tests/test_testutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/django_prometheus/testutils.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/django_prometheus/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/django_prometheus/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:25:31.114952 django-prometheus-2.3.0.dev46/django_prometheus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-05-02 15:25:31.000000 django-prometheus-2.3.0.dev46/django_prometheus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-02 15:25:31.000000 django-prometheus-2.3.0.dev46/django_prometheus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:25:31.000000 django-prometheus-2.3.0.dev46/django_prometheus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-02 15:25:31.000000 django-prometheus-2.3.0.dev46/django_prometheus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-02 15:25:31.000000 django-prometheus-2.3.0.dev46/django_prometheus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-02 15:25:31.122952 django-prometheus-2.3.0.dev46/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-02 15:25:11.000000 django-prometheus-2.3.0.dev46/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:51:24.872580 django-prometheus-2.4.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9361 2023-05-02 15:51:24.872580 django-prometheus-2.4.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:51:24.868580 django-prometheus-2.4.0.dev1/django_prometheus/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-02 15:51:17.000000 django-prometheus-2.4.0.dev1/django_prometheus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/django_prometheus/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:51:24.872580 django-prometheus-2.4.0.dev1/django_prometheus/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/django_prometheus/cache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:51:24.872580 django-prometheus-2.4.0.dev1/django_prometheus/cache/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/django_prometheus/cache/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/django_prometheus/cache/backends/django_memcached_consul.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/django_prometheus/cache/backends/filebased.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/django_prometheus/cache/backends/locmem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/django_prometheus/cache/backends/memcached.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/django_prometheus/cache/backends/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/django_prometheus/cache/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:51:24.872580 django-prometheus-2.4.0.dev1/django_prometheus/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/django_prometheus/conf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:51:24.872580 django-prometheus-2.4.0.dev1/django_prometheus/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/django_prometheus/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:51:24.872580 django-prometheus-2.4.0.dev1/django_prometheus/db/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/django_prometheus/db/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/django_prometheus/db/backends/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:51:24.872580 django-prometheus-2.4.0.dev1/django_prometheus/db/backends/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/django_prometheus/db/backends/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/django_prometheus/db/backends/mysql/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:51:24.872580 django-prometheus-2.4.0.dev1/django_prometheus/db/backends/postgis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/django_prometheus/db/backends/postgis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/django_prometheus/db/backends/postgis/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:51:24.872580 django-prometheus-2.4.0.dev1/django_prometheus/db/backends/postgresql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/django_prometheus/db/backends/postgresql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/django_prometheus/db/backends/postgresql/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:51:24.872580 django-prometheus-2.4.0.dev1/django_prometheus/db/backends/sqlite3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/django_prometheus/db/backends/sqlite3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/django_prometheus/db/backends/sqlite3/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/django_prometheus/db/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/django_prometheus/db/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/django_prometheus/exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11981 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/django_prometheus/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/django_prometheus/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/django_prometheus/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:51:24.872580 django-prometheus-2.4.0.dev1/django_prometheus/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/django_prometheus/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/django_prometheus/tests/test_django_prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/django_prometheus/tests/test_exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/django_prometheus/tests/test_testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/django_prometheus/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/django_prometheus/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/django_prometheus/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:51:24.872580 django-prometheus-2.4.0.dev1/django_prometheus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9361 2023-05-02 15:51:24.000000 django-prometheus-2.4.0.dev1/django_prometheus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-02 15:51:24.000000 django-prometheus-2.4.0.dev1/django_prometheus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:51:24.000000 django-prometheus-2.4.0.dev1/django_prometheus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-02 15:51:24.000000 django-prometheus-2.4.0.dev1/django_prometheus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-02 15:51:24.000000 django-prometheus-2.4.0.dev1/django_prometheus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-02 15:51:24.872580 django-prometheus-2.4.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-02 15:51:06.000000 django-prometheus-2.4.0.dev1/setup.py
```

### Comparing `django-prometheus-2.3.0.dev46/LICENSE` & `django-prometheus-2.4.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev46/PKG-INFO` & `django-prometheus-2.4.0.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-prometheus
-Version: 2.3.0.dev46
+Version: 2.4.0.dev1
 Summary: Django middlewares to monitor your application with Prometheus.io.
 Home-page: http://github.com/korfuri/django-prometheus
 Author: Uriel Corfa
 Author-email: uriel@corfa.fr
 License: Apache
 Project-URL: Changelog, https://github.com/korfuri/django-prometheus/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/korfuri/django-prometheus/blob/master/README.md
```

### Comparing `django-prometheus-2.3.0.dev46/README.md` & `django-prometheus-2.4.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev46/django_prometheus/__init__.py` & `django-prometheus-2.4.0.dev1/django_prometheus/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Import all files that define metrics. This has the effect that
 # `import django_prometheus` will always instantiate all metric
 # objects right away.
 from django_prometheus import middleware, models
 
 __all__ = ["middleware", "models", "pip_prometheus"]
 
-__version__ = "2.3.0.dev46"
+__version__ = "2.4.0.dev1"
 
 
 # Import pip_prometheus to export the pip metrics automatically.
 try:
     import pip_prometheus
 except ImportError:
     # If people don't have pip, don't export anything.
```

### Comparing `django-prometheus-2.3.0.dev46/django_prometheus/apps.py` & `django-prometheus-2.4.0.dev1/django_prometheus/apps.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev46/django_prometheus/cache/backends/django_memcached_consul.py` & `django-prometheus-2.4.0.dev1/django_prometheus/cache/backends/django_memcached_consul.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev46/django_prometheus/cache/backends/filebased.py` & `django-prometheus-2.4.0.dev1/django_prometheus/cache/backends/filebased.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev46/django_prometheus/cache/backends/locmem.py` & `django-prometheus-2.4.0.dev1/django_prometheus/cache/backends/locmem.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev46/django_prometheus/cache/backends/memcached.py` & `django-prometheus-2.4.0.dev1/django_prometheus/cache/backends/memcached.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev46/django_prometheus/cache/backends/redis.py` & `django-prometheus-2.4.0.dev1/django_prometheus/cache/backends/redis.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev46/django_prometheus/cache/metrics.py` & `django-prometheus-2.4.0.dev1/django_prometheus/cache/metrics.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev46/django_prometheus/db/backends/mysql/base.py` & `django-prometheus-2.4.0.dev1/django_prometheus/db/backends/mysql/base.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev46/django_prometheus/db/backends/postgis/base.py` & `django-prometheus-2.4.0.dev1/django_prometheus/db/backends/postgis/base.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev46/django_prometheus/db/backends/postgresql/base.py` & `django-prometheus-2.4.0.dev1/django_prometheus/db/backends/postgresql/base.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev46/django_prometheus/db/common.py` & `django-prometheus-2.4.0.dev1/django_prometheus/db/common.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev46/django_prometheus/db/metrics.py` & `django-prometheus-2.4.0.dev1/django_prometheus/db/metrics.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev46/django_prometheus/exports.py` & `django-prometheus-2.4.0.dev1/django_prometheus/exports.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev46/django_prometheus/middleware.py` & `django-prometheus-2.4.0.dev1/django_prometheus/middleware.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev46/django_prometheus/migrations.py` & `django-prometheus-2.4.0.dev1/django_prometheus/migrations.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev46/django_prometheus/models.py` & `django-prometheus-2.4.0.dev1/django_prometheus/models.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev46/django_prometheus/tests/test_exports.py` & `django-prometheus-2.4.0.dev1/django_prometheus/tests/test_exports.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev46/django_prometheus/tests/test_testutils.py` & `django-prometheus-2.4.0.dev1/django_prometheus/tests/test_testutils.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev46/django_prometheus/testutils.py` & `django-prometheus-2.4.0.dev1/django_prometheus/testutils.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev46/django_prometheus/utils.py` & `django-prometheus-2.4.0.dev1/django_prometheus/utils.py`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev46/django_prometheus.egg-info/PKG-INFO` & `django-prometheus-2.4.0.dev1/django_prometheus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-prometheus
-Version: 2.3.0.dev46
+Version: 2.4.0.dev1
 Summary: Django middlewares to monitor your application with Prometheus.io.
 Home-page: http://github.com/korfuri/django-prometheus
 Author: Uriel Corfa
 Author-email: uriel@corfa.fr
 License: Apache
 Project-URL: Changelog, https://github.com/korfuri/django-prometheus/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/korfuri/django-prometheus/blob/master/README.md
```

### Comparing `django-prometheus-2.3.0.dev46/django_prometheus.egg-info/SOURCES.txt` & `django-prometheus-2.4.0.dev1/django_prometheus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev46/pyproject.toml` & `django-prometheus-2.4.0.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-prometheus-2.3.0.dev46/setup.py` & `django-prometheus-2.4.0.dev1/setup.py`

 * *Files identical despite different names*

