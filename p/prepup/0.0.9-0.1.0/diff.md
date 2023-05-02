# Comparing `tmp/prepup-0.0.9.tar.gz` & `tmp/prepup-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prepup-0.0.9.tar", last modified: Mon May  1 01:53:26 2023, max compression
+gzip compressed data, was "prepup-0.1.0.tar", last modified: Tue May  2 13:55:36 2023, max compression
```

## Comparing `prepup-0.0.9.tar` & `prepup-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 01:53:26.715836 prepup-0.0.9/
--rw-rw-rw-   0        0        0      188 2023-04-29 20:41:27.000000 prepup-0.0.9/AUTHORS.rst
--rw-rw-rw-   0        0        0     1100 2023-04-29 20:41:27.000000 prepup-0.0.9/LICENSE
--rw-rw-rw-   0        0        0      129 2023-04-29 20:41:27.000000 prepup-0.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0      493 2023-05-01 01:53:26.713902 prepup-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      489 2023-04-29 20:41:27.000000 prepup-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 01:53:26.685939 prepup-0.0.9/prepup/
--rw-rw-rw-   0        0        0     5350 2023-05-01 01:45:53.000000 prepup-0.0.9/prepup/__init__.py
--rw-rw-rw-   0        0        0    27778 2023-05-01 01:52:39.000000 prepup-0.0.9/prepup/common.py
-drwxrwxrwx   0        0        0        0 2023-05-01 01:53:26.703529 prepup-0.0.9/prepup.egg-info/
--rw-rw-rw-   0        0        0      493 2023-05-01 01:53:26.000000 prepup-0.0.9/prepup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-05-01 01:53:26.000000 prepup-0.0.9/prepup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 01:53:26.000000 prepup-0.0.9/prepup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-05-01 01:53:26.000000 prepup-0.0.9/prepup.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      170 2023-05-01 01:53:26.000000 prepup-0.0.9/prepup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-01 01:53:26.000000 prepup-0.0.9/prepup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      367 2023-04-29 23:00:31.000000 prepup-0.0.9/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 01:53:26.715836 prepup-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     3159 2023-05-01 01:53:20.000000 prepup-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 01:53:26.709977 prepup-0.0.9/tests/
--rw-rw-rw-   0        0        0       37 2023-04-29 20:41:27.000000 prepup-0.0.9/tests/__init__.py
--rw-rw-rw-   0        0        0      403 2023-04-29 20:41:27.000000 prepup-0.0.9/tests/test_prepup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:55:36.821316 prepup-0.1.0/
+-rw-rw-rw-   0        0        0      188 2023-04-29 20:41:27.000000 prepup-0.1.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1100 2023-04-29 20:41:27.000000 prepup-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      129 2023-04-29 20:41:27.000000 prepup-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      493 2023-05-02 13:55:36.821316 prepup-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2023-04-29 20:41:27.000000 prepup-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 13:55:36.804796 prepup-0.1.0/prepup/
+-rw-rw-rw-   0        0        0     5350 2023-05-01 01:45:53.000000 prepup-0.1.0/prepup/__init__.py
+-rw-rw-rw-   0        0        0    27125 2023-05-02 13:54:26.000000 prepup-0.1.0/prepup/common.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:55:36.813246 prepup-0.1.0/prepup.egg-info/
+-rw-rw-rw-   0        0        0      493 2023-05-02 13:55:36.000000 prepup-0.1.0/prepup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-05-02 13:55:36.000000 prepup-0.1.0/prepup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 13:55:36.000000 prepup-0.1.0/prepup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-02 13:55:36.000000 prepup-0.1.0/prepup.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      220 2023-05-02 13:55:36.000000 prepup-0.1.0/prepup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-02 13:55:36.000000 prepup-0.1.0/prepup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      367 2023-04-29 23:00:31.000000 prepup-0.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 13:55:36.821316 prepup-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     3184 2023-05-02 13:55:33.000000 prepup-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:55:36.821316 prepup-0.1.0/tests/
+-rw-rw-rw-   0        0        0       37 2023-04-29 20:41:27.000000 prepup-0.1.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      403 2023-04-29 20:41:27.000000 prepup-0.1.0/tests/test_prepup.py
```

### Comparing `prepup-0.0.9/LICENSE` & `prepup-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prepup-0.0.9/prepup/__init__.py` & `prepup-0.1.0/prepup/__init__.py`

 * *Files identical despite different names*

### Comparing `prepup-0.0.9/prepup/common.py` & `prepup-0.1.0/prepup/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,128 +37,128 @@
         The features_available function returns a list of the features available in the dataframe.
                 
         
         :param self: Represent the instance of the class
         :return: A list of the column names in the dataframe
         :author: Neokai
         """
-        try:
-            return self.dataframe.columns
-        except:
-            print("Something went wrong...\nCouldn't intialize the dataset properly...")
+        #try:
+        return self.dataframe.columns
+        #except:
+            #print("Something went wrong...\nCouldn't intialize the dataset properly...")
 
     def dtype_features(self):
         """
         The dtype_features function returns the data types of each feature in the dataset.
             This is useful for determining which features are categorical and which are numerical.
         
         :param self: Represent the instance of the class
         :return: A series with the data type of each feature (column) in a pandas dataframe
         :author: Neokai
         """
-        try:
-            return self.dataframe.dtypes
-        except:
-            print("Something went wrong....\nCouldn't display DataTypes of Features...")
+        # try:
+        return self.dataframe.dtypes
+        # except:
+        #     print("Something went wrong....\nCouldn't display DataTypes of Features...")
 
     def missing_values(self):
         """
         The missing_values function returns the number of missing values in each column.
             Args:
                 self (DataFrame): The DataFrame object to be analyzed.
             Returns:
                 A dictionary with the columns as keys and their respective null counts as values.
         
         :param self: Represent the instance of the class
         :return: The number of missing values in each column
         :author: Neokai
         """
-        try:
-            if self.dataframe.is_empty() == True:
-                print("No Missing Value Found")
-            else:
-                missing_value = self.dataframe.null_count()
-                return missing_value
-        except:
-            print("Something went wrong....\nChecking Dataset: Recommended.\nPlease try again")
+        #try:
+        if self.dataframe.is_empty() == True:
+            print("No Missing Value Found")
+        else:
+            missing_value = self.dataframe.null_count()
+            return missing_value
+        # except:
+        #     print("Something went wrong....\nChecking Dataset: Recommended.\nPlease try again")
     
     def shape_data(self):
         """
         The shape_data function returns the shape of the dataframe.
                 :return: The shape of the dataframe as a tuple (rows, columns)
         
         :param self: Represent the instance of the class
         :return: The shape of the dataframe
         :author: Neokai
         """
-        try:
-            return self.dataframe.shape
-        except:
-            print("Something went wrong....\nChecking Dataset: Recommended.\nPlease try again")
+        #try:
+        return self.dataframe.shape
+        # except:
+        #     print("Something went wrong....\nChecking Dataset: Recommended.\nPlease try again")
     
     def missing_plot(self):
         """
         The missing_plot function takes in a dataframe and plots the missing values for each column.
             It also prints out the number of missing values for each column.
         
         :param self: Represent the instance of the class
         :return: The number of missing values for each column in the dataframe
         :author: Neokai
         """
-        try:
-            empty_count = 0
-            non_empty_count = 0
-            for column in self.dataframe.columns:
-                val = self.dataframe.select(pl.col([column]).is_null().any())
-                if val[column][0] == True:
-                    empty_count += 1
-                else:
-                    non_empty_count += 1
-            if empty_count == 0:
-                print(colored(term_font.renderText("No Missing Value Found"), 'green+'))
-                #print("No Missing Value Found")
+        #try:
+        empty_count = 0
+        non_empty_count = 0
+        for column in self.dataframe.columns:
+            val = self.dataframe.select(pl.col([column]).is_null().any())
+            if val[column][0] == True:
+                empty_count += 1
             else:
-                missing_counts = self.dataframe.null_count()
-                missing_counts = missing_counts.to_dicts()
-                df = pd.DataFrame(missing_counts)
-                melt_df = pd.melt(df, value_vars=df.columns)
-                melt_df.columns = ['Features', 'Missing_Value_Count']
-                df_new = melt_df.loc[melt_df['Missing_Value_Count'] != 0]
-                print(df_new,"\n")
-                tpl.simple_bar(df_new['Features'], df_new['Missing_Value_Count'], width=100, title='Missing Value Count in Each Feature', color='red+')
-                tpl.theme('matrix')
-                tpl.show()
-                tpl.clear_data()
-        except:
-            print("Something went wrong....\nFailed to fetch missing value count.\nPlease try again...")
+                non_empty_count += 1
+        if empty_count == 0:
+            print(colored(term_font.renderText("No Missing Value Found"), 'green+'))
+            #print("No Missing Value Found")
+        else:
+            missing_counts = self.dataframe.null_count()
+            missing_counts = missing_counts.to_dicts()
+            df = pd.DataFrame(missing_counts)
+            melt_df = pd.melt(df, value_vars=df.columns)
+            melt_df.columns = ['Features', 'Missing_Value_Count']
+            df_new = melt_df.loc[melt_df['Missing_Value_Count'] != 0]
+            print(df_new,"\n")
+            tpl.simple_bar(df_new['Features'], df_new['Missing_Value_Count'], width=100, title='Missing Value Count in Each Feature', color='red+')
+            tpl.theme('matrix')
+            tpl.show()
+            tpl.clear_data()
+        # except:
+        #     print("Something went wrong....\nFailed to fetch missing value count.\nPlease try again...")
             
     def plot_histogram(self):
         """
         The plot_histogram function plots a histogram for each numerical column in the dataframe.
             The function takes no arguments and returns nothing.
         
         :param self: Represent the instance of the class
         :return: A histogram for each of the columns in the dataframe
         :author: Neokai
         """
-        try:
-            dataframe = self.dataframe.fill_null(0)
-            for column in self.dataframe.columns:
-                if dataframe[column].dtype != pl.Categorical and dataframe[column].dtype != pl.Utf8 and dataframe[column].dtype != pl.Boolean and dataframe[column].dtype != pl.Null and dataframe[column].dtype != pl.Object and dataframe[column].dtype != pl.Unknown:
-                    tpl.clear_data()
-                    tpl.theme('dark')
-                    tpl.plotsize(80,20)
-                    print("\n")
-                    tpl.hist(dataframe[column], bins=20,color='light-blue', marker='dot') #color=46)
-                    tpl.title(column)
-                    #tpl.grid(horizontal=50, vertical=50)
-                    tpl.show()
-                    tpl.clear_data()
-        except:
-            print("Something went wrong....\nFailed to fetch feature distribution...\nPlease try again...")
+        #try:
+        dataframe = self.dataframe.fill_null(0)
+        for column in self.dataframe.columns:
+            if dataframe[column].dtype != pl.Categorical and dataframe[column].dtype != pl.Utf8 and dataframe[column].dtype != pl.Boolean and dataframe[column].dtype != pl.Null and dataframe[column].dtype != pl.Object and dataframe[column].dtype != pl.Unknown:
+                tpl.clear_data()
+                tpl.theme('dark')
+                tpl.plotsize(80,20)
+                print("\n")
+                tpl.hist(dataframe[column], bins=20,color='light-blue', marker='dot') #color=46)
+                tpl.title(column)
+                #tpl.grid(horizontal=50, vertical=50)
+                tpl.show()
+                tpl.clear_data()
+        # except:
+        #     print("Something went wrong....\nFailed to fetch feature distribution...\nPlease try again...")
 
     
 
     
     def correlation_n(self):
         """
         The correlation_n function takes in a dataframe and returns the correlation between all numerical features.
