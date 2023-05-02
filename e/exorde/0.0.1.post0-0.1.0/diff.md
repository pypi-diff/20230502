# Comparing `tmp/exorde-0.0.1.post0.tar.gz` & `tmp/exorde-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exorde-0.0.1.post0.tar", last modified: Mon Mar 20 14:43:25 2023, max compression
+gzip compressed data, was "exorde-0.1.0.tar", last modified: Tue May  2 08:20:22 2023, max compression
```

## Comparing `exorde-0.0.1.post0.tar` & `exorde-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,36 @@
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-03-20 14:43:25.035239 exorde-0.0.1.post0/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       69 2023-03-20 14:43:25.035239 exorde-0.0.1.post0/PKG-INFO
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-03-20 14:43:25.035239 exorde-0.0.1.post0/exorde/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        1 2023-03-20 13:41:04.000000 exorde-0.0.1.post0/exorde/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       84 2023-03-20 14:35:33.000000 exorde-0.0.1.post0/exorde/command.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-03-20 14:43:25.035239 exorde-0.0.1.post0/exorde.egg-info/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       69 2023-03-20 14:43:25.000000 exorde-0.0.1.post0/exorde.egg-info/PKG-INFO
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      198 2023-03-20 14:43:25.000000 exorde-0.0.1.post0/exorde.egg-info/SOURCES.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        1 2023-03-20 14:43:25.000000 exorde-0.0.1.post0/exorde.egg-info/dependency_links.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       46 2023-03-20 14:43:25.000000 exorde-0.0.1.post0/exorde.egg-info/entry_points.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        7 2023-03-20 14:43:25.000000 exorde-0.0.1.post0/exorde.egg-info/top_level.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       38 2023-03-20 14:43:25.035239 exorde-0.0.1.post0/setup.cfg
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      295 2023-03-20 14:35:27.000000 exorde-0.0.1.post0/setup.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-02 08:20:22.845802 exorde-0.1.0/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      359 2023-05-02 08:20:22.845802 exorde-0.1.0/PKG-INFO
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      235 2023-05-02 07:53:14.000000 exorde-0.1.0/README.md
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-02 08:20:22.845802 exorde-0.1.0/exorde/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       63 2023-05-02 07:53:14.000000 exorde-0.1.0/exorde/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4598 2023-05-02 07:53:14.000000 exorde-0.1.0/exorde/bindings.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      150 2023-05-02 07:53:14.000000 exorde-0.1.0/exorde/formated.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-02 08:20:22.845802 exorde-0.1.0/exorde/ipfs/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2967 2023-05-02 07:53:14.000000 exorde-0.1.0/exorde/ipfs/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      873 2023-05-02 07:53:14.000000 exorde-0.1.0/exorde/ipfs/bindings.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      158 2023-03-28 06:45:46.000000 exorde-0.1.0/exorde/ipfs/setup.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-02 08:20:22.845802 exorde-0.1.0/exorde/playwright/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4276 2023-05-02 07:53:14.000000 exorde-0.1.0/exorde/playwright/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      711 2023-05-02 07:53:14.000000 exorde-0.1.0/exorde/playwright/bindings.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      212 2023-05-02 07:53:14.000000 exorde-0.1.0/exorde/playwright/setup.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-02 08:20:22.845802 exorde-0.1.0/exorde/protocol/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    15415 2023-05-02 07:53:14.000000 exorde-0.1.0/exorde/protocol/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1671 2023-05-02 07:53:14.000000 exorde-0.1.0/exorde/protocol/bindings.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      203 2023-03-28 06:45:46.000000 exorde-0.1.0/exorde/protocol/setup.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-02 08:20:22.845802 exorde-0.1.0/exorde/translation/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1646 2023-04-13 13:33:28.000000 exorde-0.1.0/exorde/translation/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      785 2023-04-13 13:33:28.000000 exorde-0.1.0/exorde/translation/bindings.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      241 2023-04-13 13:33:28.000000 exorde-0.1.0/exorde/translation/setup.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-02 08:20:22.845802 exorde-0.1.0/exorde/twitter/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4607 2023-05-02 07:53:14.000000 exorde-0.1.0/exorde/twitter/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      738 2023-05-02 07:53:14.000000 exorde-0.1.0/exorde/twitter/bindings.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      186 2023-03-28 06:45:46.000000 exorde-0.1.0/exorde/twitter/setup.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-02 08:20:22.845802 exorde-0.1.0/exorde.egg-info/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      359 2023-05-02 08:20:22.000000 exorde-0.1.0/exorde.egg-info/PKG-INFO
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      662 2023-05-02 08:20:22.000000 exorde-0.1.0/exorde.egg-info/SOURCES.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        1 2023-05-02 08:20:22.000000 exorde-0.1.0/exorde.egg-info/dependency_links.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       50 2023-05-02 08:20:22.000000 exorde-0.1.0/exorde.egg-info/entry_points.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      126 2023-05-02 08:20:22.000000 exorde-0.1.0/exorde.egg-info/requires.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        7 2023-05-02 08:20:22.000000 exorde-0.1.0/exorde.egg-info/top_level.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       38 2023-05-02 08:20:22.845802 exorde-0.1.0/setup.cfg
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2080 2023-05-02 07:53:14.000000 exorde-0.1.0/setup.py
```

