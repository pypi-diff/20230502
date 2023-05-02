# Comparing `tmp/django-rq-2.7.0.tar.gz` & `tmp/django-rq-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-rq-2.7.0.tar", last modified: Tue Feb  7 11:11:02 2023, max compression
+gzip compressed data, was "dist/django-rq-2.8.0.tar", last modified: Tue May  2 03:20:05 2023, max compression
```

## Comparing `django-rq-2.7.0.tar` & `django-rq-2.8.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-02-07 11:11:02.098153 django-rq-2.7.0/
--rw-r--r--   0 selwin     (501) staff       (20)     7630 2023-02-07 11:09:24.000000 django-rq-2.7.0/CHANGELOG.md
--rw-r--r--   0 selwin     (501) staff       (20)     1053 2017-12-06 00:54:06.000000 django-rq-2.7.0/LICENSE.txt
--rw-r--r--   0 selwin     (501) staff       (20)      100 2019-12-07 09:59:35.000000 django-rq-2.7.0/MANIFEST.in
--rw-r--r--   0 selwin     (501) staff       (20)    22395 2023-02-07 11:11:02.098310 django-rq-2.7.0/PKG-INFO
--rw-r--r--   0 selwin     (501) staff       (20)    16837 2023-01-29 01:06:02.000000 django-rq-2.7.0/README.rst
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-02-07 11:11:02.091941 django-rq-2.7.0/django_rq/
--rw-r--r--   0 selwin     (501) staff       (20)      151 2023-02-07 11:10:05.000000 django-rq-2.7.0/django_rq/__init__.py
--rw-r--r--   0 selwin     (501) staff       (20)     1175 2021-11-17 00:53:40.000000 django-rq-2.7.0/django_rq/admin.py
--rw-r--r--   0 selwin     (501) staff       (20)     1163 2020-11-07 03:48:59.000000 django-rq-2.7.0/django_rq/decorators.py
--rw-r--r--   0 selwin     (501) staff       (20)      524 2020-03-31 10:08:21.000000 django-rq-2.7.0/django_rq/jobs.py
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-02-07 11:11:02.092797 django-rq-2.7.0/django_rq/management/
--rw-r--r--   0 selwin     (501) staff       (20)        0 2020-03-08 09:24:48.000000 django-rq-2.7.0/django_rq/management/__init__.py
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-02-07 11:11:02.093766 django-rq-2.7.0/django_rq/management/commands/
--rw-r--r--   0 selwin     (501) staff       (20)        0 2020-03-08 09:24:48.000000 django-rq-2.7.0/django_rq/management/commands/__init__.py
--rw-r--r--   0 selwin     (501) staff       (20)     1060 2022-11-01 13:42:48.000000 django-rq-2.7.0/django_rq/management/commands/rqenqueue.py
--rw-r--r--   0 selwin     (501) staff       (20)     1703 2022-11-01 13:42:48.000000 django-rq-2.7.0/django_rq/management/commands/rqscheduler.py
--rw-r--r--   0 selwin     (501) staff       (20)     3033 2020-03-31 10:08:21.000000 django-rq-2.7.0/django_rq/management/commands/rqstats.py
--rw-r--r--   0 selwin     (501) staff       (20)     5407 2022-11-01 13:51:04.000000 django-rq-2.7.0/django_rq/management/commands/rqworker.py
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-02-07 11:11:02.094165 django-rq-2.7.0/django_rq/migrations/
--rw-r--r--   0 selwin     (501) staff       (20)      967 2021-11-17 00:53:40.000000 django-rq-2.7.0/django_rq/migrations/0001_initial.py
--rw-r--r--   0 selwin     (501) staff       (20)        0 2021-11-17 00:53:40.000000 django-rq-2.7.0/django_rq/migrations/__init__.py
--rw-r--r--   0 selwin     (501) staff       (20)      668 2021-11-17 00:53:40.000000 django-rq-2.7.0/django_rq/models.py
--rw-r--r--   0 selwin     (501) staff       (20)    10481 2022-11-01 15:38:52.000000 django-rq-2.7.0/django_rq/queues.py
--rw-r--r--   0 selwin     (501) staff       (20)      877 2020-03-08 09:24:48.000000 django-rq-2.7.0/django_rq/settings.py
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-02-07 11:11:02.088003 django-rq-2.7.0/django_rq/templates/
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-02-07 11:11:02.095842 django-rq-2.7.0/django_rq/templates/django_rq/
--rw-r--r--   0 selwin     (501) staff       (20)     1098 2020-03-08 09:24:48.000000 django-rq-2.7.0/django_rq/templates/django_rq/clear_queue.html
--rw-r--r--   0 selwin     (501) staff       (20)     1642 2020-11-08 03:24:12.000000 django-rq-2.7.0/django_rq/templates/django_rq/confirm_action.html
--rw-r--r--   0 selwin     (501) staff       (20)     1260 2020-03-08 09:24:48.000000 django-rq-2.7.0/django_rq/templates/django_rq/delete_job.html
--rw-r--r--   0 selwin     (501) staff       (20)     7833 2023-01-29 01:06:02.000000 django-rq-2.7.0/django_rq/templates/django_rq/job_detail.html
--rw-r--r--   0 selwin     (501) staff       (20)     6559 2022-11-05 01:59:59.000000 django-rq-2.7.0/django_rq/templates/django_rq/jobs.html
--rw-r--r--   0 selwin     (501) staff       (20)     1156 2020-03-08 09:24:48.000000 django-rq-2.7.0/django_rq/templates/django_rq/requeue_all.html
--rw-r--r--   0 selwin     (501) staff       (20)     3482 2020-03-31 10:08:21.000000 django-rq-2.7.0/django_rq/templates/django_rq/stats.html
--rw-r--r--   0 selwin     (501) staff       (20)        3 2020-03-08 09:24:48.000000 django-rq-2.7.0/django_rq/templates/django_rq/test.html
--rw-r--r--   0 selwin     (501) staff       (20)     3353 2020-11-08 03:24:20.000000 django-rq-2.7.0/django_rq/templates/django_rq/worker_details.html
--rw-r--r--   0 selwin     (501) staff       (20)     2871 2020-11-08 03:24:12.000000 django-rq-2.7.0/django_rq/templates/django_rq/workers.html
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-02-07 11:11:02.096236 django-rq-2.7.0/django_rq/templatetags/
--rw-r--r--   0 selwin     (501) staff       (20)        0 2020-03-08 09:24:48.000000 django-rq-2.7.0/django_rq/templatetags/__init__.py
--rw-r--r--   0 selwin     (501) staff       (20)      646 2021-11-17 00:53:40.000000 django-rq-2.7.0/django_rq/templatetags/django_rq.py
--rw-r--r--   0 selwin     (501) staff       (20)      152 2022-11-01 13:42:48.000000 django-rq-2.7.0/django_rq/templatetags/jquery_path.py
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-02-07 11:11:02.098016 django-rq-2.7.0/django_rq/tests/
--rw-r--r--   0 selwin     (501) staff       (20)        0 2020-03-08 09:24:48.000000 django-rq-2.7.0/django_rq/tests/__init__.py
--rw-r--r--   0 selwin     (501) staff       (20)      491 2022-11-05 01:59:59.000000 django-rq-2.7.0/django_rq/tests/fixtures.py
--rw-r--r--   0 selwin     (501) staff       (20)     5296 2022-11-01 15:39:41.000000 django-rq-2.7.0/django_rq/tests/settings.py
--rw-r--r--   0 selwin     (501) staff       (20)    14459 2022-11-05 01:59:59.000000 django-rq-2.7.0/django_rq/tests/test_views.py
--rw-r--r--   0 selwin     (501) staff       (20)    31856 2022-11-05 01:48:37.000000 django-rq-2.7.0/django_rq/tests/tests.py
--rw-r--r--   0 selwin     (501) staff       (20)      335 2020-03-31 10:08:21.000000 django-rq-2.7.0/django_rq/tests/urls.py
--rw-r--r--   0 selwin     (501) staff       (20)      548 2020-03-08 09:24:48.000000 django-rq-2.7.0/django_rq/tests/utils.py
--rw-r--r--   0 selwin     (501) staff       (20)      334 2020-03-08 09:24:48.000000 django-rq-2.7.0/django_rq/tests/views.py
--rw-r--r--   0 selwin     (501) staff       (20)     1149 2022-11-01 13:51:04.000000 django-rq-2.7.0/django_rq/thread_queue.py
--rw-r--r--   0 selwin     (501) staff       (20)     2123 2020-11-08 03:24:12.000000 django-rq-2.7.0/django_rq/urls.py
--rw-r--r--   0 selwin     (501) staff       (20)     3192 2020-03-31 10:08:21.000000 django-rq-2.7.0/django_rq/utils.py
--rw-r--r--   0 selwin     (501) staff       (20)    16242 2023-01-29 01:06:02.000000 django-rq-2.7.0/django_rq/views.py
--rw-r--r--   0 selwin     (501) staff       (20)     1796 2020-03-31 10:08:21.000000 django-rq-2.7.0/django_rq/workers.py
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-02-07 11:11:02.092682 django-rq-2.7.0/django_rq.egg-info/
--rw-r--r--   0 selwin     (501) staff       (20)    22395 2023-02-07 11:11:02.000000 django-rq-2.7.0/django_rq.egg-info/PKG-INFO
--rw-r--r--   0 selwin     (501) staff       (20)     1598 2023-02-07 11:11:02.000000 django-rq-2.7.0/django_rq.egg-info/SOURCES.txt
--rw-r--r--   0 selwin     (501) staff       (20)        1 2023-02-07 11:11:02.000000 django-rq-2.7.0/django_rq.egg-info/dependency_links.txt
--rw-r--r--   0 selwin     (501) staff       (20)        1 2017-12-06 07:07:26.000000 django-rq-2.7.0/django_rq.egg-info/not-zip-safe
--rw-r--r--   0 selwin     (501) staff       (20)       75 2023-02-07 11:11:02.000000 django-rq-2.7.0/django_rq.egg-info/requires.txt
--rw-r--r--   0 selwin     (501) staff       (20)       10 2023-02-07 11:11:02.000000 django-rq-2.7.0/django_rq.egg-info/top_level.txt
--rw-r--r--   0 selwin     (501) staff       (20)       67 2023-02-07 11:11:02.098554 django-rq-2.7.0/setup.cfg
--rw-r--r--   0 selwin     (501) staff       (20)     1416 2023-02-07 11:09:52.000000 django-rq-2.7.0/setup.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-02 03:20:05.308218 django-rq-2.8.0/
+-rw-r--r--   0 selwin     (501) staff       (20)     7937 2023-05-02 03:15:45.000000 django-rq-2.8.0/CHANGELOG.md
+-rw-r--r--   0 selwin     (501) staff       (20)     1053 2017-12-06 00:54:06.000000 django-rq-2.8.0/LICENSE.txt
+-rw-r--r--   0 selwin     (501) staff       (20)      100 2019-12-07 09:59:35.000000 django-rq-2.8.0/MANIFEST.in
+-rw-r--r--   0 selwin     (501) staff       (20)    22989 2023-05-02 03:20:05.308385 django-rq-2.8.0/PKG-INFO
+-rw-r--r--   0 selwin     (501) staff       (20)    17351 2023-05-02 03:15:57.000000 django-rq-2.8.0/README.rst
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-02 03:20:05.300553 django-rq-2.8.0/django_rq/
+-rw-r--r--   0 selwin     (501) staff       (20)      151 2023-05-02 03:17:58.000000 django-rq-2.8.0/django_rq/__init__.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1174 2023-05-02 02:24:10.000000 django-rq-2.8.0/django_rq/admin.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1162 2023-05-02 02:24:10.000000 django-rq-2.8.0/django_rq/decorators.py
+-rw-r--r--   0 selwin     (501) staff       (20)      524 2023-02-07 11:14:52.000000 django-rq-2.8.0/django_rq/jobs.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-02 03:20:05.301658 django-rq-2.8.0/django_rq/management/
+-rw-r--r--   0 selwin     (501) staff       (20)        0 2020-03-08 09:24:48.000000 django-rq-2.8.0/django_rq/management/__init__.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-02 03:20:05.302733 django-rq-2.8.0/django_rq/management/commands/
+-rw-r--r--   0 selwin     (501) staff       (20)        0 2020-03-08 09:24:48.000000 django-rq-2.8.0/django_rq/management/commands/__init__.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1060 2022-11-01 13:42:48.000000 django-rq-2.8.0/django_rq/management/commands/rqenqueue.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1703 2022-11-01 13:42:48.000000 django-rq-2.8.0/django_rq/management/commands/rqscheduler.py
+-rw-r--r--   0 selwin     (501) staff       (20)     3033 2020-03-31 10:08:21.000000 django-rq-2.8.0/django_rq/management/commands/rqstats.py
+-rw-r--r--   0 selwin     (501) staff       (20)     5681 2023-05-02 02:24:10.000000 django-rq-2.8.0/django_rq/management/commands/rqworker.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-02 03:20:05.303103 django-rq-2.8.0/django_rq/migrations/
+-rw-r--r--   0 selwin     (501) staff       (20)      967 2021-11-17 00:53:40.000000 django-rq-2.8.0/django_rq/migrations/0001_initial.py
+-rw-r--r--   0 selwin     (501) staff       (20)        0 2021-11-17 00:53:40.000000 django-rq-2.8.0/django_rq/migrations/__init__.py
+-rw-r--r--   0 selwin     (501) staff       (20)      667 2023-05-02 02:24:10.000000 django-rq-2.8.0/django_rq/models.py
+-rw-r--r--   0 selwin     (501) staff       (20)    10687 2023-05-02 02:24:10.000000 django-rq-2.8.0/django_rq/queues.py
+-rw-r--r--   0 selwin     (501) staff       (20)      877 2023-02-07 11:14:43.000000 django-rq-2.8.0/django_rq/settings.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-02 03:20:05.294806 django-rq-2.8.0/django_rq/templates/
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-02 03:20:05.305148 django-rq-2.8.0/django_rq/templates/django_rq/
+-rw-r--r--   0 selwin     (501) staff       (20)     1098 2020-03-08 09:24:48.000000 django-rq-2.8.0/django_rq/templates/django_rq/clear_queue.html
+-rw-r--r--   0 selwin     (501) staff       (20)     1642 2020-11-08 03:24:12.000000 django-rq-2.8.0/django_rq/templates/django_rq/confirm_action.html
+-rw-r--r--   0 selwin     (501) staff       (20)     1260 2020-03-08 09:24:48.000000 django-rq-2.8.0/django_rq/templates/django_rq/delete_job.html
+-rw-r--r--   0 selwin     (501) staff       (20)     7833 2023-01-29 01:06:02.000000 django-rq-2.8.0/django_rq/templates/django_rq/job_detail.html
+-rw-r--r--   0 selwin     (501) staff       (20)     6559 2022-11-05 01:59:59.000000 django-rq-2.8.0/django_rq/templates/django_rq/jobs.html
+-rw-r--r--   0 selwin     (501) staff       (20)     1156 2020-03-08 09:24:48.000000 django-rq-2.8.0/django_rq/templates/django_rq/requeue_all.html
+-rw-r--r--   0 selwin     (501) staff       (20)     3810 2023-05-02 02:24:10.000000 django-rq-2.8.0/django_rq/templates/django_rq/stats.html
+-rw-r--r--   0 selwin     (501) staff       (20)        3 2020-03-08 09:24:48.000000 django-rq-2.8.0/django_rq/templates/django_rq/test.html
+-rw-r--r--   0 selwin     (501) staff       (20)     3353 2020-11-08 03:24:20.000000 django-rq-2.8.0/django_rq/templates/django_rq/worker_details.html
+-rw-r--r--   0 selwin     (501) staff       (20)     2871 2020-11-08 03:24:12.000000 django-rq-2.8.0/django_rq/templates/django_rq/workers.html
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-02 03:20:05.305504 django-rq-2.8.0/django_rq/templatetags/
+-rw-r--r--   0 selwin     (501) staff       (20)        0 2020-03-08 09:24:48.000000 django-rq-2.8.0/django_rq/templatetags/__init__.py
+-rw-r--r--   0 selwin     (501) staff       (20)      646 2021-11-17 00:53:40.000000 django-rq-2.8.0/django_rq/templatetags/django_rq.py
+-rw-r--r--   0 selwin     (501) staff       (20)      152 2022-11-01 13:42:48.000000 django-rq-2.8.0/django_rq/templatetags/jquery_path.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-02 03:20:05.307974 django-rq-2.8.0/django_rq/tests/
+-rw-r--r--   0 selwin     (501) staff       (20)        0 2020-03-08 09:24:48.000000 django-rq-2.8.0/django_rq/tests/__init__.py
+-rw-r--r--   0 selwin     (501) staff       (20)      493 2023-05-02 02:24:10.000000 django-rq-2.8.0/django_rq/tests/fixtures.py
+-rw-r--r--   0 selwin     (501) staff       (20)     5813 2023-05-02 03:15:57.000000 django-rq-2.8.0/django_rq/tests/settings.py
+-rw-r--r--   0 selwin     (501) staff       (20)    14477 2023-05-02 03:15:57.000000 django-rq-2.8.0/django_rq/tests/test_views.py
+-rw-r--r--   0 selwin     (501) staff       (20)    36067 2023-05-02 02:24:10.000000 django-rq-2.8.0/django_rq/tests/tests.py
+-rw-r--r--   0 selwin     (501) staff       (20)      335 2023-05-02 02:24:10.000000 django-rq-2.8.0/django_rq/tests/urls.py
+-rw-r--r--   0 selwin     (501) staff       (20)      548 2023-02-07 11:15:20.000000 django-rq-2.8.0/django_rq/tests/utils.py
+-rw-r--r--   0 selwin     (501) staff       (20)      334 2023-02-07 11:15:18.000000 django-rq-2.8.0/django_rq/tests/views.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1148 2023-05-02 02:24:10.000000 django-rq-2.8.0/django_rq/thread_queue.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1937 2023-05-02 02:24:10.000000 django-rq-2.8.0/django_rq/urls.py
+-rw-r--r--   0 selwin     (501) staff       (20)     4450 2023-05-02 02:24:10.000000 django-rq-2.8.0/django_rq/utils.py
+-rw-r--r--   0 selwin     (501) staff       (20)    16450 2023-05-02 03:15:57.000000 django-rq-2.8.0/django_rq/views.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1689 2023-05-02 02:24:10.000000 django-rq-2.8.0/django_rq/workers.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-02 03:20:05.301555 django-rq-2.8.0/django_rq.egg-info/
+-rw-r--r--   0 selwin     (501) staff       (20)    22989 2023-05-02 03:20:05.000000 django-rq-2.8.0/django_rq.egg-info/PKG-INFO
+-rw-r--r--   0 selwin     (501) staff       (20)     1598 2023-05-02 03:20:05.000000 django-rq-2.8.0/django_rq.egg-info/SOURCES.txt
+-rw-r--r--   0 selwin     (501) staff       (20)        1 2023-05-02 03:20:05.000000 django-rq-2.8.0/django_rq.egg-info/dependency_links.txt
+-rw-r--r--   0 selwin     (501) staff       (20)        1 2017-12-06 07:07:26.000000 django-rq-2.8.0/django_rq.egg-info/not-zip-safe
+-rw-r--r--   0 selwin     (501) staff       (20)       75 2023-05-02 03:20:05.000000 django-rq-2.8.0/django_rq.egg-info/requires.txt
+-rw-r--r--   0 selwin     (501) staff       (20)       10 2023-05-02 03:20:05.000000 django-rq-2.8.0/django_rq.egg-info/top_level.txt
+-rw-r--r--   0 selwin     (501) staff       (20)       67 2023-05-02 03:20:05.308648 django-rq-2.8.0/setup.cfg
+-rw-r--r--   0 selwin     (501) staff       (20)     1416 2023-05-02 03:17:48.000000 django-rq-2.8.0/setup.py
```

### Comparing `django-rq-2.7.0/CHANGELOG.md` & `django-rq-2.8.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+# Version 2.8.0 (2023-05-02)
+* Support for RQ 1.14. Thanks @Cerebro92 and @selwin!
+* Show scheduler PID information in admin interface. Thanks @gabriels1234!
+* Added `serializer` argument to `rqworker` command. Thanks @gabriels1234!
+* Added `USERNAME` and `SENTINEL_KWARGS` support. Thanks @joachimBurket!
+
 # Version 2.7.0 (2023-02-07)
 * Able to show multiple execution results for each job (requires RQ v1.12). Thanks @selwin!
 * Various admin interface improvements. Thanks @selwin!
 
 # Version 2.6.0 (2022-11-05)
 * Added `--max-jobs` argument to `rqworker` management command. Thanks @arpit-goel!
 * Remove job from `ScheduledJobRegistry` if a scheduled job is enqueued from admin. Thanks @robertaistleitner!
