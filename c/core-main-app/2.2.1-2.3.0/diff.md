# Comparing `tmp/core_main_app-2.2.1.tar.gz` & `tmp/core_main_app-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_main_app-2.2.1.tar", last modified: Thu Mar 30 21:11:15 2023, max compression
+gzip compressed data, was "core_main_app-2.3.0.tar", last modified: Tue May  2 19:40:23 2023, max compression
```

## Comparing `core_main_app-2.2.1.tar` & `core_main_app-2.3.0.tar`

### file list

```diff
@@ -1,860 +1,818 @@
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:15.585498 core_main_app-2.2.1/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-03-30 21:10:41.000000 core_main_app-2.2.1/LICENSE.md
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      219 2023-03-30 21:10:41.000000 core_main_app-2.2.1/MANIFEST.in
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7062 2023-03-30 21:11:15.581635 core_main_app-2.2.1/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5019 2023-03-30 21:10:41.000000 core_main_app-2.2.1/README.rst
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:06.270743 core_main_app-2.2.1/core_main_app/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       81 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:06.407466 core_main_app-2.2.1/core_main_app/access_control/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/access_control/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11182 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/access_control/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      628 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/access_control/decorators.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      197 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/access_control/exceptions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6065 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1335 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/apps.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:06.503343 core_main_app-2.2.1/core_main_app/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/commons/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      377 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/commons/constants.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       62 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/commons/enums.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4063 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/commons/exceptions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       82 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/commons/regex.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      332 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/commons/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9154 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/commons/validators.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:06.519060 core_main_app-2.2.1/core_main_app/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:06.549634 core_main_app-2.2.1/core_main_app/components/abstract_data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/abstract_data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5240 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/abstract_data/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:06.627568 core_main_app-2.2.1/core_main_app/components/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/blob/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1118 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/blob/access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      315 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/blob/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2729 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/blob/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3493 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/blob/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      442 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/blob/utils.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:06.722682 core_main_app-2.2.1/core_main_app/components/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4384 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/data/access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5445 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/data/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8854 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/data/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5791 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/data/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10384 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/data/tasks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:06.760668 core_main_app-2.2.1/core_main_app/components/group/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/group/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1982 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/group/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:06.811255 core_main_app-2.2.1/core_main_app/components/lock/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/lock/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      330 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/lock/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2570 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/lock/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2665 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/lock/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:06.862898 core_main_app-2.2.1/core_main_app/components/mongo/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/mongo/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1041 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/mongo/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10440 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/mongo/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:06.963625 core_main_app-2.2.1/core_main_app/components/template/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/template/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4454 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/template/access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      362 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/template/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4434 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/template/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6655 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/template/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:07.030041 core_main_app-2.2.1/core_main_app/components/template_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/template_version_manager/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2328 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/template_version_manager/access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      507 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/template_version_manager/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6205 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/template_version_manager/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4719 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/template_version_manager/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:07.082710 core_main_app-2.2.1/core_main_app/components/template_xsl_rendering/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/template_xsl_rendering/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      338 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/template_xsl_rendering/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6892 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/template_xsl_rendering/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3434 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/template_xsl_rendering/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:07.106481 core_main_app-2.2.1/core_main_app/components/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2470 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/user/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:07.168060 core_main_app-2.2.1/core_main_app/components/version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/version_manager/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4883 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/version_manager/access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3744 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/version_manager/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3248 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/version_manager/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      550 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/version_manager/utils.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:07.206444 core_main_app-2.2.1/core_main_app/components/web_page/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/web_page/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1280 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/web_page/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1097 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/web_page/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:07.234622 core_main_app-2.2.1/core_main_app/components/web_page_login/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/web_page_login/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      809 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/web_page_login/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:07.307626 core_main_app-2.2.1/core_main_app/components/workspace/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/workspace/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2493 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/workspace/access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      372 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/workspace/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16858 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/workspace/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5695 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/workspace/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:07.366913 core_main_app-2.2.1/core_main_app/components/xsl_transformation/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/xsl_transformation/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      366 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/xsl_transformation/admin_site.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2542 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/xsl_transformation/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4469 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/components/xsl_transformation/models.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1791 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/menus.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:07.427527 core_main_app-2.2.1/core_main_app/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16483 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/migrations/0001_initial.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      751 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/migrations/0002_site_update.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1880 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/migrations/0003_psql_full_text.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      823 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/migrations/0004_template_ordering.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/migrations/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      733 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/models.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:07.518224 core_main_app-2.2.1/core_main_app/permissions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/permissions/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6351 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/permissions/api.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3152 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/permissions/discover.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      644 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/permissions/rights.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      230 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/permissions/utils.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:07.564565 core_main_app-2.2.1/core_main_app/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:07.599098 core_main_app-2.2.1/core_main_app/rest/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/rest/blob/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4546 2023-03-30 21:10:41.000000 core_main_app-2.2.1/core_main_app/rest/blob/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16319 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/rest/blob/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:07.671925 core_main_app-2.2.1/core_main_app/rest/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/rest/data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9501 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/rest/data/abstract_views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2006 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/rest/data/admin_serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3187 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/rest/data/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    36899 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/rest/data/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:07.697621 core_main_app-2.2.1/core_main_app/rest/group/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/rest/group/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      293 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/rest/group/serializers.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:07.735691 core_main_app-2.2.1/core_main_app/rest/mongo_data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/rest/mongo_data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1692 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/rest/mongo_data/serializers.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:07.776152 core_main_app-2.2.1/core_main_app/rest/template/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/rest/template/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      834 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/rest/template/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4354 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/rest/template/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:07.855801 core_main_app-2.2.1/core_main_app/rest/template_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/rest/template_version_manager/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10462 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/rest/template_version_manager/abstract_views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2601 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/rest/template_version_manager/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      587 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/rest/template_version_manager/utils.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12274 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/rest/template_version_manager/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:07.898411 core_main_app-2.2.1/core_main_app/rest/template_xsl_rendering/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/rest/template_xsl_rendering/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1168 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/rest/template_xsl_rendering/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14418 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/rest/template_xsl_rendering/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14246 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/rest/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:07.934447 core_main_app-2.2.1/core_main_app/rest/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/rest/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1157 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/rest/user/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      709 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/rest/user/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2478 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/rest/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:07.992301 core_main_app-2.2.1/core_main_app/rest/web_page/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/rest/web_page/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1042 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/rest/web_page/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4688 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/rest/web_page/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:08.055395 core_main_app-2.2.1/core_main_app/rest/workspace/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/rest/workspace/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      894 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/rest/workspace/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    23285 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/rest/workspace/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:08.108633 core_main_app-2.2.1/core_main_app/rest/xsl_transformation/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/rest/xsl_transformation/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1437 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/rest/xsl_transformation/serializers.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8160 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/rest/xsl_transformation/views.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8070 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/settings.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:04.901545 core_main_app-2.2.1/core_main_app/static/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:05.131840 core_main_app-2.2.1/core_main_app/static/core_main_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:04.925557 core_main_app-2.2.1/core_main_app/static/core_main_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:04.911989 core_main_app-2.2.1/core_main_app/static/core_main_app/admin/_theme/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:08.163571 core_main_app-2.2.1/core_main_app/static/core_main_app/admin/_theme/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      251 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/admin/_theme/css/additional.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    47539 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/admin/_theme/css/skins.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)   110978 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/admin/_theme/css/theme.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:08.195106 core_main_app-2.2.1/core_main_app/static/core_main_app/admin/_theme/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    22937 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/admin/_theme/js/app.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      578 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/admin/_theme/js/menu.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:08.221975 core_main_app-2.2.1/core_main_app/static/core_main_app/admin/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1575 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/admin/css/data_migration.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       81 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/admin/css/permissions.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:08.235654 core_main_app-2.2.1/core_main_app/static/core_main_app/admin/css/templates_xslt/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1363 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/admin/css/templates_xslt/form.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:08.264485 core_main_app-2.2.1/core_main_app/static/core_main_app/admin/css/web_page/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       31 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/admin/css/web_page/style.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:08.279196 core_main_app-2.2.1/core_main_app/static/core_main_app/admin/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      831 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/admin/js/display_permissions.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:08.306772 core_main_app-2.2.1/core_main_app/static/core_main_app/admin/js/templates/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    30064 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/admin/js/templates/data_migration.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      594 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/admin/js/templates/data_migration.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:08.346159 core_main_app-2.2.1/core_main_app/static/core_main_app/admin/js/templates/upload/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1334 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/admin/js/templates/upload/dependencies.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       94 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/admin/js/templates/upload/dependencies.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      139 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/admin/js/templates/upload/dependency_resolver.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:08.359882 core_main_app-2.2.1/core_main_app/static/core_main_app/admin/js/templates_xslt/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1482 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/admin/js/templates_xslt/detail_xslt.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:04.987108 core_main_app-2.2.1/core_main_app/static/core_main_app/common/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:08.460249 core_main_app-2.2.1/core_main_app/static/core_main_app/common/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2236 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/css/XMLTree.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       68 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/css/buttons.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      178 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/css/fields.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       92 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/css/loading-spinner.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      392 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/css/share_link.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      900 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/css/switch.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      486 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/css/table.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:08.475851 core_main_app-2.2.1/core_main_app/static/core_main_app/common/css/template/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       59 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/css/template/template_ordering.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      189 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/css/word-wrap.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:08.507729 core_main_app-2.2.1/core_main_app/static/core_main_app/common/img/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      246 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/img/collapse.png
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      253 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/img/expand.png
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:08.633179 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      335 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/XMLTree.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      247 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/backtoprevious.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1828 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/csrf.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      192 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/data_detail.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      531 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/debounce.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      788 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/elementViewport.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      413 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/leave_notice.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      556 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/loading_spinner.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:08.713122 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1292 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/modals/add.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1136 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/modals/delete.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      481 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/modals/download.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      178 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/modals/download.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1257 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/modals/edit.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      439 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/modals/error_page_modal.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1880 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/notify-styles.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:08.739443 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:08.765523 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/templates/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:08.792451 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/templates/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1086 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/templates/list/modals/disable.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      125 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/templates/list/modals/disable.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      663 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/templates/list/restore.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      124 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/templates/list/restore.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1156 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/templates/sort.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       97 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/templates/sort.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:08.855238 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/templates/versions/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:08.880699 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/templates/versions/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1029 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/templates/versions/modals/disable.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      108 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/templates/versions/modals/disable.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      537 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/templates/versions/restore.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      107 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/templates/versions/restore.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      652 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/templates/versions/set_current.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      111 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/templates/versions/set_current.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:04.981440 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/xslt/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:04.983815 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/xslt/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:08.937918 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/xslt/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      859 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/xslt/list/modals/delete.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       64 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/xslt/list/modals/delete.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1012 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/xslt/list/modals/edit.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/xslt/list/modals/edit.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:08.958858 core_main_app-2.2.1/core_main_app/static/core_main_app/common/xsl/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1763 2023-03-30 21:10:42.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/common/xsl/xml2html.xsl
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:08.974110 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:05.018531 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/bootstrap/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:05.024815 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/bootstrap/4.5.2/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:08.994163 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/bootstrap/4.5.2/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)   160302 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/bootstrap/4.5.2/css/bootstrap.min.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:09.012928 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/bootstrap/4.5.2/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    60044 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/bootstrap/4.5.2/js/bootstrap.min.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:05.040737 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/datatables/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:05.052843 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/datatables/1.10.13/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:09.033372 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/datatables/1.10.13/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    15423 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/datatables/1.10.13/css/jquery.dataTables.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:09.105525 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/datatables/1.10.13/images/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      160 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/datatables/1.10.13/images/sort_asc.png
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      148 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/datatables/1.10.13/images/sort_asc_disabled.png
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      201 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/datatables/1.10.13/images/sort_both.png
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      158 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/datatables/1.10.13/images/sort_desc.png
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      146 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/datatables/1.10.13/images/sort_desc_disabled.png
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:09.119805 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/datatables/1.10.13/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)   448547 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/datatables/1.10.13/js/jquery.dataTables.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:05.064036 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/fSelect/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:09.167430 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/fSelect/css/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)     2719 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/fSelect/css/fSelect.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:09.181507 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/fSelect/js/
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)    12656 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/fSelect/js/fSelect.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:05.072588 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/font-awesome/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:05.078964 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/font-awesome/5.13.0/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:09.200842 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/font-awesome/5.13.0/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    58578 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/font-awesome/5.13.0/css/all.min.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:09.471067 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/font-awesome/5.13.0/webfonts/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)   133034 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/font-awesome/5.13.0/webfonts/fa-brands-400.eot
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)   715890 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/font-awesome/5.13.0/webfonts/fa-brands-400.svg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)   132728 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/font-awesome/5.13.0/webfonts/fa-brands-400.ttf
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    89824 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/font-awesome/5.13.0/webfonts/fa-brands-400.woff
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    76612 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/font-awesome/5.13.0/webfonts/fa-brands-400.woff2
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    34390 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/font-awesome/5.13.0/webfonts/fa-regular-400.eot
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)   144322 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/font-awesome/5.13.0/webfonts/fa-regular-400.svg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    34092 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/font-awesome/5.13.0/webfonts/fa-regular-400.ttf
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16800 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/font-awesome/5.13.0/webfonts/fa-regular-400.woff
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13584 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/font-awesome/5.13.0/webfonts/fa-regular-400.woff2
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)   202902 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/font-awesome/5.13.0/webfonts/fa-solid-900.eot
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)   897426 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/font-awesome/5.13.0/webfonts/fa-solid-900.svg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)   202616 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/font-awesome/5.13.0/webfonts/fa-solid-900.ttf
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)   103300 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/font-awesome/5.13.0/webfonts/fa-solid-900.woff
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    79444 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/font-awesome/5.13.0/webfonts/fa-solid-900.woff2
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:05.087934 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/highlight/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:05.093966 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/highlight/11.0.0/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:09.490463 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/highlight/11.0.0/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1217 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/highlight/11.0.0/css/atom-one-light.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:09.523718 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/highlight/11.0.0/js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    22386 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/highlight/11.0.0/js/highlight.min.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       20 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/highlight/11.0.0/js/init_highlight.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:05.111890 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/jquery/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:09.709940 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/jquery/3.5.1/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    89475 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/jquery/3.5.1/jquery.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:05.100980 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/jquery-ui/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:09.593374 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:09.693389 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7006 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_444444_256x240.png
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7074 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_555555_256x240.png
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4676 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_777620_256x240.png
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7013 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_777777_256x240.png
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4632 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6313 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    37326 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)   520714 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    18705 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.structure.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    18671 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.theme.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    21509 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/notify.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:09.728007 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/popper-js/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    21257 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/libs/popper-js/popper.min.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:05.138364 core_main_app-2.2.1/core_main_app/static/core_main_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:09.775624 core_main_app-2.2.1/core_main_app/static/core_main_app/user/css/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       32 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/user/css/login.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       63 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/user/css/registration.css
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/user/css/text-editor.css
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:09.790573 core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:09.830366 core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      618 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/data/change_display.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      120 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/data/change_display.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      158 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/data/detail.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:09.859045 core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/login/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      667 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/login/message.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       52 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/login/message.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1110 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/sharing_modal.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:09.902333 core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/text_editor/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      154 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/text_editor/data_text_editor.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       73 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/text_editor/template_text_editor.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5337 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/text_editor/text_editor.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:10.025282 core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/workspaces/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1873 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/workspaces/add_group.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      160 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/workspaces/add_group.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1807 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/workspaces/add_user.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/workspaces/add_user.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1138 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/workspaces/create_workspace.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       73 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/workspaces/create_workspace.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      776 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/workspaces/init.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       43 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/workspaces/init.raw.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:05.178127 core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/workspaces/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:10.174041 core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/workspaces/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      187 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/workspaces/list/modals/assign_blob_workspace.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      187 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/workspaces/list/modals/assign_data_workspace.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1455 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/workspaces/list/modals/assign_workspace.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1360 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/workspaces/list/modals/remove_rights.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/workspaces/list/modals/remove_rights.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      807 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_private.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       96 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_private.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      822 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_public.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       94 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_public.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1728 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/workspaces/list/modals/switch_right.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      144 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/workspaces/list/modals/switch_right.raw.js
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      917 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/workspaces/tables.js
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:10.206757 core_main_app-2.2.1/core_main_app/system/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/system/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2302 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/system/api.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:10.220334 core_main_app-2.2.1/core_main_app/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:05.423406 core_main_app-2.2.1/core_main_app/templates/core_main_app/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:05.230609 core_main_app-2.2.1/core_main_app/templates/core_main_app/_render/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:10.238208 core_main_app-2.2.1/core_main_app/templates/core_main_app/_render/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1302 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/_render/admin/app_wrapper.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:10.292167 core_main_app-2.2.1/core_main_app/templates/core_main_app/_render/admin/theme/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3537 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/_render/admin/theme/base.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      223 2023-03-30 21:10:43.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/_render/admin/theme/footer.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      905 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/_render/admin/theme/header.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2909 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/_render/admin/theme/menu.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:10.341934 core_main_app-2.2.1/core_main_app/templates/core_main_app/_render/admin/theme/tools/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      620 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/_render/admin/theme/tools/box.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/_render/admin/theme/tools/form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      715 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/_render/admin/theme/tools/modal.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      283 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/_render/admin/theme/tools/section.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:10.353333 core_main_app-2.2.1/core_main_app/templates/core_main_app/_render/common/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      567 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/_render/common/messages.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:10.396739 core_main_app-2.2.1/core_main_app/templates/core_main_app/_render/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1463 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/_render/user/app_wrapper.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      902 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/_render/user/default.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3462 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/_render/user/theme_base.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:10.447246 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:05.249361 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/commons/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:10.500720 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/commons/errors/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      401 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/commons/errors/errors.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      254 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/commons/errors/errors_wrapper.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:10.529691 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/commons/upload/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      691 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/commons/upload/form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      313 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/commons/upload/upload.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      103 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/dashboard.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:10.557885 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      311 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/data/detail.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      383 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/data/detail_box.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1497 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/dependency_resolver.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      211 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/list_dependencies.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:10.606429 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:10.619346 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/templates/data_migration/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7822 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/templates/data_migration/templates_list.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      289 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/templates/data_migration.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:10.645534 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/templates/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1802 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/templates/list/available.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      830 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/templates/list/disabled.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:10.660329 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/templates/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      813 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/templates/list/modals/disable.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      542 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/templates/list.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:10.677361 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/templates/upload/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      399 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/templates/upload/base.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      166 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/templates/upload.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:10.713394 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/templates/versions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3401 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/templates/versions/available.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1158 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/templates/versions/disabled.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:10.727242 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/templates/versions/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      727 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/templates/versions/modals/disable.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      677 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/templates/versions.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:10.744080 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/templates_xslt/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:10.758318 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/templates_xslt/main/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4036 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/templates_xslt/main/form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      393 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/templates_xslt/main.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      860 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/upload_template.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:10.892320 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/web_page/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      166 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/web_page/login_page.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      804 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/web_page/main.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      387 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/web_page/web_page.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      375 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/web_page/web_page_unavailable.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:10.906740 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/workspaces/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      234 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/workspaces/edit_rights.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:10.935387 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/xslt/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:10.949528 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/xslt/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1236 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/xslt/list/table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      323 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/xslt/list.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:10.963921 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/xslt/upload/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       61 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/xslt/upload/base.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      161 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/xslt/upload.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:05.408083 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:11.060264 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/buttons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/buttons/add.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      152 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/buttons/back_to_previous.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/buttons/delete.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      190 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/buttons/edit.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      104 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/buttons/go_to.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      131 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/buttons/save_ordering.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:11.102891 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      189 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/commons/error.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       97 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/commons/form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      167 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/commons/form_delete.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:11.131456 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/commons/upload/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      578 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/commons/upload/form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      313 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/commons/upload/upload.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:11.157374 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      497 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/data/detail_data.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1716 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/data/tools_data.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:11.171290 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/defender/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       90 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/defender/error.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:11.247554 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      463 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/modals/add_page_modal.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      633 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/modals/create_data_modal.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      489 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/modals/delete_page_modal.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1066 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/modals/download-options.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      467 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/modals/edit_page_modal.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      429 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/modals/error_page_modal.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:11.259631 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/pagination/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3008 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/pagination/data_source_pagination.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:11.272523 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/templates/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:11.298356 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/templates/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1524 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/templates/list/available.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      801 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/templates/list/disabled.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:11.327241 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/templates/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      805 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/templates/list/modals/disable.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      741 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/templates/list/modals/edit.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:11.340118 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/templates/versions/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2074 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/templates/versions/available.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:11.355418 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/templates/versions/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      663 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/templates/versions/modals/disable.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      265 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/templates/versions.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:11.381708 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/templates_xslt/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/templates_xslt/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:11.395860 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/templates_xslt/main/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      832 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/templates_xslt/main/form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      428 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/templates_xslt/main.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:11.432229 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/xslt/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:11.448334 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/xslt/list/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:11.476683 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/xslt/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      564 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/xslt/list/modals/delete.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      928 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/xslt/list/modals/edit.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1147 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/xslt/list/table.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      255 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/xslt/list.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:11.491997 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/xslt/upload/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       62 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/xslt/upload/base.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      163 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/common/xslt/upload.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:11.516294 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:11.531802 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      483 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/data/detail.html
--rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      139 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/homepage.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:11.557753 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/login/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2215 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/login/main.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:11.570878 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/login/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      534 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/login/modals/login_message.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      340 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/login/saml2_error.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:11.646138 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/registration/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      171 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/registration/password_reset_complete.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      390 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/registration/password_reset_confirm.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      499 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/registration/password_reset_done.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      362 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/registration/password_reset_email.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      180 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/registration/password_reset_form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       14 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/registration/password_reset_subject.txt
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:11.674412 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/sharing/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      274 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/sharing/button.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:11.709583 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/sharing/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      504 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/sharing/modals/multi-link.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      940 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/sharing/modals/single-link.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:11.737678 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/template/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      453 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/template/list_body.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/template/list_header.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:11.751685 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/text_editor/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2798 2023-03-30 21:10:44.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/text_editor/text_editor.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:11.765332 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/workspaces/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1172 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/workspaces/edit_rights.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:11.788801 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/workspaces/list/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1424 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/workspaces/list/create_workspace.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1545 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/workspaces/list/edit_rights_table.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:11.951802 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/workspaces/list/modals/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1086 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/workspaces/list/modals/add_group.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      193 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/workspaces/list/modals/add_group_form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1057 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/workspaces/list/modals/add_user.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      190 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/workspaces/list/modals/add_user_form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      832 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/workspaces/list/modals/assign_workspace.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      411 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/workspaces/list/modals/assign_workspace_form.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      958 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/workspaces/list/modals/remove_rights.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      883 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/workspaces/list/modals/set_private.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      892 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/workspaces/list/modals/set_public.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      675 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/templates/core_main_app/user/workspaces/list/modals/switch_right.html
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      147 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/templates/theme.html
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:12.096636 core_main_app-2.2.1/core_main_app/templatetags/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/templatetags/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1086 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/templatetags/auth_extras.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1097 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/templatetags/blob_tags.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      367 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/templatetags/dict_key_extras.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      514 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/templatetags/get_attribute.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      598 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/templatetags/include_static.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1124 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/templatetags/json_date.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      642 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/templatetags/stripjs.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      316 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/templatetags/timestamptags.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3319 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/templatetags/xsl_transform_tag.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5279 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:12.297180 core_main_app-2.2.1/core_main_app/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:12.348572 core_main_app-2.2.1/core_main_app/utils/admin_site/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/admin_site/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      379 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/admin_site/view_only_admin.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2447 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/blob_downloader.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      405 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/boolean.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1137 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/checksum.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1588 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/custom_context_processors.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:12.383421 core_main_app-2.2.1/core_main_app/utils/databases/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/databases/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      627 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/databases/backend.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:12.420728 core_main_app-2.2.1/core_main_app/utils/databases/mongo/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      574 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/databases/mongo/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1584 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/databases/mongo/mongoengine_database.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      873 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/databases/mongo/pymongo_database.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      286 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/datetime.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9575 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/decorators.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2805 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/file.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      377 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/group.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:12.470912 core_main_app-2.2.1/core_main_app/utils/integration_tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/integration_tests/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      262 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/integration_tests/fixture_interface.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1678 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/integration_tests/integration_base_test_case.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1068 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/integration_tests/integration_base_transaction_test_case.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      319 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/labels.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:12.494746 core_main_app-2.2.1/core_main_app/utils/logger/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/logger/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1762 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/logger/logger_utils.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      438 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/markdown_parser.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      957 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/migrations.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:12.517335 core_main_app-2.2.1/core_main_app/utils/notifications/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/notifications/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3448 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/notifications/mail.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:12.544311 core_main_app-2.2.1/core_main_app/utils/notifications/tasks/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/notifications/tasks/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2566 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/notifications/tasks/task_mail.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:12.578482 core_main_app-2.2.1/core_main_app/utils/pagination/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/pagination/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:12.618734 core_main_app-2.2.1/core_main_app/utils/pagination/django_paginator/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/pagination/django_paginator/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      773 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/pagination/django_paginator/results_paginator.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:12.657379 core_main_app-2.2.1/core_main_app/utils/pagination/mongoengine_paginator/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/pagination/mongoengine_paginator/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1109 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/pagination/mongoengine_paginator/paginator.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:12.696974 core_main_app-2.2.1/core_main_app/utils/pagination/rest_framework_paginator/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/pagination/rest_framework_paginator/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      525 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/pagination/rest_framework_paginator/pagination.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1108 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/pagination/rest_framework_paginator/rest_framework_paginator.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:12.726282 core_main_app-2.2.1/core_main_app/utils/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      145 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/query/constants.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:12.766298 core_main_app-2.2.1/core_main_app/utils/query/mongo/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/query/mongo/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14676 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/query/mongo/prepare.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3095 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/query/mongo/query_builder.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:12.820033 core_main_app-2.2.1/core_main_app/utils/raw_query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/raw_query/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1622 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/raw_query/common.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3901 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/raw_query/django_raw_query.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2134 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/raw_query/mongo_raw_query.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3182 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/rendering.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:12.882768 core_main_app-2.2.1/core_main_app/utils/requests_utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/requests_utils/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      568 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/requests_utils/access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1663 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/requests_utils/requests_utils.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2054 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/requests_utils/ssl.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:12.935976 core_main_app-2.2.1/core_main_app/utils/resolvers/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/resolvers/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1184 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/resolvers/requests_resolver.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1072 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/resolvers/resolver_utils.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/resolvers/xsd_uri_resolvers.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:12.961109 core_main_app-2.2.1/core_main_app/utils/saml2/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/saml2/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8886 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/saml2/utils.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:13.000820 core_main_app-2.2.1/core_main_app/utils/storage/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/storage/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3523 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/storage/gridfs_storage.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1791 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/storage/storage.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:13.037085 core_main_app-2.2.1/core_main_app/utils/tests_tools/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      613 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/tests_tools/MockUser.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5344 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/tests_tools/RequestMock.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/tests_tools/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1052 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:13.097045 core_main_app-2.2.1/core_main_app/utils/validation/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/validation/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1153 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/validation/regex_validation.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      644 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/validation/xpath_validation.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:13.156899 core_main_app-2.2.1/core_main_app/utils/view_builders/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/view_builders/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6572 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/view_builders/data.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16047 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/xml.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:13.266428 core_main_app-2.2.1/core_main_app/utils/xsd_flattener/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/xsd_flattener/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2095 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/xsd_flattener/xsd_flattener_database_url.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1000 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/utils/xsd_flattener/xsd_flattener_requests_url.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:13.280125 core_main_app-2.2.1/core_main_app/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/views/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:13.351871 core_main_app-2.2.1/core_main_app/views/admin/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/views/admin/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4442 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/views/admin/ajax.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:13.365855 core_main_app-2.2.1/core_main_app/views/admin/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/views/admin/commons/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:13.395974 core_main_app-2.2.1/core_main_app/views/admin/commons/upload/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/views/admin/commons/upload/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      439 2023-03-30 21:10:45.000000 core_main_app-2.2.1/core_main_app/views/admin/commons/upload/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4457 2023-03-30 21:10:46.000000 core_main_app-2.2.1/core_main_app/views/admin/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    21048 2023-03-30 21:10:46.000000 core_main_app-2.2.1/core_main_app/views/admin/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:13.460903 core_main_app-2.2.1/core_main_app/views/common/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:46.000000 core_main_app-2.2.1/core_main_app/views/common/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7191 2023-03-30 21:10:46.000000 core_main_app-2.2.1/core_main_app/views/common/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      459 2023-03-30 21:10:46.000000 core_main_app-2.2.1/core_main_app/views/common/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    29318 2023-03-30 21:10:46.000000 core_main_app-2.2.1/core_main_app/views/common/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:13.511066 core_main_app-2.2.1/core_main_app/views/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:46.000000 core_main_app-2.2.1/core_main_app/views/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16819 2023-03-30 21:10:46.000000 core_main_app-2.2.1/core_main_app/views/user/ajax.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4895 2023-03-30 21:10:46.000000 core_main_app-2.2.1/core_main_app/views/user/forms.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14848 2023-03-30 21:10:46.000000 core_main_app-2.2.1/core_main_app/views/user/views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:06.328826 core_main_app-2.2.1/core_main_app.egg-info/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7062 2023-03-30 21:11:02.000000 core_main_app-2.2.1/core_main_app.egg-info/PKG-INFO
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    33438 2023-03-30 21:11:04.000000 core_main_app-2.2.1/core_main_app.egg-info/SOURCES.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-03-30 21:11:02.000000 core_main_app-2.2.1/core_main_app.egg-info/dependency_links.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      445 2023-03-30 21:11:02.000000 core_main_app-2.2.1/core_main_app.egg-info/requires.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       25 2023-03-30 21:11:02.000000 core_main_app-2.2.1/core_main_app.egg-info/top_level.txt
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:13.568035 core_main_app-2.2.1/docs/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:46.000000 core_main_app-2.2.1/docs/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11121 2023-03-30 21:10:46.000000 core_main_app-2.2.1/docs/conf.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      278 2023-03-30 21:10:46.000000 core_main_app-2.2.1/docs/conf_urls.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      170 2023-03-30 21:10:53.000000 core_main_app-2.2.1/pyproject.toml
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       18 2023-03-30 21:10:53.000000 core_main_app-2.2.1/requirements.core.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       92 2023-03-30 21:10:53.000000 core_main_app-2.2.1/requirements.dev.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       20 2023-03-30 21:10:53.000000 core_main_app-2.2.1/requirements.mongo.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      293 2023-03-30 21:11:00.000000 core_main_app-2.2.1/requirements.txt
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-03-30 21:11:15.586788 core_main_app-2.2.1/setup.cfg
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2104 2023-03-30 21:11:00.000000 core_main_app-2.2.1/setup.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:13.643984 core_main_app-2.2.1/tests/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:56.000000 core_main_app-2.2.1/tests/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:13.680012 core_main_app-2.2.1/tests/access_control/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:56.000000 core_main_app-2.2.1/tests/access_control/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3415 2023-03-30 21:10:56.000000 core_main_app-2.2.1/tests/access_control/tests_access_control.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:13.717405 core_main_app-2.2.1/tests/commons/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:56.000000 core_main_app-2.2.1/tests/commons/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3764 2023-03-30 21:10:56.000000 core_main_app-2.2.1/tests/commons/tests_validators.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:13.730783 core_main_app-2.2.1/tests/components/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:56.000000 core_main_app-2.2.1/tests/components/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:13.783949 core_main_app-2.2.1/tests/components/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:56.000000 core_main_app-2.2.1/tests/components/blob/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:13.812823 core_main_app-2.2.1/tests/components/blob/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:56.000000 core_main_app-2.2.1/tests/components/blob/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3165 2023-03-30 21:10:56.000000 core_main_app-2.2.1/tests/components/blob/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6433 2023-03-30 21:10:56.000000 core_main_app-2.2.1/tests/components/blob/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    20721 2023-03-30 21:10:56.000000 core_main_app-2.2.1/tests/components/blob/tests_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      440 2023-03-30 21:10:56.000000 core_main_app-2.2.1/tests/components/blob/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:13.885607 core_main_app-2.2.1/tests/components/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:56.000000 core_main_app-2.2.1/tests/components/data/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:13.920219 core_main_app-2.2.1/tests/components/data/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/data/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    23919 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/data/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    66593 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/data/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    80946 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/data/tests_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3740 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/data/tests_int_ordering.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    27059 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/data/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:13.947971 core_main_app-2.2.1/tests/components/group/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/group/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:13.987319 core_main_app-2.2.1/tests/components/group/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/group/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      570 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/group/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      889 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/group/fixtures/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4790 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/group/tests_int.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:14.031827 core_main_app-2.2.1/tests/components/lock/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/lock/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4173 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/lock/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2440 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/lock/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:14.059631 core_main_app-2.2.1/tests/components/mongo_data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/mongo_data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    70475 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/mongo_data/tests_int_access_control.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:14.123844 core_main_app-2.2.1/tests/components/template/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/template/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:14.155015 core_main_app-2.2.1/tests/components/template/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/template/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2078 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/template/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    46067 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/template/tests_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7215 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/template/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:14.199353 core_main_app-2.2.1/tests/components/template_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/template_version_manager/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:14.228856 core_main_app-2.2.1/tests/components/template_version_manager/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/template_version_manager/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6470 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/template_version_manager/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    54944 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/template_version_manager/tests_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17617 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/template_version_manager/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:14.272666 core_main_app-2.2.1/tests/components/template_xsl_rendering/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/template_xsl_rendering/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:14.301573 core_main_app-2.2.1/tests/components/template_xsl_rendering/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/template_xsl_rendering/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3266 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/template_xsl_rendering/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7933 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/template_xsl_rendering/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9565 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/template_xsl_rendering/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:14.333701 core_main_app-2.2.1/tests/components/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/user/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:14.375901 core_main_app-2.2.1/tests/components/user/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/user/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1552 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/user/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1439 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/user/fixtures/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7778 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/user/tests_int.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:14.427536 core_main_app-2.2.1/tests/components/version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/version_manager/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    61669 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/version_manager/tests_int_access_control.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9899 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/version_manager/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:14.458150 core_main_app-2.2.1/tests/components/web_page/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/web_page/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4846 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/web_page/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:14.487842 core_main_app-2.2.1/tests/components/web_page_login/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/web_page_login/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3905 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/web_page_login/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:14.518823 core_main_app-2.2.1/tests/components/workspace/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/workspace/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:14.563012 core_main_app-2.2.1/tests/components/workspace/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/workspace/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1235 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/workspace/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      929 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/workspace/fixtures/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7503 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/workspace/tests_int.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:14.593819 core_main_app-2.2.1/tests/components/xsl_transformation/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/xsl_transformation/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12828 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/components/xsl_transformation/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      356 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/mocks.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:14.630769 core_main_app-2.2.1/tests/rest/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/rest/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:14.685088 core_main_app-2.2.1/tests/rest/blob/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/rest/blob/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    23681 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/rest/blob/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    19778 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/rest/blob/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)       36 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/rest/blob/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:14.750767 core_main_app-2.2.1/tests/rest/data/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/rest/data/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    47456 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/rest/data/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    41435 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/rest/data/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12424 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/rest/data/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:14.812997 core_main_app-2.2.1/tests/rest/template/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/rest/template/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2528 2023-03-30 21:10:57.000000 core_main_app-2.2.1/tests/rest/template/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5026 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/rest/template/tests_permission.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4802 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/rest/template/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:14.890316 core_main_app-2.2.1/tests/rest/template_version_manager/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/rest/template_version_manager/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    37302 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/rest/template_version_manager/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    31920 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/rest/template_version_manager/tests_permission.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3610 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/rest/template_version_manager/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:14.935207 core_main_app-2.2.1/tests/rest/template_xsl_rendering/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/rest/template_xsl_rendering/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11449 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/rest/template_xsl_rendering/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13879 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/rest/template_xsl_rendering/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3549 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/rest/tests_views.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:15.012796 core_main_app-2.2.1/tests/rest/user/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/rest/user/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1747 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/rest/user/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3147 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/rest/user/tests_permissions.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      886 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/rest/user/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:15.043028 core_main_app-2.2.1/tests/rest/web_page/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/rest/web_page/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6164 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/rest/web_page/tests_permission.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:15.095467 core_main_app-2.2.1/tests/rest/workspace/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/rest/workspace/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    71915 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/rest/workspace/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    48644 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/rest/workspace/tests_permissions.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:15.159441 core_main_app-2.2.1/tests/rest/xsl_transformation/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/rest/xsl_transformation/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:15.185363 core_main_app-2.2.1/tests/rest/xsl_transformation/fixtures/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/rest/xsl_transformation/fixtures/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1283 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/rest/xsl_transformation/fixtures/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11653 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/rest/xsl_transformation/tests_int.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12753 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/rest/xsl_transformation/tests_permission.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4365 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/rest/xsl_transformation/tests_unit.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      529 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/rest_urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:15.211516 core_main_app-2.2.1/tests/system/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/system/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4668 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/system/test_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:15.238530 core_main_app-2.2.1/tests/templatetags/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/templatetags/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1364 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/templatetags/test_get_attribute.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2758 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/test_settings.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      293 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/test_settings_sqlite3.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3445 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/urls.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:15.313471 core_main_app-2.2.1/tests/utils/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/utils/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:15.341721 core_main_app-2.2.1/tests/utils/checksum/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/utils/checksum/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1294 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/utils/checksum/tests_checksum.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:15.372808 core_main_app-2.2.1/tests/utils/migrations/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/utils/migrations/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1664 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/utils/migrations/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:15.387160 core_main_app-2.2.1/tests/utils/query/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/utils/query/__init__.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:15.433420 core_main_app-2.2.1/tests/utils/query/mongo/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/utils/query/mongo/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9855 2023-03-30 21:10:58.000000 core_main_app-2.2.1/tests/utils/query/mongo/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:15.464728 core_main_app-2.2.1/tests/utils/requests_utls/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:59.000000 core_main_app-2.2.1/tests/utils/requests_utls/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1436 2023-03-30 21:10:59.000000 core_main_app-2.2.1/tests/utils/requests_utls/tests_ssl.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4010 2023-03-30 21:10:59.000000 core_main_app-2.2.1/tests/utils/tests_int_blob_downloader.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2624 2023-03-30 21:10:59.000000 core_main_app-2.2.1/tests/utils/tests_int_file.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1726 2023-03-30 21:10:59.000000 core_main_app-2.2.1/tests/utils/tests_unit_boolean.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11988 2023-03-30 21:10:59.000000 core_main_app-2.2.1/tests/utils/tests_unit_xml_operation.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4344 2023-03-30 21:10:59.000000 core_main_app-2.2.1/tests/utils/tests_view_data.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:15.493729 core_main_app-2.2.1/tests/utils/validation/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:59.000000 core_main_app-2.2.1/tests/utils/validation/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)      681 2023-03-30 21:10:59.000000 core_main_app-2.2.1/tests/utils/validation/tests_unit_validation.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:15.522406 core_main_app-2.2.1/tests/utils/xsd_flattener/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:59.000000 core_main_app-2.2.1/tests/utils/xsd_flattener/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4358 2023-03-30 21:10:59.000000 core_main_app-2.2.1/tests/utils/xsd_flattener/tests_unit.py
-drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:11:15.567150 core_main_app-2.2.1/tests/views/
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-03-30 21:10:59.000000 core_main_app-2.2.1/tests/views/__init__.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4797 2023-03-30 21:10:59.000000 core_main_app-2.2.1/tests/views/fixtures.py
--rw-r--r--   0 jenisg    (1000) jenkins   (1000)    35505 2023-03-30 21:10:59.000000 core_main_app-2.2.1/tests/views/tests_int_access_control.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:23.024642 core_main_app-2.3.0/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1865 2023-05-02 19:39:54.000000 core_main_app-2.3.0/LICENSE.md
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      219 2023-05-02 19:39:54.000000 core_main_app-2.3.0/MANIFEST.in
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8195 2023-05-02 19:40:23.019734 core_main_app-2.3.0/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5952 2023-05-02 19:39:54.000000 core_main_app-2.3.0/README.rst
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:11.141853 core_main_app-2.3.0/core_main_app/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       81 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:11.277624 core_main_app-2.3.0/core_main_app/access_control/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/access_control/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11087 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/access_control/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      628 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/access_control/decorators.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      197 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/access_control/exceptions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6065 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1360 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/apps.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:11.401134 core_main_app-2.3.0/core_main_app/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/commons/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      412 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/commons/constants.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       62 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/commons/enums.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4063 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/commons/exceptions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       82 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/commons/regex.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      332 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/commons/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9154 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/commons/validators.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:11.419746 core_main_app-2.3.0/core_main_app/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:11.449817 core_main_app-2.3.0/core_main_app/components/abstract_data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/abstract_data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5240 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/abstract_data/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:11.530245 core_main_app-2.3.0/core_main_app/components/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/blob/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1118 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/blob/access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      315 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/blob/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2729 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/blob/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3493 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/blob/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      442 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/blob/utils.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:11.637531 core_main_app-2.3.0/core_main_app/components/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4384 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/data/access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5527 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/data/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8854 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/data/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5791 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/data/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10384 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/data/tasks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:11.669868 core_main_app-2.3.0/core_main_app/components/group/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/group/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1982 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/group/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:11.735350 core_main_app-2.3.0/core_main_app/components/lock/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/lock/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      330 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/lock/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2570 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/lock/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2665 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/lock/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:11.822113 core_main_app-2.3.0/core_main_app/components/mongo/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/mongo/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1041 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/mongo/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10440 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/mongo/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:11.896504 core_main_app-2.3.0/core_main_app/components/template/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/template/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4454 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/template/access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      362 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/template/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4434 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/template/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6655 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/template/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:11.968862 core_main_app-2.3.0/core_main_app/components/template_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/template_version_manager/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2328 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/template_version_manager/access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      507 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/template_version_manager/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6205 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/template_version_manager/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4719 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/template_version_manager/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:12.046399 core_main_app-2.3.0/core_main_app/components/template_xsl_rendering/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/template_xsl_rendering/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      338 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/template_xsl_rendering/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6892 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/template_xsl_rendering/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3434 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/template_xsl_rendering/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:12.081858 core_main_app-2.3.0/core_main_app/components/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2470 2023-05-02 19:39:54.000000 core_main_app-2.3.0/core_main_app/components/user/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:12.181067 core_main_app-2.3.0/core_main_app/components/version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/version_manager/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4883 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/version_manager/access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3744 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/version_manager/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3248 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/version_manager/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      550 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/version_manager/utils.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:12.242648 core_main_app-2.3.0/core_main_app/components/web_page/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/web_page/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1280 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/web_page/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1097 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/web_page/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:12.276722 core_main_app-2.3.0/core_main_app/components/web_page_login/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/web_page_login/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      809 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/web_page_login/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:12.366887 core_main_app-2.3.0/core_main_app/components/workspace/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/workspace/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2493 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/workspace/access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      372 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/workspace/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16858 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/workspace/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5695 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/workspace/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:12.432069 core_main_app-2.3.0/core_main_app/components/xsl_transformation/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/xsl_transformation/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      366 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/xsl_transformation/admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2542 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/xsl_transformation/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4469 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/components/xsl_transformation/models.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1791 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/menus.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:12.503910 core_main_app-2.3.0/core_main_app/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16483 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/migrations/0001_initial.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      751 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/migrations/0002_site_update.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1880 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/migrations/0003_psql_full_text.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      823 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/migrations/0004_template_ordering.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/migrations/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      733 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/models.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:12.632326 core_main_app-2.3.0/core_main_app/permissions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/permissions/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6351 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/permissions/api.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3152 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/permissions/discover.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      644 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/permissions/rights.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      230 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/permissions/utils.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:12.683755 core_main_app-2.3.0/core_main_app/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:12.745063 core_main_app-2.3.0/core_main_app/rest/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/blob/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4546 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/blob/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16319 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/blob/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:12.835586 core_main_app-2.3.0/core_main_app/rest/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7896 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/data/abstract_views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2006 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/data/admin_serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3187 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/data/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    36848 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/data/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:12.870507 core_main_app-2.3.0/core_main_app/rest/group/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/group/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      293 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/group/serializers.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:12.908156 core_main_app-2.3.0/core_main_app/rest/mongo_data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/mongo_data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1692 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/mongo_data/serializers.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:12.962235 core_main_app-2.3.0/core_main_app/rest/template/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/template/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      834 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/template/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4354 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/template/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.053400 core_main_app-2.3.0/core_main_app/rest/template_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/template_version_manager/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    10462 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/template_version_manager/abstract_views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2601 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/template_version_manager/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      587 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/template_version_manager/utils.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12274 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/template_version_manager/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.103565 core_main_app-2.3.0/core_main_app/rest/template_xsl_rendering/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/template_xsl_rendering/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1168 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/template_xsl_rendering/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14418 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/template_xsl_rendering/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14246 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.146962 core_main_app-2.3.0/core_main_app/rest/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1157 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/user/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      709 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/user/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2478 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.197981 core_main_app-2.3.0/core_main_app/rest/web_page/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/web_page/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1042 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/web_page/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4688 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/web_page/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.249793 core_main_app-2.3.0/core_main_app/rest/workspace/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/workspace/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      894 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/workspace/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    23285 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/workspace/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.311266 core_main_app-2.3.0/core_main_app/rest/xsl_transformation/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/xsl_transformation/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1437 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/xsl_transformation/serializers.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8160 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/rest/xsl_transformation/views.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8349 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/settings.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:09.841740 core_main_app-2.3.0/core_main_app/static/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:10.027334 core_main_app-2.3.0/core_main_app/static/core_main_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:09.871095 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:09.854917 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/_theme/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.376083 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/_theme/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      251 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/_theme/css/additional.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    47539 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/_theme/css/skins.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)   110978 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/_theme/css/theme.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.411146 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/_theme/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    22937 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/_theme/js/app.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      578 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/_theme/js/menu.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.443558 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1575 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/css/data_migration.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       81 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/css/permissions.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.465269 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/css/templates_xslt/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1363 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/css/templates_xslt/form.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.484385 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/css/web_page/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       31 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/css/web_page/style.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.502933 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      831 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/js/display_permissions.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.540098 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/js/templates/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    30064 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/js/templates/data_migration.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      594 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/js/templates/data_migration.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.596459 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/js/templates/upload/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1334 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/js/templates/upload/dependencies.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       94 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/js/templates/upload/dependencies.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      139 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/js/templates/upload/dependency_resolver.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.617513 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/js/templates_xslt/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1482 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/admin/js/templates_xslt/detail_xslt.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:09.989423 core_main_app-2.3.0/core_main_app/static/core_main_app/common/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.787598 core_main_app-2.3.0/core_main_app/static/core_main_app/common/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2236 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/css/XMLTree.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       68 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/css/buttons.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      178 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/css/fields.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       30 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/css/highlight.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       92 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/css/loading-spinner.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      474 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/css/select.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      392 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/css/share_link.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      940 2023-05-02 19:39:55.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/css/switch.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      486 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/css/table.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.801082 core_main_app-2.3.0/core_main_app/static/core_main_app/common/css/template/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       59 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/css/template/template_ordering.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      189 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/css/word-wrap.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.814588 core_main_app-2.3.0/core_main_app/static/core_main_app/common/css/workspace/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      333 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/css/workspace/table.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.839357 core_main_app-2.3.0/core_main_app/static/core_main_app/common/img/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      246 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/img/collapse.png
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      253 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/img/expand.png
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:13.990825 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      335 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/XMLTree.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      247 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/backtoprevious.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1828 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/csrf.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      192 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/data_detail.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      531 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/debounce.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      788 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/elementViewport.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      413 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/leave_notice.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      556 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/loading_spinner.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:14.089728 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1292 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/modals/add.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1136 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/modals/delete.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      481 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/modals/download.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      178 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/modals/download.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1257 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/modals/edit.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      439 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/modals/error_page_modal.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1950 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/notify-styles.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:14.125521 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:14.160858 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:14.211201 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1086 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/list/modals/disable.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      125 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/list/modals/disable.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      663 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/list/restore.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      124 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/list/restore.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1156 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/sort.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       97 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/sort.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:14.288764 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/versions/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:14.330352 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/versions/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1029 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/versions/modals/disable.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      108 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/versions/modals/disable.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      537 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/versions/restore.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      107 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/versions/restore.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      652 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/versions/set_current.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      111 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/versions/set_current.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:09.981688 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/xslt/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:09.984820 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/xslt/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:14.412065 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/xslt/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      859 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/xslt/list/modals/delete.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       64 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/xslt/list/modals/delete.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1012 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/xslt/list/modals/edit.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/xslt/list/modals/edit.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:14.429958 core_main_app-2.3.0/core_main_app/static/core_main_app/common/xsl/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1763 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/common/xsl/xml2html.xsl
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:14.447972 core_main_app-2.3.0/core_main_app/static/core_main_app/libs/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:10.020524 core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:14.649858 core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery/3.5.1/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    89475 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery/3.5.1/jquery.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:10.004465 core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:14.515379 core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:14.629612 core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7006 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_444444_256x240.png
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7074 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_555555_256x240.png
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4676 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_777620_256x240.png
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7013 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_777777_256x240.png
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4632 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6313 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    37326 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)   520714 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    18705 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.structure.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    18671 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.theme.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    21509 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/libs/notify.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:10.036444 core_main_app-2.3.0/core_main_app/static/core_main_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:14.735880 core_main_app-2.3.0/core_main_app/static/core_main_app/user/css/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       32 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/css/login.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       63 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/css/registration.css
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      387 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/css/text-editor.css
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:14.751718 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:14.797093 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      618 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/data/change_display.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      120 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/data/change_display.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      158 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/data/detail.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:14.827341 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/login/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      667 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/login/message.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       52 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/login/message.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1110 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/sharing_modal.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:14.900225 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/text_editor/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      154 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/text_editor/data_text_editor.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       73 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/text_editor/template_text_editor.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7080 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/text_editor/text_editor.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.012467 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1800 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/add_group.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      160 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/add_group.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1723 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/add_user.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      156 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/add_user.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1138 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/create_workspace.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       73 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/create_workspace.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      515 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/init.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       43 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/init.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:10.073284 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.196277 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      187 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/assign_blob_workspace.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      187 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/assign_data_workspace.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1455 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/assign_workspace.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1360 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/remove_rights.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       60 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/remove_rights.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      807 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_private.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       96 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_private.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      822 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_public.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       94 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_public.raw.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1728 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/switch_right.js
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      144 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/switch_right.raw.js
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.239777 core_main_app-2.3.0/core_main_app/system/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/system/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2302 2023-05-02 19:39:56.000000 core_main_app-2.3.0/core_main_app/system/api.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.256320 core_main_app-2.3.0/core_main_app/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:10.359455 core_main_app-2.3.0/core_main_app/templates/core_main_app/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:10.115107 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.278436 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1302 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/admin/app_wrapper.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.349754 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/admin/theme/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4775 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/admin/theme/base.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      223 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/admin/theme/footer.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      905 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/admin/theme/header.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2909 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/admin/theme/menu.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.412005 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/admin/theme/tools/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      620 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/admin/theme/tools/box.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/admin/theme/tools/form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      715 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/admin/theme/tools/modal.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      283 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/admin/theme/tools/section.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.428939 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/common/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      567 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/common/messages.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.475553 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1463 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/user/app_wrapper.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      902 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/user/default.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4855 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/user/theme_base.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.550891 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:10.147900 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/commons/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.591578 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/commons/errors/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      401 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/commons/errors/errors.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      254 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/commons/errors/errors_wrapper.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.621472 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/commons/upload/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      691 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/commons/upload/form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      313 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/commons/upload/upload.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      103 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/dashboard.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.674558 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      311 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/data/detail.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      383 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/data/detail_box.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1497 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/dependency_resolver.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      211 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/list_dependencies.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.742354 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.757697 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/data_migration/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7822 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/data_migration/templates_list.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      289 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/data_migration.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.790491 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1978 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/list/available.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      830 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/list/disabled.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.807268 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      813 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/list/modals/disable.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      542 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/list.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.824869 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/upload/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      399 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/upload/base.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      166 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/upload.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.855713 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/versions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3401 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/versions/available.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1158 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/versions/disabled.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.871572 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/versions/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      727 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/versions/modals/disable.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      677 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/versions.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.885628 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates_xslt/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.900097 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates_xslt/main/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4036 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates_xslt/main/form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      393 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates_xslt/main.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      860 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/upload_template.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.974598 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/web_page/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      166 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/web_page/login_page.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      804 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/web_page/main.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      387 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/web_page/web_page.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      375 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/web_page/web_page_unavailable.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:15.992011 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/workspaces/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      234 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/workspaces/edit_rights.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.028044 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/xslt/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.048461 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/xslt/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1236 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/xslt/list/table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      323 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/xslt/list.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.089446 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/xslt/upload/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       61 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/xslt/upload/base.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      161 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/xslt/upload.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:10.331431 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.204329 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/buttons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/buttons/add.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      152 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/buttons/back_to_previous.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/buttons/delete.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      190 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/buttons/edit.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      104 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/buttons/go_to.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      131 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/buttons/save_ordering.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.252471 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      189 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/commons/error.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       97 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/commons/form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      167 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/commons/form_delete.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.290828 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/commons/upload/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      578 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/commons/upload/form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      313 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/commons/upload/upload.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.320784 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      497 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/data/detail_data.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1716 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/data/tools_data.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.336749 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/defender/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       90 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/defender/error.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.426540 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      463 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/modals/add_page_modal.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      633 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/modals/create_data_modal.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      489 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/modals/delete_page_modal.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1066 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/modals/download-options.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      467 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/modals/edit_page_modal.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      429 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/modals/error_page_modal.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.444007 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/pagination/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3008 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/pagination/data_source_pagination.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.462656 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.498442 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1524 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates/list/available.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      801 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates/list/disabled.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.529465 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      805 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates/list/modals/disable.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      741 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates/list/modals/edit.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.548944 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates/versions/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2074 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates/versions/available.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.566369 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates/versions/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      663 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates/versions/modals/disable.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      265 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates/versions.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.621743 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates_xslt/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates_xslt/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.638800 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates_xslt/main/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      832 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates_xslt/main/form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      428 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates_xslt/main.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.665345 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/xslt/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.678728 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/xslt/list/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.710061 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/xslt/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      564 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/xslt/list/modals/delete.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      928 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/xslt/list/modals/edit.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1147 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/xslt/list/table.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      255 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/xslt/list.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.726780 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/xslt/upload/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       62 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/xslt/upload/base.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      163 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/common/xslt/upload.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.743116 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.768228 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      483 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/data/detail.html
+-rwxr-xr-x   0 jenisg    (1000) jenkins   (1000)      139 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/homepage.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.796980 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/login/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2215 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/login/main.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.812433 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/login/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      534 2023-05-02 19:39:57.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/login/modals/login_message.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      340 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/login/saml2_error.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.896082 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/registration/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      171 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/registration/password_reset_complete.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      390 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/registration/password_reset_confirm.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      499 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/registration/password_reset_done.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      362 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/registration/password_reset_email.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      180 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/registration/password_reset_form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       14 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/registration/password_reset_subject.txt
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.911321 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/sharing/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      274 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/sharing/button.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.938920 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/sharing/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      504 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/sharing/modals/multi-link.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      940 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/sharing/modals/single-link.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.966802 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/template/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      453 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/template/list_body.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       77 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/template/list_header.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.982344 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/text_editor/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3042 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/text_editor/text_editor.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:16.999809 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1184 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/edit_rights.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:17.031248 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1424 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/create_workspace.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1882 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/edit_rights_table.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:17.170474 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1613 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/add_group.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      193 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/add_group_form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1597 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/add_user.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      190 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/add_user_form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      832 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/assign_workspace.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      411 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/assign_workspace_form.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      958 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/remove_rights.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      883 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/set_private.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      892 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/set_public.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      675 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/switch_right.html
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      147 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templates/theme.html
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:17.307250 core_main_app-2.3.0/core_main_app/templatetags/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templatetags/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1086 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templatetags/auth_extras.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1097 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templatetags/blob_tags.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      367 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templatetags/dict_key_extras.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      514 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templatetags/get_attribute.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      598 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templatetags/include_static.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1124 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templatetags/json_date.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      642 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templatetags/stripjs.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      316 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templatetags/timestamptags.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3319 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/templatetags/xsl_transform_tag.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4501 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:17.882763 core_main_app-2.3.0/core_main_app/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:17.922136 core_main_app-2.3.0/core_main_app/utils/admin_site/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/admin_site/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1233 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/admin_site/model_admin_class.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      379 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/admin_site/view_only_admin.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2447 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/blob_downloader.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      405 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/boolean.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1137 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/checksum.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1876 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/custom_context_processors.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:17.949385 core_main_app-2.3.0/core_main_app/utils/databases/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/databases/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      627 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/databases/backend.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.001130 core_main_app-2.3.0/core_main_app/utils/databases/mongo/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      574 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/databases/mongo/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1584 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/databases/mongo/mongoengine_database.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      873 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/databases/mongo/pymongo_database.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      286 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/datetime.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9575 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/decorators.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2805 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/file.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      377 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/group.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.066009 core_main_app-2.3.0/core_main_app/utils/integration_tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/integration_tests/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      262 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/integration_tests/fixture_interface.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1641 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/integration_tests/integration_base_test_case.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1031 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/integration_tests/integration_base_transaction_test_case.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      319 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/labels.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.105448 core_main_app-2.3.0/core_main_app/utils/logger/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/logger/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1762 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/logger/logger_utils.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      438 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/markdown_parser.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      957 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/migrations.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.135129 core_main_app-2.3.0/core_main_app/utils/notifications/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/notifications/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3448 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/notifications/mail.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.163426 core_main_app-2.3.0/core_main_app/utils/notifications/tasks/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/notifications/tasks/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2566 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/notifications/tasks/task_mail.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.176093 core_main_app-2.3.0/core_main_app/utils/pagination/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/pagination/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.208625 core_main_app-2.3.0/core_main_app/utils/pagination/django_paginator/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/pagination/django_paginator/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      773 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/pagination/django_paginator/results_paginator.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.237415 core_main_app-2.3.0/core_main_app/utils/pagination/mongoengine_paginator/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/pagination/mongoengine_paginator/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1109 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/pagination/mongoengine_paginator/paginator.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.309347 core_main_app-2.3.0/core_main_app/utils/pagination/rest_framework_paginator/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/pagination/rest_framework_paginator/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      525 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/pagination/rest_framework_paginator/pagination.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1108 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/pagination/rest_framework_paginator/rest_framework_paginator.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      458 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/parser.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.344067 core_main_app-2.3.0/core_main_app/utils/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      145 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/query/constants.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.382674 core_main_app-2.3.0/core_main_app/utils/query/mongo/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/query/mongo/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14676 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/query/mongo/prepare.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3095 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/query/mongo/query_builder.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.475767 core_main_app-2.3.0/core_main_app/utils/raw_query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/raw_query/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1622 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/raw_query/common.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3901 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/raw_query/django_raw_query.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2134 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/raw_query/mongo_raw_query.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3182 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/rendering.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.551149 core_main_app-2.3.0/core_main_app/utils/requests_utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/requests_utils/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      568 2023-05-02 19:39:58.000000 core_main_app-2.3.0/core_main_app/utils/requests_utils/access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1663 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/requests_utils/requests_utils.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2054 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/requests_utils/ssl.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.651849 core_main_app-2.3.0/core_main_app/utils/resolvers/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/resolvers/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1184 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/resolvers/requests_resolver.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1072 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/resolvers/resolver_utils.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      194 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/resolvers/xsd_uri_resolvers.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.727680 core_main_app-2.3.0/core_main_app/utils/saml2/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/saml2/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8886 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/saml2/utils.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.788823 core_main_app-2.3.0/core_main_app/utils/storage/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/storage/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3523 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/storage/gridfs_storage.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1791 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/storage/storage.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.832828 core_main_app-2.3.0/core_main_app/utils/tests_tools/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      613 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/tests_tools/MockUser.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5344 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/tests_tools/RequestMock.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/tests_tools/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2238 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.956651 core_main_app-2.3.0/core_main_app/utils/validation/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/validation/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1162 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/validation/regex_validation.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      644 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/validation/xpath_validation.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:18.989580 core_main_app-2.3.0/core_main_app/utils/view_builders/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/view_builders/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6572 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/view_builders/data.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16047 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/xml.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:19.034215 core_main_app-2.3.0/core_main_app/utils/xsd_flattener/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/xsd_flattener/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2095 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/xsd_flattener/xsd_flattener_database_url.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1000 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/utils/xsd_flattener/xsd_flattener_requests_url.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:19.051016 core_main_app-2.3.0/core_main_app/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/views/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:19.111618 core_main_app-2.3.0/core_main_app/views/admin/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/views/admin/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4442 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/views/admin/ajax.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:19.128147 core_main_app-2.3.0/core_main_app/views/admin/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/views/admin/commons/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:19.165578 core_main_app-2.3.0/core_main_app/views/admin/commons/upload/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/views/admin/commons/upload/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      439 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/views/admin/commons/upload/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4457 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/views/admin/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    21048 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/views/admin/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:19.236417 core_main_app-2.3.0/core_main_app/views/common/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/views/common/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7191 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/views/common/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      459 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/views/common/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    31000 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/views/common/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:20.736534 core_main_app-2.3.0/core_main_app/views/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/views/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    16821 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/views/user/ajax.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5059 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/views/user/forms.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    14764 2023-05-02 19:39:59.000000 core_main_app-2.3.0/core_main_app/views/user/views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:11.209354 core_main_app-2.3.0/core_main_app.egg-info/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     8195 2023-05-02 19:40:06.000000 core_main_app-2.3.0/core_main_app.egg-info/PKG-INFO
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    31241 2023-05-02 19:40:09.000000 core_main_app-2.3.0/core_main_app.egg-info/SOURCES.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        1 2023-05-02 19:40:06.000000 core_main_app-2.3.0/core_main_app.egg-info/dependency_links.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      468 2023-05-02 19:40:07.000000 core_main_app-2.3.0/core_main_app.egg-info/requires.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       25 2023-05-02 19:40:07.000000 core_main_app-2.3.0/core_main_app.egg-info/top_level.txt
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:20.780481 core_main_app-2.3.0/docs/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:39:59.000000 core_main_app-2.3.0/docs/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11121 2023-05-02 19:40:00.000000 core_main_app-2.3.0/docs/conf.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      278 2023-05-02 19:40:00.000000 core_main_app-2.3.0/docs/conf_urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      170 2023-05-02 19:40:02.000000 core_main_app-2.3.0/pyproject.toml
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       18 2023-05-02 19:40:02.000000 core_main_app-2.3.0/requirements.core.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       92 2023-05-02 19:40:02.000000 core_main_app-2.3.0/requirements.dev.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       20 2023-05-02 19:40:02.000000 core_main_app-2.3.0/requirements.mongo.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      316 2023-05-02 19:40:02.000000 core_main_app-2.3.0/requirements.txt
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       38 2023-05-02 19:40:23.026275 core_main_app-2.3.0/setup.cfg
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2104 2023-05-02 19:40:02.000000 core_main_app-2.3.0/setup.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:20.870486 core_main_app-2.3.0/tests/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:20.903233 core_main_app-2.3.0/tests/access_control/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/access_control/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3415 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/access_control/tests_access_control.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:20.932772 core_main_app-2.3.0/tests/commons/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/commons/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3764 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/commons/tests_validators.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:20.946967 core_main_app-2.3.0/tests/components/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.003844 core_main_app-2.3.0/tests/components/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/blob/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.055246 core_main_app-2.3.0/tests/components/blob/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/blob/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3165 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/blob/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6398 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/blob/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    20676 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/blob/tests_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      440 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/blob/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.133841 core_main_app-2.3.0/tests/components/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/data/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.169923 core_main_app-2.3.0/tests/components/data/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/data/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    23919 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/data/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    66538 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/data/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    80876 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/data/tests_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3730 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/data/tests_int_ordering.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    27059 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/data/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.225584 core_main_app-2.3.0/tests/components/group/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/group/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.273391 core_main_app-2.3.0/tests/components/group/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/group/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      570 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/group/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      879 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/group/fixtures/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4760 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/group/tests_int.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.327329 core_main_app-2.3.0/tests/components/lock/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/lock/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4153 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/lock/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2440 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/lock/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.371912 core_main_app-2.3.0/tests/components/mongo_data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/mongo_data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    70475 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/mongo_data/tests_int_access_control.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.420744 core_main_app-2.3.0/tests/components/template/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/template/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.454933 core_main_app-2.3.0/tests/components/template/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/template/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2078 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/template/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    46022 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/template/tests_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7215 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/template/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.517694 core_main_app-2.3.0/tests/components/template_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/template_version_manager/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.550968 core_main_app-2.3.0/tests/components/template_version_manager/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/template_version_manager/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6470 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/template_version_manager/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    54873 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/template_version_manager/tests_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    17617 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/template_version_manager/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.602790 core_main_app-2.3.0/tests/components/template_xsl_rendering/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/template_xsl_rendering/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.644345 core_main_app-2.3.0/tests/components/template_xsl_rendering/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/template_xsl_rendering/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3266 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/template_xsl_rendering/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7896 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/template_xsl_rendering/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9565 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/template_xsl_rendering/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.678119 core_main_app-2.3.0/tests/components/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/user/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.721009 core_main_app-2.3.0/tests/components/user/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/user/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1552 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/user/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1429 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/user/fixtures/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7733 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/user/tests_int.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.786548 core_main_app-2.3.0/tests/components/version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/version_manager/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    61614 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/version_manager/tests_int_access_control.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9899 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/version_manager/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.816829 core_main_app-2.3.0/tests/components/web_page/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/web_page/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4846 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/web_page/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.846937 core_main_app-2.3.0/tests/components/web_page_login/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/web_page_login/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3905 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/web_page_login/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.875651 core_main_app-2.3.0/tests/components/workspace/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/workspace/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.919030 core_main_app-2.3.0/tests/components/workspace/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/workspace/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1235 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/workspace/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      919 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/workspace/fixtures/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     7478 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/workspace/tests_int.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.948447 core_main_app-2.3.0/tests/components/xsl_transformation/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/xsl_transformation/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12828 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/components/xsl_transformation/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      356 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/mocks.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:21.975865 core_main_app-2.3.0/tests/rest/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/rest/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.029568 core_main_app-2.3.0/tests/rest/blob/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/rest/blob/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    23641 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/rest/blob/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    19778 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/rest/blob/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)       36 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/rest/blob/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.117029 core_main_app-2.3.0/tests/rest/data/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/rest/data/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    47395 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/rest/data/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    36850 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/rest/data/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12424 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/rest/data/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.165051 core_main_app-2.3.0/tests/rest/template/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/rest/template/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2518 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/rest/template/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     5026 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/rest/template/tests_permission.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4802 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/rest/template/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.210737 core_main_app-2.3.0/tests/rest/template_version_manager/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/rest/template_version_manager/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    37232 2023-05-02 19:40:02.000000 core_main_app-2.3.0/tests/rest/template_version_manager/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    31920 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/template_version_manager/tests_permission.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3610 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/template_version_manager/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.257690 core_main_app-2.3.0/tests/rest/template_xsl_rendering/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/template_xsl_rendering/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11418 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/template_xsl_rendering/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    13879 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/template_xsl_rendering/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3549 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/tests_views.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.316146 core_main_app-2.3.0/tests/rest/user/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/user/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1737 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/user/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3137 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/user/tests_permissions.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      886 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/user/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.343344 core_main_app-2.3.0/tests/rest/web_page/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/web_page/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     6164 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/web_page/tests_permission.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.389766 core_main_app-2.3.0/tests/rest/workspace/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/workspace/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    71809 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/workspace/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    48644 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/workspace/tests_permissions.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.447003 core_main_app-2.3.0/tests/rest/xsl_transformation/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/xsl_transformation/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.490445 core_main_app-2.3.0/tests/rest/xsl_transformation/fixtures/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/xsl_transformation/fixtures/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1283 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/xsl_transformation/fixtures/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11618 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/xsl_transformation/tests_int.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    12753 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/xsl_transformation/tests_permission.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4365 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest/xsl_transformation/tests_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      529 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/rest_urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.527360 core_main_app-2.3.0/tests/system/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/system/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4668 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/system/test_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.559965 core_main_app-2.3.0/tests/templatetags/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/templatetags/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1364 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/templatetags/test_get_attribute.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2815 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/test_settings.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      293 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/test_settings_sqlite3.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     3445 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/urls.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.695930 core_main_app-2.3.0/tests/utils/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.729763 core_main_app-2.3.0/tests/utils/checksum/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/checksum/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1294 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/checksum/tests_checksum.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.763935 core_main_app-2.3.0/tests/utils/migrations/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/migrations/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1664 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/migrations/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.779013 core_main_app-2.3.0/tests/utils/query/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/query/__init__.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.813964 core_main_app-2.3.0/tests/utils/query/mongo/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/query/mongo/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     9855 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/query/mongo/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.854630 core_main_app-2.3.0/tests/utils/requests_utls/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/requests_utls/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1436 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/requests_utls/tests_ssl.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      902 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/test_unit_apps.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      772 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/test_unit_urls.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4010 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/tests_int_blob_downloader.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2624 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/tests_int_file.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     2368 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/tests_unit_admin_site.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1726 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/tests_unit_boolean.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)      402 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/tests_unit_parser.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    11988 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/tests_unit_xml_operation.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4334 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/tests_view_data.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.885895 core_main_app-2.3.0/tests/utils/validation/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/validation/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     1318 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/validation/tests_unit_validation.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:22.917664 core_main_app-2.3.0/tests/utils/xsd_flattener/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/xsd_flattener/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4358 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/utils/xsd_flattener/tests_unit.py
+drwxr-xr-x   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:23.003006 core_main_app-2.3.0/tests/views/
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)        0 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/views/__init__.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4797 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/views/fixtures.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)     4393 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/views/test_unit.py
+-rw-r--r--   0 jenisg    (1000) jenkins   (1000)    35415 2023-05-02 19:40:03.000000 core_main_app-2.3.0/tests/views/tests_int_access_control.py
```

### Comparing `core_main_app-2.2.1/LICENSE.md` & `core_main_app-2.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/PKG-INFO` & `core_main_app-2.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core_main_app
-Version: 2.2.1
+Version: 2.3.0
 Summary: Main functionalities for the curator core project
 Home-page: https://github.com/usnistgov/core_main_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =============
         Core Main App
