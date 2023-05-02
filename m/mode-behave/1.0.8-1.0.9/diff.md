# Comparing `tmp/mode_behave-1.0.8.tar.gz` & `tmp/mode_behave-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mode_behave-1.0.8.tar", last modified: Tue Feb 21 10:02:19 2023, max compression
+gzip compressed data, was "mode_behave-1.0.9.tar", last modified: Tue Feb 21 12:53:52 2023, max compression
```

## Comparing `mode_behave-1.0.8.tar` & `mode_behave-1.0.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-02-21 10:02:19.765571 mode_behave-1.0.8/
--rw-rw-rw-   0        0        0     1283 2023-01-26 13:58:54.000000 mode_behave-1.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0      648 2023-02-03 15:39:43.000000 mode_behave-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      272 2023-02-21 10:02:19.762569 mode_behave-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    15199 2023-02-03 15:34:48.000000 mode_behave-1.0.8/README.rst
-drwxrwxrwx   0        0        0        0 2023-02-21 10:02:19.582752 mode_behave-1.0.8/imgs/
--rw-rw-rw-   0        0        0    98864 2023-01-26 13:58:54.000000 mode_behave-1.0.8/imgs/forecast_clustering.png
--rw-rw-rw-   0        0        0    87352 2023-01-26 13:58:54.000000 mode_behave-1.0.8/imgs/forecast_sensitivity.png
-drwxrwxrwx   0        0        0        0 2023-02-21 10:02:19.607318 mode_behave-1.0.8/mode_behave.egg-info/
--rw-rw-rw-   0        0        0      272 2023-02-21 10:02:19.000000 mode_behave-1.0.8/mode_behave.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1499 2023-02-21 10:02:19.000000 mode_behave-1.0.8/mode_behave.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-21 10:02:19.000000 mode_behave-1.0.8/mode_behave.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-01-26 14:41:49.000000 mode_behave-1.0.8/mode_behave.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      165 2023-02-21 10:02:19.000000 mode_behave-1.0.8/mode_behave.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-02-21 10:02:19.000000 mode_behave-1.0.8/mode_behave.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-21 10:02:19.648414 mode_behave-1.0.8/mode_behave_public/
-drwxrwxrwx   0        0        0        0 2023-02-21 10:02:19.656194 mode_behave-1.0.8/mode_behave_public/Deployments/
--rw-rw-rw-   0        0        0     2832 2023-01-26 15:06:14.000000 mode_behave-1.0.8/mode_behave_public/Deployments/example_estimation.py
-drwxrwxrwx   0        0        0        0 2023-02-21 10:02:19.685405 mode_behave-1.0.8/mode_behave_public/InputData/
--rw-rw-rw-   0        0        0   109040 2023-01-26 13:58:54.000000 mode_behave-1.0.8/mode_behave_public/InputData/artificial_data.pickle
--rw-rw-rw-   0        0        0   328217 2023-01-26 13:58:54.000000 mode_behave-1.0.8/mode_behave_public/InputData/example_data.csv
--rw-rw-rw-   0        0        0   715538 2023-01-26 13:58:54.000000 mode_behave-1.0.8/mode_behave_public/InputData/example_data.pickle
-drwxrwxrwx   0        0        0        0 2023-02-21 10:02:19.724177 mode_behave-1.0.8/mode_behave_public/ModelParam/
--rw-rw-rw-   0        0        0     1018 2023-01-26 13:58:54.000000 mode_behave-1.0.8/mode_behave_public/ModelParam/asc_offset_hh_cars.pickle
--rw-rw-rw-   0        0        0      214 2023-01-26 13:58:54.000000 mode_behave-1.0.8/mode_behave_public/ModelParam/initial_point_artificial_data.pickle
--rw-rw-rw-   0        0        0      526 2023-01-26 13:58:54.000000 mode_behave-1.0.8/mode_behave_public/ModelParam/initial_point_car_ownership.pickle
--rw-rw-rw-   0        0        0     1104 2023-01-26 13:58:54.000000 mode_behave-1.0.8/mode_behave_public/ModelParam/initial_point_mode.pickle
--rw-rw-rw-   0        0        0    85025 2023-01-26 13:58:54.000000 mode_behave-1.0.8/mode_behave_public/ModelParam/points_artificial_data.pickle
--rw-rw-rw-   0        0        0     8127 2023-01-26 13:58:54.000000 mode_behave-1.0.8/mode_behave_public/ModelParam/shares_artificial_data.pickle
--rw-rw-rw-   0        0        0     2998 2023-01-26 13:58:54.000000 mode_behave-1.0.8/mode_behave_public/ModelParam/speed_parameters.pickle
-drwxrwxrwx   0        0        0        0 2023-02-21 10:02:19.745191 mode_behave-1.0.8/mode_behave_public/Visualizations/
--rw-rw-rw-   0        0        0   162445 2023-02-15 14:42:12.000000 mode_behave-1.0.8/mode_behave_public/Visualizations/Japan_electrified_SALES_BAN_False_EV_Market.png
--rw-rw-rw-   0        0        0   176295 2023-02-15 14:42:13.000000 mode_behave-1.0.8/mode_behave_public/Visualizations/Japan_electrified_SALES_BAN_False_Registrations.png
--rw-rw-rw-   0        0        0   163796 2023-02-15 14:43:13.000000 mode_behave-1.0.8/mode_behave_public/Visualizations/Japan_electrified_SALES_BAN_True_EV_Market.png
--rw-rw-rw-   0        0        0   186359 2023-02-15 14:43:14.000000 mode_behave-1.0.8/mode_behave_public/Visualizations/Japan_electrified_SALES_BAN_True_Registrations.png
--rw-rw-rw-   0        0        0      228 2023-01-26 13:58:54.000000 mode_behave-1.0.8/mode_behave_public/__init__.py
--rw-rw-rw-   0        0        0     1226 2023-01-26 13:58:54.000000 mode_behave-1.0.8/mode_behave_public/config.py
--rw-rw-rw-   0        0        0    10599 2023-02-07 10:23:26.000000 mode_behave-1.0.8/mode_behave_public/core.py
--rw-rw-rw-   0        0        0    35716 2023-01-26 13:58:54.000000 mode_behave-1.0.8/mode_behave_public/estimation.py
--rw-rw-rw-   0        0        0    99755 2023-02-21 10:00:30.000000 mode_behave-1.0.8/mode_behave_public/post_analysis.py
--rw-rw-rw-   0        0        0    31768 2023-02-03 13:21:52.000000 mode_behave-1.0.8/mode_behave_public/simulation.py
--rw-rw-rw-   0        0        0       42 2023-02-21 10:02:19.766570 mode_behave-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      751 2023-02-21 10:01:24.000000 mode_behave-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-21 10:02:19.757954 mode_behave-1.0.8/test/
--rw-rw-rw-   0        0        0     8413 2023-01-26 15:06:38.000000 mode_behave-1.0.8/test/test_estimation.py
--rw-rw-rw-   0        0        0     2277 2023-01-26 15:06:37.000000 mode_behave-1.0.8/test/test_simulation.py
+drwxrwxrwx   0        0        0        0 2023-02-21 12:53:52.781103 mode_behave-1.0.9/
+-rw-rw-rw-   0        0        0     1283 2023-01-26 13:58:54.000000 mode_behave-1.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      648 2023-02-03 15:39:43.000000 mode_behave-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      272 2023-02-21 12:53:52.776465 mode_behave-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    15199 2023-02-03 15:34:48.000000 mode_behave-1.0.9/README.rst
+drwxrwxrwx   0        0        0        0 2023-02-21 12:53:52.576308 mode_behave-1.0.9/imgs/
+-rw-rw-rw-   0        0        0    98864 2023-01-26 13:58:54.000000 mode_behave-1.0.9/imgs/forecast_clustering.png
+-rw-rw-rw-   0        0        0    87352 2023-01-26 13:58:54.000000 mode_behave-1.0.9/imgs/forecast_sensitivity.png
+drwxrwxrwx   0        0        0        0 2023-02-21 12:53:52.604201 mode_behave-1.0.9/mode_behave.egg-info/
+-rw-rw-rw-   0        0        0      272 2023-02-21 12:53:52.000000 mode_behave-1.0.9/mode_behave.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1499 2023-02-21 12:53:52.000000 mode_behave-1.0.9/mode_behave.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-21 12:53:52.000000 mode_behave-1.0.9/mode_behave.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-01-26 14:41:49.000000 mode_behave-1.0.9/mode_behave.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      165 2023-02-21 12:53:52.000000 mode_behave-1.0.9/mode_behave.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-02-21 12:53:52.000000 mode_behave-1.0.9/mode_behave.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-02-21 12:53:52.636024 mode_behave-1.0.9/mode_behave_public/
+drwxrwxrwx   0        0        0        0 2023-02-21 12:53:52.645410 mode_behave-1.0.9/mode_behave_public/Deployments/
+-rw-rw-rw-   0        0        0     2832 2023-01-26 15:06:14.000000 mode_behave-1.0.9/mode_behave_public/Deployments/example_estimation.py
+drwxrwxrwx   0        0        0        0 2023-02-21 12:53:52.678040 mode_behave-1.0.9/mode_behave_public/InputData/
+-rw-rw-rw-   0        0        0   109040 2023-01-26 13:58:54.000000 mode_behave-1.0.9/mode_behave_public/InputData/artificial_data.pickle
+-rw-rw-rw-   0        0        0   328217 2023-01-26 13:58:54.000000 mode_behave-1.0.9/mode_behave_public/InputData/example_data.csv
+-rw-rw-rw-   0        0        0   715538 2023-01-26 13:58:54.000000 mode_behave-1.0.9/mode_behave_public/InputData/example_data.pickle
+drwxrwxrwx   0        0        0        0 2023-02-21 12:53:52.729680 mode_behave-1.0.9/mode_behave_public/ModelParam/
+-rw-rw-rw-   0        0        0     1018 2023-01-26 13:58:54.000000 mode_behave-1.0.9/mode_behave_public/ModelParam/asc_offset_hh_cars.pickle
+-rw-rw-rw-   0        0        0      214 2023-01-26 13:58:54.000000 mode_behave-1.0.9/mode_behave_public/ModelParam/initial_point_artificial_data.pickle
+-rw-rw-rw-   0        0        0      526 2023-01-26 13:58:54.000000 mode_behave-1.0.9/mode_behave_public/ModelParam/initial_point_car_ownership.pickle
+-rw-rw-rw-   0        0        0     1104 2023-01-26 13:58:54.000000 mode_behave-1.0.9/mode_behave_public/ModelParam/initial_point_mode.pickle
+-rw-rw-rw-   0        0        0    85025 2023-01-26 13:58:54.000000 mode_behave-1.0.9/mode_behave_public/ModelParam/points_artificial_data.pickle
+-rw-rw-rw-   0        0        0     8127 2023-01-26 13:58:54.000000 mode_behave-1.0.9/mode_behave_public/ModelParam/shares_artificial_data.pickle
+-rw-rw-rw-   0        0        0     2998 2023-01-26 13:58:54.000000 mode_behave-1.0.9/mode_behave_public/ModelParam/speed_parameters.pickle
+drwxrwxrwx   0        0        0        0 2023-02-21 12:53:52.756086 mode_behave-1.0.9/mode_behave_public/Visualizations/
+-rw-rw-rw-   0        0        0   162445 2023-02-15 14:42:12.000000 mode_behave-1.0.9/mode_behave_public/Visualizations/Japan_electrified_SALES_BAN_False_EV_Market.png
+-rw-rw-rw-   0        0        0   176295 2023-02-15 14:42:13.000000 mode_behave-1.0.9/mode_behave_public/Visualizations/Japan_electrified_SALES_BAN_False_Registrations.png
+-rw-rw-rw-   0        0        0   163796 2023-02-15 14:43:13.000000 mode_behave-1.0.9/mode_behave_public/Visualizations/Japan_electrified_SALES_BAN_True_EV_Market.png
+-rw-rw-rw-   0        0        0   186359 2023-02-15 14:43:14.000000 mode_behave-1.0.9/mode_behave_public/Visualizations/Japan_electrified_SALES_BAN_True_Registrations.png
+-rw-rw-rw-   0        0        0      228 2023-01-26 13:58:54.000000 mode_behave-1.0.9/mode_behave_public/__init__.py
+-rw-rw-rw-   0        0        0     1226 2023-01-26 13:58:54.000000 mode_behave-1.0.9/mode_behave_public/config.py
+-rw-rw-rw-   0        0        0    10599 2023-02-07 10:23:26.000000 mode_behave-1.0.9/mode_behave_public/core.py
+-rw-rw-rw-   0        0        0    35716 2023-01-26 13:58:54.000000 mode_behave-1.0.9/mode_behave_public/estimation.py
+-rw-rw-rw-   0        0        0    99821 2023-02-21 12:52:45.000000 mode_behave-1.0.9/mode_behave_public/post_analysis.py
+-rw-rw-rw-   0        0        0    31768 2023-02-03 13:21:52.000000 mode_behave-1.0.9/mode_behave_public/simulation.py
+-rw-rw-rw-   0        0        0       42 2023-02-21 12:53:52.781103 mode_behave-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      751 2023-02-21 12:53:25.000000 mode_behave-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-21 12:53:52.771218 mode_behave-1.0.9/test/
+-rw-rw-rw-   0        0        0     8413 2023-01-26 15:06:38.000000 mode_behave-1.0.9/test/test_estimation.py
+-rw-rw-rw-   0        0        0     2277 2023-01-26 15:06:37.000000 mode_behave-1.0.9/test/test_simulation.py
```

### Comparing `mode_behave-1.0.8/LICENSE.txt` & `mode_behave-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mode_behave-1.0.8/MANIFEST.in` & `mode_behave-1.0.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `mode_behave-1.0.8/README.rst` & `mode_behave-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `mode_behave-1.0.8/imgs/forecast_clustering.png` & `mode_behave-1.0.9/imgs/forecast_clustering.png`

 * *Files identical despite different names*

### Comparing `mode_behave-1.0.8/imgs/forecast_sensitivity.png` & `mode_behave-1.0.9/imgs/forecast_sensitivity.png`

 * *Files identical despite different names*

### Comparing `mode_behave-1.0.8/mode_behave.egg-info/SOURCES.txt` & `mode_behave-1.0.9/mode_behave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mode_behave-1.0.8/mode_behave_public/Deployments/example_estimation.py` & `mode_behave-1.0.9/mode_behave_public/Deployments/example_estimation.py`

 * *Files identical despite different names*

### Comparing `mode_behave-1.0.8/mode_behave_public/InputData/artificial_data.pickle` & `mode_behave-1.0.9/mode_behave_public/InputData/artificial_data.pickle`

 * *Files identical despite different names*

### Comparing `mode_behave-1.0.8/mode_behave_public/InputData/example_data.csv` & `mode_behave-1.0.9/mode_behave_public/InputData/example_data.csv`

 * *Files identical despite different names*

### Comparing `mode_behave-1.0.8/mode_behave_public/InputData/example_data.pickle` & `mode_behave-1.0.9/mode_behave_public/InputData/example_data.pickle`

 * *Files identical despite different names*

### Comparing `mode_behave-1.0.8/mode_behave_public/ModelParam/asc_offset_hh_cars.pickle` & `mode_behave-1.0.9/mode_behave_public/ModelParam/asc_offset_hh_cars.pickle`

 * *Files identical despite different names*

### Comparing `mode_behave-1.0.8/mode_behave_public/ModelParam/initial_point_car_ownership.pickle` & `mode_behave-1.0.9/mode_behave_public/ModelParam/initial_point_car_ownership.pickle`

 * *Files identical despite different names*

### Comparing `mode_behave-1.0.8/mode_behave_public/ModelParam/initial_point_mode.pickle` & `mode_behave-1.0.9/mode_behave_public/ModelParam/initial_point_mode.pickle`

 * *Files identical despite different names*

### Comparing `mode_behave-1.0.8/mode_behave_public/ModelParam/points_artificial_data.pickle` & `mode_behave-1.0.9/mode_behave_public/ModelParam/points_artificial_data.pickle`

 * *Files identical despite different names*

### Comparing `mode_behave-1.0.8/mode_behave_public/ModelParam/shares_artificial_data.pickle` & `mode_behave-1.0.9/mode_behave_public/ModelParam/shares_artificial_data.pickle`

 * *Files identical despite different names*

### Comparing `mode_behave-1.0.8/mode_behave_public/ModelParam/speed_parameters.pickle` & `mode_behave-1.0.9/mode_behave_public/ModelParam/speed_parameters.pickle`

 * *Files identical despite different names*

### Comparing `mode_behave-1.0.8/mode_behave_public/Visualizations/Japan_electrified_SALES_BAN_False_EV_Market.png` & `mode_behave-1.0.9/mode_behave_public/Visualizations/Japan_electrified_SALES_BAN_False_EV_Market.png`

 * *Files identical despite different names*

### Comparing `mode_behave-1.0.8/mode_behave_public/Visualizations/Japan_electrified_SALES_BAN_False_Registrations.png` & `mode_behave-1.0.9/mode_behave_public/Visualizations/Japan_electrified_SALES_BAN_False_Registrations.png`

 * *Files identical despite different names*

### Comparing `mode_behave-1.0.8/mode_behave_public/Visualizations/Japan_electrified_SALES_BAN_True_EV_Market.png` & `mode_behave-1.0.9/mode_behave_public/Visualizations/Japan_electrified_SALES_BAN_True_EV_Market.png`

 * *Files identical despite different names*

### Comparing `mode_behave-1.0.8/mode_behave_public/Visualizations/Japan_electrified_SALES_BAN_True_Registrations.png` & `mode_behave-1.0.9/mode_behave_public/Visualizations/Japan_electrified_SALES_BAN_True_Registrations.png`

 * *Files identical despite different names*

### Comparing `mode_behave-1.0.8/mode_behave_public/config.py` & `mode_behave-1.0.9/mode_behave_public/config.py`

 * *Files identical despite different names*

### Comparing `mode_behave-1.0.8/mode_behave_public/core.py` & `mode_behave-1.0.9/mode_behave_public/core.py`

 * *Files identical despite different names*

### Comparing `mode_behave-1.0.8/mode_behave_public/estimation.py` & `mode_behave-1.0.9/mode_behave_public/estimation.py`

 * *Files identical despite different names*

### Comparing `mode_behave-1.0.8/mode_behave_public/post_analysis.py` & `mode_behave-1.0.9/mode_behave_public/post_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -2184,21 +2184,23 @@
                         
             #add shares to dataframe
             shares_pandas["share"] = self.shares.copy()
             
             #add initial point to each row
             shares_pandas.iloc[:, 1:] = self.initial_point.copy()
             
