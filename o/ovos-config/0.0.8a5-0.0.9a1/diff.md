# Comparing `tmp/ovos-config-0.0.8a5.tar.gz` & `tmp/ovos-config-0.0.9a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-config-0.0.8a5.tar", last modified: Tue Apr 18 21:51:25 2023, max compression
+gzip compressed data, was "ovos-config-0.0.9a1.tar", last modified: Mon May  1 23:10:19 2023, max compression
```

## Comparing `ovos-config-0.0.8a5.tar` & `ovos-config-0.0.9a1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:51:25.082614 ovos-config-0.0.8a5/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-18 21:51:25.082614 ovos-config-0.0.8a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-04-18 21:51:24.000000 ovos-config-0.0.8a5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:51:25.078613 ovos-config-0.0.8a5/ovos_config/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-18 21:51:24.000000 ovos-config-0.0.8a5/ovos_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-04-18 21:51:24.000000 ovos-config-0.0.8a5/ovos_config/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14538 2023-04-18 21:51:24.000000 ovos-config-0.0.8a5/ovos_config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-04-18 21:51:24.000000 ovos-config-0.0.8a5/ovos_config/locale.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-04-18 21:51:24.000000 ovos-config-0.0.8a5/ovos_config/locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-04-18 21:51:24.000000 ovos-config-0.0.8a5/ovos_config/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-04-18 21:51:24.000000 ovos-config-0.0.8a5/ovos_config/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    24138 2023-04-18 21:51:24.000000 ovos-config-0.0.8a5/ovos_config/mycroft.conf
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-18 21:51:24.000000 ovos-config-0.0.8a5/ovos_config/ovos.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-18 21:51:24.000000 ovos-config-0.0.8a5/ovos_config/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-18 21:51:24.000000 ovos-config-0.0.8a5/ovos_config/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:51:25.082614 ovos-config-0.0.8a5/ovos_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-18 21:51:25.000000 ovos-config-0.0.8a5/ovos_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-18 21:51:25.000000 ovos-config-0.0.8a5/ovos_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:51:25.000000 ovos-config-0.0.8a5/ovos_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-18 21:51:25.000000 ovos-config-0.0.8a5/ovos_config.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-18 21:51:25.000000 ovos-config-0.0.8a5/ovos_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 21:51:25.000000 ovos-config-0.0.8a5/ovos_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 21:51:25.082614 ovos-config-0.0.8a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-18 21:51:24.000000 ovos-config-0.0.8a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:10:19.436622 ovos-config-0.0.9a1/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-01 23:10:19.436622 ovos-config-0.0.9a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-05-01 23:10:19.000000 ovos-config-0.0.9a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:10:19.436622 ovos-config-0.0.9a1/ovos_config/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-01 23:10:19.000000 ovos-config-0.0.9a1/ovos_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-05-01 23:10:19.000000 ovos-config-0.0.9a1/ovos_config/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14538 2023-05-01 23:10:19.000000 ovos-config-0.0.9a1/ovos_config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-01 23:10:19.000000 ovos-config-0.0.9a1/ovos_config/locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-05-01 23:10:19.000000 ovos-config-0.0.9a1/ovos_config/locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-01 23:10:19.000000 ovos-config-0.0.9a1/ovos_config/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-05-01 23:10:19.000000 ovos-config-0.0.9a1/ovos_config/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24138 2023-05-01 23:10:19.000000 ovos-config-0.0.9a1/ovos_config/mycroft.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-01 23:10:19.000000 ovos-config-0.0.9a1/ovos_config/ovos.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-01 23:10:19.000000 ovos-config-0.0.9a1/ovos_config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-01 23:10:19.000000 ovos-config-0.0.9a1/ovos_config/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 23:10:19.436622 ovos-config-0.0.9a1/ovos_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-01 23:10:19.000000 ovos-config-0.0.9a1/ovos_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-01 23:10:19.000000 ovos-config-0.0.9a1/ovos_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 23:10:19.000000 ovos-config-0.0.9a1/ovos_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-01 23:10:19.000000 ovos-config-0.0.9a1/ovos_config.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-01 23:10:19.000000 ovos-config-0.0.9a1/ovos_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-01 23:10:19.000000 ovos-config-0.0.9a1/ovos_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 23:10:19.436622 ovos-config-0.0.9a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-01 23:10:19.000000 ovos-config-0.0.9a1/setup.py
```

### Comparing `ovos-config-0.0.8a5/README.md` & `ovos-config-0.0.9a1/README.md`

 * *Files identical despite different names*

### Comparing `ovos-config-0.0.8a5/ovos_config/__main__.py` & `ovos-config-0.0.9a1/ovos_config/__main__.py`

 * *Files identical despite different names*

### Comparing `ovos-config-0.0.8a5/ovos_config/config.py` & `ovos-config-0.0.9a1/ovos_config/config.py`

 * *Files identical despite different names*

### Comparing `ovos-config-0.0.8a5/ovos_config/locale.py` & `ovos-config-0.0.9a1/ovos_config/locale.py`

 * *Files identical despite different names*

### Comparing `ovos-config-0.0.8a5/ovos_config/locations.py` & `ovos-config-0.0.9a1/ovos_config/locations.py`

 * *Files identical despite different names*

### Comparing `ovos-config-0.0.8a5/ovos_config/meta.py` & `ovos-config-0.0.9a1/ovos_config/meta.py`

 * *Files identical despite different names*

### Comparing `ovos-config-0.0.8a5/ovos_config/models.py` & `ovos-config-0.0.9a1/ovos_config/models.py`

 * *Files identical despite different names*

### Comparing `ovos-config-0.0.8a5/ovos_config/mycroft.conf` & `ovos-config-0.0.9a1/ovos_config/mycroft.conf`

 * *Files identical despite different names*

### Comparing `ovos-config-0.0.8a5/setup.py` & `ovos-config-0.0.9a1/setup.py`

 * *Files identical despite different names*

