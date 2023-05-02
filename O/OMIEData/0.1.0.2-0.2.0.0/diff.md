# Comparing `tmp/OMIEData-0.1.0.2.tar.gz` & `tmp/OMIEData-0.2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OMIEData-0.1.0.2.tar", last modified: Sat Apr 29 23:48:01 2023, max compression
+gzip compressed data, was "OMIEData-0.2.0.0.tar", last modified: Tue May  2 20:58:45 2023, max compression
```

## Comparing `OMIEData-0.1.0.2.tar` & `OMIEData-0.2.0.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 23:48:01.057333 OMIEData-0.1.0.2/
--rw-rw-rw-   0        0        0     1091 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/LICENSE
-drwxrwxrwx   0        0        0        0 2023-04-29 23:48:00.988201 OMIEData-0.1.0.2/OMIEData/
-drwxrwxrwx   0        0        0        0 2023-04-29 23:48:01.015313 OMIEData-0.1.0.2/OMIEData/DataImport/
--rw-rw-rw-   0        0        0        0 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/DataImport/__init__.py
--rw-rw-rw-   0        0        0      131 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/DataImport/omie_data_importer.py
--rw-rw-rw-   0        0        0     1155 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/DataImport/omie_data_importer_from_folder.py
--rw-rw-rw-   0        0        0     1481 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/DataImport/omie_data_importer_from_responses.py
--rw-rw-rw-   0        0        0      793 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/DataImport/omie_energy_by_technology_importer.py
--rw-rw-rw-   0        0        0      655 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/DataImport/omie_marginalprice_importer.py
--rw-rw-rw-   0        0        0     1027 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/DataImport/omie_supply_demand_curve_importer.py
-drwxrwxrwx   0        0        0        0 2023-04-29 23:48:01.029233 OMIEData-0.1.0.2/OMIEData/Downloaders/
--rw-rw-rw-   0        0        0        0 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/Downloaders/__init__.py
--rw-rw-rw-   0        0        0      842 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/Downloaders/energy_by_technology_downloader.py
--rw-rw-rw-   0        0        0     2332 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/Downloaders/general_omie_downloader.py
--rw-rw-rw-   0        0        0      754 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/Downloaders/intra_day_price_downloader.py
--rw-rw-rw-   0        0        0      483 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/Downloaders/marginal_price_downloader.py
--rw-rw-rw-   0        0        0      331 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/Downloaders/omie_downloader.py
--rw-rw-rw-   0        0        0      680 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/Downloaders/supply_demand_curve_downloader.py
-drwxrwxrwx   0        0        0        0 2023-04-29 23:48:01.033169 OMIEData-0.1.0.2/OMIEData/Enums/
--rw-rw-rw-   0        0        0        0 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/Enums/__init__.py
--rw-rw-rw-   0        0        0     2037 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/Enums/all_enums.py
-drwxrwxrwx   0        0        0        0 2023-04-29 23:48:01.046944 OMIEData-0.1.0.2/OMIEData/FileReaders/
--rw-rw-rw-   0        0        0        0 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/FileReaders/__init__.py
--rw-rw-rw-   0        0        0        6 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/FileReaders/data_types_energy_by_technology.py
--rw-rw-rw-   0        0        0        6 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/FileReaders/data_types_marginal_price_file.py
--rw-rw-rw-   0        0        0     2433 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/FileReaders/energy_by_technology_files_reader.py
--rw-rw-rw-   0        0        0     6005 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/FileReaders/marginal_price_file_reader.py
--rw-rw-rw-   0        0        0      316 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/FileReaders/omie_file_reader.py
--rw-rw-rw-   0        0        0     1718 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/FileReaders/supply_demand_curve_file_reader.py
--rw-rw-rw-   0        0        0        0 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/OMIEData/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 23:48:01.000664 OMIEData-0.1.0.2/OMIEData.egg-info/
--rw-rw-rw-   0        0        0     5818 2023-04-29 23:48:00.000000 OMIEData-0.1.0.2/OMIEData.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1464 2023-04-29 23:48:00.000000 OMIEData-0.1.0.2/OMIEData.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 23:48:00.000000 OMIEData-0.1.0.2/OMIEData.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-04-29 23:48:00.000000 OMIEData-0.1.0.2/OMIEData.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-29 23:48:00.000000 OMIEData-0.1.0.2/OMIEData.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5818 2023-04-29 23:48:01.056239 OMIEData-0.1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5257 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-29 23:48:01.058333 OMIEData-0.1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      878 2023-04-29 23:47:27.000000 OMIEData-0.1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-29 23:48:01.048944 OMIEData-0.1.0.2/tests/
--rw-rw-rw-   0        0        0        0 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 23:48:01.054239 OMIEData-0.1.0.2/tests/filereaders_tests/
--rw-rw-rw-   0        0        0        0 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/tests/filereaders_tests/__init__.py
--rw-rw-rw-   0        0        0      893 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/tests/filereaders_tests/energy_by_technology_reader_test.py
--rw-rw-rw-   0        0        0    10294 2023-04-29 20:49:20.000000 OMIEData-0.1.0.2/tests/filereaders_tests/marginal_pricer_reader_test.py
+drwxrwxrwx   0        0        0        0 2023-05-02 20:58:45.436281 OMIEData-0.2.0.0/
+-rw-rw-rw-   0        0        0     1091 2023-04-29 20:49:20.000000 OMIEData-0.2.0.0/LICENSE
+drwxrwxrwx   0        0        0        0 2023-05-02 20:58:45.255739 OMIEData-0.2.0.0/OMIEData/
+drwxrwxrwx   0        0        0        0 2023-05-02 20:58:45.319584 OMIEData-0.2.0.0/OMIEData/DataImport/
+-rw-rw-rw-   0        0        0        0 2023-04-29 20:49:20.000000 OMIEData-0.2.0.0/OMIEData/DataImport/__init__.py
+-rw-rw-rw-   0        0        0      131 2023-04-29 20:49:20.000000 OMIEData-0.2.0.0/OMIEData/DataImport/omie_data_importer.py
+-rw-rw-rw-   0        0        0     1163 2023-05-02 20:39:20.000000 OMIEData-0.2.0.0/OMIEData/DataImport/omie_data_importer_from_folder.py
+-rw-rw-rw-   0        0        0     1488 2023-05-02 20:42:01.000000 OMIEData-0.2.0.0/OMIEData/DataImport/omie_data_importer_from_responses.py
+-rw-rw-rw-   0        0        0      793 2023-04-29 20:49:20.000000 OMIEData-0.2.0.0/OMIEData/DataImport/omie_energy_by_technology_importer.py
+-rw-rw-rw-   0        0        0      655 2023-04-29 20:49:20.000000 OMIEData-0.2.0.0/OMIEData/DataImport/omie_marginalprice_importer.py
+-rw-rw-rw-   0        0        0     1027 2023-04-29 20:49:20.000000 OMIEData-0.2.0.0/OMIEData/DataImport/omie_supply_demand_curve_importer.py
+drwxrwxrwx   0        0        0        0 2023-05-02 20:58:45.373808 OMIEData-0.2.0.0/OMIEData/Downloaders/
+-rw-rw-rw-   0        0        0        0 2023-04-29 20:49:20.000000 OMIEData-0.2.0.0/OMIEData/Downloaders/__init__.py
+-rw-rw-rw-   0        0        0      842 2023-04-29 20:49:20.000000 OMIEData-0.2.0.0/OMIEData/Downloaders/energy_by_technology_downloader.py
+-rw-rw-rw-   0        0        0     2332 2023-04-29 20:49:20.000000 OMIEData-0.2.0.0/OMIEData/Downloaders/general_omie_downloader.py
+-rw-rw-rw-   0        0        0      754 2023-04-29 20:49:20.000000 OMIEData-0.2.0.0/OMIEData/Downloaders/intra_day_price_downloader.py
+-rw-rw-rw-   0        0        0      483 2023-04-29 20:49:20.000000 OMIEData-0.2.0.0/OMIEData/Downloaders/marginal_price_downloader.py
+-rw-rw-rw-   0        0        0      331 2023-04-29 20:49:20.000000 OMIEData-0.2.0.0/OMIEData/Downloaders/omie_downloader.py
+-rw-rw-rw-   0        0        0      680 2023-04-29 20:49:20.000000 OMIEData-0.2.0.0/OMIEData/Downloaders/supply_demand_curve_downloader.py
+drwxrwxrwx   0        0        0        0 2023-05-02 20:58:45.384917 OMIEData-0.2.0.0/OMIEData/Enums/
+-rw-rw-rw-   0        0        0        0 2023-04-29 20:49:20.000000 OMIEData-0.2.0.0/OMIEData/Enums/__init__.py
+-rw-rw-rw-   0        0        0     2037 2023-04-29 20:49:20.000000 OMIEData-0.2.0.0/OMIEData/Enums/all_enums.py
+drwxrwxrwx   0        0        0        0 2023-05-02 20:58:45.419354 OMIEData-0.2.0.0/OMIEData/FileReaders/
+-rw-rw-rw-   0        0        0        0 2023-04-29 20:49:20.000000 OMIEData-0.2.0.0/OMIEData/FileReaders/__init__.py
+-rw-rw-rw-   0        0        0        6 2023-04-29 20:49:20.000000 OMIEData-0.2.0.0/OMIEData/FileReaders/data_types_energy_by_technology.py
+-rw-rw-rw-   0        0        0        6 2023-04-29 20:49:20.000000 OMIEData-0.2.0.0/OMIEData/FileReaders/data_types_marginal_price_file.py
+-rw-rw-rw-   0        0        0     2433 2023-04-29 20:49:20.000000 OMIEData-0.2.0.0/OMIEData/FileReaders/energy_by_technology_files_reader.py
+-rw-rw-rw-   0        0        0     6056 2023-05-02 20:29:55.000000 OMIEData-0.2.0.0/OMIEData/FileReaders/marginal_price_file_reader.py
+-rw-rw-rw-   0        0        0      316 2023-04-29 20:49:20.000000 OMIEData-0.2.0.0/OMIEData/FileReaders/omie_file_reader.py
+-rw-rw-rw-   0        0        0     1718 2023-04-29 20:49:20.000000 OMIEData-0.2.0.0/OMIEData/FileReaders/supply_demand_curve_file_reader.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 20:49:20.000000 OMIEData-0.2.0.0/OMIEData/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 20:58:45.278098 OMIEData-0.2.0.0/OMIEData.egg-info/
+-rw-rw-rw-   0        0        0     5819 2023-05-02 20:58:45.000000 OMIEData-0.2.0.0/OMIEData.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1464 2023-05-02 20:58:45.000000 OMIEData-0.2.0.0/OMIEData.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 20:58:45.000000 OMIEData-0.2.0.0/OMIEData.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-05-02 20:58:45.000000 OMIEData-0.2.0.0/OMIEData.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-02 20:58:45.000000 OMIEData-0.2.0.0/OMIEData.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5819 2023-05-02 20:58:45.435281 OMIEData-0.2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5257 2023-04-29 20:49:20.000000 OMIEData-0.2.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-02 20:58:45.436281 OMIEData-0.2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      879 2023-05-02 20:57:30.000000 OMIEData-0.2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 20:58:45.421716 OMIEData-0.2.0.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-29 20:49:20.000000 OMIEData-0.2.0.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 20:58:45.433502 OMIEData-0.2.0.0/tests/filereaders_tests/
+-rw-rw-rw-   0        0        0        0 2023-04-29 20:49:20.000000 OMIEData-0.2.0.0/tests/filereaders_tests/__init__.py
+-rw-rw-rw-   0        0        0      893 2023-04-29 20:49:20.000000 OMIEData-0.2.0.0/tests/filereaders_tests/energy_by_technology_reader_test.py
+-rw-rw-rw-   0        0        0    10294 2023-04-29 20:49:20.000000 OMIEData-0.2.0.0/tests/filereaders_tests/marginal_pricer_reader_test.py
```

### Comparing `OMIEData-0.1.0.2/LICENSE` & `OMIEData-0.2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `OMIEData-0.1.0.2/OMIEData/DataImport/omie_data_importer_from_folder.py` & `OMIEData-0.2.0.0/OMIEData/DataImport/omie_data_importer_from_folder.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,16 +15,17 @@
 
         # List all the files in the directory
         filenames = [f for f in os.listdir(self.folder) if os.path.isfile(os.path.join(self.folder, f))]
 
         df = pd.DataFrame(columns=self.fileReader.get_keys())
         for f in filenames:
             try:
-                df = df.append(self.fileReader.get_data_from_file(filename=os.path.join(self.folder, f)),
+                df = pd.concat([df, self.fileReader.get_data_from_file(filename=os.path.join(self.folder, f))],
                                ignore_index=True)
+
             except Exception as exc:
                 print('There was error processing file: ' + f)
                 print('{}'.format(exc) + f)
             else:
                 if verbose:
                     print('File: ' + f + ' successfully processed')
```