@@ -147,14 +147,39 @@
         
         .. code:: py
         
           EMAIL_USE_TLS = True
           EMAIL_HOST_USER = 'testsite_app'
           EMAIL_HOST_PASSWORD = 'mys3cr3tp4ssw0rd'
         
+        Enable History
+        --------------
+        
+        Django Simple History allows keeping track of changes made to an object stored in the CDCS database.
+        First, install and configure the package. See the
+        `django-simple-history <https://django-simple-history.readthedocs.io/en/latest/quick_start.html>`_ documentation.
+        
+        Then, set the `DJANGO_SIMPLE_HISTORY_MODELS` setting with a list of models to track.
+        At the moment, this feature is only available for the `Data` model.
+        
+        .. code:: python
+        
+          DJANGO_SIMPLE_HISTORY_MODELS=["Data"]
+        
+        Register models to track by updating project files.
+        For example in ``mdcs/mdcs_home/admin.py``, add the following lines:
+        
+        .. code:: python
+        
+          from core_main_app.utils.admin_site.model_admin_class import register_simple_history_models
+          from django.conf import settings
+        
+          DJANGO_SIMPLE_HISTORY_MODELS = getattr(settings, "DJANGO_SIMPLE_HISTORY_MODELS", None)
+          register_simple_history_models(DJANGO_SIMPLE_HISTORY_MODELS)
+        
         Documentation
         =============
         
         Documentation has been generated using Sphinx. To generate a local version of
         the docs, please clone the repository and run:
         
         .. code:: bash