```

### Comparing `django-rq-2.7.0/LICENSE.txt` & `django-rq-2.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-rq-2.7.0/PKG-INFO` & `django-rq-2.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-rq
-Version: 2.7.0
+Version: 2.8.0
 Summary: An app that provides django integration for RQ (Redis Queue)
 Home-page: https://github.com/rq/django-rq
 Author: Selwin Ong
 Author-email: selwin.ong@gmail.com
 License: MIT
 Description: =========
         Django-RQ
@@ -54,25 +54,36 @@
         .. code-block:: python
         
             RQ_QUEUES = {
                 'default': {
                     'HOST': 'localhost',
                     'PORT': 6379,
                     'DB': 0,
+                    'USERNAME': 'some-user',
                     'PASSWORD': 'some-password',
                     'DEFAULT_TIMEOUT': 360,
+                    'REDIS_CLIENT_KWARGS': {    # Eventual additional Redis connection arguments
+                        'ssl_cert_reqs': None,
+                    },
                 },
                 'with-sentinel': {
                     'SENTINELS': [('localhost', 26736), ('localhost', 26737)],
                     'MASTER_NAME': 'redismaster',
                     'DB': 0,
+                    # Redis username/password
+                    'USERNAME': 'redis-user',
                     'PASSWORD': 'secret',
-                    'SOCKET_TIMEOUT': None,
-                    'CONNECTION_KWARGS': {
-                        'socket_connect_timeout': 0.3
+                    'SOCKET_TIMEOUT': 0.3,
+                    'CONNECTION_KWARGS': {  # Eventual additional Redis connection arguments
+                        'ssl': True
+                    }
+                    'SENTINEL_KWARGS': {    # Eventual Sentinel connection arguments
+                        # If Sentinel also has auth, username/password can be passed here
+                        'username': 'sentinel-user',
+                        'password': 'secret',
                     },
                 },
                 'high': {
                     'URL': os.getenv('REDISTOGO_URL', 'redis://localhost:6379/0'), # If you're on Heroku
                     'DEFAULT_TIMEOUT': 500,
                 },
                 'low': {
@@ -354,16 +365,15 @@
                 'integrations': [RedisIntegration(), RqIntegration(), DjangoIntegration()]
             }
         
         
         Configuring Logging
         -------------------
         
-        Starting from version 0.3.3, RQ uses Python's ``logging``, this means
-        you can easily configure ``rqworker``'s logging mechanism in django's
+        RQ uses Python's ``logging``, this means you can easily configure ``rqworker``'s logging mechanism in django's
         ``settings.py``. For example:
         
         .. code-block:: python
         
             LOGGING = {
                 "version": 1,
                 "disable_existing_loggers": False,
@@ -372,15 +382,15 @@
                         "format": "%(asctime)s %(message)s",
                         "datefmt": "%H:%M:%S",
                     },
                 },
                 "handlers": {
                     "rq_console": {
                         "level": "DEBUG",
-                        "class": "rq.utils.ColorizingStreamHandler",
+                        "class": "rq.logutils.ColorizingStreamHandler",
                         "formatter": "rq_console",
                         "exclude": ["%(asctime)s"],
                     },
                     # If you use sentry for logging
                     'sentry': {
                         'level': 'ERROR',
                         'class': 'raven.contrib.django.handlers.SentryHandler',
@@ -497,15 +507,15 @@
         
         =============
         Running Tests
         =============
         
         To run ``django_rq``'s test suite::
         
-            `which django-admin.py` test django_rq --settings=django_rq.tests.settings --pythonpath=.
+            `which django-admin` test django_rq --settings=django_rq.tests.settings --pythonpath=.
         
         ===================
         Deploying on Ubuntu
         ===================
         
         Create an rqworker service that runs the high, default, and low queues.
```

### Comparing `django-rq-2.7.0/README.rst` & `django-rq-2.8.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -46,25 +46,36 @@
 .. code-block:: python
 
     RQ_QUEUES = {
         'default': {
             'HOST': 'localhost',
             'PORT': 6379,
             'DB': 0,
+            'USERNAME': 'some-user',
             'PASSWORD': 'some-password',
             'DEFAULT_TIMEOUT': 360,
+            'REDIS_CLIENT_KWARGS': {    # Eventual additional Redis connection arguments
+                'ssl_cert_reqs': None,
+            },
         },
         'with-sentinel': {
             'SENTINELS': [('localhost', 26736), ('localhost', 26737)],
             'MASTER_NAME': 'redismaster',
             'DB': 0,
+            # Redis username/password
+            'USERNAME': 'redis-user',
             'PASSWORD': 'secret',
-            'SOCKET_TIMEOUT': None,
-            'CONNECTION_KWARGS': {
-                'socket_connect_timeout': 0.3
+            'SOCKET_TIMEOUT': 0.3,
+            'CONNECTION_KWARGS': {  # Eventual additional Redis connection arguments
+                'ssl': True
+            }
+            'SENTINEL_KWARGS': {    # Eventual Sentinel connection arguments
+                # If Sentinel also has auth, username/password can be passed here
+                'username': 'sentinel-user',
+                'password': 'secret',
             },
         },
         'high': {
             'URL': os.getenv('REDISTOGO_URL', 'redis://localhost:6379/0'), # If you're on Heroku
             'DEFAULT_TIMEOUT': 500,
         },
         'low': {
@@ -346,16 +357,15 @@
         'integrations': [RedisIntegration(), RqIntegration(), DjangoIntegration()]
     }
 
 
 Configuring Logging
 -------------------
 
-Starting from version 0.3.3, RQ uses Python's ``logging``, this means
-you can easily configure ``rqworker``'s logging mechanism in django's
+RQ uses Python's ``logging``, this means you can easily configure ``rqworker``'s logging mechanism in django's
 ``settings.py``. For example:
 
 .. code-block:: python
 
     LOGGING = {
         "version": 1,
         "disable_existing_loggers": False,
@@ -364,15 +374,15 @@
                 "format": "%(asctime)s %(message)s",
                 "datefmt": "%H:%M:%S",
             },
         },
         "handlers": {
             "rq_console": {
                 "level": "DEBUG",
-                "class": "rq.utils.ColorizingStreamHandler",
+                "class": "rq.logutils.ColorizingStreamHandler",
                 "formatter": "rq_console",
                 "exclude": ["%(asctime)s"],
             },
             # If you use sentry for logging
             'sentry': {
                 'level': 'ERROR',
                 'class': 'raven.contrib.django.handlers.SentryHandler',
@@ -489,15 +499,15 @@
 
 =============
 Running Tests
 =============
 
 To run ``django_rq``'s test suite::
 
-    `which django-admin.py` test django_rq --settings=django_rq.tests.settings --pythonpath=.
+    `which django-admin` test django_rq --settings=django_rq.tests.settings --pythonpath=.
 
 ===================
 Deploying on Ubuntu
 ===================
 
 Create an rqworker service that runs the high, default, and low queues.
```

### Comparing `django-rq-2.7.0/django_rq/admin.py` & `django-rq-2.8.0/django_rq/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from django.contrib import admin
 
 from . import views, settings, models
 
 
 class QueueAdmin(admin.ModelAdmin):
-    """ Admin View for Django-RQ Queue """
+    """Admin View for Django-RQ Queue"""
+
     def has_add_permission(self, request):
         return False  # Hide the admin "+ Add" link for Queues
 
     def has_change_permission(self, request):
         return True
 
     def has_module_permission(self, request):
```

### Comparing `django-rq-2.7.0/django_rq/decorators.py` & `django-rq-2.8.0/django_rq/decorators.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,8 +36,7 @@
     if default_result_ttl is not None:
         kwargs.setdefault('result_ttl', default_result_ttl)
 
     decorator = _rq_job(queue, connection=connection, *args, **kwargs)
     if func:
         return decorator(func)
     return decorator
-
```

### Comparing `django-rq-2.7.0/django_rq/jobs.py` & `django-rq-2.8.0/django_rq/jobs.py`

 * *Files identical despite different names*

### Comparing `django-rq-2.7.0/django_rq/management/commands/rqenqueue.py` & `django-rq-2.8.0/django_rq/management/commands/rqenqueue.py`

 * *Files identical despite different names*

### Comparing `django-rq-2.7.0/django_rq/management/commands/rqscheduler.py` & `django-rq-2.8.0/django_rq/management/commands/rqscheduler.py`

 * *Files identical despite different names*

### Comparing `django-rq-2.7.0/django_rq/management/commands/rqstats.py` & `django-rq-2.8.0/django_rq/management/commands/rqstats.py`

 * *Files identical despite different names*

### Comparing `django-rq-2.7.0/django_rq/management/commands/rqworker.py` & `django-rq-2.8.0/django_rq/management/commands/rqworker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import sys
 
 from redis.exceptions import ConnectionError
-from rq import use_connection
+from rq import Connection
 from rq.logutils import setup_loghandlers
 
 from django.core.management.base import BaseCommand
 from django.db import connections
 
 from ...workers import get_worker
 
@@ -77,14 +77,16 @@
                             help='Report exceptions to this Sentry DSN')
         parser.add_argument('--sentry-ca-certs', action='store', default=None, dest='sentry_ca_certs',
                             help='A path to an alternative CA bundle file in PEM-format')
         parser.add_argument('--sentry-debug', action='store', default=False, dest='sentry_debug',
                             help='Turns debug mode on or off.')
         parser.add_argument('--max-jobs', action='store', default=None, dest='max_jobs', type=int,
                             help='Maximum number of jobs to execute')
+        parser.add_argument('--serializer', action='store', default='rq.serializers.DefaultSerializer', dest='serializer',
+                            help='Specify a custom Serializer.')
         parser.add_argument('args', nargs='*', type=str,
                             help='The queues to work on, separated by space')
 
     def handle(self, *args, **options):
         pid = options.get('pid')
         if pid:
             with open(os.path.expanduser(pid), "w") as fp:
@@ -112,23 +114,24 @@
             # Instantiate a worker
             worker_kwargs = {
                 'worker_class': options['worker_class'],
                 'queue_class': options['queue_class'],
                 'job_class': options['job_class'],
                 'name': options['name'],
                 'default_worker_ttl': options['worker_ttl'],
+                'serializer': options['serializer']
             }
             w = get_worker(*args, **worker_kwargs)
 
-            # Call use_connection to push the redis connection into LocalStack
+            # Call Connection context manager to push the redis connection into LocalStack
             # without this, jobs using RQ's get_current_job() will fail
-            use_connection(w.connection)
-            # Close any opened DB connection before any fork
-            reset_db_connections()
-
-            w.work(
-                burst=options.get('burst', False), with_scheduler=options.get('with_scheduler', False),
-                logging_level=level, max_jobs=options['max_jobs']
-            )
+            with Connection(w.connection):
+                # Close any opened DB connection before any fork
+                reset_db_connections()
+
+                w.work(
+                    burst=options.get('burst', False), with_scheduler=options.get('with_scheduler', False),
+                    logging_level=level, max_jobs=options['max_jobs']
+                )
         except ConnectionError as e:
             self.stderr.write(str(e))
             sys.exit(1)
```

### Comparing `django-rq-2.7.0/django_rq/migrations/0001_initial.py` & `django-rq-2.8.0/django_rq/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-rq-2.7.0/django_rq/models.py` & `django-rq-2.8.0/django_rq/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,12 +9,11 @@
     request_finished.connect(thread_queue.commit)
     got_request_exception.connect(thread_queue.clear)
 
 
 class Queue(models.Model):
     """Placeholder model with no database table, but with django admin page
     and contenttype permission"""
-
     class Meta:
         managed = False  # not in Django's database
         default_permissions = ()
         permissions = [['view', 'Access admin page']]
```

### Comparing `django-rq-2.7.0/django_rq/queues.py` & `django-rq-2.8.0/django_rq/queues.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,44 +86,48 @@
         else:
             return redis_cls.from_url(
                 config['URL'],
                 db=config.get('DB'),
             )
 
     if 'USE_REDIS_CACHE' in config.keys():
-
         try:
             # Assume that we're using django-redis
             from django_redis import get_redis_connection as get_redis
+
             return get_redis(config['USE_REDIS_CACHE'])
         except ImportError:
             pass
 
         from django.core.cache import caches
+
         cache = caches[config['USE_REDIS_CACHE']]
         # We're using django-redis-cache
         try:
             return cache._client
         except AttributeError:
             # For django-redis-cache > 0.13.1
             return cache.get_master_client()
 
     if 'UNIX_SOCKET_PATH' in config:
         return redis_cls(unix_socket_path=config['UNIX_SOCKET_PATH'], db=config['DB'])
 
     if 'SENTINELS' in config:
-        sentinel_kwargs = {
+        connection_kwargs = {
             'db': config.get('DB'),
             'password': config.get('PASSWORD'),
+            'username': config.get('USERNAME'),
             'socket_timeout': config.get('SOCKET_TIMEOUT'),
         }
-        sentinel_kwargs.update(config.get('CONNECTION_KWARGS', {}))
-        sentinel = Sentinel(config['SENTINELS'], **sentinel_kwargs)
+        connection_kwargs.update(config.get('CONNECTION_KWARGS', {}))
+        sentinel_kwargs = config.get('SENTINEL_KWARGS', {})
+        sentinel = Sentinel(config['SENTINELS'], sentinel_kwargs=sentinel_kwargs, **connection_kwargs)
         return sentinel.master_for(
-            service_name=config['MASTER_NAME'], redis_class=redis_cls,
+            service_name=config['MASTER_NAME'],
+            redis_class=redis_cls,
         )
 
     return redis_cls(
         host=config['HOST'],
         port=config['PORT'],
         db=config.get('DB', 0),
         username=config.get('USERNAME', None),
@@ -135,19 +139,28 @@
 
 
 def get_connection(name='default', use_strict_redis=False):
     """
     Returns a Redis connection to use based on parameters in settings.RQ_QUEUES
     """
     from .settings import QUEUES
+
     return get_redis_connection(QUEUES[name], use_strict_redis)
 
 
-def get_queue(name='default', default_timeout=None, is_async=None,
-              autocommit=None, connection=None, queue_class=None, job_class=None, **kwargs):
+def get_queue(
+    name='default',
+    default_timeout=None,
+    is_async=None,
+    autocommit=None,
+    connection=None,
+    queue_class=None,
+    job_class=None,
+    **kwargs
+):
     """
     Returns an rq Queue using parameters defined in ``RQ_QUEUES``
     """
     from .settings import QUEUES
 
     if kwargs.get('async') is not None:
         is_async = kwargs['async']
@@ -160,43 +173,59 @@
     job_class = get_job_class(job_class)
 
     if default_timeout is None:
         default_timeout = QUEUES[name].get('DEFAULT_TIMEOUT')
     if connection is None:
         connection = get_connection(name)
     queue_class = get_queue_class(QUEUES[name], queue_class)
-    return queue_class(name, default_timeout=default_timeout,
-                       connection=connection, is_async=is_async,
-                       job_class=job_class, autocommit=autocommit, **kwargs)
+    return queue_class(
+        name,
+        default_timeout=default_timeout,
+        connection=connection,
+        is_async=is_async,
+        job_class=job_class,
+        autocommit=autocommit,
+        **kwargs
+    )
 
 
 def get_queue_by_index(index):
     """
     Returns an rq Queue using parameters defined in ``QUEUES_LIST``
     """
     from .settings import QUEUES_LIST
+
     config = QUEUES_LIST[int(index)]
     return get_queue_class(config)(
-        config['name'],
-        connection=get_redis_connection(config['connection_config']),
-        is_async=config.get('ASYNC', True))
+        config['name'], connection=get_redis_connection(config['connection_config']), is_async=config.get('ASYNC', True)
+    )
 
 
 def filter_connection_params(queue_params):
     """
     Filters the queue params to keep only the connection related params.
     """
-    CONNECTION_PARAMS = ('URL', 'DB', 'USE_REDIS_CACHE',
-                         'UNIX_SOCKET_PATH', 'HOST', 'PORT', 'PASSWORD',
-                         'SENTINELS', 'MASTER_NAME', 'SOCKET_TIMEOUT',
-                         'SSL', 'CONNECTION_KWARGS',)
+    CONNECTION_PARAMS = (
+        'URL',
+        'DB',
+        'USE_REDIS_CACHE',
+        'UNIX_SOCKET_PATH',
+        'HOST',
+        'PORT',
+        'PASSWORD',
+        'SENTINELS',
+        'MASTER_NAME',
+        'SOCKET_TIMEOUT',
+        'SSL',
+        'CONNECTION_KWARGS',
+    )
 
-    #return {p:v for p,v in queue_params.items() if p in CONNECTION_PARAMS}
+    # return {p:v for p,v in queue_params.items() if p in CONNECTION_PARAMS}
     # Dict comprehension compatible with python 2.6
-    return dict((p,v) for (p,v) in queue_params.items() if p in CONNECTION_PARAMS)
+    return dict((p, v) for (p, v) in queue_params.items() if p in CONNECTION_PARAMS)
 
 
 def get_queues(*queue_names, **kwargs):
     """
     Return queue instances from specified queue names.
     All instances must use the same Redis connection.
     """
@@ -218,20 +247,22 @@
     # do consistency checks while building return list
     for name in queue_names[1:]:
         queue = get_queue(name, **kwargs)
         if type(queue) is not type(queues[0]):
             raise ValueError(
                 'Queues must have the same class.'
                 '"{0}" and "{1}" have '
-                'different classes'.format(name, queue_names[0]))
+                'different classes'.format(name, queue_names[0])
+            )
         if connection_params != filter_connection_params(QUEUES[name]):
             raise ValueError(
                 'Queues must have the same redis connection.'
                 '"{0}" and "{1}" have '
-                'different connections'.format(name, queue_names[0]))
+                'different connections'.format(name, queue_names[0])
+            )
         queues.append(queue)
 
     return queues
 
 
 def enqueue(func, *args, **kwargs):
     """
@@ -245,14 +276,15 @@
 
 def get_unique_connection_configs(config=None):
     """
     Returns a list of unique Redis connections from config
     """
     if config is None:
         from .settings import QUEUES
+
         config = QUEUES
 
     connection_configs = []
     for key, value in config.items():
         value = filter_connection_params(value)
         if value not in connection_configs:
             connection_configs.append(value)
@@ -268,40 +300,42 @@
     from rq_scheduler import Scheduler
 
     class DjangoScheduler(Scheduler):
         """
         Use settings ``DEFAULT_RESULT_TTL`` from ``RQ``
         and ``DEFAULT_TIMEOUT`` from ``RQ_QUEUES`` if configured.
         """
+
         def _create_job(self, *args, **kwargs):
             from .settings import QUEUES
 
             if kwargs.get('timeout') is None:
                 queue_name = kwargs.get('queue_name') or self.queue_name
                 kwargs['timeout'] = QUEUES[queue_name].get('DEFAULT_TIMEOUT')
 
             if kwargs.get('result_ttl') is None:
                 kwargs['result_ttl'] = getattr(settings, 'RQ', {}).get('DEFAULT_RESULT_TTL')
 
             return super(DjangoScheduler, self)._create_job(*args, **kwargs)
 
-
     def get_scheduler(name='default', queue=None, interval=60):
         """
         Returns an RQ Scheduler instance using parameters defined in
         ``RQ_QUEUES``
         """
         RQ = getattr(settings, 'RQ', {})
         scheduler_class = RQ.get('SCHEDULER_CLASS', DjangoScheduler)
 
         if isinstance(scheduler_class, str):
             scheduler_class = import_attribute(scheduler_class)
 
         if queue is None:
             queue = get_queue(name)
 
-        return scheduler_class(queue_name=name, interval=interval,
-                               queue=queue, job_class=queue.job_class,
-                               connection=get_connection(name))
+        return scheduler_class(
+            queue_name=name, interval=interval, queue=queue, job_class=queue.job_class, connection=get_connection(name)
+        )
+
 except ImportError:
+
     def get_scheduler(*args, **kwargs):
         raise ImproperlyConfigured('rq_scheduler not installed')
```

### Comparing `django-rq-2.7.0/django_rq/settings.py` & `django-rq-2.8.0/django_rq/settings.py`

 * *Files identical despite different names*

### Comparing `django-rq-2.7.0/django_rq/templates/django_rq/clear_queue.html` & `django-rq-2.8.0/django_rq/templates/django_rq/clear_queue.html`

 * *Files identical despite different names*

### Comparing `django-rq-2.7.0/django_rq/templates/django_rq/confirm_action.html` & `django-rq-2.8.0/django_rq/templates/django_rq/confirm_action.html`

 * *Files identical despite different names*

### Comparing `django-rq-2.7.0/django_rq/templates/django_rq/delete_job.html` & `django-rq-2.8.0/django_rq/templates/django_rq/delete_job.html`

 * *Files identical despite different names*

### Comparing `django-rq-2.7.0/django_rq/templates/django_rq/job_detail.html` & `django-rq-2.8.0/django_rq/templates/django_rq/job_detail.html`

 * *Files identical despite different names*

### Comparing `django-rq-2.7.0/django_rq/templates/django_rq/jobs.html` & `django-rq-2.8.0/django_rq/templates/django_rq/jobs.html`

 * *Files identical despite different names*

### Comparing `django-rq-2.7.0/django_rq/templates/django_rq/requeue_all.html` & `django-rq-2.8.0/django_rq/templates/django_rq/requeue_all.html`

 * *Files identical despite different names*

### Comparing `django-rq-2.7.0/django_rq/templates/django_rq/stats.html` & `django-rq-2.8.0/django_rq/templates/django_rq/stats.html`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,17 @@
                     <th>Finished Jobs</th>
                     <th>Failed Jobs</th>
                     <th>Scheduled Jobs</th>
                     <th>Workers</th>
                     <th>Host</th>
                     <th>Port</th>
                     <th>DB</th>
+                    {% if queue.scheduler_pid is not False %}
+                        <th>Scheduler PID</th>
+                    {% endif%}
                 </tr>
             </thead>
             <tbody>
                 {% for queue in queues %}
                     <tr class = "{% cycle 'row1' 'row2' %}">
                         <th>
                             <a href = "{% url 'rq_jobs' queue.index %}">
@@ -80,14 +83,17 @@
                         <th><a href = "{% url 'rq_workers' queue.index %}">
                                 {{ queue.workers }}
                             </a>
                         </th>
                         <td>{{ queue.connection_kwargs.host }}</td>
                         <td>{{ queue.connection_kwargs.port }}</td>
                         <td>{{ queue.connection_kwargs.db }}</td>
+                        {% if queue.scheduler_pid is not False %}
+                        <td>{{ queue.scheduler_pid|default_if_none:"Inactive" }}</td>
+                        {% endif %}
                     </tr>
                 {% endfor %}
             </tbody>
         </table>
         <br />
         <a href="{% url 'rq_home_json' %}">View as JSON</a>
     </div>
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
 {% extends "admin/base_site.html" %} {% block title %}Queues {{ block.super }}
 {% endblock %} {% block extrastyle %} {{ block.super }}
  {% endblock %} {% block content_title %}
 ****** RQ Queues ******
 {% endblock %} {% block breadcrumbs %}
 Home › Django_RQ
 {% endblock %} {% block content %}
-Name       Queued     Oldest Queued Job          Active Jobs        Deferred Jobs       Finished Jobs       Failed Jobs       Scheduled Jobs       Workers       Host                         Port                         DB
+Name       Queued     Oldest Queued Job          Active Jobs        Deferred Jobs       Finished Jobs       Failed Jobs       Scheduled Jobs       Workers       Host                         Port                         DB                         Scheduler PID
            Jobs
-{          {          {                          {                  {                   {                   {                 {                    {             {                            {                            {
-{          {          {                          {                  {                   {                   {                 {                    {             {                            {                            {
-queue.name queue.jobs queue.oldest_job_timestamp queue.started_jobs queue.deferred_jobs queue.finished_jobs queue.failed_jobs queue.scheduled_jobs queue.workers queue.connection_kwargs.host queue.connection_kwargs.port queue.connection_kwargs.db
-}}         }}         }}                         }}                 }}                  }}                  }}                }}                   }}            }}                           }}                           }}
+{          {          {                          {                  {                   {                   {                 {                    {             {                            {                            {                          {
+{          {          {                          {                  {                   {                   {                 {                    {             {                            {                            {                          {
+queue.name queue.jobs queue.oldest_job_timestamp queue.started_jobs queue.deferred_jobs queue.finished_jobs queue.failed_jobs queue.scheduled_jobs queue.workers queue.connection_kwargs.host queue.connection_kwargs.port queue.connection_kwargs.db queue.scheduler_pid|default_if_none:
+}}         }}         }}                         }}                 }}                  }}                  }}                }}                   }}            }}                           }}                           }}                         "Inactive" }}
 
 View_as_JSON
 {% endblock %}
```

### Comparing `django-rq-2.7.0/django_rq/templates/django_rq/worker_details.html` & `django-rq-2.8.0/django_rq/templates/django_rq/worker_details.html`

 * *Files identical despite different names*

### Comparing `django-rq-2.7.0/django_rq/templates/django_rq/workers.html` & `django-rq-2.8.0/django_rq/templates/django_rq/workers.html`

 * *Files identical despite different names*

### Comparing `django-rq-2.7.0/django_rq/templatetags/django_rq.py` & `django-rq-2.8.0/django_rq/templatetags/django_rq.py`

 * *Files identical despite different names*

### Comparing `django-rq-2.7.0/django_rq/tests/settings.py` & `django-rq-2.8.0/django_rq/tests/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,24 +6,27 @@
 SECRET_KEY = 'a'
 
 # Detect whether either django-redis or django-redis-cache is installed. This
 # is only really used to conditionally configure options for the unit tests.
 # In actually usage, no such check is necessary.
 try:
     from django_redis import get_redis_connection
+
     REDIS_CACHE_TYPE = 'django-redis'
 except ImportError:
     try:
         import redis_cache
+
         REDIS_CACHE_TYPE = 'django-redis-cache'
     except ImportError:
         REDIS_CACHE_TYPE = 'none'
 
 try:
     from django.utils.log import NullHandler
+
     nullhandler = 'django.utils.log.NullHandler'
 except:
     nullhandler = 'logging.NullHandler'
 
 INSTALLED_APPS = [
     'django.contrib.contenttypes',
     'django.contrib.admin',
@@ -72,59 +75,52 @@
             "format": "%(asctime)s %(message)s",
             "datefmt": "%H:%M:%S",
         },
     },
     "handlers": {
         "rq_console": {
             "level": "DEBUG",
-            #"class": "logging.StreamHandler",
-            "class": "rq.utils.ColorizingStreamHandler",
+            # "class": "logging.StreamHandler",
+            "class": "rq.logutils.ColorizingStreamHandler",
             "formatter": "rq_console",
             "exclude": ["%(asctime)s"],
         },
         'null': {
             'level': 'DEBUG',
             'class': nullhandler,
         },
     },
     'loggers': {
-        "rq.worker": {
-            "handlers": ['null'],
-            "level": "ERROR"
-        },
-    }
+        "rq.worker": {"handlers": ['null'], "level": "ERROR"},
+    },
 }
 
 
 RQ_QUEUES = {
-    'default': {
-        'HOST': REDIS_HOST,
-        'PORT': 6379,
-        'DB': 0,
-        'DEFAULT_TIMEOUT': 500
-    },
+    'default': {'HOST': REDIS_HOST, 'PORT': 6379, 'DB': 0, 'DEFAULT_TIMEOUT': 500},
     'test': {
         'HOST': REDIS_HOST,
         'PORT': 1,
         'DB': 1,
     },
     'sentinel': {
         'SENTINELS': [(REDIS_HOST, 26736), (REDIS_HOST, 26737)],
         'MASTER_NAME': 'testmaster',
         'DB': 1,
+        'USERNAME': 'redis-user',
         'PASSWORD': 'secret',
         'SOCKET_TIMEOUT': 10,
-        'CONNECTION_KWARGS': {},
+        'SENTINEL_KWARGS': {},
     },
     'test1': {
         'HOST': REDIS_HOST,
         'PORT': 1,
         'DB': 1,
         'DEFAULT_TIMEOUT': 400,
-        'QUEUE_CLASS': 'django_rq.tests.fixtures.DummyQueue'
+        'QUEUE_CLASS': 'django_rq.tests.fixtures.DummyQueue',
     },
     'test2': {
         'HOST': REDIS_HOST,
         'PORT': 1,
         'DB': 1,
     },
     'test3': {
@@ -149,14 +145,38 @@
         'URL': 'redis://username:password@host:1234',
     },
     'django_rq_test': {
         'HOST': REDIS_HOST,
         'PORT': 6379,
         'DB': 0,
     },
+    'scheduler_scheduler_active_test': {
+        'HOST': REDIS_HOST,
+        'PORT': 6379,
+        'DB': 0,
+        'ASYNC': False,
+    },
+    'scheduler_scheduler_inactive_test': {
+        'HOST': REDIS_HOST,
+        'PORT': 6379,
+        'DB': 0,
+        'ASYNC': False,
+    },
+    'worker_scheduler_active_test': {
+        'HOST': REDIS_HOST,
+        'PORT': 6379,
+        'DB': 0,
+        'ASYNC': False,
+    },
+    'worker_scheduler_inactive_test': {
+        'HOST': REDIS_HOST,
+        'PORT': 6379,
+        'DB': 0,
+        'ASYNC': False,
+    },
     'django-redis': {
         'USE_REDIS_CACHE': 'default',
     },
     'django_rq_test2': {
         'HOST': REDIS_HOST,
         'PORT': 6379,
         'DB': 0,
@@ -205,10 +225,8 @@
     'django.contrib.sessions.middleware.SessionMiddleware',
     'django.contrib.auth.middleware.AuthenticationMiddleware',
     'django.contrib.messages.middleware.MessageMiddleware',
 )
 
 MIDDLEWARE_CLASSES = MIDDLEWARE
 
-AUTHENTICATION_BACKENDS = (
-    'django.contrib.auth.backends.ModelBackend',
-)
+AUTHENTICATION_BACKENDS = ('django.contrib.auth.backends.ModelBackend',)
```

### Comparing `django-rq-2.7.0/django_rq/tests/test_views.py` & `django-rq-2.8.0/django_rq/tests/test_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 import uuid
 from datetime import datetime
-from unittest.mock import patch, PropertyMock
+from unittest.mock import PropertyMock, patch
 
 from django.contrib.auth.models import User
 from django.test import TestCase, override_settings
 from django.test.client import Client
 from django.urls import reverse
-
 from rq.job import Job, JobStatus
 from rq.registry import (
-    DeferredJobRegistry, 
+    DeferredJobRegistry,
     FailedJobRegistry,
-    FinishedJobRegistry, 
-    ScheduledJobRegistry, 
-    StartedJobRegistry
+    FinishedJobRegistry,
+    ScheduledJobRegistry,
+    StartedJobRegistry,
 )
 
 from django_rq import get_queue
 from django_rq.workers import get_worker
+
 from .fixtures import access_self, failing_job
 from .utils import get_queue_index
 
 
 @override_settings(RQ={'AUTOCOMMIT': True})
 class ViewTest(TestCase):
-
     def setUp(self):
         self.user = User.objects.create_user('foo', password='pass')
         self.user.is_staff = True
         self.user.is_active = True
         self.user.save()
         self.client = Client()
         self.client.login(username=self.user.username, password='pass')
@@ -53,15 +52,15 @@
         self.assertEqual(response.context['job'], job)
 
         # This page shouldn't fail when job.data is corrupt
         queue.connection.hset(job.key, 'data', 'unpickleable data')
         response = self.client.get(url)
         self.assertEqual(response.status_code, 200)
         self.assertIn('DeserializationError', response.content.decode())
-    
+
     def test_job_details_on_deleted_dependency(self):
         """Page doesn't crash even if job.dependency has been deleted"""
         queue = get_queue('default')
         queue_index = get_queue_index('default')
 
         job = queue.enqueue(access_self)
         second_job = queue.enqueue(access_self, depends_on=job)
@@ -78,16 +77,15 @@
         queue = get_queue('default')
         queue_index = get_queue_index('default')
         job = queue.enqueue(failing_job)
         worker = get_worker('default')
         worker.work(burst=True)
         job.refresh()
         self.assertTrue(job.is_failed)
-        self.client.post(reverse('rq_requeue_job', args=[queue_index, job.id]),
-                         {'requeue': 'Requeue'})
+        self.client.post(reverse('rq_requeue_job', args=[queue_index, job.id]), {'requeue': 'Requeue'})
         self.assertIn(job, queue.jobs)
         job.delete()
 
     def test_requeue_all(self):
         """
         Ensure that requeuing all failed job work properly
         """
@@ -127,32 +125,30 @@
         """
         In addition to deleting job from Redis, the job id also needs to be
         deleted from Queue.
         """
         queue = get_queue('django_rq_test')
         queue_index = get_queue_index('django_rq_test')
         job = queue.enqueue(access_self)
-        self.client.post(reverse('rq_delete_job', args=[queue_index, job.id]),
-                         {'post': 'yes'})
+        self.client.post(reverse('rq_delete_job', args=[queue_index, job.id]), {'post': 'yes'})
         self.assertFalse(Job.exists(job.id, connection=queue.connection))
         self.assertNotIn(job.id, queue.job_ids)
 
     def test_action_delete_jobs(self):
         queue = get_queue('django_rq_test')
         queue_index = get_queue_index('django_rq_test')
 
         # enqueue some jobs
         job_ids = []
         for _ in range(0, 3):
             job = queue.enqueue(access_self)
             job_ids.append(job.id)
 
         # remove those jobs using view
-        self.client.post(reverse('rq_actions', args=[queue_index]),
-                         {'action': 'delete', 'job_ids': job_ids})
+        self.client.post(reverse('rq_actions', args=[queue_index]), {'action': 'delete', 'job_ids': job_ids})
 
         # check if jobs are removed
         for job_id in job_ids:
             self.assertFalse(Job.exists(job_id, connection=queue.connection))
             self.assertNotIn(job_id, queue.job_ids)
 
     def test_enqueue_jobs(self):
@@ -167,15 +163,15 @@
 
         # This job is deferred
         last_job = job
         self.assertEqual(last_job.get_status(), JobStatus.DEFERRED)
         self.assertIsNone(last_job.enqueued_at)
 
         # We want to force-enqueue this job
-        self.client.post(reverse('rq_enqueue_job', args=[queue_index, last_job.id]))
+        response = self.client.post(reverse('rq_enqueue_job', args=[queue_index, last_job.id]))
 
         # Check that job is updated correctly
         last_job = queue.fetch_job(last_job.id)
         self.assertEqual(last_job.get_status(), JobStatus.QUEUED)
         self.assertIsNotNone(last_job.enqueued_at)
 
     def test_action_requeue_jobs(self):
@@ -195,166 +191,150 @@
         worker.work(burst=True)
 
         # check if all jobs are really failed
         for job in jobs:
             self.assertTrue(job.is_failed)
 
         # renqueue failed jobs from failed queue
-        self.client.post(reverse('rq_actions', args=[queue_index]),
-                         {'action': 'requeue', 'job_ids': job_ids})
+        self.client.post(reverse('rq_actions', args=[queue_index]), {'action': 'requeue', 'job_ids': job_ids})
 
         # check if we requeue all failed jobs
         for job in jobs:
             self.assertFalse(job.is_failed)
 
     def test_clear_queue(self):
         """Test that the queue clear actually clears the queue."""
         queue = get_queue('django_rq_test')
         queue_index = get_queue_index('django_rq_test')
         job = queue.enqueue(access_self)
-        self.client.post(reverse('rq_clear', args=[queue_index]),
-                         {'post': 'yes'})
+        self.client.post(reverse('rq_clear', args=[queue_index]), {'post': 'yes'})
         self.assertFalse(Job.exists(job.id, connection=queue.connection))
         self.assertNotIn(job.id, queue.job_ids)
 
     def test_finished_jobs(self):
         """Ensure that finished jobs page works properly."""
         queue = get_queue('django_rq_test')
         queue_index = get_queue_index('django_rq_test')
 
         job = queue.enqueue(access_self)
         registry = FinishedJobRegistry(queue.name, queue.connection)
         registry.add(job, 2)
-        response = self.client.get(
-            reverse('rq_finished_jobs', args=[queue_index])
-        )
+        response = self.client.get(reverse('rq_finished_jobs', args=[queue_index]))
         self.assertEqual(response.context['jobs'], [job])
 
     def test_failed_jobs(self):
         """Ensure that failed jobs page works properly."""
         queue = get_queue('django_rq_test')
         queue_index = get_queue_index('django_rq_test')
 
         # Test that page doesn't fail when FailedJobRegistry is empty
-        response = self.client.get(
-            reverse('rq_failed_jobs', args=[queue_index])
-        )
+        response = self.client.get(reverse('rq_failed_jobs', args=[queue_index]))
         self.assertEqual(response.status_code, 200)
 
         job = queue.enqueue(access_self)
         registry = FailedJobRegistry(queue.name, queue.connection)
         registry.add(job, 2)
-        response = self.client.get(
-            reverse('rq_failed_jobs', args=[queue_index])
-        )
+        response = self.client.get(reverse('rq_failed_jobs', args=[queue_index]))
         self.assertEqual(response.context['jobs'], [job])
 
     def test_scheduled_jobs(self):
         """Ensure that scheduled jobs page works properly."""
         queue = get_queue('django_rq_test')
         queue_index = get_queue_index('django_rq_test')
 
         # Test that page doesn't fail when ScheduledJobRegistry is empty
-        response = self.client.get(
-            reverse('rq_scheduled_jobs', args=[queue_index])
-        )
+        response = self.client.get(reverse('rq_scheduled_jobs', args=[queue_index]))
         self.assertEqual(response.status_code, 200)
 
         job = queue.enqueue_at(datetime.now(), access_self)
-        response = self.client.get(
-            reverse('rq_scheduled_jobs', args=[queue_index])
-        )
+        response = self.client.get(reverse('rq_scheduled_jobs', args=[queue_index]))
         self.assertEqual(response.context['jobs'], [job])
 
+        # Test that page doesn't fail when job_id has special characters
+        job2 = queue.enqueue_at(datetime.now(), access_self, job_id="job-!@#$%^&*()_=+[]{};':,.<>?|`~")
+        response = self.client.get(reverse('rq_scheduled_jobs', args=[queue_index]))
+        self.assertEqual(response.context['jobs'], [job, job2])
+
     def test_scheduled_jobs_registry_removal(self):
         """Ensure that non existing job is being deleted from registry by view"""
         queue = get_queue('django_rq_test')
         queue_index = get_queue_index('django_rq_test')
 
         registry = ScheduledJobRegistry(queue.name, queue.connection)
         job = queue.enqueue_at(datetime.now(), access_self)
         self.assertEqual(len(registry), 1)
 
         queue.connection.delete(job.key)
-        response = self.client.get(
-            reverse('rq_scheduled_jobs', args=[queue_index])
-        )
+        response = self.client.get(reverse('rq_scheduled_jobs', args=[queue_index]))
         self.assertEqual(response.context['jobs'], [])
 
         self.assertEqual(len(registry), 0)
 
     def test_started_jobs(self):
         """Ensure that active jobs page works properly."""
         queue = get_queue('django_rq_test')
         queue_index = get_queue_index('django_rq_test')
 
         job = queue.enqueue(access_self)
         registry = StartedJobRegistry(queue.name, queue.connection)
         registry.add(job, 2)
-        response = self.client.get(
-            reverse('rq_started_jobs', args=[queue_index])
-        )
+        response = self.client.get(reverse('rq_started_jobs', args=[queue_index]))
         self.assertEqual(response.context['jobs'], [job])
 
     def test_deferred_jobs(self):
         """Ensure that active jobs page works properly."""
         queue = get_queue('django_rq_test')
         queue_index = get_queue_index('django_rq_test')
 
         job = queue.enqueue(access_self)
         registry = DeferredJobRegistry(queue.name, queue.connection)
         registry.add(job, 2)
-        response = self.client.get(
-            reverse('rq_deferred_jobs', args=[queue_index])
-        )
+        response = self.client.get(reverse('rq_deferred_jobs', args=[queue_index]))
         self.assertEqual(response.context['jobs'], [job])
 
     def test_workers(self):
         """Worker index page should show workers for a specific queue"""
         queue_index = get_queue_index('django_rq_test')
 
         worker1 = get_worker('django_rq_test', name=uuid.uuid4().hex)
         worker1.register_birth()
 
         worker2 = get_worker('test3')
         worker2.register_birth()
 
-        response = self.client.get(
-            reverse('rq_workers', args=[queue_index])
-        )
+        response = self.client.get(reverse('rq_workers', args=[queue_index]))
         self.assertEqual(response.context['workers'], [worker1])
 
     def test_worker_details(self):
         """Worker index page should show workers for a specific queue"""
         queue_index = get_queue_index('django_rq_test')
 
         worker = get_worker('django_rq_test', name=uuid.uuid4().hex)
         worker.register_birth()
 
-        response = self.client.get(
-            reverse('rq_worker_details', args=[queue_index, worker.key])
-        )
+        response = self.client.get(reverse('rq_worker_details', args=[queue_index, worker.key]))
         self.assertEqual(response.context['worker'], worker)
 
     def test_statistics_json_view(self):
         """
         Django-RQ's statistic as JSON only viewable by staff or with API_TOKEN
         """
 
         # Override testing RQ_QUEUES
-        queues = [{
-            'connection_config': {
-                'DB': 0,
-                'HOST': 'localhost',
-                'PORT': 6379,
-            },
-            'name': 'default'
-        }]
-        with patch('django_rq.utils.QUEUES_LIST',
-                   new_callable=PropertyMock(return_value=queues)):
+        queues = [
+            {
+                'connection_config': {
+                    'DB': 0,
+                    'HOST': 'localhost',
+                    'PORT': 6379,
+                },
+                'name': 'default',
+            }
+        ]
+        with patch('django_rq.utils.QUEUES_LIST', new_callable=PropertyMock(return_value=queues)):
             response = self.client.get(reverse('rq_home'))
             self.assertEqual(response.status_code, 200)
 
             response = self.client.get(reverse('rq_home_json'))
             self.assertEqual(response.status_code, 200)
 
             # Not staff, only token
```

### Comparing `django-rq-2.7.0/django_rq/tests/tests.py` & `django-rq-2.8.0/django_rq/tests/tests.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,33 +13,38 @@
 
 from redis.exceptions import ConnectionError
 from rq import get_current_job, Queue
 from rq.exceptions import NoSuchJobError
 from rq.job import Job
 from rq.registry import FinishedJobRegistry, ScheduledJobRegistry
 from rq.worker import Worker
+from rq.serializers import DefaultSerializer, JSONSerializer
 
 from django_rq.decorators import job
 from django_rq.jobs import get_job_class
 from django_rq.management.commands import rqworker
 from django_rq.queues import (
-    get_connection, get_queue, get_queues,
-    get_unique_connection_configs, DjangoRQ,
-    get_redis_connection
+    get_connection,
+    get_queue,
+    get_queues,
+    get_unique_connection_configs,
+    DjangoRQ,
+    get_redis_connection,
 )
 from django_rq import thread_queue
 from django_rq.templatetags.django_rq import force_escape, to_localtime
 from django_rq.tests.fixtures import DummyJob, DummyQueue, DummyWorker
-from django_rq.utils import get_jobs, get_statistics
+from django_rq.utils import get_jobs, get_statistics, get_scheduler_pid
 from django_rq.workers import get_worker, get_worker_class
 
 try:
     from rq_scheduler import Scheduler
     from ..queues import get_scheduler
     from django_rq.tests.fixtures import DummyScheduler
+
     RQ_SCHEDULER_INSTALLED = True
 except ImportError:
     RQ_SCHEDULER_INSTALLED = False
 
 QUEUES = settings.RQ_QUEUES
 
 
@@ -64,39 +69,38 @@
             job = Job.fetch(job_id, connection=connection)
             job.delete()
         except NoSuchJobError:
             pass
 
 
 class RqStatsTest(TestCase):
-
     def test_get_connection_default(self):
         """
         Test that rqstats returns the right statistics
         """
         # Override testing RQ_QUEUES
-        queues = [{
-            'connection_config': {
-                'DB': 0,
-                'HOST': 'localhost',
-                'PORT': 6379,
-            },
-            'name': 'default'
-        }]
-        with patch('django_rq.utils.QUEUES_LIST',
-                   new_callable=PropertyMock(return_value=queues)):
+        queues = [
+            {
+                'connection_config': {
+                    'DB': 0,
+                    'HOST': 'localhost',
+                    'PORT': 6379,
+                },
+                'name': 'default',
+            }
+        ]
+        with patch('django_rq.utils.QUEUES_LIST', new_callable=PropertyMock(return_value=queues)):
             # Only to make sure it doesn't crash
             call_command('rqstats')
             call_command('rqstats', '-j')
             call_command('rqstats', '-y')
 
 
 @override_settings(RQ={'AUTOCOMMIT': True})
 class QueuesTest(TestCase):
-
     def setUp(self):
         """Used to test with / without sentry_sdk available."""
         self.mock_sdk = mock.MagicMock()
         self.mock_sdk.Hub.current.client.options = {}
         sys.modules["sentry_sdk"] = self.mock_sdk
 
     def tearDown(self):
@@ -143,37 +147,37 @@
         self.assertEqual(sentinel_mock.master_for.call_count, 1)
         self.assertEqual(sentinel_class_mock.call_count, 1)
 
         sentinel_instances = sentinel_class_mock.call_args[0][0]
         self.assertListEqual(config['SENTINELS'], sentinel_instances)
 
         connection_kwargs = sentinel_mock.master_for.call_args[1]
-        self.assertEqual(connection_kwargs['service_name'],
-                         config['MASTER_NAME'])
+        self.assertEqual(connection_kwargs['service_name'], config['MASTER_NAME'])
 
     @patch('django_rq.queues.Sentinel')
     def test_sentinel_class_initialized_with_kw_args(self, sentinel_class_mock):
         """
         Test that Sentinel object is initialized with proper connection kwargs.
         """
         config = {
             'SENTINELS': [],
             'MASTER_NAME': 'test_master',
             'SOCKET_TIMEOUT': 0.2,
             'DB': 0,
-            'CONNECTION_KWARGS': {
-                'socket_connect_timeout': 0.3
-            }
+            'USERNAME': 'redis-user',
+            'PASSWORD': 'redis-pass',
+            'CONNECTION_KWARGS': {'ssl': False},
+            'SENTINEL_KWARGS': {'username': 'sentinel-user', 'password': 'sentinel-pass', 'socket_timeout': 0.3},
         }
         get_redis_connection(config)
-        sentinel_init_kwargs = sentinel_class_mock.call_args[1]
+        sentinel_init_sentinel_kwargs = sentinel_class_mock.call_args[1]
         self.assertDictEqual(
-            sentinel_init_kwargs,
-            {'socket_connect_timeout': 0.3, 'db': 0,
-             'socket_timeout': 0.2, 'password': None})
+            sentinel_init_sentinel_kwargs, 
+            {'db': 0, 'username': 'redis-user', 'password': 'redis-pass', 'socket_timeout': 0.2, 'ssl': False, 'sentinel_kwargs': {'username': 'sentinel-user', 'password': 'sentinel-pass', 'socket_timeout': 0.3}}
+        )
 
     def test_get_queue_default(self):
         """
         Test that get_queue use the right parameters for `default`
         connection.
         """
         config = QUEUES['default']
@@ -264,18 +268,20 @@
         """
         Checks that passing queues via commandline arguments works
         """
         queue_names = ['django_rq_test', 'django_rq_test2']
         jobs = []
         for queue_name in queue_names:
             queue = get_queue(queue_name)
-            jobs.append({
-                'job': queue.enqueue(divide, 42, 1),
-                'finished_job_registry': FinishedJobRegistry(queue.name, queue.connection),
-            })
+            jobs.append(
+                {
+                    'job': queue.enqueue(divide, 42, 1),
+                    'finished_job_registry': FinishedJobRegistry(queue.name, queue.connection),
+                }
+            )
 
         call_command('rqworker', *queue_names, burst=True)
 
         for job in jobs:
             self.assertTrue(job['job'].is_finished)
             self.assertIn(job['job'].id, job['finished_job_registry'].get_job_ids())
 
@@ -285,67 +291,71 @@
             'https://1@sentry.io/1',
             ca_certs=None,
             debug=False,
             integrations=[
                 self.mock_sdk.integrations.redis.RedisIntegration(),
                 self.mock_sdk.integrations.rq.RqIntegration(),
                 self.mock_sdk.integrations.django.DjangoIntegration(),
-            ]
+            ],
         )
 
     def test_configure_sentry__options(self):
         """Check that debug and ca_certs can be passed through to Sentry."""
         rqworker.configure_sentry('https://1@sentry.io/1', sentry_debug=True, sentry_ca_certs='/certs')
         self.mock_sdk.init.assert_called_once_with(
             'https://1@sentry.io/1',
             ca_certs='/certs',
             debug=True,
             integrations=[
                 self.mock_sdk.integrations.redis.RedisIntegration(),
                 self.mock_sdk.integrations.rq.RqIntegration(),
                 self.mock_sdk.integrations.django.DjangoIntegration(),
-            ]
+            ],
         )
 
     def test_sentry_dsn(self):
         """Check that options are passed to configure_sentry as expected."""
         queue_names = ['django_rq_test']
