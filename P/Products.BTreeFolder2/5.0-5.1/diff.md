# Comparing `tmp/Products.BTreeFolder2-5.0.tar.gz` & `tmp/Products.BTreeFolder2-5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Products.BTreeFolder2-5.0.tar", last modified: Wed Feb  1 08:55:01 2023, max compression
+gzip compressed data, was "Products.BTreeFolder2-5.1.tar", last modified: Tue May  2 06:03:33 2023, max compression
```

## Comparing `Products.BTreeFolder2-5.0.tar` & `Products.BTreeFolder2-5.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-02-01 08:55:01.646974 Products.BTreeFolder2-5.0/
--rw-r--r--   0 jens       (501) staff       (20)     2950 2023-02-01 08:33:59.000000 Products.BTreeFolder2-5.0/CHANGES.rst
--rw-r--r--   0 jens       (501) staff       (20)      805 2023-01-31 16:29:47.000000 Products.BTreeFolder2-5.0/CONTRIBUTING.md
--rw-r--r--   0 jens       (501) staff       (20)       32 2021-11-02 08:51:10.000000 Products.BTreeFolder2-5.0/COPYRIGHT.txt
--rw-r--r--   0 jens       (501) staff       (20)     2070 2021-11-02 08:51:10.000000 Products.BTreeFolder2-5.0/LICENSE.txt
--rw-r--r--   0 jens       (501) staff       (20)      254 2023-02-01 08:33:20.000000 Products.BTreeFolder2-5.0/MANIFEST.in
--rw-r--r--   0 jens       (501) staff       (20)     7262 2023-02-01 08:55:01.647053 Products.BTreeFolder2-5.0/PKG-INFO
--rw-r--r--   0 jens       (501) staff       (20)     3313 2021-11-02 08:51:10.000000 Products.BTreeFolder2-5.0/README.rst
--rw-r--r--   0 jens       (501) staff       (20)      347 2021-11-02 08:51:10.000000 Products.BTreeFolder2-5.0/buildout.cfg
--rw-r--r--   0 jens       (501) staff       (20)      473 2023-02-01 08:55:01.647428 Products.BTreeFolder2-5.0/setup.cfg
--rw-r--r--   0 jens       (501) staff       (20)     2368 2023-02-01 08:34:08.000000 Products.BTreeFolder2-5.0/setup.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-02-01 08:55:01.638596 Products.BTreeFolder2-5.0/src/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-02-01 08:55:01.641654 Products.BTreeFolder2-5.0/src/Products/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-02-01 08:55:01.646411 Products.BTreeFolder2-5.0/src/Products/BTreeFolder2/
--rw-r--r--   0 jens       (501) staff       (20)    18047 2023-02-01 08:33:20.000000 Products.BTreeFolder2-5.0/src/Products/BTreeFolder2/BTreeFolder2.py
--rw-r--r--   0 jens       (501) staff       (20)      938 2021-11-02 08:51:10.000000 Products.BTreeFolder2-5.0/src/Products/BTreeFolder2/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)      179 2021-11-02 08:51:10.000000 Products.BTreeFolder2-5.0/src/Products/BTreeFolder2/btreefolder2.gif
--rw-r--r--   0 jens       (501) staff       (20)     3891 2021-11-02 08:51:10.000000 Products.BTreeFolder2-5.0/src/Products/BTreeFolder2/contents.dtml
--rw-r--r--   0 jens       (501) staff       (20)     1570 2021-11-02 08:51:10.000000 Products.BTreeFolder2-5.0/src/Products/BTreeFolder2/folderAdd.dtml
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-02-01 08:55:01.646806 Products.BTreeFolder2-5.0/src/Products/BTreeFolder2/tests/
--rw-r--r--   0 jens       (501) staff       (20)        0 2021-11-02 08:51:10.000000 Products.BTreeFolder2-5.0/src/Products/BTreeFolder2/tests/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)    10569 2023-02-01 08:33:20.000000 Products.BTreeFolder2-5.0/src/Products/BTreeFolder2/tests/testBTreeFolder2.py
--rw-r--r--   0 jens       (501) staff       (20)       76 2021-11-02 08:51:10.000000 Products.BTreeFolder2-5.0/src/Products/__init__.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-02-01 08:55:01.644090 Products.BTreeFolder2-5.0/src/Products.BTreeFolder2.egg-info/
--rw-r--r--   0 jens       (501) staff       (20)     7262 2023-02-01 08:55:01.000000 Products.BTreeFolder2-5.0/src/Products.BTreeFolder2.egg-info/PKG-INFO
--rw-r--r--   0 jens       (501) staff       (20)      791 2023-02-01 08:55:01.000000 Products.BTreeFolder2-5.0/src/Products.BTreeFolder2.egg-info/SOURCES.txt
--rw-r--r--   0 jens       (501) staff       (20)        1 2023-02-01 08:55:01.000000 Products.BTreeFolder2-5.0/src/Products.BTreeFolder2.egg-info/dependency_links.txt
--rw-r--r--   0 jens       (501) staff       (20)        9 2023-02-01 08:55:01.000000 Products.BTreeFolder2-5.0/src/Products.BTreeFolder2.egg-info/namespace_packages.txt
--rw-r--r--   0 jens       (501) staff       (20)        1 2022-11-01 15:18:32.000000 Products.BTreeFolder2-5.0/src/Products.BTreeFolder2.egg-info/not-zip-safe
--rw-r--r--   0 jens       (501) staff       (20)      137 2023-02-01 08:55:01.000000 Products.BTreeFolder2-5.0/src/Products.BTreeFolder2.egg-info/requires.txt
--rw-r--r--   0 jens       (501) staff       (20)        9 2023-02-01 08:55:01.000000 Products.BTreeFolder2-5.0/src/Products.BTreeFolder2.egg-info/top_level.txt
--rw-r--r--   0 jens       (501) staff       (20)     1683 2023-02-01 08:33:20.000000 Products.BTreeFolder2-5.0/tox.ini
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-05-02 06:03:33.635602 Products.BTreeFolder2-5.1/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3174 2023-05-02 06:03:33.000000 Products.BTreeFolder2-5.1/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      805 2023-05-02 06:03:33.000000 Products.BTreeFolder2-5.1/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-05-02 06:03:33.000000 Products.BTreeFolder2-5.1/COPYRIGHT.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2023-05-02 06:03:33.000000 Products.BTreeFolder2-5.1/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      254 2023-05-02 06:03:33.000000 Products.BTreeFolder2-5.1/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7486 2023-05-02 06:03:33.635715 Products.BTreeFolder2-5.1/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3313 2023-05-02 06:03:33.000000 Products.BTreeFolder2-5.1/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      347 2023-05-02 06:03:33.000000 Products.BTreeFolder2-5.1/buildout.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)      473 2023-05-02 06:03:33.636119 Products.BTreeFolder2-5.1/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2365 2023-05-02 06:03:33.000000 Products.BTreeFolder2-5.1/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-05-02 06:03:33.630866 Products.BTreeFolder2-5.1/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-05-02 06:03:33.633073 Products.BTreeFolder2-5.1/src/Products/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-05-02 06:03:33.635180 Products.BTreeFolder2-5.1/src/Products/BTreeFolder2/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    18047 2023-05-02 06:03:33.000000 Products.BTreeFolder2-5.1/src/Products/BTreeFolder2/BTreeFolder2.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      938 2023-05-02 06:03:33.000000 Products.BTreeFolder2-5.1/src/Products/BTreeFolder2/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      179 2023-05-02 06:03:33.000000 Products.BTreeFolder2-5.1/src/Products/BTreeFolder2/btreefolder2.gif
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3945 2023-05-02 06:03:33.000000 Products.BTreeFolder2-5.1/src/Products/BTreeFolder2/contents.dtml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1570 2023-05-02 06:03:33.000000 Products.BTreeFolder2-5.1/src/Products/BTreeFolder2/folderAdd.dtml
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-05-02 06:03:33.635457 Products.BTreeFolder2-5.1/src/Products/BTreeFolder2/tests/
+-rw-r--r--   0 m.howitz   (502) staff       (20)        0 2023-05-02 06:03:33.000000 Products.BTreeFolder2-5.1/src/Products/BTreeFolder2/tests/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    10569 2023-05-02 06:03:33.000000 Products.BTreeFolder2-5.1/src/Products/BTreeFolder2/tests/testBTreeFolder2.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)       76 2023-05-02 06:03:33.000000 Products.BTreeFolder2-5.1/src/Products/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-05-02 06:03:33.634358 Products.BTreeFolder2-5.1/src/Products.BTreeFolder2.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7486 2023-05-02 06:03:33.000000 Products.BTreeFolder2-5.1/src/Products.BTreeFolder2.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)      791 2023-05-02 06:03:33.000000 Products.BTreeFolder2-5.1/src/Products.BTreeFolder2.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-05-02 06:03:33.000000 Products.BTreeFolder2-5.1/src/Products.BTreeFolder2.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        9 2023-05-02 06:03:33.000000 Products.BTreeFolder2-5.1/src/Products.BTreeFolder2.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-05-02 06:03:33.000000 Products.BTreeFolder2-5.1/src/Products.BTreeFolder2.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)      134 2023-05-02 06:03:33.000000 Products.BTreeFolder2-5.1/src/Products.BTreeFolder2.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        9 2023-05-02 06:03:33.000000 Products.BTreeFolder2-5.1/src/Products.BTreeFolder2.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1683 2023-05-02 06:03:33.000000 Products.BTreeFolder2-5.1/tox.ini
```

### Comparing `Products.BTreeFolder2-5.0/CHANGES.rst` & `Products.BTreeFolder2-5.1/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Changelog
 =========
 
