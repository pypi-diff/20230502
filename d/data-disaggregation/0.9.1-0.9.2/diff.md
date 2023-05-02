# Comparing `tmp/data-disaggregation-0.9.1.tar.gz` & `tmp/data-disaggregation-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-disaggregation-0.9.1.tar", last modified: Thu Apr 27 15:38:14 2023, max compression
+gzip compressed data, was "data-disaggregation-0.9.2.tar", last modified: Tue May  2 12:04:30 2023, max compression
```

## Comparing `data-disaggregation-0.9.1.tar` & `data-disaggregation-0.9.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:14.319496 data-disaggregation-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-27 15:37:56.000000 data-disaggregation-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-27 15:38:14.319496 data-disaggregation-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-27 15:37:56.000000 data-disaggregation-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:14.315496 data-disaggregation-0.9.1/data_disaggregation/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-27 15:37:56.000000 data-disaggregation-0.9.1/data_disaggregation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-04-27 15:37:56.000000 data-disaggregation-0.9.1/data_disaggregation/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-27 15:37:56.000000 data-disaggregation-0.9.1/data_disaggregation/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-04-27 15:37:56.000000 data-disaggregation-0.9.1/data_disaggregation/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-04-27 15:37:56.000000 data-disaggregation-0.9.1/data_disaggregation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:14.315496 data-disaggregation-0.9.1/data_disaggregation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-27 15:38:14.000000 data-disaggregation-0.9.1/data_disaggregation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-27 15:38:14.000000 data-disaggregation-0.9.1/data_disaggregation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:38:14.000000 data-disaggregation-0.9.1/data_disaggregation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 15:38:14.000000 data-disaggregation-0.9.1/data_disaggregation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-27 15:38:14.000000 data-disaggregation-0.9.1/data_disaggregation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 15:38:14.319496 data-disaggregation-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-27 15:37:56.000000 data-disaggregation-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:38:14.315496 data-disaggregation-0.9.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)    16636 2023-04-27 15:37:56.000000 data-disaggregation-0.9.1/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:04:30.518600 data-disaggregation-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-02 12:04:07.000000 data-disaggregation-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-02 12:04:30.518600 data-disaggregation-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-02 12:04:07.000000 data-disaggregation-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:04:30.518600 data-disaggregation-0.9.2/data_disaggregation/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-02 12:04:07.000000 data-disaggregation-0.9.2/data_disaggregation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-05-02 12:04:07.000000 data-disaggregation-0.9.2/data_disaggregation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-02 12:04:07.000000 data-disaggregation-0.9.2/data_disaggregation/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-05-02 12:04:07.000000 data-disaggregation-0.9.2/data_disaggregation/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-05-02 12:04:07.000000 data-disaggregation-0.9.2/data_disaggregation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:04:30.518600 data-disaggregation-0.9.2/data_disaggregation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-02 12:04:30.000000 data-disaggregation-0.9.2/data_disaggregation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-02 12:04:30.000000 data-disaggregation-0.9.2/data_disaggregation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 12:04:30.000000 data-disaggregation-0.9.2/data_disaggregation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 12:04:30.000000 data-disaggregation-0.9.2/data_disaggregation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-02 12:04:30.000000 data-disaggregation-0.9.2/data_disaggregation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 12:04:30.518600 data-disaggregation-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-02 12:04:07.000000 data-disaggregation-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:04:30.518600 data-disaggregation-0.9.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    18389 2023-05-02 12:04:07.000000 data-disaggregation-0.9.2/test/test.py
```

### Comparing `data-disaggregation-0.9.1/LICENSE` & `data-disaggregation-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `data-disaggregation-0.9.1/data_disaggregation/base.py` & `data-disaggregation-0.9.2/data_disaggregation/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     * create index pairs for result
 
 """
 
 
 from typing import Mapping, Tuple
 
-from .classes import VT, F, T, V, VT_Numeric, VT_NumericExt
+from .classes import VT, F, T, V, VT_NumericExt
 from .utils import (
     group_idx_first,
     group_idx_second,
     is_map,
     is_mapping,
     is_na,
     is_subset,
@@ -89,33 +89,34 @@
 def transform(
     vtype: VT,
     data: Mapping[F, V],
     weight_map: Mapping[Tuple[F, T], float],
     size_in: Mapping[F, float] = None,
     size_out: Mapping[T, float] = None,
     threshold: float = 0.0,
-    as_int: bool = False,
     validate=True,
 ) -> Mapping[T, V]:
     if size_in is None:
         size_in = group_idx_first(weight_map)
 
     if size_out is None:
         size_out = group_idx_second(weight_map)
 
     if validate:
         # validate size_f
         assert is_mapping(size_in)
         assert is_unique(size_in)
         assert all(v > 0 for v in iter_values(size_in))
+        # assert all(isinstance(v, (float, int)) for v in iter_values(size_in))
 
         # validate size_t
         assert is_mapping(size_out)
         assert is_unique(size_out)
         assert all(v > 0 for v in iter_values(size_out))
+        # assert all(isinstance(v, (float, int)) for v in iter_values(size_out))
 
         # validate var
         assert is_mapping(data)
         assert is_unique(data)
 
         assert is_subset(
             data, size_in
@@ -123,14 +124,15 @@
 
         # validate map
         assert is_map(weight_map)
         assert is_unique(weight_map)
         assert all(v >= 0 for v in iter_values(weight_map))
         assert is_subset([x[0] for x in weight_map.keys()], size_in)
         assert is_subset([x[1] for x in weight_map.keys()], size_out)
+        # assert all(isinstance(v, (float, int)) for v in iter_values(weight_map))
 
     result = {}
 
     groups = get_groups(vtype=vtype, data=data, weight_map=weight_map, size_in=size_in)
 
     for t, vws in groups.items():
         # weights sum
@@ -151,18 +153,13 @@
 
         #  re-scale intensive => extensive
         if vtype == VT_NumericExt:
             v *= size_out[t]
 
         result[t] = v
 
-    # rounding
-    if as_int:
-        assert issubclass(vtype, VT_Numeric)
-        result = dict((t, round(v)) for t, v in result.items())
-
     if validate:
         # todo remove checks at the end
         assert is_subset(result, size_out)
         assert is_unique(result)
 
     return result
```

