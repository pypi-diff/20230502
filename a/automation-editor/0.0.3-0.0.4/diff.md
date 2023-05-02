# Comparing `tmp/automation_editor-0.0.3.tar.gz` & `tmp/automation_editor-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation_editor-0.0.3.tar", last modified: Sun Apr 30 08:01:56 2023, max compression
+gzip compressed data, was "automation_editor-0.0.4.tar", last modified: Tue May  2 09:38:10 2023, max compression
```

## Comparing `automation_editor-0.0.3.tar` & `automation_editor-0.0.4.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.603769 automation_editor-0.0.3/
--rw-rw-rw-   0        0        0     1085 2023-04-05 12:50:43.000000 automation_editor-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     5793 2023-04-30 08:01:56.602741 automation_editor-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     5065 2023-04-29 11:09:10.000000 automation_editor-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.537915 automation_editor-0.0.3/automation_editor/
--rw-rw-rw-   0        0        0      130 2023-04-29 09:53:20.000000 automation_editor-0.0.3/automation_editor/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.3/automation_editor/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.554870 automation_editor-0.0.3/automation_editor/automation_editor_ui/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.3/automation_editor/automation_editor_ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.557918 automation_editor-0.0.3/automation_editor/automation_editor_ui/editor_main/
--rw-rw-rw-   0        0        0        0 2023-04-24 10:50:57.000000 automation_editor-0.0.3/automation_editor/automation_editor_ui/editor_main/__init__.py
--rw-rw-rw-   0        0        0     1323 2023-04-30 07:37:34.000000 automation_editor-0.0.3/automation_editor/automation_editor_ui/editor_main/main_ui.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.558896 automation_editor-0.0.3/automation_editor/automation_editor_ui/menu/
--rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor-0.0.3/automation_editor/automation_editor_ui/menu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.560854 automation_editor-0.0.3/automation_editor/automation_editor_ui/menu/api_testka_menu/
--rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor-0.0.3/automation_editor/automation_editor_ui/menu/api_testka_menu/__init__.py
--rw-rw-rw-   0        0        0     3998 2023-04-29 10:27:21.000000 automation_editor-0.0.3/automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.562849 automation_editor-0.0.3/automation_editor/automation_editor_ui/menu/auto_control_menu/
--rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor-0.0.3/automation_editor/automation_editor_ui/menu/auto_control_menu/__init__.py
--rw-rw-rw-   0        0        0     4129 2023-04-29 10:27:09.000000 automation_editor-0.0.3/automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.564880 automation_editor-0.0.3/automation_editor/automation_editor_ui/menu/load_density_menu/
--rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor-0.0.3/automation_editor/automation_editor_ui/menu/load_density_menu/__init__.py
--rw-rw-rw-   0        0        0     4161 2023-04-29 10:27:56.000000 automation_editor-0.0.3/automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.566873 automation_editor-0.0.3/automation_editor/automation_editor_ui/menu/web_runner_menu/
--rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor-0.0.3/automation_editor/automation_editor_ui/menu/web_runner_menu/__init__.py
--rw-rw-rw-   0        0        0     4040 2023-04-29 10:27:42.000000 automation_editor-0.0.3/automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.569831 automation_editor-0.0.3/automation_editor/automation_editor_ui/show_code_window/
--rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor-0.0.3/automation_editor/automation_editor_ui/show_code_window/__init__.py
--rw-rw-rw-   0        0        0      791 2023-04-27 10:28:14.000000 automation_editor-0.0.3/automation_editor/automation_editor_ui/show_code_window/code_window.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.572822 automation_editor-0.0.3/automation_editor/automation_editor_ui/syntax/
--rw-rw-rw-   0        0        0        0 2023-04-27 10:28:14.000000 automation_editor-0.0.3/automation_editor/automation_editor_ui/syntax/__init__.py
--rw-rw-rw-   0        0        0      777 2023-04-29 09:53:20.000000 automation_editor-0.0.3/automation_editor/automation_editor_ui/syntax/syntax_extend.py
--rw-rw-rw-   0        0        0     3257 2023-04-27 10:28:14.000000 automation_editor-0.0.3/automation_editor/automation_editor_ui/syntax/syntax_keyword.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.573819 automation_editor-0.0.3/automation_editor/extend/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.3/automation_editor/extend/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.575850 automation_editor-0.0.3/automation_editor/extend/mail_thunder_extend/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.3/automation_editor/extend/mail_thunder_extend/__init__.py
--rw-rw-rw-   0        0        0     1696 2023-04-29 09:53:20.000000 automation_editor-0.0.3/automation_editor/extend/mail_thunder_extend/mail_thunder_setting.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.576810 automation_editor-0.0.3/automation_editor/utils/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.3/automation_editor/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.580801 automation_editor-0.0.3/automation_editor/utils/exception/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.3/automation_editor/utils/exception/__init__.py
--rw-rw-rw-   0        0        0     1500 2023-04-27 10:28:14.000000 automation_editor-0.0.3/automation_editor/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0      608 2023-04-05 12:50:43.000000 automation_editor-0.0.3/automation_editor/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.583793 automation_editor-0.0.3/automation_editor/utils/file_process/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.3/automation_editor/utils/file_process/__init__.py
--rw-rw-rw-   0        0        0     1198 2023-04-27 10:28:14.000000 automation_editor-0.0.3/automation_editor/utils/file_process/get_dir_file_list.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.585787 automation_editor-0.0.3/automation_editor/utils/json_format/
--rw-rw-rw-   0        0        0        2 2023-04-05 12:50:43.000000 automation_editor-0.0.3/automation_editor/utils/json_format/__init__.py
--rw-rw-rw-   0        0        0      991 2023-04-29 09:53:20.000000 automation_editor-0.0.3/automation_editor/utils/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.587782 automation_editor-0.0.3/automation_editor/utils/manager/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.3/automation_editor/utils/manager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.590774 automation_editor-0.0.3/automation_editor/utils/manager/package_manager/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.3/automation_editor/utils/manager/package_manager/__init__.py
--rw-rw-rw-   0        0        0     1737 2023-04-28 11:00:21.000000 automation_editor-0.0.3/automation_editor/utils/manager/package_manager/package_manager_class.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.593765 automation_editor-0.0.3/automation_editor/utils/test_executor/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.3/automation_editor/utils/test_executor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.595766 automation_editor-0.0.3/automation_editor/utils/test_executor/api_testka/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.3/automation_editor/utils/test_executor/api_testka/__init__.py
--rw-rw-rw-   0        0        0     3935 2023-04-29 09:53:20.000000 automation_editor-0.0.3/automation_editor/utils/test_executor/api_testka/api_testka_process.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.597792 automation_editor-0.0.3/automation_editor/utils/test_executor/auto_control/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.3/automation_editor/utils/test_executor/auto_control/__init__.py
--rw-rw-rw-   0        0        0     3939 2023-04-29 09:53:20.000000 automation_editor-0.0.3/automation_editor/utils/test_executor/auto_control/auto_control_process.py
--rw-rw-rw-   0        0        0      498 2023-04-29 09:53:20.000000 automation_editor-0.0.3/automation_editor/utils/test_executor/check_mail_thunder.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.599750 automation_editor-0.0.3/automation_editor/utils/test_executor/load_density/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.3/automation_editor/utils/test_executor/load_density/__init__.py
--rw-rw-rw-   0        0        0     3949 2023-04-29 09:53:20.000000 automation_editor-0.0.3/automation_editor/utils/test_executor/load_density/load_density_process.py
--rw-rw-rw-   0        0        0     5837 2023-04-28 11:00:21.000000 automation_editor-0.0.3/automation_editor/utils/test_executor/task_process_manager.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.601745 automation_editor-0.0.3/automation_editor/utils/test_executor/web_runner/
--rw-rw-rw-   0        0        0        0 2023-04-05 12:50:43.000000 automation_editor-0.0.3/automation_editor/utils/test_executor/web_runner/__init__.py
--rw-rw-rw-   0        0        0     3897 2023-04-29 09:53:20.000000 automation_editor-0.0.3/automation_editor/utils/test_executor/web_runner/web_runner_process.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:01:56.553912 automation_editor-0.0.3/automation_editor.egg-info/
--rw-rw-rw-   0        0        0     5793 2023-04-30 08:01:56.000000 automation_editor-0.0.3/automation_editor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2931 2023-04-30 08:01:56.000000 automation_editor-0.0.3/automation_editor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 08:01:56.000000 automation_editor-0.0.3/automation_editor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-04-30 08:01:56.000000 automation_editor-0.0.3/automation_editor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-30 08:01:56.000000 automation_editor-0.0.3/automation_editor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1143 2023-04-30 07:49:28.000000 automation_editor-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-30 08:01:56.603769 automation_editor-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-02 09:38:10.257572 automation_editor-0.0.4/
+-rw-rw-rw-   0        0        0     1085 2023-04-19 01:59:04.000000 automation_editor-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     5885 2023-05-02 09:38:10.256526 automation_editor-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5065 2023-05-02 01:28:19.000000 automation_editor-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 09:38:10.077057 automation_editor-0.0.4/automation_editor/
+-rw-rw-rw-   0        0        0      130 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:38:10.117128 automation_editor-0.0.4/automation_editor/automation_editor_ui/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/automation_editor_ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:38:10.124131 automation_editor-0.0.4/automation_editor/automation_editor_ui/editor_main/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/automation_editor_ui/editor_main/__init__.py
+-rw-rw-rw-   0        0        0     1323 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/automation_editor_ui/editor_main/main_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:38:10.128244 automation_editor-0.0.4/automation_editor/automation_editor_ui/menu/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/automation_editor_ui/menu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:38:10.133137 automation_editor-0.0.4/automation_editor/automation_editor_ui/menu/api_testka_menu/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/automation_editor_ui/menu/api_testka_menu/__init__.py
+-rw-rw-rw-   0        0        0     3998 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:38:10.142168 automation_editor-0.0.4/automation_editor/automation_editor_ui/menu/auto_control_menu/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/automation_editor_ui/menu/auto_control_menu/__init__.py
+-rw-rw-rw-   0        0        0     4129 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:38:10.148740 automation_editor-0.0.4/automation_editor/automation_editor_ui/menu/load_density_menu/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/automation_editor_ui/menu/load_density_menu/__init__.py
+-rw-rw-rw-   0        0        0     4161 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:38:10.155902 automation_editor-0.0.4/automation_editor/automation_editor_ui/menu/web_runner_menu/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/automation_editor_ui/menu/web_runner_menu/__init__.py
+-rw-rw-rw-   0        0        0     4040 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:38:10.160795 automation_editor-0.0.4/automation_editor/automation_editor_ui/show_code_window/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/automation_editor_ui/show_code_window/__init__.py
+-rw-rw-rw-   0        0        0      791 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/automation_editor_ui/show_code_window/code_window.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:38:10.171795 automation_editor-0.0.4/automation_editor/automation_editor_ui/syntax/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/automation_editor_ui/syntax/__init__.py
+-rw-rw-rw-   0        0        0      777 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/automation_editor_ui/syntax/syntax_extend.py
+-rw-rw-rw-   0        0        0     3257 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/automation_editor_ui/syntax/syntax_keyword.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:38:10.174795 automation_editor-0.0.4/automation_editor/extend/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/extend/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:38:10.180952 automation_editor-0.0.4/automation_editor/extend/mail_thunder_extend/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/extend/mail_thunder_extend/__init__.py
+-rw-rw-rw-   0        0        0     1696 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/extend/mail_thunder_extend/mail_thunder_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:38:10.183908 automation_editor-0.0.4/automation_editor/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:38:10.192964 automation_editor-0.0.4/automation_editor/utils/exception/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0     1500 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0      608 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:38:10.198867 automation_editor-0.0.4/automation_editor/utils/file_process/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/utils/file_process/__init__.py
+-rw-rw-rw-   0        0        0     1198 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/utils/file_process/get_dir_file_list.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:38:10.206957 automation_editor-0.0.4/automation_editor/utils/json_format/
+-rw-rw-rw-   0        0        0        2 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/utils/json_format/__init__.py
+-rw-rw-rw-   0        0        0      991 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/utils/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:38:10.208866 automation_editor-0.0.4/automation_editor/utils/manager/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/utils/manager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:38:10.214958 automation_editor-0.0.4/automation_editor/utils/manager/package_manager/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/utils/manager/package_manager/__init__.py
+-rw-rw-rw-   0        0        0     1737 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/utils/manager/package_manager/package_manager_class.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:38:10.225870 automation_editor-0.0.4/automation_editor/utils/test_executor/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/utils/test_executor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:38:10.232969 automation_editor-0.0.4/automation_editor/utils/test_executor/api_testka/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/utils/test_executor/api_testka/__init__.py
+-rw-rw-rw-   0        0        0     3935 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/utils/test_executor/api_testka/api_testka_process.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:38:10.240945 automation_editor-0.0.4/automation_editor/utils/test_executor/auto_control/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/utils/test_executor/auto_control/__init__.py
+-rw-rw-rw-   0        0        0     3939 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/utils/test_executor/auto_control/auto_control_process.py
+-rw-rw-rw-   0        0        0      498 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/utils/test_executor/check_mail_thunder.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:38:10.246518 automation_editor-0.0.4/automation_editor/utils/test_executor/load_density/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/utils/test_executor/load_density/__init__.py
+-rw-rw-rw-   0        0        0     3949 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/utils/test_executor/load_density/load_density_process.py
+-rw-rw-rw-   0        0        0     5837 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/utils/test_executor/task_process_manager.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:38:10.253615 automation_editor-0.0.4/automation_editor/utils/test_executor/web_runner/
+-rw-rw-rw-   0        0        0        0 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/utils/test_executor/web_runner/__init__.py
+-rw-rw-rw-   0        0        0     3897 2023-05-02 01:28:19.000000 automation_editor-0.0.4/automation_editor/utils/test_executor/web_runner/web_runner_process.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:38:10.113125 automation_editor-0.0.4/automation_editor.egg-info/
+-rw-rw-rw-   0        0        0     5885 2023-05-02 09:38:09.000000 automation_editor-0.0.4/automation_editor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2931 2023-05-02 09:38:10.000000 automation_editor-0.0.4/automation_editor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 09:38:09.000000 automation_editor-0.0.4/automation_editor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-05-02 09:38:09.000000 automation_editor-0.0.4/automation_editor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-02 09:38:09.000000 automation_editor-0.0.4/automation_editor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1280 2023-05-02 09:37:50.000000 automation_editor-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-02 09:38:10.258615 automation_editor-0.0.4/setup.cfg
```

### Comparing `automation_editor-0.0.3/LICENSE` & `automation_editor-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.3/PKG-INFO` & `automation_editor-0.0.4/automation_editor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
-Name: automation_editor
-Version: 0.0.3
+Name: automation-editor
+Version: 0.0.4
 Summary: Automation Editor for GUI, WEB, API, Load Automation
