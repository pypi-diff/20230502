# Comparing `tmp/openneurofirstlevel-0.1.tar.gz` & `tmp/openneurofirstlevel-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openneurofirstlevel-0.1.tar", last modified: Wed Apr 19 15:21:46 2023, max compression
+gzip compressed data, was "openneurofirstlevel-0.2.tar", last modified: Tue May  2 15:40:04 2023, max compression
```

## Comparing `openneurofirstlevel-0.1.tar` & `openneurofirstlevel-0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-04-19 15:21:46.181371 openneurofirstlevel-0.1/
--rw-rw-r--   0 paul      (1000) paul      (1000)      196 2023-04-19 15:21:46.181371 openneurofirstlevel-0.1/PKG-INFO
--rw-rw-r--   0 paul      (1000) paul      (1000)     1775 2023-04-13 17:04:22.000000 openneurofirstlevel-0.1/README.md
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-04-19 15:21:46.181371 openneurofirstlevel-0.1/openneuro_firstlevel/
--rw-rw-r--   0 paul      (1000) paul      (1000)      134 2023-04-13 17:04:22.000000 openneurofirstlevel-0.1/openneuro_firstlevel/__init__.py
--rw-rw-r--   0 paul      (1000) paul      (1000)     1460 2023-04-13 17:04:22.000000 openneurofirstlevel-0.1/openneuro_firstlevel/dataset_designs.py
--rw-rw-r--   0 paul      (1000) paul      (1000)     3313 2023-04-13 17:04:22.000000 openneurofirstlevel-0.1/openneuro_firstlevel/diagnostics.py
--rw-rw-r--   0 paul      (1000) paul      (1000)    11725 2023-04-19 14:43:55.000000 openneurofirstlevel-0.1/openneuro_firstlevel/first_level.py
--rw-rw-r--   0 paul      (1000) paul      (1000)     2236 2023-04-13 17:04:22.000000 openneurofirstlevel-0.1/openneuro_firstlevel/second_level.py
--rw-rw-r--   0 paul      (1000) paul      (1000)     3911 2023-04-19 14:21:23.000000 openneurofirstlevel-0.1/openneuro_firstlevel/utils.py
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-04-19 15:21:46.181371 openneurofirstlevel-0.1/openneurofirstlevel.egg-info/
--rw-rw-r--   0 paul      (1000) paul      (1000)      196 2023-04-19 15:21:46.000000 openneurofirstlevel-0.1/openneurofirstlevel.egg-info/PKG-INFO
--rw-rw-r--   0 paul      (1000) paul      (1000)      444 2023-04-19 15:21:46.000000 openneurofirstlevel-0.1/openneurofirstlevel.egg-info/SOURCES.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)        1 2023-04-19 15:21:46.000000 openneurofirstlevel-0.1/openneurofirstlevel.egg-info/dependency_links.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)       57 2023-04-19 15:21:46.000000 openneurofirstlevel-0.1/openneurofirstlevel.egg-info/requires.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)       21 2023-04-19 15:21:46.000000 openneurofirstlevel-0.1/openneurofirstlevel.egg-info/top_level.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)       38 2023-04-19 15:21:46.181371 openneurofirstlevel-0.1/setup.cfg
--rw-rw-r--   0 paul      (1000) paul      (1000)      324 2023-04-19 15:17:54.000000 openneurofirstlevel-0.1/setup.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-02 15:40:04.243363 openneurofirstlevel-0.2/
+-rw-r--r--   0 paul       (501) staff       (20)      115 2023-05-02 15:40:04.243122 openneurofirstlevel-0.2/PKG-INFO
+-rw-r--r--   0 paul       (501) staff       (20)     1773 2023-05-01 21:42:34.000000 openneurofirstlevel-0.2/README.md
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-02 15:40:04.241547 openneurofirstlevel-0.2/openneuro_firstlevel/
+-rw-r--r--   0 paul       (501) staff       (20)      134 2023-04-19 15:31:13.000000 openneurofirstlevel-0.2/openneuro_firstlevel/__init__.py
+-rw-r--r--   0 paul       (501) staff       (20)     1519 2023-05-01 21:17:23.000000 openneurofirstlevel-0.2/openneuro_firstlevel/dataset_designs.py
+-rw-r--r--   0 paul       (501) staff       (20)     3323 2023-05-01 21:17:23.000000 openneurofirstlevel-0.2/openneuro_firstlevel/diagnostics.py
+-rw-r--r--   0 paul       (501) staff       (20)    11864 2023-05-02 15:26:10.000000 openneurofirstlevel-0.2/openneuro_firstlevel/first_level.py
+-rw-r--r--   0 paul       (501) staff       (20)     2333 2023-05-01 21:17:23.000000 openneurofirstlevel-0.2/openneuro_firstlevel/second_level.py
+-rw-r--r--   0 paul       (501) staff       (20)     3748 2023-05-01 21:17:23.000000 openneurofirstlevel-0.2/openneuro_firstlevel/utils.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-05-02 15:40:04.242791 openneurofirstlevel-0.2/openneurofirstlevel.egg-info/
+-rw-r--r--   0 paul       (501) staff       (20)      115 2023-05-02 15:40:04.000000 openneurofirstlevel-0.2/openneurofirstlevel.egg-info/PKG-INFO
+-rw-r--r--   0 paul       (501) staff       (20)      444 2023-05-02 15:40:04.000000 openneurofirstlevel-0.2/openneurofirstlevel.egg-info/SOURCES.txt
+-rw-r--r--   0 paul       (501) staff       (20)        1 2023-05-02 15:40:04.000000 openneurofirstlevel-0.2/openneurofirstlevel.egg-info/dependency_links.txt
+-rw-r--r--   0 paul       (501) staff       (20)       57 2023-05-02 15:40:04.000000 openneurofirstlevel-0.2/openneurofirstlevel.egg-info/requires.txt
+-rw-r--r--   0 paul       (501) staff       (20)       21 2023-05-02 15:40:04.000000 openneurofirstlevel-0.2/openneurofirstlevel.egg-info/top_level.txt
+-rw-r--r--   0 paul       (501) staff       (20)       38 2023-05-02 15:40:04.243440 openneurofirstlevel-0.2/setup.cfg
+-rw-r--r--   0 paul       (501) staff       (20)      365 2023-05-02 15:39:52.000000 openneurofirstlevel-0.2/setup.py
```

### Comparing `openneurofirstlevel-0.1/README.md` & `openneurofirstlevel-0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # openneurofirstlevel
-This repo contains code for running first-level GLMs on OpenNeuro datasets. Much of the code has been repurposed from the nilearn package. The variance inflation factor code was adapted from code written by Jeanette Mumford. 
+This repo contains code for running first-level GLMs on OpenNeuro datasets. Much of the code has been repurposed from the nilearn package. The variance inflation factor code was adapted from code written by Jeanette Mumford.
 
 ## Analysis Notes
 HRF model: SPM (difference of two gamma functions) <br>
 Drift model: DCT basis set, high-pass filter cutoff = 0.1Hz <br>
 Noise model: AR(1) <br>
 Spatial smoothing: None <br>
 Confound regressors: head motion/translation + derivatives, average power in WM mask and CSF mask (14 confounds total). All are demeaned. <br>