### Comparing `data-disaggregation-0.9.1/data_disaggregation/classes.py` & `data-disaggregation-0.9.2/data_disaggregation/classes.py`

 * *Files identical despite different names*

### Comparing `data-disaggregation-0.9.1/data_disaggregation/ext.py` & `data-disaggregation-0.9.2/data_disaggregation/ext.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,29 +5,31 @@
 
 from pandas import DataFrame, Index, MultiIndex, Series
 
 from .base import transform
 from .classes import SCALAR_DIM_NAME, SCALAR_INDEX_KEY, VT, F, T
 from .utils import is_na, is_scalar
 
+SCALAR_INDEX = Index([SCALAR_INDEX_KEY], name=SCALAR_DIM_NAME)
+
 
 def is_multindex(x: Union[DataFrame, Series, Index, MultiIndex, float]) -> bool:
     if isinstance(x, (int, float)):
         return False
     if isinstance(x, (DataFrame, Series)):
         x = x.index
     return isinstance(x, MultiIndex)
 
 
 def get_dimension_levels(
     x: Union[DataFrame, Series, Index, MultiIndex, float]
 ) -> List[Tuple[str, List]]:
     if isinstance(x, (int, float)):
         # scalar: dummy dimension
-        x = Index([SCALAR_INDEX_KEY], name=SCALAR_DIM_NAME)
+        x = SCALAR_INDEX
     elif isinstance(x, (DataFrame, Series)):
         x = x.index
 
     # names must be unique
     assert len(x.names) == len(set(x.names))
 
     if isinstance(x, MultiIndex):
