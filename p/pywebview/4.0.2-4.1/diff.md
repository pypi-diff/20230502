# Comparing `tmp/pywebview-4.0.2.tar.gz` & `tmp/pywebview-4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywebview-4.0.2.tar", last modified: Tue Feb 21 21:49:45 2023, max compression
+gzip compressed data, was "pywebview-4.1.tar", last modified: Tue May  2 12:52:36 2023, max compression
```

## Comparing `pywebview-4.0.2.tar` & `pywebview-4.1.tar`

### file list

```diff
@@ -1,53 +1,88 @@
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-02-21 21:49:45.805917 pywebview-4.0.2/
--rw-r--r--   0 roman      (501) staff       (20)     1518 2021-05-23 19:47:41.000000 pywebview-4.0.2/LICENSE.md
--rw-r--r--   0 roman      (501) staff       (20)      384 2023-01-17 21:06:35.000000 pywebview-4.0.2/MANIFEST.in
--rw-r--r--   0 roman      (501) staff       (20)     6792 2023-02-21 21:49:45.805658 pywebview-4.0.2/PKG-INFO
--rw-r--r--   0 roman      (501) staff       (20)     4804 2022-03-08 09:38:16.000000 pywebview-4.0.2/README.md
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-02-21 21:49:45.785686 pywebview-4.0.2/pywebview.egg-info/
--rw-r--r--   0 roman      (501) staff       (20)     6792 2023-02-21 21:49:45.000000 pywebview-4.0.2/pywebview.egg-info/PKG-INFO
--rw-r--r--   0 roman      (501) staff       (20)     1066 2023-02-21 21:49:45.000000 pywebview-4.0.2/pywebview.egg-info/SOURCES.txt
--rw-r--r--   0 roman      (501) staff       (20)        1 2023-02-21 21:49:45.000000 pywebview-4.0.2/pywebview.egg-info/dependency_links.txt
--rw-r--r--   0 roman      (501) staff       (20)      342 2023-02-21 21:49:45.000000 pywebview-4.0.2/pywebview.egg-info/requires.txt
--rw-r--r--   0 roman      (501) staff       (20)        8 2023-02-21 21:49:45.000000 pywebview-4.0.2/pywebview.egg-info/top_level.txt
--rw-r--r--   0 roman      (501) staff       (20)       38 2023-02-21 21:49:45.805999 pywebview-4.0.2/setup.cfg
--rw-r--r--   0 roman      (501) staff       (20)     2853 2023-02-21 20:55:55.000000 pywebview-4.0.2/setup.py
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-02-21 21:49:45.790864 pywebview-4.0.2/webview/
--rwxr-xr-x   0 roman      (501) staff       (20)     8756 2023-02-21 20:55:30.000000 pywebview-4.0.2/webview/__init__.py
--rw-r--r--   0 roman      (501) staff       (20)     1684 2023-01-17 21:06:35.000000 pywebview-4.0.2/webview/event.py
--rw-r--r--   0 roman      (501) staff       (20)     2956 2023-01-17 21:06:35.000000 pywebview-4.0.2/webview/guilib.py
--rw-r--r--   0 roman      (501) staff       (20)     4793 2023-02-21 20:55:30.000000 pywebview-4.0.2/webview/http.py
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-02-21 21:49:45.795264 pywebview-4.0.2/webview/js/
--rw-r--r--   0 roman      (501) staff       (20)       55 2022-02-16 20:39:21.000000 pywebview-4.0.2/webview/js/__init__.py
--rw-r--r--   0 roman      (501) staff       (20)      163 2022-11-13 21:33:18.000000 pywebview-4.0.2/webview/js/alert.py
--rwxr-xr-x   0 roman      (501) staff       (20)     3674 2023-01-17 21:06:35.000000 pywebview-4.0.2/webview/js/api.py
--rw-r--r--   0 roman      (501) staff       (20)      518 2021-05-23 19:47:41.000000 pywebview-4.0.2/webview/js/css.py
--rw-r--r--   0 roman      (501) staff       (20)    26111 2022-11-15 06:56:03.000000 pywebview-4.0.2/webview/js/dom.py
--rw-r--r--   0 roman      (501) staff       (20)     1479 2023-01-17 21:06:35.000000 pywebview-4.0.2/webview/js/drag.py
--rw-r--r--   0 roman      (501) staff       (20)      512 2022-02-16 20:39:21.000000 pywebview-4.0.2/webview/js/event.py
--rw-r--r--   0 roman      (501) staff       (20)     8127 2022-11-15 06:56:03.000000 pywebview-4.0.2/webview/js/npo.py
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-02-21 21:49:45.798618 pywebview-4.0.2/webview/lib/
--rw-r--r--   0 roman      (501) staff       (20)   423864 2023-01-17 21:06:35.000000 pywebview-4.0.2/webview/lib/Microsoft.Web.WebView2.Core.dll
--rw-r--r--   0 roman      (501) staff       (20)     1609 2022-02-16 20:39:21.000000 pywebview-4.0.2/webview/lib/Microsoft.Web.WebView2.LICENSE.md
--rw-r--r--   0 roman      (501) staff       (20)    37816 2023-01-17 21:06:35.000000 pywebview-4.0.2/webview/lib/Microsoft.Web.WebView2.WinForms.dll
--rw-r--r--   0 roman      (501) staff       (20)     7168 2022-02-16 20:39:21.000000 pywebview-4.0.2/webview/lib/WebBrowserInterop.x64.dll
--rw-r--r--   0 roman      (501) staff       (20)     7168 2022-02-16 20:39:21.000000 pywebview-4.0.2/webview/lib/WebBrowserInterop.x86.dll
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-02-21 21:49:45.799399 pywebview-4.0.2/webview/lib/arm64/
--rw-r--r--   0 roman      (501) staff       (20)   132024 2023-01-17 21:06:35.000000 pywebview-4.0.2/webview/lib/arm64/WebView2Loader.dll
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-02-21 21:49:45.800104 pywebview-4.0.2/webview/lib/x64/
--rw-r--r--   0 roman      (501) staff       (20)   158672 2023-01-17 21:06:35.000000 pywebview-4.0.2/webview/lib/x64/WebView2Loader.dll
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-02-21 21:49:45.800590 pywebview-4.0.2/webview/lib/x86/
--rw-r--r--   0 roman      (501) staff       (20)   115128 2023-01-17 21:06:35.000000 pywebview-4.0.2/webview/lib/x86/WebView2Loader.dll
--rw-r--r--   0 roman      (501) staff       (20)      762 2022-03-08 09:38:16.000000 pywebview-4.0.2/webview/localization.py
--rw-r--r--   0 roman      (501) staff       (20)      548 2023-01-17 21:06:35.000000 pywebview-4.0.2/webview/menu.py
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-02-21 21:49:45.804654 pywebview-4.0.2/webview/platforms/
--rw-r--r--   0 roman      (501) staff       (20)        0 2022-02-16 20:39:21.000000 pywebview-4.0.2/webview/platforms/__init__.py
--rw-r--r--   0 roman      (501) staff       (20)    10566 2023-01-27 21:52:44.000000 pywebview-4.0.2/webview/platforms/cef.py
--rw-r--r--   0 roman      (501) staff       (20)    42842 2023-02-21 20:55:30.000000 pywebview-4.0.2/webview/platforms/cocoa.py
--rw-r--r--   0 roman      (501) staff       (20)     7768 2023-02-09 20:30:33.000000 pywebview-4.0.2/webview/platforms/edgechromium.py
--rwxr-xr-x   0 roman      (501) staff       (20)    26436 2023-02-21 20:52:17.000000 pywebview-4.0.2/webview/platforms/gtk.py
--rw-r--r--   0 roman      (501) staff       (20)     6427 2023-01-17 21:06:35.000000 pywebview-4.0.2/webview/platforms/mshtml.py
--rwxr-xr-x   0 roman      (501) staff       (20)    31513 2023-02-21 20:52:17.000000 pywebview-4.0.2/webview/platforms/qt.py
--rw-r--r--   0 roman      (501) staff       (20)    25812 2023-02-21 21:44:26.000000 pywebview-4.0.2/webview/platforms/winforms.py
--rw-r--r--   0 roman      (501) staff       (20)      250 2022-11-15 06:56:03.000000 pywebview-4.0.2/webview/screen.py
--rw-r--r--   0 roman      (501) staff       (20)     8421 2023-02-21 20:55:30.000000 pywebview-4.0.2/webview/util.py
--rw-r--r--   0 roman      (501) staff       (20)    13925 2023-02-21 21:40:27.000000 pywebview-4.0.2/webview/window.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-05-02 12:52:36.771821 pywebview-4.1/
+-rw-r--r--   0 roman      (501) staff       (20)     1518 2023-05-02 12:23:59.000000 pywebview-4.1/LICENSE.md
+-rw-r--r--   0 roman      (501) staff       (20)      384 2023-05-02 12:23:59.000000 pywebview-4.1/MANIFEST.in
+-rw-r--r--   0 roman      (501) staff       (20)     6206 2023-05-02 12:52:36.771595 pywebview-4.1/PKG-INFO
+-rw-r--r--   0 roman      (501) staff       (20)     4804 2023-05-02 12:23:59.000000 pywebview-4.1/README.md
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-05-02 12:52:36.751135 pywebview-4.1/pywebview.egg-info/
+-rw-r--r--   0 roman      (501) staff       (20)     6206 2023-05-02 12:52:36.000000 pywebview-4.1/pywebview.egg-info/PKG-INFO
+-rw-r--r--   0 roman      (501) staff       (20)     1907 2023-05-02 12:52:36.000000 pywebview-4.1/pywebview.egg-info/SOURCES.txt
+-rw-r--r--   0 roman      (501) staff       (20)        1 2023-05-02 12:52:36.000000 pywebview-4.1/pywebview.egg-info/dependency_links.txt
+-rw-r--r--   0 roman      (501) staff       (20)      342 2023-05-02 12:52:36.000000 pywebview-4.1/pywebview.egg-info/requires.txt
+-rw-r--r--   0 roman      (501) staff       (20)        8 2023-05-02 12:52:36.000000 pywebview-4.1/pywebview.egg-info/top_level.txt
+-rw-r--r--   0 roman      (501) staff       (20)       38 2023-05-02 12:52:36.771869 pywebview-4.1/setup.cfg
+-rw-r--r--   0 roman      (501) staff       (20)     2849 2023-05-02 12:24:27.000000 pywebview-4.1/setup.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-05-02 12:52:36.757556 pywebview-4.1/tests/
+-rw-r--r--   0 roman      (501) staff       (20)      991 2023-05-02 12:23:59.000000 pywebview-4.1/tests/test_bg_color.py
+-rwxr-xr-x   0 roman      (501) staff       (20)     2565 2023-05-02 12:23:59.000000 pywebview-4.1/tests/test_evaluate_js.py
+-rw-r--r--   0 roman      (501) staff       (20)     1329 2023-05-02 12:23:59.000000 pywebview-4.1/tests/test_expose.py
+-rw-r--r--   0 roman      (501) staff       (20)      194 2023-05-02 12:23:59.000000 pywebview-4.1/tests/test_frameless.py
+-rw-r--r--   0 roman      (501) staff       (20)      198 2023-05-02 12:23:59.000000 pywebview-4.1/tests/test_fullscreen.py
+-rw-r--r--   0 roman      (501) staff       (20)      502 2023-05-02 12:23:59.000000 pywebview-4.1/tests/test_get_current_url.py
+-rw-r--r--   0 roman      (501) staff       (20)     1235 2023-05-02 12:23:59.000000 pywebview-4.1/tests/test_get_elements.py
+-rw-r--r--   0 roman      (501) staff       (20)      293 2023-05-02 12:23:59.000000 pywebview-4.1/tests/test_hide_window.py
+-rw-r--r--   0 roman      (501) staff       (20)      822 2023-05-02 12:23:59.000000 pywebview-4.1/tests/test_http_server.py
+-rwxr-xr-x   0 roman      (501) staff       (20)     2214 2023-05-02 12:23:59.000000 pywebview-4.1/tests/test_js_api.py
+-rw-r--r--   0 roman      (501) staff       (20)      252 2023-05-02 12:23:59.000000 pywebview-4.1/tests/test_load_html.py
+-rw-r--r--   0 roman      (501) staff       (20)     1058 2023-05-02 12:23:59.000000 pywebview-4.1/tests/test_localization.py
+-rw-r--r--   0 roman      (501) staff       (20)      196 2023-05-02 12:23:59.000000 pywebview-4.1/tests/test_min_size.py
+-rw-r--r--   0 roman      (501) staff       (20)      555 2023-05-02 12:23:59.000000 pywebview-4.1/tests/test_move_window.py
+-rw-r--r--   0 roman      (501) staff       (20)     2452 2023-05-02 12:23:59.000000 pywebview-4.1/tests/test_multi_window.py
+-rw-r--r--   0 roman      (501) staff       (20)      271 2023-05-02 12:23:59.000000 pywebview-4.1/tests/test_noresize.py
+-rw-r--r--   0 roman      (501) staff       (20)      375 2023-05-02 12:23:59.000000 pywebview-4.1/tests/test_on_top.py
+-rw-r--r--   0 roman      (501) staff       (20)      427 2023-05-02 12:23:59.000000 pywebview-4.1/tests/test_resize.py
+-rw-r--r--   0 roman      (501) staff       (20)       74 2023-05-02 12:23:59.000000 pywebview-4.1/tests/test_screens.py
+-rw-r--r--   0 roman      (501) staff       (20)      247 2023-05-02 12:23:59.000000 pywebview-4.1/tests/test_set_title.py
+-rw-r--r--   0 roman      (501) staff       (20)      186 2023-05-02 12:23:59.000000 pywebview-4.1/tests/test_simple_browser.py
+-rw-r--r--   0 roman      (501) staff       (20)      801 2023-05-02 12:23:59.000000 pywebview-4.1/tests/test_start.py
+-rw-r--r--   0 roman      (501) staff       (20)      279 2023-05-02 12:23:59.000000 pywebview-4.1/tests/test_toggle_fullscreen.py
+-rw-r--r--   0 roman      (501) staff       (20)      797 2023-05-02 12:23:59.000000 pywebview-4.1/tests/test_token.py
+-rw-r--r--   0 roman      (501) staff       (20)      265 2023-05-02 12:23:59.000000 pywebview-4.1/tests/test_url_load.py
+-rw-r--r--   0 roman      (501) staff       (20)      315 2023-05-02 12:23:59.000000 pywebview-4.1/tests/test_vibrancy.py
+-rw-r--r--   0 roman      (501) staff       (20)      238 2023-05-02 12:23:59.000000 pywebview-4.1/tests/test_window.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-05-02 12:52:36.759953 pywebview-4.1/webview/
+-rwxr-xr-x   0 roman      (501) staff       (20)    11374 2023-05-02 12:23:59.000000 pywebview-4.1/webview/__init__.py
+-rw-r--r--   0 roman      (501) staff       (20)     1684 2023-05-02 12:23:59.000000 pywebview-4.1/webview/event.py
+-rw-r--r--   0 roman      (501) staff       (20)     2956 2023-05-02 12:23:59.000000 pywebview-4.1/webview/guilib.py
+-rw-r--r--   0 roman      (501) staff       (20)     6813 2023-05-02 12:23:59.000000 pywebview-4.1/webview/http.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-05-02 12:52:36.762516 pywebview-4.1/webview/js/
+-rw-r--r--   0 roman      (501) staff       (20)       55 2023-05-02 12:23:59.000000 pywebview-4.1/webview/js/__init__.py
+-rw-r--r--   0 roman      (501) staff       (20)      163 2023-05-02 12:23:59.000000 pywebview-4.1/webview/js/alert.py
+-rwxr-xr-x   0 roman      (501) staff       (20)     3674 2023-01-17 21:06:35.000000 pywebview-4.1/webview/js/api.py
+-rw-r--r--   0 roman      (501) staff       (20)      518 2023-05-02 12:23:59.000000 pywebview-4.1/webview/js/css.py
+-rw-r--r--   0 roman      (501) staff       (20)    26111 2023-05-02 12:23:59.000000 pywebview-4.1/webview/js/dom.py
+-rw-r--r--   0 roman      (501) staff       (20)     1479 2023-01-17 21:06:35.000000 pywebview-4.1/webview/js/drag.py
+-rw-r--r--   0 roman      (501) staff       (20)      512 2023-05-02 12:23:59.000000 pywebview-4.1/webview/js/event.py
+-rw-r--r--   0 roman      (501) staff       (20)     8127 2023-05-02 12:23:59.000000 pywebview-4.1/webview/js/npo.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-05-02 12:52:36.765399 pywebview-4.1/webview/lib/
+-rw-r--r--   0 roman      (501) staff       (20)   423864 2023-01-17 21:06:35.000000 pywebview-4.1/webview/lib/Microsoft.Web.WebView2.Core.dll
+-rw-r--r--   0 roman      (501) staff       (20)     1609 2023-05-02 12:23:59.000000 pywebview-4.1/webview/lib/Microsoft.Web.WebView2.LICENSE.md
+-rw-r--r--   0 roman      (501) staff       (20)    37816 2023-01-17 21:06:35.000000 pywebview-4.1/webview/lib/Microsoft.Web.WebView2.WinForms.dll
+-rw-r--r--   0 roman      (501) staff       (20)     7168 2022-02-16 20:39:21.000000 pywebview-4.1/webview/lib/WebBrowserInterop.x64.dll
+-rw-r--r--   0 roman      (501) staff       (20)     7168 2022-02-16 20:39:21.000000 pywebview-4.1/webview/lib/WebBrowserInterop.x86.dll
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-05-02 12:52:36.765702 pywebview-4.1/webview/lib/arm64/
+-rw-r--r--   0 roman      (501) staff       (20)   132024 2023-01-17 21:06:35.000000 pywebview-4.1/webview/lib/arm64/WebView2Loader.dll
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-05-02 12:52:36.766522 pywebview-4.1/webview/lib/x64/
+-rw-r--r--   0 roman      (501) staff       (20)   158672 2023-01-17 21:06:35.000000 pywebview-4.1/webview/lib/x64/WebView2Loader.dll
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-05-02 12:52:36.767188 pywebview-4.1/webview/lib/x86/
+-rw-r--r--   0 roman      (501) staff       (20)   115128 2023-01-17 21:06:35.000000 pywebview-4.1/webview/lib/x86/WebView2Loader.dll
+-rw-r--r--   0 roman      (501) staff       (20)      762 2023-05-02 12:23:59.000000 pywebview-4.1/webview/localization.py
+-rw-r--r--   0 roman      (501) staff       (20)      548 2023-05-02 12:23:59.000000 pywebview-4.1/webview/menu.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-05-02 12:52:36.769700 pywebview-4.1/webview/platforms/
+-rw-r--r--   0 roman      (501) staff       (20)        0 2022-02-16 20:39:21.000000 pywebview-4.1/webview/platforms/__init__.py
+-rw-r--r--   0 roman      (501) staff       (20)    10566 2023-05-02 12:23:59.000000 pywebview-4.1/webview/platforms/cef.py
+-rw-r--r--   0 roman      (501) staff       (20)    43762 2023-05-02 12:23:59.000000 pywebview-4.1/webview/platforms/cocoa.py
+-rw-r--r--   0 roman      (501) staff       (20)     7825 2023-05-02 12:23:59.000000 pywebview-4.1/webview/platforms/edgechromium.py
+-rwxr-xr-x   0 roman      (501) staff       (20)    26636 2023-05-02 12:23:59.000000 pywebview-4.1/webview/platforms/gtk.py
+-rw-r--r--   0 roman      (501) staff       (20)     6427 2023-05-02 12:23:59.000000 pywebview-4.1/webview/platforms/mshtml.py
+-rwxr-xr-x   0 roman      (501) staff       (20)    31932 2023-05-02 12:23:59.000000 pywebview-4.1/webview/platforms/qt.py
+-rw-r--r--   0 roman      (501) staff       (20)    26121 2023-05-02 12:23:59.000000 pywebview-4.1/webview/platforms/winforms.py
+-rw-r--r--   0 roman      (501) staff       (20)      250 2023-05-02 12:23:59.000000 pywebview-4.1/webview/screen.py
+-rw-r--r--   0 roman      (501) staff       (20)     8463 2023-05-02 12:23:59.000000 pywebview-4.1/webview/util.py
+-rw-r--r--   0 roman      (501) staff       (20)    13925 2023-05-02 12:23:59.000000 pywebview-4.1/webview/window.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-05-02 12:52:36.770948 pywebview-4.1/windows_interop/
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-05-02 12:52:36.771256 pywebview-4.1/windows_interop/Properties/
+-rw-r--r--   0 roman      (501) staff       (20)     1402 2023-05-02 12:23:59.000000 pywebview-4.1/windows_interop/Properties/AssemblyInfo.cs
+-rw-r--r--   0 roman      (501) staff       (20)      172 2023-05-02 12:23:59.000000 pywebview-4.1/windows_interop/README.txt
+-rw-r--r--   0 roman      (501) staff       (20)     5831 2022-02-16 20:39:21.000000 pywebview-4.1/windows_interop/WebBrowserInterop.cs
+-rw-r--r--   0 roman      (501) staff       (20)     5815 2023-05-02 12:23:59.000000 pywebview-4.1/windows_interop/WebBrowserInterop.csproj
+-rw-r--r--   0 roman      (501) staff       (20)     1674 2021-05-23 19:47:41.000000 pywebview-4.1/windows_interop/WebBrowserInterop.sln
```

### Comparing `pywebview-4.0.2/LICENSE.md` & `pywebview-4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pywebview-4.0.2/PKG-INFO` & `pywebview-4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,91 +1,17 @@
 Metadata-Version: 2.1
 Name: pywebview
