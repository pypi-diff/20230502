# Comparing `tmp/aa_package_monitor-1.9.1.tar.gz` & `tmp/aa_package_monitor-1.9.2.tar.gz`

## Comparing `aa_package_monitor-1.9.1.tar` & `aa_package_monitor-1.9.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/__init__.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/app_settings.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/apps.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/auth_hooks.py
--rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/managers.py
--rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/models.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/tasks.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/urls.py
--rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/core/__init__.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/core/distribution_packages.py
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/core/metadata_helpers.py
--rw-r--r--   0        0        0     5159 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/core/pypi.py
--rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/django.pot
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3648 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/management/commands/package_monitor_refresh.py
--rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/migrations/0001_initial.py
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/migrations/0002_add_editable_and_refactor_json_fields.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/migrations/0003_add_update_notifications.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/migrations/__init__.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/static/package_monitor/css/global.css
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/static/package_monitor/css/package_list.css
--rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/static/package_monitor/images/Spinner-1s-64px-dark.gif
--rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/static/package_monitor/images/Spinner-1s-64px-light.gif
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/templates/package_monitor/base.html
--rw-r--r--   0        0        0    10198 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/templates/package_monitor/index.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/tests/__init__.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/tests/test_commands.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/tests/test_integration.py
--rw-r--r--   0        0        0    18043 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/tests/test_managers.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/tests/test_models.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/tests/test_tasks.py
--rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/tests/test_views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/tests/core/__init__.py
--rw-r--r--   0        0        0     6580 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/tests/core/test_distribution_packages.py
--rw-r--r--   0        0        0     6874 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/tests/core/test_metadata_helpers.py
--rw-r--r--   0        0        0     7417 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/tests/core/test_pypi.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/tests/factories/__init__.py
--rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/tests/factories/factories.py
--rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/tests/factories/stubs.py
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/tests/factories/tests.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/LICENSE
--rw-r--r--   0        0        0     8873 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/README.md
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/pyproject.toml
--rw-r--r--   0        0        0    10223 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/PKG-INFO
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/__init__.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/app_settings.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/apps.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/auth_hooks.py
+-rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/managers.py
+-rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/models.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/tasks.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/urls.py
+-rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/core/__init__.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/core/distribution_packages.py
+-rw-r--r--   0        0        0     3060 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/core/metadata_helpers.py
+-rw-r--r--   0        0        0     5159 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/core/pypi.py
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/locale/django.pot
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3648 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/management/commands/package_monitor_refresh.py
+-rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/migrations/0002_add_editable_and_refactor_json_fields.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/migrations/0003_add_update_notifications.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/migrations/__init__.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/static/package_monitor/css/global.css
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/static/package_monitor/css/package_list.css
+-rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/static/package_monitor/images/Spinner-1s-64px-dark.gif
+-rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/static/package_monitor/images/Spinner-1s-64px-light.gif
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/templates/package_monitor/base.html
+-rw-r--r--   0        0        0    10198 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/templates/package_monitor/index.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/tests/__init__.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/tests/test_commands.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/tests/test_integration.py
+-rw-r--r--   0        0        0    18043 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/tests/test_managers.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/tests/test_models.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/tests/test_tasks.py
+-rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/tests/test_views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/tests/core/__init__.py
+-rw-r--r--   0        0        0     6580 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/tests/core/test_distribution_packages.py
+-rw-r--r--   0        0        0     7313 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/tests/core/test_metadata_helpers.py
+-rw-r--r--   0        0        0     7417 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/tests/core/test_pypi.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/tests/factories/__init__.py
+-rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/tests/factories/factories.py
+-rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/tests/factories/stubs.py
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/package_monitor/tests/factories/tests.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/LICENSE
+-rw-r--r--   0        0        0     8873 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/README.md
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/pyproject.toml
+-rw-r--r--   0        0        0    10223 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.2/PKG-INFO
```

### Comparing `aa_package_monitor-1.9.1/package_monitor/app_settings.py` & `aa_package_monitor-1.9.2/package_monitor/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/auth_hooks.py` & `aa_package_monitor-1.9.2/package_monitor/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/managers.py` & `aa_package_monitor-1.9.2/package_monitor/managers.py`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/models.py` & `aa_package_monitor-1.9.2/package_monitor/models.py`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/views.py` & `aa_package_monitor-1.9.2/package_monitor/views.py`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/core/distribution_packages.py` & `aa_package_monitor-1.9.2/package_monitor/core/distribution_packages.py`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/core/metadata_helpers.py` & `aa_package_monitor-1.9.2/package_monitor/core/metadata_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         return []
     found_apps = []
     for dist_file in _extract_files(dist, pattern="__init__.py"):
         for app in django_apps.get_app_configs():
             if not app.module:
                 continue
             my_file = app.module.__file__
-            if my_file.endswith(dist_file):
+            if my_file and my_file.endswith(dist_file):
                 found_apps.append(app.name)
                 break
     return found_apps
 
 
 def _extract_files(dist: Optional[MetadataDistribution], pattern: str) -> List[str]:
     """Extract file paths from a distribution which filename match a pattern."""
