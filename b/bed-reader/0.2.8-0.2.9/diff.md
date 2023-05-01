# Comparing `tmp/bed_reader-0.2.8.tar.gz` & `tmp/bed_reader-0.2.9.tar.gz`

## Comparing `bed_reader-0.2.8.tar` & `bed_reader-0.2.9.tar`

### file list

```diff
@@ -1,51 +1,52 @@
--rw-r--r--   0        0        0     1719 1970-01-01 00:00:00.000000 bed_reader-0.2.8/Cargo.toml
--rw-r--r--   0     1001      121       61 2022-01-17 16:30:05.000000 bed_reader-0.2.8/.flake8
--rw-r--r--   0     1001      121     3812 2022-01-17 16:30:05.000000 bed_reader-0.2.8/.github/workflows/ci.yml
--rw-r--r--   0     1001      121     2175 2022-01-17 16:30:05.000000 bed_reader-0.2.8/.gitignore
--rw-r--r--   0     1001      121       27 2022-01-17 16:30:05.000000 bed_reader-0.2.8/AUTHORS.txt
--rw-r--r--   0     1001      121    11352 2022-01-17 16:30:05.000000 bed_reader-0.2.8/LICENSE.md
--rw-r--r--   0     1001      121     2446 2022-01-17 16:30:05.000000 bed_reader-0.2.8/README.md
--rw-r--r--   0     1001      121      852 2022-01-17 16:30:05.000000 bed_reader-0.2.8/bed_reader/__init__.py
--rw-r--r--   0     1001      121    40516 2022-01-17 16:30:05.000000 bed_reader-0.2.8/bed_reader/_open_bed.py
--rw-r--r--   0     1001      121     2407 2022-01-17 16:30:05.000000 bed_reader-0.2.8/bed_reader/_sample_data.py
--rw-r--r--   0     1001      121     8557 2022-01-17 16:30:05.000000 bed_reader-0.2.8/bed_reader/_to_bed.py
--rw-r--r--   0     1001      121       50 2022-01-17 16:30:05.000000 bed_reader-0.2.8/bed_reader/tests/__init__.py
--rw-r--r--   0     1001      121  1600640 2022-01-17 16:30:05.000000 bed_reader-0.2.8/bed_reader/tests/data/500x400_o640_array.memmap
--rw-r--r--   0     1001      121       30 2022-01-17 16:30:05.000000 bed_reader-0.2.8/bed_reader/tests/data/badfile.bed
--rw-r--r--   0     1001      121        0 2022-01-17 16:30:05.000000 bed_reader-0.2.8/bed_reader/tests/data/empty.bed
--rw-r--r--   0     1001      121      303 2022-01-17 16:30:05.000000 bed_reader-0.2.8/bed_reader/tests/data/plink_sim_10s_100v_10pmiss.bed
--rw-r--r--   0     1001      121     2184 2022-01-17 16:30:05.000000 bed_reader-0.2.8/bed_reader/tests/data/plink_sim_10s_100v_10pmiss.bim
--rw-r--r--   0     1001      121      130 2022-01-17 16:30:05.000000 bed_reader-0.2.8/bed_reader/tests/data/plink_sim_10s_100v_10pmiss.fam
--rw-r--r--   0     1001      121        7 2022-01-17 16:30:05.000000 bed_reader-0.2.8/bed_reader/tests/data/small.bed
--rw-r--r--   0     1001      121       87 2022-01-17 16:30:05.000000 bed_reader-0.2.8/bed_reader/tests/data/small.bim
--rw-r--r--   0     1001      121       85 2022-01-17 16:30:05.000000 bed_reader-0.2.8/bed_reader/tests/data/small.fam
--rw-r--r--   0     1001      121       96 2022-01-17 16:30:05.000000 bed_reader-0.2.8/bed_reader/tests/data/small2_array.memmap
--rw-r--r--   0     1001      121       48 2022-01-17 16:30:05.000000 bed_reader-0.2.8/bed_reader/tests/data/small_array.memmap
--rw-r--r--   0     1001      121        7 2022-01-17 16:30:05.000000 bed_reader-0.2.8/bed_reader/tests/data/small_no_bim.bed
--rw-r--r--   0     1001      121       85 2022-01-17 16:30:05.000000 bed_reader-0.2.8/bed_reader/tests/data/small_no_bim.fam
--rw-r--r--   0     1001      121        7 2022-01-17 16:30:05.000000 bed_reader-0.2.8/bed_reader/tests/data/small_no_fam.bed
--rw-r--r--   0     1001      121       87 2022-01-17 16:30:05.000000 bed_reader-0.2.8/bed_reader/tests/data/small_no_fam.bim
--rw-r--r--   0     1001      121        6 2022-01-17 16:30:05.000000 bed_reader-0.2.8/bed_reader/tests/data/small_too_short.bed
--rw-r--r--   0     1001      121       87 2022-01-17 16:30:05.000000 bed_reader-0.2.8/bed_reader/tests/data/small_too_short.bim
--rw-r--r--   0     1001      121       85 2022-01-17 16:30:05.000000 bed_reader-0.2.8/bed_reader/tests/data/small_too_short.fam
--rw-r--r--   0     1001      121        7 2022-01-17 16:30:05.000000 bed_reader-0.2.8/bed_reader/tests/data/smallmode0.bed
--rw-r--r--   0     1001      121        7 2022-01-17 16:30:05.000000 bed_reader-0.2.8/bed_reader/tests/data/smallmodebad.bed
--rw-r--r--   0     1001      121     2503 2022-01-17 16:30:05.000000 bed_reader-0.2.8/bed_reader/tests/data/some_missing.bed
--rw-r--r--   0     1001      121     2588 2022-01-17 16:30:05.000000 bed_reader-0.2.8/bed_reader/tests/data/some_missing.bim
--rw-r--r--   0     1001      121     1690 2022-01-17 16:30:05.000000 bed_reader-0.2.8/bed_reader/tests/data/some_missing.fam
--rw-r--r--   0     1001      121    51760 2022-01-17 16:30:05.000000 bed_reader-0.2.8/bed_reader/tests/data/some_missing.properties.npz
--rw-r--r--   0     1001      121    80128 2022-01-17 16:30:05.000000 bed_reader-0.2.8/bed_reader/tests/data/some_missing.val.npy
--rw-r--r--   0     1001      121  1250003 2022-01-17 16:30:05.000000 bed_reader-0.2.8/bed_reader/tests/data/toydata.5chrom.bed
--rw-r--r--   0     1001      121   227784 2022-01-17 16:30:05.000000 bed_reader-0.2.8/bed_reader/tests/data/toydata.5chrom.bim
--rw-r--r--   0     1001      121    14361 2022-01-17 16:30:05.000000 bed_reader-0.2.8/bed_reader/tests/data/toydata.5chrom.fam
--rw-r--r--   0     1001      121     1015 2022-01-17 16:30:05.000000 bed_reader-0.2.8/bed_reader/tests/registry.txt
--rw-r--r--   0     1001      121    11011 2022-01-17 16:30:05.000000 bed_reader-0.2.8/bed_reader/tests/test_file_dot.py
--rw-r--r--   0     1001      121    29826 2022-01-17 16:30:05.000000 bed_reader-0.2.8/bed_reader/tests/test_open_bed.py
--rw-r--r--   0     1001      121      157 2022-01-17 16:30:06.000000 bed_reader-0.2.8/pyproject.toml
--rw-r--r--   0     1001      121      124 2022-01-17 16:30:06.000000 bed_reader-0.2.8/pytest.ini
--rw-r--r--   0     1001      121      137 2022-01-17 16:30:06.000000 bed_reader-0.2.8/requirements-dev.txt
--rw-r--r--   0     1001      121       41 2022-01-17 16:30:06.000000 bed_reader-0.2.8/requirements.txt
--rw-r--r--   0     1001      121    35036 2022-01-17 16:30:06.000000 bed_reader-0.2.8/src/lib.rs
--rw-r--r--   0     1001      121    14125 2022-01-17 16:30:06.000000 bed_reader-0.2.8/src/python_module.rs
--rw-r--r--   0     1001      121    27782 2022-01-17 16:30:06.000000 bed_reader-0.2.8/src/tests.rs
--rw-r--r--   0        0        0     3517 1970-01-01 00:00:00.000000 bed_reader-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1741 1970-01-01 00:00:00.000000 bed_reader-0.2.9/Cargo.toml
+-rw-r--r--   0     1001      121       61 2022-01-25 02:57:00.000000 bed_reader-0.2.9/.flake8
+-rw-r--r--   0     1001      121     3812 2022-01-25 02:57:00.000000 bed_reader-0.2.9/.github/workflows/ci.yml
+-rw-r--r--   0     1001      121     2175 2022-01-25 02:57:00.000000 bed_reader-0.2.9/.gitignore
+-rw-r--r--   0     1001      121       27 2022-01-25 02:57:00.000000 bed_reader-0.2.9/AUTHORS.txt
+-rw-r--r--   0     1001      121    11352 2022-01-25 02:57:00.000000 bed_reader-0.2.9/LICENSE.md
+-rw-r--r--   0     1001      121     2446 2022-01-25 02:57:00.000000 bed_reader-0.2.9/README.md
+-rw-r--r--   0     1001      121      852 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/__init__.py
+-rw-r--r--   0     1001      121    40516 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/_open_bed.py
+-rw-r--r--   0     1001      121     2407 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/_sample_data.py
+-rw-r--r--   0     1001      121     8620 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/_to_bed.py
+-rw-r--r--   0     1001      121       50 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/tests/__init__.py
+-rw-r--r--   0     1001      121     3115 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/tests/benchmark/benchmark.py
+-rw-r--r--   0     1001      121  1600640 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/tests/data/500x400_o640_array.memmap
+-rw-r--r--   0     1001      121       30 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/tests/data/badfile.bed
+-rw-r--r--   0     1001      121        0 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/tests/data/empty.bed
+-rw-r--r--   0     1001      121      303 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/tests/data/plink_sim_10s_100v_10pmiss.bed
+-rw-r--r--   0     1001      121     2184 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/tests/data/plink_sim_10s_100v_10pmiss.bim
+-rw-r--r--   0     1001      121      130 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/tests/data/plink_sim_10s_100v_10pmiss.fam
+-rw-r--r--   0     1001      121        7 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/tests/data/small.bed
+-rw-r--r--   0     1001      121       87 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/tests/data/small.bim
+-rw-r--r--   0     1001      121       85 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/tests/data/small.fam
+-rw-r--r--   0     1001      121       96 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/tests/data/small2_array.memmap
+-rw-r--r--   0     1001      121       48 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/tests/data/small_array.memmap
+-rw-r--r--   0     1001      121        7 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/tests/data/small_no_bim.bed
+-rw-r--r--   0     1001      121       85 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/tests/data/small_no_bim.fam
+-rw-r--r--   0     1001      121        7 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/tests/data/small_no_fam.bed
+-rw-r--r--   0     1001      121       87 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/tests/data/small_no_fam.bim
+-rw-r--r--   0     1001      121        6 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/tests/data/small_too_short.bed
+-rw-r--r--   0     1001      121       87 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/tests/data/small_too_short.bim
+-rw-r--r--   0     1001      121       85 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/tests/data/small_too_short.fam
+-rw-r--r--   0     1001      121        7 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/tests/data/smallmode0.bed
+-rw-r--r--   0     1001      121        7 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/tests/data/smallmodebad.bed
+-rw-r--r--   0     1001      121     2503 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/tests/data/some_missing.bed
+-rw-r--r--   0     1001      121     2588 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/tests/data/some_missing.bim
+-rw-r--r--   0     1001      121     1690 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/tests/data/some_missing.fam
+-rw-r--r--   0     1001      121    51760 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/tests/data/some_missing.properties.npz
+-rw-r--r--   0     1001      121    80128 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/tests/data/some_missing.val.npy
+-rw-r--r--   0     1001      121  1250003 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/tests/data/toydata.5chrom.bed
+-rw-r--r--   0     1001      121   227784 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/tests/data/toydata.5chrom.bim
+-rw-r--r--   0     1001      121    14361 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/tests/data/toydata.5chrom.fam
+-rw-r--r--   0     1001      121     1015 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/tests/registry.txt
+-rw-r--r--   0     1001      121    11011 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/tests/test_file_dot.py
+-rw-r--r--   0     1001      121    29825 2022-01-25 02:57:00.000000 bed_reader-0.2.9/bed_reader/tests/test_open_bed.py
+-rw-r--r--   0     1001      121      157 2022-01-25 02:57:00.000000 bed_reader-0.2.9/pyproject.toml
+-rw-r--r--   0     1001      121      124 2022-01-25 02:57:00.000000 bed_reader-0.2.9/pytest.ini
+-rw-r--r--   0     1001      121      137 2022-01-25 02:57:00.000000 bed_reader-0.2.9/requirements-dev.txt
+-rw-r--r--   0     1001      121       41 2022-01-25 02:57:00.000000 bed_reader-0.2.9/requirements.txt
+-rw-r--r--   0     1001      121    36635 2022-01-25 02:57:00.000000 bed_reader-0.2.9/src/lib.rs
+-rw-r--r--   0     1001      121    14050 2022-01-25 02:57:00.000000 bed_reader-0.2.9/src/python_module.rs
+-rw-r--r--   0     1001      121    27862 2022-01-25 02:57:00.000000 bed_reader-0.2.9/src/tests.rs
+-rw-r--r--   0        0        0     3517 1970-01-01 00:00:00.000000 bed_reader-0.2.9/PKG-INFO
```

