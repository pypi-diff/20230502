# Comparing `tmp/je_editor_dev-0.0.9.tar.gz` & `tmp/je_editor_dev-0.0.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "je_editor_dev-0.0.9.tar", last modified: Fri Jan 14 21:02:54 2022, max compression
+gzip compressed data, was "je_editor_dev-0.0.90.tar", last modified: Tue May  2 08:12:26 2023, max compression
```

## Comparing `je_editor_dev-0.0.9.tar` & `je_editor_dev-0.0.90.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.296718 je_editor_dev-0.0.9/
--rw-rw-rw-   0        0        0     1085 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/LICENSE
--rw-rw-rw-   0        0        0     1481 2022-01-14 21:02:54.294720 je_editor_dev-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      860 2022-01-06 12:40:47.000000 je_editor_dev-0.0.9/README.md
--rw-rw-rw-   0        0        0      909 2022-01-14 21:02:51.000000 je_editor_dev-0.0.9/dev_setup.py
-drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.033720 je_editor_dev-0.0.9/je_editor/
--rw-rw-rw-   0        0        0      608 2022-01-14 18:33:11.000000 je_editor_dev-0.0.9/je_editor/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.036723 je_editor_dev-0.0.9/je_editor/ui/
--rw-rw-rw-   0        0        0       28 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.041717 je_editor_dev-0.0.9/je_editor/ui/editor_main_ui/
--rw-rw-rw-   0        0        0       43 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/editor_main_ui/__init__.py
--rw-rw-rw-   0        0        0    11111 2022-01-14 21:02:13.000000 je_editor_dev-0.0.9/je_editor/ui/editor_main_ui/tkinter_editor.py
-drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.043734 je_editor_dev-0.0.9/je_editor/ui/ui_event/
--rw-rw-rw-   0        0        0       37 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.046718 je_editor_dev-0.0.9/je_editor/ui/ui_event/auto_save/
--rw-rw-rw-   0        0        0       47 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/auto_save/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.052732 je_editor_dev-0.0.9/je_editor/ui/ui_event/auto_save/start_auto_save/
--rw-rw-rw-   0        0        0       65 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/auto_save/start_auto_save/__init__.py
--rw-rw-rw-   0        0        0      460 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/auto_save/start_auto_save/start_auto_save.py
-drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.057723 je_editor_dev-0.0.9/je_editor/ui/ui_event/change_font/
--rw-rw-rw-   0        0        0       49 2022-01-06 12:40:47.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/change_font/__init__.py
--rw-rw-rw-   0        0        0      844 2022-01-14 11:49:29.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/change_font/change_font.py
-drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.064718 je_editor_dev-0.0.9/je_editor/ui/ui_event/close/
--rw-rw-rw-   0        0        0       43 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/close/__init__.py
--rw-rw-rw-   0        0        0      532 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/close/close_event.py
-drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.069721 je_editor_dev-0.0.9/je_editor/ui/ui_event/encoding/
--rw-rw-rw-   0        0        0       46 2022-01-14 11:46:17.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/encoding/__init__.py
--rw-rw-rw-   0        0        0       89 2022-01-14 11:49:29.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/encoding/set_encoding.py
-drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.071718 je_editor_dev-0.0.9/je_editor/ui/ui_event/execute/
--rw-rw-rw-   0        0        0       45 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/execute/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.076726 je_editor_dev-0.0.9/je_editor/ui/ui_event/execute/execute_code/
--rw-rw-rw-   0        0        0       58 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/execute/execute_code/__init__.py
--rw-rw-rw-   0        0        0      538 2022-01-09 13:01:31.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/execute/execute_code/exec_code.py
-drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.082720 je_editor_dev-0.0.9/je_editor/ui/ui_event/execute/execute_shell_command/
--rw-rw-rw-   0        0        0       67 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/execute/execute_shell_command/__init__.py
--rw-rw-rw-   0        0        0      726 2022-01-06 02:44:24.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/execute/execute_shell_command/run_on_shell.py
-drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.087718 je_editor_dev-0.0.9/je_editor/ui/ui_event/language/
--rw-rw-rw-   0        0        0       46 2022-01-14 12:08:46.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/language/__init__.py
--rw-rw-rw-   0        0        0       89 2022-01-14 12:08:46.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/language/set_language.py
-drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.090719 je_editor_dev-0.0.9/je_editor/ui/ui_event/open_file/
--rw-rw-rw-   0        0        0        2 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/open_file/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.096719 je_editor_dev-0.0.9/je_editor/ui/ui_event/open_file/open_file_to_read/
--rw-rw-rw-   0        0        0       65 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/open_file/open_file_to_read/__init__.py
--rw-rw-rw-   0        0        0      655 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/open_file/open_file_to_read/open_file_to_read.py
-drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.103719 je_editor_dev-0.0.9/je_editor/ui/ui_event/open_file/open_last_edit_file/
--rw-rw-rw-   0        0        0       67 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/open_file/open_last_edit_file/__init__.py
--rw-rw-rw-   0        0        0      638 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/open_file/open_last_edit_file/open_last_edit_file.py
-drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.105717 je_editor_dev-0.0.9/je_editor/ui/ui_event/save_file/
--rw-rw-rw-   0        0        0        0 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/save_file/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.112718 je_editor_dev-0.0.9/je_editor/ui/ui_event/save_file/save_file_to_open/
--rw-rw-rw-   0        0        0       65 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/save_file/save_file_to_open/__init__.py
--rw-rw-rw-   0        0        0      593 2022-01-06 18:18:59.000000 je_editor_dev-0.0.9/je_editor/ui/ui_event/save_file/save_file_to_open/save_file_to_open.py
-drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.115717 je_editor_dev-0.0.9/je_editor/ui/ui_utils/
--rw-rw-rw-   0        0        0       37 2022-01-06 12:40:47.000000 je_editor_dev-0.0.9/je_editor/ui/ui_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.122717 je_editor_dev-0.0.9/je_editor/ui/ui_utils/font/
--rw-rw-rw-   0        0        0       42 2022-01-06 12:40:47.000000 je_editor_dev-0.0.9/je_editor/ui/ui_utils/font/__init__.py
--rw-rw-rw-   0        0        0      292 2022-01-06 12:40:47.000000 je_editor_dev-0.0.9/je_editor/ui/ui_utils/font/font.py
-drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.126718 je_editor_dev-0.0.9/je_editor/utils/
--rw-rw-rw-   0        0        0       31 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.140721 je_editor_dev-0.0.9/je_editor/utils/code_tag/
--rw-rw-rw-   0        0        0        0 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/code_tag/__init__.py
--rw-rw-rw-   0        0        0       96 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/code_tag/keyword_list.py
--rw-rw-rw-   0        0        0     1805 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/code_tag/tag_keyword.py
-drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.153718 je_editor_dev-0.0.9/je_editor/utils/editor_content/
--rw-rw-rw-   0        0        0       46 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/editor_content/__init__.py
--rw-rw-rw-   0        0        0     1519 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/editor_content/content_save.py
-drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.164717 je_editor_dev-0.0.9/je_editor/utils/encoding/
--rw-rw-rw-   0        0        0       40 2022-01-14 11:17:11.000000 je_editor_dev-0.0.9/je_editor/utils/encoding/__init__.py
--rw-rw-rw-   0        0        0     1717 2022-01-14 11:17:11.000000 je_editor_dev-0.0.9/je_editor/utils/encoding/encoding_data_module.py
-drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.176718 je_editor_dev-0.0.9/je_editor/utils/exception/
--rw-rw-rw-   0        0        0       41 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/exception/__init__.py
--rw-rw-rw-   0        0        0      497 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/exception/je_editor_exception_tag.py
--rw-rw-rw-   0        0        0      488 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/exception/je_editor_exceptions.py
-drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.179718 je_editor_dev-0.0.9/je_editor/utils/file/
--rw-rw-rw-   0        0        0       36 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/file/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.184719 je_editor_dev-0.0.9/je_editor/utils/file/open/
--rw-rw-rw-   0        0        0       41 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/file/open/__init__.py
--rw-rw-rw-   0        0        0     1532 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/file/open/open_file.py
-drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.190721 je_editor_dev-0.0.9/je_editor/utils/file/save/
--rw-rw-rw-   0        0        0       39 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/file/save/__init__.py
--rw-rw-rw-   0        0        0     2423 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/file/save/save_file.py
-drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.196718 je_editor_dev-0.0.9/je_editor/utils/language/
--rw-rw-rw-   0        0        0       40 2022-01-14 11:56:38.000000 je_editor_dev-0.0.9/je_editor/utils/language/__init__.py
--rw-rw-rw-   0        0        0       68 2022-01-14 12:01:15.000000 je_editor_dev-0.0.9/je_editor/utils/language/language_data_module.py
-drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.206727 je_editor_dev-0.0.9/je_editor/utils/string_translate/
--rw-rw-rw-   0        0        0        0 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/string_translate/__init__.py
--rw-rw-rw-   0        0        0       54 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/string_translate/used_string.py
-drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.212718 je_editor_dev-0.0.9/je_editor/utils/text_process/
--rw-rw-rw-   0        0        0       44 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/text_process/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.228718 je_editor_dev-0.0.9/je_editor/utils/text_process/program_exec/
--rw-rw-rw-   0        0        0       57 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/text_process/program_exec/__init__.py
--rw-rw-rw-   0        0        0     5984 2022-01-14 18:36:19.000000 je_editor_dev-0.0.9/je_editor/utils/text_process/program_exec/exec_text.py
--rw-rw-rw-   0        0        0      327 2022-01-07 18:49:28.000000 je_editor_dev-0.0.9/je_editor/utils/text_process/program_exec/process_error.py
-drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.237720 je_editor_dev-0.0.9/je_editor/utils/text_process/shell/
--rw-rw-rw-   0        0        0       50 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/text_process/shell/__init__.py
--rw-rw-rw-   0        0        0      448 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/text_process/shell/shell_text.py
-drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.242718 je_editor_dev-0.0.9/je_editor/utils/theme/
--rw-rw-rw-   0        0        0        0 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/theme/__init__.py
--rw-rw-rw-   0        0        0       96 2022-01-03 07:43:33.000000 je_editor_dev-0.0.9/je_editor/utils/theme/theme.py
-drwxrwxrwx   0        0        0        0 2022-01-14 21:02:54.290718 je_editor_dev-0.0.9/je_editor_dev.egg-info/
--rw-rw-rw-   0        0        0     1481 2022-01-14 21:02:53.000000 je_editor_dev-0.0.9/je_editor_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2968 2022-01-14 21:02:53.000000 je_editor_dev-0.0.9/je_editor_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-14 21:02:53.000000 je_editor_dev-0.0.9/je_editor_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2022-01-14 21:02:53.000000 je_editor_dev-0.0.9/je_editor_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-01-14 21:02:54.296718 je_editor_dev-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      901 2022-01-13 14:16:52.000000 je_editor_dev-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:12:26.192953 je_editor_dev-0.0.90/
+-rw-rw-rw-   0        0        0     1085 2023-03-28 03:05:50.000000 je_editor_dev-0.0.90/LICENSE
+-rw-rw-rw-   0        0        0     3097 2023-05-02 08:12:26.191944 je_editor_dev-0.0.90/PKG-INFO
+-rw-rw-rw-   0        0        0     2304 2023-05-02 05:01:56.000000 je_editor_dev-0.0.90/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 08:12:25.870078 je_editor_dev-0.0.90/je_editor/
+-rw-rw-rw-   0        0        0     1429 2023-04-27 09:32:32.000000 je_editor_dev-0.0.90/je_editor/__init__.py
+-rw-rw-rw-   0        0        0      598 2023-03-28 03:05:50.000000 je_editor_dev-0.0.90/je_editor/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:12:25.877075 je_editor_dev-0.0.90/je_editor/pyside_ui/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:12:25.889075 je_editor_dev-0.0.90/je_editor/pyside_ui/auto_save/
+-rw-rw-rw-   0        0        0        0 2023-04-24 05:25:24.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/auto_save/__init__.py
+-rw-rw-rw-   0        0        0     1071 2023-04-24 05:30:02.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/auto_save/auto_save_thread.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:12:25.905094 je_editor_dev-0.0.90/je_editor/pyside_ui/code_editor/
+-rw-rw-rw-   0        0        0        0 2023-04-25 01:06:15.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/code_editor/__init__.py
+-rw-rw-rw-   0        0        0     5355 2023-04-28 07:36:34.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/code_editor/code_edit_plaintext.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:12:25.914327 je_editor_dev-0.0.90/je_editor/pyside_ui/code_process/
+-rw-rw-rw-   0        0        0        0 2023-04-24 01:06:05.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/code_process/__init__.py
+-rw-rw-rw-   0        0        0     7371 2023-05-02 01:27:43.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/code_process/code_exec.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:12:25.924333 je_editor_dev-0.0.90/je_editor/pyside_ui/code_result/
+-rw-rw-rw-   0        0        0        0 2023-04-28 02:29:59.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/code_result/__init__.py
+-rw-rw-rw-   0        0        0     1393 2023-04-28 02:38:28.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/code_result/code_record.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:12:25.933855 je_editor_dev-0.0.90/je_editor/pyside_ui/colors/
+-rw-rw-rw-   0        0        0        0 2023-04-25 00:59:39.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/colors/__init__.py
+-rw-rw-rw-   0        0        0      123 2023-04-25 00:59:39.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/colors/global_color.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:12:25.945858 je_editor_dev-0.0.90/je_editor/pyside_ui/file_dialog/
+-rw-rw-rw-   0        0        0        0 2023-04-20 01:28:13.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/file_dialog/__init__.py
+-rw-rw-rw-   0        0        0     1058 2023-04-27 01:03:49.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/file_dialog/open_file_dialog.py
+-rw-rw-rw-   0        0        0      995 2023-04-24 05:26:43.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/file_dialog/save_file_dialog.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:12:25.951219 je_editor_dev-0.0.90/je_editor/pyside_ui/main_ui/
+-rw-rw-rw-   0        0        0        0 2023-04-19 08:45:41.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/main_ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:12:25.957221 je_editor_dev-0.0.90/je_editor/pyside_ui/main_ui/editor_main_ui/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/main_ui/editor_main_ui/__init__.py
+-rw-rw-rw-   0        0        0     6550 2023-05-02 07:54:19.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/main_ui/editor_main_ui/main_editor.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:12:25.964223 je_editor_dev-0.0.90/je_editor/pyside_ui/main_ui_setting/
+-rw-rw-rw-   0        0        0        0 2023-04-18 06:44:29.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/main_ui_setting/__init__.py
+-rw-rw-rw-   0        0        0     1643 2023-05-02 03:02:45.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/main_ui_setting/ui_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:12:25.968223 je_editor_dev-0.0.90/je_editor/pyside_ui/menu/
+-rw-rw-rw-   0        0        0        0 2023-04-18 06:54:58.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/menu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:12:25.974223 je_editor_dev-0.0.90/je_editor/pyside_ui/menu/menu_bar/
+-rw-rw-rw-   0        0        0        0 2023-04-19 06:59:58.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/menu/menu_bar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:12:25.981223 je_editor_dev-0.0.90/je_editor/pyside_ui/menu/menu_bar/check_style_menu/
+-rw-rw-rw-   0        0        0        0 2023-04-25 05:11:13.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/menu/menu_bar/check_style_menu/__init__.py
+-rw-rw-rw-   0        0        0     1734 2023-05-02 02:19:26.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/menu/menu_bar/check_style_menu/build_check_style_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:12:25.987678 je_editor_dev-0.0.90/je_editor/pyside_ui/menu/menu_bar/file_menu/
+-rw-rw-rw-   0        0        0        0 2023-04-20 01:26:35.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/menu/menu_bar/file_menu/__init__.py
+-rw-rw-rw-   0        0        0     1228 2023-05-02 03:17:22.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/menu/menu_bar/file_menu/build_file_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:12:26.025452 je_editor_dev-0.0.90/je_editor/pyside_ui/menu/menu_bar/help_menu/
+-rw-rw-rw-   0        0        0        0 2023-04-26 01:29:16.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/menu/menu_bar/help_menu/__init__.py
+-rw-rw-rw-   0        0        0     1319 2023-05-02 02:19:26.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/menu/menu_bar/help_menu/build_help_menu.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:12:26.036558 je_editor_dev-0.0.90/je_editor/pyside_ui/menu/menu_bar/run_menu/
+-rw-rw-rw-   0        0        0        0 2023-04-20 01:26:45.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/menu/menu_bar/run_menu/__init__.py
+-rw-rw-rw-   0        0        0     4141 2023-05-02 03:15:20.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/menu/menu_bar/run_menu/build_run_menu.py
+-rw-rw-rw-   0        0        0     1118 2023-04-28 08:28:07.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/menu/menu_bar/set_menu_bar.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:12:26.048974 je_editor_dev-0.0.90/je_editor/pyside_ui/search_ui/
+-rw-rw-rw-   0        0        0        0 2023-04-28 01:11:42.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/search_ui/__init__.py
+-rw-rw-rw-   0        0        0      865 2023-04-28 07:10:30.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/search_ui/search_error_box.py
+-rw-rw-rw-   0        0        0      857 2023-04-28 07:10:30.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/search_ui/search_text_box.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:12:26.056970 je_editor_dev-0.0.90/je_editor/pyside_ui/shell_process/
+-rw-rw-rw-   0        0        0        0 2023-04-24 01:06:05.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/shell_process/__init__.py
+-rw-rw-rw-   0        0        0     6068 2023-05-02 01:27:43.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/shell_process/shell_exec.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:12:26.062361 je_editor_dev-0.0.90/je_editor/pyside_ui/syntax/
+-rw-rw-rw-   0        0        0        0 2023-04-24 05:50:21.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/syntax/__init__.py
+-rw-rw-rw-   0        0        0     3749 2023-04-25 07:44:44.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/syntax/python_syntax.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:12:26.067361 je_editor_dev-0.0.90/je_editor/pyside_ui/treeview/
+-rw-rw-rw-   0        0        0        0 2023-04-19 07:00:18.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/treeview/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:12:26.072877 je_editor_dev-0.0.90/je_editor/pyside_ui/treeview/project_treeview/
+-rw-rw-rw-   0        0        0        0 2023-04-19 07:00:28.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/treeview/project_treeview/__init__.py
+-rw-rw-rw-   0        0        0     1961 2023-04-28 08:28:07.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/treeview/project_treeview/set_project_treeview.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:12:26.082412 je_editor_dev-0.0.90/je_editor/pyside_ui/user_setting/
+-rw-rw-rw-   0        0        0        0 2023-05-02 06:59:59.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/user_setting/__init__.py
+-rw-rw-rw-   0        0        0      607 2023-05-02 07:26:52.000000 je_editor_dev-0.0.90/je_editor/pyside_ui/user_setting/user_setting_file.py
+-rw-rw-rw-   0        0        0      431 2023-05-02 07:41:49.000000 je_editor_dev-0.0.90/je_editor/start_editor.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:12:26.087865 je_editor_dev-0.0.90/je_editor/utils/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor_dev-0.0.90/je_editor/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:12:26.093867 je_editor_dev-0.0.90/je_editor/utils/encodings/
+-rw-rw-rw-   0        0        0        0 2023-05-02 07:45:07.000000 je_editor_dev-0.0.90/je_editor/utils/encodings/__init__.py
+-rw-rw-rw-   0        0        0     1613 2023-05-02 07:48:01.000000 je_editor_dev-0.0.90/je_editor/utils/encodings/python_encodings.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:12:26.110128 je_editor_dev-0.0.90/je_editor/utils/exception/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor_dev-0.0.90/je_editor/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0     1062 2023-05-02 07:11:45.000000 je_editor_dev-0.0.90/je_editor/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0      506 2023-03-28 03:05:50.000000 je_editor_dev-0.0.90/je_editor/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:12:26.118516 je_editor_dev-0.0.90/je_editor/utils/file/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor_dev-0.0.90/je_editor/utils/file/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:12:26.125961 je_editor_dev-0.0.90/je_editor/utils/file/open/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor_dev-0.0.90/je_editor/utils/file/open/__init__.py
+-rw-rw-rw-   0        0        0      962 2023-04-24 01:06:05.000000 je_editor_dev-0.0.90/je_editor/utils/file/open/open_file.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:12:26.137008 je_editor_dev-0.0.90/je_editor/utils/file/save/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor_dev-0.0.90/je_editor/utils/file/save/__init__.py
+-rw-rw-rw-   0        0        0      719 2023-04-27 01:03:49.000000 je_editor_dev-0.0.90/je_editor/utils/file/save/save_file.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:12:26.144010 je_editor_dev-0.0.90/je_editor/utils/json/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 je_editor_dev-0.0.90/je_editor/utils/json/__init__.py
+-rw-rw-rw-   0        0        0     1338 2023-05-02 07:11:45.000000 je_editor_dev-0.0.90/je_editor/utils/json/json_file.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:12:26.150173 je_editor_dev-0.0.90/je_editor/utils/json_format/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:05:50.000000 je_editor_dev-0.0.90/je_editor/utils/json_format/__init__.py
+-rw-rw-rw-   0        0        0      983 2023-03-28 03:05:50.000000 je_editor_dev-0.0.90/je_editor/utils/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:12:26.156169 je_editor_dev-0.0.90/je_editor/utils/redirect_manager/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:50.000000 je_editor_dev-0.0.90/je_editor/utils/redirect_manager/__init__.py
+-rw-rw-rw-   0        0        0     1991 2023-04-28 02:23:45.000000 je_editor_dev-0.0.90/je_editor/utils/redirect_manager/redirect_manager_class.py
+drwxrwxrwx   0        0        0        0 2023-05-02 08:12:26.188610 je_editor_dev-0.0.90/je_editor_dev.egg-info/
+-rw-rw-rw-   0        0        0     3097 2023-05-02 08:12:25.000000 je_editor_dev-0.0.90/je_editor_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3061 2023-05-02 08:12:25.000000 je_editor_dev-0.0.90/je_editor_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 08:12:25.000000 je_editor_dev-0.0.90/je_editor_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-05-02 08:12:25.000000 je_editor_dev-0.0.90/je_editor_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-02 08:12:25.000000 je_editor_dev-0.0.90/je_editor_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1134 2023-05-02 08:12:04.000000 je_editor_dev-0.0.90/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-02 08:12:26.193953 je_editor_dev-0.0.90/setup.cfg
```

### Comparing `je_editor_dev-0.0.9/LICENSE` & `je_editor_dev-0.0.90/LICENSE`

 * *Files identical despite different names*

### Comparing `je_editor_dev-0.0.9/je_editor/utils/encoding/encoding_data_module.py` & `je_editor_dev-0.0.90/je_editor/utils/encodings/python_encodings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-encoding_list = \
-    ['ascii',
-     'big5',
-     'big5hkscs',
-     'cp037',
-     'cp273',
-     'cp424',
-     'cp437',
-     'cp500',
-     'cp720',
-     'cp737',
-     'cp775',
-     'cp850',
-     'cp852',
-     'cp855',
-     'cp856',
-     'cp857',
-     'cp858',
-     'cp860',
-     'cp861',
-     'cp862',
-     'cp863',
-     'cp864',
-     'cp865',
-     'cp866',
-     'cp869',
-     'cp874',
-     'cp875',
-     'cp932',
-     'cp949',
-     'cp950',
-     'cp1006',
-     'cp1026',
-     'cp1125',
-     'cp1140',
-     'cp1250',
-     'cp1251',
-     'cp1252',
-     'cp1253',
-     'cp1254',
-     'cp1255',
-     'cp1256',
-     'cp1257',
-     'cp1258',
-     'cp65001',
-     'euc_jp',
-     'euc_jis_2004',
-     'euc_jisx0213',
-     'euc_kr',
-     'gb2312',
-     'gbk',
-     'gb18030',
-     'hz',
-     'iso2022_jp',
-     'iso2022_jp_1',
-     'iso2022_jp_2',
-     'iso2022_jp_2004',
-     'iso2022_jp_3',
-     'iso2022_jp_ext',
-     'iso2022_kr',
-     'latin_1',
-     'iso8859_2',
-     'iso8859_3',
-     'iso8859_4',
-     'iso8859_5',
-     'iso8859_6',
-     'iso8859_7',
-     'iso8859_8',
-     'iso8859_9',
-     'iso8859_10',
-     'iso8859_11',
-     'iso8859_13',
-     'iso8859_14',
-     'iso8859_15',
-     'iso8859_16',
-     'johab',
-     'koi8_r',
-     'koi8_t',
-     'koi8_u',
-     'kz1048',
-     'mac_cyrillic',
-     'mac_greek',
-     'mac_iceland',
-     'mac_latin2',
-     'mac_roman',
-     'mac_turkish',
-     'ptcp154',
-     'shift_jis',
-     'shift_jis_2004',
-     'shift_jisx0213',
-     'utf_32',
-     'utf_32_be',
-     'utf_32_le',
-     'utf_16',
-     'utf_16_be',
-     'utf_16_le',
-     'utf_7',
-     'utf_8',
-     'utf_8_sig']
+python_encodings_list = [
+    'ascii',
+    'big5',
+    'big5hkscs',
+    'cp037',
+    'cp273',
+    'cp424',
+    'cp437',
+    'cp500',
+    'cp720',
+    'cp737',
+    'cp775',
+    'cp850',
+    'cp852',
+    'cp855',
+    'cp856',
+    'cp857',
+    'cp858',
+    'cp860',
+    'cp861',
+    'cp862',
+    'cp863',
+    'cp864',
+    'cp865',
+    'cp866',
+    'cp869',
+    'cp874',
+    'cp875',
+    'cp932',
+    'cp949',
+    'cp950',
+    'cp1006',
+    'cp1026',
+    'cp1125',
+    'cp1140',
+    'cp1250',
+    'cp1251',
+    'cp1252',
+    'cp1253',
+    'cp1254',
+    'cp1255',
+    'cp1256',
+    'cp1257',
+    'cp1258',
+    'euc_jp',
+    'euc_jis_2004',
+    'euc_jisx0213',
+    'euc_kr',
+    'gb2312',
+    'gbk',
+    'gb18030',
+    'hz',
+    'iso2022_jp',
+    'iso2022_jp_1',
+    'iso2022_jp_2',
+    'iso2022_jp_2004',
+    'iso2022_jp_3',
+    'iso2022_jp_ext',
+    'iso2022_kr',
+    'latin_1',
+    'iso8859_2',
+    'iso8859_3',
+    'iso8859_4',
+    'iso8859_5',
+    'iso8859_6',
+    'iso8859_7',
+    'iso8859_8',
+    'iso8859_9',
+    'iso8859_10',
+    'iso8859_11',
+    'iso8859_13',
+    'iso8859_14',
+    'iso8859_15',
+    'iso8859_16',
+    'johab',
+    'koi8_r',
+    'koi8_t',
+    'koi8_u',
+    'kz1048',
+    'mac_cyrillic',
+    'mac_greek',
+    'mac_iceland',
+    'mac_latin2',
+    'mac_roman',
+    'mac_turkish',
+    'ptcp154',
+    'shift_jis',
+    'shift_jis_2004',
+    'shift_jisx0213',
+    'utf_32',
+    'utf_32_be',
+    'utf_32_le',
+    'utf_16',
+    'utf_16_be',
+    'utf_16_le',
+    'utf_7',
+    'utf_8',
+    'utf_8_sig'
+]
```

### Comparing `je_editor_dev-0.0.9/je_editor/utils/text_process/program_exec/exec_text.py` & `je_editor_dev-0.0.90/je_editor/pyside_ui/code_process/code_exec.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,139 +1,174 @@
-import sys
 import os.path
 import queue
 import shutil
 import subprocess
 from pathlib import Path
 from threading import Thread
