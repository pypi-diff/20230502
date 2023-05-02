# Comparing `tmp/CoLT5-attention-0.4.2.tar.gz` & `tmp/CoLT5-attention-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CoLT5-attention-0.4.2.tar", last modified: Tue May  2 17:50:22 2023, max compression
+gzip compressed data, was "CoLT5-attention-0.4.3.tar", last modified: Tue May  2 19:04:45 2023, max compression
```

## Comparing `CoLT5-attention-0.4.2.tar` & `CoLT5-attention-0.4.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:50:22.060546 CoLT5-attention-0.4.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:50:22.056546 CoLT5-attention-0.4.2/CoLT5_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 17:50:22.000000 CoLT5-attention-0.4.2/CoLT5_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-02 17:50:22.000000 CoLT5-attention-0.4.2/CoLT5_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 17:50:22.000000 CoLT5-attention-0.4.2/CoLT5_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-02 17:50:22.000000 CoLT5-attention-0.4.2/CoLT5_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 17:50:22.000000 CoLT5-attention-0.4.2/CoLT5_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-02 17:50:10.000000 CoLT5-attention-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 17:50:22.060546 CoLT5-attention-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-02 17:50:10.000000 CoLT5-attention-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:50:22.060546 CoLT5-attention-0.4.2/colt5_attention/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-02 17:50:10.000000 CoLT5-attention-0.4.2/colt5_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-02 17:50:10.000000 CoLT5-attention-0.4.2/colt5_attention/coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-02 17:50:10.000000 CoLT5-attention-0.4.2/colt5_attention/sinkhorn.py
--rw-r--r--   0 runner    (1001) docker     (123)    32695 2023-05-02 17:50:10.000000 CoLT5-attention-0.4.2/colt5_attention/transformer_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-05-02 17:50:10.000000 CoLT5-attention-0.4.2/colt5_attention/triton_coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 17:50:22.060546 CoLT5-attention-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-02 17:50:10.000000 CoLT5-attention-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:04:45.087289 CoLT5-attention-0.4.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:04:45.087289 CoLT5-attention-0.4.3/CoLT5_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 19:04:45.000000 CoLT5-attention-0.4.3/CoLT5_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-02 19:04:45.000000 CoLT5-attention-0.4.3/CoLT5_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 19:04:45.000000 CoLT5-attention-0.4.3/CoLT5_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-02 19:04:45.000000 CoLT5-attention-0.4.3/CoLT5_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 19:04:45.000000 CoLT5-attention-0.4.3/CoLT5_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-02 19:04:34.000000 CoLT5-attention-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 19:04:45.087289 CoLT5-attention-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-05-02 19:04:34.000000 CoLT5-attention-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:04:45.087289 CoLT5-attention-0.4.3/colt5_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-02 19:04:34.000000 CoLT5-attention-0.4.3/colt5_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-02 19:04:34.000000 CoLT5-attention-0.4.3/colt5_attention/coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-02 19:04:34.000000 CoLT5-attention-0.4.3/colt5_attention/sinkhorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32799 2023-05-02 19:04:34.000000 CoLT5-attention-0.4.3/colt5_attention/transformer_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-05-02 19:04:34.000000 CoLT5-attention-0.4.3/colt5_attention/triton_coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 19:04:45.087289 CoLT5-attention-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-02 19:04:34.000000 CoLT5-attention-0.4.3/setup.py
```

### Comparing `CoLT5-attention-0.4.2/CoLT5_attention.egg-info/PKG-INFO` & `CoLT5-attention-0.4.3/CoLT5_attention.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.4.2
+Version: 0.4.3
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.4.2/LICENSE` & `CoLT5-attention-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.4.2/PKG-INFO` & `CoLT5-attention-0.4.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.4.2
+Version: 0.4.3
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.4.2/README.md` & `CoLT5-attention-0.4.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 ## Appreciation
 
 - <a href="https://stability.ai/">Stability.ai</a> for the generous sponsorship to work on cutting edge artificial intelligence research
 
 - <a href="https://github.com/arogozhnikov/einops">einops</a> for making my life easy
 
+- <a href="https://github.com/openai/triton">Triton</a> for allowing me to speed up coordinate descent with a fused implementation in just 2 days, sparing me from having to write a thousand lines of CUDA code
+
 ## Install
 
 ```bash
 $ pip install colt5-attention
 ```
 
 ## Usage
@@ -131,17 +133,17 @@
 - [ ] in the cross attention scenario, support for routing token that first queries the source tokens, before retrieving from memories
 - [ ] make flash attention compatible
 - [ ] fused coordinate descent kernel using triton
     - [x] forwards        
     - [x] backwards
     - [x] add some tests and benchmark for triton vs plain pytorch coor_descent - 10x faster for forward, 4x faster for backwards and memory saved is n_iters times
     - [x] fall back on plain coordinate descent for cpu
