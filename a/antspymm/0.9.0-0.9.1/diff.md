# Comparing `tmp/antspymm-0.9.0.tar.gz` & `tmp/antspymm-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antspymm-0.9.0.tar", last modified: Thu Apr 20 13:41:02 2023, max compression
+gzip compressed data, was "antspymm-0.9.1.tar", last modified: Tue May  2 15:03:01 2023, max compression
```

## Comparing `antspymm-0.9.0.tar` & `antspymm-0.9.1.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-04-20 13:41:02.797792 antspymm-0.9.0/
--rw-r--r--   0 stnava     (501) staff       (20)    11357 2021-11-01 09:20:32.000000 antspymm-0.9.0/LICENSE
--rw-r--r--   0 stnava     (501) staff       (20)       33 2023-01-29 13:38:57.000000 antspymm-0.9.0/MANIFEST.in
--rw-r--r--   0 stnava     (501) staff       (20)    10184 2023-04-20 13:41:02.797531 antspymm-0.9.0/PKG-INFO
--rw-r--r--   0 stnava     (501) staff       (20)     9827 2023-04-12 13:23:21.000000 antspymm-0.9.0/README.md
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-04-20 13:41:02.790246 antspymm-0.9.0/antspymm/
--rw-r--r--   0 stnava     (501) staff       (20)     2690 2023-03-20 11:54:16.000000 antspymm-0.9.0/antspymm/__init__.py
--rw-r--r--   0 stnava     (501) staff       (20)   284711 2023-04-20 13:37:06.000000 antspymm-0.9.0/antspymm/mm.py
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-04-20 13:41:02.791689 antspymm-0.9.0/antspymm.egg-info/
--rw-r--r--   0 stnava     (501) staff       (20)    10184 2023-04-20 13:41:02.000000 antspymm-0.9.0/antspymm.egg-info/PKG-INFO
--rw-r--r--   0 stnava     (501) staff       (20)      741 2023-04-20 13:41:02.000000 antspymm-0.9.0/antspymm.egg-info/SOURCES.txt
--rw-r--r--   0 stnava     (501) staff       (20)        1 2023-04-20 13:41:02.000000 antspymm-0.9.0/antspymm.egg-info/dependency_links.txt
--rw-r--r--   0 stnava     (501) staff       (20)        1 2023-04-20 13:41:02.000000 antspymm-0.9.0/antspymm.egg-info/not-zip-safe
--rw-r--r--   0 stnava     (501) staff       (20)      112 2023-04-20 13:41:02.000000 antspymm-0.9.0/antspymm.egg-info/requires.txt
--rw-r--r--   0 stnava     (501) staff       (20)        9 2023-04-20 13:41:02.000000 antspymm-0.9.0/antspymm.egg-info/top_level.txt
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-04-20 13:41:02.795134 antspymm-0.9.0/docs/
--rw-r--r--   0 stnava     (501) staff       (20)  1939802 2023-01-29 13:48:53.000000 antspymm-0.9.0/docs/antspymm_data_dictionary.csv
--rw-r--r--   0 stnava     (501) staff       (20)      567 2023-04-12 13:06:30.000000 antspymm-0.9.0/docs/bids_cohort_example.py
--rw-r--r--   0 stnava     (501) staff       (20)     1296 2023-04-08 18:52:17.000000 antspymm-0.9.0/docs/example_run_from_directory.py
--rw-r--r--   0 stnava     (501) staff       (20)      478 2023-02-19 10:57:50.000000 antspymm-0.9.0/docs/make_dict_table.Rmd
--rw-r--r--   0 stnava     (501) staff       (20)      632 2023-04-12 13:06:30.000000 antspymm-0.9.0/docs/nrg_cohort_example.py
--rw-r--r--   0 stnava     (501) staff       (20)     2082 2023-03-20 13:00:28.000000 antspymm-0.9.0/docs/outlierness.py
--rw-r--r--   0 stnava     (501) staff       (20)     3643 2023-04-15 22:47:31.000000 antspymm-0.9.0/docs/ukbb_to_nrg_processing.py
--rw-r--r--   0 stnava     (501) staff       (20)     4546 2023-04-16 12:24:12.000000 antspymm-0.9.0/docs/ukbb_to_nrg_processing2.py
--rw-r--r--   0 stnava     (501) staff       (20)       38 2023-04-20 13:41:02.797845 antspymm-0.9.0/setup.cfg
--rw-r--r--   0 stnava     (501) staff       (20)      681 2023-04-20 13:39:29.000000 antspymm-0.9.0/setup.py
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-04-20 13:41:02.797260 antspymm-0.9.0/tests/
--rw-r--r--   0 stnava     (501) staff       (20)     5589 2022-10-21 12:35:02.000000 antspymm-0.9.0/tests/mm.py
--rw-r--r--   0 stnava     (501) staff       (20)     2087 2022-12-17 20:51:01.000000 antspymm-0.9.0/tests/mm_nrg.py
--rw-r--r--   0 stnava     (501) staff       (20)      440 2023-03-15 12:39:26.000000 antspymm-0.9.0/tests/test_bids_2_nrg.py
--rw-r--r--   0 stnava     (501) staff       (20)      394 2022-06-09 14:57:05.000000 antspymm-0.9.0/tests/test_dti_recon.py
--rw-r--r--   0 stnava     (501) staff       (20)     2507 2023-02-05 20:18:30.000000 antspymm-0.9.0/tests/test_dwi_run.py
--rw-r--r--   0 stnava     (501) staff       (20)      445 2023-02-05 00:06:28.000000 antspymm-0.9.0/tests/test_flair_run.py
--rw-r--r--   0 stnava     (501) staff       (20)     2618 2023-02-20 13:16:33.000000 antspymm-0.9.0/tests/test_joint_dti_recon.py
--rw-r--r--   0 stnava     (501) staff       (20)     1497 2023-03-15 12:44:41.000000 antspymm-0.9.0/tests/test_mm_csv.py
--rw-r--r--   0 stnava     (501) staff       (20)     2101 2022-11-16 16:52:51.000000 antspymm-0.9.0/tests/test_rsfmri_run.py
--rw-r--r--   0 stnava     (501) staff       (20)      597 2021-11-02 19:50:00.000000 antspymm-0.9.0/tests/testsr.py
--rw-r--r--   0 stnava     (501) staff       (20)     1439 2023-03-02 15:01:53.000000 antspymm-0.9.0/tests/visualize_tractogram.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-02 15:03:01.606745 antspymm-0.9.1/
+-rw-r--r--   0 stnava     (501) staff       (20)    11357 2021-11-01 09:20:32.000000 antspymm-0.9.1/LICENSE
+-rw-r--r--   0 stnava     (501) staff       (20)       33 2023-01-29 13:38:57.000000 antspymm-0.9.1/MANIFEST.in
+-rw-r--r--   0 stnava     (501) staff       (20)    10184 2023-05-02 15:03:01.606494 antspymm-0.9.1/PKG-INFO
+-rw-r--r--   0 stnava     (501) staff       (20)     9827 2023-04-12 13:23:21.000000 antspymm-0.9.1/README.md
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-02 15:03:01.588075 antspymm-0.9.1/antspymm/
+-rw-r--r--   0 stnava     (501) staff       (20)     2690 2023-03-20 11:54:16.000000 antspymm-0.9.1/antspymm/__init__.py
+-rw-r--r--   0 stnava     (501) staff       (20)   284731 2023-05-02 11:53:10.000000 antspymm-0.9.1/antspymm/mm.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-02 15:03:01.590417 antspymm-0.9.1/antspymm.egg-info/
+-rw-r--r--   0 stnava     (501) staff       (20)    10184 2023-05-02 15:03:01.000000 antspymm-0.9.1/antspymm.egg-info/PKG-INFO
+-rw-r--r--   0 stnava     (501) staff       (20)      763 2023-05-02 15:03:01.000000 antspymm-0.9.1/antspymm.egg-info/SOURCES.txt
+-rw-r--r--   0 stnava     (501) staff       (20)        1 2023-05-02 15:03:01.000000 antspymm-0.9.1/antspymm.egg-info/dependency_links.txt
+-rw-r--r--   0 stnava     (501) staff       (20)        1 2023-05-02 15:03:01.000000 antspymm-0.9.1/antspymm.egg-info/not-zip-safe
+-rw-r--r--   0 stnava     (501) staff       (20)      112 2023-05-02 15:03:01.000000 antspymm-0.9.1/antspymm.egg-info/requires.txt
+-rw-r--r--   0 stnava     (501) staff       (20)        9 2023-05-02 15:03:01.000000 antspymm-0.9.1/antspymm.egg-info/top_level.txt
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-02 15:03:01.601325 antspymm-0.9.1/docs/
+-rw-r--r--   0 stnava     (501) staff       (20)  1939802 2023-01-29 13:48:53.000000 antspymm-0.9.1/docs/antspymm_data_dictionary.csv
+-rw-r--r--   0 stnava     (501) staff       (20)      567 2023-04-12 13:06:30.000000 antspymm-0.9.1/docs/bids_cohort_example.py
+-rw-r--r--   0 stnava     (501) staff       (20)     1296 2023-04-08 18:52:17.000000 antspymm-0.9.1/docs/example_run_from_directory.py
+-rw-r--r--   0 stnava     (501) staff       (20)      478 2023-02-19 10:57:50.000000 antspymm-0.9.1/docs/make_dict_table.Rmd
+-rw-r--r--   0 stnava     (501) staff       (20)      632 2023-04-12 13:06:30.000000 antspymm-0.9.1/docs/nrg_cohort_example.py
+-rw-r--r--   0 stnava     (501) staff       (20)     2082 2023-03-20 13:00:28.000000 antspymm-0.9.1/docs/outlierness.py
+-rw-r--r--   0 stnava     (501) staff       (20)     3643 2023-04-15 22:47:31.000000 antspymm-0.9.1/docs/ukbb_to_nrg_processing.py
+-rw-r--r--   0 stnava     (501) staff       (20)     4546 2023-04-16 12:24:12.000000 antspymm-0.9.1/docs/ukbb_to_nrg_processing2.py
+-rw-r--r--   0 stnava     (501) staff       (20)       38 2023-05-02 15:03:01.606801 antspymm-0.9.1/setup.cfg
+-rw-r--r--   0 stnava     (501) staff       (20)      681 2023-05-02 11:55:31.000000 antspymm-0.9.1/setup.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-05-02 15:03:01.605975 antspymm-0.9.1/tests/
+-rw-r--r--   0 stnava     (501) staff       (20)     5589 2022-10-21 12:35:02.000000 antspymm-0.9.1/tests/mm.py
+-rw-r--r--   0 stnava     (501) staff       (20)     2087 2022-12-17 20:51:01.000000 antspymm-0.9.1/tests/mm_nrg.py
+-rw-r--r--   0 stnava     (501) staff       (20)      440 2023-03-15 12:39:26.000000 antspymm-0.9.1/tests/test_bids_2_nrg.py
+-rw-r--r--   0 stnava     (501) staff       (20)      394 2022-06-09 14:57:05.000000 antspymm-0.9.1/tests/test_dti_recon.py
+-rw-r--r--   0 stnava     (501) staff       (20)     1500 2023-05-01 14:47:40.000000 antspymm-0.9.1/tests/test_dti_reg.py
+-rw-r--r--   0 stnava     (501) staff       (20)     2507 2023-02-05 20:18:30.000000 antspymm-0.9.1/tests/test_dwi_run.py
+-rw-r--r--   0 stnava     (501) staff       (20)      445 2023-02-05 00:06:28.000000 antspymm-0.9.1/tests/test_flair_run.py
+-rw-r--r--   0 stnava     (501) staff       (20)     3368 2023-05-02 12:19:49.000000 antspymm-0.9.1/tests/test_joint_dti_recon.py
+-rw-r--r--   0 stnava     (501) staff       (20)     1497 2023-03-15 12:44:41.000000 antspymm-0.9.1/tests/test_mm_csv.py
+-rw-r--r--   0 stnava     (501) staff       (20)     2101 2022-11-16 16:52:51.000000 antspymm-0.9.1/tests/test_rsfmri_run.py
+-rw-r--r--   0 stnava     (501) staff       (20)      597 2021-11-02 19:50:00.000000 antspymm-0.9.1/tests/testsr.py
+-rw-r--r--   0 stnava     (501) staff       (20)     1439 2023-03-02 15:01:53.000000 antspymm-0.9.1/tests/visualize_tractogram.py
```

### Comparing `antspymm-0.9.0/LICENSE` & `antspymm-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.0/PKG-INFO` & `antspymm-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antspymm
-Version: 0.9.0
+Version: 0.9.1
 Summary: multi-channel/time-series medical image processing with antspyx
 Home-page: https://github.com/stnava/ANTsPyMM
 Author: Avants, Gosselin, Tustison, Reardon
 Author-email: stnava@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE
```

### Comparing `antspymm-0.9.0/README.md` & `antspymm-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.0/antspymm/__init__.py` & `antspymm-0.9.1/antspymm/__init__.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.0/antspymm/mm.py` & `antspymm-0.9.1/antspymm/mm.py`

 * *Files 0% similar despite different names*

```diff
@@ -980,27 +980,28 @@
     for k in range( nTimePoints):
         if verbose and ( ( k % counter ) ==  0 ) or ( k == (nTimePoints-1) ):
             myperc = round( k / nTimePoints * 100)
             print(myperc, end="%.", flush=True)
         temp = ants.slice_image(image, axis=idim - 1, idx=k)
         temp = ants.n4_bias_field_correction( temp )
         temp = ants.iMath(temp, "Normalize")
+        txprefix = ofnL+str(k % 2).zfill(4)+"_"
         if temp.numpy().var() > 0:
             myrig = ants.registration(
                     avg_b0, temp,
                     type_of_transform='BOLDRigid',
-                    outprefix=ofnL+str(k).zfill(4)+"_"
+                    outprefix=txprefix
                 )
             if type_of_transform == 'SyN':
                 myreg = ants.registration(
                     avg_b0, temp,
                     type_of_transform='SyNOnly',
                     total_sigma=total_sigma,
                     initial_transform=myrig['fwdtransforms'][0],
-                    outprefix=ofnL+str(k).zfill(4)+"_",
+                    outprefix=txprefix,
                     **kwargs
                 )
             else:
                 myreg = myrig
             fdptsTxI = ants.apply_transforms_to_points(
                 idim - 1, fdpts, myrig["fwdtransforms"]
             )
