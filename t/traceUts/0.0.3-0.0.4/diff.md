# Comparing `tmp/traceUts-0.0.3.tar.gz` & `tmp/TraceUts-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\traceUts-0.0.3.tar", last modified: Tue Nov 15 15:37:15 2022, max compression
+gzip compressed data, was "traceUts-0.0.4.tar", last modified: Tue May  2 14:41:28 2023, max compression
```

## Comparing `traceUts-0.0.3.tar` & `TraceUts-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-11-15 15:37:15.778180 traceUts-0.0.3/
--rw-rw-rw-   0        0        0      156 2022-11-15 15:37:06.000000 traceUts-0.0.3/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1058 2022-05-25 14:00:44.000000 traceUts-0.0.3/LICENCE.txt
--rw-rw-rw-   0        0        0       30 2022-05-25 22:21:08.000000 traceUts-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      816 2022-11-15 15:37:15.776179 traceUts-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       13 2022-11-15 15:26:30.000000 traceUts-0.0.3/README.md
--rw-rw-rw-   0        0        0      122 2022-10-04 01:40:33.000000 traceUts-0.0.3/commands.txt
--rw-rw-rw-   0        0        0       42 2022-11-15 15:37:15.778180 traceUts-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      750 2022-11-15 15:36:54.000000 traceUts-0.0.3/setup.py
--rw-rw-rw-   0        0        0      181 2022-11-15 15:30:14.000000 traceUts-0.0.3/test.py
-drwxrwxrwx   0        0        0        0 2022-11-15 15:37:15.742181 traceUts-0.0.3/traceUts/
--rw-rw-rw-   0        0        0     6766 2022-11-15 15:24:56.000000 traceUts-0.0.3/traceUts/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-15 15:37:15.774178 traceUts-0.0.3/traceUts.egg-info/
--rw-rw-rw-   0        0        0      816 2022-11-15 15:37:15.000000 traceUts-0.0.3/traceUts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2022-11-15 15:37:15.000000 traceUts-0.0.3/traceUts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-15 15:37:15.000000 traceUts-0.0.3/traceUts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-11-15 15:37:15.000000 traceUts-0.0.3/traceUts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 14:41:28.745673 traceUts-0.0.4/
+-rw-rw-rw-   0        0        0      156 2023-05-02 14:40:12.000000 traceUts-0.0.4/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1058 2023-05-02 14:40:12.000000 traceUts-0.0.4/LICENCE.txt
+-rw-rw-rw-   0        0        0       30 2023-05-02 14:40:12.000000 traceUts-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      710 2023-05-02 14:41:28.744675 traceUts-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-05-02 14:40:12.000000 traceUts-0.0.4/README.md
+-rw-rw-rw-   0        0        0      122 2023-05-02 14:40:12.000000 traceUts-0.0.4/commands.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 14:41:28.745673 traceUts-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      750 2023-05-02 14:41:10.000000 traceUts-0.0.4/setup.py
+-rw-rw-rw-   0        0        0      181 2023-05-02 14:40:12.000000 traceUts-0.0.4/test.py
+drwxrwxrwx   0        0        0        0 2023-05-02 14:41:28.716750 traceUts-0.0.4/traceUts/
+-rw-rw-rw-   0        0        0     6766 2023-05-02 14:41:04.000000 traceUts-0.0.4/traceUts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 14:41:28.742681 traceUts-0.0.4/traceUts.egg-info/
+-rw-rw-rw-   0        0        0      710 2023-05-02 14:41:28.000000 traceUts-0.0.4/traceUts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-05-02 14:41:28.000000 traceUts-0.0.4/traceUts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 14:41:28.000000 traceUts-0.0.4/traceUts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-02 14:41:28.000000 traceUts-0.0.4/traceUts.egg-info/top_level.txt
```

### Comparing `traceUts-0.0.3/LICENCE.txt` & `traceUts-0.0.4/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `traceUts-0.0.3/setup.py` & `traceUts-0.0.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='traceUts',
-  version='0.0.3',
+  version='0.0.4',
   description='Trace Functions package',
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type='text/markdown',
   url='',  
   author='Melque Lima',
   author_email='melque_ex@yahoo.com.br',
   license='MIT',
```

### Comparing `traceUts-0.0.3/traceUts/__init__.py` & `traceUts-0.0.4/traceUts/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -148,16 +148,16 @@
     def decorator(function):
         @wraps(function)
         def wrapper(*args, **kwargs):
             try:
                 rsp = Trace()
                 funcName = function.__name__
                 data = {"func_name":funcName,"status":"SUCCESS","message":"START","time":0}
-                if CallBack:CallBack(data)
                 start = time.time()
+                if CallBack:CallBack(data)
                 ret = function(*args, **kwargs)
                 end = time.time()
                 
                 if isinstance(ret,Trace):
                     if ret:
                         data = {"func_name":funcName,"status":"SUCCESS","message":"FINISH","time":end - start}
                         if CallBack:CallBack(data)
```