### Comparing `bed_reader-0.2.8/Cargo.toml` & `bed_reader-0.2.9/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [package]
 authors = ["FaST-LMM Team <fastlmm-dev@python.org>"]
 name = "bed-reader"
-version = "0.2.8"
+version = "0.2.9"
 repository = "https://github.com/fastlmm/bed-reader"
 description = "Read and write the PLINK BED format, simply and efficiently."
 exclude = ["tests/*", "doc/*", "docs/*"]
 readme = "README.md"
 license="Apache 2.0"
 keywords=["bioinformatics", "plink", "genomics", "genetics", "file-format", "reader", "genotype", "bed-format", "writer", "python", "snps"]
 edition = "2021"
@@ -41,10 +41,11 @@
 rayon = "1.5.1"
 numpy = "0.15.0"
 ndarray = { version = "0.15.4", features = ["approx", "rayon"] }
 approx = "0.5.0"
 statrs = "0.15.0"
 byteorder = { version = "1.4.3", default-features = false }
 pyo3 = { version = "0.15.1", features = ["extension-module"] }
+dpc-pariter = "0.3.1"
 
 [dev-dependencies]
 temp_testdir = "0.2.3"
```

### Comparing `bed_reader-0.2.8/.github/workflows/ci.yml` & `bed_reader-0.2.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bed_reader-0.2.8/.gitignore` & `bed_reader-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `bed_reader-0.2.8/LICENSE.md` & `bed_reader-0.2.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bed_reader-0.2.8/README.md` & `bed_reader-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `bed_reader-0.2.8/bed_reader/__init__.py` & `bed_reader-0.2.9/bed_reader/__init__.py`

 * *Files identical despite different names*

### Comparing `bed_reader-0.2.8/bed_reader/_open_bed.py` & `bed_reader-0.2.9/bed_reader/_open_bed.py`

 * *Files identical despite different names*

### Comparing `bed_reader-0.2.8/bed_reader/_sample_data.py` & `bed_reader-0.2.9/bed_reader/_sample_data.py`

 * *Files identical despite different names*

### Comparing `bed_reader-0.2.8/bed_reader/_to_bed.py` & `bed_reader-0.2.9/bed_reader/_to_bed.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,19 +55,16 @@
         Defaults to replacing the .bed file’s suffix with .bim.
     force_python_only
         If False (default), uses the faster Rust code; otherwise it uses the slower
         pure Python code.
 
     num_threads: None or int, optional
         The number of threads with which to write data.