@@ -1012,15 +1013,14 @@
                 fdptsTxIminus1 = fdptsTxI
             # take the absolute value, then the mean across columns, then the sum
             FD[k] = (fdptsTxIminus1 - fdptsTxI).abs().mean().sum()
             motion_parameters.append(myreg["fwdtransforms"])
         else:
             motion_parameters.append("NA")
 
-    for k in range(nTimePoints):
         temp = ants.slice_image(image, axis=idim - 1, idx=k)
         if temp.numpy().var() > 0:
             img1w = ants.apply_transforms( avg_b0,
                 temp,
                 motion_parameters[k] )
             motion_corrected.append(img1w)
         else:
@@ -1246,42 +1246,65 @@
         mycols = list("xyz")
     useinds = list()
     for k in range(myoffsets.shape[0]):
         if abs(myoffsets[k, :]).sum() == (idim - 2):
             useinds.append(k)
         myoffsets[k, :] = myoffsets[k, :] * fdOffset / 2.0 + centerOfMass
     fdpts = pd.DataFrame(data=myoffsets[useinds, :], columns=mycols)
+
+
+    if verbose:
+        print("begin global distortion correction")
+    # initrig = tra_initializer(avg_b0, ab0, max_rotation=60, transform=['rigid'], verbose=verbose)
+    if mask_csf:
+        bcsf = ants.threshold_image( avg_b0,"Otsu",2).threshold_image(1,1).morphology("open",1).iMath("GetLargestComponent")
+    else:
+        bcsf = avg_b0[0] * 0 + 1
+
+    initrig = ants.registration( avg_b0, ab0*bcsf,'BOLDRigid',outprefix=ofnG)
+    deftx = ants.registration( avg_dwi, adw*bcsf, 'SyNOnly',
+        syn_metric='CC', syn_sampling=2,
+        reg_iterations=[50,50,20],
+        multivariate_extras=[ [ "CC", avg_b0, ab0*bcsf, 1, 2 ]],
+        initial_transform=initrig['fwdtransforms'][0],
+        outprefix=ofnG
+        )['fwdtransforms']
+    if verbose:
+        print("end global distortion correction")
+
     if verbose:
         print("Progress:")
     counter = round( nTimePoints / 10 )
     for k in range(nTimePoints):
         if verbose and ( ( k % counter ) ==  0 ) or ( k == (nTimePoints-1) ):
             myperc = round( k / nTimePoints * 100)
             print(myperc, end="%.", flush=True)
         if k in b0_idx:
             fixed=ants.image_clone( ab0 )
         else:
             fixed=ants.image_clone( adw )
         temp = ants.slice_image(image, axis=idim - 1, idx=k)
         temp = ants.n4_bias_field_correction( temp )
         temp = ants.iMath(temp, "Normalize")
