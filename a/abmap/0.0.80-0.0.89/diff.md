# Comparing `tmp/abmap-0.0.80.tar.gz` & `tmp/abmap-0.0.89.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/abmap-0.0.80.tar", last modified: Mon May  1 12:31:49 2023, max compression
+gzip compressed data, was "/net/scratch3/scratch3-3/chihoim/ablm/dist/.tmp-edsku1mq/abmap-0.0.89.tar", last modified: Tue May  2 14:30:12 2023, max compression
```

## Comparing `abmap-0.0.80.tar` & `abmap-0.0.89.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwsr-x   0 rsingh   (15494) cb       (17681)        0 2023-05-01 12:31:49.000000 abmap-0.0.80/
--rw-rw-r--   0 rsingh   (15494) cb       (17681)     1098 2023-03-16 14:35:14.000000 abmap-0.0.80/LICENSE.txt
--rw-rw-r--   0 rsingh   (15494) cb       (17681)       15 2023-03-16 14:35:14.000000 abmap-0.0.80/MANIFEST.in
--rw-rw-r--   0 rsingh   (15494) cb       (17681)      286 2023-05-01 12:31:49.000000 abmap-0.0.80/PKG-INFO
--rw-rw-r--   0 rsingh   (15494) cb       (17681)     1787 2023-05-01 12:17:52.000000 abmap-0.0.80/README.md
-drwxrwsr-x   0 rsingh   (15494) cb       (17681)        0 2023-05-01 12:31:49.000000 abmap-0.0.80/abmap/
--rw-rw-r--   0 rsingh   (15494) cb       (17681)      395 2023-05-01 12:26:10.000000 abmap-0.0.80/abmap/__init__.py
--rw-rw-r--   0 rsingh   (15494) cb       (17681)     1747 2023-05-01 11:59:02.000000 abmap-0.0.80/abmap/__main__.py
--rw-rw-r--   0 rsingh   (15494) cb       (17681)    10758 2023-05-01 11:59:02.000000 abmap-0.0.80/abmap/abmap_augment.py
--rw-rw-r--   0 rsingh   (15494) cb       (17681)      437 2023-03-16 14:35:14.000000 abmap-0.0.80/abmap/base_config.py
-drwxrwsr-x   0 rsingh   (15494) cb       (17681)        0 2023-05-01 12:31:49.000000 abmap-0.0.80/abmap/commands/
--rw-rw-r--   0 rsingh   (15494) cb       (17681)       39 2023-03-16 14:35:14.000000 abmap-0.0.80/abmap/commands/__init__.py
--rw-rw-r--   0 rsingh   (15494) cb       (17681)     2395 2023-05-01 11:59:02.000000 abmap-0.0.80/abmap/commands/augment.py
--rw-rw-r--   0 rsingh   (15494) cb       (17681)     7470 2023-05-01 11:59:02.000000 abmap-0.0.80/abmap/commands/embed.py
--rw-rw-r--   0 rsingh   (15494) cb       (17681)    21270 2023-05-01 11:59:02.000000 abmap-0.0.80/abmap/commands/train.py
--rw-rw-r--   0 rsingh   (15494) cb       (17681)    12204 2023-03-16 14:35:14.000000 abmap-0.0.80/abmap/dataloader.py
--rw-rw-r--   0 rsingh   (15494) cb       (17681)    12094 2023-03-16 14:35:14.000000 abmap-0.0.80/abmap/libraseq_preprocess.py
--rw-rw-r--   0 rsingh   (15494) cb       (17681)    18770 2023-05-01 12:31:41.000000 abmap-0.0.80/abmap/model.py
--rw-rw-r--   0 rsingh   (15494) cb       (17681)     1531 2023-03-16 14:35:14.000000 abmap-0.0.80/abmap/mutate.py
--rw-rw-r--   0 rsingh   (15494) cb       (17681)     5626 2023-05-01 11:59:02.000000 abmap-0.0.80/abmap/plm_embed.py
--rw-rw-r--   0 rsingh   (15494) cb       (17681)    14912 2023-05-01 11:59:02.000000 abmap-0.0.80/abmap/sabdab_preprocess.py
--rw-rw-r--   0 rsingh   (15494) cb       (17681)     5700 2023-05-01 11:59:02.000000 abmap-0.0.80/abmap/utils.py
-drwxrwsr-x   0 rsingh   (15494) cb       (17681)        0 2023-05-01 12:31:49.000000 abmap-0.0.80/abmap.egg-info/
--rw-rw-r--   0 rsingh   (15494) cb       (17681)      286 2023-05-01 12:31:49.000000 abmap-0.0.80/abmap.egg-info/PKG-INFO
--rw-rw-r--   0 rsingh   (15494) cb       (17681)      721 2023-05-01 12:31:49.000000 abmap-0.0.80/abmap.egg-info/SOURCES.txt
--rw-rw-r--   0 rsingh   (15494) cb       (17681)        1 2023-05-01 12:31:49.000000 abmap-0.0.80/abmap.egg-info/dependency_links.txt
--rw-rw-r--   0 rsingh   (15494) cb       (17681)       47 2023-05-01 12:31:49.000000 abmap-0.0.80/abmap.egg-info/entry_points.txt
--rw-rw-r--   0 rsingh   (15494) cb       (17681)      125 2023-05-01 12:31:49.000000 abmap-0.0.80/abmap.egg-info/requires.txt
--rw-rw-r--   0 rsingh   (15494) cb       (17681)       15 2023-05-01 12:31:49.000000 abmap-0.0.80/abmap.egg-info/top_level.txt
-drwxrwsr-x   0 rsingh   (15494) cb       (17681)        0 2023-05-01 12:31:49.000000 abmap-0.0.80/analysis/
--rw-rw-r--   0 rsingh   (15494) cb       (17681)        0 2023-03-16 14:35:14.000000 abmap-0.0.80/analysis/__init__.py
--rw-rw-r--   0 rsingh   (15494) cb       (17681)    13874 2023-03-16 14:35:14.000000 abmap-0.0.80/analysis/briney_analysis.py
--rw-rw-r--   0 rsingh   (15494) cb       (17681)     6033 2023-03-16 14:35:14.000000 abmap-0.0.80/analysis/covabdab_analyze.py
--rw-rw-r--   0 rsingh   (15494) cb       (17681)    35361 2023-02-07 15:11:30.000000 abmap-0.0.80/analysis/desautels_analyze.py
--rw-rw-r--   0 rsingh   (15494) cb       (17681)    37858 2023-02-07 15:11:30.000000 abmap-0.0.80/analysis/strucpred_analysis.py
--rw-rw-r--   0 rsingh   (15494) cb       (17681)     7143 2023-05-01 11:59:02.000000 abmap-0.0.80/analysis/thera_analysis.py
--rw-rw-r--   0 rsingh   (15494) cb       (17681)      437 2023-05-01 11:59:04.000000 abmap-0.0.80/pyproject.toml
--rw-rw-r--   0 rsingh   (15494) cb       (17681)       38 2023-05-01 12:31:49.000000 abmap-0.0.80/setup.cfg
--rw-rw-r--   0 rsingh   (15494) cb       (17681)      875 2023-05-01 12:25:53.000000 abmap-0.0.80/setup.py
+drwxrwxr-x   0 chihoim  (26113) chihoim  (26113)        0 2023-05-02 14:30:12.000000 abmap-0.0.89/
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)     1098 2023-02-28 02:48:26.000000 abmap-0.0.89/LICENSE.txt
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)       15 2023-02-28 02:50:10.000000 abmap-0.0.89/MANIFEST.in
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)     2283 2023-05-02 14:30:12.000000 abmap-0.0.89/PKG-INFO
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)     1787 2023-05-01 15:40:47.000000 abmap-0.0.89/README.md
+drwxrwxr-x   0 chihoim  (26113) chihoim  (26113)        0 2023-05-02 14:30:12.000000 abmap-0.0.89/abmap/
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)      392 2023-05-02 14:29:31.000000 abmap-0.0.89/abmap/__init__.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)     1747 2023-04-28 00:51:56.000000 abmap-0.0.89/abmap/__main__.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)    10758 2023-04-28 00:51:56.000000 abmap-0.0.89/abmap/abmap_augment.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)      437 2023-03-02 06:59:12.000000 abmap-0.0.89/abmap/base_config.py
+drwxrwxr-x   0 chihoim  (26113) chihoim  (26113)        0 2023-05-02 14:30:12.000000 abmap-0.0.89/abmap/commands/
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)       39 2023-03-02 05:58:52.000000 abmap-0.0.89/abmap/commands/__init__.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)     2395 2023-04-28 00:51:56.000000 abmap-0.0.89/abmap/commands/augment.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)     7470 2023-04-28 00:51:56.000000 abmap-0.0.89/abmap/commands/embed.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)    20348 2023-05-02 01:26:42.000000 abmap-0.0.89/abmap/commands/train.py
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)    12204 2023-03-05 19:41:16.000000 abmap-0.0.89/abmap/dataloader.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)    12094 2023-03-02 06:10:26.000000 abmap-0.0.89/abmap/libraseq_preprocess.py
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)    18789 2023-05-02 01:18:34.000000 abmap-0.0.89/abmap/model.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)     1531 2023-03-16 18:20:17.000000 abmap-0.0.89/abmap/mutate.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)     5626 2023-04-28 00:51:57.000000 abmap-0.0.89/abmap/plm_embed.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)    14912 2023-04-28 00:51:57.000000 abmap-0.0.89/abmap/sabdab_preprocess.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)     5700 2023-04-21 14:55:50.000000 abmap-0.0.89/abmap/utils.py
+drwxrwxr-x   0 chihoim  (26113) chihoim  (26113)        0 2023-05-02 14:30:12.000000 abmap-0.0.89/abmap.egg-info/
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)     2283 2023-05-02 14:30:12.000000 abmap-0.0.89/abmap.egg-info/PKG-INFO
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)      721 2023-05-02 14:30:12.000000 abmap-0.0.89/abmap.egg-info/SOURCES.txt
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)        1 2023-05-02 14:30:12.000000 abmap-0.0.89/abmap.egg-info/dependency_links.txt
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)       46 2023-05-02 14:30:12.000000 abmap-0.0.89/abmap.egg-info/entry_points.txt
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)      125 2023-05-02 14:30:12.000000 abmap-0.0.89/abmap.egg-info/requires.txt
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)       15 2023-05-02 14:30:12.000000 abmap-0.0.89/abmap.egg-info/top_level.txt
+drwxrwxr-x   0 chihoim  (26113) chihoim  (26113)        0 2023-05-02 14:30:12.000000 abmap-0.0.89/analysis/
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)        0 2023-02-24 06:16:30.000000 abmap-0.0.89/analysis/__init__.py
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)    13874 2023-02-14 13:40:17.000000 abmap-0.0.89/analysis/briney_analysis.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)     6033 2023-02-24 06:18:30.000000 abmap-0.0.89/analysis/covabdab_analyze.py
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)    35361 2023-02-08 02:32:36.000000 abmap-0.0.89/analysis/desautels_analyze.py
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)    37858 2023-02-08 02:32:36.000000 abmap-0.0.89/analysis/strucpred_analysis.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)     7143 2023-04-28 00:51:57.000000 abmap-0.0.89/analysis/thera_analysis.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)      437 2023-05-02 14:22:39.000000 abmap-0.0.89/pyproject.toml
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)       38 2023-05-02 14:30:12.000000 abmap-0.0.89/setup.cfg
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)      875 2023-05-01 15:40:47.000000 abmap-0.0.89/setup.py
```

### Comparing `abmap-0.0.80/LICENSE.txt` & `abmap-0.0.89/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `abmap-0.0.80/README.md` & `abmap-0.0.89/README.md`

 * *Files identical despite different names*