@@ -166,155 +166,155 @@
             feature pairs and another for their corresponding correlation values. It then uses simple_bar to plot these 
             values as a bar graph.
         
         :param self: Represent the instance of the class
         :return: A bar graph of the correlation between all numerical features in the dataset
         :author: Neokai
         """
-        try:
-            dtype_select_df = self.dataframe.select([pl.col(pl.Decimal),pl.col(pl.Float32),pl.col(pl.Float64),pl.col(pl.Int16),pl.col(pl.Int32),pl.col(pl.Int64),pl.col(pl.Int8),pl.col(pl.UInt16),pl.col(pl.UInt32),pl.col(pl.UInt64),pl.col(pl.UInt8),pl.col(pl.Date),pl.col(pl.Datetime),pl.col(pl.Duration),pl.col(pl.Time)])
-            dtype_select_df = dtype_select_df.to_pandas()
-            #corr_d = pd.DataFrame()
-            features = []
-            correlation_val = []
-            for i in dtype_select_df.columns:
-                for j in dtype_select_df.columns:
-                    feature_pair = i,j
-                    features.append(feature_pair)
-                    correlation_val.append(round(dtype_select_df[i].corr(dtype_select_df[j]),2))
-            tpl.simple_bar(features, correlation_val,width=100, title='Correlation Between these Features', color=92,marker='*')
-            tpl.show()
-            tpl.clear_data()
-        except:
-            print("Something went wrong....\nFailed to fetch Correlation Matrix...\nPlease try again...")
+        #try:
+        dtype_select_df = self.dataframe.select([pl.col(pl.Decimal),pl.col(pl.Float32),pl.col(pl.Float64),pl.col(pl.Int16),pl.col(pl.Int32),pl.col(pl.Int64),pl.col(pl.Int8),pl.col(pl.UInt16),pl.col(pl.UInt32),pl.col(pl.UInt64),pl.col(pl.UInt8),pl.col(pl.Date),pl.col(pl.Datetime),pl.col(pl.Duration),pl.col(pl.Time)])
+        dtype_select_df = dtype_select_df.to_pandas()
+        #corr_d = pd.DataFrame()
+        features = []
+        correlation_val = []
+        for i in dtype_select_df.columns:
+            for j in dtype_select_df.columns:
+                feature_pair = i,j
+                features.append(feature_pair)
+                correlation_val.append(round(dtype_select_df[i].corr(dtype_select_df[j]),2))
+        tpl.simple_bar(features, correlation_val,width=100, title='Correlation Between these Features', color=92,marker='*')
+        tpl.show()
+        tpl.clear_data()
+        # except:
+        #     print("Something went wrong....\nFailed to fetch Correlation Matrix...\nPlease try again...")
 
     def scatter_plot(self):
         """
         The scatter_plot function takes the dataframe and selects all columns that are numeric.
         It then creates a scatter plot for each pair of numeric columns in the dataframe.
         
         :param self: Represent the instance of the class
         :return: A scatter plot for each column in the dataframe
         :author: Neokai
         """
-        try:
-            dtype_select_df = self.dataframe.select([pl.col(pl.Decimal),pl.col(pl.Float32),pl.col(pl.Float64),pl.col(pl.Int16),pl.col(pl.Int32),pl.col(pl.Int64),pl.col(pl.Int8),pl.col(pl.UInt16),pl.col(pl.UInt32),pl.col(pl.UInt64),pl.col(pl.UInt8),pl.col(pl.Date),pl.col(pl.Datetime),pl.col(pl.Duration),pl.col(pl.Time)])
-            dtype_select_df = dtype_select_df.to_pandas()
-            for i in dtype_select_df.columns:
-                for j in dtype_select_df.columns:
-                    scatter_p = pd.DataFrame()
-                    scatter_p["value1"] = dtype_select_df[[i]] 
-                    scatter_p["value2"] = dtype_select_df[[j]]
-                    tpl.theme('matrix')
-                    tpl.plotsize(80,20)
-                    tpl.title("\nDistribution of {0} vs {1}".format(i,j))
-                    tpl.scatter(scatter_p["value1"], scatter_p["value2"], color='white')
-                    tpl.show()
-                    tpl.clear_data()
-        except:
-            print("Something went wrong....\nScatter Plot Build Failed...\nPlease try again...")
+        #try:
+        dtype_select_df = self.dataframe.select([pl.col(pl.Decimal),pl.col(pl.Float32),pl.col(pl.Float64),pl.col(pl.Int16),pl.col(pl.Int32),pl.col(pl.Int64),pl.col(pl.Int8),pl.col(pl.UInt16),pl.col(pl.UInt32),pl.col(pl.UInt64),pl.col(pl.UInt8),pl.col(pl.Date),pl.col(pl.Datetime),pl.col(pl.Duration),pl.col(pl.Time)])
+        dtype_select_df = dtype_select_df.to_pandas()
+        for i in dtype_select_df.columns:
+            for j in dtype_select_df.columns:
+                scatter_p = pd.DataFrame()
+                scatter_p["value1"] = dtype_select_df[[i]] 
+                scatter_p["value2"] = dtype_select_df[[j]]
+                tpl.theme('matrix')
+                tpl.plotsize(80,20)
+                tpl.title("\nDistribution of {0} vs {1}".format(i,j))
+                tpl.scatter(scatter_p["value1"], scatter_p["value2"], color='white')
+                tpl.show()
+                tpl.clear_data()
+        # except:
+        #     print("Something went wrong....\nScatter Plot Build Failed...\nPlease try again...")
     
     def find_outliers(self, k=1.5):
         """
         The find_outliers function takes a dataframe and returns the outliers in each column.
             The function uses the interquartile range to determine if a value is an outlier or not.
             The default k value is 1.5, but can be changed by passing in another float as an argument.
         
         :param self: Represent the instance of the class
         :param k: Calculate the iqr (interquartile range)
         :return: A print statement of the outliers detected in each column
         :author: Neokai
         """
-        try:
-            dtype_select_df = self.dataframe.select([pl.col(pl.Decimal),pl.col(pl.Float32),pl.col(pl.Float64),pl.col(pl.Int16),pl.col(pl.Int32),pl.col(pl.Int64),pl.col(pl.Int8),pl.col(pl.UInt16),pl.col(pl.UInt32),pl.col(pl.UInt64),pl.col(pl.UInt8),pl.col(pl.Date),pl.col(pl.Datetime),pl.col(pl.Duration),pl.col(pl.Time)])
-            dtype_select_df = dtype_select_df.to_pandas()
-
-            for i in dtype_select_df.columns:
-                outliers = []
-                q1 = np.percentile(dtype_select_df[i].values, 25)
-                q3 = np.percentile(dtype_select_df[i].values, 75)
-                iqr = q3 - q1
-                lower_bound = q1 - k*iqr
-                upper_bound = q3 + k*iqr
-                for j in dtype_select_df[i].values:
-                    if j < lower_bound or j > upper_bound:
-                        outliers.append(j)
-                print(f"\tOutliers detected in {i}\n")
-        except:
-            print("Something went wrong....\nFailed to Find Outliers...\nPlease try again...")
+        #try:
+        dtype_select_df = self.dataframe.select([pl.col(pl.Decimal),pl.col(pl.Float32),pl.col(pl.Float64),pl.col(pl.Int16),pl.col(pl.Int32),pl.col(pl.Int64),pl.col(pl.Int8),pl.col(pl.UInt16),pl.col(pl.UInt32),pl.col(pl.UInt64),pl.col(pl.UInt8),pl.col(pl.Date),pl.col(pl.Datetime),pl.col(pl.Duration),pl.col(pl.Time)])
+        dtype_select_df = dtype_select_df.to_pandas()
+
+        for i in dtype_select_df.columns:
+            outliers = []
+            q1 = np.percentile(dtype_select_df[i].values, 25)
+            q3 = np.percentile(dtype_select_df[i].values, 75)
+            iqr = q3 - q1
+            lower_bound = q1 - k*iqr
+            upper_bound = q3 + k*iqr
+            for j in dtype_select_df[i].values:
+                if j < lower_bound or j > upper_bound:
+                    outliers.append(j)
+            print(f"\tOutliers detected in {i}\n")
+        # except:
+        #     print("Something went wrong....\nFailed to Find Outliers...\nPlease try again...")
     
     
     def feature_scaling(self):
         """
         The feature_scaling function normalizes the dataframe by subtracting the mean and dividing by standard deviation.
             The function takes in a dataframe as input, drops the target variable if it is specified, 
             converts to pandas dataframe and then performs feature scaling on all columns that are not categorical or boolean. 
             It then saves this normalized dataset as a csv file at user-specified path.
         
         :param self: Represent the instance of the class
         :return: A dataframe with normalized values
         :author: Neokai
         """
-        try:
-            isExist = os.path.exists("missing_data.parquet")
-            if isExist == True:
-                dataframe = pl.read_parquet("missing_data.parquet")
-            else:
-                dataframe = self.dataframe
-            target_col = input("\nEnter the Target variable to drop: (or 'None')")
-            
-            if target_col != "None":
-                df = dataframe.to_pandas()
-                df = df.drop(target_col, axis=1)
-            else:
-                df = dataframe.to_pandas()
-            
-            for column in df.columns:
-                if dataframe[column].dtype != pl.Categorical and dataframe[column].dtype != pl.Utf8 and dataframe[column].dtype != pl.Boolean and dataframe[column].dtype != pl.Null and dataframe[column].dtype != pl.Object and dataframe[column].dtype != pl.Unknown:
-                    scaler = StandardScaler()
-                    df[[column]] = scaler.fit_transform(df[[column]])
-            
-            data_path = input("\nEnter path to save normalized data : ")
-            path = data_path  
-            s = "\\"
-            if s in path:
-                path = path.replace(os.sep, '/')
-                path = path + "/NormalizedData.csv" 
-                path = str(path)
-                print(path)
-            else:
-                path = path + "/NormalizedData.csv"
-            df.to_csv(path)
-            print("\nFeature Normalized and saved succesfully")
-        except:
-            print("Something went wrong....\nFailed to perform Feature Scaling...\nPlease try again...\nImputing missing values recommended.")
+        #try:
+        isExist = os.path.exists("missing_data.parquet")
+        if isExist == True:
+            dataframe = pl.read_parquet("missing_data.parquet")
+        else:
+            dataframe = self.dataframe
+        target_col = input("\nEnter the Target variable to drop: (or 'None')")
+        
+        if target_col != "None":
+            df = dataframe.to_pandas()
+            df = df.drop(target_col, axis=1)
+        else:
+            df = dataframe.to_pandas()
+        
+        for column in df.columns:
+            if dataframe[column].dtype != pl.Categorical and dataframe[column].dtype != pl.Utf8 and dataframe[column].dtype != pl.Boolean and dataframe[column].dtype != pl.Null and dataframe[column].dtype != pl.Object and dataframe[column].dtype != pl.Unknown:
+                scaler = StandardScaler()
+                df[[column]] = scaler.fit_transform(df[[column]])
+        
+        data_path = input("\nEnter path to save normalized data : ")
+        path = data_path  
+        s = "\\"
+        if s in path:
+            path = path.replace(os.sep, '/')
+            path = path + "/NormalizedData.csv" 
+            path = str(path)
+            print(path)
+        else:
+            path = path + "/NormalizedData.csv"
+        df.to_csv(path)
+        print("\nFeature Normalized and saved succesfully")
+        # except:
+        #     print("Something went wrong....\nFailed to perform Feature Scaling...\nPlease try again...\nImputing missing values recommended.")
     
     def check_nomral_distrubution(self):
         """
         The check_nomral_distrubution function checks if the dataframe is normally distributed.
             It does this by using the Shapiro-Wilk test to check for normality. 
             The function will print out a message stating whether or not each column in the dataframe is normally distributed.
         
         :param self: Represent the instance of the class
         :return: The name of the column, whether it is normally distributed or not and its p-value
         :author: Neokai
         """
-        try:
-            dataframe = self.dataframe
-            for column in dataframe.columns:
-                if dataframe[column].dtype != pl.Categorical and dataframe[column].dtype != pl.Utf8 and dataframe[column].dtype != pl.Boolean and dataframe[column].dtype != pl.Null and dataframe[column].dtype != pl.Object and dataframe[column].dtype != pl.Unknown:
-                    stats, p_value = shapiro(dataframe[column])
-                    if p_value > 0.05:
-                        h_8 = Figlet(font='term') 
-                        print(colored(h_8.renderText(f"* {column} is Normally Distributed with a p-value of {p_value:.2f}\n"),'green'))
-                    else:
-                        h_8 = Figlet(font='term')
-                        print(colored(h_8.renderText(f"* {column} doesn't have a Normal Distribution with a p-value of {p_value:.8f} \n"), 'red'))
-        except:
-            print("Something went wrong....\nFailed to perform Feature Scaling...\nPlease try again...")
+        #try:
+        dataframe = self.dataframe
+        for column in dataframe.columns:
+            if dataframe[column].dtype != pl.Categorical and dataframe[column].dtype != pl.Utf8 and dataframe[column].dtype != pl.Boolean and dataframe[column].dtype != pl.Null and dataframe[column].dtype != pl.Object and dataframe[column].dtype != pl.Unknown:
+                stats, p_value = shapiro(dataframe[column])
+                if p_value > 0.05:
+                    h_8 = Figlet(font='term') 
+                    print(colored(h_8.renderText(f"* {column} is Normally Distributed with a p-value of {p_value:.2f}\n"),'green'))
+                else:
+                    h_8 = Figlet(font='term')
+                    print(colored(h_8.renderText(f"* {column} doesn't have a Normal Distribution with a p-value of {p_value:.8f} \n"), 'red'))
+        # except:
+        #     print("Something went wrong....\nFailed to perform Feature Scaling...\nPlease try again...")
 
 
     def imbalanced_dataset(self):    
         """
         The imbalanced_dataset function takes in a dataframe and the target variable as input.
         It then plots a bar graph of the distribution of the target variable.
         
