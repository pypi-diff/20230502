# Comparing `tmp/nustarpipeline-0.2.6.tar.gz` & `tmp/nustarpipeline-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nustarpipeline-0.2.6.tar", last modified: Fri Apr 28 09:16:09 2023, max compression
+gzip compressed data, was "nustarpipeline-0.2.7.tar", last modified: Tue May  2 07:09:12 2023, max compression
```

## Comparing `nustarpipeline-0.2.6.tar` & `nustarpipeline-0.2.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2023-04-28 09:16:09.180840 nustarpipeline-0.2.6/
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1071 2022-08-24 20:22:52.000000 nustarpipeline-0.2.6/LICENSE
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1478 2023-04-28 09:16:09.180840 nustarpipeline-0.2.6/PKG-INFO
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      688 2022-08-26 16:47:35.000000 nustarpipeline-0.2.6/README.md
-drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2023-04-28 09:16:09.180840 nustarpipeline-0.2.6/nustarpipeline/
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)        0 2022-08-26 16:41:51.000000 nustarpipeline-0.2.6/nustarpipeline/__init__.py
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)    40130 2023-02-15 00:21:50.000000 nustarpipeline-0.2.6/nustarpipeline/process.py
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)    87077 2023-04-28 09:04:17.000000 nustarpipeline-0.2.6/nustarpipeline/utils.py
-drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2023-04-28 09:16:09.180840 nustarpipeline-0.2.6/nustarpipeline.egg-info/
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1478 2023-04-28 09:16:09.000000 nustarpipeline-0.2.6/nustarpipeline.egg-info/PKG-INFO
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      343 2023-04-28 09:16:09.000000 nustarpipeline-0.2.6/nustarpipeline.egg-info/SOURCES.txt
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)        1 2023-04-28 09:16:09.000000 nustarpipeline-0.2.6/nustarpipeline.egg-info/dependency_links.txt
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      188 2023-04-28 09:16:09.000000 nustarpipeline-0.2.6/nustarpipeline.egg-info/entry_points.txt
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      101 2023-04-28 09:16:09.000000 nustarpipeline-0.2.6/nustarpipeline.egg-info/requires.txt
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)       15 2023-04-28 09:16:09.000000 nustarpipeline-0.2.6/nustarpipeline.egg-info/top_level.txt
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1541 2023-04-28 09:16:09.184840 nustarpipeline-0.2.6/setup.cfg
--rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      361 2023-04-28 09:15:40.000000 nustarpipeline-0.2.6/setup.py
+drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2023-05-02 07:09:12.745496 nustarpipeline-0.2.7/
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1071 2022-08-24 20:22:52.000000 nustarpipeline-0.2.7/LICENSE
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1478 2023-05-02 07:09:12.745496 nustarpipeline-0.2.7/PKG-INFO
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      688 2022-08-26 16:47:35.000000 nustarpipeline-0.2.7/README.md
+drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2023-05-02 07:09:12.745496 nustarpipeline-0.2.7/nustarpipeline/
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)        0 2022-08-26 16:41:51.000000 nustarpipeline-0.2.7/nustarpipeline/__init__.py
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)    40130 2023-02-15 00:21:50.000000 nustarpipeline-0.2.7/nustarpipeline/process.py
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)    90153 2023-05-02 06:46:33.000000 nustarpipeline-0.2.7/nustarpipeline/utils.py
+drwxrwxr-x   0 ferrigno  (1000) ferrigno  (1000)        0 2023-05-02 07:09:12.745496 nustarpipeline-0.2.7/nustarpipeline.egg-info/
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1478 2023-05-02 07:09:12.000000 nustarpipeline-0.2.7/nustarpipeline.egg-info/PKG-INFO
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      343 2023-05-02 07:09:12.000000 nustarpipeline-0.2.7/nustarpipeline.egg-info/SOURCES.txt
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)        1 2023-05-02 07:09:12.000000 nustarpipeline-0.2.7/nustarpipeline.egg-info/dependency_links.txt
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      188 2023-05-02 07:09:12.000000 nustarpipeline-0.2.7/nustarpipeline.egg-info/entry_points.txt
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      101 2023-05-02 07:09:12.000000 nustarpipeline-0.2.7/nustarpipeline.egg-info/requires.txt
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)       15 2023-05-02 07:09:12.000000 nustarpipeline-0.2.7/nustarpipeline.egg-info/top_level.txt
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)     1541 2023-05-02 07:09:12.745496 nustarpipeline-0.2.7/setup.cfg
+-rw-rw-r--   0 ferrigno  (1000) ferrigno  (1000)      361 2023-05-02 06:46:25.000000 nustarpipeline-0.2.7/setup.py
```

### Comparing `nustarpipeline-0.2.6/LICENSE` & `nustarpipeline-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nustarpipeline-0.2.6/PKG-INFO` & `nustarpipeline-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nustarpipeline
-Version: 0.2.6
+Version: 0.2.7
 Summary: nustar-pipeline
 Home-page: https://gitlab.astro.unige.ch/ferrigno/nustar-pipeline
 Author: C.F.
 Author-email: carlo.ferrigno@unige.ch
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `nustarpipeline-0.2.6/README.md` & `nustarpipeline-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `nustarpipeline-0.2.6/nustarpipeline/process.py` & `nustarpipeline-0.2.7/nustarpipeline/process.py`

 * *Files identical despite different names*

### Comparing `nustarpipeline-0.2.6/nustarpipeline/utils.py` & `nustarpipeline-0.2.7/nustarpipeline/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1946,44 +1946,73 @@
         err_a[i] = np.std(y)
         y = np.array([x[i] for x in sim_phi ])
         y = align_phases(y, debug=debug)
         err_phi[i] = np.std(y)
         
     return err_a, err_phi
 