-        (Writing is currently always single-threaded, but multithreading
-        may be enabled in the future.)
         Defaults to all available processors.
-        Can also be set with these
-        environment variables (listed in priority order):
+        Can also be set with these environment variables (listed in priority order):
         'PST_NUM_THREADS', 'NUM_THREADS', 'MKL_NUM_THREADS'.
 
 
     Examples
     --------
 
     In this example, all properties are given.
@@ -133,23 +130,32 @@
 
         num_threads = get_num_threads(num_threads)
 
         iid_count, sid_count = val.shape
         try:
             if val.dtype == np.float64:
                 write_f64(
-                    str(filepath), count_a1=count_A1, val=val, num_threads=num_threads
+                    str(filepath),
+                    count_a1=count_A1,
+                    val=val,
+                    num_threads=num_threads,
                 )
             elif val.dtype == np.float32:
                 write_f32(
-                    str(filepath), count_a1=count_A1, val=val, num_threads=num_threads
+                    str(filepath),
+                    count_a1=count_A1,
+                    val=val,
+                    num_threads=num_threads,
                 )
             elif val.dtype == np.int8:
                 write_i8(
-                    str(filepath), count_a1=count_A1, val=val, num_threads=num_threads
+                    str(filepath),
+                    count_a1=count_A1,
+                    val=val,
+                    num_threads=num_threads,
                 )
             else:
                 raise ValueError(
                     f"dtype '{val.dtype}' not known, only "
                     + "'int8', 'float32', and 'float64' are allowed."
                 )
         except SystemError as system_error:
```

### Comparing `bed_reader-0.2.8/bed_reader/tests/data/500x400_o640_array.memmap` & `bed_reader-0.2.9/bed_reader/tests/data/500x400_o640_array.memmap`

 * *Files identical despite different names*

### Comparing `bed_reader-0.2.8/bed_reader/tests/data/plink_sim_10s_100v_10pmiss.bim` & `bed_reader-0.2.9/bed_reader/tests/data/plink_sim_10s_100v_10pmiss.bim`

 * *Files identical despite different names*

### Comparing `bed_reader-0.2.8/bed_reader/tests/data/some_missing.bed` & `bed_reader-0.2.9/bed_reader/tests/data/some_missing.bed`

 * *Files identical despite different names*

### Comparing `bed_reader-0.2.8/bed_reader/tests/data/some_missing.bim` & `bed_reader-0.2.9/bed_reader/tests/data/some_missing.bim`

 * *Files identical despite different names*

### Comparing `bed_reader-0.2.8/bed_reader/tests/data/some_missing.fam` & `bed_reader-0.2.9/bed_reader/tests/data/some_missing.fam`

 * *Files identical despite different names*

### Comparing `bed_reader-0.2.8/bed_reader/tests/data/some_missing.properties.npz` & `bed_reader-0.2.9/bed_reader/tests/data/some_missing.properties.npz`

 * *Files identical despite different names*

### Comparing `bed_reader-0.2.8/bed_reader/tests/data/some_missing.val.npy` & `bed_reader-0.2.9/bed_reader/tests/data/some_missing.val.npy`

 * *Files identical despite different names*

### Comparing `bed_reader-0.2.8/bed_reader/tests/data/toydata.5chrom.bed` & `bed_reader-0.2.9/bed_reader/tests/data/toydata.5chrom.bed`

 * *Files identical despite different names*

### Comparing `bed_reader-0.2.8/bed_reader/tests/data/toydata.5chrom.bim` & `bed_reader-0.2.9/bed_reader/tests/data/toydata.5chrom.bim`

 * *Files identical despite different names*

### Comparing `bed_reader-0.2.8/bed_reader/tests/data/toydata.5chrom.fam` & `bed_reader-0.2.9/bed_reader/tests/data/toydata.5chrom.fam`

 * *Files identical despite different names*

### Comparing `bed_reader-0.2.8/bed_reader/tests/registry.txt` & `bed_reader-0.2.9/bed_reader/tests/registry.txt`

 * *Files identical despite different names*

### Comparing `bed_reader-0.2.8/bed_reader/tests/test_file_dot.py` & `bed_reader-0.2.9/bed_reader/tests/test_file_dot.py`

 * *Files identical despite different names*

### Comparing `bed_reader-0.2.8/bed_reader/tests/test_open_bed.py` & `bed_reader-0.2.9/bed_reader/tests/test_open_bed.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         assert (
             val.mean() == -13.142
         )  # really shouldn't do mean on data where -127 represents missing
         assert bed.chromosome[-1] == "1"
         assert bed.bp_position[-1] == 100
 
 
