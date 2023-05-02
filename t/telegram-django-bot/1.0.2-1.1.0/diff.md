# Comparing `tmp/telegram_django_bot-1.0.2.tar.gz` & `tmp/telegram_django_bot-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_django_bot-1.0.2.tar", last modified: Sat Apr 15 18:53:52 2023, max compression
+gzip compressed data, was "telegram_django_bot-1.1.0.tar", last modified: Tue May  2 13:56:29 2023, max compression
```

## Comparing `telegram_django_bot-1.0.2.tar` & `telegram_django_bot-1.1.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:53:52.743677 telegram_django_bot-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    40864 2023-04-15 18:53:52.743677 telegram_django_bot-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    39644 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-15 18:53:52.747677 telegram_django_bot-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:53:52.739677 telegram_django_bot-1.0.2/telegram_django_bot/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/admin_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:53:52.735677 telegram_django_bot-1.0.2/telegram_django_bot/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:53:52.735677 telegram_django_bot-1.0.2/telegram_django_bot/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:53:52.743677 telegram_django_bot-1.0.2/telegram_django_bot/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:53:52.743677 telegram_django_bot-1.0.2/telegram_django_bot/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/migrations/0002_delete_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/migrations/0003_botmenuelem_message_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/migrations/0004_auto_20220915_0448.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/migrations/0005_auto_20221010_1330.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/migrations/0006_auto_20221023_0157.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/migrations/0007_auto_20221202_0305.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/migrations/0008_auto_20221225_1050.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14827 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/routing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)    30066 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/td_viewset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/telegram_lib_redefinition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:53:52.743677 telegram_django_bot-1.0.2/telegram_django_bot/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/templates/dropdown_filter1.html
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12334 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/tg_dj_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/user_viewset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12160 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:53:52.739677 telegram_django_bot-1.0.2/telegram_django_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40864 2023-04-15 18:53:52.000000 telegram_django_bot-1.0.2/telegram_django_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-15 18:53:52.000000 telegram_django_bot-1.0.2/telegram_django_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 18:53:52.000000 telegram_django_bot-1.0.2/telegram_django_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-15 18:53:52.000000 telegram_django_bot-1.0.2/telegram_django_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-15 18:53:52.000000 telegram_django_bot-1.0.2/telegram_django_bot.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:53:52.743677 telegram_django_bot-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/tests/test_bme.py
--rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/tests/test_routing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/tests/test_td_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/tests/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    31352 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/tests/test_viewset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:56:29.490433 telegram_django_bot-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    40827 2023-05-02 13:56:29.490433 telegram_django_bot-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    39621 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-02 13:56:29.490433 telegram_django_bot-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:56:29.486433 telegram_django_bot-1.1.0/telegram_django_bot/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/telegram_django_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/telegram_django_bot/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/telegram_django_bot/admin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/telegram_django_bot/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/telegram_django_bot/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:56:29.482433 telegram_django_bot-1.1.0/telegram_django_bot/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:56:29.482433 telegram_django_bot-1.1.0/telegram_django_bot/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:56:29.486433 telegram_django_bot-1.1.0/telegram_django_bot/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/telegram_django_bot/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/telegram_django_bot/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:56:29.490433 telegram_django_bot-1.1.0/telegram_django_bot/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/telegram_django_bot/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/telegram_django_bot/migrations/0002_delete_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/telegram_django_bot/migrations/0003_botmenuelem_message_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/telegram_django_bot/migrations/0004_auto_20220915_0448.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/telegram_django_bot/migrations/0005_auto_20221010_1330.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/telegram_django_bot/migrations/0006_auto_20221023_0157.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/telegram_django_bot/migrations/0007_auto_20221202_0305.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/telegram_django_bot/migrations/0008_auto_20221225_1050.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/telegram_django_bot/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14827 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/telegram_django_bot/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/telegram_django_bot/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/telegram_django_bot/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/telegram_django_bot/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29635 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/telegram_django_bot/td_viewset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/telegram_django_bot/telegram_lib_redefinition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:56:29.490433 telegram_django_bot-1.1.0/telegram_django_bot/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/telegram_django_bot/templates/dropdown_filter1.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/telegram_django_bot/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12352 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/telegram_django_bot/tg_dj_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/telegram_django_bot/user_viewset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11862 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/telegram_django_bot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:56:29.486433 telegram_django_bot-1.1.0/telegram_django_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    40827 2023-05-02 13:56:29.000000 telegram_django_bot-1.1.0/telegram_django_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-02 13:56:29.000000 telegram_django_bot-1.1.0/telegram_django_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 13:56:29.000000 telegram_django_bot-1.1.0/telegram_django_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-02 13:56:29.000000 telegram_django_bot-1.1.0/telegram_django_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-02 13:56:29.000000 telegram_django_bot-1.1.0/telegram_django_bot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:56:29.490433 telegram_django_bot-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/tests/test_bme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/tests/test_routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/tests/test_td_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31361 2023-05-02 13:56:16.000000 telegram_django_bot-1.1.0/tests/test_viewset.py
```

### Comparing `telegram_django_bot-1.0.2/LICENSE` & `telegram_django_bot-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.2/PKG-INFO` & `telegram_django_bot-1.1.0/telegram_django_bot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: telegram_django_bot
-Version: 1.0.2
-Summary: Telegram Django Bot Bridge
-Home-page: https://github.com/alexanderaleskin/telegram_django_bot_bridge
+Name: telegram-django-bot
+Version: 1.1.0
+Summary: Telegram Django Bot
+Home-page: https://github.com/alexanderaleskin/telegram_django_bot
 Author: Alexander Aleskin
 Author-email: alexanderaleskin@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
@@ -25,20 +25,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Internet
 Requires-Python: >=3.8
 License-File: LICENSE
 
-Telegram Django Bot Bridge
+Telegram Django Bot
 ============================
 
 This library provides a Python high-level interface for creating Telegram Bots. It standardizes the coding in the best
 practice of the web development. The library is based on `Django <https://www.djangoproject.com/>`_ and `Python-Telegram-Bot <https://python-telegram-bot.org/>`_.
-and provides viewset interface for managing data with.
+It also provides viewset interface for managing data with.
 
 If you start a new project, you could use `Telegram django bot template <https://github.com/alexanderaleskin/telergam_django_bot_template>`_ with preconfigured settings.
 
 Install
 ------------
 
 You can install via ``pip``:
@@ -76,15 +76,15 @@
   Not necessary, but useful settings:
 
 * ``TELEGRAM_TOKEN`` - for adding "triggers",
 * ``TELEGRAM_TEST_USER_IDS`` - for adding tests for your bot,
 * Make sure, that ``LANGUAGE_CODE``, ``LANGUAGE_CODE``, ``USE_I18N`` are also used in the library for language localization.
 
 
-4. This step connects ``Telegram Django Bot Bridge`` with ``Python-Telegram-Bot``. Add ``RouterCallbackMessageCommandHandler`` in handlers for using TELEGRAM_ROOT_UTRLCONF :
+4. This step connects ``Telegram Django Bot`` with ``Python-Telegram-Bot``. Add ``RouterCallbackMessageCommandHandler`` in handlers for using TELEGRAM_ROOT_UTRLCONF :
 
 .. code-block:: python
 
     updater = Updater(bot=TG_DJ_Bot(settings.TELEGRAM_TOKEN))
     updater.dispatcher.add_handler(RouterCallbackMessageCommandHandler())
 
 or in 20.x version :
@@ -110,36 +110,30 @@
 
 and Django:
 
 * Django ORM  (communication with Database);
 * Administration panel for management.
 
 
-Telegram Django Bot Bridge provides next special opportunities:
+Telegram Django Bot provides next special opportunities:
 
 * using Viewsets (typical action with model (create, update, list, delete));
 * using Django localization.
 * using function routing like urls routing in Django.
-
-And some extra useful staff:
-
 * creating general menu items with no-coding (through Django Admin Panel);
-* extra high-level Bot functions, such as a wrapper for sending delayed (or scheduled) messages;
-* creating tests;
 * collecting stats from user actions in the bot;
-* commonly used utilities.
-
+* other useful staff.
 
 
 The key feature of the lib is ``TelegramViewSet`` - a class for managing Django ORM model. It is designed in a
 similar way as `Django rest framework Viewset <https://www.django-rest-framework.org/api-guide/viewsets/>`_ , but has
-a significant difference: while DRF Viewset provides a response in serializable format (usually in json format) to frontend app, TelegaViewSet
+a significant difference: while DRF Viewset provides a response in serializable format (usually in json format) to frontend app, TelegramViewSet
 provides a response to the user in telegram interface in message format with buttons. So, you will manage data and receive
-responses in human format by executing TelegaViewSet method. The methods use some kind of templates for generating human
-responses (it is possible to overwrite these templates). By default, TelegaViewSet has 5 methods:
+responses in human format by executing TelegramViewSet method. The methods use some kind of templates for generating human
+responses (it is possible to overwrite these templates). By default, TelegramViewSet has 5 methods:
 
 * ``create`` - create a new instance of the specified ORM model;
 * ``change`` - update instance fields of specified ORM model;
 * ``show_elem`` - show fields of the element and buttons with actions of this instance;
 * ``show_list`` - show list of model elements (with pagination);
 * ``delete`` - delete the instance
 
@@ -161,35 +155,35 @@
 
 .. code-block:: python
 
     from telegram_django_bot import forms as td_forms
     from telegram_django_bot.td_viewset import TelegramViewSet
 
 
-    class RequestForm(td_forms.TelegaModelForm):
+    class RequestForm(td_forms.TelegramModelForm):
         class Meta:
             model = Request
             fields = ['text', 'importance_level', 'project', 'tags']
 
 
     class RequestViewSet(TelegramViewSet):
-        telega_form = RequestForm
+        model_form = RequestForm
         queryset = Request.objects.all()
         viewset_name = 'Request'
 
 
 If you need, you can add extra actions to RequestViewSet for managing (see details information below) or change existing functions.
-There are several parameters and secondary functions in TelegaViewSet for customizing logic if it is necessary.
+There are several parameters and secondary functions in TelegramViewSet for customizing logic if it is necessary.
 
-In this example, ``TelegaModelForm`` was used. TelegaModelForm is a descendant of Django ModelForm. So, you could use
+In this example, ``TelegramModelForm`` was used. TelegramModelForm is a descendant of Django ModelForm. So, you could use
 labels, clean functions and other parameters and functions for managing logic and displaying.
 
 
-TelegaViewSet is designed to answer next user actions: clicking buttons and sometimes sending messages. The library imposes
-`Django URL notation <https://docs.djangoproject.com/en/4.1/topics/http/urls/>`_ for mapping user actions to TelegaViewSet methods (or usual handlers).
+TelegramViewSet is designed to answer next user actions: clicking buttons and sometimes sending messages. The library imposes
+`Django URL notation <https://docs.djangoproject.com/en/4.1/topics/http/urls/>`_ for mapping user actions to TelegramViewSet methods (or usual handlers).
 Usually, for correct mapping you just need to set ``TELEGRAM_ROOT_UTRLCONF`` and use ``RouterCallbackMessageCommandHandler`` in
 dispatcher as it is mentioned above in the *Install paragraph*.
 
 For correct mapping *RequestViewSet*  you should write in the TELEGRAM_ROOT_UTRLCONF file something like this:
 
 .. code-block:: python
 
@@ -266,15 +260,15 @@
          dp=updater.dispatcher
          dp.add_handler(RouterCallbackMessageCommandHandler())
 
 
 The example adds 1 super handler ``RouterCallbackMessageCommandHandler``, which allows you to write handlers
 in the style of handling link requests in the same way as it is done in ``Django``. ``RouterCallbackMessageCommandHandler`` allows you to handle
 messages, user commands and button clicks by users. In other words, it replaces the handlers
-``MessageHandler, CommandHandler, CallbackQueryHandler`` . Since the ``Telegram Django Bot Bridge`` library is an extension,
+``MessageHandler, CommandHandler, CallbackQueryHandler`` . Since the ``Telegram Django Bot`` library is an extension,
 it does not prohibit the use of standard handlers of the ``Python-Telegram-Bot`` library for handle user requests.
 (sometimes it is simply necessary, for example, if you need to process responses to surveys (you need to use PollAnswerHandler)).
 
 `Django notation <https://docs.djangoproject.com/en/4.1/topics/http/urls/>`_ of routing handlers is that paths to handlers are described in a separate file or files.
 As in the ``Django`` standard, the main file (root) for routing is specified in the project settings, where paths to handlers or paths to groups of handlers are stored.
 The ``TELEGRAM_ROOT_UTRLCONF`` (same as ``ROOT_URLCONF`` for WEB) attribute is used to specify the path to the file. In the example template, we have the following settings:
 
@@ -335,122 +329,122 @@
 This distribution of handlers allows you to group part of the handlers into modules and quickly connect or
 change them, while not being afraid of confusion which handlers need to be called, as it can be if all paths from
 different modules to handlers are described in one place as required by ``Python-Telegram-Bot``.
 
 In this example file ``base.utrls.py`` also ViewSets are used in addition to simple handler functions like ``def start`` and ``def some_debug_func``.
 ViewSet is an aggregator of several functions. The concept of it is that you quite often need to apply
 the same operations for a dataset, such as create, update, show, delete an example of dataset.
-There is the class ``telegram_django_bot.td_viewset.TelegaViewSet`` in the library  for such purposes. The class manages
-the Django ORM database model. ``TelegaViewSet`` has 5 functions for managing the model:
+There is the class ``telegram_django_bot.td_viewset.TelegramViewSet`` in the library  for such purposes. The class manages
+the Django ORM database model. ``TelegramViewSet`` has 5 functions for managing the model:
 
 
 ========= ======== ===========================
  Метод     UTRL      Description
 --------- -------- ---------------------------
 create     cr       Create model
 change     up       Change model attributes
 delete     de       Deleting a model
 show_elem  se       Display a model
 show_list  sl       Display a list of models
 ========= ======== ===========================
 
 Thus, if we want to call the ``BotMenuElemViewSet.create`` method to create an element, we need to use
 path 'sb/cr', whereby the first part of the path 'sb/'  the router ``RouterCallbackMessageCommandHandler`` will execute
-the ``BotMenuElemViewSet`` class, namely the ``TelegaViewSet.dispatch`` method, which in turn will call  the ``create`` method by analyzing the second part of the path
+the ``BotMenuElemViewSet`` class, namely the ``TelegramViewSet.dispatch`` method, which in turn will call  the ``create`` method by analyzing the second part of the path
 ``cr``.
 
 To sum up the scheme of handlers routing, there are following key points:
 
 1. ``telegram.ext.Update`` is used as a receiver of messages from Telegram;
-2. Standard handlers of the ``Python-Telegram-Bot`` library can be used as handlers. For convenient use Django's path scheme and ``TelegaViewSet`` you need to use ``RouterCallbackMessageCommandHandler``.
-3. ``TelegaViewSet`` aggregates a set of standard functions for managing data, what is made possible to group code associated with one type of data type in one class (place).
+2. Standard handlers of the ``Python-Telegram-Bot`` library can be used as handlers. For convenient use Django's path scheme and ``TelegramViewSet`` you need to use ``RouterCallbackMessageCommandHandler``.
+3. ``TelegramViewSet`` aggregates a set of standard functions for managing data, what is made possible to group code associated with one type of data type in one class (place).
 
 
 
 TelegramViewSet features
 ~~~~~~~~~~~~~~~~~~~~~~~~
 
-As described above, TelegaViewSet contains standard functions for data manipulation.
+As described above, TelegramViewSet contains standard functions for data manipulation.
 Due to such standard data processing methods, it turns out in the example to describe the logic of ``BotMenuElemViewSet`` in 40
 lines of code, also using some customization for beautiful data displaying.
 
 
