# Comparing `tmp/CoLT5-attention-0.4.0.tar.gz` & `tmp/CoLT5-attention-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CoLT5-attention-0.4.0.tar", last modified: Tue May  2 15:27:57 2023, max compression
+gzip compressed data, was "CoLT5-attention-0.4.1.tar", last modified: Tue May  2 16:02:57 2023, max compression
```

## Comparing `CoLT5-attention-0.4.0.tar` & `CoLT5-attention-0.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:27:57.361344 CoLT5-attention-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:27:57.361344 CoLT5-attention-0.4.0/CoLT5_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 15:27:57.000000 CoLT5-attention-0.4.0/CoLT5_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-02 15:27:57.000000 CoLT5-attention-0.4.0/CoLT5_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:27:57.000000 CoLT5-attention-0.4.0/CoLT5_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-02 15:27:57.000000 CoLT5-attention-0.4.0/CoLT5_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 15:27:57.000000 CoLT5-attention-0.4.0/CoLT5_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-02 15:27:40.000000 CoLT5-attention-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 15:27:57.361344 CoLT5-attention-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-05-02 15:27:40.000000 CoLT5-attention-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:27:57.361344 CoLT5-attention-0.4.0/colt5_attention/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-02 15:27:40.000000 CoLT5-attention-0.4.0/colt5_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-02 15:27:40.000000 CoLT5-attention-0.4.0/colt5_attention/coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-02 15:27:40.000000 CoLT5-attention-0.4.0/colt5_attention/sinkhorn.py
--rw-r--r--   0 runner    (1001) docker     (123)    32472 2023-05-02 15:27:40.000000 CoLT5-attention-0.4.0/colt5_attention/transformer_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-05-02 15:27:40.000000 CoLT5-attention-0.4.0/colt5_attention/triton_coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 15:27:57.361344 CoLT5-attention-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-02 15:27:40.000000 CoLT5-attention-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:02:57.496088 CoLT5-attention-0.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:02:57.496088 CoLT5-attention-0.4.1/CoLT5_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 16:02:57.000000 CoLT5-attention-0.4.1/CoLT5_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-02 16:02:57.000000 CoLT5-attention-0.4.1/CoLT5_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 16:02:57.000000 CoLT5-attention-0.4.1/CoLT5_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-02 16:02:57.000000 CoLT5-attention-0.4.1/CoLT5_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 16:02:57.000000 CoLT5-attention-0.4.1/CoLT5_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-02 16:02:43.000000 CoLT5-attention-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 16:02:57.496088 CoLT5-attention-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-05-02 16:02:43.000000 CoLT5-attention-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:02:57.496088 CoLT5-attention-0.4.1/colt5_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-02 16:02:43.000000 CoLT5-attention-0.4.1/colt5_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-02 16:02:43.000000 CoLT5-attention-0.4.1/colt5_attention/coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-02 16:02:43.000000 CoLT5-attention-0.4.1/colt5_attention/sinkhorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32478 2023-05-02 16:02:43.000000 CoLT5-attention-0.4.1/colt5_attention/transformer_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-05-02 16:02:43.000000 CoLT5-attention-0.4.1/colt5_attention/triton_coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 16:02:57.496088 CoLT5-attention-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-02 16:02:43.000000 CoLT5-attention-0.4.1/setup.py
```

### Comparing `CoLT5-attention-0.4.0/CoLT5_attention.egg-info/PKG-INFO` & `CoLT5-attention-0.4.1/CoLT5_attention.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.4.0
+Version: 0.4.1
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.4.0/LICENSE` & `CoLT5-attention-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.4.0/PKG-INFO` & `CoLT5-attention-0.4.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.4.0
+Version: 0.4.1
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.4.0/README.md` & `CoLT5-attention-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -130,17 +130,18 @@
 - [ ] create a variant of CoLT5 for high resolution feature maps (image attention) - then try out for diffusion
 - [ ] in the cross attention scenario, support for routing token that first queries the source tokens, before retrieving from memories
 - [ ] make flash attention compatible
 - [ ] fused coordinate descent kernel using triton
     - [x] forwards        
     - [x] backwards
     - [x] add some tests and benchmark for triton vs plain pytorch coor_descent - 25x faster for forward, 1.5x faster for backwards and memory saved is n_iters times
+    - [x] fall back on plain coordinate descent for cpu
     - [ ] allow for saving intermediates every number of iterations - trading memory for recompute efficiency during backwards
     - [ ] maximum block size in triton allowed is 131k, make sure at least quarter of million sequence length can be reached
-    - [ ] fall back on plain coordinate descent for cpu
+    - [ ] handle edge case for when a row is completely masked out for triton, or simply enforce it never to be so
 
 ## Citations
 
 ```bibtex
 @inproceedings{Ainslie2023CoLT5FL,
     title   = {CoLT5: Faster Long-Range Transformers with Conditional Computation},
     author  = {Joshua Ainslie and Tao Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and Yury Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and Yun-Hsuan Sung and Sumit Sanghai},
```

