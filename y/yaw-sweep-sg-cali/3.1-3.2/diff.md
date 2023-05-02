# Comparing `tmp/yaw_sweep_sg_cali-3.1.tar.gz` & `tmp/yaw_sweep_sg_cali-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaw_sweep_sg_cali-3.1.tar", last modified: Mon May  1 16:53:57 2023, max compression
+gzip compressed data, was "yaw_sweep_sg_cali-3.2.tar", last modified: Mon May  1 19:59:52 2023, max compression
```

## Comparing `yaw_sweep_sg_cali-3.1.tar` & `yaw_sweep_sg_cali-3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 16:53:57.428768 yaw_sweep_sg_cali-3.1/
--rw-rw-rw-   0        0        0     1114 2023-04-28 07:40:23.000000 yaw_sweep_sg_cali-3.1/LICENSE
--rw-rw-rw-   0        0        0      533 2023-05-01 16:53:57.427424 yaw_sweep_sg_cali-3.1/PKG-INFO
--rw-rw-rw-   0        0        0     9922 2023-05-01 16:40:38.000000 yaw_sweep_sg_cali-3.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-01 16:53:57.428768 yaw_sweep_sg_cali-3.1/setup.cfg
--rw-rw-rw-   0        0        0      956 2023-05-01 16:53:46.000000 yaw_sweep_sg_cali-3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 16:53:57.388801 yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali/
--rw-rw-rw-   0        0        0     5082 2023-05-01 13:24:28.000000 yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali/Calibration_factors.py
--rw-rw-rw-   0        0        0     9533 2023-05-01 13:25:44.000000 yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali/Curve_fitting.py
--rw-rw-rw-   0        0        0    12439 2023-05-01 12:42:43.000000 yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali/Load_data.py
--rw-rw-rw-   0        0        0    15705 2023-05-01 11:33:27.000000 yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali/SQL_utilities.py
--rw-rw-rw-   0        0        0    10573 2023-05-01 13:09:05.000000 yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali/Yaw_sweep_identification.py
--rw-rw-rw-   0        0        0      276 2023-05-01 08:50:48.000000 yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 16:53:57.424237 yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali.egg-info/
--rw-rw-rw-   0        0        0      533 2023-05-01 16:53:56.000000 yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      448 2023-05-01 16:53:56.000000 yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 16:53:56.000000 yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-01 16:53:56.000000 yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-01 16:53:56.000000 yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 19:59:52.736401 yaw_sweep_sg_cali-3.2/
+-rw-rw-rw-   0        0        0     1114 2023-04-28 07:40:23.000000 yaw_sweep_sg_cali-3.2/LICENSE
+-rw-rw-rw-   0        0        0      533 2023-05-01 19:59:52.736401 yaw_sweep_sg_cali-3.2/PKG-INFO
+-rw-rw-rw-   0        0        0    11547 2023-05-01 19:47:34.000000 yaw_sweep_sg_cali-3.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-01 19:59:52.736401 yaw_sweep_sg_cali-3.2/setup.cfg
+-rw-rw-rw-   0        0        0      838 2023-05-01 19:58:34.000000 yaw_sweep_sg_cali-3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 19:59:52.718770 yaw_sweep_sg_cali-3.2/yaw_sweep_sg_cali/
+-rw-rw-rw-   0        0        0     5082 2023-05-01 13:24:28.000000 yaw_sweep_sg_cali-3.2/yaw_sweep_sg_cali/Calibration_factors.py
+-rw-rw-rw-   0        0        0     9533 2023-05-01 19:48:53.000000 yaw_sweep_sg_cali-3.2/yaw_sweep_sg_cali/Curve_fitting.py
+-rw-rw-rw-   0        0        0    12439 2023-05-01 12:42:43.000000 yaw_sweep_sg_cali-3.2/yaw_sweep_sg_cali/Load_data.py
+-rw-rw-rw-   0        0        0    15696 2023-05-01 19:57:26.000000 yaw_sweep_sg_cali-3.2/yaw_sweep_sg_cali/SQL_utilities.py
+-rw-rw-rw-   0        0        0    10573 2023-05-01 13:09:05.000000 yaw_sweep_sg_cali-3.2/yaw_sweep_sg_cali/Yaw_sweep_identification.py
+-rw-rw-rw-   0        0        0      276 2023-05-01 08:50:48.000000 yaw_sweep_sg_cali-3.2/yaw_sweep_sg_cali/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 19:59:52.736401 yaw_sweep_sg_cali-3.2/yaw_sweep_sg_cali.egg-info/
+-rw-rw-rw-   0        0        0      533 2023-05-01 19:59:52.000000 yaw_sweep_sg_cali-3.2/yaw_sweep_sg_cali.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2023-05-01 19:59:52.000000 yaw_sweep_sg_cali-3.2/yaw_sweep_sg_cali.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 19:59:52.000000 yaw_sweep_sg_cali-3.2/yaw_sweep_sg_cali.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-01 19:59:52.000000 yaw_sweep_sg_cali-3.2/yaw_sweep_sg_cali.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-01 19:59:52.000000 yaw_sweep_sg_cali-3.2/yaw_sweep_sg_cali.egg-info/top_level.txt
```

### Comparing `yaw_sweep_sg_cali-3.1/LICENSE` & `yaw_sweep_sg_cali-3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yaw_sweep_sg_cali-3.1/PKG-INFO` & `yaw_sweep_sg_cali-3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaw_sweep_sg_cali
-Version: 3.1
+Version: 3.2
 Summary: Package to generate the strain gauge calibration factors when those are placed on wind turbine towers. Based on idling operations, so called, yaw sweeps.
 Author: Bruno and Zahra
 Author-email: brofa@dtu.dk
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ### Please Refer To The Gitlab page:
```

### Comparing `yaw_sweep_sg_cali-3.1/README.md` & `yaw_sweep_sg_cali-3.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -14,21 +14,23 @@
 Note: In case there is no Data already available [Data](https://gitlab.windenergy.dtu.dk/brofa/v52-strain-gauge-calibration/-/tree/main/Data) and V52 is the wanted turbine, remember to connect DTU VPN.
 
 
 ## Project Overview:
 
 Tower strain gauges are commonly used in wind turbine applications to measure the strain on the tower or structure. To ensure accurate readings, it is important to regularly calibrate these gauges. This project aims to develop an automatic routine to generate strain gauge calibration factors (offset and gain) for a given amount of input time-series, considering the zero drift. The validation of the recordings will be pursued through specific idling operations, so called **Yaw Sweeps**. 
 
-bruno- commet yaw sweep
+Basicaly, ***Yaw Sweeps*** are idling operations that might happen for the sake of detwisting the power cable of a wind turbine from time to time (if necessary). As you can see, such operations are not intrinsically related to any kind of calibration routine. However, due the quite linear yaw rotation speed presented during the yaw sweeps, where the turbine is shut down (low wind speeds, zero rotor speed and blades fully pitched), the aerodynamic contributions to the bending moment at the turbine tower are negligible and the only contribution to the bending should be structural (Center of Mass misalignment). And hopefully, the turbine mass is not changing. And by so, the measurements of bending should be constant.
+
+Strain gauges, as stresses measuring devices (and by consequence bending moment) are known for presenting zero-drift over their lifetime. So, we expect, to generate calibration factors that could correct for such offset but also check for the amplitude of the measurements.
 
 
 ## Repo files 
 
-- ***main.py*** is an example applied for DTU V52 using around 4 years of data. The code is built to be generalizable so that it can be used for different time ranges (from 2018 to 2022). 
-- ***yaw_sweep_sg_cali*** contains the modules from the package  could be used to calibrate strain gauges in any wind turbine tower.
+- ***main.py*** is an example applied for DTU V52 using around 4 years of data. The code is built so that it can be used for different time ranges (from 2018 to 2022). From april 2022 on, we faced some problems still unknown to access the V52 SQL database. 
+- ***yaw_sweep_sg_cali*** contains the modules from the package that are to calibrate strain gauges in a given wind turbine tower.
 - ***how_to_use.ipynb*** is a Jupyter notebook with an input of only one month. This will facilitate the user to understand the code and  visualize two partial results: the yaw sweep identification and the curve fitting.
 - ***Data*** contains already loaded and saved DTU V52 SQL data(1 min and 50Hz) that will be used (using also Load_data.py). The idea is to save time and help the user to visualize the functioning of the package. This will be further commented below.
 
 
 ## The research wind turbine V52
 
 The research wind turbine V52 from Vestas is situated at DTU Risø Campus as a part of the row of wind turbines at the fjord. The 850 kW wind turbine arrived at DTU in 2015.- [DTU Wind and Energy Systems](https://wind.dtu.dk/Facilities/The-research-wind-turbine-V52) 
@@ -42,21 +44,25 @@
 	
 - Package stepwise:
 
 First, identify yaw sweep operations, in which the aerodynamic contribution to the tower bending moment is negligible (low wind speed). Secondly, using such operations, automatically curve fits the raw bending moment signal and extracts relavant information, as max, min, and mean values. Finally, generate recommended calibration factors (offsets). The number of yaw sweeps operation throughout a year is unknown. 
 
 # Lets start running the code :) 
 
+We strongly recommend you to start with the [Jupyter Notebook](https://gitlab.windenergy.dtu.dk/python-at-risoe/spp-2023/group_4_shaking_hands/-/blob/main/Final_Project/Yaw_Sweep_SG_Calibration.ipynb) to learn how to use the package. 
+
+Afterwards, the **main.py** description below can further facilitate the usage of the package together with the types of inputs and outputs on each major function, based on their respective docstrings.
+
 ## main.py: Getting Started - How it works
 
-***Please make sure to have the "Data" folder as in the repo. Since, if not included, the code will ask for V52 DTU SQL login information. And not just that, but each month of data can take around 5min to be loaded. For the sake of testing, we provided the operational data already, for both 1min and 50Hz data. But feel free to remove data and test the SQL routines***
+***Please make sure to have the "Data" folder as in the repo if you want to run a first trial for the V52 turbine. Since, if not included, the code will ask for V52 DTU SQL login information (which you might have as a DTU colleague). Anyhow, each month of data can take around 5min to be loaded from the database. For the sake of testing, we provided the already loaded and saved operational data for both 1min and 50Hz cases. But feel free to remove data and test the SQL routines***
 
 The package includes four main modules:
 
-- ***Load_data.py***: for loading the 1-minute and 50Hz data from SQL or local source.
+- ***Load_data.py***: for loading the 1-minute and 50Hz data from SQL or local source and save it (if SQL).
 - ***Yaw_sweep_identification.py***: for identifying the yaw sweep instants based on the linear behavior of the yaw; and triggers of rotor speed and blade pitch.
 - ***Curve_fitting.py***: for fitting sinusoidal curves to the bending moment (strain gauge) while in a yaw sweep operation to extract max, min, mean, and error values.
 - ***Calibration_factor.py***: for calculating the calibration factors (offset, gain, and wind speed) for the yaw sensors in kNm.
 
 
 In the following section, we will provide a detailed explanation of the main.py file.
 
@@ -227,8 +233,8 @@
 
 ## Improvements performed from first submission to final submission
 
 - The code was made more robust, adding safety features to avoid the code did not run due to mistakes or missunderstandings. For this, some functions were created to avoid errors and ensure the code run as expected.  
 - The code was check with pycodestyle, to ensure was properly with the recommended standards. 
 - PEP 257 information added to each function
 
-## Peer Review
+## Peer Review
```

### Comparing `yaw_sweep_sg_cali-3.1/setup.py` & `yaw_sweep_sg_cali-3.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,22 +4,21 @@
 from pathlib import Path
 this_directory1 = Path(__file__).parent
 this_directory = this_directory1.joinpath('yaw_sweep_sg_cali')
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(name='yaw_sweep_sg_cali',
-version='3.1',
+version='3.2',
 description='Package to generate the strain gauge calibration factors when those are placed on wind turbine towers. Based on idling operations, so called, yaw sweeps.', 
 long_description = long_description,
 long_description_content_type='text/markdown',
 author='Bruno and Zahra',
 author_email='brofa@dtu.dk',
 packages=['yaw_sweep_sg_cali'],
-# packages_data={'yaw_sweep_sg_cali':['Data/V52_1min_data/*.txt', 'Data/V52_50Hz_data/*.txt','Data/V52_inputs.txt']}
 install_requires = [
           'matplotlib',
           'numpy',
           'pandas',
           'pathlib',
           'scipy',
           'mysqlclient'
```

### Comparing `yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali/Calibration_factors.py` & `yaw_sweep_sg_cali-3.2/yaw_sweep_sg_cali/Calibration_factors.py`

 * *Files identical despite different names*

### Comparing `yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali/Curve_fitting.py` & `yaw_sweep_sg_cali-3.2/yaw_sweep_sg_cali/Curve_fitting.py`

 * *Files identical despite different names*

### Comparing `yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali/Load_data.py` & `yaw_sweep_sg_cali-3.2/yaw_sweep_sg_cali/Load_data.py`

 * *Files identical despite different names*

### Comparing `yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali/SQL_utilities.py` & `yaw_sweep_sg_cali-3.2/yaw_sweep_sg_cali/SQL_utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 import pandas as pd
 
 
 def inputs_SQL():
     """
     Prompt the user to provide the necessary information
     to access the V52 DTU's SQL database.
-    This function asks the user to input the following 
-    information: the database name, host address, username, 
+    This function asks the user to input the following
+    information: the database name, host address, username,
     and password for the SQL database of the V52 DTU. It returns
     a dictionary containing this information.
     Returns
     -------
     dict
         A dictionary containing the necessary information to access the
         V52 DTU's SQL database. The dictionary has the
@@ -30,36 +30,37 @@
     Notes
     -----
     If no local data is available, the user needs to provide
     this information in order to access the SQL database of the V52 DTU.
 
     Examples
     --------
-    To obtain the necessary information to access the SQL 
+    To obtain the necessary information to access the SQL
     database of the V52 DTU, call the function as follows:
     >>> inputs_SQL()
     Please input the following necessary SQL
           database information since there is no local
           data available
     user: your_username
     password: your_password
-    {'database': 'v52_wtg', 'host': '130.226.48.160', 'user': 'your_username', 'password': 'your_password'}
+    {'database': 'v52_wtg', 'host': '130.226.48.160',
+     'user': 'your_username', 'password': 'your_password'}
     """
     print('\n Please input the following necessary SQL\n\
           database information since there is no local\n\
           data available \n')
     I = {}
     I['database'] = 'v52_wtg'  # input('database:')
     I['host'] = '130.226.48.160'  # input('host:')
     I['user'] = input('user:')
     I['password'] = input('password:')
     return I
 
 
-def get_time_series(start, stop): 
+def get_time_series(start, stop):
     '''
     Generate a list of timestamps in 10-minute intervals
     between a start and stop date.
     Parameters
     ----------
     start : tuple
         A tuple of integers representing the start date
@@ -140,21 +141,21 @@
     Parameters
     ----------
     name_str : str
         The name of the data to be accessed, formatted
         as a string with the following order:
         'YYYYMMDDhhmm', where YYYY represents the year,
         MM represents the month, DD represents the day,
-        hh represents the hour, and mm represents the minute. 
+        hh represents the hour, and mm represents the minute.
     Returns
     -------
     initial : tuple of int
         A tuple representing the date and time extracted from
         `name_str`, with the following structure:
-        (YYYY, MM, DD, hh, mm), where YYYY represents the year 
+        (YYYY, MM, DD, hh, mm), where YYYY represents the year
         as a 4-digit integer, MM represents the
         month as an integer between 1 and 12, DD represents the
         day as an integer between 1 and 31, hh
         represents the hour as an integer between 0 and 23, and
         mm represents the minute as an integer
         between 0 and 59.
     """
@@ -166,26 +167,26 @@
     mm = int(name_str[10:12])
     initial = (YYYY, MM, DD, hh, mm)
     return initial
 
 
 def slice_name_string_to(name_str):
     '''
-    Slice the input name as a string to a tuple of 
+    Slice the input name as a string to a tuple of
     int representing the end date and time.
     Note that 10 minutes are added to the end time,
     as `get_time_series` is non-inclusive for the stop (to).
     Parameters
     ----------
     name_str : str
         The name of the data to be accessed.
     Returns
     -------
     end_date : tuple of int
-        A tuple of integers representing the year, 
+        A tuple of integers representing the year,
         month, day, hour, and minute of the end time.
     '''
     YYYY = int(name_str[0:4])
     MM = int(name_str[4:6])
     DD = int(name_str[6:8])
     hh = int(name_str[8:10])
     mm = int(name_str[10:12])
@@ -198,15 +199,15 @@
 def SQLconnect(I):
     """
     Establishes a connection with a MySQL database
     using the provided credentials in the input dictionary.
     Parameters
     ----------
     I : dict
-        A dictionary that contains the necessary 
+        A dictionary that contains the necessary
         information to access the
         right MySQL database. It should contain
         the following keys:
         - host: str
             The host name or IP address of the MySQL server.
         - user: str
             The username for the MySQL account.
@@ -214,15 +215,15 @@
             The password for the MySQL account.
         - database: str
             The name of the MySQL database to connect to.
 
     Returns
     -------
     cnx : connections.Connection
-        A connection object that can be used 
+        A connection object that can be used
         to interact with the MySQL database.
     """
     cnx = MySQLdb.connect(
               host=I['host'],
               user=I['user'],
               passwd=I['password'],
               db=I['database'])
@@ -300,26 +301,26 @@
         con=cnx
         )
     return df
 
 
 def SQL_read_table(I):
     """
-    Accesses the SQL database and retrieves 
+    Accesses the SQL database and retrieves
     a DataFrame of time series data based
     on the specified parameters.
     Parameters
     ----------
     I : dict
-        A dictionary containing the necessary 
+        A dictionary containing the necessary
         information to access the SQL database,
         including 'host', 'port', 'user', 'password'
         , and 'table_name'.
 
-        The dictionary can also include the 
+        The dictionary can also include the
         following optional parameters:
         - 'cols': A list of column names to retrieve.
         If not specified or set to 'all',
                   all columns will be retrieved.
         - 'SQLrowlimit': The maximum number of rows to
         retrieve from the SQL database.
                          If not specified or set to None,
@@ -327,27 +328,26 @@
         - 'rows': A dictionary of row names and timestamps
         for filtering the results.
                   The keys are the row names, and the values
                   are lists of timestamps.
                   The resulting data will include all rows
                   that match any of the specified
                   timestamps.
-        - 'logical_statements': A list of additional logical 
+        - 'logical_statements': A list of additional logical
         statements to add to the SQL query.
                                 Each statement should be a string
                                 in SQL format and will be
                                 combined with 'AND' statements.
     Returns
     -------
     df : pandas.DataFrame
-        A DataFrame containing the time series data retrieved from the SQL database.
-
+        A DataFrame containing the time series data
+        retrieved from the SQL database.
     """
     # function implementation
-    
     cnx = SQLconnect(I)
     table_name = I['table_name']
     if 'cols' in I:
         if I['cols'] == 'all':
             cols = '*'
         else:
             cols = ','.join(I['cols'])
@@ -380,15 +380,15 @@
 
 def get_data_from_SQL(
         user, password, timestamps, database, cols,
         tablename, host, logical_statements=[]):
     '''
     This function automatically access the SQL
     database for a range
-    of time instances, sensors, and more 
+    of time instances, sensors, and more
     importantly the SQL definition
     of user, password, database and host.
     And generate a dataframe
     with all the accessed data.
     Parameters
     ----------
     user : str
@@ -400,15 +400,15 @@
     cols : list
         channels to be loaded (e.g. sensors)
     tablename : str
         depends on the timestamps to be .
         format fulfilled
     host : str
     logical_statements : list, optional
-        in case the sampling frequency 
+        in case the sampling frequency
         wants to be changed for example.
         check line 114 in Load_Data.py
         The default is [].
     Returns
     -------
     df_out : data_frame
         contains the time series from the SQL database.
```

### Comparing `yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali/Yaw_sweep_identification.py` & `yaw_sweep_sg_cali-3.2/yaw_sweep_sg_cali/Yaw_sweep_identification.py`

 * *Files identical despite different names*

### Comparing `yaw_sweep_sg_cali-3.1/yaw_sweep_sg_cali.egg-info/PKG-INFO` & `yaw_sweep_sg_cali-3.2/yaw_sweep_sg_cali.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaw-sweep-sg-cali
-Version: 3.1
+Version: 3.2
 Summary: Package to generate the strain gauge calibration factors when those are placed on wind turbine towers. Based on idling operations, so called, yaw sweeps.
 Author: Bruno and Zahra
 Author-email: brofa@dtu.dk
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ### Please Refer To The Gitlab page:
```

