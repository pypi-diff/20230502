# Comparing `tmp/simplepg-0.1.3.tar.gz` & `tmp/simplepg-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplepg-0.1.3.tar", max compression
+gzip compressed data, was "simplepg-0.1.4.tar", max compression
```

## Comparing `simplepg-0.1.3.tar` & `simplepg-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    10255 2023-01-03 08:38:50.251480 simplepg-0.1.3/LICENSE
--rw-r--r--   0        0        0       41 2023-01-03 08:41:34.060855 simplepg-0.1.3/README.md
--rw-r--r--   0        0        0     1147 2023-01-18 15:55:51.434592 simplepg-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       64 2023-01-03 08:40:33.148344 simplepg-0.1.3/simplepg/__init__.py
--rw-r--r--   0        0        0     4087 2023-01-18 15:52:38.312878 simplepg-0.1.3/simplepg/db.py
--rw-r--r--   0        0        0      691 1970-01-01 00:00:00.000000 simplepg-0.1.3/setup.py
--rw-r--r--   0        0        0      624 1970-01-01 00:00:00.000000 simplepg-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    10255 2023-01-03 08:38:50.251480 simplepg-0.1.4/LICENSE
+-rw-r--r--   0        0        0      794 2023-05-02 13:51:42.564005 simplepg-0.1.4/README.md
+-rw-r--r--   0        0        0     1214 2023-05-02 13:58:33.235465 simplepg-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       64 2023-01-03 08:40:33.148344 simplepg-0.1.4/simplepg/__init__.py
+-rw-r--r--   0        0        0     6286 2023-05-02 13:57:41.082518 simplepg-0.1.4/simplepg/db.py
+-rw-r--r--   0        0        0     1478 1970-01-01 00:00:00.000000 simplepg-0.1.4/setup.py
+-rw-r--r--   0        0        0     1377 1970-01-01 00:00:00.000000 simplepg-0.1.4/PKG-INFO
```

### Comparing `simplepg-0.1.3/LICENSE` & `simplepg-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `simplepg-0.1.3/pyproject.toml` & `simplepg-0.1.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "simplepg"
-version = "0.1.3"
+version = "0.1.4"
 description = "Simple PostgreSQL connections"
 authors = ["Mysterious Ben <datascience@tuta.io>"]
 exclude = [".git", ".gitignore", ".venv/", ".mypy_cache/", "__pycache__", ".eggs/"]
 license = "Apache License 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
@@ -15,14 +15,17 @@
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 isort = "^5.11.4"
 mypy = "^0.991"
 pytest = "^7.2.0"
 pylint = "^2.15.9"
 flake8 = "^6.0.0"
+python-dotenv = "^1.0.0"
+envparse = "^0.2.0"
+pre-commit = "^3.3.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line_length = 99
```

