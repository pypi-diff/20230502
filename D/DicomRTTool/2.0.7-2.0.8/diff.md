# Comparing `tmp/DicomRTTool-2.0.7.tar.gz` & `tmp/DicomRTTool-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DicomRTTool-2.0.7.tar", last modified: Sun Mar 26 20:09:59 2023, max compression
+gzip compressed data, was "DicomRTTool-2.0.8.tar", last modified: Mon May  1 22:09:50 2023, max compression
```

## Comparing `DicomRTTool-2.0.7.tar` & `DicomRTTool-2.0.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-03-26 20:09:59.903591 DicomRTTool-2.0.7/
-drwxrwxrwx   0        0        0        0 2023-03-26 20:09:59.886928 DicomRTTool-2.0.7/DicomRTTool.egg-info/
--rw-rw-rw-   0        0        0     2849 2023-03-26 20:09:59.000000 DicomRTTool-2.0.7/DicomRTTool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      559 2023-03-26 20:09:59.000000 DicomRTTool-2.0.7/DicomRTTool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-26 20:09:59.000000 DicomRTTool-2.0.7/DicomRTTool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      130 2023-03-26 20:09:59.000000 DicomRTTool-2.0.7/DicomRTTool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-26 20:09:59.000000 DicomRTTool-2.0.7/DicomRTTool.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-26 20:09:59.887924 DicomRTTool-2.0.7/Images/
--rw-rw-rw-   0        0        0   587168 2022-05-08 23:09:23.000000 DicomRTTool-2.0.7/Images/multiple_rings.png
--rw-rw-rw-   0        0        0    35821 2022-05-08 23:09:23.000000 DicomRTTool-2.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0      218 2022-05-08 23:09:23.000000 DicomRTTool-2.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     2849 2023-03-26 20:09:59.902594 DicomRTTool-2.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2296 2023-03-24 00:26:49.000000 DicomRTTool-2.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-03-26 20:09:59.903591 DicomRTTool-2.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1030 2023-03-26 20:09:35.000000 DicomRTTool-2.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-26 20:09:59.893707 DicomRTTool-2.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-03-26 20:09:59.899580 DicomRTTool-2.0.7/src/DicomRTTool/
--rw-rw-rw-   0        0        0    82554 2023-03-26 20:09:35.000000 DicomRTTool-2.0.7/src/DicomRTTool/ReaderWriter.py
-drwxrwxrwx   0        0        0        0 2023-03-26 20:09:59.901573 DicomRTTool-2.0.7/src/DicomRTTool/Services/
--rw-rw-rw-   0        0        0     8964 2023-03-26 20:09:35.000000 DicomRTTool-2.0.7/src/DicomRTTool/Services/DicomBases.py
--rw-rw-rw-   0        0        0     1625 2023-03-26 20:09:35.000000 DicomRTTool-2.0.7/src/DicomRTTool/Services/StaticScripts.py
--rw-rw-rw-   0        0        0        0 2023-03-26 20:09:35.000000 DicomRTTool-2.0.7/src/DicomRTTool/Services/__init__.py
--rw-rw-rw-   0        0        0     1877 2022-05-08 23:09:23.000000 DicomRTTool-2.0.7/src/DicomRTTool/Viewer.py
--rw-rw-rw-   0        0        0      193 2023-03-26 20:09:35.000000 DicomRTTool-2.0.7/src/DicomRTTool/__init__.py
--rw-rw-rw-   0        0        0      156 2022-05-08 23:09:23.000000 DicomRTTool-2.0.7/src/DicomRTTool/key_list.txt
--rw-rw-rw-   0        0        0    17286 2022-05-08 23:09:23.000000 DicomRTTool-2.0.7/src/DicomRTTool/template_RS.dcm
--rw-rw-rw-   0        0        0     6133 2022-05-08 23:09:23.000000 DicomRTTool-2.0.7/src/Distribute_Train_Test_Validation.py
--rw-rw-rw-   0        0        0     1059 2022-05-08 23:09:23.000000 DicomRTTool-2.0.7/src/Main.py
+drwxrwxrwx   0        0        0        0 2023-05-01 22:09:50.864886 DicomRTTool-2.0.8/
+drwxrwxrwx   0        0        0        0 2023-05-01 22:09:50.833644 DicomRTTool-2.0.8/DicomRTTool.egg-info/
+-rw-rw-rw-   0        0        0     2890 2023-05-01 22:09:49.000000 DicomRTTool-2.0.8/DicomRTTool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2023-05-01 22:09:49.000000 DicomRTTool-2.0.8/DicomRTTool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 22:09:49.000000 DicomRTTool-2.0.8/DicomRTTool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      239 2023-05-01 22:09:49.000000 DicomRTTool-2.0.8/DicomRTTool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-01 22:09:49.000000 DicomRTTool-2.0.8/DicomRTTool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 22:09:50.833644 DicomRTTool-2.0.8/Images/
+-rw-rw-rw-   0        0        0   587168 2022-04-25 20:23:40.000000 DicomRTTool-2.0.8/Images/multiple_rings.png
+-rw-rw-rw-   0        0        0    35821 2022-04-25 20:23:40.000000 DicomRTTool-2.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0      218 2022-04-25 20:23:40.000000 DicomRTTool-2.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     2890 2023-05-01 22:09:50.864886 DicomRTTool-2.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2296 2023-04-10 23:03:33.000000 DicomRTTool-2.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-01 22:09:50.864886 DicomRTTool-2.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1030 2023-05-01 22:09:15.000000 DicomRTTool-2.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 22:09:50.849265 DicomRTTool-2.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-05-01 22:09:50.864886 DicomRTTool-2.0.8/src/DicomRTTool/
+-rw-rw-rw-   0        0        0    83848 2023-05-01 21:51:37.000000 DicomRTTool-2.0.8/src/DicomRTTool/ReaderWriter.py
+drwxrwxrwx   0        0        0        0 2023-05-01 22:09:50.864886 DicomRTTool-2.0.8/src/DicomRTTool/Services/
+-rw-rw-rw-   0        0        0     8964 2023-04-10 23:03:33.000000 DicomRTTool-2.0.8/src/DicomRTTool/Services/DicomBases.py
+-rw-rw-rw-   0        0        0     1625 2023-04-10 23:03:33.000000 DicomRTTool-2.0.8/src/DicomRTTool/Services/StaticScripts.py
+-rw-rw-rw-   0        0        0        0 2023-04-10 23:03:33.000000 DicomRTTool-2.0.8/src/DicomRTTool/Services/__init__.py
+-rw-rw-rw-   0        0        0     1877 2022-04-25 20:23:40.000000 DicomRTTool-2.0.8/src/DicomRTTool/Viewer.py
+-rw-rw-rw-   0        0        0      193 2023-04-10 23:03:33.000000 DicomRTTool-2.0.8/src/DicomRTTool/__init__.py
+-rw-rw-rw-   0        0        0      156 2022-04-25 20:23:40.000000 DicomRTTool-2.0.8/src/DicomRTTool/key_list.txt
+-rw-rw-rw-   0        0        0    17286 2022-04-25 20:23:40.000000 DicomRTTool-2.0.8/src/DicomRTTool/template_RS.dcm
+-rw-rw-rw-   0        0        0     6133 2022-04-25 20:23:40.000000 DicomRTTool-2.0.8/src/Distribute_Train_Test_Validation.py
+-rw-rw-rw-   0        0        0     1059 2022-04-25 20:23:40.000000 DicomRTTool-2.0.8/src/Main.py
```

### Comparing `DicomRTTool-2.0.7/DicomRTTool.egg-info/PKG-INFO` & `DicomRTTool-2.0.8/DicomRTTool.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: DicomRTTool
-Version: 2.0.7
+Version: 2.0.8
 Summary: Services for reading dicom files, RT structures, and dose files, as well as tools for converting numpy prediction masks back to an RT structure
 Home-page: https://github.com/brianmanderson/Dicom_RT_and_Images_to_Mask
 Author: Brian Mark Anderson
 Author-email: b5anderson@health.ucsd.edu
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # We're published! Please check out the Technical Note here: https://www.sciencedirect.com/science/article/abs/pii/S1879850021000485 and reference this work if you find it useful
 ### DOI:https://doi.org/10.1016/j.prro.2021.02.003
