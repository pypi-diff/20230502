# Comparing `tmp/Bigsansar-1.2.8.tar.gz` & `tmp/Bigsansar-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Bigsansar-1.2.8.tar", last modified: Tue May  2 11:50:28 2023, max compression
+gzip compressed data, was "Bigsansar-1.2.9.tar", last modified: Tue May  2 12:08:36 2023, max compression
```

## Comparing `Bigsansar-1.2.8.tar` & `Bigsansar-1.2.9.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 11:50:28.628887 Bigsansar-1.2.8/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 11:50:28.578887 Bigsansar-1.2.8/Bigsansar.egg-info/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3121 2023-05-02 11:50:28.000000 Bigsansar-1.2.8/Bigsansar.egg-info/PKG-INFO
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2367 2023-05-02 11:50:28.000000 Bigsansar-1.2.8/Bigsansar.egg-info/SOURCES.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        1 2023-05-02 11:50:28.000000 Bigsansar-1.2.8/Bigsansar.egg-info/dependency_links.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       51 2023-05-02 11:50:28.000000 Bigsansar-1.2.8/Bigsansar.egg-info/entry_points.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       82 2023-05-02 11:50:28.000000 Bigsansar-1.2.8/Bigsansar.egg-info/requires.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       10 2023-05-02 11:50:28.000000 Bigsansar-1.2.8/Bigsansar.egg-info/top_level.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1091 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/LICENSE
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3121 2023-05-02 11:50:28.628887 Bigsansar-1.2.8/PKG-INFO
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2508 2023-04-29 15:26:29.000000 Bigsansar-1.2.8/README.md
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 11:50:28.588887 Bigsansar-1.2.8/bigsansar/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/apps.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 11:50:28.588887 Bigsansar-1.2.8/bigsansar/contrib/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 11:50:28.598887 Bigsansar-1.2.8/bigsansar/contrib/account/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/account/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      510 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/account/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      284 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/account/apps.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1176 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/account/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 11:50:28.598887 Bigsansar-1.2.8/bigsansar/contrib/account/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      999 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/account/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      417 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/account/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      556 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/account/models.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      351 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/account/signals.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 11:50:28.598887 Bigsansar-1.2.8/bigsansar/contrib/account/templates/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/account/templates/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/account/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/account/urls.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/account/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 11:50:28.598887 Bigsansar-1.2.8/bigsansar/contrib/blogs/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/blogs/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      541 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/blogs/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/blogs/apps.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 11:50:28.608887 Bigsansar-1.2.8/bigsansar/contrib/blogs/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2272 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/blogs/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/blogs/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1572 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/blogs/models.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/blogs/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/blogs/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 11:50:28.618887 Bigsansar-1.2.8/bigsansar/contrib/sites/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/sites/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1734 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/sites/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      203 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/sites/apps.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3018 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/sites/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 11:50:28.618887 Bigsansar-1.2.8/bigsansar/contrib/sites/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1816 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/sites/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      389 2023-04-29 15:17:47.000000 Bigsansar-1.2.8/bigsansar/contrib/sites/migrations/0002_domains_description.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      422 2023-04-30 05:58:24.000000 Bigsansar-1.2.8/bigsansar/contrib/sites/migrations/0003_alter_pages_body.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/sites/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1891 2023-04-29 15:17:38.000000 Bigsansar-1.2.8/bigsansar/contrib/sites/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 11:50:28.618887 Bigsansar-1.2.8/bigsansar/contrib/sites/templatetags/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/sites/templatetags/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      408 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/sites/templatetags/pages.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/sites/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/contrib/sites/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 11:50:28.618887 Bigsansar-1.2.8/bigsansar/core/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      524 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/core/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      414 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/core/host.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     8723 2023-05-02 11:50:10.000000 Bigsansar-1.2.8/bigsansar/core/init.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       27 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/main.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 11:50:28.618887 Bigsansar-1.2.8/bigsansar/management/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/management/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 11:50:28.618887 Bigsansar-1.2.8/bigsansar/management/commands/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/management/commands/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1122 2023-04-27 12:44:33.000000 Bigsansar-1.2.8/bigsansar/management/commands/createuser.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 11:50:28.618887 Bigsansar-1.2.8/bigsansar/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       60 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 11:50:28.618887 Bigsansar-1.2.8/bigsansar/static/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/static/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     9230 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/static/logo.png
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      525 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/static/style.css
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 11:50:28.628887 Bigsansar-1.2.8/bigsansar/templates/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      977 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/templates/404.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/templates/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      168 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/templates/acc_active_email.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1134 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/templates/base.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2252 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/templates/default.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2250 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/templates/defaultpage.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2171 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/templates/nav.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      758 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/templates/parking.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      821 2023-04-27 12:27:15.000000 Bigsansar-1.2.8/bigsansar/urls.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1908 2023-05-02 11:45:28.000000 Bigsansar-1.2.8/bigsansar/views.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       38 2023-05-02 11:50:28.628887 Bigsansar-1.2.8/setup.cfg
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1294 2023-05-02 11:47:52.000000 Bigsansar-1.2.8/setup.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 12:08:36.358882 Bigsansar-1.2.9/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 12:08:36.308882 Bigsansar-1.2.9/Bigsansar.egg-info/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3121 2023-05-02 12:08:36.000000 Bigsansar-1.2.9/Bigsansar.egg-info/PKG-INFO
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2367 2023-05-02 12:08:36.000000 Bigsansar-1.2.9/Bigsansar.egg-info/SOURCES.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        1 2023-05-02 12:08:36.000000 Bigsansar-1.2.9/Bigsansar.egg-info/dependency_links.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       51 2023-05-02 12:08:36.000000 Bigsansar-1.2.9/Bigsansar.egg-info/entry_points.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       82 2023-05-02 12:08:36.000000 Bigsansar-1.2.9/Bigsansar.egg-info/requires.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       10 2023-05-02 12:08:36.000000 Bigsansar-1.2.9/Bigsansar.egg-info/top_level.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1091 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/LICENSE
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3121 2023-05-02 12:08:36.358882 Bigsansar-1.2.9/PKG-INFO
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2508 2023-04-29 15:26:29.000000 Bigsansar-1.2.9/README.md
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 12:08:36.318882 Bigsansar-1.2.9/bigsansar/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/apps.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 12:08:36.318882 Bigsansar-1.2.9/bigsansar/contrib/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/contrib/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 12:08:36.318882 Bigsansar-1.2.9/bigsansar/contrib/account/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/contrib/account/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      510 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/contrib/account/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      284 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/contrib/account/apps.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1176 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/contrib/account/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 12:08:36.328882 Bigsansar-1.2.9/bigsansar/contrib/account/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      999 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/contrib/account/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      417 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/contrib/account/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      556 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/contrib/account/models.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      351 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/contrib/account/signals.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 12:08:36.328882 Bigsansar-1.2.9/bigsansar/contrib/account/templates/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/contrib/account/templates/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/contrib/account/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/contrib/account/urls.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/contrib/account/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 12:08:36.328882 Bigsansar-1.2.9/bigsansar/contrib/blogs/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/contrib/blogs/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      541 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/contrib/blogs/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/contrib/blogs/apps.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 12:08:36.328882 Bigsansar-1.2.9/bigsansar/contrib/blogs/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2272 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/contrib/blogs/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/contrib/blogs/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1572 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/contrib/blogs/models.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/contrib/blogs/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/contrib/blogs/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 12:08:36.328882 Bigsansar-1.2.9/bigsansar/contrib/sites/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/contrib/sites/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1734 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/contrib/sites/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      203 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/contrib/sites/apps.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3033 2023-05-02 11:56:47.000000 Bigsansar-1.2.9/bigsansar/contrib/sites/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 12:08:36.328882 Bigsansar-1.2.9/bigsansar/contrib/sites/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1816 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/contrib/sites/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      389 2023-04-29 15:17:47.000000 Bigsansar-1.2.9/bigsansar/contrib/sites/migrations/0002_domains_description.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      422 2023-04-30 05:58:24.000000 Bigsansar-1.2.9/bigsansar/contrib/sites/migrations/0003_alter_pages_body.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/contrib/sites/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1891 2023-04-29 15:17:38.000000 Bigsansar-1.2.9/bigsansar/contrib/sites/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 12:08:36.338882 Bigsansar-1.2.9/bigsansar/contrib/sites/templatetags/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/contrib/sites/templatetags/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      408 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/contrib/sites/templatetags/pages.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/contrib/sites/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/contrib/sites/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 12:08:36.338882 Bigsansar-1.2.9/bigsansar/core/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      524 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/core/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      414 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/core/host.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     8722 2023-05-02 12:07:32.000000 Bigsansar-1.2.9/bigsansar/core/init.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       27 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/main.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 12:08:36.338882 Bigsansar-1.2.9/bigsansar/management/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/management/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 12:08:36.338882 Bigsansar-1.2.9/bigsansar/management/commands/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/management/commands/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1122 2023-04-27 12:44:33.000000 Bigsansar-1.2.9/bigsansar/management/commands/createuser.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 12:08:36.338882 Bigsansar-1.2.9/bigsansar/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       60 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 12:08:36.338882 Bigsansar-1.2.9/bigsansar/static/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/static/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     9230 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/static/logo.png
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      525 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/static/style.css
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-05-02 12:08:36.358882 Bigsansar-1.2.9/bigsansar/templates/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      977 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/templates/404.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/templates/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      168 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/templates/acc_active_email.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1134 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/templates/base.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2252 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/templates/default.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2250 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/templates/defaultpage.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2171 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/templates/nav.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      758 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/templates/parking.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      821 2023-04-27 12:27:15.000000 Bigsansar-1.2.9/bigsansar/urls.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1908 2023-05-02 11:45:28.000000 Bigsansar-1.2.9/bigsansar/views.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       38 2023-05-02 12:08:36.358882 Bigsansar-1.2.9/setup.cfg
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1294 2023-05-02 12:07:45.000000 Bigsansar-1.2.9/setup.py
```

### Comparing `Bigsansar-1.2.8/Bigsansar.egg-info/PKG-INFO` & `Bigsansar-1.2.9/Bigsansar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bigsansar
-Version: 1.2.8
+Version: 1.2.9
 Summary: Build one in minutes with bigsansar - a visual site building tool!
 Home-page: https://bigsansar.com
 Author: Bikash Pokhrel
 Author-email: bigsansaroffice@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
 Project-URL: Documentations, https://docs.bigsansar.com/
