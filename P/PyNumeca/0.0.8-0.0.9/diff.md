# Comparing `tmp/PyNumeca-v0.0.8.tar.gz` & `tmp/PyNumeca-v0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyNumeca-v0.0.8.tar", last modified: Wed Oct 12 08:29:19 2022, max compression
+gzip compressed data, was "PyNumeca-v0.0.9.tar", last modified: Mon Oct 24 12:32:02 2022, max compression
```

## Comparing `PyNumeca-v0.0.8.tar` & `PyNumeca-v0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 marco      (501) staff       (20)        0 2022-10-12 08:29:19.624559 PyNumeca-v0.0.8/
--rw-r--r--   0 marco      (501) staff       (20)      657 2022-10-12 08:29:19.624646 PyNumeca-v0.0.8/PKG-INFO
-drwxr-xr-x   0 marco      (501) staff       (20)        0 2022-10-12 08:29:19.621850 PyNumeca-v0.0.8/PyNumeca/
--rw-r--r--   0 marco      (501) staff       (20)      122 2022-10-03 07:05:54.670178 PyNumeca-v0.0.8/PyNumeca/__init__.py
--rw-r--r--   0 marco      (501) staff       (20)       22 2022-07-07 07:52:42.529376 PyNumeca-v0.0.8/PyNumeca/__main__.py
--rw-r--r--   0 marco      (501) staff       (20)      106 2022-07-07 08:23:15.149886 PyNumeca-v0.0.8/PyNumeca/constants.py
-drwxr-xr-x   0 marco      (501) staff       (20)        0 2022-10-12 08:29:19.622353 PyNumeca-v0.0.8/PyNumeca/fine/
--rw-r--r--   0 marco      (501) staff       (20)       38 2022-07-08 09:12:02.446708 PyNumeca-v0.0.8/PyNumeca/fine/__init__.py
--rw-r--r--   0 marco      (501) staff       (20)     1828 2022-07-11 08:37:02.839019 PyNumeca-v0.0.8/PyNumeca/fine/fine.py
--rw-r--r--   0 marco      (501) staff       (20)        0 2022-07-07 08:11:38.852170 PyNumeca-v0.0.8/PyNumeca/fine/utils.py
-drwxr-xr-x   0 marco      (501) staff       (20)        0 2022-10-12 08:29:19.622844 PyNumeca-v0.0.8/PyNumeca/igg/
--rw-r--r--   0 marco      (501) staff       (20)       36 2022-07-08 09:12:02.453716 PyNumeca-v0.0.8/PyNumeca/igg/__init__.py
--rw-r--r--   0 marco      (501) staff       (20)      773 2022-07-07 11:57:29.969037 PyNumeca-v0.0.8/PyNumeca/igg/igg.py
--rw-r--r--   0 marco      (501) staff       (20)        1 2022-07-07 08:05:35.377419 PyNumeca-v0.0.8/PyNumeca/igg/utils.py
-drwxr-xr-x   0 marco      (501) staff       (20)        0 2022-10-12 08:29:19.623188 PyNumeca-v0.0.8/PyNumeca/postprocessing/
--rw-r--r--   0 marco      (501) staff       (20)       41 2022-10-03 07:25:52.786123 PyNumeca-v0.0.8/PyNumeca/postprocessing/__init__.py
--rw-r--r--   0 marco      (501) staff       (20)     1503 2022-10-04 07:21:18.642949 PyNumeca-v0.0.8/PyNumeca/postprocessing/plan.py
--rw-r--r--   0 marco      (501) staff       (20)     5748 2022-07-08 15:07:17.856242 PyNumeca-v0.0.8/PyNumeca/pynumeca.py
-drwxr-xr-x   0 marco      (501) staff       (20)        0 2022-10-12 08:29:19.624525 PyNumeca-v0.0.8/PyNumeca/reader/
--rw-r--r--   0 marco      (501) staff       (20)      129 2022-07-08 09:12:02.451232 PyNumeca-v0.0.8/PyNumeca/reader/__init__.py
--rw-r--r--   0 marco      (501) staff       (20)     4230 2022-07-25 13:30:33.231718 PyNumeca-v0.0.8/PyNumeca/reader/iecEntry.py
--rw-r--r--   0 marco      (501) staff       (20)      686 2022-07-05 09:05:17.677833 PyNumeca-v0.0.8/PyNumeca/reader/iecGroup.py
--rw-r--r--   0 marco      (501) staff       (20)     5005 2022-07-05 09:05:17.677963 PyNumeca-v0.0.8/PyNumeca/reader/niBladeGeometryEntry.py
--rw-r--r--   0 marco      (501) staff       (20)     2561 2022-07-05 09:05:17.678077 PyNumeca-v0.0.8/PyNumeca/reader/numecaEntry.py
--rw-r--r--   0 marco      (501) staff       (20)    28053 2022-10-12 07:33:37.340581 PyNumeca-v0.0.8/PyNumeca/reader/numecaParser.py
--rw-r--r--   0 marco      (501) staff       (20)     1673 2022-07-05 09:05:17.678380 PyNumeca-v0.0.8/PyNumeca/reader/sectionEntry.py
--rw-r--r--   0 marco      (501) staff       (20)     3148 2022-07-19 09:19:29.960944 PyNumeca-v0.0.8/PyNumeca/reader/zrCurveEntry.py
--rw-r--r--   0 marco      (501) staff       (20)       61 2021-09-13 13:48:49.996000 PyNumeca-v0.0.8/setup.cfg
--rw-r--r--   0 marco      (501) staff       (20)     1712 2022-10-12 08:28:59.838234 PyNumeca-v0.0.8/setup.py
+drwxr-xr-x   0 marco      (501) staff       (20)        0 2022-10-24 12:32:02.354287 PyNumeca-v0.0.9/
+-rw-r--r--   0 marco      (501) staff       (20)      657 2022-10-24 12:32:02.354622 PyNumeca-v0.0.9/PKG-INFO
+drwxr-xr-x   0 marco      (501) staff       (20)        0 2022-10-24 12:32:02.348364 PyNumeca-v0.0.9/PyNumeca/
+-rw-r--r--   0 marco      (501) staff       (20)      122 2022-10-03 07:05:54.670178 PyNumeca-v0.0.9/PyNumeca/__init__.py
+-rw-r--r--   0 marco      (501) staff       (20)       22 2022-07-07 07:52:42.529376 PyNumeca-v0.0.9/PyNumeca/__main__.py
+-rw-r--r--   0 marco      (501) staff       (20)      106 2022-07-07 08:23:15.149886 PyNumeca-v0.0.9/PyNumeca/constants.py
+drwxr-xr-x   0 marco      (501) staff       (20)        0 2022-10-24 12:32:02.350890 PyNumeca-v0.0.9/PyNumeca/fine/
+-rw-r--r--   0 marco      (501) staff       (20)       38 2022-07-08 09:12:02.446708 PyNumeca-v0.0.9/PyNumeca/fine/__init__.py
+-rw-r--r--   0 marco      (501) staff       (20)     1828 2022-07-11 08:37:02.839019 PyNumeca-v0.0.9/PyNumeca/fine/fine.py
+-rw-r--r--   0 marco      (501) staff       (20)        0 2022-07-07 08:11:38.852170 PyNumeca-v0.0.9/PyNumeca/fine/utils.py
+drwxr-xr-x   0 marco      (501) staff       (20)        0 2022-10-24 12:32:02.351487 PyNumeca-v0.0.9/PyNumeca/igg/
+-rw-r--r--   0 marco      (501) staff       (20)       36 2022-07-08 09:12:02.453716 PyNumeca-v0.0.9/PyNumeca/igg/__init__.py
+-rw-r--r--   0 marco      (501) staff       (20)      773 2022-07-07 11:57:29.969037 PyNumeca-v0.0.9/PyNumeca/igg/igg.py
+-rw-r--r--   0 marco      (501) staff       (20)        1 2022-07-07 08:05:35.377419 PyNumeca-v0.0.9/PyNumeca/igg/utils.py
+drwxr-xr-x   0 marco      (501) staff       (20)        0 2022-10-24 12:32:02.351943 PyNumeca-v0.0.9/PyNumeca/postprocessing/
+-rw-r--r--   0 marco      (501) staff       (20)       41 2022-10-03 07:25:52.786123 PyNumeca-v0.0.9/PyNumeca/postprocessing/__init__.py
+-rw-r--r--   0 marco      (501) staff       (20)     1503 2022-10-04 07:21:18.642949 PyNumeca-v0.0.9/PyNumeca/postprocessing/plan.py
+-rw-r--r--   0 marco      (501) staff       (20)     5748 2022-07-08 15:07:17.856242 PyNumeca-v0.0.9/PyNumeca/pynumeca.py
+drwxr-xr-x   0 marco      (501) staff       (20)        0 2022-10-24 12:32:02.354098 PyNumeca-v0.0.9/PyNumeca/reader/
+-rw-r--r--   0 marco      (501) staff       (20)      129 2022-07-08 09:12:02.451232 PyNumeca-v0.0.9/PyNumeca/reader/__init__.py
+-rw-r--r--   0 marco      (501) staff       (20)     4230 2022-07-25 13:30:33.231718 PyNumeca-v0.0.9/PyNumeca/reader/iecEntry.py
+-rw-r--r--   0 marco      (501) staff       (20)      686 2022-07-05 09:05:17.677833 PyNumeca-v0.0.9/PyNumeca/reader/iecGroup.py
+-rw-r--r--   0 marco      (501) staff       (20)     5005 2022-07-05 09:05:17.677963 PyNumeca-v0.0.9/PyNumeca/reader/niBladeGeometryEntry.py
+-rw-r--r--   0 marco      (501) staff       (20)     2561 2022-07-05 09:05:17.678077 PyNumeca-v0.0.9/PyNumeca/reader/numecaEntry.py
+-rw-r--r--   0 marco      (501) staff       (20)    31017 2022-10-24 12:29:37.297500 PyNumeca-v0.0.9/PyNumeca/reader/numecaParser.py
+-rw-r--r--   0 marco      (501) staff       (20)     2093 2022-10-24 12:29:37.298198 PyNumeca-v0.0.9/PyNumeca/reader/sectionEntry.py
+-rw-r--r--   0 marco      (501) staff       (20)     3512 2022-10-24 12:29:37.299039 PyNumeca-v0.0.9/PyNumeca/reader/zrCurveEntry.py
+-rw-r--r--   0 marco      (501) staff       (20)       61 2021-09-13 13:48:49.996000 PyNumeca-v0.0.9/setup.cfg
+-rw-r--r--   0 marco      (501) staff       (20)     1712 2022-10-24 12:32:01.369701 PyNumeca-v0.0.9/setup.py
```

### Comparing `PyNumeca-v0.0.8/PKG-INFO` & `PyNumeca-v0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: PyNumeca
-Version: v0.0.8
+Version: v0.0.9
 Summary: PyNumeca
 Home-page: https://github.com/GitMarco27/PyNumeca.git
 Author: Marco Sanguineti
 Author-email: marco.sanguineti.info@gmail.com
 License: MIT
