# Comparing `tmp/bhv-0.2.5.tar.gz` & `tmp/bhv-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bhv-0.2.5.tar", last modified: Sat Apr 29 19:08:25 2023, max compression
+gzip compressed data, was "bhv-0.2.6.tar", last modified: Tue May  2 19:26:51 2023, max compression
```

## Comparing `bhv-0.2.5.tar` & `bhv-0.2.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-04-29 19:08:25.402615 bhv-0.2.5/
--rw-r--r--   0 adamv     (1000) adamv     (1000)    35149 2023-04-23 16:58:42.000000 bhv-0.2.5/LICENSE
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1027 2023-04-29 19:08:25.402615 bhv-0.2.5/PKG-INFO
--rw-r--r--   0 adamv     (1000) adamv     (1000)     3202 2023-04-29 09:52:26.000000 bhv-0.2.5/README.md
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-04-29 19:08:25.402615 bhv-0.2.5/bhv/
--rw-r--r--   0 adamv     (1000) adamv     (1000)       64 2023-04-24 11:50:09.000000 bhv-0.2.5/bhv/__init__.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    11962 2023-04-28 20:37:06.000000 bhv-0.2.5/bhv/abstract.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1635 2023-04-11 14:49:00.000000 bhv-0.2.5/bhv/embedding.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    11175 2023-04-18 17:00:07.000000 bhv-0.2.5/bhv/np.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    11425 2023-04-24 21:41:56.000000 bhv-0.2.5/bhv/poibin.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1683 2023-04-28 18:20:39.000000 bhv-0.2.5/bhv/positions.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     8193 2023-04-18 19:16:09.000000 bhv-0.2.5/bhv/pytorch.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2356 2023-04-28 22:56:24.000000 bhv-0.2.5/bhv/shared.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1152 2023-04-24 02:20:49.000000 bhv-0.2.5/bhv/slice.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    21307 2023-04-29 09:47:12.000000 bhv-0.2.5/bhv/symbolic.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     3325 2023-04-28 20:51:52.000000 bhv-0.2.5/bhv/vanilla.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)      782 2023-04-28 16:55:18.000000 bhv-0.2.5/bhv/visualization.py
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-04-29 19:08:25.402615 bhv-0.2.5/bhv.egg-info/
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1027 2023-04-29 19:08:25.000000 bhv-0.2.5/bhv.egg-info/PKG-INFO
--rw-r--r--   0 adamv     (1000) adamv     (1000)      344 2023-04-29 19:08:25.000000 bhv-0.2.5/bhv.egg-info/SOURCES.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)        1 2023-04-29 19:08:25.000000 bhv-0.2.5/bhv.egg-info/dependency_links.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)       73 2023-04-29 19:08:25.000000 bhv-0.2.5/bhv.egg-info/requires.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)        4 2023-04-29 19:08:25.000000 bhv-0.2.5/bhv.egg-info/top_level.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)       38 2023-04-29 19:08:25.402615 bhv-0.2.5/setup.cfg
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1331 2023-04-29 19:07:56.000000 bhv-0.2.5/setup.py
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-02 19:26:51.645224 bhv-0.2.6/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    35149 2023-04-23 16:58:42.000000 bhv-0.2.6/LICENSE
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1027 2023-05-02 19:26:51.645224 bhv-0.2.6/PKG-INFO
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     3202 2023-04-29 09:52:26.000000 bhv-0.2.6/README.md
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-02 19:26:51.645224 bhv-0.2.6/bhv/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       64 2023-04-24 11:50:09.000000 bhv-0.2.6/bhv/__init__.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    11962 2023-04-28 20:37:06.000000 bhv-0.2.6/bhv/abstract.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1635 2023-04-11 14:49:00.000000 bhv-0.2.6/bhv/embedding.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    11207 2023-05-02 19:20:22.000000 bhv-0.2.6/bhv/np.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    11425 2023-04-24 21:41:56.000000 bhv-0.2.6/bhv/poibin.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1683 2023-04-28 18:20:39.000000 bhv-0.2.6/bhv/positions.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     8226 2023-05-02 19:26:10.000000 bhv-0.2.6/bhv/pytorch.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2356 2023-04-28 22:56:24.000000 bhv-0.2.6/bhv/shared.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1152 2023-04-24 02:20:49.000000 bhv-0.2.6/bhv/slice.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    21307 2023-05-02 16:47:02.000000 bhv-0.2.6/bhv/symbolic.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     3325 2023-04-28 20:51:52.000000 bhv-0.2.6/bhv/vanilla.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      782 2023-04-28 16:55:18.000000 bhv-0.2.6/bhv/visualization.py
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-02 19:26:51.645224 bhv-0.2.6/bhv.egg-info/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1027 2023-05-02 19:26:51.000000 bhv-0.2.6/bhv.egg-info/PKG-INFO
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      344 2023-05-02 19:26:51.000000 bhv-0.2.6/bhv.egg-info/SOURCES.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)        1 2023-05-02 19:26:51.000000 bhv-0.2.6/bhv.egg-info/dependency_links.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       73 2023-05-02 19:26:51.000000 bhv-0.2.6/bhv.egg-info/requires.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)        4 2023-05-02 19:26:51.000000 bhv-0.2.6/bhv.egg-info/top_level.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       38 2023-05-02 19:26:51.645224 bhv-0.2.6/setup.cfg
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1331 2023-05-02 19:26:36.000000 bhv-0.2.6/setup.py
```

### Comparing `bhv-0.2.5/LICENSE` & `bhv-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bhv-0.2.5/PKG-INFO` & `bhv-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.2.5
+Version: 0.2.6
 Summary: Boolean Hypervectors
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 Keywords: ai binary hypervector hdc bsc
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bhv-0.2.5/README.md` & `bhv-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `bhv-0.2.5/bhv/abstract.py` & `bhv-0.2.6/bhv/abstract.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.5/bhv/embedding.py` & `bhv-0.2.6/bhv/embedding.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.5/bhv/np.py` & `bhv-0.2.6/bhv/np.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     @classmethod
     def majority(cls, vs: list['NumPyBoolBHV']) -> 'NumPyBoolBHV':
         data = [v.data for v in vs]
         extra = [cls.rand().data] if len(vs) % 2 == 0 else []
 
         tensor = np.stack(data + extra)
-        counts = tensor.sum(axis=-2, dtype=np.uint8)
+        counts = tensor.sum(axis=-2, dtype=np.uint8 if len(vs) < 256 else np.uint32)
 
         threshold = (len(vs) + len(extra))//2
 
         return NumPyBoolBHV(np.greater(counts, threshold))
 
     def __eq__(self, other: 'NumPyBoolBHV') -> bool:
         return np.array_equal(self.data, other.data)
```

