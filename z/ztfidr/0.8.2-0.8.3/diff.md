# Comparing `tmp/ztfidr-0.8.2.tar.gz` & `tmp/ztfidr-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ztfidr-0.8.2.tar", last modified: Tue May  2 08:50:15 2023, max compression
+gzip compressed data, was "ztfidr-0.8.3.tar", last modified: Tue May  2 12:32:41 2023, max compression
```

## Comparing `ztfidr-0.8.2.tar` & `ztfidr-0.8.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-02 08:50:15.991643 ztfidr-0.8.2/
--rwxrwxrwx   0 rigault   (2358) staff       (20)    11357 2022-04-07 08:06:46.000000 ztfidr-0.8.2/LICENSE
--rw-r--r--   0 rigault   (2358) staff       (20)      234 2023-05-02 08:50:15.991504 ztfidr-0.8.2/PKG-INFO
--rwxrwxrwx   0 rigault   (2358) staff       (20)     2186 2022-04-30 12:26:28.000000 ztfidr-0.8.2/README.md
--rw-r--r--   0 rigault   (2358) staff       (20)       38 2023-05-02 08:50:15.991683 ztfidr-0.8.2/setup.cfg
--rwxrwxrwx   0 rigault   (2358) staff       (20)      609 2023-05-02 08:49:41.000000 ztfidr-0.8.2/setup.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-02 08:50:15.990915 ztfidr-0.8.2/ztfidr/
--rwxrwxrwx   0 rigault   (2358) staff       (20)      127 2023-05-02 08:49:55.000000 ztfidr-0.8.2/ztfidr/__init__.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    14133 2023-04-27 14:14:04.000000 ztfidr-0.8.2/ztfidr/io.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    22044 2023-03-20 14:23:14.000000 ztfidr-0.8.2/ztfidr/lightcurve.py
--rw-r--r--   0 rigault   (2358) staff       (20)    18659 2022-11-06 15:43:33.000000 ztfidr-0.8.2/ztfidr/linefitter.py
--rw-r--r--   0 rigault   (2358) staff       (20)     3215 2023-05-02 07:49:21.000000 ztfidr-0.8.2/ztfidr/plotting.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)     1893 2022-04-07 08:06:50.000000 ztfidr-0.8.2/ztfidr/salt2.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    31042 2023-04-27 13:54:23.000000 ztfidr-0.8.2/ztfidr/sample.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)      629 2022-05-02 15:53:23.000000 ztfidr-0.8.2/ztfidr/script.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)      950 2022-05-18 13:01:28.000000 ztfidr-0.8.2/ztfidr/snid.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    20341 2022-11-15 12:56:31.000000 ztfidr-0.8.2/ztfidr/spectroscopy.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    10043 2022-11-19 14:22:02.000000 ztfidr-0.8.2/ztfidr/target.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    23607 2023-04-28 14:55:40.000000 ztfidr-0.8.2/ztfidr/typing.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)     4034 2023-03-24 07:32:25.000000 ztfidr-0.8.2/ztfidr/utils.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-02 08:50:15.991337 ztfidr-0.8.2/ztfidr.egg-info/
--rwxrwxrwx   0 rigault   (2358) staff       (20)      234 2023-05-02 08:50:15.000000 ztfidr-0.8.2/ztfidr.egg-info/PKG-INFO
--rwxrwxrwx   0 rigault   (2358) staff       (20)      377 2023-05-02 08:50:15.000000 ztfidr-0.8.2/ztfidr.egg-info/SOURCES.txt
--rwxrwxrwx   0 rigault   (2358) staff       (20)        1 2023-05-02 08:50:15.000000 ztfidr-0.8.2/ztfidr.egg-info/dependency_links.txt
--rwxrwxrwx   0 rigault   (2358) staff       (20)        7 2023-05-02 08:50:15.000000 ztfidr-0.8.2/ztfidr.egg-info/top_level.txt
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-02 12:32:41.540930 ztfidr-0.8.3/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    11357 2022-04-07 08:06:46.000000 ztfidr-0.8.3/LICENSE
+-rw-r--r--   0 rigault   (2358) staff       (20)      234 2023-05-02 12:32:41.540800 ztfidr-0.8.3/PKG-INFO
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     2186 2022-04-30 12:26:28.000000 ztfidr-0.8.3/README.md
+-rw-r--r--   0 rigault   (2358) staff       (20)       38 2023-05-02 12:32:41.540967 ztfidr-0.8.3/setup.cfg
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      609 2023-05-02 12:32:23.000000 ztfidr-0.8.3/setup.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-02 12:32:41.540179 ztfidr-0.8.3/ztfidr/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      127 2023-05-02 12:32:20.000000 ztfidr-0.8.3/ztfidr/__init__.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    14128 2023-05-02 12:32:11.000000 ztfidr-0.8.3/ztfidr/io.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    22044 2023-03-20 14:23:14.000000 ztfidr-0.8.3/ztfidr/lightcurve.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    18659 2022-11-06 15:43:33.000000 ztfidr-0.8.3/ztfidr/linefitter.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     3215 2023-05-02 07:49:21.000000 ztfidr-0.8.3/ztfidr/plotting.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     1893 2022-04-07 08:06:50.000000 ztfidr-0.8.3/ztfidr/salt2.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    31042 2023-04-27 13:54:23.000000 ztfidr-0.8.3/ztfidr/sample.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      629 2022-05-02 15:53:23.000000 ztfidr-0.8.3/ztfidr/script.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      950 2022-05-18 13:01:28.000000 ztfidr-0.8.3/ztfidr/snid.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    20341 2022-11-15 12:56:31.000000 ztfidr-0.8.3/ztfidr/spectroscopy.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    10043 2022-11-19 14:22:02.000000 ztfidr-0.8.3/ztfidr/target.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    23339 2023-05-02 10:02:49.000000 ztfidr-0.8.3/ztfidr/typing.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     4034 2023-03-24 07:32:25.000000 ztfidr-0.8.3/ztfidr/utils.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-02 12:32:41.540638 ztfidr-0.8.3/ztfidr.egg-info/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      234 2023-05-02 12:32:41.000000 ztfidr-0.8.3/ztfidr.egg-info/PKG-INFO
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      377 2023-05-02 12:32:41.000000 ztfidr-0.8.3/ztfidr.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rigault   (2358) staff       (20)        1 2023-05-02 12:32:41.000000 ztfidr-0.8.3/ztfidr.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rigault   (2358) staff       (20)        7 2023-05-02 12:32:41.000000 ztfidr-0.8.3/ztfidr.egg-info/top_level.txt
```

### Comparing `ztfidr-0.8.2/LICENSE` & `ztfidr-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ztfidr-0.8.2/README.md` & `ztfidr-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `ztfidr-0.8.2/setup.py` & `ztfidr-0.8.3/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 from distutils.core import setup
 from setuptools import setup, find_packages
 
 
 packages = find_packages()
 
-VERSION = '0.8.2'
+VERSION = '0.8.3'
         
 setup(name='ztfidr',
       version=VERSION,
       description='Tools for ZTF Ia *Internal*DataReleases',
       author='Mickael Rigault',
       author_email='m.rigault@ipnl.in2p3.fr',
       url='https://github.com/MickaelRigault/ztfdr',
```