```

### Comparing `core_main_app-2.2.1/README.rst` & `core_main_app-2.3.0/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -139,14 +139,39 @@
 
 .. code:: py
 
   EMAIL_USE_TLS = True
   EMAIL_HOST_USER = 'testsite_app'
   EMAIL_HOST_PASSWORD = 'mys3cr3tp4ssw0rd'
 
+Enable History
+--------------
+
+Django Simple History allows keeping track of changes made to an object stored in the CDCS database.
+First, install and configure the package. See the
+`django-simple-history <https://django-simple-history.readthedocs.io/en/latest/quick_start.html>`_ documentation.
+
+Then, set the `DJANGO_SIMPLE_HISTORY_MODELS` setting with a list of models to track.
+At the moment, this feature is only available for the `Data` model.
+
+.. code:: python
+
+  DJANGO_SIMPLE_HISTORY_MODELS=["Data"]
+
+Register models to track by updating project files.
+For example in ``mdcs/mdcs_home/admin.py``, add the following lines:
+
+.. code:: python
+
+  from core_main_app.utils.admin_site.model_admin_class import register_simple_history_models
+  from django.conf import settings
+
+  DJANGO_SIMPLE_HISTORY_MODELS = getattr(settings, "DJANGO_SIMPLE_HISTORY_MODELS", None)
+  register_simple_history_models(DJANGO_SIMPLE_HISTORY_MODELS)
+
 Documentation
 =============
 
 Documentation has been generated using Sphinx. To generate a local version of
 the docs, please clone the repository and run:
 
 .. code:: bash
```

### Comparing `core_main_app-2.2.1/core_main_app/access_control/api.py` & `core_main_app-2.3.0/core_main_app/access_control/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,17 @@
     Returns:
 
     """
     # Raise error if anonymous user
     if user is None or user.is_anonymous:
         raise AccessControlError("Unable to write if not authenticated.")
 
+    if user.is_superuser:
+        return
+
     # TODO: data will inherit of workspace rights, which means a owner can't edit
     #  or delete a data if data in wkp that doesn't give hin write rights
     if hasattr(document, "workspace") and document.workspace is not None:
         if workspace_api.is_workspace_public(
             document.workspace
         ) and document.user_id == str(user.id):
             has_perm_publish(user, rights.PUBLISH_DATA)
@@ -287,17 +290,14 @@
         func:
         document:
         user:
 
     Returns:
 
     """
-    if user.is_superuser:
-        return func(document, user)
-
     check_can_write(document, user)
     return func(document, user)
 
 
 def can_request_write(func, document, request):
     """Can user request write
 
@@ -305,17 +305,14 @@
         func:
         document:
         request:
 
     Returns:
 
     """
-    if request.user.is_superuser:
-        return func(document, request)
-
     check_can_write(document, request.user)
     return func(document, request)
 
 
 def can_anonymous_access_public_data(func, *args, **kwargs):
     """Can anonymous access a public data
```

### Comparing `core_main_app-2.2.1/core_main_app/access_control/decorators.py` & `core_main_app-2.3.0/core_main_app/access_control/decorators.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/admin.py` & `core_main_app-2.3.0/core_main_app/admin.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/apps.py` & `core_main_app-2.3.0/core_main_app/apps.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,29 +12,39 @@
     verbose_name = "Core Main App"
 
     name = "core_main_app"
     """ :py:class:`str`: Package name
     """
 
     def ready(self):
-        from core_main_app.commons.exceptions import CoreError
         from core_main_app.permissions import discover
         from core_main_app.settings import SSL_CERTIFICATES_DIR
         from core_main_app.utils.requests_utils.ssl import (
             check_ssl_certificates_dir_setting,
         )
 
         """When the app is ready, run the discovery and init the indexes."""
         if "migrate" not in sys.argv:
-            # check celery settings
-            if (
-                settings.CELERYBEAT_SCHEDULER
-                != "django_celery_beat.schedulers:DatabaseScheduler"
-            ):
-                raise CoreError(
-                    "CELERYBEAT_SCHEDULER setting needs to be set "
-                    "to 'django_celery_beat.schedulers:DatabaseScheduler'."
-                )
+            _check_settings()
             check_ssl_certificates_dir_setting(SSL_CERTIFICATES_DIR)
             discover.init_rules(self.apps)
             discover.create_public_workspace()
             discover.init_mongo_indexing()
+
+
+def _check_settings():
+    """Check settings
+
+    Returns:
+
+    """
+    from core_main_app.commons.exceptions import CoreError
+
+    # check celery settings
+    if (
+        settings.CELERYBEAT_SCHEDULER
+        != "django_celery_beat.schedulers:DatabaseScheduler"
+    ):
+        raise CoreError(
+            "CELERYBEAT_SCHEDULER setting needs to be set "
+            "to 'django_celery_beat.schedulers:DatabaseScheduler'."
+        )
```

### Comparing `core_main_app-2.2.1/core_main_app/commons/exceptions.py` & `core_main_app-2.3.0/core_main_app/commons/exceptions.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/commons/validators.py` & `core_main_app-2.3.0/core_main_app/commons/validators.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/components/abstract_data/models.py` & `core_main_app-2.3.0/core_main_app/components/abstract_data/models.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/components/blob/access_control.py` & `core_main_app-2.3.0/core_main_app/components/blob/access_control.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/components/blob/api.py` & `core_main_app-2.3.0/core_main_app/components/blob/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/components/blob/models.py` & `core_main_app-2.3.0/core_main_app/components/blob/models.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/components/data/access_control.py` & `core_main_app-2.3.0/core_main_app/components/data/access_control.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/components/data/admin_site.py` & `core_main_app-2.3.0/core_main_app/components/data/admin_site.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """ Custom admin site for the Data model
 """
-from django.contrib import admin
+from django.conf import settings
 from django.contrib import messages
 from django.contrib.admin.helpers import ActionForm
 from django.forms import ChoiceField
 
 from core_main_app.commons.exceptions import DoesNotExist
 from core_main_app.components.user import api as user_api
 from core_main_app.components.workspace import api as workspace_api
-from django.conf import settings
+from core_main_app.utils.admin_site.model_admin_class import (
+    get_base_model_admin_class,
+)
 
 
 class UpdateActionForm(ActionForm):
     """Action form for data update"""
 
     user_id = ChoiceField(label="Owner:", required=False)
     workspace = ChoiceField(label="Workspace:", required=False)
@@ -133,15 +135,15 @@
             )
     except DoesNotExist as ex:
         model_admin.message_user(request, str(ex), messages.ERROR)
     except Exception as ex:
         model_admin.message_user(request, str(ex), messages.ERROR)
 
 
-class CustomDataAdmin(admin.ModelAdmin):
+class CustomDataAdmin(get_base_model_admin_class("Data")):
     """Custom Data Admin"""
 
     search_fields = ["title", "vector_column"]
     list_filter = ["template", "user_id", "workspace"]
     list_display = [
         "title",
         "last_modification_date",
```

### Comparing `core_main_app-2.2.1/core_main_app/components/data/api.py` & `core_main_app-2.3.0/core_main_app/components/data/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/components/data/models.py` & `core_main_app-2.3.0/core_main_app/components/data/models.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/components/data/tasks.py` & `core_main_app-2.3.0/core_main_app/components/data/tasks.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/components/group/api.py` & `core_main_app-2.3.0/core_main_app/components/group/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/components/lock/api.py` & `core_main_app-2.3.0/core_main_app/components/lock/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/components/lock/models.py` & `core_main_app-2.3.0/core_main_app/components/lock/models.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/components/mongo/api.py` & `core_main_app-2.3.0/core_main_app/components/mongo/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/components/mongo/models.py` & `core_main_app-2.3.0/core_main_app/components/mongo/models.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/components/template/access_control.py` & `core_main_app-2.3.0/core_main_app/components/template/access_control.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/components/template/api.py` & `core_main_app-2.3.0/core_main_app/components/template/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/components/template/models.py` & `core_main_app-2.3.0/core_main_app/components/template/models.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/components/template_version_manager/access_control.py` & `core_main_app-2.3.0/core_main_app/components/template_version_manager/access_control.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/components/template_version_manager/api.py` & `core_main_app-2.3.0/core_main_app/components/template_version_manager/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/components/template_version_manager/models.py` & `core_main_app-2.3.0/core_main_app/components/template_version_manager/models.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/components/template_xsl_rendering/api.py` & `core_main_app-2.3.0/core_main_app/components/template_xsl_rendering/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/components/template_xsl_rendering/models.py` & `core_main_app-2.3.0/core_main_app/components/template_xsl_rendering/models.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/components/user/api.py` & `core_main_app-2.3.0/core_main_app/components/user/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/components/version_manager/access_control.py` & `core_main_app-2.3.0/core_main_app/components/version_manager/access_control.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/components/version_manager/api.py` & `core_main_app-2.3.0/core_main_app/components/version_manager/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/components/version_manager/models.py` & `core_main_app-2.3.0/core_main_app/components/version_manager/models.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/components/version_manager/utils.py` & `core_main_app-2.3.0/core_main_app/components/version_manager/utils.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/components/web_page/api.py` & `core_main_app-2.3.0/core_main_app/components/web_page/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/components/web_page/models.py` & `core_main_app-2.3.0/core_main_app/components/web_page/models.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/components/web_page_login/api.py` & `core_main_app-2.3.0/core_main_app/components/web_page_login/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/components/workspace/access_control.py` & `core_main_app-2.3.0/core_main_app/components/workspace/access_control.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/components/workspace/api.py` & `core_main_app-2.3.0/core_main_app/components/workspace/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/components/workspace/models.py` & `core_main_app-2.3.0/core_main_app/components/workspace/models.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/components/xsl_transformation/api.py` & `core_main_app-2.3.0/core_main_app/components/xsl_transformation/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/components/xsl_transformation/models.py` & `core_main_app-2.3.0/core_main_app/components/xsl_transformation/models.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/menus.py` & `core_main_app-2.3.0/core_main_app/menus.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/migrations/0001_initial.py` & `core_main_app-2.3.0/core_main_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/migrations/0002_site_update.py` & `core_main_app-2.3.0/core_main_app/migrations/0002_site_update.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/migrations/0003_psql_full_text.py` & `core_main_app-2.3.0/core_main_app/migrations/0003_psql_full_text.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/migrations/0004_template_ordering.py` & `core_main_app-2.3.0/core_main_app/migrations/0004_template_ordering.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/models.py` & `core_main_app-2.3.0/core_main_app/models.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/permissions/api.py` & `core_main_app-2.3.0/core_main_app/permissions/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/permissions/discover.py` & `core_main_app-2.3.0/core_main_app/permissions/discover.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/permissions/rights.py` & `core_main_app-2.3.0/core_main_app/permissions/rights.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/rest/blob/serializers.py` & `core_main_app-2.3.0/core_main_app/rest/blob/serializers.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/rest/blob/views.py` & `core_main_app-2.3.0/core_main_app/rest/blob/views.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/rest/data/abstract_views.py` & `core_main_app-2.3.0/core_main_app/rest/data/abstract_views.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,66 +4,25 @@
 from abc import ABCMeta, abstractmethod
 
 from rest_framework import status
 from rest_framework.response import Response
 from rest_framework.views import APIView
 
 from core_main_app.access_control.exceptions import AccessControlError
+from core_main_app.commons.constants import DATA_JSON_FIELD
 from core_main_app.components.data import api as data_api
 from core_main_app.settings import DATA_SORTING_FIELDS
 from core_main_app.utils.query.constants import VISIBILITY_OPTION
 from core_main_app.utils.query.mongo.query_builder import QueryBuilder
 
 
 class AbstractExecuteLocalQueryView(APIView, metaclass=ABCMeta):
     """Abstract Execute Local Query View"""
 
-    sub_document_root = "dict_content"
-
-    def get(self, request):
-        """Execute query on local instance and return results
-
-        Parameters:
-
-            # get all results (paginated)
-            {"query": {}}
-            # get all results
-            {"query": {}, "all": "true"}
-            # get all results filtered by title
-            {"query": {}, "title": "title_string"}
-             # get all results filtered by workspaces
-            {"query": {}, "workspaces": [{"id":"[workspace_id]"}]}
-            # get all results filtered by private workspace
-            {"query": {}, "workspaces": [{"id":"None"}]}
-            # get all results filtered by templates
-            {"query": {}, "templates": [{"id":"[template_id]"}] }
-            # get all results that verify a given criteria
-            {"query": {"root.element.value": 2}}
-            # get values at xpath
-            {"query": {}, "xpath": "/ns:root/@element", "namespaces": {"ns": "<namespace_url>"}}
-            # get results using multiple options
-            {"query": {"root.element.value": 2}, "workspaces": [{"id":"workspace_id"}] , "all": "true"}
-            {"query": {"root.element.value": 2}, "templates": [{"id":"template_id"}] , "all": "true"}
-            {"query": {"root.element.value": 2}, "templates": [{"id":"template_id"}],
-            "workspaces": [{"id":"[workspace_id]"}] ,"all": "true"}
-
-        Args:
-
-            request: HTTP request
-
-        Returns:
-
-            - code: 200
-              content: List of data
-            - code: 400
-              content: Bad request
-            - code: 500
-              content: Internal server error
-        """
-        return self.execute_query()
+    sub_document_root = DATA_JSON_FIELD
 
     def post(self, request):
         """Execute query on local instance and return results
 
         Parameters:
 
             {"query": {"$or": [{"image.owner": "Peter"}, {"image.owner.#text":"Peter"}]}}
@@ -146,21 +105,21 @@
             The raw query
         """
         # build query builder
         query_builder = QueryBuilder(query, self.sub_document_root)
         # update the criteria with workspaces information
         if workspaces is not None and len(workspaces) > 0:
             list_workspace_ids = [
-                self._parser_id(workspace["id"]) for workspace in workspaces
+                self.parse_id(workspace["id"]) for workspace in workspaces
             ]
             query_builder.add_list_criteria("workspace", list_workspace_ids)
         # update the criteria with templates information
         if templates is not None and len(templates) > 0:
             list_template_ids = [
-                self._parser_id(template["id"]) for template in templates
+                self.parse_id(template["id"]) for template in templates
             ]
             query_builder.add_list_criteria("template", list_template_ids)
         # update the criteria with visibility information
         if options is not None and VISIBILITY_OPTION in options:
             query_builder.add_visibility_criteria(options[VISIBILITY_OPTION])
         # update the criteria with title information
         if title is not None:
@@ -196,15 +155,15 @@
         Returns:
 
             The response
         """
         raise NotImplementedError("build_response method is not implemented.")
 
     @staticmethod
-    def _parser_id(_id):
+    def parse_id(_id):
         try:
             return int(_id)
         except (ValueError, TypeError):
             return _id
 
 
 class AbstractMigrationView(APIView, metaclass=ABCMeta):
