# Comparing `tmp/Bigsansar-1.2.7.tar.gz` & `tmp/Bigsansar-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Bigsansar-1.2.7.tar", last modified: Mon May  1 11:06:07 2023, max compression
+gzip compressed data, was "Bigsansar-1.2.8.tar", last modified: Tue May  2 11:50:28 2023, max compression
```

## Comparing `Bigsansar-1.2.7.tar` & `Bigsansar-1.2.8.tar`

### file list

```diff
@@ -1,82 +1,90 @@
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-01 11:06:07.590059 Bigsansar-1.2.7/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-01 11:06:07.570059 Bigsansar-1.2.7/Bigsansar.egg-info/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3121 2023-05-01 11:06:07.000000 Bigsansar-1.2.7/Bigsansar.egg-info/PKG-INFO
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2116 2023-05-01 11:06:07.000000 Bigsansar-1.2.7/Bigsansar.egg-info/SOURCES.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        1 2023-05-01 11:06:07.000000 Bigsansar-1.2.7/Bigsansar.egg-info/dependency_links.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       51 2023-05-01 11:06:07.000000 Bigsansar-1.2.7/Bigsansar.egg-info/entry_points.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       75 2023-05-01 11:06:07.000000 Bigsansar-1.2.7/Bigsansar.egg-info/requires.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       10 2023-05-01 11:06:07.000000 Bigsansar-1.2.7/Bigsansar.egg-info/top_level.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1091 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/LICENSE
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3121 2023-05-01 11:06:07.590059 Bigsansar-1.2.7/PKG-INFO
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2508 2023-04-29 15:26:29.000000 Bigsansar-1.2.7/README.md
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-01 11:06:07.570059 Bigsansar-1.2.7/bigsansar/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/apps.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-01 11:06:07.570059 Bigsansar-1.2.7/bigsansar/contrib/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/contrib/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-01 11:06:07.570059 Bigsansar-1.2.7/bigsansar/contrib/account/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/contrib/account/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      510 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/contrib/account/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      284 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/contrib/account/apps.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1176 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/contrib/account/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-01 11:06:07.570059 Bigsansar-1.2.7/bigsansar/contrib/account/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      999 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/contrib/account/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      417 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/contrib/account/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      556 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/contrib/account/models.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      351 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/contrib/account/signals.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-01 11:06:07.570059 Bigsansar-1.2.7/bigsansar/contrib/account/templates/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/contrib/account/templates/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/contrib/account/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/contrib/account/urls.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/contrib/account/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-01 11:06:07.580059 Bigsansar-1.2.7/bigsansar/contrib/sites/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/contrib/sites/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1393 2023-04-30 07:03:51.000000 Bigsansar-1.2.7/bigsansar/contrib/sites/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      203 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/contrib/sites/apps.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      721 2023-04-30 07:01:55.000000 Bigsansar-1.2.7/bigsansar/contrib/sites/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-01 11:06:07.580059 Bigsansar-1.2.7/bigsansar/contrib/sites/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1816 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/contrib/sites/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      387 2023-04-29 15:42:28.000000 Bigsansar-1.2.7/bigsansar/contrib/sites/migrations/0002_domains_description.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      422 2023-04-30 05:58:24.000000 Bigsansar-1.2.7/bigsansar/contrib/sites/migrations/0003_alter_pages_body.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/contrib/sites/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1954 2023-04-30 05:57:56.000000 Bigsansar-1.2.7/bigsansar/contrib/sites/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-01 11:06:07.580059 Bigsansar-1.2.7/bigsansar/contrib/sites/templatetags/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/contrib/sites/templatetags/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      408 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/contrib/sites/templatetags/pages.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/contrib/sites/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/contrib/sites/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-01 11:06:07.580059 Bigsansar-1.2.7/bigsansar/core/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      524 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/core/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      414 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/core/host.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     9177 2023-04-30 08:01:38.000000 Bigsansar-1.2.7/bigsansar/core/init.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       27 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/main.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-01 11:06:07.580059 Bigsansar-1.2.7/bigsansar/management/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/management/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-01 11:06:07.580059 Bigsansar-1.2.7/bigsansar/management/commands/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/management/commands/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1122 2023-04-27 12:44:33.000000 Bigsansar-1.2.7/bigsansar/management/commands/createuser.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-01 11:06:07.580059 Bigsansar-1.2.7/bigsansar/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       60 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-01 11:06:07.590059 Bigsansar-1.2.7/bigsansar/static/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/static/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     9230 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/static/logo.png
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      525 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/static/style.css
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-01 11:06:07.590059 Bigsansar-1.2.7/bigsansar/templates/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      977 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/templates/404.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/templates/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      168 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/templates/acc_active_email.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1134 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/templates/base.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2252 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/templates/default.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2250 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/templates/defaultpage.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2171 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/templates/nav.html
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-01 11:06:07.590059 Bigsansar-1.2.7/bigsansar/templates/page/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      289 2023-05-01 11:03:31.000000 Bigsansar-1.2.7/bigsansar/templates/page/default.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      758 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/templates/parking.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.2.7/bigsansar/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1046 2023-04-30 07:26:30.000000 Bigsansar-1.2.7/bigsansar/urls.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1427 2023-05-01 11:05:48.000000 Bigsansar-1.2.7/bigsansar/views.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       38 2023-05-01 11:06:07.590059 Bigsansar-1.2.7/setup.cfg
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1304 2023-05-01 11:05:53.000000 Bigsansar-1.2.7/setup.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 11:50:28.628887 Bigsansar-1.2.8/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 11:50:28.578887 Bigsansar-1.2.8/Bigsansar.egg-info/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3121 2023-05-02 11:50:28.000000 Bigsansar-1.2.8/Bigsansar.egg-info/PKG-INFO
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2367 2023-05-02 11:50:28.000000 Bigsansar-1.2.8/Bigsansar.egg-info/SOURCES.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        1 2023-05-02 11:50:28.000000 Bigsansar-1.2.8/Bigsansar.egg-info/dependency_links.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       51 2023-05-02 11:50:28.000000 Bigsansar-1.2.8/Bigsansar.egg-info/entry_points.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       82 2023-05-02 11:50:28.000000 Bigsansar-1.2.8/Bigsansar.egg-info/requires.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       10 2023-05-02 11:50:28.000000 Bigsansar-1.2.8/Bigsansar.egg-info/top_level.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1091 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/LICENSE
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3121 2023-05-02 11:50:28.628887 Bigsansar-1.2.8/PKG-INFO
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2508 2023-04-29 15:26:29.000000 Bigsansar-1.2.8/README.md
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 11:50:28.588887 Bigsansar-1.2.8/bigsansar/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/apps.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 11:50:28.588887 Bigsansar-1.2.8/bigsansar/contrib/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 11:50:28.598887 Bigsansar-1.2.8/bigsansar/contrib/account/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/account/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      510 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/account/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      284 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/account/apps.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1176 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/account/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 11:50:28.598887 Bigsansar-1.2.8/bigsansar/contrib/account/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      999 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/account/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      417 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/account/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      556 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/account/models.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      351 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/account/signals.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 11:50:28.598887 Bigsansar-1.2.8/bigsansar/contrib/account/templates/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/account/templates/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/account/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/account/urls.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/account/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 11:50:28.598887 Bigsansar-1.2.8/bigsansar/contrib/blogs/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/blogs/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      541 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/blogs/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/blogs/apps.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 11:50:28.608887 Bigsansar-1.2.8/bigsansar/contrib/blogs/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2272 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/blogs/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/blogs/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1572 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/blogs/models.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/blogs/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/blogs/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 11:50:28.618887 Bigsansar-1.2.8/bigsansar/contrib/sites/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/sites/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1734 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/sites/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      203 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/sites/apps.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3018 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/sites/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 11:50:28.618887 Bigsansar-1.2.8/bigsansar/contrib/sites/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1816 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/sites/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      389 2023-04-29 15:17:47.000000 Bigsansar-1.2.8/bigsansar/contrib/sites/migrations/0002_domains_description.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      422 2023-04-30 05:58:24.000000 Bigsansar-1.2.8/bigsansar/contrib/sites/migrations/0003_alter_pages_body.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/sites/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1891 2023-04-29 15:17:38.000000 Bigsansar-1.2.8/bigsansar/contrib/sites/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 11:50:28.618887 Bigsansar-1.2.8/bigsansar/contrib/sites/templatetags/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/sites/templatetags/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      408 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/sites/templatetags/pages.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/sites/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/sites/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 11:50:28.618887 Bigsansar-1.2.8/bigsansar/core/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      524 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/core/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      414 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/core/host.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     8723 2023-05-02 11:50:10.000000 Bigsansar-1.2.8/bigsansar/core/init.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       27 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/main.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 11:50:28.618887 Bigsansar-1.2.8/bigsansar/management/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/management/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 11:50:28.618887 Bigsansar-1.2.8/bigsansar/management/commands/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/management/commands/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1122 2023-04-27 12:44:33.000000 Bigsansar-1.2.8/bigsansar/management/commands/createuser.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 11:50:28.618887 Bigsansar-1.2.8/bigsansar/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       60 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 11:50:28.618887 Bigsansar-1.2.8/bigsansar/static/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/static/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     9230 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/static/logo.png
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      525 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/static/style.css
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 11:50:28.628887 Bigsansar-1.2.8/bigsansar/templates/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      977 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/templates/404.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/templates/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      168 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/templates/acc_active_email.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1134 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/templates/base.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2252 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/templates/default.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2250 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/templates/defaultpage.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2171 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/templates/nav.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      758 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/templates/parking.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      821 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/urls.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1908 2023-05-02 11:45:28.000000 Bigsansar-1.2.8/bigsansar/views.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       38 2023-05-02 11:50:28.628887 Bigsansar-1.2.8/setup.cfg
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1294 2023-05-02 11:47:52.000000 Bigsansar-1.2.8/setup.py
```

### Comparing `Bigsansar-1.2.7/Bigsansar.egg-info/PKG-INFO` & `Bigsansar-1.2.8/Bigsansar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bigsansar
-Version: 1.2.7
+Version: 1.2.8
 Summary: Build one in minutes with bigsansar - a visual site building tool!
 Home-page: https://bigsansar.com
 Author: Bikash Pokhrel
 Author-email: bigsansaroffice@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
 Project-URL: Documentations, https://docs.bigsansar.com/