```

### Comparing `Bigsansar-1.2.8/Bigsansar.egg-info/SOURCES.txt` & `Bigsansar-1.2.9/Bigsansar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.8/LICENSE` & `Bigsansar-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.8/PKG-INFO` & `Bigsansar-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bigsansar
-Version: 1.2.8
+Version: 1.2.9
 Summary: Build one in minutes with bigsansar - a visual site building tool!
 Home-page: https://bigsansar.com
 Author: Bikash Pokhrel
 Author-email: bigsansaroffice@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
 Project-URL: Documentations, https://docs.bigsansar.com/
```

### Comparing `Bigsansar-1.2.8/README.md` & `Bigsansar-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.8/bigsansar/contrib/account/forms.py` & `Bigsansar-1.2.9/bigsansar/contrib/account/forms.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.8/bigsansar/contrib/account/migrations/0001_initial.py` & `Bigsansar-1.2.9/bigsansar/contrib/account/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.8/bigsansar/contrib/account/models.py` & `Bigsansar-1.2.9/bigsansar/contrib/account/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.8/bigsansar/contrib/blogs/admin.py` & `Bigsansar-1.2.9/bigsansar/contrib/blogs/admin.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.8/bigsansar/contrib/blogs/migrations/0001_initial.py` & `Bigsansar-1.2.9/bigsansar/contrib/blogs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.8/bigsansar/contrib/blogs/models.py` & `Bigsansar-1.2.9/bigsansar/contrib/blogs/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.8/bigsansar/contrib/sites/admin.py` & `Bigsansar-1.2.9/bigsansar/contrib/sites/admin.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.8/bigsansar/contrib/sites/forms.py` & `Bigsansar-1.2.9/bigsansar/contrib/sites/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 class create_domainform(forms.ModelForm):
     domain = forms.CharField(max_length=100, min_length=3, validators=[
         RegexValidator('^[a-z0-9.]+\.[a-z0-9]{1,5}$', message='Please enter your correct domain name')],
                              widget=forms.TextInput(attrs={'autofocus': True, 'class': 'form-control', }))
 
     class Meta:
         model = domains