@@ -17,8 +17,8 @@
 - For each task:
     - Design matrix (.png and .csv file)
     - The model residuals (.nii.gz file)
     - Contrast map for each contrast (z-scores, image file with a z-score=2 plotting cutoff and a .nii.gz file)
     - Diagnostics: variance inflation factor (VIF) calculated for each contrast
 
 ## Analysis scripts and example outputs
-Eventually this repo will have an analysis script for each dataset that was processed. For now, see example.py for a generic processing pipeline. See also example_design_matrix.png and example_statmap.png generated for one subject from this dataset. 
+Eventually this repo will have an analysis script for each dataset that was processed. For now, see example.py for a generic processing pipeline. See also example_design_matrix.png and example_statmap.png generated for one subject from this dataset.
```

### Comparing `openneurofirstlevel-0.1/openneuro_firstlevel/dataset_designs.py` & `openneurofirstlevel-0.2/openneuro_firstlevel/dataset_designs.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,32 +4,56 @@
 import pdb
 
 from nilearn.glm.first_level.design_matrix import make_first_level_design_matrix
 
 from .utils import _get_frame_times, _add_parametric_modulation
 
 
-
-def make_ds001734_design(img, events, confounds,
-                         slice_time_ref, t_r, min_onset,
-                         hrf_model, drift_model, high_pass,
-                         rt_column):
+def make_ds001734_design(
+    img,
+    events,
+    confounds,
+    slice_time_ref,
+    t_r,
+    min_onset,
+    hrf_model,
+    drift_model,
+    high_pass,
+    rt_column,
+):
     frame_times = _get_frame_times(img, confounds, t_r, slice_time_ref)
-    regressors = _add_parametric_modulation(confounds, rt_column, events, frame_times,
-                                            hrf_model, drift_model, high_pass, min_onset)
-    add_cols = ['gain', 'loss']
+    regressors = _add_parametric_modulation(
+        confounds,
+        rt_column,
+        events,
+        frame_times,
+        hrf_model,
+        drift_model,
+        high_pass,
+        min_onset,
+    )
+    add_cols = ["gain", "loss"]
     for col in add_cols:
-        col_label = f'{col}_centered'
+        col_label = f"{col}_centered"
         events[col_label] = events[col] - events[col].mean()
-        regressors = _add_parametric_modulation(regressors, col_label, events, frame_times,
-                                                hrf_model, drift_model, high_pass, min_onset)
+        regressors = _add_parametric_modulation(
+            regressors,
+            col_label,
+            events,
+            frame_times,
+            hrf_model,
+            drift_model,
+            high_pass,
+            min_onset,
+        )
 
     design_matrix = make_first_level_design_matrix(
         frame_times,
-        events=events[['onset', 'duration']],
+        events=events[["onset", "duration"]],
         hrf_model=hrf_model,
         drift_model=drift_model,
         high_pass=high_pass,
         min_onset=min_onset,
-        add_regs=regressors)
-    design_matrix = design_matrix.drop(columns=['dummy'])
+        add_regs=regressors,
+    )
+    design_matrix = design_matrix.drop(columns=["dummy"])
     return design_matrix
```

### Comparing `openneurofirstlevel-0.1/openneuro_firstlevel/diagnostics.py` & `openneurofirstlevel-0.2/openneuro_firstlevel/diagnostics.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,67 +8,75 @@
 import numpy as np
 from statsmodels.stats.outliers_influence import variance_inflation_factor
 import statsmodels.api as sm
 from scipy.stats import norm
 from scipy.linalg import null_space
 
 
-
 def est_vif(design_matrix):
     vif_data = pd.DataFrame()
-    vif_data['regressor'] = design_matrix.columns.drop('constant')
-    vif_data['VIF'] = [variance_inflation_factor(design_matrix.values, i)
-                       for i, col in enumerate(design_matrix.columns) if col != 'constant']
+    vif_data["regressor"] = design_matrix.columns.drop("constant")
+    vif_data["VIF"] = [
+        variance_inflation_factor(design_matrix.values, i)
+        for i, col in enumerate(design_matrix.columns)
+        if col != "constant"
+    ]
     return vif_data
 
+
 def est_contrast_vif(desmat, contrast, contrast_label):
