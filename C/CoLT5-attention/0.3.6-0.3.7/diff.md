# Comparing `tmp/CoLT5-attention-0.3.6.tar.gz` & `tmp/CoLT5-attention-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CoLT5-attention-0.3.6.tar", last modified: Mon May  1 16:52:34 2023, max compression
+gzip compressed data, was "CoLT5-attention-0.3.7.tar", last modified: Tue May  2 02:29:17 2023, max compression
```

## Comparing `CoLT5-attention-0.3.6.tar` & `CoLT5-attention-0.3.7.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:52:34.509534 CoLT5-attention-0.3.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:52:34.505534 CoLT5-attention-0.3.6/CoLT5_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-01 16:52:34.000000 CoLT5-attention-0.3.6/CoLT5_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-01 16:52:34.000000 CoLT5-attention-0.3.6/CoLT5_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 16:52:34.000000 CoLT5-attention-0.3.6/CoLT5_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-01 16:52:34.000000 CoLT5-attention-0.3.6/CoLT5_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-01 16:52:34.000000 CoLT5-attention-0.3.6/CoLT5_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-01 16:52:17.000000 CoLT5-attention-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-01 16:52:34.509534 CoLT5-attention-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-05-01 16:52:17.000000 CoLT5-attention-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:52:34.509534 CoLT5-attention-0.3.6/colt5_attention/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-01 16:52:17.000000 CoLT5-attention-0.3.6/colt5_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-01 16:52:17.000000 CoLT5-attention-0.3.6/colt5_attention/coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-01 16:52:17.000000 CoLT5-attention-0.3.6/colt5_attention/sinkhorn.py
--rw-r--r--   0 runner    (1001) docker     (123)    31461 2023-05-01 16:52:17.000000 CoLT5-attention-0.3.6/colt5_attention/transformer_block.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 16:52:34.509534 CoLT5-attention-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-01 16:52:17.000000 CoLT5-attention-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 02:29:17.358920 CoLT5-attention-0.3.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 02:29:17.354920 CoLT5-attention-0.3.7/CoLT5_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 02:29:17.000000 CoLT5-attention-0.3.7/CoLT5_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-02 02:29:17.000000 CoLT5-attention-0.3.7/CoLT5_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 02:29:17.000000 CoLT5-attention-0.3.7/CoLT5_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-02 02:29:17.000000 CoLT5-attention-0.3.7/CoLT5_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 02:29:17.000000 CoLT5-attention-0.3.7/CoLT5_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-02 02:29:04.000000 CoLT5-attention-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 02:29:17.358920 CoLT5-attention-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-05-02 02:29:04.000000 CoLT5-attention-0.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 02:29:17.358920 CoLT5-attention-0.3.7/colt5_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-02 02:29:04.000000 CoLT5-attention-0.3.7/colt5_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-02 02:29:04.000000 CoLT5-attention-0.3.7/colt5_attention/coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-02 02:29:04.000000 CoLT5-attention-0.3.7/colt5_attention/sinkhorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31461 2023-05-02 02:29:04.000000 CoLT5-attention-0.3.7/colt5_attention/transformer_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-05-02 02:29:04.000000 CoLT5-attention-0.3.7/colt5_attention/triton_coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 02:29:17.358920 CoLT5-attention-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-02 02:29:04.000000 CoLT5-attention-0.3.7/setup.py
```

### Comparing `CoLT5-attention-0.3.6/CoLT5_attention.egg-info/PKG-INFO` & `CoLT5-attention-0.3.7/CoLT5_attention.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.3.6
+Version: 0.3.7
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.3.6/LICENSE` & `CoLT5-attention-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.3.6/PKG-INFO` & `CoLT5-attention-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.3.6
+Version: 0.3.7
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.3.6/README.md` & `CoLT5-attention-0.3.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -120,23 +120,25 @@
 ```
 
 ## Todo
 
 - [x] add the coordinate descent method as another router
 - [x] allow for multi-headed routing (multiple routing tokens), only for key-values
 - [x] add an autoregressive version of the conditionally routed attention
+- [x] test out the autoregressive version and verify that more routed key / value tokens lead to better results - it works
 
-- [ ] test out the autoregressive version and verify that more routed key / value tokens lead to better results
 - [ ] for variable sequence lengths, allow for setting k as a function of sequence lengths per sample in batch
 - [ ] create a variant of CoLT5 for high resolution feature maps (image attention) - then try out for diffusion
 - [ ] in the cross attention scenario, support for routing token that first queries the source tokens, before retrieving from memories
 - [ ] make flash attention compatible
 - [ ] fused coordinate descent kernel using triton
-    - [ ] forwards
-    - [ ] backwards
+    - [x] forwards        
+    - [x] backwards
+    - [ ] allow for saving intermediates every number of iterations - trading memory for recompute efficiency during backwards
+    - [ ] add some tests and benchmark for triton vs plain pytorch coor_descent
 
 ## Citations
 
 ```bibtex
 @inproceedings{Ainslie2023CoLT5FL,
     title   = {CoLT5: Faster Long-Range Transformers with Conditional Computation},
     author  = {Joshua Ainslie and Tao Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and Yury Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and Yun-Hsuan Sung and Sumit Sanghai},
```

#### html2text {}

```diff
@@ -47,22 +47,25 @@
 tokens to route different sets of key / values to the queries. 4 attention
 heads will be allocated to each routed set in this example (8 / 2) ).cuda()
 cross_attn_out = cross_attn( tokens, context = memories, mask = tokens_mask,
 context_mask = memories_mask ) cross_attn_out.shape # (2, 1024, 512) - same as
 tokens ``` ## Todo - [x] add the coordinate descent method as another router -
 [x] allow for multi-headed routing (multiple routing tokens), only for key-
 values - [x] add an autoregressive version of the conditionally routed
-attention - [ ] test out the autoregressive version and verify that more routed
-key / value tokens lead to better results - [ ] for variable sequence lengths,
-allow for setting k as a function of sequence lengths per sample in batch - [ ]
-create a variant of CoLT5 for high resolution feature maps (image attention) -
-then try out for diffusion - [ ] in the cross attention scenario, support for
-routing token that first queries the source tokens, before retrieving from
-memories - [ ] make flash attention compatible - [ ] fused coordinate descent
-kernel using triton - [ ] forwards - [ ] backwards ## Citations ```bibtex
+attention - [x] test out the autoregressive version and verify that more routed
+key / value tokens lead to better results - it works - [ ] for variable
+sequence lengths, allow for setting k as a function of sequence lengths per
+sample in batch - [ ] create a variant of CoLT5 for high resolution feature
+maps (image attention) - then try out for diffusion - [ ] in the cross
+attention scenario, support for routing token that first queries the source
+tokens, before retrieving from memories - [ ] make flash attention compatible -
+[ ] fused coordinate descent kernel using triton - [x] forwards - [x] backwards
+- [ ] allow for saving intermediates every number of iterations - trading
+memory for recompute efficiency during backwards - [ ] add some tests and
+benchmark for triton vs plain pytorch coor_descent ## Citations ```bibtex
 @inproceedings{Ainslie2023CoLT5FL, title = {CoLT5: Faster Long-Range
 Transformers with Conditional Computation}, author = {Joshua Ainslie and Tao
 Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and Yury
 Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and
 Yun-Hsuan Sung and Sumit Sanghai}, year = {2023} } ``` ```bibtex @article
 {Tillet2019TritonAI, title = {Triton: an intermediate language and compiler for
 tiled neural network computations}, author = {Philippe Tillet and H. Kung and
```

### Comparing `CoLT5-attention-0.3.6/colt5_attention/coor_descent.py` & `CoLT5-attention-0.3.7/colt5_attention/coor_descent.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import torch
 import torch.nn.functional as F
 
+from einops import rearrange
+
 def exists(val):
     return val is not None
 
 def log(t, eps = 1e-20):
     return torch.log(t.clamp(min = eps))
 
 def coor_descent(
@@ -15,24 +17,25 @@
     eps = 1e-1,
     mask = None
 ):
     mask_value = -torch.finfo(s.dtype).max
 
     if not isinstance(k, torch.Tensor):
         k = torch.Tensor([k]).to(s)
+    else:
+        k = rearrange(k, '... -> ... 1')
 
     constant = eps * log(k)
 
+    if exists(mask):
+        s = s.masked_fill(~mask, mask_value)
+
+    a = 0
     b = -F.relu(s)
 
     for _ in range(n_iters):
-        if exists(mask):
-            s = s.masked_fill(~mask, mask_value)
 
         a = constant - eps * ((s + b) / eps).logsumexp(dim = -1, keepdim = True)
         b = -F.relu(s + a)
 
-    if exists(mask):
-        s = s.masked_fill(~mask, mask_value)
-
     scores = ((s + a + b) / eps).exp()
     return scores
```

### Comparing `CoLT5-attention-0.3.6/colt5_attention/sinkhorn.py` & `CoLT5-attention-0.3.7/colt5_attention/sinkhorn.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.3.6/colt5_attention/transformer_block.py` & `CoLT5-attention-0.3.7/colt5_attention/transformer_block.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.3.6/setup.py` & `CoLT5-attention-0.3.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'CoLT5-attention',
   packages = find_packages(),
-  version = '0.3.6',
+  version = '0.3.7',
   license='MIT',
   description = 'Conditionally Routed Attention',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/CoLT5-attention',
   keywords = [
     'artificial intelligence',
     'attention mechanism',
     'dynamic routing'
   ],
   install_requires=[
     'einops>=0.6.1',
     'local-attention>=1.8.5',
+    'packaging',
     'torch>=1.10'
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'License :: OSI Approved :: MIT License',
```

