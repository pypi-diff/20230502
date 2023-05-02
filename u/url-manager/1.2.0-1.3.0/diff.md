# Comparing `tmp/url-manager-1.2.0.tar.gz` & `tmp/url_manager-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "url-manager-1.2.0.tar", max compression
+gzip compressed data, was "url_manager-1.3.0.tar", max compression
```

## Comparing `url-manager-1.2.0.tar` & `url_manager-1.3.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0      350 2022-09-23 14:44:38.000000 url-manager-1.2.0/pyproject.toml
--rw-r--r--   0        0        0       22 2022-09-23 14:44:38.000000 url-manager-1.2.0/url_manager/__init__.py
--rw-r--r--   0        0        0      113 2022-09-23 14:44:38.000000 url-manager-1.2.0/url_manager/enum.py
--rw-r--r--   0        0        0      187 2022-09-23 14:44:38.000000 url-manager-1.2.0/url_manager/helper.py
--rw-r--r--   0        0        0      927 2022-09-23 14:44:38.000000 url-manager-1.2.0/url_manager/main.py
--rw-r--r--   0        0        0     1348 2022-09-23 14:44:38.000000 url-manager-1.2.0/url_manager/social_media.py
--rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 url-manager-1.2.0/setup.py
--rw-r--r--   0        0        0      237 1970-01-01 00:00:00.000000 url-manager-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      350 2023-05-02 14:07:45.000000 url_manager-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-02 14:07:45.000000 url_manager-1.3.0/url_manager/__init__.py
+-rw-r--r--   0        0        0      113 2023-05-02 14:07:45.000000 url_manager-1.3.0/url_manager/enum.py
+-rw-r--r--   0        0        0      187 2023-05-02 14:07:45.000000 url_manager-1.3.0/url_manager/helper.py
+-rw-r--r--   0        0        0      927 2023-05-02 14:07:45.000000 url_manager-1.3.0/url_manager/main.py
+-rw-r--r--   0        0        0     1348 2023-05-02 14:07:45.000000 url_manager-1.3.0/url_manager/social_media.py
+-rw-r--r--   0        0        0      296 1970-01-01 00:00:00.000000 url_manager-1.3.0/PKG-INFO
```

### Comparing `url-manager-1.2.0/url_manager/main.py` & `url_manager-1.3.0/url_manager/main.py`

 * *Files identical despite different names*

### Comparing `url-manager-1.2.0/url_manager/social_media.py` & `url_manager-1.3.0/url_manager/social_media.py`

 * *Files identical despite different names*