### Comparing `ztfidr-0.8.2/ztfidr/io.py` & `ztfidr-0.8.3/ztfidr/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,16 +346,15 @@
     if contains is not None:
         glob_format += f"{contains}*"
     if extension is not None:
         glob_format += f"{extension}"
 
     specfiles = glob(os.path.join(IDR_PATH, "spectra", glob_format))
     datafile = pandas.DataFrame(specfiles, columns=["fullpath"])
-    datafile["basename"] = datafile["fullpath"].str.split(
-        "/", expand=True).iloc[:, -1]
+    datafile["basename"] = datafile["fullpath"].str.split(pat="/", expand=True).iloc[:, -1]
     
     specfile = pandas.concat([datafile, parse_filename(datafile["basename"], snidres=snidres)], axis=1)
     
     if add_phase:
         from astropy.time import Time
         if data is None:
             from .sample import get_sample
```

### Comparing `ztfidr-0.8.2/ztfidr/lightcurve.py` & `ztfidr-0.8.3/ztfidr/lightcurve.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.8.2/ztfidr/linefitter.py` & `ztfidr-0.8.3/ztfidr/linefitter.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.8.2/ztfidr/plotting.py` & `ztfidr-0.8.3/ztfidr/plotting.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.8.2/ztfidr/salt2.py` & `ztfidr-0.8.3/ztfidr/salt2.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.8.2/ztfidr/sample.py` & `ztfidr-0.8.3/ztfidr/sample.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.8.2/ztfidr/script.py` & `ztfidr-0.8.3/ztfidr/script.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.8.2/ztfidr/snid.py` & `ztfidr-0.8.3/ztfidr/snid.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.8.2/ztfidr/spectroscopy.py` & `ztfidr-0.8.3/ztfidr/spectroscopy.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.8.2/ztfidr/target.py` & `ztfidr-0.8.3/ztfidr/target.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.8.2/ztfidr/typing.py` & `ztfidr-0.8.3/ztfidr/typing.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,27 +33,14 @@
     """ get the list of spectra flaged as 'to remove' in the typingapp """
     report = Reports()
     rmspec_serie = report.data[(report.data["value"].str.startswith("spec:rm")) &
                                (~report.data["value"].str.contains("none_left"))]
     rmspecs = np.asarray(rmspec_serie["value"].str.replace("spec:rm:","").values, dtype=str)
     return rmspecs
 
