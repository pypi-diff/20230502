# Comparing `tmp/catnapmodule-1.2.tar.gz` & `tmp/catnapmodule-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catnapmodule-1.2.tar", last modified: Mon May  1 10:42:51 2023, max compression
+gzip compressed data, was "catnapmodule-1.3.tar", last modified: Tue May  2 13:49:39 2023, max compression
```

## Comparing `catnapmodule-1.2.tar` & `catnapmodule-1.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 10:42:51.411156 catnapmodule-1.2/
--rw-rw-rw-   0        0        0      921 2023-05-01 10:42:51.412155 catnapmodule-1.2/PKG-INFO
--rw-rw-rw-   0        0        0      727 2023-05-01 10:42:40.000000 catnapmodule-1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 10:42:51.395144 catnapmodule-1.2/catnapmodule/
--rw-rw-rw-   0        0        0        0 2023-04-29 14:29:06.000000 catnapmodule-1.2/catnapmodule/__init__.py
--rw-rw-rw-   0        0        0      123 2023-04-29 13:26:24.000000 catnapmodule-1.2/catnapmodule/chat.py
--rw-rw-rw-   0        0        0      306 2023-05-01 10:40:51.000000 catnapmodule-1.2/catnapmodule/queq.py
-drwxrwxrwx   0        0        0        0 2023-05-01 10:42:51.409153 catnapmodule-1.2/catnapmodule.egg-info/
--rw-rw-rw-   0        0        0      921 2023-05-01 10:42:51.000000 catnapmodule-1.2/catnapmodule.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2023-05-01 10:42:51.000000 catnapmodule-1.2/catnapmodule.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 10:42:51.000000 catnapmodule-1.2/catnapmodule.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-01 10:42:51.000000 catnapmodule-1.2/catnapmodule.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 10:42:51.415158 catnapmodule-1.2/setup.cfg
--rw-rw-rw-   0        0        0      287 2023-05-01 10:40:51.000000 catnapmodule-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:49:39.684605 catnapmodule-1.3/
+-rw-rw-rw-   0        0        0      357 2023-05-02 13:49:39.685606 catnapmodule-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2023-05-02 13:49:37.000000 catnapmodule-1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 13:49:39.657706 catnapmodule-1.3/catnapmodule/
+-rw-rw-rw-   0        0        0        0 2023-04-29 14:29:06.000000 catnapmodule-1.3/catnapmodule/__init__.py
+-rw-rw-rw-   0        0        0      123 2023-04-29 13:26:24.000000 catnapmodule-1.3/catnapmodule/chat.py
+-rw-rw-rw-   0        0        0       65 2023-05-02 13:02:38.000000 catnapmodule-1.3/catnapmodule/lists.py
+-rw-rw-rw-   0        0        0      306 2023-05-01 10:40:51.000000 catnapmodule-1.3/catnapmodule/queq.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:49:39.682603 catnapmodule-1.3/catnapmodule.egg-info/
+-rw-rw-rw-   0        0        0      357 2023-05-02 13:49:39.000000 catnapmodule-1.3/catnapmodule.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-05-02 13:49:39.000000 catnapmodule-1.3/catnapmodule.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 13:49:39.000000 catnapmodule-1.3/catnapmodule.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-02 13:49:39.000000 catnapmodule-1.3/catnapmodule.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 13:49:39.688607 catnapmodule-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      287 2023-05-02 12:55:32.000000 catnapmodule-1.3/setup.py
```

