# Comparing `tmp/read_rapidpe-0.1.3.tar.gz` & `tmp/read_rapidpe-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "read_rapidpe-0.1.3.tar", max compression
+gzip compressed data, was "read_rapidpe-0.2.0.tar", max compression
```

## Comparing `read_rapidpe-0.1.3.tar` & `read_rapidpe-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2399 2023-04-17 13:15:50.969962 read_rapidpe-0.1.3/README.md
--rw-r--r--   0        0        0      593 2023-04-23 20:11:24.579020 read_rapidpe-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      353 2023-04-16 13:12:20.078578 read_rapidpe-0.1.3/read_rapidpe/__init__.py
--rw-r--r--   0        0        0     8095 2022-12-12 05:47:03.434185 read_rapidpe-0.1.3/read_rapidpe/grid_point.py
--rw-r--r--   0        0        0     6083 2023-04-16 13:20:01.614285 read_rapidpe-0.1.3/read_rapidpe/p_astro.py
--rw-r--r--   0        0        0     9718 2023-04-07 15:04:09.805939 read_rapidpe-0.1.3/read_rapidpe/parser.py
--rw-r--r--   0        0        0     1474 2023-04-16 14:05:36.413685 read_rapidpe-0.1.3/read_rapidpe/plot.py
--rw-r--r--   0        0        0    18461 2023-04-17 05:43:56.585212 read_rapidpe-0.1.3/read_rapidpe/result.py
--rw-r--r--   0        0        0     2200 2022-11-25 08:05:18.514011 read_rapidpe-0.1.3/read_rapidpe/transform.py
--rw-r--r--   0        0        0     3254 1970-01-01 00:00:00.000000 read_rapidpe-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2399 2023-04-17 13:15:50.969962 read_rapidpe-0.2.0/README.md
+-rw-r--r--   0        0        0      627 2023-05-02 06:44:20.832113 read_rapidpe-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      353 2023-04-16 13:12:20.078578 read_rapidpe-0.2.0/read_rapidpe/__init__.py
+-rw-r--r--   0        0        0     8323 2023-05-01 03:22:06.667674 read_rapidpe-0.2.0/read_rapidpe/grid_point.py
+-rw-r--r--   0        0        0     6083 2023-04-16 13:20:01.614285 read_rapidpe-0.2.0/read_rapidpe/p_astro.py
+-rw-r--r--   0        0        0     9718 2023-04-07 15:04:09.805939 read_rapidpe-0.2.0/read_rapidpe/parser.py
+-rw-r--r--   0        0        0     1474 2023-04-16 14:05:36.413685 read_rapidpe-0.2.0/read_rapidpe/plot.py
+-rw-r--r--   0        0        0    20050 2023-05-02 05:41:52.815628 read_rapidpe-0.2.0/read_rapidpe/result.py
+-rw-r--r--   0        0        0     2200 2022-11-25 08:05:18.514011 read_rapidpe-0.2.0/read_rapidpe/transform.py
+-rw-r--r--   0        0        0     3330 1970-01-01 00:00:00.000000 read_rapidpe-0.2.0/PKG-INFO
```

### Comparing `read_rapidpe-0.1.3/README.md` & `read_rapidpe-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `read_rapidpe-0.1.3/read_rapidpe/grid_point.py` & `read_rapidpe-0.2.0/read_rapidpe/grid_point.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Read single grid point output from RapidPE output.
 Author: Cory Chu <cory@gwlab.page>
 """
 
 import xml.etree.ElementTree as ET
 import gzip
 import numpy as np
+from pathlib import Path
 
 # For ligolw reading
 from ligo.lw import utils, lsctables, ligolw
 lsctables.use_in(ligolw.LIGOLWContentHandler)
 
 
 class RapidPE_grid_point:
@@ -21,15 +22,17 @@
     """
     def __init__(self, grid_point=None):
         if grid_point is None:
             self.intrinsic_table = {}
             self.intrinsic_table_raw = {}
             self.extrinsic_table = {}
             self.extrinsic_table_raw = {}
+            self.xml_filename = ""
         else:
+            self.xml_filename = grid_point.xml_filename
             self.intrinsic_table_raw = grid_point.intrinsic_table_raw
             self.extrinsic_table_raw = grid_point.extrinsic_table_raw
             self.intrinsic_table = {}
             self._set_intrinsic_table()
             self.extrinsic_table = {}
             self._set_extrinsic_table()
             self._fix_intrinsic_table_spin()  # a temporary solution
@@ -101,17 +104,20 @@
         "sngl_inspiral:table" -> self.intrinsic_table_raw
         "sim_inspiral:table" -> self.extrinsic_table_raw
         """
 
         input_xml_gz = filename
 
         if use_ligolw:
+            # time-consuming, should open only once.
             cls.xmldoc = cls._open_ligolw(input_xml_gz)
 
         grid_point = cls()
+        grid_point.xml_filename = Path(input_xml_gz).stem
+
         grid_point.intrinsic_table_raw = cls._get_ligolw_table(
             input_xml_gz,
             tablename="sngl_inspiral:table",
             use_numpy=use_numpy,
             use_ligolw=use_ligolw
             )
```