-from tkinter import DISABLED
-from tkinter import END
-from tkinter import NORMAL
-
-from je_editor.utils.exception.je_editor_exception_tag import file_not_fond_error
-from je_editor.utils.exception.je_editor_exception_tag import python_not_found_error
-from je_editor.utils.exception.je_editor_exceptions import JEditorExecException
 
-language_compiler = {"java": "javac"}
-language_compiler_param = {"java": "-encoding UTF-8 -d -cp ."}
+from PySide6.QtCore import QTimer
+from PySide6.QtWidgets import QMainWindow, QTextEdit
+
+from je_editor.pyside_ui.colors.global_color import error_color, output_color
+from je_editor.utils.exception.exception_tags import compiler_not_found_error, je_editor_init_error
+from je_editor.utils.exception.exception_tags import file_not_fond_error
+from je_editor.utils.exception.exceptions import JEditorExecException, JEditorException
 
 
 class ExecManager(object):
 
     def __init__(
             self,
-            run_result,
-            process_error_function,
-            main_window,
-            running_menu,
+            main_window=None,
             program_language="python",
-            program_encoding="utf-8"
+            program_encoding="utf-8",
+            program_buffer=10240000,
     ):
+        """
+        :param main_window: tkinter main window
+        :param program_language: which program language
+        :param program_encoding: which encoding
+        """
         self.read_program_error_output_from_thread = None
         self.read_program_output_from_thread = None
