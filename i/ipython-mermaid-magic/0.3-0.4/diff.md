# Comparing `tmp/ipython-mermaid-magic-0.3.tar.gz` & `tmp/ipython-mermaid-magic-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipython-mermaid-magic-0.3.tar", last modified: Tue May  2 15:04:16 2023, max compression
+gzip compressed data, was "ipython-mermaid-magic-0.4.tar", last modified: Tue May  2 15:08:15 2023, max compression
```

## Comparing `ipython-mermaid-magic-0.3.tar` & `ipython-mermaid-magic-0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mariussandu   (501) staff       (20)        0 2023-05-02 15:04:16.736305 ipython-mermaid-magic-0.3/
--rw-r--r--   0 mariussandu   (501) staff       (20)     1068 2023-05-02 14:22:58.000000 ipython-mermaid-magic-0.3/LICENSE.txt
-drwxr-xr-x   0 mariussandu   (501) staff       (20)        0 2023-05-02 15:04:16.717435 ipython-mermaid-magic-0.3/MermaidMagic/
--rw-r--r--   0 mariussandu   (501) staff       (20)      884 2023-05-02 15:02:40.000000 ipython-mermaid-magic-0.3/MermaidMagic/Mermaid.py
--rw-r--r--   0 mariussandu   (501) staff       (20)        0 2023-05-02 14:43:34.000000 ipython-mermaid-magic-0.3/MermaidMagic/__init__.py
--rw-r--r--   0 mariussandu   (501) staff       (20)      842 2023-05-02 15:04:16.736515 ipython-mermaid-magic-0.3/PKG-INFO
--rw-r--r--   0 mariussandu   (501) staff       (20)       22 2023-05-02 14:25:38.000000 ipython-mermaid-magic-0.3/README.md
-drwxr-xr-x   0 mariussandu   (501) staff       (20)        0 2023-05-02 15:04:16.735732 ipython-mermaid-magic-0.3/ipython_mermaid_magic.egg-info/
--rw-r--r--   0 mariussandu   (501) staff       (20)      842 2023-05-02 15:04:16.000000 ipython-mermaid-magic-0.3/ipython_mermaid_magic.egg-info/PKG-INFO
--rw-r--r--   0 mariussandu   (501) staff       (20)      313 2023-05-02 15:04:16.000000 ipython-mermaid-magic-0.3/ipython_mermaid_magic.egg-info/SOURCES.txt
--rw-r--r--   0 mariussandu   (501) staff       (20)        1 2023-05-02 15:04:16.000000 ipython-mermaid-magic-0.3/ipython_mermaid_magic.egg-info/dependency_links.txt
--rw-r--r--   0 mariussandu   (501) staff       (20)        8 2023-05-02 15:04:16.000000 ipython-mermaid-magic-0.3/ipython_mermaid_magic.egg-info/requires.txt
--rw-r--r--   0 mariussandu   (501) staff       (20)       13 2023-05-02 15:04:16.000000 ipython-mermaid-magic-0.3/ipython_mermaid_magic.egg-info/top_level.txt
--rw-r--r--   0 mariussandu   (501) staff       (20)       79 2023-05-02 15:04:16.737599 ipython-mermaid-magic-0.3/setup.cfg
--rw-r--r--   0 mariussandu   (501) staff       (20)      943 2023-05-02 15:04:13.000000 ipython-mermaid-magic-0.3/setup.py
+drwxr-xr-x   0 mariussandu   (501) staff       (20)        0 2023-05-02 15:08:15.986072 ipython-mermaid-magic-0.4/
+-rw-r--r--   0 mariussandu   (501) staff       (20)     1068 2023-05-02 14:22:58.000000 ipython-mermaid-magic-0.4/LICENSE.txt
+drwxr-xr-x   0 mariussandu   (501) staff       (20)        0 2023-05-02 15:08:15.969541 ipython-mermaid-magic-0.4/MermaidMagic/
+-rw-r--r--   0 mariussandu   (501) staff       (20)      878 2023-05-02 15:07:51.000000 ipython-mermaid-magic-0.4/MermaidMagic/Mermaid.py
+-rw-r--r--   0 mariussandu   (501) staff       (20)        0 2023-05-02 14:43:34.000000 ipython-mermaid-magic-0.4/MermaidMagic/__init__.py
+-rw-r--r--   0 mariussandu   (501) staff       (20)      842 2023-05-02 15:08:15.986277 ipython-mermaid-magic-0.4/PKG-INFO
+-rw-r--r--   0 mariussandu   (501) staff       (20)       22 2023-05-02 14:25:38.000000 ipython-mermaid-magic-0.4/README.md
+drwxr-xr-x   0 mariussandu   (501) staff       (20)        0 2023-05-02 15:08:15.985520 ipython-mermaid-magic-0.4/ipython_mermaid_magic.egg-info/
+-rw-r--r--   0 mariussandu   (501) staff       (20)      842 2023-05-02 15:08:15.000000 ipython-mermaid-magic-0.4/ipython_mermaid_magic.egg-info/PKG-INFO
+-rw-r--r--   0 mariussandu   (501) staff       (20)      313 2023-05-02 15:08:15.000000 ipython-mermaid-magic-0.4/ipython_mermaid_magic.egg-info/SOURCES.txt
+-rw-r--r--   0 mariussandu   (501) staff       (20)        1 2023-05-02 15:08:15.000000 ipython-mermaid-magic-0.4/ipython_mermaid_magic.egg-info/dependency_links.txt
+-rw-r--r--   0 mariussandu   (501) staff       (20)        8 2023-05-02 15:08:15.000000 ipython-mermaid-magic-0.4/ipython_mermaid_magic.egg-info/requires.txt
+-rw-r--r--   0 mariussandu   (501) staff       (20)       13 2023-05-02 15:08:15.000000 ipython-mermaid-magic-0.4/ipython_mermaid_magic.egg-info/top_level.txt
+-rw-r--r--   0 mariussandu   (501) staff       (20)       79 2023-05-02 15:08:15.987941 ipython-mermaid-magic-0.4/setup.cfg
+-rw-r--r--   0 mariussandu   (501) staff       (20)      943 2023-05-02 15:08:13.000000 ipython-mermaid-magic-0.4/setup.py
```

### Comparing `ipython-mermaid-magic-0.3/LICENSE.txt` & `ipython-mermaid-magic-0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ipython-mermaid-magic-0.3/MermaidMagic/Mermaid.py` & `ipython-mermaid-magic-0.4/MermaidMagic/Mermaid.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from IPython.core.magic import register_cell_magic
 from IPython.display import display, HTML
 
 
 @register_cell_magic
