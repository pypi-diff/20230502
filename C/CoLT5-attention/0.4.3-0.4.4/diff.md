# Comparing `tmp/CoLT5-attention-0.4.3.tar.gz` & `tmp/CoLT5-attention-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CoLT5-attention-0.4.3.tar", last modified: Tue May  2 19:04:45 2023, max compression
+gzip compressed data, was "CoLT5-attention-0.4.4.tar", last modified: Tue May  2 21:52:46 2023, max compression
```

## Comparing `CoLT5-attention-0.4.3.tar` & `CoLT5-attention-0.4.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:04:45.087289 CoLT5-attention-0.4.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:04:45.087289 CoLT5-attention-0.4.3/CoLT5_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 19:04:45.000000 CoLT5-attention-0.4.3/CoLT5_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-02 19:04:45.000000 CoLT5-attention-0.4.3/CoLT5_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 19:04:45.000000 CoLT5-attention-0.4.3/CoLT5_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-02 19:04:45.000000 CoLT5-attention-0.4.3/CoLT5_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 19:04:45.000000 CoLT5-attention-0.4.3/CoLT5_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-02 19:04:34.000000 CoLT5-attention-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 19:04:45.087289 CoLT5-attention-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-05-02 19:04:34.000000 CoLT5-attention-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:04:45.087289 CoLT5-attention-0.4.3/colt5_attention/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-02 19:04:34.000000 CoLT5-attention-0.4.3/colt5_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-02 19:04:34.000000 CoLT5-attention-0.4.3/colt5_attention/coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-02 19:04:34.000000 CoLT5-attention-0.4.3/colt5_attention/sinkhorn.py
--rw-r--r--   0 runner    (1001) docker     (123)    32799 2023-05-02 19:04:34.000000 CoLT5-attention-0.4.3/colt5_attention/transformer_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-05-02 19:04:34.000000 CoLT5-attention-0.4.3/colt5_attention/triton_coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 19:04:45.087289 CoLT5-attention-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-02 19:04:34.000000 CoLT5-attention-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:46.649371 CoLT5-attention-0.4.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:46.645371 CoLT5-attention-0.4.4/CoLT5_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 21:52:46.000000 CoLT5-attention-0.4.4/CoLT5_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-02 21:52:46.000000 CoLT5-attention-0.4.4/CoLT5_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:52:46.000000 CoLT5-attention-0.4.4/CoLT5_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-02 21:52:46.000000 CoLT5-attention-0.4.4/CoLT5_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 21:52:46.000000 CoLT5-attention-0.4.4/CoLT5_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-02 21:52:25.000000 CoLT5-attention-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 21:52:46.649371 CoLT5-attention-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-05-02 21:52:25.000000 CoLT5-attention-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:52:46.649371 CoLT5-attention-0.4.4/colt5_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-02 21:52:25.000000 CoLT5-attention-0.4.4/colt5_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-02 21:52:25.000000 CoLT5-attention-0.4.4/colt5_attention/coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-02 21:52:25.000000 CoLT5-attention-0.4.4/colt5_attention/sinkhorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32799 2023-05-02 21:52:25.000000 CoLT5-attention-0.4.4/colt5_attention/transformer_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-02 21:52:25.000000 CoLT5-attention-0.4.4/colt5_attention/triton_coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 21:52:46.649371 CoLT5-attention-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-02 21:52:25.000000 CoLT5-attention-0.4.4/setup.py
```

### Comparing `CoLT5-attention-0.4.3/CoLT5_attention.egg-info/PKG-INFO` & `CoLT5-attention-0.4.4/CoLT5_attention.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.4.3
+Version: 0.4.4
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.4.3/LICENSE` & `CoLT5-attention-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.4.3/PKG-INFO` & `CoLT5-attention-0.4.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.4.3
+Version: 0.4.4
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.4.3/README.md` & `CoLT5-attention-0.4.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,15 @@
     - [x] forwards        
     - [x] backwards
     - [x] add some tests and benchmark for triton vs plain pytorch coor_descent - 10x faster for forward, 4x faster for backwards and memory saved is n_iters times
     - [x] fall back on plain coordinate descent for cpu
     - [x] handle edge case for when a row is completely masked out for triton, or simply enforce it never to be so
     - [ ] allow for saving intermediates every number of iterations - trading memory for recompute efficiency during backwards
     - [ ] maximum block size in triton allowed is 131k, make sure at least quarter of million sequence length can be reached