-Download-URL: https://github.com/GitMarco27/PyNumeca/archive/refs/tags/v0.0.8.zip
+Download-URL: https://github.com/GitMarco27/PyNumeca/archive/refs/tags/v0.0.9.zip
 Description: UNKNOWN
 Keywords: PyNumeca,Numeca,Python
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PyNumeca-v0.0.8/PyNumeca/fine/fine.py` & `PyNumeca-v0.0.9/PyNumeca/fine/fine.py`

 * *Files identical despite different names*

### Comparing `PyNumeca-v0.0.8/PyNumeca/igg/igg.py` & `PyNumeca-v0.0.9/PyNumeca/igg/igg.py`

 * *Files identical despite different names*

### Comparing `PyNumeca-v0.0.8/PyNumeca/postprocessing/plan.py` & `PyNumeca-v0.0.9/PyNumeca/postprocessing/plan.py`

 * *Files identical despite different names*

### Comparing `PyNumeca-v0.0.8/PyNumeca/pynumeca.py` & `PyNumeca-v0.0.9/PyNumeca/pynumeca.py`

 * *Files identical despite different names*

### Comparing `PyNumeca-v0.0.8/PyNumeca/reader/iecEntry.py` & `PyNumeca-v0.0.9/PyNumeca/reader/iecEntry.py`

 * *Files identical despite different names*

### Comparing `PyNumeca-v0.0.8/PyNumeca/reader/iecGroup.py` & `PyNumeca-v0.0.9/PyNumeca/reader/iecGroup.py`

 * *Files identical despite different names*

### Comparing `PyNumeca-v0.0.8/PyNumeca/reader/niBladeGeometryEntry.py` & `PyNumeca-v0.0.9/PyNumeca/reader/niBladeGeometryEntry.py`

 * *Files identical despite different names*

### Comparing `PyNumeca-v0.0.8/PyNumeca/reader/numecaEntry.py` & `PyNumeca-v0.0.9/PyNumeca/reader/numecaEntry.py`

 * *Files identical despite different names*

### Comparing `PyNumeca-v0.0.8/PyNumeca/reader/numecaParser.py` & `PyNumeca-v0.0.9/PyNumeca/reader/numecaParser.py`

 * *Files 8% similar despite different names*

```diff
@@ -470,14 +470,66 @@
             suction.append(section)
         for item in ni_blade_geometry.pressureList:
             section = np.vstack([item.X, item.Y, item.Z, np.ones(item.numberOfPointsInt)]).transpose()
             section = np.flip(section, axis=0)
             pressure.append(section)
         return np.array([(np.asarray(suction), np.asarray(pressure))], dtype=float)
 