-Version: 4.0.2
+Version: 4.1
 Summary: Build GUI for your Python program with JavaScript, HTML, and CSS.
 Home-page: https://github.com/r0x0r/pywebview
+Download-URL: https://github.com/r0x0r/pywebview/archive/4.1.tar.gz
 Author: Roman Sirokov
 Author-email: roman@flowrl.com
 License: New BSD license
-Download-URL: https://github.com/r0x0r/pywebview/archive/4.0.2.tar.gz
-Description: <p align='center'><img src='logo/logo.png' width=480 alt='pywebview logo'/></p>
-        
-        <p align='center'><a href="https://opencollective.com/pywebview" alt="Financial Contributors on Open Collective"><img src="https://opencollective.com/pywebview/all/badge.svg?label=financial+contributors" /></a> <img src="https://badge.fury.io/py/pywebview.svg" alt="PyPI version" /> <img src="https://img.shields.io/pypi/dm/pywebview" alt="PyPI downloads" /> <a href="https://ci.appveyor.com/project/r0x0r/pywebview"><img src="https://ci.appveyor.com/api/projects/status/nu6mbhvbq03wudxd/branch/master?svg=true" alt="Build status" /></a>
-        
-        https://pywebview.flowrl.com
-        </p>
-        
-        
-        _pywebview_ is a lightweight cross-platform wrapper around a webview component that allows to display HTML content in its own native GUI window. It gives you power of web technologies in your desktop application, hiding the fact that GUI is browser based. You can use pywebview either with a lightweight web framework like [Flask](http://flask.pocoo.org/) or [Bottle](http://bottlepy.org/docs/dev/index.html) or on its own with a two way bridge between Python and DOM.
-        
-        _pywebview_ uses native GUI for creating a web component window: WinForms on Windows, Cocoa on macOS and QT or GTK on Linux. If you choose to freeze your application, pywebview does not bundle a heavy GUI toolkit or web renderer with it keeping the executable size small. _pywebview_ is compatible with Python 3.
-        
-        _pywebview_ is created by [Roman Sirokov](https://github.com/r0x0r/).
-        
-        
-        # Getting started
-        
-        ### Install
-        
-        
-        ``` bash
-        pip install pywebview
-        ```
-        - _Currently only python version 3.8 or older supported on Windows._
-        - _On Linux you need additional libraries. Refer to the [installation](https://pywebview.flowrl.com/guide/installation.html) page for details._
-        
-        
-        ### Hello world
-        ``` python
-        import webview
-        webview.create_window('Hello world', 'https://pywebview.flowrl.com/hello')
-        webview.start()
-        ```
-        
-        Explore _pywebview_ further by reading [documentation](https://pywebview.flowrl.com/guide), [examples](https://pywebview.flowrl.com/examples) or [contributing](https://pywebview.flowrl.com/contributing). If React is your thing, get started right away with [React boilerplate](https://github.com/r0x0r/pywebview-react-boilerplate).
-        
-        
-        
-        # Contributors
-        
-        ### Code Contributors
-        
-        This project exists thanks to all the people who contribute. [[Contribute](CONTRIBUTING.md)].
-        <a href="https://github.com/r0x0r/pywebview/graphs/contributors"><img src="https://opencollective.com/pywebview/contributors.svg?width=890&button=false" /></a>
-        
-        ### Financial Contributors
-        
-        Become a financial contributor and help us sustain our community. More donation options are outlined on the [Donating](https://pywebview.flowrl.com/contributing/donating.html) page.
-        
-        
-        #### Individuals
-        
-        <a href="https://opencollective.com/pywebview"><img src="https://opencollective.com/pywebview/individuals.svg?width=890"></a>
-        
-        <a href="https://www.patreon.com/bePatron?u=13226105" data-patreon-widget-type="become-patron-button"><img src='https://c5.patreon.com/external/logo/become_a_patron_button.png' alt='Become a Patron!'/></a>
-        
-        
-        #### Organizations
-        
-        Support this project with your organization. Your logo will show up here with a link to your website. [[Contribute](https://opencollective.com/pywebview/contribute)]
-        
-        <a href="https://opencollective.com/pywebview/organization/0/website"><img src="https://opencollective.com/pywebview/organization/0/avatar.svg"></a>
-        <a href="https://opencollective.com/pywebview/organization/1/website"><img src="https://opencollective.com/pywebview/organization/1/avatar.svg"></a>
-        <a href="https://opencollective.com/pywebview/organization/2/website"><img src="https://opencollective.com/pywebview/organization/2/avatar.svg"></a>
-        <a href="https://opencollective.com/pywebview/organization/3/website"><img src="https://opencollective.com/pywebview/organization/3/avatar.svg"></a>
-        <a href="https://opencollective.com/pywebview/organization/4/website"><img src="https://opencollective.com/pywebview/organization/4/avatar.svg"></a>
-        <a href="https://opencollective.com/pywebview/organization/5/website"><img src="https://opencollective.com/pywebview/organization/5/avatar.svg"></a>
-        <a href="https://opencollective.com/pywebview/organization/6/website"><img src="https://opencollective.com/pywebview/organization/6/avatar.svg"></a>
-        <a href="https://opencollective.com/pywebview/organization/7/website"><img src="https://opencollective.com/pywebview/organization/7/avatar.svg"></a>
-        <a href="https://opencollective.com/pywebview/organization/8/website"><img src="https://opencollective.com/pywebview/organization/8/avatar.svg"></a>
-        <a href="https://opencollective.com/pywebview/organization/9/website"><img src="https://opencollective.com/pywebview/organization/9/avatar.svg"></a>
-        
-        
 Keywords: gui,webkit,html,web
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: MacOS X
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications :: GTK
 Classifier: Environment :: X11 Applications :: Qt
@@ -101,7 +27,81 @@
 Classifier: Topic :: Software Development :: User Interfaces
 Description-Content-Type: text/markdown
 Provides-Extra: cef
 Provides-Extra: gtk
 Provides-Extra: pyside2
 Provides-Extra: pyside6
 Provides-Extra: qt
+License-File: LICENSE.md
+
+<p align='center'><img src='logo/logo.png' width=480 alt='pywebview logo'/></p>
+
+<p align='center'><a href="https://opencollective.com/pywebview" alt="Financial Contributors on Open Collective"><img src="https://opencollective.com/pywebview/all/badge.svg?label=financial+contributors" /></a> <img src="https://badge.fury.io/py/pywebview.svg" alt="PyPI version" /> <img src="https://img.shields.io/pypi/dm/pywebview" alt="PyPI downloads" /> <a href="https://ci.appveyor.com/project/r0x0r/pywebview"><img src="https://ci.appveyor.com/api/projects/status/nu6mbhvbq03wudxd/branch/master?svg=true" alt="Build status" /></a>
+
+https://pywebview.flowrl.com
+</p>
+
+
+_pywebview_ is a lightweight cross-platform wrapper around a webview component that allows to display HTML content in its own native GUI window. It gives you power of web technologies in your desktop application, hiding the fact that GUI is browser based. You can use pywebview either with a lightweight web framework like [Flask](http://flask.pocoo.org/) or [Bottle](http://bottlepy.org/docs/dev/index.html) or on its own with a two way bridge between Python and DOM.
+
+_pywebview_ uses native GUI for creating a web component window: WinForms on Windows, Cocoa on macOS and QT or GTK on Linux. If you choose to freeze your application, pywebview does not bundle a heavy GUI toolkit or web renderer with it keeping the executable size small. _pywebview_ is compatible with Python 3.
+
+_pywebview_ is created by [Roman Sirokov](https://github.com/r0x0r/).
+
+
+# Getting started
+
+### Install
+
+
+``` bash
+pip install pywebview
+```
+- _Currently only python version 3.8 or older supported on Windows._
+- _On Linux you need additional libraries. Refer to the [installation](https://pywebview.flowrl.com/guide/installation.html) page for details._
+
+
+### Hello world
+``` python
+import webview
+webview.create_window('Hello world', 'https://pywebview.flowrl.com/hello')
+webview.start()
+```
+
+Explore _pywebview_ further by reading [documentation](https://pywebview.flowrl.com/guide), [examples](https://pywebview.flowrl.com/examples) or [contributing](https://pywebview.flowrl.com/contributing). If React is your thing, get started right away with [React boilerplate](https://github.com/r0x0r/pywebview-react-boilerplate).
+
+
+
+# Contributors
+
+### Code Contributors
+
+This project exists thanks to all the people who contribute. [[Contribute](CONTRIBUTING.md)].
+<a href="https://github.com/r0x0r/pywebview/graphs/contributors"><img src="https://opencollective.com/pywebview/contributors.svg?width=890&button=false" /></a>
+
+### Financial Contributors
+
+Become a financial contributor and help us sustain our community. More donation options are outlined on the [Donating](https://pywebview.flowrl.com/contributing/donating.html) page.
+
+
+#### Individuals
+
+<a href="https://opencollective.com/pywebview"><img src="https://opencollective.com/pywebview/individuals.svg?width=890"></a>
+
+<a href="https://www.patreon.com/bePatron?u=13226105" data-patreon-widget-type="become-patron-button"><img src='https://c5.patreon.com/external/logo/become_a_patron_button.png' alt='Become a Patron!'/></a>
+
+
+#### Organizations
+
+Support this project with your organization. Your logo will show up here with a link to your website. [[Contribute](https://opencollective.com/pywebview/contribute)]
+
+<a href="https://opencollective.com/pywebview/organization/0/website"><img src="https://opencollective.com/pywebview/organization/0/avatar.svg"></a>
+<a href="https://opencollective.com/pywebview/organization/1/website"><img src="https://opencollective.com/pywebview/organization/1/avatar.svg"></a>
+<a href="https://opencollective.com/pywebview/organization/2/website"><img src="https://opencollective.com/pywebview/organization/2/avatar.svg"></a>
+<a href="https://opencollective.com/pywebview/organization/3/website"><img src="https://opencollective.com/pywebview/organization/3/avatar.svg"></a>
+<a href="https://opencollective.com/pywebview/organization/4/website"><img src="https://opencollective.com/pywebview/organization/4/avatar.svg"></a>
+<a href="https://opencollective.com/pywebview/organization/5/website"><img src="https://opencollective.com/pywebview/organization/5/avatar.svg"></a>
+<a href="https://opencollective.com/pywebview/organization/6/website"><img src="https://opencollective.com/pywebview/organization/6/avatar.svg"></a>
+<a href="https://opencollective.com/pywebview/organization/7/website"><img src="https://opencollective.com/pywebview/organization/7/avatar.svg"></a>
+<a href="https://opencollective.com/pywebview/organization/8/website"><img src="https://opencollective.com/pywebview/organization/8/avatar.svg"></a>
+<a href="https://opencollective.com/pywebview/organization/9/website"><img src="https://opencollective.com/pywebview/organization/9/avatar.svg"></a>
+
```

#### html2text {}

```diff
@@ -1,12 +1,26 @@
-Metadata-Version: 2.1 Name: pywebview Version: 4.0.2 Summary: Build GUI for
-your Python program with JavaScript, HTML, and CSS. Home-page: https://
-github.com/r0x0r/pywebview Author: Roman Sirokov Author-email: roman@flowrl.com
-License: New BSD license Download-URL: https://github.com/r0x0r/pywebview/
-archive/4.0.2.tar.gz Description:
+Metadata-Version: 2.1 Name: pywebview Version: 4.1 Summary: Build GUI for your
+Python program with JavaScript, HTML, and CSS. Home-page: https://github.com/
+r0x0r/pywebview Download-URL: https://github.com/r0x0r/pywebview/archive/
+4.1.tar.gz Author: Roman Sirokov Author-email: roman@flowrl.com License: New
+BSD license Keywords: gui,webkit,html,web Classifier: Intended Audience ::
+Developers Classifier: License :: OSI Approved :: BSD License Classifier:
+Operating System :: OS Independent Classifier: Environment :: MacOS X
+Classifier: Environment :: Win32 (MS Windows) Classifier: Environment :: X11
+Applications :: GTK Classifier: Environment :: X11 Applications :: Qt
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.6 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Topic :: Software
+Development :: Libraries :: Application Frameworks Classifier: Topic ::
+Software Development :: Libraries :: Python Modules Classifier: Topic ::
+Software Development :: User Interfaces Description-Content-Type: text/markdown
+Provides-Extra: cef Provides-Extra: gtk Provides-Extra: pyside2 Provides-Extra:
+pyside6 Provides-Extra: qt License-File: LICENSE.md
                                [pywebview logo]
                   [https://opencollective.com/pywebview/all/
 badge.svg?label=financial+contributors] [PyPI version] [PyPI downloads] [Build
                      status] https://pywebview.flowrl.com
 _pywebview_ is a lightweight cross-platform wrapper around a webview component
 that allows to display HTML content in its own native GUI window. It gives you
 power of web technologies in your desktop application, hiding the fact that GUI
@@ -42,23 +56,8 @@
 opencollective.com/pywebview/organization/2/avatar.svg] [https://
 opencollective.com/pywebview/organization/3/avatar.svg] [https://
 opencollective.com/pywebview/organization/4/avatar.svg] [https://
 opencollective.com/pywebview/organization/5/avatar.svg] [https://
 opencollective.com/pywebview/organization/6/avatar.svg] [https://
 opencollective.com/pywebview/organization/7/avatar.svg] [https://
 opencollective.com/pywebview/organization/8/avatar.svg] [https://
-opencollective.com/pywebview/organization/9/avatar.svg] Keywords:
-gui,webkit,html,web Platform: UNKNOWN Classifier: Intended Audience ::
-Developers Classifier: License :: OSI Approved :: BSD License Classifier:
-Operating System :: OS Independent Classifier: Environment :: MacOS X
-Classifier: Environment :: Win32 (MS Windows) Classifier: Environment :: X11
-Applications :: GTK Classifier: Environment :: X11 Applications :: Qt
-Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Topic :: Software
-Development :: Libraries :: Application Frameworks Classifier: Topic ::
-Software Development :: Libraries :: Python Modules Classifier: Topic ::
-Software Development :: User Interfaces Description-Content-Type: text/markdown
-Provides-Extra: cef Provides-Extra: gtk Provides-Extra: pyside2 Provides-Extra:
-pyside6 Provides-Extra: qt
+opencollective.com/pywebview/organization/9/avatar.svg]
```

### Comparing `pywebview-4.0.2/README.md` & `pywebview-4.1/README.md`

 * *Files identical despite different names*

### Comparing `pywebview-4.0.2/pywebview.egg-info/PKG-INFO` & `pywebview-4.1/pywebview.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,91 +1,17 @@
 Metadata-Version: 2.1
 Name: pywebview
-Version: 4.0.2
+Version: 4.1
 Summary: Build GUI for your Python program with JavaScript, HTML, and CSS.
 Home-page: https://github.com/r0x0r/pywebview
+Download-URL: https://github.com/r0x0r/pywebview/archive/4.1.tar.gz
 Author: Roman Sirokov
 Author-email: roman@flowrl.com
 License: New BSD license
-Download-URL: https://github.com/r0x0r/pywebview/archive/4.0.2.tar.gz
-Description: <p align='center'><img src='logo/logo.png' width=480 alt='pywebview logo'/></p>
-        
-        <p align='center'><a href="https://opencollective.com/pywebview" alt="Financial Contributors on Open Collective"><img src="https://opencollective.com/pywebview/all/badge.svg?label=financial+contributors" /></a> <img src="https://badge.fury.io/py/pywebview.svg" alt="PyPI version" /> <img src="https://img.shields.io/pypi/dm/pywebview" alt="PyPI downloads" /> <a href="https://ci.appveyor.com/project/r0x0r/pywebview"><img src="https://ci.appveyor.com/api/projects/status/nu6mbhvbq03wudxd/branch/master?svg=true" alt="Build status" /></a>
-        
-        https://pywebview.flowrl.com
-        </p>
-        
-        
-        _pywebview_ is a lightweight cross-platform wrapper around a webview component that allows to display HTML content in its own native GUI window. It gives you power of web technologies in your desktop application, hiding the fact that GUI is browser based. You can use pywebview either with a lightweight web framework like [Flask](http://flask.pocoo.org/) or [Bottle](http://bottlepy.org/docs/dev/index.html) or on its own with a two way bridge between Python and DOM.
-        
-        _pywebview_ uses native GUI for creating a web component window: WinForms on Windows, Cocoa on macOS and QT or GTK on Linux. If you choose to freeze your application, pywebview does not bundle a heavy GUI toolkit or web renderer with it keeping the executable size small. _pywebview_ is compatible with Python 3.
-        
-        _pywebview_ is created by [Roman Sirokov](https://github.com/r0x0r/).
-        
-        
-        # Getting started
-        
-        ### Install
-        
-        
-        ``` bash
-        pip install pywebview
-        ```
-        - _Currently only python version 3.8 or older supported on Windows._
-        - _On Linux you need additional libraries. Refer to the [installation](https://pywebview.flowrl.com/guide/installation.html) page for details._
-        
-        
-        ### Hello world
-        ``` python
-        import webview
-        webview.create_window('Hello world', 'https://pywebview.flowrl.com/hello')
-        webview.start()
-        ```
-        
-        Explore _pywebview_ further by reading [documentation](https://pywebview.flowrl.com/guide), [examples](https://pywebview.flowrl.com/examples) or [contributing](https://pywebview.flowrl.com/contributing). If React is your thing, get started right away with [React boilerplate](https://github.com/r0x0r/pywebview-react-boilerplate).
-        
-        
-        
-        # Contributors
-        
-        ### Code Contributors
-        
-        This project exists thanks to all the people who contribute. [[Contribute](CONTRIBUTING.md)].
-        <a href="https://github.com/r0x0r/pywebview/graphs/contributors"><img src="https://opencollective.com/pywebview/contributors.svg?width=890&button=false" /></a>
-        
-        ### Financial Contributors
-        
-        Become a financial contributor and help us sustain our community. More donation options are outlined on the [Donating](https://pywebview.flowrl.com/contributing/donating.html) page.
-        
-        
-        #### Individuals
-        
-        <a href="https://opencollective.com/pywebview"><img src="https://opencollective.com/pywebview/individuals.svg?width=890"></a>
-        
-        <a href="https://www.patreon.com/bePatron?u=13226105" data-patreon-widget-type="become-patron-button"><img src='https://c5.patreon.com/external/logo/become_a_patron_button.png' alt='Become a Patron!'/></a>
-        
-        
-        #### Organizations
-        
-        Support this project with your organization. Your logo will show up here with a link to your website. [[Contribute](https://opencollective.com/pywebview/contribute)]
-        
-        <a href="https://opencollective.com/pywebview/organization/0/website"><img src="https://opencollective.com/pywebview/organization/0/avatar.svg"></a>
-        <a href="https://opencollective.com/pywebview/organization/1/website"><img src="https://opencollective.com/pywebview/organization/1/avatar.svg"></a>
-        <a href="https://opencollective.com/pywebview/organization/2/website"><img src="https://opencollective.com/pywebview/organization/2/avatar.svg"></a>
-        <a href="https://opencollective.com/pywebview/organization/3/website"><img src="https://opencollective.com/pywebview/organization/3/avatar.svg"></a>
-        <a href="https://opencollective.com/pywebview/organization/4/website"><img src="https://opencollective.com/pywebview/organization/4/avatar.svg"></a>
-        <a href="https://opencollective.com/pywebview/organization/5/website"><img src="https://opencollective.com/pywebview/organization/5/avatar.svg"></a>
-        <a href="https://opencollective.com/pywebview/organization/6/website"><img src="https://opencollective.com/pywebview/organization/6/avatar.svg"></a>
-        <a href="https://opencollective.com/pywebview/organization/7/website"><img src="https://opencollective.com/pywebview/organization/7/avatar.svg"></a>
-        <a href="https://opencollective.com/pywebview/organization/8/website"><img src="https://opencollective.com/pywebview/organization/8/avatar.svg"></a>
-        <a href="https://opencollective.com/pywebview/organization/9/website"><img src="https://opencollective.com/pywebview/organization/9/avatar.svg"></a>
-        
-        
 Keywords: gui,webkit,html,web
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: MacOS X
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications :: GTK
 Classifier: Environment :: X11 Applications :: Qt
@@ -101,7 +27,81 @@
 Classifier: Topic :: Software Development :: User Interfaces
 Description-Content-Type: text/markdown
 Provides-Extra: cef
 Provides-Extra: gtk
 Provides-Extra: pyside2
 Provides-Extra: pyside6
 Provides-Extra: qt
+License-File: LICENSE.md
+
+<p align='center'><img src='logo/logo.png' width=480 alt='pywebview logo'/></p>
+
+<p align='center'><a href="https://opencollective.com/pywebview" alt="Financial Contributors on Open Collective"><img src="https://opencollective.com/pywebview/all/badge.svg?label=financial+contributors" /></a> <img src="https://badge.fury.io/py/pywebview.svg" alt="PyPI version" /> <img src="https://img.shields.io/pypi/dm/pywebview" alt="PyPI downloads" /> <a href="https://ci.appveyor.com/project/r0x0r/pywebview"><img src="https://ci.appveyor.com/api/projects/status/nu6mbhvbq03wudxd/branch/master?svg=true" alt="Build status" /></a>
+
+https://pywebview.flowrl.com
+</p>
+
+
+_pywebview_ is a lightweight cross-platform wrapper around a webview component that allows to display HTML content in its own native GUI window. It gives you power of web technologies in your desktop application, hiding the fact that GUI is browser based. You can use pywebview either with a lightweight web framework like [Flask](http://flask.pocoo.org/) or [Bottle](http://bottlepy.org/docs/dev/index.html) or on its own with a two way bridge between Python and DOM.
+
+_pywebview_ uses native GUI for creating a web component window: WinForms on Windows, Cocoa on macOS and QT or GTK on Linux. If you choose to freeze your application, pywebview does not bundle a heavy GUI toolkit or web renderer with it keeping the executable size small. _pywebview_ is compatible with Python 3.
+
+_pywebview_ is created by [Roman Sirokov](https://github.com/r0x0r/).
+
+
+# Getting started
+
+### Install
+
+
+``` bash
+pip install pywebview
+```
+- _Currently only python version 3.8 or older supported on Windows._
+- _On Linux you need additional libraries. Refer to the [installation](https://pywebview.flowrl.com/guide/installation.html) page for details._
+
+
+### Hello world
+``` python
+import webview
+webview.create_window('Hello world', 'https://pywebview.flowrl.com/hello')
+webview.start()
+```
+
+Explore _pywebview_ further by reading [documentation](https://pywebview.flowrl.com/guide), [examples](https://pywebview.flowrl.com/examples) or [contributing](https://pywebview.flowrl.com/contributing). If React is your thing, get started right away with [React boilerplate](https://github.com/r0x0r/pywebview-react-boilerplate).
+
+
+
+# Contributors
+
+### Code Contributors
+
+This project exists thanks to all the people who contribute. [[Contribute](CONTRIBUTING.md)].
+<a href="https://github.com/r0x0r/pywebview/graphs/contributors"><img src="https://opencollective.com/pywebview/contributors.svg?width=890&button=false" /></a>
+
+### Financial Contributors
+
+Become a financial contributor and help us sustain our community. More donation options are outlined on the [Donating](https://pywebview.flowrl.com/contributing/donating.html) page.
+
+
+#### Individuals
+
+<a href="https://opencollective.com/pywebview"><img src="https://opencollective.com/pywebview/individuals.svg?width=890"></a>
+
+<a href="https://www.patreon.com/bePatron?u=13226105" data-patreon-widget-type="become-patron-button"><img src='https://c5.patreon.com/external/logo/become_a_patron_button.png' alt='Become a Patron!'/></a>
+
+
+#### Organizations
+
+Support this project with your organization. Your logo will show up here with a link to your website. [[Contribute](https://opencollective.com/pywebview/contribute)]
+
+<a href="https://opencollective.com/pywebview/organization/0/website"><img src="https://opencollective.com/pywebview/organization/0/avatar.svg"></a>
+<a href="https://opencollective.com/pywebview/organization/1/website"><img src="https://opencollective.com/pywebview/organization/1/avatar.svg"></a>
+<a href="https://opencollective.com/pywebview/organization/2/website"><img src="https://opencollective.com/pywebview/organization/2/avatar.svg"></a>
+<a href="https://opencollective.com/pywebview/organization/3/website"><img src="https://opencollective.com/pywebview/organization/3/avatar.svg"></a>
+<a href="https://opencollective.com/pywebview/organization/4/website"><img src="https://opencollective.com/pywebview/organization/4/avatar.svg"></a>
+<a href="https://opencollective.com/pywebview/organization/5/website"><img src="https://opencollective.com/pywebview/organization/5/avatar.svg"></a>
+<a href="https://opencollective.com/pywebview/organization/6/website"><img src="https://opencollective.com/pywebview/organization/6/avatar.svg"></a>
+<a href="https://opencollective.com/pywebview/organization/7/website"><img src="https://opencollective.com/pywebview/organization/7/avatar.svg"></a>
+<a href="https://opencollective.com/pywebview/organization/8/website"><img src="https://opencollective.com/pywebview/organization/8/avatar.svg"></a>
+<a href="https://opencollective.com/pywebview/organization/9/website"><img src="https://opencollective.com/pywebview/organization/9/avatar.svg"></a>
+
```

#### html2text {}

```diff
@@ -1,12 +1,26 @@
-Metadata-Version: 2.1 Name: pywebview Version: 4.0.2 Summary: Build GUI for
-your Python program with JavaScript, HTML, and CSS. Home-page: https://
-github.com/r0x0r/pywebview Author: Roman Sirokov Author-email: roman@flowrl.com
-License: New BSD license Download-URL: https://github.com/r0x0r/pywebview/
-archive/4.0.2.tar.gz Description:
+Metadata-Version: 2.1 Name: pywebview Version: 4.1 Summary: Build GUI for your
+Python program with JavaScript, HTML, and CSS. Home-page: https://github.com/
+r0x0r/pywebview Download-URL: https://github.com/r0x0r/pywebview/archive/
+4.1.tar.gz Author: Roman Sirokov Author-email: roman@flowrl.com License: New
+BSD license Keywords: gui,webkit,html,web Classifier: Intended Audience ::
+Developers Classifier: License :: OSI Approved :: BSD License Classifier:
+Operating System :: OS Independent Classifier: Environment :: MacOS X
+Classifier: Environment :: Win32 (MS Windows) Classifier: Environment :: X11
+Applications :: GTK Classifier: Environment :: X11 Applications :: Qt
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.6 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Topic :: Software
+Development :: Libraries :: Application Frameworks Classifier: Topic ::
+Software Development :: Libraries :: Python Modules Classifier: Topic ::
+Software Development :: User Interfaces Description-Content-Type: text/markdown
+Provides-Extra: cef Provides-Extra: gtk Provides-Extra: pyside2 Provides-Extra:
+pyside6 Provides-Extra: qt License-File: LICENSE.md
                                [pywebview logo]
                   [https://opencollective.com/pywebview/all/
 badge.svg?label=financial+contributors] [PyPI version] [PyPI downloads] [Build
                      status] https://pywebview.flowrl.com
 _pywebview_ is a lightweight cross-platform wrapper around a webview component
 that allows to display HTML content in its own native GUI window. It gives you
 power of web technologies in your desktop application, hiding the fact that GUI
@@ -42,23 +56,8 @@
 opencollective.com/pywebview/organization/2/avatar.svg] [https://
 opencollective.com/pywebview/organization/3/avatar.svg] [https://
 opencollective.com/pywebview/organization/4/avatar.svg] [https://
 opencollective.com/pywebview/organization/5/avatar.svg] [https://
 opencollective.com/pywebview/organization/6/avatar.svg] [https://
 opencollective.com/pywebview/organization/7/avatar.svg] [https://
 opencollective.com/pywebview/organization/8/avatar.svg] [https://
-opencollective.com/pywebview/organization/9/avatar.svg] Keywords:
-gui,webkit,html,web Platform: UNKNOWN Classifier: Intended Audience ::
-Developers Classifier: License :: OSI Approved :: BSD License Classifier:
-Operating System :: OS Independent Classifier: Environment :: MacOS X
-Classifier: Environment :: Win32 (MS Windows) Classifier: Environment :: X11
-Applications :: GTK Classifier: Environment :: X11 Applications :: Qt
-Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Topic :: Software
-Development :: Libraries :: Application Frameworks Classifier: Topic ::
-Software Development :: Libraries :: Python Modules Classifier: Topic ::
-Software Development :: User Interfaces Description-Content-Type: text/markdown
-Provides-Extra: cef Provides-Extra: gtk Provides-Extra: pyside2 Provides-Extra:
-pyside6 Provides-Extra: qt
+opencollective.com/pywebview/organization/9/avatar.svg]
```

### Comparing `pywebview-4.0.2/setup.py` & `pywebview-4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,19 +27,19 @@
     name='pywebview',
     author='Roman Sirokov',
     author_email='roman@flowrl.com',
     description=('Build GUI for your Python program with JavaScript, HTML, and CSS.'),
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/r0x0r/pywebview',
-    download_url='https://github.com/r0x0r/pywebview/archive/4.0.2.tar.gz',
+    download_url='https://github.com/r0x0r/pywebview/archive/4.1.tar.gz',
     keywords=['gui', 'webkit', 'html', 'web'],
     install_requires=install_requires,
     extras_require=extras_require,
-    version='4.0.2',
+    version='4.1',
     include_package_data=True,
     packages=['webview', 'webview.js', 'webview.platforms'],
     package_dir={'webview': 'webview'},
     package_data={
         'webview': [
             'webview/lib/WebBrowserInterop.x64.dll',
             'webview/lib/WebBrowserInterop.x86.dll',
```

### Comparing `pywebview-4.0.2/webview/__init__.py` & `pywebview-4.1/webview/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 (C) 2014-2019 Roman Sirokov and contributors
 Licensed under BSD license
 
 http://github.com/r0x0r/pywebview/
 """
 
 
+import datetime
 import logging
 import os
 import re
+import tempfile
 import threading
 from uuid import uuid4
 from proxy_tools import module_property
 
 import webview.http as http
 
 from webview.guilib import initialize
@@ -67,15 +69,16 @@
 _storage_path = None
 
 token = _token
 windows = []
 menus = []
 
 def start(func=None, args=None, localization={}, gui=None, debug=False, http_server=False,
-          http_port=None, user_agent=None, private_mode=True, storage_path=None, menu=[], server=http.BottleServer, server_args={}):
+          http_port=None, user_agent=None, private_mode=True, storage_path=None, menu=[], 
+          server=http.BottleServer, server_args={}, ssl=False):
     """
     Start a GUI loop and display previously created windows. This function must
     be called from a main thread.
 
     :param func: Function to invoke upon starting the GUI loop.
     :param args: Function arguments. Can be either a single value or a tuple of
         values.
@@ -123,54 +126,70 @@
     if threading.current_thread().name != 'MainThread':
         raise WebViewException('pywebview must be run on a main thread.')
 
     if len(windows) == 0:
         raise WebViewException('You must create a window first before calling this function.')
 
     guilib = initialize(gui)
+    
+    if ssl:
+      # generate SSL certs and tell the windows to use them
+      keyfile, certfile = generate_ssl_cert()
+      server_args['keyfile'] = keyfile
+      server_args['certfile'] = certfile
+    else:
+      keyfile, certfile = None, None
 
     urls = [w.original_url for w in windows]
     has_local_urls = not not [
         w.original_url
         for w in windows
         if is_local_url(w.original_url)
     ]
     # start the global server if it's not running and we need it
     if (http.global_server is None) and \
         (http_server or has_local_urls or (guilib.renderer == 'gtkwebkit2')):
             if not _private_mode and not http_port:
                 http_port = DEFAULT_HTTP_PORT
-            prefix, common_path, server = http.start_global_server(http_port=http_port, urls=urls, server=server, **server_args)
+            prefix, common_path, server = http.start_global_server(http_port=http_port, urls=urls, server=server, ssl=ssl, **server_args)
 
-    for window in windows:
+    for window in windows:            
         window._initialize(guilib)
 
+    if ssl:
+      for window in windows:
+        window.gui.add_tls_cert(certfile)
+
     if len(windows) > 1:
         t = threading.Thread(target=_create_children, args=(windows[1:],))
         t.start()
 
     if func:
         if args is not None:
             if not hasattr(args, '__iter__'):
                 args = (args,)
             t = threading.Thread(target=func, args=args)
         else:
             t = threading.Thread(target=func)
         t.start()
 
-    guilib.set_app_menu(menu)
+    if menu:
+        guilib.set_app_menu(menu)
     guilib.create_window(windows[0])
+    # keyfile is deleted by the ServerAdapter right after wrap_socket()
+    if certfile:
+      os.unlink(certfile)
 
 
 def create_window(title, url=None, html=None, js_api=None, width=800, height=600, x=None, y=None,
                   resizable=True, fullscreen=False, min_size=(200, 100), hidden=False,
                   frameless=False, easy_drag=True,
                   minimized=False, on_top=False, confirm_close=False, background_color='#FFFFFF',
                   transparent=False, text_select=False, zoomable=False, draggable=False, vibrancy=False, localization=None,
-                  server=http.BottleServer, server_args={}):
+                  server=http.BottleServer, http_port=None, server_args={}):
     """
     Create a web view window using a native GUI. The execution blocks after this function is invoked, so other
     program logic must be executed in a separate thread.
     :param title: Window title
     :param url: URL to load
     :param width: window width. Default is 800px
     :param height:window height. Default is 600px
@@ -197,29 +216,81 @@
 
     uid = 'master' if len(windows) == 0 else 'child_' + uuid4().hex[:8]
 
     window = Window(uid, title, url, html,
                     width, height, x, y, resizable, fullscreen, min_size, hidden,
                     frameless, easy_drag, minimized, on_top, confirm_close, background_color,
                     js_api, text_select, transparent, zoomable, draggable, vibrancy, localization,
-                    server=server, server_args=server_args)
+                    server=server, http_port=http_port, server_args=server_args)
 
     windows.append(window)
 
     # This immediately creates the window only if `start` has already been called
     if threading.current_thread().name != 'MainThread' and guilib:
         if is_app(url) or is_local_url(url) and not server.is_running:
             url_prefix, common_path, server = http.start_server([url], server=server, **server_args)
         else:
             url_prefix, common_path, server = None, None, None
 
         window._initialize(gui = guilib, server = server)
         guilib.create_window(window)
 
     return window
+    
+def generate_ssl_cert():
+    # https://cryptography.io/en/latest/x509/tutorial/#creating-a-self-signed-certificate
+    from cryptography.hazmat.primitives.asymmetric import rsa
+    from cryptography.hazmat.primitives import serialization
+    from cryptography import x509
+    from cryptography.x509.oid import NameOID
+    from cryptography.hazmat.primitives import hashes
+    
+    with tempfile.NamedTemporaryFile(prefix='keyfile_', suffix='.pem', delete=False) as f:
+      keyfile = f.name
+      key = rsa.generate_private_key(
+          public_exponent=65537,
+          key_size=2048,
+      )
+      key_pem = key.private_bytes(
+          encoding=serialization.Encoding.PEM,
+          format=serialization.PrivateFormat.TraditionalOpenSSL,
+          encryption_algorithm=serialization.NoEncryption(), #BestAvailableEncryption(b"passphrase"),
+      )
+      f.write(key_pem)
+      
+    
+    with tempfile.NamedTemporaryFile(prefix='certfile_', suffix='.pem', delete=False) as f:
+      certfile = f.name
+      subject = issuer = x509.Name([
+          x509.NameAttribute(NameOID.COUNTRY_NAME, u"US"),
+          x509.NameAttribute(NameOID.STATE_OR_PROVINCE_NAME, u"California"),
+          x509.NameAttribute(NameOID.LOCALITY_NAME, u"San Francisco"),
+          x509.NameAttribute(NameOID.ORGANIZATION_NAME, u"pywebview"),
+          x509.NameAttribute(NameOID.COMMON_NAME, u"127.0.0.1"),
+      ])
+      cert = x509.CertificateBuilder().subject_name(
+          subject
+      ).issuer_name(
+          issuer
+      ).public_key(
+          key.public_key()
+      ).serial_number(
+          x509.random_serial_number()
+      ).not_valid_before(
+          datetime.datetime.utcnow()
+      ).not_valid_after(
+          datetime.datetime.utcnow() + datetime.timedelta(days=365)
+      ).add_extension(
+          x509.SubjectAlternativeName([x509.DNSName(u"localhost")]),
+          critical=False,
+      ).sign(key, hashes.SHA256())
+      cert_pem = cert.public_bytes(serialization.Encoding.PEM)
+      f.write(cert_pem)
+
+    return keyfile, certfile
 
 def active_window():
     """
     Get the active window
 
     :return: window object or None
     """
```

### Comparing `pywebview-4.0.2/webview/event.py` & `pywebview-4.1/webview/event.py`

 * *Files identical despite different names*

### Comparing `pywebview-4.0.2/webview/guilib.py` & `pywebview-4.1/webview/guilib.py`

 * *Files identical despite different names*

### Comparing `pywebview-4.0.2/webview/http.py` & `pywebview-4.1/webview/http.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,26 @@
+import os
 import sys
-import tempfile
 
 
 if sys.platform == 'win32' and ('pythonw.exe' in sys.executable or getattr(sys, 'frozen', False)):
     # bottle.py versions prior to 0.12.23 (the latest on PyPi as of Feb 2023) require stdout and
     # stderr to exist, which is not the case on Windows with pythonw.exe or PyInstaller >= 5.8.0
     if sys.stderr is None:
-        sys.stderr = tempfile.TemporaryFile()
+        sys.stderr = open(os.devnull, 'w')
     if sys.stdout is None:
-        sys.stdout = tempfile.TemporaryFile()
+        sys.stdout = open(os.devnull, 'w')
 
 
 import bottle
 import json
 import logging
-import os
 import threading
 import random
+import ssl
 import socket
 import uuid
 from wsgiref.simple_server import make_server, WSGIRequestHandler, WSGIServer
 from socketserver import ThreadingMixIn
 from .util import abspath, is_app, is_local_url
 
 
@@ -65,15 +65,15 @@
         self.running = False
         self.address = None
         self.js_callback = {}
         self.js_api_endpoint = None
         self.uid = str(uuid.uuid1())
 
     @classmethod
-    def start_server(self, urls, http_port):
+    def start_server(self, urls, http_port, keyfile=None, certfile=None):
         from webview import _debug
 
         apps = [u for u in urls if is_app(u)]
         server = self()
 
         if len(apps) > 0:
             app = apps[0]
@@ -104,32 +104,79 @@
                 bottle.response.set_header('Cache-Control', 'no-cache, no-store, must-revalidate')
                 bottle.response.set_header('Pragma', 'no-cache')
                 bottle.response.set_header('Expires', 0)
                 return bottle.static_file(file, root=server.root_path)
 
         server.root_path = abspath(common_path) if common_path is not None else None
         server.port = http_port or _get_random_port()
-        server.thread = threading.Thread(target=lambda: bottle.run(app=app, server=ThreadedAdapter, port=server.port, quiet=not _debug['mode']), daemon=True)
+        if keyfile and certfile:
+          server_adapter = SSLWSGIRefServer()
+          server_adapter.port = server.port
+          setattr(server_adapter, 'pywebview_keyfile', keyfile)
+          setattr(server_adapter, 'pywebview_certfile', certfile)
+        else:
+         server_adapter = ThreadedAdapter
+        server.thread = threading.Thread(target=lambda: bottle.run(app=app, server=server_adapter, port=server.port, quiet=not _debug['mode']), daemon=True)
         server.thread.start()
 
         server.running = True
-        server.address = f'http://127.0.0.1:{server.port}/'
+        protocol = 'https' if keyfile and certfile else 'http'
+        server.address = f'{protocol}://127.0.0.1:{server.port}/'
         self.common_path = common_path
         server.js_api_endpoint = f'{server.address}js_api/{server.uid}'
 
         return server.address, common_path, server
     
     @property
     def is_running(self):
         return self.running
 
+class SSLWSGIRefServer(bottle.ServerAdapter):
+    def run(self, app):  # pragma: no cover
+        from wsgiref.simple_server import make_server
+        from wsgiref.simple_server import WSGIRequestHandler, WSGIServer
+        import socket
+
+        class FixedHandler(WSGIRequestHandler):
+            def address_string(self):  # Prevent reverse DNS lookups please.
+                return self.client_address[0]
+
+            def log_request(*args, **kw):
+                if not self.quiet:
+                    return WSGIRequestHandler.log_request(*args, **kw)
+
+        handler_cls = self.options.get('handler_class', FixedHandler)
+        server_cls = self.options.get('server_class', WSGIServer)
+
+        if ':' in self.host:  # Fix wsgiref for IPv6 addresses.
+            if getattr(server_cls, 'address_family') == socket.AF_INET:
+
+                class server_cls(server_cls):
+                    address_family = socket.AF_INET6
+
+        self.srv = make_server(self.host, self.port, app, server_cls,
+                               handler_cls)
+        context = ssl.create_default_context()
+        self.srv.socket = ssl.wrap_socket(
+                self.srv.socket,
+                keyfile=self.pywebview_keyfile,
+                certfile=self.pywebview_certfile,
+                server_side=True)
+        self.port = self.srv.server_port  # update port actual port (0 means random)
+        os.unlink(self.pywebview_keyfile)
+        try:
+            self.srv.serve_forever()
+        except KeyboardInterrupt:
+            self.srv.server_close()  # Prevent ResourceWarning: unclosed socket
+            raise
+
 
 def start_server(urls, http_port=None, server=BottleServer, **server_args):
     server = server if not server is None else BottleServer
     return server.start_server(urls, http_port, **server_args)
 
 
-def start_global_server(http_port=None, urls='.', server=BottleServer, **server_args):
+def start_global_server(http_port=None, urls='.', server=BottleServer, ssl=False, **server_args):
     global global_server
     address, common_path, global_server = start_server(urls=urls, http_port=http_port, server=server, **server_args)
     return address, common_path, global_server
```

### Comparing `pywebview-4.0.2/webview/js/api.py` & `pywebview-4.1/webview/js/api.py`

 * *Files identical despite different names*

### Comparing `pywebview-4.0.2/webview/js/css.py` & `pywebview-4.1/webview/js/css.py`

 * *Files identical despite different names*

### Comparing `pywebview-4.0.2/webview/js/dom.py` & `pywebview-4.1/webview/js/dom.py`

 * *Files identical despite different names*

### Comparing `pywebview-4.0.2/webview/js/drag.py` & `pywebview-4.1/webview/js/drag.py`

 * *Files identical despite different names*

### Comparing `pywebview-4.0.2/webview/js/event.py` & `pywebview-4.1/webview/js/event.py`

 * *Files identical despite different names*

### Comparing `pywebview-4.0.2/webview/js/npo.py` & `pywebview-4.1/webview/js/npo.py`

 * *Files identical despite different names*

### Comparing `pywebview-4.0.2/webview/lib/Microsoft.Web.WebView2.Core.dll` & `pywebview-4.1/webview/lib/Microsoft.Web.WebView2.Core.dll`

 * *Files identical despite different names*

### Comparing `pywebview-4.0.2/webview/lib/Microsoft.Web.WebView2.LICENSE.md` & `pywebview-4.1/webview/lib/Microsoft.Web.WebView2.LICENSE.md`

 * *Files identical despite different names*

### Comparing `pywebview-4.0.2/webview/lib/Microsoft.Web.WebView2.WinForms.dll` & `pywebview-4.1/webview/lib/Microsoft.Web.WebView2.WinForms.dll`

 * *Files identical despite different names*

### Comparing `pywebview-4.0.2/webview/lib/WebBrowserInterop.x64.dll` & `pywebview-4.1/webview/lib/WebBrowserInterop.x64.dll`

 * *Files identical despite different names*

### Comparing `pywebview-4.0.2/webview/lib/WebBrowserInterop.x86.dll` & `pywebview-4.1/webview/lib/WebBrowserInterop.x86.dll`

 * *Files identical despite different names*

### Comparing `pywebview-4.0.2/webview/lib/arm64/WebView2Loader.dll` & `pywebview-4.1/webview/lib/arm64/WebView2Loader.dll`

 * *Files identical despite different names*

### Comparing `pywebview-4.0.2/webview/lib/x64/WebView2Loader.dll` & `pywebview-4.1/webview/lib/x64/WebView2Loader.dll`

 * *Files identical despite different names*

### Comparing `pywebview-4.0.2/webview/lib/x86/WebView2Loader.dll` & `pywebview-4.1/webview/lib/x86/WebView2Loader.dll`

 * *Files identical despite different names*

### Comparing `pywebview-4.0.2/webview/localization.py` & `pywebview-4.1/webview/localization.py`

 * *Files identical despite different names*

### Comparing `pywebview-4.0.2/webview/menu.py` & `pywebview-4.1/webview/menu.py`

 * *Files identical despite different names*

### Comparing `pywebview-4.0.2/webview/platforms/cef.py` & `pywebview-4.1/webview/platforms/cef.py`

 * *Files identical despite different names*

### Comparing `pywebview-4.0.2/webview/platforms/cocoa.py` & `pywebview-4.1/webview/platforms/cocoa.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,14 +133,22 @@
             alert.setInformativeText_(message)
             alert.runModal()
 
             if not handler.__block_signature__:
                 handler.__block_signature__ = BrowserView.pyobjc_method_signature(b'v@')
             handler()
 
+        def webView_didReceiveAuthenticationChallenge_completionHandler_(self, webview, challenge, handler):
+            # Prevent `ObjCPointerWarning: PyObjCPointer created: ... type ^{__SecTrust=}`
+            from Security import SecTrustRef
+
+            # this allows any server cert
+            credential = AppKit.NSURLCredential.credentialForTrust_(challenge.protectionSpace().serverTrust())
+            handler(AppKit.NSURLSessionAuthChallengeUseCredential, credential)
+
         # Display a JavaScript confirm panel containing the specified message
         def webView_runJavaScriptConfirmPanelWithMessage_initiatedByFrame_completionHandler_(self, webview, message, frame, handler):
             i = BrowserView.get_instance('webkit', webview)
             ok = i.localization['global.ok']
             cancel = i.localization['global.cancel']
 
             # TODO returning confirmation result does not work currently
@@ -369,23 +377,23 @@
 
         config = self.webkit.configuration()
         config.userContentController().addScriptMessageHandler_name_(self._browserDelegate, 'browserDelegate')
 
         if _private_mode:
             # nonPersisentDataStore preserves cookies for some unknown reason. For this reason we use default datastore
             # and clear all the cookies beforehand
-            datastore = WebKit.WKWebsiteDataStore.defaultDataStore()
+            self.datastore = WebKit.WKWebsiteDataStore.defaultDataStore()
 
             def dummy_completion_handler():
                 pass
 
             data_types = WebKit.WKWebsiteDataStore.allWebsiteDataTypes()
             from_start = WebKit.NSDate.dateWithTimeIntervalSince1970_(0)
-            config.setWebsiteDataStore_(datastore)
-            datastore.removeDataOfTypes_modifiedSince_completionHandler_(data_types, from_start, dummy_completion_handler)
+            config.setWebsiteDataStore_(self.datastore)
+            self.datastore.removeDataOfTypes_modifiedSince_completionHandler_(data_types, from_start, dummy_completion_handler)
         else:
             self.datastore = WebKit.WKWebsiteDataStore.defaultDataStore()
             config.setWebsiteDataStore_(self.datastore)
 
         try:
             config.preferences().setValue_forKey_(False, 'backspaceKeyNavigationEnabled')
         except KeyError:
@@ -420,15 +428,15 @@
             visualEffectView = AppKit.NSVisualEffectView.new()
             visualEffectView.setAutoresizingMask_(AppKit.NSViewWidthSizable|AppKit.NSViewHeightSizable)
             visualEffectView.setWantsLayer_(True)
             visualEffectView.setFrame_(frame_vibrancy)
             visualEffectView.setState_(AppKit.NSVisualEffectStateActive)
             visualEffectView.setBlendingMode_(AppKit.NSVisualEffectBlendingModeBehindWindow)
             self.webkit.addSubview_positioned_relativeTo_(visualEffectView, AppKit.NSWindowBelow,  self.webkit)
-    
+
         self.frameless = window.frameless
         self.easy_drag = window.easy_drag
 
         if window.frameless:
             # Make content full size and titlebar transparent
             self.window.setTitlebarAppearsTransparent_(True)
             self.window.setTitleVisibility_(NSWindowTitleHidden)
@@ -684,30 +692,34 @@
     def _add_app_menu(self):
         """
         Create a default Cocoa menu that shows 'Services', 'Hide',
         'Hide Others', 'Show All', and 'Quit'. Will append the application name
         to some menu items if it's available.
         """
 
-        mainMenu = self.app.mainMenu()
+        mainMenu = BrowserView.app.mainMenu()
+
+        if not mainMenu:
+            mainMenu = AppKit.NSMenu.alloc().init()
+            BrowserView.app.setMainMenu_(mainMenu)
 
         # Create an application menu and make it a submenu of the main menu
         mainAppMenuItem = AppKit.NSMenuItem.alloc().init()
         # The application menu is the first item, so add this menu ast the first item
         mainMenu.insertItem_atIndex_(mainAppMenuItem, 0)
         appMenu = AppKit.NSMenu.alloc().init()
         mainAppMenuItem.setSubmenu_(appMenu)
 
         appMenu.addItemWithTitle_action_keyEquivalent_(self._append_app_name(self.localization["cocoa.menu.about"]), "orderFrontStandardAboutPanel:", "")
 
         appMenu.addItem_(AppKit.NSMenuItem.separatorItem())
 
         # Set the 'Services' menu for the app and create an app menu item
         appServicesMenu = AppKit.NSMenu.alloc().init()
-        self.app.setServicesMenu_(appServicesMenu)
+        BrowserView.app.setServicesMenu_(appServicesMenu)
         servicesMenuItem = appMenu.addItemWithTitle_action_keyEquivalent_(self.localization["cocoa.menu.services"], nil, "")
         servicesMenuItem.setSubmenu_(appServicesMenu)
 
         appMenu.addItem_(AppKit.NSMenuItem.separatorItem())
 
         # Append the 'Hide', 'Hide Others', and 'Show All' menu items
         appMenu.addItemWithTitle_action_keyEquivalent_(self._append_app_name(self.localization["cocoa.menu.hide"]), "hide:", "h")
@@ -720,15 +732,19 @@
         # Append a 'Quit' menu item
         appMenu.addItemWithTitle_action_keyEquivalent_(self._append_app_name(self.localization["cocoa.menu.quit"]), "terminate:", "q")
 
     def _add_view_menu(self):
         """
         Create a default View menu that shows 'Enter Full Screen'.
         """
-        mainMenu = self.app.mainMenu()
+        mainMenu = BrowserView.app.mainMenu()
+
+        if not mainMenu:
+            mainMenu = AppKit.NSMenu.alloc().init()
+            BrowserView.app.setMainMenu_(mainMenu)
 
         # Create an View menu and make it a submenu of the main menu
         viewMenu = AppKit.NSMenu.alloc().init()
         viewMenu.setTitle_(self.localization["cocoa.menu.view"])
         viewMenuItem = AppKit.NSMenuItem.alloc().init()
         viewMenuItem.setSubmenu_(viewMenu)
         # Make the view menu the first item after the application menu
@@ -1098,7 +1114,13 @@
     return dimensions
 
 
 def get_screens():
     screens = [Screen(s.frame().size.width, s.frame().size.height) for s in AppKit.NSScreen.screens()]
     return screens
 
+
+def add_tls_cert(certfile):
+    # does not auth against the certfile
+    # see webView_didReceiveAuthenticationChallenge_completionHandler_
+    pass
+
```

### Comparing `pywebview-4.0.2/webview/platforms/edgechromium.py` & `pywebview-4.1/webview/platforms/edgechromium.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,17 @@
 
 class EdgeChrome:
     def __init__(self, form, window, cache_dir):
         self.pywebview_window = window
         self.web_view = WebView2()
         props = CoreWebView2CreationProperties()
         props.UserDataFolder = cache_dir
+        props.set_IsInPrivateModeEnabled(_private_mode)
         self.web_view.CreationProperties = props
+
         form.Controls.Add(self.web_view)
 
         self.js_results = {}
         self.js_result_semaphore = Semaphore(0)
         self.web_view.Dock = WinForms.DockStyle.Fill
         self.web_view.BringToFront()
         self.web_view.CoreWebView2InitializationCompleted += self.on_webview_ready
```

### Comparing `pywebview-4.0.2/webview/platforms/gtk.py` & `pywebview-4.1/webview/platforms/gtk.py`

 * *Files 2% similar despite different names*

```diff
@@ -564,14 +564,20 @@
 
 def toggle_fullscreen(uid):
     def _toggle_fullscreen():
         BrowserView.instances[uid].toggle_fullscreen()
     glib.idle_add(_toggle_fullscreen)
 
 
+def add_tls_cert(certfile):
+    web_context = webkit.WebContext.get_default()
+    cert = Gio.TlsCertificate.new_from_file(certfile)
+    web_context.allow_tls_certificate_for_host(cert, '127.0.0.1')
+
+
 def set_on_top(uid, top):
     def _set_on_top():
         BrowserView.instances[uid].window.set_keep_above(top)
 
     glib.idle_add(_set_on_top)
```

### Comparing `pywebview-4.0.2/webview/platforms/mshtml.py` & `pywebview-4.1/webview/platforms/mshtml.py`

 * *Files identical despite different names*

### Comparing `pywebview-4.0.2/webview/platforms/qt.py` & `pywebview-4.1/webview/platforms/qt.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,19 +38,21 @@
 from qtpy.QtWidgets import QMainWindow, QApplication, QFileDialog, QMessageBox, QAction, QMenuBar
 from qtpy.QtGui import QColor, QScreen
 from qtpy import PYQT6, PYSIDE6
 
 try:
     from qtpy.QtWebEngineWidgets import QWebEngineView as QWebView, QWebEnginePage as QWebPage, QWebEngineProfile
     from qtpy.QtWebChannel import QWebChannel
+    from qtpy.QtNetwork import QSslConfiguration, QSslCertificate
     renderer = 'qtwebengine'
     is_webengine = True
 except ImportError:
     from PyQt5 import QtWebKitWidgets
     from PyQt5.QtWebKitWidgets import QWebView, QWebPage
+    from PyQt5.QtNetwork import QSslConfiguration, QSslCertificate
     is_webengine = False
     renderer = 'qtwebkit'
 
 _main_window_created = Event()
 _main_window_created.clear()
 
 # suppress invalid style override error message on some Linux distros
@@ -909,7 +911,16 @@
     global _app
     _app = QApplication.instance() or QApplication(sys.argv)
 
     geometries = [s.geometry() for s in _app.screens()]
     screens = [Screen(g.width(), g.height()) for g in geometries]
 
     return screens
+
+def add_tls_cert(certfile):
+    config = QSslConfiguration.defaultConfiguration()
+    certs = config.caCertificates()
+    cert = QSslCertificate.fromPath(certfile)[0]
+    certs.append(cert)
+    config.setCaCertificates(certs)
+    QSslConfiguration.setDefaultConfiguration(config)
+
```

### Comparing `pywebview-4.0.2/webview/platforms/winforms.py` & `pywebview-4.1/webview/platforms/winforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,18 +5,20 @@
 Licensed under BSD license
 http://github.com/r0x0r/pywebview/
 """
 
 import os
 import sys
 import logging
-from threading import Event, Semaphore, Thread
+import threading
+from threading import Event, Semaphore
 import ctypes
 from ctypes import windll
 from platform import machine
+import tempfile
 
 from webview import windows, _private_mode, _storage_path, OPEN_DIALOG, FOLDER_DIALOG, SAVE_DIALOG
 from webview.guilib import forced_gui_
 from webview.util import parse_file_type, inject_base_uri
 from webview.screen import Screen
 from webview.window import FixPoint
 from webview.menu import Menu, MenuAction, MenuSeparator
@@ -114,31 +116,35 @@
     from . import mshtml as IE
     logger.warning('MSHTML is deprecated. See https://pywebview.flowrl.com/guide/renderer.html#web-engine on details how to use Edge Chromium')
     logger.debug('Using WinForms / MSHTML')
     renderer = 'mshtml'
 
 if not _private_mode or _storage_path:
     try:
-        app_data = Environment.GetFolderPath(Environment.SpecialFolder.ApplicationData)
-        cache_dir = _storage_path or os.path.join(app_data, 'pywebview')
+        data_folder = Environment.GetFolderPath(Environment.SpecialFolder.ApplicationData)
+        
+        if not os.access(data_folder, os.W_OK):
+            data_folder = Environment.GetFolderPath(Environment.SpecialFolder.UserProfile)
+            
+        cache_dir = _storage_path or os.path.join(data_folder, 'pywebview')
 
         if not os.path.exists(cache_dir):
             os.makedirs(cache_dir)
     except Exception as e:
         logger.exception(f'Cache directory {cache_dir} creation failed')
 else:
-    cache_dir = None
+    cache_dir = tempfile.TemporaryDirectory().name
 
 class BrowserView:
     instances = {}
 
     app_menu_list = None
 
     class BrowserForm(WinForms.Form):
-        def __init__(self, window):
+        def __init__(self, window, cache_dir):
             super().__init__()
             self.uid = window.uid
             self.pywebview_window = window
             self.real_url = None
             self.Text = window.title
             self.Size = Size(window.initial_width, window.initial_height)
             self.MinimumSize = Size(window.min_size[0], window.min_size[1])
@@ -181,15 +187,15 @@
             if window.fullscreen:
                 self.toggle_fullscreen()
 
             if window.frameless:
                 self.frameless = window.frameless
                 self.FormBorderStyle = getattr(WinForms.FormBorderStyle, 'None')
 
-            if len(BrowserView.app_menu_list):
+            if BrowserView.app_menu_list:
                 self.set_window_menu(BrowserView.app_menu_list)
 
             if is_cef:
                 self.browser = None
                 CEF.create_browser(window, self.Handle.ToInt32(), BrowserView.alert, self)
             elif is_chromium:
                 self.browser = Chromium.EdgeChrome(self, window, cache_dir)
@@ -349,15 +355,15 @@
                     for menu_line_item in line_items:
                         if isinstance(menu_line_item, MenuSeparator):
                             m.DropDownItems.Add(WinForms.ToolStripSeparator())
                             continue
                         elif isinstance(menu_line_item, MenuAction):
                             action_item = WinForms.ToolStripMenuItem(menu_line_item.title)
                             # Don't run action function on main thread
-                            action_item.Click += lambda _,__,menu_line_item=menu_line_item : Thread(target=menu_line_item.function).start()
+                            action_item.Click += lambda _,__,menu_line_item=menu_line_item : threading.Thread(target=menu_line_item.function).start()
                             m.DropDownItems.Add(action_item)
                         elif isinstance(menu_line_item, Menu):
                             create_submenu(menu_line_item.title, menu_line_item.items, m)
 
                     if supermenu:
                         supermenu.DropDownItems.Add(m)
 
@@ -517,15 +523,15 @@
         return
     WinForms.Application.EnableVisualStyles()
     WinForms.Application.SetCompatibleTextRenderingDefault(False)
     _already_set_up_app = True
 
 def create_window(window):
     def create():
-        browser = BrowserView.BrowserForm(window)
+        browser = BrowserView.BrowserForm(window, cache_dir)
         BrowserView.instances[window.uid] = browser
 
         if window.hidden:
             browser.Opacity = 0
             browser.Show()
             browser.Hide()
             browser.Opacity = 1
@@ -568,15 +574,15 @@
     if window.InvokeRequired:
         window.Invoke(Func[Type](_set_title))
     else:
         _set_title()
 
 
 def create_confirmation_dialog(title, message, uid):
-    result = WinForms.MessageBox.Show(title, message, WinForms.MessageBoxButtons.OKCancel)
+    result = WinForms.MessageBox.Show(message, title, WinForms.MessageBoxButtons.OKCancel)
     return result == WinForms.DialogResult.OK
 
 
 def create_file_dialog(dialog_type, directory, allow_multiple, save_filename, file_types, uid):
     window = BrowserView.instances[uid]
 
     if not directory:
@@ -763,7 +769,11 @@
     size = BrowserView.instances[uid].Size
     return size.Width, size.Height
 
 
 def get_screens():
     screens = [Screen(s.Bounds.Width, s.Bounds.Height) for s in WinForms.Screen.AllScreens]
     return screens
+
+def add_tls_cert(certfile):
+    raise NotImplementedError
+
```

### Comparing `pywebview-4.0.2/webview/util.py` & `pywebview-4.1/webview/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,14 +175,15 @@
 def js_bridge_call(window, func_name, param, value_id):
     def _call():
         try:
             result = func(*func_params.values())
             result = json.dumps(result).replace('\\', '\\\\').replace('\'', '\\\'')
             code = 'window.pywebview._returnValues["{0}"]["{1}"] = {{value: \'{2}\'}}'.format(func_name, value_id, result)
         except Exception as e:
+            print(traceback.format_exc())
             error = {
                 'message': str(e),
                 'name': type(e).__name__,
                 'stack': traceback.format_exc()
             }
             result = json.dumps(error).replace('\\', '\\\\').replace('\'', '\\\'')
             code = 'window.pywebview._returnValues["{0}"]["{1}"] = {{isError: true, value: \'{2}\'}}'.format(func_name, value_id, result)
```

### Comparing `pywebview-4.0.2/webview/window.py` & `pywebview-4.1/webview/window.py`

 * *Files identical despite different names*

