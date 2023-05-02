# Comparing `tmp/ztfidr-0.8.1.tar.gz` & `tmp/ztfidr-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ztfidr-0.8.1.tar", last modified: Mon May  1 19:23:50 2023, max compression
+gzip compressed data, was "ztfidr-0.8.2.tar", last modified: Tue May  2 08:50:15 2023, max compression
```

## Comparing `ztfidr-0.8.1.tar` & `ztfidr-0.8.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-01 19:23:50.530709 ztfidr-0.8.1/
--rwxrwxrwx   0 rigault   (2358) staff       (20)    11357 2022-04-07 08:06:46.000000 ztfidr-0.8.1/LICENSE
--rw-r--r--   0 rigault   (2358) staff       (20)      234 2023-05-01 19:23:50.530579 ztfidr-0.8.1/PKG-INFO
--rwxrwxrwx   0 rigault   (2358) staff       (20)     2186 2022-04-30 12:26:28.000000 ztfidr-0.8.1/README.md
--rw-r--r--   0 rigault   (2358) staff       (20)       38 2023-05-01 19:23:50.530748 ztfidr-0.8.1/setup.cfg
--rwxrwxrwx   0 rigault   (2358) staff       (20)      609 2023-05-01 19:23:26.000000 ztfidr-0.8.1/setup.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-01 19:23:50.529826 ztfidr-0.8.1/ztfidr/
--rwxrwxrwx   0 rigault   (2358) staff       (20)      127 2023-05-01 19:23:31.000000 ztfidr-0.8.1/ztfidr/__init__.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    14133 2023-04-27 14:14:04.000000 ztfidr-0.8.1/ztfidr/io.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    22044 2023-03-20 14:23:14.000000 ztfidr-0.8.1/ztfidr/lightcurve.py
--rw-r--r--   0 rigault   (2358) staff       (20)    18659 2022-11-06 15:43:33.000000 ztfidr-0.8.1/ztfidr/linefitter.py
--rw-r--r--   0 rigault   (2358) staff       (20)     3199 2023-05-01 18:55:51.000000 ztfidr-0.8.1/ztfidr/plotting.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)     1893 2022-04-07 08:06:50.000000 ztfidr-0.8.1/ztfidr/salt2.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    31042 2023-04-27 13:54:23.000000 ztfidr-0.8.1/ztfidr/sample.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)      629 2022-05-02 15:53:23.000000 ztfidr-0.8.1/ztfidr/script.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)      950 2022-05-18 13:01:28.000000 ztfidr-0.8.1/ztfidr/snid.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    20341 2022-11-15 12:56:31.000000 ztfidr-0.8.1/ztfidr/spectroscopy.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    10043 2022-11-19 14:22:02.000000 ztfidr-0.8.1/ztfidr/target.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    23607 2023-04-28 14:55:40.000000 ztfidr-0.8.1/ztfidr/typing.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)     4034 2023-03-24 07:32:25.000000 ztfidr-0.8.1/ztfidr/utils.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-01 19:23:50.530430 ztfidr-0.8.1/ztfidr.egg-info/
--rwxrwxrwx   0 rigault   (2358) staff       (20)      234 2023-05-01 19:23:50.000000 ztfidr-0.8.1/ztfidr.egg-info/PKG-INFO
--rwxrwxrwx   0 rigault   (2358) staff       (20)      377 2023-05-01 19:23:50.000000 ztfidr-0.8.1/ztfidr.egg-info/SOURCES.txt
--rwxrwxrwx   0 rigault   (2358) staff       (20)        1 2023-05-01 19:23:50.000000 ztfidr-0.8.1/ztfidr.egg-info/dependency_links.txt
--rwxrwxrwx   0 rigault   (2358) staff       (20)        7 2023-05-01 19:23:50.000000 ztfidr-0.8.1/ztfidr.egg-info/top_level.txt
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-02 08:50:15.991643 ztfidr-0.8.2/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    11357 2022-04-07 08:06:46.000000 ztfidr-0.8.2/LICENSE
+-rw-r--r--   0 rigault   (2358) staff       (20)      234 2023-05-02 08:50:15.991504 ztfidr-0.8.2/PKG-INFO
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     2186 2022-04-30 12:26:28.000000 ztfidr-0.8.2/README.md
+-rw-r--r--   0 rigault   (2358) staff       (20)       38 2023-05-02 08:50:15.991683 ztfidr-0.8.2/setup.cfg
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      609 2023-05-02 08:49:41.000000 ztfidr-0.8.2/setup.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-02 08:50:15.990915 ztfidr-0.8.2/ztfidr/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      127 2023-05-02 08:49:55.000000 ztfidr-0.8.2/ztfidr/__init__.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    14133 2023-04-27 14:14:04.000000 ztfidr-0.8.2/ztfidr/io.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    22044 2023-03-20 14:23:14.000000 ztfidr-0.8.2/ztfidr/lightcurve.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    18659 2022-11-06 15:43:33.000000 ztfidr-0.8.2/ztfidr/linefitter.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     3215 2023-05-02 07:49:21.000000 ztfidr-0.8.2/ztfidr/plotting.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     1893 2022-04-07 08:06:50.000000 ztfidr-0.8.2/ztfidr/salt2.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    31042 2023-04-27 13:54:23.000000 ztfidr-0.8.2/ztfidr/sample.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      629 2022-05-02 15:53:23.000000 ztfidr-0.8.2/ztfidr/script.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      950 2022-05-18 13:01:28.000000 ztfidr-0.8.2/ztfidr/snid.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    20341 2022-11-15 12:56:31.000000 ztfidr-0.8.2/ztfidr/spectroscopy.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    10043 2022-11-19 14:22:02.000000 ztfidr-0.8.2/ztfidr/target.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    23607 2023-04-28 14:55:40.000000 ztfidr-0.8.2/ztfidr/typing.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     4034 2023-03-24 07:32:25.000000 ztfidr-0.8.2/ztfidr/utils.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-02 08:50:15.991337 ztfidr-0.8.2/ztfidr.egg-info/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      234 2023-05-02 08:50:15.000000 ztfidr-0.8.2/ztfidr.egg-info/PKG-INFO
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      377 2023-05-02 08:50:15.000000 ztfidr-0.8.2/ztfidr.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rigault   (2358) staff       (20)        1 2023-05-02 08:50:15.000000 ztfidr-0.8.2/ztfidr.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rigault   (2358) staff       (20)        7 2023-05-02 08:50:15.000000 ztfidr-0.8.2/ztfidr.egg-info/top_level.txt
```

### Comparing `ztfidr-0.8.1/LICENSE` & `ztfidr-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ztfidr-0.8.1/README.md` & `ztfidr-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `ztfidr-0.8.1/setup.py` & `ztfidr-0.8.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 from distutils.core import setup
 from setuptools import setup, find_packages
 
 
 packages = find_packages()
 
-VERSION = '0.8.1'
+VERSION = '0.8.2'
         
 setup(name='ztfidr',
       version=VERSION,
       description='Tools for ZTF Ia *Internal*DataReleases',
       author='Mickael Rigault',
       author_email='m.rigault@ipnl.in2p3.fr',
       url='https://github.com/MickaelRigault/ztfdr',
```