-
-
-def merge_classifications(line):
-    """ """
-    # First arbiter
-    if line.arbiter_classification is not np.NaN:
-        return line.arbiter_classification, 'arbiter'
-    # Second master    
-    elif line.master_classification not in ["unclear", "None"]:
-        return line.master_classification, 'master'
-    # Final, auto    
-    return line.auto_classification, "auto"
-
 def parse_classification(line, 
                          min_review=2,
                          min_autotyping=3, 
                          min_generic_typing=3,
                          unclear_limit=0.5,
                          to_unclear_limit=0.75,
                          min_classifications_to_unclear=6,
@@ -346,15 +333,14 @@
         data = data.join(classification)
         return data
     
     def store_typing(self, **kwargs):
         """ """
         data = self.get_typing(**kwargs)
         return data.to_csv( io.get_target_typing(False), sep=" ")
-        
 
     def load_classification(self, **kwargs):
         """ """
         classifications = self.get_classification(**kwargs)
         self._data = self.data.join(classifications, on="target_name", how="outer")
         
     def get_classification(self, min_review=2,
@@ -363,53 +349,54 @@
                                 # Master keys
                                   min_review_master=1,
                                   min_autotyping_master=2,
                                   min_generic_typing_master=3):
         """ """
         # All auto | default
         auto_data = self._get_classification(prefix="auto_",
-                                                 min_review=2, min_autotyping=3, min_generic_typing=3)
+                                                 min_review=min_review, min_autotyping=min_autotyping,
+                                                 min_generic_typing=min_generic_typing)
 
         # Masters
         master = self.get_masterclassification(incl_unclear=False) # do not consider unclear's input
         master_data = master._get_classification(prefix="master_",
                                                       min_review=min_review_master, min_autotyping=min_autotyping_master,
                                                       min_generic_typing=min_generic_typing_master)
         # do not consider master's None or confusing. Only final classification
-        master_data = master_data[~master_data["master_classification"].isin(["None","confusing"])]
 
         # Arbiter
         arbiter_data = Reports.get_arbiters(prefix="arbiter_").groupby("target_name").last()[["arbiter_classification"]] # [[ to get a dataframe
         # - force in data list
         arbiter_data = arbiter_data.loc[ arbiter_data.index.isin(self.target_list) ]
 
         #
         # Now let's join
         #
         # - Default
         cdata = pandas.DataFrame(auto_data["auto_classification"].values, index=auto_data.index, columns=["classification"])
         cdata["class_origin"] = "auto"
         cdata = cdata.join(auto_data)
-
-        # make sure it is full master list
         
         # - add master
+        # do not consider bad cases
+        master_data = master_data[~master_data["master_classification"].isin(["None","confusing", np.NaN])]
+        
         cdata.loc[master_data.index, "classification"] = master_data["master_classification"]
         cdata.loc[master_data.index, "class_origin"] = "master"
         cdata = cdata.join(master_data)
-
+        
         # - add arbiter
         cdata.loc[arbiter_data.index, "classification"] = arbiter_data["arbiter_classification"]
         cdata.loc[arbiter_data.index, "class_origin"] = "arbiter"
         cdata = cdata.join(arbiter_data)
 
         return cdata
         
         
-    def _get_classification(self, prefix="", **kwargs):
+    def _get_classification(self, prefix="", reindex=True, **kwargs):
         # Normal
         class_df = self.get_classification_df()
         d_ = pandas.DataFrame(class_df.apply(parse_classification, axis=1, **kwargs).to_list(),
                                 columns=[f"{prefix}classification",f"{prefix}clevel"], index=class_df.index)
         return d_.reindex(list(self.target_list))
     # -------- #
     # GETTER   #
```

### Comparing `ztfidr-0.8.2/ztfidr/utils.py` & `ztfidr-0.8.3/ztfidr/utils.py`

 * *Files identical despite different names*

