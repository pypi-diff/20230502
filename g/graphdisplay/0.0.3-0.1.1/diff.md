# Comparing `tmp/graphdisplay-0.0.3.tar.gz` & `tmp/graphdisplay-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphdisplay-0.0.3.tar", last modified: Mon Apr 24 14:45:37 2023, max compression
+gzip compressed data, was "graphdisplay-0.1.1.tar", last modified: Tue May  2 19:43:57 2023, max compression
```

## Comparing `graphdisplay-0.0.3.tar` & `graphdisplay-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-04-24 14:45:37.618187 graphdisplay-0.0.3/
--rw-rw-r--   0 beto      (1000) beto      (1000)      420 2023-04-24 14:45:37.618187 graphdisplay-0.0.3/PKG-INFO
--rw-rw-r--   0 beto      (1000) beto      (1000)      124 2023-04-24 14:33:17.000000 graphdisplay-0.0.3/README.md
-drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-04-24 14:45:37.614187 graphdisplay-0.0.3/graphdisplay/
--rw-rw-r--   0 beto      (1000) beto      (1000)       34 2023-04-24 14:33:17.000000 graphdisplay-0.0.3/graphdisplay/__init__.py
--rw-rw-r--   0 beto      (1000) beto      (1000)     8277 2023-04-24 14:33:17.000000 graphdisplay-0.0.3/graphdisplay/graphdisplay.py
-drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-04-24 14:45:37.614187 graphdisplay-0.0.3/graphdisplay.egg-info/
--rw-rw-r--   0 beto      (1000) beto      (1000)      420 2023-04-24 14:45:37.000000 graphdisplay-0.0.3/graphdisplay.egg-info/PKG-INFO
--rw-rw-r--   0 beto      (1000) beto      (1000)      251 2023-04-24 14:45:37.000000 graphdisplay-0.0.3/graphdisplay.egg-info/SOURCES.txt
--rw-rw-r--   0 beto      (1000) beto      (1000)        1 2023-04-24 14:45:37.000000 graphdisplay-0.0.3/graphdisplay.egg-info/dependency_links.txt
--rw-rw-r--   0 beto      (1000) beto      (1000)        3 2023-04-24 14:45:37.000000 graphdisplay-0.0.3/graphdisplay.egg-info/requires.txt
--rw-rw-r--   0 beto      (1000) beto      (1000)       13 2023-04-24 14:45:37.000000 graphdisplay-0.0.3/graphdisplay.egg-info/top_level.txt
--rw-rw-r--   0 beto      (1000) beto      (1000)       38 2023-04-24 14:45:37.618187 graphdisplay-0.0.3/setup.cfg
--rw-rw-r--   0 beto      (1000) beto      (1000)     1316 2023-04-24 14:43:01.000000 graphdisplay-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:43:57.591688 graphdisplay-0.1.1/
+-rw-rw-rw-   0        0        0     1051 2023-05-02 19:43:57.590688 graphdisplay-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2023-05-02 18:43:09.000000 graphdisplay-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 19:43:57.582722 graphdisplay-0.1.1/graphdisplay/
+-rw-rw-rw-   0        0        0       34 2023-04-24 21:08:03.000000 graphdisplay-0.1.1/graphdisplay/__init__.py
+-rw-rw-rw-   0        0        0     4920 2023-05-02 18:37:35.000000 graphdisplay-0.1.1/graphdisplay/graph.py
+-rw-rw-rw-   0        0        0     9863 2023-05-02 18:40:09.000000 graphdisplay-0.1.1/graphdisplay/graphdisplay.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:43:57.589691 graphdisplay-0.1.1/graphdisplay.egg-info/
+-rw-rw-rw-   0        0        0     1051 2023-05-02 19:43:57.000000 graphdisplay-0.1.1/graphdisplay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-05-02 19:43:57.000000 graphdisplay-0.1.1/graphdisplay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 19:43:57.000000 graphdisplay-0.1.1/graphdisplay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-02 19:43:57.000000 graphdisplay-0.1.1/graphdisplay.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 19:43:57.591688 graphdisplay-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1842 2023-05-02 19:42:24.000000 graphdisplay-0.1.1/setup.py
```

