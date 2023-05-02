# Comparing `tmp/rpa_cooperativa-1.0.49.tar.gz` & `tmp/rpa_cooperativa-1.0.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpa_cooperativa-1.0.49.tar", last modified: Tue May  2 17:56:08 2023, max compression
+gzip compressed data, was "rpa_cooperativa-1.0.50.tar", last modified: Tue May  2 17:59:17 2023, max compression
```

## Comparing `rpa_cooperativa-1.0.49.tar` & `rpa_cooperativa-1.0.50.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 17:56:08.201732 rpa_cooperativa-1.0.49/
--rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.49/LICENSE
--rw-rw-rw-   0        0        0     6585 2023-05-02 17:56:08.197708 rpa_cooperativa-1.0.49/PKG-INFO
--rw-rw-rw-   0        0        0     5440 2023-05-02 17:52:50.000000 rpa_cooperativa-1.0.49/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 17:56:08.053279 rpa_cooperativa-1.0.49/rpa_coop/
--rw-rw-rw-   0        0        0      568 2023-05-02 17:34:09.000000 rpa_cooperativa-1.0.49/rpa_coop/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 17:56:08.144112 rpa_cooperativa-1.0.49/rpa_coop/img/
--rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.49/rpa_coop/img/hash
--rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.49/rpa_coop/img/relatorios_azul.PNG
--rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.49/rpa_coop/img/relatorios_verde.PNG
--rw-rw-rw-   0        0        0      379 2023-02-28 19:52:56.000000 rpa_cooperativa-1.0.49/rpa_coop/img/sacg_branco.PNG
--rw-rw-rw-   0        0        0      382 2023-02-28 19:50:17.000000 rpa_cooperativa-1.0.49/rpa_coop/img/sagc_verde.PNG
--rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.49/rpa_coop/img/siac_amarelo.PNG
--rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.49/rpa_coop/img/siac_branco.PNG
--rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.49/rpa_coop/img/siat_amarelo.PNG
--rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.49/rpa_coop/img/siat_branco.PNG
--rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.49/rpa_coop/img/transacional_azul.PNG
--rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.49/rpa_coop/img/transacional_verde.PNG
--rw-rw-rw-   0        0        0    78671 2023-05-02 17:48:06.000000 rpa_cooperativa-1.0.49/rpa_coop/rpa_coop.py
-drwxrwxrwx   0        0        0        0 2023-05-02 17:56:08.190400 rpa_cooperativa-1.0.49/rpa_cooperativa.egg-info/
--rw-rw-rw-   0        0        0     6585 2023-05-02 17:56:07.000000 rpa_cooperativa-1.0.49/rpa_cooperativa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      631 2023-05-02 17:56:07.000000 rpa_cooperativa-1.0.49/rpa_cooperativa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 17:56:07.000000 rpa_cooperativa-1.0.49/rpa_cooperativa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-02 17:56:07.000000 rpa_cooperativa-1.0.49/rpa_cooperativa.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      559 2023-05-02 17:56:07.000000 rpa_cooperativa-1.0.49/rpa_cooperativa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-02 17:56:07.000000 rpa_cooperativa-1.0.49/rpa_cooperativa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 17:56:08.202731 rpa_cooperativa-1.0.49/setup.cfg
--rw-rw-rw-   0        0        0     2323 2023-05-02 17:55:47.000000 rpa_cooperativa-1.0.49/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:59:17.785340 rpa_cooperativa-1.0.50/
+-rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.50/LICENSE
+-rw-rw-rw-   0        0        0     6585 2023-05-02 17:59:17.782316 rpa_cooperativa-1.0.50/PKG-INFO
+-rw-rw-rw-   0        0        0     5440 2023-05-02 17:52:50.000000 rpa_cooperativa-1.0.50/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 17:59:17.637392 rpa_cooperativa-1.0.50/rpa_coop/
+-rw-rw-rw-   0        0        0      568 2023-05-02 17:34:09.000000 rpa_cooperativa-1.0.50/rpa_coop/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:59:17.729851 rpa_cooperativa-1.0.50/rpa_coop/img/
+-rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.50/rpa_coop/img/hash
+-rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.50/rpa_coop/img/relatorios_azul.PNG
+-rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.50/rpa_coop/img/relatorios_verde.PNG
+-rw-rw-rw-   0        0        0      379 2023-02-28 19:52:56.000000 rpa_cooperativa-1.0.50/rpa_coop/img/sacg_branco.PNG
+-rw-rw-rw-   0        0        0      382 2023-02-28 19:50:17.000000 rpa_cooperativa-1.0.50/rpa_coop/img/sagc_verde.PNG
+-rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.50/rpa_coop/img/siac_amarelo.PNG
+-rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.50/rpa_coop/img/siac_branco.PNG
+-rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.50/rpa_coop/img/siat_amarelo.PNG
+-rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.50/rpa_coop/img/siat_branco.PNG
+-rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.50/rpa_coop/img/transacional_azul.PNG
+-rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.50/rpa_coop/img/transacional_verde.PNG
+-rw-rw-rw-   0        0        0    78671 2023-05-02 17:59:03.000000 rpa_cooperativa-1.0.50/rpa_coop/rpa_coop.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:59:17.772321 rpa_cooperativa-1.0.50/rpa_cooperativa.egg-info/
+-rw-rw-rw-   0        0        0     6585 2023-05-02 17:59:17.000000 rpa_cooperativa-1.0.50/rpa_cooperativa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      631 2023-05-02 17:59:17.000000 rpa_cooperativa-1.0.50/rpa_cooperativa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 17:59:17.000000 rpa_cooperativa-1.0.50/rpa_cooperativa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-02 17:59:17.000000 rpa_cooperativa-1.0.50/rpa_cooperativa.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      559 2023-05-02 17:59:17.000000 rpa_cooperativa-1.0.50/rpa_cooperativa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-02 17:59:17.000000 rpa_cooperativa-1.0.50/rpa_cooperativa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 17:59:17.786318 rpa_cooperativa-1.0.50/setup.cfg
+-rw-rw-rw-   0        0        0     2323 2023-05-02 17:58:41.000000 rpa_cooperativa-1.0.50/setup.py
```

### Comparing `rpa_cooperativa-1.0.49/LICENSE` & `rpa_cooperativa-1.0.50/LICENSE`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.49/PKG-INFO` & `rpa_cooperativa-1.0.50/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa_cooperativa
-Version: 1.0.49
+Version: 1.0.50
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
```