-To use all the features of the TelegaViewSet in your class, it should be inherited from it, as, for example, this is done
+To use all the features of the TelegramViewSet in your class, it should be inherited from it, as, for example, this is done
 in the ``BotMenuElemViewSet``:
 
 
 .. code-block:: python
 
     from telegram_django_bot.td_viewset import TelegramViewSet
 
     class BotMenuElemViewSet(TelegramViewSet):
 
 
 In order to customize the ViewSet, you must specify 3 required attributes:
 
 1. ``viewset_name`` - class name, used to display to telegram users
-2. ``telega_form`` - data form, used to specify which fields of the ORM database model to use in the viewset;
+2. ``model_form`` - data form, used to specify which fields of the ORM database model to use in the viewset;
 3. ``queryset`` - basic query for getting model elements.
 
 
 The ``BotMenuElemViewSet`` is used the following values:
 
 .. code-block:: python
 
     from telegram_django_bot import forms as td_forms
     from telegram_django_bot.models import BotMenuElem
 
-    class BotMenuElemForm(td_forms.TelegaModelForm):
+    class BotMenuElemForm(td_forms.TelegramModelForm):
         form_name = _("Menu elem")
 
         class Meta:
             model = BotMenuElem
             fields = ['command', "is_visable", "callbacks_db", "message", "buttons_db"]
 
-    class BotMenuElemViewSet(TelegaViewSet):
+    class BotMenuElemViewSet(TelegramViewSet):
         viewset_name = 'BotMenuElem'
-        telega_form = BotMenuElemForm
+        model_form = BotMenuElemForm
         queryset = BotMenuElem.objects.all()
 
 
 where ``BotMenuElemForm`` is a descendant of the ``Django ModelFrom`` class, so it has a similar structure and parameterization methods.
 `` form_name ``  stands for the name of the form and is used in some messages sent to Telegram users.
 
 
-TelegaViewSet has quite a lot in common with Viewset analogs tailored for WEB development (for example,
-`django-rest-framework viewsets <https://www.django-rest-framework.org/api-guide/viewsets/>`_ ). However, as part of the development of Telegram bots, TelegaViewSet
+TelegramViewSet has quite a lot in common with Viewset analogs tailored for WEB development (for example,
+`django-rest-framework viewsets <https://www.django-rest-framework.org/api-guide/viewsets/>`_ ). However, as part of the development of Telegram bots, TelegramViewSet
 has some special features:
 
 1. An unusual way to create elements;
 2. The display of information in bots is limited and most often comes down to displaying text and buttons, so the viewset in addition to business logic includes the creation of standard responses to user actions in the form of messages with buttons.
 
 
 
 Forms
 ************
 
 
 Since Telegram does not have the ability to create forms (in the classic Web sense) and communication between the bot and the user takes place in a chat, then
 the most intuitive solution for filling out a form (creating an element) is filling the form attribute by attribute,
 when the first element of the form is filled first, then the second, and so on. With this approach, it is necessary to use temporary storage for remembering
-specified values in order to create an element from the form at the end. ``TelegaModelForm`` and ``TelegaForm`` are implemented just
+specified values in order to create an element from the form at the end. ``TelegramModelForm`` and ``TelegramForm`` are implemented just
 in such way for taking over this process. The difference between these classes and the standard Django classes is precisely
 in the modification of the method of filling in the form fields, otherwise they do not differ from standard forms.
 
-``TelegaModelForm`` and ``TelegaForm`` as Django descendants of ``ModelForm`` and ``Form`` have the following parameters, which you may need to customize:
+``TelegramModelForm`` and ``TelegramForm`` as Django descendants of ``ModelForm`` and ``Form`` have the following parameters, which you may need to customize:
 
 1. The clean function and other `form validation process functions <https://docs.djangoproject.com/en/4.1/ref/forms/validation/>`_ ;
 2. ``labels`` - field names;
-3. ``forms.HiddenInput`` - designation of hidden fields (hiding fields allows them not to be shown to the user, while using and configuring in forms or in ``TelegaViewSet``).
+3. ``forms.HiddenInput`` - designation of hidden fields (hiding fields allows them not to be shown to the user, while using and configuring in forms or in ``TelegramViewSet``).
 
 
 
-``TelegaViewSet`` is designed to interact with descendants of the ``TelegaModelForm`` class and allows you to use
+``TelegramViewSet`` is designed to interact with descendants of the ``TelegramModelForm`` class and allows you to use
 generate forms with different fields, such as ``CharField, IntegerField`` or ``ForeignKey, ManyToManyField``. Also, it is a good idea
-to use the ``prechoice_fields_values`` dictionary in ``TelegaViewSet`` descendants for improving the convenience of filling out forms for users.
+to use the ``prechoice_fields_values`` dictionary in ``TelegramViewSet`` descendants for improving the convenience of filling out forms for users.
 It is possible to store a list of frequently used values of form fields in the ``prechoice_fields_values``.
 This allows users to select the desired values by clicking buttons rather than
 writing text manually. The template has an example of using this field:
 
 
 .. code-block:: python
 
@@ -512,25 +506,25 @@
 
 Like a regular handler, the function takes 3 arguments as input: bot, update, user. After saving these arguments in class,
 the determination of the current routing path is occurred. It is determined either by pressing a button in the bot (the ``callback_data`` value of the button), or
 can be stored in the user attribute ``user.current_utrl``. The second option is possible if the user manually enters
 some information (for example, filled in a text field of form). After that, the arguments are extracted from the path
 to call a specific function. Storing and interacting with arguments in a path is similar to how ``sys.argv`` works. So,
 for example, the string ``"sl&1&20"`` will be converted to the list ``['sl', '1', '20']``. The separator character between attributes
-is ``&`` by default and can be changed via the ``TelegaViewSet.ARGS_SEPARATOR_SYMBOL`` variable.
+is ``&`` by default and can be changed via the ``TelegramViewSet.ARGS_SEPARATOR_SYMBOL`` variable.
 
-When using ``TelegaViewSet`` you most likely won't have to interact with the argument string directly, since
+When using ``TelegramViewSet`` you most likely won't have to interact with the argument string directly, since
 ``dispatch`` converts a string into arguments. And for creating a ``callback_data`` button string, that the user can call another method from Telegram interface, you should use
-``TelegaViewSet.gm_callback_data`` function. In case you need more low-level interaction with function arguments, then
+``TelegramViewSet.gm_callback_data`` function. In case you need more low-level interaction with function arguments, then
 you can use the ``construct_utrl`` and ``get_utrl_params`` functions.
 
 After receiving the utrl_args arguments and checking access rights, the managing method (action) is directly selected and called.
 The first argument, which is the short name for the function, is popped from the utrl_args. All other arguments are passed as parameters
 into a function. Inside the function, the necessary business logic and the data formatting for displaying to the user as a response take place.
-Any such managing function in the ``TelegaViewSet`` class must return the action type ``chat_action`` and the parameters to that action ``chat_action_args``.
+Any such managing function in the ``TelegramViewSet`` class must return the action type ``chat_action`` and the parameters to that action ``chat_action_args``.
 By default, the class has only 1 action ﹣ ``CHAT_ACTION_MESSAGE``, which means that the user will receive
 a text message (possibly with buttons) as an answer for his/her action. The arguments for this action are the text of the message and a list of buttons (can be None).
 
 
 After the function is processed, a response is sent to the user by ``send_answer`` function and the user's action is logged.
 
 
@@ -630,15 +624,15 @@
 However, these fields are not always enough and you need to redefine the logic of helper functions for a beautiful display of information.
 
 
 Helper functions for displaying data
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 
-The ``TelegaViewSet`` class describes the following helper functions for generating a response message:
+The ``TelegramViewSet`` class describes the following helper functions for generating a response message:
 
 
 * ``def gm_no_elem`` - if no element with this ID was found;
 * ``def gm_success_created`` - successful creation of the model;
 * ``def gm_next_field`` - when moving to the next form attribute;
 * ``def gm_next_field_choice_buttons`` - generates buttons to select options for a specific form attribute (used inside ``gm_next_field``);
 * ``def gm_value_error`` - error output when adding a form attribute;
@@ -669,15 +663,15 @@
 
 * Getting or creating a user in the database;
 * In case of an error inside the handler function, returns an error message to the user;
 * Logs the handler call;
 * Tracks where the user came from;
 * Choice of language for sending messages to the user (in the case of localization enabled);
 
-This handler is also used inside ``RouterCallbackMessageCommandHandler``, and as a result in calling ``TelegaViewSet`` classes.
+This handler is also used inside ``RouterCallbackMessageCommandHandler``, and as a result in calling ``TelegramViewSet`` classes.
 
 Localization
 ~~~~~~~~~~~~~~~~
 
 The library expands the `Django localization tools <https://docs.djangoproject.com/en/4.1/topics/i18n/>`_ for use in Telegram.
 To support the use of different languages, the main elements of the Python-Telegram-Bot library are redefined in ``telegram_django_bot.telegram_lib_redefinition``:
 
@@ -687,48 +681,50 @@
 3. ``telegram.KeyboardButton`` -> ``telegram_django_bot.KeyboardButtonDJ`` ;
 4. ``telegram.InlineKeyboardButton`` -> ``telegram_django_bot.InlineKeyboardButtonDJ`` ;
 5. ``telegram.InlineKeyboardMarkup`` -> ``telegram_django_bot.InlineKeyboardMarkupDJ``.
 
 
 When using these classes in code, multilingual support comes down to the following steps:
 
+
 1. Specifying the necessary settings in the settings.py file: ``LANGUAGES`` - list of languages, ``LANGUAGE_CODE`` - default language;
-1. Necessary texts for translation are wrapped in ``gettext`` and ``gettext_lazy`` from ``django.utils.translation`` (how it works in Django `read here <https://docs.djangoproject.com/en /4.1/topics/i18n/translation/#standard-translation>`_ )
-2. Run command ``$ django-admin makemessages -a`` to generate texts for translation (created in locale folder)
-3. Generation of translation files ``$ django-admin compilemessages``.
+2. Create folder with translations: ``$ django-admin makemessages -l <language_code>``
+3. Necessary texts for translation are wrapped in ``gettext`` and ``gettext_lazy`` from ``django.utils.translation`` (how it works in Django `read here <https://docs.djangoproject.com/en /4.1/topics/i18n/translation/#standard-translation>`_ )
+4. Run command ``$ django-admin makemessages -a`` to update texts for translation (created in locale folder)
+5. Generation of translation files ``$ django-admin compilemessages``.
 
 Only a part of the functions uses localization in the template. It is made for easy understanding. The usage of localization can be seen in the example
 functions ``some_debug_func``.
 
 
 Extra lib features
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 The library provides some additional tools for the convenience of developing and managing the bot.
 
-Модели библиотеки
+Embedded ORM lib models
 ************************************
 
 
-For the correct work of ``TelegaViewSet`` and other components the Django ORM model representing the user in Telegram must be inherited
+For the correct work of ``TelegramViewSet`` and other components the Django ORM model representing the user in Telegram must be inherited
 from ``telegram_django_bot.models.TelegramUser``, as these components use its fields. ``TelegramUser`` inherited from
 ``django.contrib.auth.models.AbstractUser`` (which allows you to authorize users on the site if necessary) and has
 the following additional fields:
 
 * ``id`` - redefined to use user ID from telegrams;
 * ``seed_code`` - arbitrary value from 1 to 100 to randomly group users for tests and analysis;
 * ``telegram_username`` - username of the user in telegram;
 * ``telegram_language_code`` - telegram language code (some languages have dialects and as a result the code designation is more than 2 symbols);
 * ``timezone`` - the user's time zone (for determining the time);
-* ``current_utrl`` - path (utrl) of the last user action (used in ``TelegaViewSet``);
+* ``current_utrl`` - path (utrl) of the last user action (used in ``TelegramViewSet``);
 * ``current_utrl_code_dttm`` - time of the last action, when saving the path;
 * ``current_utrl_context_db`` - path context (utrl);
 * ``current_utrl_form_db`` - intermediate data for the form. Acts as a temporary data store when filling out a form;
 
-Fields ``current_utrl_<suffix>`` are needed for ``TelegaViewSet``, ``TelegaModelForm`` and are needed in exceptional cases
+Fields ``current_utrl_<suffix>`` are needed for ``TelegramViewSet``, ``TelegramModelForm`` and are needed in exceptional cases
 when writing code. The model also has the following methods (property) to simplify interaction with model fields:
 
 * ``current_utrl_form`` (property) - returns the current temporarily stored path form data (utrl);
 * ``current_utrl_context`` (property) - returns the current path context (utrl);
 * ``save_form_in_db`` - saves the form in the ``current_utrl_form_db`` field;
 * ``save_context_in_db`` - saves the context in the field ``current_utrl_context_db``;
 * ``clear_status`` - clears the data associated with the used path (fields ``current_utrl_<suffix>``) ;
@@ -771,25 +767,25 @@
 * ``telegram_django_bot.utils.CalendarPagination`` - class for generating a calendar with buttons;
 * ``telegram_django_bot.user_viewset.UserViewSet`` - telegram user class for changing language and time zone;
 
 
 Routing details
 ********************
 
-In this section, we will analyze the work of ``RouterCallbackMessageCommandHandler`` and ``telega_reverse`` in a little more detail.
+In this section, we will analyze the work of ``RouterCallbackMessageCommandHandler`` and ``telegram_reverse`` in a little more detail.
 
 As described earlier ``RouterCallbackMessageCommandHandler`` is used to be able to write handlers in the style
 Django. Also ``RouterCallbackMessageCommandHandler`` provides the ability to handle calls to ``BotMenuElem`` as
 through commands, and through callback. This is achieved by using the functions ``all_command_bme_handler`` and
 ``all_callback_bme_handler``. By default, ``BotMenuElem`` call handling is enabled and handled after
 no suitable path was found in the description of utrls (paths in Django notation). If there is no ``BotMenuElem`` element
 match is found, the ``BotMenuElem`` is considered to be configured incorrectly and an error message is returned to the user.
 You can create a class with the ``only_utrl=True`` attribute, what is disable calls to ``BotMenuElem``.
 
-The example template contains the use of the ``telega_reverse`` function, the essence of which is to generate a path (string) to the
+The example template contains the use of the ``telegram_reverse`` function, the essence of which is to generate a path (string) to the
 handler specified in the function argument. The function is analogous to the `reverse <https://docs.djangoproject.com/en/4.1/ref/urlresolvers/#reverse>`_ Django function
 and avoids errors when changing paths.
 
 
 
 Tests
 **********************
```

### Comparing `telegram_django_bot-1.0.2/README.rst` & `telegram_django_bot-1.1.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-Telegram Django Bot Bridge
+Telegram Django Bot
 ============================
 
 This library provides a Python high-level interface for creating Telegram Bots. It standardizes the coding in the best
 practice of the web development. The library is based on `Django <https://www.djangoproject.com/>`_ and `Python-Telegram-Bot <https://python-telegram-bot.org/>`_.
-and provides viewset interface for managing data with.
+It also provides viewset interface for managing data with.
 
 If you start a new project, you could use `Telegram django bot template <https://github.com/alexanderaleskin/telergam_django_bot_template>`_ with preconfigured settings.
 
 Install
 ------------
 
 You can install via ``pip``:
@@ -45,15 +45,15 @@
   Not necessary, but useful settings:
 
 * ``TELEGRAM_TOKEN`` - for adding "triggers",
 * ``TELEGRAM_TEST_USER_IDS`` - for adding tests for your bot,
 * Make sure, that ``LANGUAGE_CODE``, ``LANGUAGE_CODE``, ``USE_I18N`` are also used in the library for language localization.
 
 
-4. This step connects ``Telegram Django Bot Bridge`` with ``Python-Telegram-Bot``. Add ``RouterCallbackMessageCommandHandler`` in handlers for using TELEGRAM_ROOT_UTRLCONF :
+4. This step connects ``Telegram Django Bot`` with ``Python-Telegram-Bot``. Add ``RouterCallbackMessageCommandHandler`` in handlers for using TELEGRAM_ROOT_UTRLCONF :
 
 .. code-block:: python
 
     updater = Updater(bot=TG_DJ_Bot(settings.TELEGRAM_TOKEN))
     updater.dispatcher.add_handler(RouterCallbackMessageCommandHandler())
 
 or in 20.x version :
