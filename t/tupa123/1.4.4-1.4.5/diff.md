# Comparing `tmp/tupa123-1.4.4.tar.gz` & `tmp/tupa123-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tupa123-1.4.4.tar", last modified: Fri Apr 28 13:57:47 2023, max compression
+gzip compressed data, was "tupa123-1.4.5.tar", last modified: Tue May  2 17:40:46 2023, max compression
```

## Comparing `tupa123-1.4.4.tar` & `tupa123-1.4.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 13:57:47.453017 tupa123-1.4.4/
--rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.4.4/LICENSE.txt
--rw-rw-rw-   0        0        0     2352 2023-04-28 13:57:47.453017 tupa123-1.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     1876 2023-04-18 13:58:59.000000 tupa123-1.4.4/README.md
--rw-rw-rw-   0        0        0       42 2023-04-28 13:57:47.453017 tupa123-1.4.4/setup.cfg
--rw-rw-rw-   0        0        0      763 2023-04-28 13:57:02.000000 tupa123-1.4.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 13:57:47.443014 tupa123-1.4.4/tupa123/
--rw-rw-rw-   0        0        0       24 2023-03-27 17:38:15.000000 tupa123-1.4.4/tupa123/__init__.py
--rw-rw-rw-   0        0        0    72511 2023-04-28 13:53:17.000000 tupa123-1.4.4/tupa123/tupa123.py
-drwxrwxrwx   0        0        0        0 2023-04-28 13:57:47.453017 tupa123-1.4.4/tupa123.egg-info/
--rw-rw-rw-   0        0        0     2352 2023-04-28 13:57:47.000000 tupa123-1.4.4/tupa123.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-04-28 13:57:47.000000 tupa123-1.4.4/tupa123.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 13:57:47.000000 tupa123-1.4.4/tupa123.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-28 13:57:47.000000 tupa123-1.4.4/tupa123.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-28 13:57:47.000000 tupa123-1.4.4/tupa123.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 17:40:46.470552 tupa123-1.4.5/
+-rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.4.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     2352 2023-05-02 17:40:46.470552 tupa123-1.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1876 2023-04-18 13:58:59.000000 tupa123-1.4.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-02 17:40:46.486173 tupa123-1.4.5/setup.cfg
+-rw-rw-rw-   0        0        0      763 2023-05-02 17:39:54.000000 tupa123-1.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:40:46.470552 tupa123-1.4.5/tupa123/
+-rw-rw-rw-   0        0        0       24 2023-03-27 17:38:15.000000 tupa123-1.4.5/tupa123/__init__.py
+-rw-rw-rw-   0        0        0    72642 2023-05-02 17:35:55.000000 tupa123-1.4.5/tupa123/tupa123.py
+drwxrwxrwx   0        0        0        0 2023-05-02 17:40:46.470552 tupa123-1.4.5/tupa123.egg-info/
+-rw-rw-rw-   0        0        0     2352 2023-05-02 17:40:46.000000 tupa123-1.4.5/tupa123.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-05-02 17:40:46.000000 tupa123-1.4.5/tupa123.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 17:40:46.000000 tupa123-1.4.5/tupa123.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-02 17:40:46.000000 tupa123-1.4.5/tupa123.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-02 17:40:46.000000 tupa123-1.4.5/tupa123.egg-info/top_level.txt
```

### Comparing `tupa123-1.4.4/LICENSE.txt` & `tupa123-1.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tupa123-1.4.4/PKG-INFO` & `tupa123-1.4.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.4.4
+Version: 1.4.5
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `tupa123-1.4.4/README.md` & `tupa123-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `tupa123-1.4.4/setup.py` & `tupa123-1.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='tupa123',
-    version='1.4.4',
+    version='1.4.5',
     license = 'MIT',
     license_files=('LICENSE.txt',),    
     packages=['tupa123'],
     install_requires=['numpy','matplotlib','pandas'],    
     author='Leandro Schemmer',
     author_email='leandro.schemmer@gmail.com',
     description= 'fully connected neural network with four layers',
```

### Comparing `tupa123-1.4.4/tupa123/tupa123.py` & `tupa123-1.4.5/tupa123/tupa123.py`

 * *Files 1% similar despite different names*

```diff
@@ -482,15 +482,15 @@
 
 
 
 #Neural network 4 layers--------------------------------------------------------------------------------------------------------------------
 class nnet4:
 
     #global variables-------------------------------------------------------------------------
-    def __init__ (self, norma=1, coef=0, normout=1, nn1c=1, nn2c=5, nn3c=5, nn4c=1, rate=0.01, epochs=1000, fa2c=5, fa3c=5, fa4c=0, cost=0, regu=0, namenet='', shift=1, iteconv=0, conv=0, sbw=1, c1=2):
+    def __init__ (self, norma=1, coef=0, normout=1, nn1c=1, nn2c=5, nn3c=5, nn4c=1, rate=0.01, epochs=1000, fa2c=5, fa3c=5, fa4c=0, cost=0, regu=0, namenet='', shift=1, iteconv=0, conv=0, sbw=1, c1=2, txt=0):
         
         self.nn1c=nn1c
         self.nn2c=nn2c
         self.nn3c=nn3c
         self.nn4c=nn4c
         self.rate=rate
         self.epochs=epochs
@@ -503,15 +503,16 @@
         self.cost=cost
         self.regu=regu
         self.namenet=namenet
         self.shift=shift
         self.iteconv=iteconv
         self.conv=conv
         self.sbw=sbw
-        self.c1=c1 
+        self.c1=c1
+        self.txt=txt
 
 
 
 ###############################################################
 ###############################################################
 #########  Auxliar function to normalization   ################
 ###############################################################
@@ -1152,15 +1153,14 @@
 
 
 
 
 
 
 
-
     #machine learning stochastic case by case------------------------------------------------------
     def Fit_STOC(self, matX, matY, matX2=[0], matY2=[0]):
 
         tinicio = time.time()
         
         #Criação ou leitura da matriz dos pesos--------
 
@@ -1872,17 +1872,18 @@
 
             # saida----------------------------
             Calculated[caso][:] = c4[:]
 
         if (self.normout==1):            
             Calculated = self.DesNormalize(Calculated, nomepasta + "vmax_out.npy", nomepasta + "vmin_out.npy",nomepasta + "media_out.npy",nomepasta + "desvio_out.npy") 
 
-        return Calculated
-
+        if (self.txt!=0): #print txt out data
+             np.savetxt(nomepasta + "out.txt", Calculated)
 
+        return Calculated
```

### Comparing `tupa123-1.4.4/tupa123.egg-info/PKG-INFO` & `tupa123-1.4.5/tupa123.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.4.4
+Version: 1.4.5
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

