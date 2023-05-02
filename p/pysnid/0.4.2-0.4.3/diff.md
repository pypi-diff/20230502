# Comparing `tmp/pysnid-0.4.2.tar.gz` & `tmp/pysnid-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pysnid-0.4.2.tar", last modified: Fri Feb 18 14:16:58 2022, max compression
+gzip compressed data, was "pysnid-0.4.3.tar", last modified: Tue May  2 11:59:32 2023, max compression
```

## Comparing `pysnid-0.4.2.tar` & `pysnid-0.4.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 mrigault   (501) staff       (20)        0 2022-02-18 14:16:58.718603 pysnid-0.4.2/
--rw-r--r--   0 mrigault   (501) staff       (20)      256 2022-02-18 14:16:58.718291 pysnid-0.4.2/PKG-INFO
--rw-r--r--   0 mrigault   (501) staff       (20)     1297 2021-10-18 13:27:24.000000 pysnid-0.4.2/README.md
-drwxr-xr-x   0 mrigault   (501) staff       (20)        0 2022-02-18 14:16:58.715551 pysnid-0.4.2/pysnid/
--rw-r--r--   0 mrigault   (501) staff       (20)       49 2022-02-18 14:16:43.000000 pysnid-0.4.2/pysnid/__init__.py
--rw-r--r--   0 mrigault   (501) staff       (20)    31380 2022-02-18 14:02:39.000000 pysnid-0.4.2/pysnid/snid.py
--rw-r--r--   0 mrigault   (501) staff       (20)     3780 2022-02-09 13:55:29.000000 pysnid-0.4.2/pysnid/tools.py
-drwxr-xr-x   0 mrigault   (501) staff       (20)        0 2022-02-18 14:16:58.717502 pysnid-0.4.2/pysnid.egg-info/
--rw-r--r--   0 mrigault   (501) staff       (20)      256 2022-02-18 14:16:58.000000 pysnid-0.4.2/pysnid.egg-info/PKG-INFO
--rw-r--r--   0 mrigault   (501) staff       (20)      188 2022-02-18 14:16:58.000000 pysnid-0.4.2/pysnid.egg-info/SOURCES.txt
--rw-r--r--   0 mrigault   (501) staff       (20)        1 2022-02-18 14:16:58.000000 pysnid-0.4.2/pysnid.egg-info/dependency_links.txt
--rw-r--r--   0 mrigault   (501) staff       (20)        7 2022-02-18 14:16:58.000000 pysnid-0.4.2/pysnid.egg-info/top_level.txt
--rw-r--r--   0 mrigault   (501) staff       (20)       38 2022-02-18 14:16:58.718690 pysnid-0.4.2/setup.cfg
--rw-r--r--   0 mrigault   (501) staff       (20)      670 2022-02-18 14:16:47.000000 pysnid-0.4.2/setup.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-02 11:59:32.297758 pysnid-0.4.3/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    35149 2021-10-16 13:03:13.000000 pysnid-0.4.3/LICENSE
+-rw-r--r--   0 rigault   (2358) staff       (20)      222 2023-05-02 11:59:32.297636 pysnid-0.4.3/PKG-INFO
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     1297 2021-10-18 13:27:24.000000 pysnid-0.4.3/README.md
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-02 11:59:32.297031 pysnid-0.4.3/pysnid/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)       49 2023-05-02 11:59:08.000000 pysnid-0.4.3/pysnid/__init__.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    34362 2023-05-02 11:57:56.000000 pysnid-0.4.3/pysnid/snid.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     3780 2022-02-09 13:55:29.000000 pysnid-0.4.3/pysnid/tools.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-02 11:59:32.297502 pysnid-0.4.3/pysnid.egg-info/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      222 2023-05-02 11:59:32.000000 pysnid-0.4.3/pysnid.egg-info/PKG-INFO
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      196 2023-05-02 11:59:32.000000 pysnid-0.4.3/pysnid.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rigault   (2358) staff       (20)        1 2023-05-02 11:59:32.000000 pysnid-0.4.3/pysnid.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rigault   (2358) staff       (20)        7 2023-05-02 11:59:32.000000 pysnid-0.4.3/pysnid.egg-info/top_level.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)       38 2023-05-02 11:59:32.297802 pysnid-0.4.3/setup.cfg
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      670 2023-05-02 11:59:13.000000 pysnid-0.4.3/setup.py
```

### Comparing `pysnid-0.4.2/README.md` & `pysnid-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pysnid-0.4.2/pysnid/snid.py` & `pysnid-0.4.3/pysnid/snid.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,19 @@
         snid_prop["forcez"] = redshift
         if delta_redshift is not None:
             snid_prop["redshift_range"] = [redshift-delta_redshift, redshift+delta_redshift]
 
 
     # - Running SNID
     snidf = SNID()