-Author-email: JE-Chen <zenmailman@gmail.com>
+Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
-Project-URL: Homepage, https://github.com/Integrated-Testing-Environment/AutomationEditor
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

### Comparing `automation_editor-0.0.3/README.md` & `automation_editor-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.3/automation_editor/automation_editor_ui/editor_main/main_ui.py` & `automation_editor-0.0.4/automation_editor/automation_editor_ui/editor_main/main_ui.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.3/automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py` & `automation_editor-0.0.4/automation_editor/automation_editor_ui/menu/api_testka_menu/build_api_testka_menu.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.3/automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py` & `automation_editor-0.0.4/automation_editor/automation_editor_ui/menu/auto_control_menu/build_autocontrol_menu.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.3/automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py` & `automation_editor-0.0.4/automation_editor/automation_editor_ui/menu/load_density_menu/build_load_density_menu.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.3/automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py` & `automation_editor-0.0.4/automation_editor/automation_editor_ui/menu/web_runner_menu/build_webrunner_menu.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.3/automation_editor/automation_editor_ui/show_code_window/code_window.py` & `automation_editor-0.0.4/automation_editor/automation_editor_ui/show_code_window/code_window.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.3/automation_editor/automation_editor_ui/syntax/syntax_extend.py` & `automation_editor-0.0.4/automation_editor/automation_editor_ui/syntax/syntax_extend.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.3/automation_editor/automation_editor_ui/syntax/syntax_keyword.py` & `automation_editor-0.0.4/automation_editor/automation_editor_ui/syntax/syntax_keyword.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.3/automation_editor/extend/mail_thunder_extend/mail_thunder_setting.py` & `automation_editor-0.0.4/automation_editor/extend/mail_thunder_extend/mail_thunder_setting.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.3/automation_editor/utils/exception/exception_tags.py` & `automation_editor-0.0.4/automation_editor/utils/exception/exception_tags.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.3/automation_editor/utils/exception/exceptions.py` & `automation_editor-0.0.4/automation_editor/utils/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.3/automation_editor/utils/file_process/get_dir_file_list.py` & `automation_editor-0.0.4/automation_editor/utils/file_process/get_dir_file_list.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.3/automation_editor/utils/json_format/json_process.py` & `automation_editor-0.0.4/automation_editor/utils/json_format/json_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.3/automation_editor/utils/manager/package_manager/package_manager_class.py` & `automation_editor-0.0.4/automation_editor/utils/manager/package_manager/package_manager_class.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.3/automation_editor/utils/test_executor/api_testka/api_testka_process.py` & `automation_editor-0.0.4/automation_editor/utils/test_executor/api_testka/api_testka_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.3/automation_editor/utils/test_executor/auto_control/auto_control_process.py` & `automation_editor-0.0.4/automation_editor/utils/test_executor/auto_control/auto_control_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.3/automation_editor/utils/test_executor/load_density/load_density_process.py` & `automation_editor-0.0.4/automation_editor/utils/test_executor/load_density/load_density_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.3/automation_editor/utils/test_executor/task_process_manager.py` & `automation_editor-0.0.4/automation_editor/utils/test_executor/task_process_manager.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.3/automation_editor/utils/test_executor/web_runner/web_runner_process.py` & `automation_editor-0.0.4/automation_editor/utils/test_executor/web_runner/web_runner_process.py`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.3/automation_editor.egg-info/PKG-INFO` & `automation_editor-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
-Name: automation-editor
-Version: 0.0.3
+Name: automation_editor
+Version: 0.0.4
 Summary: Automation Editor for GUI, WEB, API, Load Automation
-Author-email: JE-Chen <zenmailman@gmail.com>
+Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
-Project-URL: Homepage, https://github.com/Integrated-Testing-Environment/AutomationEditor
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

### Comparing `automation_editor-0.0.3/automation_editor.egg-info/SOURCES.txt` & `automation_editor-0.0.4/automation_editor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `automation_editor-0.0.3/pyproject.toml` & `automation_editor-0.0.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,39 +2,46 @@
 # This is stable version
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "automation_editor"
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
-"Homepage" = "https://github.com/Integrated-Testing-Environment/AutomationEditor"
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