+    def exportNpyArrayCyl(self, row_number=0, blade_number=0):
+        ni_blade_geometry = self.retrieveNiBladeGeometry(row_number, blade_number)
+        if (not self.cylCoordDefined(row_number, blade_number)):
+            self.convertCartesian2Cyl(row_number, blade_number)
+        suction = []
+        pressure = []
+        for item in ni_blade_geometry.suctionList:
+            section = np.vstack([item.R, item.THETA, item.Z, np.zeros(item.numberOfPointsInt)]).transpose()
+            suction.append(section)
+        for item in ni_blade_geometry.pressureList:
+            section = np.vstack([item.R, item.THETA, item.Z, np.ones(item.numberOfPointsInt)]).transpose()
+            section = np.flip(section, axis=0)
+            pressure.append(section)
+        return np.array([(np.asarray(suction), np.asarray(pressure))], dtype=float)
+
+    def convertCartesian2Cyl(self, row_number=0, blade_number=0):
+        ni_blade_geometry = self.retrieveNiBladeGeometry(row_number, blade_number)
+        for item in ni_blade_geometry.suctionList:
+            item.R = []
+            item.THETA = []
+            for index in range(len(item.X)):
+                item.R.append(np.hypot(item.Y[index], item.X[index]))
+                item.THETA.append(np.arctan2(item.X[index], item.Y[index]))
+        for item in ni_blade_geometry.pressureList:
+            item.R = []
+            item.THETA = []
+            for index in range(len(item.X)):
+                item.R.append(np.hypot(item.Y[index], item.X[index]))
+                item.THETA.append(np.arctan2(item.X[index], item.Y[index]))
+
+    def cylCoordDefined(self, row_number=0, blade_number=0):
+        ni_blade_geometry = self.retrieveNiBladeGeometry(row_number, blade_number)
+        check = 0
+        for item in ni_blade_geometry.suctionList:
+            check+= len(item.THETA) + len(item.R)
+        for item in ni_blade_geometry.pressureList:
+            check += len(item.THETA) + len(item.R)
+        return (bool(check))
+
+
+    def importNpyArrayCyl(self, array, row_number=0, blade_number=0):
+        # array shape (2,nSections,nPoints,4)
+        ni_blade_geometry = self.retrieveNiBladeGeometry(row_number, blade_number)
+        n_sections_from_array = array.shape[1]
+        ni_blade_geometry.setNumberOfSections(n_sections_from_array)
+        for idx, suction in enumerate(ni_blade_geometry.suctionList):
+            new_list = array[0][idx].transpose().tolist()
+            suction.updateArraysCyl(new_list[0], new_list[1], new_list[2])
+        for idx, pressure in enumerate(ni_blade_geometry.pressureList):
+            new_list = array[1][idx].transpose().tolist()
+            pressure.updateArraysCyl(new_list[0][::-1], new_list[1][::-1], new_list[2][::-1])
+
     def importNpyArray(self, array, row_number=0, blade_number=0):
         # array shape (2,nSections,nPoints,4)
         ni_blade_geometry = self.retrieveNiBladeGeometry(row_number, blade_number)
         n_sections_from_array = array.shape[1]
         ni_blade_geometry.setNumberOfSections(n_sections_from_array)
         for idx, suction in enumerate(ni_blade_geometry.suctionList):
             new_list = array[0][idx].transpose().tolist()