```

### Comparing `Bigsansar-1.2.7/Bigsansar.egg-info/SOURCES.txt` & `Bigsansar-1.2.8/Bigsansar.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 LICENSE
 README.md
-setup.cfg
 setup.py
 Bigsansar.egg-info/PKG-INFO
 Bigsansar.egg-info/SOURCES.txt
 Bigsansar.egg-info/dependency_links.txt
 Bigsansar.egg-info/entry_points.txt
 Bigsansar.egg-info/requires.txt
 Bigsansar.egg-info/top_level.txt
@@ -26,14 +25,22 @@
 bigsansar/contrib/account/tests.py
 bigsansar/contrib/account/urls.py
 bigsansar/contrib/account/views.py
 bigsansar/contrib/account/migrations/0001_initial.py
 bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
 bigsansar/contrib/account/migrations/__init__.py
 bigsansar/contrib/account/templates/__init__.py
+bigsansar/contrib/blogs/__init__.py
+bigsansar/contrib/blogs/admin.py
+bigsansar/contrib/blogs/apps.py
+bigsansar/contrib/blogs/models.py
+bigsansar/contrib/blogs/tests.py
+bigsansar/contrib/blogs/views.py
+bigsansar/contrib/blogs/migrations/0001_initial.py
+bigsansar/contrib/blogs/migrations/__init__.py
 bigsansar/contrib/sites/__init__.py
 bigsansar/contrib/sites/admin.py
 bigsansar/contrib/sites/apps.py
 bigsansar/contrib/sites/forms.py
 bigsansar/contrib/sites/models.py
 bigsansar/contrib/sites/tests.py
 bigsansar/contrib/sites/views.py