-    '''
+    """
     The goal of this function is to estimate a variance inflation factor for a contrast.
     This is done by extending the effective regressor definition from Smith et al (2007)
     Meaningful design and contrast estimability (NeuroImage).  Regressors involved
     in the contrast estimate are rotated to span the same space as the original space
-    consisting of the effective regressor and and an orthogonal basis.  The rest of the 
+    consisting of the effective regressor and and an orthogonal basis.  The rest of the
     regressors are unchanged.
     input:
-        desmat: design matrix.  Assumed to be a pandas dataframe with column  
+        desmat: design matrix.  Assumed to be a pandas dataframe with column
              headings which are used define the contrast of interest
         contrast: a single contrast defined in string format
     output:
-        vif: a single VIF for the contrast of interest  
-    '''
+        vif: a single VIF for the contrast of interest
+    """
     des_nuisance_regs = desmat[desmat.columns[contrast == 0]]
     des_contrast_regs = desmat[desmat.columns[contrast != 0]]
 
     con = np.atleast_2d(contrast[contrast != 0])
     con2_t = null_space(con)
     x = des_contrast_regs.copy().values
     q = np.linalg.pinv(x.T @ x)
     f1 = np.linalg.pinv(con @ q @ con.T)
     pc = con.T @ f1 @ con @ q
     con3_t = con2_t - pc @ con2_t
     f3 = np.linalg.pinv(con3_t.T @ q @ con3_t)
     eff_reg = x @ q @ con.T @ f1
-    eff_reg = pd.DataFrame(eff_reg, columns = [contrast_label], index=desmat.index)
+    eff_reg = pd.DataFrame(eff_reg, columns=[contrast_label], index=desmat.index)
 
-    other_reg = x @ q @ con3_t @ f3 
-    other_reg_names = [f'orth_proj{val}' for val in range(other_reg.shape[1])]
-    other_reg = pd.DataFrame(other_reg, columns = other_reg_names, index=desmat.index)
+    other_reg = x @ q @ con3_t @ f3
+    other_reg_names = [f"orth_proj{val}" for val in range(other_reg.shape[1])]
+    other_reg = pd.DataFrame(other_reg, columns=other_reg_names, index=desmat.index)
 
-    des_for_vif = pd.concat([eff_reg, other_reg, des_nuisance_regs], axis = 1)
+    des_for_vif = pd.concat([eff_reg, other_reg, des_nuisance_regs], axis=1)
     vif_dat = est_vif(des_for_vif)
-    vif_dat.rename(columns={'regressor': 'contrast'}, inplace=True)
+    vif_dat.rename(columns={"regressor": "contrast"}, inplace=True)
     vif_output = vif_dat[vif_dat.contrast == contrast_label]
     # Also run regression on the design matrix to get stats on the coeffs.
-    #X_labels = des_for_vif.columns.difference([contrast_label])
-    #res = sm.OLS(des_for_vif[contrast_label], des_for_vif[X_labels]).fit()
-    return vif_output['VIF'].values[0]
-
-def est_all_contrast_vif(design_matrix, contrasts, contrast_labels, task_label, save_dir, run_ind):
-    vif_stats = {'contrast': [],
-                 'VIF': []}
+    # X_labels = des_for_vif.columns.difference([contrast_label])
+    # res = sm.OLS(des_for_vif[contrast_label], des_for_vif[X_labels]).fit()
+    return vif_output["VIF"].values[0]
+
+
+def est_all_contrast_vif(
+    design_matrix, contrasts, contrast_labels, task_label, save_dir, run_ind
+):
+    vif_stats = {"contrast": [], "VIF": []}
     for con, con_label in zip(contrasts, contrast_labels):
         vif_out = est_contrast_vif(design_matrix, con, con_label)
-        vif_stats['contrast'].append(con_label)
-        vif_stats['VIF'].append(vif_out)
+        vif_stats["contrast"].append(con_label)
+        vif_stats["VIF"].append(vif_out)
     vif_df = pd.DataFrame(vif_stats)
-    vif_df.to_csv(os.path.join(save_dir, f'task-{task_label}_run-{run_ind+1}_diagnostics.csv'), index=False)
+    vif_df.to_csv(
+        os.path.join(save_dir, f"task-{task_label}_run-{run_ind+1}_diagnostics.csv"),
+        index=False,
+    )
     return vif_df
```

### Comparing `openneurofirstlevel-0.1/openneuro_firstlevel/first_level.py` & `openneurofirstlevel-0.2/openneuro_firstlevel/first_level.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,206 +2,340 @@
 import os
 import json
 import glob
 
 import numpy as np
 import pandas as pd
 from nilearn.glm.first_level import first_level_from_bids, FirstLevelModel
-from nilearn.plotting import plot_design_matrix, plot_stat_map, plot_contrast_matrix, plot_glass_brain
+from nilearn.plotting import (
+    plot_design_matrix,
+    plot_stat_map,
+    plot_contrast_matrix,
+    plot_glass_brain,
+)
 from nilearn.interfaces.fmriprep import load_confounds
 from nilearn.interfaces.bids import get_bids_files
 from nilearn._utils.niimg_conversions import check_niimg
 from nilearn.image import get_data, concat_imgs, mean_img
 from nilearn.glm.first_level.design_matrix import make_first_level_design_matrix
 from nilearn.glm.contrasts import compute_fixed_effects
 import matplotlib.pyplot as plt
 
-from .utils import (filter_subjects, get_tr_slice_time_ref, _get_frame_times, 
-                    _add_parametric_modulation, combine_run_masks)
+from .utils import (
+    filter_subjects,
+    get_tr_slice_time_ref,
+    _get_frame_times,
+    _add_parametric_modulation,
+    combine_run_masks,
+)
 from .diagnostics import est_all_contrast_vif
 
 
-
 def get_contrasts(design_matrix, contrast_conditions):
     contrast_matrix = np.eye(design_matrix.shape[1])
-    single_contrasts = dict([(column, contrast_matrix[i])
-                            for i, column in enumerate(design_matrix.columns)])
-    contrasts = [single_contrasts[cc[0]] - single_contrasts[cc[1]]
-                 for cc in contrast_conditions]
+    single_contrasts = dict(
+        [(column, contrast_matrix[i]) for i, column in enumerate(design_matrix.columns)]
+    )
+    contrasts = [
+        single_contrasts[cc[0]] - single_contrasts[cc[1]] for cc in contrast_conditions
+    ]
     return contrasts
 
-def make_design_matrix(img, events, confounds,
-                       slice_time_ref, t_r, min_onset,
-                       hrf_model, drift_model, high_pass,
-                       rt_column):
+
+def make_design_matrix(
+    img,
+    events,
+    confounds,
+    slice_time_ref,
+    t_r,
+    min_onset,
+    hrf_model,
+    drift_model,
+    high_pass,
+    rt_column,
+):
     # Wrapper around nilearn make_first_level_design_matrix
     # that creates a design matrix with response time (RT) as a parametric
     # modulator in addition to the original unmodulated event regressors.
-    # For the RT regressor, the amplitude (but not duration) of 
+    # For the RT regressor, the amplitude (but not duration) of
     # each event is scaled by the RT (cite Jeanette's paper), and the regressor
-    # is not centered (demeaned). 
+    # is not centered (demeaned).
     frame_times = _get_frame_times(img, confounds, t_r, slice_time_ref)
-    confounds = _add_parametric_modulation(confounds, rt_column, events, frame_times,
-                                           hrf_model, drift_model, high_pass, min_onset)
+    confounds = _add_parametric_modulation(
+        confounds,
+        rt_column,
+        events,
+        frame_times,
+        hrf_model,
+        drift_model,
+        high_pass,
+        min_onset,
+    )
     # Create full design matrix with original unmodulated regressor
     # and RT-modulated regressor
     design_matrix = make_first_level_design_matrix(
         frame_times,
-        events=events[['onset', 'duration', 'trial_type']],
+        events=events[["onset", "duration", "trial_type"]],
         hrf_model=hrf_model,
         drift_model=drift_model,
         high_pass=high_pass,
         min_onset=min_onset,
-        add_regs=confounds)
+        add_regs=confounds,
+    )
     return design_matrix
 
-def fit_single_subject(subject_id, imgs, events, data_dir, derivatives_dir, 
-                       task_label, save_dir, min_onset=-24,
-                       standardize=False, signal_scaling=0, **kwargs):
+
+def fit_single_subject(
+    subject_id,
+    imgs,
+    events,
+    data_dir,
+    derivatives_dir,
+    task_label,
+    save_dir,
+    min_onset=-24,
+    standardize=False,
+    signal_scaling=0,
+    **kwargs,
+):
     n_runs = len(imgs)
     run_models, run_designs, run_masks = [], [], []
-    space_label = kwargs['space_label']
+    space_label = kwargs["space_label"]
     for run_ind in range(n_runs):
         run_imgs, run_events = imgs[run_ind], events[run_ind]
         if n_runs == 1:
-            mask_fn = f'sub-{subject_id}_task-{task_label}_space-{space_label}*mask.nii.gz'
+            mask_fn = (
+                f"sub-{subject_id}_task-{task_label}_space-{space_label}*mask.nii.gz"
+            )
         else:
-            mask_fn = f'sub-{subject_id}_task-{task_label}_run-{run_ind+1}_space-{space_label}*mask.nii.gz'
-        mask_img = glob.glob(os.path.join(
-            data_dir, derivatives_dir, f'sub-{subject_id}', 'func', mask_fn))[0]
+            mask_fn = f"sub-{subject_id}_task-{task_label}_run-{run_ind+1}_space-{space_label}*mask.nii.gz"
+        mask_img = glob.glob(
+            os.path.join(
+                data_dir, derivatives_dir, f"sub-{subject_id}", "func", mask_fn
+            )
+        )[0]
         run_masks.append(mask_img)
 
-        model = FirstLevelModel(t_r=kwargs['t_r'],
-                                slice_time_ref=kwargs['slice_time_ref'],
-                                hrf_model=kwargs['hrf_model'], 
-                                drift_model=kwargs['drift_model'],
-                                high_pass=kwargs['high_pass'], 
-                                mask_img=mask_img,
-                                smoothing_fwhm=kwargs['smoothing_fwhm'],
-                                noise_model=kwargs['noise_model'],
-                                min_onset=min_onset,
-                                standardize=standardize, 
-                                signal_scaling=signal_scaling,
-                                subject_label=subject_id,
-                                minimize_memory=False)
+        model = FirstLevelModel(
+            t_r=kwargs["t_r"],
+            slice_time_ref=kwargs["slice_time_ref"],
+            hrf_model=kwargs["hrf_model"],
+            drift_model=kwargs["drift_model"],
+            high_pass=kwargs["high_pass"],
+            mask_img=mask_img,
+            smoothing_fwhm=kwargs["smoothing_fwhm"],
+            noise_model=kwargs["noise_model"],
+            min_onset=min_onset,
+            standardize=standardize,
+            signal_scaling=signal_scaling,
+            subject_label=subject_id,
+            minimize_memory=False,
+        )
 
         # These parameters extract 6 basic head motion confounds + derivatives
         # and the average WM and CSF signal as confounds.
         # All confounds are demeaned. No scrubbing is done to remove
-        # high motion volumes. 
-        confounds, sample_mask = load_confounds(run_imgs,
-                                                strategy=('motion', 'wm_csf'),
-                                                motion='derivatives', wm_csf='basic',
-                                                demean=True)
-        run_events['duration'] = np.ones(len(run_events))  # Fix duration to 1s for all events
-        design_matrix_fn = (make_design_matrix if kwargs['design_function'] is None 
-                            else kwargs['design_function'])
-        design_matrix = design_matrix_fn(run_imgs, run_events, confounds,
-                                         kwargs['slice_time_ref'], 
-                                         kwargs['t_r'], min_onset,
-                                         kwargs['hrf_model'], 
-                                         kwargs['drift_model'], 
-                                         kwargs['high_pass'], 
-                                         kwargs['rt_column'])
+        # high motion volumes.
+        confounds, sample_mask = load_confounds(
+            run_imgs,
+            strategy=("motion", "wm_csf"),
+            motion="derivatives",
+            wm_csf="basic",
+            demean=True,
+        )
+        run_events["duration"] = np.ones(
+            len(run_events)
+        )  # Fix duration to 1s for all events
+        design_matrix_fn = (
+            make_design_matrix
+            if kwargs["design_function"] is None
+            else kwargs["design_function"]
+        )
+        design_matrix = design_matrix_fn(
+            run_imgs,
+            run_events,
+            confounds,
+            kwargs["slice_time_ref"],
+            kwargs["t_r"],
+            min_onset,
+            kwargs["hrf_model"],
+            kwargs["drift_model"],
+            kwargs["high_pass"],
+            kwargs["rt_column"],
+        )
         design_mat_fig = plot_design_matrix(design_matrix)
-        save_fn_base = f'task-{task_label}_run-{run_ind+1}'
-        plt.savefig(os.path.join(save_dir, f'{save_fn_base}_design_matrix.png'))
-        design_matrix.to_csv(os.path.join(save_dir, f'{save_fn_base}_design_matrix.csv'), 
-                             index_label=False)
+        save_fn_base = f"task-{task_label}_run-{run_ind+1}"
+        plt.savefig(os.path.join(save_dir, f"{save_fn_base}_design_matrix.png"))
+        design_matrix.to_csv(
+            os.path.join(save_dir, f"{save_fn_base}_design_matrix.csv"),
+            index_label=False,
+        )
         model.fit(run_imgs, design_matrices=design_matrix)
         run_models.append(model)
         run_designs.append(design_matrix)
         # Save residuals
-        res_path = os.path.join(save_dir, f'{save_fn_base}_residuals.nii.gz')
+        res_path = os.path.join(save_dir, f"{save_fn_base}_residuals.nii.gz")
         res = model.residuals[0]
         res.header.set_data_dtype(np.float32)
         res.to_filename(res_path)
     return run_models, run_designs, run_masks
 
-def analyze_contrasts(run_models, imgs, run_designs, run_masks, contrast_labels, 
-                      task_label, contrast_conditions, subject_id, z_thresh, save_dir):
-        contrasts = get_contrasts(run_designs[0], contrast_conditions)
-        n_runs = len(run_models)
-        # Not ideal to have two double for-loops, refactor
-        for run_ind in range(n_runs):
-            run_model, run_design, run_imgs = run_models[run_ind], run_designs[run_ind], imgs[run_ind]
-            est_all_contrast_vif(run_design, contrasts, contrast_labels, task_label, save_dir, run_ind)
 
-        for con_label, con in zip(contrast_labels, contrasts):
-            all_run_stats = []
-            for run_ind in range(n_runs):
-                save_label = f'task-{task_label}_run-{run_ind+1}_contrast-{con_label}'
-                run_model, run_design, run_imgs = run_models[run_ind], run_designs[run_ind], imgs[run_ind]
-                run_stats = run_model.compute_contrast(con, output_type='all')
-                all_run_stats.append(run_stats)
-                run_stats['z_score'].to_filename(os.path.join(save_dir, f'{save_label}_z_scores.nii.gz'))
-                z_fig = plt.figure(figsize=(12, 3))
-                bg_img = mean_img(concat_imgs(run_imgs))
-                plot_stat_map(run_stats['z_score'], threshold=z_thresh, bg_img=bg_img,
-                              display_mode='z', cut_coords=(-25, 0, 50), black_bg=True,
-                              figure=z_fig, title=f'{save_label}')
-                plt.savefig(os.path.join(save_dir, f'{save_label}_zstatmap.png'))
-                #plot_glass_brain(z_map, colorbar=True, threshold=norm.isf(0.001),
-                #                 title=f'Nilearn Z map of {label} (unc p<0.001)',
-                #                 plot_abs=False, display_mode='ortho')
-                #plt.savefig(os.path.join(save_dir, f'sub{subject_id}_{label}_glass_brain.png'))
-                #plot_contrast_matrix(con, design_matrix=design_matrix)
-                #plt.savefig(os.path.join(save_dir, f'task-{task_label}_contrast-{con_label}_contrast_matrix.png'))
-                plt.close('all')
-
-            if n_runs > 1:
-                # Compute precision-weighted run average fixed effect
-                combined_mask = combine_run_masks(run_masks)
-                combined_bg_img = mean_img(concat_imgs(imgs))
-                combine_runs(all_run_stats, save_dir, task_label, con_label, z_thresh, 
-                             combined_mask, combined_bg_img)
-
-def combine_runs(run_stats, save_dir, task_label, contrast_label, z_thresh, mask, bg_img):
-    save_label = f'task-{task_label}_run_avg_contrast-{contrast_label}'
-    contrast_imgs = [stats['effect_size'] for stats in run_stats]
-    variance_imgs = [stats['effect_variance'] for stats in run_stats]
+def analyze_contrasts(
+    run_models,
+    imgs,
+    run_designs,
+    run_masks,
+    contrast_labels,
+    task_label,
+    contrast_conditions,
+    subject_id,
+    z_thresh,
+    save_dir,
+):
+    contrasts = get_contrasts(run_designs[0], contrast_conditions)
+    n_runs = len(run_models)
+    # Not ideal to have two double for-loops, refactor
+    for run_ind in range(n_runs):
+        run_model, run_design, run_imgs = (
+            run_models[run_ind],
+            run_designs[run_ind],
+            imgs[run_ind],
+        )
+        est_all_contrast_vif(
+            run_design, contrasts, contrast_labels, task_label, save_dir, run_ind
+        )
+
+    for con_label, con in zip(contrast_labels, contrasts):
+        all_run_stats = []
+        for run_ind in range(n_runs):
+            save_label = f"task-{task_label}_run-{run_ind+1}_contrast-{con_label}"
+            run_model, run_design, run_imgs = (
+                run_models[run_ind],
+                run_designs[run_ind],
+                imgs[run_ind],
+            )
+            run_stats = run_model.compute_contrast(con, output_type="all")
+            all_run_stats.append(run_stats)
+            run_stats["z_score"].to_filename(
+                os.path.join(save_dir, f"{save_label}_z_scores.nii.gz")
+            )
+            z_fig = plt.figure(figsize=(12, 3))
+            bg_img = mean_img(concat_imgs(run_imgs))
+            plot_stat_map(
+                run_stats["z_score"],
+                threshold=z_thresh,
+                bg_img=bg_img,
+                display_mode="z",
+                cut_coords=(-25, 0, 50),
+                black_bg=True,
+                figure=z_fig,
+                title=f"{save_label}",
+            )
+            plt.savefig(os.path.join(save_dir, f"{save_label}_zstatmap.png"))
+            # plot_glass_brain(z_map, colorbar=True, threshold=norm.isf(0.001),
+            #                 title=f'Nilearn Z map of {label} (unc p<0.001)',
+            #                 plot_abs=False, display_mode='ortho')
+            # plt.savefig(os.path.join(save_dir, f'sub{subject_id}_{label}_glass_brain.png'))
+            # plot_contrast_matrix(con, design_matrix=design_matrix)
+            # plt.savefig(os.path.join(save_dir, f'task-{task_label}_contrast-{con_label}_contrast_matrix.png'))
+            plt.close("all")
+
+        if n_runs > 1:
+            # Compute precision-weighted run average fixed effect
+            combined_mask = combine_run_masks(run_masks)
+            combined_bg_img = mean_img(concat_imgs(imgs))
+            combine_runs(
+                all_run_stats,
+                save_dir,
+                task_label,
+                con_label,
+                z_thresh,
+                combined_mask,
+                combined_bg_img,
+            )
+
+
+def combine_runs(
+    run_stats, save_dir, task_label, contrast_label, z_thresh, mask, bg_img
+):
+    save_label = f"task-{task_label}_run_avg_contrast-{contrast_label}"
+    contrast_imgs = [stats["effect_size"] for stats in run_stats]
+    variance_imgs = [stats["effect_variance"] for stats in run_stats]
     fixed_fx_contrast, fixed_fx_variance, fixed_fx_stat = compute_fixed_effects(
-        contrast_imgs, variance_imgs, mask, precision_weighted=False)
-    fixed_fx_stat.to_filename(os.path.join(save_dir, f'{save_label}_t_scores.nii.gz'))
+        contrast_imgs, variance_imgs, mask, precision_weighted=False
+    )
+    fixed_fx_stat.to_filename(os.path.join(save_dir, f"{save_label}_t_scores.nii.gz"))
     plot_stat_map(
-        fixed_fx_stat, bg_img=bg_img, threshold=z_thresh, cut_coords=(-25, 0, 50),
-        display_mode='z', black_bg=True, title=f'{save_label}')
-    plt.savefig(os.path.join(save_dir, f'{save_label}_tstatmap.png'))
+        fixed_fx_stat,
+        bg_img=bg_img,
+        threshold=z_thresh,
+        cut_coords=(-25, 0, 50),
+        display_mode="z",
+        black_bg=True,
+        title=f"{save_label}",
+    )
+    plt.savefig(os.path.join(save_dir, f"{save_label}_tstatmap.png"))
+
 
 def run_first_level_analysis(data_dir, derivatives_dir, save_dir, **kwargs):
-    for task_label in kwargs['task_labels']:
-        if kwargs['t_r'] is None and kwargs['slice_time_ref'] is None:
-            t_r, slice_time_ref = get_tr_slice_time_ref(data_dir, derivatives_dir, 
-                                                        task_label,
-                                                        img_filters=kwargs['img_filters'])
-            kwargs['t_r'] = t_r
-            kwargs['slice_time_ref'] = slice_time_ref
-        # We use first_level_from_bids to get the image and event files,
+    for task_label in kwargs["task_labels"]:
+        if kwargs["t_r"] is None and kwargs["slice_time_ref"] is None:
+            t_r, slice_time_ref = get_tr_slice_time_ref(
+                data_dir, derivatives_dir, task_label, img_filters=kwargs["img_filters"]
+            )
+            kwargs["t_r"] = t_r
+            kwargs["slice_time_ref"] = slice_time_ref
+
+        # We use first_level_from_bids (nilearn) to get the image and event files,
         # but the model will be redefined with the appropriate mask image below
         # (subject-specific masks can't be passed to first_level_from_bids directly)
-        throwaway_models, models_run_imgs, models_events, _ = \
-            first_level_from_bids(data_dir, task_label, space_label=kwargs['space_label'],
-                                  slice_time_ref=kwargs['slice_time_ref'],
-                                  derivatives_folder=derivatives_dir,
-                                  img_filters=kwargs['img_filters'])
+        throwaway_models, models_run_imgs, models_events, _ = first_level_from_bids(
+            data_dir,
+            task_label,
+            space_label=kwargs["space_label"],
+            slice_time_ref=kwargs["slice_time_ref"],
+            derivatives_folder=derivatives_dir,
+            img_filters=kwargs["img_filters"],
+        )
         subject_labels = [m.subject_label for m in throwaway_models]
         all_subjects, all_imgs, all_events = filter_subjects(
-            subject_labels, models_run_imgs, models_events,
-            exclude_subjects=kwargs.get('exclude_subjects', None),
-            include_subjects=kwargs.get('include_subjects', None))
+            subject_labels,
+            models_run_imgs,
+            models_events,
+            exclude_subjects=kwargs.get("exclude_subjects", None),
+            include_subjects=kwargs.get("include_subjects", None),
+        )
+
         # Save list of included subjects
         subject_series = pd.Series(all_subjects)
-        subject_series.to_csv(os.path.join(save_dir, f'included_subjects.csv'), 
-                              index_label=False)
+        subject_series.to_csv(
+            os.path.join(save_dir, f"included_subjects.csv"), index_label=False
+        )
 
         # Fit model to each subject
         for sub, imgs, events in zip(all_subjects, all_imgs, all_events):
-            subject_save_dir = os.path.join(save_dir, f'sub-{sub}')
+            subject_save_dir = os.path.join(save_dir, f"sub-{sub}")
             os.makedirs(subject_save_dir, exist_ok=True)
             run_models, run_designs, run_masks = fit_single_subject(
-                sub, imgs, events, data_dir, derivatives_dir,
-                task_label, subject_save_dir, **kwargs)
-            analyze_contrasts(run_models, imgs, run_designs, 
-                              run_masks, kwargs['contrast_labels'], task_label,
-                              kwargs['contrast_conditions'], sub, 
-                              kwargs['z_thresh'], subject_save_dir)
-            plt.close('all')
+                sub,
+                imgs,
+                events,
+                data_dir,
+                derivatives_dir,
+                task_label,
+                subject_save_dir,
+                **kwargs,
+            )
+            analyze_contrasts(
+                run_models,
+                imgs,
+                run_designs,
+                run_masks,
+                kwargs["contrast_labels"],
+                task_label,
+                kwargs["contrast_conditions"],
+                sub,
+                kwargs["z_thresh"],
+                subject_save_dir,
+            )
+            plt.close("all")
```

### Comparing `openneurofirstlevel-0.1/openneuro_firstlevel/second_level.py` & `openneurofirstlevel-0.2/openneuro_firstlevel/second_level.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,47 +5,55 @@
 from nilearn import image
 from nilearn import plotting
 from nilearn.glm import threshold_stats_img
 from nilearn.glm.second_level import SecondLevelModel
 import matplotlib.pyplot as plt
 
 
-
-def run_second_level_analysis(save_dir, task_labels, contrast_labels, 
-                              contrast_conditions, n_runs):
+def run_second_level_analysis(
+    save_dir, task_labels, contrast_labels, contrast_conditions, n_runs
+):
     # Aggregate all first-level maps
-    subjects = pd.read_csv(os.path.join(save_dir, 'included_subjects.csv'))
+    subjects = pd.read_csv(os.path.join(save_dir, "included_subjects.csv"))
     for task_label in task_labels:
         for con_label, contrast in zip(contrast_labels, contrast_conditions):
-            save_label = f'task-{task_label}_contrast-{con_label}_second_level'
+            save_label = f"task-{task_label}_contrast-{con_label}_second_level"
             first_level_maps = []
             for sub in subjects:
-                sub_dir = os.path.join(save_dir, f'sub-{sub}') 
+                sub_dir = os.path.join(save_dir, f"sub-{sub}")
                 if n_runs == 1:
-                    map_fn = f'task-{task_label}_run-1_contrast-{con_label}_z_scores.nii.gz'
+                    map_fn = (
+                        f"task-{task_label}_run-1_contrast-{con_label}_z_scores.nii.gz"
+                    )
                 else:
-                    map_fn = f'task-{task_label}_run_avg_contrast-{con_label}_t_scores.nii.gz'
+                    map_fn = f"task-{task_label}_run_avg_contrast-{con_label}_t_scores.nii.gz"
                 first_level_maps.append(image.load_img(os.path.join(sub_dir, map_fn)))
 
             # Fit second-level model
             design_matrix = pd.DataFrame(
-                [1] * len(first_level_maps), columns=['intercept'])
+                [1] * len(first_level_maps), columns=["intercept"]
+            )
             second_level_model = SecondLevelModel(smoothing_fwhm=None)
             second_level_model = second_level_model.fit(
-                first_level_maps, design_matrix=design_matrix)
-            z_map = second_level_model.compute_contrast(output_type='z_score')
+                first_level_maps, design_matrix=design_matrix
+            )
+            z_map = second_level_model.compute_contrast(output_type="z_score")
             thresholded_map1, threshold1 = threshold_stats_img(
-                z_map, alpha=0.001, height_control='fpr',
-                cluster_threshold=10, two_sided=True)
+                z_map,
+                alpha=0.001,
+                height_control="fpr",
+                cluster_threshold=10,
+                two_sided=True,
+            )
 
             z_fig = plt.figure(figsize=(12, 3))
             plotting.plot_stat_map(
                 thresholded_map1,
                 cut_coords=(-25, 0, 50),
                 threshold=threshold1,
                 figure=z_fig,
                 title="Thresholded z map, fpr <.001, clusters > 10 voxels",
             )
-            
+
             # Save
-            plt.savefig(os.path.join(save_dir, f'{save_label}_zstatmap.png'))
-            z_map.to_filename(os.path.join(save_dir, f'{save_label}_z_scores.nii.gz'))
+            plt.savefig(os.path.join(save_dir, f"{save_label}_zstatmap.png"))
+            z_map.to_filename(os.path.join(save_dir, f"{save_label}_z_scores.nii.gz"))
```

### Comparing `openneurofirstlevel-0.1/openneuro_firstlevel/utils.py` & `openneurofirstlevel-0.2/openneuro_firstlevel/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,74 +6,96 @@
 from nilearn.interfaces.bids import get_bids_files
 from nilearn.image import get_data
 from nilearn.glm.first_level.design_matrix import make_first_level_design_matrix
 from nilearn._utils.niimg_conversions import check_niimg
 from nilearn.maskers import NiftiMasker
 
 
-
 def get_tr_slice_time_ref(data_dir, derivatives_dir, task_label, img_filters=None):
     # Get slice_time_ref and the TR from the fMRIprep metadata
     # If slice timing correction was not done, slice_time_ref = 0 (frame times will not be shifted)
     # If slice timing correction was done, slice_time_ref determined from fMRI-prep outputs:
     # frame times will be shifted by +slice_time_ref * TR (usually +TR/2)
-    # The filters are included to match the filters used internally by nilearn when 
+    # The filters are included to match the filters used internally by nilearn when
     # querying the fMRIprep metadata.
     derivatives_path = os.path.join(data_dir, derivatives_dir)
-    filters = [('task', task_label)]
+    filters = [("task", task_label)]
     if img_filters is not None:
         for img_filter in img_filters:
-            if img_filter[0] in ['acq', 'rec', 'run']:
+            if img_filter[0] in ["acq", "rec", "run"]:
                 filters.append(img_filter)
-    img_specs = get_bids_files(derivatives_path, modality_folder='func',
-                               file_tag='bold', file_type='json',
-                               filters=filters)
-    specs = json.load(open(img_specs[0], 'r'))
-    t_r = specs['RepetitionTime']
-    if specs['SliceTimingCorrected'] == False:
+    img_specs = get_bids_files(
+        derivatives_path,
+        modality_folder="func",
+        file_tag="bold",
+        file_type="json",
+        filters=filters,
+    )
+    specs = json.load(open(img_specs[0], "r"))
+    t_r = specs["RepetitionTime"]
+    if specs["SliceTimingCorrected"] == False:
         slice_time_ref = 0.0
     else:
-        slice_time_ref = specs['SliceTimingRef']
+        slice_time_ref = specs["SliceTimingRef"]
     return t_r, slice_time_ref
 
-def filter_subjects(subjects, imgs, events, exclude_subjects=None, include_subjects=None):
-    assert exclude_subjects == None or include_subjects == None, \
-        'Either exclude_subjects or include_subjects must be set to None!'
+
+def filter_subjects(
+    subjects, imgs, events, exclude_subjects=None, include_subjects=None
+):
+    assert (
+        exclude_subjects == None or include_subjects == None
+    ), "Either exclude_subjects or include_subjects must be set to None!"
     if include_subjects is not None:
         keep_idx = np.nonzero(np.isin(subjects, include_subjects))[0]
     elif exclude_subjects is not None:
         keep_idx = np.nonzero(~np.isin(subjects, exclude_subjects))[0]
     else:
         keep_idx = np.arange(len(subjects))
     keep_subjects = [sub for i, sub in enumerate(subjects) if i in keep_idx]
     keep_imgs = [img for i, img in enumerate(imgs) if i in keep_idx]
     keep_events = [event for i, event in enumerate(events) if i in keep_idx]
-    print(f'Excluding N={len(subjects) - len(keep_subjects)} subjects')
+    print(f"Excluding N={len(subjects) - len(keep_subjects)} subjects")
     return keep_subjects, keep_imgs, keep_events
 
+
 def _get_frame_times(img, confounds, t_r, slice_time_ref):
     img = check_niimg(img, ensure_ndim=4)
     n_scans = get_data(img).shape[3]
     confounds_matrix = confounds.values
     assert confounds_matrix.shape[0] == n_scans, "Confounds rows doesn't match n_scans!"
     start_time = slice_time_ref * t_r
     end_time = (n_scans - 1 + slice_time_ref) * t_r
     frame_times = np.linspace(start_time, end_time, n_scans)
     return frame_times
 
-def _add_parametric_modulation(regressors, column, events, frame_times, hrf_model, drift_model,
-                               high_pass, min_onset):
+
+def _add_parametric_modulation(
+    regressors,
+    column,
+    events,
+    frame_times,
+    hrf_model,
+    drift_model,
+    high_pass,
+    min_onset,
+):
     # Use the events variable "column" to create a parametric modulation regressor
-    events_pm = events[['onset', 'duration', column]].copy()
-    events_pm = events_pm.rename(columns={column: 'modulation'})
-    design_pm = make_first_level_design_matrix(frame_times,
-                                               events=events_pm,
-                                               hrf_model=hrf_model,
-                                               drift_model=drift_model,
-                                               high_pass=high_pass,
-                                               min_onset=min_onset)
-    regressors[f'{column}_mod'] = design_pm['dummy'].values
+    events_pm = events[["onset", "duration", column]].copy()
+    events_pm = events_pm.rename(columns={column: "modulation"})
+    design_pm = make_first_level_design_matrix(
+        frame_times,
+        events=events_pm,
+        hrf_model=hrf_model,
+        drift_model=drift_model,
+        high_pass=high_pass,
+        min_onset=min_onset,
+    )
+    regressors[f"{column}_mod"] = design_pm["dummy"].values
     return regressors
 
+
 def combine_run_masks(masks):
     # Combine masks from multiple runs by taking the product (logical and) of each run mask
-    return NiftiMasker(np.prod(np.stack([nilearn.image.get_data(i) for i in masks]), axis=0))
+    return NiftiMasker(
+        np.prod(np.stack([nilearn.image.get_data(i) for i in masks]), axis=0)
+    )
```