-        self.main_window = main_window
+        self.main_window: QMainWindow = main_window
+        self.code_result: [QTextEdit, None] = None
+        self.timer: [QTimer, None] = None
         self.still_run_program = True
-        self.run_result = run_result
-        self.process_error_function = process_error_function
         self.process = None
         self.run_output_queue = queue.Queue()
         self.run_error_queue = queue.Queue()
         self.program_language = program_language
-        self.running_menu = running_menu
         self.program_encoding = program_encoding
+        self.program_buffer = program_buffer
+
+    def later_init(self):
+        if self.main_window is not None:
+            self.code_result: QTextEdit = self.main_window.code_result
+            self.timer = QTimer(self.main_window)
+        else:
+            raise JEditorException(je_editor_init_error)
 
     def exec_code(self, exec_file_name):
         """
         :param exec_file_name: string file will open to run
         :return: if error return result and True else return result and False
         """
-        self.exit_program()
-        self.running_menu.entryconfigure(1, label="Rerun")
-        self.running_menu.entryconfigure(3, state="normal")
-        self.run_result.configure(state=NORMAL)
-        self.run_result.delete("1.0", "end-1c")
-        self.run_result.configure(state=DISABLED)
-        reformat_os_file_path = os.path.abspath(exec_file_name)
         try:
-            if not Path(exec_file_name).exists():
-                raise JEditorExecException(file_not_fond_error)
-        except OSError as error:
-            raise JEditorExecException(error)
-        if sys.platform in ["linux", "linux2", "win32", "cygwin", "msys"]:
-            compiler_path = shutil.which(self.program_language)
-        else:
+            self.exit_program()
+            self.code_result.setPlainText("")
+            reformat_os_file_path = os.path.abspath(exec_file_name)
+            # detect file is exist
+            try:
+                if not Path(exec_file_name).exists():
+                    raise JEditorExecException(file_not_fond_error)
+            except OSError as error:
+                raise JEditorExecException(error)
             compiler_path = shutil.which(self.program_language)
-        if compiler_path is None:
-            raise JEditorExecException(python_not_found_error)
-        exec_command = reformat_os_file_path
-
-        if self.program_language in language_compiler:
+            if compiler_path is None and self.program_language == "python":
+                compiler_path = shutil.which("python3")
+            elif compiler_path is None and self.program_language == "python3":
+                compiler_path = shutil.which("python")
+            if compiler_path is None:
+                raise JEditorExecException(compiler_not_found_error)
+            exec_file = reformat_os_file_path
+            # run program
+            execute_program_list = [compiler_path, exec_file]
             self.process = subprocess.Popen(
-                [
-                    shutil.which(language_compiler.get(self.program_language)),
-                    language_compiler_param.get(self.program_language),
-                    reformat_os_file_path
-                ],
+                execute_program_list,
                 stdout=subprocess.PIPE,
                 stderr=subprocess.PIPE,
+                stdin=subprocess.PIPE,
                 shell=False
             )
