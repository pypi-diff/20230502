# Comparing `tmp/qluster-0.0.4.tar.gz` & `tmp/qluster-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qluster-0.0.4.tar", last modified: Fri Apr  7 00:28:23 2023, max compression
+gzip compressed data, was "qluster-0.1.0.tar", last modified: Tue May  2 17:09:40 2023, max compression
```

## Comparing `qluster-0.0.4.tar` & `qluster-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 mdm988   (1344792526) domain users (1344200513)        0 2023-04-07 00:28:23.552783 qluster-0.0.4/
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)     1070 2023-02-23 15:50:36.000000 qluster-0.0.4/LICENSE
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      528 2023-04-07 00:28:23.548783 qluster-0.0.4/PKG-INFO
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      258 2023-04-07 00:27:06.000000 qluster-0.0.4/README.md
-drwxr-xr-x   0 mdm988   (1344792526) domain users (1344200513)        0 2023-04-07 00:28:23.548783 qluster-0.0.4/qluster/
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)     4806 2023-03-22 14:49:46.000000 qluster-0.0.4/qluster/__init__.py
-drwxr-xr-x   0 mdm988   (1344792526) domain users (1344200513)        0 2023-04-07 00:28:23.548783 qluster-0.0.4/qluster.egg-info/
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      528 2023-04-07 00:28:23.000000 qluster-0.0.4/qluster.egg-info/PKG-INFO
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      200 2023-04-07 00:28:23.000000 qluster-0.0.4/qluster.egg-info/SOURCES.txt
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)        1 2023-04-07 00:28:23.000000 qluster-0.0.4/qluster.egg-info/dependency_links.txt
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)       40 2023-04-07 00:28:23.000000 qluster-0.0.4/qluster.egg-info/requires.txt
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)        8 2023-04-07 00:28:23.000000 qluster-0.0.4/qluster.egg-info/top_level.txt
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)       38 2023-04-07 00:28:23.552783 qluster-0.0.4/setup.cfg
--rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      640 2023-04-07 00:27:20.000000 qluster-0.0.4/setup.py
+drwxr-xr-x   0 mdm988   (1344792526) domain users (1344200513)        0 2023-05-02 17:09:40.525324 qluster-0.1.0/
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)     1070 2023-02-23 15:50:36.000000 qluster-0.1.0/LICENSE
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      528 2023-05-02 17:09:40.525324 qluster-0.1.0/PKG-INFO
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      258 2023-04-07 00:27:06.000000 qluster-0.1.0/README.md
+drwxr-xr-x   0 mdm988   (1344792526) domain users (1344200513)        0 2023-05-02 17:09:40.525324 qluster-0.1.0/qluster/
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)       23 2023-04-30 14:02:45.000000 qluster-0.1.0/qluster/__init__.py
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)     5428 2023-04-30 14:31:14.000000 qluster-0.1.0/qluster/qluster.py
+drwxr-xr-x   0 mdm988   (1344792526) domain users (1344200513)        0 2023-05-02 17:09:40.525324 qluster-0.1.0/qluster.egg-info/
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      528 2023-05-02 17:09:40.000000 qluster-0.1.0/qluster.egg-info/PKG-INFO
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      219 2023-05-02 17:09:40.000000 qluster-0.1.0/qluster.egg-info/SOURCES.txt
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)        1 2023-05-02 17:09:40.000000 qluster-0.1.0/qluster.egg-info/dependency_links.txt
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)       40 2023-05-02 17:09:40.000000 qluster-0.1.0/qluster.egg-info/requires.txt
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)        8 2023-05-02 17:09:40.000000 qluster-0.1.0/qluster.egg-info/top_level.txt
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)       38 2023-05-02 17:09:40.525324 qluster-0.1.0/setup.cfg
+-rw-r--r--   0 mdm988   (1344792526) domain users (1344200513)      640 2023-05-02 17:08:48.000000 qluster-0.1.0/setup.py
```

### Comparing `qluster-0.0.4/LICENSE` & `qluster-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qluster-0.0.4/PKG-INFO` & `qluster-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qluster
-Version: 0.0.4
+Version: 0.1.0
 Summary: qluster
 Home-page: https://github.com/mdmould/qluster
 Author: Matthew Mould
 Author-email: mattdmould@gmail.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `qluster-0.0.4/qluster/__init__.py` & `qluster-0.1.0/qluster/qluster.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,17 +4,21 @@
 from tqdm import tqdm
 import tqdm_pathos
 import h5ify
 
 
 def sample_powerlaw(s, lo, hi, n=1):
 
-    return (
-        np.random.rand(n) * (hi**(s + 1) - lo**(s + 1)) + lo**(s + 1)
-        )**(1 / (s + 1))
+    if s == -1:
+        return np.exp(np.random.uniform(np.log(lo), np.log(hi), n))
+
+    else:
+        return (
+            np.random.rand(n) * (hi**(s + 1) - lo**(s + 1)) + lo**(s + 1)
+            )**(1 / (s + 1))
 
 
 def pairing(data, alpha, beta):
 
     m = data[:, 0]
 
     p1 = (m > min(m)) * m**alpha
@@ -31,20 +35,21 @@
     rest = np.delete(data, (ind1, ind2), axis=0)
 
     return bh1, bh2, rest
 
 
 def remnant(theta1, theta2, deltaphi, M, q, chi1, chi2):
 
-    s1, s2 = precession.get_fixed(q, chi1, chi2)[-2:]
-    mf = M * precession.finalmass(theta1, theta2, deltaphi, q, s1, s2)
-    chif = precession.finalspin(theta1, theta2, deltaphi, q, s1, s2)
-    vf = precession.finalkick(theta1, theta2, deltaphi, q, s1, s2, kms=True)
+    mf = M * precession.remnantmass(theta1, theta2, q, chi1, chi2)
+    chif = precession.remnantspin(theta1, theta2, deltaphi, q, chi1, chi2)
+    vf = precession.remnantkick(
+        theta1, theta2, deltaphi, q, chi1, chi2, kms=True,
+        )
 
-    return mf, chif, vf
+    return np.squeeze((mf, chif, vf))
 
 
 def check_file(file):
 
     if file[-3:] != '.h5':
         file += '.h5'
 
@@ -53,19 +58,22 @@
     return file
 
 
 def cluster(
     vesc,
     n_1g, gamma, mmin, mmax, chimin, chimax,
     alpha, beta,
-    file='./cluster.h5',
+    file='./cluster.h5'
+    seed=None,
     ):
-    
+
     file = check_file(file)
 
+    np.random.seed(seed)
+
     masses = sample_powerlaw(gamma, mmin, mmax, n_1g)
     spins = np.random.uniform(chimin, chimax, n_1g)
     generations = np.ones(n_1g)
     data = np.transpose([masses, spins, generations])
     mergers = []
 
     pbar = tqdm(total=len(data)-1, desc='Mergers')
@@ -111,14 +119,15 @@
         'mmin': mmin,
         'mmax': mmax,
         'chimin': chimin,
         'chimax': chimax,
         'alpha': alpha,
         'beta': beta,
         'n_mergers': len(mergers),
+        'seed': seed,
          }
 
     pars = (
         'M', 'q', 'chi1', 'chi2', 'theta1', 'theta2', 'deltaphi', 'generation',
         'mf', 'chif', 'vf', 'genf',
         )
     data = {par: val for par, val in zip(pars, np.transpose(mergers))}
@@ -129,34 +138,50 @@
 
 
 def clusters(
     n_clusters, delta, vescmin, vescmax,
     n_1g, gamma, mmin, mmax, chimin, chimax,
     alpha, beta,
     file='./cluster.h5',
-    multiprocess=False,
+    seed=None,
+    n_cpus=1,
     group_clusters=True,
-    keep_clusters=False,
+    keep_clusters=False
     ):
 
     file = check_file(file)
-
-    single = lambda ind, vesc: cluster(
-        vesc,
-        n_1g, gamma, mmin, mmax, chimin, chimax,
-        alpha, beta,
-        file=f'{file.split(".h5")[0]}_{ind}.h5',
-        )
+    
+    np.random.seed(seed)
 
     print('Clusters')
 
-    vescs = sample_powerlaw(delta, vescmin, vescmax, n_clusters)
+    # delta function escape speeds
+    if delta is None and vescmin == vescmax:
+        vescs = vescmin * np.ones(n_clusters)
+    # power law escape speeds
+    else:
+        vescs = sample_powerlaw(delta, vescmin, vescmax, n_clusters)
 
-    if multiprocess:
-        _ = tqdm_pathos.starmap(single, enumerate(vescs))
+    if seed is None:
+        seeds = [None] * n_clusters
+    else:
+        seeds = list(range(seed+1, seed+1+n_clusters))
+
+    def single(ind, vesc):
+
+        return cluster(
+            vesc,
+            n_1g, gamma, mmin, mmax, chimin, chimax,
+            alpha, beta,
+            file=f'{file.split(".h5")[0]}_{ind}.h5',
+            seed=seeds[ind],
+            )
+
+    if n_cpus > 1:
+        _ = tqdm_pathos.starmap(single, enumerate(vescs), n_cpus=n_cpus)
     else:
         _ = list(tqdm(map(single, range(n_clusters), vescs), total=n_clusters))
 
     if group_clusters:
         attrs = {
             'n_clusters':  n_clusters,
             'delta': delta,
@@ -166,14 +191,15 @@
             'gamma': gamma,
             'mmin': mmin,
             'mmax': mmax,
             'chimin': chimin,
             'chimax': chimax,
             'alpha': alpha,
             'beta': beta,
+            'seed': seed,
             }
         consolidate(file, attrs, keep_clusters)
 
 
 def consolidate(file, attrs, keep_clusters=False):
 
     file = check_file(file)
@@ -186,7 +212,12 @@
         data = {str(ind): h5ify.load(f'{file.split(".h5")[0]}_{ind}.h5')}
         h5ify.save(file, data, compression='gzip', compression_opts=9)
 
     if not keep_clusters:
         for ind in range(attrs['n_clusters']):
             os.system(f'rm {file.split(".h5")[0]}_{ind}.h5')
 
+
+if __name__ == '__main__':
+    
+    pass
+
```

### Comparing `qluster-0.0.4/qluster.egg-info/PKG-INFO` & `qluster-0.1.0/qluster.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qluster
-Version: 0.0.4
+Version: 0.1.0
 Summary: qluster
 Home-page: https://github.com/mdmould/qluster
 Author: Matthew Mould
 Author-email: mattdmould@gmail.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `qluster-0.0.4/setup.py` & `qluster-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 name = 'qluster'
-version = '0.0.4'
+version = '0.1.0'
 
 with open('README.md' ,'r') as f:
     long_description = f.read().strip()
 
 setup(
     name=name,
     version=version,
```

