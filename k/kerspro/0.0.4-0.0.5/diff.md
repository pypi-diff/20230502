# Comparing `tmp/kerspro-0.0.4.tar.gz` & `tmp/kerspro-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kerspro-0.0.4.tar", last modified: Tue May  2 14:49:00 2023, max compression
+gzip compressed data, was "kerspro-0.0.5.tar", last modified: Tue May  2 14:53:06 2023, max compression
```

## Comparing `kerspro-0.0.4.tar` & `kerspro-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 14:49:00.545977 kerspro-0.0.4/
--rw-rw-rw-   0        0        0      265 2023-05-02 14:49:00.544979 kerspro-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-02 14:49:00.538977 kerspro-0.0.4/kerspro/
--rw-rw-rw-   0        0        0       12 2023-05-02 14:48:34.000000 kerspro-0.0.4/kerspro/__init__.py
--rw-rw-rw-   0        0        0    13124 2023-05-02 11:58:35.000000 kerspro-0.0.4/kerspro/aipkg.py
-drwxrwxrwx   0        0        0        0 2023-05-02 14:49:00.543977 kerspro-0.0.4/kerspro.egg-info/
--rw-rw-rw-   0        0        0      265 2023-05-02 14:49:00.000000 kerspro-0.0.4/kerspro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      169 2023-05-02 14:49:00.000000 kerspro-0.0.4/kerspro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 14:49:00.000000 kerspro-0.0.4/kerspro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-02 14:49:00.000000 kerspro-0.0.4/kerspro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 14:49:00.545977 kerspro-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      449 2023-05-02 14:48:40.000000 kerspro-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 14:53:06.233472 kerspro-0.0.5/
+-rw-rw-rw-   0        0        0      265 2023-05-02 14:53:06.233472 kerspro-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-02 14:53:06.222457 kerspro-0.0.5/kerspro/
+-rw-rw-rw-   0        0        0    13124 2023-05-02 14:51:51.000000 kerspro-0.0.5/kerspro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 14:53:06.232454 kerspro-0.0.5/kerspro.egg-info/
+-rw-rw-rw-   0        0        0      265 2023-05-02 14:53:06.000000 kerspro-0.0.5/kerspro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      152 2023-05-02 14:53:06.000000 kerspro-0.0.5/kerspro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 14:53:06.000000 kerspro-0.0.5/kerspro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-02 14:53:06.000000 kerspro-0.0.5/kerspro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 14:53:06.235474 kerspro-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      449 2023-05-02 14:52:54.000000 kerspro-0.0.5/setup.py
```

### Comparing `kerspro-0.0.4/kerspro/aipkg.py` & `kerspro-0.0.5/kerspro/__init__.py`

 * *Files identical despite different names*

