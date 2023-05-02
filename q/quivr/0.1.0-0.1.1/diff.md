# Comparing `tmp/quivr-0.1.0.tar.gz` & `tmp/quivr-0.1.1.tar.gz`

## Comparing `quivr-0.1.0.tar` & `quivr-0.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/__init__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/__init__.py~
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/__version__.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/__version__.py~
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/concat.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/concat.py~
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/coordinates.py~
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/defragment.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/defragment.py~
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/errors.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/errors.py~
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/indexing.py
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/indexing.py~
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/matrix.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/matrix.py~
--rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/models.py~
--rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/quiver.py~
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/schemagraph.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/schemagraph.py~
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/streaming.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/streaming.py~
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/struct_demo.py~
--rw-r--r--   0        0        0    16606 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/tables.py
--rw-r--r--   0        0        0    13056 2020-02-02 00:00:00.000000 quivr-0.1.0/quivr/tables.py~
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 quivr-0.1.0/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.1.0/LICENSE
--rw-r--r--   0        0        0     8334 2020-02-02 00:00:00.000000 quivr-0.1.0/README.md
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 quivr-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     8732 2020-02-02 00:00:00.000000 quivr-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/__init__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/__init__.py~
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/__version__.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/__version__.py~
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/concat.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/concat.py~
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/coordinates.py~
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/defragment.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/defragment.py~
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/errors.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/errors.py~
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/indexing.py
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/indexing.py~
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/matrix.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/matrix.py~
+-rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/models.py~
+-rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/quiver.py~
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/schemagraph.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/schemagraph.py~
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/streaming.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/streaming.py~
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/struct_demo.py~
+-rw-r--r--   0        0        0    20110 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/tables.py
+-rw-r--r--   0        0        0    13056 2020-02-02 00:00:00.000000 quivr-0.1.1/quivr/tables.py~
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 quivr-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 quivr-0.1.1/LICENSE
+-rw-r--r--   0        0        0     8296 2020-02-02 00:00:00.000000 quivr-0.1.1/README.md
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 quivr-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     8694 2020-02-02 00:00:00.000000 quivr-0.1.1/PKG-INFO
```

### Comparing `quivr-0.1.0/quivr/concat.py` & `quivr-0.1.1/quivr/concat.py`

 * *Files identical despite different names*

### Comparing `quivr-0.1.0/quivr/coordinates.py~` & `quivr-0.1.1/quivr/coordinates.py~`

 * *Files identical despite different names*

### Comparing `quivr-0.1.0/quivr/indexing.py` & `quivr-0.1.1/quivr/indexing.py`

 * *Files identical despite different names*

### Comparing `quivr-0.1.0/quivr/indexing.py~` & `quivr-0.1.1/quivr/indexing.py~`

 * *Files identical despite different names*

### Comparing `quivr-0.1.0/quivr/matrix.py` & `quivr-0.1.1/quivr/matrix.py`

 * *Files identical despite different names*

### Comparing `quivr-0.1.0/quivr/matrix.py~` & `quivr-0.1.1/quivr/matrix.py~`

 * *Files identical despite different names*

### Comparing `quivr-0.1.0/quivr/models.py~` & `quivr-0.1.1/quivr/models.py~`

 * *Files identical despite different names*

### Comparing `quivr-0.1.0/quivr/quiver.py~` & `quivr-0.1.1/quivr/quiver.py~`

 * *Files identical despite different names*

### Comparing `quivr-0.1.0/quivr/schemagraph.py` & `quivr-0.1.1/quivr/schemagraph.py`

 * *Files identical despite different names*

### Comparing `quivr-0.1.0/quivr/struct_demo.py~` & `quivr-0.1.1/quivr/struct_demo.py~`

 * *Files identical despite different names*

### Comparing `quivr-0.1.0/quivr/tables.py` & `quivr-0.1.1/quivr/tables.py`

 * *Files 11% similar despite different names*

```diff
@@ -74,25 +74,101 @@
     table: pa.Table
     schema: pa.Schema = pa.schema([])
     _schema_depth: int
 
     def __init__(self, table: pa.Table):
         self.table = []
         if not isinstance(table, pa.Table):
-            raise TypeError(
-                f"Data must be a pyarrow.Table for {self.__class__.__name__}"
-            )
+            raise TypeError(f"Data must be a pyarrow.Table for {self.__class__.__name__}")
         if table.schema != self.schema:
-            raise TypeError(
-                f"Data schema must match schema for {self.__class__.__name__}"
-            )
+            raise TypeError(f"Data schema must match schema for {self.__class__.__name__}")
         self.table = table
 
     @classmethod