-def mermaid(self, line: str, cell: str) -> None:
+def mermaid(line: str, cell: str) -> None:
     """
     inspired from https://github.com/oruelle/md_mermaid;
     """
     display(
         HTML(
         f"""
         <script src='https://cdnjs.cloudflare.com/ajax/libs/mermaid/9.3.0/mermaid.min.js'></script>
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
 from IPython.core.magic import register_cell_magic from IPython.display import
-display, HTML @register_cell_magic def mermaid(self, line: str, cell: str) -
-> None: """ inspired from https://github.com/oruelle/md_mermaid; """ display
-( HTML( f"""
+display, HTML @register_cell_magic def mermaid(line: str, cell: str) -> None:
+""" inspired from https://github.com/oruelle/md_mermaid; """ display( HTML
+( f"""
 {cell}
 """ + """
  """ ) ) return None
```

### Comparing `ipython-mermaid-magic-0.3/PKG-INFO` & `ipython-mermaid-magic-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipython-mermaid-magic
-Version: 0.3
+Version: 0.4
 Summary: Cell magic to allow for usage of mermaid notation inside Databricks
 Home-page: https://github.com/sgmarius/ipython-mermaid
 Author: Marius Sandu
 Author-email: marius@ltng-bi.com
 License: MIT
 Download-URL: https://github.com/sgmarius/ipython-mermaid/blob/main/dist/ipython-mermaid-magic-0.3.tar.gz
 Keywords: IPython,Mermaid
```

### Comparing `ipython-mermaid-magic-0.3/ipython_mermaid_magic.egg-info/PKG-INFO` & `ipython-mermaid-magic-0.4/ipython_mermaid_magic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipython-mermaid-magic
-Version: 0.3
+Version: 0.4
 Summary: Cell magic to allow for usage of mermaid notation inside Databricks
 Home-page: https://github.com/sgmarius/ipython-mermaid
 Author: Marius Sandu
 Author-email: marius@ltng-bi.com
 License: MIT
 Download-URL: https://github.com/sgmarius/ipython-mermaid/blob/main/dist/ipython-mermaid-magic-0.3.tar.gz
 Keywords: IPython,Mermaid
```

### Comparing `ipython-mermaid-magic-0.3/setup.py` & `ipython-mermaid-magic-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 from distutils.core import setup
 
 setup(
   name = 'ipython-mermaid-magic',
   packages = ['MermaidMagic'],
-  version = '0.3',
+  version = '0.4',
   license='MIT',
   description = 'Cell magic to allow for usage of mermaid notation inside Databricks',
   author = 'Marius Sandu',
   author_email = 'marius@ltng-bi.com',
   url = 'https://github.com/sgmarius/ipython-mermaid',
   download_url = 'https://github.com/sgmarius/ipython-mermaid/blob/main/dist/ipython-mermaid-magic-0.3.tar.gz',
   keywords = ['IPython', 'Mermaid'],
```