+        txprefix = ofnL+str(k).zfill(4)+"rig_"
+        txprefix2 = ofnL+str(k % 2).zfill(4)+"def_"
         if temp.numpy().var() > 0:
             myrig = ants.registration(
                     fixed, temp,
                     type_of_transform='BOLDRigid',
-                    outprefix=ofnL+str(k).zfill(4)+"_",
+                    outprefix=txprefix,
                     **kwargs
                 )
             if type_of_transform == 'SyN':
                 myreg = ants.registration(
                     fixed, temp,
                     type_of_transform='SyNOnly',
                     total_sigma=total_sigma, grad_step=0.1,
                     initial_transform=myrig['fwdtransforms'][0],
-                    outprefix=ofnL+str(k).zfill(4)+"_",
+                    outprefix=txprefix2,
                     **kwargs
                 )
             else:
                 myreg = myrig
             fdptsTxI = ants.apply_transforms_to_points(
                 idim - 1, fdpts, myrig["fwdtransforms"]
             )
@@ -1293,34 +1316,14 @@
                 fdptsTxIminus1 = fdptsTxI
             # take the absolute value, then the mean across columns, then the sum
             FD[k] = (fdptsTxIminus1 - fdptsTxI).abs().mean().sum()
             motion_parameters.append(myreg["fwdtransforms"])
         else:
             motion_parameters.append("NA")
 