+5.1 (2023-05-02)
+----------------
+
+- Depend on ``Zope`` instead of ``Zope2``.
+
+- Add a confirmation prompt on ``Delete All Objects`` button.
+  (see `#9 <https://github.com/zopefoundation/Products.BTreeFolder2/issues/9>`_)
+
+
 5.0 (2023-02-01)
 ----------------
 
 - Drop support for Python 2.7, 3.5, 3.6.
 
 
 4.4 (2022-12-16)
```

### Comparing `Products.BTreeFolder2-5.0/CONTRIBUTING.md` & `Products.BTreeFolder2-5.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `Products.BTreeFolder2-5.0/LICENSE.txt` & `Products.BTreeFolder2-5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Products.BTreeFolder2-5.0/PKG-INFO` & `Products.BTreeFolder2-5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Products.BTreeFolder2
-Version: 5.0
+Version: 5.1
 Summary: A BTree based implementation for Zope's OFS.
 Home-page: https://github.com/zopefoundation/Products.BTreeFolder2
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Classifier: Development Status :: 6 - Mature
 Classifier: Environment :: Web Environment
@@ -102,14 +102,23 @@
 that the superValues() method does not return any items.  To implement
 the method in the way the Zope codebase expects would undermine the
 performance benefits gained by using BTreeFolder2.
 
 Changelog
 =========
 
+5.1 (2023-05-02)
+----------------
+
+- Depend on ``Zope`` instead of ``Zope2``.
+
+- Add a confirmation prompt on ``Delete All Objects`` button.
+  (see `#9 <https://github.com/zopefoundation/Products.BTreeFolder2/issues/9>`_)
+
+
 5.0 (2023-02-01)
 ----------------
 
 - Drop support for Python 2.7, 3.5, 3.6.
 
 
 4.4 (2022-12-16)
