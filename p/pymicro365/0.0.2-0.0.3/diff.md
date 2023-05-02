# Comparing `tmp/pymicro365-0.0.2.tar.gz` & `tmp/pymicro365-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymicro365-0.0.2.tar", last modified: Tue May  2 15:20:02 2023, max compression
+gzip compressed data, was "pymicro365-0.0.3.tar", last modified: Tue May  2 18:06:35 2023, max compression
```

## Comparing `pymicro365-0.0.2.tar` & `pymicro365-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 15:20:02.359331 pymicro365-0.0.2/
--rw-rw-rw-   0        0        0      277 2023-05-02 15:20:02.359331 pymicro365-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-02 15:20:02.340381 pymicro365-0.0.2/pymicro365/
--rw-rw-rw-   0        0        0      232 2023-05-02 14:17:34.000000 pymicro365-0.0.2/pymicro365/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 15:20:02.356344 pymicro365-0.0.2/pymicro365.egg-info/
--rw-rw-rw-   0        0        0      277 2023-05-02 15:20:02.000000 pymicro365-0.0.2/pymicro365.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2023-05-02 15:20:02.000000 pymicro365-0.0.2/pymicro365.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 15:20:02.000000 pymicro365-0.0.2/pymicro365.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-05-02 15:20:02.000000 pymicro365-0.0.2/pymicro365.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-02 15:20:02.000000 pymicro365-0.0.2/pymicro365.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 15:20:02.359331 pymicro365-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      478 2023-05-02 15:19:22.000000 pymicro365-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:06:35.858571 pymicro365-0.0.3/
+-rw-rw-rw-   0        0        0      277 2023-05-02 18:06:35.858571 pymicro365-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-02 18:06:35.844609 pymicro365-0.0.3/pymicro365/
+-rw-rw-rw-   0        0        0      210 2023-05-02 16:18:05.000000 pymicro365-0.0.3/pymicro365/__init__.py
+-rw-rw-rw-   0        0        0     2681 2023-05-02 18:00:01.000000 pymicro365-0.0.3/pymicro365/pyicalc.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:06:35.856576 pymicro365-0.0.3/pymicro365.egg-info/
+-rw-rw-rw-   0        0        0      277 2023-05-02 18:06:35.000000 pymicro365-0.0.3/pymicro365.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-05-02 18:06:35.000000 pymicro365-0.0.3/pymicro365.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 18:06:35.000000 pymicro365-0.0.3/pymicro365.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-05-02 18:06:35.000000 pymicro365-0.0.3/pymicro365.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-02 18:06:35.000000 pymicro365-0.0.3/pymicro365.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 18:06:35.858571 pymicro365-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      429 2023-05-02 18:06:26.000000 pymicro365-0.0.3/setup.py
```

