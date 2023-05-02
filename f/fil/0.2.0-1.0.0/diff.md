# Comparing `tmp/fil-0.2.0.tar.gz` & `tmp/fil-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fil-0.2.0.tar", max compression
+gzip compressed data, was "fil-1.0.0.tar", max compression
```

## Comparing `fil-0.2.0.tar` & `fil-1.0.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       52 2023-04-29 09:10:46.794486 fil-0.2.0/README.md
--rw-r--r--   0        0        0     2780 2023-04-29 14:16:41.559561 fil-0.2.0/fil.py
--rw-r--r--   0        0        0      504 2023-04-29 14:20:56.915796 fil-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      605 1970-01-01 00:00:00.000000 fil-0.2.0/setup.py
--rw-r--r--   0        0        0      674 1970-01-01 00:00:00.000000 fil-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      782 2023-05-02 15:39:14.592872 fil-1.0.0/README.md
+-rw-r--r--   0        0        0     5353 2023-05-02 15:34:01.648332 fil-1.0.0/fil.py
+-rw-r--r--   0        0        0      496 2023-05-02 15:39:39.873581 fil-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1354 1970-01-01 00:00:00.000000 fil-1.0.0/setup.py
+-rw-r--r--   0        0        0     1351 1970-01-01 00:00:00.000000 fil-1.0.0/PKG-INFO
```