-            while self.process.returncode is None:
-                self.process.poll()
-        self.process = subprocess.Popen([compiler_path, exec_command],
-                                        stdout=subprocess.PIPE,
-                                        stderr=subprocess.PIPE,
-                                        shell=False)
-        self.still_run_program = True
-        self.read_program_output_from_thread = Thread(
-            target=self.read_program_output_from_process,
-        )
-        self.read_program_output_from_thread.setDaemon(True)
-        self.read_program_output_from_thread.start()
-        self.read_program_error_output_from_thread = Thread(
-            target=self.read_program_error_output_from_process,
-        )
-        self.read_program_error_output_from_thread.setDaemon(True)
-        self.read_program_error_output_from_thread.start()
-        self.run_result.configure(state=NORMAL)
-        self.run_result.insert(END, compiler_path + " " + reformat_os_file_path + "\n")
-        self.run_result.configure(state=DISABLED)
-        self.edit_tkinter_text()
-
-    def edit_tkinter_text(self):
-        self.run_result.configure(state=NORMAL)
-        if not self.run_error_queue.empty():
-            error_message = self.run_error_queue.get_nowait()
-            self.process_error_function(self.run_result, error_message)
-        if not self.run_output_queue.empty():
-            output_message = self.run_output_queue.get_nowait()
-            self.run_result.insert(END, output_message)
-        self.run_result.configure(state=DISABLED)
-        if self.process.returncode is not None:
+            self.still_run_program = True
+            # program output message queue thread
+            self.read_program_output_from_thread = Thread(
+                target=self.read_program_output_from_process,
+                daemon=True
+            )
+            self.read_program_output_from_thread.start()
+            # program error message queue thread
+            self.read_program_error_output_from_thread = Thread(
+                target=self.read_program_error_output_from_process,
+                daemon=True
+            )
+            self.read_program_error_output_from_thread.start()
+            # show which file execute
+            self.code_result.append(compiler_path + " " + reformat_os_file_path)
+            # start tkinter_ui update
+            # start timer
+            self.timer = QTimer(self.main_window)
+            self.timer.setInterval(1)
+            self.timer.timeout.connect(self.pull_text)
+            self.timer.start()
+        except Exception as error:
+            self.code_result.setTextColor(error_color)
+            self.code_result.append(str(error))
+            self.code_result.setTextColor(output_color)
+
+    # tkinter_ui update method
+    def pull_text(self):
+        try:
+            self.code_result.setTextColor(error_color)
+            if not self.run_error_queue.empty():
+                error_message = self.run_error_queue.get_nowait()
+                error_message = str(error_message).strip()
+                if error_message:
+                    self.code_result.append(error_message)
+            self.code_result.setTextColor(output_color)
+            if not self.run_output_queue.empty():
+                output_message = self.run_output_queue.get_nowait()
+                output_message = str(output_message).strip()
+                if output_message:
+                    self.code_result.append(output_message)
+        except queue.Empty:
+            pass
+        if self.process.returncode == 0:
+            self.exit_program()
+        elif self.process.returncode is not None:
             self.exit_program()
