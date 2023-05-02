# Comparing `tmp/automation_editor_dev-0.0.3.tar.gz` & `tmp/automation_editor_dev-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation_editor_dev-0.0.3.tar", last modified: Sun Apr 30 07:49:57 2023, max compression
+gzip compressed data, was "automation_editor_dev-0.0.4.tar", last modified: Tue May  2 09:40:06 2023, max compression
```

## Comparing `automation_editor_dev-0.0.3.tar` & `automation_editor_dev-0.0.4.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 07:49:57.208912 automation_editor_dev-0.0.3/
--rw-rw-rw-   0        0        0     1085 2023-04-05 12:50:43.000000 automation_editor_dev-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     5789 2023-04-30 07:49:57.203928 automation_editor_dev-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     5065 2023-04-29 11:09:10.000000 automation_editor_dev-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 07:49:56.526164 automation_editor_dev-0.0.3/automation_editor/
--rw-rw-rw-   0        0        0      130 2023-04-29 09:53:20.000000 automation_editor_dev-0.0.3/automation_editor/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor_dev-0.0.3/automation_editor/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:49:56.528160 automation_editor_dev-0.0.3/automation_editor/automation_editor_ui/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor_dev-0.0.3/automation_editor/automation_editor_ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:49:56.532148 automation_editor_dev-0.0.3/automation_editor/automation_editor_ui/editor_main/
--rw-rw-rw-   0        0        0        0 2023-04-24 10:50:57.000000 automation_editor_dev-0.0.3/automation_editor/automation_editor_ui/editor_main/__init__.py
--rw-rw-rw-   0        0        0     1323 2023-04-30 07:37:34.000000 automation_editor_dev-0.0.3/automation_editor/automation_editor_ui/editor_main/main_ui.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:49:56.535140 automation_editor_dev-0.0.3/automation_editor/automation_editor_ui/menu/
--rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor_dev-0.0.3/automation_editor/automation_editor_ui/menu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:49:56.557081 automation_editor_dev-0.0.3/automation_editor/automation_editor_ui/menu/api_testka_menu/
--rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor_dev-0.0.3/automation_editor/automation_editor_ui/menu/api_testka_menu/__init__.py
--rw-rw-rw-   0        0        0     3998 2023-04-29 10:27:21.000000 automation_editor_dev-0.0.3/automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:49:56.576030 automation_editor_dev-0.0.3/automation_editor/automation_editor_ui/menu/auto_control_menu/
--rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor_dev-0.0.3/automation_editor/automation_editor_ui/menu/auto_control_menu/__init__.py
--rw-rw-rw-   0        0        0     4129 2023-04-29 10:27:09.000000 automation_editor_dev-0.0.3/automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:49:56.605951 automation_editor_dev-0.0.3/automation_editor/automation_editor_ui/menu/load_density_menu/
--rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor_dev-0.0.3/automation_editor/automation_editor_ui/menu/load_density_menu/__init__.py
--rw-rw-rw-   0        0        0     4161 2023-04-29 10:27:56.000000 automation_editor_dev-0.0.3/automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:49:56.623903 automation_editor_dev-0.0.3/automation_editor/automation_editor_ui/menu/web_runner_menu/
--rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor_dev-0.0.3/automation_editor/automation_editor_ui/menu/web_runner_menu/__init__.py
--rw-rw-rw-   0        0        0     4040 2023-04-29 10:27:42.000000 automation_editor_dev-0.0.3/automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:49:56.638404 automation_editor_dev-0.0.3/automation_editor/automation_editor_ui/show_code_window/
--rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor_dev-0.0.3/automation_editor/automation_editor_ui/show_code_window/__init__.py
--rw-rw-rw-   0        0        0      791 2023-04-27 10:28:14.000000 automation_editor_dev-0.0.3/automation_editor/automation_editor_ui/show_code_window/code_window.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:49:56.667326 automation_editor_dev-0.0.3/automation_editor/automation_editor_ui/syntax/
--rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor_dev-0.0.3/automation_editor/automation_editor_ui/syntax/__init__.py
--rw-rw-rw-   0        0        0      777 2023-04-29 09:53:20.000000 automation_editor_dev-0.0.3/automation_editor/automation_editor_ui/syntax/syntax_extend.py
--rw-rw-rw-   0        0        0     3257 2023-04-27 10:28:14.000000 automation_editor_dev-0.0.3/automation_editor/automation_editor_ui/syntax/syntax_keyword.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:49:56.670319 automation_editor_dev-0.0.3/automation_editor/extend/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor_dev-0.0.3/automation_editor/extend/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:49:56.686277 automation_editor_dev-0.0.3/automation_editor/extend/mail_thunder_extend/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor_dev-0.0.3/automation_editor/extend/mail_thunder_extend/__init__.py
--rw-rw-rw-   0        0        0     1696 2023-04-29 09:53:20.000000 automation_editor_dev-0.0.3/automation_editor/extend/mail_thunder_extend/mail_thunder_setting.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:49:56.688271 automation_editor_dev-0.0.3/automation_editor/utils/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor_dev-0.0.3/automation_editor/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:49:56.728165 automation_editor_dev-0.0.3/automation_editor/utils/exception/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor_dev-0.0.3/automation_editor/utils/exception/__init__.py
--rw-rw-rw-   0        0        0     1500 2023-04-27 10:28:14.000000 automation_editor_dev-0.0.3/automation_editor/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0      608 2023-04-05 12:50:43.000000 automation_editor_dev-0.0.3/automation_editor/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:49:56.745634 automation_editor_dev-0.0.3/automation_editor/utils/file_process/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor_dev-0.0.3/automation_editor/utils/file_process/__init__.py
--rw-rw-rw-   0        0        0     1198 2023-04-27 10:28:14.000000 automation_editor_dev-0.0.3/automation_editor/utils/file_process/get_dir_file_list.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:49:56.762590 automation_editor_dev-0.0.3/automation_editor/utils/json_format/
--rw-rw-rw-   0        0        0        2 2023-04-05 12:50:43.000000 automation_editor_dev-0.0.3/automation_editor/utils/json_format/__init__.py
--rw-rw-rw-   0        0        0      991 2023-04-29 09:53:20.000000 automation_editor_dev-0.0.3/automation_editor/utils/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:49:56.765581 automation_editor_dev-0.0.3/automation_editor/utils/manager/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor_dev-0.0.3/automation_editor/utils/manager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:49:56.787523 automation_editor_dev-0.0.3/automation_editor/utils/manager/package_manager/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor_dev-0.0.3/automation_editor/utils/manager/package_manager/__init__.py
--rw-rw-rw-   0        0        0     1737 2023-04-28 11:00:21.000000 automation_editor_dev-0.0.3/automation_editor/utils/manager/package_manager/package_manager_class.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:49:56.834398 automation_editor_dev-0.0.3/automation_editor/utils/test_executor/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor_dev-0.0.3/automation_editor/utils/test_executor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:49:56.859845 automation_editor_dev-0.0.3/automation_editor/utils/test_executor/api_testka/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor_dev-0.0.3/automation_editor/utils/test_executor/api_testka/__init__.py
--rw-rw-rw-   0        0        0     3935 2023-04-29 09:53:20.000000 automation_editor_dev-0.0.3/automation_editor/utils/test_executor/api_testka/api_testka_process.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:49:56.886774 automation_editor_dev-0.0.3/automation_editor/utils/test_executor/auto_control/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor_dev-0.0.3/automation_editor/utils/test_executor/auto_control/__init__.py
--rw-rw-rw-   0        0        0     3939 2023-04-29 09:53:20.000000 automation_editor_dev-0.0.3/automation_editor/utils/test_executor/auto_control/auto_control_process.py
--rw-rw-rw-   0        0        0      498 2023-04-29 09:53:20.000000 automation_editor_dev-0.0.3/automation_editor/utils/test_executor/check_mail_thunder.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:49:56.934645 automation_editor_dev-0.0.3/automation_editor/utils/test_executor/load_density/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor_dev-0.0.3/automation_editor/utils/test_executor/load_density/__init__.py
--rw-rw-rw-   0        0        0     3949 2023-04-29 09:53:20.000000 automation_editor_dev-0.0.3/automation_editor/utils/test_executor/load_density/load_density_process.py
--rw-rw-rw-   0        0        0     5837 2023-04-28 11:00:21.000000 automation_editor_dev-0.0.3/automation_editor/utils/test_executor/task_process_manager.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:49:57.040362 automation_editor_dev-0.0.3/automation_editor/utils/test_executor/web_runner/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor_dev-0.0.3/automation_editor/utils/test_executor/web_runner/__init__.py
--rw-rw-rw-   0        0        0     3897 2023-04-29 09:53:20.000000 automation_editor_dev-0.0.3/automation_editor/utils/test_executor/web_runner/web_runner_process.py
-drwxrwxrwx   0        0        0        0 2023-04-30 07:49:57.198939 automation_editor_dev-0.0.3/automation_editor_dev.egg-info/
--rw-rw-rw-   0        0        0     5789 2023-04-30 07:49:56.000000 automation_editor_dev-0.0.3/automation_editor_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2951 2023-04-30 07:49:56.000000 automation_editor_dev-0.0.3/automation_editor_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 07:49:56.000000 automation_editor_dev-0.0.3/automation_editor_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-04-30 07:49:56.000000 automation_editor_dev-0.0.3/automation_editor_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-30 07:49:56.000000 automation_editor_dev-0.0.3/automation_editor_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1127 2023-04-30 07:49:28.000000 automation_editor_dev-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-30 07:49:57.208912 automation_editor_dev-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-02 09:40:06.142743 automation_editor_dev-0.0.4/
+-rw-rw-rw-   0        0        0     1085 2023-04-19 01:59:04.000000 automation_editor_dev-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     5889 2023-05-02 09:40:06.141748 automation_editor_dev-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5065 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 09:40:05.963169 automation_editor_dev-0.0.4/automation_editor/
+-rw-rw-rw-   0        0        0      130 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:40:05.965170 automation_editor_dev-0.0.4/automation_editor/automation_editor_ui/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/automation_editor_ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:40:05.971168 automation_editor_dev-0.0.4/automation_editor/automation_editor_ui/editor_main/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/automation_editor_ui/editor_main/__init__.py
+-rw-rw-rw-   0        0        0     1323 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/automation_editor_ui/editor_main/main_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:40:05.976134 automation_editor_dev-0.0.4/automation_editor/automation_editor_ui/menu/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/automation_editor_ui/menu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:40:05.983133 automation_editor_dev-0.0.4/automation_editor/automation_editor_ui/menu/api_testka_menu/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/automation_editor_ui/menu/api_testka_menu/__init__.py
+-rw-rw-rw-   0        0        0     3998 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:40:05.990876 automation_editor_dev-0.0.4/automation_editor/automation_editor_ui/menu/auto_control_menu/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/automation_editor_ui/menu/auto_control_menu/__init__.py
+-rw-rw-rw-   0        0        0     4129 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:40:05.997878 automation_editor_dev-0.0.4/automation_editor/automation_editor_ui/menu/load_density_menu/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/automation_editor_ui/menu/load_density_menu/__init__.py
+-rw-rw-rw-   0        0        0     4161 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:40:06.005295 automation_editor_dev-0.0.4/automation_editor/automation_editor_ui/menu/web_runner_menu/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/automation_editor_ui/menu/web_runner_menu/__init__.py
+-rw-rw-rw-   0        0        0     4040 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:40:06.012360 automation_editor_dev-0.0.4/automation_editor/automation_editor_ui/show_code_window/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/automation_editor_ui/show_code_window/__init__.py
+-rw-rw-rw-   0        0        0      791 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/automation_editor_ui/show_code_window/code_window.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:40:06.021488 automation_editor_dev-0.0.4/automation_editor/automation_editor_ui/syntax/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/automation_editor_ui/syntax/__init__.py
+-rw-rw-rw-   0        0        0      777 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/automation_editor_ui/syntax/syntax_extend.py
+-rw-rw-rw-   0        0        0     3257 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/automation_editor_ui/syntax/syntax_keyword.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:40:06.024491 automation_editor_dev-0.0.4/automation_editor/extend/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/extend/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:40:06.031501 automation_editor_dev-0.0.4/automation_editor/extend/mail_thunder_extend/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/extend/mail_thunder_extend/__init__.py
+-rw-rw-rw-   0        0        0     1696 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/extend/mail_thunder_extend/mail_thunder_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:40:06.034501 automation_editor_dev-0.0.4/automation_editor/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:40:06.044501 automation_editor_dev-0.0.4/automation_editor/utils/exception/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0     1500 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0      608 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:40:06.049610 automation_editor_dev-0.0.4/automation_editor/utils/file_process/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/utils/file_process/__init__.py
+-rw-rw-rw-   0        0        0     1198 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/utils/file_process/get_dir_file_list.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:40:06.056283 automation_editor_dev-0.0.4/automation_editor/utils/json_format/
+-rw-rw-rw-   0        0        0        2 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/utils/json_format/__init__.py
+-rw-rw-rw-   0        0        0      991 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/utils/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:40:06.059825 automation_editor_dev-0.0.4/automation_editor/utils/manager/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/utils/manager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:40:06.066798 automation_editor_dev-0.0.4/automation_editor/utils/manager/package_manager/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/utils/manager/package_manager/__init__.py
+-rw-rw-rw-   0        0        0     1737 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/utils/manager/package_manager/package_manager_class.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:40:06.078263 automation_editor_dev-0.0.4/automation_editor/utils/test_executor/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/utils/test_executor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:40:06.083263 automation_editor_dev-0.0.4/automation_editor/utils/test_executor/api_testka/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/utils/test_executor/api_testka/__init__.py
+-rw-rw-rw-   0        0        0     3935 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/utils/test_executor/api_testka/api_testka_process.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:40:06.089264 automation_editor_dev-0.0.4/automation_editor/utils/test_executor/auto_control/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/utils/test_executor/auto_control/__init__.py
+-rw-rw-rw-   0        0        0     3939 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/utils/test_executor/auto_control/auto_control_process.py
+-rw-rw-rw-   0        0        0      498 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/utils/test_executor/check_mail_thunder.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:40:06.097267 automation_editor_dev-0.0.4/automation_editor/utils/test_executor/load_density/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/utils/test_executor/load_density/__init__.py
+-rw-rw-rw-   0        0        0     3949 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/utils/test_executor/load_density/load_density_process.py
+-rw-rw-rw-   0        0        0     5837 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/utils/test_executor/task_process_manager.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:40:06.104261 automation_editor_dev-0.0.4/automation_editor/utils/test_executor/web_runner/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/utils/test_executor/web_runner/__init__.py
+-rw-rw-rw-   0        0        0     3897 2023-05-02 01:28:19.000000 automation_editor_dev-0.0.4/automation_editor/utils/test_executor/web_runner/web_runner_process.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:40:06.137451 automation_editor_dev-0.0.4/automation_editor_dev.egg-info/
+-rw-rw-rw-   0        0        0     5889 2023-05-02 09:40:05.000000 automation_editor_dev-0.0.4/automation_editor_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2951 2023-05-02 09:40:05.000000 automation_editor_dev-0.0.4/automation_editor_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 09:40:05.000000 automation_editor_dev-0.0.4/automation_editor_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-05-02 09:40:05.000000 automation_editor_dev-0.0.4/automation_editor_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-02 09:40:05.000000 automation_editor_dev-0.0.4/automation_editor_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1272 2023-05-02 09:39:45.000000 automation_editor_dev-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-02 09:40:06.143742 automation_editor_dev-0.0.4/setup.cfg
```

### Comparing `automation_editor_dev-0.0.3/LICENSE` & `automation_editor_dev-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.3/PKG-INFO` & `automation_editor_dev-0.0.4/automation_editor_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
-Name: automation_editor_dev
-Version: 0.0.3
+Name: automation-editor-dev
+Version: 0.0.4
 Summary: Automation Editor for GUI, WEB, API, Load Automation