```

### Comparing `core_main_app-2.2.1/core_main_app/rest/data/admin_serializers.py` & `core_main_app-2.3.0/core_main_app/rest/data/admin_serializers.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/rest/data/serializers.py` & `core_main_app-2.3.0/core_main_app/rest/data/serializers.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/rest/data/views.py` & `core_main_app-2.3.0/core_main_app/rest/data/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -982,17 +982,15 @@
               content: Data was not found
             - raise: Exception
               content: Unknown error
         """
         try:
             # Get object
             data_object = self.get_object(request, id)
-
-            if not request.user.is_superuser:
-                check_can_write(data_object, request.user)
+            check_can_write(data_object, request.user)
             return True
         except AccessControlError:
             return False
         except Exception as exception:
             raise exception
```

### Comparing `core_main_app-2.2.1/core_main_app/rest/mongo_data/serializers.py` & `core_main_app-2.3.0/core_main_app/rest/mongo_data/serializers.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/rest/template/serializers.py` & `core_main_app-2.3.0/core_main_app/rest/template/serializers.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/rest/template/views.py` & `core_main_app-2.3.0/core_main_app/rest/template/views.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/rest/template_version_manager/abstract_views.py` & `core_main_app-2.3.0/core_main_app/rest/template_version_manager/abstract_views.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/rest/template_version_manager/serializers.py` & `core_main_app-2.3.0/core_main_app/rest/template_version_manager/serializers.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/rest/template_version_manager/utils.py` & `core_main_app-2.3.0/core_main_app/rest/template_version_manager/utils.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/rest/template_version_manager/views.py` & `core_main_app-2.3.0/core_main_app/rest/template_version_manager/views.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/rest/template_xsl_rendering/serializers.py` & `core_main_app-2.3.0/core_main_app/rest/template_xsl_rendering/serializers.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/rest/template_xsl_rendering/views.py` & `core_main_app-2.3.0/core_main_app/rest/template_xsl_rendering/views.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/rest/urls.py` & `core_main_app-2.3.0/core_main_app/rest/urls.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/rest/user/serializers.py` & `core_main_app-2.3.0/core_main_app/rest/user/serializers.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/rest/user/views.py` & `core_main_app-2.3.0/core_main_app/rest/user/views.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/rest/views.py` & `core_main_app-2.3.0/core_main_app/rest/views.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/rest/web_page/serializers.py` & `core_main_app-2.3.0/core_main_app/rest/web_page/serializers.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/rest/web_page/views.py` & `core_main_app-2.3.0/core_main_app/rest/web_page/views.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/rest/workspace/serializers.py` & `core_main_app-2.3.0/core_main_app/rest/workspace/serializers.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/rest/workspace/views.py` & `core_main_app-2.3.0/core_main_app/rest/workspace/views.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/rest/xsl_transformation/serializers.py` & `core_main_app-2.3.0/core_main_app/rest/xsl_transformation/serializers.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/rest/xsl_transformation/views.py` & `core_main_app-2.3.0/core_main_app/rest/xsl_transformation/views.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/settings.py` & `core_main_app-2.3.0/core_main_app/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 if not settings.configured:
     settings.configure()
 
 CUSTOM_NAME = getattr(settings, "CUSTOM_NAME", "Local")
 """ :py:class:`str`: Name of the local instance
 """
 
+BOOTSTRAP_VERSION = getattr(settings, "BOOTSTRAP_VERSION", "4.6.2")
+""" :py:class:`str`: Version of the boostrap library.
+"""
+
 SERVER_URI = getattr(settings, "SERVER_URI", "http://127.0.0.1:8000")
 """ :py:class:`str`: Server URI for import reference.
 """
 
 XSD_UPLOAD_DIR = getattr(settings, "XSD_UPLOAD_DIR", "xml_schemas")
 """ :py:class:`str`: Name of the media folder where XML schemas are uploaded to.
 """
@@ -241,7 +245,13 @@
 GA_TRACKING_ID = getattr(settings, "GA_TRACKING_ID", None)
 """ :py:class:`str`: Google Analytics tracking ID. Adds gtag to user pages if set.
 """
 
 MAX_DOCUMENT_EDITING_SIZE = 128 * 1024
 """ :py:class:`int`: Maximum byte size allowed for document editing.
 """
+
+DJANGO_SIMPLE_HISTORY_MODELS = getattr(
+    settings, "DJANGO_SIMPLE_HISTORY_MODELS", None
+)
+""" :py:class:`list`: Track history of listed models.
+"""
```

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/admin/_theme/css/skins.css` & `core_main_app-2.3.0/core_main_app/static/core_main_app/admin/_theme/css/skins.css`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/admin/_theme/css/theme.css` & `core_main_app-2.3.0/core_main_app/static/core_main_app/admin/_theme/css/theme.css`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/admin/_theme/js/app.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/admin/_theme/js/app.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/admin/_theme/js/menu.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/admin/_theme/js/menu.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/admin/css/data_migration.css` & `core_main_app-2.3.0/core_main_app/static/core_main_app/admin/css/data_migration.css`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/admin/css/templates_xslt/form.css` & `core_main_app-2.3.0/core_main_app/static/core_main_app/admin/css/templates_xslt/form.css`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/admin/js/display_permissions.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/admin/js/display_permissions.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/admin/js/templates/data_migration.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/admin/js/templates/data_migration.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/admin/js/templates/data_migration.raw.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/admin/js/templates/data_migration.raw.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/admin/js/templates/upload/dependencies.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/admin/js/templates/upload/dependencies.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/admin/js/templates_xslt/detail_xslt.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/admin/js/templates_xslt/detail_xslt.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/common/css/XMLTree.css` & `core_main_app-2.3.0/core_main_app/static/core_main_app/common/css/XMLTree.css`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/common/css/switch.css` & `core_main_app-2.3.0/core_main_app/static/core_main_app/common/css/switch.css`

 * *Files 18% similar despite different names*

```diff
@@ -45,7 +45,12 @@
 }
 
 input:checked + .slider:before {
   -webkit-transform: translateX(26px);
   -ms-transform: translateX(26px);
   transform: translateX(26px);
 }
+
+.row > * {
+  padding: 0;
+  margin: 0;
+}
```

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/csrf.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/csrf.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/debounce.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/debounce.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/elementViewport.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/elementViewport.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/loading_spinner.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/loading_spinner.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/modals/add.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/modals/add.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/modals/delete.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/modals/delete.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/modals/edit.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/modals/edit.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/notify-styles.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/notify-styles.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 $.notify.addStyle(
     'default', {
-        html: "<div><i class='fas fa-info-circle'/> <span data-notify-text/></div>",
+        html: "<div><i class='fas fa-info-circle'></i>&nbsp;<span data-notify-text></span></div>",
         classes: {
             base: {
                 "padding": "8px 15px",
                 "font-size": "1.1em",
                 "color": "#3A87AD",
                 "background-color": "#D9EDF7",
                 "border": "1px solid #BCE8F1",
@@ -12,31 +12,31 @@
                 "white-space": "nowrap"
             }
         }
     });
 
 $.notify.addStyle(
     'success', {
-        html: "<div><i class='fas fa-check-circle'/> <span data-notify-text/></div>",
+        html: "<div><i class='fas fa-check-circle'></i>&nbsp;<span data-notify-text></span></div>",
         classes: {
             base: {
                 "padding": "8px 15px",
-                "font-size": "1.1em",
+                "font-size": "1.2em",
                 "color": "#468847",
                 "background-color": "#DFF0D8",
                 "border": "1px solid #D6E9C6",
                 "border-radius": "4px",
                 "white-space": "nowrap"
             }
         }
     });
 
 $.notify.addStyle(
     'info', {
-        html: "<div><i class='fas fa-info-circle'/> <span data-notify-text/></div>",
+        html: "<div><i class='fas fa-info-circle'></i>&nbsp;<span data-notify-text></span></div>",
         classes: {
             base: {
                 "padding": "8px 15px",
                 "font-size": "1.1em",
                 "color": "#3A87AD",
                 "background-color": "#D9EDF7",
                 "border": "1px solid #BCE8F1",
@@ -44,15 +44,15 @@
                 "white-space": "nowrap"
             }
         }
     });
 
 $.notify.addStyle(
     'warning', {
-        html: "<div><i class='fas fa-exclamation-triangle'/> <span data-notify-text/></div>",
+        html: "<div><i class='fas fa-exclamation-triangle'></i>&nbsp;<span data-notify-text></span></div>",
         classes: {
             base: {
                 "padding": "8px 15px",
                 "font-size": "1.1em",
                 "color": "#C09853",
                 "background-color": "#FCF8E3",
                 "border": "1px solid #FBEED5",
@@ -60,15 +60,15 @@
                 "white-space": "nowrap"
             }
         }
     });
 
 $.notify.addStyle(
     'error', {
-        html: "<div><i class='fas fa-exclamation-circle'/> <span data-notify-text/></div>",
+        html: "<div><i class='fas fa-exclamation-circle'></i>&nbsp;<span data-notify-text></span></div>",
         classes: {
             base: {
                 "padding": "8px 15px",
                 "font-size": "1.1em",
                 "color": "#B94A48",
                 "background-color": "#F2DEDE",
                 "border": "1px solid #EED3D7",
```

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/templates/list/modals/disable.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/list/modals/disable.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/templates/list/restore.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/list/restore.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/templates/sort.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/sort.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/templates/versions/modals/disable.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/versions/modals/disable.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/templates/versions/restore.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/versions/restore.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/templates/versions/set_current.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/templates/versions/set_current.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/xslt/list/modals/delete.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/xslt/list/modals/delete.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/common/js/xslt/list/modals/edit.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/common/js/xslt/list/modals/edit.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/common/xsl/xml2html.xsl` & `core_main_app-2.3.0/core_main_app/static/core_main_app/common/xsl/xml2html.xsl`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/libs/jquery/3.5.1/jquery.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery/3.5.1/jquery.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_444444_256x240.png` & `core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_555555_256x240.png` & `core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_777620_256x240.png` & `core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_777777_256x240.png` & `core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_cc0000_256x240.png` & `core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_ffffff_256x240.png` & `core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.css` & `core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.structure.css` & `core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.structure.css`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.theme.css` & `core_main_app-2.3.0/core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.theme.css`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/libs/notify.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/libs/notify.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/data/change_display.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/data/change_display.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/login/message.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/login/message.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/sharing_modal.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/sharing_modal.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/text_editor/text_editor.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/text_editor/text_editor.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -1,22 +1,23 @@
 let jqError = $('.alert-danger');
 let documentID = null
 let documentName = null
 let templateID = null
 let textEditorUrl = null
 let showHTML = false
 let useModal = false
-
+let lineNumbers = 1
 
 /**
  * Load controllers for text editor
  */
 $(document).ready(function() {
     documentID = $("#document_id").html()
     editorType = $("#editor_type").html()
+    refreshLineNumbers()
     switch (editorType) {
         case "XSD":
             textEditorUrl = xsdTextEditorUrl
             break;
 
         default:
             templateID = $("#template_id").html();
@@ -30,19 +31,22 @@
     }
 
 
     $('.btn.display').on('click', display);
     $('.btn.format').on('click', format);
     $('.btn.refresh').on('click', refresh);
     $('.btn.validate').on('click', validate);
+    $('.btn.generate').on('click', generate);
     $('.btn.save').on('click', function() {
         if (useModal) createDataModal();
         else save();
     });
-
+    $(".input").scroll(function() {
+        $(".line-number").prop("scrollTop", this.scrollTop);
+    });
 
 });
 
 /**
  * AJAX, to save content
  */
 let save = function() {
@@ -64,14 +68,15 @@
         error: function(data) {
             jqError.html('<i class="fas fa-exclamation-triangle"></i> ' + data.responseText);
             jqError.show();
         }
     }).always(function(data) {
         // get old button icon
         hideSpinner($(".save > i"), icon)
+        refreshLineNumbers();
     });
     if (useModal) $("#create-data-modal").modal("hide");
 };
 
 /**
  * AJAX, to  format content
  */
@@ -89,25 +94,25 @@
         },
         dataType: "json",
         success: function(data) {
             $.notify("Document formatted successfully", {
                 style: "success"
             });
             html = hljs.highlightAuto(data).value
-            $(".content-highlight").html(html)
+            $(".input").html("<pre class=\"content-highlight m-1\">" + html + "</pre>")
         },
         error: function(data) {
-
             jqError.html('<i class="fas fa-exclamation-triangle"></i> ' + data.responseText);
             jqError.show();
 
         }
     }).always(function(data) {
         // get old button icon
         hideSpinner($(".format > i"), icon)
+        refreshLineNumbers();
     });
 };
 
 /**
  * AJAX, to validate content
  */
 var validate = function() {
@@ -132,14 +137,15 @@
         error: function(data) {
             jqError.html('<i class="fas fa-exclamation-triangle"></i> ' + data.responseText);
             jqError.show();
         }
     }).always(function(data) {
         // get old button icon
         hideSpinner($(".validate > i"), icon)
+        refreshLineNumbers();
     });
 
 };
 
 /**
  * AJAX, to refresh html content
  */
@@ -184,23 +190,78 @@
     $(".representation").attr('hidden', showHTML)
     $(".refresh").attr('hidden', showHTML)
     $("#xslt-selector").attr('hidden', showHTML)
     if (showHTML) {
         $(".input").css("width", "100%");
         $(".display").children().attr('class', 'fas fa-eye');
     } else {
-        $(".input").css("width", "49%");
+        $(".input").css("width", "45%");
+        $(".test").css("width", "45%");
         $(".input").css("display", "inline-block");
         $(".display").children().attr('class', 'fas fa-eye-slash');
 
     }
     showHTML = !showHTML
     hideSpinner($(".display > i"), icon)
 }
 
+/**
+ * AJAX, to generate content
+ */
+let generate = function() {
+    jqError.hide()
+    var icon = $(".generate > i").attr("class");
+    // Show loading spinner
+    showSpinner($(".generate > i"))
+    $.ajax({
+        url: textEditorUrl,
+        type: "POST",
+        data: {
+            'content': $(".input").text(),
+            'template_id': templateID,
+            'action': 'generate',
+        },
+        dataType: "json",
+        success: function(data) {
+            $.notify("Document generated successfully", {
+                style: "success"
+            });
+            html = hljs.highlightAuto(data).value
+            $(".input").html("<pre class=\"content-highlight m-1\">" + html + "</pre>")
+        },
+        error: function(data) {
+            jqError.html('<i class="fas fa-exclamation-triangle"></i> ' + data.responseText);
+            jqError.show();
+
+        }
+    }).always(function(data) {
+        // get old button icon
+        hideSpinner($(".generate > i"), icon)
+        // setup line numbers
+        refreshLineNumbers();
+    });
+};
+
+
 
 /**
  * Shows a dialog to choose dialog options
  */
 let createDataModal = function() {
     $("#create-data-modal").modal("show");
+}
+
+
+/**
+ * Refresh Line Numbers
+ */
+let refreshLineNumbers = function() {
+    if (lineNumbers != $(".input").text().split('\n').length) {
+        var htmlLineNumber = ""
+        lineNumbers = $(".input").text().split('\n').length
+        for (i = 1; i < lineNumbers; i++) {
+            htmlLineNumber += "<div>" + i + "</div>"
+        }
+        $(".line-number").html(htmlLineNumber)
+    }
+
 }
```

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/workspaces/add_group.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/add_user.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -1,67 +1,61 @@
 /**
  * AJAX call
  */
-load_form_add_group = function() {
-    $("#add-group-modal").modal("show");
-    $('#add-group-yes').show();
+load_form_add_user = function() {
+    $("#banner_rights_errors").hide();
+    $("#user-rights").show()
+    $('#add-user-yes').show();
+    $("#add-user-modal").modal("show");
 
     $.ajax({
-        url: editGroupRightFormsUrl,
+        url: editUserRightFormsUrl,
         type: "POST",
         dataType: "json",
         data: {
             workspace_id: workspace_id
         },
         success: function(data) {
-            $("#banner_rights_errors").hide();
-            $("#add-group-form").html(data.form);
-            InitSelectMultipleUsersOrGroups("#add-group-form #id_groups", "Groups");
+            $("#add-user-form").html(data.form);
         },
         error: function(data) {
-            $("#form_edit_group_rights_errors").html(data.responseText);
-            $("#banner_group_rights_errors").show(500);
-            $('#add-group-yes').hide();
+            $("#form_edit_rights_errors").html(data.responseText);
+            $("#banner_rights_errors").show(500);
+            $("#user-rights").hide();
+            $('#add-user-yes').hide();
         }
     });
 };
 
-add_group_from_form = function() {
-    var selected = [];
-    var select = document.getElementById("id_groups");
-    var read = document.getElementById("read_group").checked;
-    var write = document.getElementById("write_group").checked;
-
-    for (var i = 0; i < select.options.length; i++) {
-        if (select.options[i].selected == true) {
-            selected.push(select.options[i].value);
-        }
-    }
-    call_ajax_add_group(selected, read, write)
+add_user_from_form = function() {
+    var selected = new FormData($("#add-user-form")[0]).getAll("users");
+    var read = document.getElementById("read").checked;
+    var write = document.getElementById("write").checked;
+    call_ajax_add_user(selected, read, write)
 };
 
-call_ajax_add_group = function(selected, read, write) {
+call_ajax_add_user = function(selected, read, write) {
     event.preventDefault()
-    $("#banner_group_rights_errors").hide();
-    $("#form_edit_group_rights_errors").html("");
+    $("#banner_rights_errors").hide();
+    $("#form_edit_rights_errors").html("");
     $.ajax({
-        url: addGroupToWorkspaceUrl,
+        url: addUserToWorkspaceUrl,
         type: "POST",
         dataType: "json",
         data: {
             workspace_id: workspace_id,
-            groups_id: selected,
+            users_id: selected,
             read: read,
             write: write
         },
         success: function(data) {
             location.reload();
         },
         error: function(data) {
-            $("#form_edit_group_rights_errors").html(data.responseText);
-            $("#banner_group_rights_errors").show(500);
+            $("#form_edit_rights_errors").html(data.responseText);
+            $("#banner_rights_errors").show(500);
         }
     });
 };
 
-$('.add-group-btn').on('click', load_form_add_group);
-$('#add-group-yes').on('click', add_group_from_form);
+$('.add-user-btn').on('click', load_form_add_user);
+$('#add-user-yes').on('click', add_user_from_form);
```

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/workspaces/create_workspace.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/create_workspace.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/workspaces/init.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/init.js`

 * *Files 21% similar despite different names*

#### js-beautify {}

```diff
@@ -10,18 +10,8 @@
     });
 
     // Use the hash to select the correct tab (if available)
     var url = document.location.toString();
     if (url.match('#')) {
         $('.nav-tabs a[href="#' + url.split('#')[1] + '"]').tab('show');
     }
-});
-
-InitSelectMultipleUsersOrGroups = function(path_elt, place_holder) {
-    $(path_elt).fSelect({
-        placeholder: place_holder,
-        numDisplayed: 500,
-        overflowText: '{n} selected',
-        searchText: 'Search',
-        showSearch: true
-    });
-};
+});
```

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/workspaces/list/modals/assign_workspace.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/assign_workspace.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/workspaces/list/modals/remove_rights.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/remove_rights.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_private.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_private.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_public.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_public.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/static/core_main_app/user/js/workspaces/list/modals/switch_right.js` & `core_main_app-2.3.0/core_main_app/static/core_main_app/user/js/workspaces/list/modals/switch_right.js`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/system/api.py` & `core_main_app-2.3.0/core_main_app/system/api.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/_render/admin/app_wrapper.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/admin/app_wrapper.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/_render/admin/theme/header.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/admin/theme/header.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/_render/admin/theme/menu.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/admin/theme/menu.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/_render/admin/theme/tools/box.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/admin/theme/tools/box.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/_render/admin/theme/tools/modal.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/admin/theme/tools/modal.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/_render/common/messages.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/common/messages.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/_render/user/app_wrapper.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/user/app_wrapper.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/_render/user/default.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/_render/user/default.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/commons/upload/form.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/commons/upload/form.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/dependency_resolver.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/dependency_resolver.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/templates/data_migration/templates_list.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/data_migration/templates_list.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/templates/list/available.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/list/available.html`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 {% block box_tools %}
     <a href="{% url 'core-admin:core_main_app_upload_template'%}" class="float-right btn btn-secondary">
         <i class="fas fa-upload"></i> Upload {{ data.object_name }}
     </a>
 {% endblock %}
 
 {% block box_body %}
+<p>
+This page lists all Templates uploaded by admin users. Use drag and drop to update the order templates appear
+on the website, then click on "Save ordering" when done.
+</p>
 <table class="table table-bordered table-striped table-hover" data-reorderable-rows="true">
     <tr>
         <th>Display order</th>
         <th width="35%">{{ data.object_name }}</th>
         <th>Actions</th>
     </tr>
```

#### html2text {}

```diff
@@ -1,11 +1,14 @@
 {% extends 'core_main_app/_render/admin/theme/tools/box.html' %} {% block
 box_title %}Available{% endblock %} {% block box_tools %}
  Upload_{{_data.object_name_}}
  {% endblock %} {% block box_body %}
+This page lists all Templates uploaded by admin users. Use drag and drop to
+update the order templates appear on the website, then click on "Save ordering"
+when done.
 Display order              {{ data.object_name }} Actions
                                                   {% block box_actions %}
                                                    Versions
 {% if object.display_rank                          {% url
 %} {{object.display_rank}} {{ object.title }}     'core_main_app_edit_template'
 {%else %} - {%endif%}                             object.id as edit_url %} {%
                                                   include 'core_main_app/
```

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/templates/list/disabled.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/list/disabled.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/templates/list/modals/disable.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/list/modals/disable.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/templates/list.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/list.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/templates/versions/available.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/versions/available.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/templates/versions/disabled.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/versions/disabled.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/templates/versions/modals/disable.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/versions/modals/disable.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/templates/versions.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates/versions.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/templates_xslt/main/form.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/templates_xslt/main/form.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/upload_template.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/upload_template.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/web_page/main.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/web_page/main.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/admin/xslt/list/table.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/admin/xslt/list/table.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/common/commons/upload/form.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/common/commons/upload/form.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/common/data/tools_data.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/common/data/tools_data.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/common/modals/create_data_modal.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/common/modals/create_data_modal.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/common/modals/download-options.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/common/modals/download-options.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/common/pagination/data_source_pagination.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/common/pagination/data_source_pagination.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/common/templates/list/available.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates/list/available.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/common/templates/list/disabled.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates/list/disabled.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/common/templates/list/modals/disable.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates/list/modals/disable.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/common/templates/list/modals/edit.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates/list/modals/edit.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/common/templates/versions/available.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates/versions/available.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/common/templates/versions/modals/disable.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates/versions/modals/disable.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/common/templates_xslt/main/form.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/common/templates_xslt/main/form.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/common/xslt/list/modals/delete.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/common/xslt/list/modals/delete.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/common/xslt/list/modals/edit.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/common/xslt/list/modals/edit.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/common/xslt/list/table.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/common/xslt/list/table.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/user/login/main.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/user/login/main.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/user/login/modals/login_message.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/user/login/modals/login_message.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/user/sharing/modals/single-link.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/user/sharing/modals/single-link.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/user/text_editor/text_editor.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/user/text_editor/text_editor.html`

 * *Files 12% similar despite different names*

```diff
@@ -14,43 +14,47 @@
 
 <div class="alert alert-danger m-2" style="display: none;" role="alert">
     <i class="fas fa-exclamation-triangle"></i>
 </div>
 
 
 <div>
-    <div class="border rounded input" contenteditable="true">
-        <pre class="content-highlight m-1"><code>{{data.content}}</code></pre>
-    </div>
-
-    {% if data.type == 'XML' %}
+    <div class="row m-1">
+        <div class="border rounded bg-light line-number"><div>1</div></div>
+        <div class="border rounded input col" contenteditable="true">
+            <pre class="content-highlight m-1"><code>{{data.content}}</code></pre>
+        </div>
+        {% if data.type == 'XML' %}
         <div class="border rounded bg-light representation " hidden>
             <div class="tree m-2">
                 {% xsl_transform_detail xml_content=data.content template_id=data.template_id xslt_id=data.xsl_transformation_id request=request as xml_representation %}
                 {% if 'core_file_preview_app' in INSTALLED_APPS %}
                     {% render_blob_links_in_span xml_string=xml_representation as xml_representation %}
                 {% endif %}
 
                 {{ xml_representation|safe}}
             </div>
         </div>
     {% endif %}
+    </div>
+
 </div>
 
 
 <div class="float-right m-2">
         {% if data.type == 'XML' %}
             <select class="selectpicker form-control" style="width:100px; display:inline-block" id="xslt-selector" hidden>
                            {% if not data.template_xsl_rendering.default_detail_xslt %}  <option value={{None}}>Default</option>{% endif %}
                            {% for xslt in data.template_xsl_rendering.list_detail_xslt.all %}
                                 <option value="{{xslt.id}}" {% if xslt.id == xslt_id %} selected {% endif %}>{{xslt.name}} {% if xslt == template_xsl_rendering.default_detail_xslt %} (default) {% endif %}</option>
                            {% endfor %}
             </select>
             <button class="btn btn-secondary refresh mr-auto" hidden><i class="fas fa-sync" ></i> Refresh  </button>
             <button class="btn btn-secondary display mr-auto"><i class="fas fa-eye" ></i> Display  </button>
+            <button class="btn btn-secondary generate mr-auto"><i class="fas fa-cogs" ></i> Generate </button>
         {% endif %}
     	<button class="btn btn-secondary format mr-auto"><i class="fas fa-paint-brush"></i> Format </button>
         <button class="btn btn-secondary validate"><i class="fas fa-check"></i> Validate </button>
         <button class="btn btn-success save mr-auto"><i class="fas fa-save"></i> Save </button>
 
 
 </div>
```

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/user/workspaces/edit_rights.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/edit_rights.html`

 * *Files 10% similar despite different names*

```diff
@@ -17,25 +17,25 @@
          <i class="fas fa-arrow-left"></i> Previous page
 </a>
 {% endblock %}
 
 {% block box_body %}
 <br/>
     <!--FIXME: put back the tab -->
+    <h4>Users:</h4>
     {% if data.user_data %}
-        Users
         {% include data.template with objects=data.user_data group="user" %}
     {% else %}
     <div class="empty-table">
         No users have access to '{{ data.workspace.title }}'.
     </div>
     {% endif %}
 <br/>
+    <h4>Groups:</h4>
     {% if data.group_data %}
-        Groups
         {% include data.template with objects=data.group_data group="group" %}
     {%else%}
       <div class="empty-table">
         No groups have access to '{{ data.workspace.title }}'.
       </div>
     {%endif%}
 {% endblock %}
```

#### html2text {}

```diff
@@ -3,15 +3,17 @@
 {% block box_tools %} {% if not data.is_public %}
  Add users
 
  Add groups
  {% endif %}
  Previous_page
  {% endblock %} {% block box_body %}
- {% if data.user_data %} Users {% include data.template with
-objects=data.user_data group="user" %} {% else %}
+*** Users: ***
+{% if data.user_data %} {% include data.template with objects=data.user_data
+group="user" %} {% else %}
 No users have access to '{{ data.workspace.title }}'.
 {% endif %}
-{% if data.group_data %} Groups {% include data.template with
-objects=data.group_data group="group" %} {%else%}
+*** Groups: ***
+{% if data.group_data %} {% include data.template with objects=data.group_data
+group="group" %} {%else%}
 No groups have access to '{{ data.workspace.title }}'.
 {%endif%} {% endblock %}
```

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/user/workspaces/list/create_workspace.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/create_workspace.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/user/workspaces/list/modals/add_group.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/set_private.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,56 @@
 00000000: 7b25 2065 7874 656e 6473 2027 636f 7265  {% extends 'core
 00000010: 5f6d 6169 6e5f 6170 702f 5f72 656e 6465  _main_app/_rende
 00000020: 722f 6164 6d69 6e2f 7468 656d 652f 746f  r/admin/theme/to
 00000030: 6f6c 732f 6d6f 6461 6c2e 6874 6d6c 2720  ols/modal.html' 
 00000040: 257d 0a0a 7b25 2062 6c6f 636b 206d 6f64  %}..{% block mod
-00000050: 616c 5f69 6420 257d 6164 642d 6772 6f75  al_id %}add-grou
-00000060: 702d 6d6f 6461 6c7b 2520 656e 6462 6c6f  p-modal{% endblo
-00000070: 636b 2025 7d0a 7b25 2062 6c6f 636b 206d  ck %}.{% block m
-00000080: 6f64 616c 5f74 6974 6c65 2025 7d20 4769  odal_title %} Gi
-00000090: 7665 2067 726f 7570 2072 6967 6874 7320  ve group rights 
-000000a0: 746f 2077 6f72 6b73 7061 6365 207b 2520  to workspace {% 
-000000b0: 656e 6462 6c6f 636b 2025 7d0a 0a7b 2520  endblock %}..{% 
-000000c0: 626c 6f63 6b20 6d6f 6461 6c5f 626f 6479  block modal_body
-000000d0: 2025 7d0a 3c64 6976 2063 6c61 7373 3d22   %}.<div class="
-000000e0: 616c 6572 7420 616c 6572 742d 6461 6e67  alert alert-dang
-000000f0: 6572 2220 6964 3d22 6261 6e6e 6572 5f67  er" id="banner_g
-00000100: 726f 7570 5f72 6967 6874 735f 6572 726f  roup_rights_erro
-00000110: 7273 2220 7374 796c 653d 2264 6973 706c  rs" style="displ
-00000120: 6179 3a20 6e6f 6e65 3b22 3e0a 2020 2020  ay: none;">.    
-00000130: 3c68 343e 3c69 2063 6c61 7373 3d22 6661  <h4><i class="fa
-00000140: 7320 6661 2d65 7863 6c61 6d61 7469 6f6e  s fa-exclamation
-00000150: 2d63 6972 636c 6520 6661 2d31 7822 3e3c  -circle fa-1x"><
-00000160: 2f69 3e20 4572 726f 723c 2f68 343e 0a20  /i> Error</h4>. 
-00000170: 2020 203c 6469 7620 6964 3d22 666f 726d     <div id="form
-00000180: 5f65 6469 745f 6772 6f75 705f 7269 6768  _edit_group_righ
-00000190: 7473 5f65 7272 6f72 7322 3e0a 2020 2020  ts_errors">.    
-000001a0: 3c2f 6469 763e 0a3c 2f64 6976 3e0a 0a53  </div>.</div>..S
-000001b0: 656c 6563 7420 616c 6c20 6772 6f75 7073  elect all groups
-000001c0: 2079 6f75 2077 616e 7420 746f 2067 6976   you want to giv
-000001d0: 6520 7269 6768 7473 2074 6f20 7468 6520  e rights to the 
-000001e0: 776f 726b 7370 6163 653a 0a3c 6469 7620  workspace:.<div 
-000001f0: 6964 3d22 6164 642d 6772 6f75 702d 666f  id="add-group-fo
-00000200: 726d 223e 0a3c 2f64 6976 3e0a 3c64 6976  rm">.</div>.<div
-00000210: 2069 643d 226c 6973 742d 7269 6768 7473   id="list-rights
-00000220: 223e 0a20 2020 203c 6c61 6265 6c20 636c  ">.    <label cl
-00000230: 6173 733d 2273 7769 7463 6822 3e0a 2020  ass="switch">.  
-00000240: 2020 2020 2020 3c69 6e70 7574 2074 7970        <input typ
-00000250: 653d 2263 6865 636b 626f 7822 2069 643d  e="checkbox" id=
-00000260: 2272 6561 645f 6772 6f75 7022 3e0a 2020  "read_group">.  
-00000270: 2020 2020 2020 3c73 7061 6e20 636c 6173        <span clas
-00000280: 733d 2273 6c69 6465 7222 3e3c 2f73 7061  s="slider"></spa
-00000290: 6e3e 0a20 2020 203c 2f6c 6162 656c 3e20  n>.    </label> 
-000002a0: 5265 6164 0a20 2020 203c 6272 2f3e 0a20  Read.    <br/>. 
-000002b0: 2020 203c 6c61 6265 6c20 636c 6173 733d     <label class=
-000002c0: 2273 7769 7463 6822 3e0a 2020 2020 2020  "switch">.      
-000002d0: 2020 3c69 6e70 7574 2074 7970 653d 2263    <input type="c
-000002e0: 6865 636b 626f 7822 2069 643d 2277 7269  heckbox" id="wri
-000002f0: 7465 5f67 726f 7570 223e 0a20 2020 2020  te_group">.     
-00000300: 2020 203c 7370 616e 2063 6c61 7373 3d22     <span class="
-00000310: 736c 6964 6572 223e 3c2f 7370 616e 3e0a  slider"></span>.
-00000320: 2020 2020 3c2f 6c61 6265 6c3e 2057 7269      </label> Wri
-00000330: 7465 0a3c 2f64 6976 3e0a 7b25 2065 6e64  te.</div>.{% end
-00000340: 626c 6f63 6b20 257d 0a0a 7b25 2062 6c6f  block %}..{% blo
-00000350: 636b 206d 6f64 616c 5f66 6f6f 7465 7220  ck modal_footer 
-00000360: 257d 0a3c 6120 636c 6173 733d 2262 746e  %}.<a class="btn
-00000370: 2062 746e 2d73 6563 6f6e 6461 7279 2070   btn-secondary p
-00000380: 756c 6c2d 6c65 6674 2220 6461 7461 2d64  ull-left" data-d
-00000390: 6973 6d69 7373 3d22 6d6f 6461 6c22 2068  ismiss="modal" h
-000003a0: 7265 663d 2223 223e 3c69 2063 6c61 7373  ref="#"><i class
-000003b0: 3d22 6661 7320 6661 2d74 696d 6573 223e  ="fas fa-times">
-000003c0: 3c2f 693e 2043 616e 6365 6c3c 2f61 3e0a  </i> Cancel</a>.
-000003d0: 3c61 2069 643d 2261 6464 2d67 726f 7570  <a id="add-group
-000003e0: 2d79 6573 2220 636c 6173 733d 2262 746e  -yes" class="btn
-000003f0: 2062 746e 2d73 6563 6f6e 6461 7279 2220   btn-secondary" 
-00000400: 6872 6566 3d22 2322 3e3c 6920 636c 6173  href="#"><i clas
-00000410: 733d 2266 6173 2066 612d 6368 6563 6b22  s="fas fa-check"
-00000420: 3e3c 2f69 3e20 4164 643c 2f61 3e0a 7b25  ></i> Add</a>.{%
-00000430: 2065 6e64 626c 6f63 6b20 257d 0a0a        endblock %}..
+00000050: 616c 5f69 6420 257d 7072 6976 6174 652d  al_id %}private-
+00000060: 776f 726b 7370 6163 652d 6d6f 6461 6c7b  workspace-modal{
+00000070: 2520 656e 6462 6c6f 636b 2025 7d0a 7b25  % endblock %}.{%
+00000080: 2062 6c6f 636b 206d 6f64 616c 5f74 6974   block modal_tit
+00000090: 6c65 2025 7d53 6574 2077 6f72 6b73 7061  le %}Set workspa
+000000a0: 6365 2070 7269 7661 7465 7b25 2065 6e64  ce private{% end
+000000b0: 626c 6f63 6b20 257d 0a0a 0a7b 2520 626c  block %}...{% bl
+000000c0: 6f63 6b20 6d6f 6461 6c5f 626f 6479 2025  ock modal_body %
+000000d0: 7d0a 3c64 6976 2063 6c61 7373 3d22 616c  }.<div class="al
+000000e0: 6572 7420 616c 6572 742d 6461 6e67 6572  ert alert-danger
+000000f0: 2220 6964 3d22 6261 6e6e 6572 5f65 7272  " id="banner_err
+00000100: 6f72 7322 2073 7479 6c65 3d22 6469 7370  ors" style="disp
+00000110: 6c61 793a 206e 6f6e 653b 223e 0a20 2020  lay: none;">.   
+00000120: 2020 2020 203c 6120 6872 6566 3d22 2322       <a href="#"
+00000130: 2063 6c61 7373 3d22 636c 6f73 6522 2064   class="close" d
+00000140: 6174 612d 6869 6465 3d22 616c 6572 7422  ata-hide="alert"
+00000150: 2061 7269 612d 6c61 6265 6c3d 2263 6c6f   aria-label="clo
+00000160: 7365 223e 2674 696d 6573 3b3c 2f61 3e0a  se">&times;</a>.
+00000170: 2020 2020 2009 3c68 343e 3c69 2063 6c61       .<h4><i cla
+00000180: 7373 3d22 6661 7320 6661 2d65 7863 6c61  ss="fas fa-excla
+00000190: 6d61 7469 6f6e 2d63 6972 636c 6522 3e3c  mation-circle"><
+000001a0: 2f69 3e20 4572 726f 723c 2f68 343e 0a20  /i> Error</h4>. 
+000001b0: 2020 2020 2020 203c 6469 7620 6964 3d22         <div id="
+000001c0: 7072 6976 6174 655f 776f 726b 7370 6163  private_workspac
+000001d0: 655f 6572 726f 7273 223e 3c2f 6469 763e  e_errors"></div>
+000001e0: 0a3c 2f64 6976 3e0a 3c69 6e70 7574 2074  .</div>.<input t
+000001f0: 7970 653d 2268 6964 6465 6e22 2063 6c61  ype="hidden" cla
+00000200: 7373 3d22 7b7b 6461 7461 2e64 6f63 756d  ss="{{data.docum
+00000210: 656e 747d 7d2d 6964 222f 3e0a 3c70 3e41  ent}}-id"/>.<p>A
+00000220: 7265 2079 6f75 2073 7572 6520 796f 7520  re you sure you 
+00000230: 7761 6e74 2074 6f20 7365 7420 7468 6520  want to set the 
+00000240: 776f 726b 7370 6163 6520 7072 6976 6174  workspace privat
+00000250: 653f 3c2f 703e 0a7b 2520 656e 6462 6c6f  e?</p>.{% endblo
+00000260: 636b 2025 7d0a 0a7b 2520 626c 6f63 6b20  ck %}..{% block 
+00000270: 6d6f 6461 6c5f 666f 6f74 6572 2025 7d0a  modal_footer %}.
+00000280: 3c61 2063 6c61 7373 3d22 6274 6e20 6274  <a class="btn bt
+00000290: 6e2d 7365 636f 6e64 6172 7920 7075 6c6c  n-secondary pull
+000002a0: 2d6c 6566 7422 2064 6174 612d 6469 736d  -left" data-dism
+000002b0: 6973 733d 226d 6f64 616c 2220 6872 6566  iss="modal" href
+000002c0: 3d22 2322 3e0a 2020 2020 3c69 2063 6c61  ="#">.    <i cla
+000002d0: 7373 3d22 6661 7320 6661 2d74 696d 6573  ss="fas fa-times
+000002e0: 223e 3c2f 693e 2043 616e 6365 6c0a 3c2f  "></i> Cancel.</
+000002f0: 613e 0a3c 6120 6964 3d22 7072 6976 6174  a>.<a id="privat
+00000300: 652d 776f 726b 7370 6163 652d 7965 7322  e-workspace-yes"
+00000310: 2063 6c61 7373 3d22 6274 6e20 6274 6e2d   class="btn btn-
+00000320: 7072 696d 6172 7922 2068 7265 663d 2223  primary" href="#
+00000330: 223e 0a20 2020 203c 6920 636c 6173 733d  ">.    <i class=
+00000340: 2266 6173 2066 612d 6368 6563 6b22 3e3c  "fas fa-check"><
+00000350: 2f69 3e20 5365 7420 7072 6976 6174 650a  /i> Set private.
+00000360: 3c2f 613e 0a7b 2520 656e 6462 6c6f 636b  </a>.{% endblock
+00000370: 2025 7d                                   %}
```

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/user/workspaces/list/modals/assign_workspace.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/assign_workspace.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/user/workspaces/list/modals/remove_rights.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/remove_rights.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/user/workspaces/list/modals/set_private.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/set_public.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 {% extends 'core_main_app/_render/admin/theme/tools/modal.html' %}
 
-{% block modal_id %}private-workspace-modal{% endblock %}
-{% block modal_title %}Set workspace private{% endblock %}
+{% block modal_id %}public-workspace-modal{% endblock %}
+{% block modal_title %}Set workspace public{% endblock %}
 
 
 {% block modal_body %}
-<div class="alert alert-danger" id="banner_errors" style="display: none;">
+<div class="alert alert-danger" id="banner_set_public_errors" style="display: none;">
         <a href="#" class="close" data-hide="alert" aria-label="close">&times;</a>
      	<h4><i class="fas fa-exclamation-circle"></i> Error</h4>
-        <div id="private_workspace_errors"></div>
+        <div id="set_public_workspace_errors"></div>
 </div>
 <input type="hidden" class="{{data.document}}-id"/>
-<p>Are you sure you want to set the workspace private?</p>
+<p>Are you sure you want to set the workspace public?</p>
 {% endblock %}
 
 {% block modal_footer %}
 <a class="btn btn-secondary pull-left" data-dismiss="modal" href="#">
     <i class="fas fa-times"></i> Cancel
 </a>
-<a id="private-workspace-yes" class="btn btn-primary" href="#">
-    <i class="fas fa-check"></i> Set private
+<a id="public-workspace-yes" class="btn btn-primary" href="#">
+    <i class="fas fa-check"></i> Set public
 </a>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 {% extends 'core_main_app/_render/admin/theme/tools/modal.html' %} {% block
-modal_id %}private-workspace-modal{% endblock %} {% block modal_title %}Set
-workspace private{% endblock %} {% block modal_body %}
+modal_id %}public-workspace-modal{% endblock %} {% block modal_title %}Set
+workspace public{% endblock %} {% block modal_body %}
 ×
  Error
-Are you sure you want to set the workspace private?
+Are you sure you want to set the workspace public?
 {% endblock %} {% block modal_footer %}
  Cancel
 
- Set_private
+ Set_public
  {% endblock %}
```

### Comparing `core_main_app-2.2.1/core_main_app/templates/core_main_app/user/workspaces/list/modals/switch_right.html` & `core_main_app-2.3.0/core_main_app/templates/core_main_app/user/workspaces/list/modals/switch_right.html`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templatetags/auth_extras.py` & `core_main_app-2.3.0/core_main_app/templatetags/auth_extras.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templatetags/blob_tags.py` & `core_main_app-2.3.0/core_main_app/templatetags/blob_tags.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templatetags/get_attribute.py` & `core_main_app-2.3.0/core_main_app/templatetags/get_attribute.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templatetags/include_static.py` & `core_main_app-2.3.0/core_main_app/templatetags/include_static.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templatetags/json_date.py` & `core_main_app-2.3.0/core_main_app/templatetags/json_date.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templatetags/stripjs.py` & `core_main_app-2.3.0/core_main_app/templatetags/stripjs.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/templatetags/xsl_transform_tag.py` & `core_main_app-2.3.0/core_main_app/templatetags/xsl_transform_tag.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/urls.py` & `core_main_app-2.3.0/core_main_app/urls.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """ Url router for the main application
 """
 from django.conf.urls import include
 from django.contrib.auth.decorators import login_required
-from django.urls import re_path, reverse_lazy
+from django.urls import re_path
 from drf_yasg import openapi
 from drf_yasg.views import get_schema_view
 
-from core_main_app import settings
 from core_main_app.components.blob import api as blob_api
 from core_main_app.components.data import api as data_api
 from core_main_app.utils.rendering import render
+from core_main_app.utils.urls import get_auth_urls
 from core_main_app.views.common import (
     ajax as common_ajax,
     views as common_views,
 )
 from core_main_app.views.user import views as user_views, ajax as user_ajax
 
 SchemaView = get_schema_view(
@@ -36,15 +36,14 @@
         common_views.ViewData.as_view(),
         name="core_main_app_data_detail",
     ),
     re_path(
         r"^xml-editor/data",
         login_required(
             common_views.DataContentEditor.as_view(),
-            login_url=reverse_lazy("core_main_app_login"),
         ),
         name="core_main_app_xml_text_editor_view",
     ),
     re_path(
         r"^template/versions/(?P<version_manager_id>\w+)",
         user_views.manage_template_versions,
         name="core_main_app_manage_template_versions",
@@ -142,34 +141,8 @@
     re_path(
         r"^change-data-display",
         user_ajax.change_data_display,
         name="core_main_add_change_data_display",
     ),
 ]
 
-if settings.ENABLE_SAML2_SSO_AUTH:
-    from djangosaml2 import views as saml2_views
-
-    urlpatterns.append(re_path(r"saml2/", include("djangosaml2.urls")))
-    urlpatterns.append(
-        re_path(
-            r"^saml2/login",
-            saml2_views.LoginView.as_view(),
-            name="core_main_app_login",
-        )
-    )
-    urlpatterns.append(
-        re_path(
-            r"^saml2/logout",
-            saml2_views.LogoutInitView.as_view(),
-            name="core_main_app_logout",
-        )
-    )
-else:
-    urlpatterns.append(
-        re_path(r"^login", user_views.custom_login, name="core_main_app_login")
-    )
-    urlpatterns.append(
-        re_path(
-            r"^logout", user_views.custom_logout, name="core_main_app_logout"
-        )
-    )
+urlpatterns.extend(get_auth_urls())
```

### Comparing `core_main_app-2.2.1/core_main_app/utils/blob_downloader.py` & `core_main_app-2.3.0/core_main_app/utils/blob_downloader.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/utils/checksum.py` & `core_main_app-2.3.0/core_main_app/utils/checksum.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/utils/custom_context_processors.py` & `core_main_app-2.3.0/core_main_app/utils/custom_context_processors.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,8 +43,15 @@
         else [],
         "DISPLAY_NIST_HEADERS": settings.DISPLAY_NIST_HEADERS
         if hasattr(settings, "DISPLAY_NIST_HEADERS")
         else False,
         "GA_TRACKING_ID": settings.GA_TRACKING_ID
         if hasattr(settings, "GA_TRACKING_ID")
         else None,
+        "LOGIN_URL": settings.LOGIN_URL
+        if hasattr(settings, "LOGIN_URL")
+        else "",
+        "BOOTSTRAP_VERSION": settings.BOOTSTRAP_VERSION
+        if hasattr(settings, "BOOTSTRAP_VERSION")
+        and settings.BOOTSTRAP_VERSION in ["4.6.2", "5.1.3"]
+        else "4.6.2",
     }
```

### Comparing `core_main_app-2.2.1/core_main_app/utils/databases/backend.py` & `core_main_app-2.3.0/core_main_app/utils/databases/backend.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/utils/databases/mongo/__init__.py` & `core_main_app-2.3.0/core_main_app/utils/databases/mongo/__init__.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/utils/databases/mongo/mongoengine_database.py` & `core_main_app-2.3.0/core_main_app/utils/databases/mongo/mongoengine_database.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/utils/databases/mongo/pymongo_database.py` & `core_main_app-2.3.0/core_main_app/utils/databases/mongo/pymongo_database.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/utils/decorators.py` & `core_main_app-2.3.0/core_main_app/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/utils/file.py` & `core_main_app-2.3.0/core_main_app/utils/file.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/utils/integration_tests/integration_base_test_case.py` & `core_main_app-2.3.0/core_main_app/utils/integration_tests/integration_base_test_case.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 
 from core_main_app.commons.exceptions import CoreError
 
 MOCK_DATABASE_NAME = "db_mock"
 MOCK_DATABASE_HOST = "mongomock://localhost"
 
 
-# FIXME: Remove Mongo from name
-class MongoIntegrationBaseTestCase(TestCase):
+class IntegrationBaseTestCase(TestCase):
     """Represent the Integration base test case
     The integration tests must inherit of this class
     """
 
     """
         Fields
     """
```

### Comparing `core_main_app-2.2.1/core_main_app/utils/integration_tests/integration_base_transaction_test_case.py` & `core_main_app-2.3.0/core_main_app/utils/integration_tests/integration_base_transaction_test_case.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 from django.core.management import execute_from_command_line
 from django.test.testcases import TransactionTestCase
 
 from core_main_app.components.group import api as group_api
 from core_main_app.permissions import rights
 
 
-# FIXME: Remove Mongo from name
-class MongoIntegrationTransactionTestCase(TransactionTestCase):
+class IntegrationTransactionTestCase(TransactionTestCase):
     """Represent the Integration base transaction test case
     The integration tests must inherit of this class
     """
 
     """
         Fields
     """
```

### Comparing `core_main_app-2.2.1/core_main_app/utils/logger/logger_utils.py` & `core_main_app-2.3.0/core_main_app/utils/logger/logger_utils.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/utils/migrations.py` & `core_main_app-2.3.0/core_main_app/utils/migrations.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/utils/notifications/mail.py` & `core_main_app-2.3.0/core_main_app/utils/notifications/mail.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/utils/notifications/tasks/task_mail.py` & `core_main_app-2.3.0/core_main_app/utils/notifications/tasks/task_mail.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/utils/pagination/django_paginator/results_paginator.py` & `core_main_app-2.3.0/core_main_app/utils/pagination/django_paginator/results_paginator.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/utils/pagination/mongoengine_paginator/paginator.py` & `core_main_app-2.3.0/core_main_app/utils/pagination/mongoengine_paginator/paginator.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/utils/pagination/rest_framework_paginator/pagination.py` & `core_main_app-2.3.0/core_main_app/utils/pagination/rest_framework_paginator/pagination.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/utils/pagination/rest_framework_paginator/rest_framework_paginator.py` & `core_main_app-2.3.0/core_main_app/utils/pagination/rest_framework_paginator/rest_framework_paginator.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/utils/query/mongo/prepare.py` & `core_main_app-2.3.0/core_main_app/utils/query/mongo/prepare.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/utils/query/mongo/query_builder.py` & `core_main_app-2.3.0/core_main_app/utils/query/mongo/query_builder.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/utils/raw_query/common.py` & `core_main_app-2.3.0/core_main_app/utils/raw_query/common.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/utils/raw_query/django_raw_query.py` & `core_main_app-2.3.0/core_main_app/utils/raw_query/django_raw_query.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/utils/raw_query/mongo_raw_query.py` & `core_main_app-2.3.0/core_main_app/utils/raw_query/mongo_raw_query.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/utils/rendering.py` & `core_main_app-2.3.0/core_main_app/utils/rendering.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/utils/requests_utils/access_control.py` & `core_main_app-2.3.0/core_main_app/utils/requests_utils/access_control.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/utils/requests_utils/requests_utils.py` & `core_main_app-2.3.0/core_main_app/utils/requests_utils/requests_utils.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/utils/requests_utils/ssl.py` & `core_main_app-2.3.0/core_main_app/utils/requests_utils/ssl.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/utils/resolvers/requests_resolver.py` & `core_main_app-2.3.0/core_main_app/utils/resolvers/requests_resolver.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/utils/resolvers/resolver_utils.py` & `core_main_app-2.3.0/core_main_app/utils/resolvers/resolver_utils.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/utils/saml2/utils.py` & `core_main_app-2.3.0/core_main_app/utils/saml2/utils.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/utils/storage/gridfs_storage.py` & `core_main_app-2.3.0/core_main_app/utils/storage/gridfs_storage.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/utils/storage/storage.py` & `core_main_app-2.3.0/core_main_app/utils/storage/storage.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/utils/tests_tools/MockUser.py` & `core_main_app-2.3.0/core_main_app/utils/tests_tools/MockUser.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/utils/tests_tools/RequestMock.py` & `core_main_app-2.3.0/core_main_app/utils/tests_tools/RequestMock.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/utils/validation/regex_validation.py` & `core_main_app-2.3.0/core_main_app/utils/validation/regex_validation.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,9 +45,9 @@
 
     Returns:
 
     """
     # Run validate filename from Django
     validate_file_name(filename)
     # Regex check filename has extension