@@ -56,9 +63,8 @@
 bigsansar/templates/404.html
 bigsansar/templates/__init__.py
 bigsansar/templates/acc_active_email.html
 bigsansar/templates/base.html
 bigsansar/templates/default.html
 bigsansar/templates/defaultpage.html
 bigsansar/templates/nav.html
-bigsansar/templates/parking.html
-bigsansar/templates/page/default.html
+bigsansar/templates/parking.html
```

### Comparing `Bigsansar-1.2.7/LICENSE` & `Bigsansar-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.7/PKG-INFO` & `Bigsansar-1.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bigsansar
-Version: 1.2.7
+Version: 1.2.8
 Summary: Build one in minutes with bigsansar - a visual site building tool!
 Home-page: https://bigsansar.com
 Author: Bikash Pokhrel
 Author-email: bigsansaroffice@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
 Project-URL: Documentations, https://docs.bigsansar.com/
```

### Comparing `Bigsansar-1.2.7/README.md` & `Bigsansar-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.7/bigsansar/contrib/account/forms.py` & `Bigsansar-1.2.8/bigsansar/contrib/account/forms.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.7/bigsansar/contrib/account/migrations/0001_initial.py` & `Bigsansar-1.2.8/bigsansar/contrib/account/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.7/bigsansar/contrib/account/models.py` & `Bigsansar-1.2.8/bigsansar/contrib/account/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.7/bigsansar/contrib/sites/admin.py` & `Bigsansar-1.2.8/bigsansar/contrib/sites/admin.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from django.contrib import admin
 from django.contrib.admin import SimpleListFilter
 from django.utils.translation import gettext_lazy as _