@@ -48,7 +50,9 @@
 
 ###### Ring update allows for multiple rings to be represented correctly
 
 ![multiple_rings.png](./Images/multiple_rings.png)
 
 
 #### Works on oblique images for masks and predictions*
+
+
```

### Comparing `DicomRTTool-2.0.7/DicomRTTool.egg-info/SOURCES.txt` & `DicomRTTool-2.0.8/DicomRTTool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DicomRTTool-2.0.7/Images/multiple_rings.png` & `DicomRTTool-2.0.8/Images/multiple_rings.png`

 * *Files identical despite different names*

### Comparing `DicomRTTool-2.0.7/LICENSE.txt` & `DicomRTTool-2.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `DicomRTTool-2.0.7/PKG-INFO` & `DicomRTTool-2.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: DicomRTTool
-Version: 2.0.7
+Version: 2.0.8
 Summary: Services for reading dicom files, RT structures, and dose files, as well as tools for converting numpy prediction masks back to an RT structure
 Home-page: https://github.com/brianmanderson/Dicom_RT_and_Images_to_Mask
 Author: Brian Mark Anderson
 Author-email: b5anderson@health.ucsd.edu
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # We're published! Please check out the Technical Note here: https://www.sciencedirect.com/science/article/abs/pii/S1879850021000485 and reference this work if you find it useful
 ### DOI:https://doi.org/10.1016/j.prro.2021.02.003
@@ -48,7 +50,9 @@
 
 ###### Ring update allows for multiple rings to be represented correctly
 
 ![multiple_rings.png](./Images/multiple_rings.png)
 
 
 #### Works on oblique images for masks and predictions*
+
+
```