+    - [x] handle edge case for when a row is completely masked out for triton, or simply enforce it never to be so
     - [ ] allow for saving intermediates every number of iterations - trading memory for recompute efficiency during backwards
     - [ ] maximum block size in triton allowed is 131k, make sure at least quarter of million sequence length can be reached
-    - [ ] handle edge case for when a row is completely masked out for triton, or simply enforce it never to be so
 
 ## Citations
 
 ```bibtex
 @inproceedings{Ainslie2023CoLT5FL,
     title   = {CoLT5: Faster Long-Range Transformers with Conditional Computation},
     author  = {Joshua Ainslie and Tao Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and Yury Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and Yun-Hsuan Sung and Sumit Sanghai},
```

#### html2text {}

```diff
@@ -3,16 +3,18 @@
 Besides their use of coordinate descent from this_paper (main algorithm
 originally from Wright_et_al), will also add two other approaches, one based on
 cumulative softmax, the other gumbel sinkhorn (optimal transport). Update:
 unsure of how the routing normalized scores for the key-values are used. Did
 some improvising there, scaling_the_projected_values, but if you think you know
 the answer, please open an issue ## Appreciation - Stability.ai for the
 generous sponsorship to work on cutting edge artificial intelligence research -
-einops for making my life easy ## Install ```bash $ pip install colt5-attention
-``` ## Usage ```python import torch from colt5_attention import
+einops for making my life easy - Triton for allowing me to speed up coordinate
+descent with a fused implementation in just 2 days, sparing me from having to
+write a thousand lines of CUDA code ## Install ```bash $ pip install colt5-
+attention ``` ## Usage ```python import torch from colt5_attention import
 ( ConditionalRoutedFeedForward, ConditionalRoutedAttention,
 ConditionalRoutedTransformerBlock ) # mock input, say it is 32768 length tokens
 = torch.randn(2, 32768, 512) mask = torch.ones(2, 32768).bool() # can handle
 variable lengthed sequences # feedforward ff = ConditionalRoutedFeedForward
 ( dim = 512, light_ff_mult = 0.5, # hidden dimension ratio of light branch
 heavy_ff_mult = 4, # hidden dimension ratio of heavy branch num_heavy_tokens =
 1024 # heavy branch receives only 1024 routed tokens of 32768 ) ff_out = ff
@@ -57,22 +59,22 @@
 sample in batch - [ ] create a variant of CoLT5 for high resolution feature
 maps (image attention) - then try out for diffusion - [ ] in the cross
 attention scenario, support for routing token that first queries the source
 tokens, before retrieving from memories - [ ] make flash attention compatible -
 [ ] fused coordinate descent kernel using triton - [x] forwards - [x] backwards
 - [x] add some tests and benchmark for triton vs plain pytorch coor_descent -
 10x faster for forward, 4x faster for backwards and memory saved is n_iters
-times - [x] fall back on plain coordinate descent for cpu - [ ] allow for
-saving intermediates every number of iterations - trading memory for recompute
-efficiency during backwards - [ ] maximum block size in triton allowed is 131k,
-make sure at least quarter of million sequence length can be reached - [ ]
-handle edge case for when a row is completely masked out for triton, or simply
-enforce it never to be so ## Citations ```bibtex @inproceedings
-{Ainslie2023CoLT5FL, title = {CoLT5: Faster Long-Range Transformers with
-Conditional Computation}, author = {Joshua Ainslie and Tao Lei and Michiel de
-Jong and Santiago Ontan'on and Siddhartha Brahma and Yury Zemlyanskiy and David
-Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and Yun-Hsuan Sung and Sumit
-Sanghai}, year = {2023} } ``` ```bibtex @article{Tillet2019TritonAI, title =
-{Triton: an intermediate language and compiler for tiled neural network
-computations}, author = {Philippe Tillet and H. Kung and D. Cox}, journal =
-{Proceedings of the 3rd ACM SIGPLAN International Workshop on Machine Learning
-and Programming Languages}, year = {2019} } ```
+times - [x] fall back on plain coordinate descent for cpu - [x] handle edge
+case for when a row is completely masked out for triton, or simply enforce it
+never to be so - [ ] allow for saving intermediates every number of iterations
+- trading memory for recompute efficiency during backwards - [ ] maximum block
+size in triton allowed is 131k, make sure at least quarter of million sequence
+length can be reached ## Citations ```bibtex @inproceedings{Ainslie2023CoLT5FL,
+title = {CoLT5: Faster Long-Range Transformers with Conditional Computation},
+author = {Joshua Ainslie and Tao Lei and Michiel de Jong and Santiago Ontan'on
+and Siddhartha Brahma and Yury Zemlyanskiy and David Uthus and Mandy Guo and
+James Lee-Thorp and Yi Tay and Yun-Hsuan Sung and Sumit Sanghai}, year = {2023}
+} ``` ```bibtex @article{Tillet2019TritonAI, title = {Triton: an intermediate
+language and compiler for tiled neural network computations}, author =
+{Philippe Tillet and H. Kung and D. Cox}, journal = {Proceedings of the 3rd ACM
+SIGPLAN International Workshop on Machine Learning and Programming Languages},
+year = {2019} } ```
```

### Comparing `CoLT5-attention-0.4.2/colt5_attention/coor_descent.py` & `CoLT5-attention-0.4.3/colt5_attention/coor_descent.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.4.2/colt5_attention/sinkhorn.py` & `CoLT5-attention-0.4.3/colt5_attention/sinkhorn.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.4.2/colt5_attention/transformer_block.py` & `CoLT5-attention-0.4.3/colt5_attention/transformer_block.py`

 * *Files 1% similar despite different names*

```diff
@@ -750,38 +750,44 @@
         light_out = self.light_attn(x)
 
         # pad sequence to multiple of the heavy window size
         # routing will take place within each heavy window block size
 
         window_size = self.heavy_window_size
 
-        x = x[:, window_size:] # the first window has nothing to attend to, just crop out to save some simplicity with nothing being route-able
-
         x, seq_len = pad_to_multiple(x, window_size, dim = -2)
 
         padded_seq_len = x.shape[-2]
 
         # construct mask, and make sure not to attend to padding
 
         q_mask = torch.ones((batch, seq_len), dtype = torch.bool, device = device)
         q_mask = F.pad(q_mask, (0, padded_seq_len - seq_len), value = False)
 
+        # handy function
+
+        merge_to_batch = lambda t: rearrange(t, 'b n ... -> (b n) ...')
+
         # block the sequence and mask into windows for the queries
 
-        q = rearrange(x, 'b (n w) d -> (b n) w d', w = window_size)
-        q_mask = rearrange(q_mask, 'b (n w) -> (b n) w', w = window_size)
+        q = rearrange(x, 'b (n w) d -> b n w d', w = window_size)
+        q_mask = rearrange(q_mask, 'b (n w) -> b n w', w = window_size)
+
+        q, q_mask = map(merge_to_batch, (q[:, 1:], q_mask[:, 1:]))
 
         # each block of queries attend to sequences that are causally masked out appropriately
 
         windows = padded_seq_len // window_size
 
-        kv = repeat(x, 'b n d -> (b m) n d', m = windows)
+        kv = repeat(x, 'b n d -> b m n d', m = windows)
+
+        kv_mask = torch.ones((windows, windows), dtype = torch.bool, device = device).tril(-1)
+        kv_mask = repeat(kv_mask, 'm n -> b m (n w)', b = batch, w = window_size)
 
-        kv_mask = torch.ones((windows, windows), dtype = torch.bool, device = device).tril()
-        kv_mask = repeat(kv_mask, 'm n -> (b m) (n w)', b = batch, w = window_size)
+        kv, kv_mask = map(merge_to_batch, (kv[:, 1:], kv_mask[:, 1:]))
 
         # route tokens appropriately for heavy branch, if need be
 
         should_route_q = q.shape[-2] > num_heavy_tokens_q
         should_route_kv = kv.shape[-2] > num_heavy_tokens_kv
 
         if should_route_q:
@@ -821,15 +827,15 @@
             heavy_out = self.q_router.route_back(heavy_out, routed_tokens_out, indices_q)
         else:
             heavy_out = routed_tokens_out
 
         # un-window and slice out original sequence
 
         heavy_out = rearrange(heavy_out, '(b n) w d -> b (n w) d', b = batch)
-        heavy_out = heavy_out[:, :seq_len]
+        heavy_out = heavy_out[:, :(seq_len - window_size)]
 
         heavy_out = F.pad(heavy_out, (0, 0, window_size, 0), value = 0.)
 
         # sum light and heavy branches
 
         return light_out + heavy_out
```

### Comparing `CoLT5-attention-0.4.2/colt5_attention/triton_coor_descent.py` & `CoLT5-attention-0.4.3/colt5_attention/triton_coor_descent.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.4.2/setup.py` & `CoLT5-attention-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'CoLT5-attention',
   packages = find_packages(),
-  version = '0.4.2',
+  version = '0.4.3',
   license='MIT',
   description = 'Conditionally Routed Attention',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/CoLT5-attention',
   keywords = [
```

