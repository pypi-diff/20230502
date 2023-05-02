# Comparing `tmp/jaco2-3.0.tar.gz` & `tmp/jaco2-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaco2-3.0.tar", last modified: Tue May  2 18:23:31 2023, max compression
+gzip compressed data, was "jaco2-3.1.tar", last modified: Tue May  2 18:32:27 2023, max compression
```

## Comparing `jaco2-3.0.tar` & `jaco2-3.1.tar`

### file list

```diff
@@ -1,11 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 18:23:31.269939 jaco2-3.0/
--rw-rw-rw-   0        0        0      136 2023-05-02 18:23:31.261974 jaco2-3.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-02 18:23:31.245926 jaco2-3.0/jaco2.egg-info/
--rw-rw-rw-   0        0        0      136 2023-05-02 18:23:31.000000 jaco2-3.0/jaco2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      138 2023-05-02 18:23:31.000000 jaco2-3.0/jaco2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 18:23:31.000000 jaco2-3.0/jaco2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-02 18:23:31.000000 jaco2-3.0/jaco2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 18:23:31.269939 jaco2-3.0/setup.cfg
--rw-rw-rw-   0        0        0      703 2023-05-02 18:23:16.000000 jaco2-3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 18:23:31.261974 jaco2-3.0/src/
--rw-rw-rw-   0        0        0    12861 2023-05-02 18:23:10.000000 jaco2-3.0/src/jaco2.cpp
+drwxrwxrwx   0        0        0        0 2023-05-02 18:32:27.290121 jaco2-3.1/
+-rw-rw-rw-   0        0        0      136 2023-05-02 18:32:27.289535 jaco2-3.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-02 18:32:27.267240 jaco2-3.1/jaco2.egg-info/
+-rw-rw-rw-   0        0        0      136 2023-05-02 18:32:27.000000 jaco2-3.1/jaco2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-05-02 18:32:27.000000 jaco2-3.1/jaco2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 18:32:27.000000 jaco2-3.1/jaco2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-02 18:32:27.000000 jaco2-3.1/jaco2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 18:32:27.290989 jaco2-3.1/setup.cfg
+-rw-rw-rw-   0        0        0      662 2023-05-02 18:32:14.000000 jaco2-3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 18:32:27.286526 jaco2-3.1/src/
+-rw-rw-rw-   0        0        0   852480 2023-05-02 18:07:32.000000 jaco2-3.1/src/CommandLayerEthernet.dll
+-rw-rw-rw-   0        0        0   964096 2023-05-02 18:07:32.000000 jaco2-3.1/src/CommandLayerWindows.dll
+-rw-rw-rw-   0        0        0    18432 2023-05-02 18:07:32.000000 jaco2-3.1/src/CommunicationLayerEthernet.dll
+-rw-rw-rw-   0        0        0    18432 2023-05-02 18:07:32.000000 jaco2-3.1/src/CommunicationLayerWindows.dll
+-rw-rw-rw-   0        0        0    12861 2023-05-02 18:23:10.000000 jaco2-3.1/src/jaco2.cpp
```

### Comparing `jaco2-3.0/src/jaco2.cpp` & `jaco2-3.1/src/jaco2.cpp`

 * *Files identical despite different names*

