# Comparing `tmp/blacklist-checker-0.0.4.tar.gz` & `tmp/blacklist-checker-0.0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blacklist-checker-0.0.4.tar", last modified: Tue May  2 17:44:07 2023, max compression
+gzip compressed data, was "blacklist-checker-0.0.4.1.tar", last modified: Tue May  2 17:56:28 2023, max compression
```

## Comparing `blacklist-checker-0.0.4.tar` & `blacklist-checker-0.0.4.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 benoit     (501) staff       (20)        0 2023-05-02 17:44:07.302311 blacklist-checker-0.0.4/
--rw-r--r--   0 benoit     (501) staff       (20)    11357 2023-05-01 16:18:52.000000 blacklist-checker-0.0.4/LICENSE
--rw-r--r--   0 benoit     (501) staff       (20)    13516 2023-05-02 17:44:07.301538 blacklist-checker-0.0.4/PKG-INFO
--rw-r--r--   0 benoit     (501) staff       (20)       20 2023-05-01 16:16:27.000000 blacklist-checker-0.0.4/README.md
--rw-r--r--   0 benoit     (501) staff       (20)      910 2023-05-02 17:43:55.000000 blacklist-checker-0.0.4/pyproject.toml
--rw-r--r--   0 benoit     (501) staff       (20)       38 2023-05-02 17:44:07.302476 blacklist-checker-0.0.4/setup.cfg
--rw-r--r--   0 benoit     (501) staff       (20)       47 2023-05-02 17:14:58.000000 blacklist-checker-0.0.4/setup.py
-drwxr-xr-x   0 benoit     (501) staff       (20)        0 2023-05-02 17:44:07.291481 blacklist-checker-0.0.4/src/
--rw-r--r--   0 benoit     (501) staff       (20)        0 2023-05-01 16:48:21.000000 blacklist-checker-0.0.4/src/__init__.py
-drwxr-xr-x   0 benoit     (501) staff       (20)        0 2023-05-02 17:44:07.291783 blacklist-checker-0.0.4/src/blacklist_checker/
--rw-r--r--   0 benoit     (501) staff       (20)        0 2023-05-02 17:30:59.000000 blacklist-checker-0.0.4/src/blacklist_checker/__init__.py
-drwxr-xr-x   0 benoit     (501) staff       (20)        0 2023-05-02 17:44:07.295194 blacklist-checker-0.0.4/src/blacklist_checker/cli/
--rw-r--r--   0 benoit     (501) staff       (20)        0 2023-05-02 17:25:00.000000 blacklist-checker-0.0.4/src/blacklist_checker/cli/__init__.py
--rw-r--r--   0 benoit     (501) staff       (20)     1251 2023-05-02 17:37:54.000000 blacklist-checker-0.0.4/src/blacklist_checker/cli/mycli.py
-drwxr-xr-x   0 benoit     (501) staff       (20)        0 2023-05-02 17:44:07.296887 blacklist-checker-0.0.4/src/blacklist_checker/messaging/
--rw-r--r--   0 benoit     (501) staff       (20)     7492 2023-05-02 16:41:33.000000 blacklist-checker-0.0.4/src/blacklist_checker/messaging/Mailer.py
--rw-r--r--   0 benoit     (501) staff       (20)        0 2023-04-29 16:38:19.000000 blacklist-checker-0.0.4/src/blacklist_checker/messaging/__init__.py
-drwxr-xr-x   0 benoit     (501) staff       (20)        0 2023-05-02 17:44:07.298216 blacklist-checker-0.0.4/src/blacklist_checker/requester/
--rw-r--r--   0 benoit     (501) staff       (20)     2200 2023-05-01 12:31:50.000000 blacklist-checker-0.0.4/src/blacklist_checker/requester/Black_list_checker.py
--rw-r--r--   0 benoit     (501) staff       (20)        0 2023-04-24 12:19:29.000000 blacklist-checker-0.0.4/src/blacklist_checker/requester/__init__.py
-drwxr-xr-x   0 benoit     (501) staff       (20)        0 2023-05-02 17:44:07.294428 blacklist-checker-0.0.4/src/blacklist_checker.egg-info/
--rw-r--r--   0 benoit     (501) staff       (20)    13516 2023-05-02 17:44:07.000000 blacklist-checker-0.0.4/src/blacklist_checker.egg-info/PKG-INFO
--rw-r--r--   0 benoit     (501) staff       (20)      640 2023-05-02 17:44:07.000000 blacklist-checker-0.0.4/src/blacklist_checker.egg-info/SOURCES.txt
--rw-r--r--   0 benoit     (501) staff       (20)        1 2023-05-02 17:44:07.000000 blacklist-checker-0.0.4/src/blacklist_checker.egg-info/dependency_links.txt
--rw-r--r--   0 benoit     (501) staff       (20)       71 2023-05-02 17:44:07.000000 blacklist-checker-0.0.4/src/blacklist_checker.egg-info/entry_points.txt
--rw-r--r--   0 benoit     (501) staff       (20)      100 2023-05-02 17:44:07.000000 blacklist-checker-0.0.4/src/blacklist_checker.egg-info/requires.txt
--rw-r--r--   0 benoit     (501) staff       (20)       27 2023-05-02 17:44:07.000000 blacklist-checker-0.0.4/src/blacklist_checker.egg-info/top_level.txt
-drwxr-xr-x   0 benoit     (501) staff       (20)        0 2023-05-02 17:44:07.298756 blacklist-checker-0.0.4/test/
--rw-r--r--   0 benoit     (501) staff       (20)      502 2023-05-02 16:28:55.000000 blacklist-checker-0.0.4/test/test_mailer.py
+drwxr-xr-x   0 benoit     (501) staff       (20)        0 2023-05-02 17:56:28.389238 blacklist-checker-0.0.4.1/
+-rw-r--r--   0 benoit     (501) staff       (20)    11357 2023-05-01 16:18:52.000000 blacklist-checker-0.0.4.1/LICENSE
+-rw-r--r--   0 benoit     (501) staff       (20)    13518 2023-05-02 17:56:28.388608 blacklist-checker-0.0.4.1/PKG-INFO
+-rw-r--r--   0 benoit     (501) staff       (20)       20 2023-05-01 16:16:27.000000 blacklist-checker-0.0.4.1/README.md
+-rw-r--r--   0 benoit     (501) staff       (20)      925 2023-05-02 17:56:14.000000 blacklist-checker-0.0.4.1/pyproject.toml
+-rw-r--r--   0 benoit     (501) staff       (20)       38 2023-05-02 17:56:28.389369 blacklist-checker-0.0.4.1/setup.cfg
+-rw-r--r--   0 benoit     (501) staff       (20)       47 2023-05-02 17:14:58.000000 blacklist-checker-0.0.4.1/setup.py
+drwxr-xr-x   0 benoit     (501) staff       (20)        0 2023-05-02 17:56:28.364087 blacklist-checker-0.0.4.1/src/
+-rw-r--r--   0 benoit     (501) staff       (20)        0 2023-05-01 16:48:21.000000 blacklist-checker-0.0.4.1/src/__init__.py
+drwxr-xr-x   0 benoit     (501) staff       (20)        0 2023-05-02 17:56:28.365284 blacklist-checker-0.0.4.1/src/blacklist_checker/
+-rw-r--r--   0 benoit     (501) staff       (20)        0 2023-05-02 17:30:59.000000 blacklist-checker-0.0.4.1/src/blacklist_checker/__init__.py
+drwxr-xr-x   0 benoit     (501) staff       (20)        0 2023-05-02 17:56:28.382732 blacklist-checker-0.0.4.1/src/blacklist_checker/cli/
+-rw-r--r--   0 benoit     (501) staff       (20)        0 2023-05-02 17:25:00.000000 blacklist-checker-0.0.4.1/src/blacklist_checker/cli/__init__.py
+-rw-r--r--   0 benoit     (501) staff       (20)     1287 2023-05-02 17:54:28.000000 blacklist-checker-0.0.4.1/src/blacklist_checker/cli/mycli.py
+drwxr-xr-x   0 benoit     (501) staff       (20)        0 2023-05-02 17:56:28.385001 blacklist-checker-0.0.4.1/src/blacklist_checker/messaging/
+-rw-r--r--   0 benoit     (501) staff       (20)     7492 2023-05-02 16:41:33.000000 blacklist-checker-0.0.4.1/src/blacklist_checker/messaging/Mailer.py
+-rw-r--r--   0 benoit     (501) staff       (20)        0 2023-04-29 16:38:19.000000 blacklist-checker-0.0.4.1/src/blacklist_checker/messaging/__init__.py
+drwxr-xr-x   0 benoit     (501) staff       (20)        0 2023-05-02 17:56:28.386614 blacklist-checker-0.0.4.1/src/blacklist_checker/requester/
+-rw-r--r--   0 benoit     (501) staff       (20)     2200 2023-05-01 12:31:50.000000 blacklist-checker-0.0.4.1/src/blacklist_checker/requester/Black_list_checker.py
+-rw-r--r--   0 benoit     (501) staff       (20)        0 2023-04-24 12:19:29.000000 blacklist-checker-0.0.4.1/src/blacklist_checker/requester/__init__.py
+drwxr-xr-x   0 benoit     (501) staff       (20)        0 2023-05-02 17:56:28.379112 blacklist-checker-0.0.4.1/src/blacklist_checker.egg-info/
+-rw-r--r--   0 benoit     (501) staff       (20)    13518 2023-05-02 17:56:28.000000 blacklist-checker-0.0.4.1/src/blacklist_checker.egg-info/PKG-INFO
+-rw-r--r--   0 benoit     (501) staff       (20)      640 2023-05-02 17:56:28.000000 blacklist-checker-0.0.4.1/src/blacklist_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 benoit     (501) staff       (20)        1 2023-05-02 17:56:28.000000 blacklist-checker-0.0.4.1/src/blacklist_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 benoit     (501) staff       (20)       71 2023-05-02 17:56:28.000000 blacklist-checker-0.0.4.1/src/blacklist_checker.egg-info/entry_points.txt
+-rw-r--r--   0 benoit     (501) staff       (20)      106 2023-05-02 17:56:28.000000 blacklist-checker-0.0.4.1/src/blacklist_checker.egg-info/requires.txt
+-rw-r--r--   0 benoit     (501) staff       (20)       27 2023-05-02 17:56:28.000000 blacklist-checker-0.0.4.1/src/blacklist_checker.egg-info/top_level.txt
+drwxr-xr-x   0 benoit     (501) staff       (20)        0 2023-05-02 17:56:28.387220 blacklist-checker-0.0.4.1/test/
+-rw-r--r--   0 benoit     (501) staff       (20)      502 2023-05-02 16:28:55.000000 blacklist-checker-0.0.4.1/test/test_mailer.py
```

### Comparing `blacklist-checker-0.0.4/LICENSE` & `blacklist-checker-0.0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `blacklist-checker-0.0.4/PKG-INFO` & `blacklist-checker-0.0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blacklist-checker
-Version: 0.0.4
+Version: 0.0.4.1
 Summary: Check if a specific domain is in mail blaclist 
 Author-email: Benoit Chenal <ben57univ@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `blacklist-checker-0.0.4/pyproject.toml` & `blacklist-checker-0.0.4.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.2", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "blacklist-checker"