-        call_command('rqworker', *queue_names, burst=True,
-                     sentry_dsn='https://1@sentry.io/1', sentry_debug=True, sentry_ca_certs='/certs')
+        call_command(
+            'rqworker',
+            *queue_names,
+            burst=True,
+            sentry_dsn='https://1@sentry.io/1',
+            sentry_debug=True,
+            sentry_ca_certs='/certs'
+        )
 
         self.mock_sdk.init.assert_called_once_with(
             'https://1@sentry.io/1',
             ca_certs='/certs',
             debug=True,
             integrations=[
                 self.mock_sdk.integrations.redis.RedisIntegration(),
                 self.mock_sdk.integrations.rq.RqIntegration(),
                 self.mock_sdk.integrations.django.DjangoIntegration(),
-            ]
+            ],
         )
 
     @mock.patch('django_rq.management.commands.rqworker.configure_sentry')
     def test_sentry_dsn__noop(self, mocked):
         """Check that sentry is ignored if sentry_dsn is not passed in."""
         queue_names = ['django_rq_test']
-        call_command('rqworker', *queue_names, burst=True,
-                     sentry_debug=True, sentry_ca_certs='/certs')
+        call_command('rqworker', *queue_names, burst=True, sentry_debug=True, sentry_ca_certs='/certs')
 
         self.assertEqual(mocked.call_count, 0)
 
     @mock.patch('django_rq.management.commands.rqworker.configure_sentry')
     def test_sentry_sdk_import_error(self, mocked):
         """Check the command handles import errors as expected."""
         mocked.side_effect = ImportError
         queue_names = ['django_rq_test']
         with self.assertRaises(SystemExit):