@@ -337,73 +337,73 @@
         The user can choose from a variety of options to impute missing data, or drop it altogether.
         
         
         :param self: Represent the instance of the class
         :return: The dataframe with missing values imputed
         :author: Neokai
         """
-        try:
-            dataframe = self.dataframe
-            print("Choice Available to Impute Missing Data: \n")
-            print("\t1. [Press 1] Drop Missing Data.\n")
-            print("\t2. [Press 2] Impute Missing Data with Specific Value.\n")
-            print("\t3. [Press 3] Impute Missing Data with Mean.\n")
-            print("\t4. [Press 4] Impute Missing Data with Median.\n")
-            print("\t5. [Press 5] Impute Missing Data based on Distribution of each Feature..\n")
-            print("\t6. [Press 6] Impute Missing Data with Fill Forward Strategy.\n")
-            print("\t7. [Press 7] Impute Missing Data with Backward Fill Strategy.\n")
-            print("\t8. [Press 8] Impute Missing Data with Nearest Neighbours (Advisable if dataset has missing values randomly).\n")
-            choice = int(input("\nEnter your choice: "))
-            if choice == 1:
-                dataframe = dataframe.drop_nulls()
-                dataframe.write_parquet("missing_data.parquet")
-            elif choice == 2:
-                mv = int(input("Enter the value to replace missing data: "))
-                dataframe = dataframe.fill_null(mv)
-                dataframe.write_parquet("missing_data.parquet")
-            elif choice == 3:
-                dataframe = dataframe.to_pandas()
-                for column in dataframe.columns:
-                    if dataframe[column].dtype != pl.Categorical and dataframe[column].dtype != pl.Utf8 and dataframe[column].dtype != pl.Boolean and dataframe[column].dtype != pl.Null and dataframe[column].dtype != pl.Object and dataframe[column].dtype != pl.Unknown:
-                        dataframe[column] = dataframe[column].fillna(dataframe[column].mean())
-                dataframe.to_parquet("missing_data.parquet")
-            elif choice == 4:
-                dataframe = dataframe.to_pandas()
-                for column in dataframe.columns:
-                    if dataframe[column].dtype != pl.Categorical and dataframe[column].dtype != pl.Utf8 and dataframe[column].dtype != pl.Boolean and dataframe[column].dtype != pl.Null and dataframe[column].dtype != pl.Object and dataframe[column].dtype != pl.Unknown:
-                        dataframe[column] = dataframe[column].fillna(dataframe[column].median())
-                dataframe.to_parquet("missing_data.parquet")
-            elif choice == 5:
-                dataframe = dataframe.to_pandas()
-                for column in dataframe.columns:
-                    if dataframe[column].dtype != pl.Categorical and dataframe[column].dtype != pl.Utf8 and dataframe[column].dtype != pl.Boolean and dataframe[column].dtype != pl.Null and dataframe[column].dtype != pl.Object and dataframe[column].dtype != pl.Unknown:
-                        mean = dataframe[column].mean()
-                        std = dataframe[column].std()
-                        random_values = np.random.normal(loc=mean, scale=std, size=dataframe[column].isnull().sum())
-                        dataframe[column] = dataframe[column].fillna(pd.Series(random_values,index=dataframe[column][dataframe[column].isnull()].index))
-                dataframe.to_parquet("missing_data.parquet")
-            elif choice == 6:
-                dataframe = dataframe.fill_null(strategy="forward")
-                dataframe.write_parquet("missing_data.parquet")
-            elif choice == 7: 
-                dataframe = dataframe.fill_null(strategy="backward")
-                dataframe.write_parquet("missing_data.parquet")
-            elif choice == 8: 
-                dataframe = dataframe.to_pandas()
-                for column in dataframe.columns:
-                    if dataframe[column].dtype != pl.Categorical and dataframe[column].dtype != pl.Utf8 and dataframe[column].dtype != pl.Boolean and dataframe[column].dtype != pl.Null and dataframe[column].dtype != pl.Object and dataframe[column].dtype != pl.Unknown:
-                        missing_inds = dataframe[column].isnull()
-                        non_missing_inds = ~missing_inds
-                        non_missing_vals = dataframe[column][non_missing_inds]
-                        closest_inds = np.abs(dataframe[column][missing_inds].values - non_missing_vals.values.reshape(-1,1)).argmin(axis=0)
-                        dataframe.loc[missing_inds, column] = non_missing_vals.iloc[closest_inds].values
-                dataframe.to_parquet("missing_data.parquet")
-            print(colored(term_font.renderText("\nDone...")))
-        except:
-            print("Something went wrong....\nFailed to perform Feature Scaling...\nPlease try again...")
+        #try:
+        dataframe = self.dataframe
+        print("Choice Available to Impute Missing Data: \n")
+        print("\t1. [Press 1] Drop Missing Data.\n")
+        print("\t2. [Press 2] Impute Missing Data with Specific Value.\n")
+        print("\t3. [Press 3] Impute Missing Data with Mean.\n")
+        print("\t4. [Press 4] Impute Missing Data with Median.\n")
+        print("\t5. [Press 5] Impute Missing Data based on Distribution of each Feature..\n")
+        print("\t6. [Press 6] Impute Missing Data with Fill Forward Strategy.\n")
+        print("\t7. [Press 7] Impute Missing Data with Backward Fill Strategy.\n")
+        print("\t8. [Press 8] Impute Missing Data with Nearest Neighbours (Advisable if dataset has missing values randomly).\n")
+        choice = int(input("\nEnter your choice: "))
+        if choice == 1:
+            dataframe = dataframe.drop_nulls()
+            dataframe.write_parquet("missing_data.parquet")
+        elif choice == 2:
+            mv = int(input("Enter the value to replace missing data: "))
+            dataframe = dataframe.fill_null(mv)
+            dataframe.write_parquet("missing_data.parquet")
+        elif choice == 3:
+            dataframe = dataframe.to_pandas()
+            for column in dataframe.columns:
+                if dataframe[column].dtype != pl.Categorical and dataframe[column].dtype != pl.Utf8 and dataframe[column].dtype != pl.Boolean and dataframe[column].dtype != pl.Null and dataframe[column].dtype != pl.Object and dataframe[column].dtype != pl.Unknown:
+                    dataframe[column] = dataframe[column].fillna(dataframe[column].mean())
+            dataframe.to_parquet("missing_data.parquet")
+        elif choice == 4:
+            dataframe = dataframe.to_pandas()
+            for column in dataframe.columns:
+                if dataframe[column].dtype != pl.Categorical and dataframe[column].dtype != pl.Utf8 and dataframe[column].dtype != pl.Boolean and dataframe[column].dtype != pl.Null and dataframe[column].dtype != pl.Object and dataframe[column].dtype != pl.Unknown:
+                    dataframe[column] = dataframe[column].fillna(dataframe[column].median())
+            dataframe.to_parquet("missing_data.parquet")
+        elif choice == 5:
+            dataframe = dataframe.to_pandas()
+            for column in dataframe.columns:
+                if dataframe[column].dtype != pl.Categorical and dataframe[column].dtype != pl.Utf8 and dataframe[column].dtype != pl.Boolean and dataframe[column].dtype != pl.Null and dataframe[column].dtype != pl.Object and dataframe[column].dtype != pl.Unknown:
+                    mean = dataframe[column].mean()
+                    std = dataframe[column].std()
+                    random_values = np.random.normal(loc=mean, scale=std, size=dataframe[column].isnull().sum())
+                    dataframe[column] = dataframe[column].fillna(pd.Series(random_values,index=dataframe[column][dataframe[column].isnull()].index))
+            dataframe.to_parquet("missing_data.parquet")
+        elif choice == 6:
+            dataframe = dataframe.fill_null(strategy="forward")
+            dataframe.write_parquet("missing_data.parquet")
+        elif choice == 7: 
+            dataframe = dataframe.fill_null(strategy="backward")
+            dataframe.write_parquet("missing_data.parquet")
+        elif choice == 8: 
+            dataframe = dataframe.to_pandas()
+            for column in dataframe.columns:
+                if dataframe[column].dtype != pl.Categorical and dataframe[column].dtype != pl.Utf8 and dataframe[column].dtype != pl.Boolean and dataframe[column].dtype != pl.Null and dataframe[column].dtype != pl.Object and dataframe[column].dtype != pl.Unknown:
+                    missing_inds = dataframe[column].isnull()
+                    non_missing_inds = ~missing_inds
+                    non_missing_vals = dataframe[column][non_missing_inds]
+                    closest_inds = np.abs(dataframe[column][missing_inds].values - non_missing_vals.values.reshape(-1,1)).argmin(axis=0)
+                    dataframe.loc[missing_inds, column] = non_missing_vals.iloc[closest_inds].values
+            dataframe.to_parquet("missing_data.parquet")
+        print(colored(term_font.renderText("\nDone...")))
+        # except:
+        #     print("Something went wrong....\nFailed to perform Feature Scaling...\nPlease try again...")
 
         
         
 
 class NotebookCreator:
     def __init__(self):
         """