@@ -79,36 +79,30 @@
 
 and Django:
 
 * Django ORM  (communication with Database);
 * Administration panel for management.
 
 
-Telegram Django Bot Bridge provides next special opportunities:
+Telegram Django Bot provides next special opportunities:
 
 * using Viewsets (typical action with model (create, update, list, delete));
 * using Django localization.
 * using function routing like urls routing in Django.
-
-And some extra useful staff:
-
 * creating general menu items with no-coding (through Django Admin Panel);
-* extra high-level Bot functions, such as a wrapper for sending delayed (or scheduled) messages;
-* creating tests;
 * collecting stats from user actions in the bot;
-* commonly used utilities.
-
+* other useful staff.
 
 
 The key feature of the lib is ``TelegramViewSet`` - a class for managing Django ORM model. It is designed in a
 similar way as `Django rest framework Viewset <https://www.django-rest-framework.org/api-guide/viewsets/>`_ , but has
-a significant difference: while DRF Viewset provides a response in serializable format (usually in json format) to frontend app, TelegaViewSet
+a significant difference: while DRF Viewset provides a response in serializable format (usually in json format) to frontend app, TelegramViewSet
 provides a response to the user in telegram interface in message format with buttons. So, you will manage data and receive
-responses in human format by executing TelegaViewSet method. The methods use some kind of templates for generating human
-responses (it is possible to overwrite these templates). By default, TelegaViewSet has 5 methods:
+responses in human format by executing TelegramViewSet method. The methods use some kind of templates for generating human
+responses (it is possible to overwrite these templates). By default, TelegramViewSet has 5 methods:
 
 * ``create`` - create a new instance of the specified ORM model;
 * ``change`` - update instance fields of specified ORM model;
 * ``show_elem`` - show fields of the element and buttons with actions of this instance;
 * ``show_list`` - show list of model elements (with pagination);
 * ``delete`` - delete the instance
 
@@ -130,35 +124,35 @@
 
 .. code-block:: python
 
     from telegram_django_bot import forms as td_forms
     from telegram_django_bot.td_viewset import TelegramViewSet
 
 
-    class RequestForm(td_forms.TelegaModelForm):
+    class RequestForm(td_forms.TelegramModelForm):
         class Meta:
             model = Request
             fields = ['text', 'importance_level', 'project', 'tags']
 
 
     class RequestViewSet(TelegramViewSet):
-        telega_form = RequestForm
+        model_form = RequestForm
         queryset = Request.objects.all()
         viewset_name = 'Request'
 
 
 If you need, you can add extra actions to RequestViewSet for managing (see details information below) or change existing functions.
-There are several parameters and secondary functions in TelegaViewSet for customizing logic if it is necessary.
+There are several parameters and secondary functions in TelegramViewSet for customizing logic if it is necessary.
 
-In this example, ``TelegaModelForm`` was used. TelegaModelForm is a descendant of Django ModelForm. So, you could use
+In this example, ``TelegramModelForm`` was used. TelegramModelForm is a descendant of Django ModelForm. So, you could use
 labels, clean functions and other parameters and functions for managing logic and displaying.
 
 
-TelegaViewSet is designed to answer next user actions: clicking buttons and sometimes sending messages. The library imposes
-`Django URL notation <https://docs.djangoproject.com/en/4.1/topics/http/urls/>`_ for mapping user actions to TelegaViewSet methods (or usual handlers).
+TelegramViewSet is designed to answer next user actions: clicking buttons and sometimes sending messages. The library imposes
+`Django URL notation <https://docs.djangoproject.com/en/4.1/topics/http/urls/>`_ for mapping user actions to TelegramViewSet methods (or usual handlers).
 Usually, for correct mapping you just need to set ``TELEGRAM_ROOT_UTRLCONF`` and use ``RouterCallbackMessageCommandHandler`` in
 dispatcher as it is mentioned above in the *Install paragraph*.
 
 For correct mapping *RequestViewSet*  you should write in the TELEGRAM_ROOT_UTRLCONF file something like this:
 
 .. code-block:: python
 
@@ -235,15 +229,15 @@
          dp=updater.dispatcher
          dp.add_handler(RouterCallbackMessageCommandHandler())
 
 
 The example adds 1 super handler ``RouterCallbackMessageCommandHandler``, which allows you to write handlers
 in the style of handling link requests in the same way as it is done in ``Django``. ``RouterCallbackMessageCommandHandler`` allows you to handle
 messages, user commands and button clicks by users. In other words, it replaces the handlers
-``MessageHandler, CommandHandler, CallbackQueryHandler`` . Since the ``Telegram Django Bot Bridge`` library is an extension,
+``MessageHandler, CommandHandler, CallbackQueryHandler`` . Since the ``Telegram Django Bot`` library is an extension,
 it does not prohibit the use of standard handlers of the ``Python-Telegram-Bot`` library for handle user requests.
 (sometimes it is simply necessary, for example, if you need to process responses to surveys (you need to use PollAnswerHandler)).
 
 `Django notation <https://docs.djangoproject.com/en/4.1/topics/http/urls/>`_ of routing handlers is that paths to handlers are described in a separate file or files.
 As in the ``Django`` standard, the main file (root) for routing is specified in the project settings, where paths to handlers or paths to groups of handlers are stored.
 The ``TELEGRAM_ROOT_UTRLCONF`` (same as ``ROOT_URLCONF`` for WEB) attribute is used to specify the path to the file. In the example template, we have the following settings:
 
@@ -304,122 +298,122 @@
 This distribution of handlers allows you to group part of the handlers into modules and quickly connect or
 change them, while not being afraid of confusion which handlers need to be called, as it can be if all paths from
 different modules to handlers are described in one place as required by ``Python-Telegram-Bot``.
 
 In this example file ``base.utrls.py`` also ViewSets are used in addition to simple handler functions like ``def start`` and ``def some_debug_func``.
 ViewSet is an aggregator of several functions. The concept of it is that you quite often need to apply
 the same operations for a dataset, such as create, update, show, delete an example of dataset.
-There is the class ``telegram_django_bot.td_viewset.TelegaViewSet`` in the library  for such purposes. The class manages
-the Django ORM database model. ``TelegaViewSet`` has 5 functions for managing the model:
+There is the class ``telegram_django_bot.td_viewset.TelegramViewSet`` in the library  for such purposes. The class manages
+the Django ORM database model. ``TelegramViewSet`` has 5 functions for managing the model:
 
 
 ========= ======== ===========================
  Метод     UTRL      Description
 --------- -------- ---------------------------
 create     cr       Create model
 change     up       Change model attributes
 delete     de       Deleting a model
 show_elem  se       Display a model
 show_list  sl       Display a list of models
 ========= ======== ===========================
 
 Thus, if we want to call the ``BotMenuElemViewSet.create`` method to create an element, we need to use
 path 'sb/cr', whereby the first part of the path 'sb/'  the router ``RouterCallbackMessageCommandHandler`` will execute
-the ``BotMenuElemViewSet`` class, namely the ``TelegaViewSet.dispatch`` method, which in turn will call  the ``create`` method by analyzing the second part of the path
+the ``BotMenuElemViewSet`` class, namely the ``TelegramViewSet.dispatch`` method, which in turn will call  the ``create`` method by analyzing the second part of the path
 ``cr``.
 
 To sum up the scheme of handlers routing, there are following key points:
 
 1. ``telegram.ext.Update`` is used as a receiver of messages from Telegram;
-2. Standard handlers of the ``Python-Telegram-Bot`` library can be used as handlers. For convenient use Django's path scheme and ``TelegaViewSet`` you need to use ``RouterCallbackMessageCommandHandler``.
-3. ``TelegaViewSet`` aggregates a set of standard functions for managing data, what is made possible to group code associated with one type of data type in one class (place).
+2. Standard handlers of the ``Python-Telegram-Bot`` library can be used as handlers. For convenient use Django's path scheme and ``TelegramViewSet`` you need to use ``RouterCallbackMessageCommandHandler``.
+3. ``TelegramViewSet`` aggregates a set of standard functions for managing data, what is made possible to group code associated with one type of data type in one class (place).
 
 
 
 TelegramViewSet features
 ~~~~~~~~~~~~~~~~~~~~~~~~
 
-As described above, TelegaViewSet contains standard functions for data manipulation.
+As described above, TelegramViewSet contains standard functions for data manipulation.
 Due to such standard data processing methods, it turns out in the example to describe the logic of ``BotMenuElemViewSet`` in 40
 lines of code, also using some customization for beautiful data displaying.
 
 
-To use all the features of the TelegaViewSet in your class, it should be inherited from it, as, for example, this is done
+To use all the features of the TelegramViewSet in your class, it should be inherited from it, as, for example, this is done
 in the ``BotMenuElemViewSet``:
 
 
 .. code-block:: python
 
     from telegram_django_bot.td_viewset import TelegramViewSet
 
     class BotMenuElemViewSet(TelegramViewSet):
 
 
 In order to customize the ViewSet, you must specify 3 required attributes:
 
 1. ``viewset_name`` - class name, used to display to telegram users
-2. ``telega_form`` - data form, used to specify which fields of the ORM database model to use in the viewset;
+2. ``model_form`` - data form, used to specify which fields of the ORM database model to use in the viewset;
 3. ``queryset`` - basic query for getting model elements.
 
 
 The ``BotMenuElemViewSet`` is used the following values:
 
 .. code-block:: python
 
     from telegram_django_bot import forms as td_forms
     from telegram_django_bot.models import BotMenuElem
 
-    class BotMenuElemForm(td_forms.TelegaModelForm):
+    class BotMenuElemForm(td_forms.TelegramModelForm):
         form_name = _("Menu elem")
 
         class Meta:
             model = BotMenuElem
             fields = ['command', "is_visable", "callbacks_db", "message", "buttons_db"]
 
-    class BotMenuElemViewSet(TelegaViewSet):
+    class BotMenuElemViewSet(TelegramViewSet):
         viewset_name = 'BotMenuElem'
-        telega_form = BotMenuElemForm
+        model_form = BotMenuElemForm
         queryset = BotMenuElem.objects.all()
 
 
 where ``BotMenuElemForm`` is a descendant of the ``Django ModelFrom`` class, so it has a similar structure and parameterization methods.
 `` form_name ``  stands for the name of the form and is used in some messages sent to Telegram users.
 
 
-TelegaViewSet has quite a lot in common with Viewset analogs tailored for WEB development (for example,
-`django-rest-framework viewsets <https://www.django-rest-framework.org/api-guide/viewsets/>`_ ). However, as part of the development of Telegram bots, TelegaViewSet
+TelegramViewSet has quite a lot in common with Viewset analogs tailored for WEB development (for example,
+`django-rest-framework viewsets <https://www.django-rest-framework.org/api-guide/viewsets/>`_ ). However, as part of the development of Telegram bots, TelegramViewSet
 has some special features:
 
 1. An unusual way to create elements;
 2. The display of information in bots is limited and most often comes down to displaying text and buttons, so the viewset in addition to business logic includes the creation of standard responses to user actions in the form of messages with buttons.
 
 
 
 Forms
 ************
 
 
 Since Telegram does not have the ability to create forms (in the classic Web sense) and communication between the bot and the user takes place in a chat, then
 the most intuitive solution for filling out a form (creating an element) is filling the form attribute by attribute,
 when the first element of the form is filled first, then the second, and so on. With this approach, it is necessary to use temporary storage for remembering
-specified values in order to create an element from the form at the end. ``TelegaModelForm`` and ``TelegaForm`` are implemented just
+specified values in order to create an element from the form at the end. ``TelegramModelForm`` and ``TelegramForm`` are implemented just
 in such way for taking over this process. The difference between these classes and the standard Django classes is precisely
 in the modification of the method of filling in the form fields, otherwise they do not differ from standard forms.
 
-``TelegaModelForm`` and ``TelegaForm`` as Django descendants of ``ModelForm`` and ``Form`` have the following parameters, which you may need to customize:
+``TelegramModelForm`` and ``TelegramForm`` as Django descendants of ``ModelForm`` and ``Form`` have the following parameters, which you may need to customize:
 
 1. The clean function and other `form validation process functions <https://docs.djangoproject.com/en/4.1/ref/forms/validation/>`_ ;
 2. ``labels`` - field names;
-3. ``forms.HiddenInput`` - designation of hidden fields (hiding fields allows them not to be shown to the user, while using and configuring in forms or in ``TelegaViewSet``).
+3. ``forms.HiddenInput`` - designation of hidden fields (hiding fields allows them not to be shown to the user, while using and configuring in forms or in ``TelegramViewSet``).
 
 
 
-``TelegaViewSet`` is designed to interact with descendants of the ``TelegaModelForm`` class and allows you to use
+``TelegramViewSet`` is designed to interact with descendants of the ``TelegramModelForm`` class and allows you to use
 generate forms with different fields, such as ``CharField, IntegerField`` or ``ForeignKey, ManyToManyField``. Also, it is a good idea
-to use the ``prechoice_fields_values`` dictionary in ``TelegaViewSet`` descendants for improving the convenience of filling out forms for users.
+to use the ``prechoice_fields_values`` dictionary in ``TelegramViewSet`` descendants for improving the convenience of filling out forms for users.
 It is possible to store a list of frequently used values of form fields in the ``prechoice_fields_values``.
 This allows users to select the desired values by clicking buttons rather than
 writing text manually. The template has an example of using this field:
 
 
 .. code-block:: python
 
@@ -481,25 +475,25 @@
 
 Like a regular handler, the function takes 3 arguments as input: bot, update, user. After saving these arguments in class,
 the determination of the current routing path is occurred. It is determined either by pressing a button in the bot (the ``callback_data`` value of the button), or
 can be stored in the user attribute ``user.current_utrl``. The second option is possible if the user manually enters
 some information (for example, filled in a text field of form). After that, the arguments are extracted from the path
 to call a specific function. Storing and interacting with arguments in a path is similar to how ``sys.argv`` works. So,
 for example, the string ``"sl&1&20"`` will be converted to the list ``['sl', '1', '20']``. The separator character between attributes
-is ``&`` by default and can be changed via the ``TelegaViewSet.ARGS_SEPARATOR_SYMBOL`` variable.
+is ``&`` by default and can be changed via the ``TelegramViewSet.ARGS_SEPARATOR_SYMBOL`` variable.
 
-When using ``TelegaViewSet`` you most likely won't have to interact with the argument string directly, since
+When using ``TelegramViewSet`` you most likely won't have to interact with the argument string directly, since
 ``dispatch`` converts a string into arguments. And for creating a ``callback_data`` button string, that the user can call another method from Telegram interface, you should use
-``TelegaViewSet.gm_callback_data`` function. In case you need more low-level interaction with function arguments, then
+``TelegramViewSet.gm_callback_data`` function. In case you need more low-level interaction with function arguments, then
 you can use the ``construct_utrl`` and ``get_utrl_params`` functions.
 
 After receiving the utrl_args arguments and checking access rights, the managing method (action) is directly selected and called.
 The first argument, which is the short name for the function, is popped from the utrl_args. All other arguments are passed as parameters
 into a function. Inside the function, the necessary business logic and the data formatting for displaying to the user as a response take place.
-Any such managing function in the ``TelegaViewSet`` class must return the action type ``chat_action`` and the parameters to that action ``chat_action_args``.
+Any such managing function in the ``TelegramViewSet`` class must return the action type ``chat_action`` and the parameters to that action ``chat_action_args``.
 By default, the class has only 1 action ﹣ ``CHAT_ACTION_MESSAGE``, which means that the user will receive
 a text message (possibly with buttons) as an answer for his/her action. The arguments for this action are the text of the message and a list of buttons (can be None).
 
 
 After the function is processed, a response is sent to the user by ``send_answer`` function and the user's action is logged.
 
 