### Comparing `read_rapidpe-0.1.3/read_rapidpe/p_astro.py` & `read_rapidpe-0.2.0/read_rapidpe/p_astro.py`

 * *Files identical despite different names*

### Comparing `read_rapidpe-0.1.3/read_rapidpe/parser.py` & `read_rapidpe-0.2.0/read_rapidpe/parser.py`

 * *Files identical despite different names*

### Comparing `read_rapidpe-0.1.3/read_rapidpe/plot.py` & `read_rapidpe-0.2.0/read_rapidpe/plot.py`

 * *Files identical despite different names*

### Comparing `read_rapidpe-0.1.3/read_rapidpe/result.py` & `read_rapidpe-0.2.0/read_rapidpe/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 Author: Cory Chu <cory@gwlab.page>
 """
 
 from pathlib import Path
 from joblib import Parallel, delayed
 import re
 import numpy as np
+import h5py
+import pandas as pd
 from .grid_point import RapidPE_grid_point
 from .transform import transform_m1m2_to_mceta, transform_mceta_to_m1m2
 from .transform import jacobian_mceta_by_m1m2
 
 from matplotlib.tri import Triangulation
 from matplotlib.tri import LinearTriInterpolator, CubicTriInterpolator
 from scipy.interpolate import LinearNDInterpolator, NearestNDInterpolator
@@ -124,15 +126,15 @@
             Whether using ligo.lw to read xml files
 
         extrinsic_table : bool
             Whether loading extrinsic_table as well
 
         """
         results_dir = Path(run_dir)/Path("results")
-        xml_array = [f.as_posix() for f in results_dir.glob("*.xml.gz")]
+        xml_array = [f.as_posix() for f in sorted(results_dir.glob("*.xml.gz"))]  # noqa: E501
 
         return cls.from_xml_array(xml_array,
                                   use_numpy=use_numpy,
                                   use_ligolw=use_ligolw,
                                   extrinsic_table=extrinsic_table,
                                   parallel_n=parallel_n)
 
@@ -235,14 +237,54 @@
         if ("mass_1" in result._keys) and ("mass_2" in result._keys):
             result.chirp_mass, result.symmetric_mass_ratio = \
                 transform_m1m2_to_mceta(result.mass_1, result.mass_2)
             result._keys.extend(["chirp_mass", "symmetric_mass_ratio"])
 
         return cls(result)
 
+    def to_hdf(self, hdf_filename, compression=None):
+        """
+        Save result to hdf file
+
+        Parameters
+        ----------
+        filename : str
+            The name of the hdf file
+
+        compression : str, optional (default: None)
+            The compression method, e.g., "gzip", "lzf".
+        """
+
+        with h5py.File(hdf_filename, 'w') as f:
+
+            # Cobine intrinsic parameters into "grid_points" dataset
+            result_df = pd.DataFrame({key: getattr(self, key) for key in self._keys})  # noqa: E501
+            result_np = result_df.to_records(index=False)
+            f.create_dataset("grid_points", data=result_np)
+
+            # Create "grid_points_raw" group to hold self.grid_points
+            group_grid_points_raw = \
+                f.create_group("grid_points_raw", track_order=True)
+
+            for i, gp in enumerate(self.grid_points):
+                group_gp = group_grid_points_raw.create_group(str(i))
+
+                # Add intrinsic_table
+                it = pd.DataFrame(gp.intrinsic_table).to_records(index=False)
+                group_gp.create_dataset("intrinsic_table", data=it)
+
+                # Add extrinsic_table
+                et = pd.DataFrame(gp.extrinsic_table).to_records(index=False)
+                group_gp.create_dataset("extrinsic_table",
+                                        data=et,
+                                        compression=compression)
+
+                # Add xml_filename
+                group_gp.attrs["xml_filename"] = gp.xml_filename
+
     def do_interpolate_marg_log_likelihood_m1m2(
             self,
             method="linear-scipy",
             gaussian_sigma_to_grid_size_ratio=0.5
             ):
         """
         Perfom triangular interpolation of marg_log_likelihood in
```

### Comparing `read_rapidpe-0.1.3/read_rapidpe/transform.py` & `read_rapidpe-0.2.0/read_rapidpe/transform.py`

 * *Files identical despite different names*

### Comparing `read_rapidpe-0.1.3/PKG-INFO` & `read_rapidpe-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: read-rapidpe
-Version: 0.1.3
+Version: 0.2.0
 Summary: Read and analyse results generated by rapidpe-rift-pipe
 Home-page: https://github.com/c0rychu/read-rapidpe
 Author: Cory Chu
 Author-email: cory@gwlab.page
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: h5py (>=3.8.0,<4.0.0)
 Requires-Dist: joblib (>=1.2.0,<2.0.0)
 Requires-Dist: lalsuite (>=7.14,<8.0)
 Requires-Dist: matplotlib (>=3.6.2,<4.0.0)
 Requires-Dist: numpy (>=1.23.4,<2.0.0)
+Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: python-ligo-lw (>=1.8.3,<2.0.0)
 Requires-Dist: scipy (>=1.9.3,<2.0.0)
 Project-URL: Repository, https://git.ligo.org/yu-kuang.chu/read-rapidpe
 Description-Content-Type: text/markdown
 
 Read Rapid-PE
 ===
```

