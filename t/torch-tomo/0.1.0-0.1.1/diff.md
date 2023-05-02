# Comparing `tmp/torch_tomo-0.1.0-py3-none-any.whl.zip` & `tmp/torch_tomo-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 8108 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat     7711 b- defN 23-Mar-10 05:49 torch_tomo/CSET_pytorch.py
+Zip file size: 8985 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat     7949 b- defN 23-May-02 05:32 torch_tomo/CSET_pytorch.py
 -rw-rw-rw-  2.0 fat       64 b- defN 23-Mar-17 06:33 torch_tomo/__init__.py
 -rw-rw-rw-  2.0 fat    21705 b- defN 23-Mar-10 09:41 torch_tomo/tilt_series_alignment.py
--rw-rw-rw-  2.0 fat      233 b- defN 23-Mar-17 06:35 torch_tomo-0.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-17 06:35 torch_tomo-0.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Mar-17 06:35 torch_tomo-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      562 b- defN 23-Mar-17 06:35 torch_tomo-0.1.0.dist-info/RECORD
-7 files, 30378 bytes uncompressed, 7108 bytes compressed:  76.6%
+-rw-rw-rw-  2.0 fat     1080 b- defN 23-May-02 05:35 torch_tomo-0.1.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      219 b- defN 23-May-02 05:35 torch_tomo-0.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-02 05:35 torch_tomo-0.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-May-02 05:35 torch_tomo-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      653 b- defN 23-May-02 05:35 torch_tomo-0.1.1.dist-info/RECORD
+8 files, 31773 bytes uncompressed, 7841 bytes compressed:  75.3%
```

## zipnote {}

```diff
@@ -3,20 +3,23 @@
 
 Filename: torch_tomo/__init__.py
 Comment: 
 
 Filename: torch_tomo/tilt_series_alignment.py
 Comment: 
 
-Filename: torch_tomo-0.1.0.dist-info/METADATA
+Filename: torch_tomo-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: torch_tomo-0.1.0.dist-info/WHEEL
+Filename: torch_tomo-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: torch_tomo-0.1.0.dist-info/top_level.txt
+Filename: torch_tomo-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: torch_tomo-0.1.0.dist-info/RECORD
+Filename: torch_tomo-0.1.1.dist-info/top_level.txt
+Comment: 
+
+Filename: torch_tomo-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## torch_tomo/CSET_pytorch.py

```diff
@@ -17,23 +17,23 @@
         self.num_adr = len(adr)
         
         self.ts = []
         for i in range(self.num_adr):
             self.ts.append(tifffile.imread(adr[i]))
         
         if self.ts[0].shape[1] != self.ts[0].shape[2]:
-            print("The width and height of tilt-series images must be the same")
-            return
+            print("Warning: The width and height of tilt-series images must be the same")
+
         
         self.edge_length = self.ts[0].shape[1]
         
         self.ta = angles
         if self.ts[0].shape[0] != len(self.ta):
-            print("the number of angles is wrong")
-            return
+            print("Warning: the number of angles is wrong")
+
         self.n_tilt = len(self.ta)
         
         self.cuda_device = cuda_device
         print("cuda device: ", self.cuda_device)
         
         
     def NUFFT(self, pad_ratio=2.0, tilt_axis="horizontal"):
@@ -105,21 +105,23 @@
         FT_ts = np.asarray(FT_ts)
         
         kdata = torch.tensor(FT_ts.flatten()).to(torch.complex64).unsqueeze(0).unsqueeze(0)
         kdata = kdata.to(self.cuda_device)
         
         return kdata
 
-    def recontruct(self, n_iter=200, lmbd_l1=5E-4, lmbd_tv=3.0, l_rate=2E-5, save_adr="reconstructed_", verbose=True):
+    def recontruct(self, n_iter=200, lmbd_l1=5E-4, lmbd_tv=3.0, l_rate=2E-5, save_result=True, save_adr="reconstructed_", verbose=True):
         
+        self.reconstruction_result = []
         print(tabulate([
                         ["total number of iteration", n_iter], 
                         ["lambda_L1", lmbd_l1],
                         ["lambda_TV", lmbd_tv],
-                        ["learning rate", l_rate], 
+                        ["learning rate", l_rate],
+                        ["save the result (tiff)", save_result],
                         ["prefix for save", save_adr],
                         ]))
         
         solution = np.random.randn(self.edge_length, self.edge_length, self.edge_length)
         solution = torch.tensor(solution).to(torch.complex64).unsqueeze(0).unsqueeze(0)
         solution = solution.cuda(self.cuda_device)
         solution.requires_grad_(requires_grad=True)
@@ -185,9 +187,12 @@
                                     ["-main loss", main_loss.item(), main_loss.item()*100/total_loss.item()],
                                     ["-L1 loss", l1_reg.item(), l1_reg.item()*100/total_loss.item()], 
                                     ["-TV reg.", tv_reg.item(), tv_reg.item()*100/total_loss.item()],
                                     ]))
             print("The %d optimization has been finished."%(i+1))
 
             restored_object = solution.squeeze().data.cpu().numpy()
-
-            tifffile.imwrite(save_adr+"%02d.tif"%(i+1), np.real(restored_object).astype(np.float32))
+            
+            self.reconstruction_result.append(np.real(restored_object))
+            
+            if save_result:
+                tifffile.imwrite(save_adr+"%02d.tif"%(i+1), np.real(restored_object).astype(np.float32))
```

## Comparing `torch_tomo-0.1.0.dist-info/RECORD` & `torch_tomo-0.1.1.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,8 @@
-torch_tomo/CSET_pytorch.py,sha256=Tb1BXfwKT2P6Sa1c5u9XDv_o9RBABEpnhp43WHBxW-8,7711
+torch_tomo/CSET_pytorch.py,sha256=Evvkumq0sRAAfyjRF-kdrhloaa1eh5hUlzLPUEQx9XY,7949
 torch_tomo/__init__.py,sha256=xBwNr3xtJaU7-g9U1b_echbnxhR-cAsu96mKl1sGvWo,64
 torch_tomo/tilt_series_alignment.py,sha256=Fvz_4UVvPnMgGpJgiiLT1TiYiwyX5I0VuOfYrqt48E8,21705
-torch_tomo-0.1.0.dist-info/METADATA,sha256=chKlM8jI7jNIlvl65YBe6wpzvEb_A9SiTClk-Lolte0,233
-torch_tomo-0.1.0.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-torch_tomo-0.1.0.dist-info/top_level.txt,sha256=9y4hRDZ3s_8j0r7L3CbbzaPUE8Td-LkmgoaPLu2ynzc,11
-torch_tomo-0.1.0.dist-info/RECORD,,
+torch_tomo-0.1.1.dist-info/LICENSE,sha256=q2orF-8-HxSji3sPF5xVNfe6vjCXlvuRToFFtPm5FkE,1080
+torch_tomo-0.1.1.dist-info/METADATA,sha256=Ic1Fl1qGUMqICpYUMPyP630icLirAF1o8OTcLmtJD0A,219
+torch_tomo-0.1.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+torch_tomo-0.1.1.dist-info/top_level.txt,sha256=9y4hRDZ3s_8j0r7L3CbbzaPUE8Td-LkmgoaPLu2ynzc,11
+torch_tomo-0.1.1.dist-info/RECORD,,
```