-def align_phases(y, nbins=20, debug=False, distance_factor=2):
+def align_phases(y, nbins=20, debug=False, distance_factor=1.5, margin=0.1, label=None):
+    """align_phases: tries to align phases by building an histogram of phases.
+    If only one peak is found, it is considered as a phae shiter only if it is 
+    - in 0-margin(0.1) phases higher than 0.1+margin are shifted by -1
+    - in (1-margin)(0.9)-1. phases lower than 0.9-margin are shifted by +1
+
+    If more than one peak in the interval 0-margin(0.1) or (1-margin)(0.9)-1.0 are found, the higher phases are
+    shifted by -1 (these peaks are often artifact of the algorithm)
+
+    Args:
+        y (numpy array): the phases to be aligned (in 0.-1.0 interval)
+        nbins (int, optional): number of bins of the histogram to be built. Defaults to 20.
+        debug (bool, optional): if True makes debug plots. Defaults to False.
+        distance_factor (float, optional): if peaks are closer than 1/distace_factor times the maximum span, they are 
+                                            rejected. Defaults to 1.5.
+        margin (float, optional): . Defaults to 0.1.
+        label (str, optional): a label of the debug plot (e.g. the energy). Defaults to None.
+
+    Returns:
+        numpy array: the aligned phases
+    """    
     hist,bins = np.histogram(y, bins=nbins)
     from scipy.signal import find_peaks
-    peaks, _ = find_peaks(np.concatenate(([np.min(hist)],hist, [np.min(hist)])), distance=nbins/distance_factor)#, prominence=(0.5))
+    peaks, properties = find_peaks(np.concatenate(([np.min(hist)],hist, [np.min(hist)])), 
+                          distance=nbins/distance_factor, prominence=0)
     peaks-=1
     if(debug):
-        plt.figure()
-        plt.hist(y, bins=nbins)
-
-        print(hist)
-        print(bins)
-        print(peaks)
+        fig, ax = plt.subplots()
+        ax.bar(bins[:-1], hist, width=np.diff(bins), edgecolor="blue", align="edge")
+        for ppp in peaks:
+            ax.axvline(bins[ppp+1], color='red')
+        if label is not None:
+            ax.set_title(label)
+            
+    logger.debug(label)
+    logger.debug(hist)
+    logger.debug(bins)
+    logger.debug(peaks)
+    logger.debug(properties['prominences'])
+    logger.debug('\n')
         
     if (len(peaks) == 2):
         ind_division = int((peaks[0]+peaks[1])/2)
-        if (peaks[0] > 0.25*nbins and peaks[0] < 0.75*nbins ) or (peaks[1] > 0.25*nbins and peaks[1] < 0.75*nbins ):
-            
+        if (peaks[0] > margin*nbins and peaks[0] < (1.-margin)*nbins ) or \
+        (peaks[1] > margin*nbins and peaks[1] < (1.-margin)*nbins ):
             logger.debug("No phase shift for two peaks")
+            
         else:
             phase_division = bins[ind_division]
             logger.debug("two peaks, phase_Division %f" % phase_division)
             y[y>phase_division]-=1.
     elif len(peaks) == 1:
-        if peaks[0] < nbins/4:
-            phase_division = bins[int(0.75*nbins)]
+        if peaks[0] < margin:
+            phase_division = bins[int((0.9-margin)*nbins)]
             logger.debug("Phase_division" ,phase_division)
             logger.debug(np.sum(y>phase_division))
             y[y>phase_division]-=1
-        if peaks[0]>0.75*nbins:
-            phase_division = bins[int(0.25*nbins)]
+        if peaks[0]>(1-margin):
+            phase_division = bins[int((0.1+margin)*nbins)]
             logger.debug("Phase_division" ,phase_division)
             logger.debug(np.sum(y>phase_division))
             y[y<phase_division]+=1
             
     return y
 
 def rate_filter(time, rate, drate, level_down=0, level_up = 1e10, quantile=0.8, make_plot=True, 
@@ -2107,14 +2136,15 @@
         pp (numpy array): the nergy or time-phase matrix
         plot (bool, optional): if making debug plots. Defaults to False.
         n_to_fit (int, optional): number of bins to use for the fit on each side of the peak. Defaults to 3.
 
     Returns:
         numpy arrays: lag, correlation
     """
+    
     from lmfit.models import PolynomialModel, GaussianModel
     poly_mod = PolynomialModel(prefix='poly_', degree=0)
     gauss = GaussianModel(prefix='g'  + '_')
 
     n_pulse=pp.shape[1]
     if n_to_fit > n_pulse/3:
         logger.warning('The pulse has size %s and you try to use % points' %(n_pulse, 2*n_to_fit+1))
@@ -2125,24 +2155,28 @@
 
         x = (pp[i, :] - np.mean(pp[i, :])) / np.std(pp[i, :])
         y = np.sum(pp[0:i, :], 0) + np.sum(pp[i + 1:, :], 0)
         y = (y - np.mean(y)) / np.std(y)
         corr = np.correlate(np.tile(x, 2), y) / len(x)
 
         i_max = np.argmax(corr)
-
         if i_max - n_to_fit >= 0 and i_max + n_to_fit <= len(x) :
-            to_fit =  corr[i_max-n_to_fit:i_max+n_to_fit]
+            to_fit =  corr[i_max-n_to_fit:i_max+n_to_fit+1]
         elif i_max - n_to_fit < 0:
-            to_fit = np.concatenate([corr[i_max-n_to_fit:], corr[0:i_max+n_to_fit]])
+            logger.debug('First')
+            to_fit = np.concatenate([corr[i_max-n_to_fit-1:-1], corr[0:i_max+n_to_fit+1]])
         else:
-            to_fit = np.concatenate([corr[i_max-n_to_fit:], corr[1:i_max+n_to_fit-len(x)]])
-            
+            logger.debug('Last !')
+            to_fit = np.concatenate([corr[i_max-n_to_fit:], corr[1:i_max+n_to_fit-len(x)+1]])
+        logger.debug("Check vector %f %f " %( corr[0], corr[-1]) )
+        
+        x_to_fit = np.arange(i_max-n_to_fit,i_max+n_to_fit+1, dtype=float)
         
-        x_to_fit = np.arange(i_max-n_to_fit,i_max+n_to_fit, dtype=float) 
+        #for aa,bb in zip(x_to_fit, to_fit):
+        #    print(aa,bb)
         
         pars = poly_mod.guess(to_fit, x=x_to_fit, degree=0)
         mod = poly_mod
     
         pars.update(gauss.make_params())
         pars['g' +  '_center'].set(value=float(i_max), min=i_max-n_to_fit, max=i_max+n_to_fit)
         pars['g' +  '_sigma'].set(value=1., min=0, max=n_to_fit)
@@ -2154,24 +2188,31 @@
         correlation.append(np.max(out.eval(x=np.linspace(x_to_fit[0], x_to_fit[-1], 100))))
         lag.append(out.best_values['g' +  '_center'])
 
         if plot:
             import matplotlib.pyplot as plt
             plt.figure()
             plt.subplot(1, 2, 1)
-            plt.plot(corr)
+            plt.plot(x_to_fit, to_fit, label='X-corr values', color='blue', marker='o', linestyle='')
+            plt.plot(np.linspace(x_to_fit[0], x_to_fit[-1],100),
+                                 out.eval(x=np.linspace(x_to_fit[0], x_to_fit[-1], 100))
+                                 , label='X-corr fit', color='orange')
+            
             plt.title('correlation')
             plt.axvline(lag[-1])
             plt.axhline(correlation[-1])
             plt.subplot(1, 2, 2)
-            plt.plot(x, label='Pulse')
-            plt.plot(y, linestyle='--', label='Average')
+            plt.plot(x, label='Pulse', color='blue')
+            plt.plot(y, linestyle='--', label='Average', color='orange')
+            plt.title('Pulse and average')
+            plt.legend()
+            
 
     lag = np.array(lag) / n_pulse
-    lag[lag > 0.5] -= 1.
+
     return lag, np.array(correlation)
 
 def get_cross_correlation_with_error(pp, dpp, ee_pulsed=[], dee_pulsed=[], n_simul=100, 
                             use_poisson=False, n_to_fit=3, debug_plot=False, stem=None, title=''):
     """Makes the cross correlation of each pulse in the matrix with the average of the rest of the matrix
 
     Args:
@@ -2200,29 +2241,54 @@
 
     for i in range(n_simul):
         if use_poisson:
             fake_pp = random.poisson(pp)
         else:
             fake_pp = random.normal(pp, dpp)
 
-        fake_lags[i, :], fake_corrs[i, :] = get_cross_correlation(fake_pp, n_to_fit=n_to_fit)
+        fake_lags[i, :], fake_corrs[i, :] = get_cross_correlation(fake_pp, n_to_fit=n_to_fit)#, plot=debug_plot)
+    
+    for i in range(fake_lags.shape[1]):
+        fake_lags[:,i] = align_phases(fake_lags[:,i], debug=debug_plot, label='%.1f kev' % (ee_pulsed[i]))
+        
     
-    lag_errors = np.std(align_phases(fake_lags), 0)
+    lag_errors = np.std(fake_lags, 0)
+    lag_checks = np.mean(fake_lags, 0)
     correlation_errors = np.std(fake_corrs, 0)
+    
+    lags[lags>0.5] -= 1.0
+    lag_checks[lag_checks>0.5] -= 1.0
+    
+    lags[lags<0.5] += 1.0
+    lag_checks[lag_checks<0.5] += 1.0
+    
+    if debug_plot:
+        for i in range(fake_lags.shape[1]):
+            fig, (ax1, ax2) = plt.subplots(1, 2, figsize=(6, 8))
+            ax1.hist(fake_lags[:,i], bins=int(n_simul/5))
+            ax1.set_xlabel('Lags')
+            ax1.set_title('%.1f keV' % ee_pulsed[i])
+            ax2.hist(fake_corrs[:,i], bins=int(n_simul/5))
+            ax1.set_ylabel('Correlations')
+        
 
     if stem is not None:
         if len(ee_pulsed) != len(lags):
-            raise ValueError('You should provide energy vetcors with size %d to plot' % len(lags))
+            
+            raise ValueError('You should provide energy vetcors with size %d to plot, but was %d' % \
+                             (len(lags), len(ee_pulsed)))
         
         fig, (ax1, ax2) = plt.subplots(2, 1, figsize=(6, 8), sharex=True, gridspec_kw={'height_ratios': [1, 1],
                                                                               'hspace': 0.0})
         ax1.errorbar(ee_pulsed, correlations, xerr=dee_pulsed, yerr=correlation_errors, marker='.', linestyle='')
         ax1.set_title(title)
         ax1.set_ylabel('Correlation')
         ax2.errorbar(ee_pulsed, lags, xerr=dee_pulsed, yerr=lag_errors, marker='x', linestyle='')
+        if debug_plot:
+            ax2.scatter(ee_pulsed, lag_checks, marker='o', color='green')
         ax2.set_ylabel('Lag (phase units)')
         ax2.set_xlabel('Energy [keV]')
         ax2.set_xscale('log')
         fig.savefig(stem+'_lag_correlation.png' )
 
     return lags, lag_errors, correlations, correlation_errors
```

### Comparing `nustarpipeline-0.2.6/nustarpipeline.egg-info/PKG-INFO` & `nustarpipeline-0.2.7/nustarpipeline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nustarpipeline
-Version: 0.2.6
+Version: 0.2.7
 Summary: nustar-pipeline
 Home-page: https://gitlab.astro.unige.ch/ferrigno/nustar-pipeline
 Author: C.F.
 Author-email: carlo.ferrigno@unige.ch
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `nustarpipeline-0.2.6/setup.cfg` & `nustarpipeline-0.2.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.6
+current_version = 0.2.7
 commit = True
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\-(?P<release>[a-z]+)(?P<build>\d+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}{build}
 	{major}.{minor}.{patch}
```

