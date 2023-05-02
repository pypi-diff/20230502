# Comparing `tmp/CoLT5-attention-0.3.7.tar.gz` & `tmp/CoLT5-attention-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CoLT5-attention-0.3.7.tar", last modified: Tue May  2 02:29:17 2023, max compression
+gzip compressed data, was "CoLT5-attention-0.3.8.tar", last modified: Tue May  2 03:10:11 2023, max compression
```

## Comparing `CoLT5-attention-0.3.7.tar` & `CoLT5-attention-0.3.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 02:29:17.358920 CoLT5-attention-0.3.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 02:29:17.354920 CoLT5-attention-0.3.7/CoLT5_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 02:29:17.000000 CoLT5-attention-0.3.7/CoLT5_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-02 02:29:17.000000 CoLT5-attention-0.3.7/CoLT5_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 02:29:17.000000 CoLT5-attention-0.3.7/CoLT5_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-02 02:29:17.000000 CoLT5-attention-0.3.7/CoLT5_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 02:29:17.000000 CoLT5-attention-0.3.7/CoLT5_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-02 02:29:04.000000 CoLT5-attention-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 02:29:17.358920 CoLT5-attention-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-05-02 02:29:04.000000 CoLT5-attention-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 02:29:17.358920 CoLT5-attention-0.3.7/colt5_attention/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-02 02:29:04.000000 CoLT5-attention-0.3.7/colt5_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-02 02:29:04.000000 CoLT5-attention-0.3.7/colt5_attention/coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-02 02:29:04.000000 CoLT5-attention-0.3.7/colt5_attention/sinkhorn.py
--rw-r--r--   0 runner    (1001) docker     (123)    31461 2023-05-02 02:29:04.000000 CoLT5-attention-0.3.7/colt5_attention/transformer_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-05-02 02:29:04.000000 CoLT5-attention-0.3.7/colt5_attention/triton_coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 02:29:17.358920 CoLT5-attention-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-02 02:29:04.000000 CoLT5-attention-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:10:11.117909 CoLT5-attention-0.3.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:10:11.113909 CoLT5-attention-0.3.8/CoLT5_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 03:10:11.000000 CoLT5-attention-0.3.8/CoLT5_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-02 03:10:11.000000 CoLT5-attention-0.3.8/CoLT5_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 03:10:11.000000 CoLT5-attention-0.3.8/CoLT5_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-02 03:10:11.000000 CoLT5-attention-0.3.8/CoLT5_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 03:10:11.000000 CoLT5-attention-0.3.8/CoLT5_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-02 03:09:59.000000 CoLT5-attention-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 03:10:11.113909 CoLT5-attention-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-05-02 03:09:59.000000 CoLT5-attention-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:10:11.113909 CoLT5-attention-0.3.8/colt5_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-02 03:09:59.000000 CoLT5-attention-0.3.8/colt5_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-02 03:09:59.000000 CoLT5-attention-0.3.8/colt5_attention/coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-02 03:09:59.000000 CoLT5-attention-0.3.8/colt5_attention/sinkhorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31461 2023-05-02 03:09:59.000000 CoLT5-attention-0.3.8/colt5_attention/transformer_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-05-02 03:09:59.000000 CoLT5-attention-0.3.8/colt5_attention/triton_coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 03:10:11.117909 CoLT5-attention-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-02 03:09:59.000000 CoLT5-attention-0.3.8/setup.py
```

### Comparing `CoLT5-attention-0.3.7/CoLT5_attention.egg-info/PKG-INFO` & `CoLT5-attention-0.3.8/CoLT5_attention.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.3.7
+Version: 0.3.8
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.3.7/LICENSE` & `CoLT5-attention-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.3.7/PKG-INFO` & `CoLT5-attention-0.3.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.3.7
+Version: 0.3.8
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.3.7/README.md` & `CoLT5-attention-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.3.7/colt5_attention/coor_descent.py` & `CoLT5-attention-0.3.8/colt5_attention/coor_descent.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.3.7/colt5_attention/sinkhorn.py` & `CoLT5-attention-0.3.8/colt5_attention/sinkhorn.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.3.7/colt5_attention/transformer_block.py` & `CoLT5-attention-0.3.8/colt5_attention/transformer_block.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.3.7/colt5_attention/triton_coor_descent.py` & `CoLT5-attention-0.3.8/colt5_attention/triton_coor_descent.py`

 * *Files 3% similar despite different names*

```diff
@@ -228,20 +228,25 @@
     @classmethod
     def forward(
         self,
         ctx,
         x,
         n_iters,
         k,
-        eps
+        eps,
+        mask
     ):
         assert x.is_cuda
 
         batch, requires_grad = x.shape[0], x.requires_grad
 
+        if exists(mask):
+            mask_value = -torch.finfo(x.dtype).max
+            x = x.masked_fill(~mask, mask_value)
+
         x, shape = pack_one(x, '* n')
 
         n_rows, n_cols = x.shape
 
         if isinstance(k, (int, float)):
             k = torch.full((n_rows,), k)
 
@@ -305,10 +310,18 @@
             n_iters,
             eps,
             n_cols,
             num_warps = num_warps,
             BLOCK_SIZE = BLOCK_SIZE
         )
 
-        return unpack_one(dx, shape, '* n'), None, None, None
+        return unpack_one(dx, shape, '* n'), None, None, None, None
 
-triton_coor_descent = _coor_descent.apply
+def triton_coor_descent(
+    s,
+    *,
+    n_iters,
+    k,
+    eps = 1e-1,
+    mask = None
+):
+    return _coor_descent.apply(s, n_iters, k, eps, mask)
```

### Comparing `CoLT5-attention-0.3.7/setup.py` & `CoLT5-attention-0.3.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'CoLT5-attention',
   packages = find_packages(),
-  version = '0.3.7',
+  version = '0.3.8',
   license='MIT',
   description = 'Conditionally Routed Attention',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/CoLT5-attention',
   keywords = [
```