-Author-email: JE-Chen <zenmailman@gmail.com>
+Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
-Project-URL: Homepage, https://github.com/JE-Chen/Integration-testing-environment
-Classifier: Programming Language :: Python :: 3.7
+Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/AutomationEditor
+Project-URL: Code, https://github.com/Intergration-Automation-Testing/AutomationEditor
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
 Classifier: Environment :: X11 Applications
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `automation_editor_dev-0.0.3/README.md` & `automation_editor_dev-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.3/automation_editor/automation_editor_ui/editor_main/main_ui.py` & `automation_editor_dev-0.0.4/automation_editor/automation_editor_ui/editor_main/main_ui.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.3/automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py` & `automation_editor_dev-0.0.4/automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.3/automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py` & `automation_editor_dev-0.0.4/automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.3/automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py` & `automation_editor_dev-0.0.4/automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.3/automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py` & `automation_editor_dev-0.0.4/automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.3/automation_editor/automation_editor_ui/show_code_window/code_window.py` & `automation_editor_dev-0.0.4/automation_editor/automation_editor_ui/show_code_window/code_window.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.3/automation_editor/automation_editor_ui/syntax/syntax_extend.py` & `automation_editor_dev-0.0.4/automation_editor/automation_editor_ui/syntax/syntax_extend.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.3/automation_editor/automation_editor_ui/syntax/syntax_keyword.py` & `automation_editor_dev-0.0.4/automation_editor/automation_editor_ui/syntax/syntax_keyword.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.3/automation_editor/extend/mail_thunder_extend/mail_thunder_setting.py` & `automation_editor_dev-0.0.4/automation_editor/extend/mail_thunder_extend/mail_thunder_setting.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.3/automation_editor/utils/exception/exception_tags.py` & `automation_editor_dev-0.0.4/automation_editor/utils/exception/exception_tags.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.3/automation_editor/utils/exception/exceptions.py` & `automation_editor_dev-0.0.4/automation_editor/utils/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.3/automation_editor/utils/file_process/get_dir_file_list.py` & `automation_editor_dev-0.0.4/automation_editor/utils/file_process/get_dir_file_list.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.3/automation_editor/utils/json_format/json_process.py` & `automation_editor_dev-0.0.4/automation_editor/utils/json_format/json_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.3/automation_editor/utils/manager/package_manager/package_manager_class.py` & `automation_editor_dev-0.0.4/automation_editor/utils/manager/package_manager/package_manager_class.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.3/automation_editor/utils/test_executor/api_testka/api_testka_process.py` & `automation_editor_dev-0.0.4/automation_editor/utils/test_executor/api_testka/api_testka_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.3/automation_editor/utils/test_executor/auto_control/auto_control_process.py` & `automation_editor_dev-0.0.4/automation_editor/utils/test_executor/auto_control/auto_control_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.3/automation_editor/utils/test_executor/load_density/load_density_process.py` & `automation_editor_dev-0.0.4/automation_editor/utils/test_executor/load_density/load_density_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.3/automation_editor/utils/test_executor/task_process_manager.py` & `automation_editor_dev-0.0.4/automation_editor/utils/test_executor/task_process_manager.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.3/automation_editor/utils/test_executor/web_runner/web_runner_process.py` & `automation_editor_dev-0.0.4/automation_editor/utils/test_executor/web_runner/web_runner_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.3/automation_editor_dev.egg-info/PKG-INFO` & `automation_editor_dev-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
-Name: automation-editor-dev
-Version: 0.0.3
+Name: automation_editor_dev
+Version: 0.0.4
 Summary: Automation Editor for GUI, WEB, API, Load Automation
-Author-email: JE-Chen <zenmailman@gmail.com>
+Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
-Project-URL: Homepage, https://github.com/JE-Chen/Integration-testing-environment
-Classifier: Programming Language :: Python :: 3.7
+Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/AutomationEditor
+Project-URL: Code, https://github.com/Intergration-Automation-Testing/AutomationEditor
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
 Classifier: Environment :: X11 Applications
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `automation_editor_dev-0.0.3/automation_editor_dev.egg-info/SOURCES.txt` & `automation_editor_dev-0.0.4/automation_editor_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `automation_editor_dev-0.0.3/pyproject.toml` & `automation_editor_dev-0.0.4/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -2,39 +2,46 @@
 # This is dev version
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "automation_editor_dev"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
-    { name = "JE-Chen", email = "zenmailman@gmail.com" },
+    { name = "JE-Chen", email = "jechenmailman@gmail.com" },
 ]
 description = "Automation Editor for GUI, WEB, API, Load Automation"
-readme = { file = "README.md", content-type = "text/markdown" }
 requires-python = ">=3.8"
 license = { text = "MIT" }
 dependencies = [
     "je-editor", "je_auto_control", "je_web_runner",
     "je_load_density", "je_api_testka"
 ]
 classifiers = [
-    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
     "Development Status :: 2 - Pre-Alpha",
     "Environment :: Win32 (MS Windows)",
     "Environment :: MacOS X",
     "Environment :: X11 Applications",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 
 [project.optional-dependencies]
 full_extension = [
     "je-mail-thunder"
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/JE-Chen/Integration-testing-environment"
+Homepage = "https://github.com/Intergration-Automation-Testing/AutomationEditor"
+Code = "https://github.com/Intergration-Automation-Testing/AutomationEditor"
+
+[project.readme]
+file = "README.md"
+content-type = "text/markdown"
+
+[tool.setuptools]
+license-files = ["LICENSE"]
 
 [tool.setuptools.packages]
 find = { namespaces = false }
```

