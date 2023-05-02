# Comparing `tmp/robotControl-1.0.1.tar.gz` & `tmp/robotControl-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotControl-1.0.1.tar", last modified: Tue May  2 10:24:47 2023, max compression
+gzip compressed data, was "robotControl-1.0.2.tar", last modified: Tue May  2 10:44:09 2023, max compression
```

## Comparing `robotControl-1.0.1.tar` & `robotControl-1.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 10:24:47.488873 robotControl-1.0.1/
--rw-rw-rw-   0        0        0      115 2023-05-02 10:24:47.488873 robotControl-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-02 10:24:47.483364 robotControl-1.0.1/robotControl.egg-info/
--rw-rw-rw-   0        0        0      115 2023-05-02 10:24:47.000000 robotControl-1.0.1/robotControl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      152 2023-05-02 10:24:47.000000 robotControl-1.0.1/robotControl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 10:24:47.000000 robotControl-1.0.1/robotControl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-02 10:24:47.000000 robotControl-1.0.1/robotControl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 10:24:47.489962 robotControl-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      321 2023-05-02 10:24:40.000000 robotControl-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 10:44:09.468526 robotControl-1.0.2/
+-rw-rw-rw-   0        0        0      110 2023-05-02 10:44:09.460502 robotControl-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-02 10:44:09.460502 robotControl-1.0.2/robotControl.egg-info/
+-rw-rw-rw-   0        0        0      110 2023-05-02 10:44:09.000000 robotControl-1.0.2/robotControl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      152 2023-05-02 10:44:09.000000 robotControl-1.0.2/robotControl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 10:44:09.000000 robotControl-1.0.2/robotControl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-02 10:44:09.000000 robotControl-1.0.2/robotControl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 10:44:09.468526 robotControl-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      413 2023-05-02 10:43:03.000000 robotControl-1.0.2/setup.py
```