-    if re.match(r"^[\w]+\.[a-z0-9]{2,4}$", filename) is None:
+    if re.match(r"^[a-zA-Z0-9-_]+\.[a-z0-9]{2,4}$", filename) is None:
         raise ValidationError("Invalid filename.")
```

### Comparing `core_main_app-2.2.1/core_main_app/utils/validation/xpath_validation.py` & `core_main_app-2.3.0/core_main_app/utils/validation/xpath_validation.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/utils/view_builders/data.py` & `core_main_app-2.3.0/core_main_app/utils/view_builders/data.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/utils/xml.py` & `core_main_app-2.3.0/core_main_app/utils/xml.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/utils/xsd_flattener/xsd_flattener_database_url.py` & `core_main_app-2.3.0/core_main_app/utils/xsd_flattener/xsd_flattener_database_url.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/utils/xsd_flattener/xsd_flattener_requests_url.py` & `core_main_app-2.3.0/core_main_app/utils/xsd_flattener/xsd_flattener_requests_url.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/views/admin/ajax.py` & `core_main_app-2.3.0/core_main_app/views/admin/ajax.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/views/admin/forms.py` & `core_main_app-2.3.0/core_main_app/views/admin/forms.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/views/admin/views.py` & `core_main_app-2.3.0/core_main_app/views/admin/views.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/views/common/ajax.py` & `core_main_app-2.3.0/core_main_app/views/common/ajax.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/core_main_app/views/common/views.py` & `core_main_app-2.3.0/core_main_app/views/common/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-"""
-    Common views
+""" Common views
 """
 import json
 from abc import ABCMeta, abstractmethod
+from datetime import datetime
 
+from django.conf import settings as conf_settings
 from django.contrib import messages
 from django.contrib.auth.decorators import login_required
 from django.http import (
     HttpResponseBadRequest,
     HttpResponseForbidden,
     HttpResponse,
 )
@@ -190,36 +191,23 @@
         if workspace_api.is_workspace_public(workspace):
             context.update({"is_public": True})
         if workspace_api.is_workspace_global(workspace):
             context.update({"is_global": True})
 
         assets = {
             "css": [
-                "core_main_app/libs/datatables/1.10.13/css/jquery.dataTables.css",
-                "core_main_app/libs/fSelect/css/fSelect.css",
                 "core_main_app/common/css/switch.css",
+                "core_main_app/common/css/select.css",
             ],
             "js": [
                 {
-                    "path": "core_main_app/libs/datatables/1.10.13/js/jquery.dataTables.js",
-                    "is_raw": True,
-                },
-                {
-                    "path": "core_main_app/libs/fSelect/js/fSelect.js",
-                    "is_raw": False,
-                },
-                {
                     "path": "core_main_app/common/js/backtoprevious.js",
                     "is_raw": True,
                 },
                 {
-                    "path": "core_main_app/user/js/workspaces/tables.js",
-                    "is_raw": True,
-                },
-                {
                     "path": "core_main_app/user/js/workspaces/add_user.js",
                     "is_raw": False,
                 },
                 {
                     "path": "core_main_app/user/js/workspaces/list/modals/switch_right.js",
                     "is_raw": False,
                 },
@@ -522,25 +510,17 @@
         """
         assets = {
             "js": [
                 {
                     "path": "core_main_app/user/js/text_editor/text_editor.js",
                     "is_raw": True,
                 },
-                {
-                    "path": "core_main_app/libs/highlight/11.0.0/js/highlight.min.js",
-                    "is_raw": False,
-                },
-                {
-                    "path": "core_main_app/libs/highlight/11.0.0/js/init_highlight.js",
-                    "is_raw": False,
-                },
             ],
             "css": [
-                "core_main_app/libs/highlight/11.0.0/css/atom-one-light.css",
+                "core_main_app/common/css/highlight.css",
                 "core_main_app/user/css/text-editor.css",
             ],
         }
         return assets
 
     def _get_context(self, document_id, document_name, type_content, content):
         """get context
@@ -684,14 +664,91 @@
         if error is not None:
             raise exceptions.XMLError(error)
         return HttpResponse(
             json.dumps("Validated successfully"),
             "application/javascript",
         )
 
+    def generate(self, *args, **kwargs):
+        """Generate xml content
+
+        Args:
+            args:
+            kwargs:
+
+        Returns:
+
+        """
+        content = self.request.POST["content"].strip()
+        template_id = self.request.POST["template_id"]
+
+        if "core_curate_app" not in conf_settings.INSTALLED_APPS:
+            raise exceptions.CoreError(
+                "The Curate App needs to be installed to use this feature."
+            )
+
+        if content:
+            raise exceptions.XMLError(
+                "Please clear form before generating a new XML document."
+            )
+
+        from core_main_app.utils.parser import get_parser
+        from core_parser_app.components.data_structure_element import (
+            api as data_structure_element_api,
+        )
+        from core_curate_app.components.curate_data_structure.models import (
+            CurateDataStructure,
+        )
+        from core_curate_app.components.curate_data_structure import (
+            api as curate_data_structure_api,
+        )
+        from core_curate_app.views.user import views as curate_views
+
+        # Get template
+        template = template_api.get_by_id(template_id, self.request)
+        # Create temp data structure
+        curate_data_structure = CurateDataStructure(
+            user=str(self.request.user.id),
+            template=template,
+            name="text_editor_tmp_" + str(datetime.now()),
+        )
+        # create new curate data structure
+        curate_data_structure_api.upsert(
+            curate_data_structure, self.request.user
+        )
+        # build parser
+        parser = get_parser(request=self.request)
+        # generate form
+        root_element_id = parser.generate_form(
+            xsd_doc_data=template.content,
+            xml_doc_data=None,
+            data_structure=curate_data_structure,
+            request=self.request,
+        )
+        # get the root element
+        root_element = data_structure_element_api.get_by_id(
+            root_element_id, self.request
+        )
+
+        # generate xml string
+        xml_data = curate_views.render_xml(self.request, root_element)
+
+        # prettify content
+        xml_data = main_xml_utils.format_content_xml(xml_data)
+
+        # delete temp data structure
+        curate_data_structure_api.delete(
+            curate_data_structure, self.request.user
+        )
+
+        return HttpResponse(
+            json.dumps(xml_data),
+            "application/javascript",
+        )
+
     def _get_assets(self):
         """get assets
 
         Return:
         """
         # get assets
         assets = super()._get_assets()
```

### Comparing `core_main_app-2.2.1/core_main_app/views/user/ajax.py` & `core_main_app-2.3.0/core_main_app/views/user/ajax.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         if len(users_with_no_access) > 0:
             users_with_no_access.remove(
                 user_api.get_user_by_id(workspace.owner)
             )
 
         if len(users_with_no_access) == 0:
             return HttpResponseBadRequest(
-                "There is no users that can be added."
+                "There are no users that can be added."
             )
 
         form = UserRightForm(users_with_no_access)
     except AccessControlError as ace:
         return HttpResponseBadRequest(escape(str(ace)))
     except DoesNotExist as dne:
         return HttpResponseBadRequest(escape(str(dne)))
@@ -394,15 +394,15 @@
                 [
                     group_api.get_anonymous_group(),
                     group_api.get_default_group(),
                 ],
             )
         if len(groups_with_no_access) == 0:
             return HttpResponseBadRequest(
-                "There is no groups that can be added."
+                "There are no groups that can be added."
             )
 
         form = GroupRightForm(groups_with_no_access)
     except AccessControlError as ace:
         return HttpResponseBadRequest(escape(str(ace)))
     except DoesNotExist as dne:
         return HttpResponseBadRequest(escape(str(dne)))
```

### Comparing `core_main_app-2.2.1/core_main_app/views/user/forms.py` & `core_main_app-2.3.0/core_main_app/views/user/forms.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,19 @@
 
 class GroupRightForm(forms.Form):
     """
     Form to select group to add rights.
     """
 
     groups = forms.MultipleChoiceField(
-        label="", required=True, widget=forms.SelectMultiple()
+        label="",
+        required=True,
+        widget=forms.CheckboxSelectMultiple(
+            attrs={"class": "multiple-columns"}
+        ),
     )
     GROUPS_OPTIONS = []
 
     def __init__(self, groups_with_no_access):
         self.GROUPS_OPTIONS = []
 
         # We sort by name, case sensitive
@@ -48,15 +52,19 @@
 
 class UserRightForm(forms.Form):
     """
     Form to select user to add rights.
     """
 
     users = forms.MultipleChoiceField(
-        label="", required=True, widget=forms.SelectMultiple()
+        label="",
+        required=True,
+        widget=forms.CheckboxSelectMultiple(
+            attrs={"class": "multiple-columns"}
+        ),
     )
     USERS_OPTIONS = []
 
     def __init__(self, users_with_no_access):
         self.USERS_OPTIONS = []
 
         # We sort by username, case sensitive
```

### Comparing `core_main_app-2.2.1/core_main_app/views/user/views.py` & `core_main_app-2.3.0/core_main_app/views/user/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from django.contrib.auth.decorators import login_required
 from django.contrib.auth.forms import PasswordResetForm, SetPasswordForm
 from django.contrib.auth.tokens import default_token_generator
 from django.contrib.staticfiles import finders
 from django.http.response import HttpResponse, HttpResponseRedirect
 from django.shortcuts import redirect, resolve_url
 from django.urls import reverse
-from django.urls import reverse_lazy
 from django.utils.encoding import force_text
 from django.utils.http import urlsafe_base64_decode
 from rest_framework.status import HTTP_405_METHOD_NOT_ALLOWED
 
 from core_main_app.components.template_version_manager import (
     api as template_version_manager_api,
 )
@@ -200,15 +199,15 @@
         assets["js"] = [
             {"path": "core_main_app/js/homepage.js", "is_raw": False}
         ]
 
     return render(request, "core_main_app/user/homepage.html", assets=assets)
 
 
-@login_required(login_url=reverse_lazy("core_main_app_login"))
+@login_required
 def manage_template_versions(request, version_manager_id):
     """View that allows template versions management
 
     Args:
         request:
         version_manager_id:
```

### Comparing `core_main_app-2.2.1/core_main_app.egg-info/PKG-INFO` & `core_main_app-2.3.0/core_main_app.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core-main-app
-Version: 2.2.1
+Version: 2.3.0
 Summary: Main functionalities for the curator core project
 Home-page: https://github.com/usnistgov/core_main_app
 Author: NIST IT Lab
 Author-email: itl_inquiries@nist.gov
 License: UNKNOWN
 Description: =============
         Core Main App
@@ -147,14 +147,39 @@
         
         .. code:: py
         
           EMAIL_USE_TLS = True
           EMAIL_HOST_USER = 'testsite_app'
           EMAIL_HOST_PASSWORD = 'mys3cr3tp4ssw0rd'
         
+        Enable History
+        --------------
+        
+        Django Simple History allows keeping track of changes made to an object stored in the CDCS database.
+        First, install and configure the package. See the
+        `django-simple-history <https://django-simple-history.readthedocs.io/en/latest/quick_start.html>`_ documentation.
+        
+        Then, set the `DJANGO_SIMPLE_HISTORY_MODELS` setting with a list of models to track.
+        At the moment, this feature is only available for the `Data` model.
+        
+        .. code:: python
+        
+          DJANGO_SIMPLE_HISTORY_MODELS=["Data"]
+        
+        Register models to track by updating project files.
+        For example in ``mdcs/mdcs_home/admin.py``, add the following lines:
+        
+        .. code:: python
+        
+          from core_main_app.utils.admin_site.model_admin_class import register_simple_history_models
+          from django.conf import settings
+        
+          DJANGO_SIMPLE_HISTORY_MODELS = getattr(settings, "DJANGO_SIMPLE_HISTORY_MODELS", None)
+          register_simple_history_models(DJANGO_SIMPLE_HISTORY_MODELS)
+        
         Documentation
         =============
         
         Documentation has been generated using Sphinx. To generate a local version of
         the docs, please clone the repository and run:
         
         .. code:: bash
```

### Comparing `core_main_app-2.2.1/core_main_app.egg-info/SOURCES.txt` & `core_main_app-2.3.0/core_main_app.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -152,20 +152,23 @@
 core_main_app/static/core_main_app/admin/js/templates/upload/dependencies.js
 core_main_app/static/core_main_app/admin/js/templates/upload/dependencies.raw.js
 core_main_app/static/core_main_app/admin/js/templates/upload/dependency_resolver.js
 core_main_app/static/core_main_app/admin/js/templates_xslt/detail_xslt.js
 core_main_app/static/core_main_app/common/css/XMLTree.css
 core_main_app/static/core_main_app/common/css/buttons.css
 core_main_app/static/core_main_app/common/css/fields.css
+core_main_app/static/core_main_app/common/css/highlight.css
 core_main_app/static/core_main_app/common/css/loading-spinner.css
+core_main_app/static/core_main_app/common/css/select.css
 core_main_app/static/core_main_app/common/css/share_link.css
 core_main_app/static/core_main_app/common/css/switch.css
 core_main_app/static/core_main_app/common/css/table.css
 core_main_app/static/core_main_app/common/css/word-wrap.css
 core_main_app/static/core_main_app/common/css/template/template_ordering.css
+core_main_app/static/core_main_app/common/css/workspace/table.css
 core_main_app/static/core_main_app/common/img/collapse.png
 core_main_app/static/core_main_app/common/img/expand.png
 core_main_app/static/core_main_app/common/js/XMLTree.js
 core_main_app/static/core_main_app/common/js/backtoprevious.js
 core_main_app/static/core_main_app/common/js/csrf.js
 core_main_app/static/core_main_app/common/js/data_detail.js
 core_main_app/static/core_main_app/common/js/debounce.js
@@ -193,56 +196,25 @@
 core_main_app/static/core_main_app/common/js/templates/versions/modals/disable.raw.js
 core_main_app/static/core_main_app/common/js/xslt/list/modals/delete.js
 core_main_app/static/core_main_app/common/js/xslt/list/modals/delete.raw.js
 core_main_app/static/core_main_app/common/js/xslt/list/modals/edit.js
 core_main_app/static/core_main_app/common/js/xslt/list/modals/edit.raw.js
 core_main_app/static/core_main_app/common/xsl/xml2html.xsl
 core_main_app/static/core_main_app/libs/notify.js
-core_main_app/static/core_main_app/libs/bootstrap/4.5.2/css/bootstrap.min.css
-core_main_app/static/core_main_app/libs/bootstrap/4.5.2/js/bootstrap.min.js
-core_main_app/static/core_main_app/libs/datatables/1.10.13/css/jquery.dataTables.css
-core_main_app/static/core_main_app/libs/datatables/1.10.13/images/sort_asc.png
-core_main_app/static/core_main_app/libs/datatables/1.10.13/images/sort_asc_disabled.png
-core_main_app/static/core_main_app/libs/datatables/1.10.13/images/sort_both.png
-core_main_app/static/core_main_app/libs/datatables/1.10.13/images/sort_desc.png
-core_main_app/static/core_main_app/libs/datatables/1.10.13/images/sort_desc_disabled.png
-core_main_app/static/core_main_app/libs/datatables/1.10.13/js/jquery.dataTables.js
-core_main_app/static/core_main_app/libs/fSelect/css/fSelect.css
-core_main_app/static/core_main_app/libs/fSelect/js/fSelect.js
-core_main_app/static/core_main_app/libs/font-awesome/5.13.0/css/all.min.css
-core_main_app/static/core_main_app/libs/font-awesome/5.13.0/webfonts/fa-brands-400.eot
-core_main_app/static/core_main_app/libs/font-awesome/5.13.0/webfonts/fa-brands-400.svg
-core_main_app/static/core_main_app/libs/font-awesome/5.13.0/webfonts/fa-brands-400.ttf
-core_main_app/static/core_main_app/libs/font-awesome/5.13.0/webfonts/fa-brands-400.woff
-core_main_app/static/core_main_app/libs/font-awesome/5.13.0/webfonts/fa-brands-400.woff2
-core_main_app/static/core_main_app/libs/font-awesome/5.13.0/webfonts/fa-regular-400.eot
-core_main_app/static/core_main_app/libs/font-awesome/5.13.0/webfonts/fa-regular-400.svg
-core_main_app/static/core_main_app/libs/font-awesome/5.13.0/webfonts/fa-regular-400.ttf
-core_main_app/static/core_main_app/libs/font-awesome/5.13.0/webfonts/fa-regular-400.woff
-core_main_app/static/core_main_app/libs/font-awesome/5.13.0/webfonts/fa-regular-400.woff2
-core_main_app/static/core_main_app/libs/font-awesome/5.13.0/webfonts/fa-solid-900.eot
-core_main_app/static/core_main_app/libs/font-awesome/5.13.0/webfonts/fa-solid-900.svg
-core_main_app/static/core_main_app/libs/font-awesome/5.13.0/webfonts/fa-solid-900.ttf
-core_main_app/static/core_main_app/libs/font-awesome/5.13.0/webfonts/fa-solid-900.woff
-core_main_app/static/core_main_app/libs/font-awesome/5.13.0/webfonts/fa-solid-900.woff2
-core_main_app/static/core_main_app/libs/highlight/11.0.0/css/atom-one-light.css
-core_main_app/static/core_main_app/libs/highlight/11.0.0/js/highlight.min.js
-core_main_app/static/core_main_app/libs/highlight/11.0.0/js/init_highlight.js
 core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.css
 core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.js
 core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.structure.css
 core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/jquery-ui.theme.css
 core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_444444_256x240.png
 core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_555555_256x240.png
 core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_777620_256x240.png
 core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_777777_256x240.png
 core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_cc0000_256x240.png
 core_main_app/static/core_main_app/libs/jquery-ui/1.12.1/images/ui-icons_ffffff_256x240.png
 core_main_app/static/core_main_app/libs/jquery/3.5.1/jquery.js
-core_main_app/static/core_main_app/libs/popper-js/popper.min.js
 core_main_app/static/core_main_app/user/css/login.css
 core_main_app/static/core_main_app/user/css/registration.css
 core_main_app/static/core_main_app/user/css/text-editor.css
 core_main_app/static/core_main_app/user/js/sharing_modal.js
 core_main_app/static/core_main_app/user/js/data/change_display.js
 core_main_app/static/core_main_app/user/js/data/change_display.raw.js
 core_main_app/static/core_main_app/user/js/data/detail.js
@@ -255,15 +227,14 @@
 core_main_app/static/core_main_app/user/js/workspaces/add_group.raw.js
 core_main_app/static/core_main_app/user/js/workspaces/add_user.js
 core_main_app/static/core_main_app/user/js/workspaces/add_user.raw.js
 core_main_app/static/core_main_app/user/js/workspaces/create_workspace.js
 core_main_app/static/core_main_app/user/js/workspaces/create_workspace.raw.js
 core_main_app/static/core_main_app/user/js/workspaces/init.js
 core_main_app/static/core_main_app/user/js/workspaces/init.raw.js
-core_main_app/static/core_main_app/user/js/workspaces/tables.js
 core_main_app/static/core_main_app/user/js/workspaces/list/modals/assign_blob_workspace.raw.js
 core_main_app/static/core_main_app/user/js/workspaces/list/modals/assign_data_workspace.raw.js
 core_main_app/static/core_main_app/user/js/workspaces/list/modals/assign_workspace.js
 core_main_app/static/core_main_app/user/js/workspaces/list/modals/remove_rights.js
 core_main_app/static/core_main_app/user/js/workspaces/list/modals/remove_rights.raw.js
 core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_private.js
 core_main_app/static/core_main_app/user/js/workspaces/list/modals/set_private.raw.js
@@ -405,18 +376,20 @@
 core_main_app/utils/datetime.py
 core_main_app/utils/decorators.py
 core_main_app/utils/file.py
 core_main_app/utils/group.py
 core_main_app/utils/labels.py
 core_main_app/utils/markdown_parser.py
 core_main_app/utils/migrations.py
+core_main_app/utils/parser.py
 core_main_app/utils/rendering.py
 core_main_app/utils/urls.py
 core_main_app/utils/xml.py
 core_main_app/utils/admin_site/__init__.py
+core_main_app/utils/admin_site/model_admin_class.py
 core_main_app/utils/admin_site/view_only_admin.py
 core_main_app/utils/databases/__init__.py
 core_main_app/utils/databases/backend.py
 core_main_app/utils/databases/mongo/__init__.py
 core_main_app/utils/databases/mongo/mongoengine_database.py
 core_main_app/utils/databases/mongo/pymongo_database.py
 core_main_app/utils/integration_tests/__init__.py
@@ -594,17 +567,21 @@
 tests/rest/xsl_transformation/fixtures/__init__.py
 tests/rest/xsl_transformation/fixtures/fixtures.py
 tests/system/__init__.py
 tests/system/test_unit.py
 tests/templatetags/__init__.py
 tests/templatetags/test_get_attribute.py
 tests/utils/__init__.py
+tests/utils/test_unit_apps.py
+tests/utils/test_unit_urls.py
 tests/utils/tests_int_blob_downloader.py
 tests/utils/tests_int_file.py
+tests/utils/tests_unit_admin_site.py
 tests/utils/tests_unit_boolean.py
+tests/utils/tests_unit_parser.py
 tests/utils/tests_unit_xml_operation.py
 tests/utils/tests_view_data.py
 tests/utils/checksum/__init__.py
 tests/utils/checksum/tests_checksum.py
 tests/utils/migrations/__init__.py
 tests/utils/migrations/tests_unit.py
 tests/utils/query/__init__.py
@@ -614,8 +591,9 @@
 tests/utils/requests_utls/tests_ssl.py
 tests/utils/validation/__init__.py
 tests/utils/validation/tests_unit_validation.py
 tests/utils/xsd_flattener/__init__.py
 tests/utils/xsd_flattener/tests_unit.py
 tests/views/__init__.py
 tests/views/fixtures.py
+tests/views/test_unit.py
 tests/views/tests_int_access_control.py
```

### Comparing `core_main_app-2.2.1/docs/conf.py` & `core_main_app-2.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/setup.py` & `core_main_app-2.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     long_desc = f.read()
 
 # Allow setup.py to be run from any path
 chdir(normpath(join(abspath(__file__), pardir)))
 
 setup(
     name="core_main_app",
-    version="2.2.1",
+    version="2.3.0",
     description="Main functionalities for the curator core project",
     long_description=long_desc,
     author="NIST IT Lab",
     author_email="itl_inquiries@nist.gov",
     url="https://github.com/usnistgov/core_main_app",
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `core_main_app-2.2.1/tests/access_control/tests_access_control.py` & `core_main_app-2.3.0/tests/access_control/tests_access_control.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/commons/tests_validators.py` & `core_main_app-2.3.0/tests/commons/tests_validators.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/components/blob/fixtures/fixtures.py` & `core_main_app-2.3.0/tests/components/blob/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/components/blob/tests_int.py` & `core_main_app-2.3.0/tests/components/blob/tests_int.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,24 @@
     BlobFixtures,
     AccessControlBlobFixture,
 )
 
 from core_main_app.commons import exceptions
 from core_main_app.components.blob.models import Blob
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.components.blob import api as blob_api
 
 fixture_blob = BlobFixtures()
 fixture_blob_workspace = AccessControlBlobFixture()
 
 
-class TestBlobGetAll(MongoIntegrationBaseTestCase):
+class TestBlobGetAll(IntegrationBaseTestCase):
     """TestBlobGetAll"""
 
     fixture = fixture_blob
 
     def test_blob_get_all_return_collection_of_blob(self):
         """test_blob_get_all_return_collection_of_blob
 
@@ -43,15 +43,15 @@
         """
         # Act
         result = Blob.get_all()
         # Assert
         self.assertTrue(len(self.fixture.blob_collection) == result.count())
 
 
-class TestBlobGetById(MongoIntegrationBaseTestCase):
+class TestBlobGetById(IntegrationBaseTestCase):
     """TestBlobGetById"""
 
     fixture = fixture_blob
 
     def test_blob_get_by_id_raises_does_not_exist_error_if_not_found(self):
         """test_blob_get_by_id_raises_does_not_exist_error_if_not_found
 
@@ -70,15 +70,15 @@
         """
         # Act
         result = Blob.get_by_id(self.fixture.blob_1.id)
         # Assert
         self.assertEqual(result, self.fixture.blob_1)
 
 
-class TestBlobGetAllByUserId(MongoIntegrationBaseTestCase):
+class TestBlobGetAllByUserId(IntegrationBaseTestCase):
     """TestBlobGetAllByUserId"""
 
     fixture = fixture_blob
 
     def test_blob_get_all_by_user_id_return_collection_of_blob_from_user(self):
         """test_blob_get_all_by_user_id_return_collection_of_blob_from_user
 
@@ -104,15 +104,15 @@
         user_id = 800
         # Act
         result = Blob.get_all_by_user_id(user_id)
         # Assert
         self.assertTrue(result.count() == 0)
 
 
-class TestBlobGetAllByWorkspace(MongoIntegrationBaseTestCase):
+class TestBlobGetAllByWorkspace(IntegrationBaseTestCase):
     """TestBlobGetAllByWorkspace"""
 
     fixture = fixture_blob_workspace
 
     def test_blob_get_all_by_workspace_return_collection_of_blob_from_user(
         self,
     ):
@@ -141,15 +141,15 @@
         """
         # Act
         result = Blob.get_all_by_workspace(self.fixture.workspace_without_data)
         # Assert
         self.assertTrue(result.count() == 0)
 
 
-class TestBlobGetAllByListWorkspace(MongoIntegrationBaseTestCase):
+class TestBlobGetAllByListWorkspace(IntegrationBaseTestCase):
     """TestBlobGetAllByListWorkspace"""
 
     fixture = fixture_blob_workspace
 
     def test_blob_get_all_by_workspace_return_collection_of_blob_from_user(
         self,
     ):
@@ -183,15 +183,15 @@
         result = Blob.get_all_by_list_workspace(
             [self.fixture.workspace_without_data]
         )
         # Assert
         self.assertTrue(result.count() == 0)
 
 
-class TestBlobInsert(MongoIntegrationBaseTestCase):
+class TestBlobInsert(IntegrationBaseTestCase):
     """TestBlobInsert"""
 
     def setUp(self):
         """setUp
 
         Returns:
```

### Comparing `core_main_app-2.2.1/tests/components/blob/tests_int_access_control.py` & `core_main_app-2.3.0/tests/components/blob/tests_int_access_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 from tests.components.blob.fixtures.fixtures import AccessControlBlobFixture
 
 from core_main_app.access_control.exceptions import AccessControlError
 from core_main_app.commons import exceptions
 from core_main_app.components.blob import api as blob_api
 from core_main_app.components.blob.models import Blob
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 
 fixture_blob = AccessControlBlobFixture()
 
 
-class TestBlobGetById(MongoIntegrationBaseTestCase):
+class TestBlobGetById(IntegrationBaseTestCase):
     """TestBlobGetById"""
 
     fixture = fixture_blob
 
     def test_get_by_id_owner_with_read_access_returns_blob(self):
         """test_get_by_id_owner_with_read_access_returns_blob
 
@@ -81,15 +81,15 @@
             fixture_blob.USER_1_NO_WORKSPACE
         ].id
         mock_user = _create_user("2")
         with self.assertRaises(AccessControlError):
             blob_api.get_by_id(blob_id, mock_user)
 
 
-class TestBlobGetAll(MongoIntegrationBaseTestCase):
+class TestBlobGetAll(IntegrationBaseTestCase):
     """TestBlobGetAll"""
 
     fixture = fixture_blob
 
     def test_get_all_as_superuser_returns_all_blob(self):
         """test_get_all_as_superuser_returns_all_blob
 
@@ -107,15 +107,15 @@
 
         """
         mock_user = _create_user("1")
         with self.assertRaises(AccessControlError):
             blob_api.get_all(mock_user)
 
 
-class TestBlobGetAllByUser(MongoIntegrationBaseTestCase):
+class TestBlobGetAllByUser(IntegrationBaseTestCase):
     """TestBlobGetAllByUser"""
 
     fixture = fixture_blob
 
     def test_get_all_by_user_returns_owned_blob(self):
         """test_get_all_by_user_returns_owned_blob
 
@@ -145,15 +145,15 @@
         """
         mock_user = _create_user("1", is_superuser=True)
         blob_list = blob_api.get_all_by_user(mock_user)
         self.assertTrue(len(blob_list) == 2)
         self.assertTrue(blob.user_id == "1" for blob in blob_list)
 
 
-class TestBlobGetAllByWorkspace(MongoIntegrationBaseTestCase):
+class TestBlobGetAllByWorkspace(IntegrationBaseTestCase):
     """TestBlobGetAllByWorkspace"""
 
     fixture = fixture_blob
 
     @patch(
         "core_main_app.components.workspace.api.get_all_workspaces_with_write_access_by_user"
     )
@@ -241,15 +241,15 @@
         ]
         blob_list = blob_api.get_all_by_workspace(
             self.fixture.workspace_1, mock_user
         )
         self.assertTrue(blob.user_id == mock_user.id for blob in blob_list)
 
 
-class TestBlobDelete(MongoIntegrationBaseTestCase):
+class TestBlobDelete(IntegrationBaseTestCase):
     """TestBlobDelete"""
 
     fixture = fixture_blob
 
     @patch(
         "core_main_app.components.workspace.api.get_all_workspaces_with_write_access_by_user"
     )
@@ -385,15 +385,15 @@
         with self.assertRaises(AccessControlError):
             blob_api.delete(
                 fixture_blob.blob_collection[fixture_blob.USER_2_NO_WORKSPACE],
                 mock_user,
             )
 
 
-class TestBlobChangeOwner(MongoIntegrationBaseTestCase):
+class TestBlobChangeOwner(IntegrationBaseTestCase):
     """TestBlobChangeOwner"""
 
     fixture = fixture_blob
 
     def test_change_owner_from_owner_to_owner_ok(self):
         """test_change_owner_from_owner_to_owner_ok
 
@@ -454,15 +454,15 @@
                 fixture_blob.USER_1_NO_WORKSPACE
             ],
             new_user=mock_user,
             user=mock_user,
         )
 
 
-class TestBlobInsert(MongoIntegrationBaseTestCase):
+class TestBlobInsert(IntegrationBaseTestCase):
     """TestBlobInsert"""
 
     def setUp(self):
         """setUp
 
         Returns:
 
@@ -530,15 +530,15 @@
         with self.assertRaises(exceptions.ApiError):
             blob_api.insert(
                 fixture_blob.blob_collection[fixture_blob.USER_1_NO_WORKSPACE],
                 self.superuser,
             )
 
 
-class TestBlobAssign(MongoIntegrationBaseTestCase):
+class TestBlobAssign(IntegrationBaseTestCase):
     """TestBlobAssign"""
 
     fixture = fixture_blob
 
     def test_assign_blob_as_anonymous_raises_error(self):
         """test_assign_blob_as_anonymous_raises_error