### Comparing `rpa_cooperativa-1.0.49/README.md` & `rpa_cooperativa-1.0.50/README.md`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.49/rpa_coop/__init__.py` & `rpa_cooperativa-1.0.50/rpa_coop/__init__.py`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.49/rpa_coop/img/relatorios_azul.PNG` & `rpa_cooperativa-1.0.50/rpa_coop/img/relatorios_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.49/rpa_coop/img/relatorios_verde.PNG` & `rpa_cooperativa-1.0.50/rpa_coop/img/relatorios_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.49/rpa_coop/img/transacional_azul.PNG` & `rpa_cooperativa-1.0.50/rpa_coop/img/transacional_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.49/rpa_coop/img/transacional_verde.PNG` & `rpa_cooperativa-1.0.50/rpa_coop/img/transacional_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.49/rpa_coop/rpa_coop.py` & `rpa_cooperativa-1.0.50/rpa_coop/rpa_coop.py`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.49/rpa_cooperativa.egg-info/PKG-INFO` & `rpa_cooperativa-1.0.50/rpa_cooperativa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa-cooperativa
-Version: 1.0.49
+Version: 1.0.50
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
```

### Comparing `rpa_cooperativa-1.0.49/rpa_cooperativa.egg-info/SOURCES.txt` & `rpa_cooperativa-1.0.50/rpa_cooperativa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.49/rpa_cooperativa.egg-info/requires.txt` & `rpa_cooperativa-1.0.50/rpa_cooperativa.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.49/setup.py` & `rpa_cooperativa-1.0.50/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(
     name="rpa_cooperativa",
-    version="1.0.49",
+    version="1.0.50",
     license='MIT License',
     author="Edenilson Fernandes dos Santos",
     author_email='santoeen@gmail.com',
     description="Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc",
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords='rpa cooperativa fluid api automação sql sqlalchemy',
```