@@ -598,28 +650,34 @@
                     zrList = self["ROOT"]["GEOMTURBO"]["CHANNEL_0"][key]["zrcurve_0"]
                     basic_curve_dict[name] = (key, zrList)
                 except:
                     pass
         return (basic_curve_dict)
 
     def append_and_update_curves(self, basic_curve_dict, vertex_list):
+        for item in basic_curve_dict.items():
+            curve = item[1][1]
+            if curve.numberOfPoints == 2:
+                # QUI bisogna aggiungere i punti
+                #pass
+                curve.uniformIncreasePointsNumber(50)
+
         base_curve = vertex_list[1][2]
         for curve in vertex_list[2:]:
             basic_curve_dict[base_curve][1].append(basic_curve_dict[curve[2]][1])
             key_to_remove = basic_curve_dict[curve[2]][0]
             del self["ROOT"]["GEOMTURBO"]["CHANNEL_0"][key_to_remove]
             del self["ROOT"]["GEOMTURBO"]["CHANNEL_0"][curve[0]][curve[1]]
 
     def exportZRNpyArrays(self):
         basic_curve_dict = self.get_basic_curve_dict()
         hub_curve_name = self["ROOT"]["GEOMTURBO"]["CHANNEL_0"]["channel_curve_hub_0"]["VERTEX"].value[0]
         shroud_curve_name = self["ROOT"]["GEOMTURBO"]["CHANNEL_0"]["channel_curve_shroud_0"]["VERTEX"].value[0]
         hub_curve = basic_curve_dict[hub_curve_name][1]
         shroud_curve = basic_curve_dict[shroud_curve_name][1]