```

### Comparing `core_main_app-2.2.1/tests/components/data/fixtures/fixtures.py` & `core_main_app-2.3.0/tests/components/data/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/components/data/tests_int.py` & `core_main_app-2.3.0/tests/components/data/tests_int.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,33 +11,33 @@
 from core_main_app.components.data.api import check_xml_file_is_valid
 from core_main_app.components.data.models import Data
 from core_main_app.components.template import api as template_api
 from core_main_app.settings import DATA_SORTING_FIELDS
 from core_main_app.system import api as system_api
 from core_main_app.utils.datetime import datetime_now
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.integration_tests.integration_base_transaction_test_case import (
-    MongoIntegrationTransactionTestCase,
+    IntegrationTransactionTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from tests.components.data.fixtures.fixtures import (
     DataFixtures,
     AccessControlDataFixture,
 )
 from tests.components.data.fixtures.fixtures import DataMigrationFixture
 from tests.components.user.fixtures.fixtures import UserFixtures
 
 fixture_data_template = DataMigrationFixture()
 fixture_data = DataFixtures()
 access_control_data_fixture = AccessControlDataFixture()
 
 
-class TestDataGetAll(MongoIntegrationBaseTestCase):
+class TestDataGetAll(IntegrationBaseTestCase):
     """TestDataGetAll"""
 
     fixture = access_control_data_fixture
 
     def test_data_get_all_return_collection_of_data(self):
         """test_data_get_all_return_collection_of_data
 
@@ -160,15 +160,15 @@
         # Assert
         self.assertListEqual(
             [data.title for data in list(queryset)],
             [data.title for data in self.fixture.data_collection],
         )
 
 
-class TestDataGetAllExcept(MongoIntegrationBaseTestCase):
+class TestDataGetAllExcept(IntegrationBaseTestCase):
     """TestDataGetAllExcept"""
 
     fixture = access_control_data_fixture
 
     def test_data_get_all_except_return_collection_of_data(self):
         """test_data_get_all_except_return_collection_of_data
 
@@ -365,15 +365,15 @@
             self.fixture.data_4.user_id, descending_result.all()[3].user_id
         )
         self.assertEqual(
             self.fixture.data_5.user_id, descending_result.all()[4].user_id
         )
 
 
-class TestDataGetById(MongoIntegrationBaseTestCase):
+class TestDataGetById(IntegrationBaseTestCase):
     """TestDataGetById"""
 
     fixture = fixture_data
 
     def test_data_get_by_id_raises_api_error_if_not_found(self):
         """test_data_get_by_id_raises_api_error_if_not_found
 
@@ -392,15 +392,15 @@
         """
         # Act
         result = Data.get_by_id(self.fixture.data_1.id)
         # Assert
         self.assertEqual(result, self.fixture.data_1)
 
 
-class TestDataGetAllByUserId(MongoIntegrationBaseTestCase):
+class TestDataGetAllByUserId(IntegrationBaseTestCase):
     """TestDataGetAllByUserId"""
 
     fixture = access_control_data_fixture
 
     def test_data_get_all_by_user_id_return_collection_of_data_from_user(self):
         """test_data_get_all_by_user_id_return_collection_of_data_from_user
 
@@ -543,15 +543,15 @@
         # Assert
         self.assertListEqual(
             list(data),
             [self.fixture.data_1, self.fixture.data_3, self.fixture.data_5],
         )
 
 
-class TestDataGetAllExceptUserId(MongoIntegrationBaseTestCase):
+class TestDataGetAllExceptUserId(IntegrationBaseTestCase):
     """TestDataGetAllExceptUserId"""
 
     fixture = access_control_data_fixture
 
     def test_data_get_all_except_user_id_return_collection_of_data_where_user_is_not_owner(
         self,
     ):
@@ -695,15 +695,15 @@
         data = data_api.get_all_except_user(mock_user)
         # Assert
         self.assertListEqual(
             list(data), [self.fixture.data_2, self.fixture.data_4]
         )
 
 
-class TestExecuteQuery(MongoIntegrationTransactionTestCase):
+class TestExecuteQuery(IntegrationTransactionTestCase):
     """TestExecuteQuery"""
 
     fixture = access_control_data_fixture
 
     def test_execute_query_data_ordering(self):
         """test_execute_query_data_ordering
 
@@ -815,15 +815,15 @@
         # Assert
         self.assertListEqual(
             [data.title for data in list(queryset)],
             [data.title for data in self.fixture.data_collection],
         )
 
 
-class TestGetAllByWorkspace(MongoIntegrationBaseTestCase):
+class TestGetAllByWorkspace(IntegrationBaseTestCase):
     """TestGetAllByWorkspace"""
 
     fixture = access_control_data_fixture
 
     def test_get_all_by_workspace_data_ordering(self):
         """test_get_all_by_workspace_data_ordering
 
@@ -939,15 +939,15 @@
         data = data_api.get_all_by_workspace(workspace, mock_user)
         # Assert
         self.assertListEqual(
             list(data), [self.fixture.data_3, self.fixture.data_5]
         )
 
 
-class TestGetByIdList(MongoIntegrationBaseTestCase):
+class TestGetByIdList(IntegrationBaseTestCase):
     """TestGetByIdList"""
 
     fixture = access_control_data_fixture
 
     def setUp(self):
         """setUp
 
@@ -1014,15 +1014,15 @@
         Returns:
 
         """
         result = data_api.get_by_id_list([-1], self.user)
         self.assertEqual(len(result), 0)
 
 
-class TestDataMigration(MongoIntegrationTransactionTestCase):
+class TestDataMigration(IntegrationTransactionTestCase):
     """TestDataMigration"""
 
     fixture = fixture_data_template
 
     def setUp(self):
         """Insert needed data.
```

### Comparing `core_main_app-2.2.1/tests/components/data/tests_int_access_control.py` & `core_main_app-2.3.0/tests/components/data/tests_int_access_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,27 +14,27 @@
 )
 
 from core_main_app.access_control.exceptions import AccessControlError
 from core_main_app.commons.exceptions import QueryError
 from core_main_app.components.data import api as data_api
 from core_main_app.components.data.models import Data
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import create_mock_request
 
 fixture_data = AccessControlDataFixture()
 fixture_data2 = AccessControlDataFixture2()
 fixture_data_full_text = AccessControlDataFullTextSearchFixture()
 fixture_data_numeric = AccessControlDataNumericFixture()
 fixture_data_none = AccessControlDataNoneFixture()
 
 
-class TestDataGetById(MongoIntegrationBaseTestCase):
+class TestDataGetById(IntegrationBaseTestCase):
     """TestDataGetById"""
 
     fixture = fixture_data
 
     @patch(
         "core_main_app.components.workspace.api.get_all_workspaces_with_read_access_by_user"
     )
@@ -126,15 +126,15 @@
             fixture_data.USER_1_NO_WORKSPACE
         ].id
         mock_user = create_mock_user(2)
         with self.assertRaises(AccessControlError):
             data_api.get_by_id(data_id, mock_user)
 
 
-class TestDataGetByIdList(MongoIntegrationBaseTestCase):
+class TestDataGetByIdList(IntegrationBaseTestCase):
     """TestDataGetByIdList"""
 
     fixture = fixture_data
 
     @patch(
         "core_main_app.components.workspace.api.get_all_workspaces_with_read_access_by_user"
     )
@@ -289,15 +289,15 @@
             fixture_data.USER_1_NO_WORKSPACE
         ].id
         mock_user = create_mock_user(None, is_anonymous=True)
         with self.assertRaises(AccessControlError):
             data_api.get_by_id_list([data_id], mock_user)
 
 
-class TestDataGetAll(MongoIntegrationBaseTestCase):
+class TestDataGetAll(IntegrationBaseTestCase):
     """TestDataGetAll"""
 
     fixture = fixture_data
 
     def test_get_all_as_superuser_returns_all_data(self):
         """test get all as superuser returns all data
 
@@ -315,15 +315,15 @@
 
         """
         mock_user = create_mock_user(1)
         with self.assertRaises(AccessControlError):
             data_api.get_all(mock_user)
 
 
-class TestDataGetAllByUser(MongoIntegrationBaseTestCase):
+class TestDataGetAllByUser(IntegrationBaseTestCase):
     """TestDataGetAllByUser"""
 
     fixture = fixture_data
 
     @patch(
         "core_main_app.components.workspace.api.get_all_workspaces_with_read_access_by_user"
     )
@@ -390,15 +390,15 @@
         """
         mock_user = create_mock_user(1, is_superuser=True)
         data_list = data_api.get_all_by_user(mock_user)
         self.assertTrue(len(data_list) == 3)
         self.assertTrue(data.user_id == "1" for data in data_list)
 
 
-class TestDataGetAllExceptUser(MongoIntegrationBaseTestCase):
+class TestDataGetAllExceptUser(IntegrationBaseTestCase):
     """TestDataGetAllExceptUser"""
 
     # NOTE: Will always fail when private data are present
     # (data.workspace=None, data.user_id!=user.id)
     fixture = fixture_data
 
     @patch(
@@ -450,15 +450,15 @@
         """
         mock_user = create_mock_user(1, is_superuser=True)
         data_list = data_api.get_all_except_user(mock_user)
         self.assertTrue(len(data_list) > 0)
         self.assertTrue(data.user_id != mock_user.id for data in data_list)
 
 
-class TestDataUpsert(MongoIntegrationBaseTestCase):
+class TestDataUpsert(IntegrationBaseTestCase):
     """TestDataUpsert"""
 
     fixture = fixture_data
 
     def test_upsert_data_as_anonymous_raises_error(self):
         """test upsert data as anonymous raises error
 
@@ -622,15 +622,15 @@
         """
         user = create_mock_user(user_id=1)
         mock_request = create_mock_request(user)
         fixture_data.data_1.xml_content = '<tag  xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" ></tag>'
         data_api.upsert(fixture_data.data_1, mock_request)
 
 
-class TestDataExecuteQuery(MongoIntegrationBaseTestCase):
+class TestDataExecuteQuery(IntegrationBaseTestCase):
     """TestDataExecuteQuery"""
 
     fixture = fixture_data
 
     @patch(
         "core_main_app.components.workspace.api.get_all_workspaces_with_read_access_by_user"
     )
@@ -944,15 +944,15 @@
         get_all_workspaces_with_read_access_by_user.return_value = []
         with self.assertRaises(AccessControlError):
             data_api.execute_json_query(
                 {"$and": [{"workspace": 1}, {"user_id": 3}]}, mock_user
             )
 
 
-class TestDataExecuteRawQuery(MongoIntegrationBaseTestCase):
+class TestDataExecuteRawQuery(IntegrationBaseTestCase):
     """TestDataExecuteRawQuery"""
 
     fixture = fixture_data2
 
     @patch(
         "core_main_app.components.workspace.api.get_all_workspaces_with_read_access_by_user"
     )
@@ -1863,15 +1863,15 @@
                         {"$or": [{"root.element": {"$where": ["1", "2"]}}]}
                     ]
                 },
                 mock_user,
             )
 
 
-class TestDataExecuteNoneQuery(MongoIntegrationBaseTestCase):
+class TestDataExecuteNoneQuery(IntegrationBaseTestCase):
     """TestDataExecuteNoneQuery"""
 
     fixture = fixture_data_none
 
     @patch(
         "core_main_app.components.workspace.api.get_all_workspaces_with_read_access_by_user"
     )
@@ -1909,15 +1909,15 @@
         mock_user = create_mock_user(2)
         get_all_workspaces_with_read_access_by_user.return_value = []
         query = {"dict_content.root.element": None}
         data_list = data_api.execute_json_query(query, mock_user)
         self.assertEqual(data_list.count(), 0)
 
 
-class TestDataExecuteFullTextQuery(MongoIntegrationBaseTestCase):
+class TestDataExecuteFullTextQuery(IntegrationBaseTestCase):
     """TestDataExecuteFullTextQuery"""
 
     fixture = fixture_data_full_text
 
     @patch(
         "core_main_app.components.workspace.api.get_all_workspaces_with_read_access_by_user"
     )
@@ -2083,15 +2083,15 @@
         mock_user = create_mock_user("1")
         get_all_workspaces_with_read_access_by_user.return_value = []
         query = {"$text": {"$search": 1}}
         with self.assertRaises(QueryError):
             data_api.execute_json_query(query, mock_user)
 
 
-class TestDataDelete(MongoIntegrationBaseTestCase):
+class TestDataDelete(IntegrationBaseTestCase):
     """TestDataDelete"""
 
     fixture = fixture_data
 
     @patch(
         "core_main_app.components.workspace.api.get_all_workspaces_with_write_access_by_user"
     )
@@ -2228,15 +2228,15 @@
         with self.assertRaises(AccessControlError):
             data_api.delete(
                 fixture_data.data_collection[fixture_data.USER_2_NO_WORKSPACE],
                 mock_user,
             )
 
 
-class TestDataChangeOwner(MongoIntegrationBaseTestCase):
+class TestDataChangeOwner(IntegrationBaseTestCase):
     """TestDataChangeOwner"""
 
     fixture = fixture_data
 
     def test_change_owner_from_owner_to_owner_ok(self):
         """test change owner from owner to owner ok
 
@@ -2297,15 +2297,15 @@
                 fixture_data.USER_1_NO_WORKSPACE
             ],
             new_user=mock_user,
             user=mock_user,
         )
 
 
-class TestDataExecuteNumericQuery(MongoIntegrationBaseTestCase):
+class TestDataExecuteNumericQuery(IntegrationBaseTestCase):
     """TestDataExecuteNumericQuery"""
 
     fixture = fixture_data_numeric
 
     def test_exact_matches_returns_data(
         self,
     ):
```

### Comparing `core_main_app-2.2.1/tests/components/data/tests_int_ordering.py` & `core_main_app-2.3.0/tests/components/data/tests_int_ordering.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """ Integration test for data ordering
 """
 from tests.components.data.fixtures.fixtures import AccessControlDataFixture
 
 from core_main_app.components.data.models import Data
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 
 # FIXME move other tests (from tests_int.py) here
 ordering_data_fixture = AccessControlDataFixture()
 
 
-class TestGetAllByListTemplate(MongoIntegrationBaseTestCase):
+class TestGetAllByListTemplate(IntegrationBaseTestCase):
     """TestGetAllByListTemplate"""
 
     fixture = ordering_data_fixture
 
     def test_get_all_by_list_template_data_ordering(self):
         """test_get_all_by_list_template_data_ordering
```

### Comparing `core_main_app-2.2.1/tests/components/data/tests_unit.py` & `core_main_app-2.3.0/tests/components/data/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/components/group/fixtures/fixtures.py` & `core_main_app-2.3.0/tests/components/group/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/components/group/fixtures/tests_int.py` & `core_main_app-2.3.0/tests/components/group/fixtures/tests_int.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """ Integration Test for Group Fixtures
 """
 
 from tests.components.group.fixtures.fixtures import GroupFixtures
 
 from core_main_app.components.group import api as group_api
 from core_main_app.utils.integration_tests.integration_base_transaction_test_case import (
-    MongoIntegrationTransactionTestCase,
+    IntegrationTransactionTestCase,
 )
 
 
-class TestGroupFixtures(MongoIntegrationTransactionTestCase):
+class TestGroupFixtures(IntegrationTransactionTestCase):
     """Test Group fixtures"""
 
     def test_create_group(self):
         """test create group
 
         Returns:
```

### Comparing `core_main_app-2.2.1/tests/components/group/tests_int.py` & `core_main_app-2.3.0/tests/components/group/tests_int.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """ Integration Test for Group
 """
 
 from tests.components.group.fixtures.fixtures import GroupFixtures
 from django.contrib.auth.models import Group
 from core_main_app.components.group import api as group_api
 from core_main_app.utils.integration_tests.integration_base_transaction_test_case import (
-    MongoIntegrationTransactionTestCase,
+    IntegrationTransactionTestCase,
 )
 
 
-class TestGetAllGroups(MongoIntegrationTransactionTestCase):
+class TestGetAllGroups(IntegrationTransactionTestCase):
     """Test Get All Groups"""
 
     def test_get_all_groups_returns_default_groups(self):
         """test_get_all_groups_returns_default_groups
 
         Returns:
 
@@ -37,15 +37,15 @@
         list_groups = group_api.get_all_groups()
 
         # Assert
         self.assertEqual(len(list_groups), 3)
         self.assertTrue(all(isinstance(group, Group) for group in list_groups))
 
 
-class TestGetGroupByNameAndPermission(MongoIntegrationTransactionTestCase):
+class TestGetGroupByNameAndPermission(IntegrationTransactionTestCase):
     """Test Get Group By Name And Permission"""
 
     def test_get_group_by_name_and_permission_returns_group_list(self):
         """test get group by name and permission returns group list
 
         Returns:
 
@@ -88,15 +88,15 @@
         # Act
         result = group_api.get_by_name_and_permission(group.name, "Wrong")
 
         # Assert
         self.assertEqual(len(result), 0)
 
 
-class TestGetAllGroupByListId(MongoIntegrationTransactionTestCase):
+class TestGetAllGroupByListId(IntegrationTransactionTestCase):
     """Test Get All Group By List Id"""
 
     def test_get_all_groups_by_list_id_returns_list(self):
         """test get all groups by list id returns list
 
         Returns:
 
@@ -128,15 +128,15 @@
         # Act
         result = group_api.get_all_groups_by_list_id([1, -1])
 
         # Assert
         self.assertEqual(len(result), 1)
 
 
-class TestGetAllGroupExceptListId(MongoIntegrationTransactionTestCase):
+class TestGetAllGroupExceptListId(IntegrationTransactionTestCase):
     """Test Get All Group Except List Id"""
 
     def test_get_all_groups_except_list_id_returns_list(self):
         """test get all groups except list id returns list
 
         Returns:
 
@@ -161,15 +161,15 @@
         # Act
         result = group_api.get_all_groups_except_list_id([1, 2])
 
         # Assert
         self.assertEqual(len(result), 0)
 
 
-class TestGetAllGroupExceptList(MongoIntegrationTransactionTestCase):
+class TestGetAllGroupExceptList(IntegrationTransactionTestCase):
     """Test Get All Group Except List"""
 
     def test_get_all_groups_except_list_returns_list(self):
         """test get all groups except list returns list
 
         Returns:
```

### Comparing `core_main_app-2.2.1/tests/components/lock/tests_int.py` & `core_main_app-2.3.0/tests/components/lock/tests_int.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 """
 
 from core_main_app.commons.exceptions import LockError
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 
 from tests.components.data.fixtures.fixtures import DataFixtures
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.components.lock import api as lock_api
 
 
 fixture_data = DataFixtures()
 
 
-class TestLockIsObjectLocked(MongoIntegrationBaseTestCase):
+class TestLockIsObjectLocked(IntegrationBaseTestCase):
     """Test Lock Is Object Locked"""
 
     fixture = fixture_data
     user1 = create_mock_user("1")
     user2 = create_mock_user("2")
 
     def test_is_object_locked_returns_true_when_locked(self):
@@ -46,15 +46,15 @@
         # Act
         result = lock_api.is_object_locked(self.fixture.data_1, self.user1)
 
         # Assert
         self.assertEqual(result, False)
 
 
-class TestLockSetLock(MongoIntegrationBaseTestCase):
+class TestLockSetLock(IntegrationBaseTestCase):
     """Test Set Lock"""
 
     fixture = fixture_data
     user1 = create_mock_user("1")
     user2 = create_mock_user("2")
 
     def test_set_lock_locks_object_when_object_is_unlocked(self):
@@ -101,15 +101,15 @@
         lock_api.set_lock_object(self.fixture.data_1, self.user1)
 
         # Act  # Assert
         with self.assertRaises(LockError):
             lock_api.set_lock_object(self.fixture.data_1, self.user2)
 
 
-class TestLockRemoveLockOnObject(MongoIntegrationBaseTestCase):
+class TestLockRemoveLockOnObject(IntegrationBaseTestCase):
     """Test Remove Lock On Object"""
 
     fixture = fixture_data
     user1 = create_mock_user("1")
     user2 = create_mock_user("2")
 
     def test_remove_lock_unlocks_object_when_locked(self):
```

### Comparing `core_main_app-2.2.1/tests/components/lock/tests_unit.py` & `core_main_app-2.3.0/tests/components/lock/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/components/mongo_data/tests_int_access_control.py` & `core_main_app-2.3.0/tests/components/mongo_data/tests_int_access_control.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/components/template/fixtures/fixtures.py` & `core_main_app-2.3.0/tests/components/template/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/components/template/tests_int_access_control.py` & `core_main_app-2.3.0/tests/components/template/tests_int_access_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 from tests.components.template.fixtures.fixtures import (
     AccessControlTemplateFixture,
 )
 
 from core_main_app.access_control.exceptions import AccessControlError
 from core_main_app.components.template import api as template_api
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import create_mock_request
 
 fixture_template = AccessControlTemplateFixture()
 
 
-class TestTemplateUpsert(MongoIntegrationBaseTestCase):
+class TestTemplateUpsert(IntegrationBaseTestCase):
     """TestTemplateUpsert"""
 
     fixture = fixture_template
 
     def setUp(self):
         """setUp
 
@@ -183,15 +183,15 @@
         Returns:
 
         """
         mock_request = create_mock_request(user=self.superuser1)
         template_api.upsert(self.fixture.global_template, request=mock_request)
 
 
-class TestTemplateSetDisplayName(MongoIntegrationBaseTestCase):
+class TestTemplateSetDisplayName(IntegrationBaseTestCase):
     """TestTemplateSetDisplayName"""
 
     fixture = fixture_template
 
     def setUp(self):
         """setUp
 
@@ -367,15 +367,15 @@
         """
         mock_request = create_mock_request(user=self.superuser1)
         template_api.set_display_name(
             self.fixture.global_template, "new_name", request=mock_request
         )
 
 
-class TestTemplateGet(MongoIntegrationBaseTestCase):
+class TestTemplateGet(IntegrationBaseTestCase):
     """TestTemplateGet"""
 
     fixture = fixture_template
 
     def setUp(self):
         """setUp
 
@@ -511,15 +511,15 @@
         mock_request = create_mock_request(user=self.staff_user1)
         with self.assertRaises(AccessControlError):
             template_api.get_by_id(
                 self.fixture.user2_template.id, request=mock_request
             )
 
 
-class TestTemplateGetAllAccessibleByIdList(MongoIntegrationBaseTestCase):
+class TestTemplateGetAllAccessibleByIdList(IntegrationBaseTestCase):
     """TestTemplateGetAllAccessibleByIdList"""
 
     fixture = fixture_template
 
     def setUp(self):
         """setUp
 
@@ -610,15 +610,15 @@
             self.template_id_list, request=mock_request
         )
         self.assertTrue(self.fixture.user1_template in list(templates))
         self.assertTrue(self.fixture.user2_template in list(templates))
         self.assertTrue(self.fixture.global_template in list(templates))
 
 
-class TestTemplateGetAllByHash(MongoIntegrationBaseTestCase):
+class TestTemplateGetAllByHash(IntegrationBaseTestCase):
     """TestTemplateGetAllByHash"""
 
     fixture = fixture_template
 
     def setUp(self):
         """setUp
 
@@ -821,15 +821,15 @@
             self.fixture.user2_template.hash, request=mock_request
         )
         self.assertTrue(self.fixture.user1_template not in list(templates))
         self.assertTrue(self.fixture.user2_template in list(templates))
         self.assertTrue(self.fixture.global_template not in list(templates))
 
 
-class TestTemplateGetAllByHashList(MongoIntegrationBaseTestCase):
+class TestTemplateGetAllByHashList(IntegrationBaseTestCase):
     """TestTemplateGetAllByHashList"""
 
     fixture = fixture_template
 
     def setUp(self):
         """setUp
 
@@ -1040,15 +1040,15 @@
             [self.fixture.user2_template.hash], request=mock_request
         )
         self.assertTrue(self.fixture.user1_template not in list(templates))
         self.assertTrue(self.fixture.user2_template in list(templates))
         self.assertTrue(self.fixture.global_template not in list(templates))
 
 
-class TestTemplateGetAll(MongoIntegrationBaseTestCase):
+class TestTemplateGetAll(IntegrationBaseTestCase):
     """TestTemplateGetAll"""
 
     fixture = fixture_template
 
     def setUp(self):
         """setUp
 
@@ -1124,15 +1124,15 @@
         templates = template_api.get_all(request=mock_request)
         self.assertEqual(templates.count(), 3)
         self.assertTrue(self.fixture.user1_template in list(templates))
         self.assertTrue(self.fixture.user2_template in list(templates))
         self.assertTrue(self.fixture.global_template in list(templates))
 
 
-class TestTemplateDelete(MongoIntegrationBaseTestCase):
+class TestTemplateDelete(IntegrationBaseTestCase):
     """TestTemplateDelete"""
 
     fixture = fixture_template
 
     def setUp(self):
         """setUp
```

### Comparing `core_main_app-2.2.1/tests/components/template/tests_unit.py` & `core_main_app-2.3.0/tests/components/template/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/components/template_version_manager/fixtures/fixtures.py` & `core_main_app-2.3.0/tests/components/template_version_manager/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/components/template_version_manager/tests_int_access_control.py` & `core_main_app-2.3.0/tests/components/template_version_manager/tests_int_access_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from django.test import override_settings
 
 from core_main_app.access_control.exceptions import AccessControlError
 from core_main_app.components.template_version_manager import (
     api as template_vm_api,
 )
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import create_mock_request
 from core_main_app.components.template_version_manager import access_control
 
 from tests.components.template_version_manager.fixtures.fixtures import (
     TemplateVersionManagerAccessControlFixtures,
@@ -20,15 +20,15 @@
 )
 
 
 fixture_template_vm = TemplateVersionManagerAccessControlFixtures()
 fixture_template_vm_ordering = TemplateVersionManagerOrderingFixtures()
 
 
-class TestTemplateVersionManagerGet(MongoIntegrationBaseTestCase):
+class TestTemplateVersionManagerGet(IntegrationBaseTestCase):
     """TestTemplateVersionManagerGet"""
 
     fixture = fixture_template_vm
 
     def setUp(self):
         """setUp
 
@@ -168,15 +168,15 @@
         mock_request = create_mock_request(user=self.staff_user1)
         with self.assertRaises(AccessControlError):
             template_vm_api.get_by_id(
                 self.fixture.user2_tvm.id, request=mock_request
             )
 
 
-class TestTemplateVersionManagerGetByIdList(MongoIntegrationBaseTestCase):
+class TestTemplateVersionManagerGetByIdList(IntegrationBaseTestCase):
     """TesTemplateVersionManagerGetByIdList"""
 
     fixture = fixture_template_vm
 
     def setUp(self):
         """setUp
 
@@ -385,15 +385,15 @@
         )
         self.assertTrue(self.fixture.user1_tvm not in list(version_managers))
         self.assertTrue(self.fixture.user2_tvm in list(version_managers))
         self.assertTrue(self.fixture.global_tvm not in list(version_managers))
 
 
 class TestTemplateVersionManagerGetActiveGlobalVersionManagerByTitle(
-    MongoIntegrationBaseTestCase
+    IntegrationBaseTestCase
 ):
     """TestTemplateVersionManagerGetActiveGlobalVersionManagerByTitle"""
 
     fixture = fixture_template_vm
 
     def setUp(self):
         """setUp
@@ -483,15 +483,15 @@
             template_vm_api.get_active_global_version_manager_by_title(
                 self.fixture.global_tvm.title, request=mock_request
             )
         )
         self.assertEqual(version_manager, self.fixture.global_tvm)
 
 
-class TestTemplateVersionManagerInsert(MongoIntegrationBaseTestCase):
+class TestTemplateVersionManagerInsert(IntegrationBaseTestCase):
     """TestTemplateVersionManagerInsert"""
 
     fixture = fixture_template_vm
 
     def setUp(self):
         """setUp
 
@@ -691,15 +691,15 @@
         template_vm_api.insert(
             self.fixture.global_tvm,
             self.fixture.global_template,
             request=mock_request,
         )
 
 
-class TestTemplateEditTitle(MongoIntegrationBaseTestCase):
+class TestTemplateEditTitle(IntegrationBaseTestCase):
     """TestTemplateEditTitle"""
 
     fixture = fixture_template_vm
 
     def setUp(self):
         """setUp
 
@@ -875,15 +875,15 @@
         """
         mock_request = create_mock_request(user=self.superuser1)
         template_vm_api.edit_title(
             self.fixture.global_tvm, "new_name", request=mock_request
         )
 
 
-class TestTemplateGetGlobalVersionManagers(MongoIntegrationBaseTestCase):
+class TestTemplateGetGlobalVersionManagers(IntegrationBaseTestCase):
     """TestTemplateGetGlobalVersionManagers"""
 
     fixture = fixture_template_vm
 
     def setUp(self):
         """setUp
 
@@ -960,15 +960,15 @@
         list_tvm = template_vm_api.get_global_version_managers(
             request=mock_request
         )
         for tvm in list_tvm:
             self.assertEqual(tvm.user, None)
 
 
-class TestTemplateGetActiveGlobalVersionManager(MongoIntegrationBaseTestCase):
+class TestTemplateGetActiveGlobalVersionManager(IntegrationBaseTestCase):
     """TestTemplateGetActiveGlobalVersionManager"""
 
     fixture = fixture_template_vm
 
     def setUp(self):
         """setUp
 
@@ -1053,17 +1053,15 @@
         list_tvm = template_vm_api.get_active_global_version_manager(
             request=mock_request
         )
         for tvm in list_tvm:
             self.assertEqual(tvm.user, None)
 
 
-class TestTemplateGetActiveVersionManagerByUserId(
-    MongoIntegrationBaseTestCase
-):
+class TestTemplateGetActiveVersionManagerByUserId(IntegrationBaseTestCase):
     """TestTemplateGetActiveVersionManagerByUserId"""
 
     fixture = fixture_template_vm
 
     def setUp(self):
         """setUp
 
@@ -1147,15 +1145,15 @@
         list_tvm = template_vm_api.get_active_version_manager_by_user_id(
             request=mock_request
         )
         for tvm in list_tvm:
             self.assertEqual(tvm.user, str(self.superuser1.id))
 
 
-class TestTemplateGetAllByUserId(MongoIntegrationBaseTestCase):
+class TestTemplateGetAllByUserId(IntegrationBaseTestCase):
     """TestTemplateGetAllByUserId"""
 
     fixture = fixture_template_vm
 
     def setUp(self):
         """setUp
 
@@ -1221,15 +1219,15 @@
         """
         mock_request = create_mock_request(user=self.superuser1)
         list_tvm = template_vm_api.get_all_by_user_id(request=mock_request)
         for tvm in list_tvm:
             self.assertEqual(tvm.user, str(self.superuser1.id))
 
 
-class TestUpdateTemplatesOrdering(MongoIntegrationBaseTestCase):
+class TestUpdateTemplatesOrdering(IntegrationBaseTestCase):
     """Test Update Templates Ordering"""
 
     fixture = fixture_template_vm_ordering
 
     def setUp(self):
         """setUp
 
@@ -1383,15 +1381,15 @@
         ]
         # Act
         template_vm_api.update_templates_ordering(
             list_templates_ordering, user=self.superuser1
         )
 
 
-class TestAccessControlCanWriteList(MongoIntegrationBaseTestCase):
+class TestAccessControlCanWriteList(IntegrationBaseTestCase):
     """Test Access Control Can Write List"""
 
     fixture = fixture_template_vm_ordering
 
     def setUp(self):
         """setUp
 
@@ -1505,15 +1503,15 @@
         access_control.can_write_list(
             template_vm_api.update_templates_ordering,
             template_vm_list,
             self.superuser1,
         )
 
 
-class TestTemplateVersionManagerSortByIdList(MongoIntegrationBaseTestCase):
+class TestTemplateVersionManagerSortByIdList(IntegrationBaseTestCase):
     """Test Template Version Manager Sort By Id List"""
 
     fixture = fixture_template_vm_ordering
 
     def setUp(self):
         """setUp
```

### Comparing `core_main_app-2.2.1/tests/components/template_version_manager/tests_unit.py` & `core_main_app-2.3.0/tests/components/template_version_manager/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/components/template_xsl_rendering/fixtures/fixtures.py` & `core_main_app-2.3.0/tests/components/template_xsl_rendering/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/components/template_xsl_rendering/tests_int.py` & `core_main_app-2.3.0/tests/components/template_xsl_rendering/tests_int.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,21 +10,21 @@
     TemplateXslRendering,
 )
 
 from core_main_app.components.template_xsl_rendering import (
     api as template_xsl_rendering_api,
 )
 from core_main_app.utils.integration_tests.integration_base_transaction_test_case import (
-    MongoIntegrationTransactionTestCase,
+    IntegrationTransactionTestCase,
 )
 
 fixture_template_rendering = TemplateXslRenderingFixtures()
 
 
-class TestTemplateXslRenderingAddOrDelete(MongoIntegrationTransactionTestCase):
+class TestTemplateXslRenderingAddOrDelete(IntegrationTransactionTestCase):
     """Test Template Xsl Rendering Add Or Delete"""
 
     fixture = fixture_template_rendering
 
     def test_add_or_delete_returns_none_when_nothing_happened(self):
         """test_add_or_delete_returns_none_when_nothing_happened
 
@@ -151,17 +151,15 @@
             list_xslt=None,
             default_detail_xslt=None,
             list_detail_xslt=None,
             template_xsl_rendering_id=template_xsl.id,
         )
 
 
-class TestTemplateXslRenderingAddDetailXslt(
-    MongoIntegrationTransactionTestCase
-):
+class TestTemplateXslRenderingAddDetailXslt(IntegrationTransactionTestCase):
     """Test Template Xsl Rendering Add Detail Xslt"""
 
     fixture = fixture_template_rendering
 
     def test_template_xsl_add_detail_xslt_raises_error_when_already_exist_in_detail_list(
         self,
     ):
@@ -198,17 +196,15 @@
         # Assert
         self.assertTrue(
             self.fixture.xsl_transformation_1
             in self.fixture.template_xsl_rendering_1.list_detail_xslt.all()
         )
 
 
-class TestTemplateXslRenderingDeleteDetailXslt(
-    MongoIntegrationTransactionTestCase
-):
+class TestTemplateXslRenderingDeleteDetailXslt(IntegrationTransactionTestCase):
     """Test Template Xsl Rendering Delete Detail Xslt"""
 
     fixture = fixture_template_rendering
 
     def test_template_xsl_delete_detail_xslt_raises_error_when_xslt_is_not_in_detail_list(
         self,
     ):