-def test_write1(tmp_path, shared_datadir):
+def test_write(tmp_path, shared_datadir):
     in_file = shared_datadir / "plink_sim_10s_100v_10pmiss.bed"
     out_file = tmp_path / "out.bed"
     with open_bed(in_file) as bed:
         val0 = bed.read()
         properties0 = {
             "fid": bed.fid,
             "iid": bed.iid,
```

### Comparing `bed_reader-0.2.8/src/lib.rs` & `bed_reader-0.2.9/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 // Inspired by C++ version by Chris Widmer and Carl Kadie
 
 // See: https://towardsdatascience.com/nine-rules-for-writing-python-extensions-in-rust-d35ea3a4ec29?sk=f8d808d5f414154fdb811e4137011437
 // for an article on how this project uses Rust to create a Python extension.
 
 use byteorder::{LittleEndian, ReadBytesExt};
 use core::fmt::Debug;
+use dpc_pariter::{scope, IteratorExt};
 use ndarray as nd;
 use ndarray::ShapeBuilder;
 use num_traits::{Float, FromPrimitive, ToPrimitive};
 use rayon::iter::{IntoParallelRefIterator, ParallelIterator};
 use rayon::{iter::ParallelBridge, ThreadPoolBuildError};
 use statrs::distribution::{Beta, Continuous};
+use std::fs::{self};
 use std::ops::AddAssign;
 use std::ops::{Div, Sub};
 use std::{
     fs::File,
     io::{BufRead, BufWriter, Read, Write},
 };
 use std::{io::SeekFrom, path::PathBuf};
@@ -61,14 +63,17 @@
         "Ill-formed BED file. BED file header is incorrect. Expected mode to be 0 or 1. '{0}'"
     )]
     BadMode(String),
 
     #[error("Attempt to write illegal value to BED file. Only 0,1,2,missing allowed. '{0}'")]
     BadValue(String),
 
+    #[error("Multithreading resulted in panic(s)")]
+    PanickedThread(),
+
     #[error("No individual observed for the SNP.")]
     NoIndividuals,
 
     #[error("Illegal SNP mean.")]
     IllegalSnpMean,
 
     #[error("Index to individual larger than the number of individuals. (Index value {0})")]