-
         hub_section    = np.vstack([np.zeros(hub_curve.numberOfPoints), hub_curve.R, hub_curve.Z, np.zeros(hub_curve.numberOfPoints)]).transpose()
         shroud_section = np.vstack([np.zeros(shroud_curve.numberOfPoints), shroud_curve.R, shroud_curve.Z, np.ones(shroud_curve.numberOfPoints)]).transpose()
         return (np.expand_dims(hub_section,axis=0), np.expand_dims(shroud_section,axis=0))
 
     def importZRNpyArrays(self, hub_section, shroud_section):
         self.importZRNpyHubArray(hub_section)
         self.importZRNpyShroudArray(shroud_section)
```

### Comparing `PyNumeca-v0.0.8/PyNumeca/reader/sectionEntry.py` & `PyNumeca-v0.0.9/PyNumeca/reader/sectionEntry.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 from PyNumeca.reader.iecEntry import iecEntry
+import numpy as np
 class sectionEntry(iecEntry):
     def __init__(self, *args):
         super(sectionEntry, self).__init__()
         self.headerComment = None
         self.numberOfPointsInt = 0
         self.numberOfPointsEntry = iecEntry()
         self.referenceFrame = "XYZ"
         self.leadingSpaceString = ""
         self.X2YSpaceString = ""
         self.Y2ZSpaceString = ""
         self.trailingSpaceString = ""
         self.X = []
         self.Y = []
         self.Z = []
