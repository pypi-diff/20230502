# Comparing `tmp/tiny_ai_helper-0.1.6.tar.gz` & `tmp/tiny_ai_helper-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiny_ai_helper-0.1.6.tar", last modified: Tue Apr 18 08:30:33 2023, max compression
+gzip compressed data, was "tiny_ai_helper-0.1.7.tar", last modified: Tue May  2 09:09:50 2023, max compression
```

## Comparing `tiny_ai_helper-0.1.6.tar` & `tiny_ai_helper-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-04-18 08:30:33.916846 tiny_ai_helper-0.1.6/
--rw-rw-r--   0 www-data  (1000) www-data  (1000)     1103 2023-03-09 17:46:27.000000 tiny_ai_helper-0.1.6/LICENSE
--rw-rw-r--   0 www-data  (1000) www-data  (1000)      784 2023-04-18 08:30:33.916846 tiny_ai_helper-0.1.6/PKG-INFO
--rw-rw-r--   0 www-data  (1000) www-data  (1000)       74 2022-09-27 15:48:25.000000 tiny_ai_helper-0.1.6/README.md
--rw-rw-r--   0 www-data  (1000) www-data  (1000)       38 2023-04-18 08:30:33.916846 tiny_ai_helper-0.1.6/setup.cfg
--rw-rw-r--   0 www-data  (1000) www-data  (1000)     1029 2023-04-18 08:29:21.000000 tiny_ai_helper-0.1.6/setup.py
-drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-04-18 08:30:33.916846 tiny_ai_helper-0.1.6/tiny_ai_helper/
--rw-rw-r--   0 www-data  (1000) www-data  (1000)    14092 2023-04-08 13:19:55.000000 tiny_ai_helper-0.1.6/tiny_ai_helper/Model.py
--rw-rw-r--   0 www-data  (1000) www-data  (1000)    10280 2023-04-08 09:58:47.000000 tiny_ai_helper-0.1.6/tiny_ai_helper/Trainer.py
--rw-rw-r--   0 www-data  (1000) www-data  (1000)      367 2023-04-18 08:29:27.000000 tiny_ai_helper-0.1.6/tiny_ai_helper/__init__.py
--rw-rw-r--   0 www-data  (1000) www-data  (1000)     6232 2023-03-23 11:28:02.000000 tiny_ai_helper-0.1.6/tiny_ai_helper/layers.py
--rw-rw-r--   0 www-data  (1000) www-data  (1000)     9071 2023-03-15 18:42:46.000000 tiny_ai_helper-0.1.6/tiny_ai_helper/mp.py
--rw-rw-r--   0 www-data  (1000) www-data  (1000)    14216 2023-04-17 11:26:04.000000 tiny_ai_helper-0.1.6/tiny_ai_helper/utils.py
-drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-04-18 08:30:33.916846 tiny_ai_helper-0.1.6/tiny_ai_helper.egg-info/
--rw-rw-r--   0 www-data  (1000) www-data  (1000)      784 2023-04-18 08:30:31.000000 tiny_ai_helper-0.1.6/tiny_ai_helper.egg-info/PKG-INFO
--rw-rw-r--   0 www-data  (1000) www-data  (1000)      325 2023-04-18 08:30:31.000000 tiny_ai_helper-0.1.6/tiny_ai_helper.egg-info/SOURCES.txt
--rw-rw-r--   0 www-data  (1000) www-data  (1000)        1 2023-04-18 08:30:31.000000 tiny_ai_helper-0.1.6/tiny_ai_helper.egg-info/dependency_links.txt
--rw-rw-r--   0 www-data  (1000) www-data  (1000)       15 2023-04-18 08:30:31.000000 tiny_ai_helper-0.1.6/tiny_ai_helper.egg-info/top_level.txt
+drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-05-02 09:09:50.948392 tiny_ai_helper-0.1.7/
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)     1103 2023-03-09 17:46:27.000000 tiny_ai_helper-0.1.7/LICENSE
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)      784 2023-05-02 09:09:50.948392 tiny_ai_helper-0.1.7/PKG-INFO
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)       74 2022-09-27 15:48:25.000000 tiny_ai_helper-0.1.7/README.md
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)       38 2023-05-02 09:09:50.948392 tiny_ai_helper-0.1.7/setup.cfg
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)     1029 2023-05-02 08:38:57.000000 tiny_ai_helper-0.1.7/setup.py
+drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-05-02 09:09:50.944392 tiny_ai_helper-0.1.7/tiny_ai_helper/
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)    14107 2023-05-01 18:50:11.000000 tiny_ai_helper-0.1.7/tiny_ai_helper/Model.py
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)    10452 2023-04-30 10:47:53.000000 tiny_ai_helper-0.1.7/tiny_ai_helper/Trainer.py
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)      367 2023-05-02 08:39:07.000000 tiny_ai_helper-0.1.7/tiny_ai_helper/__init__.py
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)     6232 2023-03-23 11:28:02.000000 tiny_ai_helper-0.1.7/tiny_ai_helper/layers.py
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)     9071 2023-03-15 18:42:46.000000 tiny_ai_helper-0.1.7/tiny_ai_helper/mp.py
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)    19836 2023-05-02 09:06:06.000000 tiny_ai_helper-0.1.7/tiny_ai_helper/utils.py
+drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-05-02 09:09:50.948392 tiny_ai_helper-0.1.7/tiny_ai_helper.egg-info/
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)      784 2023-05-02 09:09:50.000000 tiny_ai_helper-0.1.7/tiny_ai_helper.egg-info/PKG-INFO
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)      325 2023-05-02 09:09:50.000000 tiny_ai_helper-0.1.7/tiny_ai_helper.egg-info/SOURCES.txt
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)        1 2023-05-02 09:09:50.000000 tiny_ai_helper-0.1.7/tiny_ai_helper.egg-info/dependency_links.txt
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)       15 2023-05-02 09:09:50.000000 tiny_ai_helper-0.1.7/tiny_ai_helper.egg-info/top_level.txt
```

### Comparing `tiny_ai_helper-0.1.6/LICENSE` & `tiny_ai_helper-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tiny_ai_helper-0.1.6/PKG-INFO` & `tiny_ai_helper-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiny_ai_helper
-Version: 0.1.6
+Version: 0.1.7
 Summary: Tiny AI Helper for PyTorch
 Home-page: https://github.com/bayrell/ai_helper
 Author: Ildar Bikmamatov
 Author-email: support@bayrell.org
 License: MIT License
 Keywords: ai helper,pytorch
 Platform: UNKNOWN
