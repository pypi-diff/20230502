# Comparing `tmp/JupyterPiDAQ-0.8.0a0.tar.gz` & `tmp/JupyterPiDAQ-0.8.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JupyterPiDAQ-0.8.0a0.tar", last modified: Thu Apr 20 13:35:46 2023, max compression
+gzip compressed data, was "JupyterPiDAQ-0.8.1.dev0.tar", last modified: Tue May  2 14:32:58 2023, max compression
```

## Comparing `JupyterPiDAQ-0.8.0a0.tar` & `JupyterPiDAQ-0.8.1.dev0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-20 13:35:46.704400 JupyterPiDAQ-0.8.0a0/
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-20 13:35:46.699470 JupyterPiDAQ-0.8.0a0/JupyterPiDAQ.egg-info/
--rw-r--r--   0 gutow    (60685682) staff       (20)     4666 2023-04-20 13:35:46.000000 JupyterPiDAQ-0.8.0a0/JupyterPiDAQ.egg-info/PKG-INFO
--rw-r--r--   0 gutow    (60685682) staff       (20)      856 2023-04-20 13:35:46.000000 JupyterPiDAQ-0.8.0a0/JupyterPiDAQ.egg-info/SOURCES.txt
--rw-r--r--   0 gutow    (60685682) staff       (20)        1 2023-04-20 13:35:46.000000 JupyterPiDAQ-0.8.0a0/JupyterPiDAQ.egg-info/dependency_links.txt
--rw-r--r--   0 gutow    (60685682) staff       (20)      371 2023-04-20 13:35:46.000000 JupyterPiDAQ-0.8.0a0/JupyterPiDAQ.egg-info/requires.txt
--rw-r--r--   0 gutow    (60685682) staff       (20)       19 2023-04-20 13:35:46.000000 JupyterPiDAQ-0.8.0a0/JupyterPiDAQ.egg-info/top_level.txt
--rw-r--r--   0 gutow    (60685682) staff       (20)     4666 2023-04-20 13:35:46.704219 JupyterPiDAQ-0.8.0a0/PKG-INFO
--rw-r--r--   0 gutow    (60685682) staff       (20)     3972 2023-04-19 19:23:05.000000 JupyterPiDAQ-0.8.0a0/README.md
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-20 13:35:46.699727 JupyterPiDAQ-0.8.0a0/Tests/
--rw-r--r--   0 gutow    (60685682) staff       (20)        0 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0a0/Tests/__init__.py
--rw-r--r--   0 gutow    (60685682) staff       (20)     4894 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0a0/Tests/test_boards.py
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-20 13:35:46.701069 JupyterPiDAQ-0.8.0a0/jupyterpidaq/
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-20 13:35:46.701603 JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-20 13:35:46.702293 JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/PiGPIO/
--rw-r--r--   0 gutow    (60685682) staff       (20)     8820 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/PiGPIO/ADS1115.py
--rw-r--r--   0 gutow    (60685682) staff       (20)     8063 2023-04-20 01:16:08.000000 JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/PiGPIO/DAQC2.py
--rw-r--r--   0 gutow    (60685682) staff       (20)       69 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/PiGPIO/__init__.py
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-20 13:35:46.702822 JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/Simulated/
--rw-r--r--   0 gutow    (60685682) staff       (20)     7977 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/Simulated/ADCsim.py
--rw-r--r--   0 gutow    (60685682) staff       (20)     9380 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/Simulated/ADCsim_line.py
--rw-r--r--   0 gutow    (60685682) staff       (20)       55 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/Simulated/__init__.py
--rw-r--r--   0 gutow    (60685682) staff       (20)      131 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/__init__.py
--rw-r--r--   0 gutow    (60685682) staff       (20)     7617 2023-04-08 16:27:02.000000 JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/boards.py
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-20 13:35:46.703185 JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/vernier/
--rw-r--r--   0 gutow    (60685682) staff       (20)       62 2023-04-08 16:27:02.000000 JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/vernier/__init__.py
--rw-r--r--   0 gutow    (60685682) staff       (20)    11392 2023-04-20 01:25:10.000000 JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/vernier/labquest.py
--rw-r--r--   0 gutow    (60685682) staff       (20)     9279 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0a0/jupyterpidaq/ChannelSettings.py
--rw-r--r--   0 gutow    (60685682) staff       (20)     4794 2023-04-14 15:10:40.000000 JupyterPiDAQ-0.8.0a0/jupyterpidaq/DAQProc.py
--rw-r--r--   0 gutow    (60685682) staff       (20)    34634 2023-04-20 01:10:28.000000 JupyterPiDAQ-0.8.0a0/jupyterpidaq/DAQinstance.py
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-20 13:35:46.703583 JupyterPiDAQ-0.8.0a0/jupyterpidaq/Sensors/
--rw-r--r--   0 gutow    (60685682) staff       (20)       91 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0a0/jupyterpidaq/Sensors/__init__.py
--rw-r--r--   0 gutow    (60685682) staff       (20)    27233 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0a0/jupyterpidaq/Sensors/sensors.py
--rw-r--r--   0 gutow    (60685682) staff       (20)      243 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.0a0/jupyterpidaq/__init__.py
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-20 13:35:46.703790 JupyterPiDAQ-0.8.0a0/jupyterpidaq/javascript/
--rw-r--r--   0 gutow    (60685682) staff       (20)     4901 2023-04-03 16:01:44.000000 JupyterPiDAQ-0.8.0a0/jupyterpidaq/javascript/JupyterPiDAQmnu.js
--rw-r--r--   0 gutow    (60685682) staff       (20)       38 2023-04-20 13:35:46.704443 JupyterPiDAQ-0.8.0a0/setup.cfg
--rw-r--r--   0 gutow    (60685682) staff       (20)     1815 2023-04-20 13:35:37.000000 JupyterPiDAQ-0.8.0a0/setup.py
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-05-02 14:32:58.715225 JupyterPiDAQ-0.8.1.dev0/
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-05-02 14:32:58.710112 JupyterPiDAQ-0.8.1.dev0/JupyterPiDAQ.egg-info/
+-rw-r--r--   0 gutow    (60685682) staff       (20)     4697 2023-05-02 14:32:58.000000 JupyterPiDAQ-0.8.1.dev0/JupyterPiDAQ.egg-info/PKG-INFO
+-rw-r--r--   0 gutow    (60685682) staff       (20)      856 2023-05-02 14:32:58.000000 JupyterPiDAQ-0.8.1.dev0/JupyterPiDAQ.egg-info/SOURCES.txt
+-rw-r--r--   0 gutow    (60685682) staff       (20)        1 2023-05-02 14:32:58.000000 JupyterPiDAQ-0.8.1.dev0/JupyterPiDAQ.egg-info/dependency_links.txt
+-rw-r--r--   0 gutow    (60685682) staff       (20)      371 2023-05-02 14:32:58.000000 JupyterPiDAQ-0.8.1.dev0/JupyterPiDAQ.egg-info/requires.txt
+-rw-r--r--   0 gutow    (60685682) staff       (20)       19 2023-05-02 14:32:58.000000 JupyterPiDAQ-0.8.1.dev0/JupyterPiDAQ.egg-info/top_level.txt
+-rw-r--r--   0 gutow    (60685682) staff       (20)     4697 2023-05-02 14:32:58.715036 JupyterPiDAQ-0.8.1.dev0/PKG-INFO
+-rw-r--r--   0 gutow    (60685682) staff       (20)     4000 2023-05-02 13:46:48.000000 JupyterPiDAQ-0.8.1.dev0/README.md
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-05-02 14:32:58.710373 JupyterPiDAQ-0.8.1.dev0/Tests/
+-rw-r--r--   0 gutow    (60685682) staff       (20)        0 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.1.dev0/Tests/__init__.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)     4894 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.1.dev0/Tests/test_boards.py
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-05-02 14:32:58.711845 JupyterPiDAQ-0.8.1.dev0/jupyterpidaq/
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-05-02 14:32:58.712434 JupyterPiDAQ-0.8.1.dev0/jupyterpidaq/Boards/
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-05-02 14:32:58.713115 JupyterPiDAQ-0.8.1.dev0/jupyterpidaq/Boards/PiGPIO/
+-rw-r--r--   0 gutow    (60685682) staff       (20)     8820 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.1.dev0/jupyterpidaq/Boards/PiGPIO/ADS1115.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)     8063 2023-04-20 20:10:14.000000 JupyterPiDAQ-0.8.1.dev0/jupyterpidaq/Boards/PiGPIO/DAQC2.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)       69 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.1.dev0/jupyterpidaq/Boards/PiGPIO/__init__.py
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-05-02 14:32:58.713605 JupyterPiDAQ-0.8.1.dev0/jupyterpidaq/Boards/Simulated/
+-rw-r--r--   0 gutow    (60685682) staff       (20)     7977 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.1.dev0/jupyterpidaq/Boards/Simulated/ADCsim.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)     9380 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.1.dev0/jupyterpidaq/Boards/Simulated/ADCsim_line.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)       55 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.1.dev0/jupyterpidaq/Boards/Simulated/__init__.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)      131 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.1.dev0/jupyterpidaq/Boards/__init__.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)     7617 2023-04-20 20:10:14.000000 JupyterPiDAQ-0.8.1.dev0/jupyterpidaq/Boards/boards.py
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-05-02 14:32:58.713960 JupyterPiDAQ-0.8.1.dev0/jupyterpidaq/Boards/vernier/
+-rw-r--r--   0 gutow    (60685682) staff       (20)       62 2023-04-20 20:10:14.000000 JupyterPiDAQ-0.8.1.dev0/jupyterpidaq/Boards/vernier/__init__.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)    11274 2023-05-02 13:16:16.000000 JupyterPiDAQ-0.8.1.dev0/jupyterpidaq/Boards/vernier/labquest.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)     9279 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.1.dev0/jupyterpidaq/ChannelSettings.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)     4794 2023-04-20 20:10:14.000000 JupyterPiDAQ-0.8.1.dev0/jupyterpidaq/DAQProc.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)    34763 2023-05-02 13:16:16.000000 JupyterPiDAQ-0.8.1.dev0/jupyterpidaq/DAQinstance.py
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-05-02 14:32:58.714343 JupyterPiDAQ-0.8.1.dev0/jupyterpidaq/Sensors/
+-rw-r--r--   0 gutow    (60685682) staff       (20)       91 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.1.dev0/jupyterpidaq/Sensors/__init__.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)    27233 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.1.dev0/jupyterpidaq/Sensors/sensors.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)      243 2022-11-10 17:43:21.000000 JupyterPiDAQ-0.8.1.dev0/jupyterpidaq/__init__.py
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-05-02 14:32:58.714733 JupyterPiDAQ-0.8.1.dev0/jupyterpidaq/javascript/
+-rw-r--r--   0 gutow    (60685682) staff       (20)     4901 2023-04-20 20:10:14.000000 JupyterPiDAQ-0.8.1.dev0/jupyterpidaq/javascript/JupyterPiDAQmnu.js
+-rw-r--r--   0 gutow    (60685682) staff       (20)       38 2023-05-02 14:32:58.715269 JupyterPiDAQ-0.8.1.dev0/setup.cfg
+-rw-r--r--   0 gutow    (60685682) staff       (20)     1819 2023-05-02 13:46:48.000000 JupyterPiDAQ-0.8.1.dev0/setup.py
```

### Comparing `JupyterPiDAQ-0.8.0a0/JupyterPiDAQ.egg-info/PKG-INFO` & `JupyterPiDAQ-0.8.1.dev0/JupyterPiDAQ.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JupyterPiDAQ
-Version: 0.8.0a0
+Version: 0.8.1.dev0
 Summary: Live Data Acquisition in Jupyter notebooks
 Home-page: https://github.com/JupyterPhysSciLab/JupyterPiDAQ
 Author: Jonathan Gutow
 Author-email: gutow@uwosh.edu
 License: GPL-3.0+
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -18,30 +18,31 @@
 
 ## JupyterPiDAQ
 [Introduction](#introduction) | [License](#license)
 
 ### [Website/Documentation](https://jupyterphysscilab.github.io/JupyterPiDAQ/)
 
 ### Introduction:
-This software allows realtime collection and plotting of 
-digitized data inside  a Jupyter notebook. The package was initially developed
+This software allows GUI (Graphical User Interface) driven live collection, 
+plotting and analysis of 
+digitized data inside a Jupyter notebook. The package was initially developed
 to provide an inexpensive laboratory system for teaching based on
-the Raspberry Pi.  __However, it now also works on other hardware__. 
+the Raspberry Pi.  **However, it now works on other hardware**. 
 Presently the working combinations are:
 
-__on Raspberry Pis__ 
+**on Raspberry Pis** 
 * Adafruit compliant ADS1115 boards 
 ([example](https://www.amazon.com/KNACRO-4-Channel-Raspberry-ADS1115-Channel/dp/B07149WH7P),
 also available from other vendors);
 * The [&pi;-Plates DAQC2 plate](https://pi-plates.com/daqc2r1/).
 
-__on Macs (and probably Windows)__
+**on Macs and Windows**
 * [Vernier](https://www.vernier.com) LabQuest USB A-to-Ds.
 
-__demo mode on anything Jupyter runs on__
+**demo mode on anything Jupyter runs on**
 * A demo mode will run on any computer with a Jupyter notebook install and
 Python 3.6+. You can try the demo mode without installing on your own 
   computer by launching an instance on the MyBinder servers:
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JupyterPhysSciLab/JupyterPiDAQ.git/HEAD?urlpath=/tree/usage_examples)
   
 The goal is for the user interface to be as close to self-explanatory as
  possible. However, documentation is being developed along with some example
@@ -50,32 +51,32 @@
 ##### Sensors:
 Like many commercial educational packages the software knows about the
 properties of some sensors, so can collect data directly in the units
 appropriate for the sensor, in addition to the raw voltage signal returned
 by the sensor. Not all sensors are compatible with all boards.
 The developer(s) attempt to keep this list of known sensors up-to-date, but the
 code may provide additional sensors not listed here:
-* __ADS1115 compatible__ (board can provide 3.3 V of power/reference to
+* **ADS1115 compatible** (board can provide 3.3 V of power/reference to
  sensors):
   * voltage reading (V, mV) from any sensor that puts out a voltage in the
    range +/-3.3 V.
   * built-in thermistor (V, mV, K, C, F).
   * Vernier SS temperature probe (V, mV, K, C, F).
   
-* __DAQC2 compatible__ (board can provide 5.0 V of power/reference to sensors):
+* **DAQC2 compatible** (board can provide 5.0 V of power/reference to sensors):
   * voltage reading (V, mV) from any sensor that puts out a voltage in the
    range +/- 12 V.
   * Vernier SS temperature probe (V, mV, K, C, F).
   * Vernier old and new pressure sensors (V, Pa, kPa, Bar, Torr, mmHg, atm)  
   * Vernier standard pH probe (V, mV, pH).
   * Vernier flat (tris compatible) pH probe (V, mV, pH).
   * Compatible with standard Vernier analog probes. Default calibrations
   being added as time and sensors become available.
   
-* __LabQuest compatible__ (board provides 5.0 V of power/reference to sensors):
+* **LabQuest compatible** (board provides 5.0 V of power/reference to sensors):
   * voltage reading (V, mV) from any sensor that puts out a voltage in the
    range +/- 10 V.
   * Vernier SS temperature probe (V, mV, K, C, F).
   * Vernier old and new pressure sensors (V, Pa, kPa, Bar, Torr, mmHg, atm)  
   * Vernier standard pH probe (V, mV, pH).
   * Vernier flat (tris compatible) pH probe (V, mV, pH).
   * Compatible with standard Vernier analog probes. Default calibrations
```

### Comparing `JupyterPiDAQ-0.8.0a0/JupyterPiDAQ.egg-info/SOURCES.txt` & `JupyterPiDAQ-0.8.1.dev0/JupyterPiDAQ.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `JupyterPiDAQ-0.8.0a0/PKG-INFO` & `JupyterPiDAQ-0.8.1.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JupyterPiDAQ
-Version: 0.8.0a0
+Version: 0.8.1.dev0
 Summary: Live Data Acquisition in Jupyter notebooks
 Home-page: https://github.com/JupyterPhysSciLab/JupyterPiDAQ
 Author: Jonathan Gutow
 Author-email: gutow@uwosh.edu
 License: GPL-3.0+
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -18,30 +18,31 @@
 
 ## JupyterPiDAQ
 [Introduction](#introduction) | [License](#license)
 
 ### [Website/Documentation](https://jupyterphysscilab.github.io/JupyterPiDAQ/)
 
 ### Introduction:
-This software allows realtime collection and plotting of 
-digitized data inside  a Jupyter notebook. The package was initially developed
+This software allows GUI (Graphical User Interface) driven live collection, 
+plotting and analysis of 
+digitized data inside a Jupyter notebook. The package was initially developed
 to provide an inexpensive laboratory system for teaching based on
-the Raspberry Pi.  __However, it now also works on other hardware__. 
+the Raspberry Pi.  **However, it now works on other hardware**. 
 Presently the working combinations are:
 
-__on Raspberry Pis__ 
+**on Raspberry Pis** 
 * Adafruit compliant ADS1115 boards 
 ([example](https://www.amazon.com/KNACRO-4-Channel-Raspberry-ADS1115-Channel/dp/B07149WH7P),
 also available from other vendors);
 * The [&pi;-Plates DAQC2 plate](https://pi-plates.com/daqc2r1/).
 
-__on Macs (and probably Windows)__
+**on Macs and Windows**
 * [Vernier](https://www.vernier.com) LabQuest USB A-to-Ds.
 
-__demo mode on anything Jupyter runs on__
+**demo mode on anything Jupyter runs on**
 * A demo mode will run on any computer with a Jupyter notebook install and
 Python 3.6+. You can try the demo mode without installing on your own 
   computer by launching an instance on the MyBinder servers:
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JupyterPhysSciLab/JupyterPiDAQ.git/HEAD?urlpath=/tree/usage_examples)
   
 The goal is for the user interface to be as close to self-explanatory as
  possible. However, documentation is being developed along with some example
@@ -50,32 +51,32 @@
 ##### Sensors:
 Like many commercial educational packages the software knows about the
 properties of some sensors, so can collect data directly in the units
 appropriate for the sensor, in addition to the raw voltage signal returned
 by the sensor. Not all sensors are compatible with all boards.
 The developer(s) attempt to keep this list of known sensors up-to-date, but the
 code may provide additional sensors not listed here:
-* __ADS1115 compatible__ (board can provide 3.3 V of power/reference to
+* **ADS1115 compatible** (board can provide 3.3 V of power/reference to
  sensors):
   * voltage reading (V, mV) from any sensor that puts out a voltage in the
    range +/-3.3 V.
   * built-in thermistor (V, mV, K, C, F).
   * Vernier SS temperature probe (V, mV, K, C, F).
   
-* __DAQC2 compatible__ (board can provide 5.0 V of power/reference to sensors):
+* **DAQC2 compatible** (board can provide 5.0 V of power/reference to sensors):
   * voltage reading (V, mV) from any sensor that puts out a voltage in the
    range +/- 12 V.
   * Vernier SS temperature probe (V, mV, K, C, F).
   * Vernier old and new pressure sensors (V, Pa, kPa, Bar, Torr, mmHg, atm)  
   * Vernier standard pH probe (V, mV, pH).
   * Vernier flat (tris compatible) pH probe (V, mV, pH).
   * Compatible with standard Vernier analog probes. Default calibrations
   being added as time and sensors become available.
   
-* __LabQuest compatible__ (board provides 5.0 V of power/reference to sensors):
+* **LabQuest compatible** (board provides 5.0 V of power/reference to sensors):
   * voltage reading (V, mV) from any sensor that puts out a voltage in the
    range +/- 10 V.
   * Vernier SS temperature probe (V, mV, K, C, F).
   * Vernier old and new pressure sensors (V, Pa, kPa, Bar, Torr, mmHg, atm)  
   * Vernier standard pH probe (V, mV, pH).
   * Vernier flat (tris compatible) pH probe (V, mV, pH).
   * Compatible with standard Vernier analog probes. Default calibrations
```

### Comparing `JupyterPiDAQ-0.8.0a0/README.md` & `JupyterPiDAQ-0.8.1.dev0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 ## JupyterPiDAQ
 [Introduction](#introduction) | [License](#license)
 
 ### [Website/Documentation](https://jupyterphysscilab.github.io/JupyterPiDAQ/)
 
 ### Introduction:
-This software allows realtime collection and plotting of 
-digitized data inside  a Jupyter notebook. The package was initially developed
+This software allows GUI (Graphical User Interface) driven live collection, 
+plotting and analysis of 
+digitized data inside a Jupyter notebook. The package was initially developed
 to provide an inexpensive laboratory system for teaching based on
-the Raspberry Pi.  __However, it now also works on other hardware__. 
+the Raspberry Pi.  **However, it now works on other hardware**. 
 Presently the working combinations are:
 
-__on Raspberry Pis__ 
+**on Raspberry Pis** 
 * Adafruit compliant ADS1115 boards 
 ([example](https://www.amazon.com/KNACRO-4-Channel-Raspberry-ADS1115-Channel/dp/B07149WH7P),
 also available from other vendors);
 * The [&pi;-Plates DAQC2 plate](https://pi-plates.com/daqc2r1/).
 
-__on Macs (and probably Windows)__
+**on Macs and Windows**
 * [Vernier](https://www.vernier.com) LabQuest USB A-to-Ds.
 
-__demo mode on anything Jupyter runs on__
+**demo mode on anything Jupyter runs on**
 * A demo mode will run on any computer with a Jupyter notebook install and
 Python 3.6+. You can try the demo mode without installing on your own 
   computer by launching an instance on the MyBinder servers:
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JupyterPhysSciLab/JupyterPiDAQ.git/HEAD?urlpath=/tree/usage_examples)
   
 The goal is for the user interface to be as close to self-explanatory as
  possible. However, documentation is being developed along with some example
@@ -32,32 +33,32 @@
 ##### Sensors:
 Like many commercial educational packages the software knows about the
 properties of some sensors, so can collect data directly in the units
 appropriate for the sensor, in addition to the raw voltage signal returned
 by the sensor. Not all sensors are compatible with all boards.
 The developer(s) attempt to keep this list of known sensors up-to-date, but the
 code may provide additional sensors not listed here:
-* __ADS1115 compatible__ (board can provide 3.3 V of power/reference to
+* **ADS1115 compatible** (board can provide 3.3 V of power/reference to
  sensors):
   * voltage reading (V, mV) from any sensor that puts out a voltage in the
    range +/-3.3 V.
   * built-in thermistor (V, mV, K, C, F).
   * Vernier SS temperature probe (V, mV, K, C, F).
   
-* __DAQC2 compatible__ (board can provide 5.0 V of power/reference to sensors):
+* **DAQC2 compatible** (board can provide 5.0 V of power/reference to sensors):
   * voltage reading (V, mV) from any sensor that puts out a voltage in the
    range +/- 12 V.
   * Vernier SS temperature probe (V, mV, K, C, F).
   * Vernier old and new pressure sensors (V, Pa, kPa, Bar, Torr, mmHg, atm)  
   * Vernier standard pH probe (V, mV, pH).
   * Vernier flat (tris compatible) pH probe (V, mV, pH).
   * Compatible with standard Vernier analog probes. Default calibrations
   being added as time and sensors become available.
   
-* __LabQuest compatible__ (board provides 5.0 V of power/reference to sensors):
+* **LabQuest compatible** (board provides 5.0 V of power/reference to sensors):
   * voltage reading (V, mV) from any sensor that puts out a voltage in the
    range +/- 10 V.
   * Vernier SS temperature probe (V, mV, K, C, F).
   * Vernier old and new pressure sensors (V, Pa, kPa, Bar, Torr, mmHg, atm)  
   * Vernier standard pH probe (V, mV, pH).
   * Vernier flat (tris compatible) pH probe (V, mV, pH).
   * Compatible with standard Vernier analog probes. Default calibrations
```

### Comparing `JupyterPiDAQ-0.8.0a0/Tests/test_boards.py` & `JupyterPiDAQ-0.8.1.dev0/Tests/test_boards.py`

 * *Files identical despite different names*

### Comparing `JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/PiGPIO/ADS1115.py` & `JupyterPiDAQ-0.8.1.dev0/jupyterpidaq/Boards/PiGPIO/ADS1115.py`

 * *Files identical despite different names*

### Comparing `JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/PiGPIO/DAQC2.py` & `JupyterPiDAQ-0.8.1.dev0/jupyterpidaq/Boards/PiGPIO/DAQC2.py`

 * *Files identical despite different names*

### Comparing `JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/Simulated/ADCsim.py` & `JupyterPiDAQ-0.8.1.dev0/jupyterpidaq/Boards/Simulated/ADCsim.py`

 * *Files identical despite different names*

### Comparing `JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/Simulated/ADCsim_line.py` & `JupyterPiDAQ-0.8.1.dev0/jupyterpidaq/Boards/Simulated/ADCsim_line.py`

 * *Files identical despite different names*

### Comparing `JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/boards.py` & `JupyterPiDAQ-0.8.1.dev0/jupyterpidaq/Boards/boards.py`

 * *Files identical despite different names*

### Comparing `JupyterPiDAQ-0.8.0a0/jupyterpidaq/Boards/vernier/labquest.py` & `JupyterPiDAQ-0.8.1.dev0/jupyterpidaq/Boards/vernier/labquest.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from jupyterpidaq.Boards import Board
 
 logger = logging.getLogger(__name__)
 
 # Optimized for Pi 3B+ for an installed ADS1115 ADC PiHAT. This is
 # actually ignored by this board, but necessary for ADC call
 # compatibility.
-RATE = 10000 #maximum 10 kHz
+RATE = 500 #maximum 10 kHz
 
 def find_boards():
     """
     A rountine like this must be implemented by all board packages.
 
     :return: list of LabQuests (Types too?)
     """
@@ -295,27 +295,25 @@
             while len(cmd_deque) > 0:
                 cmd = cmd_deque.popleft()
                 if cmd[0] == 'close':
                     # stop thread
                     running = False
                 if cmd[0] == 'start':
                     # restart data collection to get good zero
-                    #lqs.stop()
-                    #lqs.start(PERIOD)
-                    print("Reached start.")
-                    labquest.buf.buffer_clear()
-                    now = time.time()
-                    starttime.value = now
+                    lqs.stop()
+                    lqs.start(PERIOD)
+                    starttime.value = time.time()
                     for k in range(3):
                         samples[k].value = 0
-                    print("  Time should set to: "+str(now))
                 if cmd[0] == 'send':
                     # return requested amount of data for the channel
                     chan = 'ch'+str(cmd[2])
-                    data = lqs.read_multi_pt(chan,cmd[3],device=cmd[1])
+                    data = []
+                    for k in range(cmd[3]):
+                        data.append(lqs.read(chan, device=cmd[1]))
                     datasend.send(data)
         lqs.close()
         return
     else:
         # something happened
         lqs.close()
         raise IOError("")
```

### Comparing `JupyterPiDAQ-0.8.0a0/jupyterpidaq/ChannelSettings.py` & `JupyterPiDAQ-0.8.1.dev0/jupyterpidaq/ChannelSettings.py`

 * *Files identical despite different names*

### Comparing `JupyterPiDAQ-0.8.0a0/jupyterpidaq/DAQProc.py` & `JupyterPiDAQ-0.8.1.dev0/jupyterpidaq/DAQProc.py`

 * *Files identical despite different names*

### Comparing `JupyterPiDAQ-0.8.0a0/jupyterpidaq/DAQinstance.py` & `JupyterPiDAQ-0.8.1.dev0/jupyterpidaq/DAQinstance.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 # Start Logging
 import JPSLUtils
 
 logname = 'DAQinstance_' + time.strftime('%y-%m-%d_%H%M%S',
                                          time.localtime()) + '.log'
 logging.basicConfig(filename=logname, level=logging.WARN)
+# logging.basicConfig(filename=logname, level=logging.DEBUG)
 
 # below is equivalent to %matplotlib notebook in a Jupyter cell
 from IPython import get_ipython
 
 ipython = get_ipython()
 print('Importing drivers and searching for available data acquisition '
       'hardware.',end='')
@@ -137,14 +138,18 @@
             data collection. If False a separate set of time will be
             recorded for each channel.
         """
         from plotly import graph_objects as go
         self.ignore_skew = kwargs.pop('ignore_skew',True)
         self.idno = idno
         self.livefig = go.FigureWidget(layout_template='simple_white')
+        self.PLTconn, self.DAQconn = Pipe()
+        self.DAQCTL, self.PLTCTL = Pipe()
+        self.pltthread = threading.Thread(target=self.updatingplot, args=(
+                                        self.PLTconn, self.PLTCTL))
         self.title = str(title)
         self.svname = title + '.jpidaq.html'
         self.averaging_time = 0.1  # seconds adjusted based on collection rate
         self.gain = [1] * ntraces
         self.data = []
         self.timestamp = []
         self.stdev = []
@@ -442,16 +447,14 @@
             btn.button_style = 'danger'
             btn.tooltip = 'Stop the data collection'
             # do not allow parameters to be reset after starting run.
             self.setupbtn.disabled = True
             self.setupbtn.tooltip = 'Parameters locked. The run has started.'
             self.rateinp.disabled = True
             self.timelbl.disabled = True
-            PLTconn, DAQconn = Pipe()
-            DAQCTL, PLTCTL = Pipe()
             nactive = 0
             for k in self.traces:
                 if k.isactive:
                     nactive += 1
             whichchn = []
             gains =[]
             for i in range(self.ntraces):
@@ -473,25 +476,24 @@
             # Use up to 30% of the time for averaging if channels were spaced
             # evenly between data collection times (with DACQ2 they appear
             # more synchronous than that).
             self.averaging_time = self.delta / nactive / 3
             DAQ = Process(target=DAQProc,
                           args=(
                               whichchn, gains, self.averaging_time, self.delta,
-                              DAQconn, DAQCTL))
+                              self.DAQconn, self.DAQCTL))
             DAQ.start()
-            thread = threading.Thread(target=self.updatingplot, args=(
-                                        PLTconn, PLTCTL))
-            thread.start()
+            self.pltthread.start()
             # self.updatingplot() hangs up user interface
         else:
             btn.description = 'Done'
             btn.button_style = ''
             btn.tooltip = ''
-            time.sleep(3)  # wait a few seconds for end of data collection
+            # wait a plotting thread to terminate
+            self.pltthread.join()
             self.data = data
             self.timestamp = timestamp
             self.stdev = stdev
             self.fillpandadf()
             # save data to html file so it is human readable and can be loaded
             # elsewhere.
             #self.svname = self.title + '_' + time.strftime('%y-%m-%d_%H%M%S',
@@ -695,14 +697,15 @@
                 msg = PLTCTL.recv()
                 # print (str(msg))
                 if (msg != 'done'):
                     print('Received unexpected message: ' + str(msg))
         for k in range(len(self.livefig.data)):
             self.livefig.data[k].x = toplotx[k]
             self.livefig.data[k].y = toploty[k]
+        return
 
 # TODO delete newRun once sure not needed.
 # def newRun(livefig):
 #     """
 #     Set up a new data collection run and add it to the list of runs.
 #     """
 #     nrun = len(runs) + 1
```

### Comparing `JupyterPiDAQ-0.8.0a0/jupyterpidaq/Sensors/sensors.py` & `JupyterPiDAQ-0.8.1.dev0/jupyterpidaq/Sensors/sensors.py`

 * *Files identical despite different names*

### Comparing `JupyterPiDAQ-0.8.0a0/jupyterpidaq/javascript/JupyterPiDAQmnu.js` & `JupyterPiDAQ-0.8.1.dev0/jupyterpidaq/javascript/JupyterPiDAQmnu.js`

 * *Files identical despite different names*

### Comparing `JupyterPiDAQ-0.8.0a0/setup.py` & `JupyterPiDAQ-0.8.1.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="JupyterPiDAQ",
     url = "https://github.com/JupyterPhysSciLab/JupyterPiDAQ",
-    version="0.8.0a",
+    version="0.8.1.dev0",
     description="Live Data Acquisition in Jupyter notebooks",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Jonathan Gutow",
     author_email="gutow@uwosh.edu",
     license="GPL-3.0+",
     packages=setuptools.find_packages(exclude=("dist","build","dev_testing",)),
```

