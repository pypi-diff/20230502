# Comparing `tmp/skysurvey-0.3.8.tar.gz` & `tmp/skysurvey-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skysurvey-0.3.8.tar", last modified: Mon Dec 19 09:18:01 2022, max compression
+gzip compressed data, was "skysurvey-0.3.9.tar", last modified: Tue Dec 20 19:53:35 2022, max compression
```

## Comparing `skysurvey-0.3.8.tar` & `skysurvey-0.3.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2022-12-19 09:18:01.802768 skysurvey-0.3.8/
--rw-r--r--   0 rigault   (2358) staff       (20)    11357 2022-08-10 14:40:58.000000 skysurvey-0.3.8/LICENSE
--rw-r--r--   0 rigault   (2358) staff       (20)      257 2022-12-19 09:18:01.802657 skysurvey-0.3.8/PKG-INFO
--rw-r--r--   0 rigault   (2358) staff       (20)     2333 2022-09-14 19:00:29.000000 skysurvey-0.3.8/README.md
--rw-r--r--   0 rigault   (2358) staff       (20)       38 2022-12-19 09:18:01.802805 skysurvey-0.3.8/setup.cfg
--rw-r--r--   0 rigault   (2358) staff       (20)      632 2022-12-19 09:17:53.000000 skysurvey-0.3.8/setup.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2022-12-19 09:18:01.799729 skysurvey-0.3.8/skysurvey/
--rw-r--r--   0 rigault   (2358) staff       (20)       92 2022-12-19 09:17:49.000000 skysurvey-0.3.8/skysurvey/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)      398 2022-08-16 14:00:03.000000 skysurvey-0.3.8/skysurvey/config.py
--rw-r--r--   0 rigault   (2358) staff       (20)     7196 2022-09-29 17:14:54.000000 skysurvey-0.3.8/skysurvey/dag.py
--rw-r--r--   0 rigault   (2358) staff       (20)    19071 2022-12-17 16:54:37.000000 skysurvey-0.3.8/skysurvey/dataset.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2022-12-19 09:18:01.800657 skysurvey-0.3.8/skysurvey/survey/
--rw-r--r--   0 rigault   (2358) staff       (20)      101 2022-09-17 12:56:09.000000 skysurvey-0.3.8/skysurvey/survey/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)     8111 2022-12-17 16:44:50.000000 skysurvey-0.3.8/skysurvey/survey/core.py
--rw-r--r--   0 rigault   (2358) staff       (20)    10972 2022-12-17 16:46:15.000000 skysurvey-0.3.8/skysurvey/survey/healpix.py
--rw-r--r--   0 rigault   (2358) staff       (20)     5306 2022-12-17 16:44:36.000000 skysurvey-0.3.8/skysurvey/survey/polygon.py
--rw-r--r--   0 rigault   (2358) staff       (20)     1140 2022-12-19 09:16:48.000000 skysurvey-0.3.8/skysurvey/survey/ztf.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2022-12-19 09:18:01.802500 skysurvey-0.3.8/skysurvey/target/
--rw-r--r--   0 rigault   (2358) staff       (20)       67 2022-09-29 07:34:56.000000 skysurvey-0.3.8/skysurvey/target/__init__.py
--rw-r--r--   0 rigault   (2358) staff       (20)     8328 2022-10-06 11:54:26.000000 skysurvey-0.3.8/skysurvey/target/collection.py
--rw-r--r--   0 rigault   (2358) staff       (20)    22876 2022-12-14 09:25:25.000000 skysurvey-0.3.8/skysurvey/target/core.py
--rw-r--r--   0 rigault   (2358) staff       (20)      391 2022-10-06 08:31:16.000000 skysurvey-0.3.8/skysurvey/target/environments.py
--rw-r--r--   0 rigault   (2358) staff       (20)      165 2022-09-17 13:52:22.000000 skysurvey-0.3.8/skysurvey/target/kilonova.py
--rw-r--r--   0 rigault   (2358) staff       (20)     9415 2022-10-06 08:36:21.000000 skysurvey-0.3.8/skysurvey/target/snia.py
--rw-r--r--   0 rigault   (2358) staff       (20)     1927 2022-10-07 13:10:54.000000 skysurvey-0.3.8/skysurvey/target/snii.py
--rw-r--r--   0 rigault   (2358) staff       (20)      606 2022-09-26 14:53:44.000000 skysurvey-0.3.8/skysurvey/target/stars.py
--rw-r--r--   0 rigault   (2358) staff       (20)     2261 2022-10-06 11:55:05.000000 skysurvey-0.3.8/skysurvey/target/timeserie.py
--rw-r--r--   0 rigault   (2358) staff       (20)    15523 2022-12-07 13:53:25.000000 skysurvey-0.3.8/skysurvey/template.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2022-12-19 09:18:01.800155 skysurvey-0.3.8/skysurvey.egg-info/
--rw-r--r--   0 rigault   (2358) staff       (20)      257 2022-12-19 09:18:01.000000 skysurvey-0.3.8/skysurvey.egg-info/PKG-INFO
--rw-r--r--   0 rigault   (2358) staff       (20)      647 2022-12-19 09:18:01.000000 skysurvey-0.3.8/skysurvey.egg-info/SOURCES.txt
--rw-r--r--   0 rigault   (2358) staff       (20)        1 2022-12-19 09:18:01.000000 skysurvey-0.3.8/skysurvey.egg-info/dependency_links.txt
--rw-r--r--   0 rigault   (2358) staff       (20)       10 2022-12-19 09:18:01.000000 skysurvey-0.3.8/skysurvey.egg-info/top_level.txt
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2022-12-20 19:53:35.475514 skysurvey-0.3.9/
+-rw-r--r--   0 rigault   (2358) staff       (20)    11357 2022-08-10 14:40:58.000000 skysurvey-0.3.9/LICENSE
+-rw-r--r--   0 rigault   (2358) staff       (20)      257 2022-12-20 19:53:35.475378 skysurvey-0.3.9/PKG-INFO
+-rw-r--r--   0 rigault   (2358) staff       (20)     2333 2022-09-14 19:00:29.000000 skysurvey-0.3.9/README.md
+-rw-r--r--   0 rigault   (2358) staff       (20)       38 2022-12-20 19:53:35.475554 skysurvey-0.3.9/setup.cfg
+-rw-r--r--   0 rigault   (2358) staff       (20)      632 2022-12-20 19:53:02.000000 skysurvey-0.3.9/setup.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2022-12-20 19:53:35.471337 skysurvey-0.3.9/skysurvey/
+-rw-r--r--   0 rigault   (2358) staff       (20)       92 2022-12-20 19:52:56.000000 skysurvey-0.3.9/skysurvey/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      398 2022-08-16 14:00:03.000000 skysurvey-0.3.9/skysurvey/config.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     7196 2022-09-29 17:14:54.000000 skysurvey-0.3.9/skysurvey/dag.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    19776 2022-12-20 19:50:41.000000 skysurvey-0.3.9/skysurvey/dataset.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2022-12-20 19:53:35.473076 skysurvey-0.3.9/skysurvey/survey/
+-rw-r--r--   0 rigault   (2358) staff       (20)      101 2022-09-17 12:56:09.000000 skysurvey-0.3.9/skysurvey/survey/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     8363 2022-12-19 09:32:29.000000 skysurvey-0.3.9/skysurvey/survey/core.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    10972 2022-12-17 16:46:15.000000 skysurvey-0.3.9/skysurvey/survey/healpix.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     5306 2022-12-17 16:44:36.000000 skysurvey-0.3.9/skysurvey/survey/polygon.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     1698 2022-12-20 11:13:58.000000 skysurvey-0.3.9/skysurvey/survey/ztf.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2022-12-20 19:53:35.475096 skysurvey-0.3.9/skysurvey/target/
+-rw-r--r--   0 rigault   (2358) staff       (20)       67 2022-09-29 07:34:56.000000 skysurvey-0.3.9/skysurvey/target/__init__.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     8328 2022-10-06 11:54:26.000000 skysurvey-0.3.9/skysurvey/target/collection.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    23105 2022-12-20 19:21:14.000000 skysurvey-0.3.9/skysurvey/target/core.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      391 2022-10-06 08:31:16.000000 skysurvey-0.3.9/skysurvey/target/environments.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      165 2022-09-17 13:52:22.000000 skysurvey-0.3.9/skysurvey/target/kilonova.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     9415 2022-10-06 08:36:21.000000 skysurvey-0.3.9/skysurvey/target/snia.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     1927 2022-10-07 13:10:54.000000 skysurvey-0.3.9/skysurvey/target/snii.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      606 2022-09-26 14:53:44.000000 skysurvey-0.3.9/skysurvey/target/stars.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     2261 2022-10-06 11:55:05.000000 skysurvey-0.3.9/skysurvey/target/timeserie.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    15523 2022-12-07 13:53:25.000000 skysurvey-0.3.9/skysurvey/template.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2022-12-20 19:53:35.471973 skysurvey-0.3.9/skysurvey.egg-info/
+-rw-r--r--   0 rigault   (2358) staff       (20)      257 2022-12-20 19:53:35.000000 skysurvey-0.3.9/skysurvey.egg-info/PKG-INFO
+-rw-r--r--   0 rigault   (2358) staff       (20)      647 2022-12-20 19:53:35.000000 skysurvey-0.3.9/skysurvey.egg-info/SOURCES.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)        1 2022-12-20 19:53:35.000000 skysurvey-0.3.9/skysurvey.egg-info/dependency_links.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)       10 2022-12-20 19:53:35.000000 skysurvey-0.3.9/skysurvey.egg-info/top_level.txt
```

### Comparing `skysurvey-0.3.8/LICENSE` & `skysurvey-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `skysurvey-0.3.8/README.md` & `skysurvey-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `skysurvey-0.3.8/setup.py` & `skysurvey-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 from distutils.core import setup
 from setuptools import setup, find_packages
 
 
 packages = find_packages()
 