-    if verbose:
-        print("begin global distortion correction")
-    # initrig = tra_initializer(avg_b0, ab0, max_rotation=60, transform=['rigid'], verbose=verbose)
-    if mask_csf:
-        bcsf = ants.threshold_image( avg_b0,"Otsu",2).threshold_image(1,1).morphology("open",1).iMath("GetLargestComponent")
-    else:
-        bcsf = avg_b0[0] * 0 + 1
-
-    initrig = ants.registration( avg_b0, ab0*bcsf,'BOLDRigid',outprefix=ofnG)
-    deftx = ants.registration( avg_dwi, adw*bcsf, 'SyNOnly',
-        syn_metric='CC', syn_sampling=2,
-        reg_iterations=[50,50,20],
-        multivariate_extras=[ [ "CC", avg_b0, ab0*bcsf, 1, 2 ]],
-        initial_transform=initrig['fwdtransforms'][0],
-        outprefix=ofnG
-        )['fwdtransforms']
-    if verbose:
-        print("end global distortion correction")
-
-    for k in range(nTimePoints):
         temp = ants.slice_image(image, axis=idim - 1, idx=k)
         if k in b0_idx:
             fixed=ants.image_clone( ab0 )
         else:
             fixed=ants.image_clone( adw )
         if temp.numpy().var() > 0:
             motion_parameters[k]=deftx+motion_parameters[k]
```

### Comparing `antspymm-0.9.0/antspymm.egg-info/PKG-INFO` & `antspymm-0.9.1/antspymm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antspymm
-Version: 0.9.0
+Version: 0.9.1
 Summary: multi-channel/time-series medical image processing with antspyx
 Home-page: https://github.com/stnava/ANTsPyMM
 Author: Avants, Gosselin, Tustison, Reardon
 Author-email: stnava@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE
```

### Comparing `antspymm-0.9.0/antspymm.egg-info/SOURCES.txt` & `antspymm-0.9.1/antspymm.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 docs/outlierness.py
 docs/ukbb_to_nrg_processing.py
 docs/ukbb_to_nrg_processing2.py
 tests/mm.py
 tests/mm_nrg.py
 tests/test_bids_2_nrg.py
 tests/test_dti_recon.py