+        self.R = []
+        self.THETA = []
 
     def __repr__(self):
         pass
 
     def __str__(self):
         pass
 
     def outputString(self):
         outputString = ""
         outputString += self.headerComment.outputString()
         outputString += self.referenceFrame.outputString()
         outputString += self.numberOfPointsEntry.outputString()
         for i in range(self.numberOfPointsInt):
-            #print(len(self.X2YSpaceString),  len(self.Y2ZSpaceString[0]), len(self.Y2ZSpaceString[1]))
-            #print (str(self.X[i]),"\n", str(self.Y[i]),"\n", str(self.Z[i]))
             outputString += self.leadingSpaceString + str(self.X[i]) + \
                             self.X2YSpaceString + str(self.Y[i]) + \
                             self.Y2ZSpaceString + str(self.Z[i]) + \
                             self.trailingSpaceString
         return outputString
 
     def updateArrays(self, newX, newY, newZ):
@@ -40,8 +41,24 @@
             exit()
         self.numberOfPointsInt = len(newX)
         self.numberOfPointsEntry.key = str(self.numberOfPointsInt)
         self.X = newX
         self.Y = newY
         self.Z = newZ
 
+    def updateArraysCyl(self, newR, newTHETA, newZ):
+        if (len(newR) != len(newTHETA) or len(newTHETA) != len(newZ)):
+            print ("ERRORE")
+            exit()
+        self.numberOfPointsInt = len(newR)
+        self.numberOfPointsEntry.key = str(self.numberOfPointsInt)
+        self.R = newR
+        self.THETA = newTHETA
+        self.Z = newZ
+        for index in range(len(newR)):
+            self.X[index] = self.R[index] * np.cos(self.THETA[index])
+            self.Y[index] = self.R[index] * np.sin(self.THETA[index])
+
+
+
+
```

### Comparing `PyNumeca-v0.0.8/setup.py` & `PyNumeca-v0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from distutils.core import setup
-__version__ = 'v0.0.8'
+__version__ = 'v0.0.9'
 
 setup(
     name='PyNumeca',  # How you named your package folder (MyLib)
     packages=['PyNumeca',
               'PyNumeca.fine',
               'PyNumeca.postprocessing',
               'PyNumeca.igg',
@@ -12,15 +12,15 @@
     version=__version__,  # Start with a small number and increase it with every change you make
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='PyNumeca',  # Give a short description about
     # your library
     author='Marco Sanguineti',  # Type in your name
     author_email='marco.sanguineti.info@gmail.com',  # Type in your E-Mail
     url='https://github.com/GitMarco27/PyNumeca.git',  # Provide either the link to your github or to your website
-    download_url='https://github.com/GitMarco27/PyNumeca/archive/refs/tags/v0.0.8.zip',  # I explain this later on
+    download_url='https://github.com/GitMarco27/PyNumeca/archive/refs/tags/v0.0.9.zip',  # I explain this later on
     keywords=['PyNumeca', 'Numeca', 'Python'],  # Keywords that define your package best
     install_requires=[  # I get to this in a second
         'numpy',
         'pandas',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
```