-VERSION = '0.3.8'
+VERSION = '0.3.9'
         
 setup(name='skysurvey',
       version=VERSION,
       description='Simulating Transient in the sky and how to observe them',
       author='Mickael Rigault',
       author_email='m.rigault@ipnl.in2p3.fr',
       url='https://github.com/MickaelRigault/skysurvey',
```

### Comparing `skysurvey-0.3.8/skysurvey/dag.py` & `skysurvey-0.3.9/skysurvey/dag.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.3.8/skysurvey/dataset.py` & `skysurvey-0.3.9/skysurvey/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     list_of_parameters = [p_.to_dict() for i_,p_ in parameters.iterrows()] # sncosmo format
     
     # realize LC
     list_of_observations = sncosmo.realize_lcs(sncosmo_obs, template, list_of_parameters)
     if len(list_of_observations) == 0:
         return None
     
-    return pandas.concat([l.to_pandas() for l in list_of_observations],  keys=parameters.index)
+    return pandas.concat([l.to_pandas().set_index(observations.index) for l in list_of_observations],  keys=parameters.index)
 
 
 
 # ================== #
 #                    #
 #    DataSet         #
 #                    #
@@ -265,14 +265,39 @@
             ndetection = data.reset_index().set_index(["level_0","level_1","band"]).groupby(level=[0,2])["detected"].sum()
         else:
             ndetection = data.groupby(level=0)["detected"].sum()
 
             
         return ndetection
 
+
+    def get_target_lightcurve(self, index, detection_only=False, detlimit=5.):
+        """ get the observation of the given target.
+        
+        = short cut to self.data.xs(index) = 
+
+        Parameters
+        ----------
+        detection_only: bool
+            only the detected points of the lightcurves 
+
+        detlimit: float
+            definition of a detection (flux/fluxerr>=detlimit)
+
+        Returns
+        -------
+        pandas.DataFrame
+            the lightcurve
+
+        """
+        data = self.data.xs(index)
+        if detection_only:
+            data = data[data["flux"]/data["fluxerr"]>=detlimit]
+
+        return data
     
     # -------- #
     #  FIT     #
     # -------- #
     def fit_lightcurves(self, source, index=None,
                            use_dask=True,
                            phase_fitrange=[-50,200],
@@ -440,15 +465,15 @@
         
         if format_time:
             from astropy.time import Time
         if index is None:
             index = np.random.choice(self.obs_index)
 
         # Data
-        obs_ = self.data.xs(index).copy()
+        obs_ = self.get_target_lightcurve(index)
         if phase_window is not None:
             t0 = self.targets.data["t0"].loc[index]
             phase_window = np.asarray(phase_window)+t0
             obs_ = obs_[obs_["time"].between(*phase_window)]
 
         coef = 10 ** (-(obs_["zp"] - zp) / 2.5)
         obs_["flux_zp"] = obs_["flux"] * coef
@@ -496,14 +521,15 @@
         dfieldids_ = survey.radec_to_fieldid(targets.data[["ra","dec"]])
         # merge conserves the dtypes of fieldids, not join.
         targets_data = targets.data.merge(dfieldids_, left_index=True, right_index=True)
 
 
         # index them per fieldids names.
         target_indexed = targets_data.reset_index().set_index(["index"]+survey.fieldids.names)
+        
         # best performance when passing by one groupby calls rather than indexing and xs()
         gsurvey_indexed = survey.data[["mjd","band","skynoise","gain", "zp"]+survey.fieldids.names].groupby(survey.fieldids.names)
 
         # get list of 
         # This works for any size of fieldids
         names = survey.fieldids.names
         levels = np.arange(1, len(names)+1).tolist()
@@ -526,14 +552,15 @@
 
             # get() returns copy
             sncosmo_model = template.get(**template_prop)  
             # survey matching the input fieldids row
 
             # Taking the data we need
             this_target = target_indexed.xs(index_, level=levels)[template_columns]
+            
             # Get the lightcurves
             this_lc = get_obsdata(sncosmo_model, this_survey, this_target)
             this_lc[names] = index_
 
             return this_lc
 
         lc_out = [realize_index_lc(index_) for index_ in fieldids_indexes]
```

### Comparing `skysurvey-0.3.8/skysurvey/survey/core.py` & `skysurvey-0.3.9/skysurvey/survey/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,24 +164,26 @@
 
         if fieldid is not None:
             data = data[data["fieldid"].isin( np.atleast_1d(fieldid) )]
         
         if ax is None:
             import matplotlib.pyplot as plt
             fig = plt.figure(figsize=(9,2))
-            ax = fig.add_axes([0.075, 0.3, 0.85, 0.6])
+            ax = fig.add_axes([0.075, 0.2, 0.85, 0.6])
         else:
             fig = ax.figure
 
         if not perband:
             nobs = data.groupby(exposure_key).first().groupby("day").size()
+            max_obs = nobs.max()
             all_days = nobs.index
             nbands = 1
         else:
             nobs = data.groupby(exposure_key).first().groupby(["day", band_key]).size()
+            max_obs = nobs.groupby(level=0).sum().max()
             all_days = nobs.index.levels[0]
             if bands is None:
                 bands = nobs.index.levels[1]
             nbands = len(bands)
 
         times = Time(all_days.astype( float ), format="mjd").datetime
 
@@ -213,15 +215,15 @@
         [ax.spines[which].set_visible(False) for which in clearwhich]
         ax.tick_params(axis="y", labelsize="small", 
                                    labelcolor="0.7", color="0.7")
 
         ax.grid(axis="y", lw=0.5, color='0.7', zorder=1, alpha=0.5)
         ax.set_ylabel("exposures per day", color="0.7", fontsize="small")
 
-        ax.set_ylim(ymin=0, ymax=np.round(nobs.max()*1.05,decimals=-1) )
+        ax.set_ylim(ymin=0, ymax=np.round(max_obs*1.05,decimals=-1) )
         print(nobs.max())
         if legend:
             ax.legend(loc=[0,1], ncol=nbands, frameon=False, fontsize="small")
             
         return fig
     
     # ============== #
@@ -249,7 +251,13 @@
             
         return self._nfields
     
     @property
     def of_type(self):
         """ kind of survey that is """
         return str(type(self)).split("'")[-2].split(".")[-1]
+
+    @property
+    def date_range(self):
+        """ first and last date of the survey """
+        return np.min(self.data["mjd"]), np.max(self.data["mjd"])
+
```

### Comparing `skysurvey-0.3.8/skysurvey/survey/healpix.py` & `skysurvey-0.3.9/skysurvey/survey/healpix.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.3.8/skysurvey/survey/polygon.py` & `skysurvey-0.3.9/skysurvey/survey/polygon.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.3.8/skysurvey/survey/ztf.py` & `skysurvey-0.3.9/skysurvey/survey/ztf.py`

 * *Files 20% similar despite different names*

```diff
@@ -34,7 +34,25 @@
         fields
         """
         this = cls(level=level)
         this.draw_random(size, bands,  
                         mjd_range, skynoise_range, 
                         inplace=True, **kwargs)
         return this
+
+
+    def show(self, data=None, **kwargs):
+        """ shows the sky coverage 
+
+        **kwargs goes to ztffields.skyplot_fields
+        """
+        import ztffields
+        if data is None:
+            data = self.data
+        
+        datamain = data[data["fieldid"]<1000] # main grid
+        fieldid_s = datamain.groupby("expid").first().groupby("fieldid").size()
+
+        fig = ztffields.skyplot_fields(fieldid_s, 
+                                        label="number of observations (main grid)",
+                                           **kwargs)
+
```

### Comparing `skysurvey-0.3.8/skysurvey/target/collection.py` & `skysurvey-0.3.9/skysurvey/target/collection.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.3.8/skysurvey/target/core.py` & `skysurvey-0.3.9/skysurvey/target/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,25 @@
         class instance
             not implemented yet
         """
         raise NotImplementedError("from_setting is not Implemented ")
 
 
     @classmethod
+    def from_data(cls, data, template=None):
+        """ """
+        this = cls()
+
+        if template is not None:
+            self.set_template(template)
+
+        this._data = data
+        return this
+        
+    @classmethod
     def from_draw(cls, size=None, model=None, template=None,
                       zmax=None, tstart=None, tstop=None,
                       nyears=None,
                       **kwargs):
         """ loads the instance from a random draw of targets given the model 
 
         Parameters
```

### Comparing `skysurvey-0.3.8/skysurvey/target/snia.py` & `skysurvey-0.3.9/skysurvey/target/snia.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.3.8/skysurvey/target/snii.py` & `skysurvey-0.3.9/skysurvey/target/snii.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.3.8/skysurvey/target/stars.py` & `skysurvey-0.3.9/skysurvey/target/stars.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.3.8/skysurvey/target/timeserie.py` & `skysurvey-0.3.9/skysurvey/target/timeserie.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.3.8/skysurvey/template.py` & `skysurvey-0.3.9/skysurvey/template.py`

 * *Files identical despite different names*

### Comparing `skysurvey-0.3.8/skysurvey.egg-info/SOURCES.txt` & `skysurvey-0.3.9/skysurvey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

