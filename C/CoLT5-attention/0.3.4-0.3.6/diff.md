# Comparing `tmp/CoLT5-attention-0.3.4.tar.gz` & `tmp/CoLT5-attention-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CoLT5-attention-0.3.4.tar", last modified: Fri Apr 28 23:39:15 2023, max compression
+gzip compressed data, was "CoLT5-attention-0.3.6.tar", last modified: Mon May  1 16:52:34 2023, max compression
```

## Comparing `CoLT5-attention-0.3.4.tar` & `CoLT5-attention-0.3.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:39:15.825781 CoLT5-attention-0.3.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:39:15.825781 CoLT5-attention-0.3.4/CoLT5_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-28 23:39:15.000000 CoLT5-attention-0.3.4/CoLT5_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-28 23:39:15.000000 CoLT5-attention-0.3.4/CoLT5_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 23:39:15.000000 CoLT5-attention-0.3.4/CoLT5_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-28 23:39:15.000000 CoLT5-attention-0.3.4/CoLT5_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 23:39:15.000000 CoLT5-attention-0.3.4/CoLT5_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-28 23:39:04.000000 CoLT5-attention-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-28 23:39:15.825781 CoLT5-attention-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-04-28 23:39:04.000000 CoLT5-attention-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:39:15.825781 CoLT5-attention-0.3.4/colt5_attention/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-28 23:39:04.000000 CoLT5-attention-0.3.4/colt5_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-28 23:39:04.000000 CoLT5-attention-0.3.4/colt5_attention/coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-28 23:39:04.000000 CoLT5-attention-0.3.4/colt5_attention/sinkhorn.py
--rw-r--r--   0 runner    (1001) docker     (123)    31461 2023-04-28 23:39:04.000000 CoLT5-attention-0.3.4/colt5_attention/transformer_block.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 23:39:15.825781 CoLT5-attention-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-28 23:39:04.000000 CoLT5-attention-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:52:34.509534 CoLT5-attention-0.3.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:52:34.505534 CoLT5-attention-0.3.6/CoLT5_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-01 16:52:34.000000 CoLT5-attention-0.3.6/CoLT5_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-01 16:52:34.000000 CoLT5-attention-0.3.6/CoLT5_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 16:52:34.000000 CoLT5-attention-0.3.6/CoLT5_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-01 16:52:34.000000 CoLT5-attention-0.3.6/CoLT5_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-01 16:52:34.000000 CoLT5-attention-0.3.6/CoLT5_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-01 16:52:17.000000 CoLT5-attention-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-01 16:52:34.509534 CoLT5-attention-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-05-01 16:52:17.000000 CoLT5-attention-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:52:34.509534 CoLT5-attention-0.3.6/colt5_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-01 16:52:17.000000 CoLT5-attention-0.3.6/colt5_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-01 16:52:17.000000 CoLT5-attention-0.3.6/colt5_attention/coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-01 16:52:17.000000 CoLT5-attention-0.3.6/colt5_attention/sinkhorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31461 2023-05-01 16:52:17.000000 CoLT5-attention-0.3.6/colt5_attention/transformer_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 16:52:34.509534 CoLT5-attention-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-01 16:52:17.000000 CoLT5-attention-0.3.6/setup.py
```

### Comparing `CoLT5-attention-0.3.4/CoLT5_attention.egg-info/PKG-INFO` & `CoLT5-attention-0.3.6/CoLT5_attention.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.3.4
+Version: 0.3.6
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.3.4/LICENSE` & `CoLT5-attention-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.3.4/PKG-INFO` & `CoLT5-attention-0.3.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.3.4
+Version: 0.3.6
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.3.4/README.md` & `CoLT5-attention-0.3.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -126,18 +126,29 @@
 - [x] add an autoregressive version of the conditionally routed attention
 
 - [ ] test out the autoregressive version and verify that more routed key / value tokens lead to better results
 - [ ] for variable sequence lengths, allow for setting k as a function of sequence lengths per sample in batch
 - [ ] create a variant of CoLT5 for high resolution feature maps (image attention) - then try out for diffusion
 - [ ] in the cross attention scenario, support for routing token that first queries the source tokens, before retrieving from memories
 - [ ] make flash attention compatible
