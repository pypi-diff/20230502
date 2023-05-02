# Comparing `tmp/antarctic-0.5.0.tar.gz` & `tmp/antarctic-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antarctic-0.5.0.tar", max compression
+gzip compressed data, was "antarctic-0.6.2.tar", max compression
```

## Comparing `antarctic-0.5.0.tar` & `antarctic-0.6.2.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0        0 2023-01-22 10:37:02.690391 antarctic-0.5.0/antarctic/__init__.py
--rw-r--r--   0        0        0     3234 2023-01-22 10:37:02.690391 antarctic-0.5.0/antarctic/document.py
--rw-r--r--   0        0        0     2016 2023-01-22 10:37:02.690391 antarctic-0.5.0/antarctic/pandas_field.py
--rw-r--r--   0        0        0      500 2023-01-22 10:37:19.734561 antarctic-0.5.0/pyproject.toml
--rwxr-xr-x   0        0        0     3724 2023-01-22 10:37:02.694391 antarctic-0.5.0/readme.md
--rw-r--r--   0        0        0     4488 1970-01-01 00:00:00.000000 antarctic-0.5.0/setup.py
--rw-r--r--   0        0        0     4313 1970-01-01 00:00:00.000000 antarctic-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-02 03:20:45.020995 antarctic-0.6.2/antarctic/__init__.py
+-rw-r--r--   0        0        0     3234 2023-05-02 03:20:45.020995 antarctic-0.6.2/antarctic/document.py
+-rw-r--r--   0        0        0     2016 2023-05-02 03:20:45.020995 antarctic-0.6.2/antarctic/pandas_field.py
+-rw-r--r--   0        0        0      505 2023-05-02 03:21:13.027791 antarctic-0.6.2/pyproject.toml
+-rwxr-xr-x   0        0        0     4393 2023-05-02 03:20:45.020995 antarctic-0.6.2/readme.md
+-rw-r--r--   0        0        0     4965 1970-01-01 00:00:00.000000 antarctic-0.6.2/PKG-INFO
```

### Comparing `antarctic-0.5.0/antarctic/document.py` & `antarctic-0.6.2/antarctic/document.py`

 * *Files identical despite different names*

### Comparing `antarctic-0.5.0/antarctic/pandas_field.py` & `antarctic-0.6.2/antarctic/pandas_field.py`

 * *Files identical despite different names*

### Comparing `antarctic-0.5.0/readme.md` & `antarctic-0.6.2/readme.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,15 @@
-# Antarctic
+# [Antarctic](https://tschm.github.io/antarctic/)
 