```

### Comparing `prepup-0.0.9/setup.py` & `prepup-0.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,22 +56,22 @@
 #     zip_safe=False,
 # )
 
 import setuptools
 
 setuptools.setup(
     name="prepup",
-    version="0.0.9",
+    version="0.1.0",
     author="Sudhanshu Mukherjee",
     author_email="sudhanshumukherjeexx@gmail.com",
     description="Prepup is a free, open-source package that lets you open, explore, visualize, and pre-process datasets in your Computer's Terminal.",
     packages=setuptools.find_packages(),
     entry_points={
         "console_scripts": [
-            "prepup = prepup:main",
+            "prepup = prepup.__init__:main",
         ]
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
@@ -82,21 +82,22 @@
         "termcolor",
         "pyfiglet",
         "blessed",
         "imbalanced_learn",
         "imblearn",
         "joblib",
         "matplotlib",
-        #"nbclient",
-        #"nbformat",
+        "pyarrow",
+        "nbclient",
+        "nbformat",
         "numpy",
         "pandas",
         "plotext",
-        #"prefect",
-        #"prefect_jupyter",
+        "prefect",
+        "prefect_jupyter",
         "pydantic",
         "pyfiglet",
         "pytest",
         "scikit_learn",
         "scipy",
         "seaborn",
         "termcolor",
```

