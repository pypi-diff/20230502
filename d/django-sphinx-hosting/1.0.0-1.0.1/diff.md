# Comparing `tmp/django-sphinx-hosting-1.0.0.tar.gz` & `tmp/django-sphinx-hosting-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sphinx-hosting-1.0.0.tar", last modified: Fri Apr 28 18:37:03 2023, max compression
+gzip compressed data, was "django-sphinx-hosting-1.0.1.tar", last modified: Mon May  1 22:10:47 2023, max compression
```

## Comparing `django-sphinx-hosting-1.0.0.tar` & `django-sphinx-hosting-1.0.1.tar`

### file list

```diff
@@ -1,82 +1,84 @@
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-04-28 18:37:03.888882 django-sphinx-hosting-1.0.0/
--rw-rw-r--   0 cmalek     (501) admin       (80)     1459 2023-04-28 16:31:54.000000 django-sphinx-hosting-1.0.0/LICENSE.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)      177 2023-02-21 21:57:12.000000 django-sphinx-hosting-1.0.0/MANIFEST.in
--rw-rw-r--   0 cmalek     (501) admin       (80)     2207 2023-04-28 18:37:03.889110 django-sphinx-hosting-1.0.0/PKG-INFO
--rw-rw-r--   0 cmalek     (501) admin       (80)     1188 2023-04-28 17:53:11.000000 django-sphinx-hosting-1.0.0/README.md
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-04-28 18:37:03.833571 django-sphinx-hosting-1.0.0/django_sphinx_hosting.egg-info/
--rw-rw-r--   0 cmalek     (501) admin       (80)     2207 2023-04-28 18:37:03.000000 django-sphinx-hosting-1.0.0/django_sphinx_hosting.egg-info/PKG-INFO
--rw-rw-r--   0 cmalek     (501) admin       (80)     2480 2023-04-28 18:37:03.000000 django-sphinx-hosting-1.0.0/django_sphinx_hosting.egg-info/SOURCES.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)        1 2023-04-28 18:37:03.000000 django-sphinx-hosting-1.0.0/django_sphinx_hosting.egg-info/dependency_links.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)      324 2023-04-28 18:37:03.000000 django-sphinx-hosting-1.0.0/django_sphinx_hosting.egg-info/requires.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)       15 2023-04-28 18:37:03.000000 django-sphinx-hosting-1.0.0/django_sphinx_hosting.egg-info/top_level.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)     1256 2023-04-28 18:37:03.890009 django-sphinx-hosting-1.0.0/setup.cfg
--rw-rw-r--   0 cmalek     (501) admin       (80)     1821 2023-04-28 18:36:09.000000 django-sphinx-hosting-1.0.0/setup.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-04-28 18:37:03.843859 django-sphinx-hosting-1.0.0/sphinx_hosting/
--rw-r--r--   0 cmalek     (501) admin       (80)       21 2023-04-28 18:36:09.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/__init__.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-04-28 18:37:03.847148 django-sphinx-hosting-1.0.0/sphinx_hosting/api/
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-10-21 23:25:25.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/api/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)      331 2023-03-28 15:43:43.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/api/apps.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     4896 2023-03-28 15:50:00.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/api/serializers.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     1274 2023-02-22 19:04:46.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/api/urls.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     8676 2023-04-06 17:29:54.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/api/views.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      305 2023-02-22 19:04:46.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/apps.py
--rw-r--r--   0 cmalek     (501) admin       (80)       49 2022-11-03 21:55:52.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/exc.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     6843 2023-04-27 16:25:48.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/forms.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    21291 2023-04-27 16:27:31.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/importers.py
--rw-r--r--   0 cmalek     (501) admin       (80)       62 2022-11-17 22:11:14.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/logging.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-04-28 18:37:03.847841 django-sphinx-hosting-1.0.0/sphinx_hosting/management/
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-03 21:42:32.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/management/__init__.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-04-28 18:37:03.850800 django-sphinx-hosting-1.0.0/sphinx_hosting/management/commands/
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-03 21:42:44.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/management/commands/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     2568 2023-02-22 19:04:46.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/management/commands/import_docs.py
--rw-r--r--   0 cmalek     (501) admin       (80)     1626 2023-02-01 17:53:25.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/management/commands/parse_globaltoc.py
--rw-r--r--   0 cmalek     (501) admin       (80)     1421 2023-02-01 17:06:59.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/management/commands/print_classifier_tree.py
--rw-r--r--   0 cmalek     (501) admin       (80)     2288 2023-02-01 17:06:33.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/management/commands/print_doctree.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-04-28 18:37:03.859265 django-sphinx-hosting-1.0.0/sphinx_hosting/migrations/
--rw-r--r--   0 cmalek     (501) admin       (80)     6366 2022-11-22 19:27:09.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/migrations/0001_initial.py
--rw-r--r--   0 cmalek     (501) admin       (80)     1592 2022-11-22 23:23:38.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/migrations/0002_original_html.py
--rw-r--r--   0 cmalek     (501) admin       (80)      659 2022-12-08 23:32:00.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/migrations/0003_globaltoc.py
--rw-r--r--   0 cmalek     (501) admin       (80)      586 2022-12-09 00:04:04.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/migrations/0004_next_page_FK.py
--rw-r--r--   0 cmalek     (501) admin       (80)      683 2023-01-06 00:23:12.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/migrations/0005_orig_global_toc.py
--rw-r--r--   0 cmalek     (501) admin       (80)     3829 2023-03-24 22:50:14.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/migrations/0006_classifiers_and_permissiongroups.py
--rw-r--r--   0 cmalek     (501) admin       (80)      658 2023-01-19 19:26:47.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/migrations/0007_load_classifiers.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      497 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/migrations/0008_Version_archived.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      857 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/migrations/0009_SphinxPage_searchable.py
--rw-r--r--   0 cmalek     (501) admin       (80)     2858 2023-03-28 21:23:19.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/migrations/0010_add_groups.py
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-04 18:37:19.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/migrations/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    31797 2023-04-28 16:10:05.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/models.py
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-18 23:13:36.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/py.typed
--rw-rw-r--   0 cmalek     (501) admin       (80)     1663 2023-04-27 18:08:13.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/search_indexes.py
--rw-r--r--   0 cmalek     (501) admin       (80)      566 2023-03-24 21:26:47.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/settings.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-04-28 18:37:03.828040 django-sphinx-hosting-1.0.0/sphinx_hosting/static/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-04-28 18:37:03.828402 django-sphinx-hosting-1.0.0/sphinx_hosting/static/sphinx_hosting/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-04-28 18:37:03.863526 django-sphinx-hosting-1.0.0/sphinx_hosting/static/sphinx_hosting/css/
--rw-r--r--   0 cmalek     (501) admin       (80)     1075 2023-02-02 18:58:20.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/static/sphinx_hosting/css/_classifierfilterblock.scss
--rw-r--r--   0 cmalek     (501) admin       (80)     4819 2022-11-22 19:08:46.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/static/sphinx_hosting/css/_pygments.scss
--rw-r--r--   0 cmalek     (501) admin       (80)    18183 2023-01-10 17:44:02.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/static/sphinx_hosting/css/_sphinx_layout.scss
--rw-r--r--   0 cmalek     (501) admin       (80)    34945 2023-02-02 18:58:21.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.css
--rw-r--r--   0 cmalek     (501) admin       (80)     2896 2023-02-01 21:52:48.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.scss
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-04-28 18:37:03.864325 django-sphinx-hosting-1.0.0/sphinx_hosting/static/sphinx_hosting/images/
--rw-r--r--   0 cmalek     (501) admin       (80)    37933 2022-11-17 21:25:05.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/static/sphinx_hosting/images/logo.jpg
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-04-28 18:37:03.829139 django-sphinx-hosting-1.0.0/sphinx_hosting/templates/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-04-28 18:37:03.828838 django-sphinx-hosting-1.0.0/sphinx_hosting/templates/search/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-04-28 18:37:03.828953 django-sphinx-hosting-1.0.0/sphinx_hosting/templates/search/indexes/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-04-28 18:37:03.865380 django-sphinx-hosting-1.0.0/sphinx_hosting/templates/search/indexes/sphinxhostingcore/
--rw-rw-r--   0 cmalek     (501) admin       (80)       36 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/templates/search/indexes/sphinxhostingcore/sphinxpage_text.txt
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-04-28 18:37:03.866069 django-sphinx-hosting-1.0.0/sphinx_hosting/templates/sphinx_hosting/
--rw-r--r--   0 cmalek     (501) admin       (80)      523 2023-01-18 19:41:49.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/templates/sphinx_hosting/base.html
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-10-21 21:37:03.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/types.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     1653 2023-03-28 18:47:58.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/urls.py
--rw-r--r--   0 cmalek     (501) admin       (80)      606 2022-11-02 23:23:01.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/validators.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    20844 2023-04-28 17:09:25.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/views.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-04-28 18:37:03.883111 django-sphinx-hosting-1.0.0/sphinx_hosting/wildewidgets/
--rw-rw-r--   0 cmalek     (501) admin       (80)      255 2023-04-28 16:10:38.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/wildewidgets/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)     6553 2023-04-27 20:10:51.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/wildewidgets/classifier.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-04-28 18:37:03.888462 django-sphinx-hosting-1.0.0/sphinx_hosting/wildewidgets/core/
--rw-r--r--   0 cmalek     (501) admin       (80)       39 2023-01-18 23:39:43.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/wildewidgets/core/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2023-01-18 23:39:52.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/wildewidgets/core/basic.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     4463 2023-04-06 17:29:54.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/wildewidgets/navigation.py
--rw-r--r--   0 cmalek     (501) admin       (80)    14263 2023-04-27 19:40:10.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/wildewidgets/project.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    11411 2023-04-27 20:32:48.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/wildewidgets/search.py
--rw-r--r--   0 cmalek     (501) admin       (80)     7084 2023-04-27 20:42:19.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/wildewidgets/sphinx_page.py
--rw-r--r--   0 cmalek     (501) admin       (80)     8438 2023-04-27 23:13:13.000000 django-sphinx-hosting-1.0.0/sphinx_hosting/wildewidgets/version.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.652818 django-sphinx-hosting-1.0.1/
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1459 2023-04-28 16:31:54.000000 django-sphinx-hosting-1.0.1/LICENSE.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)      221 2023-05-01 22:07:11.000000 django-sphinx-hosting-1.0.1/MANIFEST.in
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2207 2023-05-01 22:10:47.652970 django-sphinx-hosting-1.0.1/PKG-INFO
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1188 2023-04-28 17:53:11.000000 django-sphinx-hosting-1.0.1/README.md
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.605493 django-sphinx-hosting-1.0.1/django_sphinx_hosting.egg-info/
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2207 2023-05-01 22:10:47.000000 django-sphinx-hosting-1.0.1/django_sphinx_hosting.egg-info/PKG-INFO
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2521 2023-05-01 22:10:47.000000 django-sphinx-hosting-1.0.1/django_sphinx_hosting.egg-info/SOURCES.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)        1 2023-05-01 22:10:47.000000 django-sphinx-hosting-1.0.1/django_sphinx_hosting.egg-info/dependency_links.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)      324 2023-05-01 22:10:47.000000 django-sphinx-hosting-1.0.1/django_sphinx_hosting.egg-info/requires.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)       15 2023-05-01 22:10:47.000000 django-sphinx-hosting-1.0.1/django_sphinx_hosting.egg-info/top_level.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1256 2023-05-01 22:10:47.653801 django-sphinx-hosting-1.0.1/setup.cfg
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1821 2023-05-01 22:09:56.000000 django-sphinx-hosting-1.0.1/setup.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.614796 django-sphinx-hosting-1.0.1/sphinx_hosting/
+-rw-r--r--   0 cmalek     (501) admin       (80)       21 2023-05-01 22:09:56.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/__init__.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.618031 django-sphinx-hosting-1.0.1/sphinx_hosting/api/
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-10-21 23:25:25.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/api/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      331 2023-03-28 15:43:43.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/api/apps.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     4896 2023-03-28 15:50:00.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/api/serializers.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1274 2023-02-22 19:04:46.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/api/urls.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     8676 2023-04-06 17:29:54.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/api/views.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      305 2023-02-22 19:04:46.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/apps.py
+-rw-r--r--   0 cmalek     (501) admin       (80)       49 2022-11-03 21:55:52.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/exc.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.618787 django-sphinx-hosting-1.0.1/sphinx_hosting/fixtures/
+-rw-r--r--   0 cmalek     (501) admin       (80)    12034 2023-04-07 22:07:37.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/fixtures/classifiers.json
+-rw-rw-r--   0 cmalek     (501) admin       (80)     6843 2023-04-27 16:25:48.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/forms.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    21291 2023-04-27 16:27:31.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/importers.py
+-rw-r--r--   0 cmalek     (501) admin       (80)       62 2022-11-17 22:11:14.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/logging.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.619653 django-sphinx-hosting-1.0.1/sphinx_hosting/management/
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-03 21:42:32.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/management/__init__.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.624504 django-sphinx-hosting-1.0.1/sphinx_hosting/management/commands/
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-03 21:42:44.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/management/commands/__init__.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2568 2023-02-22 19:04:46.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/management/commands/import_docs.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     1626 2023-02-01 17:53:25.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/management/commands/parse_globaltoc.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     1421 2023-02-01 17:06:59.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/management/commands/print_classifier_tree.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     2288 2023-02-01 17:06:33.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/management/commands/print_doctree.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.634644 django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/
+-rw-r--r--   0 cmalek     (501) admin       (80)     6366 2022-11-22 19:27:09.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0001_initial.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     1592 2022-11-22 23:23:38.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0002_original_html.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      659 2022-12-08 23:32:00.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0003_globaltoc.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      586 2022-12-09 00:04:04.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0004_next_page_FK.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      683 2023-01-06 00:23:12.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0005_orig_global_toc.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     3829 2023-03-24 22:50:14.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0006_classifiers_and_permissiongroups.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      658 2023-01-19 19:26:47.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0007_load_classifiers.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      497 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0008_Version_archived.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      857 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0009_SphinxPage_searchable.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     2858 2023-03-28 21:23:19.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0010_add_groups.py
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-04 18:37:19.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/__init__.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    31797 2023-05-01 22:09:26.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/models.py
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-18 23:13:36.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/py.typed
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1663 2023-04-27 18:08:13.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/search_indexes.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      566 2023-03-24 21:26:47.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/settings.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.600059 django-sphinx-hosting-1.0.1/sphinx_hosting/static/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.600360 django-sphinx-hosting-1.0.1/sphinx_hosting/static/sphinx_hosting/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.640666 django-sphinx-hosting-1.0.1/sphinx_hosting/static/sphinx_hosting/css/
+-rw-r--r--   0 cmalek     (501) admin       (80)     1075 2023-02-02 18:58:20.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/static/sphinx_hosting/css/_classifierfilterblock.scss
+-rw-r--r--   0 cmalek     (501) admin       (80)     4819 2022-11-22 19:08:46.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/static/sphinx_hosting/css/_pygments.scss
+-rw-r--r--   0 cmalek     (501) admin       (80)    18183 2023-01-10 17:44:02.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/static/sphinx_hosting/css/_sphinx_layout.scss
+-rw-r--r--   0 cmalek     (501) admin       (80)    34945 2023-02-02 18:58:21.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.css
+-rw-r--r--   0 cmalek     (501) admin       (80)     2896 2023-02-01 21:52:48.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.scss
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.641605 django-sphinx-hosting-1.0.1/sphinx_hosting/static/sphinx_hosting/images/
+-rw-r--r--   0 cmalek     (501) admin       (80)    37933 2022-11-17 21:25:05.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/static/sphinx_hosting/images/logo.jpg
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.601164 django-sphinx-hosting-1.0.1/sphinx_hosting/templates/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.600855 django-sphinx-hosting-1.0.1/sphinx_hosting/templates/search/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.600980 django-sphinx-hosting-1.0.1/sphinx_hosting/templates/search/indexes/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.643072 django-sphinx-hosting-1.0.1/sphinx_hosting/templates/search/indexes/sphinxhostingcore/
+-rw-rw-r--   0 cmalek     (501) admin       (80)       36 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/templates/search/indexes/sphinxhostingcore/sphinxpage_text.txt
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.644102 django-sphinx-hosting-1.0.1/sphinx_hosting/templates/sphinx_hosting/
+-rw-r--r--   0 cmalek     (501) admin       (80)      523 2023-01-18 19:41:49.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/templates/sphinx_hosting/base.html
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-10-21 21:37:03.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/types.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1653 2023-03-28 18:47:58.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/urls.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      606 2022-11-02 23:23:01.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/validators.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    20844 2023-04-28 17:09:25.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/views.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.650803 django-sphinx-hosting-1.0.1/sphinx_hosting/wildewidgets/
+-rw-rw-r--   0 cmalek     (501) admin       (80)      255 2023-04-28 16:10:38.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/wildewidgets/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     6553 2023-04-27 20:10:51.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/wildewidgets/classifier.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-01 22:10:47.652523 django-sphinx-hosting-1.0.1/sphinx_hosting/wildewidgets/core/
+-rw-r--r--   0 cmalek     (501) admin       (80)       39 2023-01-18 23:39:43.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/wildewidgets/core/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2023-01-18 23:39:52.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/wildewidgets/core/basic.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     4463 2023-04-06 17:29:54.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/wildewidgets/navigation.py
+-rw-r--r--   0 cmalek     (501) admin       (80)    14263 2023-04-27 19:40:10.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/wildewidgets/project.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    11411 2023-04-27 20:32:48.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/wildewidgets/search.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     7084 2023-04-27 20:42:19.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/wildewidgets/sphinx_page.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     8438 2023-04-27 23:13:13.000000 django-sphinx-hosting-1.0.1/sphinx_hosting/wildewidgets/version.py
```

### Comparing `django-sphinx-hosting-1.0.0/LICENSE.txt` & `django-sphinx-hosting-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/PKG-INFO` & `django-sphinx-hosting-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sphinx-hosting
-Version: 1.0.0
+Version: 1.0.1
 Summary: Reusable Django app for hosting Sphinx documentation privately.
 Home-page: https://github.com/caltechads/django-sphinx-hosting
 Author: Caltech IMSS ADS
 Author-email: imss-ads-staff@caltech.edu
 Keywords: documentation,sphinx,django
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `django-sphinx-hosting-1.0.0/README.md` & `django-sphinx-hosting-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/django_sphinx_hosting.egg-info/PKG-INFO` & `django-sphinx-hosting-1.0.1/django_sphinx_hosting.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sphinx-hosting
-Version: 1.0.0
+Version: 1.0.1
 Summary: Reusable Django app for hosting Sphinx documentation privately.
 Home-page: https://github.com/caltechads/django-sphinx-hosting
 Author: Caltech IMSS ADS
 Author-email: imss-ads-staff@caltech.edu
 Keywords: documentation,sphinx,django
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `django-sphinx-hosting-1.0.0/django_sphinx_hosting.egg-info/SOURCES.txt` & `django-sphinx-hosting-1.0.1/django_sphinx_hosting.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 sphinx_hosting/validators.py
 sphinx_hosting/views.py
 sphinx_hosting/api/__init__.py
 sphinx_hosting/api/apps.py
 sphinx_hosting/api/serializers.py
 sphinx_hosting/api/urls.py
 sphinx_hosting/api/views.py