```

### Comparing `tiny_ai_helper-0.1.6/setup.py` & `tiny_ai_helper-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 from setuptools import setup, find_packages
 from os.path import abspath, dirname, join
 
 setup(
 	name="tiny_ai_helper",
-	version="0.1.6",
+	version="0.1.7",
 	description="Tiny AI Helper for PyTorch",
 	long_description=open(join(abspath(dirname(__file__)), 'README.md'), encoding='utf-8').read(),
 	long_description_content_type='text/markdown',
 	author="Ildar Bikmamatov",
 	author_email="support@bayrell.org",
 	license="MIT License",
 	url = "https://github.com/bayrell/ai_helper",
```

### Comparing `tiny_ai_helper-0.1.6/tiny_ai_helper/Model.py` & `tiny_ai_helper-0.1.7/tiny_ai_helper/Model.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 from torch.utils.data import DataLoader, TensorDataset
 from .utils import TransformDataset, list_files, \
     get_default_device, batch_to, tensor_size, load_json, summary
 
 
 class Model:
     
-    def __init__(self, name=None):
+    def __init__(self, module=None, name=None):
         self.device = None
         self.transform_x = None
         self.transform_y = None
-        self.module = None
+        self.module = module
         self.optimizer = None
         self.scheduler = None
         self.loss = None
         self.acc_fn = None
         self.name = name
         self.model_path = None
         self.epoch = 0
@@ -70,16 +70,16 @@
     
     
     def set_path(self, model_path):
         self.model_path = model_path
         return self
     
     
-    def init(self, acc=None, optimizer=None, loss=None, scheduler=None, lr=1e-3,
-        transform_x=None, transform_y=None):
+    def init(self, acc=None, optimizer=None, loss=None, scheduler=None,
+        lr=1e-3, transform_x=None, transform_y=None):
         
         """
         Init model
         """
         
         if acc is not None:
             self.acc_fn = acc
```

### Comparing `tiny_ai_helper-0.1.6/tiny_ai_helper/Trainer.py` & `tiny_ai_helper-0.1.7/tiny_ai_helper/Trainer.py`

 * *Files 8% similar despite different names*

```diff
@@ -94,16 +94,16 @@
         # Получить текущий lr
         res_lr = []
         for param_group in self.model.optimizer.param_groups:
             res_lr.append(param_group['lr'])
         res_lr_str = str(res_lr)
         
         # Результат обучения
-        loss_train = '%.3e' % (self.loss_train / self.count_train)
-        loss_val = '%.3e' % (self.loss_val / self.count_val)
+        loss_train = '%.3e' % (self.loss_train / self.batch_train)
+        loss_val = '%.3e' % (self.loss_val / self.batch_val)
         
         acc_train = self.acc_train / self.count_train
         acc_val = self.acc_val / self.count_val
         acc_rel = acc_train / acc_val if acc_val > 0 else 0
         acc_train = str(round(acc_train * 10000) / 100)
         acc_val = str(round(acc_val * 10000) / 100)
         acc_train = acc_train.ljust(5, "0")
@@ -117,16 +117,16 @@
             f"loss: {loss_train}, loss_val: {loss_val}, lr: {res_lr_str}, " +
             f"t: {time}s"
         )
         
         # Update model history
         self.model.epoch = self.epoch
         self.model.history[self.epoch] = {
-            "loss_train": self.loss_train / self.count_train,
-            "loss_val": self.loss_val / self.count_val,
+            "loss_train": self.loss_train / self.batch_train,
+            "loss_val": self.loss_val / self.batch_val,
             "acc_train": self.acc_train / self.count_train,
             "acc_val": self.acc_val / self.count_val,
             "acc_rel": acc_rel,
             "count_train": self.count_train,
             "count_val": self.count_val,
             "batch_iter": self.batch_iter,
             "res_lr": res_lr,
@@ -157,20 +157,22 @@
         loss_value_item = loss_value.item()
         batch_count = len(batch_x[0]) if isinstance(batch_x, list) else len(batch_x)
         
         if kind == "train":
             self.acc_train = self.acc_train + acc
             self.loss_train = self.loss_train + loss_value_item
             self.count_train = self.count_train + batch_count
+            self.batch_train = self.batch_train + 1
             self.batch_iter = self.batch_iter + batch_count
         
         elif kind == "valid":
             self.acc_val = self.acc_val + acc
             self.loss_val = self.loss_val + loss_value_item
             self.count_val = self.count_val + batch_count
+            self.batch_val = self.batch_val + 1
             self.batch_iter = self.batch_iter + batch_count
     
     
     def fit(self, model, train_dataset, val_dataset, batch_size=64, epochs=10):
         
         """
         Fit model
@@ -213,14 +215,16 @@
                 
                 self.loss_train = 0
                 self.loss_val = 0
                 self.acc_train = 0
                 self.acc_val = 0
                 self.count_train = 0
                 self.count_val = 0
+                self.batch_train = 0
+                self.batch_val = 0
                 self.batch_iter = 0
                 self.epoch = self.epoch + 1
                 self.time_start = time.time()
                 
                 self.on_start_epoch()
                 module.train()
```

### Comparing `tiny_ai_helper-0.1.6/tiny_ai_helper/layers.py` & `tiny_ai_helper-0.1.7/tiny_ai_helper/layers.py`

 * *Files identical despite different names*

### Comparing `tiny_ai_helper-0.1.6/tiny_ai_helper/mp.py` & `tiny_ai_helper-0.1.7/tiny_ai_helper/mp.py`

 * *Files identical despite different names*

### Comparing `tiny_ai_helper-0.1.6/tiny_ai_helper/utils.py` & `tiny_ai_helper-0.1.7/tiny_ai_helper/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -160,15 +160,15 @@
 
 def batch_to(x, device):
     
     """
     Move batch to device
     """
     
-    if isinstance(x, list):
+    if isinstance(x, list) or isinstance(x, tuple):
         for i in range(len(x)):
             x[i] = x[i].to(device)
     else:
         x = x.to(device)
     
     return x
 
@@ -467,24 +467,23 @@
         if file:
             file.close()
             file = None
     
     return obj
 
 
-def summary(module, x, model_name=None, transform_x=None, device=None):
+def summary(module, x, y=None, model_name=None, batch_transform=None, device=None):
         
         """
         Show model summary
         """
         
         hooks = []
         layers = []
         res = {
-            "layer_name_max": 10,
             "params_count": 0,
             "params_train_count": 0,
             "total_size": 0,
         }
         
         def forward_hook(module, input, output):
             
@@ -494,17 +493,14 @@
             layer = {
                 "name": module.__class__.__name__,
                 "class_name": module.__class__.__module__ + "." + module.__class__.__name__,
                 "shape": output.shape,
                 "params": 0
             }
             
-            if res["layer_name_max"] < len(module.__class__.__name__):
-                res["layer_name_max"] = len(module.__class__.__name__)
-            
             # Get weight
             if hasattr(module, "weight"):
                 params, size = tensor_size(module.weight)
                 res["params_count"] += params
                 res["total_size"] += size
                 layer["params"] += params
                 
@@ -537,26 +533,29 @@
                 x,
                 batch_size=2,
                 drop_last=False,
                 shuffle=False
             )
             it = loader._get_iterator()
             
-            x, _ = next(it)
+            x, y = next(it)
+        
+        if batch_transform is None:
+            batch_transform = getattr(module, "batch_transform", None)
         
         # Trasform
-        if transform_x is not None:
-            x = transform_x(x)
+        if batch_transform is not None:
+            x, _ = batch_transform(x, y)
         
         # Move to device
         if device is not None:
             x = batch_to(x, device)
         
         # Add input size
-        if isinstance(x, list):
+        if isinstance(x, list) or isinstance(x, tuple):
             shapes = []
             for i in range(len(x)):
                 params, size = tensor_size(x[i])
                 shapes.append(x[i].shape)
             res["total_size"] += size
             layers.append({
                 "name": "Input",
@@ -580,37 +579,218 @@
         if torch.cuda.is_available():
             torch.cuda.empty_cache()
         
         # Remove hooks
         for item in hooks:
             item.remove()
         
-        # Print info
-        def format_row(res, args):
-            layer_name_max = res["layer_name_max"] + 5
-            s = "{:<5} {:>"+str(layer_name_max)+"} {:>20} {:>15}"
-            return s.format(*args)
-        
         res['total_size'] = round(res['total_size'] / 1024 / 1024 * 100) / 100
         
-        width = 63
-        print( "=" * width )
-        print( format_row(res, ["", "Layer", "Output", "Params"]) )
-        print( "-" * width )
-        
+        # Calc info
+        values = [ ["", "Layer", "Output", "Params"] ]
         for i, layer in enumerate(layers):
             shape = layer["shape"]
             shape_str = ""
             if isinstance(shape, list):
                 shape = [ "(" + ", ".join(map(str,s)) + ")" for s in shape ]
                 shape_str = "[" + ", ".join(shape) + "]"
             else:
                 shape_str = "(" + ", ".join(map(str,shape)) + ")"
-            print( format_row(res, [i + 1, layer["name"], shape_str, layer["params"]]) )
+            
+            values.append([i + 1, layer["name"], shape_str, layer["params"]])
+        
+        # Print info
+        info_sizes = [2, 7, 7, 5]
+        for _, value in enumerate(values):
+            for i in range(4):
+                sz = len(str(value[i]))
+                if info_sizes[i] < sz:
+                    info_sizes[i] = sz
+            
+        def format_row(arr, size):
+            s = "{:<"+str(size[0] + 1)+"} {:>"+str(size[1] + 2)+"}" + \
+                "{:>"+str(size[2] + 3)+"} {:>"+str(size[3] + 2)+"}"
+            return s.format(*arr)
+        
+        width = 63
+        print( "=" * width )
+        print( format_row(["", "Layer", "Output", "Params"], info_sizes) )
+        print( "-" * width )
+        
+        for _, value in enumerate(values):
+            print( format_row(value, info_sizes) )
         
         print( "-" * width )
         if model_name is not None:
             print( f"Model name: {model_name}" )
         print( f"Total params: {res['params_count']}" )
         print( f"Trainable params: {res['params_train_count']}" )
         print( f"Total size: {res['total_size']} MiB" )
-        print( "=" * width )
+        print( "=" * width )
+
+
+def fit(model, train_dataset, val_dataset,
+    batch_size=64, epochs=10, device=None,
+    min_lr=1e-5, reduction='mean'
+):
+    
+    if torch.cuda.is_available():
+        torch.cuda.empty_cache()
+    
+    module = model.module
+    optimizer = model.optimizer
+    scheduler = model.scheduler
+    loss_fn = model.loss
+    
+    batch_transform = getattr(module, "batch_transform", None)
+    
+    train_loader = DataLoader(
+        train_dataset,
+        batch_size=batch_size,
+        drop_last=False,
+        shuffle=True
+    )
+    val_loader = DataLoader(
+        val_dataset,
+        batch_size=batch_size,
+        drop_last=False,
+        shuffle=False
+    )
+    
+    module = module.to(device)
+    
+    print ("Start train")
+    try:
+        for epoch in range(epochs):
+            
+            time_start = time.time()
+            train_count = 0
+            train_loss = 0
+            train_iter = 0
+            val_count = 0
+            val_loss = 0
+            val_iter = 0
+            total_count = len(train_dataset) + len(val_dataset)
+            pos = 0
+            
+            # train mode
+            module.train()
+            
+            for x_batch, y_batch in train_loader:
+                
+                # data to device
+                x_batch = x_batch.to(device)
+                y_batch = y_batch.to(device)
+                if batch_transform:
+                    x_batch, y_batch = batch_transform(x_batch, y_batch)
+                
+                # set parameter gradients to zero
+                optimizer.zero_grad()
+                
+                # forward
+                y_pred = module(x_batch)
+                loss = loss_fn(y_pred, y_batch)
+                loss.backward()
+                optimizer.step()
+
+                # add metrics
+                batch_len = len(x_batch[0]) \
+                    if isinstance(x_batch, tuple) or isinstance(x_batch, list) \
+                    else len(x_batch)
+                train_loss += loss
+                train_count += batch_len
+                train_iter += 1
+                pos += batch_len
+
+                del x_batch, y_batch, y_pred, loss
+
+                if torch.cuda.is_available():
+                    torch.cuda.empty_cache()
+                
+                print(f"\r{round(pos / total_count * 100)}%", end="")
+
+            
+            with torch.no_grad():
+
+                # testing mode
+                module.eval()
+                
+                for x_batch, y_batch in val_loader:
+                    
+                    # data to device
+                    x_batch = x_batch.to(device)
+                    y_batch = y_batch.to(device)
+                    if batch_transform:
+                        x_batch, y_batch = batch_transform(x_batch, y_batch)
+                    
+                    # forward
+                    y_pred = module(x_batch)
+                    loss = loss_fn(y_pred, y_batch)
+                    
+                    # add metrics
+                    batch_len = len(x_batch[0]) \
+                        if isinstance(x_batch, tuple) or isinstance(x_batch, list) \
+                        else len(x_batch)
+                    val_loss += loss
+                    val_count += batch_len
+                    val_iter += 1
+                    pos += batch_len
+                    
+                    del x_batch, y_batch, y_pred, loss
+
+                    if torch.cuda.is_available():
+                        torch.cuda.empty_cache()
+                    
+                    print(f"\r{round(pos / total_count * 100)}%", end="")
+            
+            if reduction == "mean":
+                train_loss = (train_loss / train_iter).item()
+                val_loss = (val_loss / val_iter).item()
+            
+            elif reduction == "sum":
+                train_loss = (train_loss / train_count).item()
+                val_loss = (val_loss / val_count).item()
+            
+            scheduler.step(val_loss)
+            
+            # Current lr
+            res_lr = []
+            for param_group in optimizer.param_groups:
+                res_lr.append( round(param_group['lr'], 7) )
+            res_lr_str = str(res_lr)
+            
+            time_end = time.time()
+            t = round(time_end - time_start)
+            
+            h = {
+                "loss_train": train_loss,
+                "loss_val": val_loss,
+                "count_train": train_count,
+                "count_val": val_count,
+                "res_lr": res_lr,
+                "time": t,
+            }
+            
+            model.history[epoch] = h
+            
+            # Print result
+            train_loss = "{:.9f}".format(train_loss)
+            val_loss = "{:.9f}".format(val_loss)
+            
+            print(f'\repoch: {epoch + 1}, ' +
+                'train_loss: {train_loss}, val_loss: {val_loss}, ' +
+                'lr: {res_lr_str}, t: {t}s')
+            
+            if res_lr[0] < min_lr:
+                break
+
+        print ("Ok")
+
+    except KeyboardInterrupt:
+        
+        print ("")
+        print ("Stopped manually")
+        print ("")
+
+    if torch.cuda.is_available():
+        torch.cuda.empty_cache()
+
```

### Comparing `tiny_ai_helper-0.1.6/tiny_ai_helper.egg-info/PKG-INFO` & `tiny_ai_helper-0.1.7/tiny_ai_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiny-ai-helper
-Version: 0.1.6
+Version: 0.1.7
 Summary: Tiny AI Helper for PyTorch
 Home-page: https://github.com/bayrell/ai_helper
 Author: Ildar Bikmamatov
 Author-email: support@bayrell.org
 License: MIT License
 Keywords: ai helper,pytorch
 Platform: UNKNOWN
```

