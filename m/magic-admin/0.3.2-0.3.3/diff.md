# Comparing `tmp/magic-admin-0.3.2.tar.gz` & `tmp/magic-admin-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/magic-admin-0.3.2.tar", last modified: Fri Mar 24 22:34:48 2023, max compression
+gzip compressed data, was "magic-admin-0.3.3.tar", last modified: Tue May  2 19:03:50 2023, max compression
```

## Comparing `magic-admin-0.3.2.tar` & `magic-admin-0.3.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 justin     (501) staff       (20)        0 2023-03-24 22:34:48.000000 magic-admin-0.3.2/
--rw-r--r--   0 justin     (501) staff       (20)     4581 2023-03-24 22:34:48.000000 magic-admin-0.3.2/PKG-INFO
-drwxr-xr-x   0 justin     (501) staff       (20)        0 2023-03-24 22:34:48.000000 magic-admin-0.3.2/magic_admin/
--rw-r--r--   0 justin     (501) staff       (20)     1110 2022-11-23 19:09:59.000000 magic-admin-0.3.2/magic_admin/magic.py
--rw-r--r--   0 justin     (501) staff       (20)      449 2022-11-23 19:09:59.000000 magic-admin-0.3.2/magic_admin/config.py
--rw-r--r--   0 justin     (501) staff       (20)       18 2023-03-24 22:34:14.000000 magic-admin-0.3.2/magic_admin/version.py
--rw-r--r--   0 justin     (501) staff       (20)     2196 2023-03-15 18:09:32.000000 magic-admin-0.3.2/magic_admin/error.py
--rw-r--r--   0 justin     (501) staff       (20)     4550 2022-11-23 19:09:59.000000 magic-admin-0.3.2/magic_admin/http_client.py
-drwxr-xr-x   0 justin     (501) staff       (20)        0 2023-03-24 22:34:48.000000 magic-admin-0.3.2/magic_admin/resources/
--rw-r--r--   0 justin     (501) staff       (20)     1778 2023-01-04 23:30:48.000000 magic-admin-0.3.2/magic_admin/resources/user.py
--rw-r--r--   0 justin     (501) staff       (20)     5230 2023-03-15 18:09:32.000000 magic-admin-0.3.2/magic_admin/resources/token.py
--rw-r--r--   0 justin     (501) staff       (20)     2222 2023-03-24 22:34:14.000000 magic-admin-0.3.2/magic_admin/resources/nft.py
--rw-r--r--   0 justin     (501) staff       (20)      184 2023-03-24 19:59:14.000000 magic-admin-0.3.2/magic_admin/resources/__init__.py
--rw-r--r--   0 justin     (501) staff       (20)     1488 2022-11-23 19:09:59.000000 magic-admin-0.3.2/magic_admin/resources/base.py
--rw-r--r--   0 justin     (501) staff       (20)      496 2023-01-04 23:30:48.000000 magic-admin-0.3.2/magic_admin/resources/wallet.py
--rw-r--r--   0 justin     (501) staff       (20)      199 2022-11-23 19:09:59.000000 magic-admin-0.3.2/magic_admin/__init__.py
--rw-r--r--   0 justin     (501) staff       (20)      187 2022-11-23 19:09:59.000000 magic-admin-0.3.2/magic_admin/response.py
-drwxr-xr-x   0 justin     (501) staff       (20)        0 2023-03-24 22:34:48.000000 magic-admin-0.3.2/magic_admin/utils/
--rw-r--r--   0 justin     (501) staff       (20)      199 2022-11-23 19:09:59.000000 magic-admin-0.3.2/magic_admin/utils/time.py
--rw-r--r--   0 justin     (501) staff       (20)      745 2023-03-15 18:09:32.000000 magic-admin-0.3.2/magic_admin/utils/did_token.py
--rw-r--r--   0 justin     (501) staff       (20)        0 2022-11-23 19:09:59.000000 magic-admin-0.3.2/magic_admin/utils/__init__.py
--rw-r--r--   0 justin     (501) staff       (20)      371 2022-11-23 19:09:59.000000 magic-admin-0.3.2/magic_admin/utils/http.py
--rw-r--r--   0 justin     (501) staff       (20)     3100 2022-11-23 19:09:59.000000 magic-admin-0.3.2/README.md
--rw-r--r--   0 justin     (501) staff       (20)     1696 2022-11-23 19:09:59.000000 magic-admin-0.3.2/setup.py
-drwxr-xr-x   0 justin     (501) staff       (20)        0 2023-03-24 22:34:48.000000 magic-admin-0.3.2/magic_admin.egg-info/
--rw-r--r--   0 justin     (501) staff       (20)     4581 2023-03-24 22:34:48.000000 magic-admin-0.3.2/magic_admin.egg-info/PKG-INFO
--rw-r--r--   0 justin     (501) staff       (20)        1 2023-03-15 18:10:58.000000 magic-admin-0.3.2/magic_admin.egg-info/not-zip-safe
--rw-r--r--   0 justin     (501) staff       (20)      697 2023-03-24 22:34:48.000000 magic-admin-0.3.2/magic_admin.egg-info/SOURCES.txt
--rw-r--r--   0 justin     (501) staff       (20)       35 2023-03-24 22:34:48.000000 magic-admin-0.3.2/magic_admin.egg-info/requires.txt
--rw-r--r--   0 justin     (501) staff       (20)       12 2023-03-24 22:34:48.000000 magic-admin-0.3.2/magic_admin.egg-info/top_level.txt
--rw-r--r--   0 justin     (501) staff       (20)        1 2023-03-24 22:34:48.000000 magic-admin-0.3.2/magic_admin.egg-info/dependency_links.txt
--rw-r--r--   0 justin     (501) staff       (20)      106 2023-03-24 22:34:48.000000 magic-admin-0.3.2/setup.cfg
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-05-02 19:03:50.607137 magic-admin-0.3.3/
+-rw-r--r--   0 ben        (501) staff       (20)     1081 2023-05-02 16:31:00.000000 magic-admin-0.3.3/LICENSE.txt
+-rw-r--r--   0 ben        (501) staff       (20)     3712 2023-05-02 19:03:50.607211 magic-admin-0.3.3/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)     3100 2023-05-02 16:31:00.000000 magic-admin-0.3.3/README.md
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-05-02 19:03:50.604067 magic-admin-0.3.3/magic_admin/
+-rw-r--r--   0 ben        (501) staff       (20)      199 2023-05-02 16:31:00.000000 magic-admin-0.3.3/magic_admin/__init__.py
+-rw-r--r--   0 ben        (501) staff       (20)      449 2023-05-02 16:31:00.000000 magic-admin-0.3.3/magic_admin/config.py
+-rw-r--r--   0 ben        (501) staff       (20)     2196 2023-05-02 16:31:00.000000 magic-admin-0.3.3/magic_admin/error.py
+-rw-r--r--   0 ben        (501) staff       (20)     4550 2023-05-02 16:31:00.000000 magic-admin-0.3.3/magic_admin/http_client.py
+-rw-r--r--   0 ben        (501) staff       (20)     1110 2023-05-02 16:31:00.000000 magic-admin-0.3.3/magic_admin/magic.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-05-02 19:03:50.606301 magic-admin-0.3.3/magic_admin/resources/
+-rw-r--r--   0 ben        (501) staff       (20)      142 2023-05-02 16:36:19.000000 magic-admin-0.3.3/magic_admin/resources/__init__.py
+-rw-r--r--   0 ben        (501) staff       (20)     1488 2023-05-02 16:31:00.000000 magic-admin-0.3.3/magic_admin/resources/base.py
+-rw-r--r--   0 ben        (501) staff       (20)     5230 2023-05-02 16:31:00.000000 magic-admin-0.3.3/magic_admin/resources/token.py
+-rw-r--r--   0 ben        (501) staff       (20)     1778 2023-05-02 16:31:00.000000 magic-admin-0.3.3/magic_admin/resources/user.py
+-rw-r--r--   0 ben        (501) staff       (20)      496 2023-05-02 16:31:00.000000 magic-admin-0.3.3/magic_admin/resources/wallet.py
+-rw-r--r--   0 ben        (501) staff       (20)      187 2023-05-02 16:31:00.000000 magic-admin-0.3.3/magic_admin/response.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-05-02 19:03:50.606949 magic-admin-0.3.3/magic_admin/utils/
+-rw-r--r--   0 ben        (501) staff       (20)        0 2023-05-02 16:31:00.000000 magic-admin-0.3.3/magic_admin/utils/__init__.py
+-rw-r--r--   0 ben        (501) staff       (20)      745 2023-05-02 16:31:00.000000 magic-admin-0.3.3/magic_admin/utils/did_token.py
+-rw-r--r--   0 ben        (501) staff       (20)      371 2023-05-02 16:31:00.000000 magic-admin-0.3.3/magic_admin/utils/http.py
+-rw-r--r--   0 ben        (501) staff       (20)      199 2023-05-02 16:31:00.000000 magic-admin-0.3.3/magic_admin/utils/time.py
+-rw-r--r--   0 ben        (501) staff       (20)       18 2023-05-02 16:32:49.000000 magic-admin-0.3.3/magic_admin/version.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2023-05-02 19:03:50.605184 magic-admin-0.3.3/magic_admin.egg-info/
+-rw-r--r--   0 ben        (501) staff       (20)     3712 2023-05-02 19:03:50.000000 magic-admin-0.3.3/magic_admin.egg-info/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)      680 2023-05-02 19:03:50.000000 magic-admin-0.3.3/magic_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 ben        (501) staff       (20)        1 2023-05-02 19:03:50.000000 magic-admin-0.3.3/magic_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 ben        (501) staff       (20)        1 2023-05-02 19:03:50.000000 magic-admin-0.3.3/magic_admin.egg-info/not-zip-safe
+-rw-r--r--   0 ben        (501) staff       (20)       35 2023-05-02 19:03:50.000000 magic-admin-0.3.3/magic_admin.egg-info/requires.txt
+-rw-r--r--   0 ben        (501) staff       (20)       12 2023-05-02 19:03:50.000000 magic-admin-0.3.3/magic_admin.egg-info/top_level.txt
+-rw-r--r--   0 ben        (501) staff       (20)      106 2023-05-02 19:03:50.607457 magic-admin-0.3.3/setup.cfg
+-rw-r--r--   0 ben        (501) staff       (20)     1696 2023-05-02 16:31:00.000000 magic-admin-0.3.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `magic-admin-0.3.2/magic_admin/magic.py` & `magic-admin-0.3.3/magic_admin/magic.py`

 * *Files identical despite different names*