+            self.timer.stop()
         if self.still_run_program:
-            self.main_window.after(10, self.edit_tkinter_text)
+            # poll return code
             self.process.poll()
-        else:
-            self.running_menu.entryconfigure(1, label="Run")
-            self.running_menu.entryconfigure(3, state="disable")
 
+    # exit program change run flag to false and clean read thread and queue and process
     def exit_program(self):
         self.still_run_program = False
         if self.read_program_output_from_thread is not None:
             self.read_program_output_from_thread = None
         if self.read_program_error_output_from_thread is not None:
             self.read_program_error_output_from_thread = None
-        self.run_output_queue = queue.Queue()
-        self.run_error_queue = queue.Queue()
+        self.print_and_clear_queue()
         if self.process is not None:
             self.process.terminate()
 
+    def print_and_clear_queue(self):
+        try:
+            for std_output in iter(self.run_output_queue.get_nowait, None):
+                std_output = str(std_output).strip()
+                if std_output:
+                    self.code_result.append(std_output)
+            self.code_result.setTextColor(error_color)
+            for std_err in iter(self.run_error_queue.get_nowait, None):
+                std_err = str(std_err).strip()
+                if std_err:
+                    self.code_result.append(std_err)
+            self.code_result.setTextColor(output_color)
+        except queue.Empty:
+            pass
+        self.run_output_queue = queue.Queue()
+        self.run_error_queue = queue.Queue()
+
     def read_program_output_from_process(self):
         while self.still_run_program:
-            program_output_data = self.process.stdout.raw.read(1024).decode(self.program_encoding)
-            self.run_output_queue.put(program_output_data)
+            program_output_data = self.process.stdout.raw.read(self.program_buffer).decode(self.program_encoding)
+            self.run_output_queue.put_nowait(program_output_data)
 
     def read_program_error_output_from_process(self):
         while self.still_run_program:
-            program_error_output_data = self.process.stderr.raw.read(1024).decode(self.program_encoding)
-            self.run_error_queue.put(program_error_output_data)
+            program_error_output_data = self.process.stderr.raw.read(self.program_buffer).decode(self.program_encoding)
+            self.run_error_queue.put_nowait(program_error_output_data)
+
+
+exec_manage = ExecManager()
```

### Comparing `je_editor_dev-0.0.9/je_editor_dev.egg-info/SOURCES.txt` & `je_editor_dev-0.0.90/je_editor_dev.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,68 +1,70 @@
 LICENSE
 README.md
-dev_setup.py
-setup.py
+pyproject.toml
 je_editor/__init__.py
-je_editor/ui/__init__.py
-je_editor/ui/editor_main_ui/__init__.py
-je_editor/ui/editor_main_ui/tkinter_editor.py
-je_editor/ui/ui_event/__init__.py
-je_editor/ui/ui_event/auto_save/__init__.py
-je_editor/ui/ui_event/auto_save/start_auto_save/__init__.py
-je_editor/ui/ui_event/auto_save/start_auto_save/start_auto_save.py
-je_editor/ui/ui_event/change_font/__init__.py
-je_editor/ui/ui_event/change_font/change_font.py
-je_editor/ui/ui_event/close/__init__.py
-je_editor/ui/ui_event/close/close_event.py
-je_editor/ui/ui_event/encoding/__init__.py
-je_editor/ui/ui_event/encoding/set_encoding.py
-je_editor/ui/ui_event/execute/__init__.py
-je_editor/ui/ui_event/execute/execute_code/__init__.py
-je_editor/ui/ui_event/execute/execute_code/exec_code.py
-je_editor/ui/ui_event/execute/execute_shell_command/__init__.py
-je_editor/ui/ui_event/execute/execute_shell_command/run_on_shell.py
-je_editor/ui/ui_event/language/__init__.py
-je_editor/ui/ui_event/language/set_language.py
-je_editor/ui/ui_event/open_file/__init__.py
-je_editor/ui/ui_event/open_file/open_file_to_read/__init__.py
-je_editor/ui/ui_event/open_file/open_file_to_read/open_file_to_read.py
-je_editor/ui/ui_event/open_file/open_last_edit_file/__init__.py
-je_editor/ui/ui_event/open_file/open_last_edit_file/open_last_edit_file.py
-je_editor/ui/ui_event/save_file/__init__.py
-je_editor/ui/ui_event/save_file/save_file_to_open/__init__.py
-je_editor/ui/ui_event/save_file/save_file_to_open/save_file_to_open.py
-je_editor/ui/ui_utils/__init__.py
-je_editor/ui/ui_utils/font/__init__.py
-je_editor/ui/ui_utils/font/font.py
+je_editor/__main__.py
+je_editor/start_editor.py
+je_editor/pyside_ui/__init__.py
+je_editor/pyside_ui/auto_save/__init__.py
+je_editor/pyside_ui/auto_save/auto_save_thread.py
+je_editor/pyside_ui/code_editor/__init__.py
+je_editor/pyside_ui/code_editor/code_edit_plaintext.py
+je_editor/pyside_ui/code_process/__init__.py
+je_editor/pyside_ui/code_process/code_exec.py
+je_editor/pyside_ui/code_result/__init__.py
+je_editor/pyside_ui/code_result/code_record.py
+je_editor/pyside_ui/colors/__init__.py
+je_editor/pyside_ui/colors/global_color.py
+je_editor/pyside_ui/file_dialog/__init__.py
+je_editor/pyside_ui/file_dialog/open_file_dialog.py
+je_editor/pyside_ui/file_dialog/save_file_dialog.py
+je_editor/pyside_ui/main_ui/__init__.py
+je_editor/pyside_ui/main_ui/editor_main_ui/__init__.py
+je_editor/pyside_ui/main_ui/editor_main_ui/main_editor.py
+je_editor/pyside_ui/main_ui_setting/__init__.py
+je_editor/pyside_ui/main_ui_setting/ui_setting.py
+je_editor/pyside_ui/menu/__init__.py
+je_editor/pyside_ui/menu/menu_bar/__init__.py
+je_editor/pyside_ui/menu/menu_bar/set_menu_bar.py
+je_editor/pyside_ui/menu/menu_bar/check_style_menu/__init__.py
+je_editor/pyside_ui/menu/menu_bar/check_style_menu/build_check_style_menu.py
+je_editor/pyside_ui/menu/menu_bar/file_menu/__init__.py
+je_editor/pyside_ui/menu/menu_bar/file_menu/build_file_menu.py
+je_editor/pyside_ui/menu/menu_bar/help_menu/__init__.py
+je_editor/pyside_ui/menu/menu_bar/help_menu/build_help_menu.py
+je_editor/pyside_ui/menu/menu_bar/run_menu/__init__.py
+je_editor/pyside_ui/menu/menu_bar/run_menu/build_run_menu.py
+je_editor/pyside_ui/search_ui/__init__.py
+je_editor/pyside_ui/search_ui/search_error_box.py
+je_editor/pyside_ui/search_ui/search_text_box.py
+je_editor/pyside_ui/shell_process/__init__.py
+je_editor/pyside_ui/shell_process/shell_exec.py
+je_editor/pyside_ui/syntax/__init__.py
+je_editor/pyside_ui/syntax/python_syntax.py
+je_editor/pyside_ui/treeview/__init__.py
+je_editor/pyside_ui/treeview/project_treeview/__init__.py
+je_editor/pyside_ui/treeview/project_treeview/set_project_treeview.py
+je_editor/pyside_ui/user_setting/__init__.py
+je_editor/pyside_ui/user_setting/user_setting_file.py
 je_editor/utils/__init__.py