-    def from_arrays(cls, arrays: list[pa.array]):
+    def from_data(cls, data: Optional[Any] = None, **kwargs) -> Self:
+        """Create an instance of the TableBase and populate it with data.
+
+        This is a convenience method which tries to infer the right
+        underlying constructors to use based on the type of data. It
+        can also accept keyword-style arguments to pass data in. If
+        you know the data's structure well in advance, the more
+        precise constructors (from_arrays, from_pylist, etc) should be
+        preferred.
+
+        Examples:
+            >>> import quivr
+            >>> class MyTable(quivr.TableBase):
+            ...     schema = pyarrow.schema([
+            ...         pyarrow.field("a", pyarrow.string()),
+            ...         pyarrow.field("b", pyarrow.int64()),
+            ...     ])
+            ...
+            >>> # All of these are equivalent:
+            >>> MyTable.from_data([["a", 1], ["b", 2]])
+            MyTable(size=2)
+            >>> MyTable.from_data({"a": ["a", "b"], "b": [1, 2]})
+            MyTable(size=2)
+            >>> MyTable.from_data([{"a": "a", "b": 1}, {"a": "b", "b": 2}])
+            MyTable(size=2)
+            >>> MyTable.from_data(a=["a", "b"], b=[1, 2])
+            MyTable(size=2)
+            >>> import numpy as np
+            >>> MyTable.from_data(a=np.array(["a", "b"]), b=np.array([1, 2]))
+            MyTable(size=2)
+        """
+        if data is None:
+            return cls.from_kwargs(**kwargs)
+
+        if isinstance(data, pa.Table):
+            return cls(table=data)
+        if isinstance(data, dict):
+            return cls.from_pydict(data)
+        if isinstance(data, list):
+            if len(data) == 0:
+                return cls.from_rows(data)
+            if isinstance(data[0], dict):
+                return cls.from_rows(data)
+            elif isinstance(data[0], list):
+                return cls.from_lists(data)
+        if isinstance(data, pd.DataFrame):
+            return cls.from_pandas(data)
+        if isinstance(data, np.ndarray):
+            return cls.from_numpy(data)
+        raise TypeError(f"Unsupported data type: {type(data)}")
+
+    @classmethod
+    def from_kwargs(cls, **kwargs) -> Self:
+        """Create a TableBase object from keyword arguments.
+
+        Each keyword argument corresponds to a column in the table.
+
+        Each keyword value can be a list, numpy array, pyarrow array,
+        or TableBase instance.
+
+        """
+
+        arrays = []
+        for column_name in cls.schema.names:
+            if column_name not in kwargs:
+                raise ValueError(f"Missing column {column_name}")
+            value = kwargs[column_name]
+            if isinstance(value, TableBase):
+                arrays.append(value.to_structarray())
+            elif isinstance(value, pa.Array):
+                arrays.append(value)
+            elif isinstance(value, np.ndarray):
+                arrays.append(pa.array(value))
+            elif isinstance(value, list):
+                arrays.append(pa.array(value))
+            else:
+                raise TypeError(f"Unsupported type for {column_name}: {type(value)}")
+        return cls.from_arrays(arrays)
+
+    @classmethod
+    def from_arrays(cls, arrays: list[pa.array]) -> Self:
         """Create a TableBase object from a list of arrays.
 
         Args:
             arrays: A list of pyarrow.Array objects.
 
         Returns:
             A TableBase object.
@@ -103,19 +179,17 @@
 
     @classmethod
     def from_pydict(cls, d: dict[str, Union[pa.array, list, np.ndarray]]):
         table = pa.Table.from_pydict(d, schema=cls.schema)
         return cls(table=table)
 
     @classmethod
-    def from_pylist(cls, l: list):
+    def from_rows(cls, l: list[dict]):
         """
-        Create a TableBase object from a list of values.
-
-        Nested and hierarchical values can be represented as dictionaries in the list.
+        Create a TableBase object from a list of dictionaries.
 
         Args:
             l: A list of values. Each value corresponds to a row in the table.
 
         Returns:
             A TableBase object.
 
@@ -131,14 +205,31 @@
             >>> Outer.from_pylist(data)
             Outer(size=2)
         """
         table = pa.Table.from_pylist(l, schema=cls.schema)
         return cls(table=table)
 
     @classmethod
+    def from_lists(cls, l: list[list]) -> Self:
+        """Create a TableBase object from a list of lists.
+
+        Each inner list corresponds to a column in the table. They
+        should be specified in the same order as the columns in the
+        schema.
+
+        Args:
+            l: A list of lists. Each inner list corresponds to a column in the table.
+
+        Returns:
+            A TableBase object.
+        """
+        table = pa.Table.from_arrays(list(map(pa.array, l)), schema=cls.schema)
+        return cls(table=table)
+
+    @classmethod
     def from_dataframe(cls, df: pd.DataFrame):
         """Load a DataFrame into the Table.
 
         If the DataFrame is missing any of the Table's columns, an
         error is raised. If the DataFrame has extra columns, they are
         ignored.
 