#### html2text {}

```diff
@@ -57,20 +57,22 @@
 sample in batch - [ ] create a variant of CoLT5 for high resolution feature
 maps (image attention) - then try out for diffusion - [ ] in the cross
 attention scenario, support for routing token that first queries the source
 tokens, before retrieving from memories - [ ] make flash attention compatible -
 [ ] fused coordinate descent kernel using triton - [x] forwards - [x] backwards
 - [x] add some tests and benchmark for triton vs plain pytorch coor_descent -
 25x faster for forward, 1.5x faster for backwards and memory saved is n_iters
-times - [ ] allow for saving intermediates every number of iterations - trading
-memory for recompute efficiency during backwards - [ ] maximum block size in
-triton allowed is 131k, make sure at least quarter of million sequence length
-can be reached - [ ] fall back on plain coordinate descent for cpu ## Citations
-```bibtex @inproceedings{Ainslie2023CoLT5FL, title = {CoLT5: Faster Long-Range
-Transformers with Conditional Computation}, author = {Joshua Ainslie and Tao
-Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and Yury
-Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and
-Yun-Hsuan Sung and Sumit Sanghai}, year = {2023} } ``` ```bibtex @article
-{Tillet2019TritonAI, title = {Triton: an intermediate language and compiler for
-tiled neural network computations}, author = {Philippe Tillet and H. Kung and
-D. Cox}, journal = {Proceedings of the 3rd ACM SIGPLAN International Workshop
-on Machine Learning and Programming Languages}, year = {2019} } ```
+times - [x] fall back on plain coordinate descent for cpu - [ ] allow for
+saving intermediates every number of iterations - trading memory for recompute
+efficiency during backwards - [ ] maximum block size in triton allowed is 131k,
+make sure at least quarter of million sequence length can be reached - [ ]
+handle edge case for when a row is completely masked out for triton, or simply
+enforce it never to be so ## Citations ```bibtex @inproceedings
+{Ainslie2023CoLT5FL, title = {CoLT5: Faster Long-Range Transformers with
+Conditional Computation}, author = {Joshua Ainslie and Tao Lei and Michiel de
+Jong and Santiago Ontan'on and Siddhartha Brahma and Yury Zemlyanskiy and David
+Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and Yun-Hsuan Sung and Sumit
+Sanghai}, year = {2023} } ``` ```bibtex @article{Tillet2019TritonAI, title =
+{Triton: an intermediate language and compiler for tiled neural network
+computations}, author = {Philippe Tillet and H. Kung and D. Cox}, journal =
+{Proceedings of the 3rd ACM SIGPLAN International Workshop on Machine Learning
+and Programming Languages}, year = {2019} } ```
```

### Comparing `CoLT5-attention-0.4.0/colt5_attention/coor_descent.py` & `CoLT5-attention-0.4.1/colt5_attention/coor_descent.py`

 * *Files 21% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     constant = eps * log(k)
 
     if exists(mask):
         s = s.masked_fill(~mask, mask_value)
 
     a = 0
-    b = -F.relu(s)
+    b = -s
 
     for _ in range(n_iters):
 
         a = constant - eps * ((s + b) / eps).logsumexp(dim = -1, keepdim = True)
         b = -F.relu(s + a)
 
     scores = ((s + a + b) / eps).exp()
```

### Comparing `CoLT5-attention-0.4.0/colt5_attention/sinkhorn.py` & `CoLT5-attention-0.4.1/colt5_attention/sinkhorn.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.4.0/colt5_attention/transformer_block.py` & `CoLT5-attention-0.4.1/colt5_attention/transformer_block.py`

 * *Files 0% similar despite different names*

```diff
@@ -916,15 +916,15 @@
         normalized_scores_kv = None
 
         should_route_kv = key_value_length > num_tokens_kv
 
         if should_route_kv:
             normalized_scores_kv, indices_kv = self.kv_router(context, num_tokens = num_tokens_kv, mask = context_mask)
 
-            routed_tokens_kv = batched_gather(x, indices_kv)
+            routed_tokens_kv = batched_gather(context, indices_kv)
 
             routed_tokens_kv_mask = None
             if exists(context_mask):
                 routed_tokens_kv_mask = batched_gather(context_mask, indices_kv)
 
         # do the heavier branch with only routed tokens
```

### Comparing `CoLT5-attention-0.4.0/colt5_attention/triton_coor_descent.py` & `CoLT5-attention-0.4.1/colt5_attention/triton_coor_descent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from math import log
 
 import torch
 from torch import Tensor
 from torch import autograd
 import torch.nn.functional as F
 