### Comparing `ztfidr-0.8.1/ztfidr/io.py` & `ztfidr-0.8.2/ztfidr/io.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.8.1/ztfidr/lightcurve.py` & `ztfidr-0.8.2/ztfidr/lightcurve.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.8.1/ztfidr/linefitter.py` & `ztfidr-0.8.2/ztfidr/linefitter.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.8.1/ztfidr/plotting.py` & `ztfidr-0.8.2/ztfidr/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,7 +78,9 @@
     ax.text(rest+30,-2, f'{rest}', fontsize="large",
             color="k", va="center", ha="left")
 
     clearwhich = ["bottom","right","top",] # "bottom"
     [ax.spines[which].set_visible(False) for which in clearwhich]
     ax.set_xticks([])
     ax.set_yticks([1,0,-1,-2], ["SN Ia\nnorm","SN Ia","SN Ia\npeculiar", "Unclear"])
+
+    return fig
```

### Comparing `ztfidr-0.8.1/ztfidr/salt2.py` & `ztfidr-0.8.2/ztfidr/salt2.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.8.1/ztfidr/sample.py` & `ztfidr-0.8.2/ztfidr/sample.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.8.1/ztfidr/script.py` & `ztfidr-0.8.2/ztfidr/script.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.8.1/ztfidr/snid.py` & `ztfidr-0.8.2/ztfidr/snid.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.8.1/ztfidr/spectroscopy.py` & `ztfidr-0.8.2/ztfidr/spectroscopy.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.8.1/ztfidr/target.py` & `ztfidr-0.8.2/ztfidr/target.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.8.1/ztfidr/typing.py` & `ztfidr-0.8.2/ztfidr/typing.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.8.1/ztfidr/utils.py` & `ztfidr-0.8.2/ztfidr/utils.py`

 * *Files identical despite different names*