### Comparing `DicomRTTool-2.0.7/README.md` & `DicomRTTool-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `DicomRTTool-2.0.7/setup.py` & `DicomRTTool-2.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='DicomRTTool',
     author='Brian Mark Anderson',
     author_email='b5anderson@health.ucsd.edu',
-    version='2.0.7',
+    version='2.0.8',
     description='Services for reading dicom files, RT structures, and dose files, as well as tools for '
                 'converting numpy prediction masks back to an RT structure',
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir={'DicomRTTool': 'src/DicomRTTool'},
     packages=['DicomRTTool'],
     include_package_data=True,
```

### Comparing `DicomRTTool-2.0.7/src/DicomRTTool/ReaderWriter.py` & `DicomRTTool-2.0.8/src/DicomRTTool/ReaderWriter.py`

 * *Files 1% similar despite different names*

```diff
@@ -780,15 +780,18 @@
                     loading_rois.append(roi)
                 else:
                     if self.associations:
                         for association in self.associations:
                             if association.roi_name == roi:
                                 loading_rois += association.other_names
         loading_rois = list(set(loading_rois))
-        final_out_dict = {'PatientID': [], 'RTPath': []}
+        final_out_dict = {'PatientID': [], 'PixelSpacingX': [], 'PixelSpacingY': [],
+                          'SliceThickness': [], 'zzzRTPath': [], 'zzzImagePath': []}
+        image_out_dict = {'PatientID': [], 'ImagePath': [], 'PixelSpacingX': [], 'PixelSpacingY': [],
+                          'SliceThickness': []}
         temp_associations = {}
         column_names = []
         for roi in loading_rois:
             if self.associations:
                 for association in self.associations:
                     if roi in association.other_names:
                         true_name = association.roi_name
@@ -809,24 +812,33 @@
             for roi in column_names:
                 if roi in self.rois_in_loaded_index:
                     has_wanted_roi = True
                     break
             if not has_wanted_roi:
                 continue
             image_base = self.series_instances_dictionary[index]