+tests/test_dti_reg.py
 tests/test_dwi_run.py
 tests/test_flair_run.py
 tests/test_joint_dti_recon.py
 tests/test_mm_csv.py
 tests/test_rsfmri_run.py
 tests/testsr.py
 tests/visualize_tractogram.py
```

### Comparing `antspymm-0.9.0/docs/antspymm_data_dictionary.csv` & `antspymm-0.9.1/docs/antspymm_data_dictionary.csv`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.0/docs/bids_cohort_example.py` & `antspymm-0.9.1/docs/bids_cohort_example.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.0/docs/example_run_from_directory.py` & `antspymm-0.9.1/docs/example_run_from_directory.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.0/docs/nrg_cohort_example.py` & `antspymm-0.9.1/docs/nrg_cohort_example.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.0/docs/outlierness.py` & `antspymm-0.9.1/docs/outlierness.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.0/docs/ukbb_to_nrg_processing.py` & `antspymm-0.9.1/docs/ukbb_to_nrg_processing.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.0/docs/ukbb_to_nrg_processing2.py` & `antspymm-0.9.1/docs/ukbb_to_nrg_processing2.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.0/setup.py` & `antspymm-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 long_description = open("README.md").read()
 
 with open("./requirements.txt") as f:
       requirements = f.read().splitlines()
 
 setup(name='antspymm',
-      version='0.9.0',
+      version='0.9.1',
       description='multi-channel/time-series medical image processing with antspyx',
       long_description=long_description,
       long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
       url='https://github.com/stnava/ANTsPyMM',
       author='Avants, Gosselin, Tustison, Reardon',
       author_email='stnava@gmail.com',
       license='Apache 2.0',
```

### Comparing `antspymm-0.9.0/tests/mm.py` & `antspymm-0.9.1/tests/mm.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.0/tests/mm_nrg.py` & `antspymm-0.9.1/tests/mm_nrg.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.0/tests/test_dwi_run.py` & `antspymm-0.9.1/tests/test_dwi_run.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.0/tests/test_joint_dti_recon.py` & `antspymm-0.9.1/tests/test_joint_dti_recon.py`

 * *Files 14% similar despite different names*

```diff
@@ -68,7 +68,31 @@
         verbose = True )
 
 if True:
     ants.image_write( myoutx['recon_fa'], '/tmp/temp1fa.nii.gz'  )
     ants.image_write( myoutx['recon_md'], '/tmp/temp1md.nii.gz'  )
     ants.image_write( myoutx['dwi_LR_dewarped'], '/tmp/temp1moco.nii.gz'  )
     ants.image_write( myoutx['dtrecon_LR_dewarp']['RGB'], '/tmp/temp1rgb.nii.gz'  )
+
+
+myoutx = antspymm.joint_dti_recon(
+        img_LR_in,
+        img_LR_bval,
+        img_LR_bvec,
+        jhu_atlas = JHU_atlas,
+        jhu_labels = JHU_labels,
+        reference_B0=btpB0,
+        reference_DWI=btpDW,
+        srmodel = None,
+        img_RL = img_RL_in,
+        bval_RL = img_RL_bval,
+        bvec_RL = img_RL_bvec,
+        motion_correct = 'SyN',
+        brain_mask = mask,
+        denoise = False,
+        verbose = True )
+
+if True:
+    ants.image_write( myoutx['recon_fa'], '/tmp/temp1fas.nii.gz'  )
+    ants.image_write( myoutx['recon_md'], '/tmp/temp1mds.nii.gz'  )
+    ants.image_write( myoutx['dwi_LR_dewarped'], '/tmp/temp1mocos.nii.gz'  )
+    ants.image_write( myoutx['dtrecon_LR_dewarp']['RGB'], '/tmp/temp1rgbs.nii.gz'  )
```

### Comparing `antspymm-0.9.0/tests/test_mm_csv.py` & `antspymm-0.9.1/tests/test_mm_csv.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.0/tests/test_rsfmri_run.py` & `antspymm-0.9.1/tests/test_rsfmri_run.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.0/tests/testsr.py` & `antspymm-0.9.1/tests/testsr.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.9.0/tests/visualize_tractogram.py` & `antspymm-0.9.1/tests/visualize_tractogram.py`

 * *Files identical despite different names*