@@ -35,27 +37,29 @@
     else:
         return [(x.name, x.values)]
 
 
 def get_idx_out(
     weights: Series, i_out: Union[DataFrame, Series, Index, MultiIndex, float]
 ):
+    """ """
     map_levels = get_dimension_levels(weights)
+
     from_levels = get_dimension_levels(i_out)
     from_level_names = [x[0] for x in from_levels]
 
     # determine out from difference (in - map)
     to_levels = [(k, v) for k, v in map_levels if k not in from_level_names]
 
-    to_is_multindex = len(to_levels) > 1
     if not to_levels:  # aggregation to scalar
-        to_levels = [(SCALAR_DIM_NAME, [SCALAR_INDEX_KEY])]
+        to_levels = get_dimension_levels(SCALAR_INDEX)
 
     to_levels_names = [x[0] for x in to_levels]
     to_levels_values = [x[1] for x in to_levels]
+    to_is_multindex = len(to_levels) > 1
 
     if to_is_multindex:
         return MultiIndex.from_product(to_levels_values, names=to_levels_names)
     else:
         return Index(to_levels_values[0], name=to_levels_names[0])
 
 
@@ -74,25 +78,27 @@
     from_levels_names = [x[0] for x in from_levels]
     from_is_multindex = is_multindex(idx_in)
 
     to_levels = get_dimension_levels(idx_out)
     to_levels_names = [x[0] for x in to_levels]
     to_is_multindex = is_multindex(idx_out)
 
+    # from_levels AND to_levels (unique)
     all_levels = []
     for name, items in from_levels:
         if name in dict(to_levels):
             continue
         all_levels.append((name, items))
     for name, items in to_levels:
         all_levels.append((name, items))
 
     # create indices mapping
     all_levels_names = [x[0] for x in all_levels]
     all_levels_values = [x[1] for x in all_levels]
+
     from_level_idcs = [all_levels_names.index(n) for n, _ in from_levels]
     to_level_idcs = [all_levels_names.index(n) for n, _ in to_levels]
     # this also ensures that map <= (from | to)
     try:
         map_level_idcs = [all_levels_names.index(n) for n, _ in map_levels]
     except Exception as e:
         raise ValueError(f"weight map cannot be created: {e}")
@@ -102,24 +108,26 @@
         if not is_multindex:
             assert len(indices) == 1
             key = key[0]
         return key
 
     result = {}
 
+    # create cross product of all levels
     for row in product(*all_levels_values):
         key_map = get_key(row, map_level_idcs, map_is_multindex)
         val_map = weights.get(key_map)
         if is_na(val_map):
             continue
 
-        key_from = get_key(row, from_level_idcs, from_is_multindex)
-        key_to = get_key(row, to_level_idcs, to_is_multindex)
+        # get in/out keys
+        key_in = get_key(row, from_level_idcs, from_is_multindex)
+        key_out = get_key(row, to_level_idcs, to_is_multindex)
 
-        key = (key_from, key_to)
+        key = (key_in, key_out)
         result[key] = val_map
 
     from_name = (
         tuple(from_levels_names) if len(from_levels_names) > 1 else from_levels_names[0]
     )
     to_name = tuple(to_levels_names) if len(to_levels_names) > 1 else to_levels_names[0]
 
@@ -128,22 +136,21 @@
     return result
 
 
 def transform_ds(
     vtype: VT,
     data: Series,
     weights: Series,
-    dim_in: Series = None,
-    dim_out: Series = None,
+    dim_in: Union[Index, Series] = None,
+    dim_out: Union[Index, Series] = None,
     threshold: float = 0.0,
-    as_int: bool = False,
     validate=True,
 ) -> Series:
     if is_scalar(data):
-        data = Series({SCALAR_INDEX_KEY: data}).rename_axis([SCALAR_DIM_NAME])
+        data = Series(data, index=SCALAR_INDEX)
 
     if isinstance(dim_in, Index):
         idx_in = dim_in
         size_in = None
     elif isinstance(dim_in, Series):
         idx_in = dim_in
         size_in = dim_in