```

### Comparing `aa_package_monitor-1.9.1/package_monitor/core/pypi.py` & `aa_package_monitor-1.9.2/package_monitor/core/pypi.py`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/locale/django.pot` & `aa_package_monitor-1.9.2/package_monitor/locale/django.pot`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/locale/de/LC_MESSAGES/django.po` & `aa_package_monitor-1.9.2/package_monitor/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/locale/en/LC_MESSAGES/django.po` & `aa_package_monitor-1.9.2/package_monitor/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/locale/es/LC_MESSAGES/django.po` & `aa_package_monitor-1.9.2/package_monitor/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/locale/fr_FR/LC_MESSAGES/django.po` & `aa_package_monitor-1.9.2/package_monitor/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/locale/it_IT/LC_MESSAGES/django.po` & `aa_package_monitor-1.9.2/package_monitor/locale/it_IT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/locale/ja/LC_MESSAGES/django.po` & `aa_package_monitor-1.9.2/package_monitor/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/locale/ko_KR/LC_MESSAGES/django.po` & `aa_package_monitor-1.9.2/package_monitor/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/locale/ru/LC_MESSAGES/django.mo` & `aa_package_monitor-1.9.2/package_monitor/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/locale/ru/LC_MESSAGES/django.po` & `aa_package_monitor-1.9.2/package_monitor/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/locale/uk/LC_MESSAGES/django.mo` & `aa_package_monitor-1.9.2/package_monitor/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/locale/uk/LC_MESSAGES/django.po` & `aa_package_monitor-1.9.2/package_monitor/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_package_monitor-1.9.2/package_monitor/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/management/commands/package_monitor_refresh.py` & `aa_package_monitor-1.9.2/package_monitor/management/commands/package_monitor_refresh.py`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/migrations/0001_initial.py` & `aa_package_monitor-1.9.2/package_monitor/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/migrations/0002_add_editable_and_refactor_json_fields.py` & `aa_package_monitor-1.9.2/package_monitor/migrations/0002_add_editable_and_refactor_json_fields.py`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/migrations/0003_add_update_notifications.py` & `aa_package_monitor-1.9.2/package_monitor/migrations/0003_add_update_notifications.py`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/static/package_monitor/css/global.css` & `aa_package_monitor-1.9.2/package_monitor/static/package_monitor/css/global.css`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/static/package_monitor/css/package_list.css` & `aa_package_monitor-1.9.2/package_monitor/static/package_monitor/css/package_list.css`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/static/package_monitor/images/Spinner-1s-64px-dark.gif` & `aa_package_monitor-1.9.2/package_monitor/static/package_monitor/images/Spinner-1s-64px-dark.gif`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/static/package_monitor/images/Spinner-1s-64px-light.gif` & `aa_package_monitor-1.9.2/package_monitor/static/package_monitor/images/Spinner-1s-64px-light.gif`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/templates/package_monitor/index.html` & `aa_package_monitor-1.9.2/package_monitor/templates/package_monitor/index.html`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/tests/test_commands.py` & `aa_package_monitor-1.9.2/package_monitor/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/tests/test_integration.py` & `aa_package_monitor-1.9.2/package_monitor/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/tests/test_managers.py` & `aa_package_monitor-1.9.2/package_monitor/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/tests/test_models.py` & `aa_package_monitor-1.9.2/package_monitor/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/tests/test_views.py` & `aa_package_monitor-1.9.2/package_monitor/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/tests/core/test_distribution_packages.py` & `aa_package_monitor-1.9.2/package_monitor/tests/core/test_distribution_packages.py`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/tests/core/test_metadata_helpers.py` & `aa_package_monitor-1.9.2/package_monitor/tests/core/test_metadata_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,26 @@
         dist = MetadataDistributionStubFactory(files=["alpha/apps.py"])
         mock_django_apps.get_app_configs.return_value = []
         # when
         result = identify_installed_django_apps(dist)
         # then
         self.assertListEqual(result, [])
 
+    def test_should_handle_no_module_file(self, mock_django_apps):
+        # given
+        dist = MetadataDistributionStubFactory(
+            files=["alpha/__init__.py", "alpha/apps.py"]
+        )
+        app = DjangoAppConfigStub("alpha_app", None)
+        mock_django_apps.get_app_configs.return_value = [app]
+        # when
+        result = identify_installed_django_apps(dist)
+        # then
+        self.assertListEqual(result, [])
+
 
 class TestParseRequirements(NoSocketsTestCase):
     def test_should_parse_requirements_correctly(self):
         # given
         dist = MetadataDistributionStubFactory(requires=["bravo>=1.0.0", "alpha<5"])
 
         # when
```

### Comparing `aa_package_monitor-1.9.1/package_monitor/tests/core/test_pypi.py` & `aa_package_monitor-1.9.2/package_monitor/tests/core/test_pypi.py`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/tests/factories/factories.py` & `aa_package_monitor-1.9.2/package_monitor/tests/factories/factories.py`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/tests/factories/stubs.py` & `aa_package_monitor-1.9.2/package_monitor/tests/factories/stubs.py`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/package_monitor/tests/factories/tests.py` & `aa_package_monitor-1.9.2/package_monitor/tests/factories/tests.py`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/LICENSE` & `aa_package_monitor-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/README.md` & `aa_package_monitor-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/pyproject.toml` & `aa_package_monitor-1.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.1/PKG-INFO` & `aa_package_monitor-1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-package-monitor
-Version: 1.9.1
+Version: 1.9.2
 Summary: An app that helps keep track of installed packages and outstanding updates for Alliance Auth
 Project-URL: Homepage, https://gitlab.com/ErikKalkoken/aa-package-monitor
 Project-URL: Source, https://gitlab.com/ErikKalkoken/aa-package-monitor
 Project-URL: Changelog, https://gitlab.com/ErikKalkoken/aa-package-monitor/-/blob/master/CHANGELOG.md
 Project-URL: Tracker, https://gitlab.com/ErikKalkoken/aa-package-monitor/-/issues
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>
 License-Expression: MIT
```