```

### Comparing `Products.BTreeFolder2-5.0/README.rst` & `Products.BTreeFolder2-5.1/README.rst`

 * *Files identical despite different names*

### Comparing `Products.BTreeFolder2-5.0/setup.py` & `Products.BTreeFolder2-5.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ##############################################################################
 
 from setuptools import find_packages
 from setuptools import setup
 
 
 setup(name='Products.BTreeFolder2',
-      version='5.0',
+      version='5.1',
       url='https://github.com/zopefoundation/Products.BTreeFolder2',
       license='ZPL 2.1',
       description="A BTree based implementation for Zope's OFS.",
       author='Zope Foundation and Contributors',
       author_email='zope-dev@zope.dev',
       long_description=(open('README.rst').read()
                         + '\n'
@@ -49,15 +49,15 @@
       install_requires=[
           'setuptools',
           'AccessControl',
           'Acquisition',
           'BTrees',
           'ExtensionClass>=4.1a1',
           'Persistence',
-          'Zope2 >= 4.0a5',
+          'Zope >= 4.0',
           'zope.container',
           'zope.event',
           'zope.lifecycleevent',
       ],
       include_package_data=True,
       zip_safe=False,
       )
```

### Comparing `Products.BTreeFolder2-5.0/src/Products/BTreeFolder2/BTreeFolder2.py` & `Products.BTreeFolder2-5.1/src/Products/BTreeFolder2/BTreeFolder2.py`

 * *Files identical despite different names*

### Comparing `Products.BTreeFolder2-5.0/src/Products/BTreeFolder2/__init__.py` & `Products.BTreeFolder2-5.1/src/Products/BTreeFolder2/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.BTreeFolder2-5.0/src/Products/BTreeFolder2/contents.dtml` & `Products.BTreeFolder2-5.1/src/Products/BTreeFolder2/contents.dtml`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
    value="Paste" />
   </dtml-if>
   </dtml-unless>
   <dtml-if "_.SecurityCheckPermission('Delete objects',this())">
   <input class="form-element" type="submit" name="manage_delObjects:method"
    value="Delete" />
   <input class="form-element" type="submit" name="manage_delAllObjects:method"
-   value="Delete All Objects" />
+   value="Delete All Objects" onClick="return confirm('Really delete all objects?')"/>
   </dtml-if>
   <dtml-if "_.SecurityCheckPermission('Import/Export objects', this())">
   <input class="form-element" type="submit"
    name="manage_importExportForm:method"
    value="Import/Export" />
   </dtml-if>
 <script type="text/javascript">
```

### Comparing `Products.BTreeFolder2-5.0/src/Products/BTreeFolder2/folderAdd.dtml` & `Products.BTreeFolder2-5.1/src/Products/BTreeFolder2/folderAdd.dtml`

 * *Files identical despite different names*

### Comparing `Products.BTreeFolder2-5.0/src/Products/BTreeFolder2/tests/testBTreeFolder2.py` & `Products.BTreeFolder2-5.1/src/Products/BTreeFolder2/tests/testBTreeFolder2.py`

 * *Files identical despite different names*

### Comparing `Products.BTreeFolder2-5.0/src/Products.BTreeFolder2.egg-info/PKG-INFO` & `Products.BTreeFolder2-5.1/src/Products.BTreeFolder2.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Products.BTreeFolder2
-Version: 5.0
+Version: 5.1
 Summary: A BTree based implementation for Zope's OFS.
 Home-page: https://github.com/zopefoundation/Products.BTreeFolder2
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Classifier: Development Status :: 6 - Mature
 Classifier: Environment :: Web Environment
@@ -102,14 +102,23 @@
 that the superValues() method does not return any items.  To implement
 the method in the way the Zope codebase expects would undermine the
 performance benefits gained by using BTreeFolder2.
 
 Changelog
 =========
 
+5.1 (2023-05-02)
+----------------
+
+- Depend on ``Zope`` instead of ``Zope2``.
+
+- Add a confirmation prompt on ``Delete All Objects`` button.
+  (see `#9 <https://github.com/zopefoundation/Products.BTreeFolder2/issues/9>`_)
+
+
 5.0 (2023-02-01)
 ----------------
 
 - Drop support for Python 2.7, 3.5, 3.6.
 
 
 4.4 (2022-12-16)
```

### Comparing `Products.BTreeFolder2-5.0/src/Products.BTreeFolder2.egg-info/SOURCES.txt` & `Products.BTreeFolder2-5.1/src/Products.BTreeFolder2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Products.BTreeFolder2-5.0/tox.ini` & `Products.BTreeFolder2-5.1/tox.ini`

 * *Files identical despite different names*

