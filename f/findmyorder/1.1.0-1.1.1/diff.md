# Comparing `tmp/findmyorder-1.1.0.tar.gz` & `tmp/findmyorder-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.1.0.tar", max compression
+gzip compressed data, was "findmyorder-1.1.1.tar", max compression
```

## Comparing `findmyorder-1.1.0.tar` & `findmyorder-1.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-05-02 06:09:52.837325 findmyorder-1.1.0/LICENSE
--rw-r--r--   0        0        0     1925 2023-05-02 06:09:52.837325 findmyorder-1.1.0/README.md
--rw-r--r--   0        0        0      113 2023-05-02 06:09:53.569324 findmyorder-1.1.0/findmyorder/__init__.py
--rw-r--r--   0        0        0      392 2023-05-02 06:09:52.837325 findmyorder-1.1.0/findmyorder/config.py
--rw-r--r--   0        0        0      312 2023-05-02 06:09:52.837325 findmyorder-1.1.0/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     3818 2023-05-02 06:09:52.837325 findmyorder-1.1.0/findmyorder/main.py
--rw-r--r--   0        0        0     1223 2023-05-02 06:09:53.569324 findmyorder-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2745 1970-01-01 00:00:00.000000 findmyorder-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-02 08:18:12.266852 findmyorder-1.1.1/LICENSE
+-rw-r--r--   0        0        0     1925 2023-05-02 08:18:12.266852 findmyorder-1.1.1/README.md
+-rw-r--r--   0        0        0      113 2023-05-02 08:18:13.282859 findmyorder-1.1.1/findmyorder/__init__.py
+-rw-r--r--   0        0        0      392 2023-05-02 08:18:12.266852 findmyorder-1.1.1/findmyorder/config.py
+-rw-r--r--   0        0        0      312 2023-05-02 08:18:12.266852 findmyorder-1.1.1/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     3851 2023-05-02 08:18:12.266852 findmyorder-1.1.1/findmyorder/main.py
+-rw-r--r--   0        0        0     1223 2023-05-02 08:18:13.282859 findmyorder-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2745 1970-01-01 00:00:00.000000 findmyorder-1.1.1/PKG-INFO
```

### Comparing `findmyorder-1.1.0/LICENSE` & `findmyorder-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.1.0/README.md` & `findmyorder-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `findmyorder-1.1.0/findmyorder/main.py` & `findmyorder-1.1.1/findmyorder/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,24 +50,24 @@
             stop_loss = Combine(
                     Suppress(settings.stop_loss_identifier) + Word(nums)
                 ).set_results_name("stop_loss")
             take_profit = Combine(
                 Suppress(settings.take_profit_identifier) + Word(nums)
                 ).set_results_name("take_profit")
             quantity = Combine(
-                Suppress(settings.quantity_identifier) + Word(nums)
+                Suppress(settings.quantity_identifier) + Word(nums) + Optional(Suppress("%"))
                 ).set_results_name("quantity")
             order_type = one_of(
                 settings.order_type_identifier, caseless=True
                 ).set_results_name("order_type")
             leverage_type = one_of(
                 settings.leverage_type_identifier, caseless=True
                 ).set_results_name("leverage_type")
-            comment = one_of(
-                settings.comment_identifier, caseless=True
+            comment = Combine(
+            Suppress(settings.comment_identifier) + Word(alphas)
                 ).set_results_name("comment")
 
             order_grammar = (
                 action("action")
                 + Optional(instrument,default=None)
                 + Optional(stop_loss,default=1000)
                 + Optional(take_profit,default=1000)
```

### Comparing `findmyorder-1.1.0/pyproject.toml` & `findmyorder-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findmyorder"
-version = "1.1.0"
+version = "1.1.1"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
```

### Comparing `findmyorder-1.1.0/PKG-INFO` & `findmyorder-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.1.0
+Version: 1.1.1
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