-from bigsansar.contrib.sites.forms import create_domainform
+from bigsansar.contrib.sites.forms import create_domainform, customaddpageform, custompageform
 from bigsansar.contrib.sites.models import domains, pages
 
 
 # Register your models here.
 
 
 class domain_filter(SimpleListFilter):
@@ -26,17 +26,26 @@
 
 class domainadmin(admin.ModelAdmin):
     form = create_domainform
     list_display = ['domain', 'publish_date', 'visitor']
 
 
 class pageadmin(admin.ModelAdmin):
-    #add_form = customaddpageform
-    #form = custompageform
+    add_form = customaddpageform
+    form = custompageform
     prepopulated_fields = {"slug": ("title",)}
     list_display = ['title', 'domain', 'publish_date', 'visitor']
     list_filter = (domain_filter,)
 
-    
+    def get_form(self, request, obj=None, **kwargs):
+        """
+        Use special form during foo creation
+        """
+        defaults = {}
+        if obj is None:
+            defaults['form'] = self.add_form
+        defaults.update(kwargs)
+        return super().get_form(request, obj, **defaults)
+
 
 admin.site.register(domains, domainadmin)
 admin.site.register(pages, pageadmin)
```

### Comparing `Bigsansar-1.2.7/bigsansar/contrib/sites/migrations/0001_initial.py` & `Bigsansar-1.2.8/bigsansar/contrib/sites/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.7/bigsansar/contrib/sites/models.py` & `Bigsansar-1.2.8/bigsansar/contrib/sites/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os
 import shutil
 
 from django.contrib.auth.models import User
 from django.db import models
-from ckeditor_uploader.fields import RichTextUploadingField
+
 from www.settings import BASE_DIR
 
 
 # Create your models here.
 
 
 class domains(models.Model):
     user = models.ForeignKey(User, on_delete=models.CASCADE)
     domain = models.CharField(max_length=100, unique=True)
-    Description = models.CharField(max_length=15, blank=True)
+    Description = models.CharField(max_length=15, default=None)
     publish_date = models.DateField(auto_now_add=True)
     visitor = models.IntegerField(default=1)
 
     def __str__(self):
         return self.domain
 
     class Meta:
@@ -39,15 +39,15 @@
         super().delete()
 
 
 class pages(models.Model):
     domain = models.ForeignKey(domains, on_delete=models.CASCADE)
     title = models.CharField(max_length=50)
     slug = models.SlugField()
-    body = RichTextUploadingField()
+    body = models.TextField()
     visitor = models.IntegerField(default=0)
     publish_date = models.DateField(auto_now_add=True)
 
     class Meta:
         verbose_name = 'Pages'
         verbose_name_plural = 'Pages'
```

### Comparing `Bigsansar-1.2.7/bigsansar/core/__init__.py` & `Bigsansar-1.2.8/bigsansar/core/__init__.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.7/bigsansar/core/init.py` & `Bigsansar-1.2.8/bigsansar/core/init.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,17 +41,17 @@
 
                     code = "    'bigsansar.apps.BigsansarConfig'," \
                            "\n" \
                            "    'bigsansar.contrib.account.apps.AccountConfig'," \
                            "\n" \
                            "    'bigsansar.contrib.sites.apps.SitesConfig'," \
                            "\n" \
-                           "    'ckeditor'," \
+                           "    '#bigsansar.contrib.blogs.apps.BlogsConfig'," \
                            "\n" \