@@ -170,21 +177,19 @@
     result = transform(
         vtype=vtype,
         data=data,
         weight_map=weight_map,
         size_in=size_in,
         size_out=size_out,
         threshold=threshold,
-        as_int=as_int,
         validate=validate,
     )
 
     index_names = weight_map.index.names[1]
-    dtype = data.dtype
 
     # scalar
     if set(result.keys()) == set([SCALAR_INDEX_KEY]):
         result = result[SCALAR_INDEX_KEY]
     else:
-        result = Series(result).rename_axis(index_names).astype(dtype)
+        result = Series(result).rename_axis(index_names)
 
     return result
```

### Comparing `data-disaggregation-0.9.1/data_disaggregation/utils.py` & `data-disaggregation-0.9.2/data_disaggregation/utils.py`

 * *Files identical despite different names*

### Comparing `data-disaggregation-0.9.1/setup.py` & `data-disaggregation-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         packages=["data_disaggregation"],
         name="data-disaggregation",
         install_requires=["pandas"],
         keywords=[],
         description="",
         long_description=long_description_md,
         long_description_content_type="text/markdown",
-        version="0.9.1",
+        version="0.9.2",
         author="Christian Winger",
         platforms=["any"],
         license="MIT",
         project_urls={
             "Documentation": "https://wingechr.github.io/data-disaggregation",
             "Source": "https://github.com/wingechr/data-disaggregation",
         },
```

### Comparing `data-disaggregation-0.9.1/test/test.py` & `data-disaggregation-0.9.2/test/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -191,17 +191,15 @@
             ("b", "F"): 2,
             ("c", "E"): 2,
             ("c", "F"): 1,
         }
 
         var = {"a": 5, "b": 10, "c": 30}
 
-        return transform(
-            vtype=vtype, data=var, weight_map=map, as_int=issubclass(vtype, VT_Numeric)
-        )
+        return transform(vtype=vtype, data=var, weight_map=map)
 
     def test_example_type_categorical(self):
         res = self.get_example(VT_Nominal)
         for k, v in {"D": 10, "E": 30, "F": 5}.items():
             self.assertEqual(v, res[k])
 
     def test_example_type_ordinal(self):
@@ -212,16 +210,20 @@
     def test_example_type_metric(self):
         res = self.get_example(VT_Numeric)
         for k, v in {"D": 10, "E": 30, "F": 12}.items():
             self.assertEqual(v, res[k])
 
     def test_example_type_metric_ext(self):
         res = self.get_example(VT_NumericExt)