+[![Test](https://github.com/tschm/antarctic/actions/workflows/main.yml/badge.svg)](https://github.com/tschm/antarctic/actions/workflows/main.yml)
+[![Book](https://github.com/tschm/antarctic/actions/workflows/book.yml/badge.svg)](https://github.com/tschm/antarctic/actions/workflows/book.yml)
 [![Release](https://github.com/tschm/antarctic/workflows/Release/badge.svg)](https://github.com/tschm/antarctic/actions/)
 [![DeepSource](https://deepsource.io/gh/tschm/antarctic.svg/?label=active+issues&show_trend=true&token=Ap44D1XBPLUb19JqC763UIWf)](https://deepsource.io/gh/tschm/antarctic/?ref=repository-badge)
+[![Publish Docker image](https://github.com/tschm/antarctic/actions/workflows/binder.yml/badge.svg)](https://github.com/tschm/antarctic/actions/workflows/binder.yml)
+[![Binder](http://mybinder.org/badge_logo.svg)](http://mybinder.org/v2/gh/tschm/antarctic/HEAD)
 
 Project to persist Pandas data structures in a MongoDB database. 
 
 ## Installation
 ```python
 pip install antarctic
 ```
@@ -16,15 +20,15 @@
 to make Antarctic a convenient choice for storing Pandas (time series) data. 
 
 ### Fields
 We introduce first a new field --- the PandasField.
 
 ```python
 from mongoengine import Document, connect
-from antarctic.pandas_fields import PandasField
+from antarctic.pandas_field import PandasField
 
 # connect with your existing MongoDB (here I am using a popular interface mocking a MongoDB)
 client = connect(db="test", host="mongomock://localhost")
 
 
 # Define the blueprint for a portfolio document
 class Portfolio(Document):
@@ -34,64 +38,64 @@
 ```
 
 The portfolio objects works exactly the way you think it works
 
 ```python
 
 p = Portfolio()
-p.nav = pd.Series(...)
+p.nav = pd.Series(...).to_frame(name="nav")
 p.prices = pd.DataFrame(...)
 p.save()
 
-print(p.nav)
+print(p.nav["nav"])
 print(p.prices)
 ```
 
-Behind the scenes we convert the both Series and Frame objects into parquet bytestreams and
+Behind the scenes we convert the Frame objects into parquet bytestreams and
 store them in a MongoDB database.
 
 The format should also be readable by R. 
 
 #### Documents
 
 In most cases we have copies of very similar documents, e.g. we store Portfolios and Symbols rather than just a Portfolio or a Symbol.
 For this purpose we have developed the abstract `XDocument` class relying on the Document class of MongoEngine.
 It provides some convenient tools to simplify looping over all or a subset of Documents of the same type, e.g.
 
 ```python
 from antarctic.document import XDocument
-from antarctic.pandas_fields import PandasField
+from antarctic.pandas_field import PandasField
 
 client = connect(db="test", host="mongodb://localhost")
 
 
 class Symbol(XDocument):
 	price = PandasField()
 ```
 We define a bunch of symbols and assign a price for each (or some of it):
 
 ```python
-s1 = Symbol(name="A", price=pd.Series(...)).save()
-s2 = Symbol(name="B", price=pd.Series(...)).save()
+s1 = Symbol(name="A", price=pd.Series(...).to_frame(name="price")).save()
+s2 = Symbol(name="B", price=pd.Series(...).to_frame(name="price")).save()
 
 # We can access subsets like
 for symbol in Symbol.subset(names=["B"]):
 	print(symbol)
 
 # often we need a dictionary of Symbols:
 Symbol.to_dict(objects=[s1, s2])
 
 # Each XDocument also provides a field for reference data:
 s1.reference["MyProp1"] = "ABC"
 s2.reference["MyProp2"] = "BCD"
 
 # You can loop over (subsets) of Symbols and extract reference and/or series data
 print(Symbol.reference_frame(objects=[s1, s2]))
-print(Symbol.series(series="price"))
-print(Symbol.apply(func=lambda x: x.price.mean(), default=np.nan))
+print(Symbol.frame(series="price", key="price"))
+print(Symbol.apply(func=lambda x: x.price["price"].mean(), default=np.nan))
 ```
 
 The XDocument class is exposing DataFrames both for reference and time series data.
 There is an `apply` method for using a function on (subset) of documents.
```

### Comparing `antarctic-0.5.0/PKG-INFO` & `antarctic-0.6.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: antarctic
-Version: 0.5.0
+Version: 0.6.2
 Summary: ...
 Home-page: https://github.com/tschm/antarctic
 Author: Thomas Schmelzer
 Requires-Python: >=3.9.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fastparquet
 Requires-Dist: mongoengine
-Requires-Dist: pandas
+Requires-Dist: pandas (<2.0.0)
 Requires-Dist: pyarrow
-Requires-Dist: setuptools
 Project-URL: Repository, https://github.com/tschm/antarctic
 Description-Content-Type: text/markdown
 
-# Antarctic
+# [Antarctic](https://tschm.github.io/antarctic/)
 
+[![Test](https://github.com/tschm/antarctic/actions/workflows/main.yml/badge.svg)](https://github.com/tschm/antarctic/actions/workflows/main.yml)
+[![Book](https://github.com/tschm/antarctic/actions/workflows/book.yml/badge.svg)](https://github.com/tschm/antarctic/actions/workflows/book.yml)
 [![Release](https://github.com/tschm/antarctic/workflows/Release/badge.svg)](https://github.com/tschm/antarctic/actions/)
 [![DeepSource](https://deepsource.io/gh/tschm/antarctic.svg/?label=active+issues&show_trend=true&token=Ap44D1XBPLUb19JqC763UIWf)](https://deepsource.io/gh/tschm/antarctic/?ref=repository-badge)
+[![Publish Docker image](https://github.com/tschm/antarctic/actions/workflows/binder.yml/badge.svg)](https://github.com/tschm/antarctic/actions/workflows/binder.yml)
+[![Binder](http://mybinder.org/badge_logo.svg)](http://mybinder.org/v2/gh/tschm/antarctic/HEAD)
 
 Project to persist Pandas data structures in a MongoDB database. 
 
 ## Installation
 ```python
 pip install antarctic
 ```
@@ -35,15 +38,15 @@
 to make Antarctic a convenient choice for storing Pandas (time series) data. 
 
 ### Fields
 We introduce first a new field --- the PandasField.
 
 ```python
 from mongoengine import Document, connect
-from antarctic.pandas_fields import PandasField
+from antarctic.pandas_field import PandasField
 
 # connect with your existing MongoDB (here I am using a popular interface mocking a MongoDB)
 client = connect(db="test", host="mongomock://localhost")
 
 
 # Define the blueprint for a portfolio document
 class Portfolio(Document):
@@ -53,64 +56,64 @@
 ```
 
 The portfolio objects works exactly the way you think it works
 
 ```python
 
 p = Portfolio()
-p.nav = pd.Series(...)
+p.nav = pd.Series(...).to_frame(name="nav")
 p.prices = pd.DataFrame(...)
 p.save()
 
-print(p.nav)
+print(p.nav["nav"])
 print(p.prices)
 ```
 
-Behind the scenes we convert the both Series and Frame objects into parquet bytestreams and
+Behind the scenes we convert the Frame objects into parquet bytestreams and
 store them in a MongoDB database.
 
 The format should also be readable by R. 
 
 #### Documents
 
 In most cases we have copies of very similar documents, e.g. we store Portfolios and Symbols rather than just a Portfolio or a Symbol.
 For this purpose we have developed the abstract `XDocument` class relying on the Document class of MongoEngine.
 It provides some convenient tools to simplify looping over all or a subset of Documents of the same type, e.g.
 
 ```python
 from antarctic.document import XDocument
-from antarctic.pandas_fields import PandasField
+from antarctic.pandas_field import PandasField
 
 client = connect(db="test", host="mongodb://localhost")
 
 
 class Symbol(XDocument):
 	price = PandasField()
 ```
 We define a bunch of symbols and assign a price for each (or some of it):
 
 ```python
-s1 = Symbol(name="A", price=pd.Series(...)).save()
-s2 = Symbol(name="B", price=pd.Series(...)).save()
+s1 = Symbol(name="A", price=pd.Series(...).to_frame(name="price")).save()
+s2 = Symbol(name="B", price=pd.Series(...).to_frame(name="price")).save()
 
 # We can access subsets like
 for symbol in Symbol.subset(names=["B"]):
 	print(symbol)
 
 # often we need a dictionary of Symbols:
 Symbol.to_dict(objects=[s1, s2])
 
 # Each XDocument also provides a field for reference data:
 s1.reference["MyProp1"] = "ABC"
 s2.reference["MyProp2"] = "BCD"
 
 # You can loop over (subsets) of Symbols and extract reference and/or series data
 print(Symbol.reference_frame(objects=[s1, s2]))
-print(Symbol.series(series="price"))
-print(Symbol.apply(func=lambda x: x.price.mean(), default=np.nan))
+print(Symbol.frame(series="price", key="price"))
+print(Symbol.apply(func=lambda x: x.price["price"].mean(), default=np.nan))
 ```
 
 The XDocument class is exposing DataFrames both for reference and time series data.
 There is an `apply` method for using a function on (subset) of documents.
```