### Comparing `bhv-0.2.5/bhv/poibin.py` & `bhv-0.2.6/bhv/poibin.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.5/bhv/positions.py` & `bhv-0.2.6/bhv/positions.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.5/bhv/pytorch.py` & `bhv-0.2.6/bhv/pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,17 +67,17 @@
 
     @classmethod
     def majority(cls, vs: list['TorchBoolBHV']) -> 'TorchBoolBHV':
         data = [v.data for v in vs]
         extra = [cls.rand().data] if len(vs) % 2 == 0 else []
 
         tensor = torch.stack(data + extra)
-        counts = tensor.sum(dim=-2, dtype=torch.int8)
+        counts = tensor.sum(dim=-2, dtype=torch.uint8 if len(vs) < 256 else torch.int32)
 
-        threshold = (len(vs) + len(extra)) // 2
+        threshold = (len(vs) + len(extra))//2
 
         return TorchBoolBHV(torch.greater(counts,  threshold).to(torch.bool))
 
     def roll_bits(self, n: int) -> 'TorchBoolBHV':
         return TorchBoolBHV(torch.roll(self.data, n))
 
     def permute_bits(self, permutation: TorchBoolPermutation) -> 'TorchBoolBHV':
```

### Comparing `bhv-0.2.5/bhv/shared.py` & `bhv-0.2.6/bhv/shared.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.5/bhv/slice.py` & `bhv-0.2.6/bhv/slice.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.5/bhv/symbolic.py` & `bhv-0.2.6/bhv/symbolic.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.5/bhv/vanilla.py` & `bhv-0.2.6/bhv/vanilla.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.5/bhv/visualization.py` & `bhv-0.2.6/bhv/visualization.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.5/bhv.egg-info/PKG-INFO` & `bhv-0.2.6/bhv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.2.5
+Version: 0.2.6
 Summary: Boolean Hypervectors
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 Keywords: ai binary hypervector hdc bsc
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bhv-0.2.5/setup.py` & `bhv-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.5'
+VERSION = '0.2.6'
 DESCRIPTION = 'Boolean Hypervectors'
 LONG_DESCRIPTION = 'Boolean Hypervectors with various operators for experiments in hyperdimensional computing (HDC).'
 
 setup(
     name="bhv",
     version=VERSION,
     author="Adam Vandervorst",
```