-        for k, v in {"D": round(3.33333333), "E": 20, "F": round(21.6666667)}.items():
-            self.assertEqual(v, res[k])
+        for k, v in {
+            "D": 3.333333333333333333,
+            "E": 20,
+            "F": 21.6666666666666667,
+        }.items():
+            self.assertAlmostEqual(v, res[k])
 
 
 class TestDataframe(TestCase):
     """"""
 
     def get_example(self, vtype):
         """
@@ -246,27 +248,23 @@
         s_map = Series(
             {
                 ("a", "F"): 2,
                 ("b", "D"): 1,
                 ("b", "F"): 2,
                 ("c", "E"): 2,
                 ("c", "F"): 1,
-            }
+            },
+            dtype=float,
         )
         s_map.index.names = ["d1", "d2"]
 
         s_var = Series({"a": 5, "b": 10, "c": 30})
         s_var.index.names = ["d1"]
 
-        return transform(
-            weight_map=s_map,
-            data=s_var,
-            vtype=vtype,
-            as_int=issubclass(vtype, VT_Numeric),
-        )
+        return transform(weight_map=s_map, data=s_var, vtype=vtype)
 
     def test_example_type_categorical(self):
         res = self.get_example(VT_Nominal)
         for k, v in {"D": 10, "E": 30, "F": 5}.items():
             self.assertEqual(v, res[k])
 
     def test_example_type_ordinal(self):
@@ -277,16 +275,16 @@
     def test_example_type_metric(self):
         res = self.get_example(VT_Numeric)
         for k, v in {"D": 10, "E": 30, "F": 12}.items():
             self.assertEqual(v, res[k])
 
     def test_example_type_metric_ext(self):
         res = self.get_example(VT_NumericExt)
-        for k, v in {"D": round(3.333), "E": 20, "F": round(21.667)}.items():
-            self.assertEqual(v, res[k])
+        for k, v in {"D": 3.333333333333333, "E": 20, "F": 21.66666666666667}.items():
+            self.assertAlmostEqual(v, res[k])
 
 
 class TestBaseExamples(TestCase):
     def test_aggregate_ext(self):
         res = transform(
             vtype=VT_NumericExt,
             data={1: 1, 2: 1, 3: 10},
@@ -371,14 +369,34 @@
         )
 
         self.assertEqual(res[("u1", "t1")], 10 * 0.7)
         self.assertEqual(res[("u3", "t2")], 13 / (99 + 11) * 11)
         self.assertEqual(sum(v for k, v in res.items() if k[1] == "t1"), 10 + 11)
         self.assertEqual(sum(v for k, v in res.items() if k[1] == "t2"), 12 + 13)
 
+    def test_int_to_float(self):
+        dim_region = Index(["r1", "r2"], name="region")
+        dim_time = Index(["t1", "t2", "t3"], name="time")
+
+        idcs_in = [dim_region]
+        idcs_out = [dim_time]
+        idcs_weights = [dim_region]
+        vtype = VT_NumericExt
+
+        data = Series(10, index=MultiIndex.from_product(idcs_in))
+        weights = Series(1, index=MultiIndex.from_product(idcs_weights))
+
+        res = transform_ds(
+            vtype=vtype,
+            data=data,
+            weights=weights,
+            dim_out=MultiIndex.from_product(idcs_out),
+        )
+        self.assertAlmostEqual(res.sum(), data.sum())
+
     def test_ex_1(self):
         # create dimensions as pandas Index
         idx_month = Index(["1", "2"], name="month")
         idx_hour = Index(["11", "21", "22"], name="hour")
         idx_region = Index(["a", "b"], name="region")
 
         # create multi dimensions as pandas MultiIndex
@@ -499,7 +517,38 @@
                 ]
             ),
         )
 
         # ... and back
         s = transform_ds(VT_NumericExt, s_time, weights=w_time)
         self.assertEqual(s, 100)
+
+    def test_ex_3(self):
+        d_region = Index(["r1", "r2"], name="region")
+        d_subregion = Index(["r11", "r12", "r21", "r22"], name="subregion")
+        d_time = Index(["t1", "t2", "t3"], name="time")
+        # d_sector = Index(["s1", "s2"], name="sector")
+        # d_sector_b = Index(["sb1", "sb2", "sb3"], name="sector_b")
+
+        # s_region_subregion = Series(
+        #    {("r1", "r11"): 1, ("r1", "r12"): 1, ("r2", "r21"): 1, ("r2", "r22"): 1},
+        #    index=MultiIndex.from_product([d_region, d_subregion]),
+        # )
+        # s_region_subregion = Series(
+        #    dict(((sr[:2], sr), 1) for sr in d_subregion),
+        # ).rename_axis(["region", "subregion"])
+
+        s_region = Series({"r1": 100, "r2": 200}, index=d_region)
+        s_time = Series({"t1": 2, "t2": 3, "t3": 5}, index=d_time)
+
+        res = transform_ds(
+            vtype=VT_NumericExt,
+            data=s_region,
+            weights=s_time,
+            dim_out=MultiIndex.from_product([d_region, d_time]),
+        )
+
+        from math import isclose
+
+        MultiIndex.from_product([d_region, d_subregion, d_time])
+
+        assert isclose(res.sum(), s_region.sum())
```