+    - [ ] issue with intermittent gradient errors is because of masking - load the key padding mask into triton and mask out during each iteration
 
 ## Citations
 
 ```bibtex
 @inproceedings{Ainslie2023CoLT5FL,
     title   = {CoLT5: Faster Long-Range Transformers with Conditional Computation},
     author  = {Joshua Ainslie and Tao Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and Yury Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and Yun-Hsuan Sung and Sumit Sanghai},
```

#### html2text {}

```diff
@@ -64,17 +64,19 @@
 - [x] add some tests and benchmark for triton vs plain pytorch coor_descent -
 10x faster for forward, 4x faster for backwards and memory saved is n_iters
 times - [x] fall back on plain coordinate descent for cpu - [x] handle edge
 case for when a row is completely masked out for triton, or simply enforce it
 never to be so - [ ] allow for saving intermediates every number of iterations
 - trading memory for recompute efficiency during backwards - [ ] maximum block
 size in triton allowed is 131k, make sure at least quarter of million sequence
-length can be reached ## Citations ```bibtex @inproceedings{Ainslie2023CoLT5FL,
-title = {CoLT5: Faster Long-Range Transformers with Conditional Computation},
-author = {Joshua Ainslie and Tao Lei and Michiel de Jong and Santiago Ontan'on
-and Siddhartha Brahma and Yury Zemlyanskiy and David Uthus and Mandy Guo and
-James Lee-Thorp and Yi Tay and Yun-Hsuan Sung and Sumit Sanghai}, year = {2023}
-} ``` ```bibtex @article{Tillet2019TritonAI, title = {Triton: an intermediate
+length can be reached - [ ] issue with intermittent gradient errors is because
+of masking - load the key padding mask into triton and mask out during each
+iteration ## Citations ```bibtex @inproceedings{Ainslie2023CoLT5FL, title =
+{CoLT5: Faster Long-Range Transformers with Conditional Computation}, author =
+{Joshua Ainslie and Tao Lei and Michiel de Jong and Santiago Ontan'on and
+Siddhartha Brahma and Yury Zemlyanskiy and David Uthus and Mandy Guo and James
+Lee-Thorp and Yi Tay and Yun-Hsuan Sung and Sumit Sanghai}, year = {2023} } ```
+```bibtex @article{Tillet2019TritonAI, title = {Triton: an intermediate
 language and compiler for tiled neural network computations}, author =
 {Philippe Tillet and H. Kung and D. Cox}, journal = {Proceedings of the 3rd ACM
 SIGPLAN International Workshop on Machine Learning and Programming Languages},
 year = {2019} } ```
```

### Comparing `CoLT5-attention-0.4.3/colt5_attention/coor_descent.py` & `CoLT5-attention-0.4.4/colt5_attention/coor_descent.py`

 * *Files 22% similar despite different names*

```diff
@@ -29,13 +29,21 @@
     if exists(mask):
         s = s.masked_fill(~mask, mask_value)
 
     a = 0
     b = -s
 
     for _ in range(n_iters):
+        sb = ((s + b) / eps)
 
-        a = constant - eps * ((s + b) / eps).logsumexp(dim = -1, keepdim = True)
+        if exists(mask):
+            sb = sb.masked_fill(~mask, mask_value)
+
+        a = constant - eps * sb.logsumexp(dim = -1, keepdim = True)
         b = -F.relu(s + a)
 
     scores = ((s + a + b) / eps).exp()
+
+    if exists(mask):
+        scores = scores.masked_fill(~mask, 0.)
+
     return scores
```

### Comparing `CoLT5-attention-0.4.3/colt5_attention/sinkhorn.py` & `CoLT5-attention-0.4.4/colt5_attention/sinkhorn.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.4.3/colt5_attention/transformer_block.py` & `CoLT5-attention-0.4.4/colt5_attention/transformer_block.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.4.3/colt5_attention/triton_coor_descent.py` & `CoLT5-attention-0.4.4/colt5_attention/triton_coor_descent.py`

 * *Files 16% similar despite different names*

```diff
@@ -41,32 +41,42 @@
 
 # forwards
 
 @triton.jit
 def coor_descent_kernel_forward(
     output_ptr,
     input_ptr,
+    mask_ptr,
     k_ptr,
     output_row_stride,
     input_row_stride,
+    mask_row_stride,
     k_row_stride,
     n_iters,
     eps,
     n_cols,
     BLOCK_SIZE: tl.constexpr
 ):
     row_idx = tl.program_id(0)
 
     row_start_ptr = input_ptr + row_idx * input_row_stride
     k_ptr = k_ptr + row_idx * k_row_stride
 
     col_offsets = tl.arange(0, BLOCK_SIZE)
     input_ptrs = row_start_ptr + col_offsets
 
-    mask = col_offsets < n_cols
+    col_mask = col_offsets < n_cols
+
+    # load mask as ints (for some reason as boolean breaks triton)
+
+    mask_start_ptr = mask_ptr + row_idx * mask_row_stride
+    mask_ptrs = mask_start_ptr + col_offsets
+
+    mask_ints = tl.load(mask_ptrs, mask = col_mask, other = 0)
+    mask = mask_ints == 1
 
     # load the scores s
 
     s = tl.load(input_ptrs, mask = mask, other = -float('inf'))
 
     # load k - controls the sparsity of output
 
@@ -76,19 +86,20 @@
 
     inv_eps = 1. / eps
 
     # initialize a and b for coordinate descent
 
     a = k * 0 # init a to 0, triton needs to know shape and type outside loop
 
-    b = tl.where(mask, -s, -float('inf'))
+    b = -s
 
     for _ in range(n_iters):        
 
         a = (s + b) * inv_eps
+        a = tl.where(mask, a, -float('inf'))
 
         # stable log sum exp
 
         a_max = tl.max(a, axis = 0)
         a_minus_max = a - a_max
         exp = tl.exp(a_minus_max)
         sum_exp = tl.sum(exp, axis = 0)
@@ -102,36 +113,50 @@
         b = tl.where(b >= 0., -b, 0.)
 
     s = tl.exp((s + a + b) * inv_eps)
 
     output_row_start_ptr = output_ptr + row_idx * output_row_stride
     output_ptrs = output_row_start_ptr + col_offsets
 
-    tl.store(output_ptrs, s, mask = mask)
+    s = tl.where(mask, s, 0.)
+    tl.store(output_ptrs, s)
 
 # backwards
 
 @triton.jit
 def coor_descent_kernel_backward(
     output_ptr,
     input_ptr,
+    mask_ptr,
     grad_ptr,
     k_ptr,
     output_row_stride,
     input_row_stride,
+    mask_row_stride,
     grad_row_stride,
     k_row_stride,
     n_iters,
     eps,
     n_cols,
     BLOCK_SIZE: tl.constexpr
 ):
     row_idx = tl.program_id(0)
     col_offsets = tl.arange(0, BLOCK_SIZE)
-    mask = col_offsets < n_cols
+
+    # load and generate mask
+
+    col_mask = col_offsets < n_cols
+
+    # load mask as ints (for some reason as boolean breaks triton)
+
+    mask_start_ptr = mask_ptr + row_idx * mask_row_stride
+    mask_ptrs = mask_start_ptr + col_offsets
+
+    mask_ints = tl.load(mask_ptrs, mask = col_mask, other = 0)
+    mask = mask_ints == 1
 
     # load input
 
     row_start_ptr = input_ptr + row_idx * input_row_stride
     input_ptrs = row_start_ptr + col_offsets
 
     s = tl.load(input_ptrs, mask = mask, other = -float('inf'))
@@ -149,15 +174,15 @@
     grad_ptrs = grad_row_start_ptr + col_offsets
 
     grad_row = tl.load(grad_ptrs, mask = mask, other = 0.)
 
     # recompute
 
     init_a = k * 0
-    init_b = tl.where(mask, -s, -float('inf'))
+    init_b = -s
 
     ds = s * 0
     db = s * 0
     last_da = k * 0
 
     inv_eps = 1. / eps
 
@@ -166,71 +191,77 @@
     for ind in range(n_iters):
         is_first = ind == 0
 
         a = init_a
         b = init_b
 
         sa = s * 0
-        exp = s * 0
-        sum_exp = k * 0
+        softmax = s * 0
 
         for _ in range(n_iters - ind):
 
             sb = (s + b) * inv_eps
+            sb = tl.where(mask, sb, -float('inf'))
 
             # stable log sum exp
 
             sb_max = tl.max(sb, axis = 0)
             sb_minus_max = sb - sb_max
             exp = tl.exp(sb_minus_max)
             sum_exp = tl.sum(exp, axis = 0)
+            softmax = exp / sum_exp
             log_sum_exp = tl.log(sum_exp) + sb_max
 
             a = constant - eps * log_sum_exp
 
             # update b
 
             sa = s + a
             b = tl.where(sa >= 0., -sa, 0.)
 
         if is_first:
             o = tl.exp((s + a + b) * inv_eps)
 
+            o = tl.where(mask, o, 0.)
+
             ds = grad_row * o
             ds *= inv_eps
 
+            ds = tl.where(mask, ds, 0.)
+
             last_da = tl.sum(ds, axis = 0)
             db = ds
 
         # go backwards
 
         if n_iters > 0:
 
             dsa = db * tl.where(sa >= 0, -1., 0.)
             ds += dsa
 
             da = tl.sum(dsa, axis = 0) + last_da
             da *= -eps
 
-            dsb = exp * da / sum_exp
+            dsb = da * softmax
             dsb *= inv_eps
 
             ds += dsb
             db = dsb
 
             last_da = 0.
 
     ds += -db
 
     # store output
 
     output_row_start_ptr = output_ptr + row_idx * output_row_stride
     output_ptrs = output_row_start_ptr + col_offsets
 
-    tl.store(output_ptrs, ds, mask = mask)
+    ds = tl.where(mask, ds, 0.)
+    tl.store(output_ptrs, ds)
 
 # function forwards and backwards
 
 class _coor_descent(autograd.Function):
     @classmethod
     def forward(
         self,
@@ -241,19 +272,22 @@
         eps,
         mask
     ):
         assert x.is_cuda, 'triton coordinate descent must be on cuda'
 
         batch, requires_grad = x.shape[0], x.requires_grad
 
-        if exists(mask):
-            mask_value = -torch.finfo(x.dtype).max
-            x = x.masked_fill(~mask, mask_value)
+        if not exists(mask):
+            mask = torch.ones_like(x, dtype = torch.bool, device = x.device)
 
         x, shape = pack_one(x, '* n')
+        mask, _ = pack_one(mask, '* n')
+
+        x = x.masked_fill(~mask, -torch.finfo(x.dtype).max)
+        mask_ints = mask.int()
 
         n_rows, n_cols = x.shape
 
         if isinstance(k, (int, float)):
             k = torch.full((n_rows,), k)
         elif k.ndim == 1:
             k = repeat(k, 'n -> (b n)', b = x.shape[0] // k.shape[0])
@@ -264,28 +298,30 @@
         num_warps = calc_num_warps(BLOCK_SIZE)
 
         y = torch.empty_like(x)
 
         coor_descent_kernel_forward[(n_rows,)](
             y,
             x,
+            mask_ints,
             k,
             y.stride(0),
             x.stride(0),
+            mask_ints.stride(0),
             k.stride(0),
             n_iters,
             eps,
             n_cols,
             num_warps = num_warps,
             BLOCK_SIZE = BLOCK_SIZE,
         )
 
         if requires_grad:
             ctx.args = (n_iters, eps)
-            ctx.save_for_backward(x, k)
+            ctx.save_for_backward(x, k, mask)
 
         y = unpack_one(y, shape, '* n')
 
         return y
 
     @classmethod
     def backward(
@@ -294,31 +330,38 @@
         grad_probs
     ):
         assert grad_probs.is_cuda
 
         batch = grad_probs.shape[0]
 
         n_iters, eps = ctx.args
-        x, k = ctx.saved_tensors
+        x, k, mask = ctx.saved_tensors
+
+        if exists(mask):
+            grad_probs = grad_probs.masked_fill(~mask, 0.)
 
         grad_probs, shape = pack_one(grad_probs, '* n')
         n_rows, n_cols = grad_probs.shape
 
         BLOCK_SIZE = triton.next_power_of_2(n_cols)
         num_warps = calc_num_warps(BLOCK_SIZE)
 
         dx = torch.empty_like(grad_probs)
 
+        mask_int = mask.int()
+
         coor_descent_kernel_backward[(n_rows,)](
             dx,
             x,
+            mask_int,
             grad_probs,
             k,
             dx.stride(0),
             x.stride(0),
+            mask_int.stride(0),
             grad_probs.stride(0),
             k.stride(0),
             n_iters,
             eps,
             n_cols,
             num_warps = num_warps,
             BLOCK_SIZE = BLOCK_SIZE
```

### Comparing `CoLT5-attention-0.4.3/setup.py` & `CoLT5-attention-0.4.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'CoLT5-attention',
   packages = find_packages(),
-  version = '0.4.3',
+  version = '0.4.4',
   license='MIT',
   description = 'Conditionally Routed Attention',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/CoLT5-attention',
   keywords = [
```