@@ -599,15 +593,15 @@
 However, these fields are not always enough and you need to redefine the logic of helper functions for a beautiful display of information.
 
 
 Helper functions for displaying data
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 
-The ``TelegaViewSet`` class describes the following helper functions for generating a response message:
+The ``TelegramViewSet`` class describes the following helper functions for generating a response message:
 
 
 * ``def gm_no_elem`` - if no element with this ID was found;
 * ``def gm_success_created`` - successful creation of the model;
 * ``def gm_next_field`` - when moving to the next form attribute;
 * ``def gm_next_field_choice_buttons`` - generates buttons to select options for a specific form attribute (used inside ``gm_next_field``);
 * ``def gm_value_error`` - error output when adding a form attribute;
@@ -638,15 +632,15 @@
 
 * Getting or creating a user in the database;
 * In case of an error inside the handler function, returns an error message to the user;
 * Logs the handler call;
 * Tracks where the user came from;
 * Choice of language for sending messages to the user (in the case of localization enabled);
 
-This handler is also used inside ``RouterCallbackMessageCommandHandler``, and as a result in calling ``TelegaViewSet`` classes.
+This handler is also used inside ``RouterCallbackMessageCommandHandler``, and as a result in calling ``TelegramViewSet`` classes.
 
 Localization
 ~~~~~~~~~~~~~~~~
 
 The library expands the `Django localization tools <https://docs.djangoproject.com/en/4.1/topics/i18n/>`_ for use in Telegram.
 To support the use of different languages, the main elements of the Python-Telegram-Bot library are redefined in ``telegram_django_bot.telegram_lib_redefinition``:
 
@@ -656,48 +650,50 @@
 3. ``telegram.KeyboardButton`` -> ``telegram_django_bot.KeyboardButtonDJ`` ;
 4. ``telegram.InlineKeyboardButton`` -> ``telegram_django_bot.InlineKeyboardButtonDJ`` ;
 5. ``telegram.InlineKeyboardMarkup`` -> ``telegram_django_bot.InlineKeyboardMarkupDJ``.
 
 
 When using these classes in code, multilingual support comes down to the following steps:
 
+
 1. Specifying the necessary settings in the settings.py file: ``LANGUAGES`` - list of languages, ``LANGUAGE_CODE`` - default language;
-1. Necessary texts for translation are wrapped in ``gettext`` and ``gettext_lazy`` from ``django.utils.translation`` (how it works in Django `read here <https://docs.djangoproject.com/en /4.1/topics/i18n/translation/#standard-translation>`_ )
-2. Run command ``$ django-admin makemessages -a`` to generate texts for translation (created in locale folder)
-3. Generation of translation files ``$ django-admin compilemessages``.
+2. Create folder with translations: ``$ django-admin makemessages -l <language_code>``
+3. Necessary texts for translation are wrapped in ``gettext`` and ``gettext_lazy`` from ``django.utils.translation`` (how it works in Django `read here <https://docs.djangoproject.com/en /4.1/topics/i18n/translation/#standard-translation>`_ )
+4. Run command ``$ django-admin makemessages -a`` to update texts for translation (created in locale folder)
+5. Generation of translation files ``$ django-admin compilemessages``.
 
 Only a part of the functions uses localization in the template. It is made for easy understanding. The usage of localization can be seen in the example
 functions ``some_debug_func``.
 
 
 Extra lib features
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 The library provides some additional tools for the convenience of developing and managing the bot.
 
-Модели библиотеки
+Embedded ORM lib models
 ************************************
 
 
-For the correct work of ``TelegaViewSet`` and other components the Django ORM model representing the user in Telegram must be inherited
+For the correct work of ``TelegramViewSet`` and other components the Django ORM model representing the user in Telegram must be inherited
 from ``telegram_django_bot.models.TelegramUser``, as these components use its fields. ``TelegramUser`` inherited from
 ``django.contrib.auth.models.AbstractUser`` (which allows you to authorize users on the site if necessary) and has
 the following additional fields:
 
 * ``id`` - redefined to use user ID from telegrams;
 * ``seed_code`` - arbitrary value from 1 to 100 to randomly group users for tests and analysis;
 * ``telegram_username`` - username of the user in telegram;
 * ``telegram_language_code`` - telegram language code (some languages have dialects and as a result the code designation is more than 2 symbols);
 * ``timezone`` - the user's time zone (for determining the time);
-* ``current_utrl`` - path (utrl) of the last user action (used in ``TelegaViewSet``);
+* ``current_utrl`` - path (utrl) of the last user action (used in ``TelegramViewSet``);
 * ``current_utrl_code_dttm`` - time of the last action, when saving the path;
 * ``current_utrl_context_db`` - path context (utrl);
 * ``current_utrl_form_db`` - intermediate data for the form. Acts as a temporary data store when filling out a form;
 
-Fields ``current_utrl_<suffix>`` are needed for ``TelegaViewSet``, ``TelegaModelForm`` and are needed in exceptional cases
+Fields ``current_utrl_<suffix>`` are needed for ``TelegramViewSet``, ``TelegramModelForm`` and are needed in exceptional cases
 when writing code. The model also has the following methods (property) to simplify interaction with model fields:
 
 * ``current_utrl_form`` (property) - returns the current temporarily stored path form data (utrl);
 * ``current_utrl_context`` (property) - returns the current path context (utrl);
 * ``save_form_in_db`` - saves the form in the ``current_utrl_form_db`` field;
 * ``save_context_in_db`` - saves the context in the field ``current_utrl_context_db``;
 * ``clear_status`` - clears the data associated with the used path (fields ``current_utrl_<suffix>``) ;
@@ -740,25 +736,25 @@
 * ``telegram_django_bot.utils.CalendarPagination`` - class for generating a calendar with buttons;
 * ``telegram_django_bot.user_viewset.UserViewSet`` - telegram user class for changing language and time zone;
 
 
 Routing details
 ********************
 
-In this section, we will analyze the work of ``RouterCallbackMessageCommandHandler`` and ``telega_reverse`` in a little more detail.
+In this section, we will analyze the work of ``RouterCallbackMessageCommandHandler`` and ``telegram_reverse`` in a little more detail.
 
 As described earlier ``RouterCallbackMessageCommandHandler`` is used to be able to write handlers in the style
 Django. Also ``RouterCallbackMessageCommandHandler`` provides the ability to handle calls to ``BotMenuElem`` as
 through commands, and through callback. This is achieved by using the functions ``all_command_bme_handler`` and
 ``all_callback_bme_handler``. By default, ``BotMenuElem`` call handling is enabled and handled after
 no suitable path was found in the description of utrls (paths in Django notation). If there is no ``BotMenuElem`` element
 match is found, the ``BotMenuElem`` is considered to be configured incorrectly and an error message is returned to the user.
 You can create a class with the ``only_utrl=True`` attribute, what is disable calls to ``BotMenuElem``.
 
-The example template contains the use of the ``telega_reverse`` function, the essence of which is to generate a path (string) to the
+The example template contains the use of the ``telegram_reverse`` function, the essence of which is to generate a path (string) to the
 handler specified in the function argument. The function is analogous to the `reverse <https://docs.djangoproject.com/en/4.1/ref/urlresolvers/#reverse>`_ Django function
 and avoids errors when changing paths.
 
 
 
 Tests
 **********************
```

### Comparing `telegram_django_bot-1.0.2/setup.cfg` & `telegram_django_bot-1.1.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = telegram_django_bot
-version = 1.0.2
-description = Telegram Django Bot Bridge
+version = 1.1.0
+description = Telegram Django Bot
 long_description = file: README.rst
-url = https://github.com/alexanderaleskin/telegram_django_bot_bridge
+url = https://github.com/alexanderaleskin/telegram_django_bot
 author = Alexander Aleskin
 author_email = alexanderaleskin@gmail.com
 license = MIT
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Framework :: Django
 	Framework :: Django :: 3.0
```

### Comparing `telegram_django_bot-1.0.2/telegram_django_bot/admin.py` & `telegram_django_bot-1.1.0/telegram_django_bot/admin.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.2/telegram_django_bot/admin_utils.py` & `telegram_django_bot-1.1.0/telegram_django_bot/admin_utils.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.2/telegram_django_bot/forms.py` & `telegram_django_bot-1.1.0/telegram_django_bot/forms.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,27 +3,42 @@
 from django.forms import HiddenInput
 from django.db import models
 
 
 # todo: PreChoise logic to fields
 # todo: support media
 
-# class TelegaErrorList(ErrorList):
+# class TelegramErrorList(ErrorList):
 #     def __str__(self):
 #         return self.as_text()
 #
 
-class TelegaErrorDict(ErrorDict):
+class TelegramErrorDict(ErrorDict):
     def __str__(self):
         return self.as_text()
 
 
 class BaseTelegramForm(BaseForm):
     # field_order = None
-    form_name = ''
+
+    # form_name = ''  # make sure that this name is unique!! It is used for storing in User details while adding or
+    # # updating element attributes.
+    # todo: add check if there are forms with same form_names
+
+    @property
+    def form_name(self) -> str:
+        """ just for easy creating class. So, the name of class should be unique  """
+        return self.__str__()
+
+    def __repr__(self):
+        return f'{self.__class__.__name__}'
+
+    def __str__(self):
+        return f'{self.__class__.__name__}'
+
 
     def _multichoice_intersection(self, set_from_user, set_from_db):
         # todo: in another place should be check with check from field type
 
         if len(set_from_db):
             db_values_type = type(next(iter(set_from_db)))  # int (if standart pk)
             set_from_user = set([db_values_type(elem) for elem in set_from_user])
@@ -78,15 +93,15 @@
 
     def __init__(self, user, data=None, files=None, initial=None):
 
         self.user = user
         data = self._init_helper_get_data(user, data)
 
         super().__init__(data, files, initial=initial)
-        # self.error_class = TelegaErrorList
+        # self.error_class = TelegramErrorList
 
         self.fields, self.next_field = self._init_helper_fields_detection(data)
 
     def save(self, commit=True):
         """ save temp data to user data"""
         if self.is_valid():
             self.user.save_form_in_db(self.__class__.__name__, self.cleaned_data, do_save=commit)
@@ -97,15 +112,15 @@
         """info about next field for full validation (creating) form"""
         return self.next_field
 
     def full_clean(self):
         """
         Clean all of self.data and populate self._errors and self.cleaned_data.
         """
-        self._errors = TelegaErrorDict()  # only for change TelegaErrorDict()
+        self._errors = TelegramErrorDict()  # only for change TelegramErrorDict()
         if not self.is_bound:  # Stop further processing.
             return
         self.cleaned_data = {}
         # If the form is permitted to be empty, and none of the form data has
         # changed from the initial data, short circuit any validation.
         if self.empty_permitted and not self.has_changed():
             return
@@ -140,18 +155,18 @@
 
                     if use_from_db:
                         data[model_field] = getattr(instance, model_field)
                         if issubclass(type(data[model_field]), models.Manager):
                             data[model_field] = data[model_field].all()
                 else:
                     raise ValueError(
-                        f'fields in Telegamodelform should have same name: {model_field}, {instance.__dict__.keys()}')
+                        f'fields in TelegramModelForm should have same name: {model_field}, {instance.__dict__.keys()}')
 
         BaseModelForm.__init__(self, data, files, initial=initial, instance=instance)
-        # self.error_class = TelegaErrorList
+        # self.error_class = TelegramErrorList
 
         self.next_field = None
         self.fields, self.next_field = self._init_helper_fields_detection(data)
 
     def save(self, commit=True, is_completed=True):
         """
 
@@ -173,10 +188,7 @@
 class TelegramForm(BaseTelegramForm, metaclass=DeclarativeFieldsMetaclass):
     """just for executing metaclass"""
 
 
 class TelegramModelForm(BaseTelegramModelForm, metaclass=ModelFormMetaclass):
     """just for executing metaclass"""
 
-
-TelegaForm = TelegramForm
-TelegaModelForm = TelegramModelForm
```

### Comparing `telegram_django_bot-1.0.2/telegram_django_bot/locale/ru/LC_MESSAGES/django.mo` & `telegram_django_bot-1.1.0/telegram_django_bot/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.2/telegram_django_bot/locale/ru/LC_MESSAGES/django.po` & `telegram_django_bot-1.1.0/telegram_django_bot/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.2/telegram_django_bot/migrations/0001_initial.py` & `telegram_django_bot-1.1.0/telegram_django_bot/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.2/telegram_django_bot/migrations/0003_botmenuelem_message_format.py` & `telegram_django_bot-1.1.0/telegram_django_bot/migrations/0003_botmenuelem_message_format.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.2/telegram_django_bot/migrations/0004_auto_20220915_0448.py` & `telegram_django_bot-1.1.0/telegram_django_bot/migrations/0004_auto_20220915_0448.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.2/telegram_django_bot/migrations/0007_auto_20221202_0305.py` & `telegram_django_bot-1.1.0/telegram_django_bot/migrations/0007_auto_20221202_0305.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.2/telegram_django_bot/migrations/0008_auto_20221225_1050.py` & `telegram_django_bot-1.1.0/telegram_django_bot/migrations/0008_auto_20221225_1050.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.2/telegram_django_bot/models.py` & `telegram_django_bot-1.1.0/telegram_django_bot/models.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.2/telegram_django_bot/routing.py` & `telegram_django_bot-1.1.0/telegram_django_bot/routing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 from .models import BotMenuElem
 from .utils import handler_decor
-from .td_viewset import TelegaViewSet
+from .td_viewset import TelegramViewSet
 from django.urls import resolve, Resolver404, reverse
 from django.conf import settings
 from django.contrib.auth import get_user_model
 
 from telegram import (
     Update,
 )
@@ -16,15 +16,15 @@
     # version 20.x +
     from telegram.ext import BaseHandler as Handler
 except ImportError:
     # old version
     from telegram.ext import Handler
 
 
-def telega_resolve(path, utrl_conf=None):
+def telegram_resolve(path, utrl_conf=None):
     if path[0] != '/':
         path = f'/{path}'
 
     if '?' in path:
         path = path.split('?')[0]
 
     if utrl_conf is None:
@@ -33,15 +33,15 @@
     try:
         resolver_match = resolve(path, utrl_conf)
     except Resolver404:
         resolver_match = None
     return resolver_match
 
 
-def telega_reverse(viewname, utrl_conf=None, args=None, kwargs=None, current_app=None):
+def telegram_reverse(viewname, utrl_conf=None, args=None, kwargs=None, current_app=None):
     if utrl_conf is None:
         utrl_conf = settings.TELEGRAM_ROOT_UTRLCONF
 
     response = reverse(viewname, utrl_conf, args, kwargs, current_app)
     if response[0] == '/':
         response = response[1:]
     return response
@@ -89,28 +89,28 @@
         self.utrl_conf = utrl_conf
         self.only_utrl = only_utrl # without BME elems
 
     def get_callback_utrl(self, update):
         callback_func = None
         # check if utrls
         if update.callback_query:
-            callback_func = telega_resolve(update.callback_query.data, self.utrl_conf)
+            callback_func = telegram_resolve(update.callback_query.data, self.utrl_conf)
         elif update.message and update.message.text and update.message.text[0] == '/':  # is it ok? seems message couldnt be an url
-            callback_func = telega_resolve(update.message.text, self.utrl_conf)
+            callback_func = telegram_resolve(update.message.text, self.utrl_conf)
 
         if callback_func is None:
             # update.message -- could be data or info for managing, command could not be a data, it is managing info
             if update.message and (update.message.text is None or update.message.text[0] != '/'):
                 user_details = update.message.from_user
 
                 user = get_user_model().objects.filter(id=user_details.id).first()
                 if user:
                     logging.info(f'user.current_utrl {user.current_utrl}')
                     if user.current_utrl:
-                        callback_func = telega_resolve(user.current_utrl, self.utrl_conf)
+                        callback_func = telegram_resolve(user.current_utrl, self.utrl_conf)
         return callback_func
 
     def check_update(self, update: object):
         """
         check if callback or message (command actually is message)
         :param update:
         :return:
@@ -136,15 +136,15 @@
         context=None,
     ):
         # todo: add flush utrl and data if viewset utrl change or error
 
         callback_func = self.get_callback_utrl(update)
 
         if not callback_func is None:
-            if inspect.isclass(callback_func.func) and issubclass(callback_func.func, TelegaViewSet):
+            if inspect.isclass(callback_func.func) and issubclass(callback_func.func, TelegramViewSet):
                 viewset = callback_func.func(callback_func.route)
 
                 decorating = handler_decor(log_type='N',)
 
                 callback_func = decorating(viewset.dispatch)
 
             else:
```

### Comparing `telegram_django_bot-1.0.2/telegram_django_bot/tasks.py` & `telegram_django_bot-1.1.0/telegram_django_bot/tasks.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-# from bot_conf.celery import app
 from django.conf import settings
 
 from django.utils import timezone
 from django.db.models import Count
 from django.db.models.functions import Coalesce
 from django.db.models import OuterRef, Exists
 
 from django.contrib.auth import get_user_model
 from .models import Trigger, UserTrigger, ActionLog
 from .tg_dj_bot import TG_DJ_Bot
 from celery import current_app
-# from .utils import send_botmenuelem, task_send_message_handler
 
 
 @current_app.task
 def create_triggers():
     def get_duration_dict(trigger, elem, add_prefix=True):
         prefix = 'actionlog__'
         if not add_prefix:
@@ -81,15 +79,15 @@
             trigger=trigger,
             user=OuterRef('id'),
             dttm_added__gte=dttm_now - trigger.min_duration
         )
 
         users = users.annotate(exist_trigger=Exists(user_triggers)).filter(exist_trigger=False)
 
-        # todo: пересечение с другими триггерами -- минимальное время между триггерами сделать?
+        # todo: intersection with other triggers -- minimum time between triggers to do?
 
         UserTrigger.objects.bulk_create([
             UserTrigger(trigger=trigger, user=user) for user in users
         ])
 
         trig_users = []
         for user in users:
@@ -105,15 +103,15 @@
 
 @current_app.task
 def send_triggers(user_ids):
     dttm_now = timezone.now()
     UserTrigger.objects.filter(
         is_sent=False,
         user_id__in=user_ids,
-        dttm_added__lt=dttm_now - timezone.timedelta(hours=16),  # триггеры  не присланные в первые 16 часов удаляем
+        dttm_added__lt=dttm_now - timezone.timedelta(hours=16),  # triggers not sent in the first 16 hours are deleted
     ).update(dttm_deleted=dttm_now)
 
     user_triggers = UserTrigger.objects.filter(
         is_sent=False,
         dttm_deleted__isnull=True,
         user_id__in=user_ids,
     ).select_related('trigger', 'trigger__botmenuelem', 'user')
@@ -125,15 +123,15 @@
 
     sent_user_triggers = []
     for user_trigger in user_triggers:
         is_sent, res_mess = bot.task_send_message_handler(
             _send_wrapper,
             user_trigger.user,
             None,
-            user_trigger.user,  # для task_send_message_handler и для send_botmenuelem
+            user_trigger.user,  # for task_send_message_handler и для send_botmenuelem
             user_trigger.trigger.botmenuelem
         )
         if is_sent:
             sent_user_triggers.append(user_trigger)
 
     UserTrigger.objects.filter(id__in=[x.id for x in sent_user_triggers]).update(is_sent=True)
     ActionLog.objects.bulk_create([
```

### Comparing `telegram_django_bot-1.0.2/telegram_django_bot/td_viewset.py` & `telegram_django_bot-1.1.0/telegram_django_bot/td_viewset.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,17 +43,18 @@
 
         new_class.command_routings = command_routings
         new_class.show_texts_dict = show_texts_dict
         return new_class
 
 
 class TelegramViewSet(metaclass=TelegramViewSetMetaClass):
-    permission_classes = [PermissionAllowAny]
-    actions = ['create', 'change', 'delete', 'show_elem', 'show_list']
+    permission_classes = [PermissionAllowAny]   # in dispatch function check permission for calling action with args
+    actions = ['create', 'change', 'delete', 'show_elem', 'show_list']  # actions of the class
 
+    # utrl for actions
     command_routing_create = 'cr'
     command_routing_change = 'up'
     command_routing_delete = 'de'
     command_routing_show_elem = 'se'
     command_routing_show_list = 'sl'
 
     WRITE_MESSAGE_VARIANT_SYMBOLS = '!WMVS!'
@@ -61,18 +62,17 @@
     GO_NEXT_MULTICHOICE_SYMBOLS = '!GNMS!'
 
     CHAT_ACTION_MESSAGE = 'message'
 
     ARGS_SEPARATOR_SYMBOL = '&'
 
     model_form = None
-    telega_form = model_form  # for legacy
 
     queryset = None
-    viewset_name = ''
+    # viewset_name = ''  # used in message for user, redefined as property by default
     foreign_filter_amount = 0
 
     prechoice_fields_values = {}
 
     updating_fields = None
 
     show_cancel_updating_button = True
@@ -81,19 +81,19 @@
 
     use_name_and_id_in_elem_showing = True
 
     meta_texts_dict = {
         'succesfully_deleted': gettext_lazy('The %(viewset_name)s  %(model_id)s is successfully deleted.'),
         'confirm_deleting': gettext_lazy('Are you sure you want to delete %(viewset_name)s  %(model_id)s?'),
         'confirm_delete_button_text': gettext_lazy('🗑 Yes, delete'),
-        'generate_message_next_field': gettext_lazy('Please, fill the field %(label)s\n\n'),
-        'generate_message_success_created': gettext_lazy('The %(viewset_name)s is created! \n\n'),
-        'generate_message_value_error': gettext_lazy('While adding %(label)s the next errors were occurred: %(errors)s\n\n'),
-        'generate_message_self_variant': gettext_lazy('Please, write the value for field %(label)s \n\n'),
-        'generate_message_no_elem': gettext_lazy(
+        'gm_next_field': gettext_lazy('Please, fill the field %(label)s\n\n'),
+        'gm_success_created': gettext_lazy('The %(viewset_name)s is created! \n\n'),
+        'gm_value_error': gettext_lazy('While adding %(label)s the next errors were occurred: %(errors)s\n\n'),
+        'gm_self_variant': gettext_lazy('Please, write the value for field %(label)s \n\n'),
+        'gm_no_elem': gettext_lazy(
             'The %(viewset_name)s %(model_id)s has not been found 😱 \nPlease try again from the beginning.'
         ),
         'leave_blank_button_text': gettext_lazy('Leave blank'),
     }
 
     def __init__(self, prefix, user=None, bot=None, update=None, foreign_filters=None):
         self.user = user
@@ -103,29 +103,41 @@
         self.foreign_filters = foreign_filters or []
 
         self.viewset_routing = {}
 
         if self.queryset is None:
             raise ValueError('queryset could not be None')
 
-        if self.telega_form is None:
-            raise ValueError('telega_form could not be None')
+        if self.model_form is None:
+            raise ValueError('model_form could not be None')
 
         for action in self.actions:
             cr_action = f'command_routing_{action}'
             if not cr_action in self.command_routings.keys():
                 raise ValueError(
                     f'for action {action} must be determinate {cr_action},'
                     f' but list is {self.command_routings.keys()}'
                 )
 
             self.viewset_routing[self.command_routings[cr_action]] = self.__getattribute__(action)
 
         self.prefix = prefix.replace('^', '').replace('$', '')
 
+    @property
+    def viewset_name(self) -> str:
+        """ just for easy creating class """
+        return self.__str__()
+
+    def __repr__(self):
+        return f'{self.__class__.__name__}'
+
+    def __str__(self):
+        return f'{self.__class__.__name__}'
+
+
     # Entrance and exit of the class:
     # dispatch gets info about user action, checks permissions, selects and executes function
     # (one of the 5 main or self written) basing on user action, and finally send answer to user
 
     def dispatch(self, bot, update, user):
         """ terminate function for response """
 
@@ -173,58 +185,58 @@
             )
         else:
             raise ValueError(f'unknown chat_action {chat_reply_action} {utrl}, {self.user}')
         return res
 
     # 5 main functions for data managing
 
-    def create(self, field=None, value=None):
+    def create(self, field=None, value=None, initial_data=None):
         """creating item, could be several steps"""
 
         if field is None and value is None:
             # then it is starting adding
             self.user.clear_status(commit=False)
 
-        return self.create_or_update_helper(field, value, 'create')
+        return self.create_or_update_helper(field, value, 'create', initial_data=initial_data)
 
     def change(self, model_or_pk, field, value=None):
         """
         change item
         :param model_or_pk: django models.Model or pk
         :param field:
         :param value:
         :return:
         """
 
-        model = self._get_elem(model_or_pk)
+        model = self.get_orm_model(model_or_pk)
 
         self.user.clear_status(commit=True)
 
         if model:
             return self.create_or_update_helper(field, value, func_response='change', instance=model)
         else:
-            return self.generate_message_no_elem(model_or_pk)
+            return self.gm_no_elem(model_or_pk)
 
     def delete(self, model_or_pk, is_confirmed=False):
         """delete item"""
 
-        model = self._get_elem(model_or_pk)
+        model = self.get_orm_model(model_or_pk)
 
         if model:
             if self.deleting_with_confirm and not is_confirmed:
                 # just ask for confirmation
                 mess, buttons = self.gm_delete_getting_confirmation(model)
             else:
                 # real deleting
                 model.delete()
                 mess, buttons = self.gm_delete_successfully(model)
 
             return self.CHAT_ACTION_MESSAGE, (mess, buttons)
         else:
-            return self.generate_message_no_elem(model_or_pk)
+            return self.gm_no_elem(model_or_pk)
 
     def show_elem(self, model_or_pk, mess=''):
         """
 
         :param model_or_pk:
         :param mess:
         :return:
@@ -239,15 +251,15 @@
                 mess += f'{self.viewset_name} #{model.pk} \n'
             mess += self.gm_show_elem_or_list_fields(model, is_elem=True)
 
             buttons = self.gm_show_elem_create_buttons(model)
 
             return self.CHAT_ACTION_MESSAGE, (mess, buttons)
         else:
-            return self.generate_message_no_elem(model_or_pk)
+            return self.gm_no_elem(model_or_pk)
 
     def show_list(self, page=0, per_page=10, columns=1, *args, **kwargs):
         """show list items"""
         page = int(page)
 
         # generate content
         count_models, page_models, first_this_page, first_next_page = self.show_list_get_queryset(
@@ -282,15 +294,15 @@
         if self.queryset._result_cache:
             self.queryset._result_cache = None
             self.queryset._prefetch_done = False
         return self.queryset
 
     def create_or_update_helper(self, field, value, func_response='create', instance=None, initial_data=None):
         # init data
-        is_multichoice_field = self.telega_form.base_fields[field].__class__ == ModelMultipleChoiceField if field else False
+        is_multichoice_field = self.model_form.base_fields[field].__class__ == ModelMultipleChoiceField if field else False
         show_field_variants_for_update = (func_response == 'change') and (value is None) and (self.update.message is None)
         want_1more_variant_for_multichoice = True
         want_write_self_variant = False
         data = {} if initial_data is None else copy.deepcopy(initial_data)
 
         # understanding what user has sent
         if (type(field) == str) and field:
@@ -318,47 +330,47 @@
             'data': data,
         }
         instance_id = None
         if instance:
             form_kwargs['instance'] = instance
             instance_id = instance.pk
 
-        self.form = self.telega_form(**form_kwargs)
+        self.form = self.model_form(**form_kwargs)
         form = self.form
 
         # show message or change data in backend...
         if want_write_self_variant:
-            res = self.generate_message_self_variant(field, func_response=func_response, instance_id=instance_id)
+            res = self.gm_self_variant(field, func_response=func_response, instance_id=instance_id)
         else:
             if not form.is_valid():
-                res = self.generate_message_value_error(
+                res = self.gm_value_error(
                     field or list(form.fields.keys())[-1],
                     form.errors, func_response=func_response, instance_id=instance_id
                 )
             else:
                 if not show_field_variants_for_update:
                     # todo: rewrite as is_completed will work only form ModelForm
                     form.save(is_completed=not want_1more_variant_for_multichoice)
 
                 if want_1more_variant_for_multichoice or show_field_variants_for_update:
-                    res = self.generate_message_next_field(
+                    res = self.gm_next_field(
                         field,
                         func_response=func_response,
                         instance_id=instance_id
                     )
 
                 elif form.next_field:
-                    res = self.generate_message_next_field(
+                    res = self.gm_next_field(
                         form.next_field,
                         func_response=func_response,
                         instance_id=instance_id
                     )
                 else:
                     if func_response == 'create':
-                        res = self.generate_message_success_created(self.form.instance)
+                        res = self.gm_success_created(self.form.instance)
                     else:
                         res = self.show_elem(self.form.instance, _('The field has been updated!\n\n'))
         return res
 
     def show_list_get_queryset(self, page=0, per_page=10, columns=1, *args, **kwargs):
         count_models = self.get_queryset().count()
         first_this_page = page * per_page * columns
@@ -379,26 +391,26 @@
     def gm_show_elem_create_buttons(self, model, elem_per_raw=2):
 
         buttons = []
         if 'change' in self.actions:
             if type(self.updating_fields) == list and len(self.updating_fields):
                 updating_fields = self.updating_fields
             else:
-                updating_fields = list(self.telega_form.base_fields.keys())
+                updating_fields = list(self.model_form.base_fields.keys())
 
             raw_elems = []
             for field in updating_fields:
-                if type(self.telega_form.base_fields[field].widget) != HiddenInput:
+                if type(self.model_form.base_fields[field].widget) != HiddenInput:
                     if len(raw_elems) >= elem_per_raw:
                         buttons.append(raw_elems)
                         raw_elems = []
 
                     raw_elems.append(
                         inlinebutt(
-                            text=f'🔄 {self.telega_form.base_fields[field].label}',
+                            text=f'🔄 {self.model_form.base_fields[field].label}',
                             callback_data=self.generate_message_callback_data(
                                 self.command_routings['command_routing_change'],
                                 model.id,
                                 field,
                             )
                         )
                     )
@@ -436,15 +448,15 @@
         :return:
         """
 
         if 'full_show' in kwargs:
             is_elem = kwargs['full_show']
 
         mess = ''
-        for field_name, field in self.telega_form.base_fields.items():
+        for field_name, field in self.model_form.base_fields.items():
             if type(field.widget) != HiddenInput:
                 mess += f'<b>{field.label}</b>: {self.gm_value_str(model, field, field_name)}\n'
 
         return mess
 
     def gm_value_str(self, model, field, field_name, try_field='name'):
         value = getattr(model, field_name, "")
@@ -466,15 +478,15 @@
             choice = list(filter(lambda x: x[0] == value, choices))
             if len(choice):
                 value = choice[0][1]
         return value
 
     def gm_show_list_elem_info(self, model, it_m:int) -> str:
         mess = f'{it_m}. {self.viewset_name} #{model.pk}\n' if self.use_name_and_id_in_elem_showing else f'{it_m}. '
-        mess += self.generate_show_fields(model)
+        mess += self.gm_show_elem_or_list_fields(model)
         mess += '\n\n'
         return mess
 
     def gm_show_list_button_names(self, it_m, model):
         return f'{it_m}. {self.viewset_name} #{ model.pk}'
 
     def gm_show_list_create_pagination(
@@ -534,17 +546,17 @@
             func_response,
             choices,
             selected_variants,
             callback_path,
             self_variant=True,
             show_next_button=True,
     ):
-        is_boolean_field = issubclass(type(self.telega_form.base_fields[next_field]), BooleanField)
-        is_choice_field = issubclass(type(self.telega_form.base_fields[next_field]), ChoiceField)
-        is_multichoice_field = self.telega_form.base_fields[next_field].__class__ == ModelMultipleChoiceField
+        is_boolean_field = issubclass(type(self.model_form.base_fields[next_field]), BooleanField)
+        is_choice_field = issubclass(type(self.model_form.base_fields[next_field]), ChoiceField)
+        is_multichoice_field = self.model_form.base_fields[next_field].__class__ == ModelMultipleChoiceField
 
         buttons = list([
             [inlinebutt(
                 text=text if not value in selected_variants else f'✅ {text}',
                 callback_data=callback_path(value)
             )] for value, text in choices
         ])
@@ -557,36 +569,36 @@
             buttons.append([
                 inlinebutt(text=_('Next'), callback_data=callback_path(self.GO_NEXT_MULTICHOICE_SYMBOLS))
             ])
         return buttons
 
     def gm_next_field(self, next_field, mess='', func_response='create', instance_id=None):
 
-        is_choice_field = issubclass(type(self.telega_form.base_fields[next_field]), ChoiceField)
+        is_choice_field = issubclass(type(self.model_form.base_fields[next_field]), ChoiceField)
 
         if is_choice_field or self.prechoice_fields_values.get(next_field):
             buttons = []
-            field = self.telega_form.base_fields[next_field]
+            field = self.model_form.base_fields[next_field]
 
-            mess += self.show_texts_dict['generate_message_next_field'] % {'label': field.label}
+            mess += self.show_texts_dict['gm_next_field'] % {'label': field.label}
             if field.help_text:
                 mess += f'{field.help_text}\n\n'
 
             if instance_id:
                 callback_path = lambda x: self.generate_message_callback_data(
                     self.command_routings[f'command_routing_{func_response}'], instance_id, next_field, x
                 )
             else:
                 callback_path = lambda x: self.generate_message_callback_data(
                     self.command_routings[f'command_routing_{func_response}'], next_field, x
                 )
             # todo: add beautiful text view
 
             choices = self.prechoice_fields_values.get(next_field) or \
-                      list(filter(lambda x: x[0], self.telega_form.base_fields[next_field].choices))
+                      list(filter(lambda x: x[0], self.model_form.base_fields[next_field].choices))
 
             selected_variants = []
             if self.form and self.form.is_valid() and next_field in self.form.cleaned_data:
                 field_value = self.form.cleaned_data[next_field]
                 selected_variants = [field_value]
 
                 if field_value:
@@ -597,22 +609,22 @@
                         selected_variants = [field_value.pk]
                     elif (type(field_value) in [set, list, models.QuerySet]):
                         if all(map(lambda x: issubclass(x.__class__, models.Model), field_value)):
                             selected_variants = list([el.pk for el in field_value])
                         else:
                             selected_variants = field_value
 
-            buttons += self.generate_message_next_field_choice_buttons(
+            buttons += self.gm_next_field_choice_buttons(
                 next_field, func_response, choices, selected_variants, callback_path
             )
 
             # required=False also for multichoice field or field with default value,
             # so it is better create button in app logic.
 
-            # if not self.telega_form.base_fields[next_field].required:
+            # if not self.model_form.base_fields[next_field].required:
             #     buttons.append([
             #         inlinebutt(
             #             text=self.show_texts_dict['leave_blank_button_text'],
             #             callback_data=callback_path(self.NONE_VARIANT_SYMBOLS)
             #         )
             #     ])
 
@@ -625,35 +637,35 @@
                         self.command_routings[f'command_routing_show_elem'],
                         instance_id
                     )
                 )])
 
             return self.CHAT_ACTION_MESSAGE, (mess, buttons)
         else:
-            return self.generate_message_self_variant(next_field, mess, func_response=func_response, instance_id=instance_id)
+            return self.gm_self_variant(next_field, mess, func_response=func_response, instance_id=instance_id)
 
     def gm_success_created(self, model_or_pk=None, mess=''):
 
-        mess += self.show_texts_dict['generate_message_success_created'] % {'viewset_name': self.viewset_name}
+        mess += self.show_texts_dict['gm_success_created'] % {'viewset_name': self.viewset_name}
 
         if model_or_pk:
             return self.show_elem(model_or_pk, mess)
         return self.CHAT_ACTION_MESSAGE, (mess, [])
 
     def gm_value_error(self, field_name, errors, mess='', func_response='create', instance_id=None):
-        field = self.telega_form.base_fields[field_name]
-        mess += self.show_texts_dict['generate_message_value_error'] % {'label': field.label, 'errors': errors}
+        field = self.model_form.base_fields[field_name]
+        mess += self.show_texts_dict['gm_value_error'] % {'label': field.label, 'errors': errors}
 
         # error could be only in self_variant?
-        return self.generate_message_self_variant(field_name, mess, func_response=func_response, instance_id=instance_id)
+        return self.gm_self_variant(field_name, mess, func_response=func_response, instance_id=instance_id)
 
     def gm_self_variant(self, field_name, mess='', func_response='create', instance_id=None):
-        field = self.telega_form.base_fields[field_name]
+        field = self.model_form.base_fields[field_name]
 
-        mess += self.show_texts_dict['generate_message_self_variant'] % {'label': field.label}
+        mess += self.show_texts_dict['gm_self_variant'] % {'label': field.label}
 
         if field.help_text:
             mess += f'{field.help_text}\n\n'
 
         if instance_id:
             current_utrl = self.generate_message_callback_data(
                 self.command_routings[f'command_routing_{func_response}'],
@@ -668,15 +680,15 @@
 
         self.user.current_utrl = current_utrl
         self.user.save()
 
         # add return buttons
         buttons = []
 
-        if not self.telega_form.base_fields[field_name].required:
+        if not self.model_form.base_fields[field_name].required:
             if func_response == 'create':
                 button_args = [func_response, field_name, self.NONE_VARIANT_SYMBOLS]
             else:
                 button_args = [func_response, instance_id, field_name, self.NONE_VARIANT_SYMBOLS]
 
             buttons.append([
                 inlinebutt(
@@ -695,15 +707,15 @@
                     self.command_routings[f'command_routing_show_elem'],
                     instance_id
                 )
             )])
         return self.CHAT_ACTION_MESSAGE, (mess, buttons)
 
     def gm_no_elem(self, model_id):
-        mess = self.show_texts_dict['generate_message_no_elem'] % {
+        mess = self.show_texts_dict['gm_no_elem'] % {
             'viewset_name': self.viewset_name,
             'model_id': model_id,
         }
         return self.CHAT_ACTION_MESSAGE, (mess, [])
 
     def gm_delete_getting_confirmation(self, model):
         mess = self.show_texts_dict['confirm_deleting'] % {
@@ -746,23 +758,10 @@
                     callback_data=self.generate_message_callback_data(
                         self.command_routings['command_routing_show_list'],
                     )
                 )]
             ]
         return mess, buttons
 
-    # for supporting legacy
-    _get_elem = get_orm_model
-    generate_message_no_elem = gm_no_elem
-    generate_message_self_variant = gm_self_variant
-    generate_message_value_error = gm_value_error
-    generate_message_success_created = gm_success_created
-    generate_message_next_field = gm_next_field
-    generate_message_next_field_choice_buttons = gm_next_field_choice_buttons
-    generate_elem_buttons = gm_show_elem_create_buttons
-    generate_show_fields = gm_show_elem_or_list_fields
-    generate_value_str = gm_value_str
-
 
-TelegaViewSet = TelegramViewSet  # for legacy
```

### Comparing `telegram_django_bot-1.0.2/telegram_django_bot/telegram_lib_redefinition.py` & `telegram_django_bot-1.1.0/telegram_django_bot/telegram_lib_redefinition.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.2/telegram_django_bot/templates/dropdown_filter1.html` & `telegram_django_bot-1.1.0/telegram_django_bot/templates/dropdown_filter1.html`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.2/telegram_django_bot/test.py` & `telegram_django_bot-1.1.0/telegram_django_bot/test.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.2/telegram_django_bot/tg_dj_bot.py` & `telegram_django_bot-1.1.0/telegram_django_bot/tg_dj_bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,34 +230,34 @@
                     response = bot.send_media_group(
                         chat_id,
                         media=media_files_list,
 
                     )
                 else:
                     if message_format == MESSAGE_FORMAT.PHOTO:
-                        telega_func = bot.send_photo
+                        telegram_func = bot.send_photo
                     elif message_format == MESSAGE_FORMAT.AUDIO:
-                        telega_func = bot.send_audio
+                        telegram_func = bot.send_audio
                     elif message_format == MESSAGE_FORMAT.VIDEO:
-                        telega_func = bot.send_video
+                        telegram_func = bot.send_video
                     elif message_format == MESSAGE_FORMAT.GIF:
-                        telega_func = bot.send_animation
+                        telegram_func = bot.send_animation
                     elif message_format == MESSAGE_FORMAT.VIDEO_NOTE:
-                        telega_func = bot.send_video_note
+                        telegram_func = bot.send_video_note
                     elif message_format == MESSAGE_FORMAT.VOICE:
-                        telega_func = bot.send_voice
+                        telegram_func = bot.send_voice
                     elif message_format == MESSAGE_FORMAT.STICKER:
-                        telega_func = bot.send_sticker
+                        telegram_func = bot.send_sticker
                     elif message_format == MESSAGE_FORMAT.LOCATION:
                         raise NotImplementedError()
                     # elif message_format == MESSAGE_FORMAT.DOCUMENT:
                     else:
-                        telega_func = bot.send_document
+                        telegram_func = bot.send_document
 
-                    response = telega_func(
+                    response = telegram_func(
                         chat_id,
                         media_files_list[0],
                         caption=text,
                         **telegram_message_kwargs
                     )
 
         media_files_codes = []
```

### Comparing `telegram_django_bot-1.0.2/telegram_django_bot/user_viewset.py` & `telegram_django_bot-1.1.0/telegram_django_bot/user_viewset.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from django.contrib.auth import get_user_model
 from django.conf import settings
 from django.utils.translation import gettext_lazy as _
 from django.utils import translation
 
-from .forms import TelegaModelForm, BaseModelForm, BaseTelegramForm
-from .td_viewset import TelegaViewSet
+from .forms import TelegramModelForm, BaseModelForm, BaseTelegramForm
+from .td_viewset import TelegramViewSet
 
 
 
-class UserForm(TelegaModelForm):
+class UserForm(TelegramModelForm):
     form_name = _('User')
 
     class Meta:
         model = get_user_model()
 
         fields = ['timezone', 'telegram_language_code', ]
 
@@ -32,19 +32,19 @@
             if settings.USE_I18N:
                 translation.activate(self.user.language_code)
         else:
             BaseTelegramForm.save(self, commit=commit)
 
 
 
-class UserViewSet(TelegaViewSet):
+class UserViewSet(TelegramViewSet):
     actions = ['change', 'show_elem']
 
     queryset = get_user_model().objects.all()
-    telega_form = UserForm
+    model_form = UserForm
     use_name_and_id_in_elem_showing = False
 
     prechoice_fields_values = {
         "timezone": list([(f'{tm}:0:0', f'+{tm} UTC' if tm > 0 else f'{tm} UTC') for tm in range(-11, 13)]),
         "telegram_language_code": settings.LANGUAGES,
     }
 
@@ -52,19 +52,19 @@
         return super().get_queryset().filter(id=self.user.id)
 
     def show_elem(self, model_id=None, mess=''):
         _, (mess, buttons) = super().show_elem(self.user.id, mess)
 
         return self.CHAT_ACTION_MESSAGE, (mess, buttons)
 
-    def generate_value_str(self, model, field, field_name, try_field='name'):
+    def gm_value_str(self, model, field, field_name, try_field='name'):
         if field_name == 'timezone':
             value = getattr(model, field_name, "")
             value = int(value.total_seconds() // 3600)
             return f'+{value} UTC' if value > 0 else f'{value} UTC'
 
         else:
-            return super().generate_value_str(model, field, field_name, try_field)
+            return super().gm_value_str(model, field, field_name, try_field)
 
-    def generate_message_next_field_choice_buttons(self, *args, **kwargs):
+    def gm_next_field_choice_buttons(self, *args, **kwargs):
         kwargs['self_variant'] = False
-        return super().generate_message_next_field_choice_buttons(*args, **kwargs)
+        return super().gm_next_field_choice_buttons(*args, **kwargs)
```

### Comparing `telegram_django_bot-1.0.2/telegram_django_bot/utils.py` & `telegram_django_bot-1.1.0/telegram_django_bot/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -140,20 +140,22 @@
 
 
 
 # todo: rewrite code
 # ButtonPagination WITHOUT WARRANTY
 class ButtonPagination:
     """
-    buttons -- массив кнопок с значением, которые отображать, формат кнопок:
+    construct several pages with buttons
+
+    buttons -- array of buttons with values for display to user, button format:
         [text; value]
-    selected_buttons -- выбранные кнопки в таком же формате
-    header_buttons -- кнопки, которые закреплены сверху на каждой странице и могут вести в другое местое, формат:
-       [text; value; callback_prefix]  -- callback_prefix=None тогда береться self.callback_prefix
-    footer_buttons -- аналогично header_buttons
+    selected_buttons -- selected buttons (add icon)
+    header_buttons -- buttons in the header for navigation or other cases, format:
+       [text; value; callback_prefix]  -- if callback_prefix=None then self.callback_prefix is selected
+    footer_buttons -- same as header_buttons, but in the footer
 
     """
 
     def __init__(
             self,
             callback_prefix,
             buttons=None,
@@ -161,15 +163,15 @@
             callback_prefix_context_values=None,
             rows=8,
             columns=1,
     ):
         self.SELECTED_TICK = '✅ '
         self.PREV_PAGE_STR = '⏮'
         self.NEXT_PAGE_STR = '⏭'
-        self.PAGE_CALLBACK_SYMBOL = 'telega_p'
+        self.PAGE_CALLBACK_SYMBOL = 'telegram_p'
 
         self.callback_prefix = callback_prefix
         self.buttons = buttons
         self.callback_prefix_context_values = callback_prefix_context_values
         self.selected_values = selected_values
         self.rows = rows
         self.columns = columns
@@ -183,40 +185,42 @@
         context_callback = ''
         if self.callback_prefix_context_values:
             context_callback = '-'.join(map(str, self.callback_prefix_context_values)) + '-'
         return self.callback_prefix + context_callback
 
     def value_page(self, value):
         """
-        выбирает какую страницу отобразить по дефолту
-        :param value:  значени кнопки
+        select the default page for display
+
+        :param value: ???
         :return:
         """
 
         selected_item_index = list(
             map(lambda x: x[1], self.buttons)
         ).index(value)
         return selected_item_index // self.buttons_per_page
 
     def _select_page_buttons(self, page_num):
         """
-        выбирает какие кнопки с значениями выбрать
-        :param page_num: Если None, то вызывает _select_page
+        select buttons for display on the page_num page. Func is created for easy logic redefinition.
+        :param page_num: if None, then  _select_page is called
         :return:
         """
         return self.buttons[page_num * self.buttons_per_page: (page_num + 1) * self.buttons_per_page]
 
     def construct_inline_curr_page(self, page_num=None, ):
         """
-        Cтроит inline кнопки (в переписке, не в меню) в формате телеграмм
+        Created  inline buttons
+
         :param page_num:
         :return:
         """
 
-        telega_buttons = []
+        telegram_buttons = []
         if page_num is None:
             if self.selected_values:
                 page_num = self.value_page(self.selected_values[0])
             else:
                 page_num = 0
 
         value_buttons = self._select_page_buttons(page_num)
@@ -228,18 +232,18 @@
                 button_text += self.SELECTED_TICK
 
             button_text += button[0]
             button_telegram = inlinebutt(button_text, callback_data=self.full_callback_prefix + button[1])
 
             if col_index == 0:
                 # new row
-                telega_buttons.append([button_telegram])
+                telegram_buttons.append([button_telegram])
             else:
                 # add in last row
-                telega_buttons[-1].append(button_telegram)
+                telegram_buttons[-1].append(button_telegram)
 
             col_index += 1
             if col_index == self.columns:
                 col_index = 0
 
         # neighbor pages
         neighbor_buttons = []
@@ -250,17 +254,17 @@
             )
         if page_num < int(len(self.buttons) / self.buttons_per_page + 0.9999) - 1:
             callback_data = self.full_callback_prefix + self.PAGE_CALLBACK_SYMBOL + str(page_num + 1)
             neighbor_buttons.append(
                 inlinebutt(self.NEXT_PAGE_STR, callback_data=callback_data)
             )
         if neighbor_buttons:
-            telega_buttons.append(neighbor_buttons)
+            telegram_buttons.append(neighbor_buttons)
 
-        return telega_buttons
+        return telegram_buttons
 
 
 class CalendarPagination:
     def __init__(
             self,
             callback_prefix,
             curr_month,
```

### Comparing `telegram_django_bot-1.0.2/telegram_django_bot.egg-info/PKG-INFO` & `telegram_django_bot-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: telegram-django-bot
-Version: 1.0.2
-Summary: Telegram Django Bot Bridge
-Home-page: https://github.com/alexanderaleskin/telegram_django_bot_bridge
+Name: telegram_django_bot
+Version: 1.1.0
+Summary: Telegram Django Bot
+Home-page: https://github.com/alexanderaleskin/telegram_django_bot
 Author: Alexander Aleskin
 Author-email: alexanderaleskin@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
@@ -25,20 +25,20 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Internet
 Requires-Python: >=3.8
 License-File: LICENSE
 
-Telegram Django Bot Bridge
+Telegram Django Bot
 ============================
 
 This library provides a Python high-level interface for creating Telegram Bots. It standardizes the coding in the best
 practice of the web development. The library is based on `Django <https://www.djangoproject.com/>`_ and `Python-Telegram-Bot <https://python-telegram-bot.org/>`_.
-and provides viewset interface for managing data with.
+It also provides viewset interface for managing data with.
 
 If you start a new project, you could use `Telegram django bot template <https://github.com/alexanderaleskin/telergam_django_bot_template>`_ with preconfigured settings.
 
 Install
 ------------
 
 You can install via ``pip``:
@@ -76,15 +76,15 @@
   Not necessary, but useful settings:
 
 * ``TELEGRAM_TOKEN`` - for adding "triggers",
 * ``TELEGRAM_TEST_USER_IDS`` - for adding tests for your bot,
 * Make sure, that ``LANGUAGE_CODE``, ``LANGUAGE_CODE``, ``USE_I18N`` are also used in the library for language localization.
 
 
-4. This step connects ``Telegram Django Bot Bridge`` with ``Python-Telegram-Bot``. Add ``RouterCallbackMessageCommandHandler`` in handlers for using TELEGRAM_ROOT_UTRLCONF :
+4. This step connects ``Telegram Django Bot`` with ``Python-Telegram-Bot``. Add ``RouterCallbackMessageCommandHandler`` in handlers for using TELEGRAM_ROOT_UTRLCONF :
 
 .. code-block:: python
 
     updater = Updater(bot=TG_DJ_Bot(settings.TELEGRAM_TOKEN))
     updater.dispatcher.add_handler(RouterCallbackMessageCommandHandler())
 
 or in 20.x version :
@@ -110,36 +110,30 @@
 
 and Django:
 
 * Django ORM  (communication with Database);
 * Administration panel for management.
 
 
-Telegram Django Bot Bridge provides next special opportunities:
+Telegram Django Bot provides next special opportunities:
 
 * using Viewsets (typical action with model (create, update, list, delete));
 * using Django localization.
 * using function routing like urls routing in Django.
-
-And some extra useful staff:
-
 * creating general menu items with no-coding (through Django Admin Panel);
-* extra high-level Bot functions, such as a wrapper for sending delayed (or scheduled) messages;
-* creating tests;
 * collecting stats from user actions in the bot;
-* commonly used utilities.
-
+* other useful staff.
 
 
 The key feature of the lib is ``TelegramViewSet`` - a class for managing Django ORM model. It is designed in a
 similar way as `Django rest framework Viewset <https://www.django-rest-framework.org/api-guide/viewsets/>`_ , but has
-a significant difference: while DRF Viewset provides a response in serializable format (usually in json format) to frontend app, TelegaViewSet
+a significant difference: while DRF Viewset provides a response in serializable format (usually in json format) to frontend app, TelegramViewSet
 provides a response to the user in telegram interface in message format with buttons. So, you will manage data and receive
-responses in human format by executing TelegaViewSet method. The methods use some kind of templates for generating human
-responses (it is possible to overwrite these templates). By default, TelegaViewSet has 5 methods:
+responses in human format by executing TelegramViewSet method. The methods use some kind of templates for generating human
+responses (it is possible to overwrite these templates). By default, TelegramViewSet has 5 methods:
 
 * ``create`` - create a new instance of the specified ORM model;
 * ``change`` - update instance fields of specified ORM model;
 * ``show_elem`` - show fields of the element and buttons with actions of this instance;
 * ``show_list`` - show list of model elements (with pagination);
 * ``delete`` - delete the instance
 
@@ -161,35 +155,35 @@
 
 .. code-block:: python
 
     from telegram_django_bot import forms as td_forms
     from telegram_django_bot.td_viewset import TelegramViewSet
 
 
-    class RequestForm(td_forms.TelegaModelForm):
+    class RequestForm(td_forms.TelegramModelForm):
         class Meta:
             model = Request
             fields = ['text', 'importance_level', 'project', 'tags']
 
 
     class RequestViewSet(TelegramViewSet):
-        telega_form = RequestForm
+        model_form = RequestForm
         queryset = Request.objects.all()
         viewset_name = 'Request'
 
 
 If you need, you can add extra actions to RequestViewSet for managing (see details information below) or change existing functions.
-There are several parameters and secondary functions in TelegaViewSet for customizing logic if it is necessary.
+There are several parameters and secondary functions in TelegramViewSet for customizing logic if it is necessary.
 
-In this example, ``TelegaModelForm`` was used. TelegaModelForm is a descendant of Django ModelForm. So, you could use
+In this example, ``TelegramModelForm`` was used. TelegramModelForm is a descendant of Django ModelForm. So, you could use
 labels, clean functions and other parameters and functions for managing logic and displaying.
 
 
-TelegaViewSet is designed to answer next user actions: clicking buttons and sometimes sending messages. The library imposes
-`Django URL notation <https://docs.djangoproject.com/en/4.1/topics/http/urls/>`_ for mapping user actions to TelegaViewSet methods (or usual handlers).
+TelegramViewSet is designed to answer next user actions: clicking buttons and sometimes sending messages. The library imposes
+`Django URL notation <https://docs.djangoproject.com/en/4.1/topics/http/urls/>`_ for mapping user actions to TelegramViewSet methods (or usual handlers).
 Usually, for correct mapping you just need to set ``TELEGRAM_ROOT_UTRLCONF`` and use ``RouterCallbackMessageCommandHandler`` in
 dispatcher as it is mentioned above in the *Install paragraph*.
 
 For correct mapping *RequestViewSet*  you should write in the TELEGRAM_ROOT_UTRLCONF file something like this:
 
 .. code-block:: python
 
@@ -266,15 +260,15 @@
          dp=updater.dispatcher
          dp.add_handler(RouterCallbackMessageCommandHandler())
 
 
 The example adds 1 super handler ``RouterCallbackMessageCommandHandler``, which allows you to write handlers
 in the style of handling link requests in the same way as it is done in ``Django``. ``RouterCallbackMessageCommandHandler`` allows you to handle
 messages, user commands and button clicks by users. In other words, it replaces the handlers
-``MessageHandler, CommandHandler, CallbackQueryHandler`` . Since the ``Telegram Django Bot Bridge`` library is an extension,
+``MessageHandler, CommandHandler, CallbackQueryHandler`` . Since the ``Telegram Django Bot`` library is an extension,
 it does not prohibit the use of standard handlers of the ``Python-Telegram-Bot`` library for handle user requests.
 (sometimes it is simply necessary, for example, if you need to process responses to surveys (you need to use PollAnswerHandler)).
 
 `Django notation <https://docs.djangoproject.com/en/4.1/topics/http/urls/>`_ of routing handlers is that paths to handlers are described in a separate file or files.
 As in the ``Django`` standard, the main file (root) for routing is specified in the project settings, where paths to handlers or paths to groups of handlers are stored.
 The ``TELEGRAM_ROOT_UTRLCONF`` (same as ``ROOT_URLCONF`` for WEB) attribute is used to specify the path to the file. In the example template, we have the following settings:
 
@@ -335,122 +329,122 @@
 This distribution of handlers allows you to group part of the handlers into modules and quickly connect or
 change them, while not being afraid of confusion which handlers need to be called, as it can be if all paths from
 different modules to handlers are described in one place as required by ``Python-Telegram-Bot``.
 
 In this example file ``base.utrls.py`` also ViewSets are used in addition to simple handler functions like ``def start`` and ``def some_debug_func``.
 ViewSet is an aggregator of several functions. The concept of it is that you quite often need to apply
 the same operations for a dataset, such as create, update, show, delete an example of dataset.
-There is the class ``telegram_django_bot.td_viewset.TelegaViewSet`` in the library  for such purposes. The class manages
-the Django ORM database model. ``TelegaViewSet`` has 5 functions for managing the model:
+There is the class ``telegram_django_bot.td_viewset.TelegramViewSet`` in the library  for such purposes. The class manages
+the Django ORM database model. ``TelegramViewSet`` has 5 functions for managing the model:
 
 
 ========= ======== ===========================
  Метод     UTRL      Description
 --------- -------- ---------------------------
 create     cr       Create model
 change     up       Change model attributes
 delete     de       Deleting a model
 show_elem  se       Display a model
 show_list  sl       Display a list of models
 ========= ======== ===========================
 
 Thus, if we want to call the ``BotMenuElemViewSet.create`` method to create an element, we need to use
 path 'sb/cr', whereby the first part of the path 'sb/'  the router ``RouterCallbackMessageCommandHandler`` will execute
-the ``BotMenuElemViewSet`` class, namely the ``TelegaViewSet.dispatch`` method, which in turn will call  the ``create`` method by analyzing the second part of the path
+the ``BotMenuElemViewSet`` class, namely the ``TelegramViewSet.dispatch`` method, which in turn will call  the ``create`` method by analyzing the second part of the path
 ``cr``.
 
 To sum up the scheme of handlers routing, there are following key points:
 
 1. ``telegram.ext.Update`` is used as a receiver of messages from Telegram;
-2. Standard handlers of the ``Python-Telegram-Bot`` library can be used as handlers. For convenient use Django's path scheme and ``TelegaViewSet`` you need to use ``RouterCallbackMessageCommandHandler``.
-3. ``TelegaViewSet`` aggregates a set of standard functions for managing data, what is made possible to group code associated with one type of data type in one class (place).
+2. Standard handlers of the ``Python-Telegram-Bot`` library can be used as handlers. For convenient use Django's path scheme and ``TelegramViewSet`` you need to use ``RouterCallbackMessageCommandHandler``.
+3. ``TelegramViewSet`` aggregates a set of standard functions for managing data, what is made possible to group code associated with one type of data type in one class (place).
 
 
 
 TelegramViewSet features
 ~~~~~~~~~~~~~~~~~~~~~~~~
 
-As described above, TelegaViewSet contains standard functions for data manipulation.
+As described above, TelegramViewSet contains standard functions for data manipulation.
 Due to such standard data processing methods, it turns out in the example to describe the logic of ``BotMenuElemViewSet`` in 40
 lines of code, also using some customization for beautiful data displaying.
 
 
-To use all the features of the TelegaViewSet in your class, it should be inherited from it, as, for example, this is done
+To use all the features of the TelegramViewSet in your class, it should be inherited from it, as, for example, this is done
 in the ``BotMenuElemViewSet``:
 
 
 .. code-block:: python
 
     from telegram_django_bot.td_viewset import TelegramViewSet
 
     class BotMenuElemViewSet(TelegramViewSet):
 
 
 In order to customize the ViewSet, you must specify 3 required attributes:
 
 1. ``viewset_name`` - class name, used to display to telegram users
-2. ``telega_form`` - data form, used to specify which fields of the ORM database model to use in the viewset;
+2. ``model_form`` - data form, used to specify which fields of the ORM database model to use in the viewset;
 3. ``queryset`` - basic query for getting model elements.
 
 
 The ``BotMenuElemViewSet`` is used the following values:
 
 .. code-block:: python
 
     from telegram_django_bot import forms as td_forms
     from telegram_django_bot.models import BotMenuElem
 
-    class BotMenuElemForm(td_forms.TelegaModelForm):
+    class BotMenuElemForm(td_forms.TelegramModelForm):
         form_name = _("Menu elem")
 
         class Meta:
             model = BotMenuElem
             fields = ['command', "is_visable", "callbacks_db", "message", "buttons_db"]
 
-    class BotMenuElemViewSet(TelegaViewSet):
+    class BotMenuElemViewSet(TelegramViewSet):
         viewset_name = 'BotMenuElem'
-        telega_form = BotMenuElemForm
+        model_form = BotMenuElemForm
         queryset = BotMenuElem.objects.all()
 
 
 where ``BotMenuElemForm`` is a descendant of the ``Django ModelFrom`` class, so it has a similar structure and parameterization methods.
 `` form_name ``  stands for the name of the form and is used in some messages sent to Telegram users.
 
 
-TelegaViewSet has quite a lot in common with Viewset analogs tailored for WEB development (for example,
-`django-rest-framework viewsets <https://www.django-rest-framework.org/api-guide/viewsets/>`_ ). However, as part of the development of Telegram bots, TelegaViewSet
+TelegramViewSet has quite a lot in common with Viewset analogs tailored for WEB development (for example,
+`django-rest-framework viewsets <https://www.django-rest-framework.org/api-guide/viewsets/>`_ ). However, as part of the development of Telegram bots, TelegramViewSet
 has some special features:
 
 1. An unusual way to create elements;
 2. The display of information in bots is limited and most often comes down to displaying text and buttons, so the viewset in addition to business logic includes the creation of standard responses to user actions in the form of messages with buttons.
 
 
 
 Forms
 ************
 
 
 Since Telegram does not have the ability to create forms (in the classic Web sense) and communication between the bot and the user takes place in a chat, then
 the most intuitive solution for filling out a form (creating an element) is filling the form attribute by attribute,
 when the first element of the form is filled first, then the second, and so on. With this approach, it is necessary to use temporary storage for remembering
-specified values in order to create an element from the form at the end. ``TelegaModelForm`` and ``TelegaForm`` are implemented just
+specified values in order to create an element from the form at the end. ``TelegramModelForm`` and ``TelegramForm`` are implemented just
 in such way for taking over this process. The difference between these classes and the standard Django classes is precisely
 in the modification of the method of filling in the form fields, otherwise they do not differ from standard forms.
 
-``TelegaModelForm`` and ``TelegaForm`` as Django descendants of ``ModelForm`` and ``Form`` have the following parameters, which you may need to customize:
+``TelegramModelForm`` and ``TelegramForm`` as Django descendants of ``ModelForm`` and ``Form`` have the following parameters, which you may need to customize:
 
 1. The clean function and other `form validation process functions <https://docs.djangoproject.com/en/4.1/ref/forms/validation/>`_ ;
 2. ``labels`` - field names;
-3. ``forms.HiddenInput`` - designation of hidden fields (hiding fields allows them not to be shown to the user, while using and configuring in forms or in ``TelegaViewSet``).
+3. ``forms.HiddenInput`` - designation of hidden fields (hiding fields allows them not to be shown to the user, while using and configuring in forms or in ``TelegramViewSet``).
 
 
 
-``TelegaViewSet`` is designed to interact with descendants of the ``TelegaModelForm`` class and allows you to use
+``TelegramViewSet`` is designed to interact with descendants of the ``TelegramModelForm`` class and allows you to use
 generate forms with different fields, such as ``CharField, IntegerField`` or ``ForeignKey, ManyToManyField``. Also, it is a good idea
-to use the ``prechoice_fields_values`` dictionary in ``TelegaViewSet`` descendants for improving the convenience of filling out forms for users.
+to use the ``prechoice_fields_values`` dictionary in ``TelegramViewSet`` descendants for improving the convenience of filling out forms for users.
 It is possible to store a list of frequently used values of form fields in the ``prechoice_fields_values``.
 This allows users to select the desired values by clicking buttons rather than
 writing text manually. The template has an example of using this field:
 
 
 .. code-block:: python
 
@@ -512,25 +506,25 @@
 
 Like a regular handler, the function takes 3 arguments as input: bot, update, user. After saving these arguments in class,
 the determination of the current routing path is occurred. It is determined either by pressing a button in the bot (the ``callback_data`` value of the button), or
 can be stored in the user attribute ``user.current_utrl``. The second option is possible if the user manually enters
 some information (for example, filled in a text field of form). After that, the arguments are extracted from the path
 to call a specific function. Storing and interacting with arguments in a path is similar to how ``sys.argv`` works. So,
 for example, the string ``"sl&1&20"`` will be converted to the list ``['sl', '1', '20']``. The separator character between attributes
-is ``&`` by default and can be changed via the ``TelegaViewSet.ARGS_SEPARATOR_SYMBOL`` variable.
+is ``&`` by default and can be changed via the ``TelegramViewSet.ARGS_SEPARATOR_SYMBOL`` variable.
 
-When using ``TelegaViewSet`` you most likely won't have to interact with the argument string directly, since
+When using ``TelegramViewSet`` you most likely won't have to interact with the argument string directly, since
 ``dispatch`` converts a string into arguments. And for creating a ``callback_data`` button string, that the user can call another method from Telegram interface, you should use
-``TelegaViewSet.gm_callback_data`` function. In case you need more low-level interaction with function arguments, then
+``TelegramViewSet.gm_callback_data`` function. In case you need more low-level interaction with function arguments, then
 you can use the ``construct_utrl`` and ``get_utrl_params`` functions.
 
 After receiving the utrl_args arguments and checking access rights, the managing method (action) is directly selected and called.
 The first argument, which is the short name for the function, is popped from the utrl_args. All other arguments are passed as parameters
 into a function. Inside the function, the necessary business logic and the data formatting for displaying to the user as a response take place.
-Any such managing function in the ``TelegaViewSet`` class must return the action type ``chat_action`` and the parameters to that action ``chat_action_args``.
+Any such managing function in the ``TelegramViewSet`` class must return the action type ``chat_action`` and the parameters to that action ``chat_action_args``.
 By default, the class has only 1 action ﹣ ``CHAT_ACTION_MESSAGE``, which means that the user will receive
 a text message (possibly with buttons) as an answer for his/her action. The arguments for this action are the text of the message and a list of buttons (can be None).
 
 
 After the function is processed, a response is sent to the user by ``send_answer`` function and the user's action is logged.
 
 
@@ -630,15 +624,15 @@
 However, these fields are not always enough and you need to redefine the logic of helper functions for a beautiful display of information.
 
 
 Helper functions for displaying data
 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 
-The ``TelegaViewSet`` class describes the following helper functions for generating a response message:
+The ``TelegramViewSet`` class describes the following helper functions for generating a response message:
 
 
 * ``def gm_no_elem`` - if no element with this ID was found;
 * ``def gm_success_created`` - successful creation of the model;
 * ``def gm_next_field`` - when moving to the next form attribute;
 * ``def gm_next_field_choice_buttons`` - generates buttons to select options for a specific form attribute (used inside ``gm_next_field``);
 * ``def gm_value_error`` - error output when adding a form attribute;
@@ -669,15 +663,15 @@
 
 * Getting or creating a user in the database;
 * In case of an error inside the handler function, returns an error message to the user;
 * Logs the handler call;
 * Tracks where the user came from;
 * Choice of language for sending messages to the user (in the case of localization enabled);
 
-This handler is also used inside ``RouterCallbackMessageCommandHandler``, and as a result in calling ``TelegaViewSet`` classes.
+This handler is also used inside ``RouterCallbackMessageCommandHandler``, and as a result in calling ``TelegramViewSet`` classes.
 
 Localization
 ~~~~~~~~~~~~~~~~
 
 The library expands the `Django localization tools <https://docs.djangoproject.com/en/4.1/topics/i18n/>`_ for use in Telegram.
 To support the use of different languages, the main elements of the Python-Telegram-Bot library are redefined in ``telegram_django_bot.telegram_lib_redefinition``:
 
@@ -687,48 +681,50 @@
 3. ``telegram.KeyboardButton`` -> ``telegram_django_bot.KeyboardButtonDJ`` ;
 4. ``telegram.InlineKeyboardButton`` -> ``telegram_django_bot.InlineKeyboardButtonDJ`` ;
 5. ``telegram.InlineKeyboardMarkup`` -> ``telegram_django_bot.InlineKeyboardMarkupDJ``.
 
 
 When using these classes in code, multilingual support comes down to the following steps:
 
+
 1. Specifying the necessary settings in the settings.py file: ``LANGUAGES`` - list of languages, ``LANGUAGE_CODE`` - default language;
-1. Necessary texts for translation are wrapped in ``gettext`` and ``gettext_lazy`` from ``django.utils.translation`` (how it works in Django `read here <https://docs.djangoproject.com/en /4.1/topics/i18n/translation/#standard-translation>`_ )
-2. Run command ``$ django-admin makemessages -a`` to generate texts for translation (created in locale folder)
-3. Generation of translation files ``$ django-admin compilemessages``.
+2. Create folder with translations: ``$ django-admin makemessages -l <language_code>``
+3. Necessary texts for translation are wrapped in ``gettext`` and ``gettext_lazy`` from ``django.utils.translation`` (how it works in Django `read here <https://docs.djangoproject.com/en /4.1/topics/i18n/translation/#standard-translation>`_ )
+4. Run command ``$ django-admin makemessages -a`` to update texts for translation (created in locale folder)
+5. Generation of translation files ``$ django-admin compilemessages``.
 
 Only a part of the functions uses localization in the template. It is made for easy understanding. The usage of localization can be seen in the example
 functions ``some_debug_func``.
 
 
 Extra lib features
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 The library provides some additional tools for the convenience of developing and managing the bot.
 
-Модели библиотеки
+Embedded ORM lib models
 ************************************
 
 
-For the correct work of ``TelegaViewSet`` and other components the Django ORM model representing the user in Telegram must be inherited
+For the correct work of ``TelegramViewSet`` and other components the Django ORM model representing the user in Telegram must be inherited
 from ``telegram_django_bot.models.TelegramUser``, as these components use its fields. ``TelegramUser`` inherited from
 ``django.contrib.auth.models.AbstractUser`` (which allows you to authorize users on the site if necessary) and has
 the following additional fields:
 
 * ``id`` - redefined to use user ID from telegrams;
 * ``seed_code`` - arbitrary value from 1 to 100 to randomly group users for tests and analysis;
 * ``telegram_username`` - username of the user in telegram;
 * ``telegram_language_code`` - telegram language code (some languages have dialects and as a result the code designation is more than 2 symbols);
 * ``timezone`` - the user's time zone (for determining the time);
-* ``current_utrl`` - path (utrl) of the last user action (used in ``TelegaViewSet``);
+* ``current_utrl`` - path (utrl) of the last user action (used in ``TelegramViewSet``);
 * ``current_utrl_code_dttm`` - time of the last action, when saving the path;
 * ``current_utrl_context_db`` - path context (utrl);
 * ``current_utrl_form_db`` - intermediate data for the form. Acts as a temporary data store when filling out a form;
 
-Fields ``current_utrl_<suffix>`` are needed for ``TelegaViewSet``, ``TelegaModelForm`` and are needed in exceptional cases
+Fields ``current_utrl_<suffix>`` are needed for ``TelegramViewSet``, ``TelegramModelForm`` and are needed in exceptional cases
 when writing code. The model also has the following methods (property) to simplify interaction with model fields:
 
 * ``current_utrl_form`` (property) - returns the current temporarily stored path form data (utrl);
 * ``current_utrl_context`` (property) - returns the current path context (utrl);
 * ``save_form_in_db`` - saves the form in the ``current_utrl_form_db`` field;
 * ``save_context_in_db`` - saves the context in the field ``current_utrl_context_db``;
 * ``clear_status`` - clears the data associated with the used path (fields ``current_utrl_<suffix>``) ;
@@ -771,25 +767,25 @@
 * ``telegram_django_bot.utils.CalendarPagination`` - class for generating a calendar with buttons;
 * ``telegram_django_bot.user_viewset.UserViewSet`` - telegram user class for changing language and time zone;
 
 
 Routing details
 ********************
 
-In this section, we will analyze the work of ``RouterCallbackMessageCommandHandler`` and ``telega_reverse`` in a little more detail.
+In this section, we will analyze the work of ``RouterCallbackMessageCommandHandler`` and ``telegram_reverse`` in a little more detail.
 
 As described earlier ``RouterCallbackMessageCommandHandler`` is used to be able to write handlers in the style
 Django. Also ``RouterCallbackMessageCommandHandler`` provides the ability to handle calls to ``BotMenuElem`` as
 through commands, and through callback. This is achieved by using the functions ``all_command_bme_handler`` and
 ``all_callback_bme_handler``. By default, ``BotMenuElem`` call handling is enabled and handled after
 no suitable path was found in the description of utrls (paths in Django notation). If there is no ``BotMenuElem`` element
 match is found, the ``BotMenuElem`` is considered to be configured incorrectly and an error message is returned to the user.
 You can create a class with the ``only_utrl=True`` attribute, what is disable calls to ``BotMenuElem``.
 
-The example template contains the use of the ``telega_reverse`` function, the essence of which is to generate a path (string) to the
+The example template contains the use of the ``telegram_reverse`` function, the essence of which is to generate a path (string) to the
 handler specified in the function argument. The function is analogous to the `reverse <https://docs.djangoproject.com/en/4.1/ref/urlresolvers/#reverse>`_ Django function
 and avoids errors when changing paths.
 
 
 
 Tests
 **********************
```

### Comparing `telegram_django_bot-1.0.2/telegram_django_bot.egg-info/SOURCES.txt` & `telegram_django_bot-1.1.0/telegram_django_bot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.2/tests/test_bme.py` & `telegram_django_bot-1.1.0/tests/test_bme.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.2/tests/test_routing.py` & `telegram_django_bot-1.1.0/tests/test_routing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,64 +1,64 @@
 import telegram
 
-from telegram_django_bot.routing import telega_resolve, telega_reverse, RouterCallbackMessageCommandHandler
+from telegram_django_bot.routing import telegram_resolve, telegram_reverse, RouterCallbackMessageCommandHandler
 from telegram_django_bot.test import TD_TestCase
 from telegram_django_bot.models import BotMenuElem, ActionLog
 from django.urls.exceptions import NoReverseMatch
 from django.conf import settings
 
 # import os, sys
 # sys.path.append(os.path.dirname(__file__))
 # print(sys.path, os.path.dirname(__file__))
 
 from test_app.models import User, Category
 from test_app.views import CategoryViewSet, EntityViewSet
 from test_app.handlers import me
 import unittest
 
-class TestTelegaResolve(TD_TestCase):
+class TestTelegramResolve(TD_TestCase):
     def test_exist(self):
-        res = telega_resolve('cat/se')
+        res = telegram_resolve('cat/se')
         self.assertEqual(CategoryViewSet, res.func)
 
-        res = telega_resolve('/cat/', utrl_conf='test_app.utrls')
+        res = telegram_resolve('/cat/', utrl_conf='test_app.utrls')
         self.assertEqual(CategoryViewSet, res.func)
 
-        res = telega_resolve('cat/up&1&2&3')
+        res = telegram_resolve('cat/up&1&2&3')
         self.assertEqual(CategoryViewSet, res.func)
 
-        res = telega_resolve('ent/cr&some_name&cat/')
+        res = telegram_resolve('ent/cr&some_name&cat/')
         self.assertEqual(EntityViewSet, res.func)
 
-        res = telega_resolve('start')
+        res = telegram_resolve('start')
         self.assertEqual(me, res.func)
 
 
     def test_not_exist(self):
-        self.assertIsNone(telega_resolve('abracadabra'))
-        self.assertIsNone(telega_resolve('cat'))
-        self.assertIsNone(telega_resolve('startstart/'))
+        self.assertIsNone(telegram_resolve('abracadabra'))
+        self.assertIsNone(telegram_resolve('cat'))
+        self.assertIsNone(telegram_resolve('startstart/'))
 
 
 
-class TestTelegaReverse(TD_TestCase):
+class TestTelegramReverse(TD_TestCase):
     def test_exist(self):
-        res = telega_reverse('CategoryViewSet')
+        res = telegram_reverse('CategoryViewSet')
         self.assertEqual('cat/', res)
 
-        res = telega_reverse('EntityViewSet')
+        res = telegram_reverse('EntityViewSet')
         self.assertEqual('ent/', res)
 
-        res = telega_reverse('self_info')
+        res = telegram_reverse('self_info')
         self.assertEqual('me', res)
 
     def test_not_exist(self):
         catched = False
         try:
-            telega_reverse('abracadabra')
+            telegram_reverse('abracadabra')
         except NoReverseMatch:
             catched = True
 
         self.assertTrue(catched)
```

### Comparing `telegram_django_bot-1.0.2/tests/test_td_bot.py` & `telegram_django_bot-1.1.0/tests/test_td_bot.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.2/tests/test_user.py` & `telegram_django_bot-1.1.0/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.2/tests/test_utils.py` & `telegram_django_bot-1.1.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.2/tests/test_viewset.py` & `telegram_django_bot-1.1.0/tests/test_viewset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from telegram_django_bot.test import TD_TestCase
-from telegram_django_bot.routing import telega_reverse, RouterCallbackMessageCommandHandler
+from telegram_django_bot.routing import telegram_reverse, RouterCallbackMessageCommandHandler
 from django.conf import settings
 
 from test_app.models import Entity, Order, Size, User, Category
 from test_app.views import CategoryViewSet, EntityViewSet, OrderViewSet
 
 import unittest
 import telegram
 
 
-class TestTelegaViewSet(TD_TestCase):
+class TestTelegramViewSet(TD_TestCase):
     def setUp(self) -> None:
         user_id = settings.TELEGRAM_TEST_USER_IDS[0]
         self.user = User.objects.create(id=user_id, username=user_id)
         self.cvs = CategoryViewSet(
-            telega_reverse('CategoryViewSet'),
+            telegram_reverse('CategoryViewSet'),
             user=self.user,
             bot=self.test_callback_context.bot
         )
         self.evs = EntityViewSet(
-            telega_reverse('EntityViewSet'),
+            telegram_reverse('EntityViewSet'),
             user=self.user,
             bot=self.test_callback_context.bot
         )
         self.ovs = OrderViewSet(
-            telega_reverse('OrderViewSet'),
+            telegram_reverse('OrderViewSet'),
             user=self.user,
             bot=self.test_callback_context.bot
         )
         # self.rc_mch = RouterCallbackMessageCommandHandler()
         # self.handle_update = lambda update: self.rc_mch.handle_update(
         #     update, 'some_str', 'some_str', self.test_callback_context
         # )
@@ -718,15 +718,15 @@
         res_message = self.handle_update(action_show_settings)
 
         buttons = res_message.reply_markup.to_dict()['inline_keyboard']
         self.assertEqual(buttons[0][0]['text'], '🔄 Timezone')
         self.assertEqual(buttons[0][0]['callback_data'], f'us/up&{self.user.id}&timezone')
         self.assertEqual(buttons[0][1]['text'], '🔄 Language')
         self.assertEqual(buttons[0][1]['callback_data'], f'us/up&{self.user.id}&telegram_language_code')
-        self.assertEqual(res_message.text, 'Timezone: 3:00:00\nLanguage: English')
+        self.assertEqual(res_message.text, 'Timezone: +3 UTC\nLanguage: English')
 
     def test_change_language(self):
         start = self.create_update({'text': '/start'})
         res_message = self.handle_update(start)
 
         action_change_timezone = self.create_update(
             res_message.to_dict(),
```

