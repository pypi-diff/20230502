# Comparing `tmp/client_bank_1c-0.2.2.tar.gz` & `tmp/client_bank_1c-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "client_bank_1c-0.2.2.tar", max compression
+gzip compressed data, was "client_bank_1c-0.2.3.tar", max compression
```

## Comparing `client_bank_1c-0.2.2.tar` & `client_bank_1c-0.2.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1057 2023-04-04 23:35:03.689527 client_bank_1c-0.2.2/LICENSE
--rw-r--r--   0        0        0     4478 2023-04-19 07:17:04.187385 client_bank_1c-0.2.2/client_bank_1c.py
--rw-r--r--   0        0        0      888 2023-04-19 07:19:28.631007 client_bank_1c-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 client_bank_1c-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-04-04 23:35:03.689527 client_bank_1c-0.2.3/LICENSE
+-rw-r--r--   0        0        0     4487 2023-05-02 07:01:05.507966 client_bank_1c-0.2.3/client_bank_1c.py
+-rw-r--r--   0        0        0      888 2023-05-02 07:02:58.819738 client_bank_1c-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 client_bank_1c-0.2.3/PKG-INFO
```

### Comparing `client_bank_1c-0.2.2/LICENSE` & `client_bank_1c-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `client_bank_1c-0.2.2/client_bank_1c.py` & `client_bank_1c-0.2.3/client_bank_1c.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         for line in stream:
             if not line.strip():
                 continue
 
             key, value = self._parse_line(line)
 
             if key == 'СекцияРасчСчет':
-                assert section == 'info'
+                assert section in {'info', False}
                 section = key
                 section_values = {}
 
             elif key == 'СекцияДокумент':
                 assert section in {'info', False}
                 section = key
                 section_values = {'ВидДокумента': value}
```

### Comparing `client_bank_1c-0.2.2/pyproject.toml` & `client_bank_1c-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "client-bank-1c"
-version = "0.2.2"
+version = "0.2.3"
 description = "1C Client Bank Exchange Format"
 authors = ["Dmitry Voronin <dimka665@gmail.com>"]
 
 repository = "https://github.com/odoo-ru/client-bank-1c"
 license = "MIT"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `client_bank_1c-0.2.2/PKG-INFO` & `client_bank_1c-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: client-bank-1c
-Version: 0.2.2
+Version: 0.2.3
 Summary: 1C Client Bank Exchange Format
 Home-page: https://github.com/odoo-ru/client-bank-1c
 License: MIT
 Author: Dmitry Voronin
 Author-email: dimka665@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Intended Audience :: Developers
```