### Comparing `abmap-0.0.80/abmap/__main__.py` & `abmap-0.0.89/abmap/__main__.py`

 * *Files identical despite different names*

### Comparing `abmap-0.0.80/abmap/abmap_augment.py` & `abmap-0.0.89/abmap/abmap_augment.py`

 * *Files identical despite different names*

### Comparing `abmap-0.0.80/abmap/commands/augment.py` & `abmap-0.0.89/abmap/commands/augment.py`

 * *Files identical despite different names*

### Comparing `abmap-0.0.80/abmap/commands/embed.py` & `abmap-0.0.89/abmap/commands/embed.py`

 * *Files identical despite different names*

### Comparing `abmap-0.0.80/abmap/commands/train.py` & `abmap-0.0.89/abmap/commands/train.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 type_to_dim = {'beplerberger':6165, 'esm1b':1280, 'tape':768, 'dscript':100}
 
 
 class TrainArguments(NamedTuple):
     cmd: str
     device_num: int
-    log_name: str
+    log_file: str
     exec_type: str
     num_epochs: int
     embed_dir: str
     batch_size: int
     print_every: int
     ckpt_every: int
     lr: float
@@ -41,22 +41,23 @@
     emb_type: str
     model_loadpath: str
     model_savepath: str
     mut_type: str
     chain_type: str
     region: str
     lambda1: float