@@ -356,38 +447,32 @@
         """
         table = self.table
         if flatten:
             table = self.flattened_table()
         return table.to_pandas()
 
     @classmethod
-    def as_field(
-        cls, name: str, nullable: bool = True, metadata: Optional[dict] = None
-    ):
+    def as_field(cls, name: str, nullable: bool = True, metadata: Optional[dict] = None):
         metadata = metadata or {}
         metadata[_METADATA_NAME_KEY] = cls.__name__
         metadata[_METADATA_MODEL_KEY] = pickle.dumps(cls)
-        field = pa.field(
-            name, pa.struct(cls.schema), nullable=nullable, metadata=metadata
-        )
+        field = pa.field(name, pa.struct(cls.schema), nullable=nullable, metadata=metadata)
         return field
 
     def column(self, field_name: str):
         field = self.schema.field(field_name)
         if field.metadata is not None and _METADATA_MODEL_KEY in field.metadata:
             # If the field has type information attached to it in
             # metadata, pull it out. The metadata store the model (as
             # a class object), and may optionally have some keyword
             # arguments to be used when instantiating the model from
             # the data.
             model = pickle.loads(field.metadata[_METADATA_MODEL_KEY])
             if _METADATA_UNPICKLE_KWARGS_KEY in field.metadata:
-                init_kwargs = pickle.loads(
-                    field.metadata[_METADATA_UNPICKLE_KWARGS_KEY]
-                )
+                init_kwargs = pickle.loads(field.metadata[_METADATA_UNPICKLE_KWARGS_KEY])
             else:
                 init_kwargs = {}
             table = _sub_table(self.table, field_name)
             return model(table=table, **init_kwargs)
         return self.table.column(field_name)
 
     def __repr__(self):
```

### Comparing `quivr-0.1.0/quivr/tables.py~` & `quivr-0.1.1/quivr/tables.py~`

 * *Files identical despite different names*

### Comparing `quivr-0.1.0/LICENSE` & `quivr-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quivr-0.1.0/README.md` & `quivr-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: quivr
+Version: 0.1.1
+Summary: Container library for working with tabular Arrow data
+Project-URL: Source, https://github.com/spenczar/quivr
+Author-email: Spencer Nelson <spencer@spencerwnelson.com>
+License-File: LICENSE
+Requires-Python: >=3.11
+Requires-Dist: mmh3
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: pyarrow
+Description-Content-Type: text/markdown
+
 # quivr
 
 Quivr is a Python library which provides great containers for Arrow data.
 
 Quivr's `Table`s are like DataFrames, but with strict schemas to
 enforce types and expectations. They are backed by the
 high-performance Arrow memory model, making them well-suited for
@@ -65,22 +79,22 @@
     )
 ```
 
 Then, you can construct tables from data:
 
 ```python
 
-coords = Coordinates.from_pydict({
-    "x": np.array([ 1.00760887, -2.06203093,  1.24360546, -1.00131722]),
-    "y": np.array([-2.7227298 ,  0.70239707,  2.23125432,  0.37269832]),
-    "z": np.array([-0.27148738, -0.31768623, -0.2180482 , -0.02528401]),
-    "vx": np.array([ 0.00920172, -0.00570486, -0.00877929, -0.00809866]),
-    "vy": np.array([ 0.00297888, -0.00914301,  0.00525891, -0.01119134]),
-    "vz": np.array([-0.00160217,  0.00677584,  0.00091095, -0.00140548])
-})
+coords = Coordinates.from_data(
+    x=np.array([ 1.00760887, -2.06203093,  1.24360546, -1.00131722]),
+    y=np.array([-2.7227298 ,  0.70239707,  2.23125432,  0.37269832]),
+    z=np.array([-0.27148738, -0.31768623, -0.2180482 , -0.02528401]),
+    vx=np.array([ 0.00920172, -0.00570486, -0.00877929, -0.00809866]),
+    vy=np.array([ 0.00297888, -0.00914301,  0.00525891, -0.01119134]),
+    vz=np.array([-0.00160217,  0.00677584,  0.00091095, -0.00140548])
+)
 
 # Sort the table by the z column. This returns a copy.
 coords_z_sorted = coords.sort_by("z")
 
 print(len(coords))
 # prints 4
 
@@ -105,20 +119,20 @@
             pa.field("radius", pa.float64(), nullable=True),
             Coordinates.as_field("coords"),
         ]
     )
 
 # You can construct embedded fields from Arrow StructArrays, which you can get from
 # other Quivr tables using the to_structarray() method with zero copy.
-orbits = AsteroidOrbit.from_pydict({
-    "designation": np.array(["Ceres", "Pallas", "Vesta", "2023 DW"]),
-    "mass": np.array([9.393e20, 2.06e21, 2.59e20, None]),
-    "radius": np.array([4.6e6, 2.7e6, 2.6e6, None]),
-    "coords": coords.to_structarray(),
-})
+orbits = AsteroidOrbit.from_data(
+    designation=np.array(["Ceres", "Pallas", "Vesta", "2023 DW"]),
+    mass=np.array([9.393e20, 2.06e21, 2.59e20, None]),
+    radius=np.array([4.6e6, 2.7e6, 2.6e6, None]),
+    coords=coords.to_structarray(),
+)
 ```
 
 ### Computing
 
 You can use the columns of the data to do computations:
 
 ```python
```

### Comparing `quivr-0.1.0/pyproject.toml` & `quivr-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quivr-0.1.0/PKG-INFO` & `quivr-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: quivr
-Version: 0.1.0
-Summary: Container library for working with tabular Arrow data
-Project-URL: Source, https://github.com/spenczar/quivr
-Author-email: Spencer Nelson <spencer@spencerwnelson.com>
-License-File: LICENSE
-Requires-Python: >=3.11
-Requires-Dist: mmh3
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: pyarrow
-Description-Content-Type: text/markdown
-
 # quivr
 
 Quivr is a Python library which provides great containers for Arrow data.
 
 Quivr's `Table`s are like DataFrames, but with strict schemas to
 enforce types and expectations. They are backed by the
 high-performance Arrow memory model, making them well-suited for
@@ -79,22 +65,22 @@
     )
 ```
 
 Then, you can construct tables from data:
 
 ```python
 
-coords = Coordinates.from_pydict({
-    "x": np.array([ 1.00760887, -2.06203093,  1.24360546, -1.00131722]),
-    "y": np.array([-2.7227298 ,  0.70239707,  2.23125432,  0.37269832]),
-    "z": np.array([-0.27148738, -0.31768623, -0.2180482 , -0.02528401]),
-    "vx": np.array([ 0.00920172, -0.00570486, -0.00877929, -0.00809866]),
-    "vy": np.array([ 0.00297888, -0.00914301,  0.00525891, -0.01119134]),
-    "vz": np.array([-0.00160217,  0.00677584,  0.00091095, -0.00140548])
-})
+coords = Coordinates.from_data(
+    x=np.array([ 1.00760887, -2.06203093,  1.24360546, -1.00131722]),
+    y=np.array([-2.7227298 ,  0.70239707,  2.23125432,  0.37269832]),
+    z=np.array([-0.27148738, -0.31768623, -0.2180482 , -0.02528401]),
+    vx=np.array([ 0.00920172, -0.00570486, -0.00877929, -0.00809866]),
+    vy=np.array([ 0.00297888, -0.00914301,  0.00525891, -0.01119134]),
+    vz=np.array([-0.00160217,  0.00677584,  0.00091095, -0.00140548])
+)
 
 # Sort the table by the z column. This returns a copy.
 coords_z_sorted = coords.sort_by("z")
 
 print(len(coords))
 # prints 4
 
@@ -119,20 +105,20 @@
             pa.field("radius", pa.float64(), nullable=True),
             Coordinates.as_field("coords"),
         ]
     )
 
 # You can construct embedded fields from Arrow StructArrays, which you can get from
 # other Quivr tables using the to_structarray() method with zero copy.
-orbits = AsteroidOrbit.from_pydict({
-    "designation": np.array(["Ceres", "Pallas", "Vesta", "2023 DW"]),
-    "mass": np.array([9.393e20, 2.06e21, 2.59e20, None]),
-    "radius": np.array([4.6e6, 2.7e6, 2.6e6, None]),
-    "coords": coords.to_structarray(),
-})
+orbits = AsteroidOrbit.from_data(
+    designation=np.array(["Ceres", "Pallas", "Vesta", "2023 DW"]),
+    mass=np.array([9.393e20, 2.06e21, 2.59e20, None]),
+    radius=np.array([4.6e6, 2.7e6, 2.6e6, None]),
+    coords=coords.to_structarray(),
+)
 ```
 
 ### Computing
 
 You can use the columns of the data to do computations:
 
 ```python
```