### Comparing `magic-admin-0.3.2/magic_admin/error.py` & `magic-admin-0.3.3/magic_admin/error.py`

 * *Files identical despite different names*

### Comparing `magic-admin-0.3.2/magic_admin/http_client.py` & `magic-admin-0.3.3/magic_admin/http_client.py`

 * *Files identical despite different names*

### Comparing `magic-admin-0.3.2/magic_admin/resources/user.py` & `magic-admin-0.3.3/magic_admin/resources/user.py`

 * *Files identical despite different names*

### Comparing `magic-admin-0.3.2/magic_admin/resources/token.py` & `magic-admin-0.3.3/magic_admin/resources/token.py`

 * *Files identical despite different names*

### Comparing `magic-admin-0.3.2/magic_admin/resources/base.py` & `magic-admin-0.3.3/magic_admin/resources/base.py`

 * *Files identical despite different names*

### Comparing `magic-admin-0.3.2/magic_admin/utils/did_token.py` & `magic-admin-0.3.3/magic_admin/utils/did_token.py`

 * *Files identical despite different names*

### Comparing `magic-admin-0.3.2/README.md` & `magic-admin-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `magic-admin-0.3.2/setup.py` & `magic-admin-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `magic-admin-0.3.2/magic_admin.egg-info/SOURCES.txt` & `magic-admin-0.3.3/magic_admin.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 README.md
 setup.cfg
 setup.py
 magic_admin/__init__.py
 magic_admin/config.py
 magic_admin/error.py
 magic_admin/http_client.py
@@ -12,15 +13,14 @@
 magic_admin.egg-info/SOURCES.txt
 magic_admin.egg-info/dependency_links.txt
 magic_admin.egg-info/not-zip-safe
 magic_admin.egg-info/requires.txt
 magic_admin.egg-info/top_level.txt
 magic_admin/resources/__init__.py
 magic_admin/resources/base.py
-magic_admin/resources/nft.py
 magic_admin/resources/token.py
 magic_admin/resources/user.py
 magic_admin/resources/wallet.py
 magic_admin/utils/__init__.py
 magic_admin/utils/did_token.py
 magic_admin/utils/http.py
 magic_admin/utils/time.py
```

