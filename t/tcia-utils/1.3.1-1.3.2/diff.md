# Comparing `tmp/tcia_utils-1.3.1.tar.gz` & `tmp/tcia_utils-1.3.2.tar.gz`

## Comparing `tcia_utils-1.3.1.tar` & `tcia_utils-1.3.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 tcia_utils-1.3.1/src/tcia_utils/__init__.py
--rw-r--r--   0        0        0     6700 2020-02-02 00:00:00.000000 tcia_utils-1.3.1/src/tcia_utils/datacite.py
--rw-r--r--   0        0        0    48455 2020-02-02 00:00:00.000000 tcia_utils-1.3.1/src/tcia_utils/nbia.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 tcia_utils-1.3.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 tcia_utils-1.3.1/LICENSE
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 tcia_utils-1.3.1/README.md
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 tcia_utils-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 tcia_utils-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 tcia_utils-1.3.2/src/tcia_utils/__init__.py
+-rw-r--r--   0        0        0     6700 2020-02-02 00:00:00.000000 tcia_utils-1.3.2/src/tcia_utils/datacite.py
+-rw-r--r--   0        0        0    51536 2020-02-02 00:00:00.000000 tcia_utils-1.3.2/src/tcia_utils/nbia.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 tcia_utils-1.3.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 tcia_utils-1.3.2/LICENSE
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 tcia_utils-1.3.2/README.md
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 tcia_utils-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 tcia_utils-1.3.2/PKG-INFO
```

### Comparing `tcia_utils-1.3.1/src/tcia_utils/datacite.py` & `tcia_utils-1.3.2/src/tcia_utils/datacite.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.3.1/src/tcia_utils/nbia.py` & `tcia_utils-1.3.2/src/tcia_utils/nbia.py`

 * *Files 2% similar despite different names*

```diff
@@ -590,14 +590,15 @@
 ####### downloadSeries function
 # Ingests a set of seriesUids and downloads them
 # By default, series_data expects JSON containing "SeriesInstanceUID" elements
 # Set number = n to download the first n series if you don't want the full dataset
 # Set hash = "y" if you'd like to retrieve MD5 hash values for each image
 # Saves to tciaDownload folder in current directory if no path is specified
 # Set input_type = "list" to pass a list of Series UIDs instead of JSON
