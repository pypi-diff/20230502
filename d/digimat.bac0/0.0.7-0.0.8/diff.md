# Comparing `tmp/digimat.bac0-0.0.7.tar.gz` & `tmp/digimat.bac0-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digimat.bac0-0.0.7.tar", last modified: Mon Apr 17 21:47:27 2023, max compression
+gzip compressed data, was "digimat.bac0-0.0.8.tar", last modified: Tue Apr 18 07:03:55 2023, max compression
```

## Comparing `digimat.bac0-0.0.7.tar` & `digimat.bac0-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 21:47:27.247465 digimat.bac0-0.0.7/
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-17 21:47:27.247112 digimat.bac0-0.0.7/PKG-INFO
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       38 2023-04-17 21:47:27.247560 digimat.bac0-0.0.7/setup.cfg
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      984 2023-04-17 21:47:22.000000 digimat.bac0-0.0.7/setup.py
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 21:47:27.239590 digimat.bac0-0.0.7/src/
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 21:47:27.240342 digimat.bac0-0.0.7/src/digimat/
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       57 2014-09-24 08:13:04.000000 digimat.bac0-0.0.7/src/digimat/__init__.py
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 21:47:27.246605 digimat.bac0-0.0.7/src/digimat/bac0/
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       25 2023-04-15 20:24:12.000000 digimat.bac0-0.0.7/src/digimat/bac0/__init__.py
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)    10140 2023-04-17 21:45:15.000000 digimat.bac0-0.0.7/src/digimat/bac0/bacnet.py
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-17 21:47:27.245673 digimat.bac0-0.0.7/src/digimat.bac0.egg-info/
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-17 21:47:27.000000 digimat.bac0-0.0.7/src/digimat.bac0.egg-info/PKG-INFO
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-16 10:41:01.000000 digimat.bac0-0.0.7/src/digimat.bac0.egg-info/PKG-INFO (imacfhe.local's conflicted copy 2023-04-16)
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      455 2023-04-17 21:47:27.000000 digimat.bac0-0.0.7/src/digimat.bac0.egg-info/SOURCES.txt
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        1 2023-04-17 21:47:27.000000 digimat.bac0-0.0.7/src/digimat.bac0.egg-info/dependency_links.txt
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        8 2023-04-17 21:47:27.000000 digimat.bac0-0.0.7/src/digimat.bac0.egg-info/namespace_packages.txt
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        1 2023-04-15 19:35:42.000000 digimat.bac0-0.0.7/src/digimat.bac0.egg-info/not-zip-safe
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       42 2023-04-17 21:47:27.000000 digimat.bac0-0.0.7/src/digimat.bac0.egg-info/requires.txt
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        8 2023-04-17 21:47:27.000000 digimat.bac0-0.0.7/src/digimat.bac0.egg-info/top_level.txt
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-18 07:03:55.952926 digimat.bac0-0.0.8/
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-18 07:03:55.952643 digimat.bac0-0.0.8/PKG-INFO
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       38 2023-04-18 07:03:55.953020 digimat.bac0-0.0.8/setup.cfg
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      984 2023-04-18 07:03:49.000000 digimat.bac0-0.0.8/setup.py
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-18 07:03:55.948579 digimat.bac0-0.0.8/src/
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-18 07:03:55.949123 digimat.bac0-0.0.8/src/digimat/
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       57 2014-09-24 08:13:04.000000 digimat.bac0-0.0.8/src/digimat/__init__.py
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-18 07:03:55.952155 digimat.bac0-0.0.8/src/digimat/bac0/
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       25 2023-04-15 20:24:12.000000 digimat.bac0-0.0.8/src/digimat/bac0/__init__.py
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)    10499 2023-04-18 07:03:18.000000 digimat.bac0-0.0.8/src/digimat/bac0/bacnet.py
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-18 07:03:55.951643 digimat.bac0-0.0.8/src/digimat.bac0.egg-info/
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-18 07:03:55.000000 digimat.bac0-0.0.8/src/digimat.bac0.egg-info/PKG-INFO
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-16 10:41:01.000000 digimat.bac0-0.0.8/src/digimat.bac0.egg-info/PKG-INFO (imacfhe.local's conflicted copy 2023-04-16)
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      455 2023-04-18 07:03:55.000000 digimat.bac0-0.0.8/src/digimat.bac0.egg-info/SOURCES.txt
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        1 2023-04-18 07:03:55.000000 digimat.bac0-0.0.8/src/digimat.bac0.egg-info/dependency_links.txt
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        8 2023-04-18 07:03:55.000000 digimat.bac0-0.0.8/src/digimat.bac0.egg-info/namespace_packages.txt
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        1 2023-04-15 19:35:42.000000 digimat.bac0-0.0.8/src/digimat.bac0.egg-info/not-zip-safe
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       42 2023-04-18 07:03:55.000000 digimat.bac0-0.0.8/src/digimat.bac0.egg-info/requires.txt
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        8 2023-04-18 07:03:55.000000 digimat.bac0-0.0.8/src/digimat.bac0.egg-info/top_level.txt
```

### Comparing `digimat.bac0-0.0.7/setup.py` & `digimat.bac0-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='digimat.bac0',
-    version='0.0.7',
+    version='0.0.8',
     description='Digimat BACnet BAC0 Wrapper',
     namespace_packages=['digimat'],
     author='Frederic Hess',
     author_email='fhess@st-sa.ch',
     url='http://www.digimat.ch',
     license='PSF',
     packages=find_packages('src'),
```

### Comparing `digimat.bac0-0.0.7/src/digimat/bac0/bacnet.py` & `digimat.bac0-0.0.8/src/digimat/bac0/bacnet.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,24 +75,28 @@
             if points:
                 for point in points:
                     if not self.point(point.properties.name):
                         self._pointsByName[point.properties.name]=point
                         self._pointsIndexByName[point.properties.name]=len(self._points)
                         self._points.append(point)
 
-    def cov(self, enable=True):
+    def covSubscribe(self, lifeTime=300, confirmed=True):
         points=self.points()
         if points:
             for point in points:
-                if enable:
-                    if not point.cov_registered:
-                        point.subscribe_cov()
-                else:
-                    if point.cov_registered:
-                        point.cancel_cov()
+                point.cancel_cov()
+                if lifeTime<60:
+                    lifeTime=60
+                point.subscribe_cov(confirmed=confirmed, lifetime=lifeTime)
+
+    def covCancel(self):
+        points=self.points()
+        if points:
+            for point in points:
+                point.cancel_cov()
 
     def properties(self, index):
         point=self.point(index)
         if point:
             return point.properties
 
     def dump(self, key=None):
@@ -104,18 +108,19 @@
             t.align['name']='l'
             t.align['type']='l'
             t.align['value']='r'
             t.align['unit']='l'
             t.align['description']='l'
             for point in points:
                 index=self._pointsIndexByName[point.properties.name]
+                address='%s:%s' % (point.properties.type, point.properties.address)
                 cov=''
                 if point.cov_registered:
                     cov='X'
-                t.add_row([index, point.properties.name, point.properties.type, point.value, cov, point.units, point.properties.description])
+                t.add_row([index, point.properties.name, address, point.value, cov, point.units, point.properties.description])
             print(t)
 
     def refresh(self, key=None):
         points=self.points(key)
         if points:
             for point in points:
                 point.value
@@ -199,31 +204,37 @@
             if key:
                 if key not in point.properties.name.lower() and \
                         key not in point.properties.description.lower():
                     continue
             items.append(point)
         return items
 
-    def ai(self, key=None):
-        return self.points(key, objectType='analogInput')
+    def find(self, objectType, objectAddress):
+        try:
+            return self._device.find_point(objectType, objectAddress)
+        except:
+            pass
+
+    def ai(self, index):
+        return self.find('analogInput', index)
 
-    def ao(self, key=None):
-        return self.points(key, objectType='analogOuput')
+    def ao(self, index):
+        return self.find('analogOutput', index)
 
-    def bi(self, key=None):
-        return self.points(key, objectType='binaryInput')
+    def bi(self, index):
+        return self.find('binaryInput', index)
 
-    def bo(self, key=None):
-        return self.points(key, objectType='binaryOutput')
+    def bo(self, index):
+        return self.find('binaryOutput', index)
 
-    def bv(self, key=None):
-        return self.points(key, objectType='binaryValue')
+    def av(self, index):
+        return self.find('analogValue', index)
 
-    def av(self, key=None):
-        return self.points(key, objectType='analogValue')
+    def bv(self, index):
+        return self.find('binaryValue', index)
 
     def __getitem__(self, key):
         try:
             return self.points(key)[0]
         except:
             pass
 
@@ -238,15 +249,17 @@
             t.align['value']='r'
             t.align['unit']='l'
             t.align['description']='l'
             for point in points:
                 cov=''
                 if point.cov_registered:
                     cov='X'
-                t.add_row([point.properties.name, point.properties.type, point.value, cov, point.units, point.properties.description])
+                address='%s:%s' % (point.properties.type, point.properties.address)
+                t.add_row([point.properties.name, address,
+                           point.value, cov, point.units, point.properties.description])
             print(t)
 
     def bag(self, key=None):
         return BACBag(self, key)
 
     def __iter__(self):
         return iter(self._device.points)
```

