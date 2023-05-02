# Comparing `tmp/ixbrl_viewer-0.0.0.dev1683038679426.tar.gz` & `tmp/ixbrl_viewer-0.0.0.dev1683038682633.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ixbrl_viewer-0.0.0.dev1683038679426.tar", last modified: Tue May  2 14:44:44 2023, max compression
+gzip compressed data, was "ixbrl_viewer-0.0.0.dev1683038682633.tar", last modified: Tue May  2 14:44:47 2023, max compression
```

## Comparing `ixbrl_viewer-0.0.0.dev1683038679426.tar` & `ixbrl_viewer-0.0.0.dev1683038682633.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:44:44.695225 ixbrl_viewer-0.0.0.dev1683038679426/
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-02 14:44:44.695225 ixbrl_viewer-0.0.0.dev1683038679426/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:44:44.695225 ixbrl_viewer-0.0.0.dev1683038679426/ixbrl_viewer.egg-info/
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-02 14:44:44.000000 ixbrl_viewer-0.0.0.dev1683038679426/ixbrl_viewer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      162 2023-05-02 14:44:44.000000 ixbrl_viewer-0.0.0.dev1683038679426/ixbrl_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 14:44:44.000000 ixbrl_viewer-0.0.0.dev1683038679426/ixbrl_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-02 14:44:44.000000 ixbrl_viewer-0.0.0.dev1683038679426/ixbrl_viewer.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 14:44:39.000000 ixbrl_viewer-0.0.0.dev1683038679426/module.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-02 14:44:44.695225 ixbrl_viewer-0.0.0.dev1683038679426/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      132 2023-05-02 14:44:39.000000 ixbrl_viewer-0.0.0.dev1683038679426/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:44:47.937474 ixbrl_viewer-0.0.0.dev1683038682633/
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-02 14:44:47.933474 ixbrl_viewer-0.0.0.dev1683038682633/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 14:44:47.933474 ixbrl_viewer-0.0.0.dev1683038682633/ixbrl_viewer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-02 14:44:47.000000 ixbrl_viewer-0.0.0.dev1683038682633/ixbrl_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      162 2023-05-02 14:44:47.000000 ixbrl_viewer-0.0.0.dev1683038682633/ixbrl_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 14:44:47.000000 ixbrl_viewer-0.0.0.dev1683038682633/ixbrl_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-02 14:44:47.000000 ixbrl_viewer-0.0.0.dev1683038682633/ixbrl_viewer.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 14:44:42.000000 ixbrl_viewer-0.0.0.dev1683038682633/module.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-02 14:44:47.937474 ixbrl_viewer-0.0.0.dev1683038682633/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      132 2023-05-02 14:44:42.000000 ixbrl_viewer-0.0.0.dev1683038682633/setup.py
```

