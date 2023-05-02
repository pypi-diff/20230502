# Comparing `tmp/pyp8s-3.0.0-py3-none-any.whl.zip` & `tmp/pyp8s-3.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 19059 bytes, number of entries: 10
--rw-r--r--  2.0 unx      298 b- defN 23-Feb-11 05:23 pyp8s/__init__.py
--rw-r--r--  2.0 unx      250 b- defN 23-Feb-11 05:23 pyp8s/_version.py
--rw-r--r--  2.0 unx    11600 b- defN 23-Feb-11 05:23 pyp8s/metrics.py
--rw-r--r--  2.0 unx      226 b- defN 23-Feb-11 05:23 tests/__init__.py
--rw-r--r--  2.0 unx     1300 b- defN 23-Feb-11 05:23 tests/test_import.py
--rw-r--r--  2.0 unx    35149 b- defN 23-Feb-11 05:24 pyp8s-3.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2462 b- defN 23-Feb-11 05:24 pyp8s-3.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-11 05:24 pyp8s-3.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Feb-11 05:24 pyp8s-3.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      747 b- defN 23-Feb-11 05:24 pyp8s-3.0.0.dist-info/RECORD
-10 files, 52136 bytes uncompressed, 17805 bytes compressed:  65.8%
+Zip file size: 19182 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      298 b- defN 23-May-02 00:01 pyp8s/__init__.py
+-rw-r--r--  2.0 unx      250 b- defN 23-May-02 00:01 pyp8s/_version.py
+-rw-r--r--  2.0 unx    12339 b- defN 23-May-02 00:01 pyp8s/metrics.py
+-rw-r--r--  2.0 unx      226 b- defN 23-May-02 00:01 tests/__init__.py
+-rw-r--r--  2.0 unx     1300 b- defN 23-May-02 00:01 tests/test_import.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-May-02 00:01 pyp8s-3.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2462 b- defN 23-May-02 00:01 pyp8s-3.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-02 00:01 pyp8s-3.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-02 00:01 pyp8s-3.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      747 b- defN 23-May-02 00:01 pyp8s-3.1.0.dist-info/RECORD
+10 files, 52875 bytes uncompressed, 17928 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/test_import.py
 Comment: 
 
-Filename: pyp8s-3.0.0.dist-info/LICENSE
+Filename: pyp8s-3.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: pyp8s-3.0.0.dist-info/METADATA
+Filename: pyp8s-3.1.0.dist-info/METADATA
 Comment: 
 
-Filename: pyp8s-3.0.0.dist-info/WHEEL
+Filename: pyp8s-3.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: pyp8s-3.0.0.dist-info/top_level.txt
+Filename: pyp8s-3.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pyp8s-3.0.0.dist-info/RECORD
+Filename: pyp8s-3.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyp8s/_version.py

```diff
@@ -1,8 +1,8 @@
 #!/usr/bin/env python3
 # pylint: disable=line-too-long, missing-function-docstring, logging-fstring-interpolation
 # pylint: disable=too-many-locals, broad-except, too-many-arguments, raise-missing-from
 """
     pyp8s module
 """
 
-__version__ = "3.0.0"
+__version__ = "3.1.0"
```

## pyp8s/metrics.py

```diff
@@ -49,21 +49,30 @@
         if cls._instance is None:
             cls._instance = super(Singleton, cls).__call__(*args, **kwargs)
         return cls._instance
 
 
 class Metric():
 
-    def __init__(self):
-        self.metric_name = None
+    def __init__(self, metric_name=None):
+        self.metric_name = metric_name
         self.help_header = None
         self.metric_type = None
 
         self.data = {}
 
+    def __unicode__(self):
+        return f"<Metric {self.metric_name} ({self.metric_type}) with {len(self.data.keys())} labels>"
+
+    def __str__(self):
+        return f"<Metric {self.metric_name} ({self.metric_type}) with {len(self.data.keys())} labels>"
+
+    def __repr__(self):
+        return self.__str__()
+
     def __format_labels(self, **kwargs):
         return ["=".join([f"{pair[0]}", f'"{pair[1]}"']) for pair in kwargs.items()]
 
     def __craft_labelset_key(self, **kwargs):
 
         logging.debug(f"Crafting a metric key from kwargs='{kwargs}'")
 
@@ -94,20 +103,26 @@
                 "labels_formatted": self.__format_labels(**kwargs)
             }
 
             logging.debug(f"New metric initialised: '{self.data[labelset_key]}'")
 
         return self.data[labelset_key]
 
+    def set_name(self, metric_name):
+        self.metric_name = metric_name
+
     def set_type(self, metric_type):
         self.metric_type = metric_type
 
     def set_help(self, help_header):
         self.help_header = help_header
 
+    def get_name(self):
+        return self.metric_name
+
     def get_type(self):
         return self.metric_type
 
     def get_help(self):
         return self.help_header
 
     def get_labelsets(self):
@@ -197,19 +212,25 @@
     @staticmethod
     def get_metrics():
         self = MetricsHandler()
         logging.debug("Returning metrics")
         return self.metrics
 
     @staticmethod
+    def get_metric(metric_name):
+        self = MetricsHandler()
+        logging.debug(f"Returning metric {metric_name}")
+        return self.metrics[metric_name]
+
+    @staticmethod
     def __get_metric_obj(metric_name):
         self = MetricsHandler()
 
         if metric_name not in self.metrics:
-            self.metrics[metric_name] = Metric()
+            self.metrics[metric_name] = Metric(metric_name=metric_name)
 
         return self.metrics[metric_name]
 
     @staticmethod
     def inc(metric_name, increment, *args, **kwargs):
         """Increments metric by given number
 
@@ -344,11 +365,13 @@
         "from": "Glasgow",
         "if": "fi",
     }
 
     MetricsHandler.set("busy", 200, **small_hack)
     MetricsHandler.set("busy", 4, **{"for": "the", "gods": "sake", "please": "stop"})
 
+    logging.info(f"Metrics: {MetricsHandler.get_metrics()}")
+
     MetricsHandler.serve(listen_address="127.0.0.1", listen_port=9000)
     logging.debug("Waiting before shutdown")
     time.sleep(20)
     MetricsHandler.shutdown()
```

## Comparing `pyp8s-3.0.0.dist-info/LICENSE` & `pyp8s-3.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyp8s-3.0.0.dist-info/METADATA` & `pyp8s-3.1.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyp8s
-Version: 3.0.0
+Version: 3.1.0
 Summary: Customisable prometheus exporter for your python application
 Home-page: https://github.com/pyp8s/pyp8s
 Author: Pavel Kim
 Author-email: hello@pavelkim.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