-            call_command('rqworker', *queue_names, burst=True,
-                         sentry_dsn='https://1@sentry.io/1')
+            call_command('rqworker', *queue_names, burst=True, sentry_dsn='https://1@sentry.io/1')
 
-    @mock.patch('django_rq.management.commands.rqworker.use_connection')
+    @mock.patch('django_rq.management.commands.rqworker.Connection')
     def test_connection_error(self, mocked):
         """Check that redis ConnectionErrors are handled correctly."""
         mocked.side_effect = ConnectionError("Unable to connect")
         queue_names = ['django_rq_test']
         with self.assertRaises(SystemExit):
             call_command('rqworker', *queue_names)
 
@@ -356,32 +366,25 @@
             'DB': 0,
         }
         connection_params_2 = {
             'HOST': 'localhost',
             'PORT': 6379,
             'DB': 1,
         }
-        config = {
-            'default': connection_params_1,
-            'test': connection_params_2
-        }
+        config = {'default': connection_params_1, 'test': connection_params_2}
         unique_configs = get_unique_connection_configs(config)
         self.assertEqual(len(unique_configs), 2)
         self.assertIn(connection_params_1, unique_configs)
         self.assertIn(connection_params_2, unique_configs)
 
         # self.assertEqual(get_unique_connection_configs(config),
         #                  [connection_params_1, connection_params_2])