-    alpha: float
+    init_alpha: float
+    update_alpha: bool
 
 
 def add_args(parser):
     parser.add_argument('--device_num', type=int, default=0,
                         help='Indicate which GPU device to train the model on')
 
-    parser.add_argument('--log_name', type=str,
+    parser.add_argument('--log_file', type=str,
                         help='Name of the log file with plot values.')
 
     parser.add_argument('--exec_type', type=str, default='train',
                         choices=['train', 'evaluate'],
                         help='Execution Mode.')
 
     parser.add_argument('--num_epochs', type=int, default=1,
@@ -77,15 +78,14 @@
     parser.add_argument('--lr', type=float, default=0.01,
                         help='Model learning rate')
 
     parser.add_argument('--gamma', type=float, default=0.1,
                         help='Decay rate for the lr scheduler.')
 
     parser.add_argument('--emb_type', type=str, default='beplerberger',
-                        choices=['beplerberger', 'esm1b', 'tape', 'dscript', 'concat', 'protbert'],
                         help='Embedding Type.')
 
     parser.add_argument('--model_loadpath', type=str, default='None',
                         help='Path to an already trained model.')
 
     parser.add_argument('--model_savepath', type=str, default='',
                         help='Path to save the trained model.')
@@ -100,26 +100,29 @@
 
     parser.add_argument('--region', type=str, default='whole',
                         help='Which region on the sequence you would like to train on')
 
     parser.add_argument('--lambda1', type=float, default=0.0005,
                         help='Weight on the regularization loss')
 
-    parser.add_argument('--alpha', type=float, default = 7,
-                        help='Weight on the mse losses')
+    parser.add_argument('--init_alpha', type=float, default = 0.0,
+                        help='Weight on the mse losses. 0 means an equal weight.')
+
+    parser.add_argument('--update_alpha', action="store_true", dest='update_alpha',
+                        help='The alpha value for the mse losses will be updated iteratively.')
 
     return parser
 
 
-def train_model(device_num, log_name, exec_type, num_epochs, model_loadpath, model_savepath, region,
-                embed_dir, batch_size, chain_type, alpha, lambda1, print_every=100, lr=0.01, emb_type='beplerberger', 
-                ckpt_every=10, mut_type='cat2', gamma=0.5, **kwargs):
+def train_model(device_num, log_file, exec_type, num_epochs, model_loadpath, model_savepath, region,
+                embed_dir, batch_size, chain_type, init_alpha, update_alpha, lambda1, print_every=100, 
+                lr=0.01, emb_type='beplerberger', ckpt_every=10, mut_type='cat2', gamma=0.5, **kwargs):
     start_time = time.time()
 
-    if log_name == None:
+    if log_file == None:
         print("Your log will not be saved...")
 
     device = torch.device("cuda:{}".format(device_num) if torch.cuda.is_available() else "cpu")
 
     if embed_dir == "":
         print("You must provide the name of the directory for input embeddings")
         raise ValueError
@@ -133,25 +136,28 @@
     print("done loading!")
     train_size = len(train_loader_sab.dataset)
 
     # load model/operators
     if emb_type == 'beplerberger':
         model = AbMAPAttn(embed_dim=2200, mid_dim2=1024, mid_dim3=512, 
                                      proj_dim=252, num_enc_layers=1, num_heads=16).to(device)
-    if emb_type == 'protbert':
+    elif emb_type == 'protbert':
         model = AbMAPAttn(embed_dim=1024, mid_dim2=512, mid_dim3=256, 
                                      proj_dim=252, num_enc_layers=1, num_heads=16).to(device)
-    if emb_type == 'esm1b':
+    elif emb_type == 'esm1b' or emb_type == 'esm2':
         model = AbMAPAttn(embed_dim=1280, mid_dim2=512, mid_dim3=256, 
                                      proj_dim=252, num_enc_layers=1, num_heads=16).to(device)
-    if emb_type == 'tape':
+    elif emb_type == 'tape':
         model = AbMAPAttn(embed_dim=768, mid_dim2=256, mid_dim3=128, 
                                      proj_dim=60, num_enc_layers=1, num_heads=8).to(device)
+    else:
+        raise ValueError(f"The Embed Type {emb_type} Doesn't Exist!")
+
     loss_fn = nn.MSELoss()
-    loss_wrapper = MultiTaskLossWrapper(2).to(device)
+    loss_wrapper = MultiTaskLossWrapper(2, init_alpha, update_alpha).to(device)
     # loss_opt = opt.SGD(loss_wrapper.parameters(), lr=lr)
     
     if model_loadpath == 'None':
         prev_epochs = 0
         optimizer = opt.SGD([{'params': model.parameters()},
                              {'params': loss_wrapper.parameters(), 'lr': 1e-3},], lr=lr)
         scheduler = MultiStepLR(optimizer, milestones=[40, 45], gamma=gamma)
@@ -216,24 +222,15 @@
                 # compute loss and back propagate
                 reg_term = torch.zeros(e1_s.shape).cuda(device)
                 for em in [e1_s, e2_s, e1_f, e2_f]:
                     em_sq = em ** 2
                     reg_term += em_sq*torch.log(em_sq + 1e-7)
                 reg_loss = lambda1*torch.sum(reg_term)
 
-
-                if i < 0:
-                    mse_loss_s = loss_fn(pred_s, tmscore.cuda(device))
-                    mse_loss_f = loss_fn(pred_f, func_sc.cuda(device))
-
-                    # mse_loss = mse_loss_s + mse_loss_f
-                    mse_loss = mse_loss_s*alpha + mse_loss_f/alpha
-                    alpha_print = alpha
-                else:
-                    mse_loss = loss_wrapper(pred_s, tmscore.cuda(device), pred_f, func_sc.cuda(device))
+                mse_loss = loss_wrapper(pred_s, tmscore.cuda(device), pred_f, func_sc.cuda(device))
 
                 total_reg_loss += reg_loss.item()
                 total_mse_loss += mse_loss.item()
                 total_mse_loss_s += loss_wrapper.loss_s.item()
                 total_mse_loss_f += loss_wrapper.loss_f.item()
                 loss = mse_loss + reg_loss
                 
@@ -246,16 +243,14 @@
                 train_preds_s.append(pred_s)
                 train_preds_f.append(pred_f)
                 train_targs_s.append(tmscore.cuda(device))
                 train_targs_f.append(func_sc.cuda(device))
 
                 # print intermediate loss values
                 if k % print_every == 0:
-                    # writer.add_scalar('Loss/train', total_loss/(k+1), stept)#i+(k+1)*batch_size/train_size)
-                    # stept += 1
                     print("TRAIN Epoch {}, Batch {}, MSE Loss S: {}, MSE Loss F: {}, Reg Loss: {}, Alpha: {}".format(prev_epochs+i+1, 
                                             k, total_mse_loss_s/(k+1), total_mse_loss_f/(k+1), total_reg_loss/(k+1), loss_wrapper.alpha.item()))
 
             train_losses.append((total_loss/batch_count, total_mse_loss/batch_count, total_reg_loss/batch_count))
 
             # computing spearman rank scores
             train_preds_s, train_targs_s = torch.cat(train_preds_s), torch.cat(train_targs_s)
@@ -303,21 +298,16 @@
                     reg_term = torch.zeros(e1_s.shape).cuda(device)
                     for em in [e1_s, e2_s, e1_f, e2_f]:
                         em_sq = em ** 2
                         reg_term += em_sq*torch.log(em_sq + 1e-7)
                     reg_loss = lambda1*torch.sum(reg_term)
                     # reg_loss = lambda1*torch.sum((e1_s - unit_norm)**2 + (e2_s - unit_norm)**2 + (e1_f - unit_norm)**2 + (e2_f - unit_norm)**2)
 
-                    if i < 0:
-                        mse_loss_s = loss_fn(pred_s, tmscore.cuda(device))
-                        mse_loss_f = loss_fn(pred_f, func_sc.cuda(device))
-                        # mse_loss = mse_loss_s + mse_loss_f
-                        mse_loss = mse_loss_s*alpha + mse_loss_f/alpha
-                    else:
-                        mse_loss = loss_wrapper(pred_s, tmscore.cuda(device), pred_f, func_sc.cuda(device))
+                    mse_loss = loss_wrapper(pred_s, tmscore.cuda(device), pred_f, func_sc.cuda(device))
+
 
                     total_reg_loss += reg_loss.item()
                     total_mse_loss += mse_loss.item()
                     loss = mse_loss + reg_loss
 
                 total_loss += loss.item()
 
@@ -346,18 +336,14 @@
 
             # saving models:
             if (i+1)%ckpt_every == 0 and model_savepath != "":
                 if not os.path.isdir(model_savepath):
                     os.mkdir(model_savepath)
 
                 raw_model = model.module if hasattr(model, "module") else model
-                # model_sum = {'epoch':prev_epochs+i, 'model_state_dict': raw_model.state_dict(),
-                #             'optimizer_state_dict': optimizer.state_dict(),
-                            # 'model_attn_weights': [raw_model.attn_wts_s, raw_model.attn_wts_f],
-                            # 'loss_wrapper': loss_wrapper}
                 model_sum = raw_model.state_dict()
                 savepath = os.path.join(model_savepath, 'AbMAP_{}_{}_epoch{}.pt'.format(emb_type, chain_type, prev_epochs+i+1))
                 torch.save(model_sum, savepath)
 
             # learning rate schedule
             scheduler.step()
 
@@ -440,16 +426,16 @@
                               'train_spearmans': train_spearmans_f, 'val_spearmans':val_spearmans_f}
 
             logs[k]["train_losses"] = plots_dict['train_losses']
             logs[k]["val_losses"] = plots_dict['val_losses']
             logs[k]["train_spearmans"] = plots_dict['train_spearmans']
             logs[k]["val_spearmans"] = plots_dict['val_spearmans']
 
-    if log_name != None:
-        with open("../../logs/{}.p".format(log_name), "wb") as f:
+    if log_file != None:
+        with open(log_file, "wb") as f:
             pickle.dump(logs, f)
 
     end_time = time.time()
     print("It took {:.2f} minutes to train!".format((end_time-start_time)/60))
 
 
 def main(args):
```

### Comparing `abmap-0.0.80/abmap/dataloader.py` & `abmap-0.0.89/abmap/dataloader.py`

 * *Files identical despite different names*

### Comparing `abmap-0.0.80/abmap/libraseq_preprocess.py` & `abmap-0.0.89/abmap/libraseq_preprocess.py`

 * *Files identical despite different names*

### Comparing `abmap-0.0.80/abmap/model.py` & `abmap-0.0.89/abmap/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,30 +338,29 @@
 
         pred = transform(pred)
 
         return torch.reshape(pred, (-1,)), x1, x2
 
 
 class MultiTaskLossWrapper(nn.Module):
-    def __init__(self, task_num):
+    def __init__(self, task_num, init_alpha, update_alpha):
         super(MultiTaskLossWrapper, self).__init__()
         self.task_num = task_num
-        self.weights = nn.Parameter(torch.tensor(-2.0)) # if -2.0, alpha = e^2 = 7.xx
+        self.weights = nn.Parameter(torch.tensor(init_alpha), requires_grad=update_alpha) # if -2.0, alpha = e^2 = 7.xx
         self.loss_fn = nn.MSELoss()
         self.loss_s, self.loss_f = None, None
         self.alpha = None
 
     def forward(self, pred_s, label_s, pred_f, label_f):
         loss_s = self.loss_fn(pred_s, label_s)
         loss_f = self.loss_fn(pred_f, label_f)
 
         self.loss_s, self.loss_f = loss_s, loss_f
 
         precision_s = torch.exp(-self.weights)
-        precision_s = torch.tensor(7.0)
         loss_s = precision_s*loss_s
         self.alpha = precision_s
 
         precision_f = 1/precision_s
         loss_f = precision_f*loss_f
         
         return loss_s + loss_f
```

### Comparing `abmap-0.0.80/abmap/mutate.py` & `abmap-0.0.89/abmap/mutate.py`

 * *Files identical despite different names*

### Comparing `abmap-0.0.80/abmap/plm_embed.py` & `abmap-0.0.89/abmap/plm_embed.py`

 * *Files identical despite different names*

### Comparing `abmap-0.0.80/abmap/sabdab_preprocess.py` & `abmap-0.0.89/abmap/sabdab_preprocess.py`

 * *Files identical despite different names*

### Comparing `abmap-0.0.80/abmap/utils.py` & `abmap-0.0.89/abmap/utils.py`

 * *Files identical despite different names*

### Comparing `abmap-0.0.80/abmap.egg-info/SOURCES.txt` & `abmap-0.0.89/abmap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `abmap-0.0.80/analysis/briney_analysis.py` & `abmap-0.0.89/analysis/briney_analysis.py`

 * *Files identical despite different names*

### Comparing `abmap-0.0.80/analysis/covabdab_analyze.py` & `abmap-0.0.89/analysis/covabdab_analyze.py`

 * *Files identical despite different names*

### Comparing `abmap-0.0.80/analysis/desautels_analyze.py` & `abmap-0.0.89/analysis/desautels_analyze.py`

 * *Files identical despite different names*

### Comparing `abmap-0.0.80/analysis/strucpred_analysis.py` & `abmap-0.0.89/analysis/strucpred_analysis.py`

 * *Files identical despite different names*

### Comparing `abmap-0.0.80/analysis/thera_analysis.py` & `abmap-0.0.89/analysis/thera_analysis.py`

 * *Files identical despite different names*

### Comparing `abmap-0.0.80/setup.py` & `abmap-0.0.89/setup.py`

 * *Files identical despite different names*