@@ -343,61 +348,102 @@
         missing_value,
         &mut val.view_mut(),
     )?;
 
     Ok(val)
 }
 
+// Thanks to Dawid for his dpc-pariter library that makes this function scale.
+// https://dpc.pw/adding-parallelism-to-your-rust-iterators
 pub fn write<T: From<i8> + Default + Copy + Debug + Sync + Send + PartialEq>(
     filename: &str,
     val: &nd::ArrayView2<'_, T>,
     count_a1: bool,
     missing: T,
+    num_threads: usize,
+) -> Result<(), BedErrorPlus> {
+    let (iid_count, sid_count) = val.dim();
+
+    // 4 genotypes per byte so round up
+    let (iid_count_div4, _) = try_div_4(iid_count, sid_count, CB_HEADER_U64)?;
+
+    // We create and write to a file.
+    // If there is an error, we will delete it.
+    if let Err(e) = write_internal(
+        filename,
+        iid_count_div4,
+        val,
+        count_a1,
+        missing,
+        num_threads,
+    ) {
+        // Clean up the file
+        let _ = fs::remove_file(filename);
+        Err(e)
+    } else {
+        Ok(())
+    }
+}
+
+fn write_internal<T: From<i8> + Default + Copy + Debug + Sync + Send + PartialEq>(
+    filename: &str,
+    iid_count_div4: usize,
+    val: &nd::ArrayView2<'_, T>,
+    count_a1: bool,
+    missing: T,
+    num_threads: usize,
 ) -> Result<(), BedErrorPlus> {
     let mut writer = BufWriter::new(File::create(filename)?);
     writer.write_all(&[BED_FILE_MAGIC1, BED_FILE_MAGIC2, 0x01])?;
 
+    #[allow(clippy::eq_op)]
+    let use_nan = missing != missing; // generic NAN test
     let zero_code = if count_a1 { 3u8 } else { 0u8 };
     let two_code = if count_a1 { 0u8 } else { 3u8 };
 
     let homozygous_primary_allele = T::from(0); // Major Allele
     let heterozygous_allele = T::from(1);
     let homozygous_secondary_allele = T::from(2); // Minor Allele
 
-    let (iid_count, sid_count) = val.dim();
-
-    // 4 genotypes per byte so round up
-    let (iid_count_div4, _) = try_div_4(iid_count, sid_count, CB_HEADER_U64)?;
-
-    #[allow(clippy::eq_op)]
-    let use_nan = missing != missing; // Generic way to look for NaN
-    for column in val.axis_iter(nd::Axis(1)) {
-        let mut bytes_vector: Vec<u8> = vec![0; iid_count_div4]; // inits to 0
-        for (iid_i, &v0) in column.iter().enumerate() {
-            #[allow(clippy::eq_op)]
-            let genotype_byte = if v0 == homozygous_primary_allele {
-                zero_code
-            } else if v0 == heterozygous_allele {
-                2
-            } else if v0 == homozygous_secondary_allele {
-                two_code
-            } else if (use_nan && v0 != v0) || (!use_nan && v0 == missing) {
-                // v0!=0 is generic NAN check
-                1
-            } else {
-                return Err(BedError::BadValue(filename.to_string()).into());
-            };
-            // Possible optimization: We could pre-compute the conversion, the division, the mod, and the multiply*2
-            let i_div_4 = iid_i / 4;
-            let i_mod_4 = iid_i % 4;
-            bytes_vector[i_div_4] |= genotype_byte << (i_mod_4 * 2);
-        }
-        writer.write_all(&bytes_vector)?;
-    }
-    Ok(())
+    scope(|scope| {
+        val.axis_iter(nd::Axis(1))
+            .parallel_map_scoped(scope, {
+                move |column| {
+                    // Convert each column into a bytes_vector
+                    let mut bytes_vector: Vec<u8> = vec![0; iid_count_div4]; // inits to 0
+                    for (iid_i, &v0) in column.iter().enumerate() {
+                        #[allow(clippy::eq_op)]
+                        let genotype_byte = if v0 == homozygous_primary_allele {
+                            zero_code
+                        } else if v0 == heterozygous_allele {
+                            2
+                        } else if v0 == homozygous_secondary_allele {
+                            two_code
+                        //                    v0 !=v0 is generic NAN check
+                        } else if (use_nan && v0 != v0) || (!use_nan && v0 == missing) {
+                            1
+                        } else {
+                            return Err(BedError::BadValue(filename.to_string()));
+                        };
+                        // Possible optimization: We could pre-compute the conversion, the division, the mod, and the multiply*2
+                        let i_div_4 = iid_i / 4;
+                        let i_mod_4 = iid_i % 4;
+                        bytes_vector[i_div_4] |= genotype_byte << (i_mod_4 * 2);
+                    }
+                    Ok(bytes_vector)
+                }
+            })
+            .threads(num_threads)
+            .try_for_each(|bytes_vector| {
+                // Write the bytes vector, they must be in order.
+                writer.write_all(&bytes_vector?)?;
+                Ok(())
+            })
+    })
+    .map_err(|_e| BedError::PanickedThread())?
 }
 
 fn count_lines(path_buf: PathBuf) -> Result<usize, BedErrorPlus> {
     let file = match File::open(&path_buf) {
         Err(_) => {
             let string_path = path_buf.to_string_lossy().to_string();
             return Err(BedErrorPlus::BedError(BedError::CannotOpenFamOrBim(
```

### Comparing `bed_reader-0.2.8/src/python_module.rs` & `bed_reader-0.2.9/src/python_module.rs`

 * *Files 2% similar despite different names*

```diff
@@ -147,45 +147,45 @@
         filename: &str,
         count_a1: bool,
         val: &PyArray2<f64>,
         num_threads: usize,
     ) -> Result<(), PyErr> {
         let val = unsafe { val.as_array() };
 
-        create_pool(num_threads)?.install(|| write(filename, &val, count_a1, f64::NAN))?;
+        write(filename, &val, count_a1, f64::NAN, num_threads)?;
 
         Ok(())
     }
 
     #[pyfn(m)]
     #[pyo3(name = "write_f32")]
     fn write_f32(
         filename: &str,
         count_a1: bool,
         val: &PyArray2<f32>,
         num_threads: usize,
     ) -> Result<(), PyErr> {
         let val = unsafe { val.as_array() };
 
-        create_pool(num_threads)?.install(|| write(filename, &val, count_a1, f32::NAN))?;
+        write(filename, &val, count_a1, f32::NAN, num_threads)?;
 
         Ok(())
     }
 
     #[pyfn(m)]
     #[pyo3(name = "write_i8")]
     fn write_i8(
         filename: &str,
         count_a1: bool,
         val: &PyArray2<i8>,
         num_threads: usize,
     ) -> Result<(), PyErr> {
         let val = unsafe { val.as_array() };
 
-        create_pool(num_threads)?.install(|| write(filename, &val, count_a1, -127))?;
+        write(filename, &val, count_a1, -127, num_threads)?;
 
         Ok(())
     }
 
     #[pyfn(m)]
     #[pyo3(name = "subset_f64_f64")]
     fn subset_f64_f64(
```

### Comparing `bed_reader-0.2.8/src/tests.rs` & `bed_reader-0.2.9/src/tests.rs`

 * *Files 1% similar despite different names*

```diff
@@ -280,59 +280,62 @@
     let filename = "bed_reader/tests/data/some_missing.bed";
     let val = read(filename, false, true, -127).unwrap();
 
     let temp = TempDir::default();
     let path2 = PathBuf::from(temp.as_ref()).join("rust_bed_reader_writer_test.bed");
     let filename2 = path2.as_os_str().to_str().unwrap();
 
-    write(filename2, &val.view(), true, -127).unwrap();
+    write(filename2, &val.view(), true, -127, 1).unwrap();
     for ext in ["fam", "bim"].iter() {
         let from = Path::new(filename).with_extension(ext);
         let to = Path::new(filename2).with_extension(ext);
         std::fs::copy(from, to).unwrap();
     }
 
     let val2 = read(filename2, false, true, -127).unwrap();
     assert!(allclose(&val.view(), &val2.view(), 0, true));
 
     let val = read(filename, false, true, f64::NAN).unwrap();
 
     let path2 = PathBuf::from(temp.as_ref()).join("rust_bed_reader_writer_testf64.bed");
     let filename2 = path2.as_os_str().to_str().unwrap();
 
-    write(filename2, &val.view(), true, f64::NAN).unwrap();
+    write(filename2, &val.view(), true, f64::NAN, 1).unwrap();
     for ext in ["fam", "bim"].iter() {
         let from = Path::new(filename).with_extension(ext);
         let to = Path::new(filename2).with_extension(ext);
         std::fs::copy(from, to).unwrap();
     }
 
     let val2 = read(filename2, false, true, f64::NAN).unwrap();
 
     assert!(allclose(&val.view(), &val2.view(), 1e-8, true));
 
     let mut val = read(filename, false, true, f64::NAN).unwrap();
     val[(0, 0)] = 5.0;
     let path = PathBuf::from(temp.as_ref()).join("rust_bed_reader_writer_testf64_5.bed");
     let filename = path.as_os_str().to_str().unwrap();
-    let result = write(filename, &val.view(), true, f64::NAN);
-    match result {
-        Err(BedErrorPlus::BedError(BedError::BadValue(_))) => (),
-        _ => panic!("test failure"),
+
+    if let Err(BedErrorPlus::BedError(BedError::BadValue(_))) =
+        write(filename, &val.view(), true, f64::NAN, 1)
+    {
+        assert!(!Path::new(filename).exists(), "file should not exist");
+    } else {
+        panic!("test failure")
     };
 
     let val = nd::Array2::zeros((0, 0));
     let path = PathBuf::from(temp.as_ref()).join("rust_bed_reader_writer_testf64_0s.bed");
     let filename = path.as_os_str().to_str().unwrap();
-    write(filename, &val.view(), true, f64::NAN).unwrap();
+    write(filename, &val.view(), true, f64::NAN, 1).unwrap();
 
     let val: nd::Array2<i8> = nd::Array2::zeros((3, 0));
     let path = PathBuf::from(temp.as_ref()).join("rust_bed_reader_writer_testf64_3_0.bed");
     let filename = path.as_os_str().to_str().unwrap();
-    write(filename, &val.view(), true, -127).unwrap();
+    write(filename, &val.view(), true, -127, 1).unwrap();
 }
 
 #[test]
 fn subset1() {
     let in_val1 = nd::arr3(&[
         [[0.0], [1.0], [2.0]],
         [[3.0], [4.0], [5.0]],
@@ -745,28 +748,28 @@
     matrix_subset_no_alloc(&(in_val.view()), &[], &[], &mut out_val.view_mut()).unwrap();
 
     // Writing zero length vals
     let temp = TempDir::default();
     let path = PathBuf::from(temp.as_ref()).join("rust_bed_reader_writer_zeros.bed");
     let filename = path.as_os_str().to_str().unwrap();
 
-    write(filename, &out_val01.view(), true, f64::NAN).unwrap();
+    write(filename, &out_val01.view(), true, f64::NAN, 1).unwrap();
     write_fake_metadata(filename, 0, sid_count);
     let result = read(filename, true, true, f64::NAN);
     let in_val01 = result.unwrap();
     assert!(in_val01.shape() == [0, sid_count]);
     assert!(allclose(&in_val01.view(), &out_val01.view(), 1e-08, true));
 
-    write(filename, &out_val10.view(), true, f64::NAN).unwrap();
+    write(filename, &out_val10.view(), true, f64::NAN, 1).unwrap();
     write_fake_metadata(filename, iid_count, 0);
     let in_val10 = read(filename, true, true, f64::NAN).unwrap();
     assert!(in_val10.shape() == [iid_count, 0]);
     assert!(allclose(&in_val10.view(), &out_val10.view(), 1e-08, true));
 
-    write(filename, &out_val00.view(), true, f64::NAN).unwrap();
+    write(filename, &out_val00.view(), true, f64::NAN, 1).unwrap();
     write_fake_metadata(filename, 0, 0);
     let in_val00 = read(filename, true, true, f64::NAN).unwrap();
     assert!(in_val00.shape() == [0, 0]);
     assert!(allclose(&in_val00.view(), &out_val00.view(), 1e-08, true));
 }
 #[test]
 fn file_ata_small() {
```

### Comparing `bed_reader-0.2.8/PKG-INFO` & `bed_reader-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bed-reader
-Version: 0.2.8
+Version: 0.2.9
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
 Requires-Dist: numpy>=1.13.3
@@ -13,17 +13,17 @@
 Summary: Read and write the PLINK BED format, simply and efficiently.
 Keywords: bioinformatics,plink,genomics,genetics,file-format,reader,genotype,bed-format,writer,python,snps
 Author: FaST-LMM Team <fastlmm-dev@python.org>
 Author-email: FaST-LMM Team <fastlmm-dev@python.org>
 License: Apache 2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Documentation, http://fastlmm.github.io/bed-reader
-Project-URL: Bug Tracker, https://github.com/fastlmm/bed-reader/issues
 Project-URL: Source Code, https://github.com/fastlmm/bed-reader
+Project-URL: Bug Tracker, https://github.com/fastlmm/bed-reader/issues
+Project-URL: Documentation, http://fastlmm.github.io/bed-reader
 Project-URL: Homepage, https://fastlmm.github.io
 
 [![PyPI version](https://badge.fury.io/py/bed-reader.svg)](https://badge.fury.io/py/bed-reader)
 [![Build Status](https://github.com/fastlmm/bed-reader/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/fastlmm/bed-reader/actions/workflows/ci.yml)
 ![PyPI](https://img.shields.io/pypi/v/bed-reader)
```

