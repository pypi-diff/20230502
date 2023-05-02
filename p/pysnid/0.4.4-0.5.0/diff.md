# Comparing `tmp/pysnid-0.4.4.tar.gz` & `tmp/pysnid-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysnid-0.4.4.tar", last modified: Tue May  2 13:12:44 2023, max compression
+gzip compressed data, was "pysnid-0.5.0.tar", last modified: Tue May  2 13:22:25 2023, max compression
```

## Comparing `pysnid-0.4.4.tar` & `pysnid-0.5.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-02 13:12:44.563648 pysnid-0.4.4/
--rwxrwxrwx   0 rigault   (2358) staff       (20)    35149 2021-10-16 13:03:13.000000 pysnid-0.4.4/LICENSE
--rw-r--r--   0 rigault   (2358) staff       (20)      222 2023-05-02 13:12:44.563509 pysnid-0.4.4/PKG-INFO
--rwxrwxrwx   0 rigault   (2358) staff       (20)     1297 2021-10-18 13:27:24.000000 pysnid-0.4.4/README.md
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-02 13:12:44.562762 pysnid-0.4.4/pysnid/
--rwxrwxrwx   0 rigault   (2358) staff       (20)       49 2023-05-02 13:12:26.000000 pysnid-0.4.4/pysnid/__init__.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    34365 2023-05-02 13:11:52.000000 pysnid-0.4.4/pysnid/snid.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)     3780 2022-02-09 13:55:29.000000 pysnid-0.4.4/pysnid/tools.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-02 13:12:44.563360 pysnid-0.4.4/pysnid.egg-info/
--rwxrwxrwx   0 rigault   (2358) staff       (20)      222 2023-05-02 13:12:44.000000 pysnid-0.4.4/pysnid.egg-info/PKG-INFO
--rwxrwxrwx   0 rigault   (2358) staff       (20)      196 2023-05-02 13:12:44.000000 pysnid-0.4.4/pysnid.egg-info/SOURCES.txt
--rwxrwxrwx   0 rigault   (2358) staff       (20)        1 2023-05-02 13:12:44.000000 pysnid-0.4.4/pysnid.egg-info/dependency_links.txt
--rwxrwxrwx   0 rigault   (2358) staff       (20)        7 2023-05-02 13:12:44.000000 pysnid-0.4.4/pysnid.egg-info/top_level.txt
--rw-r--r--   0 rigault   (2358) staff       (20)       38 2023-05-02 13:12:44.563693 pysnid-0.4.4/setup.cfg
--rwxrwxrwx   0 rigault   (2358) staff       (20)      670 2023-05-02 13:12:32.000000 pysnid-0.4.4/setup.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-02 13:22:25.453347 pysnid-0.5.0/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    35149 2021-10-16 13:03:13.000000 pysnid-0.5.0/LICENSE
+-rw-r--r--   0 rigault   (2358) staff       (20)      222 2023-05-02 13:22:25.453225 pysnid-0.5.0/PKG-INFO
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     1297 2021-10-18 13:27:24.000000 pysnid-0.5.0/README.md
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-02 13:22:25.452648 pysnid-0.5.0/pysnid/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)       49 2023-05-02 13:21:11.000000 pysnid-0.5.0/pysnid/__init__.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    34362 2023-05-02 13:20:41.000000 pysnid-0.5.0/pysnid/snid.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     3780 2022-02-09 13:55:29.000000 pysnid-0.5.0/pysnid/tools.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-02 13:22:25.453086 pysnid-0.5.0/pysnid.egg-info/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      222 2023-05-02 13:22:25.000000 pysnid-0.5.0/pysnid.egg-info/PKG-INFO
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      196 2023-05-02 13:22:25.000000 pysnid-0.5.0/pysnid.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rigault   (2358) staff       (20)        1 2023-05-02 13:22:25.000000 pysnid-0.5.0/pysnid.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rigault   (2358) staff       (20)        7 2023-05-02 13:22:25.000000 pysnid-0.5.0/pysnid.egg-info/top_level.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)       38 2023-05-02 13:22:25.453386 pysnid-0.5.0/setup.cfg
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      670 2023-05-02 13:21:17.000000 pysnid-0.5.0/setup.py
```

### Comparing `pysnid-0.4.4/LICENSE` & `pysnid-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysnid-0.4.4/README.md` & `pysnid-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pysnid-0.4.4/pysnid/snid.py` & `pysnid-0.5.0/pysnid/snid.py`

 * *Files 0% similar despite different names*

```diff
@@ -517,17 +517,17 @@
             
         res = self.get_results(rlap_range=[min_rlap,None], **resprop).iloc[:nfirst]
         #
         # - Rankind
         #
         types_values = res.reset_index().groupby("type")["no."].apply(list).sort_values()
         # Loop over groups
-        for i_,(name, nos) in enumerate(types_values.to_frame().items()):
+        for i_, (name, nos) in enumerate(types_values.items()):
             color = f"C{i_}"
-            for j_, v_ in enumerate(np.asarray(nos, dtype="int")):
+            for j_, v_ in enumerate(np.asarray( list(nos), dtype="int")):
                 if j_==0:
                     label= f"{name}: #{v_}"  
                 else:
                     label= "_no_legend_"
 
                 ax.axvspan(v_-1,v_, facecolor=color, edgecolor="0.7", lw=0.5, label=label)
                 if j_==0:
```

### Comparing `pysnid-0.4.4/pysnid/tools.py` & `pysnid-0.5.0/pysnid/tools.py`

 * *Files identical despite different names*

### Comparing `pysnid-0.4.4/setup.py` & `pysnid-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from setuptools import setup, find_packages
 
 
 packages = find_packages()
 print(f"packages to be installed: {packages}")
 
 CODENAME = "pysnid"
-VERSION = '0.4.4'
+VERSION = '0.5.0'
         
 setup(name=CODENAME,
       version=VERSION,
       description='Tools to run and read SNID',
       author='Mickael Rigault',
       author_email='m.rigault@ipnl.in2p3.fr',
       url=f'https://github.com/MickaelRigault/{CODENAME}',
```

