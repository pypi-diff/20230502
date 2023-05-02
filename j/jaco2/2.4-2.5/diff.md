# Comparing `tmp/jaco2-2.4.tar.gz` & `tmp/jaco2-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaco2-2.4.tar", last modified: Tue May  2 16:58:44 2023, max compression
+gzip compressed data, was "jaco2-2.5.tar", last modified: Tue May  2 17:13:59 2023, max compression
```

## Comparing `jaco2-2.4.tar` & `jaco2-2.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 16:58:44.150691 jaco2-2.4/
--rw-rw-rw-   0        0        0      136 2023-05-02 16:58:44.142694 jaco2-2.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-02 16:58:44.142694 jaco2-2.4/jaco2.egg-info/
--rw-rw-rw-   0        0        0      136 2023-05-02 16:58:44.000000 jaco2-2.4/jaco2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      147 2023-05-02 16:58:44.000000 jaco2-2.4/jaco2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 16:58:44.000000 jaco2-2.4/jaco2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-02 16:58:44.000000 jaco2-2.4/jaco2.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-02 16:58:44.142694 jaco2-2.4/robotControl/
--rw-rw-rw-   0        0        0    12847 2023-05-02 16:17:13.000000 jaco2-2.4/robotControl/jaco2.cpp
--rw-rw-rw-   0        0        0       42 2023-05-02 16:58:44.150691 jaco2-2.4/setup.cfg
--rw-rw-rw-   0        0        0      625 2023-05-02 16:58:38.000000 jaco2-2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:13:59.672814 jaco2-2.5/
+-rw-rw-rw-   0        0        0      136 2023-05-02 17:13:59.671147 jaco2-2.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-02 17:13:59.666959 jaco2-2.5/jaco2.egg-info/
+-rw-rw-rw-   0        0        0      136 2023-05-02 17:13:59.000000 jaco2-2.5/jaco2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      147 2023-05-02 17:13:59.000000 jaco2-2.5/jaco2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 17:13:59.000000 jaco2-2.5/jaco2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-02 17:13:59.000000 jaco2-2.5/jaco2.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 17:13:59.666959 jaco2-2.5/robotControl/
+-rw-rw-rw-   0        0        0    12847 2023-05-02 16:17:13.000000 jaco2-2.5/robotControl/jaco2.cpp
+-rw-rw-rw-   0        0        0       42 2023-05-02 17:13:59.672814 jaco2-2.5/setup.cfg
+-rw-rw-rw-   0        0        0      836 2023-05-02 17:13:37.000000 jaco2-2.5/setup.py
```

### Comparing `jaco2-2.4/robotControl/jaco2.cpp` & `jaco2-2.5/robotControl/jaco2.cpp`

 * *Files identical despite different names*