+from colt5_attention.coor_descent import coor_descent
 from einops import pack, unpack, repeat
 
 try:
     import triton
     import triton.language as tl
 except ImportError as e:
     print('triton is not installed, please install by running `pip install triton -U --pre`')
@@ -69,22 +70,24 @@
 
     # load k - controls the sparsity of output
 
     k = tl.load(k_ptr)
 
     constant = tl.log(k) * eps
 
+    inv_eps = 1. / eps
+
     # initialize a and b for coordinate descent
 
     a = k * 0                           # init a to 0, triton needs to know shape and type outside loop
-    b = tl.where(s >= 0., -s, 0.)
+    b = -s
 
     for _ in range(n_iters):        
 
-        a = (s + b) / eps
+        a = (s + b) * inv_eps
 
         # stable log sum exp
 
         a_max = tl.max(a, axis = 0)
         a_minus_max = a - a_max
         exp = tl.exp(a_minus_max)
         sum_exp = tl.sum(exp, axis = 0)
@@ -93,15 +96,15 @@
         a = constant - eps * log_sum_exp
 
         # update b
 
         b = s + a
         b = tl.where(b >= 0., -b, 0.)
 
-    s = tl.exp((s + a + b) / eps)
+    s = tl.exp((s + a + b) * inv_eps)
 
     output_row_start_ptr = output_ptr + row_idx * output_row_stride
     output_ptrs = output_row_start_ptr + col_offsets
 
     tl.store(output_ptrs, s, mask = mask)
 
 # backwards
@@ -145,35 +148,37 @@
     grad_ptrs = grad_row_start_ptr + col_offsets
 
     grad_row = tl.load(grad_ptrs, mask = mask, other = 0.)
 
     # recompute
 
     init_a = k * 0
-    init_b = tl.where(s >= 0., -s, 0.)
+    init_b = -s
 
     ds = s * 0
     db = s * 0
     last_da = k * 0
 
+    inv_eps = 1. / eps
+
     # backwards
 
     for ind in range(n_iters):
         is_first = ind == 0
 
         a = init_a
         b = init_b
 
         sa = s * 0
         exp = s * 0
         sum_exp = k * 0
 
         for _ in range(n_iters - ind):
 
-            sb = (s + b) / eps
+            sb = (s + b) * inv_eps
 
             # stable log sum exp
 
             sb_max = tl.max(sb, axis = 0)
             sb_minus_max = sb - sb_max
             exp = tl.exp(sb_minus_max)
             sum_exp = tl.sum(exp, axis = 0)
@@ -183,18 +188,18 @@
 
             # update b
 
             sa = s + a
             b = tl.where(sa >= 0., -sa, 0.)
 
         if is_first:
-            o = tl.exp((s + a + b) / eps)
+            o = tl.exp((s + a + b) * inv_eps)
 
             ds = grad_row * o
-            ds /= eps
+            ds *= inv_eps
 
             last_da = tl.sum(ds, axis = 0)
             db = ds
 
         # go backwards
 
         if n_iters > 0:
@@ -202,22 +207,22 @@
             dsa = db * tl.where(sa >= 0, -1., 0.)
             ds += dsa
 
             da = tl.sum(dsa, axis = 0) + last_da
             da *= -eps
 
             dsb = exp * da / sum_exp
-            dsb /= eps
+            dsb *= inv_eps
 
             ds += dsb
             db = dsb
 
             last_da = 0.
 
-    ds += db * tl.where(s >= 0., -1., 0.)
+    ds += -db
 
     # store output
 
     output_row_start_ptr = output_ptr + row_idx * output_row_stride
     output_ptrs = output_row_start_ptr + col_offsets
 
     tl.store(output_ptrs, ds, mask = mask)
@@ -271,15 +276,20 @@
             BLOCK_SIZE = BLOCK_SIZE,
         )
 
         if requires_grad:
             ctx.args = (n_iters, eps)
             ctx.save_for_backward(x, k)
 
-        return unpack_one(y, shape, '* n')
+        y = unpack_one(y, shape, '* n')
+
+        if exists(mask):
+            y = y.masked_fill(~mask, 0.)
+
+        return y
 
     @classmethod
     def backward(
         self,
         ctx,
         grad_probs
     ):
@@ -320,8 +330,11 @@
     s,
     *,
     n_iters,
     k,
     eps = 1e-1,
     mask = None
 ):
+    if not s.is_cuda:
+        return coor_descent(s, n_iters = n_iters, k = k, eps = eps, mask = mask)
+
     return _coor_descent.apply(s, n_iters, k, eps, mask)
```

### Comparing `CoLT5-attention-0.4.0/setup.py` & `CoLT5-attention-0.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'CoLT5-attention',
   packages = find_packages(),
-  version = '0.4.0',
+  version = '0.4.1',
   license='MIT',
   description = 'Conditionally Routed Attention',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/CoLT5-attention',
   keywords = [
```

