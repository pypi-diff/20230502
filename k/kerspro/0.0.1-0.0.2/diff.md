# Comparing `tmp/kerspro-0.0.1.tar.gz` & `tmp/kerspro-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kerspro-0.0.1.tar", last modified: Tue May  2 12:07:51 2023, max compression
+gzip compressed data, was "kerspro-0.0.2.tar", last modified: Tue May  2 12:11:56 2023, max compression
```

## Comparing `kerspro-0.0.1.tar` & `kerspro-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 12:07:51.723412 kerspro-0.0.1/
--rw-rw-rw-   0        0        0      575 2023-05-02 12:07:51.722406 kerspro-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-02 12:07:51.720405 kerspro-0.0.1/kerspro.egg-info/
--rw-rw-rw-   0        0        0      575 2023-05-02 12:07:51.000000 kerspro-0.0.1/kerspro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      132 2023-05-02 12:07:51.000000 kerspro-0.0.1/kerspro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 12:07:51.000000 kerspro-0.0.1/kerspro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 12:07:51.000000 kerspro-0.0.1/kerspro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 12:07:51.724511 kerspro-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      779 2023-05-02 12:07:37.000000 kerspro-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:11:56.312050 kerspro-0.0.2/
+-rw-rw-rw-   0        0        0      265 2023-05-02 12:11:56.311063 kerspro-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-02 12:11:56.289826 kerspro-0.0.2/kerspro/
+-rw-rw-rw-   0        0        0       24 2023-05-02 12:11:27.000000 kerspro-0.0.2/kerspro/__init__.py
+-rw-rw-rw-   0        0        0    13124 2023-05-02 11:58:35.000000 kerspro-0.0.2/kerspro/aipkg.py
+drwxrwxrwx   0        0        0        0 2023-05-02 12:11:56.310136 kerspro-0.0.2/kerspro.egg-info/
+-rw-rw-rw-   0        0        0      265 2023-05-02 12:11:55.000000 kerspro-0.0.2/kerspro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      169 2023-05-02 12:11:56.000000 kerspro-0.0.2/kerspro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 12:11:55.000000 kerspro-0.0.2/kerspro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-02 12:11:55.000000 kerspro-0.0.2/kerspro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 12:11:56.314483 kerspro-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      449 2023-05-02 12:11:49.000000 kerspro-0.0.2/setup.py
```