+            points_array = np.array(self.points)
+            
             #subtitute initial point values by values from points.
             for a, attr in enumerate(self.param["constant"]["random"]):
                 for c in range(self.count_c):
                     #same random value for each choice alternative (-constant- parameter)
-                    shares_pandas[attr + "_" + str(c)] = self.points.T[a].copy()
+                    shares_pandas[attr + "_" + str(c)] = points_array.T[a].copy()
             for a, attr in enumerate(self.param["variable"]["random"]):
                 for c in range(self.count_c):
-                    shares_pandas[attr + "_" + str(c)] = self.points.T[len_con_ran + len_var_ran*c + a].copy()
+                    shares_pandas[attr + "_" + str(c)] = points_array.T[len_con_ran + len_var_ran*c + a].copy()
                                 
             if PATH_SAVE:
                 t_stats_pandas.to_csv(PATH_SAVE + "MNL_estimates.csv")
                 shares_pandas.to_csv(PATH_SAVE + "MXL_estimates.csv")
             else:
                 return t_stats_pandas.to_csv(), shares_pandas.to_csv()
```

### Comparing `mode_behave-1.0.8/mode_behave_public/simulation.py` & `mode_behave-1.0.9/mode_behave_public/simulation.py`

 * *Files identical despite different names*

### Comparing `mode_behave-1.0.8/setup.py` & `mode_behave-1.0.9/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='mode_behave',
-      version='1.0.8',
+      version='1.0.9',
       description='Estimation and simulation of discrete choice models',
       author='Julian Reul',
       author_email='j.reul@fz-juelich.de',
       url='https://github.com/julianreul/mode_behave',
       license='MIT',
       packages=['mode_behave_public'],
       install_requires=[
```

### Comparing `mode_behave-1.0.8/test/test_estimation.py` & `mode_behave-1.0.9/test/test_estimation.py`

 * *Files identical despite different names*

### Comparing `mode_behave-1.0.8/test/test_simulation.py` & `mode_behave-1.0.9/test/test_simulation.py`

 * *Files identical despite different names*