-                           "    'ckeditor_uploader'," \
+                           "    'ckeditor'," \
                            "\n"
 
                     lines.insert(x, code)
 
                 elif line.find('MIDDLEWARE = [') != -1:
 
                     print('Reading the lines MIDDLEWARE = [')
@@ -87,24 +87,14 @@
                                "MEDIA_URL = 'images/'" \
                                "\n" \
                                "\n" \
                                "STATIC_ROOT = BASE_DIR/'static'" \
                                "\n" \
                                "\n" \
                                "SECURE_PROXY_SSL_HEADER = ('HTTP_X_FORWARDED_PROTO', 'https')" \
-                               "\n" \
-                               "\n" \
-                               "CKEDITOR_UPLOAD_PATH = ''" \
-                               "\n" \
-                               "\n" \
-                               "CKEDITOR_RESTRICT_BY_USER = True" \
-                               "\n" \
-                               "\n" \
-                               "CKEDITOR_ALLOW_NONIMAGE_FILES = False" \
-                               "\n" \
                                "\n"
 
                     lines.insert(xyz, hostcode)
 
                 elif line.find("ROOT_URLCONF = 'www.urls'") != -1:
                     rooturlindex = lines.index(line)
```

### Comparing `Bigsansar-1.2.7/bigsansar/management/commands/createuser.py` & `Bigsansar-1.2.8/bigsansar/management/commands/createuser.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.7/bigsansar/static/logo.png` & `Bigsansar-1.2.8/bigsansar/static/logo.png`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.7/bigsansar/static/style.css` & `Bigsansar-1.2.8/bigsansar/static/style.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.7/bigsansar/templates/404.html` & `Bigsansar-1.2.8/bigsansar/templates/404.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.7/bigsansar/templates/base.html` & `Bigsansar-1.2.8/bigsansar/templates/base.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.7/bigsansar/templates/default.html` & `Bigsansar-1.2.8/bigsansar/templates/default.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.7/bigsansar/templates/defaultpage.html` & `Bigsansar-1.2.8/bigsansar/templates/defaultpage.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.7/bigsansar/templates/nav.html` & `Bigsansar-1.2.8/bigsansar/templates/nav.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.7/bigsansar/templates/parking.html` & `Bigsansar-1.2.8/bigsansar/templates/parking.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.7/bigsansar/urls.py` & `Bigsansar-1.2.8/bigsansar/urls.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,22 +10,16 @@
     1. Add an import:  from other_app.views import Home
     2. Add a URL to urlpatterns:  path('', Home.as_view(), name='home')
 Including another URLconf
     1. Import the include() function: from django.urls import include, path
     2. Add a URL to urlpatterns:  path('blog/', include('blog.urls'))
 """
 
-from django.conf import settings
-from django.urls import include, path
-from django.conf.urls.static import static
+from django.urls import path
 
 from bigsansar import views
 
 urlpatterns = [
-    path('files/', include('ckeditor_uploader.urls')),
     path('', views.index, name='index'),
     path('<url>', views.pathviews, name='path'),
 
 ]
-
-urlpatterns += static(settings.MEDIA_URL, document_root=settings.MEDIA_ROOT)
-
```

### Comparing `Bigsansar-1.2.7/setup.py` & `Bigsansar-1.2.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="Bigsansar",
-    version="1.2.7",
+    version="1.2.8",
     author="Bikash Pokhrel",
     author_email="bigsansaroffice@gmail.com",
     description="Build one in minutes with bigsansar - a visual site building tool!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bigsansar.com",
     project_urls={
@@ -19,19 +19,19 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 
     packages=setuptools.find_packages(),
-    package_data={'': ['templates/*', 'templates/page/*', 'static/*']},
+    package_data={'': ['templates/*', 'static/*']},
 
     entry_points={
         'console_scripts': [
                     'bigsansar = bigsansar.core:main',
                 ],
     },
 
     python_requires=">=3.6",
-    install_requires=['django', 'django-phonenumber-field[phonenumberslite]', 'django-ckeditor', 'requests'],
+    install_requires=['django', 'django-phonenumber-field[phonenumberslite]', 'django-ckeditor', 'requests', 'pillow'],
     keywords=['python', 'django host', 'bigsansar', 'django', 'django sites framework', 'django flatpages']
 )
```