-        config = {
-            'default': connection_params_1,
-            'test': connection_params_1
-        }
+        config = {'default': connection_params_1, 'test': connection_params_1}
         # Should return one connection config since it filters out duplicates
-        self.assertEqual(get_unique_connection_configs(config),
-                         [connection_params_1])
+        self.assertEqual(get_unique_connection_configs(config), [connection_params_1])
 
     def test_get_unique_connection_configs_with_different_timeout(self):
         connection_params_1 = {
             'HOST': 'localhost',
             'PORT': 6379,
             'DB': 0,
         }
@@ -461,56 +464,62 @@
         # Ensure that decorator passes in the right queue from settings.py
         queue_name = 'test3'
         config = QUEUES[queue_name]
 
         @job(queue_name)
         def test():
             pass
+
         result = test.delay()
         queue = get_queue(queue_name)
         self.assertEqual(result.origin, queue_name)
         result.delete()
 
     def test_job_decorator_default(self):
         # Ensure that decorator passes in the right queue from settings.py
         @job
         def test():
             pass
+
         result = test.delay()
         self.assertEqual(result.origin, 'default')
         result.delete()
 
     def test_job_decorator_result_ttl_default(self):
         from rq.defaults import DEFAULT_RESULT_TTL
 
         @job
         def test():
             pass