-- [ ] work out a triton forward / backward version of coordinate descent (coor_descent), as it seems torch compile does not work well enough for coor_descent function just yet
+- [ ] fused coordinate descent kernel using triton
+    - [ ] forwards
+    - [ ] backwards
 
 ## Citations
 
 ```bibtex
 @inproceedings{Ainslie2023CoLT5FL,
     title   = {CoLT5: Faster Long-Range Transformers with Conditional Computation},
     author  = {Joshua Ainslie and Tao Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and Yury Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and Yun-Hsuan Sung and Sumit Sanghai},
     year    = {2023}
 }
 ```
+
+```bibtex
+@article{Tillet2019TritonAI,
+    title   = {Triton: an intermediate language and compiler for tiled neural network computations},
+    author  = {Philippe Tillet and H. Kung and D. Cox},
+    journal = {Proceedings of the 3rd ACM SIGPLAN International Workshop on Machine Learning and Programming Languages},
+    year    = {2019}
+}
+```
```

#### html2text {}

```diff
@@ -53,15 +53,18 @@
 values - [x] add an autoregressive version of the conditionally routed
 attention - [ ] test out the autoregressive version and verify that more routed
 key / value tokens lead to better results - [ ] for variable sequence lengths,
 allow for setting k as a function of sequence lengths per sample in batch - [ ]
 create a variant of CoLT5 for high resolution feature maps (image attention) -
 then try out for diffusion - [ ] in the cross attention scenario, support for
 routing token that first queries the source tokens, before retrieving from
-memories - [ ] make flash attention compatible - [ ] work out a triton forward
-/ backward version of coordinate descent (coor_descent), as it seems torch
-compile does not work well enough for coor_descent function just yet ##
-Citations ```bibtex @inproceedings{Ainslie2023CoLT5FL, title = {CoLT5: Faster
-Long-Range Transformers with Conditional Computation}, author = {Joshua Ainslie
-and Tao Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and
-Yury Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay
-and Yun-Hsuan Sung and Sumit Sanghai}, year = {2023} } ```
+memories - [ ] make flash attention compatible - [ ] fused coordinate descent
+kernel using triton - [ ] forwards - [ ] backwards ## Citations ```bibtex
+@inproceedings{Ainslie2023CoLT5FL, title = {CoLT5: Faster Long-Range
+Transformers with Conditional Computation}, author = {Joshua Ainslie and Tao
+Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and Yury
+Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and
+Yun-Hsuan Sung and Sumit Sanghai}, year = {2023} } ``` ```bibtex @article
+{Tillet2019TritonAI, title = {Triton: an intermediate language and compiler for
+tiled neural network computations}, author = {Philippe Tillet and H. Kung and
+D. Cox}, journal = {Proceedings of the 3rd ACM SIGPLAN International Workshop
+on Machine Learning and Programming Languages}, year = {2019} } ```
```

### Comparing `CoLT5-attention-0.3.4/colt5_attention/coor_descent.py` & `CoLT5-attention-0.3.6/colt5_attention/coor_descent.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,27 +9,30 @@
 
 def coor_descent(
     s,
     *,
     n_iters,
     k,
     eps = 1e-1,
-    clamp_fn = F.relu,
-    mask = None,
+    mask = None
 ):
     mask_value = -torch.finfo(s.dtype).max
+
+    if not isinstance(k, torch.Tensor):
+        k = torch.Tensor([k]).to(s)
+
     constant = eps * log(k)
 
-    b = -clamp_fn(s)
+    b = -F.relu(s)
 
     for _ in range(n_iters):
         if exists(mask):
             s = s.masked_fill(~mask, mask_value)
 
         a = constant - eps * ((s + b) / eps).logsumexp(dim = -1, keepdim = True)
-        b = -clamp_fn(s + a)
+        b = -F.relu(s + a)
 
     if exists(mask):
         s = s.masked_fill(~mask, mask_value)
 
     scores = ((s + a + b) / eps).exp()
-    return scores
+    return scores
```

### Comparing `CoLT5-attention-0.3.4/colt5_attention/sinkhorn.py` & `CoLT5-attention-0.3.6/colt5_attention/sinkhorn.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.3.4/colt5_attention/transformer_block.py` & `CoLT5-attention-0.3.6/colt5_attention/transformer_block.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.3.4/setup.py` & `CoLT5-attention-0.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'CoLT5-attention',
   packages = find_packages(),
-  version = '0.3.4',
+  version = '0.3.6',
   license='MIT',
   description = 'Conditionally Routed Attention',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/CoLT5-attention',
   keywords = [
```

