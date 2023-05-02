# Comparing `tmp/buildington-1.5.2.tar.gz` & `tmp/buildington-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildington-1.5.2.tar", last modified: Fri Apr 28 09:21:27 2023, max compression
+gzip compressed data, was "buildington-1.6.tar", last modified: Tue May  2 16:45:15 2023, max compression
```

## Comparing `buildington-1.5.2.tar` & `buildington-1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 09:21:27.445551 buildington-1.5.2/
--rw-rw-rw-   0        0        0     2259 2023-04-28 09:21:27.442552 buildington-1.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     1733 2023-04-23 10:51:50.000000 buildington-1.5.2/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-28 09:21:27.396550 buildington-1.5.2/buildington/
--rw-rw-rw-   0        0        0     4549 2023-04-28 09:19:41.000000 buildington-1.5.2/buildington/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 09:21:27.436549 buildington-1.5.2/buildington.egg-info/
--rw-rw-rw-   0        0        0     2259 2023-04-28 09:21:27.000000 buildington-1.5.2/buildington.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-04-28 09:21:27.000000 buildington-1.5.2/buildington.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 09:21:27.000000 buildington-1.5.2/buildington.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-28 09:21:27.000000 buildington-1.5.2/buildington.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-28 09:21:27.000000 buildington-1.5.2/buildington.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-28 09:21:27.448547 buildington-1.5.2/setup.cfg
--rw-rw-rw-   0        0        0      650 2023-04-28 09:20:12.000000 buildington-1.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 16:45:15.124433 buildington-1.6/
+-rw-rw-rw-   0        0        0     2257 2023-05-02 16:45:15.119351 buildington-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1733 2023-04-23 10:51:50.000000 buildington-1.6/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 16:45:15.069302 buildington-1.6/buildington/
+-rw-rw-rw-   0        0        0     4422 2023-05-02 16:44:28.000000 buildington-1.6/buildington/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 16:45:15.119351 buildington-1.6/buildington.egg-info/
+-rw-rw-rw-   0        0        0     2257 2023-05-02 16:45:14.000000 buildington-1.6/buildington.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-05-02 16:45:14.000000 buildington-1.6/buildington.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 16:45:14.000000 buildington-1.6/buildington.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-02 16:45:14.000000 buildington-1.6/buildington.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-02 16:45:14.000000 buildington-1.6/buildington.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 16:45:15.124433 buildington-1.6/setup.cfg
+-rw-rw-rw-   0        0        0      648 2023-05-02 16:44:40.000000 buildington-1.6/setup.py
```

### Comparing `buildington-1.5.2/PKG-INFO` & `buildington-1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildington
-Version: 1.5.2
+Version: 1.6
 Summary: Building websites like React, and hosting 'em like Flask!
 Author: RixTheTyrunt
 Author-email: rixthetyrunt@gmail.com
 Classifier: Environment :: Console
 Classifier: Framework :: Flask
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
```

### Comparing `buildington-1.5.2/README.txt` & `buildington-1.6/README.txt`

 * *Files identical despite different names*

### Comparing `buildington-1.5.2/buildington/__init__.py` & `buildington-1.6/buildington/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,25 +19,21 @@
 
 	def __str__(self):
 		def escapeHTML(txt):
 			res = ""
 			for char in txt:
 				res += "&#" + str(ord(char)) + ";"
 			return res
+        
 		return "<" + self.html + ">" + escapeHTML(self.innerHTML) + "</" + self.html + ">"
 
 class Header(Para):
 	def __init__(self, innerHTML, props=None):
-		self.innerHTML = innerHTML
-		self.props = props
-		if not isinstance(self.props, dict):
-			self.props = {}
-		elif type(self.props) != dict:
-			self.props = dict(self.props)
-		self.html = "h" + str(self.props["size"])
+		super().__init__(innerHTML, props)
+		self.html = "h" + str(int(self.props["size"]))
 
 def page(route, opts=None):
 	if opts is None:
 		opts = {}
 	opts = dict(opts)
 	if "met" not in opts:
 		opts["met"] = ALLMETS
```

### Comparing `buildington-1.5.2/buildington.egg-info/PKG-INFO` & `buildington-1.6/buildington.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildington
-Version: 1.5.2
+Version: 1.6
 Summary: Building websites like React, and hosting 'em like Flask!
 Author: RixTheTyrunt
 Author-email: rixthetyrunt@gmail.com
 Classifier: Environment :: Console
 Classifier: Framework :: Flask
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
```

### Comparing `buildington-1.5.2/setup.py` & `buildington-1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
 	name="buildington",
-	version="1.5.2",
+	version="1.6",
 	author="RixTheTyrunt",
 	author_email="rixthetyrunt@gmail.com",
 	description="Building websites like React, and hosting 'em like Flask!",
 	packages=["buildington"],
 	classifiers=[
 		"Environment :: Console",
 		"Framework :: Flask",
```