-    outfile = snidf.run(filename, **{**snid_prop,**kwargs})
+    options = {**snid_prop,**kwargs}
+    if verbose:
+        print("options used:", options)
+        
+    outfile = snidf.run(filename, **options)
     if outfile is None:
         warnings.warn("SNID fit failed. Nothing returned")
         return None
 
     if get_results:        
         snidres = SNIDReader.from_filename(outfile)
         return snidres
@@ -62,15 +66,14 @@
     
     if as_dask == "gather":
         if client is None:
             return dask.delayed(list)(run_delayed).compute()
         return client.gather( client.compute(run_delayed) )
     
     raise ValueError(f"as_dask can only delayed, compute and gather: {as_dask} given")
-        
     
 
 
 class SNIDReader( object ):
 
     def __init__(self, data=None, results=None, models=None):
         """ """
@@ -108,21 +111,20 @@
                 else:
                     warnings.warn(f"not a single 'comp' stored in the input filename {filename}")
 
         this._filename = filename
         hdata.close()
         return this
 
-
     @property
-    def from_run(cls, filename, forcez=None, phase_range=[-20,50], redshift_range=[-0.01,0.4],
+    def from_run(cls, filename, 
                      **kwargs):
         """ """
         raise NotImplementedError("To be implemented")
-            
+
     # ============== #
     #  Method        #
     # ============== #
     def set_results(self, results):
         """ """
         results = results.copy()
         types = results["type"].str.replace("II","II-", regex=False
@@ -165,53 +167,89 @@
         bestmatches = pandas.merge(bestmatches, size_, left_index=True, right_index=True
                                        ).sort_values("rlap", ascending=False)
         
         if "cutoff" in bestmatches.index:
             return bestmatches.drop("cutoff")
         return bestmatches
 
-    def get_results(self, types="*", rlap_range=None, 
-                    lap_range=None, age_range=None, z_range=None,
-                    grade="good"):
+    def get_results(self, types="*", typing=None,
+                        rlap_range=None, 
+                        lap_range=None, age_range=None, z_range=None,
+                        grade="good", nfirst=30):
+        
         """ get a subset of the result dataframe """
+        
         def _get_in_range_(res_, key, rmin=None, rmax=None):
             """ """
             if not rmin is None or not rmax is None:
                 if rmax is None:
                     res_ = res_[res_[key]>=rmin]
                 elif rmin is None:
                     res_ = res_[res_[key]<=rmax]
                 else:
                     res_ = res_[res_[key].between(rmin, rmax)]
+                    
             return res_    
 
+        # Go
         if grade is None:
-            res = self.results.copy()
+            res = self.results
         else:
             res = self.results[self.results["grade"] == grade]
 
         if not (types is None or types in ["*","all"]):
             if "*" in types:
                 t_ = types.replace("*","")
                 types = [t for t in res["type"].astype("str").unique() if t_ in t]
             else:
                 types = np.atleast_1d(types)
 
             res = res[res["type"].isin(types)]
 
         if rlap_range is not None:
             res = _get_in_range_(res, "rlap", *rlap_range)
+            
         if z_range is not None:
             res = _get_in_range_(res, "z", *z_range)
+            
         if age_range is not None:
             res = _get_in_range_(res, "age", *age_range)
 
         if lap_range is not None:
             res = _get_in_range_(res, "lap", *lap_range)
 
+        #
+        # = Typing
+        #
+        if typing in ["*","all", "any"]:
+            typing = None
+
+        if typing in ["snia", "sn ia", "Ia"]:
+            typing = res[res["typing"] == "Ia"]["type"].unique()
+            
+        elif typing is not None:
+            if typing == "auto":
+                auto_type = self.get_type()
+                typing_, subtype_ = np.transpose(auto_type)[0]
+                
+                if typing_ == "unclear":
+                    typing = None    
+                elif subtype_ == "unclear":
+                    typing = bestres[bestres["typing"] == "Ia"]["type"].unique()
+                else:
+                    typing = f"{typing_}-{subtype_}"
+                    
+        # else typing is None            
+        if typing is not None:
+            res = res[res["type"].isin(np.atleast_1d(typing))]
+        # ============ #
+        
+        if nfirst is not None:
+            res = res.iloc[:nfirst]
+            
         return res
 
     def get_inputdata(self, fluxcorr=True):
         """ For some reason, the 'data' spectra recorded by SNID (and
         insite self.data) corresponds to input_flux*input_lbda.
         fluxcorr enables to return the correct flux such that:
         
@@ -266,15 +304,15 @@
         if full_output:
             return rlap_sums
 
         if len(rlap_sums)==0:
             warnings.warn(f"No 'rlap' greater than {min_rlap} ; '{fallback}'  returned")
             best_type, best_typefrac = (fallback, np.NaN)
         else:
-            typing_frac = rlap_sums.sum(level=0) # already a frac
+            typing_frac = rlap_sums.groupby(level=0).sum() # already a frac
             if typing_frac.iloc[0] < min_prob: # because stored by ascending=False
                 warnings.warn(f"No 'probabilities' above the {min_prob:.0%} ; '{fallback}' typing returned")
                 best_type, best_typefrac = (fallback, np.NaN)
             else:
                 best_typing = typing_frac.iloc[0] # because stored by ascending=False
                 best_type, best_typefrac = typing_frac.index[0],typing_frac.iloc[0]
 
@@ -292,14 +330,62 @@
         subtypes = rlap_sums.xs(best_type)
         subtype_frac = (subtypes/subtypes.sum()).sort_values(ascending=False)
 
         if subtype_frac.iloc[0]<min_prob:
             return (best_type, best_typefrac), (fallback, np.NaN)
         return (best_type, best_typefrac), (subtype_frac.index[0],subtype_frac.iloc[0])
 
+    def get_typing_result(self, typing="auto", 
+                         rlap_range=[5,None], nfirst=30):
+        """ """
+        bestres = self.get_results(rlap_range=rlap_range)
+        if nfirst is not None:
+            bestres = bestres.iloc[:30]
+
+        return bestres
+    
+    def get_redshift(self, typing="auto", weight_by="rlap",
+                    rlap_range=[5,None], nfirst=30,
+                    dredshift="nmad", **kwargs):
+        """ 
+
+        Parameters
+        ----------
+        typing: [None, string or list of] -optional-
+            if None or "*" all types will be used.
+            if auto, typing comes from auto-typing (self.get_type())
+            if given (could be a list), only given type is used.
+            if "Ia" all subtypes
+
+        """
+        DEFAULT = [np.nan, np.nan]
+        bestres = self.get_results(typing=typing, nfirst=nfirst,
+                                    rlap_range=rlap_range, **kwargs)
+
+        # nothing so back to nan
+        if len(bestres) == 0:
+            return DEFAULT
+
+        
+        if weight_by is not None:
+            weights = bestres[weight_by]
+            
+        # Redshift
+        redshift = np.average(bestres["z"], weights=weights)
+
+        # Error on
+        if dredshift == "nmad":
+            from scipy.stats import median_abs_deviation
+            dredshift = median_abs_deviation(bestres["z"])
+        else:
+            dredshift = getattr(np,"dredshift")(bestres["z"])
+            
+        return redshift, dredshift
+
+    
     # --------- #
     #  GETTER   #
     # --------- #
     def show(self, axes=None, fig=None,
                  nbest=4,min_rlap=5,nfirst_resummary=30,
                  show_typing=True, label=None,
                  sumprop={},
@@ -444,18 +530,21 @@
                     label= "_no_legend_"
 
                 ax.axvspan(v_-1,v_, facecolor=color, edgecolor="0.7", lw=0.5, label=label)
                 if j_==0:
                     ax.text(v_-0.5, -0.8, f"{res.loc[str(v_)]['rlap']:.1f}", 
                            color=color, va="top", ha="center", fontsize="x-small")
         # - ranking legend
-        ax.legend(loc=[0,1.2], 
+        try:
+            ax.legend(loc=[0,1.2], 
                   ncol=np.min([2,len(types_values)]), fontsize="x-small", frameon=False,
                  columnspacing=2, handlelength=1) 
-
+        except:
+            warnings.warn("legend failed")
+            
         _ = ax.set_xlim(0,nfirst)#len(res))
         _ = ax.set_yticks([])
         _ = ax.set_xticks([])
         # - Ranking texts
         ax.text(-0.08,   0.3, "rank", va="center", ha="right",
                     fontsize="x-small", color="0.6",
                     transform=ax.transAxes)
@@ -661,93 +750,105 @@
             self._snidid = f"{np.random.randint(1000000):08d}"
         else:
             self._snidid = f"{id_}"
         
     @staticmethod
     def build_snid_command(filename, 
                             forcez=None,
-                            lbda_range=[4000,8000], 
+                            lbda_range=[4000,9000], 
                             phase_range=[-20,50],
-                            redshift_range=[-0.01,0.4],
+                            redshift_range=[-0.05,0.4],
                             medlen=20, fwmed=None,
-                            min_rlap=2, 
+                            rlapmin=2, 
                             fluxout=30,
                             skyclip=False, aband=False, inter=False, plot=False,
                             param=None, verbose=True):
         """ """
-        lbdamin, lbdamax = lbda_range
-        agemin, agemax = phase_range
-        zmin, zmax = redshift_range
+
+
+
         
         cmd_snid  = f"snid "
         if param is not None:
             cmd_snid += f"param={param} "
+
+        if lbda_range is not None:
+            lbdamin, lbdamax = lbda_range
+            cmd_snid += f"wmin={int(lbdamin)} wmax={int(lbdamax)} "
             
-        cmd_snid += f"wmin={int(lbdamin)} wmax={int(lbdamax)} "
         # Redshift
         if forcez is not None:
             cmd_snid += f"forcez={forcez} "
-        cmd_snid += f"zmin={zmin} zmax={zmax} "
+
+        if redshift_range is not None:
+            zmin, zmax = redshift_range
+            cmd_snid += f"zmin={zmin} zmax={zmax} "
+            
         # Phase
-        cmd_snid += f"agemin={agemin:.0f} agemax={agemax:.0f} "
+        if phase_range is not None:
+            agemin, agemax = phase_range
+            cmd_snid += f"agemin={agemin:.0f} agemax={agemax:.0f} "
+            
         # Input Spectral Structure
         cmd_snid += f"skyclip={int(skyclip)} " 
         if medlen is not None:
             cmd_snid += f"medlen={int(medlen)} " 
         if fwmed is not None:
             cmd_snid += f"fwmed={int(fwmed)} " 
             
-        cmd_snid += f"fluxout={int(fluxout)} aband={int(aband)} min_rlap={int(min_rlap)} inter={int(inter)} plot={int(plot)} "
+        cmd_snid += f"fluxout={int(fluxout)} aband={int(aband)} rlapmin={int(rlapmin)} inter={int(inter)} plot={int(plot)} "
         cmd_snid += f"{filename}"
         if verbose:
             print(cmd_snid)
+            
         return cmd_snid
     
     def run(self, filename, fileout=None,
                 dirout=None, tmpdir=None,
                 cleanout=True, verbose=False,
                 quiet=False, paramfile=None, in_tmpdir=True,
                 **kwargs):
         """ run SNID and store the result as a hdf5 file. 
         
         **kwargs goes to build_snid_command
         forcez=None,
         lbda_range=[4000,8000], 
         phase_range=[-20,30],
         redshift_range=[0,0.2],
-        medlen=20, min_rlap=4, 
+        medlen=20, rlapmin=4, 
         fluxout=30,
         skyclip=False, aband=False, inter=False, plot=False
         
         """
+        import shutil
         from subprocess import PIPE, run
         from glob import glob
         #
         basename = os.path.basename(filename)
         dirname  = os.path.dirname(filename)        
         #
-        # Create a symlink to bypass the SNID filepath limitation
+        # Create a copy to bypass the SNID filepath limitation
         
         if tmpdir is None:
             tmpdir = f"tmpsnid_{self._snidid}"
         if not os.path.isdir(tmpdir):
             os.makedirs(tmpdir, exist_ok=True)
         if in_tmpdir:
             old_pwd=os.getcwd()
             os.chdir(tmpdir)
             self._tmpfile = f"snid_{self._snidid}_spectofit.ascii"
         else:
             old_pwd = None
             self._tmpfile = os.path.join(tmpdir, f"snid_{self._snidid}_spectofit.ascii")
             
-        os.symlink(filename, self._tmpfile)
+        shutil.copy(filename, self._tmpfile)
 
         tmpbase = os.path.basename(self._tmpfile).split(".")[0]
         
-        snid_cmd = self.build_snid_command(self._tmpfile, param=paramfile, **kwargs)
+        snid_cmd = self.build_snid_command(self._tmpfile, param=paramfile, verbose=verbose, **kwargs)
         
         self._result = run(snid_cmd.split(), stdout=PIPE, stderr=PIPE, universal_newlines=True)
         if verbose:
             print(f" running: {snid_cmd}")
             print(self._result.stdout.split("\n"))
         
         if self._result.returncode != 0:
@@ -772,15 +873,17 @@
             data = SNIDReader._read_snidflux_(datafile)
             models = pandas.concat({int(f_.split("comp")[-1].split("_")[0]):SNIDReader._read_snidflux_(f_) 
                                         for i,f_ in enumerate(modelfiles)})
             
             if fileout is None:
                 if dirout is None:
                     dirout = dirname
-                fileout = os.path.join(dirout,basename.split(".")[0]+"_snid.h5")
+
+                basename_noext, ext = os.path.splitext(basename)
+                fileout = os.path.join(dirout, basename_noext+"_snid.h5")
                 
             elif not fileout.endswith("h5"):
                 fileout+=".h5"
                 
             result.to_hdf(fileout, key="results", format='table')
             data.to_hdf(fileout, key="data", format='table')
             models.to_hdf(fileout, key="models", format='table')
```

### Comparing `pysnid-0.4.2/pysnid/tools.py` & `pysnid-0.4.3/pysnid/tools.py`

 * *Files identical despite different names*

### Comparing `pysnid-0.4.2/setup.py` & `pysnid-0.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from setuptools import setup, find_packages
 
 
 packages = find_packages()
 print(f"packages to be installed: {packages}")
 
 CODENAME = "pysnid"
-VERSION = '0.4.2'
+VERSION = '0.4.3'
         
 setup(name=CODENAME,
       version=VERSION,
       description='Tools to run and read SNID',
       author='Mickael Rigault',
       author_email='m.rigault@ipnl.in2p3.fr',
       url=f'https://github.com/MickaelRigault/{CODENAME}',
```