### Comparing `OMIEData-0.1.0.2/OMIEData/DataImport/omie_data_importer_from_responses.py` & `OMIEData-0.2.0.0/OMIEData/DataImport/omie_data_importer_from_responses.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,15 +22,16 @@
     def read_to_dataframe(self, verbose=False) -> pd.DataFrame:
 
         df = pd.DataFrame(columns=self.fileReader.get_keys())
         for response in self.fileDownloader.url_responses(date_ini=self.date_ini,
                                                           date_end=self.date_end,
                                                           verbose=verbose):
             try:
-                df = df.append(self.fileReader.get_data_from_response(response=response), ignore_index=True)
+                df = df.concat([df, self.fileReader.get_data_from_response(response=response)],ignore_index=True)
+
             except Exception as exc:
                 print('There was error processing file: ' + response.url)
                 print('{}'.format(exc) + response.url)
             else:
                 if verbose:
                     print('Url: ' + response.url + ' successfully processed')
```

### Comparing `OMIEData-0.1.0.2/OMIEData/DataImport/omie_energy_by_technology_importer.py` & `OMIEData-0.2.0.0/OMIEData/DataImport/omie_energy_by_technology_importer.py`

 * *Files identical despite different names*

### Comparing `OMIEData-0.1.0.2/OMIEData/DataImport/omie_marginalprice_importer.py` & `OMIEData-0.2.0.0/OMIEData/DataImport/omie_marginalprice_importer.py`

 * *Files identical despite different names*

### Comparing `OMIEData-0.1.0.2/OMIEData/DataImport/omie_supply_demand_curve_importer.py` & `OMIEData-0.2.0.0/OMIEData/DataImport/omie_supply_demand_curve_importer.py`

 * *Files identical despite different names*

### Comparing `OMIEData-0.1.0.2/OMIEData/Downloaders/energy_by_technology_downloader.py` & `OMIEData-0.2.0.0/OMIEData/Downloaders/energy_by_technology_downloader.py`

 * *Files identical despite different names*

### Comparing `OMIEData-0.1.0.2/OMIEData/Downloaders/general_omie_downloader.py` & `OMIEData-0.2.0.0/OMIEData/Downloaders/general_omie_downloader.py`

 * *Files identical despite different names*

### Comparing `OMIEData-0.1.0.2/OMIEData/Downloaders/intra_day_price_downloader.py` & `OMIEData-0.2.0.0/OMIEData/Downloaders/intra_day_price_downloader.py`

 * *Files identical despite different names*

### Comparing `OMIEData-0.1.0.2/OMIEData/Downloaders/supply_demand_curve_downloader.py` & `OMIEData-0.2.0.0/OMIEData/Downloaders/supply_demand_curve_downloader.py`

 * *Files identical despite different names*

### Comparing `OMIEData-0.1.0.2/OMIEData/Enums/all_enums.py` & `OMIEData-0.2.0.0/OMIEData/Enums/all_enums.py`

 * *Files identical despite different names*

### Comparing `OMIEData-0.1.0.2/OMIEData/FileReaders/energy_by_technology_files_reader.py` & `OMIEData-0.2.0.0/OMIEData/FileReaders/energy_by_technology_files_reader.py`

 * *Files identical despite different names*

### Comparing `OMIEData-0.1.0.2/OMIEData/FileReaders/marginal_price_file_reader.py` & `OMIEData-0.2.0.0/OMIEData/FileReaders/marginal_price_file_reader.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,17 +30,17 @@
             [DataTypeInMarginalPriceFile.ENERGY_IBERIAN, 1.0],
         'Energía total del mercado Ibérico (MWh)':
             [DataTypeInMarginalPriceFile.ENERGY_IBERIAN, 1.0],
         'Energía total con bilaterales del mercado Ibérico (MWh)':
             [DataTypeInMarginalPriceFile.ENERGY_IBERIAN_WITH_BILLATERAL, 1.0]}
 
     __key_list_retrieve__ = ['DATE', 'CONCEPT',
-                             'H1', 'H2', 'H3', 'H4','H5', 'H6','H7', 'H8','H9','H10',
-                             'H11', 'H12','H13', 'H14','H15', 'H16','H17', 'H18','H19','H20',
-                             'H21', 'H22','H23', 'H24']
+                             'H1', 'H2', 'H3', 'H4','H5', 'H6', 'H7', 'H8','H9','H10',
+                             'H11', 'H12', 'H13', 'H14', 'H15', 'H16', 'H17', 'H18', 'H19', 'H20',
+                             'H21', 'H22', 'H23', 'H24']
 
     __dateFormatInFile__ = '%d/%m/%Y'
     __localeInFile__ = "en_DK.UTF-8"
 
     def __init__(self, types=None):
         self.conceptsToLoad = [v for v in DataTypeInMarginalPriceFile] if not types else types
 