@@ -248,15 +244,15 @@
         self.assertTrue(
             self.fixture.xsl_transformation_3
             not in self.fixture.template_xsl_rendering_2.list_detail_xslt.all()
         )
 
 
 class TestTemplateXslRenderingSetDefaultDetailXslt(
-    MongoIntegrationTransactionTestCase
+    IntegrationTransactionTestCase
 ):
     """Test Template Xsl Rendering Set Default Detail Xslt"""
 
     fixture = fixture_template_rendering
 
     def test_template_xsl_set_default_detail_xslt_raises_error_when_xslt_is_not_in_detail_list(
         self,
```

### Comparing `core_main_app-2.2.1/tests/components/template_xsl_rendering/tests_unit.py` & `core_main_app-2.3.0/tests/components/template_xsl_rendering/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/components/user/fixtures/fixtures.py` & `core_main_app-2.3.0/tests/components/user/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/components/user/fixtures/tests_int.py` & `core_main_app-2.3.0/tests/components/user/fixtures/tests_int.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """ Integration Test for User Fixtures
 """
 
 from tests.components.user.fixtures.fixtures import UserFixtures
 
 from core_main_app.components.user import api as user_api
 from core_main_app.utils.integration_tests.integration_base_transaction_test_case import (
-    MongoIntegrationTransactionTestCase,
+    IntegrationTransactionTestCase,
 )
 
 
-class TestUserFixtures(MongoIntegrationTransactionTestCase):
+class TestUserFixtures(IntegrationTransactionTestCase):
     """Test User fixtures"""
 
     def test_create_user(self):
         """test create user
 
         Returns:
```

### Comparing `core_main_app-2.2.1/tests/components/user/tests_int.py` & `core_main_app-2.3.0/tests/components/user/tests_int.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """ Integration Test for User
 """
 
 from tests.components.user.fixtures.fixtures import UserFixtures
 from django.contrib.auth.models import User
 from core_main_app.components.user import api as user_api
 from core_main_app.utils.integration_tests.integration_base_transaction_test_case import (
-    MongoIntegrationTransactionTestCase,
+    IntegrationTransactionTestCase,
 )
 
 
-class TestUserGetActiveUsers(MongoIntegrationTransactionTestCase):
+class TestUserGetActiveUsers(IntegrationTransactionTestCase):
     """Test User Get Active Users"""
 
     def test_get_active_users_returns_empty_list(self):
         """test get active users returns empty list
 
         Returns:
 
@@ -32,15 +32,15 @@
         UserFixtures().create_user(username="username")
         # Assert
         result = user_api.get_active_users()
         self.assertEqual(len(result), 1)
         self.assertTrue(user.is_active() for user in result)
 
 
-class TestUserGetUserByUsername(MongoIntegrationTransactionTestCase):
+class TestUserGetUserByUsername(IntegrationTransactionTestCase):
     """Test User Get User By Username"""
 
     def test_get_user_by_username_raises_error_when_does_not_exist(self):
         """test get user by username raises error when does not exist
 
         Returns:
 
@@ -60,15 +60,15 @@
         # Act
         result = user_api.get_user_by_username("username")
         # Assert
         self.assertIsInstance(result, User)
         self.assertEqual(result.username, user.username)
 
 
-class TestUserCreateAndSaveUser(MongoIntegrationTransactionTestCase):
+class TestUserCreateAndSaveUser(IntegrationTransactionTestCase):
     """Test User Create And Save User"""
 
     def test_create_and_save_user_creates_user(self):
         """test create and save user creates user
 
         Returns:
 
@@ -79,15 +79,15 @@
             "username", "password", "firstname", "lastname", "email"
         )
         # Assert
         self.assertIsInstance(result, User)
         self.assertEqual(result.username, "username")
 
 
-class TestUserUpsert(MongoIntegrationTransactionTestCase):
+class TestUserUpsert(IntegrationTransactionTestCase):
     """Test User Upsert"""
 
     def test_upsert_user_creates_user(self):
         """test upsert creates user
 
         Returns:
 
@@ -113,15 +113,15 @@
         # Act
         result = user_api.upsert(user)
         # Assert
         self.assertIsInstance(result, User)
         self.assertEqual(result.username, "new_username")
 
 
-class TestUserGetAllUsersExceptList(MongoIntegrationTransactionTestCase):
+class TestUserGetAllUsersExceptList(IntegrationTransactionTestCase):
     """Test User Get All Users Except List"""
 
     def test_get_all_users_except_list_returns_empty_list(self):
         """test get all users except list returns empty list
 
         Returns:
 
@@ -149,15 +149,15 @@
         # Assert
         self.assertEqual(len(result), 2)
         self.assertNotIn(user1, result)
         self.assertIn(user2, result)
         self.assertIn(user3, result)
 
 
-class TestUserGetAllUsersExceptListId(MongoIntegrationTransactionTestCase):
+class TestUserGetAllUsersExceptListId(IntegrationTransactionTestCase):
     """Test User Get All Users Except List Id"""
 
     def test_get_all_users_except_list_id_returns_empty_list(self):
         """test get all users except list id returns empty list
 
         Returns:
 
@@ -185,15 +185,15 @@
         # Assert
         self.assertEqual(len(result), 2)
         self.assertNotIn(user1, result)
         self.assertIn(user2, result)
         self.assertIn(user3, result)
 
 
-class TestUserGetAllUsersByListId(MongoIntegrationTransactionTestCase):
+class TestUserGetAllUsersByListId(IntegrationTransactionTestCase):
     """Test User Get All Users By List Id"""
 
     def test_get_all_users_by_list_id_returns_empty_list(self):
         """test get all users By list id returns empty list
 
         Returns:
 
@@ -233,15 +233,15 @@
         # Assert
         self.assertEqual(len(result), 2)
         self.assertIn(user1, result)
         self.assertIn(user2, result)
         self.assertNotIn(user3, result)
 
 
-class TestUserGetIdUsernameDict(MongoIntegrationTransactionTestCase):
+class TestUserGetIdUsernameDict(IntegrationTransactionTestCase):
     """Test User Get Id Username Dict"""
 
     def test_get_id_username_dict_returns_empty_list(self):
         """test get id username dict returns empty list
 
         Returns:
```

### Comparing `core_main_app-2.2.1/tests/components/version_manager/tests_int_access_control.py` & `core_main_app-2.3.0/tests/components/version_manager/tests_int_access_control.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 )
 from core_main_app.components.version_manager import (
     access_control as access_control_api,
 )
 from core_main_app.access_control.exceptions import AccessControlError
 from core_main_app.components.version_manager import api as version_manager_api
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import create_mock_request
 
 fixture_template_vm = TemplateVersionManagerAccessControlFixtures()
 
 
-class TestVersionManagerDisable(MongoIntegrationBaseTestCase):
+class TestVersionManagerDisable(IntegrationBaseTestCase):
     """TestVersionManagerDisable"""
 
     fixture = fixture_template_vm
 
     def setUp(self):
         """setup
 
@@ -218,15 +218,15 @@
         mock_request = create_mock_request(user=self.superuser1)
         version_manager_api.disable(
             self.fixture.user2_tvm, request=mock_request
         )
         self.assertTrue(self.fixture.user2_tvm.is_disabled)
 
 
-class TestVersionManagerRestore(MongoIntegrationBaseTestCase):
+class TestVersionManagerRestore(IntegrationBaseTestCase):
     """TestVersionManagerRestore"""
 
     fixture = fixture_template_vm
 
     def setUp(self):
         """setup
 
@@ -420,15 +420,15 @@
         mock_request = create_mock_request(user=self.superuser1)
         version_manager_api.restore(
             self.fixture.user2_tvm, request=mock_request
         )
         self.assertFalse(self.fixture.user2_tvm.is_disabled)
 
 
-class TestVersionManagerRestoreVersion(MongoIntegrationBaseTestCase):
+class TestVersionManagerRestoreVersion(IntegrationBaseTestCase):
     """TestVersionManagerRestoreVersion"""
 
     fixture = fixture_template_vm
 
     def setUp(self):
         """setup
 
@@ -642,15 +642,15 @@
         )
         self.assertTrue(
             str(self.fixture.user2_template.id)
             not in self.fixture.user2_template.version_manager.disabled_versions
         )
 
 
-class TestVersionManagerDisableVersion(MongoIntegrationBaseTestCase):
+class TestVersionManagerDisableVersion(IntegrationBaseTestCase):
     """TestVersionManagerDisableVersion"""
 
     fixture = fixture_template_vm
 
     def setUp(self):
         """setup
 
@@ -857,15 +857,15 @@
         )
         self.assertTrue(
             str(self.fixture.user2_template.id)
             in self.fixture.user2_template.version_manager.disabled_versions
         )
 
 
-class TestVersionManagerSetCurrent(MongoIntegrationBaseTestCase):
+class TestVersionManagerSetCurrent(IntegrationBaseTestCase):
     """TestVersionManagerSetCurrent"""
 
     fixture = fixture_template_vm
 
     def setUp(self):
         """setup
 
@@ -1072,15 +1072,15 @@
         )
         self.assertEqual(
             str(self.fixture.user2_template.id),
             self.fixture.user2_template.version_manager.current,
         )
 
 
-class TestVersionManagerUpsert(MongoIntegrationBaseTestCase):
+class TestVersionManagerUpsert(IntegrationBaseTestCase):
     """TestVersionManagerUpsert"""
 
     fixture = fixture_template_vm
 
     def setUp(self):
         """setup
 
@@ -1256,15 +1256,15 @@
         """
         mock_request = create_mock_request(user=self.superuser1)
         version_manager_api.upsert(
             self.fixture.global_tvm, request=mock_request
         )
 
 
-class TestVersionManagerGetVersionNumber(MongoIntegrationBaseTestCase):
+class TestVersionManagerGetVersionNumber(IntegrationBaseTestCase):
     """TestVersionManagerGetVersionNumber"""
 
     fixture = fixture_template_vm
 
     def setUp(self):
         """setup
 
@@ -1430,15 +1430,15 @@
             version_manager_api.get_version_number(
                 self.fixture.user2_tvm,
                 self.fixture.user2_template,
                 request=mock_request,
             )
 
 
-class TestVersionManagerGetVersionByNumber(MongoIntegrationBaseTestCase):
+class TestVersionManagerGetVersionByNumber(IntegrationBaseTestCase):
     """TestVersionManagerGetVersionByNumber"""
 
     fixture = fixture_template_vm
 
     def setUp(self):
         """setup
 
@@ -1582,15 +1582,15 @@
         mock_request = create_mock_request(user=self.staff_user1)
         with self.assertRaises(AccessControlError):
             version_manager_api.get_version_by_number(
                 self.fixture.user2_tvm, 1, request=mock_request
             )
 
 
-class TestAccessControlCanRead(MongoIntegrationBaseTestCase):
+class TestAccessControlCanRead(IntegrationBaseTestCase):
     """Test Access Control Can Read"""
 
     fixture = fixture_template_vm
 
     def setUp(self):
         """setUp
 
@@ -1740,15 +1740,15 @@
             self.fixture.user1_tvm.clean, document_id, mock_request
         )
 
         # Assert
         self.assertEqual(result, self.fixture.user1_tvm)
 
 
-class TestAccessControlCanReadGlobal(MongoIntegrationBaseTestCase):
+class TestAccessControlCanReadGlobal(IntegrationBaseTestCase):
     """Test Access Control Can Read Global"""
 
     fixture = fixture_template_vm
 
     def setUp(self):
         """setUp
```

### Comparing `core_main_app-2.2.1/tests/components/version_manager/tests_unit.py` & `core_main_app-2.3.0/tests/components/version_manager/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/components/web_page/tests_unit.py` & `core_main_app-2.3.0/tests/components/web_page/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/components/web_page_login/tests_unit.py` & `core_main_app-2.3.0/tests/components/web_page_login/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/components/workspace/fixtures/fixtures.py` & `core_main_app-2.3.0/tests/components/workspace/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/components/workspace/fixtures/tests_int.py` & `core_main_app-2.3.0/tests/components/workspace/fixtures/tests_int.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """ Integration Test for Workspace Fixtures
 """
 
 from tests.components.workspace.fixtures.fixtures import WorkspaceFixtures
 
 from core_main_app.components.workspace import api as workspace_api
 from core_main_app.utils.integration_tests.integration_base_transaction_test_case import (
-    MongoIntegrationTransactionTestCase,
+    IntegrationTransactionTestCase,
 )
 
 TITLE = "title"
 
 
-class TestWorkspaceFixtures(MongoIntegrationTransactionTestCase):
+class TestWorkspaceFixtures(IntegrationTransactionTestCase):
     """Test Workspace fixtures"""
 
     def test_create_workspace(self):
         """test create workspace
 
         Returns:
```

### Comparing `core_main_app-2.2.1/tests/components/workspace/tests_int.py` & `core_main_app-2.3.0/tests/components/workspace/tests_int.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 from tests.components.workspace.fixtures.fixtures import WorkspaceFixtures
 
 from core_main_app.commons import exceptions
 from core_main_app.components.data.models import Data
 from core_main_app.components.template.models import Template
 from core_main_app.components.workspace import api as workspace_api
 from core_main_app.utils.integration_tests.integration_base_transaction_test_case import (
-    MongoIntegrationTransactionTestCase,
+    IntegrationTransactionTestCase,
 )
 
 TITLE_1 = "title 1"
 
 
-class TestCreateWorkspace(MongoIntegrationTransactionTestCase):
+class TestCreateWorkspace(IntegrationTransactionTestCase):
     """TestCreateWorkspace"""
 
     def test_create_one_workspace(self):
         """test create one workspace
 
         Returns:
 
@@ -82,15 +82,15 @@
         # Act
         workspace = workspace_api.create_and_save(TITLE_1)
         # Assert
         self.assertEqual(workspace.title, TITLE_1)
         self.assertIsNone(workspace.owner)
 
 
-class TestIsWorkspaceGlobal(MongoIntegrationTransactionTestCase):
+class TestIsWorkspaceGlobal(IntegrationTransactionTestCase):
     """Test Is Workspace Global"""
 
     def test_is_workspace_global_true(self):
         """test is workspace global true
 
         Returns:
 
@@ -112,15 +112,15 @@
         workspace = WorkspaceFixtures.create_workspace("1", TITLE_1)
         # Act
         result = workspace_api.is_workspace_global(workspace)
         # Assert
         self.assertFalse(result)
 
 
-class TestGetGlobalWorkspace(MongoIntegrationTransactionTestCase):
+class TestGetGlobalWorkspace(IntegrationTransactionTestCase):
     """Test Get Global Workspace"""
 
     def test_get_global_workspace(self):
         """test get global workspace
 
         Returns:
 
@@ -155,15 +155,15 @@
         # Context
         WorkspaceFixtures.create_workspace("1", TITLE_1)
         # Act
         with self.assertRaises(exceptions.DoesNotExist):
             workspace_api.get_global_workspace()
 
 
-class TestCheckIfWorkspaceCanBeChanged(MongoIntegrationTransactionTestCase):
+class TestCheckIfWorkspaceCanBeChanged(IntegrationTransactionTestCase):
     """Test Check If Workspace Can Be Changed"""
 
     def test_workspace_can_be_changed_return_true_if_workspace_is_none_and_allow_public_is_false(
         self,
     ):
         """test workspace can be changed return true if workspace is none and allow public is false
```

### Comparing `core_main_app-2.2.1/tests/components/xsl_transformation/tests_unit.py` & `core_main_app-2.3.0/tests/components/xsl_transformation/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/rest/blob/tests_int.py` & `core_main_app-2.3.0/tests/rest/blob/tests_int.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,25 +11,25 @@
     AccessControlBlobFixture,
 )
 
 from core_main_app.components.blob.models import Blob
 from core_main_app.components.workspace.models import Workspace
 from core_main_app.rest.blob import views
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import RequestMock
 
 RESOURCES_PATH = join(dirname(abspath(__file__)), "data")
 fixture_blob = BlobFixtures()
 fixture_blob_workspace = AccessControlBlobFixture()
 
 
-class TestBlobListAdmin(MongoIntegrationBaseTestCase):
+class TestBlobListAdmin(IntegrationBaseTestCase):
     """TestBlobListAdmin"""
 
     fixture = fixture_blob
 
     @override_settings(ROOT_URLCONF="core_main_app.urls")
     def test_get_as_user_returns_http_403(self):
         """test_get_as_user_returns_http_403
@@ -63,15 +63,15 @@
             views.BlobListAdmin.as_view(), user
         )
 
         # Assert
         self.assertEqual(len(response.data), 3)
 
 
-class TestBlobList(MongoIntegrationBaseTestCase):
+class TestBlobList(IntegrationBaseTestCase):
     """TestBlobList"""
 
     fixture = fixture_blob
 
     def setUp(self):
         """setUp
 
@@ -283,15 +283,15 @@
             views.BlobList.as_view(), user, data=self.data, content_type=None
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_400_BAD_REQUEST)
 
 
-class TestBlobDetail(MongoIntegrationBaseTestCase):
+class TestBlobDetail(IntegrationBaseTestCase):
     """TestBlobDetail"""
 
     fixture = fixture_blob
 
     def setUp(self):
         """setUp
 
@@ -475,15 +475,15 @@
             param={"pk": str(self.fixture.blob_1.id)},
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_204_NO_CONTENT)
 
 
-class TestBlobDownload(MongoIntegrationBaseTestCase):
+class TestBlobDownload(IntegrationBaseTestCase):
     """TestBlobDownload"""
 
     fixture = fixture_blob
 
     def setUp(self):
         """setUp
 
@@ -548,15 +548,15 @@
             param={"pk": str(self.fixture.blob_1.id)},
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
 
 
-class TestBlobDeleteList(MongoIntegrationBaseTestCase):
+class TestBlobDeleteList(IntegrationBaseTestCase):
     """TestBlobDeleteList"""
 
     fixture = fixture_blob
 
     def setUp(self):
         """setUp
 
@@ -602,15 +602,15 @@
             views.BlobDeleteList.as_view(), user, data=self.data
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_204_NO_CONTENT)
 
 
-class TestBlobAssign(MongoIntegrationBaseTestCase):
+class TestBlobAssign(IntegrationBaseTestCase):
     """TestBlobAssign"""
 
     fixture = fixture_blob_workspace
 
     @patch.object(Workspace, "get_by_id")
     @patch.object(Blob, "get_by_id")
     def test_get_returns_http_200(self, blob_get_by_id, workspace_get_by_id):
@@ -752,15 +752,15 @@
             param={"pk": blob.id, "workspace_id": fake_workspace_id},
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_404_NOT_FOUND)
 
 
-class TestBlobChangeOwner(MongoIntegrationBaseTestCase):
+class TestBlobChangeOwner(IntegrationBaseTestCase):
     """TestBlobChangeOwner"""
 
     fixture = fixture_blob_workspace
 
     @patch("core_main_app.components.user.api.get_user_by_id")
     @patch.object(Blob, "get_by_id")
     def test_get_returns_http_200_if_user_is_superuser(
```

### Comparing `core_main_app-2.2.1/tests/rest/blob/tests_permissions.py` & `core_main_app-2.3.0/tests/rest/blob/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/rest/data/tests_int.py` & `core_main_app-2.3.0/tests/rest/data/tests_int.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 
 from core_main_app.components.data import api as data_api
 from core_main_app.components.data.models import Data
 from core_main_app.components.workspace import api as workspace_api
 from core_main_app.components.workspace.models import Workspace
 from core_main_app.rest.data import views as data_rest_views
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.integration_tests.integration_base_transaction_test_case import (
-    MongoIntegrationTransactionTestCase,
+    IntegrationTransactionTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import RequestMock
 
 fixture_data = DataFixtures()
 fixture_data_query = QueryDataFixtures()
 fixture_data_workspace = AccessControlDataFixture()
 
 
-class TestDataListByWorkspace(MongoIntegrationBaseTestCase):
+class TestDataListByWorkspace(IntegrationBaseTestCase):
     """Test Data List By Workspace"""
 
     fixture = fixture_data_workspace
 
     def setUp(self):
         """setUp
 
@@ -109,15 +109,15 @@
             param={"workspace_id": self.fixture.workspace_1.id},
         )
 
         # Assert
         self.assertEqual(len(response.data), 2)
 
 
-class TestDataList(MongoIntegrationBaseTestCase):
+class TestDataList(IntegrationBaseTestCase):
     """TestDataList"""
 
     fixture = fixture_data
 
     def setUp(self):
         """setUp
 
@@ -314,15 +314,15 @@
             data_rest_views.DataList.as_view(), user, data=mock_data
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_400_BAD_REQUEST)
 
 
-class TestDataDetail(MongoIntegrationBaseTestCase):
+class TestDataDetail(IntegrationBaseTestCase):
     """Test Data Detail"""
 
     fixture = fixture_data
 
     def setUp(self):
         """setUp
 
@@ -477,15 +477,15 @@
             param={"pk": self.fixture.data_1.id},
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_400_BAD_REQUEST)
 
 
-class TestDataDownload(MongoIntegrationBaseTestCase):
+class TestDataDownload(IntegrationBaseTestCase):
     """TestDataDownload"""
 
     fixture = fixture_data
 
     def setUp(self):
         """setUp
 
@@ -571,15 +571,15 @@
             data={"pretty_print": "true"},
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_400_BAD_REQUEST)
 
 
-class TestExecuteLocalQueryView(MongoIntegrationBaseTestCase):
+class TestExecuteLocalQueryView(IntegrationBaseTestCase):
     """TestExecuteLocalQueryView"""
 
     fixture = fixture_data_query
 
     def setUp(self):
         """setUp
 
@@ -876,17 +876,15 @@
             data=self.data,
         )
 
         # Assert
         self.assertEqual(len(response.data), 1)
 
 
-class TestExecuteLocalQueryViewWorkspaceCase(
-    MongoIntegrationTransactionTestCase
-):
+class TestExecuteLocalQueryViewWorkspaceCase(IntegrationTransactionTestCase):
     """TestExecuteLocalQueryViewWorkspaceCase"""
 
     fixture = fixture_data_workspace
 
     def setUp(self):
         """setUp
 
@@ -1266,15 +1264,15 @@
             data=self.data,
         )
 
         # Assert
         self.assertEqual(len(response.data), 0)
 
 
-class TestDataAssign(MongoIntegrationBaseTestCase):
+class TestDataAssign(IntegrationBaseTestCase):
     """TestDataAssign"""
 
     fixture = fixture_data_workspace
 
     @patch.object(Workspace, "get_by_id")
     @patch.object(Data, "get_by_id")
     def test_get_returns_http_200(self, data_get_by_id, workspace_get_by_id):
@@ -1416,15 +1414,15 @@
             param={"pk": data.id, "workspace_id": fake_workspace_id},
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_404_NOT_FOUND)
 
 
-class TestDataChangeOwner(MongoIntegrationBaseTestCase):
+class TestDataChangeOwner(IntegrationBaseTestCase):
     """TestDataChangeOwner"""
 
     fixture = fixture_data_workspace
 
     @patch("core_main_app.components.user.api.get_user_by_id")
     @patch.object(Data, "get_by_id")
     def test_get_returns_http_200_if_user_is_superuser(
@@ -1522,15 +1520,15 @@
             param={"pk": data.id, "user_id": self.fixture.workspace_1.id},
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
 
 
-class TestDataPermissions(MongoIntegrationTransactionTestCase):
+class TestDataPermissions(IntegrationTransactionTestCase):
     """TestDataPermissions"""
 
     fixture = fixture_data_workspace
 
     def setUp(self):
         """Insert needed data.
```

### Comparing `core_main_app-2.2.1/tests/rest/data/tests_permissions.py` & `core_main_app-2.3.0/tests/rest/data/tests_permissions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 """ Authentication tests for Data REST API
 """
 from unittest.mock import patch, Mock
 
 from django.test import SimpleTestCase
 from rest_framework import status
-from rest_framework.response import Response
-from rest_framework.status import HTTP_200_OK
+from tests.mocks import MockQuerySet
 
 from core_main_app.components.data import api as data_api
 from core_main_app.components.data.models import Data
 from core_main_app.components.workspace import api as workspace_api
 from core_main_app.rest.data import views as data_rest_views
-from core_main_app.rest.data.abstract_views import (
-    AbstractExecuteLocalQueryView,
-)
 from core_main_app.rest.data.admin_serializers import AdminDataSerializer
 from core_main_app.rest.data.serializers import (
     DataSerializer,
     DataWithTemplateInfoSerializer,
 )
 from core_main_app.rest.data.views import Migration as data_migration
 from core_main_app.rest.data.views import Validation as data_validation
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import RequestMock
-from tests.mocks import MockQuerySet
 
 
 class TestDataListPostPermissions(SimpleTestCase):
     """TestDataListPostPermissions"""
 
     def test_anonymous_returns_http_403(self):
         """test_anonymous_returns_http_403
@@ -727,94 +722,14 @@
             mock_user,
             data={"id": 0},
         )
 
         self.assertEqual(response.status_code, status.HTTP_200_OK)
 
 
-class TestDataLocalQueryGetPermissions(SimpleTestCase):
-    """TestDataLocalQueryGetPermissions"""
-
-    @patch.object(AbstractExecuteLocalQueryView, "execute_query")
-    def test_anonymous_returns_http_200(
-        self, mock_abstract_local_query_execute_query
-    ):
-        """test_anonymous_returns_http_200
-
-        Args:
-            mock_abstract_local_query_execute_query:
-
-        Returns:
-
-        """
-        mock_abstract_local_query_execute_query.return_value = Response(
-            status=HTTP_200_OK
-        )
-
-        response = RequestMock.do_request_get(
-            data_rest_views.ExecuteLocalQueryView.as_view(),
-            None,
-            data={"query": "{}"},
-        )
-
-        self.assertEqual(response.status_code, status.HTTP_200_OK)
-
-    @patch.object(AbstractExecuteLocalQueryView, "execute_query")
-    def test_authenticated_returns_http_200(
-        self, mock_abstract_local_query_execute_query
-    ):
-        """test_authenticated_returns_http_200
-
-        Args:
-            mock_abstract_local_query_execute_query:
-
-        Returns:
-
-        """
-        mock_abstract_local_query_execute_query.return_value = Response(
-            status=HTTP_200_OK
-        )
-
-        mock_user = create_mock_user(1)
-
-        response = RequestMock.do_request_get(
-            data_rest_views.ExecuteLocalQueryView.as_view(),
-            mock_user,
-            data={"query": "{}"},
-        )
-
-        self.assertEqual(response.status_code, status.HTTP_200_OK)
-
-    @patch.object(AbstractExecuteLocalQueryView, "execute_query")
-    def test_staff_returns_http_200(
-        self, mock_abstract_local_query_execute_query
-    ):
-        """test_staff_returns_http_200
-
-        Args:
-            mock_abstract_local_query_execute_query:
-
-        Returns:
-
-        """
-        mock_abstract_local_query_execute_query.return_value = Response(
-            status=HTTP_200_OK
-        )
-
-        mock_user = create_mock_user(1, is_staff=True)
-
-        response = RequestMock.do_request_get(
-            data_rest_views.ExecuteLocalQueryView.as_view(),
-            mock_user,
-            data={"query": "{}"},
-        )
-
-        self.assertEqual(response.status_code, status.HTTP_200_OK)
-
-
 class TestDataLocalQueryPostPermissions(SimpleTestCase):
     """TestDataLocalQueryPostPermissions"""
 
     @patch.object(data_api, "execute_query")
     def test_anonymous_returns_http_200(self, mock_data_api_execute_query):
         """test_anonymous_returns_http_200
 
@@ -874,94 +789,14 @@
             data_rest_views.ExecuteLocalQueryView.as_view(),
             mock_user,
             data={"query": "{}"},
         )
 
         self.assertEqual(response.status_code, status.HTTP_200_OK)
 
-
-class TestDataKeywordQueryGetPermissions(SimpleTestCase):
-    """TestDataKeywordQueryGetPermissions"""
-
-    @patch.object(AbstractExecuteLocalQueryView, "execute_query")
-    def test_anonymous_returns_http_200(
-        self, mock_abstract_local_query_execute_query
-    ):
-        """test_anonymous_returns_http_200
-
-        Args:
-            mock_abstract_local_query_execute_query:
-
-        Returns:
-
-        """
-        mock_abstract_local_query_execute_query.return_value = Response(
-            status=HTTP_200_OK
-        )
-
-        response = RequestMock.do_request_get(
-            data_rest_views.ExecuteLocalQueryView.as_view(),
-            None,
-            data={"query": "{}"},
-        )
-
-        self.assertEqual(response.status_code, status.HTTP_200_OK)
-
-    @patch.object(AbstractExecuteLocalQueryView, "execute_query")
-    def test_authenticated_returns_http_200(
-        self, mock_abstract_local_query_execute_query
-    ):
-        """test_authenticated_returns_http_200
-
-        Args:
-            mock_abstract_local_query_execute_query:
-
-        Returns:
-
-        """
-        mock_abstract_local_query_execute_query.return_value = Response(
-            status=HTTP_200_OK
-        )
-
-        mock_user = create_mock_user(1)
-
-        response = RequestMock.do_request_get(
-            data_rest_views.ExecuteLocalQueryView.as_view(),
-            mock_user,
-            data={"query": "{}"},
-        )
-
-        self.assertEqual(response.status_code, status.HTTP_200_OK)
-
-    @patch.object(AbstractExecuteLocalQueryView, "execute_query")
-    def test_staff_returns_http_200(
-        self, mock_abstract_local_query_execute_query
-    ):
-        """test_staff_returns_http_200
-
-        Args:
-            mock_abstract_local_query_execute_query:
-
-        Returns:
-
-        """
-        mock_abstract_local_query_execute_query.return_value = Response(
-            status=HTTP_200_OK
-        )
-
-        mock_user = create_mock_user(1, is_staff=True)
-
-        response = RequestMock.do_request_get(
-            data_rest_views.ExecuteLocalQueryView.as_view(),
-            mock_user,
-            data={"query": "{}"},
-        )
-
-        self.assertEqual(response.status_code, status.HTTP_200_OK)
-
 
 class TestDataKeywordQueryPostPermissions(SimpleTestCase):
     """TestDataKeywordQueryPostPermissions"""
 
     @patch.object(data_api, "execute_query")
     def test_anonymous_returns_http_200(self, mock_data_api_execute_query):
         """test_anonymous_returns_http_200
```

### Comparing `core_main_app-2.2.1/tests/rest/data/tests_unit.py` & `core_main_app-2.3.0/tests/rest/data/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/rest/template/tests_int.py` & `core_main_app-2.3.0/tests/rest/template/tests_int.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 from rest_framework import status
 from tests.components.template.fixtures.fixtures import (
     AccessControlTemplateFixture,
 )
 
 from core_main_app.rest.template import views as template_rest_views
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import RequestMock
 
 
-class TestTemplateDownload(MongoIntegrationBaseTestCase):
+class TestTemplateDownload(IntegrationBaseTestCase):
     fixture = AccessControlTemplateFixture()
 
     def setUp(self):
         super(TestTemplateDownload, self).setUp()
 
     def test_get_returns_http_200(self):
         # Arrange
```

### Comparing `core_main_app-2.2.1/tests/rest/template/tests_permission.py` & `core_main_app-2.3.0/tests/rest/template/tests_permission.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/rest/template/tests_unit.py` & `core_main_app-2.3.0/tests/rest/template/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/rest/template_version_manager/tests_int.py` & `core_main_app-2.3.0/tests/rest/template_version_manager/tests_int.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,28 +10,28 @@
     TemplateVersionManagerOrderingFixtures,
     TemplateVersionManagerAccessControlFixtures,
 )
 
 from core_main_app.components.template import api as template_api
 from core_main_app.rest.template_version_manager import views
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import (
     RequestMock,
     create_mock_request,
 )
 
 fixture_template = TemplateVersionManagerFixtures()
 fixture_template_2 = TemplateVersionManagerAccessControlFixtures()
 fixture_template_vm_ordering = TemplateVersionManagerOrderingFixtures()
 
 
-class TestGlobalTemplateVersionManagerList(MongoIntegrationBaseTestCase):
+class TestGlobalTemplateVersionManagerList(IntegrationBaseTestCase):
     """TestGlobalTemplateVersionManagerList"""
 
     fixture = fixture_template
 
     def setUp(self):
         """setUp
 
@@ -164,15 +164,15 @@
             data={"is_disabled": not self.fixture.template_vm_1.is_disabled},
         )
 
         # Assert
         self.assertEqual(len(response.data), 0)
 
 
-class TestUserTemplateVersionManagerList(MongoIntegrationBaseTestCase):
+class TestUserTemplateVersionManagerList(IntegrationBaseTestCase):
     """TestUserTemplateVersionManagerList"""
 
     fixture = fixture_template
 
     def setUp(self):
         """setUp
 
@@ -305,15 +305,15 @@
             data={"is_disabled": not self.fixture.template_vm_2.is_disabled},
         )
 
         # Assert
         self.assertEqual(len(response.data), 0)
 
 
-class TestTemplateVersionManagerDetail(MongoIntegrationBaseTestCase):
+class TestTemplateVersionManagerDetail(IntegrationBaseTestCase):
     """TestTemplateVersionManagerDetail"""
 
     fixture = fixture_template
 
     def setUp(self):
         """setUp
 
@@ -378,15 +378,15 @@
             param={"pk": -1},
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_404_NOT_FOUND)
 
 
-class TestTemplateVersion(MongoIntegrationBaseTestCase):
+class TestTemplateVersion(IntegrationBaseTestCase):
     """TestTemplateVersion"""
 
     fixture = fixture_template
 
     def setUp(self):
         """setUp
 
@@ -517,15 +517,15 @@
             param={"pk": str(self.fixture.template_vm_1.id)},
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
 
 
-class TestUserTemplateList(MongoIntegrationBaseTestCase):
+class TestUserTemplateList(IntegrationBaseTestCase):
     """TestUserTemplateList"""
 
     fixture = fixture_template
 
     def setUp(self):
         """setUp
 
@@ -688,15 +688,15 @@
             views.UserTemplateList.as_view(), user, data=self.data
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_400_BAD_REQUEST)
 
 
-class TestGlobalTemplateList(MongoIntegrationBaseTestCase):
+class TestGlobalTemplateList(IntegrationBaseTestCase):
     """TestGlobalTemplateList"""
 
     fixture = fixture_template
 
     def setUp(self):
         """setUp
 
@@ -787,15 +787,15 @@
             template_id, request=mock_request
         )
 
         # Assert
         self.assertEqual(template_object.version_manager.user, None)
 
 