-        fields = ('domain', 'user',)
+        fields = ('domain', 'Description', 'user',)
 
 
 class customaddpageform(forms.ModelForm):
     class Meta:
         model = pages
         fields = '__all__'
         exclude = ('body',)
```

### Comparing `Bigsansar-1.2.8/bigsansar/contrib/sites/migrations/0001_initial.py` & `Bigsansar-1.2.9/bigsansar/contrib/sites/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.8/bigsansar/contrib/sites/models.py` & `Bigsansar-1.2.9/bigsansar/contrib/sites/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.8/bigsansar/core/__init__.py` & `Bigsansar-1.2.9/bigsansar/core/__init__.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.8/bigsansar/core/init.py` & `Bigsansar-1.2.9/bigsansar/core/init.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
                     code = "    'bigsansar.apps.BigsansarConfig'," \
                            "\n" \
                            "    'bigsansar.contrib.account.apps.AccountConfig'," \
                            "\n" \
                            "    'bigsansar.contrib.sites.apps.SitesConfig'," \
                            "\n" \
-                           "    '#bigsansar.contrib.blogs.apps.BlogsConfig'," \
+                           "    'bigsansar.contrib.blogs.apps.BlogsConfig'," \
                            "\n" \
                            "    'ckeditor'," \
                            "\n"
 
                     lines.insert(x, code)
 
                 elif line.find('MIDDLEWARE = [') != -1:
```

### Comparing `Bigsansar-1.2.8/bigsansar/management/commands/createuser.py` & `Bigsansar-1.2.9/bigsansar/management/commands/createuser.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.8/bigsansar/static/logo.png` & `Bigsansar-1.2.9/bigsansar/static/logo.png`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.8/bigsansar/static/style.css` & `Bigsansar-1.2.9/bigsansar/static/style.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.8/bigsansar/templates/404.html` & `Bigsansar-1.2.9/bigsansar/templates/404.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.8/bigsansar/templates/base.html` & `Bigsansar-1.2.9/bigsansar/templates/base.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.8/bigsansar/templates/default.html` & `Bigsansar-1.2.9/bigsansar/templates/default.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.8/bigsansar/templates/defaultpage.html` & `Bigsansar-1.2.9/bigsansar/templates/defaultpage.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.8/bigsansar/templates/nav.html` & `Bigsansar-1.2.9/bigsansar/templates/nav.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.8/bigsansar/templates/parking.html` & `Bigsansar-1.2.9/bigsansar/templates/parking.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.8/bigsansar/urls.py` & `Bigsansar-1.2.9/bigsansar/urls.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.8/bigsansar/views.py` & `Bigsansar-1.2.9/bigsansar/views.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.2.8/setup.py` & `Bigsansar-1.2.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="Bigsansar",
-    version="1.2.8",
+    version="1.2.9",
     author="Bikash Pokhrel",
     author_email="bigsansaroffice@gmail.com",
     description="Build one in minutes with bigsansar - a visual site building tool!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bigsansar.com",
     project_urls={
```