-version = "0.0.4"
+version = "0.0.4.1"
 description = "Check if a specific domain is in mail blaclist "
 readme = "README.md"
 authors = [{ name = "Benoit Chenal", email = "ben57univ@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -19,14 +19,15 @@
 
 
 
 
 keywords = ["blacklist", "domain", "mail"]
 dependencies = [
     "requests",
+    "typer",
     "configparser",
     'tomli; python_version < "3.11"',
 ]
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
```

### Comparing `blacklist-checker-0.0.4/src/blacklist_checker/cli/mycli.py` & `blacklist-checker-0.0.4.1/src/blacklist_checker/cli/mycli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import typer
 import sys
-from requester.Black_list_checker import BlackListListChecker
-from messaging.Mailer import MyMailer
+from blacklist_checker.requester.Black_list_checker import BlackListListChecker
+from blacklist_checker.messaging.Mailer import MyMailer
 app = typer.Typer()
 
 @app.command()
 def checkdns(domain:str = typer.Option("", help=("domain to test")),config:str=typer.Option("",help=("Configuration file")),reporting:bool=typer.Option(False,help=("If set a reporting is sent ")),provider:str=typer.Option("",help=("provider file"))):
     try:
         if config=="":
             config_file="config.ini"
```

### Comparing `blacklist-checker-0.0.4/src/blacklist_checker/messaging/Mailer.py` & `blacklist-checker-0.0.4.1/src/blacklist_checker/messaging/Mailer.py`

 * *Files identical despite different names*

### Comparing `blacklist-checker-0.0.4/src/blacklist_checker/requester/Black_list_checker.py` & `blacklist-checker-0.0.4.1/src/blacklist_checker/requester/Black_list_checker.py`

 * *Files identical despite different names*

### Comparing `blacklist-checker-0.0.4/src/blacklist_checker.egg-info/PKG-INFO` & `blacklist-checker-0.0.4.1/src/blacklist_checker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blacklist-checker
-Version: 0.0.4
+Version: 0.0.4.1
 Summary: Check if a specific domain is in mail blaclist 
 Author-email: Benoit Chenal <ben57univ@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `blacklist-checker-0.0.4/src/blacklist_checker.egg-info/SOURCES.txt` & `blacklist-checker-0.0.4.1/src/blacklist_checker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