+sphinx_hosting/fixtures/classifiers.json
 sphinx_hosting/management/__init__.py
 sphinx_hosting/management/commands/__init__.py
 sphinx_hosting/management/commands/import_docs.py
 sphinx_hosting/management/commands/parse_globaltoc.py
 sphinx_hosting/management/commands/print_classifier_tree.py
 sphinx_hosting/management/commands/print_doctree.py
 sphinx_hosting/migrations/0001_initial.py
```

### Comparing `django-sphinx-hosting-1.0.0/setup.cfg` & `django-sphinx-hosting-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/setup.py` & `django-sphinx-hosting-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="django-sphinx-hosting",
-    version="1.0.0",
+    version="1.0.1",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "django-braces >= 1.15.0",
         "django-crispy-forms>=1.14.0",
         "django-extensions >= 3.2.1",
         "django-filter >= 22.1",
```

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/api/serializers.py` & `django-sphinx-hosting-1.0.1/sphinx_hosting/api/serializers.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/api/urls.py` & `django-sphinx-hosting-1.0.1/sphinx_hosting/api/urls.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/api/views.py` & `django-sphinx-hosting-1.0.1/sphinx_hosting/api/views.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/forms.py` & `django-sphinx-hosting-1.0.1/sphinx_hosting/forms.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/importers.py` & `django-sphinx-hosting-1.0.1/sphinx_hosting/importers.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/management/commands/import_docs.py` & `django-sphinx-hosting-1.0.1/sphinx_hosting/management/commands/import_docs.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/management/commands/parse_globaltoc.py` & `django-sphinx-hosting-1.0.1/sphinx_hosting/management/commands/parse_globaltoc.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/management/commands/print_classifier_tree.py` & `django-sphinx-hosting-1.0.1/sphinx_hosting/management/commands/print_classifier_tree.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/management/commands/print_doctree.py` & `django-sphinx-hosting-1.0.1/sphinx_hosting/management/commands/print_doctree.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/migrations/0001_initial.py` & `django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/migrations/0002_original_html.py` & `django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0002_original_html.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/migrations/0003_globaltoc.py` & `django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0003_globaltoc.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/migrations/0004_next_page_FK.py` & `django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0004_next_page_FK.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/migrations/0005_orig_global_toc.py` & `django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0005_orig_global_toc.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/migrations/0006_classifiers_and_permissiongroups.py` & `django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0006_classifiers_and_permissiongroups.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/migrations/0007_load_classifiers.py` & `django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0007_load_classifiers.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/migrations/0009_SphinxPage_searchable.py` & `django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0009_SphinxPage_searchable.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/migrations/0010_add_groups.py` & `django-sphinx-hosting-1.0.1/sphinx_hosting/migrations/0010_add_groups.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/models.py` & `django-sphinx-hosting-1.0.1/sphinx_hosting/models.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/search_indexes.py` & `django-sphinx-hosting-1.0.1/sphinx_hosting/search_indexes.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/settings.py` & `django-sphinx-hosting-1.0.1/sphinx_hosting/settings.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/static/sphinx_hosting/css/_classifierfilterblock.scss` & `django-sphinx-hosting-1.0.1/sphinx_hosting/static/sphinx_hosting/css/_classifierfilterblock.scss`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/static/sphinx_hosting/css/_pygments.scss` & `django-sphinx-hosting-1.0.1/sphinx_hosting/static/sphinx_hosting/css/_pygments.scss`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/static/sphinx_hosting/css/_sphinx_layout.scss` & `django-sphinx-hosting-1.0.1/sphinx_hosting/static/sphinx_hosting/css/_sphinx_layout.scss`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.css` & `django-sphinx-hosting-1.0.1/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.css`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.scss` & `django-sphinx-hosting-1.0.1/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.scss`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/static/sphinx_hosting/images/logo.jpg` & `django-sphinx-hosting-1.0.1/sphinx_hosting/static/sphinx_hosting/images/logo.jpg`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/templates/sphinx_hosting/base.html` & `django-sphinx-hosting-1.0.1/sphinx_hosting/templates/sphinx_hosting/base.html`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/urls.py` & `django-sphinx-hosting-1.0.1/sphinx_hosting/urls.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/validators.py` & `django-sphinx-hosting-1.0.1/sphinx_hosting/validators.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/views.py` & `django-sphinx-hosting-1.0.1/sphinx_hosting/views.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/wildewidgets/classifier.py` & `django-sphinx-hosting-1.0.1/sphinx_hosting/wildewidgets/classifier.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/wildewidgets/navigation.py` & `django-sphinx-hosting-1.0.1/sphinx_hosting/wildewidgets/navigation.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/wildewidgets/project.py` & `django-sphinx-hosting-1.0.1/sphinx_hosting/wildewidgets/project.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/wildewidgets/search.py` & `django-sphinx-hosting-1.0.1/sphinx_hosting/wildewidgets/search.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/wildewidgets/sphinx_page.py` & `django-sphinx-hosting-1.0.1/sphinx_hosting/wildewidgets/sphinx_page.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.0.0/sphinx_hosting/wildewidgets/version.py` & `django-sphinx-hosting-1.0.1/sphinx_hosting/wildewidgets/version.py`

 * *Files identical despite different names*