-je_editor/utils/code_tag/__init__.py
-je_editor/utils/code_tag/keyword_list.py
-je_editor/utils/code_tag/tag_keyword.py
-je_editor/utils/editor_content/__init__.py
-je_editor/utils/editor_content/content_save.py
-je_editor/utils/encoding/__init__.py
-je_editor/utils/encoding/encoding_data_module.py
+je_editor/utils/encodings/__init__.py
+je_editor/utils/encodings/python_encodings.py
 je_editor/utils/exception/__init__.py
-je_editor/utils/exception/je_editor_exception_tag.py
-je_editor/utils/exception/je_editor_exceptions.py
+je_editor/utils/exception/exception_tags.py
+je_editor/utils/exception/exceptions.py
 je_editor/utils/file/__init__.py
 je_editor/utils/file/open/__init__.py
 je_editor/utils/file/open/open_file.py
 je_editor/utils/file/save/__init__.py
 je_editor/utils/file/save/save_file.py
-je_editor/utils/language/__init__.py
-je_editor/utils/language/language_data_module.py
-je_editor/utils/string_translate/__init__.py
-je_editor/utils/string_translate/used_string.py
-je_editor/utils/text_process/__init__.py
-je_editor/utils/text_process/program_exec/__init__.py
-je_editor/utils/text_process/program_exec/exec_text.py
-je_editor/utils/text_process/program_exec/process_error.py
-je_editor/utils/text_process/shell/__init__.py
-je_editor/utils/text_process/shell/shell_text.py
-je_editor/utils/theme/__init__.py
-je_editor/utils/theme/theme.py
+je_editor/utils/json/__init__.py
+je_editor/utils/json/json_file.py
+je_editor/utils/json_format/__init__.py
+je_editor/utils/json_format/json_process.py
+je_editor/utils/redirect_manager/__init__.py
+je_editor/utils/redirect_manager/redirect_manager_class.py
 je_editor_dev.egg-info/PKG-INFO
 je_editor_dev.egg-info/SOURCES.txt
 je_editor_dev.egg-info/dependency_links.txt
+je_editor_dev.egg-info/requires.txt
 je_editor_dev.egg-info/top_level.txt
```