@@ -71,15 +71,15 @@
                 if first_col in MarginalPriceFileReader.__dic_static_concepts__.keys():
                     concept_type = MarginalPriceFileReader.__dic_static_concepts__[first_col][0]
 
                     if concept_type in self.conceptsToLoad:
                         units = MarginalPriceFileReader.__dic_static_concepts__[first_col][1]
 
                         dico = self._process_line(date=date, concept=concept_type, values=splits[1:], multiplier=units)
-                        res = res.append(dico, ignore_index=True)
+                        res = pd.concat([res, pd.DataFrame([dico])], ignore_index=True)
 
             return res
 
     def get_data_from_file(self, filename: str) -> pd.DataFrame:
 
         # Method yield each dictionary one by one
         res = pd.DataFrame(columns=self.get_keys())
@@ -104,15 +104,15 @@
                 if first_col in MarginalPriceFileReader.__dic_static_concepts__.keys():
                     concept_type = MarginalPriceFileReader.__dic_static_concepts__[first_col][0]
 
                     if concept_type in self.conceptsToLoad:
                         units = MarginalPriceFileReader.__dic_static_concepts__[first_col][1]
 
                         dico = self._process_line(date=date, concept=concept_type, values=splits[1:], multiplier=units)
-                        res = res.append(dico, ignore_index=True)
+                        res = pd.concat([res, pd.DataFrame([dico])], ignore_index=True)
 
             return res
 
     def _process_line(self, date: dt.date, concept: DataTypeInMarginalPriceFile, values: list, multiplier=1.0) -> dict:
 
         key_list = MarginalPriceFileReader.__key_list_retrieve__