-class TestCurrentTemplateVersion(MongoIntegrationBaseTestCase):
+class TestCurrentTemplateVersion(IntegrationBaseTestCase):
     """TestCurrentTemplateVersion"""
 
     fixture = fixture_template
 
     def test_patch_returns_http_200(self):
         """test_patch_returns_http_200
 
@@ -888,15 +888,15 @@
             param={"pk": str(self.fixture.template_2_1.id)},
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
 
 
-class TestDisableTemplateVersion(MongoIntegrationBaseTestCase):
+class TestDisableTemplateVersion(IntegrationBaseTestCase):
     """TestDisableTemplateVersion"""
 
     fixture = fixture_template
 
     def test_patch_returns_http_200(self):
         """test_patch_returns_http_200
 
@@ -1008,15 +1008,15 @@
             param={"pk": str(self.fixture.template_2_1.id)},
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
 
 
-class TestRestoreTemplateVersion(MongoIntegrationBaseTestCase):
+class TestRestoreTemplateVersion(IntegrationBaseTestCase):
     """TestRestoreTemplateVersion"""
 
     fixture = fixture_template
 
     def test_patch_returns_http_200(self):
         """test_patch_returns_http_200
 
@@ -1109,15 +1109,15 @@
             param={"pk": str(self.fixture.template_2_1.id)},
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
 
 
-class TestDisableTemplateVersionManager(MongoIntegrationBaseTestCase):
+class TestDisableTemplateVersionManager(IntegrationBaseTestCase):
     """TestDisableTemplateVersionManager"""
 
     fixture = fixture_template
 
     def test_patch_returns_http_200(self):
         """test_patch_returns_http_200
 
@@ -1211,15 +1211,15 @@
             param={"pk": str(self.fixture.template_vm_2.id)},
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
 
 
-class TestRestoreTemplateVersionManager(MongoIntegrationBaseTestCase):
+class TestRestoreTemplateVersionManager(IntegrationBaseTestCase):
     """TestRestoreTemplateVersionManager"""
 
     fixture = fixture_template
 
     def test_patch_returns_http_200(self):
         """test_patch_returns_http_200
 
@@ -1313,15 +1313,15 @@
             param={"pk": str(self.fixture.template_vm_2.id)},
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
 
 
-class TemplateVersionManagerOrdering(MongoIntegrationBaseTestCase):
+class TemplateVersionManagerOrdering(IntegrationBaseTestCase):
     """TemplateVersionManagerOrdering"""
 
     fixture = fixture_template_vm_ordering
 
     def test_patch_as_owner_returns_http_200(self):
         """test_patch_as_owner_returns_http_200
 
@@ -1383,15 +1383,15 @@
             },
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_200_OK)
 
 
-class TestTemplateVersionManagerList(MongoIntegrationBaseTestCase):
+class TestTemplateVersionManagerList(IntegrationBaseTestCase):
     """TestTemplateVersionManagerList"""
 
     fixture = fixture_template_2
 
     def setUp(self):
         """setUp
```

### Comparing `core_main_app-2.2.1/tests/rest/template_version_manager/tests_permission.py` & `core_main_app-2.3.0/tests/rest/template_version_manager/tests_permission.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/rest/template_version_manager/tests_unit.py` & `core_main_app-2.3.0/tests/rest/template_version_manager/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/rest/template_xsl_rendering/tests_int.py` & `core_main_app-2.3.0/tests/rest/template_xsl_rendering/tests_int.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 from rest_framework import status
 from tests.components.template_xsl_rendering.fixtures.fixtures import (
     TemplateXslRenderingFixtures,
 )
 
 from core_main_app.rest.template_xsl_rendering import views
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import RequestMock
 
 fixture_template_xsl_rendering = TemplateXslRenderingFixtures()
 
 
-class TestTemplateXslRenderingAddDetailXslt(MongoIntegrationBaseTestCase):
+class TestTemplateXslRenderingAddDetailXslt(IntegrationBaseTestCase):
     """TestTemplateXslRenderingAddDetailXslt"""
 
     fixture = fixture_template_xsl_rendering
 
     def setUp(self):
         """setUp
 
@@ -113,17 +113,15 @@
         # Assert
 
         self.assertEqual(
             response.status_code, status.HTTP_500_INTERNAL_SERVER_ERROR
         )
 
 
-class TestTemplateXslRenderingSetDefaultDetailXslt(
-    MongoIntegrationBaseTestCase
-):
+class TestTemplateXslRenderingSetDefaultDetailXslt(IntegrationBaseTestCase):
     """TestTemplateXslRenderingSetDefaultDetailXslt"""
 
     fixture = fixture_template_xsl_rendering
 
     def setUp(self):
         """setUp
 
@@ -188,15 +186,15 @@
         # Assert
 
         self.assertEqual(
             response.status_code, status.HTTP_500_INTERNAL_SERVER_ERROR
         )
 
 
-class TestTemplateXslRenderingRemoveDetailXslt(MongoIntegrationBaseTestCase):
+class TestTemplateXslRenderingRemoveDetailXslt(IntegrationBaseTestCase):
     """TestTemplateXslRenderingRemoveDetailXslt"""
 
     fixture = fixture_template_xsl_rendering
 
     def setUp(self):
         """setUp
 
@@ -326,15 +324,15 @@
         # Assert
 
         self.assertEqual(
             response.status_code, status.HTTP_500_INTERNAL_SERVER_ERROR
         )
 
 
-class TestTemplateXslRenderingSetListDetailXslt(MongoIntegrationBaseTestCase):
+class TestTemplateXslRenderingSetListDetailXslt(IntegrationBaseTestCase):
     """TestTemplateXslRenderingSetListDetailXslt"""
 
     fixture = fixture_template_xsl_rendering
 
     def setUp(self):
         """setUp
```

### Comparing `core_main_app-2.2.1/tests/rest/template_xsl_rendering/tests_permissions.py` & `core_main_app-2.3.0/tests/rest/template_xsl_rendering/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/rest/tests_views.py` & `core_main_app-2.3.0/tests/rest/tests_views.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/rest/user/tests_int.py` & `core_main_app-2.3.0/tests/rest/user/tests_int.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """ Integration Test for User Rest API
 """
 from rest_framework.status import HTTP_404_NOT_FOUND
 from tests.components.user.fixtures.fixtures import UserFixtures
 
 from core_main_app.rest.user import views as user_rest_views
 from core_main_app.utils.integration_tests.integration_base_transaction_test_case import (
-    MongoIntegrationTransactionTestCase,
+    IntegrationTransactionTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import RequestMock
 
 user_fixture = UserFixtures()
 
 
-class TestUserDetail(MongoIntegrationTransactionTestCase):
+class TestUserDetail(IntegrationTransactionTestCase):
     """TestUserDetail"""
 
     def setUp(self):
         """setUp
 
         Returns:
```

### Comparing `core_main_app-2.2.1/tests/rest/user/tests_permissions.py` & `core_main_app-2.3.0/tests/rest/user/tests_permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 """
 from django.test import TestCase
 from rest_framework import status
 from tests.components.user.fixtures.fixtures import UserFixtures
 
 from core_main_app.rest.user import views as user_rest_views
 from core_main_app.utils.integration_tests.integration_base_transaction_test_case import (
-    MongoIntegrationTransactionTestCase,
+    IntegrationTransactionTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import RequestMock
 
 user_fixture = UserFixtures()
 
 
-class TestUserGetPermissions(MongoIntegrationTransactionTestCase):
+class TestUserGetPermissions(IntegrationTransactionTestCase):
     """TestUserGetPermissions"""
 
     def setUp(self):
         """setUp
 
         Returns:
```

### Comparing `core_main_app-2.2.1/tests/rest/user/tests_unit.py` & `core_main_app-2.3.0/tests/rest/user/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/rest/web_page/tests_permission.py` & `core_main_app-2.3.0/tests/rest/web_page/tests_permission.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/rest/workspace/tests_int.py` & `core_main_app-2.3.0/tests/rest/workspace/tests_int.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 from tests.components.group.fixtures.fixtures import GroupFixtures
 from tests.components.user.fixtures.fixtures import UserFixtures
 from tests.components.workspace.fixtures.fixtures import WorkspaceFixtures
 
 from core_main_app.components.workspace import api as workspace_api
 from core_main_app.rest.workspace import views as workspace_rest_views
 from core_main_app.utils.integration_tests.integration_base_transaction_test_case import (
-    MongoIntegrationTransactionTestCase,
+    IntegrationTransactionTestCase,
 )
 from core_main_app.utils.tests_tools.RequestMock import RequestMock
 
 TITLE_1 = "title 1"
 TITLE_2 = "title 2"
 TITLE_3 = "title 3"
 
 FAKE_WORKSPACE_ID = -1
 
 
-class TestWorkspaceDetail(MongoIntegrationTransactionTestCase):
+class TestWorkspaceDetail(IntegrationTransactionTestCase):
     """Test Workspace Detail"""
 
     def test_get_returns_http_200(self):
         """test_get_returns_http_200
 
         Returns:
 
@@ -166,15 +166,15 @@
             param={"pk": workspace.id},
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
 
 
-class TestWorkspaceList(MongoIntegrationTransactionTestCase):
+class TestWorkspaceList(IntegrationTransactionTestCase):
     """Test Workspace List"""
 
     def test_get_returns_http_200(self):
         """test_get_returns_http_200
 
         Returns:
 
@@ -314,15 +314,15 @@
             workspace_rest_views.WorkspaceList.as_view(), user, data=mock_data
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_400_BAD_REQUEST)
 
 
-class TestWorkspaceReadAccess(MongoIntegrationTransactionTestCase):
+class TestWorkspaceReadAccess(IntegrationTransactionTestCase):
     """Test Workspace Read Access"""
 
     def test_get_workspace_with_read_access_return_http_200(self):
         """test_get_workspace_with_read_access_return_http_200
 
         Returns:
 
@@ -413,15 +413,15 @@
             workspace_rest_views.get_workspaces_with_read_access, user2
         )
 
         # Assert
         self.assertEqual(response.data[0]["title"], TITLE_1)
 
 
-class TestWorkspaceWriteAccess(MongoIntegrationTransactionTestCase):
+class TestWorkspaceWriteAccess(IntegrationTransactionTestCase):
     """Test Workspace Write Access"""
 
     def test_get_workspace_with_write_access_return_http_200(self):
         """test_get_workspace_with_write_access_return_http_200
 
         Returns:
 
@@ -514,15 +514,15 @@
             workspace_rest_views.get_workspaces_with_write_access, user2
         )
 
         # Assert
         self.assertEqual(len(response.data), 0)
 
 
-class TestWorkspaceIsPublic(MongoIntegrationTransactionTestCase):
+class TestWorkspaceIsPublic(IntegrationTransactionTestCase):
     """Test Workspace Is Public"""
 
     def test_is_workspace_public_return_http_200(self):
         """test_is_workspace_public_return_http_200
 
         Returns:
 
@@ -599,15 +599,15 @@
             param={"pk": FAKE_WORKSPACE_ID},
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_404_NOT_FOUND)
 
 
-class TestWorkspaceSetPublic(MongoIntegrationTransactionTestCase):
+class TestWorkspaceSetPublic(IntegrationTransactionTestCase):
     """Test Workspace Set Public"""
 
     def test_set_workspace_public_return_http_200(self):
         """test_set_workspace_public_return_http_200
 
         Returns:
 
@@ -755,15 +755,15 @@
             param={"pk": workspace.id},
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
 
 
-class TestWorkspaceSetPrivate(MongoIntegrationTransactionTestCase):
+class TestWorkspaceSetPrivate(IntegrationTransactionTestCase):
     """Test Workspace Set Private"""
 
     def test_set_workspace_private_return_http_200(self):
         """test_set_workspace_private_return_http_200
 
         Returns:
 
@@ -894,15 +894,15 @@
             param={"pk": workspace.id},
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
 
 
-class TestWorkspaceListUserCanRead(MongoIntegrationTransactionTestCase):
+class TestWorkspaceListUserCanRead(IntegrationTransactionTestCase):
     """Test Workspace List User Can read"""
 
     def test_get_list_user_can_read_workspace_return_http_200(self):
         """test_get_list_user_can_read_workspace_return_http_200
 
         Returns:
 
@@ -1051,15 +1051,15 @@
 
         # Assert
         self.assertEqual(len(response.data), 1)
         self.assertEqual(response.data[0]["id"], user2.id)
         self.assertEqual(response.data[0]["username"], user2.username)
 
 
-class TestWorkspaceListUserCanWrite(MongoIntegrationTransactionTestCase):
+class TestWorkspaceListUserCanWrite(IntegrationTransactionTestCase):
     """Test Workspace List User Can Write"""
 
     def test_get_list_user_can_write_workspace_return_http_200(self):
         """test_get_list_user_can_write_workspace_return_http_200
 
         Returns:
 
@@ -1212,15 +1212,15 @@
 
         # Assert
         self.assertEqual(len(response.data), 1)
         self.assertEqual(response.data[0]["id"], user2.id)
         self.assertEqual(response.data[0]["username"], user2.username)
 
 
-class TestWorkspaceListGroupCanRead(MongoIntegrationTransactionTestCase):
+class TestWorkspaceListGroupCanRead(IntegrationTransactionTestCase):
     """Test Workspace List Group Can read"""
 
     def test_get_list_group_can_read_workspace_return_http_200(self):
         """test_get_list_group_can_read_workspace_return_http_200
 
         Returns:
 
@@ -1352,15 +1352,15 @@
 
         # Assert
         self.assertEqual(len(response.data), 1)
         self.assertEqual(response.data[0]["id"], group.id)
         self.assertEqual(response.data[0]["name"], group.name)
 
 
-class TestWorkspaceListGroupCanWrite(MongoIntegrationTransactionTestCase):
+class TestWorkspaceListGroupCanWrite(IntegrationTransactionTestCase):
     """Test Workspace List Group Can Write"""
 
     def test_get_list_group_can_write_workspace_return_http_200(self):
         """test_get_list_group_can_write_workspace_return_http_200
 
         Returns:
 
@@ -1492,15 +1492,15 @@
 
         # Assert
         self.assertEqual(len(response.data), 1)
         self.assertEqual(response.data[0]["id"], group.id)
         self.assertEqual(response.data[0]["name"], group.name)
 
 
-class TestAddUserReadRightToWorkspace(MongoIntegrationTransactionTestCase):
+class TestAddUserReadRightToWorkspace(IntegrationTransactionTestCase):
     """Test Add User Read Right To Workspace"""
 
     def test_add_user_read_right_to_workspace_return_http_200(self):
         """test_add_user_read_right_to_workspace_return_http_200
 
         Returns:
 
@@ -1591,15 +1591,15 @@
             len(
                 workspace_api.get_list_user_can_read_workspace(workspace, user)
             ),
             1,
         )
 
 
-class TestAddUserWriteRightToWorkspace(MongoIntegrationTransactionTestCase):
+class TestAddUserWriteRightToWorkspace(IntegrationTransactionTestCase):
     """Test Add User Write Right To Workspace"""
 
     def test_add_user_write_right_to_workspace_return_http_200(self):
         """test_add_user_write_right_to_workspace_return_http_200
 
         Returns:
 
@@ -1694,15 +1694,15 @@
                     workspace, user
                 )
             ),
             1,
         )
 
 
-class TestAddGroupReadRightToWorkspace(MongoIntegrationTransactionTestCase):
+class TestAddGroupReadRightToWorkspace(IntegrationTransactionTestCase):
     """Test Add Group Read Right To Workspace"""
 
     def test_add_group_read_right_to_workspace_return_http_200(self):
         """test_add_group_read_right_to_workspace_return_http_200
 
         Returns:
 
@@ -1798,15 +1798,15 @@
                     workspace, user
                 )
             ),
             1,
         )
 
 
-class TestAddGroupWriteRightToWorkspace(MongoIntegrationTransactionTestCase):
+class TestAddGroupWriteRightToWorkspace(IntegrationTransactionTestCase):
     """Test Add Group Write Right To Workspace"""
 
     def test_add_group_write_right_to_workspace_return_http_200(self):
         """test_add_group_write_right_to_workspace_return_http_200
 
         Returns:
 
@@ -1903,15 +1903,15 @@
                     workspace, user
                 )
             ),
             1,
         )
 
 
-class TestRemoveUserReadRightToWorkspace(MongoIntegrationTransactionTestCase):
+class TestRemoveUserReadRightToWorkspace(IntegrationTransactionTestCase):
     """Test Remove User Read Right To Workspace"""
 
     def test_remove_user_read_right_to_workspace_return_http_200(self):
         """test_remove_user_read_right_to_workspace_return_http_200
 
         Returns:
 
@@ -2003,15 +2003,15 @@
             len(
                 workspace_api.get_list_user_can_read_workspace(workspace, user)
             ),
             0,
         )
 
 
-class TestRemoveUserWriteRightToWorkspace(MongoIntegrationTransactionTestCase):
+class TestRemoveUserWriteRightToWorkspace(IntegrationTransactionTestCase):
     """Test Remove User Write Right To Workspace"""
 
     def test_remove_user_write_right_to_workspace_return_http_200(self):
         """test_remove_user_write_right_to_workspace_return_http_200
 
         Returns:
 
@@ -2109,15 +2109,15 @@
                     workspace, user
                 )
             ),
             0,
         )
 
 
-class TestRemoveGroupReadRightToWorkspace(MongoIntegrationTransactionTestCase):
+class TestRemoveGroupReadRightToWorkspace(IntegrationTransactionTestCase):
     """Test Remove Group Read Right To Workspace"""
 
     def test_remove_group_read_right_to_workspace_return_http_200(self):
         """test_remove_group_read_right_to_workspace_return_http_200
 
         Returns:
 
@@ -2216,17 +2216,15 @@
                     workspace, user
                 )
             ),
             0,
         )
 
 
-class TestRemoveGroupWriteRightToWorkspace(
-    MongoIntegrationTransactionTestCase
-):
+class TestRemoveGroupWriteRightToWorkspace(IntegrationTransactionTestCase):
     """Test Remove Group Write Right To Workspace"""
 
     def test_remove_group_write_right_to_workspace_return_http_200(self):
         """test_remove_group_write_right_to_workspace_return_http_200
 
         Returns:
```

### Comparing `core_main_app-2.2.1/tests/rest/workspace/tests_permissions.py` & `core_main_app-2.3.0/tests/rest/workspace/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/rest/xsl_transformation/fixtures/fixtures.py` & `core_main_app-2.3.0/tests/rest/xsl_transformation/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/rest/xsl_transformation/tests_int.py` & `core_main_app-2.3.0/tests/rest/xsl_transformation/tests_int.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 from rest_framework import status
 from tests.rest.xsl_transformation.fixtures.fixtures import (
     XslTransformationFixtures,
 )
 
 from core_main_app.rest.xsl_transformation import views as xsl_views
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.utils.tests_tools.RequestMock import RequestMock
 
 fixture_data = XslTransformationFixtures()
 
 
-class TestGetAllXslTransformationList(MongoIntegrationBaseTestCase):
+class TestGetAllXslTransformationList(IntegrationBaseTestCase):
     """TestGetAllXslTransformationList"""
 
     fixture = fixture_data
 
     def setUp(self):
         """setUp
 
@@ -43,15 +43,15 @@
             xsl_views.XslTransformationList.as_view(), user
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_403_FORBIDDEN)
 
 
-class TestPostXslTransformationList(MongoIntegrationBaseTestCase):
+class TestPostXslTransformationList(IntegrationBaseTestCase):
     """TestPostXslTransformationList"""
 
     fixture = fixture_data
 
     def setUp(self):
         """setUp
 
@@ -118,15 +118,15 @@
             xsl_views.XslTransformationList.as_view(), user, self.data
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_201_CREATED)
 
 
-class TestGetXslTransformationDetail(MongoIntegrationBaseTestCase):
+class TestGetXslTransformationDetail(IntegrationBaseTestCase):
     """TestGetXslTransformationDetail"""
 
     fixture = fixture_data
 
     def setUp(self):
         """setUp
 
@@ -198,15 +198,15 @@
 
         # Assert
         self.assertEqual(
             response.status_code, status.HTTP_500_INTERNAL_SERVER_ERROR
         )
 
 
-class TestDeleteXslTransformationDetail(MongoIntegrationBaseTestCase):
+class TestDeleteXslTransformationDetail(IntegrationBaseTestCase):
     """TestDeleteXslTransformationDetail"""
 
     fixture = fixture_data
 
     def setUp(self):
         """setUp
 
@@ -299,15 +299,15 @@
             self.param,
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_204_NO_CONTENT)
 
 
-class TestPatchXslTransformationDetail(MongoIntegrationBaseTestCase):
+class TestPatchXslTransformationDetail(IntegrationBaseTestCase):
     """TestPatchXslTransformationDetail"""
 
     fixture = fixture_data
 
     def setUp(self):
         """setUp
 
@@ -400,15 +400,15 @@
             self.param,
         )
 
         # Assert
         self.assertEqual(response.status_code, status.HTTP_200_OK)
 
 
-class TestPostXslTransformationTransform(MongoIntegrationBaseTestCase):
+class TestPostXslTransformationTransform(IntegrationBaseTestCase):
     """TestPostXslTransformationTransform"""
 
     fixture = fixture_data
 
     def setUp(self):
         """setUp
```

### Comparing `core_main_app-2.2.1/tests/rest/xsl_transformation/tests_permission.py` & `core_main_app-2.3.0/tests/rest/xsl_transformation/tests_permission.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/rest/xsl_transformation/tests_unit.py` & `core_main_app-2.3.0/tests/rest/xsl_transformation/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/rest_urls.py` & `core_main_app-2.3.0/tests/rest_urls.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/system/test_unit.py` & `core_main_app-2.3.0/tests/system/test_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/templatetags/test_get_attribute.py` & `core_main_app-2.3.0/tests/templatetags/test_get_attribute.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/test_settings.py` & `core_main_app-2.3.0/tests/test_settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     "django.contrib.staticfiles",
     # Extra apps
     "defender",
     "tz_detect",
     "menu",
     # Local apps
     "core_main_app",
+    "core_parser_app",
     "tests",
 ]
 
 # SERVER URI
 SERVER_URI = "http://127.0.0.1:8000"
 
 # TEST DATABASE
@@ -99,7 +100,8 @@
 ENABLE_SAML2_SSO_AUTH = False
 VERIFY_DATA_ACCESS = False
 
 USE_TZ = True
 CHECKSUM_ALGORITHM = "MD5"
 MONGODB_INDEXING = False
 MONGODB_ASYNC_SAVE = False
+DJANGO_SIMPLE_HISTORY_MODELS = []
```

### Comparing `core_main_app-2.2.1/tests/urls.py` & `core_main_app-2.3.0/tests/urls.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/utils/checksum/tests_checksum.py` & `core_main_app-2.3.0/tests/utils/checksum/tests_checksum.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/utils/migrations/tests_unit.py` & `core_main_app-2.3.0/tests/utils/migrations/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/utils/query/mongo/tests_unit.py` & `core_main_app-2.3.0/tests/utils/query/mongo/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/utils/requests_utls/tests_ssl.py` & `core_main_app-2.3.0/tests/utils/requests_utls/tests_ssl.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/utils/tests_int_blob_downloader.py` & `core_main_app-2.3.0/tests/utils/tests_int_blob_downloader.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/utils/tests_int_file.py` & `core_main_app-2.3.0/tests/utils/tests_int_file.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/utils/tests_unit_boolean.py` & `core_main_app-2.3.0/tests/utils/tests_unit_boolean.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/utils/tests_unit_xml_operation.py` & `core_main_app-2.3.0/tests/utils/tests_unit_xml_operation.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/utils/tests_view_data.py` & `core_main_app-2.3.0/tests/utils/tests_view_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     _get_field,
     xslt_selector,
 )
 from tests.components.template_xsl_rendering.fixtures.fixtures import (
     TemplateXslRenderingFixtures,
 )
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 
 fixture_template_rendering = TemplateXslRenderingFixtures()
 
 
 class TestGetField(TestCase):
     """Test _get_field"""
@@ -98,15 +98,15 @@
         data = {"title": self.title}
         # Act
         data_title = _get_field(data, "bad")
         # Assert
         self.assertEqual(data_title, None)
 
 
-class TestXsltSelector(MongoIntegrationBaseTestCase):
+class TestXsltSelector(IntegrationBaseTestCase):
     """Test raw_xml_to_dict"""
 
     fixture = fixture_template_rendering
 
     def test_xslt_selector_returns_default_config_when_template_xsl_rendering_is_not_set(
         self,
     ):
```

### Comparing `core_main_app-2.2.1/tests/utils/xsd_flattener/tests_unit.py` & `core_main_app-2.3.0/tests/utils/xsd_flattener/tests_unit.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/views/fixtures.py` & `core_main_app-2.3.0/tests/views/fixtures.py`

 * *Files identical despite different names*

### Comparing `core_main_app-2.2.1/tests/views/tests_int_access_control.py` & `core_main_app-2.3.0/tests/views/tests_int_access_control.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from django.test import RequestFactory
 from tests.views.fixtures import AccessControlDataFixture
 
 from core_main_app.components.blob import api as blob_api
 from core_main_app.components.data import api as data_api
 from core_main_app.settings import MAX_DOCUMENT_EDITING_SIZE
 from core_main_app.utils.integration_tests.integration_base_test_case import (
-    MongoIntegrationBaseTestCase,
+    IntegrationBaseTestCase,
 )
 from core_main_app.utils.tests_tools.MockUser import create_mock_user
 from core_main_app.views.common.views import (
     ViewData,
     EditWorkspaceRights,
     TemplateXSLRenderingView,
     DataContentEditor,
@@ -33,15 +33,15 @@
     load_add_group_form,
     add_group_right_to_workspace,
 )
 from core_main_app.views.user.views import manage_template_versions
 from tests.test_settings import LOGIN_URL
 
 
-class TestViewData(MongoIntegrationBaseTestCase):
+class TestViewData(IntegrationBaseTestCase):
     """TestViewData"""
 
     def setUp(self):
         """setUp
 
         Returns:
 
@@ -113,15 +113,15 @@
         self.assertTrue(
             self.fixture.data_public_workspace.title
             not in response.content.decode()
         )
         self.assertTrue("Error" in response.content.decode())
 
 
-class TestManageTemplateVersions(MongoIntegrationBaseTestCase):
+class TestManageTemplateVersions(IntegrationBaseTestCase):
     """TestManageTemplateVersions"""
 
     def setUp(self):
         """setUp
 
         Returns:
 
@@ -141,15 +141,15 @@
         request = self.factory.get("core_main_app_manage_template_versions")
         request.user = self.anonymous
         response = manage_template_versions(request)
         self.assertEqual(response.status_code, 302)
         self.assertTrue(response.url.startswith(LOGIN_URL))
 
 
-class TestTemplateXSLRenderingView(MongoIntegrationBaseTestCase):
+class TestTemplateXSLRenderingView(IntegrationBaseTestCase):
     """TestTemplateXSLRenderingView"""
 
     def setUp(self):
         """setUp
 
         Returns:
 
@@ -169,15 +169,15 @@
         request = self.factory.get("core_main_app_template_xslt")
         request.user = self.anonymous
         response = TemplateXSLRenderingView.as_view()(request)
         self.assertEqual(response.status_code, 302)
         self.assertTrue(response.url.startswith(LOGIN_URL))
 
 
-class TestAssignDataView(MongoIntegrationBaseTestCase):
+class TestAssignDataView(IntegrationBaseTestCase):
     """TestAssignDataView"""
 
     def setUp(self):
         """setUp
 
         Returns:
 
@@ -248,15 +248,15 @@
         request = self.factory.post("core_main_assign_data_workspace", data)
         request.user = self.anonymous
         response = AssignView.as_view(api=data_api)(request)
         self.assertEqual(response.status_code, 302)
         self.assertTrue(response.url.startswith(LOGIN_URL))
 
 
-class TestAssignBlobView(MongoIntegrationBaseTestCase):
+class TestAssignBlobView(IntegrationBaseTestCase):
     """TestAssignBlobView"""
 
     def setUp(self):
         """setUp
 
         Returns:
 
@@ -327,15 +327,15 @@
         request = self.factory.post("core_main_assign_blob_workspace", data)
         request.user = self.anonymous
         response = AssignView.as_view(api=blob_api)(request)
         self.assertEqual(response.status_code, 302)
         self.assertTrue(response.url.startswith(LOGIN_URL))
 
 
-class TestChangeDataDisplayView(MongoIntegrationBaseTestCase):
+class TestChangeDataDisplayView(IntegrationBaseTestCase):
     """TestChangeDataDisplayView"""
 
     def setUp(self):
         """setUp
 
         Returns:
 
@@ -430,15 +430,15 @@
         }
         request = self.factory.post("core_main_add_change_data_display", data)
         request.user = self.anonymous
         response = change_data_display(request)
         self.assertEqual(response.status_code, 403)
 
 
-class TestEditRights(MongoIntegrationBaseTestCase):
+class TestEditRights(IntegrationBaseTestCase):
     """TestEditRights"""
 
     def setUp(self):
         """setUp
 
         Returns:
 
@@ -458,15 +458,15 @@
         request = self.factory.post("core_main_edit_rights_workspace")
         request.user = self.anonymous
         response = EditWorkspaceRights.as_view()(request)
         self.assertEqual(response.status_code, 302)
         self.assertTrue(response.url.startswith(LOGIN_URL))
 
 
-class TestLoadFormChangeWorkspace(MongoIntegrationBaseTestCase):
+class TestLoadFormChangeWorkspace(IntegrationBaseTestCase):
     """TestLoadFormChangeWorkspace"""
 
     def setUp(self):
         """setUp
 
         Returns:
 
@@ -487,15 +487,15 @@
         request = self.factory.post("core_main_change_workspace", data)
         request.user = self.anonymous
         response = LoadFormChangeWorkspace.as_view()(request)
         self.assertEqual(response.status_code, 302)
         self.assertTrue(response.url.startswith(LOGIN_URL))
 
 
-class TestLoadAddUserForm(MongoIntegrationBaseTestCase):
+class TestLoadAddUserForm(IntegrationBaseTestCase):
     """TestLoadAddUserForm"""
 
     def setUp(self):
         """setUp
 
         Returns:
 
@@ -515,15 +515,15 @@
         request = self.factory.post("core_main_edit_rights_users_form")
         request.user = self.anonymous
         response = load_add_user_form(request)
         self.assertEqual(response.status_code, 302)
         self.assertTrue(response.url.startswith(LOGIN_URL))
 
 
-class TestAddUserToWorkspace(MongoIntegrationBaseTestCase):
+class TestAddUserToWorkspace(IntegrationBaseTestCase):
     """TestAddUserToWorkspace"""
 
     def setUp(self):
         """setUp
 
         Returns:
 
@@ -543,15 +543,15 @@
         request = self.factory.post("core_main_add_user_right_to_workspace")
         request.user = self.anonymous
         response = add_user_right_to_workspace(request)
         self.assertEqual(response.status_code, 302)
         self.assertTrue(response.url.startswith(LOGIN_URL))
 
 
-class TestSwitchRight(MongoIntegrationBaseTestCase):
+class TestSwitchRight(IntegrationBaseTestCase):
     """TestSwitchRight"""
 
     def setUp(self):
         """setUp
 
         Returns:
 
@@ -571,15 +571,15 @@
         request = self.factory.post("core_main_switch_right")
         request.user = self.anonymous
         response = switch_right(request)
         self.assertEqual(response.status_code, 302)
         self.assertTrue(response.url.startswith(LOGIN_URL))
 
 
-class TestRemoveRights(MongoIntegrationBaseTestCase):
+class TestRemoveRights(IntegrationBaseTestCase):
     """TestRemoveRights"""
 
     def setUp(self):
         """setUp
 
         Returns:
 
@@ -599,15 +599,15 @@
         request = self.factory.post("core_main_remove_rights")
         request.user = self.anonymous
         response = remove_user_or_group_rights(request)
         self.assertEqual(response.status_code, 302)
         self.assertTrue(response.url.startswith(LOGIN_URL))
 
 
-class TestAddGroupForm(MongoIntegrationBaseTestCase):
+class TestAddGroupForm(IntegrationBaseTestCase):
     """TestAddGroupForm"""
 
     def setUp(self):
         """setUp
 
         Returns:
 
@@ -627,15 +627,15 @@
         request = self.factory.post("core_main_edit_rights_groups_form")
         request.user = self.anonymous
         response = load_add_group_form(request)
         self.assertEqual(response.status_code, 302)
         self.assertTrue(response.url.startswith(LOGIN_URL))
 
 
-class TestAddGroupRightToWorkspace(MongoIntegrationBaseTestCase):
+class TestAddGroupRightToWorkspace(IntegrationBaseTestCase):
     """TestAddGroupRightToWorkspace"""
 
     def setUp(self):
         """setUp
 
         Returns:
 
@@ -655,15 +655,15 @@
         request = self.factory.post("core_main_add_group_right_to_workspace")
         request.user = self.anonymous
         response = add_group_right_to_workspace(request)
         self.assertEqual(response.status_code, 302)
         self.assertTrue(response.url.startswith(LOGIN_URL))
 
 
-class TestAbstractEditorView(MongoIntegrationBaseTestCase):
+class TestAbstractEditorView(IntegrationBaseTestCase):
     """Test Get XML Text Editor View"""
 
     def setUp(self):
 
         """setUp
 
         Returns:
@@ -699,15 +699,15 @@
 
         """
         # Assert
         with self.assertRaises(NotImplementedError):
             AbstractEditorView.save(self)
 
 
-class TestDataContentEditorView(MongoIntegrationBaseTestCase):
+class TestDataContentEditorView(IntegrationBaseTestCase):
     """Test Post Data Content Editor View"""
 
     def setUp(self):
         """setUp
 
         Returns:
 
@@ -930,15 +930,15 @@
         request.user = self.user1
         response = DataContentEditor.as_view()(request)
         self.assertTrue(
             "MAX_DOCUMENT_EDITING_SIZE" in response.content.decode()
         )
 
 
-class TestXSDTextEditorView(MongoIntegrationBaseTestCase):
+class TestXSDTextEditorView(IntegrationBaseTestCase):
     """Test Post XSD Text Editor View"""
 
     def setUp(self):
         """setUp
 
         Returns:
```