+
         result = test.delay()
         self.assertEqual(result.result_ttl, DEFAULT_RESULT_TTL)
         result.delete()
 
     @override_settings(RQ={'AUTOCOMMIT': True, 'DEFAULT_RESULT_TTL': 5432})
     def test_job_decorator_result_ttl(self):
         @job
         def test():
             pass
+
         result = test.delay()
         self.assertEqual(result.result_ttl, 5432)
         result.delete()
 
     @override_settings(RQ={'AUTOCOMMIT': True, 'DEFAULT_RESULT_TTL': 0})
     def test_job_decorator_result_ttl_zero(self):
         @job
         def test():
             pass
+
         result = test.delay()
         self.assertEqual(result.result_ttl, 0)
         result.delete()
 
+
 @override_settings(RQ={'AUTOCOMMIT': True})
 class WorkersTest(TestCase):
     def test_get_worker_default(self):
         """
         By default, ``get_worker`` should return worker for ``default`` queue.
         """
         worker = get_worker()
@@ -524,21 +533,33 @@
         """
         w = get_worker('test3')
         self.assertEqual(len(w.queues), 1)
         queue = w.queues[0]
         self.assertEqual(queue.name, 'test3')
 
     def test_get_worker_custom_classes(self):
-        w = get_worker(job_class='django_rq.tests.fixtures.DummyJob',
-                       queue_class='django_rq.tests.fixtures.DummyQueue',
-                       worker_class='django_rq.tests.fixtures.DummyWorker')
+        w = get_worker(
+            job_class='django_rq.tests.fixtures.DummyJob',
+            queue_class='django_rq.tests.fixtures.DummyQueue',
+            worker_class='django_rq.tests.fixtures.DummyWorker',
+        )
         self.assertIs(w.job_class, DummyJob)
         self.assertIsInstance(w.queues[0], DummyQueue)
         self.assertIsInstance(w, DummyWorker)
 
+    def test_get_worker_custom_serializer(self):
+        w = get_worker(
+            serializer='rq.serializers.JSONSerializer',
+        )
+        self.assertEqual(w.serializer, JSONSerializer)
+
+    def test_get_worker_default_serializer(self):
+        w = get_worker()
+        self.assertEqual(w.serializer, DefaultSerializer)
+
     def test_get_current_job(self):
         """
         Ensure that functions using RQ's ``get_current_job`` doesn't fail
         when run from rqworker (the job id is not in the failed queue).
         """
         queue = get_queue()
         job = queue.enqueue(access_self)
@@ -558,15 +579,14 @@
         for verbosity in [0, 1, 2, 3]:
             setup_loghandlers_mock.reset_mock()
             call_command('rqworker', verbosity=verbosity, burst=True)
             setup_loghandlers_mock.assert_called_once_with(expected_level[verbosity])
 
 
 class ThreadQueueTest(TestCase):
-
     @override_settings(RQ={'AUTOCOMMIT': True})
     def test_enqueue_autocommit_on(self):
         """
         Running ``enqueue`` when AUTOCOMMIT is on should
         immediately persist job into Redis.
         """
         queue = get_queue()
@@ -631,15 +651,14 @@
         self.assertEqual(queue.count, 0)
         url = reverse('error')
         self.assertRaises(ValueError, self.client.get, url)
         self.assertEqual(queue.count, 0)
 
 
 class SchedulerTest(TestCase):
-
     @skipIf(RQ_SCHEDULER_INSTALLED is False, 'RQ Scheduler not installed')
     def test_get_scheduler(self):
         """
         Ensure get_scheduler creates a scheduler instance with the right
         connection params for `test` queue.
         """
         config = QUEUES['test']
@@ -697,29 +716,26 @@
         job = scheduler.enqueue_at(datetime.datetime.now() + datetime.timedelta(days=1), divide, 1, 1)
         self.assertTrue(job in scheduler.get_jobs())
         self.assertEqual(job.result_ttl, 5432)
         job.delete()
 
 
 class RedisCacheTest(TestCase):
-
-    @skipIf(settings.REDIS_CACHE_TYPE != 'django-redis',
-            'django-redis not installed')
+    @skipIf(settings.REDIS_CACHE_TYPE != 'django-redis', 'django-redis not installed')
     @patch('django_redis.get_redis_connection')
     def test_get_queue_django_redis(self, mocked):
         """
         Test that the USE_REDIS_CACHE option for configuration works.
         """
         queue = get_queue('django-redis')
         queue.enqueue(access_self)
         self.assertEqual(len(queue), 1)
         self.assertEqual(mocked.call_count, 1)
 
-    @skipIf(settings.REDIS_CACHE_TYPE != 'django-redis-cache',
-            'django-redis-cache not installed')
+    @skipIf(settings.REDIS_CACHE_TYPE != 'django-redis-cache', 'django-redis-cache not installed')
     def test_get_queue_django_redis_cache(self):
         """
         Test that the USE_REDIS_CACHE option for configuration works.
         """
         queueName = 'django-redis-cache'
         queue = get_queue(queueName)
         connection_kwargs = queue.connection.connection_pool.connection_kwargs
@@ -732,67 +748,57 @@
         self.assertEqual(connection_kwargs['host'], cacheHost)
         self.assertEqual(connection_kwargs['port'], int(cachePort))
         self.assertEqual(connection_kwargs['db'], int(cacheDBNum))
         self.assertEqual(connection_kwargs['password'], None)
 
 
 class JobClassTest(TestCase):
-
     def test_default_job_class(self):
         job_class = get_job_class()
         self.assertIs(job_class, Job)
 
     @override_settings(RQ={'JOB_CLASS': 'django_rq.tests.fixtures.DummyJob'})
     def test_custom_class(self):
         job_class = get_job_class()
         self.assertIs(job_class, DummyJob)
 
     def test_local_override(self):
-        self.assertIs(
-            get_job_class('django_rq.tests.fixtures.DummyJob'),
-            DummyJob
-        )
+        self.assertIs(get_job_class('django_rq.tests.fixtures.DummyJob'), DummyJob)
 
 
 class QueueClassTest(TestCase):
-
     def test_default_queue_class(self):
         queue = get_queue('test')
         self.assertIsInstance(queue, DjangoRQ)
 
     def test_for_queue(self):
         queue = get_queue('test1')
         self.assertIsInstance(queue, DummyQueue)
 
     def test_in_kwargs(self):
         queue = get_queue('test', queue_class=DummyQueue)
         self.assertIsInstance(queue, DummyQueue)
 
 
 class WorkerClassTest(TestCase):
-
     def test_default_worker_class(self):
         worker = get_worker()
         self.assertIsInstance(worker, Worker)
 
     @override_settings(RQ={'WORKER_CLASS': 'django_rq.tests.fixtures.DummyWorker'})
     def test_custom_class(self):
         worker = get_worker()
         self.assertIsInstance(worker, DummyWorker)
 
     def test_local_override(self):
-        self.assertIs(
-            get_worker_class('django_rq.tests.fixtures.DummyWorker'),
-            DummyWorker
-        )
+        self.assertIs(get_worker_class('django_rq.tests.fixtures.DummyWorker'), DummyWorker)
 
 
 @override_settings(RQ={'AUTOCOMMIT': True})
 class TemplateTagTest(TestCase):
-
     def test_to_localtime(self):
         with self.settings(TIME_ZONE='Asia/Jakarta'):
             queue = get_queue()
             job = queue.enqueue(access_self)
             time = to_localtime(job.created_at)
 
             self.assertIsNotNone(time.tzinfo)
@@ -813,30 +819,109 @@
 
         escaped_string = force_escape(safe_string)
         expected = "hello world"
 
         self.assertEqual(escaped_string, expected)
 
 
-
-class UtilsTest(TestCase):
-
-    def test_get_statistics(self):
-        """get_statistics() returns the right number of workers"""
+class SchedulerPIDTest(TestCase):
+    @skipIf(RQ_SCHEDULER_INSTALLED is False, 'RQ Scheduler not installed')
+    def test_scheduler_scheduler_pid_active(self):
+        test_queue = 'scheduler_scheduler_active_test'
         queues = [{
             'connection_config': {
                 'DB': 0,
                 'HOST': 'localhost',
                 'PORT': 6379,
             },
-            'name': 'async'
+            'name': test_queue,
+        }]        
+        with patch('django_rq.utils.QUEUES_LIST',
+            new_callable=PropertyMock(return_value=queues)):
+            scheduler = get_scheduler(test_queue)
+            scheduler.register_birth()
+            self.assertIs(get_scheduler_pid(get_queue(scheduler.queue_name)), False)
+            scheduler.register_death()
+    
+    @skipIf(RQ_SCHEDULER_INSTALLED is False, 'RQ Scheduler not installed')
+    def test_scheduler_scheduler_pid_inactive(self):
+        test_queue = 'scheduler_scheduler_inactive_test'
+        queues = [{
+            'connection_config': {
+                'DB': 0,
+                'HOST': 'localhost',
+                'PORT': 6379,
+            },
+            'name': test_queue,
+        }]        
+        with patch('django_rq.utils.QUEUES_LIST',
+            new_callable=PropertyMock(return_value=queues)):
+            connection = get_connection(test_queue)
+            connection.flushall()  # flush is needed to isolate from other tests
+            scheduler = get_scheduler(test_queue)
+            scheduler.remove_lock()
+            scheduler.register_death()  # will mark the scheduler as death so get_scheduler_pid will return None
+            self.assertIs(get_scheduler_pid(get_queue(scheduler.queue_name)), False)
+
+    @skipIf(RQ_SCHEDULER_INSTALLED is True, 'RQ Scheduler installed (no worker--with-scheduler)')
+    def test_worker_scheduler_pid_active(self):
+        '''The worker works as scheduler too if RQ Scheduler not installed, and the pid scheduler_pid is correct'''
+        test_queue = 'worker_scheduler_active_test'
+        queues = [{
+            'connection_config': {
+                'DB': 0,
+                'HOST': 'localhost',
+                'PORT': 6379,
+            },
+            'name': test_queue,
         }]
-
+        with patch('rq.scheduler.RQScheduler.release_locks') as mock_release_locks:
+            with patch('django_rq.utils.QUEUES_LIST',
+                new_callable=PropertyMock(return_value=queues)):
+                queue = get_queue(test_queue)
+                worker = get_worker(test_queue, name=uuid4().hex)
+                worker.work(with_scheduler=True, burst=True)  # force the worker to acquire a scheduler lock
+                pid = get_scheduler_pid(queue)
+                self.assertIsNotNone(pid)
+                self.assertIsNot(pid, False)
+                self.assertIsInstance(pid, int)
+
+    @skipIf(RQ_SCHEDULER_INSTALLED is True, 'RQ Scheduler installed (no worker--with-scheduler)')
+    def test_worker_scheduler_pid_inactive(self):
+        '''The worker works as scheduler too if RQ Scheduler not installed, and the pid scheduler_pid is correct'''
+        test_queue = 'worker_scheduler_inactive_test'
+        queues = [{
+            'connection_config': {
+                'DB': 0,
+                'HOST': 'localhost',
+                'PORT': 6379,
+            },
+            'name': test_queue,
+        }]        
         with patch('django_rq.utils.QUEUES_LIST',
-                   new_callable=PropertyMock(return_value=queues)):
+            new_callable=PropertyMock(return_value=queues)):
+            worker = get_worker(test_queue, name=uuid4().hex)
+            worker.work(with_scheduler=False, burst=True)  # worker will not acquire lock, scheduler_pid should return None
+            self.assertIsNone(get_scheduler_pid(worker.queues[0]))
+
+class UtilsTest(TestCase):
+    def test_get_statistics(self):
+        """get_statistics() returns the right number of workers"""
+        queues = [
+            {
+                'connection_config': {
+                    'DB': 0,
+                    'HOST': 'localhost',
+                    'PORT': 6379,
+                },
+                'name': 'async',
+            }
+        ]
+
+        with patch('django_rq.utils.QUEUES_LIST', new_callable=PropertyMock(return_value=queues)):
             worker = get_worker('async', name=uuid4().hex)
             worker.register_birth()
             statistics = get_statistics()
             data = statistics['queues'][0]
             self.assertEqual(data['name'], 'async')
             self.assertEqual(data['workers'], 1)
             worker.register_death()
@@ -847,29 +932,20 @@
 
         registry = ScheduledJobRegistry(queue.name, queue.connection)
         flush_registry(registry)
 
         now = datetime.datetime.now()
         job = queue.enqueue_at(now, access_self)
         job2 = queue.enqueue_at(now, access_self)
-        self.assertEqual(
-            get_jobs(queue, [job.id, job2.id]),
-            [job, job2]
-        )
+        self.assertEqual(get_jobs(queue, [job.id, job2.id]), [job, job2])
         self.assertEqual(len(registry), 2)
 
         # job has been deleted, so the result will be filtered out
         queue.connection.delete(job.key)
-        self.assertEqual(
-            get_jobs(queue, [job.id, job2.id]),
-            [job2]
-        )
+        self.assertEqual(get_jobs(queue, [job.id, job2.id]), [job2])
         self.assertEqual(len(registry), 2)
 
         # If job has been deleted and `registry` is passed,
         # job will also be removed from registry
         queue.connection.delete(job2.key)
-        self.assertEqual(
-            get_jobs(queue, [job.id, job2.id], registry),
-            []
-        )
+        self.assertEqual(get_jobs(queue, [job.id, job2.id], registry), [])
         self.assertEqual(len(registry), 0)
```

### Comparing `django-rq-2.7.0/django_rq/tests/utils.py` & `django-rq-2.8.0/django_rq/tests/utils.py`

 * *Files identical despite different names*

### Comparing `django-rq-2.7.0/django_rq/thread_queue.py` & `django-rq-2.8.0/django_rq/thread_queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,10 +36,10 @@
             queue.original_enqueue_call(*args, **kwargs)
     finally:
         clear()
 
 
 def clear(*args, **kwargs):
     try:
-        del(_thread_data.job_queue)
+        del _thread_data.job_queue
     except AttributeError:
         pass
```

### Comparing `django-rq-2.7.0/django_rq/urls.py` & `django-rq-2.8.0/django_rq/urls.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,32 @@
 from django.urls import re_path
 
 from . import views
 
-
 urlpatterns = [
-    re_path(r'^$',
-            views.stats, name='rq_home'),
-    re_path(r'^stats.json/(?P<token>[\w]+)?/?$',
-            views.stats_json, name='rq_home_json'),
-    re_path(r'^queues/(?P<queue_index>[\d]+)/$',
-            views.jobs, name='rq_jobs'),
-    re_path(r'^workers/(?P<queue_index>[\d]+)/$',
-            views.workers, name='rq_workers'),
-    re_path(r'^workers/(?P<queue_index>[\d]+)/(?P<key>[-\w\.\:\$]+)/$',
-            views.worker_details, name='rq_worker_details'),
-    re_path(r'^queues/(?P<queue_index>[\d]+)/finished/$',
-            views.finished_jobs, name='rq_finished_jobs'),
-    re_path(r'^queues/(?P<queue_index>[\d]+)/failed/$',
-            views.failed_jobs, name='rq_failed_jobs'),
-    re_path(r'^queues/(?P<queue_index>[\d]+)/scheduled/$',
-            views.scheduled_jobs, name='rq_scheduled_jobs'),
-    re_path(r'^queues/(?P<queue_index>[\d]+)/started/$',
-            views.started_jobs, name='rq_started_jobs'),
-    re_path(r'^queues/(?P<queue_index>[\d]+)/deferred/$',
-            views.deferred_jobs, name='rq_deferred_jobs'),
-    re_path(r'^queues/(?P<queue_index>[\d]+)/empty/$',
-            views.clear_queue, name='rq_clear'),
-    re_path(r'^queues/(?P<queue_index>[\d]+)/requeue-all/$',
-            views.requeue_all, name='rq_requeue_all'),
-    re_path(r'^queues/(?P<queue_index>[\d]+)/(?P<job_id>[-\w\.\:\$]+)/$',
-            views.job_detail, name='rq_job_detail'),
-    re_path(r'^queues/(?P<queue_index>[\d]+)/(?P<job_id>[-\w\.\:\$]+)/delete/$',
-            views.delete_job, name='rq_delete_job'),
-    re_path(r'^queues/confirm-action/(?P<queue_index>[\d]+)/$',
-            views.confirm_action, name='rq_confirm_action'),
-    re_path(r'^queues/actions/(?P<queue_index>[\d]+)/$',
-            views.actions, name='rq_actions'),
-    re_path(r'^queues/(?P<queue_index>[\d]+)/(?P<job_id>[-\w\.\:\$]+)/requeue/$',
-            views.requeue_job_view, name='rq_requeue_job'),
-    re_path(r'^queues/(?P<queue_index>[\d]+)/(?P<job_id>[-\w\.\:\$]+)/enqueue/$',
-            views.enqueue_job, name='rq_enqueue_job'),
+    re_path(r'^$', views.stats, name='rq_home'),
+    re_path(r'^stats.json/(?P<token>[\w]+)?/?$', views.stats_json, name='rq_home_json'),
+    re_path(r'^queues/(?P<queue_index>[\d]+)/$', views.jobs, name='rq_jobs'),
+    re_path(r'^workers/(?P<queue_index>[\d]+)/$', views.workers, name='rq_workers'),
+    re_path(r'^workers/(?P<queue_index>[\d]+)/(?P<key>[-\w\.\:\$]+)/$', views.worker_details, name='rq_worker_details'),
+    re_path(r'^queues/(?P<queue_index>[\d]+)/finished/$', views.finished_jobs, name='rq_finished_jobs'),
+    re_path(r'^queues/(?P<queue_index>[\d]+)/failed/$', views.failed_jobs, name='rq_failed_jobs'),
+    re_path(r'^queues/(?P<queue_index>[\d]+)/scheduled/$', views.scheduled_jobs, name='rq_scheduled_jobs'),
+    re_path(r'^queues/(?P<queue_index>[\d]+)/started/$', views.started_jobs, name='rq_started_jobs'),
+    re_path(r'^queues/(?P<queue_index>[\d]+)/deferred/$', views.deferred_jobs, name='rq_deferred_jobs'),
+    re_path(r'^queues/(?P<queue_index>[\d]+)/empty/$', views.clear_queue, name='rq_clear'),
+    re_path(r'^queues/(?P<queue_index>[\d]+)/requeue-all/$', views.requeue_all, name='rq_requeue_all'),
+    re_path(r'^queues/(?P<queue_index>[\d]+)/(?P<job_id>[^/]+)/$', views.job_detail, name='rq_job_detail'),
+    re_path(
+        r'^queues/(?P<queue_index>[\d]+)/(?P<job_id>[^/]+)/delete/$', views.delete_job, name='rq_delete_job'
+    ),
+    re_path(r'^queues/confirm-action/(?P<queue_index>[\d]+)/$', views.confirm_action, name='rq_confirm_action'),
+    re_path(r'^queues/actions/(?P<queue_index>[\d]+)/$', views.actions, name='rq_actions'),
+    re_path(
+        r'^queues/(?P<queue_index>[\d]+)/(?P<job_id>[^/]+)/requeue/$',
+        views.requeue_job_view,
+        name='rq_requeue_job',
+    ),
+    re_path(
+        r'^queues/(?P<queue_index>[\d]+)/(?P<job_id>[^/]+)/enqueue/$', views.enqueue_job, name='rq_enqueue_job'
+    ),
 ]
```

### Comparing `django-rq-2.7.0/django_rq/views.py` & `django-rq-2.8.0/django_rq/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,29 +27,25 @@
 from .settings import API_TOKEN
 from .utils import get_statistics, get_jobs
 
 
 @never_cache
 @staff_member_required
 def stats(request):
-    context_data = {
-        **admin.site.each_context(request),
-        **get_statistics(run_maintenance_tasks=True)
-    }
+    context_data = {**admin.site.each_context(request), **get_statistics(run_maintenance_tasks=True)}
     return render(request, 'django_rq/stats.html', context_data)
 
 
 def stats_json(request, token=None):
     if request.user.is_staff or (token and token == API_TOKEN):
         return JsonResponse(get_statistics())
 
-    return JsonResponse({
-        "error": True,
-        "description": "Please configure API_TOKEN in settings.py before accessing this view."
-    })
+    return JsonResponse(
+        {"error": True, "description": "Please configure API_TOKEN in settings.py before accessing this view."}
+    )
 
 
 @never_cache
 @staff_member_required
 def jobs(request, queue_index):
     queue_index = int(queue_index)
     queue = get_queue_by_index(queue_index)
@@ -230,16 +226,15 @@
 @never_cache
 @staff_member_required
 def workers(request, queue_index):
     queue_index = int(queue_index)
     queue = get_queue_by_index(queue_index)
     clean_worker_registry(queue)
     all_workers = Worker.all(queue.connection)
-    workers = [worker for worker in all_workers
-               if queue.name in worker.queue_names()]
+    workers = [worker for worker in all_workers if queue.name in worker.queue_names()]
 
     context_data = {
         **admin.site.each_context(request),
         'queue': queue,
         'queue_index': queue_index,
         'workers': workers,
     }
@@ -260,15 +255,15 @@
     context_data = {
         **admin.site.each_context(request),
         'queue': queue,
         'queue_index': queue_index,
         'worker': worker,
         'queue_names': queue_names,
         'job': worker.get_current_job(),
-        'total_working_time': worker.total_working_time * 1000
+        'total_working_time': worker.total_working_time * 1000,
     }
     return render(request, 'django_rq/worker_details.html', context_data)
 
 
 @never_cache
 @staff_member_required
 def deferred_jobs(request, queue_index):
@@ -327,15 +322,15 @@
     except:
         data_is_valid = False
 
     # Backward compatibility support for RQ < 1.12.0
     rv = job.connection.hget(job.key, 'result')
     if rv is not None:
         # cache the result
-        job.legacy_result = job.serializer.loads(rv)    
+        job.legacy_result = job.serializer.loads(rv)
     try:
         exc_info = job._exc_info
     except AttributeError:
         exc_info = None
 
     context_data = {
         **admin.site.each_context(request),
@@ -401,15 +396,18 @@
 
     if request.method == 'POST':
         try:
             queue.empty()
             messages.info(request, 'You have successfully cleared the queue %s' % queue.name)
         except ResponseError as e:
             if 'EVALSHA' in e.message:
-                messages.error(request, 'This action is not supported on Redis versions < 2.6.0, please use the bulk delete command instead')
+                messages.error(
+                    request,
+                    'This action is not supported on Redis versions < 2.6.0, please use the bulk delete command instead',
+                )
             else:
                 raise e
         return redirect('rq_jobs', queue_index)
 
     context_data = {
         **admin.site.each_context(request),
         'queue_index': queue_index,
@@ -498,22 +496,26 @@
 
     return redirect(next_url)
 
 
 @never_cache
 @staff_member_required
 def enqueue_job(request, queue_index, job_id):
-    """ Enqueue deferred jobs
-    """
+    """Enqueue deferred jobs"""
     queue_index = int(queue_index)
     queue = get_queue_by_index(queue_index)
     job = Job.fetch(job_id, connection=queue.connection)
 
     if request.method == 'POST':
-        queue.enqueue_job(job)
+        try:
+            # _enqueue_job is new in RQ 1.14, this is used to enqueue
+            # job regardless of its dependencies
+            queue._enqueue_job(job)
+        except AttributeError:
+            queue.enqueue_job(job)
 
         # Remove job from correct registry if needed
         if job.get_status() == JobStatus.DEFERRED:
             registry = DeferredJobRegistry(queue.name, queue.connection)
             registry.remove(job)
         elif job.get_status() == JobStatus.FINISHED:
             registry = FinishedJobRegistry(queue.name, queue.connection)
```

### Comparing `django-rq-2.7.0/django_rq/workers.py` & `django-rq-2.8.0/django_rq/workers.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,18 +39,19 @@
 
 def get_worker(*queue_names, **kwargs):
     """
     Returns a RQ worker for all queues or specified ones.
     """
     job_class = get_job_class(kwargs.pop('job_class', None))
     queue_class = kwargs.pop('queue_class', None)
-    queues = get_queues(*queue_names, **{'job_class': job_class,
-                                         'queue_class': queue_class})
+    queues = get_queues(*queue_names, **{'job_class': job_class, 'queue_class': queue_class})
     # normalize queue_class to what get_queues returns
     queue_class = queues[0].__class__
     worker_class = get_worker_class(kwargs.pop('worker_class', None))
-    return worker_class(queues,
-                        connection=queues[0].connection,
-                        exception_handlers=get_exception_handlers() or None,
-                        job_class=job_class,
-                        queue_class=queue_class,
-                        **kwargs)
+    return worker_class(
+        queues,
+        connection=queues[0].connection,
+        exception_handlers=get_exception_handlers() or None,
+        job_class=job_class,
+        queue_class=queue_class,
+        **kwargs
+    )
```

### Comparing `django-rq-2.7.0/django_rq.egg-info/PKG-INFO` & `django-rq-2.8.0/django_rq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-rq
-Version: 2.7.0
+Version: 2.8.0
 Summary: An app that provides django integration for RQ (Redis Queue)
 Home-page: https://github.com/rq/django-rq
 Author: Selwin Ong
 Author-email: selwin.ong@gmail.com
 License: MIT
 Description: =========
         Django-RQ
@@ -54,25 +54,36 @@
         .. code-block:: python
         
             RQ_QUEUES = {
                 'default': {
                     'HOST': 'localhost',
                     'PORT': 6379,
                     'DB': 0,
+                    'USERNAME': 'some-user',
                     'PASSWORD': 'some-password',
                     'DEFAULT_TIMEOUT': 360,
+                    'REDIS_CLIENT_KWARGS': {    # Eventual additional Redis connection arguments
+                        'ssl_cert_reqs': None,
+                    },
                 },
                 'with-sentinel': {
                     'SENTINELS': [('localhost', 26736), ('localhost', 26737)],
                     'MASTER_NAME': 'redismaster',
                     'DB': 0,
+                    # Redis username/password
+                    'USERNAME': 'redis-user',
                     'PASSWORD': 'secret',
-                    'SOCKET_TIMEOUT': None,
-                    'CONNECTION_KWARGS': {
-                        'socket_connect_timeout': 0.3
+                    'SOCKET_TIMEOUT': 0.3,
+                    'CONNECTION_KWARGS': {  # Eventual additional Redis connection arguments
+                        'ssl': True
+                    }
+                    'SENTINEL_KWARGS': {    # Eventual Sentinel connection arguments
+                        # If Sentinel also has auth, username/password can be passed here
+                        'username': 'sentinel-user',
+                        'password': 'secret',
                     },
                 },
                 'high': {
                     'URL': os.getenv('REDISTOGO_URL', 'redis://localhost:6379/0'), # If you're on Heroku
                     'DEFAULT_TIMEOUT': 500,
                 },
                 'low': {
@@ -354,16 +365,15 @@
                 'integrations': [RedisIntegration(), RqIntegration(), DjangoIntegration()]
             }
         
         
         Configuring Logging
         -------------------
         
-        Starting from version 0.3.3, RQ uses Python's ``logging``, this means
-        you can easily configure ``rqworker``'s logging mechanism in django's
+        RQ uses Python's ``logging``, this means you can easily configure ``rqworker``'s logging mechanism in django's
         ``settings.py``. For example:
         
         .. code-block:: python
         
             LOGGING = {
                 "version": 1,
                 "disable_existing_loggers": False,
@@ -372,15 +382,15 @@
                         "format": "%(asctime)s %(message)s",
                         "datefmt": "%H:%M:%S",
                     },
                 },
                 "handlers": {
                     "rq_console": {
                         "level": "DEBUG",
-                        "class": "rq.utils.ColorizingStreamHandler",
+                        "class": "rq.logutils.ColorizingStreamHandler",
                         "formatter": "rq_console",
                         "exclude": ["%(asctime)s"],
                     },
                     # If you use sentry for logging
                     'sentry': {
                         'level': 'ERROR',
                         'class': 'raven.contrib.django.handlers.SentryHandler',
@@ -497,15 +507,15 @@
         
         =============
         Running Tests
         =============
         
         To run ``django_rq``'s test suite::
         
-            `which django-admin.py` test django_rq --settings=django_rq.tests.settings --pythonpath=.
+            `which django-admin` test django_rq --settings=django_rq.tests.settings --pythonpath=.
         
         ===================
         Deploying on Ubuntu
         ===================
         
         Create an rqworker service that runs the high, default, and low queues.
```

### Comparing `django-rq-2.7.0/django_rq.egg-info/SOURCES.txt` & `django-rq-2.8.0/django_rq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-rq-2.7.0/setup.py` & `django-rq-2.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 setup(
     name='django-rq',
-    version='2.7.0',
+    version='2.8.0',
     author='Selwin Ong',
     author_email='selwin.ong@gmail.com',
     packages=['django_rq'],
     url='https://github.com/rq/django-rq',
     license='MIT',
     description='An app that provides django integration for RQ (Redis Queue)',
     long_description=open('README.rst').read(),
```