+            image_out_dict['PatientID'].append(image_base.PatientID)
+            image_out_dict['ImagePath'].append(image_base.path)
+            image_out_dict['PixelSpacingX'].append(image_base.pixel_spacing_x)
+            image_out_dict['PixelSpacingY'].append(image_base.pixel_spacing_y)
+            image_out_dict['SliceThickness'].append(image_base.slice_thickness)
             self.get_images()
             """
             If there is no image set, move along
             """
             dimension = np.prod(self.dicom_handle.GetSpacing())  # Voxel dimensions, in mm
             for rt_index in image_base.RTs:
                 rt_base = image_base.RTs[rt_index]
                 self.__check_contours_at_index__(index)
                 final_out_dict['PatientID'].append(rt_base.PatientID)
-                final_out_dict['RTPath'].append(rt_base.path)
+                final_out_dict['zzzRTPath'].append(rt_base.path)
+                final_out_dict['zzzImagePath'].append(image_base.path)
+                final_out_dict['PixelSpacingX'].append(image_base.pixel_spacing_x)
+                final_out_dict['PixelSpacingY'].append(image_base.pixel_spacing_y)
+                final_out_dict['SliceThickness'].append(image_base.slice_thickness)
                 """
                 Default values to be nothing, then replace them as they come
                 """
                 for roi in column_names:
                     final_out_dict[f"{roi} cc"].append(np.nan)
                 for roi in column_names:
                     if roi in rt_base.ROI_Names:
@@ -836,15 +848,20 @@
         for key in temp_associations.keys():
             if temp_associations[key] not in final_out_dict:
                 final_out_dict[temp_associations[key]] = [np.nan for _ in range(len(final_out_dict['PatientID']))]
         df = pd.DataFrame(final_out_dict)
         for key in temp_associations:
             df[temp_associations[key]] = df[f"{key} cc"] + df.fillna(0)[temp_associations[key]]
         df = df.reindex(sorted(df.columns), axis=1)
-        df.to_excel(excel_path, index=False)
+        df_image = pd.DataFrame(image_out_dict)
+        with pd.ExcelWriter(excel_path) as writer:
+            # use to_excel function and specify the sheet_name and index
+            # to store the dataframe in specified sheet
+            df.to_excel(writer, sheet_name="ROIs", index=False)
+            df_image.to_excel(writer, sheet_name="Images", index=False)
 
     def which_indexes_lack_all_rois(self):
         if self.Contour_Names:
             print('The following indexes are lacking all ROIs')
             indexes_lacking_rois = []
             for index in self.series_instances_dictionary:
                 if index not in self.indexes_with_contours:
```

### Comparing `DicomRTTool-2.0.7/src/DicomRTTool/Services/DicomBases.py` & `DicomRTTool-2.0.8/src/DicomRTTool/Services/DicomBases.py`

 * *Files identical despite different names*

### Comparing `DicomRTTool-2.0.7/src/DicomRTTool/Services/StaticScripts.py` & `DicomRTTool-2.0.8/src/DicomRTTool/Services/StaticScripts.py`

 * *Files identical despite different names*

### Comparing `DicomRTTool-2.0.7/src/DicomRTTool/Viewer.py` & `DicomRTTool-2.0.8/src/DicomRTTool/Viewer.py`

 * *Files identical despite different names*

### Comparing `DicomRTTool-2.0.7/src/DicomRTTool/template_RS.dcm` & `DicomRTTool-2.0.8/src/DicomRTTool/template_RS.dcm`

 * *Files identical despite different names*

### Comparing `DicomRTTool-2.0.7/src/Distribute_Train_Test_Validation.py` & `DicomRTTool-2.0.8/src/Distribute_Train_Test_Validation.py`

 * *Files identical despite different names*

### Comparing `DicomRTTool-2.0.7/src/Main.py` & `DicomRTTool-2.0.8/src/Main.py`

 * *Files identical despite different names*