+# Set input_type = "manifest" to pass the path of a *.TCIA manifest file as series_data
 # Format can be set to "df" or "csv" to return series metadata
 # Setting a csv_filename will create the csv even if format isn't specified
 # The metadata includes info about series that have previously been downloaded
 
 def downloadSeries(series_data,
                    number = 0,
                    path = "",
@@ -615,14 +616,18 @@
 
     # Prep a dataframe for later
     if format == "df" or format == "csv" or csv_filename != "":
         manifestDF=pd.DataFrame()
 
     # get base URL
     base_url = setApiUrl(endpoint, api_url)
+    
+    # if input = manifest convert manifest to python list of uids
+    if input_type == "manifest":
+        series_data = manifestToList(series_data)
 
     # set sample size if you don't want to download the full set of results
     if number > 0:
         _log.info(f"Downloading {number} out of {len(series_data)} Series Instance UIDs (scans).")
     else:
         _log.info(f"Downloading {len(series_data)} Series Instance UIDs (scans).")
 
@@ -632,15 +637,15 @@
     else:
         downloadOptions = "getImage?NewFileNames=Yes&SeriesInstanceUID="
 
     # get the data
     try:
         for x in series_data:
             # specify whether input data is json or list
-            if input_type == "list":
+            if input_type == "list" or input_type == "manifest":
                 seriesUID = x
             else:
                 seriesUID = x['SeriesInstanceUID']
             # set path for downloads and check for previously downloaded data
             if path != "":
                 pathTmp = path + "/" + seriesUID
             else:
@@ -857,16 +862,16 @@
     if modality:
         options['Modality'] = modality
 
     data = queryData(endpoint, options, api_url, format)
     return data
 
 ####### getManufacturerCounts function (Advanced)
-# Get counts of Body Part metadata from Advanced API
-# Allows filtering by collection and modality
+# Get counts of Manufacturer metadata from Advanced API
+# Allows filtering by collection, body part and modality
 
 def getManufacturerCounts(collection = "",
                       modality = "",
                       bodyPart = "",
                       api_url = "",
                       format = ""):
 
@@ -1161,48 +1166,114 @@
     except requests.exceptions.RequestException as err:
         _log.error(err)
 
 ##########################
 ##########################
 # Miscellaneous
 
-####### makeSeriesReport function
-# Ingests JSON output from getSeries() or getSharedCart() and creates summary report
+def makeSeriesReport(series_data, input_type = "", format = "", filename = None, api_url = ""):
+# Ingests JSON output from any function that returns series-level data and creates summary report
+# Specify input_type = "manifest" to ingest a *.TCIA manifest file or "list" for a python list of UIDs
+# If input_type = "manifest" or "list" and there are series UIDs that are restricted
+#    you must call getToken() with a user ID that has access to all UIDs before calling this function.
+# Specifying api_url is only necessary if you are using input_type = "manifest" or "list" with NLST data (e.g. api_url = "nlst") 
+# Specify format = "var" to return the report values as a dictionary
+# Access variables example after saving function output to report_data: subjects = report_data["subjects"]
+# Specify format = "file" to save the report to a file
+# Specify a filename parameter to set a filename if you don't want the default
+
+
+    # if input_type is manifest convert it to a list
+    if input_type == "manifest":
+        series_data = manifestToList(series_data)
+        
+    # if input_type is a list or manifest download relevant metadata
+    if input_type == "list" or input_type == "manifest":
+        df = getSeriesList(series_data, api_url = "", csv_filename = "")
+        # Rename the headers
+        if df is None or df.empty:
+            raise StopExecution
+        else:
+            df = df.rename(columns={'Subject ID': 'PatientID', 'Study UID': 'StudyInstanceUID', 'Series ID': 'SeriesInstanceUID', 'Number of images': 'ImageCount', 'Collection Name': 'Collection'})
+            # Add an empty column called "BodyPartExamined" since getSeriesList() doesn't return this info -- FEATURE REQUEST SUBMITTED TO ADD THIS
+            df['BodyPartExamined'] = ''
+    else:
+        # Create a DataFrame from the series_data
+        df = pd.DataFrame(series_data)
 
-def makeSeriesReport(series_data):
+    # Calculate summary statistics for a given collection
 
-    df = pd.DataFrame(series_data)
+    # Scan Inventory
+    subjects = len(df['PatientID'].value_counts())
+    studies = len(df['StudyInstanceUID'].value_counts())
+    series = len(df['SeriesInstanceUID'].value_counts())
+    images = df['ImageCount'].sum()
 
-    # Calculate summary statistics for a given collection
+    # Summarize Collections
+    collections = df['Collection'].value_counts(dropna=False)
+
+    # Summarize modalities
+    modalities = df['Modality'].value_counts(dropna=False)
+
+    # Summarize body parts
+    body_parts = df['BodyPartExamined'].value_counts(dropna=False)
 
-    _log.info(
+    # Summarize manufacturers
+    manufacturers = df['Manufacturer'].value_counts(dropna=False)
+
+    report = (
         # Scan Inventory
-        'Summary Statistics\n'
-        f"Subjects: {len(df['PatientID'].value_counts())} subjects\n"
-        f"Studies: {len(df['StudyInstanceUID'].value_counts())} studies\n"
-        f"Series: {len(df['SeriesInstanceUID'].value_counts())} series\n"
-        f"Images: {df['ImageCount'].sum()} images\n\n"
+        f"Summary Statistics\n"
+        f"Subjects: {subjects}\n"
+        f"Studies: {studies}\n"
+        f"Series: {series}\n"
+        f"Images: {images}\n\n"
 
         # Summarize Collections
-        "Series Counts - Collections:\n"
-        f"{df['Collection'].value_counts(dropna=False)}\n\n"
+        f"Series Counts - Collections:\n"
+        f"{collections}\n\n"
 
         # Summarize modalities
-        "Series Counts - Modality:\n"
-        f"{df['Modality'].value_counts(dropna=False)}\n\n"
+        f"Series Counts - Modality:\n"
+        f"{modalities}\n\n"
 
         # Summarize body parts
-        "Series Counts - Body Parts Examined:\n"
-        f"{df['BodyPartExamined'].value_counts(dropna=False)}\n\n"
+        f"Series Counts - Body Parts Examined:\n"
+        f"{body_parts}\n\n"
 
         # Summarize manufacturers
-        "Series Counts - Device Manufacturers:\n"
-        f"{df['Manufacturer'].value_counts(dropna=False)}"
+        f"Series Counts - Device Manufacturers:\n"
+        f"{manufacturers}"
     )
 
+    if format == "var":
+        # Return the variables as a dictionary
+        return {
+            "subjects": subjects,
+            "studies": studies,
+            "series": series,
+            "images": images,
+            "collections": collections,
+            "modalities": modalities,
+            "body_parts": body_parts,
+            "manufacturers": manufacturers
+        }
+    elif format == "file":
+        if filename is None:
+            # Generate default filename based on current date and time
+            current_datetime = datetime.now().strftime("%Y%m%d-%H%M%S")
+            filename = f"seriesReport-{current_datetime}.txt"
+
+        # Save the report to a text file
+        with open(filename, "w") as file:
+            file.write(report)
+        print(f"Report saved to {filename}.")
+    else:
+        _log.info(report)
+
 ####### manifestToList function
 # Ingests a TCIA manifest file and removes header
 # Returns a list of series UIDs
 
 def manifestToList(manifest):
 
     # initialize variable
@@ -1318,13 +1389,12 @@
 
             image += np.int16(intercept)
 
         pixel_data = np.array(image, dtype=np.int16)
 
         # slide through dicom images using a slide bar
         def dicom_animation(x):
-            plt.figure(figsize=[10,10])
             plt.imshow(pixel_data[x], cmap = plt.cm.gray)
-            return x
+            plt.show()
         interact(dicom_animation, x=(0, len(pixel_data)-1))
     else:
         seriesInvalid(seriesUid)
```

### Comparing `tcia_utils-1.3.1/.gitignore` & `tcia_utils-1.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.3.1/LICENSE` & `tcia_utils-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.3.1/README.md` & `tcia_utils-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.3.1/pyproject.toml` & `tcia_utils-1.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tcia_utils"
-version = "1.3.1"
+version = "1.3.2"
 authors = [
   { name="Justin Kirby", email="justin.kirby@nih.gov" },
 ]
 description = "A package to simplify common tasks one might perform when interacting with The Cancer Imaging Archive (TCIA) via Jupyter/Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `tcia_utils-1.3.1/PKG-INFO` & `tcia_utils-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcia_utils
-Version: 1.3.1
+Version: 1.3.2
 Summary: A package to simplify common tasks one might perform when interacting with The Cancer Imaging Archive (TCIA) via Jupyter/Python.
 Project-URL: Homepage, https://github.com/kirbyju/tcia_utils
 Project-URL: Bug Tracker, https://github.com/kirbyju/tcia_utils/issues
 Author-email: Justin Kirby <justin.kirby@nih.gov>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