```

### Comparing `OMIEData-0.1.0.2/OMIEData/FileReaders/supply_demand_curve_file_reader.py` & `OMIEData-0.2.0.0/OMIEData/FileReaders/supply_demand_curve_file_reader.py`

 * *Files identical despite different names*

### Comparing `OMIEData-0.1.0.2/OMIEData.egg-info/PKG-INFO` & `OMIEData-0.2.0.0/OMIEData.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: OMIEData
-Version: 0.1.0.2
+Version: 0.2.0.0
 Summary: Package to download electricity time series from https://www.omie.es/
 Home-page: https://github.com/acruzgarcia/OMIEData
 Author: Alberto Cruz and Mirel Mora
 Author-email: a.cruz.garcia@gmail.com, mirel.mora@gmail.com
 Keywords: OMIE,Electricity prices
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OMIEData: 
 
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 [![PyPI version fury.io](https://img.shields.io/pypi/v/OMIEData.svg)](https://pypi.org/project/OMIEData/)
```

### Comparing `OMIEData-0.1.0.2/OMIEData.egg-info/SOURCES.txt` & `OMIEData-0.2.0.0/OMIEData.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OMIEData-0.1.0.2/PKG-INFO` & `OMIEData-0.2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: OMIEData
-Version: 0.1.0.2
+Version: 0.2.0.0
 Summary: Package to download electricity time series from https://www.omie.es/
 Home-page: https://github.com/acruzgarcia/OMIEData
 Author: Alberto Cruz and Mirel Mora
 Author-email: a.cruz.garcia@gmail.com, mirel.mora@gmail.com
 Keywords: OMIE,Electricity prices
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OMIEData: 
 
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 [![PyPI version fury.io](https://img.shields.io/pypi/v/OMIEData.svg)](https://pypi.org/project/OMIEData/)
```

### Comparing `OMIEData-0.1.0.2/README.md` & `OMIEData-0.2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `OMIEData-0.1.0.2/setup.py` & `OMIEData-0.2.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="OMIEData",
-    version="0.1.0.2",
+    version="0.2.0.0",
     author="Alberto Cruz and Mirel Mora",
     author_email="a.cruz.garcia@gmail.com, mirel.mora@gmail.com",
     description="Package to download electricity time series from https://www.omie.es/",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/acruzgarcia/OMIEData",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=setuptools.find_packages(),
-    python_requires='>=3.6',
+    python_requires='>=3.11',
     keywords=['OMIE', 'Electricity prices'],
-    install_requires=['pandas<=1.5.3', 'requests', 'datetime']
+    install_requires=['pandas>=2.0.1', 'requests', 'datetime']
 )
```

### Comparing `OMIEData-0.1.0.2/tests/filereaders_tests/energy_by_technology_reader_test.py` & `OMIEData-0.2.0.0/tests/filereaders_tests/energy_by_technology_reader_test.py`

 * *Files identical despite different names*

### Comparing `OMIEData-0.1.0.2/tests/filereaders_tests/marginal_pricer_reader_test.py` & `OMIEData-0.2.0.0/tests/filereaders_tests/marginal_pricer_reader_test.py`

 * *Files identical despite different names*

